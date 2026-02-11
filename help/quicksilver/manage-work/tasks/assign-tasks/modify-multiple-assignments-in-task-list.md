---
product-area: projects;user-management
navigation-topic: assign-tasks
title: 작업 목록에서 여러 사용자 할당 수정
description: 작업 할당을 관리할 때 작업 목록의 일괄 편집 기능을 사용하여 한 번에 여러 작업에 대해 동시에 수정할 수 있습니다.
author: Lisa
feature: Work Management, Tasks, Resource Management
role: User
exl-id: 04f7761f-da94-4858-85c5-8dc97bd78bee
source-git-commit: 21c98e443a6d6ca79045e2f4aba5f792340833cd
workflow-type: tm+mt
source-wordcount: '762'
ht-degree: 3%

---

# 작업 목록에서 여러 사용자 할당 수정

<!--Audited: 11/2025-->

<!--remove the old/new experience references when the toggles are removed-->

<!--
this article is similar and updates on this one might need to be repeated here: help/quicksilver/manage-work/issues/manage-issues/edit-assignments-for-multiple-issues.md</p>
-->

<!--<div class="preview"> 

The highlighted information on this page refers to functionality not yet generally available. It is available only in the Preview environment for all customers. The same features will also be available in the Production environment for all customers starting with a week from the Preview release.      

For more information, see [Second Quarter 2026 release overview](/help/quicksilver/product-announcements/product-releases/26-q2-release-activity/26-q2-release-overview.md).  

</div>-->

작업 할당을 관리할 때 작업 목록의 일괄 편집 기능을 사용하여 한 번에 여러 작업에 대해 동시에 수정할 수 있습니다.

이 문서에서는 작업 목록의 여러 작업에 대한 여러 사용자 할당을 수정하는 것을 의미합니다. 다른 영역의 여러 작업에 대한 할당을 수정하려면 다음 문서를 참조하십시오.

* 업무 균형자를 사용하여 작업을 할당하는 방법에 대한 자세한 내용은 [업무 균형자에서 작업 할당 개요](../../../resource-mgmt/workload-balancer/assign-work-in-workload-balancer.md)를 참조하십시오.

목록의 리소스 하나에 작업을 할당하는 방법에 대한 자세한 내용은 [작업 할당](../../../manage-work/tasks/assign-tasks/assign-tasks.md)을 참조하십시오.

## 액세스 요구 사항

+++ 이 문서의 기능에 대한 액세스 요구 사항을 보려면 확장하십시오.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>Adobe Workfront 패키지</td> 
   <td> <p>Any</p> </td> 
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

1. 할당을 수정할 작업을 선택한 다음 **편집** 아이콘 ![편집 아이콘](assets/edit-icon.png)을 클릭합니다.

   1. 피할당자를 추가하거나 제거하려면 다음 중 하나를 수행합니다.

      * 피할당자를 추가하려면 **사람, 역할 또는 팀 검색** 필드에 피할당자의 이름을 입력한 다음 목록에 표시될 때 선택하십시오.

        선택한 작업의 기존 할당자에 새 할당자가 추가됩니다.
      * 피할당자를 제거하려면 **피할당자 제거** 상자에서 피할당자의 이름을 클릭합니다

        또는

        **기존 피할당자 모두 제거**&#x200B;를 클릭합니다.

        할당자는 선택한 모든 작업에서 제거됩니다.

        작업에서 사용자를 제거하면 작업 시간 및 할당 비율에 영향을 줄 수 있습니다.

        자세한 내용은 [작업 할당 수정 개요](../../../manage-work/tasks/assign-tasks/modify-task-assignments-overview.md)를 참조하십시오.


        >[!TIP]
        >
        >* 여러 사용자, 작업 역할 또는 팀을 할당할 수 있습니다. 활성 사용자, 작업 역할 및 팀만 할당할 수 있습니다.
        >   
        >* 사용자 할당을 추가할 때 아바타, 사용자의 기본 역할 또는 이메일 주소에 따라 이름이 동일한 사용자가 구분되는지 확인합니다. 사용자를 추가할 때 이를 보려면 사용자를 하나 이상의 작업 역할과 연결해야 합니다. 사용자의 이메일을 보려면 사용자의 액세스 수준에서 연락처 정보 보기 설정을 활성화해야 합니다. 자세한 내용은 [사용자에게 액세스 권한 부여](../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-other-users.md)를 참조하십시오.
        > 
        >   비활성화되기 전에 사용자, 작업 역할 또는 팀이 할당된 경우 작업 항목에 할당된 상태로 유지됩니다. 이 경우 다음 사항을 권장합니다.
        >   
        >* 작업 항목을 활성 리소스에 재할당합니다.
        >* 비활성화된 팀의 사용자를 활성 팀과 연결하고 작업 항목을 활성 팀에 재할당합니다.


   1. (선택 사항) 피할당자에 대해 다음 옵션 중 하나를 수정합니다.

      * (조건부) **할당 % 또는 시간**: 새 할당 백분율 또는 시간을 지정하십시오.

      >[!NOTE]
      >
      >편집 중인 모든 작업에서 기간 유형이 동일한 경우에만 이 옵션을 수정할 수 있습니다. 기간 유형이 계산된 작업량 또는 작업량 고정 유형인 경우 할당 %를 갱신할 수 있습니다. 기간 유형이 단순하면 시간을 업데이트할 수 있습니다. 기간 유형에 대한 자세한 내용은 [작업 기간 및 기간 유형 개요](../../../manage-work/tasks/taskdurtn/task-duration-and-duration-type.md)를 참조하십시오.
      >
      >
      >필드가 비어 있으면 작업 간에 값이 다르지만 수정할 수 있습니다.

      * **기본으로 설정**: 선택한 작업 위로 마우스를 가져간 후 이 옵션을 선택하여 피할당자를 편집 중인 모든 작업에 대한 작업의 소유자로 설정합니다.
      * **피할당자의 역할**: 드롭다운 목록에서 역할을 선택합니다. 선택하지 않으면 Adobe Workfront이 자동으로 사용자의 기본 역할을 선택합니다.
      * **기간 유형**
      * **기간**
      * **계획된 시간**

   1. **저장**&#x200B;을 클릭합니다.

<!-- temporary content - for Assignments redesign:

Editing assignments on tasks differs depending on which environment you choose. 

1. (Conditional) If you are using the Production environment to assign tasks, the **Edit Tasks** box opens in the new experience. Do the following in the Production environment: 

   1. To add or remove assignees, do one of the following:

      * To add assignees, start typing the name of an assignee in the **Search people, roles, or teams** field, then select them when they display in the list. 
      * To remove assignees, click the **x** icon to the right of their name. Only assignees that are common to all tasks display in the list. 
      * Click Assign to me to assign the selected tasks to yourself.

   1. (Conditional) When using the new experience, click **Save**.

   1. (Optional) Click **Switch to old experience** at the bottom of the **Edit Tasks** box.
      
      The **Edit Tasks** box opens in the old experience.

   1. (Conditional) In the old experience, do the following to modify the assignees:

      1. Go to the **Assignments** section.

         >[!IMPORTANT]
         >
         >Removing assignees can affect the task hours and allocation percentages. For more information, see the section [How removing assignees affects task hours and allocation percentages](#how-removing-assignees-affects-task-hours-and-allocation-percentages) in this article.

      1. Do one of the following to add or remove assignees:

         * To add a new assignee:

            1. In the **Assignments** section, select **Assignee**.

               Information that is common across all tasks selected displays. For example, if the same user is assigned to all tasks, that user displays in the **Assignee** column. If information is not common across the tasks selected, no information displays.
            
            1. Start typing the name of a user, role, or team, then select it when it displays in the list. The assignment is added and does not replace the current assignments on the selected tasks.

            >[!TIP]
            >
            > * You can assign multiple users, job roles, or teams. You can assign only active users, job roles, and teams.
            >   
            > * When adding a user assignment, notice the avatar, the user's Primary Role, or their email address to distinguish between users with identical names. Users must be associated with at least one job role to view it as you add them. You must have the View Contact Info setting enabled in your access level for Users to view users' emails. For information, see [Grant access to users](../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-other-users.md).
            > 
            >   If a user, job role, or a team was assigned before they were deactivated, they remain assigned to the work item. In this case, we recommend the following:
            >   
            >     * Reassign the work item to active resources.
            >     * Associate the users in a deactivated team with an active team and reassign the work item to the active team.


         * To remove individual assignees:

            1. Click the **X icon** next to the name of the assignee that you want to remove if the assignee displays in the Assignments list.

               Or

               (Conditional) If the assignee that you want to remove does not display in the Assignments section because the assignee is assigned to only some of the tasks that you have selected, click **Remove Assignee** and start typing the name of the assignee that you want to remove, then click the name when it appears in the drop-down list.

         * To remove all existing assignees:

            1. Click **Remove All Existing Assignees**, then click **Yes, Delete All Assignees**.

               This removes not only common assignees (assignees that are displayed in the edit dialog box), but also all assignees on all the selected tasks.

            Removing users from tasks can affect task hours and allocation percentages.
            
            For more information, see [Overview of modifying task assignments](../../../manage-work/tasks/assign-tasks/modify-task-assignments-overview.md).

      1. (Optional) Modify any of the following options for assignees:

         * (Conditional) **Allocation % or Hours**: Specify a new allocation percentage or hours.

         >[!NOTE]
         >
         >This option can be modified only if the Duration Type is the same across all tasks that are being edited. When the Duration Type is Calculated Work or Effort Driven you can update the Allocation %. When the Duration Type is Simple you can update the Hours. For information about Duration Type, see [Overview of Task Duration and Duration Type](../../../manage-work/tasks/taskdurtn/task-duration-and-duration-type.md).
         >
         >
         >If the field is blank, this means that the value is different across tasks; however, you are still able to modify it.

         * **Task Owner**: Select this option to make the assignee the owner of the task for all tasks being edited.
         * **Assignee's Role**: Select a role from the drop-down list. If left unselected, Adobe Workfront automatically selects the Primary Role of the user. 

      1. Click **Save Changes.**
        

1. <span class="preview">(Conditional) If you are using the Preview environment to assign tasks, the **Edit Tasks** box opens. Do the following in the Preview environment: </span>

   <div class="preview">-->





