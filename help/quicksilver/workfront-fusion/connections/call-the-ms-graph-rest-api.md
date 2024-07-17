---
title: ' [!DNL Adobe Workfront Fusion] HTTP &gt; OAuth 2.0 요청 모듈 만들기 를 통해 MS Graph REST API를 호출합니다.'
description: ' [!DNL Adobe Workfront Fusion] HTTP &gt; OAuth 2.0 요청 모듈 만들기 를 통해 MS Graph REST API를 호출합니다.'
author: Becky
feature: Workfront Fusion
exl-id: adae390d-8b9e-4dab-8551-605e50af5a1e
source-git-commit: b90343eab40e91c6f5cddeaa960ce9c9c97b1d29
workflow-type: tm+mt
source-wordcount: '571'
ht-degree: 1%

---

# [!DNL Adobe Workfront Fusion] [!UICONTROL HTTP] > [!UICONTROL OAuth 2.0 요청 만들기] 모듈을 통해 [!UICONTROL  MS Graph REST API]를 호출합니다

<!-- Audited: 3/2024-->

[!DNL Microsoft Graph API]을(를) 통해 많은 [!DNL Microsoft] 웹 서비스에 액세스할 수 있습니다. [!DNL Workfront Fusion] [!DNL HTTP] > [!UICONTROL OAuth 2.0 요청 만들기] 모듈을 사용하여 [!DNL Microsoft Graph API]에 연결할 수 있습니다.

## 액세스 요구 사항

이 문서의 기능을 사용하려면 다음 액세스 권한이 있어야 합니다.

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] 플랜</td> 
   <td> <p>임의</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader">[!DNL Adobe Workfront] 라이센스</td> 
   <td> <p>새로운 기능: [!UICONTROL Standard]</p><p>또는</p><p>현재: [!UICONTROL Work] 이상</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront Fusion] 라이센스**</td> 
   <td>
   <p>현재: [!DNL Workfront Fusion] 라이선스 요구 사항이 없습니다.</p>
   <p>또는</p>
   <p>레거시: 모두 </p>
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader">제품</td> 
   <td>
   <p>신규:</p> <ul><li>[!UICONTROL Select] 또는 [!UICONTROL Prime] [!DNL Workfront] 플랜: 조직에서 [!DNL Adobe Workfront Fusion]을(를) 구매해야 합니다.</li><li>[!UICONTROL Ultimate] [!DNL Workfront] 계획: [!DNL Workfront Fusion]이(가) 포함되어 있습니다.</li></ul>
   <p>또는</p>
   <p>현재: 조직에서 [!DNL Adobe Workfront Fusion]을(를) 구매해야 합니다.</p>
   </td> 
  </tr>
 </tbody> 
</table>

이 표의 정보에 대한 자세한 내용은 [Workfront 설명서의 액세스 요구 사항](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)을 참조하십시오.

[!DNL Adobe Workfront Fusion] 라이선스에 대한 자세한 내용은 [[!DNL Adobe Workfront Fusion] 라이선스](../../workfront-fusion/get-started/license-automation-vs-integration.md)를 참조하세요.

## [!DNL Microsoft Application Registration Portal]에서 [!DNL Workfront Fusion] 등록

[!DNL Microsoft Graph REST API]에 대한 연결을 만들려면 먼저 [!DNL Adobe Workfront Fusion]을(를) 등록해야 합니다.

1. [!DNL Microsoft] 설명서의 [앱 등록](https://docs.microsoft.com/en-us/graph/auth-register-app-v2)에 설명된 대로 새 응용 프로그램 등록을 시작합니다.

   등록의 일부로 [!DNL Microsoft]에는 다음 정보가 필요합니다.

   <table style="table-layout:auto">
      <tr>
        <td>[!UICONTROL Application name]</td>
        <td>응용 프로그램 이름(예: "내 [!DNL Workfront Fusion] 응용 프로그램")을 입력하십시오.</td>
      </tr>
      <tr>
        <td>[!UICONTROL 리디렉션 URL]</td>
        <td><code>https://app.workfrontfusion.com/oauth/cb/oauth2</code></td>
      </tr>
    </table>

1. 앱 등록을 완료하면 [!UICONTROL 응용 프로그램 ID]를 메모하세요.

   >[!IMPORTANT]
   >
   >[!DNL Workfront Fusion]에서 연결을 설정하려면 응용 프로그램 ID가 필요합니다.

1. [!UICONTROL 응용 프로그램 암호]를 생성합니다. 이 비밀을 메모해 두십시오.

   지침은 [!DNL Microsoft] 설명서의 [앱 등록](https://docs.microsoft.com/en-us/graph/auth-register-app-v2)을 참조하십시오.

   >[!IMPORTANT]
   >
   >[!DNL Workfront Fusion]에서 연결을 설정하려면 [!UICONTROL 응용 프로그램 암호]가 필요합니다.

1. 애플리케이션에 대한 권한을 구성합니다.

   이러한 필드를 찾고 구성하는 방법에 대한 자세한 내용은 [!UICONTROL Microsoft] 설명서의 [사용자 없이 액세스 받기](https://docs.microsoft.com/en-us/graph/auth-v2-service)에서 &quot;Microsoft 그래프에 대한 권한 구성&quot; 섹션을 참조하십시오.

   <table style="table-layout:auto">
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">[!UICONTROL 애플리케이션에 필요한 권한 유형은 무엇입니까?]</td> 
      <td><code>[!UICONTROL Delegated permissions]</code>을(를) 선택합니다.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL 권한 선택]</td> 
      <td> <p>다음 권한을 선택합니다.</p> 
       <ul> 
        <li> <p><code>offline_access</code> </p> </li> 
        <li> <p><code>openid</code> </p> </li> 
        <li> <p>통합에 필요한 다른 모든 권한(예: <code>User.Read</code>)</p> </li> 
       </ul> <p><b>중요</b>: [!DNL Workfront Fusion]에서 연결을 설정하려면 선택한 권한이 필요합니다.</p> </td> 
     </tr> 
    </tbody> 
   </table>

1. [연결 구성 [!DNL Workfront Fusion]](#configure-your-ms-graph-api-connection-in-workfront-fusion)로 진행합니다. [!DNL MS Graph API] 

## [!DNL Workfront Fusion]에서 [!DNL MS Graph API] 연결 구성

 [!DNL Microsoft Application Registration Portal]](#register-workfront-fusion-in-the-microsoft-application-registration-portal)의 [등록 [!DNL Workfront Fusion] 에서 설명한 대로 [!DNL Workfront Fusion]을(를) 등록한 후 [!UICONTROL HTTP] > [!UICONTROL Oauth 2.0] 요청 모듈에서 연결을 구성할 수 있습니다.

1. 시나리오에 [!UICONTROL HTTP] > [!UICONTROL OAuth 2.0 호출 만들기] 모듈을 추가합니다.
1. [!UICONTROL 연결] 필드 옆에 있는 **[!UICONTROL 추가]**&#x200B;를 클릭합니다.
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
      <td> <p><a href="#register-workfront-fusion-in-the-microsoft-application-registration-portal" class="MCXref xref">등록 [!DNL Workfront Fusion]의 4단계에서 선택한 권한을 [!DNL Microsoft Application Registration Portal]</a>에 입력하십시오.</p> <p>각 범위에 대해 <b>[!UICONTROL 추가]</b>를 클릭하고 권한을 입력하십시오.</p> <p>예: <code>offline_access</code></p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL 범위 구분 기호]</td> 
      <td><code>SPACE</code> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL 클라이언트 ID]</td> 
      <td><a href="#register-workfront-fusion-in-the-microsoft-application-registration-portal" class="MCXref xref">[!DNL Microsoft Application Registration Portal]</a>에 [!DNL Workfront Fusion] 등록의 2단계에서 [!UICONTROL 응용 프로그램 ID]를 입력하십시오.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL 클라이언트 암호]</td> 
      <td><a href="#register-workfront-fusion-in-the-microsoft-application-registration-portal" class="MCXref xref">등록 [!DNL Workfront Fusion]의 [!DNL Microsoft Application Registration Portal]</a>에서 3단계에서 생성한 [!UICONTROL 응용 프로그램 암호를 입력하십시오.</td> 
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
        <li value="1"> <p><b>[!UICONTROL 추가]</b>를 클릭합니다.</p> </li> 
        <li value="2"> <p><b>[!UICONTROL 키]</b> 필드에 <code>scope</code>을(를) 입력합니다.</p> </li> 
        <li value="3"> <p><b>[!UICONTROL 값]</b> 필드에 범위 필드에 입력한 모든 [!UICONTROL 범위]를 공백으로 구분하여 입력합니다.</p> <p>예: <code>offline_access openid User.Read</code></p> </li> 
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

1. **[!UICONTROL 계속]**&#x200B;을 클릭합니다.
1. 표시되는 창에서 **[!UICONTROL 수락]**&#x200B;을 클릭하여 연결을 완료하고 모듈로 돌아갑니다.
