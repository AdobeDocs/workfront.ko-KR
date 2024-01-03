---
title: 용 OAuth2 애플리케이션 만들기 [!DNL Workfront] 통합
user-type: administrator
product-area: system-administration;workfront-integrations
navigation-topic: administrator-integrations
description: '(으)로 [!DNL Adobe Workfront] 관리자는 의 인스턴스에 대해 OAuth2 애플리케이션을 만들 수 있습니다. [!DNL Workfront]: 다른 애플리케이션이 Workfront에 액세스할 수 있도록 합니다. 그런 다음 사용자는 다른 애플리케이션에 자신의 Workfront 데이터에 액세스할 수 있는 권한을 부여할 수 있습니다. 이러한 방식으로 Workfront을 사내 애플리케이션을 포함하여 원하는 애플리케이션과 통합할 수 있습니다.'
author: Becky
feature: System Setup and Administration, Workfront Integrations and Apps
role: Admin
exl-id: e13c7dda-8945-47ad-b6d3-4d6a62b368f5
source-git-commit: ff24fcc65791b6c18668a0dd3c58e033772a2def
workflow-type: tm+mt
source-wordcount: '1945'
ht-degree: 6%

---

# 용 OAuth2 애플리케이션 만들기 [!DNL Workfront] 통합

(으)로 [!DNL Adobe Workfront] 관리자는 의 인스턴스에 대해 OAuth2 애플리케이션을 만들 수 있습니다. [!DNL Workfront]: 다른 애플리케이션이 액세스할 수 있도록 허용 [!DNL Workfront]. 그런 다음 사용자는 다른 애플리케이션에 액세스할 권한을 부여할 수 있습니다 [!DNL Workfront] 데이터. 이러한 방식으로 자체 애플리케이션을 포함하여 원하는 애플리케이션과 통합할 수 있습니다.

다음을 만들 때 [!UICONTROL OAuth2] 응용 프로그램에서는 클라이언트 ID와 클라이언트 암호를 생성합니다. 그런 다음 사용자는 API 호출에서 클라이언트 ID를 사용하여 만든 애플리케이션과 통합할 수 있습니다.

>[!NOTE]
>
>OAuth2의 컨텍스트에서 &quot;앱 만들기&quot;는 다음과 같이 앱과 서버 간에 이러한 종류의 액세스 링크를 만드는 프로세스를 말합니다. [!DNL Workfront].

* 사용자 자격 증명(인증 코드 흐름)을 통해 OAuth2 애플리케이션을 구성하고 사용하는 방법에 대한 지침은 을 참조하십시오. [인증 코드 흐름을 사용하여 조직의 사용자 지정 OAuth 2 애플리케이션 구성 및 사용](../../wf-api/api/oauth-app-code-token-flow.md).
* 서버 인증(JWT 흐름)을 사용한 OAuth2 애플리케이션 구성 및 사용에 대한 지침은 을 참조하십시오. [JWT 플로우를 사용하여 조직의 사용자 지정 OAuth 2 애플리케이션 구성 및 사용](../../wf-api/api/oauth-app-jwt-flow.md).
* PKCE를 사용하여 OAuth2 애플리케이션을 구성하고 사용하는 방법에 대한 지침은 를 참조하십시오. [PKCE 플로우를 사용하여 조직의 사용자 정의 OAuth 2 애플리케이션 구성 및 사용](../../wf-api/api/oauth-app-pkce-flow.md).

## 액세스 요구 사항

이 문서의 단계를 수행하려면 다음 액세스 권한이 있어야 합니다.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] 플랜*</td> 
   <td> <p>임의</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] 라이센스*</td> 
   <td><p>새로운 기능: [!UICONTROL Standard]</p>
   또는
   <p>현재:[!UICONTROL 계획]</p></td> 
  </tr> 
  <tr> 
   <td role="rowheader">액세스 수준 구성*</td> 
   <td> 다음이어야 합니다: [!DNL Workfront] 관리자. </td> 
  </tr> 
 </tbody> 
</table>

&#42;보유 중인 플랜, 라이선스 유형 또는 액세스 권한을 알아보려면 [!DNL Workfront] 관리자.

## OAuth2 개요

애플리케이션에서 특정 정보를 가져와야 한다고 상상해 보십시오. [!DNL Workfront]. 정보를 요청하는 애플리케이션을 클라이언트라고 합니다. 이 예에서 클라이언트 이름은 ClientApp입니다. ClientApp은 특정 사용자의 정보에 액세스해야 하므로 이에 액세스해야 합니다 [!DNL Workfront] 을(를) 해당 사용자로 추가합니다. 사용자가 ClientApp에 사용자 이름과 암호를 제공하면 ClientApp은 사용자가 액세스할 수 있는 모든 데이터에 액세스할 수 있습니다. ClientApp에는 소량의 특정 정보만 필요하므로 이는 보안 위험이 있습니다.

ClientApp용 OAuth2 앱을 만들 때 기본적으로 다음과 같은 내용이 표시됩니다 [!DNL Workfront] ClientApp에서 액세스할 수 있음 [!DNL Workfront]: 그러나 ClientApp이 액세스하는 계정의 사용자가 액세스에 대한 권한을 부여하는 경우에만 해당합니다.

## OAuth2 애플리케이션 만들기

OAuth2 애플리케이션을 만들 때 통합의 요구 사항에 가장 적합한 애플리케이션 유형을 선택합니다.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th>애플리케이션 유형</th> 
   <th>다음에 최적</th> 
   <th>인증 방법</th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <p>머신 투 머신 애플리케이션</p> </td> 
   <td> <p>서버에서 실행되는 CLI, 데몬 또는 스크립트에 적합</p> <p>예:</p> 
    <ul> 
     <li> <p>[!DNL Shell] </p> </li> 
     <li> <p>[!DNL Python]</p> </li> 
    </ul> </td> 
   <td> <p>JSON 웹 토큰을 통한 공개/비공개 키 쌍 인코딩으로 인증.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>단일 페이지 웹 애플리케이션</p> </td> 
   <td> <p>모바일 또는 단일 페이지 웹 애플리케이션에 적합</p> <p>예:</p> 
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
   <td> <p>서버에서 자격 증명 및 토큰을 처리하는 서버측 애플리케이션에 적합</p> <p>예:</p> 
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
>한 번에 최대 10개의 OAuth2 애플리케이션을 보유할 수 있습니다.

* [서버 인증을 사용하여 OAuth2 애플리케이션 만들기(JWT 흐름)](#create-an-oauth2-application-using-server-authentication-jwt-flow)
* [사용자 자격 증명을 사용하여 OAuth2 애플리케이션 만들기(인증 코드 흐름)](#create-an-oauth2-application-using-user-credentials-authorization-code-flow)
* [PKCE를 사용하여 OAuth2 단일 페이지 웹 애플리케이션 만들기](#create-an-oauth2-single-page-web-application-using-pkce)

### 서버 인증을 사용하여 OAuth2 애플리케이션 만들기(JWT 흐름) {#create-an-oauth2-application-using-server-authentication-jwt-flow}

{{step-1-to-setup}}

1. 왼쪽 탐색 패널에서 을 클릭합니다. **[!UICONTROL 시스템]**&#x200B;을 선택한 다음 을 선택합니다. **[!UICONTROL OAuth2 애플리케이션]**.
1. 클릭 **[!UICONTROL 앱 통합 만들기]**.
다음 **새 OAuth2 애플리케이션** 상자가 표시됩니다.
1. 다음에서 **새 OAuth2 애플리케이션** 상자, 선택 **[!UICONTROL 머신 투 머신 애플리케이션]**.
1. 새 응용 프로그램의 이름을 입력하십시오(예: &quot;).[!DNL Workfront] for ClientApp.&quot;
1. Click **[!UICONTROL Create]**.
1. 새 앱의 필드를 채웁니다.

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">[!UICONTROL 클라이언트 ID]</td> 
      <td> <p>이 필드는 자동으로 생성됩니다.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL 클라이언트 암호]</td> 
      <td> <p>이 필드는 자동으로 생성됩니다.</p> <p><b>중요 사항</b>:  <p>이 페이지를 닫기 전에 이 필드의 내용을 다른 보안 파일에 복사합니다. 이 비밀 키를 다시 볼 수 없습니다.</p> <p>이 키를 분실하면 삭제하고 클라이언트 암호를 만드십시오.</p> 
        <ol> 
         <li value="1"> <p>다음을 클릭합니다. <b>[!UICONTROL Delete]</b> 아이콘 <img src="assets/delete.png"> 현재 클라이언트 암호를 삭제합니다.</p> </li> 
         <li value="2"> <p>클릭 <b>[!UICONTROL 클라이언트 암호 추가]</b> 새 클라이언트 암호를 생성합니다.</p> </li> 
        </ol> </p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL 공개 키]</td> 
      <td> <p>서버 간 앱은 인증을 위해 공개 및 개인 키를 사용합니다. 다음 중 하나를 수행하십시오.</p> 
       <ul> 
        <li> <p>클릭 <b>[!UICONTROL 공개 키 추가]</b> 다른 응용 프로그램에서 공개 키를 입력합니다.</p> </li> 
        <li> <p>클릭 <b>[!UICONTROL 공개/개인 키 쌍 생성]</b>그런 다음 다른 응용 프로그램과 공개 키를 공유합니다.</p> </li> 
       </ul> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL 이름]</td> 
      <td>앱에 지정한 이름과 동일한 이름입니다. 이 필드는 비워 둘 수 없습니다.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL 설명]</td> 
      <td>통합에 대한 설명을 입력합니다.</td> 
     </tr> 
    </tbody> 
   </table>

1. **[!UICONTROL 저장]**&#x200B;을 클릭합니다.

사용자 자격 증명(인증 코드 흐름)을 통해 OAuth2 애플리케이션을 구성하고 사용하는 방법에 대한 지침은 을 참조하십시오. [JWT 플로우를 사용하여 조직의 사용자 지정 OAuth 2 애플리케이션 구성 및 사용](../../wf-api/api/oauth-app-jwt-flow.md).

### 사용자 자격 증명을 사용하여 OAuth2 애플리케이션 만들기(인증 코드 흐름) {#create-an-oauth2-application-using-user-credentials-authorization-code-flow}

{{step-1-to-setup}}

1. 왼쪽 탐색 패널에서 을 클릭합니다. **[!UICONTROL 시스템]**&#x200B;을 선택한 다음 을 선택합니다. **[!UICONTROL OAuth2 애플리케이션]**.
1. 클릭 **[!UICONTROL 앱 통합 만들기]**.

   다음 **새 OAuth2 애플리케이션** 표시됩니다.
1. 다음에서 **새 OAuth2 애플리케이션** 상자, 선택 **[!UICONTROL 웹 애플리케이션]**.
1. 새 OAuth2 애플리케이션 이름(예: &quot;) 입력[!DNL Workfront] for ClientApp.&quot;
1. Click **[!UICONTROL Create]**.
1. 새 앱의 필드를 채웁니다.

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">[!UICONTROL 클라이언트 ID]</td> 
      <td> <p>이 필드는 자동으로 생성됩니다.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL 클라이언트 암호]</td> 
      <td> <p>이 필드는 자동으로 생성됩니다.</p> <p><b>중요 사항</b>:  <p>이 페이지를 닫기 전에 이 필드의 내용을 다른 보안 파일에 복사합니다. 이 비밀 키를 다시 볼 수 없습니다.</p> <p>이 키를 분실하면 삭제하고 클라이언트 암호를 만드십시오.</p> 
        <ol> 
         <li value="1"> <p>다음을 클릭합니다. <b>[!UICONTROL Delete]</b> 아이콘 <img src="assets/delete.png"> 현재 클라이언트 암호를 삭제합니다.</p> </li> 
         <li value="2"> <p>클릭 <b>[!UICONTROL 클라이언트 암호 추가]</b> 새 클라이언트 암호를 생성합니다.</p> </li> 
        </ol> </p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL 리디렉션 URL]</td> 
      <td>사용자는으로 인증되면 이 경로로 리디렉션됩니다. [!DNL Workfront].</td> 
     </tr> 
     <tr data-mc-conditions=""> 
      <td role="rowheader">[!UICONTROL 새로 고침 토큰 순환]</td> 
      <td>새로 고침 토큰을 사용할 때마다 새 새로 고침 토큰을 발급하려면 이 옵션을 활성화합니다. 애플리케이션은 매번 새로 고침 후에 새 새로 고침 토큰을 저장해야 합니다.</td> 
     </tr> 
     <tr data-mc-conditions=""> 
      <td role="rowheader">[!UICONTROL 절대 새로 고침 토큰 만료]</td> 
      <td> <p>새로 고침 토큰이 만료되기 전에 존재할 시간을 선택합니다. 만료되면 사용자는 통합에 다시 로그인해야 합니다. 새로 고침 토큰이 만료되지 않도록 하려면 "[!UICONTROL 만료 없음]"을 선택합니다.</p> </td> 
     </tr> 
     <tr data-mc-conditions=""> 
      <td role="rowheader">토큰 만료 새로 고침 중지</td> 
      <td> <p>사용자가 시스템에서 활성 상태가 아닌 경우 이후 새로 고침 토큰이 만료되는 시간을 선택합니다. </p> <p>예를 들어 비활성 새로 고침 토큰 만료가 6개월이고 사용자가 6개월 동안 로그인하지 않으면 절대 새로 고침 토큰 만료가 더 오래 설정될 수 있어도 새로 고침 토큰이 만료됩니다.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL 로고]</td> 
      <td>로고를 추가하여 이 앱의 식별 가능성을 높일 수 있습니다. </td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL 이름]</td> 
      <td>앱에 지정한 이름과 동일한 이름입니다. 이 필드는 비워 둘 수 없습니다.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL 설명]</td> 
      <td>통합에 대한 설명을 입력합니다.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL 앱 설명 URL]</td> 
      <td>"정보" 페이지 또는 통합에 대한 자세한 정보가 포함된 페이지에 대한 링크일 수 있습니다.</td> 
     </tr> 
    </tbody> 
   </table>

1. **[!UICONTROL 저장]**&#x200B;을 클릭합니다.

사용자 자격 증명(인증 코드 흐름)을 통해 OAuth2 애플리케이션을 구성하고 사용하는 방법에 대한 지침은 을 참조하십시오. [인증 코드 흐름을 사용하여 조직의 사용자 지정 OAuth 2 애플리케이션 구성 및 사용](../../wf-api/api/oauth-app-code-token-flow.md).

### PKCE를 사용하여 OAuth2 단일 페이지 웹 애플리케이션 만들기 {#create-an-oauth2-single-page-web-application-using-pkce}

{{step-1-to-setup}}

1. 왼쪽 탐색 패널에서 을 클릭합니다. **[!UICONTROL 시스템]**&#x200B;을 선택한 다음 을 선택합니다. **[!UICONTROL OAuth2 애플리케이션]**.
1. 클릭 **[!UICONTROL 앱 통합 만들기]**.

   다음 **새 OAuth2 애플리케이션** 상자가 표시됩니다.
1. 다음에서 **새 OAuth2 애플리케이션** 상자, 선택 **[!UICONTROL 단일 페이지 웹 애플리케이션]**.
1. 새 이름 입력 [!UICONTROL OAuth2] 애플리케이션(예: &quot;)[!DNL Workfront] for ClientApp.&quot;
1. Click **[!UICONTROL Create]**.
1. 새 앱의 필드를 채웁니다.

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">[!UICONTROL 클라이언트 ID]</td> 
      <td> <p>이 필드는 자동으로 생성됩니다.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL 리디렉션 URL]</td> 
      <td>사용자가 Workfront으로 인증되면 이 경로로 리디렉션됩니다.</td> 
     </tr> 
     <tr data-mc-conditions=""> 
      <td role="rowheader">[!UICONTROL 사용할 때마다 새로 고침 토큰을 회전합니다.]</td> 
      <td>새로 고침 토큰을 사용할 때마다 새 새로 고침 토큰을 발급하려면 이 옵션을 활성화합니다. 애플리케이션은 매번 새로 고침 후에 새 새로 고침 토큰을 저장해야 합니다.</td> 
     </tr> 
     <tr data-mc-conditions=""> 
      <td role="rowheader">[!UICONTROL 절대 만료]</td> 
      <td> <p>새로 고침 토큰이 만료되기 전에 존재할 시간을 선택합니다. 만료되면 사용자는 통합에 다시 로그인해야 합니다. 새로 고침 토큰이 만료되지 않도록 하려면 "[!UICONTROL 만료 없음]"을 선택합니다.</p> </td> 
     </tr> 
     <tr data-mc-conditions=""> 
      <td role="rowheader">[!UICONTROL 비활성 만료]</td> 
      <td> <p>사용자가 시스템에서 활성 상태가 아닌 경우 이후 새로 고침 토큰이 만료되는 시간을 선택합니다. </p> <p>예를 들어 비활성 새로 고침 토큰 만료가 6개월이고 사용자가 6개월 동안 로그인하지 않으면 절대 새로 고침 토큰 만료가 더 오래 설정될 수 있어도 새로 고침 토큰이 만료됩니다.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL 로고]</td> 
      <td>로고를 추가하여 이 앱의 식별 가능성을 높일 수 있습니다. </td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL 이름]</td> 
      <td>앱에 지정한 이름과 동일한 이름입니다. 이 필드는 비워 둘 수 없습니다.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL 설명]</td> 
      <td>통합에 대한 설명을 입력합니다.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL Developer name]</td> 
      <td>OAuth2 애플리케이션을 설정하는 개발자의 이름입니다.</td> 
     </tr> 
   <tr> 
      <td role="rowheader">[!UICONTROL 개발자 이메일 주소]</td> 
      <td>OAuth2 애플리케이션을 설정하는 개발자의 이메일 주소입니다.</td> 
     </tr> 
   <tr> 
      <td role="rowheader">[!UICONTROL 개인정보 처리방침 URL]</td> 
      <td>조직에서 개인정보 처리방침을 저장하는 위치에 대한 링크입니다.</td> 
     </tr>


   </tbody> 
   </table>

   <!-- removed this from the table, and added "Developer name" and following rows:
   [!UICONTROL App Description URL]</td> 
      <td>This can be a link to an "About us" page or a page with more information about the integration.> -->

1. **[!UICONTROL 저장]**&#x200B;을 클릭합니다.

## 생성된 OAuth2 애플리케이션 구성 및 사용

생성된 OAuth2 애플리케이션을 추가로 구성하고 사용하려면 API 호출을 비롯한 몇 가지 기술 지식이 필요합니다.

* 사용자 자격 증명(인증 코드 흐름)을 통해 OAuth2 애플리케이션을 구성하고 사용하는 방법에 대한 지침은 을 참조하십시오. [인증 코드 흐름을 사용하여 조직의 사용자 지정 OAuth 2 애플리케이션 구성 및 사용](../../wf-api/api/oauth-app-code-token-flow.md).
* 서버 인증(JWT 흐름)을 사용한 OAuth2 애플리케이션 구성 및 사용에 대한 지침은 을 참조하십시오. [JWT 플로우를 사용하여 조직의 사용자 지정 OAuth 2 애플리케이션 구성 및 사용](../../wf-api/api/oauth-app-jwt-flow.md).
* PKCE를 사용하여 OAuth2 애플리케이션을 구성하고 사용하는 방법에 대한 지침은 를 참조하십시오. [PKCE 플로우를 사용하여 조직의 사용자 정의 OAuth 2 애플리케이션 구성 및 사용](../../wf-api/api/oauth-app-pkce-flow.md).

## 인증 코드 흐름에 대한 OAuth2 프로세스

>[!NOTE]
>
>사용자는 [!UICONTROL OAuth2] api를 통한 애플리케이션. 이 섹션에서는 일반적인 용어로 기능을 설명하며 참조용으로만 제공됩니다.
>
>특정 API 호출을 포함하여 OAuth2 애플리케이션 사용에 대한 특정 지침은 를 참조하십시오. [인증 코드 흐름을 사용하여 조직의 사용자 지정 OAuth 2 애플리케이션 구성 및 사용](../../wf-api/api/oauth-app-code-token-flow.md).

### 인증 코드 및 액세스 토큰을 사용하여 인증 {#authorizing-with-an-authorization-code-and-access-token}

1. ClientApp에는 다음 정보가 필요합니다. [!DNL Workfront]에 대한 요청을 [!DNL Workfront] API `/authorize` 엔드포인트. 요청에는 다음이 포함됩니다. [!UICONTROL response_type] `code`: 요청이 인증 코드를 반환해야 함을 나타냅니다.
1. 이 트리거는 [!DNL Workfront] 사용자에게 인증 프롬프트를 보냅니다. 사용자는 프롬프트에 자격 증명을 입력할 수 있습니다. [!DNL Workfront] ClientApp과 통신할 수 있는 권한입니다. 사용자가 이미 로그인한 경우 [!DNL Workfront], 이 단계는 건너뛸 수 있습니다.
1. 다음 [!DNL Workfront] API가 ClientApp에 인증 코드를 보냅니다.
1. ClientApp은 요청에 다음 정보를 [!DNL Workfront] API `/token`   끝점:

   * 3단계에서 ClientApp으로 전송된 인증 코드입니다. 이는 사용자 권한의 특정 인스턴스를 식별합니다.
   * 에서 ClientApp OAuth2 앱을 설정할 때 생성된 클라이언트 암호 [!DNL Workfront]. 이렇게 하면 [!DNL Workfront] 요청이 ClientApp에서 오고 있음을 알기 위함입니다.

1. 인증 코드와 클라이언트 암호가 올바른 경우 [!DNL Workfront] 는 액세스 토큰을 ClientApp에 보냅니다. 이 액세스 토큰은에서 직접 전송됩니다. [!DNL Workfront] 다른 사용자나 클라이언트 응용 프로그램에서 보거나 복사하거나 사용할 수 없습니다.
1. ClientApp이 액세스 토큰을 (으)로 보냅니다. [!DNL Workfront] 을 참조하십시오.
1. 액세스 토큰이 정확하기 때문에, [!DNL Workfront] 는 정보를 ClientApp에 보냅니다.

#### 액세스 토큰 새로 고침

보안을 위해 액세스 토큰은 짧은 시간 후에 만료됩니다. 매번 자격 증명을 입력할 필요 없이 새 액세스 토큰을 가져오려면 [!DNL OAuth2] 새로 고침 토큰을 사용합니다. 새로 고침 토큰은 클라이언트에 의해 저장됩니다.

새로 고침 토큰을 획득하는 프로세스는 단원에서 설명한 절차와 동일합니다 [인증 코드 및 액세스 토큰을 사용하여 인증](#authorizing-with-an-authorization-code-and-access-token). 인증 코드에 대한 요청에는 범위가 포함됩니다 `offline_access`: 요청이 인증 코드와 함께 요청 토큰을 반환해야 함을 나타냅니다.
