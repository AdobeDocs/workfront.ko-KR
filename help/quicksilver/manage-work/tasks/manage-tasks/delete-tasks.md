---
product-area: projects
navigation-topic: manage-tasks
title: 작업 삭제
description: 중복되거나 오류로 생성된 작업을 삭제할 수 있습니다.
author: Alina
feature: Work Management
exl-id: aee5c293-e5fa-413e-9d9b-c62528941be7
source-git-commit: dbc4404501e20b3f1905a5eebd13734a65db27ae
workflow-type: tm+mt
source-wordcount: '782'
ht-degree: 5%

---

# 작업 삭제

중복되거나 오류로 생성된 작업을 삭제할 수 있습니다.

내역 정보(업데이트, 일정, 상태 또는 기타 필드 변경)가 있는 작업의 경우 삭제하지 않고 닫거나 정지된 상태로 표시하는 것이 좋습니다. 이렇게 하면 프로젝트의 내역 정보를 유지하는 데 도움이 됩니다.

## 액세스 요구 사항

+++ 이 문서의 기능에 대한 액세스 요구 사항을 보려면 확장하십시오.

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
   <p>작업 이상</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">액세스 수준 구성</td> 
   <td> <p>삭제 액세스 권한이 있는 작업 및 프로젝트에 대한 액세스 편집</p></td> 
  </tr> 
  <tr> 
   <td role="rowheader">개체 권한</td> 
   <td> <p>작업 이상을 추가할 수 있는 권한으로 프로젝트에 참여</p> <p>작업을 만들 때 작업에 대한 관리 권한을 자동으로 받습니다</p></td> 
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
   <td> <p>Work or higher</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Access level configurations*</td> 
   <td> <p>Edit access to Tasks and Projects with access to Delete</p> <p>Note: If you still don't have access, ask your Workfront administrator if they set additional restrictions in your access level. For information about access to tasks, see <a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-tasks.md" class="MCXref xref">Grant access to tasks</a>. For information on how a Workfront administrator can change your access level, see <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Create or modify custom access levels</a>. </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Object permissions</td> 
   <td> <p>Contribute permissions to the project with ability to Add Tasks or higher</p> <p>When you create a task you automatically receive Manage permissions to the task</p> <p> For information about task permissions, see <a href="../../../workfront-basics/grant-and-request-access-to-objects/share-a-task.md" class="MCXref xref">Share a task </a>. </p> <p>For information on requesting additional permissions, see <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Request access to objects </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>-->

## 작업 삭제 프로세스 이해

* [작업 삭제 제한](#limitations-for-deleting-tasks)
* [작업 삭제의 영향](#the-impact-of-deleting-tasks)

### 작업 삭제 제한 사항  {#limitations-for-deleting-tasks}

* 프로젝트가 완료 상태일 때는 Workfront 관리자 또는 그룹 관리자가 프로젝트 환경 설정 영역에서 이를 허용한 경우에만 작업을 삭제할 수 있습니다. 프로젝트 환경 설정 설정에 대한 자세한 내용은 [시스템 전체 프로젝트 환경 설정 구성](../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-project-preferences.md)을 참조하십시오.

* 작업에 시간이 기록된 경우 Workfront 또는 그룹 관리자는 Workfront 인스턴스에서 작업 및 문제 환경 설정을 구성하여 이러한 작업을 삭제할 수 있도록 허용해야 합니다. 시간이 기록된 작업이 있는 프로젝트를 삭제하려고 할 때도 적용됩니다.

  <!--
  (NOTE: the last statement is NWE only; not possible in classic)
  -->

  시간이 기록된 작업의 삭제를 활성화하는 방법에 대한 자세한 내용은 [시스템 전체 작업 및 문제 환경 설정 구성](../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-task-issue-preferences.md)의 &quot;삭제&quot; 섹션을 참조하십시오.

### 작업 삭제의 영향 {#the-impact-of-deleting-tasks}

작업을 삭제하면 작업에 연결된 다른 오브젝트에 영향을 줍니다.

다음 사항을 고려하십시오.

* 작업을 삭제하면 작업에 첨부된 다음 개체도 삭제됩니다.

   * 문서

  체크 아웃된 문서가 첨부된 작업은 삭제할 수 없습니다. 문서 체크 아웃에 대한 자세한 내용은 [문서 체크 아웃](../../../documents/managing-documents/check-out-documents.md)을 참조하십시오.

   * 문제
   * 하위 작업
   * 참고
   * 승인

* Workfront 관리자가 Workfront 인스턴스의 타임시트 및 시간 환경 설정에서 프로젝트, 작업 또는 문제 삭제 환경 설정을 구성하는 방법에 따라, 작업을 삭제할 때 작업에 기록된 시간이 다음 중 한 방법으로 처리됩니다.

   * 프로젝트로 이동하며 작업이 나중에 복원되는 경우 작업에 복원되지 않습니다.
   * 작업이 나중에 복원되면 삭제되고 작업에 복원됩니다.

  시간이 기록된 작업이 있는 프로젝트를 삭제하려고 할 때도 적용됩니다.

  문제에 기록된 시간에 대한 삭제 환경 설정을 구성하는 방법에 대한 자세한 내용은 [타임시트 및 시간 환경 설정 구성](../../../administration-and-setup/set-up-workfront/configure-timesheets-schedules/timesheet-and-hour-preferences.md)을 참조하십시오.
   * 작업에 대한 경비가 프로젝트로 이동됩니다.

   * 작업 또는 작업 승인에 할당된 사용자가 프로젝트 팀에 남아 있습니다.

  프로젝트 팀에 대한 자세한 내용은 [프로젝트 팀 개요](../../../manage-work/projects/planning-a-project/project-team-overview.md)를 참조하십시오.

* 하위 작업을 삭제하고 상위 작업을 다른 프로젝트로 이동한 다음 삭제된 하위 작업을 복원하면 작업이 원래 프로젝트에 주 작업으로 다시 추가됩니다.

<!--
  <MadCap:conditionalText data-mc-conditions="QuicksilverOrClassic.Draft mode">
  (NOTE: this stays NWE; not possible in classic;)
  </MadCap:conditionalText>
  -->

## 작업 삭제

* [프로젝트에서 동시에 여러 작업 삭제](#delete-multiple-tasks-in-a-project-simultaneously)
* [단일 작업 삭제](#delete-a-single-task)

### 프로젝트에서 동시에 여러 작업 삭제  {#delete-multiple-tasks-in-a-project-simultaneously}

{{step1-to-projects}}

1. 삭제할 작업이 포함된 프로젝트 이름을 클릭합니다.
1. 왼쪽 패널에서 **작업**&#x200B;을 클릭합니다.
1. 다음 중 하나를 수행하십시오.

   1. (조건부) **자동 저장** 전환이 활성화된 경우:

      1. 삭제할 작업을 선택한 다음 **자세히**&#x200B;를 클릭합니다
      1. **삭제**&#x200B;를 클릭한 다음 **삭제**&#x200B;를 클릭하여 삭제를 확인합니다.

         작업이 삭제됩니다.

   1. (조건부) 작업 목록에 변경한 내용을 취소하려면 **플랜 모드** 아이콘을 클릭하고 **수동 저장**&#x200B;을 선택합니다.

      ![수동 저장 선택](assets/manual-save-option.png)

      다음을 수행합니다.

      1. 삭제할 작업을 선택합니다.
      1. **삭제**&#x200B;를 클릭합니다.
      1. (선택 사항) 변경 내용을 취소하고 작업을 삭제하지 않으려면 **실행 취소**&#x200B;를 클릭하십시오.
      1. 변경 내용을 유지하고 작업을 삭제하려면 **다시 실행**&#x200B;을 클릭합니다.
      1. 작업을 삭제하려면 **저장**&#x200B;을 클릭하세요.

         작업은 변경 내용을 저장한 후에만 삭제됩니다.

### 단일 작업 삭제 {#delete-a-single-task}

{{step1-to-projects}}

1. 삭제할 작업이 포함된 프로젝트 이름을 클릭합니다.
1. 왼쪽 패널에서 **작업**&#x200B;을 클릭합니다.
1. 삭제할 작업의 이름을 클릭합니다.
1. 오른쪽 상단의 **자세히** 아이콘 ![](assets/qs-more-menu.png)을(를) 클릭합니다.

   ![](assets/delete-tasks-task-level-nwe-350x225.png)

1. **작업 삭제**&#x200B;를 클릭합니다.
1. 삭제가 허용되는 경우 **삭제**&#x200B;를 클릭하십시오.

   Workfront 관리자 또는 그룹 관리자는 시간이 기록된 작업의 삭제를 허용하지 않을 수 있습니다.

   작업을 삭제하는 데 필요한 액세스 및 권한에 대한 자세한 내용은 이 문서의 [작업 삭제 제한](#limitations-for-deleting-tasks) 섹션을 참조하십시오.

## 삭제된 작업 복원

[삭제된 항목 복원](../../../administration-and-setup/manage-workfront/manage-deleted-items/restore-deleted-items.md)에 설명된 대로 Workfront 또는 그룹 관리자는 작업을 삭제한 후 30일 이내에 복원할 수 있습니다.
