---
title: 구성 [!DNL SharePoint] 통합
user-type: administrator
product-area: system-administration;workfront-integrations;setup
navigation-topic: administrator-integrations
description: '통합할 수 있습니다 [!DNL Workfront] with [!DNL SharePoint] 온라인, 사용자에게 이동, 링크 및 추가 기능을 제공합니다. [!DNL SharePoint] Workfront 내의 문서. 제공된 기능은 다른 기능과 비슷합니다 [!DNL Workfront] 통합(예: Google 드라이브, 상자 및 Dropbox).'
author: Becky, Caroline
feature: System Setup and Administration, [!DNL Workfront] Integrations and Apps, Digital Content and Documents
role: Admin
exl-id: fd45e1bc-9a35-4960-a73a-ff845216afe4
source-git-commit: 5292069412a73f824dbcd967d47737cff5ef58fa
workflow-type: tm+mt
source-wordcount: '2515'
ht-degree: 0%

---

# 기존 구성 [!DNL SharePoint] 통합

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">**DON'T DELETE, DRAFT OR HIDE THIS ARTICLE. IT IS LINKED TO THE PRODUCT, THROUGH THE CONTEXT SENSITIVE HELP LINKS. **</p>
-->

>[!IMPORTANT]
>
>새로운 [!DNL SharePoint] 22.3 릴리스(2022년 7월)와 함께 프로덕션에 통합이 릴리스되었습니다. 사용자는 기존 문서를 통해 연결된 문서에 계속 액세스할 수 있지만 [!DNL SharePoint] 통합하려면 새로운 [!DNL SharePoint] SharePoint에서 문서를 연결하는 통합입니다.
>
>* 새로운 SharePoint 통합은 관리자가 구성할 필요가 없으며 개별 사용자가 설정할 수 있습니다. 그러나 새 SharePoint 통합으로 원활하게 전환하려면 Workfront 관리자가 Workfront 설정 영역에서 몇 가지 작은 설정을 변경해야 합니다.
   >
   >    자세한 내용 및 지침은 [문서에 계속 액세스할 수 있도록 기존 SharePoint 통합을 구성합니다](#configure-the-legacy-sharepoint-integration-for-continued-access-to-documents) 참조하십시오.
>    
>* 사용자가 현재 기존 파일을 통해 연결된 문서를 연결하는 것이 좋습니다 [!DNL SharePoint] 통합을 통해 통합할 수 있습니다.
   >    
   >    문서 연결에 대한 지침은 [외부 응용 프로그램에서 문서 연결](../../documents/adding-documents-to-workfront/link-documents-from-external-apps.md).


통합할 수 있습니다 [!DNL Workfront] with [!DNL SharePoint Online]로 이동, 링크 및 추가 기능을 사용자에게 제공하는 방법 [!DNL SharePoint] Workfront 내의 문서. 제공된 기능은 다른 기능과 비슷합니다 [!DNL Workfront] 통합 [!DNL Google Drive], [!DNL Box], 및 [!DNL Dropbox].

이 통합은 [!DNL SharePoint Online]. 의 온-프레미스 인스턴스 [!DNL SharePoint] 지원되지 않습니다.

## 액세스 요구 사항

이 문서의 절차를 수행하려면 다음 사항이 있어야 합니다.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] 플랜</td> 
   <td>모든</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] 라이선스</td> 
   <td>[!UICONTROL 계획]</td> 
  </tr> 
  <tr> 
   <td role="rowheader">액세스 수준 구성*</td> 
   <td> <p>넌 [!DNL Workfront] 관리자 에 대한 자세한 정보 [!DNL Workfront] 관리자 <a href="../../administration-and-setup/add-users/configure-and-grant-access/grant-a-user-full-administrative-access.md" class="MCXref xref">사용자에게 전체 관리자 액세스 권한 부여</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;어떤 계획, 라이센스 유형 또는 액세스 권한을 보유하고 있는지 확인하려면 [!DNL Workfront] 관리자

## 전제 조건

에 필요한 액세스 또는 권한이 있어야 합니다. [!DNL SharePoint] 조직의 수정 또는 구성 [!DNL SharePoint].

## 새로운 SharePoint 통합을 통해 문서 연결

개별 사용자는 새로운 [!DNL SharePoint] 통합. 통합에는 관리자 구성이 필요하지 않습니다. 대신 사용자가 로그인됩니다 [!DNL Microsoft] 사용자가 사용 가능한 문서에 액세스할 수 있도록 통합에서 문서를 연결할 때 계정이 설정됩니다 [!DNL SharePoint].

사용자가 처음 [!DNL Workfront] [!DNL SharePoint] 통합 [!DNL SharePoint] 계정, 사용자는 [!DNL Workfront] 상호 작용할 때 사용 [!UICONTROL SharePoint] 계정이 필요합니다. 읽기 권한 허용 [!DNL Workfront] 에서 파일을 보고 액세스할 수 있습니다. [!DNL SharePoint], 및 쓰기 권한을 통해 사용자가 파일을 [!DNL SharePoint].

문서 연결에 대한 지침은 [!DNL SharePoint] 통합 [외부 문서를 [!DNL Workfront]](../../documents/adding-documents-to-workfront/link-documents-from-external-apps.md#link-an-external-document-to-workfront)

>[!NOTE]
>
>* A [!DNL SharePoint] 통합은 단일 [!DNL SharePoint] 인스턴스. 따라서 사용자는 하나의 통합을 설정할 수 있습니다 [!DNL SharePoint]인 경우 두 번째에 대한 통합을 설정할 수 없습니다 [!DNL SharePoint], 두 번째 태그와 문서에 대한 권한이 있어도 [!DNL SharePoint].
>
>* 사용자는 를 통해 동일한 사이트, 컬렉션, 폴더, 하위 폴더 및 파일에 액세스할 수 있습니다 [!DNL Workfront] [!DNL SharePoint] 보유한 통합 [!DNL SharePoint] 계정이 필요합니다.


## 문서에 계속 액세스할 수 있도록 기존 SharePoint 통합을 구성합니다

사용자가 이전 SharePoint 통합을 통해 Workfront에 연결된 문서에 계속 액세스할 수 있도록 하려면 기존 SharePoint 통합에 대한 액세스를 다시 구성하고 SharePoint 클라이언트 암호를 최신 상태로 유지해야 합니다.

* [기존 액세스 재구성 [!DNL SharePoint] 통합](#reconfigure-access-to-the-legacy-dnl-sharepoint-integration)
* [기존 파일에 계속 액세스할 수 있도록 클라이언트 암호 구성 [!DNL SharePoint] 통합](#configure-the-client-secret-for-continued-access-to-the-legacy-dnl-sharepoint-integration)

### 기존 액세스 재구성 [!DNL SharePoint] 통합

기존 문서를 통해 연결된 문서에 액세스할 수 있도록 하기 위해 [!DNL SharePoint] 통합을 통해 사용자가 해당 통합을 통해 새 문서를 연결할 수 없도록 하려면 다음 절차를 완료하십시오.

>[!NOTE]
>
> * 기존 [!DNL SharePoint] 통합에는 &quot; 레이블이 지정됩니다.[!DNL SharePoint].&quot;
> * 새로운 [!DNL SharePoint] 통합에는 &quot; 레이블이 지정됩니다.[!UICONTROL [!DNL SharePoint] (그래프 API)].&quot;


1. 을(를) 클릭합니다. **[!UICONTROL 기본 메뉴]** 아이콘 ![기본 메뉴](assets/main-menu-icon.png) Adobe Workfront의 오른쪽 위 모서리에서 을(를) 클릭하고 **[!UICONTROL 설정]** ![설정](../get-started-wf-administration/assets/gear-icon-settings.png).
1. 선택 **[!UICONTROL 문서]** 왼쪽 탐색에서 를 선택하고 **[!UICONTROL 클라우드 공급자]**.
1. 다음을 확인합니다. **[!DNL SharePoint]** 옵션 및 **[!UICONTROL [!DNL SharePoint](그래프 API)]** 이 두 가지 옵션을 모두 사용할 수 있습니다.
1. **[!UICONTROL 저장]**&#x200B;을 클릭합니다.
1. 선택 **[!UICONTROL 문서]** 왼쪽 탐색에서 를 선택하고 **[!UICONTROL [!DNL SharePoint]통합]**.
1. 기존 통합을 위해 목록 왼쪽의 확인 표시를 선택한 다음 을 선택합니다 **[!UICONTROL 비활성화]**.


### 기존 파일에 계속 액세스할 수 있도록 클라이언트 암호 구성 [!DNL SharePoint] 통합

사용자 [!DNL SharePoint] 클라이언트 암호 만료는 1년에 한 번 만료됩니다. 기존 문서에 계속 액세스할 수 있도록 [!DNL SharePoint] 통합을 유지해야 합니다. [!DNL SharePoint] 클라이언트 암호 최신입니다.

>[!IMPORTANT]
>
> 왜냐면 [!DNL SharePoint] 클라이언트 암호는 [!DNL Microsoft], 클라이언트 암호 기능 및 절차는 [!DNL SharePoint] 만든 사람 [!DNL Microsoft]. 항상 [!DNL Microsoft] 의 절차 및 기능에 대한 최신 정보를 보려면 [!DNL SharePoint].

<!--1. Go to the site that your [!DNL SharePoint] integration uses. This may be a site that you created when setting up the integrations, or it may be your organization's root site.

1. Add `/_layouts/15/appregnew.aspx` to the end of the URL in the search bar at the top of your browser window.-->

1. 에 설명된 대로 새 클라이언트 암호 생성 [에서 만료되는 클라이언트 암호 바꾸기 [!DNL SharePoint] 추가 기능](https://docs.microsoft.com/en-us/sharepoint/dev/sp-add-ins/replace-an-expiring-client-secret-in-a-sharepoint-add-in#generate-a-new-secret)
1. 이 클라이언트 암호를 보안 위치에 복사합니다.
1. 에 로그인합니다. [!DNL Workfront] 관리자로.
1. Workfront에서 **[!UICONTROL 기본 메뉴]** 아이콘 ![](assets/main-menu-icon.png) Adobe Workfront의 오른쪽 위 모서리에서 을(를) 클릭하고 **[!UICONTROL 설정]** ![](assets/gear-icon-settings.png).
1. 왼쪽 패널에서 **[!UICONTROL 문서]** > **[!UICONTROL [!DNL SharePoint]통합]**.
1. 을(를) 클릭합니다. [!DNL SharePoint] 업데이트할 통합을 클릭한 다음 **[!UICONTROL 편집]**.
1. 새 클라이언트 암호를 **[!UICONTROL 클라이언트 암호]** 필드.
1. **[!UICONTROL 저장]**&#x200B;을 클릭합니다.



## 레거시 SharePoint 통합 설정에 대한 지침

>[!IMPORTANT]
>
>이 통합은 더 이상 사용되지 않습니다. 이 지침은 정보만을 위한 것이며 가까운 시일 내에 제거됩니다.


Workfront에 연결 [!DNL SharePoint] 사용자 인증 및 권한 부여를 위해 대부분의 웹 기반 통합에서 사용하는 표준인 OAuth 2.0을 사용하여 온라인 상태가 됩니다.

OAuth를 구성하려면 다음을 만들어야 합니다 [!DNL SharePoint] 내의 사이트 및 사이트 앱 [!DNL SharePoint]. 이 프로세스는 다음 섹션에 설명되어 있습니다.

OAuth에 대한 자세한 내용은 [http://oauth.net](http://oauth.net/).

>[!TIP]
>
>사이에 정보를 쉽게 복사하고 붙여넣을 수 있도록 [!DNL Workfront] 및 [!DNL SharePoint] 이 단계에서는 두 응용 프로그램을 별도의 탭에서 열어 두는 것이 좋습니다.

* [만들기 및 구성 [!DNL SharePoint] 사이트](#create-and-configure-a-sharepoint-site)
* [사이트 앱에 쓰기 권한 부여](#grant-write-permissions-to-the-site-app)
* [만들기 [!DNL Workfront] [!DNL SharePoint] 통합 인스턴스](#create-a-workfront-sharepoint-integration-instance)
* [통합 완료](#complete-your-integration)
* [문서 추가](#add-documents)

### 만들기 및 구성 [!DNL SharePoint] 사이트  {#create-and-configure-a-sharepoint-site}

대상 [!DNL Workfront] 인증 [!DNL SharePoint], [!DNL Workfront] 사용자가 [!UICONTROL 전체 제어] 권한 수준 또는 특정 관리 권한 이 마스터 사이트는 [!DNL Workfront].

을(를) 만들고 구성하려면 [!DNL SharePoint] 사이트:

1. (선택 사항) 조직의 루트 사이트를 사용하지 않으려는 경우 [!DNL SharePoint].

   지침은 [사이트 만들기](https://docs.microsoft.com/en-us/sharepoint/create-site-collection) 에서 [!DNL Microsoft] 설명서.

   * 을(를) 선택합니다 **[!UICONTROL 팀 사이트]** 옵션을 선택합니다.

1. (조건부) 1단계에서 사이트를 만든 경우 방금 만든 사이트로 이동합니다.

   또는

   1단계에서 사이트를 만들지 않은 경우 조직의 루트 사이트로 이동합니다.

1. 추가 `/_layouts/15/appregnew.aspx` 를 클릭합니다.
1. 다음 필드를 구성합니다.

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader"> <p>[!UICONTROL Client ID]</p> </td> 
      <td> <p>클릭 <strong>[!UICONTROL Generate]</strong> 클라이언트 ID를 생성합니다. 이 ID를 보안 위치에 복사합니다. 나중에 설정할 때 사용하게 됩니다 [!DNL SharePoint] 통합 [!DNL Workfront].</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"> <p>[!UICONTROL Client Secret]</p> </td> 
      <td> <p>클릭 <strong>[!UICONTROL Generate]</strong> 클라이언트 암호를 생성합니다. 이 암호를 보안 위치에 복사합니다. 나중에 설정할 때 사용하게 됩니다 [!DNL SharePoint] 통합 [!DNL Workfront].</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"> <p>제목</p> </td> 
      <td> <p>다음과 같은 제목을 입력합니다 [!DNL Workfront] 사이트 앱. 사용자는 문서를 추가할 때 이 제목을 볼 수 있습니다.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"> <p>[!UICONTROL App Domain]</p> </td> 
      <td> <p><code>my.workfront.com</code> </p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"> <p>[!UICONTROL 리디렉션 URI]</p> </td> 
      <td> <p><code>https://oauth.my.workfront.com/oauth2/redirect</code> </p> </td> 
     </tr> 
    </tbody> 
   </table>

1. Click **[!UICONTROL Create]**
1. 계속 [사이트 앱에 쓰기 권한 부여](#grant-write-permissions-to-the-site-app).

### 사이트 앱에 쓰기 권한 부여  {#grant-write-permissions-to-the-site-app}

이 시점에서 사이트 앱을 성공적으로 만들어 내에 등록했습니다 [!DNL Workfront]. 이 사이트 앱은 에서도 앱 주도자라고도 합니다 [!DNL SharePoint]. 임차인 내에 있습니다. 새 사이트 앱은 테넌트 내의 사이트 컬렉션에 자동으로 액세스할 수 없습니다. 각 사이트 모음에 대해 권한을 명시적으로 부여해야 합니다. 아래 단계는 새 사이트 앱에 사이트 컬렉션에 쓰기 권한을 부여하는 방법을 보여 줍니다. 아래에 추가한 각 사이트 모음에 대해 이 단계를 반복합니다 [!UICONTROL 표시되는 사이트 컬렉션] 위의 단계에서 다음을 수행합니다.

이 사이트 앱에는 [!UICONTROL 쓰기] 사용자가 액세스 [!DNL Workfront].

1. 의 URL에 &#39;/_layouts/15/appinv.aspx&#39;을 추가합니다 [!DNL Sharepoint].

   **예:**

   ```
   https://mycompany.sharepoint.com/sites/mysite/_layouts/15/appinv.aspx
   ```

1. 다음 필드를 구성합니다

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">[!UICONTROL 앱 ID]</td> 
      <td> <p>에서 만든 클라이언트 ID를 추가합니다 <a href="#create-and-configure-a-sharepoint-site" class="MCXref xref">만들기 및 구성 [!DNL SharePoint] 사이트 </a>을(를) 클릭합니다. <strong>[!UICONTROL 조회]</strong>.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"> <p>[!UICONTROL Client] / [!UICONTROL App Domain] / [!UICONTROL 리디렉션 URL]</p> </td> 
      <td> <p>이 기능은 [!UICONTROL 조회]를 클릭하면 자동으로 채워집니다.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL 권한 요청 XML]</td> 
      <td> <p>다음 XML을 [!UICONTROL 권한 요청 XML] 필드에 복사합니다. 추가 공백 없이 표시된 대로 추가되었는지 확인합니다. 오류를 방지하기 위해 사용됩니다.</p> 
      <div></a> 
      <div style="mc-code-lang: XML;" class="codeSnippetBody" data-mc-continue="False" data-mc-line-number-start="1" data-mc-use-line-numbers="False"> 
       <pre></pre></div></div></td></tr></tbody></table>

1. Click **[!UICONTROL Create]**.
1. 대화 상자가 나타나면 **[!UICONTROL 믿어라]**.
1. 를 클릭하여 사이트 앱에 사이트 모음에 액세스할 수 있는지 확인합니다. **[!UICONTROL 사이트 모음 앱 권한]** 링크 위치 [!UICONTROL 사이트 설정].
1. 나머지 사이트 컬렉션에 대해 위의 단계를 반복한 다음 계속 진행합니다 [만들기 [!DNL Workfront] [!DNL SharePoint] 통합 인스턴스](#create-a-workfront-sharepoint-integration-instance).

### 만들기 [!DNL Workfront] [!DNL SharePoint] 통합 인스턴스 {#create-a-workfront-sharepoint-integration-instance}

에서 사이트 앱을 만든 경우 [!DNL SharePoint]이제 사이트 앱의 정보를 [!DNL Workfront]. 사이트 앱은 앱 주도자이며, 사이트 모음 내의 문서에 액세스하기 위해 OAuth 요청을 수행하는 전달 역할을 합니다.

1. 에 로그인합니다. [!DNL Workfront] 관리자로.
1. 을(를) 클릭합니다. **[!UICONTROL 기본 메뉴]** 아이콘 ![](assets/main-menu-icon.png) Adobe Workfront의 오른쪽 위 모서리에서 을(를) 클릭하고 **[!UICONTROL 설정]** ![](assets/gear-icon-settings.png).

1. 왼쪽 패널에서 **[!UICONTROL 문서]** > **[!UICONTROL [!DNL SharePoint]통합]**.
1. 클릭 **[!UICONTROL 추가[!DNL SharePoint]]**.
1. 다음 필드를 구성합니다.

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader"> <p>[!UICONTROL Name]</p> </td> 
      <td> <p>이름 입력 [!DNL SharePoint] 통합. 사용자는 [!UICONTROL 추가] &gt; [!UICONTROL From] '통합 이름'을 클릭하면 이 이름이 표시됩니다. </p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"> <p>[!UICONTROL [!DNL SharePoint] 호스트 인스턴스]</p> </td> 
      <td> <p><code>&lt;YourDomain&gt;.sharepoint.com</code> </p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"> <p>[!UICONTROL [!DNL Azure] 액세스 도메인]</p> </td> 
      <td> <p><code>&lt;YourDomain&gt;.onmicrosoft.com</code> </p> <p>이는 사용자가 인증하는 데 사용할 기본 사이트를 나타냅니다. [!UICONTROL]과 동일한 도메인이 있을 수 있습니다 [!DNL SharePoint] 호스트 인스턴스].</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"> <p>
      </p> </td> 
      <td> <b>중요 사항</b> 사이트 컬렉션은 기존 [!DNL SharePoint] 통합.
       <ul> 
        <li> <p><b>조직의 루트 사이트를 사용하는 경우</b><b>:</b> </p> <p>입력 <code>/</code></p> </li> 
        <li> <p><b>마스터 사이트 및 하위 사이트를 사용하는 경우:</b> </p> <p><b>중요 사항</b>: [!DNL Microsoft SharePoint] 더 이상 하위 사이트를 사용하지 않는 것이 좋습니다.</p> <p>위의 섹션에서 만든 사이트 모음의 URL 체계를 입력합니다.</p> <p>.com 다음에 나오는 URL의 섹션입니다.</p> <p>예: URL용 <code>https://mycompany.sharepoint.com/sites/mysite</code>이렇게 하면 <code>/sites/mysite</code>.</p> </li> 
       </ul> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL [!DNL SharePoint] 클라이언트 ID]</td> 
      <td>생성한 클라이언트 ID를 입력합니다. <a href="#create-and-configure-a-sharepoint-site" class="MCXref xref">만들기 및 구성 [!DNL SharePoint] 사이트 </a>.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL [!DNL SharePoint] 클라이언트 암호]</td> 
      <td>생성한 클라이언트 암호 입력 <a href="#create-and-configure-a-sharepoint-site" class="MCXref xref">만들기 및 구성 [!DNL SharePoint] 사이트 </a>.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL Visible Site Collections]</td> 
      <td> <b>중요 사항</b> 사이트 컬렉션은 기존 [!DNL SharePoint] 통합.
       <ul> 
        <li> <p><b> 조직의 루트 사이트를 사용하는 경우</b><b>:</b> </p> <p>입력 <code>/</code></p> </li> 
        <li> <p><b>마스터 사이트 및 하위 사이트를 사용하는 경우:</b> </p> <p><b>중요 사항</b>: [!DNL Microsoft SharePoint] 더 이상 하위 사이트를 사용하지 않는 것이 좋습니다.</p> <p>추가할 각 하위 사이트에 대해 [!DNL SharePoint] 통합하려면 하위 사이트의 줄기세포를 입력합니다.</p> <p>예: URL용<code>https://mycompany.sharepoint.com/sites/mysite/mysubsite</code>이렇게 하면 <code>/sites/mysite/mysubsite</code>.</p> <p><b>메모</b>:   <p>구성 전용(하위 사이트 없음)을 테스트하려면 마스터 사이트의 스템을 입력합니다. </p> <p>예: URL용 <code> https://mycompany.sharepoint.com/sites/mysite</code>이렇게 하면 <code>/sites/mysite</code>.</p> <p>에 설명된 대로 구성을 테스트한 경우 <a href="#complete-your-integration" class="MCXref xref">통합 완료</a>를 눌러 마스터 사이트를 제거하고 하위 사이트를 입력해야 합니다.</p> 
          <ol> 
           <li value="1">을(를) 클릭합니다. <strong>[!UICONTROL 기본 메뉴]</strong> 아이콘 <img src="assets/main-menu-icon.png"> 의 오른쪽 위 모서리에서 [!DNL Adobe Workfront]를 클릭한 다음 <strong>[!UICONTROL 설정]</strong> <img src="assets/gear-icon-settings.png">.<li><p>왼쪽 패널에서 <strong>[!UICONTROL Documents]</strong> &gt; <strong>[!UICONTROL [!DNL SharePoint] 통합]</strong>.</p></li><li><p>을(를) 클릭합니다. [!DNL SharePoint] 설정하는 통합을 설정한 다음 편집을 클릭합니다.</p></li><li><p>[!UICONTROL Visible Site Collections] 필드에서 마스터 사이트의 스템을 삭제합니다.</p></li><li><p>추가할 각 하위 사이트에 대해 [!DNL SharePoint] 통합하려면 하위 사이트의 줄기세포를 입력합니다.</p></li><p>예: URL용<code>https://mycompany.sharepoint.com/sites/mysite/mysubsite</code>이렇게 하면 <code>/sites/mysite/mysubsite</code>.</p></li> 
          </ol> </p> </li> 
       </ul> <p> </p> <p> </p> </td> 
     </tr> 
    </tbody> 
   </table>

1. **[!UICONTROL 저장]**&#x200B;을 클릭합니다
1. 계속 [통합 완료](#complete-your-integration).

### 통합 완료 {#complete-your-integration}

기본 구성이 거의 완료되었습니다.

1. Workfront에서 **[!UICONTROL 기본 메뉴]** 아이콘 ![](assets/main-menu-icon.png) Adobe Workfront의 오른쪽 위 모서리에서 을(를) 클릭하고 **[!UICONTROL 문서]** ![](assets/document-icon.png).
1. 클릭 **[!UICONTROL 새로 추가]**.
1. 클릭 **[!UICONTROL From]`<title of your [!DNL SharePoint] site>`** 아래에 표시됩니다.

   이 사이트를 신뢰할 수 있도록 초대하는 대화 상자가 나타납니다.

   >[!NOTE]
   >
   >이 대화 상자가 나타나지 않으면 [!DNL SharePoint] 통합이 올바르게 구성되지 않았습니다.

1. 클릭 **[!UICONTROL 믿어라]**.

### 문서 추가 {#add-documents}

이제에서 문서를 추가할 수 있습니다 [!DNL SharePoint] 사이트.

자세한 내용은 [외부 문서를 [!DNL Workfront]](../../documents/adding-documents-to-workfront/link-documents-from-external-apps.md#linking-existing-documents) in [외부 응용 프로그램에서 문서 연결](../../documents/adding-documents-to-workfront/link-documents-from-external-apps.md)

>[!IMPORTANT]
>
>폴더를 연결한 사용자가 외부 응용 프로그램에 더 이상 액세스할 수 없는 경우 [!DNL Workfront] 더 이상 폴더의 컨텐츠에 액세스할 수 없습니다. 예를 들어 폴더를 처음 연결한 사용자가 회사를 나가는 경우 이러한 문제가 발생할 수 있습니다. 계속 액세스하려면 폴더에 액세스할 수 있는 사용자가 해당 폴더를 다시 연결해야 합니다.

## 문제 해결

* [문제: 사용자가 [!DNL SharePoint] 통합.](#problem-users-experience-authentication-based-errors-when-using-the-sharepoint-integration)
* [문제: 로서의 [!DNL Workfront] 사용자, 새 [!DNL SharePoint] 인스턴스. 내가 하려고 하면 오류가 보인다.](#problem-as-a-workfront-user-i-am-unable-to-provision-a-new-sharepoint-instance-when-i-attempt-to-do-i-see-an-error)
* [문제: 찾아보기를 시도할 때 [!DNL SharePoint] 파일 [!DNL Workfront]: 내 사이트 컬렉션이 하나도 표시되지 않습니다.](#problem-when-attempting-to-browse-sharepoint-files-in-workfront-i-do-not-see-any-or-all-of-my-site-collections)
* [문제: 이전에 연결된 폴더 및 문서에 액세스할 수 없습니다 [!DNL SharePoint].](#problem-i-cannot-access-previously-linked-folders-and-documents-in-sharepoint)

### 문제: 사용자가 [!DNL SharePoint] 통합. {#problem-users-experience-authentication-based-errors-when-using-the-sharepoint-integration}

솔루션:

사용자는 [!DNL SharePoint] 사이트.

사용 중인 사용자 [!UICONTROL 전체 제어] 액세스 권한에 대한 모든 필수 권한 [!DNL SharePoint] 통합. 사용자에게 전체 제어 액세스 권한을 부여하지 않으려면 다음 권한을 부여해야 합니다.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Design]</p> </td> 
   <td> <p>보기, 추가, 업데이트, 삭제, 승인 및 사용자 지정할 수 있습니다</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Edit]</p> </td> 
   <td> <p>목록을 추가, 편집 및 삭제할 수 있습니다. 목록 항목 및 문서를 보고, 추가하고, 업데이트하고, 삭제할 수 있습니다</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Contribute]</p> </td> 
   <td> <p>목록 항목 및 문서를 보고, 추가하고, 업데이트하고, 삭제할 수 있습니다</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL 보기만]</p> </td> 
   <td> <p>페이지, 목록 항목 및 문서를 볼 수 있습니다(서버측 파일 처리기가 있는 문서 유형은 브라우저에서 볼 수 있지만 다운로드되지는 않음)</p> </td> 
  </tr> 
 </tbody> 
</table>

권한 수준 만들기 및 편집에 대한 지침은 [권한 수준을 만들고 편집하는 방법](https://docs.microsoft.com/en-us/sharepoint/how-to-create-and-edit-permission-levels) ( Microsoft 설명서)를 참조하십시오.

### 문제: 로서의 [!DNL Workfront] 사용자, 새 [!DNL SharePoint] 인스턴스. 내가 하려고 하면 오류가 보인다. {#problem-as-a-workfront-user-i-am-unable-to-provision-a-new-sharepoint-instance-when-i-attempt-to-do-i-see-an-error}

솔루션:

이것은 두 가지 중 하나에서 시작되는 많은 항목에 의해 발생할 수 있습니다 [!DNL Workfront] 또는 [!DNL SharePoint]의 구성입니다. 다음을 확인합니다.

* 클라이언트 ID, 클라이언트 암호, 반환 URL 및 기타 구성 필드가 [!DNL Workfront] [!DNL SharePoint] 통합 인스턴스 및 [!DNL SharePoint] 사이트 앱.
* 사용자가 [!UICONTROL 전체 제어] 인증에 사용되는 사이트 모음에 대한 권한입니다.
* 사이트 앱은 아래에 나열됩니다 [!UICONTROL 사이트 앱 권한] 대상 [!UICONTROL 사이트 모음] 인증에 사용됩니다.

### 문제: 찾아보기를 시도할 때 [!DNL SharePoint] 파일 [!DNL Workfront]: 내 사이트 컬렉션이 하나도 표시되지 않습니다. {#problem-when-attempting-to-browse-sharepoint-files-in-workfront-i-do-not-see-any-or-all-of-my-site-collections}

솔루션:

에서 사이트 컬렉션을 보려면 [!DNL Workfront]를 채울 때는 다음 조건을 충족해야 합니다.

* 사이트 모음은 [!DNL Workfront] [!DNL SharePoint] 통합 인스턴스.

   에서 확인하려면 [!DNL Workfront]:

   1. 이동 [!UICONTROL 설정] > [!UICONTROL 문서] > [!UICONTROL [!DNL SharePoint] 통합].
   1. 편집 [!DNL SharePoint] 통합 인스턴스 정보.
   1. 사이트 모음이 아래에 나열되는지 확인합니다. [!UICONTROL 표시되는 사이트 컬렉션].

* 사용자는에서 사이트 컬렉션에 대한 보기 액세스 권한이 있어야 합니다. [!DNL SharePoint].
* 에서 확인하려면 [!DNL SharePoint], 이동 [!DNL SharePoint]를 열고 사이트 모음 > 을 엽니다. [!UICONTROL 설정] > [!UICONTROL 사이트 권한].
* 다음 [!DNL SharePoint] 사이트 앱에 사이트 모음에 액세스할 수 있어야 합니다.

   에서 확인하려면 [!DNL SharePoint]:

   1. 사이트 모음 > [!UICONTROL 설정] > [!UICONTROL 사이트 앱 권한].
   1. 다음을 확인합니다. [!UICONTROL 사이트 앱] 사용 [!DNL Workfront] 여기에 나열됩니다.
   1. (조건부) 사이트 앱이 나열되지 않은 경우 _layouts/15/appinv.aspx 을 사용하여 사이트 모음에 추가합니다.

      사이트 모음 추가에 대한 자세한 내용은 사이트 앱에 쓰기 권한 부여를 참조하십시오.

### 문제: 이전에 연결된 폴더 및 문서에 액세스할 수 없습니다 [!DNL SharePoint]. {#problem-i-cannot-access-previously-linked-folders-and-documents-in-sharepoint}

솔루션:

사용자가 [!DNL SharePoint] 폴더는 더 이상 인증할 수 없습니다. [!DNL Workfront] 더 이상 폴더의 컨텐츠에 액세스할 수 없습니다. 예를 들어 폴더를 처음 연결한 사용자가 회사를 나가는 경우 이러한 문제가 발생할 수 있습니다.

계속 액세스하려면 폴더에 액세스할 수 있는 사용자가 해당 폴더를 다시 연결해야 합니다.

외부 공급자의 폴더 연결에 대한 자세한 내용은 [외부 응용 프로그램에서 문서 연결](../../documents/adding-documents-to-workfront/link-documents-from-external-apps.md).

### 문제: 에서 문서를 추가하려고 할 때 &quot;404 찾을 수 없음&quot; 오류가 표시됩니다. [!DNL Sharepoint]

#### 솔루션:

이 오류는 다음에서 구성한 사이트 중 하나가 [!UICONTROL 표시되는 사이트 컬렉션] Sharepoint에서 목록이 삭제되었습니다. 을(를) 확인합니다. [!UICONTROL 표시되는 사이트 컬렉션] Sharepoint에서 삭제된 사이트를 나열하고 제거합니다.
