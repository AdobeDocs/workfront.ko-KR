---
product-area: documents;workfront-integrations
navigation-topic: adobe-workfront-for-experince-manager-asset-essentials
title: Use Workfront Fusion to create a Workfront Project that has Adobe Experience Manager workflows
description: If you are creating a project through Workfront Fusion and want to include Adobe Experience Manager workflows on the project, you must use a specific Fusion module configuration, described in this article.
author: Becky
feature: Digital Content and Documents, Workfront Integrations and Apps, Workfront Fusion
exl-id: b8132d5e-234d-47f6-a09c-ca46018a2d77
source-git-commit: 90eb99fa46e706a53427f995d484e2fb42e9c293
workflow-type: tm+mt
source-wordcount: '925'
ht-degree: 8%

---

# Workfront Fusion을 사용하여 Workfront 문제를 Adobe Experience Manager 워크플로가 포함된 프로젝트로 변환합니다

If you are creating a project through Workfront Fusion and want to include Adobe Experience Manager workflows on the project, you must use a specific Fusion module configuration, described in this article.

>[!NOTE]
>
>Workflows are available only in an Adobe Experience Manager as a Cloud Service integration. They are not available in integrations with Adobe Experience Manager Assets Essentials.<br>
>이 기능은 새 문서 영역에서 사용할 수 없습니다.


## 액세스 요구 사항

+++ 이 문서의 기능에 대한 액세스 요구 사항을 보려면 확장하십시오.

<table>
  <tr>
    <td><strong>Adobe Workfront 패키지</strong></td>
   <td> <p>모든 Adobe Workfront 워크플로 패키지 및 모든 Adobe Workfront 자동화 및 통합 패키지</p><p>Workfront Ultimate</p><p>Workfront Prime 및 Select 패키지 및 Workfront Fusion 추가 구매.</p> </td> 
  </tr>
  <tr>
   <td><strong>Adobe Workfront 라이선스</strong></td>
   <td><p>기여자 이상</p><p>요청 이상</p></td>
  </tr>
  <tr>
   <td><strong>제품</strong></td>
   <td>
     <p><b>Adobe Experience Manager:</b></p>
     <ul>
       <li>
         <p>You must have Experience Manager Assets as a Cloud Service or Assets Essentials, and you must be added to the product as a user in the Admin Console.</p>
       </li>
       <li>
        <p>You must have write access to the repository in Adobe Experience Manager.</p>
       </li>
     </ul>
     <p><b>Workfront Fusion:</b></p>
     <ul>
       <li>
        <p>조직에 Workfront 자동화 및 통합이 포함되지 않은 Select 또는 Prime Workfront 패키지가 있는 경우 Adobe Workfront Fusion을 구매해야 합니다.</li></ul>
       </li>
     </ul>
   </td>
  </tr>
  <tr>
   <td><strong>Access level configurations</strong>
   </td>
   <td><p>문서에 대한 액세스 편집</p>
   </td>
  </tr>
</table>

+++

## 전제 조건

Before you begin,

* Your Workfront administrator must configure workflows in an Adobe Experience Manager integration. For more information, see [Configure the Experience Manager Assets as a Cloud Service integration](../../administration-and-setup/configure-integrations/configure-aacs-integration.md#set-up-workflows-optional).
* You must have a project template configured with an Adobe Experience Manager integration linked folder workflow.
* You must have created an OAuth application in Workfront to configure the connection for this module.

  For instructions, see [Create an OAuth application](#create-an-oauth-application) in this article.

## Module configuration

In Workfront Fusion, if you want to create a project that includes Adobe Experience Manager workflows, you must use the Workfront > Misc Action module.

1. Add the **Workfront** > **Misc Action** module to your scenario.
1. In the **Connection** field, select the Workfront connection that connects to the account this module will use.

   For instructions on creating a connection, see [Connect [!DNL Workfront] to [!DNL Workfront Fusion]](https://experienceleague.adobe.com/en/docs/workfront-fusion/using/references/apps-and-their-modules/adobe-connectors/workfront-modules#connect-workfront-to-workfront-fusion) in the article Workfront modules.

   For instructions on creating the Client ID and Client Secret you will need to create a connection, see [Create an OAuth application](#create-an-oauth-application) in this article.

1. **레코드 종류** 필드에서 `Issue`을(를) 선택합니다.
1. In the **Action** field, select `convertToProject`.
1. In the **ID** field, enter or map the ID of the issue that you are converting to a project.
1. Enable **Show advanced settings**.
1. Scroll to the bottom of the module and locate the **Project (Advanced Collection)** field.
1. Paste the following text into the **Project (Advanced Collection)** field.

   ```
   {
       "aemNativeFolderTreeIDs": ["Folder Tree ID here"],
       "aemNativeFolderWorkflowEnabled": "true",
       "name": "New project name here",
       "templateID": "Template ID here"
   }
   ```

1. Replace `Folder tree ID here` with the folder IDs.

   To locate folder tree IDs, see [Locate folder tree IDs](#locate-folder-tree-ids) in this article.

   To use more than one folder tree, separate IDs with a comma:

   `"aemNativeFolderTreeIDs": ["Folder tree ID here","Second folder tree ID here"],`
1. Replace `New project name here` with the name that the new project will have.
1. Replace `Template ID here` with the ID of the template that you are using for the new project.

   You can map the template ID from a previous module (such as a Workfront > Search module) or locate it in the URL of the template&#39;s page in Workfront.

1. Click **OK** to save the module configuration.

## Locate folder tree IDs

To locate the folder tree IDs:

>[!NOTE]
>
>These instructions use the Chrome browser.

1. In Workfront, open the template that you want to use for this project. This template must include the Adobe Experience Manager configuration that you want to use for the project.
1. Open the developer tools for your browser.
1. Open the **Network** tab in the developer tools.
1. In the **Filter** box, enter `object-workflow`.
1. 이름 열에서 나타나는 영숫자 ID를 클릭합니다.

   ![폴더 ID 찾기](assets/finding-folder-id-1.png)

1. 영숫자 ID 오른쪽에 있는 **미리 보기** 탭을 클릭합니다.
1. 축소된 다음 섹션을 엽니다.
   1. `data`
   1. `objectWorkflow`
   1. `workflows`
   1. `enhancedLinkedFolderCreationWorkflow`
   1. `enhancedLinkedFolderCreationWorkflowConfigurations`

   각 폴더 트리는 숫자로 표시됩니다. 0(영)은 목록의 첫 번째 폴더를 나타내고, 1은 두 번째 폴더를 나타냅니다. 템플릿에 폴더 트리가 하나만 포함되어 있으면 이 값은 0입니다.

1. 새 프로젝트에 사용할 폴더 트리를 엽니다. `_id` 필드 값을 기록해 두십시오. 둘 이상의 폴더 트리를 사용하려면 사용할 폴더 트리의 모든 `_id` 필드 값을 메모해 두십시오.

   ![폴더 ID 찾기](assets/finding-folder-id-2.png)

   **Workfront** > **기타 작업** Fusion 모듈의 **프로젝트(고급 컬렉션)** 필드에 입력할 `aemNativeFolderTreeIDs` 값입니다.

## OAuth 애플리케이션 만들기

이 모듈의 연결을 위해 Workfront에서 OAuth 애플리케이션을 설정해야 합니다. Fusion에서 제공된 Workfront 연결에 대해 이 작업을 한 번만 수행하면 됩니다.

1. [!DNL Workfront] 통합을 위한 OAuth2 애플리케이션 만들기 문서의 [사용자 자격 증명(인증 코드 흐름)을 사용하여 OAuth2 애플리케이션 만들기](/help/quicksilver/administration-and-setup/configure-integrations/create-oauth-application.md#create-an-oauth2-application-using-user-credentials-authorization-code-flow)에 설명된 대로 Workfront에서 OAuth 애플리케이션 만들기를 시작합니다.
1. 클라이언트 ID 및 클라이언트 암호를 안전한 위치에 복사합니다.
1. **리디렉션 URI** 필드에 다음을 입력하십시오.

   ```
   http://app.workfrontfusion.com/oauth/cb/workfront-workfront
   ```

1. **저장**&#x200B;을 클릭합니다.

Fusion에서 모듈의 연결을 구성할 때 이 클라이언트 ID와 클라이언트 암호를 사용합니다.

연결 만들기에 대한 지침은 Workfront 모듈 문서에서 [연결 [!DNL Workfront] to [!DNL Workfront Fusion]](https://experienceleague.adobe.com/en/docs/workfront-fusion/using/references/apps-and-their-modules/adobe-connectors/workfront-modules#connect-workfront-to-workfront-fusion)을 참조하십시오.
