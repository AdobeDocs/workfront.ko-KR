---
content-type: overview
product-area: projects
navigation-topic: plan-a-project
title: 프로젝트 계획 완료 일자 설정
description: 프로젝트의 계획된 완료 일자는 프로젝트가 완료되도록 설정된 일자입니다.
author: Alina
feature: Work Management, Projects
role: User
exl-id: 996398c5-de92-445e-8e86-36b2efdcf6b5
source-git-commit: dbc4404501e20b3f1905a5eebd13734a65db27ae
workflow-type: tm+mt
source-wordcount: '523'
ht-degree: 4%

---

# 프로젝트 계획된 완료 일자 설정

<!-- Audited: 4/2025 -->

프로젝트의 계획된 완료 일자는 프로젝트가 완료되도록 설정된 일자입니다.

프로젝트의 계획된 시작 및 계획된 완료 일자는 프로젝트에 대한 작업 일자에 따라 달라집니다. 이 문서에서는 프로젝트의 계획된 완료 일자를 수동 또는 자동으로 설정하는 방법에 대해 설명합니다. 작업의 계획된 완료 날짜에 대한 자세한 내용은 [작업의 계획된 완료 일자 개요](../../../manage-work/tasks/task-information/task-planned-completion-date.md)를 참조하십시오.

프로젝트의 계획된 완료 일자는 시작 일자부터 또는 완료 일자부터 프로젝트를 스케줄링하는지에 따라 수동 또는 자동으로 설정할 수 있습니다.

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
   <p>플랜</p>
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader">액세스 수준 구성</td> 
   <td> <p>프로젝트에 대한 액세스 편집</p>  </td> 
  </tr> 
  <tr> 
   <td role="rowheader">개체 권한</td> 
   <td> <p>프로젝트에 대한 권한 관리</p> </td> 
  </tr> 
 </tbody> 
</table>

이 표의 정보에 대한 자세한 내용은 [Workfront 설명서의 액세스 요구 사항](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)을 참조하십시오.

+++

<!--Old:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront plan</td> 
   <td> <p>Any</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront license</td> 
   <td><p>
   New: Standard

   Or

   Current: Plan </p>
   
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Access level configurations</td> 
   <td> <p>Edit access to Projects</p> <p><b>NOTE</b>
   
   If you still don't have access, ask your Workfront administrator if they set additional restrictions in your access level. For information on how a Workfront administrator can modify your access level, see <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Create or modify custom access levels</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Object permissions</td> 
   <td> <p>Manage permissions to the project</p> <p>For information on requesting additional access, see <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Request access to objects </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>-->

## 프로젝트의 계획된 완료 일자 수동 설정

완료 일자부터 프로젝트를 예약할 때 프로젝트의 계획된 완료 일자를 수동으로 설정해야 합니다.

>[!NOTE]
>
>프로젝트의 계획된 완료 일자를 수동으로 설정하면 Workfront은 모든 작업의 기간을 기반으로 프로젝트의 계획된 시작 일자를 자동으로 계산합니다.


완료 일자부터 프로젝트를 스케줄링하려면

{{step1-to-projects}}

1. **새 프로젝트**&#x200B;를 클릭한 다음 드롭다운에서 **새 프로젝트**&#x200B;을 선택합니다.

   프로젝트 만들기에 대한 자세한 내용은 문서 [프로젝트 만들기](../../../manage-work/projects/create-projects/create-project.md)를 참조하십시오.

1. 왼쪽 패널에서 **프로젝트 세부 정보**&#x200B;을(를) 선택합니다.

1. 오른쪽 상단의 **프로젝트 편집** 아이콘 ![편집 아이콘](/help/quicksilver/manage-work/projects/planning-a-project/assets/qs-edit-icon.png)을 클릭한 다음 나타나는 드롭다운에서 **개요**&#x200B;를 선택합니다.

1. **프로젝트 날짜** 섹션에서 **일정 모드** 필드를 클릭한 다음 **완료 날짜**&#x200B;를 선택합니다.

1. 프로젝트의 **계획된 완료 일자**&#x200B;를 지정하십시오.
1. **변경 내용 저장**&#x200B;을 클릭합니다.

   프로젝트에 작업을 추가할 때 프로젝트의 **계획된 시작 일자**&#x200B;는 모든 작업의 총 기간을 기반으로 계산됩니다.

## 프로젝트의 계획된 완료 일자 자동 설정

프로젝트의 계획된 완료 일자는 시작 일자부터 프로젝트를 예약할 때 Workfront에 의해 자동으로 계산됩니다.

시작 일자부터 프로젝트를 스케줄링하려면

{{step1-to-projects}}

1. **새 프로젝트**&#x200B;를 클릭한 다음 나타나는 드롭다운에서 **새 프로젝트**&#x200B;을 선택합니다.

   프로젝트 만들기에 대한 자세한 내용은 문서 [프로젝트 만들기](../../../manage-work/projects/create-projects/create-project.md)를 참조하십시오.

1. 왼쪽 패널에서 **프로젝트 세부 정보**&#x200B;을(를) 선택합니다.

1. 오른쪽 상단의 **프로젝트 편집** 아이콘 ![편집 아이콘](/help/quicksilver/manage-work/projects/planning-a-project/assets/qs-edit-icon.png)을 클릭한 다음 나타나는 드롭다운에서 **개요**&#x200B;를 선택합니다.

1. **프로젝트 날짜** 섹션에서 **일정 모드** 필드를 클릭한 다음 **시작 날짜**&#x200B;를 선택합니다.

1. 프로젝트의 **계획된 시작 일자**&#x200B;를 지정하십시오.
1. **변경 내용 저장**&#x200B;을 클릭합니다.

   프로젝트에 작업을 추가하면 프로젝트의 **계획된 완료 일자**&#x200B;가 모든 작업의 총 기간을 기반으로 계산됩니다.

   작업 기간에 대한 자세한 내용은 문서 [작업 기간 및 기간 유형 개요](../../../manage-work/tasks/taskdurtn/task-duration-and-duration-type.md)를 참조하십시오.

   이 경우 프로젝트의 계획된 완료 일자와 프로젝트의 마지막 작업의 계획된 완료 일자가 일치합니다.

<!--
<div data-mc-conditions="QuicksilverOrClassic.Draft mode">
<h2>The Planned Completion Date of a task</h2>
<p>(NOTE: drafted because I created a new article, here: /Content/Manage work/Tasks/Task information/task-planned-completion-date.htm)</p>
<p>You can either specify the Planned Completion Date of a task, or you can leave it up to Workfront to calculate it depending on certain criteria. </p>
<ul>
<li><a href="#manually-set-the-planned-completion-date-of-a-task" class="MCXref xref">Manually set the Planned Completion Date of a task</a> </li>
<li><a href="#how-the-planned-completion-date-is-calculated-for-a-task" class="MCXref xref">How the Planned Completion Date is calculated for a task</a> </li>
</ul>
<p><strong>Manually set the Planned Completion Date of a task</strong></p>
<p>Setting the Planned Completion Date of a task depends on the type of Task Constraint you assign to the task. </p>
<p>You can manually set the Planned Completion Date when creating a task, as described in the article <a href="../../../manage-work/tasks/create-tasks/create-tasks-in-project.md" class="MCXref xref">Create tasks in a project</a>.</p>
<p>You can manually specify the Planned Completion Date when you select any of the following Task Constraints: </p>
<table border="1" cellspacing="15" cellpadding="1">
<col>
<col>
<thead>
<tr>
<th> <p><strong>Task Constraint Type</strong> </p> </th>
<th> <p><strong>Effect of Manually Changing the Planned Completion Date</strong> </p> </th>
</tr>
</thead>
<tbody>
<tr>
<td> <p>Must Finish On</p> <p>Finish No Later Than</p> <p>Finish No Earlier Than</p> </td>
<td> <p><span class="s1">The Planned Start Date is adjusted in order to keep the Duration the same.</span> </p> </td>
</tr>
<tr>
<td> <p>Fixed Dates</p> </td>
<td> <p>The Duration is adjusted in order to keep the Planned Start Date the same.</p> </td>
</tr>
</tbody>
</table>
<p><strong>How the Planned Completion Date is calculated for a task</strong></p>
<p>When it is calculated automatically by the system, the following can influence the Planned Completion Date of a Task:</p>
<ul>
<li> <p>Task Constraint</p> <p>For more information about Task Constraints, see the article <a href="../../../manage-work/tasks/task-constraints/task-constraint-overview.md" class="MCXref xref">Task Constraint overview</a>.</p> </li>
<li> <p>Task predecessor relationship</p> <p>For more information about task predecessors, see the article <a href="../../../manage-work/tasks/use-prdcssrs/predecessors-overview.md" class="MCXref xref">Overview of task predecessors</a>.</p> </li>
<li>Project Completion Date, when the project is scheduled from Completion Date.</li>
<li> <p>The time off schedule of the Primary Assignee of the task. </p> <p>When the Primary Assignee has time off scheduled during the duration of the task, the planned dates of the task adjust accordingly when the <strong>Consider user time off in task durations</strong> setting is selected for the <strong>User Time Off</strong> field. New projects inherit this setting from the Project Preferences area, but you can edit the setting at the project level. </p> <p>For example, if a task with a Constraint of As Soon As Possible is scheduled to start on June 1 and complete on June 3, and the Primary Assignee has June 2 marked for Time-off, the task Planned Completion Date becomes June 4. </p> <p>For information about the <strong>User Time Off</strong> preference, see the articles <a href="../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-project-preferences.md" class="MCXref xref">Configure system-wide project preferences</a> or <a href="../../../manage-work/projects/manage-projects/edit-projects.md" class="MCXref xref">Edit projects</a>.</p> </li>
</ul>
<p>When set automatically, the Planned Completion Date is determined based on the following calculation: </p>
<p><code>Planned Completion Date = Planned Start Date + Duration</code> </p>
<p>For example, if your task has a start date of September 16 and a duration of 10 days, the Planned Completion Date is September 26.</p> <note type="note">
 The Update Type for the project must also be set to Automatic and On Change or Automatically in order for the Planned Hours and Duration to be automatically adjusted.
<br>For more information about the Update Type, see the article
<a href="../../../manage-work/projects/manage-projects/select-project-update-type.md" class="MCXref xref">Select the project Update Type </a>.
</note>
</div>
-->
