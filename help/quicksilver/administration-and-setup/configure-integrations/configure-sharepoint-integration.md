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
source-git-commit: 2a5e793077e520e34fdbb9187ba17f1e1bde43e9
workflow-type: tm+mt
source-wordcount: '1573'
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

### SharePoint에서 문서 연결

SharePoint의 문서를 새 페이지를 통해 연결하는 방법에 대한 지침 [!DNL SharePoint] 통합, 참조 [외부 문서 연결 대상 [!DNL Workfront]](../../documents/adding-documents-to-workfront/link-documents-from-external-apps.md#link-an-external-document-to-workfront)

### SharePoint에 문서 보내기

SharePoint으로 문서를 전송하려면 다음 작업을 수행하십시오.

1. 다음을 클릭합니다. **전송 대상** 아이콘 ![전송 대상](assets/send-to-icon.png) SharePoint(Graph API)를 선택합니다.
1. (선택 사항) 검색 창에서 문서를 보낼 사이트 또는 폴더를 검색합니다.
1. 목록에서 사이트 또는 폴더를 선택합니다.

   * 사이트가 다음으로 표시됨 ![사이트 아이콘](assets/site-icon.png).

   * 폴더가 다음으로 표시됨 ![폴더 아이콘](assets/folder-icon.png).

   * 파일이 아이콘으로 표시되지 않습니다.

1. **저장**&#x200B;을 클릭합니다.


## 에 대한 보안, 액세스 및 인증 정보 [!DNL SharePoint] 통합

### 인증 및 권한 부여

[!DNL Workfront] 는 OAuth2를 사용하여 액세스 토큰 및 새로 고침 토큰을 검색합니다. 이 액세스 토큰은 모두와의 인증에 사용됩니다. [!DNL SharePoint] 영역.

### 액세스 및 권한

사용자가에 문서를 처음 추가할 때 [!DNL Workfront] 출처: [!DNL SharePoint], 다음 권한을 요청하는 화면으로 이동합니다.

| 액세스 | 이유 |
|---|---|
| 파일에 대한 전체 액세스 권한 보유 | 허용 [!DNL Workfront] 를 클릭하여 사용자의 파일에 액세스하여 에셋을 연결합니다. 문서를 보낼 때 [!DNL Workfront] 끝 [!DNL SharePoint], [!DNL Workfront] 에셋을 만들려면 액세스 권한이 필요합니다. |
| 모든 사이트 모음의 항목 읽기 | 허용 [!DNL Workfront] 에셋을 읽어 사용자 탐색을 활성화합니다. |
| 모든 사이트 모음의 항목 편집 또는 삭제 | 허용 [!DNL Workfront] 를 클릭하여 사이트 및 사이트 모음에 자산을 만듭니다. 삭제는 실패한 링크 시도 후 정리할 때만 사용됩니다. |
| 액세스 권한을 부여한 데이터에 대한 액세스 유지 | 허용 [!DNL Workfront] 새로 고침 토큰을 생성합니다. |
| 로그인 및 사용자 프로필 읽기 | 허용 [!DNL Workfront] OAuth2 로그인 플로우를 통해 액세스 토큰을 사용하여 사용자를 대신하여 작업을 수행합니다. |

이 액세스 권한은 사용자가 통합을 처음 사용할 때 부여되며 언제든지 취소할 수 있습니다.

액세스 권한과 관련하여 다음 사항을 고려하십시오. [!DNL SharePoint] 다음을 통해 [!DNL Workfront] [!DNL SharePoint] 통합:

* 이 통합에 대해 요청된 권한은 다음과 같습니다. **위임됨** 사용 권한.
* [!DNL Workfront] 는 통합에서 작업을 수행하는 데 필요한 최소 액세스를 요청합니다.
* 보기, 편집 또는 삭제 액세스 권한 [!DNL Adobe Workfront] 문서 연결 대상 [!DNL SharePoint] 에서 사용자의 액세스 권한을 기반으로 합니다. [!DNL Workfront]. 단, 탐색, 다운로드 또는 편집 [!DNL SharePoint] 파일 또는 폴더에 대한 액세스 권한 필요 [!DNL SharePoint], 그리고 이러한 작업에 대한 액세스는 [!DNL SharePoint].
* 사용자는 썸네일을 보고 다음에서 가져온 이미지를 미리 볼 수 있습니다. [!DNL SharePoint]에서 파일 및 폴더 이름을 볼 수 있습니다 [!DNL SharePoint], 로그인하지 않음 [!DNL SharePoint].
* 사용자의 액세스 토큰은 사용자가 오프라인 상태이고 다른 사용자가 연결된 폴더의 컨텐츠를 볼 때만 사용됩니다. [!DNL Workfront]. 액세스 토큰은 폴더의 문서가 추가, 제거 또는 편집되었는지 확인하는 데 사용됩니다.

### 보안

간의 모든 통신 [!DNL Workfront] 및 [!DNL SharePoint] 은 정보를 암호화하는 HTTPS를 통해 수행됩니다.

[!DNL Workfront] 에서 데이터를 저장, 복사 또는 복제하지 않음 [!DNL SharePoint]. 유일한 예외는 [!DNL Workfront] 에서 축소판 저장 [!DNL SharePoint] 를 클릭하여 목록 보기 및 미리 보기에 표시합니다.

에셋이에 처음 업로드된 경우 [!DNL Workfront]를 참조한 다음 (으)로 전송됨 [!DNL SharePoint], [!DNL Workfront] 는 사용자가 이전 버전의 를 다운로드할 수 있으므로 첫 번째 파일에 대한 데이터를 유지합니다. [!DNL Workfront] 문서. 문서를 만든 위치: [!DNL SharePoint], [!DNL Workfront] 는 해당 파일 데이터를 저장하지 않습니다.

## 레거시 구성 [!DNL SharePoint] 문서에 대한 지속적인 액세스를 위한 통합

사용자가 레거시를 통해 Workfront에 연결된 문서에 계속 액세스할 수 있도록 합니다 [!DNL SharePoint] 통합하려면 기존 액세스를 다시 구성해야 합니다. [!DNL SharePoint] 통합하고 SharePoint 클라이언트 암호를 최신 상태로 유지합니다.

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

<!--

## Instructions for setting up the legacy SharePoint integration

>[!IMPORTANT]
>
>This integration has been deprecated. The instructions here are for information only and will be removed in the near future.


Workfront connects to [!DNL SharePoint] Online using OAuth 2.0, a standard used by most web-based integrations for the authentication and authorization of users.

To configure OAuth, you need to create a [!DNL SharePoint] site and a Site App within [!DNL SharePoint]. This process is described in the following sections.

For more information about OAuth, see [http://oauth.net](http://oauth.net/).

>[!TIP]
>
>To make it easy to copy and paste information between [!DNL Workfront] and [!DNL SharePoint] in these steps, we recommend keeping both applications open in separate tabs.

* [Create and configure a [!DNL SharePoint] site](#create-and-configure-a-sharepoint-site) 
* [Grant write permissions to the site app](#grant-write-permissions-to-the-site-app) 
* [Create a [!DNL Workfront] [!DNL SharePoint] integration instance](#create-a-workfront-sharepoint-integration-instance) 
* [Complete your integration](#complete-your-integration) 
* [Add documents](#add-documents)

### Create and configure a [!DNL SharePoint] site  {#create-and-configure-a-sharepoint-site}

In order for [!DNL Workfront] to authenticate with [!DNL SharePoint], [!DNL Workfront] ca use a master site where users have the [!UICONTROL Full Control] permission level or specific Manage permissions. This master site acts as an Authentication Entry Point for [!DNL Workfront].

To create and configure a [!DNL SharePoint] Site:

1. (Optional) If you do not want to use your organization's root site, you can create a master site in [!DNL SharePoint].

   For instructions, visit [Create a site](https://docs.microsoft.com/en-us/sharepoint/create-site-collection) in the [!DNL Microsoft] Documentation.

   * Select the **[!UICONTROL Team Site]** option when creating the site.

1. (Conditional) If you created a site in step 1, go to the site you just created.

   Or

   If you did not create a site in step 1, go to your organization's root site.

1. Add `/_layouts/15/appregnew.aspx` to the end of the URL in the search bar at the top of your browser window.
1. Configure the following fields:

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader"> <p>[!UICONTROL Client ID]</p> </td> 
      <td> <p>Click <strong>[!UICONTROL Generate]</strong> to generate a Client ID. Copy this ID to a secure location. You will use it later when you set up the [!DNL SharePoint] integration in [!DNL Workfront].</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"> <p>[!UICONTROL Client Secret]</p> </td> 
      <td> <p>Click <strong>[!UICONTROL Generate]</strong> to generate a Client Secret. Copy this Secret to a secure location. You will use it later when you set up the [!DNL SharePoint] integration in [!DNL Workfront].</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"> <p>Title</p> </td> 
      <td> <p>Enter a title, such as [!DNL Workfront] Site App. Users see this title when adding documents..</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"> <p>[!UICONTROL App Domain]</p> </td> 
      <td> <p><code>my.workfront.com</code> </p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"> <p>[!UICONTROL Redirect URI]</p> </td> 
      <td> <p><code>https://oauth.my.workfront.com/oauth2/redirect</code> </p> </td> 
     </tr> 
    </tbody> 
   </table>

1. Click **[!UICONTROL Create]**
1. Continue to [Grant write permissions to the site app](#grant-write-permissions-to-the-site-app).

### Grant write permissions to the site app  {#grant-write-permissions-to-the-site-app}

At this point, you have successfully created a Site App and registered it within [!DNL Workfront]. This site app is also known as an app principal in [!DNL SharePoint]. It resides within your tenant. New site apps do not automatically have access to site collections within the tenant. Permissions must be granted explicitly, for each site collection. The steps below will show you how to grant Write permission to the new Site App a site collection. Repeat these steps for each of the site collections you added under [!UICONTROL Visible Site Collections] in the steps above.

This site app must have [!UICONTROL Write] permission to any site collections that users need to access through [!DNL Workfront].

1. Add '/_layouts/15/appinv.aspx' to the URL in [!DNL Sharepoint].

   **Example:**

   ```
   https://mycompany.sharepoint.com/sites/mysite/_layouts/15/appinv.aspx
   ```

1. Configure the following fields

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">[!UICONTROL App ID]</td> 
      <td> <p>Add the Client ID that you created in <a href="#create-and-configure-a-sharepoint-site" class="MCXref xref">Create and configure a [!DNL SharePoint] site </a>and click <strong>[!UICONTROL Lookup]</strong>.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"> <p>[!UICONTROL Client] / [!UICONTROL App Domain] / [!UICONTROL Redirect URL]</p> </td> 
      <td> <p>These automatically fill when you click [!UICONTROL Lookup].</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL Permission Request XML]</td> 
      <td> <p>Copy the following XML to the [!UICONTROL Permission Request XML] field. Make sure that it is added exactly as shown without additional spaces etc. in order to avoid errors.</p> 
      <div></a> 
      <div style="mc-code-lang: XML;" class="codeSnippetBody" data-mc-continue="False" data-mc-line-number-start="1" data-mc-use-line-numbers="False"> 
       <pre><code><span style="color: #63a35c; ">&lt;AppPermissionRequests&gt;</span><br><span style="color: #63a35c; ">&lt;AppPermissionRequest <span style="color: #795da3; ">Scope</span><span style="color: #df5000; ">="http://sharepoint/content/sitecollection/web"</span> <span style="color: #795da3; ">Right</span><span style="color: #df5000; ">="Write"</span>/&gt;</span><br><span style="color: #63a35c; ">&lt;/AppPermissionRequests&gt;</span></code></pre> 
      </div> 
      </div> </td> 
     </tr> 
    </tbody> 
   </table>

1. Click **[!UICONTROL Create]**. 
1. In the dialog that appears, click **[!UICONTROL Trust it]**.
1. Verify that the site app has access to the site collection by clicking the **[!UICONTROL Site collection app permissions]** link in [!UICONTROL Site Settings].
1. Repeat the steps above for the remaining site collections, then continue with [Create a [!DNL Workfront] [!DNL SharePoint] integration instance](#create-a-workfront-sharepoint-integration-instance).

### Create a [!DNL Workfront] [!DNL SharePoint] integration instance {#create-a-workfront-sharepoint-integration-instance}

When you have created a site app in [!DNL SharePoint], you can now copy information from the site app into [!DNL Workfront]. The site app is an app principal and acts as the conduit through which OAuth requests are made to access documents within site collections.

1. Log into [!DNL Workfront] as an administrator.
1. Click the **[!UICONTROL Main Menu]** icon ![](assets/main-menu-icon.png) in the upper-right corner of Adobe Workfront, then click **[!UICONTROL Setup]** ![](assets/gear-icon-settings.png).

1. In the left panel, click **[!UICONTROL Documents]** > **[!UICONTROL [!DNL SharePoint] Integration]**.
1. Click **[!UICONTROL Add [!DNL SharePoint]]**.
1. Configure the following fields:

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader"> <p>[!UICONTROL Name]</p> </td> 
      <td> <p>Enter a name for the [!DNL SharePoint] integration. Users see this name when they click [!UICONTROL Add] &gt; [!UICONTROL From] 'name of integration'. </p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"> <p>[!UICONTROL [!DNL SharePoint] Host Instance]</p> </td> 
      <td> <p><code>&lt;YourDomain&gt;.sharepoint.com</code> </p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"> <p>[!UICONTROL [!DNL Azure] Access Domain]</p> </td> 
      <td> <p><code>&lt;YourDomain&gt;.onmicrosoft.com</code> </p> <p>This refers to the Master Site that users will use to authenticate through. It is likely the same domain as the [!UICONTROL [!DNL SharePoint] Host Instance].</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"> <p>
      </p> </td> 
      <td> <b>Important</b> Site collections are used only in the Legacy [!DNL SharePoint] Integration.
       <ul> 
        <li> <p><b>If you are using your organization's root site</b><b>:</b> </p> <p>Enter <code>/</code></p> </li> 
        <li> <p><b>If you are using a master site and subsites:</b> </p> <p><b>IMPORTANT</b>: [!DNL Microsoft SharePoint] no longer recommends the use of subsites.</p> <p>Enter the URL stem for the site collection that you created in the section above.</p> <p>This is the section of the URL after .com.</p> <p>Example: for the URL <code>https://mycompany.sharepoint.com/sites/mysite</code>, the stem would be <code>/sites/mysite</code>.</p> </li> 
       </ul> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL [!DNL SharePoint] Client ID]</td> 
      <td>Enter the Client ID that you generated in <a href="#create-and-configure-a-sharepoint-site" class="MCXref xref">Create and configure a [!DNL SharePoint] site </a>.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL [!DNL SharePoint] Client Secret]</td> 
      <td>Enter the Client Secret that you generated in <a href="#create-and-configure-a-sharepoint-site" class="MCXref xref">Create and configure a [!DNL SharePoint] site </a>.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL Visible Site Collections]</td> 
      <td> <b>Important</b> Site collections are used only in the Legacy [!DNL SharePoint] integration.
       <ul> 
        <li> <p><b> If you are using your organization's root site</b><b>:</b> </p> <p>Enter <code>/</code></p> </li> 
        <li> <p><b>If you are using a master site and subsites:</b> </p> <p><b>IMPORTANT</b>: [!DNL Microsoft SharePoint] no longer recommends the use of subsites.</p> <p>For each subsite you want to add to your [!DNL SharePoint] integration, enter the stem of the subsite.</p> <p>Example: for the URL<code>https://mycompany.sharepoint.com/sites/mysite/mysubsite</code>, the stem would be <code>/sites/mysite/mysubsite</code>.</p> <p><b>NOTE</b>:   <p>If you want to test your configuration only (no subsites), enter the stem of the master site. </p> <p>Example: for the URL <code> https://mycompany.sharepoint.com/sites/mysite</code>, the stem would be <code>/sites/mysite</code>.</p> <p>When you have tested your configuration as described in <a href="#complete-your-integration" class="MCXref xref">Complete your integration</a>, you must remove the master site and enter the subsites.</p> 
          <ol> 
           <li value="1">Click the <strong>[!UICONTROL Main Menu]</strong> icon <img src="assets/main-menu-icon.png"> in the upper-right corner of [!DNL Adobe Workfront], then click <strong>[!UICONTROL Setup]</strong> <img src="assets/gear-icon-settings.png">.<li><p>In the left panel, click <strong>[!UICONTROL Documents]</strong> &gt; <strong>[!UICONTROL [!DNL SharePoint] Integration]</strong>.</p></li><li><p>Click the [!DNL SharePoint] integration you are setting up, then click Edit.</p></li><li><p>Delete the stem for the master site from the [!UICONTROL Visible Site Collections] field.</p></li><li><p>For each subsite you want to add to your [!DNL SharePoint] integration, enter the stem of the subsite.</p></li><p>Example: for the URL<code>https://mycompany.sharepoint.com/sites/mysite/mysubsite</code>, the stem would be <code>/sites/mysite/mysubsite</code>.</p></li> 
          </ol> </p> </li> 
       </ul> <p> </p> <p> </p> </td> 
     </tr> 
    </tbody> 
   </table>

1. Click **[!UICONTROL Save]**
1. Continue to [Complete your integration](#complete-your-integration).

### Complete your integration {#complete-your-integration}

The basic configuration is almost complete.

1. In Workfront, Click the **[!UICONTROL Main Menu]** icon ![](assets/main-menu-icon.png) in the upper-right corner of Adobe Workfront, then click **[!UICONTROL Documents]** ![](assets/document-icon.png).
1. Click **[!UICONTROL Add new]**.
1. Click **[!UICONTROL From] `<title of your [!DNL SharePoint] site>`** in the dropdown.

   A dialog that invites you to Trust this site appears.

   >[!NOTE]
   >
   >If this dialog does not appear, your [!DNL SharePoint] integration is not configured correctly.

1. Click **[!UICONTROL Trust it]**.

### Add documents {#add-documents}

You can now add documents from your [!DNL SharePoint] site.

For instructions, see [Link an external document to [!DNL Workfront]](../../documents/adding-documents-to-workfront/link-documents-from-external-apps.md#linking-existing-documents) in [Link documents from external applications](../../documents/adding-documents-to-workfront/link-documents-from-external-apps.md)

>[!IMPORTANT]
>
>If the user who linked a folder no longer has access to the external application, [!DNL Workfront] can no longer access the contents of the folder. This may happen, for example, if the user who originally linked the folder leaves the company. To ensure continued access, a user with access to the folder must re-link the folder.
> 

-->

## 문제 해결

* [문제: 사용자는 다음을 사용할 때 인증 기반 오류가 발생합니다. [!DNL SharePoint] 통합.](#problem-users-experience-authentication-based-errors-when-using-the-sharepoint-integration)
* [문제: 찾아보기 시도 시 [!DNL SharePoint] 의 파일 [!DNL Workfront], 사이트 모음이 모두 또는 일부만 표시됩니다.](#problem-when-attempting-to-browse-sharepoint-files-in-workfront-i-do-not-see-any-or-all-of-my-site-collections)
* [문제: 의 이전에 연결된 폴더 및 문서에 액세스할 수 없음 [!DNL SharePoint].](#problem-i-cannot-access-previously-linked-folders-and-documents-in-sharepoint)

### 문제: 사용자는 다음을 사용할 때 인증 기반 오류가 발생합니다. [!DNL SharePoint] 통합. {#problem-users-experience-authentication-based-errors-when-using-the-sharepoint-integration}

솔루션:

사용자에게 다음에 대한 적절한 권한이 있어야 합니다. [!DNL SharePoint] 사이트.

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

<!--

### Problem: As a [!DNL Workfront] user, I am unable to provision a new [!DNL SharePoint] instance. When I attempt to do I see an error. {#problem-as-a-workfront-user-i-am-unable-to-provision-a-new-sharepoint-instance-when-i-attempt-to-do-i-see-an-error}

Solutions:

This can be caused by a number of things, originating in either [!DNL Workfront] or [!DNL SharePoint]'s configuration. Verify that:

* The Client ID, Client Secret, return URL and other configuration fields are correctly mapped between the [!DNL Workfront] [!DNL SharePoint] Integration instance and the [!DNL SharePoint] Site App.
* The user has [!UICONTROL Full Control] permission to the Site Collection used for authentication.
* The Site App is listed under [!UICONTROL Site App Permissions] for the [!UICONTROL Site Collection] used for authentication.

-->

### 문제: 찾아보기 시도 시 [!DNL SharePoint] 의 파일 [!DNL Workfront], 사이트 모음이 모두 또는 일부만 표시됩니다. {#problem-when-attempting-to-browse-sharepoint-files-in-workfront-i-do-not-see-any-or-all-of-my-site-collections}

솔루션:

에서 사이트 모음을 보려면 [!DNL Workfront], 다음 조건을 충족해야 합니다.

<!--

* The site collection must be registered in the [!DNL Workfront] [!DNL SharePoint] Integration instance.

  To verify this in [!DNL Workfront]:

   1. Go to [!UICONTROL Setup] > [!UICONTROL Documents] > [!UICONTROL [!DNL SharePoint] Integration].
   1. Edit the [!DNL SharePoint] Integration instance information.
   1. Verify that the site collection is listed under [!UICONTROL Visible Site Collections].
   -->

* 사용자는 의 사이트 모음에 대한 보기 액세스 권한이 있어야 합니다. [!DNL SharePoint].

  에서 확인하려면 [!DNL SharePoint]로 이동합니다. [!DNL SharePoint]을 클릭하고 사이트 모음을 엽니다. > [!UICONTROL 설정] > [!UICONTROL 사이트 권한].
<!--* The [!DNL SharePoint] Site App must have access to the site collection.

  To verify this in [!DNL SharePoint]:

   1. Go to the site collection > [!UICONTROL Settings] > [!UICONTROL Site app permissions].
   1. Ensure that the [!UICONTROL Site App] used by [!DNL Workfront] is listed here.
   1. (Conditional) If the Site App is not listed, add to the site collection using _layouts/15/appinv.aspx.

      For information about adding the site collection, see Granting Write Permissions To The Site App.
      
-->

### 문제: 의 이전에 연결된 폴더 및 문서에 액세스할 수 없음 [!DNL SharePoint]. {#problem-i-cannot-access-previously-linked-folders-and-documents-in-sharepoint}

해결 방법:

을(를) 연결한 사용자가 [!DNL SharePoint] 폴더를 더 이상 인증할 수 없습니다. [!DNL Workfront] 은(는) 더 이상 폴더의 콘텐츠에 액세스할 수 없습니다. 예를 들어 원래 폴더를 연결한 사용자가 회사를 그만두는 경우 이러한 상황이 발생할 수 있습니다.

계속 액세스하려면 폴더에 대한 액세스 권한이 있는 사용자가 폴더를 다시 연결해야 합니다.

외부 공급자의 폴더 연결에 대한 자세한 내용은 [외부 애플리케이션에서 문서 연결](../../documents/adding-documents-to-workfront/link-documents-from-external-apps.md).

<!--

### Problem: I see a "404 not found" error when attempting to add a document from [!DNL Sharepoint]

#### Solution:

This error might occur if one of the sites configured in the [!UICONTROL Visible Site Collections] list has been deleted in Sharepoint. Check the [!UICONTROL Visible Site Collections] list, and remove any sites that have been deleted in Sharepoint.-->