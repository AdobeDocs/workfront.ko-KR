---
title: ' [!DNL SharePoint] 통합 구성'
user-type: administrator
product-area: system-administration;workfront-integrations;setup
navigation-topic: administrator-integrations
description: ' [!DNL Workfront] 을(를)  [!DNL SharePoint] 온라인과 통합하여 사용자에게 Workfront 내에서  [!DNL SharePoint] 문서로 이동하고, 연결하고, 추가할 수 있는 기능을 제공할 수 있습니다. 제공된 기능은 다른  [!DNL Workfront] 문서 통합의 기능과 유사합니다.'
author: Becky
feature: System Setup and Administration, [!DNL Workfront] Integrations and Apps, Digital Content and Documents
role: Admin
exl-id: fd45e1bc-9a35-4960-a73a-ff845216afe4
source-git-commit: 3c87c88245e79581c2a880c13038bcedb24caf4b
workflow-type: tm+mt
source-wordcount: '1729'
ht-degree: 0%

---

# [!DNL SharePoint] 통합 구성

<!--Audited: 12/2023-->

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">**DON'T DELETE, DRAFT OR HIDE THIS ARTICLE. IT IS LINKED TO THE PRODUCT, THROUGH THE CONTEXT SENSITIVE HELP LINKS. **</p>
-->

>[!IMPORTANT]
>
>새로운 [!DNL SharePoint] 통합은 22.3 릴리스(2022년 7월)를 사용하여 프로덕션에 릴리스되었습니다.
>
>* 사용자는 이전 [!DNL SharePoint] 통합을 통해 연결된 문서에 계속 액세스할 수 있지만 이를 통해 문서를 연결할 수는 없습니다. SharePoint의 문서를 연결하려면 새 [!DNL SharePoint] 통합을 사용해야 합니다.
>
>* 기존 SharePoint 통합이 구성되어 있지 않으면 추가할 수 없습니다. 문서를 SharePoint에 연결하려면 새 SharePoint 통합을 사용해야 합니다.
>
>* 새 SharePoint 통합은 관리자가 구성하지 않아도 되며, 개별 사용자가 설정할 수 있습니다. 그러나 새 SharePoint 통합으로 원활하게 전환하려면 Workfront 관리자가 Workfront 설정 영역에서 일부 설정을 변경해야 합니다.
>
>    자세한 내용 및 지침은 이 문서의 [문서에 계속 액세스할 수 있도록 기존 SharePoint 통합 구성](#configure-the-legacy-sharepoint-integration-for-continued-access-to-documents)을 참조하십시오.
>    
>* 사용자가 현재 새 통합을 통해 기존 [!DNL SharePoint] 통합을 통해 연결된 문서를 연결하는 것이 좋습니다.
>    
>    문서 연결에 대한 지침은 [외부 응용 프로그램에서 문서 연결](../../documents/adding-documents-to-workfront/link-documents-from-external-apps.md)을 참조하십시오.

[!DNL Workfront]을(를) [!DNL SharePoint Online]과(와) 통합하여 사용자에게 Workfront 내에서 [!DNL SharePoint]개의 문서로 이동하고, 연결하고, 추가할 수 있는 기능을 제공할 수 있습니다. 제공된 기능은 [!DNL Google Drive], [!DNL Box] 및 [!DNL Dropbox]과(와) 같은 다른 [!DNL Workfront] 통합의 기능과 유사합니다.

이 통합은 [!DNL SharePoint Online]과만 호환됩니다. [!DNL SharePoint]의 온-프레미스 인스턴스는 지원되지 않습니다.

## 액세스 요구 사항

+++ 을 확장하여 이 문서의 기능에 대한 액세스 요구 사항을 봅니다.

이 문서의 단계를 수행하려면 다음이 있어야 합니다.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] 플랜</td> 
   <td>임의</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] 라이센스</td> 
   <td>새로운 기능: 표준 <p>또는</p><p>현재: 플랜</p></td> 
  </tr> 
  <tr> 
   <td role="rowheader">액세스 수준 구성*</td> 
   <td>[!DNL Workfront] 관리자여야 합니다. </td> 
  </tr> 
 </tbody> 
</table>

이 표의 정보에 대한 자세한 내용은 [Workfront 설명서의 액세스 요구 사항](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)을 참조하십시오.

+++

## 전제 조건

[!DNL SharePoint] 통합을 수정하거나 구성하려면 [!DNL SharePoint]에 필요한 액세스 또는 권한이 있어야 합니다.

## 새로운 SharePoint 통합을 통해 문서 연결

개별 사용자는 새 [!DNL SharePoint] 통합을 통해 문서를 연결할 수 있습니다. 통합에는 관리자 구성이 필요하지 않습니다. 대신 사용자가 문서를 연결할 때 [!DNL Microsoft] 계정에 로그온하면 통합에서 사용자의 [!DNL SharePoint]에서 사용 가능한 문서에 액세스할 수 있습니다.

사용자가 처음으로 [!DNL Workfront] [!DNL SharePoint] 통합을 [!DNL SharePoint] 계정에 연결하면 [!DNL Workfront]이(가) [!UICONTROL SharePoint] 계정과 상호 작용할 때 사용하는 모든 권한을 확인하고 이에 동의하거나 Microsoft 관리자에게 권한을 요청할 수 있습니다. 읽기 권한을 사용하면 [!DNL Workfront]이(가) [!DNL SharePoint]의 파일을 보고 액세스할 수 있으며 쓰기 권한을 사용하면 사용자가 [!DNL SharePoint]에 파일을 업로드할 수 있습니다.

![Sharepoint 권한](assets/sharepoint-permissions.png)

새 [!DNL SharePoint] 통합을 통해 문서를 연결하는 방법에 대한 지침은 [외부 문서 연결 [!DNL Workfront]](../../documents/adding-documents-to-workfront/link-documents-from-external-apps.md#link-an-external-document-to-workfront)을 참조하세요.

>[!NOTE]
>
>* 조직의 Microsoft 구성에 따라 사용자에게 &quot;권한 요청&quot; 페이지 대신 &quot;승인 필수&quot; 페이지가 표시될 수 있습니다. 이 경우 사용자는 이 페이지를 사용하여 조직의 Microsoft 관리자가 Sharepoint 통합에 대한 권한을 부여하도록 요청할 수 있습니다.
>
>* [!DNL SharePoint] 통합은 단일 [!DNL SharePoint] 인스턴스에 연결할 수 있습니다. 따라서 사용자는 하나의 [!DNL SharePoint]에 대한 통합을 설정할 수 있지만, 두 번째 [!DNL SharePoint]에 대한 및 문서에 대한 권한이 있어도 두 번째 [!DNL SharePoint]에 대한 통합을 설정할 수 없습니다.
>
>* 사용자는 [!DNL Workfront] [!DNL SharePoint] 통합을 통해 [!DNL SharePoint] 계정에 있는 동일한 사이트, 컬렉션, 폴더, 하위 폴더 및 파일에 액세스할 수 있습니다.

### SharePoint에서 문서 연결

새 [!DNL SharePoint] 통합을 통해 SharePoint의 문서를 연결하는 방법에 대한 지침은 [외부 문서를 연결 [!DNL Workfront]](../../documents/adding-documents-to-workfront/link-documents-from-external-apps.md#link-an-external-document-to-workfront)을 참조하십시오.

### SharePoint에 문서 보내기

SharePoint으로 문서를 전송하려면 다음 작업을 수행하십시오.

1. **전송 대상** 아이콘 ![전송 대상](assets/send-to-icon.png)을 클릭하고 SharePoint(Graph API)를 선택합니다.
1. (선택 사항) 검색 창에서 문서를 보낼 사이트 또는 폴더를 검색합니다.
1. 목록에서 사이트 또는 폴더를 선택합니다.

   * 사이트가 ![사이트 아이콘](assets/site-icon.png)(으)로 표시되어 있습니다.

   * 폴더가 ![폴더 아이콘](assets/folder-icon.png)(으)로 표시되어 있습니다.

   * 파일이 아이콘으로 표시되지 않습니다.

1. **저장**&#x200B;을 클릭합니다.


## [!DNL SharePoint] 통합에 대한 보안, 액세스 및 권한 부여 정보

### 인증 및 권한 부여

[!DNL Workfront]은(는) OAuth2를 사용하여 액세스 토큰과 새로 고침 토큰을 검색합니다. 이 액세스 토큰은 모든 [!DNL SharePoint] 영역의 인증에 사용됩니다.

### 액세스 및 권한

사용자가 [!DNL SharePoint]에서 [!DNL Workfront]에 문서를 처음 추가하면 해당 사용자는 SharePoint 통합에 대한 권한을 부여할 수 있는 권한 요청 페이지로 이동됩니다.

>[!NOTE]
>
>조직의 Microsoft 구성에 따라 사용자에게 &quot;권한 요청&quot; 페이지 대신 &quot;승인 필수&quot; 페이지가 표시될 수 있습니다. 이 경우 사용자는 이 페이지를 사용하여 조직의 Microsoft 관리자가 Sharepoint 통합에 대한 권한을 부여하도록 요청할 수 있습니다.

다음 권한이 요청됩니다.

| 액세스 | 이유 |
|---|---|
| 파일에 대한 전체 액세스 권한 보유 | [!DNL Workfront]이(가) 사용자의 파일에 액세스하여 자산을 연결할 수 있도록 허용합니다. 문서를 [!DNL Workfront]에서 [!DNL SharePoint](으)로 보낼 때 [!DNL Workfront]은(는) 에셋을 만들 수 있는 액세스 권한이 필요합니다. |
| 모든 사이트 모음의 항목 읽기 | [!DNL Workfront]이(가) 에셋을 읽어서 사용자 탐색을 사용하도록 허용합니다. |
| 모든 사이트 모음의 항목 편집 또는 삭제 | [!DNL Workfront]에서 사이트 및 사이트 모음에 자산을 만들 수 있습니다. 삭제는 실패한 링크 시도 후 정리할 때만 사용됩니다. |
| 액세스 권한을 부여한 데이터에 대한 액세스 유지 | [!DNL Workfront]이(가) 새로 고침 토큰을 생성할 수 있도록 허용합니다. |
| 로그인 및 사용자 프로필 읽기 | [!DNL Workfront]이(가) OAuth2 로그인 흐름을 통해 액세스 토큰을 사용하여 사용자를 대신할 수 있습니다. |

* 이 액세스 권한은 사용자가 통합을 처음 사용할 때 부여되며 언제든지 취소할 수 있습니다.
* 이 통합에 대해 요청된 권한은 **위임됨** 권한입니다.
* [!DNL Workfront]이(가) 통합에서 작업을 수행하는 데 필요한 최소 액세스 권한을 요청합니다.
* [!DNL SharePoint]에 연결된 [!DNL Adobe Workfront] 문서를 보거나 편집하거나 삭제할 수 있는 액세스는 [!DNL Workfront]에서 사용자의 액세스 권한을 기반으로 합니다. 그러나 [!DNL SharePoint] 파일 또는 폴더를 탐색하거나 다운로드하거나 편집하려면 [!DNL SharePoint]에 액세스해야 하며 이러한 작업에 대한 액세스는 [!DNL SharePoint]에 의해 제어됩니다.
* 사용자는 [!DNL SharePoint]에 로그인하지 않고도 [!DNL SharePoint]에서 가져온 썸네일을 보고 이미지를 미리 볼 수 있으며 [!DNL SharePoint]에서 파일 및 폴더 이름을 볼 수 있습니다.
* 사용자의 액세스 토큰은 사용자가 오프라인 상태이고 다른 사용자가 [!DNL Workfront]에 연결된 폴더의 콘텐츠를 볼 때만 사용됩니다. 액세스 토큰은 폴더의 문서가 추가, 제거 또는 편집되었는지 확인하는 데 사용됩니다.

### 보안

[!DNL Workfront]과(와) [!DNL SharePoint] 사이의 모든 통신은 HTTPS를 통해 수행되며, 이 HTTPS는 정보를 암호화합니다.

[!DNL Workfront]은(는) [!DNL SharePoint]의 데이터를 저장, 복사 또는 복제하지 않습니다. 유일한 예외는 [!DNL Workfront]이(가) [!DNL SharePoint]의 축소판을 저장하여 목록 보기와 미리 보기에 표시한다는 것입니다.

에셋을 [!DNL Workfront]에 업로드한 다음 [!DNL SharePoint](으)로 보낸 경우 사용자가 이전 버전의 [!DNL Workfront] 문서를 다운로드할 수 있으므로 [!DNL Workfront]에서 첫 번째 파일에 대한 데이터를 유지합니다. [!DNL SharePoint]에서 문서를 만든 경우 [!DNL Workfront]은(는) 해당 파일 데이터를 저장하지 않습니다.

## 문서에 계속 액세스할 수 있도록 레거시 [!DNL SharePoint] 통합을 구성하십시오.

사용자가 이전 [!DNL SharePoint] 통합을 통해 Workfront에 연결된 문서에 계속 액세스할 수 있도록 하려면 이전 [!DNL SharePoint] 통합에 대한 액세스를 다시 구성하고 SharePoint 클라이언트 암호를 최신 상태로 유지해야 합니다.

* [기존  [!DNL SharePoint] 통합에 대한 액세스 다시 구성](#reconfigure-access-to-the-legacy-sharepoint-integration)
* [기존  [!DNL SharePoint] 통합에 계속 액세스할 수 있도록 클라이언트 암호 구성](#configure-the-client-secret-for-continued-access-to-the-legacy-sharepoint-integration)

### 레거시 [!DNL SharePoint] 통합에 대한 액세스를 다시 구성하십시오.

기존 [!DNL SharePoint] 통합을 다시 구성하면 사용자가 기존 [!DNL SharePoint] 통합을 통해 연결된 문서에 액세스할 수 있으며 사용자가 해당 통합을 통해 새 문서에 연결할 수 없도록 할 수 있습니다.

>[!NOTE]
>
> * 기존 [!DNL SharePoint] 통합에는 &quot;[!DNL SharePoint]&quot; 레이블이 지정됩니다.
> * 새 [!DNL SharePoint] 통합에는 &quot;[!UICONTROL [!DNL SharePoint](Graph API)]&quot; 레이블이 지정됩니다.

1. Adobe Workfront의 오른쪽 상단에 있는 **[!UICONTROL 주 메뉴]** 아이콘 ![주 메뉴](assets/main-menu-icon.png)을 클릭하거나(가능한 경우) 왼쪽 상단에 있는 **[!UICONTROL 주 메뉴]** 아이콘 ![주 메뉴](/help/_includes/assets/main-menu-icon-left-nav.png)을 클릭한 다음 **[!UICONTROL 설정]** ![설정 아이콘](/help/_includes/assets/gear-icon-setup.png)을 클릭합니다.
1. 왼쪽 탐색에서 **[!UICONTROL 문서]**&#x200B;를 선택한 다음 **[!UICONTROL 클라우드 공급자]**&#x200B;를 선택하십시오.
1. **[!DNL SharePoint]** 옵션과 **[!UICONTROL [!DNL SharePoint](Graph API)]** 옵션이 모두 활성화되어 있는지 확인하십시오.
1. **[!UICONTROL 저장]**&#x200B;을 클릭합니다.
1. 왼쪽 탐색에서 **[!UICONTROL 문서]**&#x200B;를 선택한 다음 **[!UICONTROL [!DNL SharePoint]통합]**&#x200B;을 선택합니다.
1. 기존의 모든 통합에 대해 목록의 왼쪽에 있는 확인 표시를 선택한 다음 **[!UICONTROL 사용 안 함]**을 선택합니다.
   ![](assets/disable-old-sharepoint.png)


### 기존 [!DNL SharePoint] 통합에 계속 액세스할 수 있도록 클라이언트 암호 구성

[!DNL SharePoint] 클라이언트 암호가 1년에 한 번 만료됩니다. 기존 [!DNL SharePoint] 통합의 문서에 계속 액세스하려면 해당 [!DNL SharePoint] 클라이언트 암호를 최신 상태로 유지해야 합니다.

>[!IMPORTANT]
>
> [!DNL SharePoint] 클라이언트 암호는 [!DNL Microsoft]에서 처리되므로 [!DNL Microsoft]에서 수행한 [!DNL SharePoint] 업데이트에 따라 클라이언트 암호 기능 및 절차가 변경될 수 있습니다. [!DNL SharePoint]의 절차 및 기능에 대한 최신 정보는 항상 [!DNL Microsoft] 설명서를 확인하십시오.

<!--1. Go to the site that your [!DNL SharePoint] integration uses. This may be a site that you created when setting up the integrations, or it may be your organization's root site.

1. Add `/_layouts/15/appregnew.aspx` to the end of the URL in the search bar at the top of your browser window.-->

1. [추가 기능 [!DNL SharePoint] 에서 만료되는 클라이언트 암호 바꾸기](https://docs.microsoft.com/en-us/sharepoint/dev/sp-add-ins/replace-an-expiring-client-secret-in-a-sharepoint-add-in#generate-a-new-secret)에 설명된 대로 새 클라이언트 암호를 생성합니다.
1. 이 클라이언트 암호를 안전한 위치에 복사합니다.
1. [!DNL Workfront]에 관리자로 로그인합니다.
1. Workfront에서 Adobe Workfront의 오른쪽 상단에 있는 **[!UICONTROL 주 메뉴]** 아이콘 ![주 메뉴](assets/main-menu-icon.png)을 클릭하거나(가능한 경우) 왼쪽 상단에 있는 **[!UICONTROL 주 메뉴]** 아이콘 ![주 메뉴](/help/_includes/assets/main-menu-icon-left-nav.png)을 클릭한 다음 **[!UICONTROL 설정]** ![설정 아이콘](/help/_includes/assets/gear-icon-setup.png)을 클릭합니다.
1. 왼쪽 패널에서 **[!UICONTROL 문서]** > **[!UICONTROL [!DNL SharePoint]통합]**&#x200B;을 클릭합니다.
1. 업데이트할 [!DNL SharePoint] 통합을 클릭한 다음 **[!UICONTROL 편집]**&#x200B;을 클릭합니다.
1. 편집 창에서 **연결 정보** 섹션을 찾은 다음 **[!UICONTROL SharePoint 클라이언트 암호]** 필드에 새 클라이언트 암호를 입력합니다.
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

* [문제:  [!DNL SharePoint] 통합을 사용할 때 사용자에게 인증 기반 오류가 발생합니다.](#problem-users-experience-authentication-based-errors-when-using-the-sharepoint-integration)
* [문제: [!DNL Workfront]의  [!DNL SharePoint] 파일을 검색하려고 할 때 내 사이트 컬렉션이 일부 또는 모두 표시되지 않습니다.](#problem-when-attempting-to-browse-sharepoint-files-in-workfront-i-do-not-see-any-or-all-of-my-site-collections)
* [문제:  [!DNL SharePoint]에서 이전에 연결된 폴더 및 문서에 액세스할 수 없습니다.](#problem-i-cannot-access-previously-linked-folders-and-documents-in-sharepoint)

### 문제: [!DNL SharePoint] 통합을 사용할 때 사용자에게 인증 기반 오류가 발생합니다. {#problem-users-experience-authentication-based-errors-when-using-the-sharepoint-integration}

솔루션:

사용자는 [!DNL SharePoint] 사이트에 대한 적절한 권한이 있어야 합니다.

[!UICONTROL 전체 제어] 액세스 권한이 있는 사용자는 [!DNL SharePoint] 통합에 필요한 모든 권한을 갖습니다. 사용자에게 전체 제어 액세스 권한을 부여하지 않으려면 다음 권한을 부여해야 합니다.

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

권한 수준을 만들고 편집하는 방법에 대한 지침은 Microsoft 설명서에서 [권한 수준을 만들고 편집하는 방법](https://docs.microsoft.com/en-us/sharepoint/how-to-create-and-edit-permission-levels)을 참조하세요.

<!--

### Problem: As a [!DNL Workfront] user, I am unable to provision a new [!DNL SharePoint] instance. When I attempt to do I see an error. {#problem-as-a-workfront-user-i-am-unable-to-provision-a-new-sharepoint-instance-when-i-attempt-to-do-i-see-an-error}

Solutions:

This can be caused by a number of things, originating in either [!DNL Workfront] or [!DNL SharePoint]'s configuration. Verify that:

* The Client ID, Client Secret, return URL and other configuration fields are correctly mapped between the [!DNL Workfront] [!DNL SharePoint] Integration instance and the [!DNL SharePoint] Site App.
* The user has [!UICONTROL Full Control] permission to the Site Collection used for authentication.
* The Site App is listed under [!UICONTROL Site App Permissions] for the [!UICONTROL Site Collection] used for authentication.

-->

### 문제: [!DNL Workfront]에서 [!DNL SharePoint]개의 파일을 검색하려고 할 때 내 사이트 컬렉션이 일부 또는 모두 표시되지 않습니다. {#problem-when-attempting-to-browse-sharepoint-files-in-workfront-i-do-not-see-any-or-all-of-my-site-collections}

솔루션:

[!DNL Workfront]에서 사이트 모음을 보려면 다음 조건을 충족해야 합니다.

<!--

* The site collection must be registered in the [!DNL Workfront] [!DNL SharePoint] Integration instance.

  To verify this in [!DNL Workfront]:

   1. Go to [!UICONTROL Setup] > [!UICONTROL Documents] > [!UICONTROL [!DNL SharePoint] Integration].
   1. Edit the [!DNL SharePoint] Integration instance information.
   1. Verify that the site collection is listed under [!UICONTROL Visible Site Collections].
   -->

* 사용자는 [!DNL SharePoint]의 사이트 컬렉션에 대한 보기 액세스 권한이 있어야 합니다.

  [!DNL SharePoint]에서 이를 확인하려면 SharePoint에서 사이트 모음의 권한을 확인하십시오.

<!--* The [!DNL SharePoint] Site App must have access to the site collection.

  To verify this in [!DNL SharePoint]:

   1. Go to the site collection > [!UICONTROL Settings] > [!UICONTROL Site app permissions].
   1. Ensure that the [!UICONTROL Site App] used by [!DNL Workfront] is listed here.
   1. (Conditional) If the Site App is not listed, add to the site collection using _layouts/15/appinv.aspx.

      For information about adding the site collection, see Granting Write Permissions To The Site App.
      
-->

### 문제: [!DNL SharePoint]에서 이전에 연결된 폴더 및 문서에 액세스할 수 없습니다. {#problem-i-cannot-access-previously-linked-folders-and-documents-in-sharepoint}

해결 방법:

[!DNL SharePoint] 폴더를 연결한 사용자가 더 이상 인증할 수 없는 경우 [!DNL Workfront]은(는) 더 이상 폴더의 내용에 액세스할 수 없습니다. 예를 들어 원래 폴더를 연결한 사용자가 회사를 그만두는 경우 이러한 상황이 발생할 수 있습니다.

계속 액세스하려면 폴더에 대한 액세스 권한이 있는 사용자가 폴더를 다시 연결해야 합니다.

외부 공급자의 폴더 연결에 대한 자세한 내용은 [외부 응용 프로그램에서 문서 연결](../../documents/adding-documents-to-workfront/link-documents-from-external-apps.md)을 참조하십시오.

<!--

### Problem: I see a "404 not found" error when attempting to add a document from [!DNL Sharepoint]

#### Solution:

This error might occur if one of the sites configured in the [!UICONTROL Visible Site Collections] list has been deleted in Sharepoint. Check the [!UICONTROL Visible Site Collections] list, and remove any sites that have been deleted in Sharepoint.-->