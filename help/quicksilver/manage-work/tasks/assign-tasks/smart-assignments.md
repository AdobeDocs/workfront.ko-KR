---
content-type: overview;how-to-procedural
product-area: projects;user-management
navigation-topic: assign-tasks
title: 스마트 할당 개요
description: 작업 및 문제 할당을 관리할 때 스마트 할당을 사용하여 작업을 완료하는 데 가장 적합한 사용자를 식별할 수 있습니다. 스마트 할당은 작업에 가장 적합한 리소스를 결정하는 알고리즘을 기반으로 리소스에 작업 항목을 할당할 때 Adobe Workfront이 제공하는 제안입니다.
author: Lisa
feature: Work Management
exl-id: 8d17eff6-5ff0-4985-b575-4934a3bb7c0b
source-git-commit: 259fd0e3fdaa07bfdb0301d60bf0d9b1090b4ef7
workflow-type: tm+mt
source-wordcount: '556'
ht-degree: 0%

---

# 스마트 할당 개요

<!--Audited: 07/2024-->

<!--keep the yellow around the Rate card job roles and the Preview intro for those-->

<span class="preview">이 페이지에서 강조 표시된 정보는 미리 보기 환경에서만 사용할 수 있는 기능을 참조합니다.</span>

<!--<span class="preview">For information about fast releases, see [Enable or disable fast releases for your organization](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/enable-fast-release-process.md).</span>

<span class="preview"> This functionality will be removed from the Production environment for customers who enabled fast release with the 25.1 release in January 2025. For information about the 25.1 release, see [First Quarter 2025 release overview](/help/quicksilver/product-announcements/product-releases/25-q1-release-activity/25-q1-release-overview.md). -->

작업 및 문제 할당을 관리할 때 스마트 할당을 사용하여 작업을 완료하는 데 가장 적합한 리소스를 식별할 수 있습니다.

스마트 할당은 작업에 가장 적합한 리소스를 결정하는 알고리즘을 기반으로 리소스에 작업 항목을 할당할 때 Adobe Workfront이 제공하는 제안입니다. 스마트 할당은 사용자, 작업 역할 또는 팀이 될 수 있습니다.

>[!NOTE]
>
>사용자를 제안할 때 스마트 할당은 사용자의 가용성을 고려하지 않습니다. 하지만 일정에 따른 가용성은 작업 및 문제의 계획 및 예상 일자에 영향을 미칩니다. 일정에 대한 자세한 내용은 문서 [일정 만들기](../../../administration-and-setup/set-up-workfront/configure-timesheets-schedules/create-schedules.md)를 참조하십시오.

이 문서에는 스마트 할당에 대한 일반 정보가 포함되어 있습니다. 스마트 할당을 사용하여 사용자에게 작업 및 문제를 할당하는 방법에 대한 자세한 내용은 [스마트 할당 만들기](../../../manage-work/tasks/assign-tasks/make-smart-assignments.md)를 참조하십시오.

## 스마트 할당 개요

스마트 할당으로 작업할 때 다음 사항을 고려하십시오.

<!--* <span class="preview">The algorithm works independently for tasks and issues. This means that the list of suggested users for issues might differ from the list of suggested users for a task because Workfront builds the lists according to criteria pertaining to issues and tasks separately. </span>-->
<!--not sure this is accurate: * Smart assignments do not recommend job roles or teams. Instead, they are suggestions of users who are best fit to complete a task or an issue. -->
* 제안된 할당은 항상 활성 사용자, 작업 역할 또는 팀입니다.
* 먼저 나열된 리소스는 작업에 가장 적합한 리소스여야 합니다.

## 스마트 할당 제안 찾기

다음 영역에서 작업 또는 문제를 할당할 수 있는 스마트 할당을 볼 수 있습니다.

* 할당 열의 문제 목록 또는 보고서

  ![](assets/smart-assignments-issue-list.png)

* 할당 열의 작업 목록 또는 보고서

  ![](assets/smart-assignments-task-list.png)

* 할당 필드의 작업 헤더

  ![](assets/smart-assignments-task-header-nwe-350x302.png)

* 할당 필드의 문제 헤더

  ![](assets/smart-assignments-issue-header.png)

* 할당 영역의 작업 또는 문제 요약 패널

  ![](assets/issue-assignments-summary-panel.png)

<!--* The Assignments field in the New Task box, when adding a task to a project

  ![](assets/smart-assignments-new-task-modal.png)-->

<!--this is not possible in the new home  - we have Summary there: 
* The Assignments field for an item listed in the Home area, when you open a task or issue

  ![](assets/smart-assignments-in-home-nwe-350x216.png)
-->

* 작업 또는 문제를 할당할 때 할당 대상 영역의 업무 균형자

  ![](assets/smart-assignments-workload-balancer-bulk-assignments.png)


## 스마트 할당 기준

<!--Smart assignments work differently for tasks than for issues.  -->

<!--### Smart assignments criteria for tasks

The task smart assignments calculation works in <span class="preview">two phases which use two different algorithms.</span>

<span class="preview">Depending on which algorithm finds the smart assignment, the assignments are listed under two separate sections in the Assignments field.</span> For information, see [Make smart assignments](/help/quicksilver/manage-work/tasks/assign-tasks/make-smart-assignments.md). 

![](assets/smart-assignments-task-list.png)

<div class="preview">

#### First phase of smart assignment calculation for tasks 

In the first phase of calculating smart assignments, Workfront calculates a similarity score for every assignment. 

>[!NOTE]
>
>The first phase of the smart assignments calculation does not apply to the following task areas:
>
>* Bulk Assignments in the Workload Balancer.
>* Connected cards on boards.


The calculation for the similarity score and the order in which the assignments are listed take into account the following:  

* A score of 100% is given to an existing assignment where the task, project, and portfolio names are identical to the task you're trying to assign. The project and portfolio names of the task of an existing assignment must also match the project and portfolio of the task you are trying to assign.   

* If only some of this information from other assignments matches on the existing tasks, the score might be lower than 100%.  

  For example, if you are assigning a task called "My second task" on a project called "My project" in a portfolio called "My portfolio" and you have an existing task called "My task" in another project called "My project" in a portfolio called "My portfolio", the user assigned to "My task" might get a score of 95% because the name of the existing task and the task you're trying to assign now are similar, but not identical.  
 
    >[!TIP]
    >
    >  Workfront looks for matches only in the Name fields of tasks, projects, and portfolios and not in any other fields. 

* An assignment could get a higher score when they are assigned to a lot of tasks in the system that have similar names. For example, if a team called "Development" is assigned to 50% of the tasks in the system containing "AI" in the name and you are now assigning another task with "AI" in the name, the score of the "Development" team is higher. In this case, the names of  projects and portfolios are not as important.  

* Taking into account this scoring system, the first 7 suggestions are listed as smart assignments, in the descending order of their scores. Assignments with scores lower than 40% do not display.  

* If several assignments have identical scores, they display in order of the date on which the assignments were made, starting from the most recent date.  

  For example, if Rick was assigned to a similar task earlier today and Jennifer was assigned to a similar task two days ago, Rick displays first.  

* Assignments identified in this phase are listed in the    **Suggested assignments**  section of the Assignments field for tasks. 

* If there are no matches using this calculation, the second phase of smart assignments starts which is calculated using a different algorithm.  

</div>

#### Second phase of smart assignment calculation for tasks-->

<!--If the first step of task smart assignments has found no matches,-->

Workfront은 문제에 대한 스마트 할당을 계산하는 것과 동일한 방식으로 작업에 대한 스마트 할당을 계산합니다.

<!--For more information, see the section [Smart assignments criteria for tasks and issues](#smart-assignments-criteria-for-tasks-and-issues) in this article. -->

식별된 할당은 할당 필드의 **사용자 및 팀**, **작업 역할 할당** 및 <span class="preview">**등급 카드 역할**</span> 섹션에 나열됩니다. <span class="preview">등급 카드에 대한 자세한 내용은 [등급 카드 관리](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/manage-rate-cards.md)</span>를 참조하십시오. <!--keep the rate cards roles in yellow after the release of assignments to Prod-->

<!--
### Smart assignments criteria for tasks and issues 

>[!NOTE]
>
>The following criteria applies for tasks only when the first phase of the task smart assignment calculation did not find any matches. For information, see the section [First phase of smart assignment calculation for tasks](#first-phase-of-smart-assignment-calculation-for-tasks) in this article. The following criteria always applies for issues, by default. -->

![](assets/smart-assignments-issue-header.png)

다음 기준의 조합(가장 중요한 것에서 가장 중요하지 않은 것의 순서로 나열됨)을 기반으로 스마트 할당 드롭다운 목록에서 사용자를 권장합니다.

1. 할당한 사용자가 지난 30일 동안 다른 작업 항목에 할당한 사용자입니다. 이 기준과 일치하는 처음 50명의 사용자가 표시됩니다. 가장 자주 할당되는 사용자가 먼저 표시됩니다.

2. 작업 항목이 팀이나 역할에 할당된 경우 아래의 기존 할당을 고려하여 제안된 사용자 목록을 추가로 필터링합니다. 이 경우 제안 목록에 다음 사용자만 표시됩니다.

   * 홈 팀이 작업 항목에 할당된 팀인 사용자.
   * 기본 역할이 작업 항목에 할당된 역할인 사용자.

>[!TIP]
>
>* 작업 또는 문제에 할당된 역할 또는 팀이 없는 경우 Workfront에 지난 30일 동안 할당된 모든 사용자(최대 50명)가 표시됩니다.
>
>* 지난 30일 동안 할당하지 않은 경우 할당된 팀에 속하거나 작업 항목에 할당된 역할이 있는 사용자만 스마트 할당 목록에 표시됩니다.



<!--the commented out piece in the tip above was live before but I am not totally sure that smart assignments look at your team. I think they look JUST at the team/ role assigned to the work item; see this help site request for more info: https://experience.adobe.com/#/@adobeinternalworkfront/so:hub-Hub/workfront/issue/62fd222200037eb87572c5b6ad6bf53e/overview -->
<!--
<div data-mc-conditions="QuicksilverOrClassic.Draft mode">
<div>
<h3>Smart assignments criteria for the Production environment</h3>
<p>(NOTE: drafted,this was the case BEFORE we updated the logic in the WB - with the 21.4 release)</p>
</div>
<p>Smart assignments display on tasks and issues when the following conditions are met:</p>
<ul>
<li>The task or issue is subordinate to a parent task or issue that has a user, team, or job role currently assigned. </li>
</ul>
<p>Smart assignments display the top twenty recommendations based on a proprietary algorithm that uses your own team information.</p>
<p>Users are recommended in the smart assignments drop-down list based on a combination of the following criteria (listed in order from most important to least important):</p>
<ul>
<li>The user has the team assigned to the task or issue designated as their Home Team</li>
<li>The user is also assigned to the parent task</li>
<li>The user has the same primary job role as is currently assigned to the task or issue</li>
<li>The user has the team assigned to the parent task or issue designated as their Home Team</li>
<li>The user is associated with the same primary job role currently assigned to the parent task</li>
<li>The user is a member of the same team as the user who assigned the task or issue and the team is designated as their Home Team</li>
<li>The user is a member of the same Home Group as the user who is assigning the task or issue</li>
<li>The user has the same primary job role as the user who is assigning the task or issue.</li>
</ul>
</div>
-->

<!--
<div data-mc-conditions="QuicksilverOrClassic.Draft mode">
<h2>Make smart assignments</h2>
<p>(NOTE:&nbsp;this was moved to its own article: make-smart-assignments.) </p>
<p>Smart assignments are available in most locations where you can make assignments in Workfront.</p>
<p>You can use smart assignments on tasks and issues that have previously been assigned to a job role or a team.</p> <note type="note">
You must have a Plan or a Work license and have at least Contribute permissions to a task or an issue to be able to make assignments to the task or the issue. You must have the Make Assignments option enabled in your permission level to make assignments.
</note>
<p>To use smart assignments:</p>
<ol>
<li value="1">Navigate to an issue or a task and click one of the following fields to edit them: <br>
<ul>
<li><p data-mc-conditions="QuicksilverOrClassic.Quicksilver">The <strong>Assignments</strong> field in the task or issue header</p></li>
<li>The <strong>Assignments</strong> field of a task or issue list using in-line editing in a task or issue list. </li>
<li>The <strong>Assignee</strong> field after you have clicked <strong>Advanced</strong> from a task or an issue. </li>
</ul></li>
<li value="2"> <p>Place your cursor in the assignment field, and wait for two seconds, then the <strong>Suggestions</strong> list is displayed.</p> <p>Users displayed in this list are the smart assignment suggestions for the task or the issue.<br></p> <p> <img src="assets/nwe-smart-assignment-suggestions-350x160.png" style="width: 350;height: 160;" data-mc-conditions="QuicksilverOrClassic.Quicksilver"> </p> </li>
<li value="3"> <p>Select the user in the recommendations list by clicking their name. </p> <p>If there are no suggestions, the suggestion list does not open.</p> </li>
<li value="4">(Optional) If you do not want to use one of the recommended users from the smart assignments list, start typing the name of the desired user and select the name when it appears in the list.</li>
<li value="5">Click <strong>Enter</strong> to make the assignment. </li>
</ol>
</div>
-->
