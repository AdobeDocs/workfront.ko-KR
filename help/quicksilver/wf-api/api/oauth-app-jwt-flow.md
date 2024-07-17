---
content-type: api
navigation-topic: api-navigation-topic
title: 사용자 정의 OAuth 2 애플리케이션에 JWT 플로우 사용
description: 사용자 정의 OAuth 2 애플리케이션에 JWT 플로우 사용
author: Becky
feature: Workfront API
role: Developer
exl-id: 4bd56fe6-1f36-4c36-82cd-96de748ad680
source-git-commit: 6f041459caf040846ffdec5bc75e9d74c99e318b
workflow-type: tm+mt
source-wordcount: '497'
ht-degree: 0%

---

# JWT 플로우를 사용하여 조직의 사용자 지정 OAuth 2 애플리케이션 구성 및 사용

Workfront과 통합하고 클라이언트 앱이 사용자를 대신하여 Workfront과 통신할 수 있도록 하려면 다음을 수행해야 합니다.

* OAuth2 애플리케이션 만들기
* 공개 키 인증서 만들기
* JSON 웹 토큰(JWT) 생성

## OAuth2 애플리케이션 만들기

OAuth2 애플리케이션 만들기에 대한 지침은 [Workfront 통합을 위한 OAuth2 애플리케이션 만들기](../../administration-and-setup/configure-integrations/create-oauth-application.md)에서 [서버 인증을 사용하여 OAuth2 애플리케이션 만들기(JWT 흐름)](../../administration-and-setup/configure-integrations/create-oauth-application.md#create2)를 참조하십시오.

>[!NOTE]
>
>한 번에 최대 10개의 OAuth2 애플리케이션을 보유할 수 있습니다.

## 공개 키 인증서 만들기

액세스 요청에 포함하려면 JWT에 서명이 있고 base-64로 인코딩되어야 합니다. JWT 라이브러리는 이러한 작업을 수행하는 기능을 제공합니다.

디지털 서명 인증서에 대한 개인 키를 사용하여 토큰에 서명해야 합니다. 이렇게 하면 연결된 인증서의 개인 키를 사용하여 JWT에 서명할 수 있습니다.

사용된 알고리즘은 RS256(SHA-256을 사용한 RSA 서명)입니다. 이 알고리즘은 비대칭 알고리즘이며 공개/개인 키 쌍을 사용합니다. ID 공급자는 서명을 생성하는 데 사용되는 개인(비밀) 키를 가지며 JWT의 소비자는 서명의 유효성을 검사하는 공개 키를 받습니다.

공개 키를 생성하려면 다음 중 **하나**&#x200B;를 실행하십시오.

* macOS/Linux 터미널을 열고 다음 명령을 실행한 다음 Workfront의 OAuth2 애플리케이션 설정에서 **공개 키 추가** 단추를 사용하여 `certificate_pub.crt`을(를) 업로드합니다.

  <!-- [Copy](javascript:void(0);) -->
  <pre><code>openssl req -x509 -sha256 -nodes -newkey rsa:2048 -keyout private.key -out certificate_pub.crt</code></pre>

* Workfront의 OAuth2 애플리케이션 설정에서 **공개/비공개 키 쌍 생성** 버튼을 사용하여 RSA를 생성합니다.

## JSON 웹 토큰 만들기

서비스 계정 인증을 위한 JSON 웹 토큰에는 특정 클레임 집합이 필요하며 유효한 디지털 서명 인증서를 사용하여 서명해야 합니다. JWT를 작성하는 데 공개적으로 사용 가능한 라이브러리 또는 도구 중 하나를 사용하는 것이 좋습니다.

다음 표에는 JWT 토큰을 구성할 때 필요할 수 있는 필드에 대한 정보가 나와 있습니다.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">만료</td> 
   <td> <p>필수. 만료 매개 변수는 01/01/1970 GMT 이후의 절대 시간을 측정하는 필수 매개 변수입니다. 만료 시간이 문제 시간 이후인지 확인해야 합니다. 이 시간이 지나면 JWT는 더 이상 유효하지 않습니다. </p> <p>참고: 매우 짧은 수명 토큰(몇 분)이 있으므로 액세스 토큰으로 교환된 직후 만료되도록 하는 것이 좋습니다. 새로운 액세스 토큰이 필요할 때마다 하나의 JWT에 서명하고 교환합니다. 이는 보다 안전한 접근 방식입니다. 필요에 따라 액세스 토큰을 얻기 위해 다시 사용되는 장기 토큰은 사용하지 않는 것이 좋습니다.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">iss</td> 
   <td>필수. 발급자는 OAuth2 앱 세부 사항에서 고객 ID입니다.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">하위</td> 
   <td>필수. 제목은 설정에서 공개 키를 만든 사용자 ID입니다.</td> 
  </tr> 
 </tbody> 
</table>

## JWT를 교환하여 액세스 토큰 검색

1. POST 요청을 다음으로 보내기:

   <!-- [Copy](javascript:void(0);) -->
   <pre><code>https://yourdomain.my.workfront.com/integrations/oauth2/api/v1/jwt/exchange</code></pre>

1. 요청 본문에는 클라이언트 ID, 클라이언트 암호 및 JWT가 있는 URL로 인코딩된 매개 변수가 포함되어야 합니다.

   <!-- [Copy](javascript:void(0);) -->
   <pre><code>client_id={client_id_value}&client_secret={client_secret_value}&jwt_token={base64_encoded_JWT}</code></pre>

 
