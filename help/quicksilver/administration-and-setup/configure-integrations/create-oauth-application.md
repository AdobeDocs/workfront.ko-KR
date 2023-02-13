---
title: 용 OAuth2 애플리케이션 만들기 [!DNL Workfront] 통합
user-type: administrator
product-area: system-administration;workfront-integrations
navigation-topic: administrator-integrations
description: '로서의 [!DNL Adobe Workfront] 관리자는 [!DNL Workfront]: 다른 애플리케이션에서 Workfront에 액세스할 수 있습니다. 그런 다음 사용자는 다른 애플리케이션에 자신의 Workfront 데이터에 액세스할 수 있는 권한을 부여할 수 있습니다. 이러한 방식으로 사내 애플리케이션을 포함하여 원하는 애플리케이션과 Workfront을 통합할 수 있습니다.'
feature: System Setup and Administration, Workfront Integrations and Apps
role: Admin
exl-id: e13c7dda-8945-47ad-b6d3-4d6a62b368f5
source-git-commit: f7e3182776e6b62103cd755b2fbd5057efc95394
workflow-type: tm+mt
source-wordcount: '1917'
ht-degree: 6%

---

# 용 OAuth2 애플리케이션 만들기 [!DNL Workfront] 통합

로서의 [!DNL Adobe Workfront] 관리자는 [!DNL Workfront]: 다른 응용 프로그램이 액세스할 수 있도록 합니다 [!DNL Workfront]. 그런 다음 사용자는 다른 응용 프로그램에 액세스하여 액세스할 수 있는 권한을 부여할 수 있습니다 [!DNL Workfront] 데이터. 이러한 방식으로 자체 내부 애플리케이션을 포함하여 원하는 애플리케이션과 통합할 수 있습니다.

를 만들 때 [!UICONTROL OAuth2] 응용 프로그램에서 클라이언트 ID와 클라이언트 암호를 생성합니다. 그런 다음 사용자는 API 호출에서 클라이언트 ID를 사용하여 만든 애플리케이션과 통합할 수 있습니다.

>[!NOTE]
>
>OAuth2 컨텍스트에서 &quot;앱 만들기&quot;는 앱과 서버 간에 이러한 종류의 액세스 링크를 만드는 프로세스를 말합니다 [!DNL Workfront].

* 사용자 자격 증명(인증 코드 흐름)과 함께 OAuth2 응용 프로그램을 구성하고 사용하는 방법에 대한 지침은 [인증 코드 흐름을 사용하여 조직의 사용자 지정 OAuth 2 애플리케이션을 구성하고 사용합니다](../../wf-api/api/oauth-app-code-token-flow.md).
* 서버 인증(JWT 흐름)을 사용하여 OAuth2 애플리케이션을 구성하고 사용하는 방법에 대한 지침은 [JWT 흐름을 사용하여 조직의 사용자 지정 OAuth 2 애플리케이션을 구성하고 사용합니다](../../wf-api/api/oauth-app-jwt-flow.md).
* PKCE를 사용하여 OAuth2 응용 프로그램을 구성하고 사용하는 방법에 대한 지침은 [PKCE 플로우를 사용하여 조직의 사용자 지정 OAuth 2 응용 프로그램 구성 및 사용](../../wf-api/api/oauth-app-pkce-flow.md).

## 액세스 요구 사항

이 문서의 절차를 수행하려면 다음 액세스 권한이 있어야 합니다.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] 플랜*</td> 
   <td> <p>[!UICONTROL Pro] 이상</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] 라이센스*</td> 
   <td>[!UICONTROL 계획]</td> 
  </tr> 
  <tr> 
   <td role="rowheader">액세스 수준 구성*</td> 
   <td> 넌 [!DNL Workfront] 관리자 </td> 
  </tr> 
 </tbody> 
</table>

&#42;어떤 계획, 라이센스 유형 또는 액세스 권한을 보유하고 있는지 확인하려면 [!DNL Workfront] 관리자

## OAuth2 개요

애플리케이션이 [!DNL Workfront]. 정보를 요청하는 응용 프로그램을 클라이언트라고 합니다. 이 예제에서 클라이언트 이름은 ClientApp입니다. ClientApp은 특정 사용자의 정보에 액세스해야 하므로 액세스해야 합니다 [!DNL Workfront] 해당 사용자. 사용자가 ClientApp에 사용자 이름과 암호를 제공하면 ClientApp은 사용자가 액세스할 수 있는 모든 데이터에 액세스할 수 있습니다. ClientApp에는 소규모 특정 정보 세트만 필요하므로 이는 보안 위험입니다.

ClientApp용 OAuth2 앱을 만들 때 기본적으로 [!DNL Workfront] ClientApp이 [!DNL Workfront]그러나 ClientApp 계정이 액세스하는 사용자에게 액세스 권한을 제공하는 경우에만 해당됩니다.

## OAuth2 애플리케이션 만들기

OAuth2 애플리케이션을 만들 때 통합 요구 사항에 가장 적합한 애플리케이션 유형을 선택합니다.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th>애플리케이션 유형</th> 
   <th>가장 적합한 대상</th> 
   <th>인증 방법</th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <p>머신 투 머신 애플리케이션</p> </td> 
   <td> <p>서버에서 실행 중인 CLI, 데몬 또는 스크립트에 가장 적합합니다</p> <p>예:</p> 
    <ul> 
     <li> <p>[!DNL Shell] </p> </li> 
     <li> <p>[!DNL Python]</p> </li> 
    </ul> </td> 
   <td> <p>JSON 웹 토큰을 통한 공개/비공개 키 쌍 인코딩으로 인증.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>단일 페이지 웹 애플리케이션</p> </td> 
   <td> <p>모바일 또는 단일 페이지 웹 애플리케이션에 가장 적합합니다</p> <p>예:</p> 
    <ul> 
     <li> <p>[!DNL Javascript]</p> </li> 
     <li> <p>[!DNL Angular]</p> </li> 
     <li> <p>[!DNL React]</p> </li> 
     <li> <p>[!DNL Vue]</p> </li> 
    </ul> </td> 
   <td> <p>PKCE(Proof Key for Code Exchange)를 사용하여 OAuth 2.0 인증 코드 흐름을 통한 인증.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>웹 애플리케이션</p> </td> 
   <td> <p>서버에서 자격 증명과 토큰을 처리하는 서버측 애플리케이션에 가장 적합합니다</p> <p>예:</p> 
    <ul> 
     <li> <p>[!DNL Go]</p> </li> 
     <li> <p>[!DNL Java]</p> </li> 
     <li> <p>[!DNL ASP.Net]</p> </li> 
     <li> <p>[!DNL Node.js]</p> </li> 
     <li> <p>[!DNL PHP]</p> </li> 
    </ul> </td> 
   <td> <p>OAuth 2.0 인증 코드 흐름을 통한 인증.</p> </td> 
  </tr> 
 </tbody> 
</table>

>[!NOTE]
>
>한 번에 최대 10개의 OAuth2 애플리케이션을 가질 수 있습니다.

* [서버 인증(JWT 흐름)을 사용하여 OAuth2 응용 프로그램을 만듭니다](#create-an-oauth2-application-using-server-authentication-jwt-flow)
* [사용자 자격 증명(인증 코드 흐름)을 사용하여 OAuth2 응용 프로그램을 만듭니다](#create-an-oauth2-application-using-user-credentials-authorization-code-flow)
* [PKCE를 사용하여 OAuth2 단일 페이지 웹 응용 프로그램 만들기](#create-an-oauth2-single-page-web-application-using-pkce)

### 서버 인증(JWT 흐름)을 사용하여 OAuth2 응용 프로그램을 만듭니다 {#create-an-oauth2-application-using-server-authentication-jwt-flow}

1. 을(를) 클릭합니다. **[!UICONTROL 기본 메뉴]** 아이콘 ![](assets/main-menu-icon.png) 의 오른쪽 위 모서리에서 [!DNL Adobe Workfront]를 클릭한 다음 **[!UICONTROL 설정]** ![](assets/gear-icon-settings.png).

1. 왼쪽 탐색 패널에서 **[!UICONTROL 시스템]**&#x200B;를 선택하고 을 선택합니다. **[!UICONTROL OAuth 애플리케이션]**.
1. 클릭 **[!UICONTROL 앱 통합 만들기]**.
1. 표시되는 창에서 **[!UICONTROL 서버 인증]**.
1. 새 응용 프로그램의 이름을 입력합니다(예: &quot;).[!DNL Workfront] ClientApp용.&quot;
1. Click **[!UICONTROL Create]**.
1. 새 앱의 필드를 채웁니다.

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">[!UICONTROL Client ID]</td> 
      <td> <p>이 필드는 자동으로 생성됩니다.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL Client Secret]</td> 
      <td> <p>이 필드는 자동으로 생성됩니다</p> <p><b>중요 사항</b>:  <p>이 페이지를 닫기 전에 이 필드의 내용을 다른 보안 파일에 복사합니다. 이 비밀 키를 다시 볼 수 없습니다.</p> <p>이 키를 잃어버리면 삭제하고 새 클라이언트 암호를 만듭니다.</p> 
        <ol> 
         <li value="1"> <p>을(를) 클릭합니다. <b>[!UICONTROL Delete]</b> 아이콘 <img src="assets/delete.png"> 현재 클라이언트 암호를 삭제합니다.</p> </li> 
         <li value="2"> <p>클릭 <b>[!UICONTROL 클라이언트 암호 추가]</b> 새 클라이언트 암호를 생성합니다.</p> </li> 
        </ol> </p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL 공개 키]</td> 
      <td> <p>서버 간 앱에서는 인증에 공개 및 개인 키를 사용합니다. 다음 중 하나를 수행하십시오.</p> 
       <ul> 
        <li> <p>클릭 <b>[!UICONTROL 공개 키 추가]</b> 다른 응용 프로그램의 공개 키를 입력합니다.</p> </li> 
        <li> <p>클릭 <b>[!UICONTROL 공용/개인 키 쌍 생성]</b>그런 다음 공개 키를 다른 애플리케이션과 공유합니다.</p> </li> 
       </ul> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL Name]</td> 
      <td>앱을 제공한 것과 동일한 이름입니다. 이 필드는 비워 둘 수 없습니다.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL Description]</td> 
      <td>통합에 대한 설명을 입력합니다.</td> 
     </tr> 
    </tbody> 
   </table>

1. **[!UICONTROL 저장]**&#x200B;을 클릭합니다.

사용자 자격 증명(인증 코드 흐름)과 함께 OAuth2 응용 프로그램을 구성하고 사용하는 방법에 대한 지침은 [JWT 흐름을 사용하여 조직의 사용자 지정 OAuth 2 애플리케이션을 구성하고 사용합니다](../../wf-api/api/oauth-app-jwt-flow.md).

### 사용자 자격 증명(인증 코드 흐름)을 사용하여 OAuth2 응용 프로그램을 만듭니다 {#create-an-oauth2-application-using-user-credentials-authorization-code-flow}

1. 을(를) 클릭합니다. **[!UICONTROL 기본 메뉴]** 아이콘 ![](assets/main-menu-icon.png) 의 오른쪽 위 모서리에서 [!DNL Adobe Workfront]를 클릭한 다음 **[!UICONTROL 설정]** ![](assets/gear-icon-settings.png).
1. 왼쪽 탐색 패널에서 **[!UICONTROL 시스템]**&#x200B;를 선택하고 을 선택합니다. **[!UICONTROL OAuth 애플리케이션]**.
1. 클릭 **[!UICONTROL 앱 통합 만들기]**.
1. 표시되는 창에서 **[!UICONTROL 사용자 인증]**.
1. 새 OAuth2 응용 프로그램의 이름(예: &quot;)을 입력합니다.[!DNL Workfront] ClientApp용.&quot;
1. Click **[!UICONTROL Create]**.
1. 새 앱의 필드를 채웁니다.

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">[!UICONTROL Client ID]</td> 
      <td> <p>이 필드는 자동으로 생성됩니다.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL Client Secret]</td> 
      <td> <p>이 필드는 자동으로 생성됩니다</p> <p><b>중요 사항</b>:  <p>이 페이지를 닫기 전에 이 필드의 내용을 다른 보안 파일에 복사합니다. 이 비밀 키를 다시 볼 수 없습니다.</p> <p>이 키를 잃어버리면 삭제하고 새 클라이언트 암호를 만듭니다.</p> 
        <ol> 
         <li value="1"> <p>을(를) 클릭합니다. <b>[!UICONTROL Delete]</b> 아이콘 <img src="assets/delete.png"> 현재 클라이언트 암호를 삭제합니다.</p> </li> 
         <li value="2"> <p>클릭 <b>[!UICONTROL 클라이언트 암호 추가]</b> 새 클라이언트 암호를 생성합니다.</p> </li> 
        </ol> </p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL 리디렉션 URL]</td> 
      <td>사용자가 다음을 인증하면 이 경로로 리디렉션됩니다. [!DNL Workfront].</td> 
     </tr> 
     <tr data-mc-conditions=""> 
      <td role="rowheader">[!UICONTROL 새로 고침 토큰 회전]</td> 
      <td>새로 고침 토큰을 사용할 때마다 새 새로 고침 토큰을 발급하려면 이 옵션을 활성화합니다. 애플리케이션은 매번 새로 고침 후에 새 새로 고침 토큰을 저장해야 합니다.</td> 
     </tr> 
     <tr data-mc-conditions=""> 
      <td role="rowheader">[!UICONTROL 절대 새로 고침 토큰 만료]</td> 
      <td> <p>새로 고침 토큰이 만료되기 전에 존재할 시간을 선택합니다. 만료되면 사용자가 통합에 다시 로그인해야 합니다. 새로 고침 토큰이 만료되지 않도록 하려면 "[!UICONTROL 만료 없음]"을 선택하십시오.</p> </td> 
     </tr> 
     <tr data-mc-conditions=""> 
      <td role="rowheader">토큰 만료 새로 고침 중지</td> 
      <td> <p>사용자가 시스템에서 활성 상태가 아닌 경우 새로 고침 토큰이 만료되는 이후의 시간을 선택합니다. </p> <p>예를 들어 비활성 새로 고침 토큰 만료가 6개월이고 사용자가 6개월 동안 로그인하지 않으면 절대 새로 고침 토큰 만료가 더 오래 설정될 수 있어도 새로 고침 토큰이 만료됩니다.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL 로고]</td> 
      <td>로고를 추가하여 이 앱을 더 쉽게 식별할 수 있습니다. </td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL Name]</td> 
      <td>앱을 제공한 것과 동일한 이름입니다. 이 필드는 비워 둘 수 없습니다.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL Description]</td> 
      <td>통합에 대한 설명을 입력합니다.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL 앱 설명 URL]</td> 
      <td>통합에 대한 자세한 정보가 있는 "정보" 페이지 또는 페이지에 대한 링크일 수 있습니다.</td> 
     </tr> 
    </tbody> 
   </table>

1. **[!UICONTROL 저장]**&#x200B;을 클릭합니다.

사용자 자격 증명(인증 코드 흐름)과 함께 OAuth2 응용 프로그램을 구성하고 사용하는 방법에 대한 지침은 [인증 코드 흐름을 사용하여 조직의 사용자 지정 OAuth 2 애플리케이션을 구성하고 사용합니다](../../wf-api/api/oauth-app-code-token-flow.md).

### PKCE를 사용하여 OAuth2 단일 페이지 웹 응용 프로그램 만들기 {#create-an-oauth2-single-page-web-application-using-pkce}

1. 을(를) 클릭합니다. **[!UICONTROL 기본 메뉴]** 아이콘 ![](assets/main-menu-icon.png) 의 오른쪽 위 모서리에서 [!DNL Adobe Workfront]를 클릭한 다음 **[!UICONTROL 설정]** ![](assets/gear-icon-settings.png).
1. 왼쪽 탐색 패널에서 **[!UICONTROL 시스템]**&#x200B;를 선택하고 을 선택합니다. **[!UICONTROL OAuth 애플리케이션]**.
1. 클릭 **[!UICONTROL 앱 통합 만들기]**.
1. 표시되는 창에서 **[!UICONTROL 단일 페이지 웹 애플리케이션]**.
1. 새 이름을 입력합니다 [!UICONTROL OAuth2] 애플리케이션(예: &quot;)[!DNL Workfront] ClientApp용.&quot;
1. Click **[!UICONTROL Create]**.
1. 새 앱의 필드를 채웁니다.

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">[!UICONTROL Client ID]</td> 
      <td> <p>이 필드는 자동으로 생성됩니다.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL 리디렉션 URL]</td> 
      <td>사용자가 Workfront에 대해 인증되면 이 경로로 리디렉션됩니다.</td> 
     </tr> 
     <tr data-mc-conditions=""> 
      <td role="rowheader">[!UICONTROL 새로 고침 토큰 회전]</td> 
      <td>새로 고침 토큰을 사용할 때마다 새 새로 고침 토큰을 발급하려면 이 옵션을 활성화합니다. 애플리케이션은 매번 새로 고침 후에 새 새로 고침 토큰을 저장해야 합니다.</td> 
     </tr> 
     <tr data-mc-conditions=""> 
      <td role="rowheader">[!UICONTROL 절대 새로 고침 토큰 만료]</td> 
      <td> <p>새로 고침 토큰이 만료되기 전에 존재할 시간을 선택합니다. 만료되면 사용자가 통합에 다시 로그인해야 합니다. 새로 고침 토큰이 만료되지 않도록 하려면 "[!UICONTROL 만료 없음]"을 선택하십시오.</p> </td> 
     </tr> 
     <tr data-mc-conditions=""> 
      <td role="rowheader">[!UICONTROL 비활성 새로 고침 토큰 만료]</td> 
      <td> <p>사용자가 시스템에서 활성 상태가 아닌 경우 새로 고침 토큰이 만료되는 이후의 시간을 선택합니다. </p> <p>예를 들어 비활성 새로 고침 토큰 만료가 6개월이고 사용자가 6개월 동안 로그인하지 않으면 절대 새로 고침 토큰 만료가 더 오래 설정될 수 있어도 새로 고침 토큰이 만료됩니다.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL 로고]</td> 
      <td>로고를 추가하여 이 앱을 더 쉽게 식별할 수 있습니다. </td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL Name]</td> 
      <td>앱을 제공한 것과 동일한 이름입니다. 이 필드는 비워 둘 수 없습니다.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL Description]</td> 
      <td>통합에 대한 설명을 입력합니다.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL 앱 설명 URL]</td> 
      <td>통합에 대한 자세한 정보가 있는 "정보" 페이지 또는 페이지에 대한 링크일 수 있습니다.</td> 
     </tr> 
    </tbody> 
   </table>

1. **[!UICONTROL 저장]**&#x200B;을 클릭합니다.

## 만든 OAuth2 애플리케이션 구성 및 사용

생성된 OAuth2 애플리케이션을 추가로 구성 및 사용하려면 API 호출을 비롯한 일부 기술 지식이 필요합니다.

* 사용자 자격 증명(인증 코드 흐름)과 함께 OAuth2 응용 프로그램을 구성하고 사용하는 방법에 대한 지침은 [인증 코드 흐름을 사용하여 조직의 사용자 지정 OAuth 2 애플리케이션을 구성하고 사용합니다](../../wf-api/api/oauth-app-code-token-flow.md).
* 서버 인증(JWT 흐름)을 사용하여 OAuth2 애플리케이션을 구성하고 사용하는 방법에 대한 지침은 [JWT 흐름을 사용하여 조직의 사용자 지정 OAuth 2 애플리케이션을 구성하고 사용합니다](../../wf-api/api/oauth-app-jwt-flow.md).
* PKCE를 사용하여 OAuth2 응용 프로그램을 구성하고 사용하는 방법에 대한 지침은 [PKCE 플로우를 사용하여 조직의 사용자 지정 OAuth 2 응용 프로그램 구성 및 사용](../../wf-api/api/oauth-app-pkce-flow.md).

## 인증 코드 흐름을 위한 OAuth2 프로세스

>[!NOTE]
>
>사용자가 [!UICONTROL OAuth2] api를 통해 애플리케이션을 생성합니다. 이 섹션에서는 기능을 일반적으로 설명하며, 정보용으로만 제공됩니다.
>
>특정 API 호출을 포함하여 OAuth2 애플리케이션 사용에 대한 특정 지침은 [인증 코드 흐름을 사용하여 조직의 사용자 지정 OAuth 2 애플리케이션을 구성하고 사용합니다](../../wf-api/api/oauth-app-code-token-flow.md).

### 인증 코드 및 액세스 토큰으로 인증 {#authorizing-with-an-authorization-code-and-access-token}

1. ClientApp에는 [!DNL Workfront]로 설정되면, [!DNL Workfront] API `/authorize` 엔드포인트. 요청에는 다음이 포함됩니다 [!UICONTROL response_type] `code`: 요청이 인증 코드를 반환해야 함을 나타냅니다.
1. 이 트리거 [!DNL Workfront] 사용자에게 인증 프롬프트를 보내려면 사용자는 프롬프트에 자격 증명을 입력할 수 있으며, [!DNL Workfront] 클라이언트 앱과 통신할 수 있는 권한. 사용자가 이미 로그인한 경우 [!DNL Workfront]로 지정하는 경우 이 단계를 건너뛸 수 있습니다.
1. 다음 [!DNL Workfront] API가 ClientApp에 인증 코드를 전송합니다.
1. ClientApp이 요청에서 다음 정보를 [!DNL Workfront] API `/token`   endpoint:

   * 3단계에서 ClientApp으로 전송된 인증 코드입니다. 사용자 권한의 특정 인스턴스를 식별합니다.
   * 에서 ClientApp OAuth2 앱을 설정할 때 생성된 클라이언트 암호 [!DNL Workfront]. 이렇게 하면 [!DNL Workfront] 요청이 ClientApp에서 오고 있음을 알리기 위한 것입니다.

1. 인증 코드와 클라이언트 암호가 맞다면 [!DNL Workfront] ClientApp에 액세스 토큰을 보냅니다. 이 액세스 토큰은 [!DNL Workfront] ClientApp에 대한 매핑이고, 다른 사용자 또는 클라이언트 애플리케이션에서 보거나, 복사하거나 사용할 수 없습니다.
1. ClientApp이 액세스 토큰을 [!DNL Workfront] 특정 정보 요청과 함께.
1. 액세스 토큰이 정확하므로 [!DNL Workfront] 클라이언트 앱에 정보를 보냅니다.

#### 액세스 토큰 새로 고침

보안의 경우 액세스 토큰은 짧은 시간 후에 만료됩니다. 매번 자격 증명을 입력하지 않고도 새 액세스 토큰을 받으려면 [!DNL OAuth2] 은 새로 고침 토큰을 사용합니다. 새로 고침 토큰은 클라이언트가 저장합니다.

새로 고침 토큰을 가져오는 프로세스는 섹션에서 설명한 절차와 동일합니다 [인증 코드 및 액세스 토큰으로 인증](#authorizing-with-an-authorization-code-and-access-token). 인증 코드에 대한 요청에는 범위가 포함됩니다 `offline_access`: 요청이 인증 코드와 함께 요청 토큰을 반환해야 함을 나타냅니다.
