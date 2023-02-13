---
product-area: projects;user-management
navigation-topic: assign-tasks
title: 작업 목록에서 여러 사용자 할당 수정
description: 작업 지정을 관리할 때 작업 목록의 벌크 편집 기능을 사용하여 한 번에 여러 작업에 대해 동시에 수정할 수 있습니다.
author: Alina
feature: Work Management
exl-id: 04f7761f-da94-4858-85c5-8dc97bd78bee
source-git-commit: 3f5e5e9832fc33d39ea5dfbbc513b80adbf113f5
workflow-type: tm+mt
source-wordcount: '999'
ht-degree: 0%

---

# 작업 목록에서 여러 사용자 할당 수정

<!--
<p>There is a similar article in Resource Scheduling and a similar one for Issues; when things change, you might need to update all 3</p>
-->

작업 지정을 관리할 때 작업 목록의 벌크 편집 기능을 사용하여 한 번에 여러 작업에 대해 동시에 수정할 수 있습니다.

이 문서는 작업 목록의 여러 작업에 대한 여러 사용자 지정을 수정하는 것을 말합니다. 다른 영역의 여러 작업에 대한 할당을 수정하려면 다음 문서를 참조하십시오.

* 예약 영역에서 여러 작업에 대한 지정 수정에 대한 자세한 내용은 [예약 영역에서 작업에 할당된 여러 사용자를 수정합니다](../../../resource-mgmt/resource-scheduling/modify-multipl-assignments-scheduling-areas.md).
* 작업 로드 밸런서를 사용하여 작업을 지정하는 방법에 대한 자세한 내용은 [작업 로드 밸런서에서 작업 할당 개요](../../../resource-mgmt/workload-balancer/assign-work-in-workload-balancer.md).

목록의 한 리소스에 작업을 할당하는 방법에 대한 내용은 [작업 할당](../../../manage-work/tasks/assign-tasks/assign-tasks.md).

## 액세스 요구 사항

이 문서의 절차를 수행하려면 다음 액세스 권한이 있어야 합니다.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront 플랜*</td> 
   <td> <p>모든</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront 라이선스*</td> 
   <td> <p>작업 이상</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">액세스 수준 구성*</td> 
   <td> <p>프로젝트 및 작업에 대한 액세스 편집</p> <p>사용자에 대한 액세스 권한 보기 이상</p> <p>참고: 여전히 액세스 권한이 없는 경우 Workfront 관리자에게 액세스 수준에서 추가 제한 사항을 설정하는지 문의하십시오. Workfront 관리자가 액세스 수준을 수정하는 방법에 대한 자세한 내용은 <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">사용자 정의 액세스 수준 만들기 또는 수정</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">개체 권한</td> 
   <td> <p>작업에 대한 권한 기여</p> <p>추가 액세스 요청에 대한 자세한 내용은 <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">개체에 대한 액세스 요청 </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;어떤 계획, 라이선스 유형 또는 액세스 권한을 보유하고 있는지 알아보려면 Workfront 관리자에게 문의하십시오.

<!--
<div data-mc-conditions="QuicksilverOrClassic.Draft mode">
<h2>When to modify user assignments on tasks</h2>
<p>(NOTE: moved to the new article: /Content/Manage work/Tasks/Assign tasks/modify-task-assignments-overview.htm) </p>
<p>You might want to modify the user assignments for multiple tasks for a variety of reasons, including the following:</p>
<ul>
<li>Users join or leave your team</li>
<li> <p>A user takes a vacation that extends beyond task due dates</p> <note type="note">
When assigning users to work, their availability according to their schedules affects the Planned and Projected Dates of tasks. For information about schedules, see
<a href="../../../administration-and-setup/set-up-workfront/configure-timesheets-schedules/create-schedules.md" class="MCXref xref">Create a schedule</a>.
</note> </li>
<li>A specific role or user is set as the assignee for multiple tasks and you want to quickly modify all items to be assigned to a different user or role</li>
</ul>
<p><strong>How removing assignees affects task hours and allocation percentages</strong></p>
<p>(NOTE: move to the new article: /Content/Manage work/Tasks/Assign tasks/modify-task-assignments-overview.htm) </p>
<p>Removing users can affect task hours and allocation percentages. The effect that removing a user has on the task depends on the Duration Type that was selected for the task. For information about Duration&nbsp;Type, see <a href="../../../manage-work/tasks/taskdurtn/task-duration-and-duration-type.md" class="MCXref xref">Overview of Task Duration and Duration Type</a>.</p>
<p>When you delete a user from a task with the following Duration&nbsp;Types:</p>
<ul>
<li> <p><strong>Simple:</strong> The planned hours assigned to that user are subtracted from the task's total planned hours.</p> <note type="important">
<span class="s1">This could negatively affect your project plan because it changes the total planned hours for the task and the project.</span>
</note> </li>
<li><span class="s1"><strong>Effort Driven:</strong> The allocation percentage does not change for other users.</span> </li>
<li><span class="s1"><strong>Calculated Assignment:</strong> The allocation percentages of other users are adjusted so that the total equals 100%.</span> </li>
<li><span class="s1"><strong>Calculated Work:</strong> The allocation percentage does not change for other users.</span> </li>
</ul>
</div>
-->

## 여러 작업에 대한 할당 수정

1. 지정을 수정할 작업이 포함된 목록으로 이동합니다.
1. (선택 사항) 수정할 할당자에게 할당된 작업만 표시할 필터를 만듭니다.

   예를 들어 프로젝트에 여러 작업의 기본 담당자로 특정 역할이 포함되어 있는 경우 필터를 생성하여 해당 역할을 담당자로 사용하는 작업만 표시할 수 있습니다. 그런 다음 역할을 특정 사용자로 대체할 수 있습니다.

   필터 만들기에 대한 내용은 [필터 만들기 또는 편집](../../../reports-and-dashboards/reports/reporting-elements/create-filters.md).


1. 역할에 대해 필터링하려면 을 선택합니다. **할당 역할**&#x200B;를 클릭한 다음 **ID**.

   >[!TIP]
   >
   >를 사용하지 마십시오 **지정 대상** 필드. 이렇게 하면 작업에 할당할 수 있는 역할 대신 작업에 대한 기본 소유자만 찾습니다.

   또는

   사용자에 대해 필터링하려면 **할당 사용자,** 을 클릭한 다음 **ID.**

   >[!TIP]
   >
   >를 사용하지 마십시오 **지정 대상** 필드. 이렇게 하면 사용자에게 할당할 수 있는 사용자 대신 작업에 대한 기본 소유자만 찾습니다.

1. 할당을 수정할 작업을 선택한 다음 **편집** 아이콘 ![](assets/edit-icon.png).

   작업 편집 페이지가 표시됩니다. 편집하는 항목은 페이지의 왼쪽 위 모서리에 표시됩니다.

1. 로 이동합니다. **지정** 섹션을 참조하십시오.
1. 다음 중 하나를 수행하여 할당을 추가하거나 제거합니다.

   >[!IMPORTANT]
   >
   >할당을 제거하면 작업 시간 및 할당 백분율에 영향을 줄 수 있습니다. 자세한 내용은 섹션을 참조하십시오 [할당 제거 방법이 작업 시간 및 할당 백분율에 미치는 영향](#how-removing-assignees-affects-task-hours-and-allocation-percentages) 참조하십시오.

   * 새 할당자를 추가하려면

      1. 에서 **지정** 섹션, **할당자**.

         선택한 모든 작업에 공통인 정보가 표시됩니다. 예를 들어 동일한 사용자가 모든 작업에 할당되면 해당 사용자는 **할당자** 열. 선택한 작업 간에 정보가 일반적이지 않으면 정보가 표시되지 않습니다.

      1. 사용자, 역할 또는 팀의 이름을 입력하고 목록에 표시될 때 선택합니다. 할당이 추가되고 선택한 작업의 현재 할당을 대체하지 않습니다.
      >[!TIP]
      >
      > * 여러 사용자, 작업 역할 또는 팀을 할당할 수 있습니다. 활성 사용자, 작업 역할 및 팀만 할당할 수 있습니다.
      >   
      > * 사용자 지정을 추가할 때 아바타, 사용자의 기본 역할 또는 이메일 주소를 확인하여 동일한 이름을 사용하는 사용자를 구별하십시오. 사용자를 추가할 때 해당 역할을 보려면 사용자를 하나 이상의 작업 역할과 연결해야 합니다.

         > 
         >   사용자, 작업 역할 또는 팀이 비활성화되기 전에 할당된 경우 작업 항목에 지정된 상태로 유지됩니다. 이 경우 다음을 권장합니다.
         >   
         >     * 작업 항목을 활성 자원에 재지정합니다.
         >     * 비활성화된 팀의 사용자를 활성 팀과 연결하고 작업 항목을 활성 팀에 재할당합니다.



   * 개별 할당을 제거하려면 다음을 수행합니다.

      1. 을(를) 클릭합니다. **X 아이콘** 할당자가 지정 목록에 표시되는 경우 제거할 할당자의 이름 옆에 있습니다.

         또는

         (조건부) 할당자가 선택한 일부 작업에만 할당되어 제거하려는 할당자가 지정 섹션에 표시되지 않는 경우 을 클릭합니다 **할당자 제거** 제거할 할당자의 이름을 입력하고 드롭다운 목록에 나타나면 이름을 클릭합니다.
   * 기존 담당자를 모두 제거하려면

      1. 클릭 **기존 할당 모두 제거**&#x200B;를 클릭한 다음 **예, 모든 담당자 삭제**.

         따라서 편집 대화 상자에 표시되는 지정자뿐만 아니라 선택한 모든 작업의 지정자도 제거됩니다.
      작업에서 사용자를 제거하면 작업 시간 및 할당 백분율에 영향을 줄 수 있습니다.

      자세한 내용은 [작업 지정 수정 개요](../../../manage-work/tasks/assign-tasks/modify-task-assignments-overview.md).





1. (선택 사항) 할당자를 위해 다음 옵션을 수정합니다.

   * (조건부) **할당 % 또는 시간**: 새 할당 백분율 또는 시간을 지정합니다.

      >[!NOTE]
      >
      >편집 중인 모든 작업에서 기간 유형이 동일한 경우에만 이 옵션을 수정할 수 있습니다. 기간 유형이 계산된 작업 또는 투입 중심인 경우 할당 퍼센트를 갱신할 수 있습니다. 기간 유형이 단순하면 시간을 업데이트할 수 있습니다. 기간 유형에 대한 자세한 내용은 [작업 기간 및 기간 유형 개요](../../../manage-work/tasks/taskdurtn/task-duration-and-duration-type.md).
      필드가 비어 있으면 값이 작업 간에 다른 것입니다. 그러나 수정할 수 있습니다.

   * **작업 소유자**: 편집 중인 모든 작업에 대해 할당자를 작업 소유자로 만들려면 이 옵션을 선택합니다.
   * **할당자의 역할**: 드롭다운 목록에서 역할을 선택합니다. 선택하지 않은 경우 Adobe Workfront은 자동으로 사용자의 기본 역할을 선택합니다.

1. 클릭 **변경 사항을 저장합니다.**
