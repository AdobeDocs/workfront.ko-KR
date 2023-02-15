---
product-area: resource-management
navigation-topic: the-workload-balancer
title: 작업 로드 밸런서에서 작업 할당 개요
description: 리소스 관리자는 Adobe Workfront 작업 로드 밸런서를 사용하여 사용자에게 아직 할당되지 않은 작업 항목을 보고 이러한 항목을 할당할 수 있습니다.
author: Alina
feature: Resource Management
exl-id: 98779b67-b975-4501-8426-63e255b1d7df
source-git-commit: 3486a2523a038bdd83c3c2001001a119fd0508ad
workflow-type: tm+mt
source-wordcount: '983'
ht-degree: 0%

---

# 작업 로드 밸런서에서 작업 할당 개요

<!--drafted for Work Time story:
<span class="preview">The highlighted information on this page refers to functionality not yet generally available. It is available only in the Preview environment.</span> 
-->

리소스 관리자는 Adobe Workfront 작업 로드 밸런서를 사용하여 사용자에게 아직 할당되지 않은 작업 항목을 보고 이러한 항목을 할당할 수 있습니다.

작업 로드 밸런서에 대한 일반적인 정보는 다음을 참조하십시오 [작업 로드 밸런서 개요](../../resource-mgmt/workload-balancer/overview-workload-balancer.md).

Workfront의 다른 영역에서 사용자에게 작업 항목(작업 및 문제)을 할당할 수 있습니다. 그러나 Workload Balancer를 사용하면 사용자의 가용성을 쉽게 파악하고 다른 모든 항목을 명확히 볼 수 있으므로 작업 시간을 더 많이 할당할 수 있습니다.

Workfront의 다른 영역에서 작업 항목을 지정하는 방법에 대한 자세한 내용은 다음 문서를 참조하십시오.

* [작업 할당](../../manage-work/tasks/assign-tasks/assign-tasks.md)
* [문제 할당](../../manage-work/issues/manage-issues/assign-issues.md)

## 작업 로드 밸런서의 사용자 가용성

작업 로드 밸런서에서 사용자의 사용 가능한 시간과 일치하도록 작업을 지정할 수 있습니다. 사용자에게 적합한 작업 금액을 할당하고 초과 할당하지 않도록 하려면 사용자에게 할당된 작업 항목의 총 계획 시간의 합계가 사용자 일별 또는 주별 할당과 일치해야 합니다.

Workfront이 사용자의 사용 가능한 시간을 계산하는 방법을 이해해야 합니다.

Workfront은 다음 정보를 사용하여 작업 로드 밸런서에서 사용자의 용량을 계산합니다.

* 리소스 관리 기본 설정입니다. Workfront 관리자는 설정의 리소스 관리 영역에서 다음 중 하나를 사용하도록 선택하여 시스템에 대해 사용 가능한 시간을 계산하는 방법을 결정합니다.

   * Workfront 시스템의 기본 일정 및 사용자의 FTE입니다.
   * 사용자 프로필 영역에 표시된 사용자의 일정입니다.

      이 경우 사용자의 일별 및 주별 가용성을 계산합니다. 선택한 스케줄에 대한 모든 스케줄 예외는 작업 로드 밸런서에서 사용자의 능력에 반영됩니다.
   자세한 내용은 [리소스 관리 환경 설정 구성](../../administration-and-setup/set-up-workfront/configure-system-defaults/configure-resource-mgmt-preferences.md).

   예약에 대한 자세한 내용은 [예약 만들기](../../administration-and-setup/set-up-workfront/configure-timesheets-schedules/create-schedules.md)

* 사용자의 시간입니다. 사용자가 이륙할 날짜를 나타냅니다.

   자세한 내용은 [Adobe Workfront에서 개인 시간 설정](../../workfront-basics/manage-your-account-and-profile/configuring-your-user-profile/personal-time-overview.md).

<!--drafted for Work Time: 
* The user's Work Time. This indicates the percentage of FTE time that the user is available to perform actual project-related work, not including overhead. Set the Work Time value to  1 to indicate that the user is available for project-related work their entire full-time equivalent. -->

## 작업 로드 밸런서에서 작업 할당

사용자에게 아직 할당되지 않은 작업 항목을 할당하거나 작업 로드 밸런서에서 사용자에게 할당된 항목을 재할당할 수 있습니다.

다음과 같은 방법으로 작업 로드 밸런서에서 작업을 할당할 수 있습니다.

* 각 항목을 수동으로 할당하여 한 번에 한 개 품목.

   품목을 수동으로 한 번에 하나씩 지정할 때 고급 지정을 수행할 수 있습니다.

   자세한 내용은 [작업 로드 밸런서를 사용하여 수동으로 작업 할당](../../resource-mgmt/workload-balancer/assign-work-in-workload-balancer-manually.md).

* 작업 항목을 할당해야 하는 사용자에게 끌어다 놓아 한 번에 한 개의 항목을 드래그하여 놓습니다.

   자세한 내용은 [드래그 앤 드롭으로 작업 로드 밸런서에서 작업 할당](../../resource-mgmt/workload-balancer/assign-work-in-workload-balancer-by-drag-and-drop.md).

* 일괄 지정 옵션을 사용하여 한 번에 여러 항목을 지정합니다. 한 번에 여러 사용자에게 항목을 할당하는 규칙을 정의할 수 있습니다.

   자세한 내용은 [작업 로드 밸런서를 사용하여 일괄 작업 할당](../../resource-mgmt/workload-balancer/assign-work-in-workload-balancer-in-bulk.md).

작업 할당 해제에 대한 자세한 내용은 [작업 로드 밸런서에서 작업 할당 취소](../../resource-mgmt/workload-balancer/unassign-work-in-workload-balancer.md).

## 작업 로드 밸런서의 지정 영역

자원 조정 영역, 프로젝트 또는 팀 레벨에서 작업 로드 밸런서를 사용하여 사용자에게 작업을 할당할 수 있습니다. 작업 로드 밸런서가 Workfront에 있는 위치에 대한 자세한 내용은 [작업 로드 밸런서를 찾습니다.](../../resource-mgmt/workload-balancer/locate-workload-balancer.md).

작업 로드 밸런서에는 작업 항목을 볼 수 있는 두 가지 영역이 있습니다.

* **할당되지 않은 작업**: 사용자에게 할당되지 않은 항목을 표시합니다.
* **지정된 작업 시간**: 사용자에게 할당된 항목을 표시합니다.

다음 표에서는 지정된 내용에 따라 각 영역에 표시되는 항목을 설명합니다.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td><strong>할당 유형</strong> </td> 
   <td colspan="2"><strong>할당이 표시되는 영역</strong> </td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td>미할당 작업 </td> 
   <td>할당된 작업 </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td><span style="font-weight: normal;">지정되지 않은 항목</span> </td> 
   <td><span>✔</span> </td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>팀</td> 
   <td>✔</td> 
   <td> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td><span data-mc-edit-date="2020-04-08T15:57:40.7175506-04:00" data-mc-editor="alinawilson" data-mc-comment="Drafted because role only is not displayed; first it will be displayed in Unassigned - 20.2 beta" data-mc-initials="AL" data-mc-creator="alinawilson" data-mc-create-date="2019-11-15T13:24:04.5189150-05:00">역할</span> </td> 
   <td><span>✔</span> </td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>역할 및 팀</td> 
   <td>✔</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>사용자</td> 
   <td> </td> 
   <td>✔</td> 
  </tr> 
  <tr> 
   <td>사용자 및 팀</td> 
   <td> <p> </p> </td> 
   <td>✔</td> 
  </tr> 
  <tr> 
   <td>사용자, 역할 및 팀</td> 
   <td>✔*</td> 
   <td>✔**</td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> <p>사용자 및 역할</p> </td> 
   <td><span data-mc-edit-date="2019-11-15T13:37:42.5435254-05:00" data-mc-editor="alinawilson" data-mc-comment="drafted because it's not in the Unassigned" data-mc-initials="AL" data-mc-creator="alinawilson" data-mc-create-date="2019-11-15T13:37:33.3097484-05:00">✔</span>*</td> 
   <td>✔**</td> 
  </tr> 
 </tbody> 
</table>

&#42;작업 항목이 사용자 및 역할에 지정되면 해당 역할이 주 할당자인 경우에만 미지정 작업 영역에 표시됩니다.

&#42;&#42;작업 항목이 사용자 및 다른 엔티티에 지정되면 사용자가 기본 할당자인 경우에만 지정된 작업 영역에 표시됩니다.

작업 로드 밸런서의 지정되지 않음 및 할당된 영역에 대한 자세한 내용은 다음을 참조하십시오 [작업 로드 밸런서 탐색](../../resource-mgmt/workload-balancer/navigate-the-workload-balancer.md).

## Job 역할, 팀 및 사용자에게 여러 지정 고려 사항

여러 리소스를 작업 항목에 할당할 때 다음 사항을 고려하십시오.

* 사용자는 프로필과 연결된 두 개 이상의 작업 역할을 가질 수 있습니다. 사용자와 작업 역할 연결에 대한 자세한 내용은 [사용자 프로필 편집](../../administration-and-setup/add-users/create-and-manage-users/edit-a-users-profile.md).

* 작업 또는 문제는 일반적으로 하나 이상의 작업 역할이나 팀에 먼저 할당됩니다. 프로젝트를 시작할 준비가 되면 사용자에게 할당해야 할 수도 있습니다.\
   작업 또는 문제가 하나 이상의 역할에 할당되어 있고 그 다음 사용자도 할당하면 Adobe Workfront에서 다음 규칙에 따라 추가 사용자(있는 경우)와 연결할 작업 역할을 결정합니다.

   * 할당된 작업 역할이 하나만 있고 사용자의 기본 역할과 일치하는 경우 해당 작업이나 문제는 기본 역할을 수행하는 사용자만 할당됩니다.
   * 여러 개의 역할이 할당되고 역할 중 하나 이상이 사용자의 보조 역할과 일치하는 경우 해당 작업이나 문제가 다른 역할 중 하나를 수행하는 사용자에게 할당됩니다. 즉, Workfront에서 일치하는 항목이 여러 개 있으면 무작위로 선택합니다. 또한 할당된 추가 역할과 해당 역할 중 하나 이상이 할당됩니다.
   * 하나 이상의 작업 역할이 할당되어 있고 사용자의 역할에 일치하는 항목이 없는 경우 해당 작업이나 문제는 사용자뿐만 아니라 역할이나 역할 모두에 할당됩니다.

* 작업이나 문제가 팀에 할당되어 있고 사용자도 할당하면 작업이나 문제가 팀과 사용자 모두에 할당된 상태로 유지됩니다.

<!--
<div data-mc-conditions="QuicksilverOrClassic.Draft mode">
<h2 data-mc-conditions="QuicksilverOrClassic.Quicksilver"> Manually assign one item at a time</h2>
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: Moved manual assignment and drag-and-drop to their own articles) </p>
<ol>
<li value="1">Go to the Workload Balancer.</li>
<li value="2"> <p>Go to the <strong>Unassigned Work</strong> area and apply a filter to view work items</p> <p>Or</p> <p>Go to the <strong>Assigned Work</strong> area and expand the name of a user to view the work items assigned to them.</p> <note type="important">
<span>You cannot view and assign issues from the Unassigned Work area. You can only reassign issues already assigned to users in the Assigned Work area. Otherwise,</span> you can assign issues from a list or at the issue level. For information, see
<a href="../../manage-work/issues/manage-issues/assign-issues.md" class="MCXref xref">Assign issues</a>.
</note> </li>
<li value="3"> <p>Click the <strong>More menu</strong> <img src="assets/qs-more-menu.png"> on the bar of a work item, then click <strong>Assign this to</strong>. </p> <p> <img src="assets/workload-balancer-assign-this-to-link-from-task-350x117.png" style="width: 350;height: 117;"> </p> <note type="tip">
<p><span>You can also use the following shortcuts to assign tasks or issues:</span> </p>
<ul>
<li><span>In Windows: CTRL+click the task or issue bar.</span> </li>
<li><span>In&nbsp;Mac: CMD+click the task or issue bar.</span> </li>
</ul>
</note> </li>
<li value="4"> <p>Start typing the name of a user, job role, or team that you want to assign to the item in the <strong>Search people, role or teams</strong> field, select it when it displays in the list, then click&nbsp;<strong>Save</strong>. </p> <p> <img src="assets/assignments-box-wb.png"> </p> <p>This assigns or reassigns the work item to the specified assignees.</p> <p>If you assign an item to just a team or a job role, the item displays only in the Unassigned Work area. You must assign work items to users in order to display them in the Assigned Work area of the Workload Balancer.</p> <note type="tip">
<p>You can assign multiple users or job roles, and you can assign only one team. <span>You can assign only active users, <span>job roles</span>, and teams.</span></p>
<p><span>If a user, <span>job role</span>, or a team was assigned before they were deactivated, they remain assigned to the work item. In this case, we recommend the following:</span> </p>
<ul>
<li> <p><span>Reassign the work item to active resources.</span> </p> </li>
<li> <p><span>Associate the users in a deactivated team with an active team and reassign the work item to the active team.</span> </p> </li>
</ul>
</note> </li>
<li value="5"> <p>(Optional) Click the <strong>Show allocations icon</strong> <img src="assets/show-allocations-icon-small.png">, then click the <strong>More menu</strong> <img src="assets/qs-more-menu.png"> > <strong>Edit allocations</strong>.</p> <p>Or</p> <p>Double-click a daily or weekly allocation to modify the amount of time the user is allocated to the work item.</p> <p>For information about modifying user allocations in the Workload Balancer, see the "Modify user allocations"&nbsp;section in the article <a href="../../resource-mgmt/workload-balancer/manage-user-allocations-workload-balancer.md" class="MCXref xref">Manage user allocations in the Workload Balancer</a>.</p> </li>
</ol>
<div data-mc-conditions="QuicksilverOrClassic.Quicksilver">
<h2>Assign an item by dragging and dropping</h2>
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: consider retitling this to "Assign one item at a time by dragging and dropping" when bulk assignments will come???)&nbsp;</p>
<p>You can assign an item from the Unassigned Work area to a user, or you can reassign an already assigned item to another user in the Assigned Work area.</p>
<ol>
<li value="1">Go to the Workload Balancer.</li>
<li value="2"> <p>Go to the <strong>Unassigned Work</strong> area and apply a filter to view work items.</p> <note type="important">
<span>You cannot view and assign issues from the Unassigned Work area.</span>
</note> </li>
<li value="3"> <p>Click the bar of a work item that indicates either the planned or the projected timeline and drag it over the name of a user in the <strong>Assigned</strong> area.</p> <p>The user you hover over to drop the work item to is highlighted.</p> <note type="tip">
The Planned Hours for the user you're hovering over update in real time with the number of daily Planned Hours from the work item, to indicate what the impact of adding a new item might be to their overall allocation.
</note> <p> <img src="assets/drag-drop-item-from-unassigned-to-assigned-wb-nwe-350x152.png" style="width: 350;height: 152;"> </p> </li>
<li value="4"> <p>When you are ready, drop the selected work item in the same line as the user's name in the Assigned Area. The item is assigned and the allocated Planned Hours are updated for the user with the new hours from the work item.</p> <note type="tip">
<p>If you enabled Group by Project in the Settings area, the assigned task displays under the corresponding project. If the setting is disabled, the assigned task displays in the user area. </p>
<p>The item displays according to the Workload Balancer criteria for sorting work items.&nbsp;For more information, see <a href="../../resource-mgmt/workload-balancer/navigate-the-workload-balancer.md" class="MCXref xref">Navigate the Workload Balancer</a>.</p>
</note> </li>
<li value="5"> <p>(Optional) Click the <strong>Show allocations icon</strong> <img src="assets/show-allocations-icon-small.png">, then click the <strong>More menu</strong> <img src="assets/qs-more-menu.png"> > <strong>Edit allocations</strong>. (NOTE: make sure these are still called this, and that the icon has not changed)</p> <p>Or</p> <p>Double-click a daily or weekly allocation to modify the amount of time the user is allocated to the work item.</p> <p>For information about modifying user allocations in the Workload Balancer, see the "Modify user allocations"&nbsp;section in the article <a href="../../resource-mgmt/workload-balancer/manage-user-allocations-workload-balancer.md" class="MCXref xref">Manage user allocations in the Workload Balancer</a>.</p> </li>
</ol> 
<div data-mc-conditions="QuicksilverOrClassic.Draft mode">
<h2>Assign items in bulk</h2>
<p>(NOTE: This is also a separate article. Should we keep this section or the separate article?) </p>
</div>
<p>&nbsp;</p>
</div>
</div>
-->

<!--
<div data-mc-conditions="QuicksilverOrClassic.Draft mode">
<h2>Unassign work items in the Workload Balancer</h2>
<p>(NOTE: moved this section to a new article. Draft here at release to preview) </p>
<p>You can either unassign items from users and move them to the Unassigned Work area, or reassign them to other users. </p>
<p>To unassign work items from users: </p>
<ol>
<li value="1">In the Workload Balancer, go to the <strong>Assigned Work</strong> area and expand a user.</li>
<li value="2">Do 
<MadCap:conditionalText data-mc-conditions="QuicksilverOrClassic.Draft mode">
one of
</MadCap:conditionalText>
the following:
<ul>
<li class="preview" data-mc-conditions="QuicksilverOrClassic.Draft mode"><p>Find the item you want to unassign in a user's area, click it, drag and drop it in the Unassigned area or in another user's area. </p></li>
<li><p>Click the <strong>More</strong> icon <img src="assets/more-icon-task-list.png"> to the right of the name of a work item, click&nbsp;<strong>Assign this to</strong> , then remove the name of the entities assigned to the work item or enter another name and click&nbsp;<strong>Save</strong>.</p><p><img src="assets/workload-balancer-assign-this-to-link-from-task-350x117.png" style="width: 350;height: 117;"></p></li>
</ul><p>The item displays in the Unassigned Work area if it matches the filtering criteria for that area and it is not assigned to any users or it displays in the user area if it is assigned to that user. </p><note type="tip">
Unassigned issues do not display in the Unassigned area.
</note><p>For information about filtering information in the Workload Balancer, see <a href="../../resource-mgmt/workload-balancer/filter-information-workload-balancer.md" class="MCXref xref">Manage filters in the Workload Balancer</a>. </p></li>
</ol>
</div>
-->
