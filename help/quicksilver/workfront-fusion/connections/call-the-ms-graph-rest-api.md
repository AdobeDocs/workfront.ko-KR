---
title: 를 통해 MS Graph REST API를 호출합니다. [!DNL Adobe Workfront Fusion] HTTP &gt; OAuth 2.0 요청 모듈 만들기
description: 를 통해 MS Graph REST API를 호출합니다. [!DNL Adobe Workfront Fusion] HTTP &gt; OAuth 2.0 요청 모듈 만들기
author: Becky
draft: Probably
feature: Workfront Fusion
exl-id: adae390d-8b9e-4dab-8551-605e50af5a1e
source-git-commit: f783e3033a67b4702e4e2d80214cbb0c4591b922
workflow-type: tm+mt
source-wordcount: '610'
ht-degree: 0%

---

# 호출[!UICONTROL  MS Graph REST API] 를 통해 [!DNL Adobe Workfront Fusion] [!UICONTROL HTTP] > [!UICONTROL OAuth 2.0 요청] 모듈

많음 [!DNL Microsoft] 웹 서비스는 [!DNL Microsoft Graph API]. 이 문서에서는 다음을 사용하여 해당 API에 대한 연결을 만드는 방법을 설명합니다. [!DNL Workfront Fusion] [!DNL HTTP] > [!UICONTROL OAuth 2.0 요청] 모듈.

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
   <td role="rowheader">[!DNL Adobe Workfront Fusion] 라이센스**</td> 
   <td>
   <p>현재 라이선스 요구 사항: 아니요 [!DNL Workfront Fusion] 라이센스 요구 사항.</p>
   <p>또는</p>
   <p>기존 라이선스 요구 사항: [!UICONTROL [!DNL Workfront Fusion] for Work Automation and Integration] </p>
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader">제품</td> 
   <td>
   <p>현재 제품 요구 사항: [!UICONTROL Select] 또는 [!UICONTROL Prime]이 있는 경우 [!DNL Adobe Workfront] 플랜, 조직은 다음을 구매해야 합니다. [!DNL Adobe Workfront Fusion] 뿐만 아니라 [!DNL Adobe Workfront] 이 문서에 설명된 기능을 사용하십시오. [!DNL Workfront Fusion] [!UICONTROL Ultimate]에 포함되어 있습니다. [!DNL Workfront] 계획.</p>
   <p>또는</p>
   <p>레거시 제품 요구 사항: 조직에서 구매해야 함 [!DNL Adobe Workfront Fusion] 뿐만 아니라 [!DNL Adobe Workfront] 이 문서에 설명된 기능을 사용하십시오.</p>
   </td> 
  </tr>
 </tbody> 
</table>

보유 중인 플랜, 라이선스 유형 또는 액세스 권한을 알아보려면 [!DNL Workfront] 관리자.

다음에 대한 정보: [!DNL Adobe Workfront Fusion] 라이센스, 참조 [[!DNL Adobe Workfront Fusion] 라이선스](../../workfront-fusion/get-started/license-automation-vs-integration.md).

## 등록 [!DNL Workfront Fusion] 다음에서 [!DNL Microsoft Application Registration Portal]

에 대한 연결을 만들려면 [!DNL Microsoft Graph REST API], 먼저 등록해야 합니다. [!DNL Adobe Workfront Fusion].

1. 에 설명된 대로 새 애플리케이션 등록 시작 [앱 등록](https://docs.microsoft.com/en-us/graph/auth-register-app-v2) 다음에서 [!DNL Microsoft] 설명서를 참조하십시오.

   등록의 일부로, [!DNL Microsoft] 를 사용하려면 다음 정보가 필요합니다.

   <table style="table-layout:auto">
      <tr>
        <td>[!UICONTROL Application name]</td>
        <td>응용 프로그램 이름 입력(예: "내") [!DNL Workfront Fusion] 응용 프로그램."</td>
      </tr>
      <tr>
        <td>[!UICONTROL 리디렉션 URL]</td>
        <td><code>https://app.workfrontfusion.com/oauth/cb/oauth2</code></td>
      </tr>
    </table>

1. 앱 등록을 완료하면 다음을 참고하십시오. [!UICONTROL 애플리케이션 ID].

   >[!IMPORTANT]
   >
   >에서 연결을 설정하려면 애플리케이션 ID가 필요합니다. [!DNL Workfront Fusion].

1. 생성 [!UICONTROL 애플리케이션 암호]. 이 비밀을 메모해 두십시오.

   자세한 내용은 [앱 등록](https://docs.microsoft.com/en-us/graph/auth-register-app-v2) 다음에서 [!DNL Microsoft] 설명서를 참조하십시오.

   >[!IMPORTANT]
   >
   >다음이 필요합니다. [!UICONTROL 애플리케이션 암호] 에서 연결을 설정하려면 [!DNL Workfront Fusion].

1. 애플리케이션에 대한 권한을 구성합니다.

   이러한 필드를 찾고 구성하는 방법에 대한 자세한 내용은 의 &quot;Microsoft 그래프에 대한 권한 구성&quot; 섹션을 참조하십시오. [사용자 없이 액세스](https://docs.microsoft.com/en-us/graph/auth-v2-service) 다음에서 [!UICONTROL Microsoft] 설명서를 참조하십시오.

   <table style="table-layout:auto">
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">[!UICONTROL 애플리케이션에 필요한 권한 유형은 무엇입니까?]</td> 
      <td>선택 <code>[!UICONTROL Delegated permissions]</code>.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL 권한 선택]</td> 
      <td> <p>다음 권한을 선택합니다.</p> 
       <ul> 
        <li> <p><code>offline_access</code> </p> </li> 
        <li> <p><code>openid</code> </p> </li> 
        <li> <p>통합에 필요한 기타 모든 권한 (예: <code>User.Read</code>)</p> </li> 
       </ul> <p>중요:에서 연결을 설정하려면 선택한 권한이 필요합니다. [!DNL Workfront Fusion].</p> </td> 
     </tr> 
    </tbody> 
   </table>

1. 다음으로 진행 [구성 [!DNL MS Graph API] 의 연결 [!DNL Workfront Fusion]](#configure-your-ms-graph-api-connection-in-workfront-fusion).

## 구성 [!DNL MS Graph API] 의 연결 [!DNL Workfront Fusion]

등록 후 [!DNL Workfront Fusion] 에서 논의된대로 [등록 [!DNL Workfront Fusion] 다음에서 [!DNL Microsoft Application Registration Portal]](#register-workfront-fusion-in-the-microsoft-application-registration-portal)에서 연결을 구성할 수 있습니다. [!UICONTROL HTTP] >[!UICONTROL Oauth 2.0 만들기] 모듈 요청.

1. 추가 [!UICONTROL HTTP] >[!UICONTROL OAuth 2.0 호출] 을 시나리오에 연결합니다.
1. 클릭 **[!UICONTROL 추가]** 다음 옆에 [!UICONTROL 연결] 필드.
1. 연결 필드를 다음과 같이 구성합니다.

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
      <td role="rowheader">[!UICONTROL 권한 부여 URI]</td> 
      <td><code>https://login.microsoftonline.com/common/oauth2/v2.0/authorize</code> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL 토큰 URI]</td> 
      <td><code>https://login.microsoftonline.com/common/oauth2/v2.0/token</code> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL 범위]</td> 
      <td> <p>의 4단계에서 선택한 권한을 입력하십시오. <a href="#register-workfront-fusion-in-the-microsoft-application-registration-portal" class="MCXref xref">등록 [!DNL Workfront Fusion] 다음에서 [!DNL Microsoft Application Registration Portal]</a>.</p> <p>각 범위에 대해 <b>[!UICONTROL 추가]</b> 을 누르고 권한을 입력합니다.</p> <p>예: <code>offline_access</code>.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL 범위 구분 기호]</td> 
      <td><code>SPACE</code> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL 클라이언트 ID]</td> 
      <td>의 2단계에서 [!UICONTROL Application ID]를 입력하십시오. <a href="#register-workfront-fusion-in-the-microsoft-application-registration-portal" class="MCXref xref">등록 [!DNL Workfront Fusion] 다음에서 [!DNL Microsoft Application Registration Portal]</a>.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL 클라이언트 암호]</td> 
      <td>의 2단계에서 생성한 [!UICONTROL 응용 프로그램 암호]를 입력합니다. <a href="#register-workfront-fusion-in-the-microsoft-application-registration-portal" class="MCXref xref">등록 [!DNL Workfront Fusion] 다음에서 [!DNL Microsoft Application Registration Portal]</a>.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL Authorize parameters]</td> 
      <td> <p>다음 승인 매개 변수를 추가합니다.</p> 
       <ul> 
        <li> <p>[!UICONTROL 키]:<code> response_mode</code> [!UICONTROL 값]: <code>query</code></p> </li> 
        <li> <p>[!UICONTROL 키]: <code>prompt </code>[!UICONTROL 값]: <code>consent</code></p> </li> 
       </ul> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL 액세스 토큰 매개 변수]</td> 
      <td>이 필드에는 아무 것도 입력할 필요가 없습니다.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL 토큰 매개 변수 새로 고침]</td> 
      <td> 
       <ol> 
        <li value="1"> <p>클릭 <b>[!UICONTROL 추가]</b>.</p> </li> 
        <li value="2"> <p>다음에서 <b>[!UICONTROL 키]</b> 필드, 입력 <code>scope</code>.</p> </li> 
        <li value="3"> <p>다음에서 <b>[!UICONTROL 값]</b> 필드에 범위 필드에 입력한 모든 [!UICONTROL 범위]를 공백으로 구분하여 입력합니다.</p> <p>예: <code>offline_access openid User.Read</code></p> </li> 
       </ol> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL 사용자 지정 헤더]</td> 
      <td>이 필드에는 아무 것도 입력할 필요가 없습니다.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL 토큰 배치]</td> 
      <td><code>[!UICONTROL In the header]</code> </td> 
     </tr> 
    </tbody> 
   </table>

1. 클릭 **[!UICONTROL 계속]**.
1. 표시되는 창에서 을 클릭합니다. **[!UICONTROL Accept]** 를 클릭하여 연결을 완료하고 모듈로 돌아갑니다.
