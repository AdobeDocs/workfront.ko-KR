---
content-type: overview
product-area: reporting
navigation-topic: reporting-elements
title: Adobe Workfront의 보기 개요
description: 목록이나 보고서의 보기를 관리하여 목록이나 보고서에 표시되는 정보 유형을 사용자 지정할 수 있습니다. 뷰에 객체와 해당 속성을 표시할 수 있습니다.
author: Lisa
feature: Reports and Dashboards
exl-id: 18016417-e24d-4797-9422-00915db47bb9
source-git-commit: 54f4c136cfaaaaaa90a4fc64d3ffd06816cff9cb
workflow-type: tm+mt
source-wordcount: '475'
ht-degree: 0%

---

# Adobe Workfront의 보기 개요

목록이나 보고서의 보기를 관리하여 목록이나 보고서에 표시되는 정보 유형을 사용자 지정할 수 있습니다. 뷰에 객체와 해당 속성을 표시할 수 있습니다. Adobe Workfront 객체에 대한 자세한 내용은 [Adobe Workfront의 개체 이해](../../../workfront-basics/navigate-workfront/workfront-navigation/understand-objects.md).

## 보기에 대한 고려 사항

* 기존 보기를 사용자 지정할 수 있습니다. 보기를 볼 수 있는 모든 사용자도 변경 사항을 볼 수 있습니다.
* 보기를 만들 수 있도록 Adobe Workfront 관리자가 필터, 보기 및 그룹을 편집할 수 있는 액세스 권한을 부여해야 합니다.

   편집 액세스 권한 부여에 대한 자세한 내용은 [필터, 보기 및 그룹화에 대한 액세스 권한 부여](../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-fvg.md).

* 보기에 대한 권한 수준은 보기가 저장되는 방식을 나타냅니다. 원래 뷰를 생성한 경우에는 변경 사항을 저장할 수 있습니다. 그렇지 않으면 뷰 버전을 저장하라는 메시지가 표시됩니다. 다른 사용자와 공유한 보기를 변경하면 해당 뷰에도 영향을 줍니다.
* 공유된 뷰를 공유한 사용자가 액세스 관리를 부여한 경우에만 사용자와 공유된 뷰를 사용자 정의할 수 있습니다. 보기 공유에 대한 자세한 내용은 [필터, 보기 또는 그룹화 공유](../../../reports-and-dashboards/reports/reporting-elements/share-filter-view-grouping.md).

기존 보기를 사용자 정의하거나, 기존 보기를 기반으로 새 보기를 만들거나, 처음부터 새 보기를 만들 수 있습니다.

## Workfront의 보기 유형

다음은 Workfront의 목록 또는 보고서에 적용할 수 있는 보기 유형입니다.

<table style="table-layout:auto">
    <tr>
        <td><strong>표준 보기</strong></td>
        <td>객체 목록이나 보고서에 적용할 수 있습니다. 표준 보기는 사용자 지정할 수 있습니다. 표준 보기를 사용자 지정하고 다른 사용자와 공유할 수 있습니다. 자세한 내용은 다음을 참조하십시오. <a href="/help/quicksilver/reports-and-dashboards/reports/reporting-elements/create-edit-views.md">Adobe Workfront에서 보기 만들기 또는 편집</a>.</td>
    </tr>
    <tr>
        <td><strong>민첩한 보기</strong></td>
        <td>프로젝트의 작업 섹션에 있는 작업 목록에 적용할 수 있습니다. 다른 사용자와 기민한 보기를 사용자 지정하고 공유할 수 있습니다. 자세한 내용은 <a href="/help/quicksilver/reports-and-dashboards/reports/reporting-elements/create-edit-views.md">Adobe Workfront에서 보기 만들기 또는 편집</a>.</td>
    </tr>
    <tr>
        <td><strong>간트 보기</strong></td>
        <td>프로젝트의 작업 섹션에 있는 작업 목록에 적용하거나 프로젝트 목록을 적용하거나 작업 또는 프로젝트 보고서에 추가할 수 있습니다. 미리 정의된 기본 제공 옵션을 사용하여 간트 보기에서 보는 정보를 사용자 지정할 수 있습니다. 작업 또는 프로젝트를 볼 수 있는 액세스 권한이 있는 모든 사용자는 Gantt 보기에서 볼 수 있습니다. 자세한 내용은 <a href="/help/quicksilver/manage-work/gantt-chart/use-the-gantt-chart/get-started-with-gantt.md">Gantt 차트 시작</a>.</td>
    </tr>
</table>

<!--
<div data-mc-conditions="QuicksilverOrClassic.Draft mode">
<h2>Create or customize a view</h2>
<p>(NOTE: drafted, because it has been moved to its own article: create-edit-views.htm) </p>
<p>The process for creating or customizing a view differs depending on whether you are creating or customizing a standard view or an agile view.</p>
<ul>
<li><a href="#create-or-customize-a-standard-view" class="MCXref xref">Create or customize a standard view</a> </li>
<li><a href="#create-or-customize-an-agile-view" class="MCXref xref">Create or customize an Agile view</a> </li>
</ul>
<p><strong>Create or customize a standard view</strong></p>
<p>You can create a new standard view, or you can customize an existing standard view that you previously created.</p>
<ol>
<li value="1">Click the<strong>View</strong> drop-down menu on any list where you want to create or customize a view.</li>
<li value="2">(Optional) To customize an existing view, select the standard View you want to customize.<br>Standard Views are available on any type of list in Workfront, such as a report, project list, or task list.</li>
<li value="3">Click the <strong>View</strong> drop-down menu, then click <strong>Customize View</strong> or<strong>New View</strong>.<br>The <strong>Customize View</strong> dialog box displays.<br></li>
<li value="4"> <p>In the <strong>Column Preview</strong> section, do any of the following:</p>
<ul>
<li>Modify the value of any column by clicking the column title and then selecting a new field.</li>
<li>Add a column by clicking <strong>Add Column</strong>, begin typing the name of the column that you want to add, then click it when it appears in the drop-down list.</li>
<li>Adjust the order that columns appear by dragging the column title to a new location.
<ul>
<li>(Optional) In the <strong>Column Settings</strong> area, click the <strong>Summarize this column by</strong> drop-down list, then select one of the available options for summarizing the information. When you choose this option, the information in your column is aggregated in the groupings of the report.<br>For date fields, you can summarize the values by the following options:
<ul>
<li>Maximum</li>
<li>Minimum</li>
</ul><p>For number and currency fields, you can summarize the values by the following options:</p>
<ul>
<li>Count</li>
<li>Sum</li>
<li>Average</li>
<li>Maximum</li>
<li>Minimum</li>
</ul> <note type="note">  
<p>The following exceptions apply for parent objects (for example, parent tasks) when you are aggregating values for the following fields in groupings:</p>
<ul>
<li>All the number and currency fields except Actual Hours (for example, Planned/ Actual Labor Cost, Planned/ Actual Expense Cost, Planned/ Actual Cost, Planned Hours) aggregate only the values for the children tasks, and standalone tasks. They do not aggregate the values for the parent tasks or parents of parents.</li>
<li>Actual Hours aggregate the values for the main parent and the standalone tasks; they do not aggregate the numbers for the parents of parent tasks or the children tasks.</li>
<li>Custom data fields for number and currency values aggregate all tasks: parents, children, parents of parents, and standalone tasks.</li>
</ul>
</note><p>For more information about using groupings in a report, see the article <a href="../../../reports-and-dashboards/reports/reporting-elements/groupings-overview.md" class="MCXref xref">Groupings overview in Adobe Workfront</a>.</p></li>
<li>(Optional) Click <strong>Advanced Options</strong> to specify the following information for the column:<p>
<table style="table-layout:auto">
<col>
<col>
<thead>
<tr>
<th> </th>
<th> </th>
</tr>
</thead>
<tbody>
<tr>
<td role="rowheader"><strong>Custom Column Label</strong></td>
<td><p>Specify a custom label for the column. This label replaces the default label.</p></td>
</tr>
<tr>
<td role="rowheader"><strong>Field Format</strong></td>
<td>Select the format in which you want the values to be displayed for fields in the column.</td>
</tr>
<tr>
<td role="rowheader"><strong>Show this column when on a Dashboard</strong></td>
<td><p>Select this option to show this column on a dashboard, when the report is displayed side by side with another report. When this option is unselected, this column is not displayed when viewing the report on a dashboard where reports are displayed side by side.</p></td>
</tr>
<tr>
<td role="rowheader"><strong>Column Rules</strong></td>
<td><p>Click <strong>Add a Rule for this Column</strong> to define a rule for the column. After you add a rule, you can define field and text styles for how fields that match that rule are displayed. Click <strong>Add Rule</strong> after you have finished defining the rule.</p></td>
</tr>
</tbody>
</table></p><p>For more information about conditionally formatting views in reports, see the article <a href="../../../reports-and-dashboards/reports/text-mode/use-conditional-formatting-text-mode.md" class="MCXref xref">Use conditional formatting in Text Mode</a>.</p></li>
</ul></li>
</ul> </li>
<li value="5">(Conditional) If you clicked <strong>Advanced Options</strong>, click <strong>Done</strong>.</li>
<li value="6"> <p>Click <strong>Save View</strong> to create a new View or to replace the current View with your changes.<br>Or<br>Click <strong>Save as New View</strong> to save your changes as a new View.</p> <note type="tip">
The
<strong>Save as New View</strong> is the only option available when you customize a built-in Workfront view.
</note> <p>Your access dictates how the view is saved. If you created the view originally, you can save the changes; otherwise, you are prompted to save a version. Keep in mind that changes you make to the view impact users with whom the view has been shared.</p> </li>
</ol>
<p><strong>Create or customize an Agile view</strong></p>
<p>You can create a new Agile view or customize an existing Agile view that you previously created.</p> <note type="important">
Agile views are available only when viewing a project.
</note>
<p>For more information about Agile views, see the article <a href="../../../manage-work/projects/manage-projects/manage-projects-in-agile-view.md" class="MCXref xref">Manage a project in the Agile View</a>.</p>
<p>(NOTE: Alina: [! The information in the following steps is more or less duplicated in "Creating and Managing Agile Teams."]) </p>
<p>To create or customize an Agile view:</p>
<ol>
<li value="1">Go to the list of tasks on a project.</li>
<li value="2">Click the <strong>Agile</strong> icon .<br></li>
<li value="3">(Conditional) To customize an existing Agile view:
<ol>
<li value="1">Click the <strong>View</strong> drop-down menu, then select the Agile View you want to customize.<br>You cannot customize the default Agile view.</li>
<li value="2">Click the <strong>View</strong> drop-down menu again, then click <strong>Customize View</strong>.<br><img src="assets/view-agile-customize.png" alt=""></li>
</ol></li>  
<li value="4">(Conditional) To create a new Agile view, click <strong>New View</strong>.<br>The <strong>Customize Agile View</strong> dialog box displays.<br></li>
<li value="5">In the <strong>Customize Agile View</strong> dialog box, specify a name for the Agile view.<br>We recommend that you include the word "Agile" in your view name, so users know this is an Agile view.<br>This name is displayed in the <strong>View</strong> drop-down menu when selecting a view.</li>
<li value="6"> <p>Define the status columns to display on the story board in the agile view. These are the task statuses that are defined by the Workfront administrator, as described in <a href="../../../administration-and-setup/customize-workfront/creating-custom-status-and-priority-labels/create-or-edit-a-status.md" class="MCXref xref">Create or edit a status</a>.</p> <p>Only system statuses are available to use on the Agile story board. If a status is available only for an individual group you are a member of, the status is not available on the agile story board. Furthermore, tasks that are in a status that is available only to a custom group are not visible when viewing the project in an Agile view.</p> <p>Users can move stories among these status columns on the Agile story board.<br>When defining status columns, you can do the following:</p> <p>
<table style="table-layout:auto">
<col>
<col>
<thead>
<tr>
<th> </th>
<th> </th>
</tr>
</thead>
<tbody>
<tr>
<td role="rowheader"><strong>Reorder status columns:</strong> </td>
<td> Drag a status column to the order where you want it to appear.<br><img src="assets/agile-project-reorderstatuses-350x141.png" alt="" style="width: 350;height: 141;"></td>
</tr>
<tr>
<td role="rowheader"><strong>Remove status columns:</strong> </td>
<td>Click the (x) icon on the column that you want to remove.<br>You cannot remove the "New" status unless a custom status has been added to the view and that custom status equates with "New."<br>For information about creating a custom status, see <a href="../../../administration-and-setup/customize-workfront/creating-custom-status-and-priority-labels/create-or-edit-a-status.md" class="MCXref xref">Create or edit a status</a>.</td>
</tr>
<tr>
<td role="rowheader"><strong>Add status columns:</strong> </td>
<td> <p>Click the <strong>Plus</strong> icon, then select the status you want to add.<br>All default system statuses are displayed, as well as any custom statuses that have been shared with you.<br>You can configure up to 10 statuses to display.</p> 
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: Alina: research this and add: [! What if the status has been shared with me or a group I'm in (so I can see it here), but the status hasn't been shared with another user who also has access to a project where I later apply this view? Can that user still see this status on the project?])</p>
</td>
</tr>
</tbody>
</table> </p> <p> </p> <p> </p> </li>
<li value="7"> <p>In the <strong>Associate Card Color to</strong> area, select from the following options: </p> <p>
<table style="table-layout:auto">
<col>
<col>
<thead>
<tr>
<th> </th>
<th> </th>
</tr>
</thead>
<tbody>
<tr>
<td role="rowheader"><strong>Story:</strong> </td>
<td>Any subtasks match the color of the parent task, so that the colors of all stories in any given swimlane are the same.<br>Colors are randomly assigned to tasks when they are created if the task does not have any subtasks or does not have a parent task.</td>
</tr>
<tr>
<td role="rowheader"><strong>Free Form:</strong> </td>
<td> All cards are displayed as blue by default until a user changes the color manually, as described in the article <a href="../../../agile/use-scrum-in-an-agile-team/scrum-board/categorize-stories-by-color.md" class="MCXref xref">Categorize stories by color on the Scrum board</a>. </td>
</tr>
<tr>
<td role="rowheader"><strong>Priority:</strong> </td>
<td> <p> Colors are associated with the story priority, as follows:</p>
<ul>
<li>High = Red</li>
<li>Medium = Yellow</li>
<li>Low = Green<br>If your Workfront administrator has configured custom priorities for your Workfront system, the highest priority is red, the second-highest is yellow, and the remaining are green.</li>
</ul> </td>
</tr>
<tr>
<td role="rowheader"><strong>Task Owner:</strong> </td>
<td> All stories with the same primary assignee are the same color.<br>The primary assignee is the user who was first assigned to the task. </td>
</tr>
</tbody>
</table> </p> </li>
<li value="8"> <p>In the <strong>Agile</strong> section, in the <strong>Additional Fields</strong> area, click <strong>Add Field</strong>, then select the field you want to add to story cards. (These are the same fields you can add when creating customizing a view or creating columns for a report.)<br>Repeat this process to add up to 3 additional fields to the story cards.<br>When you add fields to story cards, fields are view-only and display only when the field is populated.</p> <p>By default, the following types of data is displayed on the story card:</p>
<ul>
<li>Story name with a link directly to the task</li>
<li>The project name with a link directly to the project<br>This link is displayed only when using the agile view on an iteration; it is not displayed when using an Agile view on a project.</li>
<li>The task description</li>
<li>Current commitment</li>
<li>View and edit the percent complete either by adjusting the percent complete itself or by adjusting the number of points or hours that are complete</li>
<li>Assigned Users</li>
</ul> <p>You can display additional data (including custom data) on story cards. You might want to display additional fields on story cards for any number of reasons. For example, you might want to display the Customer ID if you are working on stories for multiple customers within the project, or you might want to display the Task Start Date.</p> </li>
<li value="9">Click <strong>Save</strong>.<br>Your access dictates how the View is saved. If you created the View originally, you can save the changes; otherwise, you are prompted to save a version. Keep in mind that changes you make to the View impact users with whom the View has been shared.</li>
</ol>
</div>
-->

## 보기 공유

보기를 공유하는 방법에 대한 자세한 내용은 [필터, 보기 또는 그룹화 공유](../../../reports-and-dashboards/reports/reporting-elements/share-filter-view-grouping.md).

## 보기 제거

보기를 처음 만들었는지 또는 보기가 사용자와 공유되었는지에 따라 보기를 제거하는 기능은 다르게 작동합니다. 기본 보기는 제거할 수 없습니다.

자세한 내용은 [필터, 보기 및 그룹화 제거](../../../reports-and-dashboards/reports/reporting-elements/remove-filters-views-groupings.md).

<!--
<div data-mc-conditions="QuicksilverOrClassic.Draft mode">
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: drafted this content because it is repeating in the article linked above.)</p>
<ul>
<li><strong>If you created the view and you remove it</strong>, the view is removed from the Workfront system. The view is no longer available to any users who you previously shared it with.</li>
<li><strong>If the view was shared with you and you remove it</strong>, the view is removed only for you. The user who originally created it and any other users it has been shared with still have access to the view.</li>
</ul>
<p>To remove a view:</p>
<ol>
<li value="1">To remove a standard view, ensure that you are currently viewing a standard view.<br>Or<br>To remove an Agile view, ensure that you are currently viewing an agile view.</li>
<li value="2"> <p>Go to a list of objects, and in the <strong>View</strong> drop-down menu, click <strong>Remove View</strong>.<br>The <strong>My Views</strong> dialog box displays.<br><br>If you are deleting a standard view, all standard views that you have rights to remove are available to remove.</p> <p>If you are deleting an Agile view, all Agile views that you have rights to remove are available to remove.</p> <p>Standard views or Agile views that you do not have rights to remove display as dimmed.<br></p> </li>
<li value="3">Click the <strong>x</strong> icon next to any views you want to remove, then click <strong>Done</strong>.</li>
</ol>
</div>
-->
