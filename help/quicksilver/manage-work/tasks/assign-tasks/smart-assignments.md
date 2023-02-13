---
content-type: overview;how-to-procedural
product-area: projects;user-management
navigation-topic: assign-tasks
title: 스마트 할당 개요
description: 작업 및 문제 지정을 관리할 때 스마트 지정을 사용하여 작업을 완료하는 데 가장 적합한 사용자를 식별할 수 있습니다. 스마트 할당은 작업에 가장 적합한 리소스를 결정하는 알고리즘을 기반으로 리소스에 작업 항목을 할당할 때 Adobe Workfront이 제공하는 제안 사항입니다.
author: Alina
feature: Work Management
exl-id: 8d17eff6-5ff0-4985-b575-4934a3bb7c0b
source-git-commit: 7e220e496aff2675910416bd86e3ddf7b9231afa
workflow-type: tm+mt
source-wordcount: '526'
ht-degree: 0%

---

# 스마트 할당 개요

작업 및 문제 지정을 관리할 때 스마트 지정을 사용하여 작업을 완료하는 데 가장 적합한 사용자를 식별할 수 있습니다. 스마트 할당은 작업에 가장 적합한 리소스를 결정하는 알고리즘을 기반으로 리소스에 작업 항목을 할당할 때 Adobe Workfront이 제공하는 제안 사항입니다.

>[!NOTE]
>
>스마트 할당에서는 사용자의 가용성을 고려하지 않습니다. 하지만 스케줄에 따른 가용성은 작업 및 작업이 지정되는 경우 계획된 일자와 예상 일자에 영향을 줍니다. 일정에 대한 자세한 내용은 문서를 참조하십시오 [예약 만들기](../../../administration-and-setup/set-up-workfront/configure-timesheets-schedules/create-schedules.md).

이 문서에는 스마트 할당에 대한 일반적인 정보가 포함되어 있습니다. 스마트 할당을 사용하여 사용자에게 작업 및 문제를 할당하는 방법에 대한 내용은 [스마트 할당 만들기](../../../manage-work/tasks/assign-tasks/make-smart-assignments.md).

## 스마트 할당 개요

스마트 지정을 사용할 때 다음 사항을 고려하십시오.

* 알고리즘은 작업 및 문제에 대해 독립적으로 작동합니다. 즉, Workfront은 문제 및 작업과 관련된 기준에 따라 목록을 빌드하므로 문제에 대해 제안된 사용자 목록이 작업에 대해 제안된 사용자 목록과 다를 수 있습니다.
* 스마트 할당에서는 작업 역할이나 팀을 권장하지 않습니다. 대신 작업이나 문제를 완료하는 데 가장 적합한 사용자를 제안합니다.
* 제안된 지정은 항상 활성 사용자입니다.
* 먼저 나열된 사용자가 작업에 가장 잘 일치해야 합니다.

## 스마트 할당 제안 찾기

작업 또는 문제를 지정할 수 있는 다음 영역에서 스마트 지정을 볼 수 있습니다.

* 작업 또는 문제 목록 또는 보고서

   ![](assets/smart-assignments-task-list-nwe-350x280.png)

* 작업 또는 문제 헤더

   ![](assets/smart-assignments-task-header-nwe-350x302.png)

* 작업 또는 문제 요약 패널

   ![](assets/smart-assignments-summary-panel-nwe-350x332.png)

* 홈 영역에 나열된 항목에 대한 지정 필드

   ![](assets/smart-assignments-in-home-nwe-350x216.png)


<!--removed for scheduling deprecation: 

* Resource Scheduling

  ![](assets/smart-assignments-scheduling-350x219.png)

  >[!CAUTION]
  >
  >Resource Scheduling is a deprecated feature. For more information, see [Deprecation of Resource Scheduling tools in Adobe Workfront](../../../resource-mgmt/resource-mgmt-overview/deprecate-resource-scheduling.md).

-->
* 워크로드 밸런서

   ![](assets/smart-assignments-workload-balancer-bulk-assignments.png)


## 스마트 할당 기준

스마트 할당에는 소유 알고리즘을 기반으로 상위 50개 권장 사항이 표시됩니다.

사용자는 다음 기준의 조합을 기준으로 스마트 할당 드롭다운 목록에서 권장됩니다(가장 중요한 목록에서 가장 덜 중요한 순서로 나열됨).

* 사용자가 할당을 수행하여 지난 30일 동안 다른 작업 항목에 할당된 사용자입니다. 이 기준과 일치하는 처음 50명의 사용자가 표시됩니다. 가장 많이 할당된 사용자가 먼저 표시됩니다.

   작업 항목이 팀이나 역할에 할당되면 제안된 사용자 목록이 아래의 기존 지정을 고려하여 추가로 필터링됩니다. 이 경우 다음 사용자만 제안 목록에 표시됩니다.

   * 홈 팀이 작업 항목에 할당된 사용자입니다.
   * 기본 역할이 작업 항목에 지정된 역할을 가진 사용자.

      >[!TIP]
      >
      >* If <!--you're not part of any team and --> 작업이나 문제에 지정된 역할이나 팀이 없습니다. Workfront에는 지난 30일 동안 지정된 모든 사용자를 최대 50명의 사용자가 표시됩니다.
      >* 지난 30일 동안 배정을 하지 않은 경우 지정된 팀에 속하거나 작업 항목에 할당된 역할이 있는 사용자만 스마트 할당 목록에 표시됩니다.


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
