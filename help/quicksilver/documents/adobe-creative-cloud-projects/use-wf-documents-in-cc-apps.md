---
product-area: documents;workfront-integrations
navigation-topic: adobe-creative-cloud-projects
title: Creative Cloud 앱에서 Workfront 문서 사용
description: Photoshop, Illustrator 및 InDesign에서 Workfront 문서를 열고, 편집하고, 저장하고, 이에 대한 승인을 요청합니다.
author: Courtney
feature: Digital Content and Documents, Workfront Integrations and Apps
product_v2:
  - id: c4a86a5d-6562-4fc6-aa00-bfa25833aed9
    internal-label: Workfront
feature_v2:
  - id: f48b5020-b9cd-4d99-bc6e-42c35e90c1f8
    internal-label: Integrations
role_v2:
  - id: b69b2659-1057-424e-8fc5-ed9e016dc554
    internal-label: User
source-git-commit: 485b9a47cb2d5dee9dfbb77f3f6da76995df88ad
workflow-type: tm+mt
source-wordcount: '662'
ht-degree: 2%
---
# Creative Cloud 앱에서 Workfront 문서 사용

Workfront 프로젝트를 Creative Cloud 프로젝트 패널에서 사용할 수 있으면 Photoshop, Illustrator 또는 InDesign에서 직접 문서를 사용하여 작업할 수 있습니다.

## 전제 조건

* 조직은 Adobe 클라우드 스토리지를 지원하는 Workfront 버전을 사용해야 합니다.
* Workfront 및 Photoshop, Illustrator 또는 InDesign은 동일한 Adobe IMS(Identity Management System) 조직에서 권한을 부여받아야 합니다.

## 액세스 요구 사항

+++ 이 문서의 기능에 대한 액세스 요구 사항을 보려면 확장하십시오.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront 버전</td> 
   <td>Adobe 클라우드 스토리지가 활성화된 워크플로우 Ultimate</td> 
  </tr> 
  <tr> 
   <td role="rowheader">개체 권한</td> 
   <td>
      <p>프로젝트에 대한 액세스 권한을 보고 Creative Cloud 프로젝트 패널에서 볼 수 있습니다</p>
      <p>프로젝트에 대한 액세스 권한을 편집하여 추가, 편집 또는 삭제</p>
   </td> 
  </tr> 
 </tbody> 
</table>

자세한 내용은 [Workfront 설명서의 액세스 요구 사항](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)을 참조하십시오.

+++

## Workfront 프로젝트 액세스

Workfront 프로젝트의 문서 폴더 구조는 프로젝트 패널에서 미러링됩니다. 프로젝트 폴더에서 문서를 열고 편집하고 저장하면 변경 사항이 Workfront에 표시됩니다.

>[!NOTE]
>
>레거시 Workfront 스토리지 프로젝트는 프로젝트 패널에서만 Adobe 클라우드 스토리지 프로젝트에서 지원되지 않습니다.


Photoshop, Illustrator 또는 InDesign에서 Workfront 프로젝트에 액세스하려면:

1. Photoshop, Illustrator 또는 InDesign을 엽니다.
1. 앱 왼쪽의 **프로젝트** 패널에서 열려는 Workfront 프로젝트를 선택합니다.

   ![프로젝트 패널에 나열된 Workfront 프로젝트](assets/cc-projects.png)

1. 편집할 문서를 프로젝트에서 엽니다. 변경 사항을 저장하면 자동으로 다시 Workfront 프로젝트에 저장됩니다.


>[!TIP]
>
>Word 또는 Excel 문서와 같이 Photoshop, Illustrator 또는 InDesign에서 열 수 없는 파일 형식을 편집하려면 Adobe Cloud Drive를 대신 사용하십시오. 자세한 내용은 [Adobe Cloud Drive 개요](/help/quicksilver/documents/adobe-cloud-drive/adobe-cloud-drive-overview.md)를 참조하세요.

## Creative Cloud 앱에서 Workfront에 새 문서 저장

새 파일을 Workfront에 저장하거나 기존 파일의 새 사본을 Photoshop, Illustrator 또는 InDesign에서 Workfront에 저장할 수 있습니다.

새 문서를 Workfront에 저장하려면 다음을 수행합니다.

1. Photoshop, Illustrator 또는 InDesign을 열고 새 파일을 만듭니다.
1. 상단 메뉴에서 다음 중 하나를 수행합니다.
   * 새 파일을 저장하려면 **저장**&#x200B;을 클릭하세요.
   * 기존 파일의 새 복사본을 저장하려면 **다른 이름으로 저장**&#x200B;을 클릭하세요.
1. **다른 이름으로 저장** 대화 상자에서 **클라우드 문서에 저장**&#x200B;을 선택한 다음 필요한 Workfront 프로젝트를 선택합니다.

   >[!NOTE]
   >
   >Workfront 프로젝트에 이미 문서를 저장할 때 다른 이름으로 저장 대화 상자가 열리지 않습니다. Workfront 프로젝트를 선택하거나, 다른 폴더에 저장하거나, 다른 Workfront 프로젝트를 선택할 수 있습니다.


   ![workfront에 새 문서 저장](assets/save-new-to-wf.png)

1. 문서 폴더를 선택한 다음 **저장**&#x200B;을 클릭합니다. 폴더를 선택하지 않으면 문서가 프로젝트 루트 폴더에 저장됩니다.

   ![workfront에 새 문서를 저장할 폴더 선택](assets/save-to-folder.png)

## 문서에 대한 승인 요청

Workfront, Illustrator, InDesign 또는 다른 문서와 마찬가지로 Adobe Cloud Drive에서 업로드한 모든 문서에 Photoshop의 문서 승인을 추가할 수 있습니다. 자세한 내용은 [문서 승인 워크플로 만들기](/help/quicksilver/review-and-approve-work/document-reviews-and-approvals/manage-document-approvals/create-a-document-approval.md)를 참조하십시오.



## Creative Cloud 앱에서 Workfront 문서 버전 관리

Photoshop, Illustrator 또는 InDesign에서 Workfront으로 문서를 저장하면 저장한 변경 사항이 버전 탭의 현재 파일에 나타나고 &quot;새 업데이트&quot; 배지로 표시됩니다.

새 버전의 문서를 업로드하는 대신 현재 파일에 대한 승인을 요청할 수 있습니다. 자세한 내용은 [현재 파일에 대한 승인 요청](#request-approval-on-the-current-file)을 참조하세요.

![새 변경 사항이 있는 현재 파일](assets/current-file.png)

### 현재 파일에 대한 승인 요청

Workfront에서 문서의 현재 파일에 대한 승인을 요청하려면:

1. 승인을 요청할 문서가 포함된 Workfront의 프로젝트로 이동합니다.
1. 문서를 열고 **버전** 탭으로 이동합니다.
1. 현재 파일에서 **자세히** 메뉴를 클릭한 다음 **승인 요청**&#x200B;을 클릭합니다.
1. **승인 요청** 대화 상자에서 [문서 승인 워크플로 만들기](/help/quicksilver/review-and-approve-work/document-reviews-and-approvals/manage-document-approvals/create-a-document-approval.md)의 단계에 따라 승인을 만듭니다.

   ![현재 파일에 대한 승인 요청](assets/request-update-on-current-file.png)

