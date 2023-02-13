---
content-type: reference
product-previous: workfront-fusion
product-area: workfront-integrations
keywords: 커넥터
navigation-topic: http-modules
title: HTTP &gt; OAuth 2.0 요청 모듈 만들기
description: 다음을 만들려면 [!DNL Adobe Workfront Fusion] OAuth 2.0 인증이 필요한 서버에 대한 HTTP(S) 요청은 먼저 OAuth 연결을 만들어야 합니다. [!DNL Adobe Workfront Fusion] 은 이 연결을 사용하여 호출된 모든 호출에 적절한 인증 헤더가 있으며 필요한 경우 관련 토큰을 자동으로 새로 고침하도록 합니다.
author: Becky
feature: Workfront Fusion
exl-id: 6c68c9b9-9f74-44a7-94ed-3785081b8331
source-git-commit: 885d93dd4383945538e977fd3edbfd55bda88b70
workflow-type: tm+mt
source-wordcount: '2172'
ht-degree: 0%

---

# [!UICONTROL HTTP] > [!UICONTROL OAuth 2.0 요청 만들기] 모듈

>[!NOTE]
>
>[!DNL Adobe Workfront Fusion] 를 사용하려면 [!DNL Adobe Workfront Fusion] 라이센스 [!DNL Adobe Workfront] 라이센스.

다음을 만들려면 [!DNL Adobe Workfront Fusion] OAuth 2.0 인증이 필요한 서버에 대한 HTTP(S) 요청은 먼저 OAuth 연결을 만들어야 합니다. [!DNL Adobe Workfront Fusion] 은 이 연결을 사용하여 호출된 모든 호출에 적절한 인증 헤더가 있으며 필요한 경우 관련 토큰을 자동으로 새로 고침하도록 합니다.

[!DNL Workfront Fusion] 은 다음 OAuth 2.0 인증 흐름을 지원합니다.

* 인증 코드 흐름
* 암시적 흐름

리소스 소유자 암호 자격 증명 흐름 및 클라이언트 자격 증명 흐름과 같은 다른 흐름은 이 모듈을 통해 자동으로 지원되지 않습니다.

OAuth 2.0 인증에 대한 자세한 내용은 [OAuth 2.0 인증 프레임워크](https://tools.ietf.org/html/rfc6749).

## 액세스 요구 사항

이 문서의 기능을 사용하려면 다음 액세스 권한이 있어야 합니다.

<table style="table-layout:auto">  
 <col> 
 <col> 
 <tbody> 
  <tr> 
    <td role="rowheader">[!DNL Adobe Workfront] 플랜*</td> 
   <td> <p>[!UICONTROL Pro] 이상</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader">[!DNL Adobe Workfront] 라이센스*</td> 
   <td> <p>[!UICONTROL Plan], [!UICONTROL Work]</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront Fusion] license**</td> 
   <td> <p>[!UICONTROL [!DNL Workfront Fusion] 작업 자동화 및 통합을 위한] </p>  </td> 
  </tr> 
  <tr> 
   <td role="rowheader">제품</td> 
   <td>조직이 구매해야 합니다 [!DNL Adobe Workfront Fusion] 뿐만 아니라 [!DNL Adobe Workfront] 을 참조하십시오.</td> 
  </tr>
 </tbody> 
</table>

어떤 계획, 라이센스 유형 또는 액세스 권한을 보유하고 있는지 확인하려면 [!DNL Workfront] 관리자

에 대한 자세한 정보 [!DNL Adobe Workfront Fusion] 라이센스 [[!DNL Adobe Workfront Fusion] 라이선스](../../../workfront-fusion/get-started/license-automation-vs-integration.md)

## 에 대한 연결 만들기 [!DNL OAuth] 요청

* [HTTP > OAuth 2.0 요청 모듈에서 연결을 만드는 데 필요한 일반 지침](#general-instructions-for-creating-a-connection-in-the-http--make-an-oauth-20-request-module)
* [HTTP >[!UICONTROL 만들기] OAuth 2.0 요청 모듈](#instructions-for-creating-a-connection-to-google-in-the-http-make-an-oauth-20-request-module)
* [HTTP > OAuth 2.0 요청 모듈을 통해 Microsoft Graph API에 연결하는 지침](#instructions-for-connecting-to-microsoft-graph-api-via-the-http--make-an-oauth-20-request-module)

### 에서 연결을 만들기 위한 일반적인 지침 [!UICONTROL HTTP] > [!UICONTROL OAuth 2.0 요청 만들기] 모듈

1. 에서 OAuth 클라이언트 만들기 [!DNL target] 원하는 서비스 [!DNL Adobe Workfront Fusion] 통신하기 위해 이 옵션은 [!UICONTROL 개발자] 해당 서비스의 섹션.

   1. 클라이언트를 작성할 때 `[!UICONTROL Redirect URL]` 또는 `[!UICONTROL Callback URL]` 필드:

      | 미국/APAC | https://app.workfrontfusion.com/oauth/cb/oauth2 |
      |---|---|
      | EMEA | https://app-eu.workfrontfusion.com/oauth/cb/oauth2 |

   1. 클라이언트를 만들면 지정된 서비스에는 다음과 같은 2개의 키가 표시됩니다. `[!UICONTROL Client ID]` 및 `[!UICONTROL Client Secret]`. 일부 서비스에서는 이러한 기능을 `[!UICONTROL App Key]` 및 `[!UICONTROL App Secret]` . 보안 위치에 키와 암호를 저장하므로 Workfront Fusion에서 연결을 만들 때 키를 제공할 수 있습니다.

1. 를 찾습니다. `[!UICONTROL Authorize URI]` 및 `[!UICONTROL Token URI]` ( 해당 서비스의 API 설명서 )를 참조하십시오. 다음 URL은 [!DNL Workfront Fusion] 와의 통신 [!DNL target] 서비스. 주소는 OAuth 인증을 위해 사용됩니다.

   >[!NOTE]
   >
   >서비스에서 암시적 플로우를 사용하는 경우 `[!UICONTROL Authorize URI]`.

   >[!INFO]
   >
   >**예:** Yahoo 주소:
   >
   >* 권한 부여 URI:
   >
   >`https://api.login.yahoo.com/oauth2/request_auth`
   >
   >* 토큰 URI:
   >
   >`https://api.login.yahoo.com/oauth2/get_token`

1. (조건부) 대상 서비스가 범위(액세스 권한)를 사용하는 경우 서비스에서 개별 범위를 구분하는 방법을 확인하고 그에 따라 고급 설정에서 구분자를 설정했는지 확인합니다. 구분 기호가 올바로 설정되지 않으면, [!DNL Workfront Fusion] 연결을 만들지 못했으므로 잘못된 범위 오류가 표시됩니다.
1. 위의 단계를 완료하면에서 OAuth 연결을 만들 수 있습니다 [!DNL Workfront Fusion]. 시나리오에 OAuth 2.0 HTTP(S) 요청 및 응답 처리 모듈을 추가합니다.
1. 모듈의 연결 필드에서 **[!UICONTROL 추가]**.

1. 연결을 만들려면 다음 필드를 입력합니다.

   <table style="table-layout:auto">  
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">[!UICONTROL 연결 이름] </td> 
      <td> <p>연결의 이름을 입력합니다.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"> <p>[!UICONTROL 흐름 유형]</p> </td> 
      <td> <p>토큰을 가져오는 흐름을 선택합니다.</p> 
       <ul> 
        <li><strong>[!UICONTROL Authorization Code]</strong>: 을(를) 입력합니다. <code>[!UICONTROL Authorize URI]</code> 및 <code>[!UICONTROL Token URI]</code> 를 참조하십시오.</li> 
        <li><strong>[!UICONTROL Implicit]</strong>: 을(를) 입력합니다. <code>[!UICONTROL Authorize URI]</code> 를 참조하십시오.</li> 
       </ul> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL 범위] </td> 
      <td> <p>개별 범위를 추가합니다. 해당 서비스의 개발자(API) 설명서에서 이 정보를 찾을 수 있습니다.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL 범위 구분 기호] </td> 
      <td> <p>위에 입력한 범위를 구분하여 선택합니다. 해당 서비스의 개발자(API) 설명서에서 이 정보를 찾을 수 있습니다.</p> <p>경고: 구분 기호가 올바로 설정되지 않으면, [!DNL Workfront Fusion] 연결을 만들지 못했습니다. 잘못된 범위 오류가 표시됩니다.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL Client ID] </td> 
      <td> <p>클라이언트 ID를 입력합니다. 연결할 서비스에서 OAuth 클라이언트를 만들 때 클라이언트 ID를 받았습니다.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL Client Secret]</td> 
      <td> <p> 클라이언트 암호를 입력합니다. 연결하려는 서비스에서 OAuth 클라이언트를 만들 때 클라이언트 암호를 받았습니다.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"> <p>[!UICONTROL Authorization 매개 변수]</p> </td> 
      <td> <p>인증 호출에 포함할 매개 변수를 추가합니다. 다음 표준 매개 변수는 항상 자동으로 포함되며 추가할 필요가 없습니다.</p> <p>표준 매개 변수:</p> 
       <ul> 
        <li> <p><strong>[!UICONTROL response_type]</strong> </p> <p> <code>code </code>[!UICONTROL 인증 코드 흐름] 및 <code>token </code>[!UICONTROL 암시적 흐름]용</p> </li> 
        <li> <p><strong>[!UICONTROL redirect_uri]</strong> </p> 
         <table style="table-layout:auto">  
          <col> 
          <col> 
          <tbody> 
           <tr> 
            <td role="rowheader">미국/APAC</td> 
            <td>https://app.workfrontfusion.com/oauth/cb/oauth2</td> 
           </tr> 
           <tr> 
            <td role="rowheader">EMEA </td> 
            <td>https://app-eu.workfrontfusion.com/oauth/cb/oauth2</td> 
           </tr> 
          </tbody> 
         </table> </li> 
        <li> <p><strong>[!UICONTROL client_id]</strong> </p> <p> 계정을 만들 때 받은 클라이언트 ID</p> </li> 
       </ul> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"> <p>[!UICONTROL 액세스 토큰 매개 변수]</p> </td> 
      <td> <p>토큰 호출에 포함할 매개 변수를 추가합니다. 다음 표준 매개 변수는 항상 자동으로 포함되며 추가할 필요가 없습니다.</p> <p>표준 매개 변수:</p> 
       <ul> 
        <li><strong>[!UICONTROL grant_type]</strong>: <code>authorization_code</code></li> 
        <li> <p><strong>[!UICONTROL redirect_uri]:</strong> </p> 
         <table style="table-layout:auto">  
          <col> 
          <col> 
          <tbody> 
           <tr> 
            <td role="rowheader">미국/APAC</td> 
            <td>https://app.workfrontfusion.com/oauth/cb/oauth2</td> 
           </tr> 
           <tr> 
            <td role="rowheader">EMEA </td> 
            <td>https://app-eu.workfrontfusion.com/oauth/cb/oauth2</td> 
           </tr> 
          </tbody> 
         </table> </li> 
        <li><strong>[!UICONTROL client_id]</strong>: 계정을 만들 때 받은 클라이언트 ID는 요청 본문에 자동으로 포함됩니다</li> 
        <li><strong>client_secret</strong>: 계정을 만들 때 받은 클라이언트 암호는 요청 본문에 자동으로 포함됩니다</li> 
        <li><strong>코드</strong>: 인증 요청에서 반환된 코드</li> 
       </ul> <p>참고:  <p>OAuth 2.0 표준은 이 단계(<code>[!UICONTROL client_secret_basic]</code> 및 <code>[!UICONTROL client_secret_post]</code>). [!DNL Workfront Fusion] 는 자동으로 <code>[!UICONTROL client_secret_post]</code> 메서드를 사용합니다. 따라서 이러한 매개 변수는 자동으로 토큰 요청 본문의 일부로 포함됩니다. </p> <p>OAuth 2.0 인증에 대한 자세한 내용은 <a href="https://tools.ietf.org/html/rfc6749">OAuth 2.0 인증 프레임워크</a>.</p> </p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"> <p>[!UICONTROL 새로 고침 토큰 매개 변수]</p> </td> 
      <td> <p>토큰 호출에 포함할 매개 변수를 추가합니다. 다음 표준 매개 변수는 항상 자동으로 포함되며 추가할 필요가 없습니다.</p> <p>표준 매개 변수:</p> 
       <ul> 
        <li> <p><strong>[!UICONTROL grant_type]</strong>: <code>refresh_token</code></p> </li> 
        <li> <p><strong>[!UICONTROL refresh_token]</strong>: 연결 중인 서비스에서 얻은 가장 최근 새로 고침 토큰</p> </li> 
        <li> <p><strong>[!UICONTROL client_id]</strong>: 계정을 만들 때 받은 클라이언트 ID는 요청 본문에 자동으로 포함됩니다</p> </li> 
        <li> <p><strong>[!UICONTROL client_secret]</strong>: 계정을 만들 때 받은 클라이언트 암호는 요청 본문에 자동으로 포함됩니다</p> </li> 
       </ul> <p>참고:  <p>OAuth 2.0 표준은 이 단계(<code>[!UICONTROL client_secret_basic]</code> 및 <code>[!UICONTROL client_secret_post]</code>). [!DNL Workfront Fusion] 는 자동으로 <code>[!UICONTROL client_secret_post]</code> 메서드를 사용합니다. 따라서 이러한 매개 변수는 자동으로 토큰 요청 본문의 일부로 포함됩니다. </p> <p>OAuth 2.0 인증에 대한 자세한 내용은 <a href="https://tools.ietf.org/html/rfc6749">OAuth 2.0 인증 프레임워크</a>.</p> </p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"> <p>[!UICONTROL Custom Headers]</p> </td> 
      <td> <p>[!UICONTROL 토큰] 및 R[!UICONTROL 참조 토큰] 단계의 헤더에 포함할 추가 키와 값을 지정합니다.</p> <p>참고:  <p>OAuth 2.0 표준은 이 단계(<code>[!UICONTROL client_secret_basic]</code> 및 <code>[!UICONTROL client_secret_post]</code>). [!DNL Workfront Fusion] 은 자동으로 을 지원하지 않습니다 <code>[!UICONTROL client_secret_basic]</code> 메서드를 사용합니다. 연결하는 서비스에서 클라이언트 ID와 클라이언트 암호를 단일 문자열로 결합하고 base64를 인증 헤더로 인코딩해야 하는 경우 해당 헤더와 키 값을 여기에 추가해야 합니다.</p> <p> OAuth 2.0 인증에 대한 자세한 내용은 <a href="https://tools.ietf.org/html/rfc6749">OAuth 2.0 인증 프레임워크</a>.</p> </p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"> <p>[!UICONTROL 토큰 배치]</p> </td> 
      <td> <p>[!UICONTROL header], [!UICONTROL 쿼리 문자열]에서 토큰을 전송할지 또는 지정된 URL에 연결할 때 양식에서 토큰을 전송할지를 선택합니다.</p> <p>토큰은 가장 일반적으로 요청 헤더에서 전송됩니다.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL 헤더 토큰 이름] </td> 
      <td> <p>헤더에 인증 토큰의 이름을 입력합니다. 기본: <code>[!UICONTROL Bearer]</code>.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL 쿼리 문자열 매개 변수 이름] </td> 
      <td> <p>쿼리 문자열에 인증 토큰의 이름을 입력합니다. 기본: <code>[!UICONTROL access_token]</code>.</p> </td> 
     </tr> 
    </tbody> 
   </table>

1. 클릭 **[!UICONTROL 계속]** 연결 설정을 저장하려면 다음을 수행하십시오.
1. 계속 [OAuth 2.0 요청 모듈 설정](#oauth-20-request-module-setup).

### 연결 만들기 지침 [!DNL Google] 에서 [!UICONTROL HTTP] >[!UICONTROL OAuth 2.0 요청 모듈 만들기]

다음 예는 를 사용하는 방법을 보여줍니다. [!UICONTROL HTTP] > [!UICONTROL OAuth 2.0 만들기] 연결할 모듈을 요청합니다. [!DNL Google].

1. 에 설명된 대로 프로젝트를 만들고, OAuth 설정을 구성하고, 자격 증명을 생성했는지 확인합니다. [Connect [!DNL Adobe Workfront Fusion] to [!DNL Google Services] 사용자 지정 OAuth 클라이언트 사용](../../../workfront-fusion/connections/connect-fusion-to-google-using-oauth.md).
1. 를 엽니다. [!UICONTROL HTTP] >[!UICONTROL OAuth 2.0 요청 만들기] 모듈.
1. 클릭 **[!UICONTROL 추가]** 연결 상자 옆에 있습니다.
1. 다음 값을 입력합니다.

   <table style="table-layout:auto">  
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">[!UICONTROL 연결 이름] </td> 
      <td> <p>연결의 이름을 입력합니다.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"> <p>[!UICONTROL 흐름 유형]</p> </td> 
      <td> <p>[!UICONTROL Authorization Code]</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL 권한 URI]</td> 
      <td><code>https://accounts.google.com/o/oauth2/v2/auth</code> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL 토큰 URI]</td> 
      <td><code>https://www.googleapis.com/oauth2/v4/token</code> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL 범위] </td> 
      <td> <p>개별 범위를 추가합니다. 범위에 대한 자세한 내용은 <a href="https://developers.google.com/identity/protocols/oauth2/scopes">에 대한 OAuth 2.O 범위 [!DNL Google] API</a> 에서 [!DNL Google] 설명서.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL 범위 구분 기호] </td> 
      <td> <p>[!UICONTROL SPACE]</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL Client ID] </td> 
      <td> <p>을(를) 입력합니다. [!DNL Google] 클라이언트 ID. </p> <p>클라이언트 ID를 만들려면 다음을 참조하십시오 <a href="../../../workfront-fusion/connections/connect-fusion-to-google-using-oauth.md#create2" class="MCXref xref">OAuth 자격 증명 만들기</a> in <a href="../../../workfront-fusion/connections/connect-fusion-to-google-using-oauth.md" class="MCXref xref">[!DNL Connect Adobe Workfront Fusion] to [!DNL Google Services] 사용자 지정 OAuth 클라이언트 사용</a>.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL Client Secret]</td> 
      <td> <p>을(를) 입력합니다. [!DNL Google] 클라이언트 암호. </p> <p>클라이언트 암호를 만들려면 다음을 참조하십시오 <a href="../../../workfront-fusion/connections/connect-fusion-to-google-using-oauth.md#create2" class="MCXref xref">OAuth 자격 증명 만들기</a> in <a href="../../../workfront-fusion/connections/connect-fusion-to-google-using-oauth.md" class="MCXref xref">[!DNL Connect Adobe Workfront Fusion] to [!DNL Google] 사용자 지정 OAuth 클라이언트를 사용하는 서비스</a>.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"> <p>[!UICONTROL Authorization 매개 변수]</p> </td> 
      <td> <p>추가 <code>[!UICONTROL access_type]</code> - <code>[!UICONTROL offline] </code>키-값 쌍입니다.</p> <p> <img src="assets/google-authentication-http.png"> </p> <p>참고: 토큰 새로 고침과 같은 인증 문제가 발생하는 경우에는 <code>[!UICONTROL prompt] </code>- <code>[!UICONTROL consent] </code>키-값 쌍입니다.</p> </td> 
     </tr> 
    </tbody> 
   </table>

1. 클릭 **[!UICONTROL 계속]** 연결 설정을 저장하려면 다음을 수행하십시오.
1. 계속 [OAuth 2.0 요청 모듈 설정](#oauth-20-request-module-setup).

### 연결 지침 [!DNL Microsoft Graph API] 사용 [!UICONTROL HTTP] > [!UICONTROL OAuth 2.0 요청 만들기] 모듈

관련 지침 [!DNL Microsoft Graph API]를 참조하십시오. [호출 [!DNL MS Graph REST API] 사용 [!DNL Adobe Workfront Fusion] [!UICONTROL HTTP] > [!UICONTROL OAuth 2.0 요청 만들기] 모듈](../../../workfront-fusion/connections/call-the-ms-graph-rest-api-.md).

## OAuth 2.0 요청 모듈 설정

을(를) 설정한 경우 [!DNL Oauth 2]에 설명된 대로 [에 대한 연결 만들기 [!DNL OAuth] 요청](#creating-a-connection-for-an-oauth-request)원하는 대로 모듈을 계속 설정합니다. 모든 인증 토큰은 이 요청과 동일한 연결을 사용하는 다른 모든 요청에 자동으로 포함됩니다.

를 구성할 때 [!UICONTROL HTTP] >[!UICONTROL OAuth 2.0 요청 만들기] 모듈, [!DNL Workfront Fusion] 아래 나열된 필드를 표시합니다. 모듈에서 굵게 표시된 제목은 필수 필드를 나타냅니다.

필드 또는 함수 위에 맵 단추가 표시되면 이 단추를 사용하여 해당 필드에 대한 변수와 함수를 설정할 수 있습니다. 자세한 내용은 [의 한 모듈에서 다른 모듈로 정보 매핑 [!DNL Adobe Workfront Fusion]](../../../workfront-fusion/mapping/map-information-between-modules.md).

<!--
<img src="assets/map-toggle-350x74.png" style="width: 350;height: 74;" data-mc-conditions="QuicksilverOrClassic.Draft mode">
-->

<table style="table-layout:auto">  
 <col> 
 <col> 
 <tbody> 
  <tr data-mc-conditions=""> 
   <td role="rowheader">[!UICONTROL Connection]</td> 
   <td> <p>연결 설정에 대한 자세한 내용은 <a href="#creating-a-connection-for-an-oauth-request" class="MCXref xref">OAuth 요청에 대한 연결 만들기</a> 참조하십시오.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL 모든 상태를 오류로 평가(2xx 및 3xx 제외) </td> 
   <td> <p>이 옵션을 사용하여 오류 처리를 설정합니다.</p> <p>자세한 내용은 <a href="../../../workfront-fusion/errors/error-handling.md" class="MCXref xref">에서 오류 처리 중 [!DNL Adobe Workfront Fusion]</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL URL] </td> 
   <td> <p>API 엔드포인트, 웹 사이트 등과 같이 요청을 전송할 URL을 입력합니다.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL 메서드]</p> </td> 
   <td> <p>API 호출을 구성하는 데 필요한 HTTP 요청 메서드를 선택합니다. 자세한 내용은 <a href="../../../workfront-fusion/modules/http-request-methods.md" class="MCXref xref">의 HTTP 요청 메서드 [!DNL Adobe Workfront Fusion]</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Headers] </td> 
   <td> <p>요청의 헤더를 표준 JSON 개체 형태로 추가합니다. For example, <code>{"Content-type":"application/json"}</code></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL 쿼리 문자열]</td> 
   <td> <p> 원하는 쿼리 키-값 쌍을 입력합니다.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Body type]</p> </td> 
   <td> <p>HTTP Body는 사용할 데이터 바이트가 있는 경우 헤더 바로 뒤에 HTTP 트랜잭션 메시지로 전송되는 데이터 바이트입니다.</p> 
    <ul> 
     <li> <p><strong>[!UICONTROL Raw]</strong> </p> <p>원시 본문 유형은 일반적으로 개발자 설명서에서 전송할 데이터를 지정하지 않는 경우에도 대부분의 HTTP 본문 요청에 적합합니다.</p> <p>[!UICONTROL 콘텐츠 유형] 필드에서 데이터를 구문 분석하는 형식을 지정합니다.</p> <p>컨텐츠 유형을 선택했지만, 데이터는 개발자 설명서에서 규정하거나 필요로 하는 형식으로 입력됩니다.</p> </li> 
     <li> <p><strong>[!UICONTROL Application/x-www-form-urlencoded]</strong> </p> <p>이 본문 유형은 <code>[!UICONTROL application/x-www-form-urlencoded]</code>.</p> <p>대상 <code>[!UICONTROL application/x-www-form-urlencoded]</code>를 지정하는 경우, 서버로 전송되는 HTTP 메시지의 본문은 기본적으로 하나의 쿼리 문자열입니다. 키 및 값은 키-값 쌍으로 구분되어 인코딩됩니다 <code>&amp;</code> 그리고 <code>=</code> 키와 값 사이에 있을 수 있습니다. </p> <p>이진 데이터의 경우, <code>use [!UICONTROL multipart/form-data]</code> 을 가리키도록 업데이트하는 것이 좋습니다.</p> 
      <div class="example" data-mc-autonum="<b>Example: </b>">
       <span class="autonumber"><span><b>예: </b></span></span> 
       <p>결과 HTTP 요청 형식의 예:</p> 
       <p><code>field1=value1&amp;field2=value2</code> </p> 
      </div> </li> 
     <li> <p><strong>[!UICONTROL Multipart/form-data]</strong> </p> <p>[!UICONTROL Multipart/form-data]는 파일과 데이터를 보내는 데 사용되는 HTTP 다중 부분 요청입니다. 일반적으로 서버에 파일을 업로드하는 데 사용됩니다.</p> <p>요청에서 전송할 필드를 추가합니다. 각 필드에는 키-값 쌍이 포함되어야 합니다.</p> 
      <ul> 
       <li> <p><strong>[!UICONTROL Text]</strong> </p> <p>요청 본문 내에 전송할 키와 값을 입력합니다.</p> </li> 
       <li> <p><strong>[!UICONTROL File]</strong> </p> <p>키를 입력하고 요청 본문에 전송할 소스 파일을 지정합니다.</p> <p>이전 모듈에서 업로드할 파일(예: [!UICONTROL HTTP] &gt;[!UICONTROL 파일 가져오기] 또는 [!UICONTROL Google Drive] &gt;[!UICONTROL 파일 다운로드)]을 매핑하거나 파일 이름과 파일 데이터를 수동으로 입력합니다.</p> </li> 
      </ul> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL 구문 분석 응답]</p> </td> 
   <td> <p>[!UICONTROL JSON] &gt; [!UICONTROL Parse JSON] 또는 [!UICONTROL XML] &gt; [!UICONTROL Parse XML] 모듈을 사용할 필요가 없도록 응답을 자동으로 구문 분석하고 JSON 및 XML 응답을 변환하려면 이 옵션을 활성화합니다.</p> <p>구문 분석된 JSON 또는 XML 컨텐츠를 사용하기 전에 모듈이 응답 컨텐츠를 인식하고 후속 모듈에 매핑할 수 있도록 모듈을 한 번 수동으로 실행하십시오.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Timeout] </td> 
   <td> <p>요청 시간 제한(초-1-300)을 입력합니다. 기본값은 40초입니다.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL 다른 HTTP 모듈과 쿠키 공유]</td> 
   <td> <p> 시나리오의 모든 HTTP 모듈과 서버에서 쿠키를 공유하려면 이 옵션을 활성화합니다.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL 자체 서명 인증서]</td> 
   <td> <p> 자체 서명된 인증서를 사용하여 TLS를 사용하려면 인증서를 업로드합니다.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL 확인되지 않은(자체 서명) 인증서를 사용하는 연결 거부] </td> 
   <td> <p>확인되지 않은 TLS 인증서를 사용하는 연결을 거부하려면 이 옵션을 활성화합니다.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL 리디렉션 후]</td> 
   <td> <p> 3xx 응답이 있는 URL 리디렉션을 따르려면 이 옵션을 활성화합니다.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL 모든 리디렉션 따르기] </td> 
   <td> <p>모든 응답 코드가 있는 URL 리디렉션을 따르려면 이 옵션을 활성화합니다.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL 배열과 동일한 여러 쿼리 문자열 키의 직렬화를 사용하지 않도록 설정]</p> </td> 
   <td> <p>기본적으로 [!DNL Workfront Fusion] 배열과 동일한 URL 쿼리 문자열 매개 변수 키의 여러 값을 처리합니다. 예, <code>www.test.com?foo=bar&amp;foo=baz</code> 은(는) <code>www.test.com?foo[0]=bar&amp;foo[1]=baz</code>. 이 기능을 비활성화하려면 이 옵션을 활성화합니다. </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL 압축된 콘텐츠 요청]</td> 
   <td> <p> 웹 사이트의 압축 버전을 요청하려면 이 옵션을 활성화합니다.</p> <p>이 옵션을 추가하면 <code>[!UICONTROL Accept-Encoding]</code> 헤더를 사용하여 압축된 콘텐츠를 요청합니다.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Use Mutual TLS]</td> 
   <td> <p>HTTP 요청에서 상호 TLS를 사용하려면 이 옵션을 활성화하십시오.</p> <p>상호 TLS에 대한 자세한 내용은 다음을 참조하십시오 <a href="../../../workfront-fusion/apps-and-their-modules/http-modules/use-mtls-in-http-modules.md" class="MCXref xref">의 HTTP 모듈에서 상호 TLS 사용 [!DNL Adobe Workfront Fusion]</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>
