---
product-area: projects;user-management
navigation-topic: assign-tasks
title: 작업 목록에서 여러 사용자 할당 수정
description: 작업 할당을 관리할 때 작업 목록의 일괄 편집 기능을 사용하여 한 번에 여러 작업에 대해 동시에 수정할 수 있습니다.
author: Lisa
feature: Work Management, Tasks, Resource Management
role: User
exl-id: 04f7761f-da94-4858-85c5-8dc97bd78bee
source-git-commit: ac24b2486b9fc5a0b8c2944a6ec240140238b908
workflow-type: tm+mt
source-wordcount: '932'
ht-degree: 0%

---

# 작업 목록에서 여러 사용자 할당 수정

<!--Audited: 11/2025-->

<!--
this article is similar and updates on this one might need to be repeated here: help/quicksilver/manage-work/issues/manage-issues/edit-assignments-for-multiple-issues.md</p>
-->

<!--<div class="preview"> 

The highlighted information on this page refers to functionality not yet generally available. It is available only in the Preview environment for all customers. The same features will also be available in the Production environment for all customers starting with a week from the Preview release.      

For more information, see [Interface modernization](/help/quicksilver/product-announcements/product-releases/interface-modernization/interface-modernization.md).  

</div> -->

작업 할당을 관리할 때 작업 목록의 일괄 편집 기능을 사용하여 한 번에 여러 작업에 대해 동시에 수정할 수 있습니다.

이 문서에서는 작업 목록의 여러 작업에 대한 여러 사용자 할당을 수정하는 것을 의미합니다. 다른 영역의 여러 작업에 대한 할당을 수정하려면 다음 문서를 참조하십시오.

* 업무 균형자를 사용하여 작업을 할당하는 방법에 대한 자세한 내용은 [업무 균형자에서 작업 할당 개요](../../../resource-mgmt/workload-balancer/assign-work-in-workload-balancer.md)를 참조하십시오.

목록의 리소스 하나에 작업을 할당하는 방법에 대한 자세한 내용은 [작업 할당](../../../manage-work/tasks/assign-tasks/assign-tasks.md)을 참조하십시오.

## 액세스 요구 사항

+++ 을 확장하여 이 문서의 기능에 대한 액세스 요구 사항을 봅니다.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>Adobe Workfront 패키지</td> 
   <td> <p>임의</p> </td> 
  </tr> 
  <tr> 
   <td>Adobe Workfront 라이선스</td> 
   <td> <p>표준</p>
   <p>작업 이상</p>
   </td> 
  </tr> 
  <tr> 
   <td>액세스 수준 구성</td> 
   <td> <p>프로젝트 및 작업에 대한 액세스 편집</p> <p>사용자에 대한 보기 또는 상위 액세스 권한</p> </td> 
  </tr> 
  <tr> 
   <td>개체 권한</td>
   <td>작업에 대한 또는 더 높은 권한 기여</td>
  </tr>
 </tbody>
</table>

자세한 내용은 [Workfront 설명서의 액세스 요구 사항](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)을 참조하십시오.

+++

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
<p>Removing users can affect task hours and allocation percentages. The effect that removing a user has on the task depends on the Duration Type that was selected for the task. For information about Duration Type, see <a href="../../../manage-work/tasks/taskdurtn/task-duration-and-duration-type.md" class="MCXref xref">Overview of Task Duration and Duration Type</a>.</p>
<p>When you delete a user from a task with the following Duration Types:</p>
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

1. 할당을 수정할 작업이 포함된 목록으로 이동합니다.
1. (선택 사항) 필터를 생성하여 수정하려는 할당자에게 할당된 작업만 표시합니다.

   예를 들어, 프로젝트에 여러 작업의 기본 피할당자로 특정 역할이 포함된 경우 해당 역할을 피할당자로 사용하는 작업만 표시하도록 필터를 만들 수 있습니다. 그런 다음 역할을 특정 사용자로 바꿀 수 있습니다.

   필터 만들기에 대한 자세한 내용은 [필터 만들기 또는 편집](../../../reports-and-dashboards/reports/reporting-elements/create-filters.md)을 참조하세요.


1. 역할을 필터링하려면 **할당 역할**&#x200B;을 선택한 다음 **ID**&#x200B;을(를) 클릭합니다.

   >[!TIP]
   >
   >**할당 대상** 필드를 사용하지 마십시오. 할당된 역할 대신 작업에 대한 기본 소유자만 찾습니다.

   또는

   사용자를 필터링하려면 **할당 사용자,**&#x200B;를 선택한 다음 **ID.**&#x200B;를 클릭하십시오.

   >[!TIP]
   >
   >**할당 대상** 필드를 사용하지 마십시오. 할당된 사용자가 아닌 작업에 대한 기본 소유자만 찾습니다.

1. 할당을 수정할 작업을 선택한 다음 **편집** 아이콘 ![](assets/edit-icon.png)을(를) 클릭합니다.

   **작업 편집** 상자가 <!--<span class="preview">in the new experience</span>--> 열립니다.

   <!--1. <span class="preview">(Optional) Click **Switch to old experience** at the bottom of the **Edit Tasks** box.</span> 
   <span class="preview">The **Edit Tasks** box opens in the old experience.</span>-->

1. **할당** 섹션으로 이동합니다.

   >[!IMPORTANT]
   >
   >피할당자를 제거하면 작업 시간 및 할당 비율에 영향을 줄 수 있습니다. 자세한 내용은 이 문서의 섹션 [피할당자 제거가 작업 시간 및 할당 비율에 미치는 방식](#how-removing-assignees-affects-task-hours-and-allocation-percentages)을 참조하십시오.
1. 다음 중 하나를 수행하여 피할당자를 추가하거나 제거합니다.

   * 새 피할당자를 추가하려면:

      1. **할당** 섹션에서 **피할당자**&#x200B;를 선택합니다.

         선택한 모든 작업에서 공통되는 정보가 표시됩니다. 예를 들어, 동일한 사용자가 모든 작업에 할당되면 해당 사용자는 **피할당자** 열에 표시됩니다. 선택한 작업에서 정보가 공통되지 않으면 정보가 표시되지 않습니다.

      1. 사용자, 역할 또는 팀의 이름을 입력한 다음 목록에 표시될 때 선택합니다. 할당이 추가되고 선택한 작업에 대한 현재 할당이 대체되지 않습니다.


     >[!TIP]
     >
     > * 여러 사용자, 작업 역할 또는 팀을 할당할 수 있습니다. 활성 사용자, 작업 역할 및 팀만 할당할 수 있습니다.
     >   
     > * 사용자 할당을 추가할 때 아바타, 사용자의 기본 역할 또는 이메일 주소에 따라 이름이 동일한 사용자가 구분되는지 확인합니다. 사용자를 추가할 때 이를 보려면 사용자를 하나 이상의 작업 역할과 연결해야 합니다. 사용자의 이메일을 보려면 사용자의 액세스 수준에서 연락처 정보 보기 설정을 활성화해야 합니다. 자세한 내용은 [사용자에게 액세스 권한 부여](../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-other-users.md)를 참조하십시오.
     > 
     >   비활성화되기 전에 사용자, 작업 역할 또는 팀이 할당된 경우 작업 항목에 할당된 상태로 유지됩니다. 이 경우 다음 사항을 권장합니다.
     >   
     >     * 작업 항목을 활성 리소스에 재할당합니다.
     >     * 비활성화된 팀의 사용자를 활성 팀과 연결하고 작업 항목을 활성 팀에 재할당합니다.


   * 개별 피할당자를 제거하려면 다음 작업을 수행하십시오.

      1. 피할당자가 할당 목록에 표시되면 제거할 피할당자의 이름 옆에 있는 **X 아이콘**&#x200B;을 클릭합니다.

         또는

         (조건부) 선택한 작업 중 일부에만 할당되어 제거할 할당자가 할당 섹션에 표시되지 않는 경우 **할당자 제거**&#x200B;를 클릭하고 제거할 할당자의 이름을 입력한 다음 드롭다운 목록에 표시될 때 이름을 클릭합니다.

   * 기존 피할당자를 모두 제거하려면 다음 작업을 수행하십시오.

      1. **기존 피할당자 모두 제거**&#x200B;를 클릭한 다음 **예, 모든 피할당자 삭제**&#x200B;를 클릭합니다.

         이렇게 하면 공통 할당자(편집 대화 상자에 표시된 할당자)뿐만 아니라 선택한 모든 작업의 모든 할당자가 제거됩니다.

     작업에서 사용자를 제거하면 작업 시간 및 할당 비율에 영향을 줄 수 있습니다.

     자세한 내용은 [작업 할당 수정 개요](../../../manage-work/tasks/assign-tasks/modify-task-assignments-overview.md)를 참조하십시오.

1. (선택 사항) 피할당자에 대해 다음 옵션 중 하나를 수정합니다.

   * (조건부) **할당 % 또는 시간**: 새 할당 백분율 또는 시간을 지정하십시오.

     >[!NOTE]
     >
     >편집 중인 모든 작업에서 기간 유형이 동일한 경우에만 이 옵션을 수정할 수 있습니다. 기간 유형이 계산된 작업량 또는 작업량 고정 유형인 경우 할당 %를 갱신할 수 있습니다. 기간 유형이 단순하면 시간을 업데이트할 수 있습니다. 기간 유형에 대한 자세한 내용은 [작업 기간 및 기간 유형 개요](../../../manage-work/tasks/taskdurtn/task-duration-and-duration-type.md)를 참조하십시오.
     >
     >
     >필드가 비어 있으면 작업 간에 값이 다르지만 수정할 수 있습니다.

   * **작업 소유자**: 피할당자를 편집 중인 모든 작업에 대한 작업의 소유자로 설정하려면 이 옵션을 선택하십시오.
   * **피할당자의 역할**: 드롭다운 목록에서 역할을 선택합니다. 선택하지 않으면 Adobe Workfront이 자동으로 사용자의 기본 역할을 선택합니다.

1. **변경 내용 저장**&#x200B;을 클릭합니다.

<!--
1. <span class="preview"> (Optional) Click **Try new experience** in the upper-right corner of the **Edit Tasks** box. The Edit Tasks box opens in the new experience. Do one of the following:</span>

   <div class="preview">

   * To add assignees, start typing the name of an assignee in the **Search people, roles, or teams** field, then select them when they display in the list. 
   * To remove assignees, click the **x** icon to the right of their name. Only assignees that are common to all tasks display in the list. 
   * Click Assign to me to assign the selected tasks to yourself.

   </div>
1. <span class="preview">(Conditional) When using the new experience, click **Save**.</span>

-->
