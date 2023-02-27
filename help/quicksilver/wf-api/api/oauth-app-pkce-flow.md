---
content-type: api
navigation-topic: api-navigation-topic
title: OAuth 2 응용 프로그램에 PKCE 흐름 사용
description: OAuth 2 응용 프로그램에 PKCE 흐름 사용
author: Becky
feature: Workfront API
exl-id: 61fe77b6-c6d7-4f23-bfb6-617bccaa1989
source-git-commit: f050c8b95145552c9ed67b549608c16115000606
workflow-type: tm+mt
source-wordcount: '792'
ht-degree: 0%

---

# PKCE 플로우를 사용하여 조직의 사용자 지정 OAuth 2 응용 프로그램 구성 및 사용

PKCE는 모바일 앱과 같은 응용 프로그램을 동적으로 새로 고치는 데 잘 작동하지만 모든 OAuth2 클라이언트에서 중요합니다. PKCE는 정적 클라이언트 암호 대신 동적으로 생성된 문자열을 사용하여 유출된 클라이언트 비밀의 위험을 제거합니다.

## PKCE 개요

PKCE 플로우에는 다음 단계가 있습니다. 이 섹션의 단계는 정보에 대해서만 제공됩니다. 이러한 절차를 수행하려면 이 문서의 다른 섹션을 참조하십시오.

1. 클라이언트가 `code_challenge` 변환 `code_verifier` 사용 `S256` 암호화.

1. 클라이언트는 생성된 와 함께 브라우저를 OAuth2 로그인 페이지로 보냅니다 `code_challenge`. OAuth2가 인증 요청을 수락할 수 있도록 앱(클라이언트)을 등록해야 합니다. 등록 후 앱은 브라우저를 OAuth2로 리디렉션할 수 있습니다.

1. OAuth2 인증 서버는 인증 프롬프트를 사용자에게 리디렉션합니다.

1. 사용자는 구성된 로그인 옵션 중 하나를 사용하여 인증되며, OAuth2 권한이 애플리케이션에 제공되는 동의 페이지를 볼 수 있습니다.

1. OAuth2는 를 사용하여 다시 응용 프로그램으로 리디렉션합니다. `authorization code`.

1. 애플리케이션이 와 함께 이 코드를 전송합니다 `code_verifier`를 OAuth2로 전송하는 중입니다.

1. OAuth2 인증 서버가 `code_verifier` 사용 `code_challenge_method` 초기 인증 요청에서 결과를 확인하고 `code_challenge`. 두 문자열의 값이 일치하는 경우 서버는 요청이 동일한 클라이언트에서 전달되었음을 확인하고 `access token`.

1. OAuth2는 `access token`, 및 선택적으로 `refresh token`.

1. 이제 애플리케이션에서 이러한 토큰을 사용하여 사용자를 대신하여 API와 같은 리소스 서버를 호출할 수 있습니다.

1. 리소스 서버는 요청에 응답하기 전에 토큰의 유효성을 검사합니다.


## 애플리케이션 구성

인증을 구현하려면 먼저 Workfront에서 앱 통합을 만들어 OAuth2에 앱을 등록해야 합니다.

OAuth2 애플리케이션 만들기에 대한 지침은 [PKCE를 사용하여 OAuth2 단일 페이지 웹 응용 프로그램 만들기 ](../../administration-and-setup/configure-integrations/create-oauth-application.md#create-an-oauth2-single-page-web-application-using-pkce) in [Workfront 통합을 위한 OAuth2 애플리케이션 만들기](../../administration-and-setup/configure-integrations/create-oauth-application.md)


## 코드 교환용 증명 키 만들기

표준 인증 코드 흐름과 유사하게, 앱은 사용자의 브라우저를 인증 서버의 브라우저로 리디렉션하여 시작합니다 `/authorize` 엔드포인트. 그러나 이 경우 코드 문제를 통과해야 합니다.

첫 번째 단계는 코드 확인 프로그램과 과제를 생성하는 것입니다.

<table>
  <col/>
  <col/>
    <tbody>
      <tr>
        <td role="rowheader">코드 확인 프로그램</td>
        <td>
          <p>최소 길이가 43자인 임의의 URL 안전 문자열</p>
        </td>
      </tr>
      <tr>
        <td role="rowheader">코드 문제</td>
        <td>
          <p>코드 확인기의 Base64 URL로 인코딩된 SHA-256 해시</p>
        </td>
      </tr>
    </tbody>
</table>


코드 확인 및 코드 문제를 만들려면 클라이언트 앱에 코드를 추가해야 합니다.

PKCE 생성기 코드는 다음과 유사한 출력을 생성합니다.

>[!INFO]
>
>**예:**
>
>
```
>{
>
>
  "code\_verifier":"N28zVMsKU6ptUjHaYWg3T1NFTDQqcW1R4BU5NXywapNac4hhfkxjwfhZQat",
>
>
  "code\_challenge":"wzgjYF9qEiWep-CwqgrTE78-2ghjwCtRO3vj23o4W\_fw"
>
>
}
>```

앱에서 를 저장합니다. `code_verifier` 나중에 및에서 `code_challenge` 인증 서버의 인증 요청과 함께 `/authorize` URL.

## 인증 코드 요청

기본 사용자 지정 인증 서버를 사용하는 경우 요청 URL은 다음과 비슷합니다.

>[!INFO]
>
>**예:**
>
>
>
```
>/authorize?client\_id=<clientID>&response\_type=code&redirect\_uri=<redirectURL>
>
>
&code\_challenge\_method=S256&code\_challenge=wzgjYF9qEiWep-CwqgrTE78-2ghjwCtRO3vj23o4W\_fw"
>```

전달되는 매개 변수를 확인합니다.

* `client_id` 는 애플리케이션을 구성할 때에서 만든 OAuth2 애플리케이션의 클라이언트 ID와 일치합니다.

   지침은 Workfront 통합을 위한 OAuth2 애플리케이션 만들기에서 PKCE를 사용하여 OAuth2 단일 페이지 웹 애플리케이션 만들기 를 참조하십시오.

* `response_type` is `code`는 응용 프로그램에서 인증 코드 부여 유형을 사용하기 때문에 발생합니다.

* `redirect_uri` 는 사용자 에이전트가 과 함께 전달되는 콜백 위치입니다 `code`. 이 값은 OAuth2 애플리케이션을 만들 때 지정한 리디렉션 URL 중 하나와 일치해야 합니다.

* `code_challenge_method` 이 해시 메서드는 항상 문제를 생성하는 데 사용됩니다 `S256` PKCE를 사용하는 Workfront Oauth2 애플리케이션용.

* `code_challenge` 는 PKCE에 사용되는 코드 과제입니다.


## 토큰에 대한 코드 교환

액세스 토큰에 대한 인증 코드를 교환하려면 인증 서버의 `/token` 끝점과 `code_verifier`.

>[!INFO]
>
>**예:**
>
>
```
>/token \\
>
>
  --header 'accept: application/json' \\
>
>
  --header 'cache-control: no-cache' \\
>
>
  --header 'content-type: application/x-www-form-urlencoded' \\
>
>
  --data 'grant\_type=authorization\_code&client\_id=<clientID>&redirect\_uri=<redirectURL>&code=<code>&code\_verifier=N28zVMsKU6ptUjHaYWg3T1NFTDQqcW1R4BU5NXywapNac4hhfkxjwfhZQat
>```

>[!IMPORTANT]
>
> 일반 인증 코드 흐름과 달리, 이 호출에는 클라이언트 ID와 암호가 있는 인증 헤더가 필요하지 않습니다. 따라서 이 버전의 인증 코드 흐름은 백엔드가 없는 모바일 애플리케이션이나 단일 페이지 애플리케이션과 같은 기본 앱에 적합합니다.

전달되는 매개 변수를 확인합니다.

* `grant_type` is `authorization_code`: 앱이 인증 코드 부여 유형을 사용하므로.

* `redirect_uri` 는 인증 코드를 가져오는 데 사용된 URI와 일치해야 합니다.

* `code` 은 /authorization 끝점에서 받은 인증 코드입니다.

* `code_verifier` 는 앱이 [코드 교환용 증명 키 만들기](#Create).

* `client_id` 클라이언트를 식별하고 OAuth2에 사전 등록된 값과 일치해야 합니다.


코드가 여전히 유효하고 코드 확인자가 일치하는 경우 애플리케이션이 액세스 토큰을 받습니다.

>[!INFO]
>
>**예:**
>
>
```
>{
>
>
    "access\_token": "eyJhd\[...\]Yozv",
>
>
    "expires\_in": 3600,
>
>
    "token\_type": "Bearer"
>
>
}
>```

## 액세스 토큰 유효성 검사

애플리케이션이 액세스 토큰을 사용하여 요청을 전달하면 리소스 서버가 이 요청을 확인해야 합니다.

다음과 유사한 API 호출을 사용하여 액세스 토큰의 유효성을 검사할 수 있습니다.

>[!INFO]
>
>**예:**
>
>
```
>/attask/api/<api version>/proj/search \\
>
>
  --header 'sessionID: <access\_token>' \\
>```

## 새로 고침 토큰 요청

새로 고침 토큰을 요청하기 위해 다음과 같이 API에 POST 호출을 수행할 수 있습니다.

>[!INFO]
>
>**예:**
>
>
```
>/token \\
>
>
  --header 'accept: application/json' \\
>
>
  --header 'cache-control: no-cache' \\
>
>
  --header 'content-type: application/x-www-form-urlencoded' \\
>
>
  --data 'grant\_type=refresh\_token&client\_id=<clientID>&redirect\_uri=<redirectURL>&refresh\_token=<refresh\_token>
>```
