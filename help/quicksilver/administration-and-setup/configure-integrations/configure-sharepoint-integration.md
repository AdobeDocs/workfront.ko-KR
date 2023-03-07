---
title: 구성 [!DNL SharePoint] 통합
user-type: administrator
product-area: system-administration;workfront-integrations;setup
navigation-topic: administrator-integrations
description: 다음을 통합할 수 있습니다. [!DNL Workfront] 포함 [!DNL SharePoint] 온라인 - 사용자에게 탐색, 링크 및 추가 기능 제공 [!DNL SharePoint] Workfront 내의 문서입니다. 제공된 기능은 다른 기능과 유사합니다 [!DNL Workfront] Google Drive, Box 및 Dropbox 등의 통합
author: Becky, Caroline
feature: System Setup and Administration, [!DNL Workfront] Integrations and Apps, Digital Content and Documents
role: Admin
exl-id: fd45e1bc-9a35-4960-a73a-ff845216afe4
source-git-commit: 15aa025c9a35e30867f942047ec1989fdd6834e5
workflow-type: tm+mt
source-wordcount: '2517'
ht-degree: 0%

---

# 레거시 구성 [!DNL SharePoint] 통합

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">**DON'T DELETE, DRAFT OR HIDE THIS ARTICLE. IT IS LINKED TO THE PRODUCT, THROUGH THE CONTEXT SENSITIVE HELP LINKS. **</p>
-->

>[!IMPORTANT]
>
>새로운 [!DNL SharePoint] 22.3 릴리스(2022년 7월)와 함께 프로덕션에 통합이 릴리스되었습니다. 사용자는 여전히 기존 을 통해 연결된 문서에 액세스할 수 있습니다 [!DNL SharePoint] 통합하려면 새 [!DNL SharePoint] SharePoint에서 문서를 연결하는 통합.
>
>* 새 SharePoint 통합은 관리자가 구성할 필요가 없으며 개별 사용자가 설정할 수 있습니다. 그러나 새 SharePoint 통합으로 원활하게 전환하려면 Workfront 관리자가 Workfront 설정 영역에서 일부 설정을 변경해야 합니다.
   >
   >    자세한 내용 및 지침은 [문서에 대한 지속적인 액세스를 위해 레거시 SharePoint 통합 구성](#configure-the-legacy-sharepoint-integration-for-continued-access-to-documents) 이 문서에서.
>    
>* 사용자가 현재 레거시를 통해 연결된 문서를 연결하는 것이 좋습니다 [!DNL SharePoint] 새로운 통합을 통한 통합.
   >    
   >    문서 연결에 대한 지침은 [외부 애플리케이션에서 문서 연결](../../documents/adding-documents-to-workfront/link-documents-from-external-apps.md).


다음을 통합할 수 있습니다. [!DNL Workfront] 포함 [!DNL SharePoint Online], 사용자에게 탐색, 링크 및 추가 기능 제공 [!DNL SharePoint] Workfront 내의 문서입니다. 제공된 기능은 다른 기능과 유사합니다 [!DNL Workfront] 다음과 같은 통합 [!DNL Google Drive], [!DNL Box], 및 [!DNL Dropbox].

이 통합은 와만 호환됩니다. [!DNL SharePoint Online]. 의 온-프레미스 인스턴스 [!DNL SharePoint] 은(는) 지원되지 않습니다.

## 액세스 요구 사항

이 문서의 단계를 수행하려면 다음이 있어야 합니다.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] 플랜</td> 
   <td>모든</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] 라이센스</td> 
   <td>[!UICONTROL 계획]</td> 
  </tr> 
  <tr> 
   <td role="rowheader">액세스 수준 구성*</td> 
   <td> <p>다음이어야 합니다: [!DNL Workfront] 관리자. 다음에 대한 정보: [!DNL Workfront] 관리자, 참조 <a href="../../administration-and-setup/add-users/configure-and-grant-access/grant-a-user-full-administrative-access.md" class="MCXref xref">사용자에게 전체 관리 액세스 권한 부여</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;보유 중인 플랜, 라이선스 유형 또는 액세스 권한을 알아보려면 [!DNL Workfront] 관리자.

## 전제 조건

에서 필요한 액세스 또는 권한이 있어야 합니다. [!DNL SharePoint] 조직의 를 수정하거나 구성하려면 [!DNL SharePoint].

## 새로운 SharePoint 통합을 통해 문서 연결

개별 사용자는 새 링크를 통해 문서를 연결할 수 있습니다. [!DNL SharePoint] 통합. 통합에는 관리자 구성이 필요하지 않습니다. 대신 사용자는 [!DNL Microsoft] 계정 : 문서를 연결할 때 통합에서 사용자의 [!DNL SharePoint].

사용자가 처음으로 연결할 때 [!DNL Workfront] [!DNL SharePoint] 통합 대상 [!DNL SharePoint] 계정, 사용자는 다음의 모든 권한을 확인하고 이에 동의하게 됩니다. [!DNL Workfront] 는 와 상호 작용할 때 를 사용합니다 [!UICONTROL SharePoint] 계정입니다. 읽기 권한 허용 [!DNL Workfront] 에 있는 파일을 보고 액세스하려면 [!DNL SharePoint], 및 쓰기 권한을 통해 사용자는에 파일을 업로드할 수 있습니다. [!DNL SharePoint].

![Sharepoint 권한](assets/sharepoint-permissions.png)

를 통해 문서를 연결하는 방법에 대한 지침 [!DNL SharePoint] 통합, 참조 [외부 문서 연결 대상 [!DNL Workfront]](../../documents/adding-documents-to-workfront/link-documents-from-external-apps.md#link-an-external-document-to-workfront)

>[!NOTE]
>
>* A [!DNL SharePoint] 통합은 하나에 연결할 수 있음 [!DNL SharePoint] 인스턴스. 따라서 사용자는 하나의 통합을 설정할 수 있습니다 [!DNL SharePoint], 하지만 을(를) 초로 통합을 설정할 수 없습니다. [!DNL SharePoint], 및에 대한 권한이 있는 경우에도 두 번째 [!DNL SharePoint].
>
>* 사용자는 를 통해 동일한 사이트, 컬렉션, 폴더, 하위 폴더 및 파일에 액세스할 수 있습니다 [!DNL Workfront] [!DNL SharePoint] 에 있는 것과 같은 통합 [!DNL SharePoint] 계정입니다.


## 문서에 대한 지속적인 액세스를 위해 레거시 SharePoint 통합 구성

기존 SharePoint 통합을 통해 사용자가 Workfront에 연결된 문서에 계속 액세스할 수 있도록 하려면 기존 SharePoint 통합에 대한 액세스를 다시 구성하고 SharePoint 클라이언트 보안을 최신 상태로 유지해야 합니다.

* [레거시 액세스 재구성 [!DNL SharePoint] 통합](#reconfigure-access-to-the-legacy-dnl-sharepoint-integration)
* [레거시 액세스를 계속할 수 있도록 클라이언트 암호 구성 [!DNL SharePoint] 통합](#configure-the-client-secret-for-continued-access-to-the-legacy-dnl-sharepoint-integration)

### 레거시 액세스 재구성 [!DNL SharePoint] 통합

기존 을 통해 연결된 문서에 액세스할 수 있도록 합니다. [!DNL SharePoint] 통합하되, 사용자가 해당 통합을 통해 새 문서를 연결할 수 없도록 하려면 다음 절차를 완료하십시오.

>[!NOTE]
>
> * 레거시 [!DNL SharePoint] 통합에는 &quot; 레이블이 지정됩니다[!DNL SharePoint].&quot;
> * 새로운 [!DNL SharePoint] 통합에는 &quot; 레이블이 지정됩니다[!UICONTROL [!DNL SharePoint] (Graph API)].&quot;


1. 다음을 클릭합니다. **[!UICONTROL 메인 메뉴]** 아이콘 ![메인 메뉴](assets/main-menu-icon.png) Adobe Workfront의 오른쪽 상단에서 을(를) 클릭한 다음 **[!UICONTROL 설정]** ![설정](../get-started-wf-administration/assets/gear-icon-settings.png).
1. 선택 **[!UICONTROL 문서]** 왼쪽 탐색에서 을(를) 선택합니다. **[!UICONTROL 클라우드 공급자]**.
1. 다음을 확인하십시오. **[!DNL SharePoint]** 옵션 및 **[!UICONTROL [!DNL SharePoint](Graph API)]** 옵션이 모두 활성화됩니다.
1. **[!UICONTROL 저장]**&#x200B;을 클릭합니다.
1. 선택 **[!UICONTROL 문서]** 왼쪽 탐색에서 을(를) 선택합니다. **[!UICONTROL [!DNL SharePoint]통합]**.
1. 기존의 모든 통합에 대해 목록 왼쪽에 있는 확인 표시를 선택한 다음 를 선택합니다 **[!UICONTROL 사용 안 함]**.


### 레거시 액세스를 계속할 수 있도록 클라이언트 암호 구성 [!DNL SharePoint] 통합

사용자 [!DNL SharePoint] 클라이언트 암호는 1년에 한 번 만료됩니다. 기존 문서에 대한 지속적인 액세스 보장 [!DNL SharePoint] 통합, 다음을 유지해야 합니다. [!DNL SharePoint] 최신 클라이언트 암호.

>[!IMPORTANT]
>
> 이유 [!DNL SharePoint] 클라이언트 암호는 다음에서 처리됩니다. [!DNL Microsoft], 클라이언트 암호 기능 및 프로시저는 다음에 대한 업데이트에 따라 변경될 수 있습니다. [!DNL SharePoint] 만든 사람 [!DNL Microsoft]. 항상 다음 확인 [!DNL Microsoft] 의 절차 및 기능에 대한 최신 정보를 제공하는 설명서 [!DNL SharePoint].

<!--1. Go to the site that your [!DNL SharePoint] integration uses. This may be a site that you created when setting up the integrations, or it may be your organization's root site.

1. Add `/_layouts/15/appregnew.aspx` to the end of the URL in the search bar at the top of your browser window.-->

1. 에 설명된 대로 새 클라이언트 암호 생성 [에서 만료될 클라이언트 암호 바꾸기 [!DNL SharePoint] 추가 기능](https://docs.microsoft.com/en-us/sharepoint/dev/sp-add-ins/replace-an-expiring-client-secret-in-a-sharepoint-add-in#generate-a-new-secret)
1. 이 클라이언트 암호를 안전한 위치에 복사합니다.
1. 에 로그인 [!DNL Workfront] 관리자입니다.
1. Workfront에서 **[!UICONTROL 메인 메뉴]** 아이콘 ![](assets/main-menu-icon.png) Adobe Workfront의 오른쪽 상단에서 을(를) 클릭한 다음 **[!UICONTROL 설정]** ![](assets/gear-icon-settings.png).
1. 왼쪽 패널에서 **[!UICONTROL 문서]** > **[!UICONTROL [!DNL SharePoint]통합]**.
1. 을(를) 클릭합니다 [!DNL SharePoint] 업데이트할 통합을 클릭한 다음 **[!UICONTROL 편집]**.
1. 새 클라이언트 암호를 **[!UICONTROL 클라이언트 암호]** 필드.
1. **[!UICONTROL 저장]**&#x200B;을 클릭합니다.



## 기존 SharePoint 통합 설정 지침

>[!IMPORTANT]
>
>이 통합은 더 이상 사용되지 않습니다. 여기서의 지침은 정보용이며 곧 제거될 예정입니다.


Workfront은에 연결합니다. [!DNL SharePoint] 사용자의 인증 및 권한 부여를 위해 대부분의 웹 기반 통합에서 사용하는 표준인 OAuth 2.0을 사용하는 온라인.

OAuth를 구성하려면 다음을 생성해야 합니다. [!DNL SharePoint] 사이트 및 사이트 앱 [!DNL SharePoint]. 이 프로세스는 다음 섹션에 설명되어 있습니다.

OAuth에 대한 자세한 내용은 [http://oauth.net](http://oauth.net/).

>[!TIP]
>
>다음 사이에 정보를 쉽게 복사하여 붙여넣을 수 있도록 지원 [!DNL Workfront] 및 [!DNL SharePoint] 이 단계에서는 두 응용 프로그램을 별도의 탭에서 열어 두는 것이 좋습니다.

* [만들기 및 구성 [!DNL SharePoint] 사이트](#create-and-configure-a-sharepoint-site)
* [사이트 앱에 쓰기 권한 부여](#grant-write-permissions-to-the-site-app)
* [만들기 [!DNL Workfront] [!DNL SharePoint] 통합 인스턴스](#create-a-workfront-sharepoint-integration-instance)
* [통합 완료](#complete-your-integration)
* [문서 추가](#add-documents)

### 만들기 및 구성 [!DNL SharePoint] 사이트  {#create-and-configure-a-sharepoint-site}

주문 [!DNL Workfront] 을(를) 통해 인증 [!DNL SharePoint], [!DNL Workfront] 를 사용하는 마스터 사이트를 사용할 수 있습니다. [!UICONTROL 전체 제어] 권한 수준 또는 특정 관리 권한. 이 마스터 사이트는 의 인증 진입점 역할을 합니다. [!DNL Workfront].

을(를) 만들고 구성하려면 [!DNL SharePoint] 사이트:

1. (선택 사항) 조직의 루트 사이트를 사용하지 않으려면에서 마스터 사이트를 만들 수 있습니다. [!DNL SharePoint].

   자세한 내용은 다음을 참조하십시오. [사이트 만들기](https://docs.microsoft.com/en-us/sharepoint/create-site-collection) 다음에서 [!DNL Microsoft] 설명서입니다.

   * 다음 항목 선택 **[!UICONTROL 팀 사이트]** 옵션을 사용하여 사이트를 만들 수 있습니다.

1. (조건부) 1단계에서 사이트를 만든 경우 방금 만든 사이트로 이동합니다.

   또는

   1단계에서 사이트를 만들지 않은 경우 조직의 루트 사이트로 이동합니다.

1. 추가 `/_layouts/15/appregnew.aspx` 을 클릭하여 브라우저 창의 맨 위에 있는 검색 막대에서 URL의 끝으로 이동합니다.
1. 다음 필드를 구성합니다.

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader"> <p>[!UICONTROL 클라이언트 ID]</p> </td> 
      <td> <p>클릭 <strong>[!UICONTROL Generate]</strong> 클라이언트 ID를 생성합니다. 이 ID를 보안 위치에 복사합니다. 나중에 를 설정할 때 사용합니다. [!DNL SharePoint] 통합 위치 [!DNL Workfront].</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"> <p>[!UICONTROL 클라이언트 암호]</p> </td> 
      <td> <p>클릭 <strong>[!UICONTROL Generate]</strong> 클라이언트 암호를 생성합니다. 이 암호를 안전한 위치에 복사합니다. 나중에 를 설정할 때 사용합니다. [!DNL SharePoint] 통합 위치 [!DNL Workfront].</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"> <p>제목</p> </td> 
      <td> <p>다음과 같은 제목 입력 [!DNL Workfront] 사이트 앱. 문서를 추가할 때 이 제목이 표시됩니다.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"> <p>[!UICONTROL 앱 도메인]</p> </td> 
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

이 시점에서 사이트 앱을 정상적으로 만들고 다음 내에 등록했습니다. [!DNL Workfront]. 이 사이트 앱은에서 앱 주도자라고도 합니다. [!DNL SharePoint]. 테넌트 내에 있습니다. 새 사이트 앱은 테넌트 내의 사이트 모음에 자동으로 액세스할 수 없습니다. 각 사이트 모음에 대해 명시적으로 권한을 부여해야 합니다. 아래 단계에서는 사이트 모음에 새 사이트 앱에 쓰기 권한을 부여하는 방법을 보여 줍니다. 아래에 추가한 각 사이트 모음에 대해 이 단계를 반복합니다 [!UICONTROL 사이트 모음 표시] 위의 단계에서 다음을 수행합니다.

이 사이트 앱에는 다음이 있어야 합니다. [!UICONTROL 쓰기] 사용자가 액세스해야 하는 사이트 모음에 대한 권한 [!DNL Workfront].

1. 의 URL에 &#39;/_layouts/15/appinv.aspx&#39; 추가 [!DNL Sharepoint].

   **예:**

   ```
   https://mycompany.sharepoint.com/sites/mysite/_layouts/15/appinv.aspx
   ```

1. 다음 필드 구성

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">[!UICONTROL 앱 ID]</td> 
      <td> <p>만든 클라이언트 ID를 추가합니다 <a href="#create-and-configure-a-sharepoint-site" class="MCXref xref">만들기 및 구성 [!DNL SharePoint] 사이트 </a>및 클릭 <strong>[!UICONTROL 조회]</strong>.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"> <p>[!UICONTROL Client] / [!UICONTROL App Domain] / [!UICONTROL 리디렉션 URL]</p> </td> 
      <td> <p>[!UICONTROL 조회]를 클릭하면 자동으로 채워집니다.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL 권한 요청 XML]</td> 
      <td> <p>다음 XML을 [!UICONTROL 권한 요청 XML] 필드에 복사합니다. 추가 공백 없이 표시된 대로 정확하게 추가되었는지 확인하십시오. 오류를 방지하기 위해.</p> 
      <div></a> 
      <div style="mc-code-lang: XML;" class="codeSnippetBody" data-mc-continue="False" data-mc-line-number-start="1" data-mc-use-line-numbers="False"> 
       <pre></pre></div></div></td></tr></tbody></table>

1. Click **[!UICONTROL Create]**.
1. 표시되는 대화 상자에서 **[!UICONTROL 신뢰]**.
1. 를 클릭하여 사이트 앱에서 사이트 모음에 액세스할 수 있는지 확인합니다. **[!UICONTROL 사이트 모음 앱 권한]** 링크 위치 [!UICONTROL 사이트 설정].
1. 나머지 사이트 모음에 대해 위의 단계를 반복한 다음 을 사용하여 계속합니다. [만들기 [!DNL Workfront] [!DNL SharePoint] 통합 인스턴스](#create-a-workfront-sharepoint-integration-instance).

### 만들기 [!DNL Workfront] [!DNL SharePoint] 통합 인스턴스 {#create-a-workfront-sharepoint-integration-instance}

에서 사이트 앱을 만든 경우 [!DNL SharePoint], 이제 사이트 앱의 정보를 [!DNL Workfront]. 사이트 앱은 앱 주체로서 사이트 모음 내의 문서에 액세스하기 위해 OAuth 요청이 수행되는 통로 역할을 합니다.

1. 에 로그인 [!DNL Workfront] 관리자입니다.
1. 다음을 클릭합니다. **[!UICONTROL 메인 메뉴]** 아이콘 ![](assets/main-menu-icon.png) Adobe Workfront의 오른쪽 상단에서 을(를) 클릭한 다음 **[!UICONTROL 설정]** ![](assets/gear-icon-settings.png).

1. 왼쪽 패널에서 **[!UICONTROL 문서]** > **[!UICONTROL [!DNL SharePoint]통합]**.
1. 클릭 **[!UICONTROL 추가[!DNL SharePoint]]**.
1. 다음 필드를 구성합니다.

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader"> <p>[!UICONTROL 이름]</p> </td> 
      <td> <p>에 대한 이름 입력 [!DNL SharePoint] 통합. 사용자가 [!UICONTROL Add] &gt; [!UICONTROL From] 'name of integration'을 클릭하면 이 이름이 표시됩니다. </p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"> <p>[!UICONTROL [!DNL SharePoint] 호스트 인스턴스]</p> </td> 
      <td> <p><code>&lt;YourDomain&gt;.sharepoint.com</code> </p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"> <p>[!UICONTROL [!DNL Azure] 액세스 도메인]</p> </td> 
      <td> <p><code>&lt;YourDomain&gt;.onmicrosoft.com</code> </p> <p>사용자가 을 통해 인증하는 데 사용할 기본 사이트를 나타냅니다. [!UICONTROL]과(와) 동일한 도메인일 수 있습니다. [!DNL SharePoint] 호스트 인스턴스].</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"> <p>
      </p> </td> 
      <td> <b>중요 사항</b> 사이트 모음은 레거시에서만 사용됩니다. [!DNL SharePoint] 통합.
       <ul> 
        <li> <p><b>조직의 루트 사이트를 사용하는 경우</b><b>:</b> </p> <p>입력 <code>/</code></p> </li> 
        <li> <p><b>마스터 사이트 및 하위 사이트를 사용하는 경우:</b> </p> <p><b>중요 사항</b>: [!DNL Microsoft SharePoint] 는 더 이상 하위 사이트 사용을 권장합니다.</p> <p>위의 섹션에서 만든 사이트 모음의 URL 줄기를 입력합니다.</p> <p>.com 뒤에 있는 URL의 섹션입니다.</p> <p>예: URL <code>https://mycompany.sharepoint.com/sites/mysite</code>, 줄기는 다음과 같습니다 <code>/sites/mysite</code>.</p> </li> 
       </ul> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL [!DNL SharePoint] 클라이언트 ID]</td> 
      <td>생성한 클라이언트 ID를 입력합니다 <a href="#create-and-configure-a-sharepoint-site" class="MCXref xref">만들기 및 구성 [!DNL SharePoint] 사이트 </a>.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL [!DNL SharePoint] 클라이언트 암호]</td> 
      <td>에서 생성한 클라이언트 암호 입력 <a href="#create-and-configure-a-sharepoint-site" class="MCXref xref">만들기 및 구성 [!DNL SharePoint] 사이트 </a>.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL 보이는 사이트 모음]</td> 
      <td> <b>중요 사항</b> 사이트 모음은 레거시에서만 사용됩니다. [!DNL SharePoint] 통합.
       <ul> 
        <li> <p><b> 조직의 루트 사이트를 사용하는 경우</b><b>:</b> </p> <p>입력 <code>/</code></p> </li> 
        <li> <p><b>마스터 사이트 및 하위 사이트를 사용하는 경우:</b> </p> <p><b>중요 사항</b>: [!DNL Microsoft SharePoint] 는 더 이상 하위 사이트 사용을 권장합니다.</p> <p>에 추가할 각 하위 사이트 [!DNL SharePoint] 통합에서 하위 사이트의 줄기를 입력합니다.</p> <p>예: URL<code>https://mycompany.sharepoint.com/sites/mysite/mysubsite</code>, 줄기는 다음과 같습니다 <code>/sites/mysite/mysubsite</code>.</p> <p><b>메모</b>:   <p>구성만 테스트하려면(하위 사이트 없음) 마스터 사이트의 스템을 입력합니다. </p> <p>예: URL <code> https://mycompany.sharepoint.com/sites/mysite</code>, 줄기는 다음과 같습니다 <code>/sites/mysite</code>.</p> <p>에 설명된 대로 구성을 테스트한 경우 <a href="#complete-your-integration" class="MCXref xref">통합 완료</a>을(를) 통해 마스터 사이트를 제거하고 하위 사이트를 입력해야 합니다.</p> 
          <ol> 
           <li value="1">다음을 클릭합니다. <strong>[!UICONTROL 주 메뉴]</strong> 아이콘 <img src="assets/main-menu-icon.png"> 의 오른쪽 위 모서리 [!DNL Adobe Workfront]을 클릭한 다음 을 클릭합니다 <strong>[!UICONTROL 설치]</strong> <img src="assets/gear-icon-settings.png">.<li><p>왼쪽 패널에서 <strong>[!UICONTROL 문서]</strong> &gt; <strong>[!UICONTROL [!DNL SharePoint] 통합]</strong>.</p></li><li><p>다음을 클릭합니다. [!DNL SharePoint] 설정 중인 통합을 클릭한 다음 편집을 클릭합니다.</p></li><li><p>[!UICONTROL Visible Site Collections] 필드에서 마스터 사이트에 대한 스템을 삭제합니다.</p></li><li><p>에 추가할 각 하위 사이트 [!DNL SharePoint] 통합에서 하위 사이트의 줄기를 입력합니다.</p></li><p>예: URL<code>https://mycompany.sharepoint.com/sites/mysite/mysubsite</code>, 줄기는 다음과 같습니다 <code>/sites/mysite/mysubsite</code>.</p></li> 
          </ol> </p> </li> 
       </ul> <p> </p> <p> </p> </td> 
     </tr> 
    </tbody> 
   </table>

1. **[!UICONTROL 저장]**&#x200B;을 클릭합니다
1. 계속 [통합 완료](#complete-your-integration).

### 통합 완료 {#complete-your-integration}

기본 구성이 거의 완료되었습니다.

1. Workfront에서 **[!UICONTROL 메인 메뉴]** 아이콘 ![](assets/main-menu-icon.png) Adobe Workfront의 오른쪽 상단에서 을(를) 클릭한 다음 **[!UICONTROL 문서]** ![](assets/document-icon.png).
1. 클릭 **[!UICONTROL 새로 추가]**.
1. 클릭 **[!UICONTROL 출처:]`<title of your [!DNL SharePoint] site>`** 드롭다운에서 을 클릭합니다.

   이 사이트를 신뢰하도록 초대하는 대화 상자가 나타납니다.

   >[!NOTE]
   >
   >이 대화 상자가 나타나지 않으면 [!DNL SharePoint] 통합이 올바르게 구성되지 않았습니다.

1. 클릭 **[!UICONTROL 신뢰]**.

### 문서 추가 {#add-documents}

이제 의 문서를 추가할 수 있습니다. [!DNL SharePoint] 사이트.

자세한 내용은 [외부 문서 연결 대상 [!DNL Workfront]](../../documents/adding-documents-to-workfront/link-documents-from-external-apps.md#linking-existing-documents) 위치: [외부 애플리케이션에서 문서 연결](../../documents/adding-documents-to-workfront/link-documents-from-external-apps.md)

>[!IMPORTANT]
>
>폴더를 연결한 사용자에게 외부 애플리케이션에 대한 액세스 권한이 더 이상 없는 경우 [!DNL Workfront] 은(는) 더 이상 폴더의 콘텐츠에 액세스할 수 없습니다. 예를 들어 원래 폴더를 연결한 사용자가 회사를 그만두는 경우 이러한 상황이 발생할 수 있습니다. 계속 액세스하려면 폴더에 대한 액세스 권한이 있는 사용자가 폴더를 다시 연결해야 합니다.

## 문제 해결

* [문제: 사용자는 다음을 사용할 때 인증 기반 오류가 발생합니다. [!DNL SharePoint] 통합.](#problem-users-experience-authentication-based-errors-when-using-the-sharepoint-integration)
* [문제: (으)로 [!DNL Workfront] 사용자, 새 사용자를 프로비저닝할 수 없음 [!DNL SharePoint] 인스턴스. 하려고 하면 오류가 표시됩니다.](#problem-as-a-workfront-user-i-am-unable-to-provision-a-new-sharepoint-instance-when-i-attempt-to-do-i-see-an-error)
* [문제: 찾아보기 시도 시 [!DNL SharePoint] 의 파일 [!DNL Workfront], 사이트 모음이 모두 또는 일부만 표시됩니다.](#problem-when-attempting-to-browse-sharepoint-files-in-workfront-i-do-not-see-any-or-all-of-my-site-collections)
* [문제: 의 이전에 연결된 폴더 및 문서에 액세스할 수 없음 [!DNL SharePoint].](#problem-i-cannot-access-previously-linked-folders-and-documents-in-sharepoint)

### 문제: 사용자는 다음을 사용할 때 인증 기반 오류가 발생합니다. [!DNL SharePoint] 통합. {#problem-users-experience-authentication-based-errors-when-using-the-sharepoint-integration}

솔루션:

사용자는 다음에 대한 적절한 권한이 있는 그룹의 구성원이어야 합니다. [!DNL SharePoint] 사이트.

을 사용하는 사용자 [!UICONTROL 전체 제어] 액세스는 다음에 필요한 모든 권한을 가집니다. [!DNL SharePoint] 통합. 사용자에게 전체 제어 액세스 권한을 부여하지 않으려면 다음 권한을 부여해야 합니다.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL 디자인]</p> </td> 
   <td> <p>보기, 추가, 업데이트, 삭제, 승인 및 사용자 지정 가능</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL 편집]</p> </td> 
   <td> <p>목록을 추가, 편집 및 삭제할 수 있고 목록 항목 및 문서를 보기, 추가, 업데이트 및 삭제할 수 있습니다.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Contribute]</p> </td> 
   <td> <p>목록 항목 및 문서를 보고, 추가하고, 업데이트하고, 삭제할 수 있습니다.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL 보기 전용]</p> </td> 
   <td> <p>페이지, 목록 항목 및 문서를 볼 수 있음(서버측 파일 핸들러가 있는 문서 유형은 브라우저에서 볼 수 있지만 다운로드할 수 없음)</p> </td> 
  </tr> 
 </tbody> 
</table>

권한 수준 만들기 및 편집에 대한 지침은 [권한 수준을 만들고 편집하는 방법](https://docs.microsoft.com/en-us/sharepoint/how-to-create-and-edit-permission-levels) Microsoft 설명서에서 확인할 수 있습니다.

### 문제: (으)로 [!DNL Workfront] 사용자, 새 사용자를 프로비저닝할 수 없음 [!DNL SharePoint] 인스턴스. 하려고 하면 오류가 표시됩니다. {#problem-as-a-workfront-user-i-am-unable-to-provision-a-new-sharepoint-instance-when-i-attempt-to-do-i-see-an-error}

솔루션:

이 문제는 다음 중 하나에서 비롯된 여러 가지 원인으로 인해 발생할 수 있습니다. [!DNL Workfront] 또는 [!DNL SharePoint]의 구성입니다. 다음을 확인합니다.

* 클라이언트 ID, 클라이언트 암호, 반환 URL 및 기타 구성 필드가 [!DNL Workfront] [!DNL SharePoint] 통합 인스턴스 및 [!DNL SharePoint] 사이트 앱.
* 사용자에게 다음이 적용됨: [!UICONTROL 전체 제어] 인증에 사용되는 사이트 모음에 대한 권한입니다.
* 사이트 앱은 [!UICONTROL 사이트 앱 권한] 대상: [!UICONTROL 사이트 모음] 인증에 사용됩니다.

### 문제: 찾아보기 시도 시 [!DNL SharePoint] 의 파일 [!DNL Workfront], 사이트 모음이 모두 또는 일부만 표시됩니다. {#problem-when-attempting-to-browse-sharepoint-files-in-workfront-i-do-not-see-any-or-all-of-my-site-collections}

솔루션:

에서 사이트 모음을 보려면 [!DNL Workfront], 다음 조건을 충족해야 합니다.

* 사이트 컬렉션이에 등록되어야 합니다. [!DNL Workfront] [!DNL SharePoint] 통합 인스턴스.

   에서 확인하려면 [!DNL Workfront]:

   1. 다음으로 이동 [!UICONTROL 설정] > [!UICONTROL 문서] > [!UICONTROL [!DNL SharePoint] 통합].
   1. 편집 [!DNL SharePoint] 통합 인스턴스 정보입니다.
   1. 사이트 모음이 다음 목록에 있는지 확인합니다. [!UICONTROL 사이트 모음 표시].

* 사용자는 의 사이트 모음에 대한 보기 액세스 권한이 있어야 합니다. [!DNL SharePoint].
* 에서 확인하려면 [!DNL SharePoint]로 이동합니다. [!DNL SharePoint]을 클릭하고 사이트 모음을 엽니다. > [!UICONTROL 설정] > [!UICONTROL 사이트 권한].
* 다음 [!DNL SharePoint] 사이트 앱은 사이트 모음에 액세스할 수 있어야 합니다.

   에서 확인하려면 [!DNL SharePoint]:

   1. 사이트 모음으로 이동 > [!UICONTROL 설정] > [!UICONTROL 사이트 앱 권한].
   1. 다음을 확인합니다. [!UICONTROL 사이트 앱] 사용한 사람 [!DNL Workfront] 이(가) 여기에 나열됩니다.
   1. (조건부) 사이트 앱이 목록에 없으면 _layouts/15/appinv.aspx을 사용하여 사이트 모음에 을 추가합니다.

      사이트 모음 추가에 대한 자세한 내용은 사이트 앱에 쓰기 권한 부여를 참조하십시오.

### 문제: 의 이전에 연결된 폴더 및 문서에 액세스할 수 없음 [!DNL SharePoint]. {#problem-i-cannot-access-previously-linked-folders-and-documents-in-sharepoint}

해결 방법:

을(를) 연결한 사용자가 [!DNL SharePoint] 폴더를 더 이상 인증할 수 없습니다. [!DNL Workfront] 은(는) 더 이상 폴더의 콘텐츠에 액세스할 수 없습니다. 예를 들어 원래 폴더를 연결한 사용자가 회사를 그만두는 경우 이러한 상황이 발생할 수 있습니다.

계속 액세스하려면 폴더에 대한 액세스 권한이 있는 사용자가 폴더를 다시 연결해야 합니다.

외부 공급자의 폴더 연결에 대한 자세한 내용은 [외부 애플리케이션에서 문서 연결](../../documents/adding-documents-to-workfront/link-documents-from-external-apps.md).

### 문제: 에서 문서를 추가하려고 할 때 &quot;404 찾을 수 없음&quot; 오류가 표시됩니다. [!DNL Sharepoint]

#### 해결 방법:

이 오류는 사이트 중 하나가에 구성된 경우 발생할 수 있습니다. [!UICONTROL 사이트 모음 표시] 목록이 Sharepoint에서 삭제되었습니다. 다음 확인: [!UICONTROL 사이트 모음 표시] sharepoint에서 삭제된 사이트를 모두 나열하고 제거합니다.
