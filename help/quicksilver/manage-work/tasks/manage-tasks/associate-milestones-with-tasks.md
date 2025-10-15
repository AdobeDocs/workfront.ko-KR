---
product-area: projects
navigation-topic: manage-tasks
title: 작업과 마일스톤 연결
description: 프로젝트의 라이프타임에서 중요한 단계에 도달하는 시기를 나타내기 위해 이정표를 작업과 연결할 수 있습니다. 마일스톤을 프로젝트의 작업과 연결하려면 먼저 마일스톤 경로를 프로젝트와 연결해야 합니다.
author: Alina
feature: Work Management
exl-id: 56410640-fde4-417f-8ea0-f089315476f7
source-git-commit: 7427706f6ce6cad3370b91269c1b4e7a10ed09f9
workflow-type: tm+mt
source-wordcount: '364'
ht-degree: 1%

---

# 작업과 마일스톤 연결

<!--Audited: 01/2024-->

프로젝트의 라이프타임에서 중요한 단계에 도달하는 시기를 나타내기 위해 이정표를 작업과 연결할 수 있습니다.

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
   <td> <p>표준</p> 
   <p>작업 이상</p> 
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader">액세스 수준 구성</td> 
   <td> <p>작업에 대한 액세스 편집</p></td> 
  </tr> 
  <tr> 
   <td role="rowheader">개체 권한</td> 
   <td> <p>작업에 대한 권한 관리</p></td> 
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
   <td> <p>New license: Standard</p> 
   <p>Current license: Work or higher</p> 
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Access level configurations*</td> 
   <td> <p>Edit access to Tasks</p> <p><b>NOTE</b>
   
   If you don't have access, ask your Workfront administrator if they set additional restrictions in your access level. For information on how a Workfront administrator can modify your access level, see <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Create or modify custom access levels</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Object permissions</td> 
   <td> <p>Manage permissions to the task</p> <p>For information on requesting additional access, see <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Request access to objects </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>-->

## 전제 조건

마일스톤을 작업과 연결하려면 먼저 다음 항목이 있어야 합니다.

* [마일스톤 경로 만들기](../../../administration-and-setup/customize-workfront/configure-approval-milestone-processes/create-milestone-path.md)에 설명된 대로 Workfront 관리자는 마일스톤 경로를 만들어야 합니다.

* 마일스톤 경로를 프로젝트에 연결해야 합니다.

  자세한 내용은 [프로젝트 편집](/help/quicksilver/manage-work/projects/manage-projects/edit-projects.md)을 참조하세요.

* 마일스톤 경로를 프로젝트와 연결하려면 프로젝트가 계획 중 또는 현재 상태여야 합니다.

  >[!TIP]
  >
  >마일스톤 보기를 사용하여 프로젝트에서 마일스톤의 진행 상황에 대한 최상의 개요를 얻으려면 상위 작업을 만들고 이를 프로젝트의 각 주요 단계와 연결해야 합니다. 그런 다음 이러한 상위 작업을 마일스톤 경로의 각 마일스톤과 연결합니다.

## 작업과 마일스톤 연결

마일스톤 경로가 프로젝트와 연결되면 작업에 마일스톤을 할당할 수 있습니다.

1. 작업으로 이동한 다음 작업 이름 오른쪽에 있는 **자세히** 아이콘 ![](assets/more-icon.png)을 클릭한 다음 **편집**&#x200B;을 클릭합니다.

   작업 및 마일스톤에 1:1 관계가 있습니다. 동일한 이정표를 여러 작업에 첨부할 수 없습니다. 각 작업은 하나의 마일스톤에 연결되거나 각 마일스톤을 하나의 작업에 매핑할 수 있습니다.

1. **설정**&#x200B;을 클릭한 다음 작업의 **마일스톤** 필드에서 마일스톤을 선택하십시오.
1. **저장**&#x200B;을 클릭합니다.
1. (선택 사항) 작업 목록에서 **상태 아이콘** 열을 추가하여 마일스톤이 있는 작업을 식별합니다. 마일스톤 다이아몬드 표시기가 상태 아이콘 열에 표시됩니다.

   자세한 내용은 [Adobe Workfront에서 보기 만들기 또는 편집](/help/quicksilver/reports-and-dashboards/reports/reporting-elements/create-edit-views.md)을 참조하세요.

   ![](assets/amwt3.png)

1. (선택 사항) 프로젝트 목록으로 이동하여 **마일스톤** 보기를 선택하여 마일스톤 작업의 진행 상황을 식별합니다.

   ![](assets/milestone-view-project-list.png)
