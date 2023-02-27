---
content-type: api
navigation-topic: api-navigation-topic
title: 사용자 지정 OAuth 2 애플리케이션에 JWT 흐름 사용
description: 사용자 지정 OAuth 2 애플리케이션에 JWT 흐름 사용
author: Becky
feature: Workfront API
exl-id: 4bd56fe6-1f36-4c36-82cd-96de748ad680
source-git-commit: f050c8b95145552c9ed67b549608c16115000606
workflow-type: tm+mt
source-wordcount: '477'
ht-degree: 0%

---

# JWT 흐름을 사용하여 조직의 사용자 지정 OAuth 2 애플리케이션을 구성하고 사용합니다

Workfront과 통합하고 클라이언트 앱이 사용자를 대신하여 Workfront과 통신할 수 있도록 하려면 다음을 수행해야 합니다.

* OAuth2 애플리케이션 만들기
* 공개 키 인증서 만들기
* JSON 웹 토큰(JWT) 만들기

## OAuth2 애플리케이션 만들기

OAuth2 애플리케이션 만들기에 대한 지침은 [서버 인증(JWT 흐름)을 사용하여 OAuth2 응용 프로그램을 만듭니다](../../administration-and-setup/configure-integrations/create-oauth-application.md#create2) in [Workfront 통합을 위한 OAuth2 애플리케이션 만들기](../../administration-and-setup/configure-integrations/create-oauth-application.md)

## 공개 키 인증서 만들기

JWT는 액세스 요청에 포함하려면 서명하고 base-64로 인코딩되어야 합니다. JWT 라이브러리는 이러한 작업을 수행하는 기능을 제공합니다.

디지털 서명 인증서에 대한 개인 키를 사용하여 토큰을 서명해야 합니다. 그럴 경우 연결된 인증서의 개인 키를 사용하여 JWT에 서명할 수 있습니다.

사용되는 알고리즘은 RS256(SHA-256의 RSA 서명)입니다. 비대칭 알고리즘이며 공개/개인 키 쌍을 사용합니다. ID 제공업체는 서명을 생성하는 데 사용되는 개인(비밀) 키를 가지고 있으며 JWT 소비자가 서명을 확인할 공개 키를 받습니다.

공개 키를 생성하려면 다음을 수행합니다. **하나** 다음을 참조하십시오.

* MacOS/Linux 터미널을 열고 다음 명령을 실행한 다음 업로드합니다 `certificate_pub.crt` 사용 **공개 키 추가** 버튼을 클릭합니다.

   <!-- [Copy](javascript:void(0);) -->
   <pre><code>openssl req -x509 -sha256 -nodes -newkey rsa:2048 -keyout private.key -out certificate_pub.crt</code></pre>

* 를 사용하십시오 **공용/개인 키 쌍 생성** 단추를 클릭하여 RSA를 생성합니다.

## JSON 웹 토큰 만들기

서비스 계정 인증용 JSON 웹 토큰은 특정 클레임 세트가 필요하며, 유효한 디지털 서명 인증서를 사용하여 서명해야 합니다. JWT를 빌드하기 위해 공개적으로 사용 가능한 라이브러리 또는 도구 중 하나를 사용하는 것이 좋습니다.

다음 표에는 JWT 토큰을 구성할 때 필요할 수 있는 필드에 대한 정보가 포함되어 있습니다.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">exp</td> 
   <td> <p>필수. 만료 매개 변수는 01/01/1970 GMT 이후 절대 시간을 측정하는 필수 매개 변수입니다. 만료 시간이 문제 발생 시간보다 늦는지 확인해야 합니다. 이 시간 이후에는 JWT가 더 이상 유효하지 않습니다. </p> <p>참고: 액세스 토큰으로 교환된 후 즉시 만료되도록 짧은 유효 토큰(몇 분)이 있는 것이 좋습니다. 새 액세스 토큰이 필요할 때마다 하나의 JWT가 서명되어 교환됩니다. 이는 보다 안전한 접근 방법입니다. 필요에 따라 액세스 토큰을 가져오는 데 다시 사용되는 더 이상 사용되지 않는 토큰을 권장합니다.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">is</td> 
   <td>필수. 발급자는 OAuth2 앱 세부 정보의 고객 ID입니다.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">하위</td> 
   <td>필수. 제목은 설정에서 공개 키를 만든 사용자 ID입니다.</td> 
  </tr> 
 </tbody> 
</table>

## JWT를 교환하여 액세스 토큰 검색

1. 다음 주소로 POST 요청을 보냅니다.

   <!-- [Copy](javascript:void(0);) -->
   <pre><code>https://yourdomain.my.workfront.com/integrations/oauth2/api/v1/jwt/exchange</code></pre>

1. 요청 본문에는 클라이언트 ID, 클라이언트 암호 및 JWT가 있는 URL로 인코딩된 매개 변수가 포함되어 있어야 합니다.

   <!-- [Copy](javascript:void(0);) -->
   <pre><code>client_id={client_id_value}&client_secret={client_secret_value}&jwt_token={base64_encoded_JWT}</code></pre>

 
