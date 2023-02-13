---
title: 프로젝트 삭제
product-area: projects
navigation-topic: manage-projects
description: 프로젝트 및 해당 데이터가 더 이상 필요하지 않은 경우 프로젝트를 삭제할 수 있습니다.
author: Alina
feature: Work Management
exl-id: a0e80c4d-29a8-4bf8-aa19-0c2d493236c6
source-git-commit: dc3461803e23f61877c31efa2c52fffdc7bd79bf
workflow-type: tm+mt
source-wordcount: '854'
ht-degree: 1%

---

# 프로젝트 삭제

프로젝트 및 해당 데이터가 더 이상 필요하지 않은 경우 프로젝트를 삭제할 수 있습니다.

프로젝트를 삭제하는 대신, 프로젝트를 편집하고 상태를 완료 또는 없음으로 변경하는 것이 좋습니다. 따라서 사용자의 작업 목록에서 프로젝트와 관련된 모든 현재 작업이 제거되지만 프로젝트와 연결된 모든 데이터가 저장됩니다.

## 액세스 요구 사항

<!-- drafted for P&P:
<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td> <p>Adobe Workfront plan*</p> </td> 
   <td>Any</td> 
  </tr> 
  <tr> 
   <td> <p>Adobe Workfront license*</p> </td> 
   <td> <p>Current license: Standard </p> 
   Or
   <p>Legacy license: Plan </p>
   </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td><strong>Access level configurations*</strong> </td> 
   <td> <p>Edit access to Projects with ability to Create <span>and Delete</span> projects</p> <p><b>NOTE</b>
   
   If you still don't have access, ask your Workfront administrator if they set additional restrictions in your access level. For information on how a Workfront administrator can change your access level, see <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Create or modify custom access levels</a>.</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> <p><strong>Object permissions</strong> </p> </td> 
   <td> <p>Edit access to Projects, Tasks,&nbsp;Issues with ability to Delete projects, tasks, and issues</p> <p>Note: If you still don't have access, ask your Workfront administrator if they set additional restrictions in your access level. For information on how a Workfront administrator can modify your access level, see <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Create or modify custom access levels</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>
-->

이 문서의 절차를 수행하려면 다음 사항이 있어야 합니다.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront 플랜*</td> 
   <td> <p>모든 </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront 라이선스*</td> 
   <td> <p>플랜 </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">액세스 수준 구성*</td> 
   <td> <p>프로젝트, 작업, 프로젝트 삭제 기능 문제 액세스 편집</p> <p>참고: 여전히 액세스 권한이 없는 경우 Workfront 관리자에게 액세스 수준에서 추가 제한 사항을 설정하는지 문의하십시오. Workfront 관리자가 액세스 수준을 수정하는 방법에 대한 자세한 내용은 <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">사용자 정의 액세스 수준 만들기 또는 수정</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">개체 권한</td> 
   <td> <p>프로젝트, 작업 및 문제를 삭제할 수 있는 기능을 사용하여 프로젝트의 프로젝트, 작업 및 문제에 대한 권한을 관리합니다. </p> <p>추가 액세스 요청에 대한 자세한 내용은 <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">개체에 대한 액세스 요청 </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;어떤 계획, 라이선스 유형 또는 액세스 권한을 보유하고 있는지 알아보려면 Workfront 관리자에게 문의하십시오.
프로젝트 목록 또는 프로젝트 수준에서 프로젝트를 삭제할 수 있습니다.

## 프로젝트 삭제 프로세스 이해

* [프로젝트 삭제 제한 사항](#limitations-for-deleting-projects)
* [프로젝트 삭제의 영향](#the-impact-of-deleting-projects)

### 프로젝트 삭제 제한 사항  {#limitations-for-deleting-projects}

* 삭제된 항목은 30일 동안 휴지통으로 이동하며 Workfront 관리자만 복구할 수 있습니다.

   개체 복원에 대한 자세한 내용은 문서를 참조하십시오 [삭제된 항목 복원](../../../administration-and-setup/manage-workfront/manage-deleted-items/restore-deleted-items.md).

* 프로젝트에 로그된 시간에 대한 작업이나 문제가 있는 경우, Workfront 또는 그룹 관리자가 Workfront 인스턴스에서 작업 및 문제 환경 설정을 구성하여 작업이 포함된 프로젝트를 삭제할 수 있도록 허용해야 합니다.

   시간이 기록되는 작업, 문제 또는 프로젝트의 삭제를 활성화하는 방법에 대한 자세한 내용은 [시스템 전체 작업 및 문제 환경 설정 구성](../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-task-issue-preferences.md).

   <!--
  <p data-mc-conditions="QuicksilverOrClassic.Quicksilver,QuicksilverOrClassic.Draft mode">(NOTE: this bullet stays in NWE only forever)</p>
  -->

### 프로젝트 삭제의 영향 {#the-impact-of-deleting-projects}

* 프로젝트를 삭제하면 프로젝트에 연결된 다른 개체가 영향을 받습니다.

   프로젝트를 삭제할 때 프로젝트에 첨부된 다음 개체도 삭제됩니다.

   * 문서

      첨부된 문서가 체크 아웃된 프로젝트는 삭제할 수 없습니다. 문서 체크 아웃에 대한 자세한 내용은 [문서 체크 아웃](../../../documents/managing-documents/check-out-documents.md).

   * 작업
   * 하위 작업
   * 문제
   * 메모
   * 승인
   * 경비

* Workfront 관리자가 Workfront 인스턴스의 작업표 및 시간 환경 설정에서 프로젝트, 작업 또는 문제 삭제 환경 설정을 구성하는 방법에 따라, 작업, 문제 또는 프로젝트에 대해 기록된 시간은 프로젝트를 삭제할 때 다음 방법 중 하나로 처리됩니다.

   * 작업표에 일반 시간으로 남아 있는 시간입니다.
   * 시간이 삭제되고 프로젝트가 복원되면 복원됩니다.

   로그온한 시간 동안의 삭제 환경 설정 구성에 대한 자세한 내용은 다음을 참조하십시오 [작업표 및 시간 환경 설정 구성](../../../administration-and-setup/set-up-workfront/configure-timesheets-schedules/timesheet-and-hour-preferences.md).

* 삭제한 프로젝트가 Workfront Scenario Planner의 이니셔티브에 연결되어 있는 경우

   * 이니셔티브는 계획에 남아 있지만 프로젝트에 대한 링크는 제거됩니다.
   * 삭제한 프로젝트가 계획에서 게시된 유일한 이니셔티브에 연결되어 있는 경우 계획이 게시되었다는 표시도 제거됩니다.
   * 삭제된 프로젝트를 복구하면 프로젝트가 복구되지만 이니셔티브에 대한 링크가 복원되지 않고 시나리오 계획자 영역이 더 이상 프로젝트 세부 정보에 표시되지 않습니다.

      시나리오 플래너는 새 Adobe Workfront 경험에서만 사용할 수 있으며 추가 라이센스가 필요합니다. Workfront 시나리오 플래너에 대한 자세한 내용은 [시나리오 계획자 개요](../../../scenario-planner/scenario-planner-overview.md).

      시나리오 플래너의 이니셔티브에 연결된 프로젝트에 대한 자세한 내용은 [시나리오 계획자에서 이니셔티브를 게시하여 프로젝트를 업데이트하거나 생성합니다](../../../scenario-planner/publish-scenarios-update-projects.md).

* 프로젝트가 Workfront 목표의 목표에 대한 활동이기도 한 경우:

   * 프로젝트가 대상에서 삭제됩니다. 프로젝트에 의해 목표에 표시된 진행도 제거됩니다.

   * 삭제된 프로젝트를 복구하면 프로젝트가 목표의 활동으로도 복원됩니다.

      이 경우 추가 라이센스가 필요합니다. Workfront 목표에 대한 자세한 내용은 [Adobe Workfront 목표 개요](../../../workfront-goals/goal-management/wf-goals-overview.md).

      프로젝트와 목표를 연결하는 방법에 대한 자세한 내용은 [Adobe Workfront 목표의 목표에 프로젝트 추가](../../../workfront-goals/results-and-activities/connect-projects-to-goals-overview.md).

## 목록에서 프로젝트 삭제

프로젝트 목록에서 프로젝트를 삭제할 수 있습니다.

1. 프로젝트 목록 또는 프로젝트 보고서로 이동합니다.
1. 삭제할 프로젝트를 선택한 다음 **삭제** 를 클릭합니다.

1. 클릭 **예, 삭제합니다.** 를 클릭하여 삭제를 확인합니다.

   프로젝트가 삭제되어 30일 동안 휴지통에 저장됩니다. Workfront 관리자는 이 시간 동안 휴지통에서 복원할 수 있습니다.

## 프로젝트 수준에서 프로젝트 삭제

1. 삭제할 프로젝트로 이동합니다.
1. 을(를) 클릭합니다. **자세히** 아이콘 ![](assets/qs-more-menu.png).

1. 클릭 **프로젝트 삭제**.

1. 클릭 **예, 삭제합니다.**.

   프로젝트가 삭제되어 30일 동안 휴지통에 저장됩니다. Workfront 관리자는 이 시간 동안 휴지통에서 복원할 수 있습니다.

## 삭제된 프로젝트 복원

시스템 또는 그룹 관리자는 문서에 설명된 대로 프로젝트를 삭제한 후 30일 이내에 복원할 수 있습니다 [삭제된 항목 복원](../../../administration-and-setup/manage-workfront/manage-deleted-items/restore-deleted-items.md).
