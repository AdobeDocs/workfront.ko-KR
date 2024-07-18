---
product-area: documents;workfront-integrations
navigation-topic: adobe-workfront-for-experince-manager-asset-essentials
title: Workfront Fusion을 사용하여 Adobe Experience Manager 워크플로가 있는 Workfront 프로젝트 만들기
description: Workfront Fusion을 통해 프로젝트를 생성하고 프로젝트에 Adobe Experience Manager 워크플로를 포함하려는 경우 이 문서에 설명된 특정 Fusion 모듈 구성을 사용해야 합니다.
author: Becky
feature: Digital Content and Documents, Workfront Integrations and Apps, Workfront Fusion
exl-id: b8132d5e-234d-47f6-a09c-ca46018a2d77
source-git-commit: b87839d6c6dbfe978a3e14ef4b448560742f95c3
workflow-type: tm+mt
source-wordcount: '894'
ht-degree: 0%

---

# Workfront Fusion을 사용하여 Workfront 문제를 Adobe Experience Manager 워크플로가 포함된 프로젝트로 변환합니다

Workfront Fusion을 통해 프로젝트를 생성하고 프로젝트에 Adobe Experience Manager 워크플로를 포함하려는 경우 이 문서에 설명된 특정 Fusion 모듈 구성을 사용해야 합니다.

>[!NOTE]
>
>워크플로우는 Adobe Experience Manager as a Cloud Service 통합에서만 사용할 수 있습니다. Adobe Experience Manager Assets Essentials과의 통합에서는 사용할 수 없습니다.


## 액세스 요구 사항

+++ 을 확장하여 이 문서의 기능에 대한 액세스 요구 사항을 봅니다.

다음 항목이 있어야 합니다.

<table>
  <tr>
    <td><strong>Adobe Workfront 플랜*</strong></td>
    <td>임의</td>
  </tr>
  <tr>
   <td><strong>Adobe Workfront 라이센스*</strong></td>
   <td>요청 이상</td>
  </tr>
  <tr>
   <td><strong>제품</strong></td>
   <td>
     <p><b>Adobe Experience Manager:</b></p>
     <ul>
       <li>
         <p>Experience Manager Assets as a Cloud Service 또는 Assets Essentials이 있어야 하며 Admin Console에서 사용자로 제품에 추가되어야 합니다.</p>
       </li>
       <li>
        <p>Adobe Experience Manager의 저장소에 대한 쓰기 액세스 권한이 있어야 합니다.</p>
       </li>
     </ul>
     <p><b>Workfront Fusion:</b></p>
     <p>신규:</p>
     <ul>
       <li>
         <p>Select 또는 Prime Workfront 플랜: 조직에서 Adobe Workfront Fusion을 구매해야 합니다.</p>
       </li>
       <li> 
         <p>Ultimate Workfront Plan: Workfront Fusion이 포함됩니다.</p>
       </li>
     </ul>
     <p>또는</p>
     <p>현재: 조직은 Adobe Workfront Fusion을 구매해야 합니다.</p>
   </td>
  </tr>
  <tr>
   <td><strong>액세스 수준 구성*</strong>
   </td>
   <td>문서에 대한 액세스 편집
     <p>
       <strong>참고: </strong>아직 액세스 권한이 없는 경우 Workfront 관리자에게 액세스 수준에 추가 제한을 설정했는지 문의하세요. Workfront 관리자가 액세스 수준을 수정하는 방법에 대한 자세한 내용은 <strong>사용자 지정 액세스 수준 만들기 또는 수정</strong>을 참조하십시오.
     </p>
   </td>
  </tr>
</table>

+++

## 전제 조건

시작하기 전에,

* Workfront 관리자는 Adobe Experience Manager 통합에서 워크플로우를 구성해야 합니다. 자세한 내용은 [Experience Manager Assets as a Cloud Service 통합 구성](../../administration-and-setup/configure-integrations/configure-aacs-integration.md#set-up-workflows-optional)을 참조하십시오.
* Adobe Experience Manager 통합 연결 폴더 워크플로로 구성된 프로젝트 템플릿이 있어야 합니다.
* 이 모듈에 대한 연결을 구성하려면 Workfront에서 OAuth 애플리케이션을 생성해야 합니다.

  자세한 내용은 이 문서에서 [OAuth 응용 프로그램 만들기](#create-an-oauth-application)를 참조하십시오.

## 모듈 구성

Workfront Fusion에서 Adobe Experience Manager 워크플로가 포함된 프로젝트를 만들려면 Workfront > 기타 작업 모듈을 사용해야 합니다.

1. 시나리오에 **Workfront** > **기타 작업** 모듈을 추가합니다.
1. **연결** 필드에서 이 모듈에서 사용할 계정에 연결하는 Workfront 연결을 선택합니다.

   연결 만들기에 대한 지침은 Workfront 모듈 문서에서 [연결 [!DNL Workfront] to [!DNL Workfront Fusion]](/help/quicksilver/workfront-fusion/apps-and-their-modules/workfront-modules.md#connect-workfront-to-workfront-fusion)을 참조하십시오.

   클라이언트 ID 및 클라이언트 암호를 만드는 방법에 대한 지침은 이 문서에서 [OAuth 응용 프로그램 만들기](#create-an-oauth-application)를 참조하십시오.

1. **레코드 종류** 필드에서 `Issue`을(를) 선택합니다.
1. **Action** 필드에서 `convertToProject`을(를) 선택합니다.
1. **ID** 필드에 프로젝트로 전환할 문제의 ID를 입력하거나 매핑합니다.
1. **고급 설정 표시**&#x200B;를 사용하도록 설정합니다.
1. 모듈의 맨 아래로 스크롤하여 **프로젝트(고급 컬렉션)** 필드를 찾습니다.
1. 다음 텍스트를 **프로젝트(고급 컬렉션)** 필드에 붙여 넣으십시오.

   ```
   {
       "aemNativeFolderTreeIDs": ["Folder Tree ID here"],
       "aemNativeFolderWorkflowEnabled": "true",
       "name": "New project name here",
       "templateID": "Template ID here"
   }
   ```

1. `Folder tree ID here`을(를) 폴더 ID로 바꾸십시오.

   폴더 트리 ID를 찾으려면 이 문서에서 [폴더 트리 ID 찾기](#locate-folder-tree-ids)를 참조하십시오.

   둘 이상의 폴더 트리를 사용하려면 쉼표로 ID를 구분하십시오.

   `"aemNativeFolderTreeIDs": ["Folder tree ID here","Second folder tree ID here"],`
1. `New project name here`을(를) 새 프로젝트에 포함될 이름으로 바꾸십시오.
1. `Template ID here`을(를) 새 프로젝트에 사용하는 템플릿의 ID로 바꾸십시오.

   이전 모듈(예: Workfront > 검색 모듈)의 템플릿 ID를 매핑하거나 Workfront에 있는 템플릿 페이지의 URL에서 찾을 수 있습니다.

1. **확인**&#x200B;을 클릭하여 모듈 구성을 저장합니다.

## 폴더 트리 ID 찾기

폴더 트리 ID를 찾으려면:

>[!NOTE]
>
>이 지침은 Chrome 브라우저를 사용합니다.

1. Workfront에서 이 프로젝트에 사용할 템플릿을 엽니다. 이 템플릿에는 프로젝트에 사용할 Adobe Experience Manager 구성이 포함되어야 합니다.
1. 브라우저용 개발자 도구를 엽니다.
1. 개발자 도구에서 **네트워크** 탭을 엽니다.
1. **필터** 상자에 `object-workflow`을(를) 입력하십시오.
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

연결 만들기에 대한 지침은 Workfront 모듈 문서에서 [연결 [!DNL Workfront] to [!DNL Workfront Fusion]](/help/quicksilver/workfront-fusion/apps-and-their-modules/workfront-modules.md#connect-workfront-to-workfront-fusion)을 참조하십시오.
