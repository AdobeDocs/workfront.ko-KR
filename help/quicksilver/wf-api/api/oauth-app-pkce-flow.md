---
content-type: api
navigation-topic: api-navigation-topic
title: OAuth 2 애플리케이션에 PKCE 플로우 사용
description: OAuth 2 애플리케이션에 PKCE 플로우 사용
author: Becky
feature: Workfront API
role: Developer
exl-id: 61fe77b6-c6d7-4f23-bfb6-617bccaa1989
source-git-commit: cd0214917620e0b147d0da3402ea2d34e28bc9c3
workflow-type: tm+mt
source-wordcount: '811'
ht-degree: 0%

---

# PKCE 플로우를 사용하여 조직의 사용자 정의 OAuth 2 애플리케이션 구성 및 사용

PKCE는 모바일 앱과 같이 동적으로 새로 고치는 애플리케이션에서 잘 작동하는 보안 인증 흐름이지만 모든 OAuth2 클라이언트에서 매우 중요합니다. PKCE에서는 정적 클라이언트 암호 대신 동적으로 생성된 문자열을 사용하므로 클라이언트 암호가 유출될 위험이 없습니다.

## PKCE 개요

PKCE 흐름에는 다음과 같은 단계가 있습니다. 이 섹션의 단계는 정보용으로만 제공됩니다. 이러한 절차를 수행하려면 이 문서의 다른 섹션을 참조하십시오.

1. 클라이언트가 `code_challenge` 암호화를 사용하여 `code_verifier`을(를) 변환하여 `S256`을(를) 만듭니다.

1. 클라이언트가 생성된 `code_challenge`과(와) 함께 브라우저를 OAuth2 로그인 페이지로 보냅니다. OAuth2가 인증 요청을 수락할 수 있도록 앱(클라이언트)을 등록해야 합니다. 등록 후 앱에서 브라우저를 OAuth2로 리디렉션할 수 있습니다.

1. OAuth2 인증 서버는 인증 프롬프트를 사용자에게 리디렉션합니다.

1. 사용자는 구성된 로그인 옵션 중 하나를 사용하여 인증하며, OAuth2가 애플리케이션에 부여할 권한을 나열하는 동의 페이지를 볼 수 있습니다.

1. OAuth2가 `authorization code`을(를) 사용하여 응용 프로그램으로 다시 리디렉션합니다.

1. 응용 프로그램에서 이 코드를 `code_verifier`과(와) 함께 OAuth2로 보냅니다.

1. OAuth2 인증 서버는 초기 인증 요청에서 `code_verifier`을(를) 사용하여 `code_challenge_method`을(를) 변환하고 `code_challenge`에 대해 결과를 확인합니다. 두 문자열의 값이 일치하면 서버에서 요청이 동일한 클라이언트에서 온 것을 확인하고 `access token`을(를) 발행합니다.

1. OAuth2는 `access token`을(를) 반환하고 선택적으로 `refresh token`을(를) 반환합니다.

1. 이제 애플리케이션은 이러한 토큰을 사용하여 사용자를 대신하여 API와 같은 리소스 서버를 호출할 수 있습니다.

1. 리소스 서버는 요청에 응답하기 전에 토큰을 확인합니다.


## 애플리케이션 구성

인증을 구현하려면 먼저 Workfront에서 앱 통합을 만들어 OAuth2에 앱을 등록해야 합니다.

OAuth2 응용 프로그램을 만드는 방법에 대한 지침은 [Workfront 통합을 위한 OAuth2 응용 프로그램 만들기](../../administration-and-setup/configure-integrations/create-oauth-application.md#create-an-oauth2-single-page-web-application-using-pkce)에서 [PKCE를 사용하여 OAuth2 단일 페이지 웹 응용 프로그램 만들기](../../administration-and-setup/configure-integrations/create-oauth-application.md)를 참조하십시오.

>[!NOTE]
>
>한 번에 최대 10개의 OAuth2 애플리케이션을 보유할 수 있습니다.


## 코드 교환을 위한 증명 키 만들기

표준 인증 코드 흐름과 마찬가지로 사용자의 브라우저를 인증 서버의 `/authorize` 끝점으로 리디렉션하여 앱을 시작합니다. 그러나 이 경우 코드 챌린지도 전달해야 합니다.

첫 번째 단계는 코드 검증기 및 챌린지를 생성하는 것입니다.

<table>
  <col/>
  <col/>
    <tbody>
      <tr>
        <td role="rowheader">코드 검증기</td>
        <td>
          <p>최소 길이가 43자인 임의의 URL 안전 문자열</p>
        </td>
      </tr>
      <tr>
        <td role="rowheader">코드 챌린지</td>
        <td>
          <p>코드 검증자의 Base64 URL 인코딩 SHA-256 해시</p>
        </td>
      </tr>
    </tbody>
</table>


코드 검증자와 코드 챌린지를 만들려면 클라이언트 앱에 코드를 추가해야 합니다.

PKCE 생성기 코드는 다음과 유사한 출력을 생성합니다.

>[!INFO]
>
>**예:**
>
>```
>{
>  "code\_verifier":"N28zVMsKU6ptUjHaYWg3T1NFTDQqcW1R4BU5NXywapNac4hhfkxjwfhZQat",
>  "code\_challenge":"wzgjYF9qEiWep-CwqgrTE78-2ghjwCtRO3vj23o4W\_fw"
>}
>```

앱에서 나중에 `code_verifier`을(를) 저장하고 인증 요청과 함께 `code_challenge`을(를) 인증 서버의 `/authorize` URL로 보냅니다.

## 인증 코드 요청

기본 사용자 지정 인증 서버를 사용하는 경우 요청 URL은 다음과 비슷합니다.

>[!INFO]
>
>**예:**
>
>
>```
>/authorize?client\_id=<clientID>&response\_type=code&redirect\_uri=<redirectURL>
>&code\_challenge\_method=S256&code\_challenge=wzgjYF9qEiWep-CwqgrTE78-2ghjwCtRO3vj23o4W\_fw"
>```

전달되는 매개 변수를 주목하십시오.

* `client_id`은(는) 응용 프로그램을 구성할 때에서 만든 OAuth2 응용 프로그램의 클라이언트 ID와 일치합니다.

  지침은 Workfront 통합을 위한 OAuth2 애플리케이션 만들기에서 PKCE를 사용하여 OAuth2 단일 페이지 웹 애플리케이션 만들기 를 참조하십시오.

* 응용 프로그램에서 인증 코드 부여 형식을 사용하므로 `response_type`은(는) `code`입니다.
* `redirect_uri`은(는) 사용자 에이전트가 `code`과(와) 함께 보내는 콜백 위치입니다. OAuth2 애플리케이션을 만들 때 지정한 리디렉션 URL 중 하나와 일치해야 합니다.
* `code_challenge_method`은(는) 챌린지를 생성하는 데 사용되는 해시 메서드입니다. PKCE를 사용하는 Workfront Oauth2 응용 프로그램에는 항상 `S256`입니다.
* `code_challenge`은(는) PKCE에 사용되는 코드 챌린지입니다.


## 토큰을 위한 코드 교환

인증 코드를 액세스 토큰으로 교환하려면 인증 서버의 `/token` 끝점에 `code_verifier`과(와) 함께 전달합니다.

>[!INFO]
>
>**예:**
>
>```
>/token \\
>  --header 'accept: application/json' \\
>  --header 'cache-control: no-cache' \\
>  --header 'content-type: application/x-www-form-urlencoded' \\
>  --data 'grant\_type=authorization\_code&client\_id=<clientID>&redirect\_uri=<redirectURL>&code=<code>&code\_verifier=N28zVMsKU6ptUjHaYWg3T1NFTDQqcW1R4BU5NXywapNac4hhfkxjwfhZQat
>```

>[!IMPORTANT]
>
> 일반 인증 코드 흐름과 달리 이 호출에는 클라이언트 ID 및 암호가 포함된 인증 헤더가 필요하지 않습니다. 이 버전의 인증 코드 흐름은 모바일 애플리케이션이나 백엔드가 없는 단일 페이지 애플리케이션과 같은 기본 앱에 적합합니다.

전달되는 매개 변수를 주목하십시오.

* 앱에서 인증 코드 부여 형식을 사용하므로 `grant_type`은(는) `authorization_code`입니다.

* `redirect_uri`은(는) 인증 코드를 가져오는 데 사용된 URI와 일치해야 합니다.

* `code`은(는) /authorize 끝점에서 받은 인증 코드입니다.

* `code_verifier`은(는) 앱이 [코드 교환용 증명 키 만들기](#Create)에서 생성한 PKCE 코드 검증자입니다.

* `client_id`은(는) 클라이언트를 식별하며 OAuth2에 사전 등록된 값과 일치해야 합니다.


코드가 여전히 유효하고 코드 검증자가 일치하는 경우 응용 프로그램에서 액세스 토큰을 받습니다.

>[!INFO]
>
>**예:**
>
>```
>{
>    "access\_token": "eyJhd\[...\]Yozv",
>    "expires\_in": 3600,
>    "token\_type": "Bearer"
>}
>```

## 액세스 토큰 유효성 검사

애플리케이션이 액세스 토큰을 사용하여 요청을 전달하면 리소스 서버에서 유효성을 검사해야 합니다.

다음과 유사한 API 호출을 사용하여 액세스 토큰의 유효성을 검사할 수 있습니다.

>[!INFO]
>
>**예:**
>
>```
>/attask/api/<api version>/proj/search \\
>  --header 'sessionID: <access\_token>' \\
>```

## 새로 고침 토큰 요청

새로 고침 토큰을 요청하기 위해 다음과 같이 API에 대한 POST 호출을 수행할 수 있습니다.

>[!INFO]
>
>**예:**
>
>```
>/token \\
>  --header 'accept: application/json' \\
>  --header 'cache-control: no-cache' \\
>  --header 'content-type: application/x-www-form-urlencoded' \\
>  --data 'grant\_type=refresh\_token&client\_id=<clientID>&redirect\_uri=<redirectURL>&refresh\_token=<refresh\_token>
>```
