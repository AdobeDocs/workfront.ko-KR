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
source-git-commit: deeb63ceccc28b8f376713d4a6fb6c103ab4e06b
workflow-type: tm+mt
source-wordcount: '337'
ht-degree: 4%
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

## 문서에 대한 승인 요청

Workfront, Illustrator, InDesign 또는 다른 문서와 마찬가지로 Adobe Cloud Drive에서 업로드한 모든 문서에 Photoshop의 문서 승인을 추가할 수 있습니다. 자세한 내용은 [문서 승인 워크플로 만들기](/help/quicksilver/review-and-approve-work/document-reviews-and-approvals/manage-document-approvals/create-a-document-approval.md)를 참조하십시오.

<!--
need to verify
Creating an approval on a Creative Cloud document also creates a new version of the document. For more information, see [Manage document versions](/help/quicksilver/documents/managing-documents/manage-document-versions.md#view-the-current-file-during-an-approval).
-->