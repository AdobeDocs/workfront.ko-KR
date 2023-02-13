---
title: 를 통해 MS Graph REST API를 호출합니다 [!DNL Adobe Workfront Fusion] HTTP &gt; OAuth 2.0 요청 모듈 만들기
description: 를 통해 MS Graph REST API를 호출합니다 [!DNL Adobe Workfront Fusion] HTTP &gt; OAuth 2.0 요청 모듈 만들기
author: Becky
draft: Probably
feature: Workfront Fusion
exl-id: adae390d-8b9e-4dab-8551-605e50af5a1e
source-git-commit: 885d93dd4383945538e977fd3edbfd55bda88b70
workflow-type: tm+mt
source-wordcount: '568'
ht-degree: 1%

---

# 호출[!UICONTROL  MS Graph REST API] 사용 [!DNL Adobe Workfront Fusion] [!UICONTROL HTTP] > [!UICONTROL OAuth 2.0 요청 만들기] 모듈

많은 [!DNL Microsoft] 웹 서비스는 [!DNL Microsoft Graph API]. 이 문서에서는 [!DNL Workfront Fusion] [!DNL HTTP] > [!UICONTROL OAuth 2.0 요청 만들기] 모듈.

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
   <td> <p>[!UICONTROL [!DNL Workfront Fusion] 작업 자동화 및 통합을 위한] </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">제품</td> 
   <td>조직이 구매해야 합니다 [!DNL Adobe Workfront Fusion] 뿐만 아니라 [!DNL Adobe Workfront] 을 참조하십시오.</td> 
  </tr>
 </tbody> 
</table>

어떤 계획, 라이센스 유형 또는 액세스 권한을 보유하고 있는지 확인하려면 [!DNL Workfront] 관리자

에 대한 자세한 정보 [!DNL Adobe Workfront Fusion] 라이센스 [[!DNL Adobe Workfront Fusion] 라이선스](../../workfront-fusion/get-started/license-automation-vs-integration.md).

## 등록 [!DNL Workfront Fusion] 에서 [!DNL Microsoft Application Registration Portal]

에 대한 연결을 만들려면 [!DNL Microsoft Graph REST API], 먼저 등록해야 합니다. [!DNL Adobe Workfront Fusion].

1. 에 설명된 대로 새 응용 프로그램 등록을 시작합니다. [앱 등록](https://docs.microsoft.com/en-us/graph/auth-register-app-v2) 에서 [!DNL Microsoft] 설명서.

   등록의 일환으로 [!DNL Microsoft] 를 사용하려면 다음 정보가 필요합니다.

   <table style="table-layout:auto">
      <tr>
        <td>[!UICONTROL 응용 프로그램 이름]</td>
        <td>"My"와 같이 응용 프로그램의 이름을 입력합니다. [!DNL Workfront Fusion] 응용 프로그램."</td>
      </tr>
      <tr>
        <td>[!UICONTROL 리디렉션 URL]</td>
        <td><code>https://app.workfrontfusion.com/oauth/cb/oauth2</code></td>
      </tr>
    </table>

1. 앱 등록을 완료하면 다음을 참고하십시오 [!UICONTROL 애플리케이션 ID].

   >[!IMPORTANT]
   >
   >에서 연결을 설정하려면 애플리케이션 ID가 필요합니다 [!DNL Workfront Fusion].

1. 생성 [!UICONTROL 응용 프로그램 암호]. 이 비밀을 명심해라.

   자세한 내용은 [앱 등록](https://docs.microsoft.com/en-us/graph/auth-register-app-v2) 에서 [!DNL Microsoft] 설명서.

   >[!IMPORTANT]
   >
   >다음을 수행해야 합니다. [!UICONTROL 응용 프로그램 암호] 에서 연결을 설정하려면 다음을 수행하십시오. [!DNL Workfront Fusion].

1. 애플리케이션에 대한 권한을 구성합니다.

   이러한 필드를 찾고 구성하는 방법에 대한 자세한 내용은 의 &quot;Microsoft 그래프에 대한 권한 구성&quot; 섹션을 참조하십시오 [사용자 없이 액세스 가능](https://docs.microsoft.com/en-us/graph/auth-v2-service) 에서 [!UICONTROL Microsoft] 설명서.

   <table style="table-layout:auto">
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">[!UICONTROL 응용 프로그램에 필요한 권한 유형은 무엇입니까?]</td> 
      <td>선택 <code>[!UICONTROL Delegated permissions]</code>.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL 권한 선택]</td> 
      <td> <p>다음 권한을 선택합니다.</p> 
       <ul> 
        <li> <p><code>offline_access</code> </p> </li> 
        <li> <p><code>openid</code> </p> </li> 
        <li> <p>통합에 필요한 기타 권한(예: <code>User.Read</code>)</p> </li> 
       </ul> <p>중요 사항: 에서 연결을 설정하려면 선택한 권한이 필요합니다 [!DNL Workfront Fusion].</p> </td> 
     </tr> 
    </tbody> 
   </table>

1. 다음 단계로 진행합니다 [구성 [!DNL MS Graph API] 연결 [!DNL Workfront Fusion]](#configure-your-ms-graph-api-connection-in-workfront-fusion).

## 구성 [!DNL MS Graph API] 연결 [!DNL Workfront Fusion]

등록 후 [!DNL Workfront Fusion] 에 설명된 대로 [등록 [!DNL Workfront Fusion] 에서 [!DNL Microsoft Application Registration Portal]](#register-workfront-fusion-in-the-microsoft-application-registration-portal)를 사용하여 연결을 구성할 수 있습니다. [!UICONTROL HTTP] >[!UICONTROL Oauth 2.0 만들기] 요청 모듈입니다.

1. 추가 [!UICONTROL HTTP] >[!UICONTROL OAuth 2.0 호출 만들기] 모듈에 대해 고려합니다.
1. 클릭 **[!UICONTROL 추가]** 다음 [!UICONTROL 연결] 필드.
1. 다음과 같이 연결 필드를 구성합니다.

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">[!UICONTROL 연결 이름]</td> 
      <td>연결의 이름을 입력합니다.</td> 
     </tr> 
     <tr> 
      <td role="rowheader"> <p role="rowheader">[!UICONTROL 흐름 유형]</p> </td> 
      <td><code>[!UICONTROL Authorization Code]</code> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL 권한 URI]</td> 
      <td><code>https://login.microsoftonline.com/common/oauth2/v2.0/authorize</code> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL 토큰 URI]</td> 
      <td><code>https://login.microsoftonline.com/common/oauth2/v2.0/token</code> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL 범위]</td> 
      <td> <p>4단계에서 선택한 권한을 입력합니다 <a href="#register-workfront-fusion-in-the-microsoft-application-registration-portal" class="MCXref xref">등록 [!DNL Workfront Fusion] 에서 [!DNL Microsoft Application Registration Portal]</a>.</p> <p>각 범위에 대해 <b>[!UICONTROL Add]</b> 을 입력하고 권한을 입력합니다.</p> <p>예: <code>offline_access</code>.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL 범위 구분 기호]</td> 
      <td><code>SPACE</code> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL Client ID]</td> 
      <td>의 2단계에서 [!UICONTROL 응용 프로그램 ID]를 입력합니다 <a href="#register-workfront-fusion-in-the-microsoft-application-registration-portal" class="MCXref xref">등록 [!DNL Workfront Fusion] 에서 [!DNL Microsoft Application Registration Portal]</a>.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL Client Secret]</td> 
      <td>2단계에서 생성한 [!UICONTROL 응용 프로그램 암호]를 입력합니다 <a href="#register-workfront-fusion-in-the-microsoft-application-registration-portal" class="MCXref xref">등록 [!DNL Workfront Fusion] 에서 [!DNL Microsoft Application Registration Portal]</a>.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL Authorization 매개 변수]</td> 
      <td> <p>다음 권한 부여 매개 변수를 추가합니다.</p> 
       <ul> 
        <li> <p>[!UICONTROL Key]:<code> response_mode</code> [!UICONTROL Value]: <code>query</code></p> </li> 
        <li> <p>[!UICONTROL Key]: <code>prompt </code>[!UICONTROL Value]: <code>consent</code></p> </li> 
       </ul> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL 액세스 토큰 매개 변수]</td> 
      <td>이 필드에 아무 것도 입력할 필요가 없습니다.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL 새로 고침 토큰 매개 변수]</td> 
      <td> 
       <ol> 
        <li value="1"> <p>클릭 <b>[!UICONTROL Add]</b>.</p> </li> 
        <li value="2"> <p>에서 <b>[!UICONTROL Key]</b> 필드, 입력 <code>scope</code>.</p> </li> 
        <li value="3"> <p>에서 <b>[!UICONTROL Value]</b> 필드에 범위 필드에 입력한 모든 [!UICONTROL 범위]를 공백으로 구분하여 입력합니다.</p> <p>예: <code>offline_access openid User.Read</code></p> </li> 
       </ol> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL Custom Headers]</td> 
      <td>이 필드에 아무 것도 입력할 필요가 없습니다.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL 토큰 배치]</td> 
      <td><code>[!UICONTROL In the header]</code> </td> 
     </tr> 
    </tbody> 
   </table>

1. 클릭 **[!UICONTROL 계속]**.
1. 표시되는 창에서 **[!UICONTROL 수락]** 를 클릭하여 연결을 완료하고 모듈로 돌아갑니다.
