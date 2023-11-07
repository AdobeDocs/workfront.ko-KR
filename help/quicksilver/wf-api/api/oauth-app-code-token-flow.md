---
content-type: api
navigation-topic: api-navigation-topic
title: 사용자 지정 OAuth 2 애플리케이션에 대한 인증 코드 흐름
description: 사용자 지정 OAuth 2 애플리케이션에 대한 인증 코드 흐름
author: Becky
feature: Workfront API
role: Developer
exl-id: a1ab60c4-4255-4d80-87f1-f36d325254c2
source-git-commit: 3e339e2bfb26e101f0305c05f620a21541394993
workflow-type: tm+mt
source-wordcount: '690'
ht-degree: 0%

---


# 인증 코드 흐름을 사용하여 조직의 사용자 지정 OAuth 2 애플리케이션 구성 및 사용

Workfront과 통합하고 클라이언트 앱이 사용자를 대신하여 Workfront과 통신할 수 있도록 하려면 다음을 수행해야 합니다.

* OAuth2 애플리케이션 만들기
* 타사 애플리케이션 구성
* 사용자의 Authorize 페이지 링크
* 인증 코드 흐름 설정: 사용자가 Workfront 인스턴스에 로그인하고 클라이언트 애플리케이션이 자신을 대신하여 Workfront에 연결할 수 있도록 하는 데 동의합니다. 그 결과 액세스 및 새로 고침 토큰과 교환할 인증 코드를 받게 됩니다.
* 새로 고침 토큰 흐름 설정: 이 흐름에서 이전 액세스 토큰이 만료되면 새로 고침 토큰을 사용하여 새 액세스 토큰을 가져옵니다.

## OAuth2 애플리케이션 만들기

OAuth2 애플리케이션 만들기에 대한 지침은 [사용자 자격 증명을 사용하여 OAuth2 애플리케이션 만들기(인증 코드 흐름)](../../administration-and-setup/configure-integrations/create-oauth-application.md#create3) 위치: [Workfront 통합을 위한 OAuth2 애플리케이션 만들기](../../administration-and-setup/configure-integrations/create-oauth-application.md)

## 사용자의 Authorize 페이지 링크

사용자가 자신의 계정에서 이 통합을 승인하려면 로그인해야 합니다. 인증을 위한 페이지에는 여기에 설명된 특정 형식이 있습니다. 이 정보를 사용하여 앱에 대한 인증 페이지 주소를 결정하고 사용자에게 이 주소 또는 링크를 제공합니다.

* 조직 도메인의 전체 URL. 예:

  ```
  https://myorganization.my.workfront.com
  ```


* `client_id`: Workfront에서 OAuth2 앱을 만들 때 생성된 클라이언트 ID입니다.

* `redirect_uri`: 앱을 만들 때 입력한 리디렉션 URL입니다. 사용자가 계정에 대한 앱을 승인하면 이 페이지로 이동합니다.

* `response_type`: 값이 있어야 합니다. `code`.

따라서 인증 페이지의 URL은 다음과 같습니다.

```
https://<URL of your organization's domain>/integrations/oauth2/authorize?client_id=<Your ClientID>&redirect_uri=<Your redirect URL>&response_type=code
```

>[!NOTE]
>
>사용자가 이 페이지로 이동하기 위해 클릭할 수 있는 단추 또는 기타 링크를 만드는 것이 좋습니다.

## 타사 애플리케이션 구성

타사 응용 프로그램에는 구성이 필요할 수 있습니다. 다음 표에는 타사 응용 프로그램을 구성할 때 필요할 수 있는 필드에 대한 정보가 나와 있습니다.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">인증 URI</td> 
   <td> <p><code>https://&lt;the full URL of your organization's domain&gt;/integrations/oauth2/authorize</code> </p> <p class="example" data-mc-autonum="<b>Example: </b>"><span class="autonumber"><span><b>예: </b></span></span><code> https://myorganization.my.workfront.com/integrations/oauth2/authorize</code> </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">토큰 URL</td> 
   <td> <p><code>https://&lt;the full URL of your organization's domain&gt;/integrations/oauth2/api/v1/token</code> </p> <p class="example" data-mc-autonum="<b>Example: </b>"><span class="autonumber"><span><b>예: </b></span></span><code>https://myorganization.my.workfront.com/integrations/oauth2/api/v1/token</code> </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">범위</td> 
   <td>범위를 지정할 필요가 없습니다. </td> 
  </tr> 
 </tbody> 
</table>

## 인증 코드 흐름 설정

![](assets/oauth-2-authorization-code-flow-350x194.png)

OAuth2로 사용자를 로그인하려면 다음 프로세스를 사용하십시오.

1. 사용자가 인증 페이지를 열면 Workfront 로그인 페이지로 리디렉션되므로 Workfront에 로그인할 수 있습니다. 사용자에게 SSO 구성이 있는 경우 ID 공급자 로그인 페이지가 열립니다.

   사용자가 동일한 브라우저에서 Workfront에 이미 로그인되어 있거나 Workfront에 성공적으로 로그인된 경우 사용자는 동의 화면으로 리디렉션됩니다.

   ![](assets/consent-screen-350x227.png)

1. 사용자가 액세스를 허용하면 페이지가 `redirect_url`. 리디렉션에는 다음 쿼리 매개 변수가 포함되어야 합니다.

* `code`: 액세스/새로 고침 토큰을 가져오는 데 필요한 인증 코드입니다.
* `domain`: 조직의 도메인. 예: in `myorganization.my.workfront.com`, 도메인 `myorganization`.
* `lane`: 요청의 레인. 예: in `myorganization.preview.workfront.com`, 레인은 `preview`.

  >[!IMPORTANT]
  >
  >다음 `code` 은(는) 2분 동안만 유효합니다. 따라서 해당 시간 내에 새로 고침 및 액세스 토큰을 받아야 합니다.

1. 코드가 있으면에서 클라이언트 앱 자격 증명과 함께 코드를 보냄으로써 새로 고침을 요청하고 토큰에 액세스할 수 있습니다. `/integrations/oauth2/api/v1/token` 엔드포인트.

   전체 토큰 요청 URL은

   ```
   https://<URL of your organization's domain></span>/integrations/oauth2/api/v1/token
   ```

   **예:**  토큰 엔드포인트에 대한 CURL 호출의 예:

   예 1

   ```
      curl --location --request POST '**<workfront host>**/integrations/oauth2/api/v1/token' \
      --header 'Authorization: Basic **<base64(client_id:client_secret)>**' \
      --header 'Content-Type: application/json' \
      --data-raw '{
      "code": "**<code>**",
      "grant_type": "**authorization_code**",
      "redirect_uri": "**<redirect_url>**"
      }'
   ```

   예제 2

   ```
      curl --location --request POST '**<workfront host>**/integrations/oauth2/api/v1/token' \
      --header 'Content-Type: application/x-www-form-urlencoded' \
      --data-urlencode 'grant_type=**authorization_code**' \
      --data-urlencode 'redirect_uri=**<redirect_url>**' \
      --data-urlencode 'code=**<code>**' \
      --data-urlencode 'client_id=**<client_id>**' \
      --data-urlencode 'client_secret=**<client_secret>**'  
   ```


   >[!IMPORTANT]
   >
   > 클라이언트 암호는 Workfront에서 앱을 등록할 때 생성되었습니다. 분실 시 복구할 수 없으므로 안전한 장소에 보관해야 합니다.

   전달된 모든 매개 변수가 올바르면 토큰 끝점이 다음 페이로드를 반환합니다.

   ```
   {
      "token_type": "sessionID",
      "access_token": "string", // the value of sessionID
      "refresh_token": "string",
      "expires_in": 0,
      "wid": "string"
   }
   ```

   액세스 토큰은 와 동일합니다. ```sessionID```, 및 는 일반과 동일한 방식으로 만료됩니다 ```sessionID```

   >[!IMPORTANT]
   >
   > 보안 위치에 새로 고침 토큰을 저장합니다. 이전 토큰이 만료되면 새 새로 고침 토큰을 받아야 합니다. Workfront은 새로 고침 토큰을 저장하지 않습니다.

1. 이제 액세스 토큰이 있으면 Workfront에 대한 API를 호출할 수 있습니다

   ```
   curl --request GET 'https://<workfront host>/attask/api/v14.0/proj/search \
   --header 'sessionID: <access_token>'
   ```

## 액세스 토큰 새로 고침 설정

![](assets/refresh-access-token-flow-350x142.png)

access_token을 새로 고치려면 토큰 끝점에 대해 &#39;POST&#39; 호출을 다시 수행해야 합니다. 이번에는 다음과 같이 다른 양식 데이터를 보냅니다.

```
curl --location --request POST '<workfront host>/integrations/oauth2/api/v1/token' \
--header 'Authorization: Basic <base64(client_id:client_secret)>' \
--header 'Content-Type: application/json' \
--data-raw '{
   "grant_type": "refresh_token",
   "refresh_token": "<refresh_token>"
}'

###### OR

curl --location --request POST '<workfront host>/integrations/oauth2/api/v1/token' \
--header 'Content-Type: application/x-www-form-urlencoded' \
--data-urlencode 'grant_type=refresh_token' \
--data-urlencode 'redirect_uri=<redirect_url>' \
--data-urlencode 'refresh_token=<refresh_token>' \
--data-urlencode 'client_id=<client_id>' \
--data-urlencode 'client_secret=<client_secret>'
```

이 메서드는 다음 결과를 반환합니다.

```
{
  "token_type": "sessionID",
  "access_token": "string", // the value of sessionID
  "refresh_token": "string",
  "expires_in": 0,
  "wid": "string"
}
```

그리고 액세스 토큰은 `sessionID` Workfront에 API 요청을 하는 데 사용할 수 있습니다.
