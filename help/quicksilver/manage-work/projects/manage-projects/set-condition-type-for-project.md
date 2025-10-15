---
product-area: projects
navigation-topic: manage-projects
title: 프로젝트의 상태 유형 설정
description: 프로젝트 관리자는 프로젝트의 상태 유형을 업데이트하여 프로젝트의 상태를 계산하는 방법을 결정할 수 있습니다. 프로젝트 상태는 프로젝트가 진행되는 방식을 시각적으로 보여 줍니다.
author: Alina
feature: Work Management
exl-id: e6b99c48-5ccc-4956-8465-6f22f14468ef
source-git-commit: 5bc7a1c00b72cfc07270cafee5bf753989b48d33
workflow-type: tm+mt
source-wordcount: '301'
ht-degree: 2%

---

# 프로젝트의 상태 유형 설정

프로젝트 관리자는 프로젝트의 상태 유형을 업데이트하여 프로젝트의 상태를 계산하는 방법을 결정할 수 있습니다. 프로젝트 상태는 프로젝트가 진행되는 방식을 시각적으로 보여 줍니다.

## 액세스 요구 사항

+++ 을 확장하여 이 문서의 기능에 대한 액세스 요구 사항을 봅니다. 


<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront 패키지</td> 
   <td> <p>임의</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront 라이선스</td> 
   <td><p>표준</p> 
   <p>플랜</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">액세스 수준 구성</td> 
   <td> <p>프로젝트에 대한 액세스 편집</p></td> 
  </tr> 
  <tr> 
   <td role="rowheader">개체 권한</td> 
   <td> 
    <ul> 
     <li> <p>프로젝트 세부 정보 영역에서 상태 유형을 편집할 수 있는 권한을 프로젝트에 제공 </p> </li> 
     <li> <p>프로젝트 편집 상자에서 상태 유형을 편집할 프로젝트에 대한 권한 관리</p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

자세한 내용은 [Workfront 설명서의 액세스 요구 사항](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)을 참조하십시오.

+++

<!--Old:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront plan*</td> 
   <td> <p>Any</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront license*</td> 
   <td> <p>Plan </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Access level configurations*</td> 
   <td> <p>Edit access to Projects</p> <p>Note: If you still don't have access, ask your Workfront administrator if they set additional restrictions in your access level. For information about access to projects, see <a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-projects.md" class="MCXref xref">Grant access to projects</a>. For information on how a Workfront administrator can change your access level, see <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Create or modify custom access levels</a>. </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Object permissions</td> 
   <td> 
    <ul> 
     <li> <p>Contribute permissions to a project to edit the Condition Type in the Project Details area </p> </li> 
     <li> <p>Manage permissions to a project to edit the Condition Type in the Edit Project box</p> </li> 
    </ul> <p> For information about project permissions, see <a href="../../../workfront-basics/grant-and-request-access-to-objects/share-a-project.md" class="MCXref xref">Share a project in Adobe Workfront</a>.</p> <p>For information on requesting additional access, see <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Request access to objects </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>-->

## 프로젝트에 대한 조건 유형 설정

1. 조건 유형을 업데이트할 프로젝트로 이동합니다.
1. 다음 중 하나를 수행하십시오.

   * 프로젝트 이름의 오른쪽에 있는 **자세히** 메뉴 ![추가 메뉴](assets/qs-more-menu.png)를 클릭한 다음 **편집**&#x200B;을 클릭합니다.
   * 왼쪽 패널에서 **프로젝트 세부 정보**&#x200B;를 클릭합니다.

   ![](assets/update-condition-type-nwe-350x108.png)

1. **조건 유형** 필드에서 다음 중 하나를 선택합니다.

   * **수동:** 프로젝트 소유자가 프로젝트에 대한 조건을 수동으로 설정합니다.

     이 경우 프로젝트 소유자는 프로젝트 헤더 또는 프로젝트 세부 정보 섹션에서 프로젝트의 상태를 업데이트할 수 있습니다.

   * **진행 상태:** Workfront은 프로젝트의 진행 상태를 기반으로 조건을 설정합니다. 진행 상태를 계산하는 방법에 대한 자세한 내용은 [프로젝트 진행 상태 개요](../../../manage-work/projects/planning-a-project/project-progress-status.md)를 참조하십시오.

1. 프로젝트 편집 상자에서 조건 유형을 수정할 때 **저장**&#x200B;을 클릭합니다.

   프로젝트 세부 정보 섹션에서 조건 유형을 수정할 때 **변경 내용 저장**&#x200B;을 클릭합니다.


