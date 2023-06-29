---
product-area: projects;user-management
navigation-topic: assign-tasks
title: 작업 할당
description: 작업을 사용자, 역할 또는 팀에 할당하여 작업 완료를 담당하는 사람을 표시할 수 있습니다. 한 번에 두 개 이상의 리소스에 작업을 할당할 수 있습니다.
author: Alina
feature: Work Management
exl-id: 611b136e-2c3f-4eac-9d75-e8c12e06148d
source-git-commit: 8dbb48e6aa2df874caa816468cf2e3ad408ebf7e
workflow-type: tm+mt
source-wordcount: '1901'
ht-degree: 1%

---

# 작업 할당

{{highlighted-preview}}

작업을 사용자, 작업 역할 또는 팀에 할당하여 작업 완료를 담당하는 사람을 표시할 수 있습니다. 한 번에 두 개 이상의 리소스에 작업을 할당할 수 있습니다.

>[!TIP]
>
>여러 사용자, 작업 역할 또는 팀을 할당할 수 있습니다. 활성 사용자, 작업 역할 및 팀만 할당할 수 있습니다.
>
>비활성화되기 전에 사용자, 작업 역할 또는 팀이 할당된 경우 작업 항목에 할당된 상태로 유지됩니다. 이 경우 다음 사항을 권장합니다.
>
>* 작업 항목을 활성 리소스에 재할당합니다.
>* 비활성화된 팀의 사용자를 활성 팀과 연결하고 작업 항목을 활성 팀에 재할당합니다.
>

작업에 할당된 사용자 수와 작업 소유자의 일정은 작업의 계획된 일자를 수정하여 프로젝트의 타임라인을 변경할 수 있습니다. 작업에 여러 사용자를 할당하면 어떤 영향이 있는지 알려면 다음을 참조하십시오. [작업 할당 수정 개요](../../../manage-work/tasks/assign-tasks/modify-task-assignments-overview.md).

이 문서 외에도 작업 할당에 대한 자세한 내용은 다음 문서를 읽는 것이 좋습니다.

* [작업 할당 수정 개요](../../../manage-work/tasks/assign-tasks/modify-task-assignments-overview.md)
* [스마트 할당 개요](../../../manage-work/tasks/assign-tasks/smart-assignments.md)
* [스마트 할당 만들기](../../../manage-work/tasks/assign-tasks/make-smart-assignments.md)
* [고급 할당 만들기](../../../manage-work/tasks/assign-tasks/create-advanced-assignments.md)
* [작업 목록에서 여러 사용자 할당 수정](../../../manage-work/tasks/assign-tasks/modify-multiple-assignments-in-task-list.md)
* [작업 편집](../../../manage-work/tasks/manage-tasks/edit-tasks.md)
* [프로젝트 계획 개요](../../../manage-work/projects/planning-a-project/plan-project.md)
* [작업 계획 완료 일자 개요](../../../manage-work/tasks/task-information/task-planned-completion-date.md)
* [프로젝트 계획된 완료 일자 설정](../../../manage-work/projects/planning-a-project/project-planned-completion-date.md)
* [시스템 전체 프로젝트 환경 설정 구성](../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-project-preferences.md)
* [업무 균형자에서 작업 할당 개요](../../../resource-mgmt/workload-balancer/assign-work-in-workload-balancer.md)

## 액세스 요구 사항

<!--drafted for P&P - replace table below with this:

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
   <td> <p>Current license: Standard</p> 
   Or
   <p>Legacy license: Work or higher</p>
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Access level configurations*</td> 
   <td> <p>Edit access to Projects and Tasks</p> <p>View or higher access to Users</p> <p><b>NOTE</b>
   
   If you still don't have access, ask your Workfront administrator if they set additional restrictions in your access level. For information on how a Workfront administrator can modify your access level, see <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Create or modify custom access levels</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Object permissions</td> 
   <td> <p>Contribute or higher permissions to tasks</p> <p>For information on requesting additional access, see <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Request access to objects </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

-->

이 문서의 단계를 수행하려면 다음 액세스 권한이 있어야 합니다.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront 플랜*</td> 
   <td> <p>모든</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront 라이센스*</td> 
   <td> <p>작업 이상</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">액세스 수준 구성*</td> 
   <td> <p>프로젝트 및 작업에 대한 액세스 편집</p> <p>사용자에 대한 보기 또는 상위 액세스 권한</p> <p><b>메모</b>

여전히 액세스 권한이 없는 경우 Workfront 관리자에게 액세스 수준에 추가 제한을 설정하는지 문의하십시오. Workfront 관리자가 액세스 수준을 수정하는 방법에 대한 자세한 내용은 <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">사용자 정의 액세스 수준 만들기 또는 수정</a>.</p> </td>
</tr> 
  <tr> 
   <td role="rowheader">개체 권한</td> 
   <td> <p>작업에 대한 기여 또는 더 높은 권한</p> <p>추가 액세스 요청에 대한 자세한 내용은 <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">오브젝트에 대한 액세스 요청 </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

*보유 중인 플랜, 라이선스 유형 또는 액세스 권한을 확인하려면 Workfront 관리자에게 문의하십시오.

## 작업 역할, 팀 및 사용자에 대한 여러 할당 고려 사항

작업 항목에 여러 리소스를 할당할 때 다음 사항을 고려하십시오.

* 사용자는 프로필과 연결된 작업 역할을 두 개 이상 가질 수 있습니다. 사용자를 작업 역할과 연결하는 방법에 대한 자세한 내용은 [사용자 프로필 편집](../../../administration-and-setup/add-users/create-and-manage-users/edit-a-users-profile.md).

* 작업 또는 문제에 두 명 이상의 사용자를 할당하면 선택한 첫 번째 사용자가 자동으로 작업 또는 문제의 소유자로 지정됩니다.
이를 변경하는 방법에 대한 지침은 문서에서 기본 옵션으로 설정에 대한 정보를 참조하십시오 [고급 할당 만들기](create-advanced-assignments.md).

* 팀은 작업 또는 문제의 기본 피할당자가 될 수 없습니다. 사용자 또는 작업 역할만 작업 또는 문제에 대한 기본으로 지정할 수 있습니다.

<!-- If a task is assigned to multiple teams, the primary team sees the Work On It button. waiting on team to verify if this is true. (Courtney)
You cannot make a team be a Primary on a task/ issue. (Alina) -->

* 프로젝트의 작업 및 문제가 하나 이상의 팀 또는 작업 역할에 먼저 할당될 수 있습니다. 프로젝트를 시작할 준비가 되면 사용자에게 할당해야 할 수도 있습니다.

  <table>
  <col> 
  <col> 
  <tbody>
  <tr>
   <td>팀</td>
   <td>팀에 작업을 할당하고 사용자도 할당하면 사용자가 팀의 구성원이 아니더라도 작업은 팀 및 사용자에게 할당된 상태로 유지됩니다.</td>
  </tr>
  <tr>
   <td>작업 역할</td>
   <td><p>하나 이상의 역할에 작업 또는 문제를 할당한 다음 사용자도 할당하는 경우, 에서는 다음 규칙에 따라 추가 사용자와 연결할 작업 역할(있는 경우)을 결정합니다.</p>
     <ul>
      <li>작업 역할이 하나만 할당되고 사용자의 기본 역할(프로필에 구성됨)과 일치하는 경우 작업 또는 문제는 해당 사용자에게만 할당됩니다.</li>
      <li>여러 개의 역할이 할당되고 이 중 하나 이상이 사용자의 다른 역할 중 하나와 일치하는 경우, 작업 또는 문제가 사용자에게 할당됩니다(일치하는 역할이 여러 개인 경우 임의로 역할 선택). 할당된 추가 역할도 함께 할당됩니다</li>
      <li>하나 이상의 작업 역할이 할당되고 사용자의 작업 역할과 일치하는 항목이 없으면 작업 또는 문제가 역할 또는 역할 및 사용자 모두에 할당됩니다.</li>
     </ul>
   <p>사용자의 기본 역할 및 기타 역할에 대한 자세한 내용은 <a href="../../../administration-and-setup/add-users/create-and-manage-users/edit-a-users-profile.md">사용자 프로필 편집</a>.</p>
   </td> 
     </tr>
  </tbody>
  </table>

<!--
<div data-mc-conditions="QuicksilverOrClassic.Draft mode">
<h2>Considerations for multiple user assignments and using schedules</h2>
<p>(NOTE: moved to the Modify task assignments overview standalone article)</p>
<p>You can assign multiple resources to a task. When you assign a user to a task, Workfront uses the user's schedule to calculate the planned dates for the task which ultimately determine the timeline of the project. Using the schedule of the user takes into account their time off, holidays, and weekend days which are considered non-working days when task activity cannot occur. </p>
<p>When you assign multiple users to a task, your Workfront administrator <span>or a group administrator</span> determines which one of the following schedules Workfront uses to determine the planned dates of the tasks, based on schedules: </p>
<ul>
<li> <p><strong>The Primary Assignee's schedule</strong>: this is the schedule associated with the user designated as the task Owner.</p> <p>For information about associating users with schedules, see <a href="../../../administration-and-setup/add-users/create-and-manage-users/edit-a-users-profile.md" class="MCXref xref">Edit a user's profile</a>.</p> </li>
<li><strong>The Project's schedule</strong>: this is the schedule associated with the project. For adding a schedule to a project, see <a href="../../../manage-work/projects/manage-projects/edit-projects.md" class="MCXref xref">Edit projects</a>.</li>
</ul>
<p>For information about setting up which schedule a project uses in the case of multiple assignments, see <a href="../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-project-preferences.md" class="MCXref xref">Configure system-wide project preferences</a>. </p>
</div>
-->

## 단일 작업 할당

1. 할당할 작업으로 이동합니다.
1. 클릭 **할당 대상** 다음에서 **할당** 작업 또는 문제의 헤더에 있는 필드.

   또는

   작업 또는 문제가 이미 할당된 경우 할당명을 클릭합니다.

   ![](../assign-tasks/assets/advanced-assignments-link-from-task-header-nwe-350x267.png)

1. 다음 중 하나를 수행하십시오.

   * 할당하려는 사용자, 역할 또는 팀의 이름을 입력한 다음 목록에 나타나면 클릭합니다.


     >[!TIP]
     >
     >사용자 할당을 추가할 때 아바타, 사용자의 기본 역할 또는 이메일 주소에 따라 이름이 동일한 사용자가 구분되는지 확인합니다. 사용자를 추가할 때 이를 보려면 사용자를 하나 이상의 작업 역할과 연결해야 합니다.
     >
     ><span class="preview">작업 역할 할당을 추가할 때 작업 역할이나 위치를 검색할 수 있습니다. 발령에 대한 기본 청구 요율을 사용하려면 시스템/기본 작업 역할을 선택하고, 요율 카드에서 청구 요율을 사용하려면 요율 카드 작업 역할을 선택합니다. 등급 카드에 대한 자세한 내용은 [등급 카드 관리](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/manage-rate-cards.md).</span>


   * (조건부) **제안된 할당** 목록(이 목록이 표시되는 경우) 자세한 내용은 [스마트 할당 개요](../../../manage-work/tasks/assign-tasks/smart-assignments.md).

   * 클릭 **고급**

     고급 할당 방법에 대한 자세한 내용은 다음을 참조하십시오. [고급 할당 만들기](../../../manage-work/tasks/assign-tasks/create-advanced-assignments.md).

1. **저장**&#x200B;을 클릭합니다.
1. (선택 사항 및 조건부) **X 아이콘** 을 클릭한 경우 할당을 제거할 작업의 오른쪽 패널에 있는 할당 이름 옆에 있습니다 **고급**.

## 목록에서 작업 할당

목록 보기에 할당 필드가 표시되면 목록이나 보고서에서 작업을 할당할 수 있습니다. 작업을 더 빠르게 할당할 수 있는 방법입니다. 이 문서에서는 목록의 한 작업에 대한 할당을 수정하는 방법에 대해 설명합니다. 목록의 복수 태스크에 대한 복수 지정을 수정하는 방법에 대한 자세한 내용은 [작업 목록에서 여러 사용자 할당 수정](../../../manage-work/tasks/assign-tasks/modify-multiple-assignments-in-task-list.md).

보기에 표시되는 필드에 따라 다음 엔티티를 작업에 할당할 수 있습니다.

| 필드 | 할당된 엔티티 |
|---|---|
| **할당 대상** | 사용자 1명 할당 |
| **할당됨** | 사용자 1명 할당 |
| **할당** | 사용자, 작업 역할 또는 팀 할당 |

목록에서 작업을 할당하려면 다음을 수행합니다.

1. 뷰에 지정 대상, 지정 또는 지정 필드가 있는 작업 목록으로 이동합니다.
1. (선택 사항) **자동 저장** 드롭다운 메뉴를 클릭하고 다음 옵션 중에서 선택합니다.

   | 옵션 | 옵션 설명 |
   |---|---| 
   | 자동 저장 | 작업에 대한 변경 사항은 자동으로 저장되며 되돌릴 수 없습니다. |
   | 수동 저장 | 변경 사항을 수동으로 저장해야 합니다. 저장하기 전에 변경 사항을 되돌릴 수 있습니다. |
   | 타임라인 계획 수립 | 변경 사항을 수동으로 저장해야 합니다. 저장하기 전에 변경 사항을 되돌릴 수 있습니다. 변경 사항 및 모든 프로젝트 종속성을 저장하는 것은 수동 저장을 선택하는 것보다 빠릅니다. |

   목록에서 작업을 편집할 때 저장하는 방법에 대한 자세한 내용은 [목록에서 작업 편집](../../../manage-work/tasks/manage-tasks/edit-tasks-in-a-list.md).

1. 작업을 할당하려면 다음 중 하나를 수행합니다.

   * 내부를 클릭합니다. **할당 대상** 또는 **할당됨** 필드에 작업에 지정할 활성 사용자의 이름을 입력한 다음 목록에 표시될 때 클릭합니다.
   * 내부를 클릭합니다. **할당** 필드에 작업을 할당할 활성 사용자, 작업 역할 또는 팀의 이름을 입력한 다음 목록에 표시될 때 클릭합니다.

     >[!TIP]
     >
     >사용자 할당을 추가할 때 아바타, 사용자의 기본 역할 또는 이메일 주소에 따라 이름이 동일한 사용자가 구분되는지 확인합니다. 사용자를 추가할 때 이를 보려면 사용자를 하나 이상의 작업 역할과 연결해야 합니다.
     >
     ><span class="preview">작업 역할 할당을 추가할 때 작업 역할이나 위치를 검색할 수 있습니다. 발령에 대한 기본 청구 요율을 사용하려면 시스템/기본 작업 역할을 선택하고, 요율 카드에서 청구 요율을 사용하려면 요율 카드 작업 역할을 선택합니다. 등급 카드에 대한 자세한 내용은 [등급 카드 관리](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/manage-rate-cards.md).</span>


1. (조건부) 다음 위치에 표시될 때 **할당** 필드를 클릭하고 **사람** 아이콘 을 클릭하여 할당 상자의 오른쪽 위 모서리에 있는 **고급 할당** 상자를 표시하고 고급 할당을 만듭니다.

   <!--
   there is a People icon in NWE but it's hard to see - you need to assign the task to at least 2 users, not roles, or teams, before it shows up</p>
   -->

   자세한 내용은 [고급 할당 만들기](../../../manage-work/tasks/assign-tasks/create-advanced-assignments.md).

   >[!TIP]
   >
   >할당 대상 또는 할당 대상 필드에서 고급 할당을 수행할 수 없습니다.

1. 자동 저장을 선택한 경우 작업에 피할당자를 추가한 후 Enter 키를 누르거나 페이지의 아무 곳이나 클릭하여 변경 사항을 저장합니다. 그렇지 않으면 **저장**.

## 사용자에게 여러 작업 할당

1. 일괄 할당할 작업 목록으로 이동합니다.
1. (조건부) 다음을 확인합니다. **자동 저장** 프로젝트 아래 작업 목록에 있는 경우 옵션이 선택됩니다.

   >[!IMPORTANT]
   >
   >프로젝트에 작업을 수동으로 저장할 때 작업을 일괄적으로 편집할 수 없습니다.

1. 작업 목록에서 여러 작업을 선택합니다.
1. 클릭 **편집**.

   다음 **작업 편집** 대화 상자가 열립니다.

1. 다음에서 **할당** 영역을 선택하고 **할당자** 그런 다음 모든 작업에 지정할 사용자, 작업 역할 또는 팀의 이름을 입력하십시오.

   >[!IMPORTANT]
   >
   >작업이 이미 할당된 경우 여기에 표시하는 리소스는 작업에 있는 기존 리소스를 대체하는 대신 작업에 추가됩니다.

1. (선택 사항) **작업 소유자** 열에 하나 이상의 자원을 작업에 지정할 때 기본 담당자 또는 작업 소유자인 자원을 나타냅니다. 이 기능은 팀에 사용할 수 없습니다.
1. (조건부) **할당 %** 선택한 모든 태스크에 기간 유형이 투입 고정 또는 계산된 지정인 경우 태스크에 지정된 각 자원에 대해. 이는 이러한 리소스가 작업 완료에 소비해야 하는 시간을 나타냅니다. 사용자 및 작업 역할에만 사용할 수 있습니다.

   또는

   금액 지정 **시간** 선택한 모든 작업의 기간 유형이 단순인 경우 작업에 할당된 각 리소스에 대해. 모든 리소스에 대한 총 시간 은 작업에 대한 계획된 시간 수와 같아야 합니다.

   >[!IMPORTANT]
   >
   >선택한 작업에 다른 기간 유형이 있거나 선택한 작업에 다른 기간 유형이 있는 경우 자원당 할당 백분율 또는 시간 수를 지정할 수 없습니다.

   작업의 기간 유형에 대한 자세한 내용은 을 참조하십시오 [작업 기간 및 기간 유형 개요](../../../manage-work/tasks/taskdurtn/task-duration-and-duration-type.md).

1. (선택 사항)에서 사용자가 작업에 대해 이행해야 하는 역할을 선택합니다. **역할 선택** 드롭다운 메뉴 **피할당자의 역할** 열을 사용하십시오. 역할을 선택하지 않으면 Workfront에서 자동으로 사용자의 기본 역할을 선택합니다.

1. (선택 사항) 모든 작업에서 기존 피할당자를 제거하려면 다음 중 하나를 수행합니다.

   1. 작업에서 제거할 사용자, 역할 또는 팀의 이름을 입력한 다음 목록에 표시될 때 선택하고 **피할당자 제거** 추가 피할당자를 제거합니다.
   1. 클릭 **기존 할당자 모두 제거** 을 눌러 선택한 모든 작업에서 모든 피할당자를 제거합니다.

1. 클릭 **변경 내용 저장**.
1. (선택 사항 및 조건부) 할당 대상 또는 할당 필드가 작업 목록에 표시되면 작업에 대해 이러한 열 중 하나를 클릭한 다음 **X 아이콘** 피할당자 이름 옆에 있는 을 클릭하여 작업에서 제거합니다.

<!--
<div data-mc-conditions="QuicksilverOrClassic.Draft mode">
<h2>Considerations about unassigning tasks</h2>
<p>(NOTE: moved this to the new article: /Content/Manage work/Tasks/Assign tasks/modify-task-assignments-overview.htm)</p>
<p>You can remove assignments from one task at a time, or you can remove assignments from multiple tasks in bulk.</p>
<p>For more information about removing assignments from tasks in bulk, see <a href="../../../manage-work/tasks/assign-tasks/modify-multiple-assignments-in-task-list.md" class="MCXref xref">Modify multiple user assignments in a task list</a>. </p>
<p>Consider the following when removing assignments from tasks: </p>
<ul>
<li>When you unassign a user from a task, the task remains assigned to the job role that the user fulfilled on the task.</li>
<li>When you unassign a job role or a team from a task, the task remains unassigned if it is not assigned to any other resources. </li>
</ul>
</div>
-->


