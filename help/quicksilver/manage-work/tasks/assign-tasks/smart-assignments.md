---
content-type: overview;how-to-procedural
product-area: projects;user-management
navigation-topic: assign-tasks
title: 스마트 할당 개요
description: 작업 및 문제 할당을 관리할 때 스마트 할당을 사용하여 작업을 완료하는 데 가장 적합한 사용자를 식별할 수 있습니다. 스마트 할당은 작업에 가장 적합한 리소스를 결정하는 알고리즘을 기반으로 리소스에 작업 항목을 할당할 때 Adobe Workfront이 제공하는 제안입니다.
author: Alina
feature: Work Management
exl-id: 8d17eff6-5ff0-4985-b575-4934a3bb7c0b
source-git-commit: 412645a802bdf9057bb61a5a96df257daa1c3948
workflow-type: tm+mt
source-wordcount: '1255'
ht-degree: 0%

---

# 스마트 할당 개요

<!--Audited: 07/2024-->

<!--keep the yellow around the Rate card job roles and the Preview intro for those-->

<span class="preview">이 페이지에서 강조 표시된 정보는 빠른 릴리스를 사용하도록 설정한 고객의 프로덕션 환경에서만 사용할 수 있는 기능을 참조합니다.</span>

<span class="preview">빠른 릴리스에 대한 자세한 내용은 [조직의 빠른 릴리스 사용 또는 사용 안 함](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/enable-fast-release-process.md).</span>을 참조하세요.

<span class="preview"> 이 기능은 2025년 1월에 25.1 릴리스로 빠른 릴리스를 활성화한 고객의 프로덕션 환경에서 제거됩니다. 25.1 릴리스에 대한 자세한 내용은 [2025년 1분기 릴리스 개요](/help/quicksilver/product-announcements/product-releases/25-q1-release-activity/25-q1-release-overview.md)를 참조하십시오.

작업 및 문제 할당을 관리할 때 스마트 할당을 사용하여 작업을 완료하는 데 가장 적합한 리소스를 식별할 수 있습니다. 스마트 할당은 작업에 가장 적합한 리소스를 결정하는 알고리즘을 기반으로 리소스에 작업 항목을 할당할 때 Adobe Workfront이 제공하는 제안입니다. 스마트 할당은 사용자, 작업 역할 또는 팀이 될 수 있습니다.

>[!NOTE]
>
>사용자를 제안할 때 스마트 할당은 사용자의 가용성을 고려하지 않습니다. 하지만 일정에 따른 가용성은 작업 및 문제의 계획 및 예상 일자에 영향을 미칩니다. 일정에 대한 자세한 내용은 문서 [일정 만들기](../../../administration-and-setup/set-up-workfront/configure-timesheets-schedules/create-schedules.md)를 참조하십시오.

이 문서에는 스마트 할당에 대한 일반 정보가 포함되어 있습니다. 스마트 할당을 사용하여 사용자에게 작업 및 문제를 할당하는 방법에 대한 자세한 내용은 [스마트 할당 만들기](../../../manage-work/tasks/assign-tasks/make-smart-assignments.md)를 참조하십시오.

## 스마트 할당 개요

스마트 할당으로 작업할 때 다음 사항을 고려하십시오.

* <span class="preview">알고리즘이 작업 및 문제에 대해 독립적으로 작동합니다. 즉, Workfront은 문제 및 작업과 관련된 기준에 따라 목록을 빌드하므로 문제에 대한 제안 사용자 목록은 작업에 대한 제안 사용자 목록과 다를 수 있습니다. </span>
<!--not sure this is accurate: * Smart assignments do not recommend job roles or teams. Instead, they are suggestions of users who are best fit to complete a task or an issue. -->
* 제안된 할당은 항상 활성 사용자, 작업 역할 또는 팀입니다.
* 먼저 나열된 리소스는 작업에 가장 적합한 리소스여야 합니다.

## 스마트 할당 제안 찾기

다음 영역에서 작업 또는 문제를 할당할 수 있는 스마트 할당을 볼 수 있습니다.

* 할당 열의 문제 목록 또는 보고서

  ![](assets/smart-assignments-issue-list.png)

* <span class="preview">할당 열의 작업 목록 또는 보고서</span>

  ![](assets/smart-assignments-task-list.png)

* <span class="preview">할당 필드의 작업 헤더</span>

  ![](assets/smart-assignments-task-header-nwe-350x302.png)

* 할당 필드의 문제 헤더

  ![](assets/smart-assignments-issue-header.png)

* 할당 영역의 작업 또는 문제 요약 패널

  ![](assets/issue-assignments-summary-panel.png)

* <span class="preview">프로젝트에 작업을 추가할 때 새 작업 상자의 할당 필드</span>

  ![](assets/smart-assignments-new-task-modal.png)

<!--this is not possible in the new home  - we have Summary there: 
* The Assignments field for an item listed in the Home area, when you open a task or issue

  ![](assets/smart-assignments-in-home-nwe-350x216.png)
-->

* <span class="preview">작업 또는 문제를 할당할 때 할당된 대상 영역의 업무 균형자</span>

  ![](assets/smart-assignments-workload-balancer-bulk-assignments.png)


## 스마트 할당 기준

스마트 할당은 작업에 대해 문제와 다르게 작동합니다.

### 작업에 대한 스마트 할당 기준

작업 스마트 할당 계산은 <span class="preview">두 개의 다른 알고리즘을 사용하는 두 단계에서 작동합니다.</span>

<span class="preview">스마트 할당을 찾는 알고리즘에 따라 할당은 [할당] 필드의 두 개의 별도 섹션 아래에 나열됩니다.</span> 자세한 내용은 [스마트 할당 만들기](/help/quicksilver/manage-work/tasks/assign-tasks/make-smart-assignments.md)를 참조하십시오.

![](assets/smart-assignments-task-list.png)

<div class="preview">

#### 작업에 대한 스마트 할당 계산의 첫 번째 단계

스마트 할당 계산의 첫 번째 단계에서 Workfront은 모든 할당에 대한 유사성 점수를 계산합니다.

>[!NOTE]
>
>스마트 할당 계산의 첫 번째 단계는 다음 작업 영역에 적용되지 않습니다.
>
>* 업무 균형자에서 일괄 할당.
>* 보드에 연결된 카드.


유사성 점수와 할당이 나열된 순서에 대한 계산은 다음을 고려합니다.

* 작업, 프로젝트 및 포트폴리오 이름이 할당하려는 작업과 동일한 기존 할당에 100%의 점수가 제공됩니다. 기존 할당 작업의 프로젝트 및 포트폴리오 이름도 할당하려는 작업의 프로젝트 및 포트폴리오와 일치해야 합니다.

* 다른 할당의 이 정보 중 일부만 기존 작업과 일치하는 경우 점수가 100%보다 낮을 수 있습니다.

  예를 들어, &quot;내 포트폴리오&quot;라는 포트폴리오의 &quot;내 프로젝트&quot;라는 프로젝트에 &quot;내 두 번째 작업&quot;이라는 작업을 할당하고 &quot;내 포트폴리오&quot;라는 포트폴리오의 &quot;내 프로젝트&quot;라는 다른 프로젝트에 &quot;내 작업&quot;이라는 기존 작업이 있는 경우 기존 작업과 지금 할당하려는 작업의 이름은 유사하지만 동일하지 않으므로 &quot;내 작업&quot;에 할당된 사용자가 95%의 점수를 받을 수 있습니다.

  >[!TIP]
  >
  >  Workfront은 작업, 프로젝트 및 포트폴리오의 이름 필드에서만 일치 항목을 찾고 다른 필드에서는 찾지 않습니다.

* 이름이 비슷한 시스템에서 많은 작업에 할당되었을 때 할당은 더 높은 점수를 받을 수 있습니다. 예를 들어 &#39;개발&#39;이라는 팀이 이름에 &#39;AI&#39;가 포함된 시스템 내 작업의 50%에 할당되고 이제 이름에 &#39;AI&#39;가 포함된 다른 작업을 할당하는 경우 &#39;개발&#39; 팀의 점수가 더 높아집니다. 이 경우 프로젝트 이름과 포트폴리오는 중요하지 않습니다.

* 이러한 채점 체계를 고려하여 처음 7개의 제안이 점수의 내림차순으로 스마트 과제로 나열되어 있다. 점수가 40%보다 낮은 할당은 표시되지 않습니다.

* 점수가 동일한 할당이 여러 개 있는 경우 가장 최근 날짜부터 할당한 날짜 순서대로 표시됩니다.

  예를 들어 릭이 오늘 일찍 유사한 작업에 할당되었고 제니퍼가 이틀 전에 유사한 작업에 할당되었다면 릭이 먼저 표시됩니다.

* 이 단계에서 식별된 할당은    작업에 대한 할당 필드의 **제안된 할당** 섹션.

* 이 계산을 사용하여 일치하는 항목이 없으면 스마트 할당의 두 번째 단계가 시작되고 다른 알고리즘을 사용하여 계산됩니다.

</div>

#### 작업에 대한 스마트 할당 계산의 두 번째 단계

작업 스마트 할당의 첫 번째 단계에서 일치하는 항목을 찾지 못한 경우 Workfront은 문제에 대한 스마트 할당을 계산하는 것과 동일한 방식으로 작업에 대한 스마트 할당을 계산합니다.

자세한 내용은 이 문서의 [작업 및 문제에 대한 스마트 할당 기준](#smart-assignments-criteria-for-tasks-and-issues) 섹션을 참조하십시오.

이 단계에서 식별된 할당은 할당 필드의 **사용자 및 팀**, **작업 역할 할당** 및 <span class="preview">**등급 카드 역할**</span> 섹션에 나열됩니다. <span class="preview">등급 카드에 대한 자세한 내용은 [등급 카드 관리](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/manage-rate-cards.md)</span>를 참조하십시오. <!--keep the rate cards roles in yellow after the release of assignments to Prod-->

### 작업 및 문제에 대한 스마트 할당 기준


>[!NOTE]
>
>다음 기준은 작업 스마트 할당 계산의 첫 번째 단계에서 일치하는 항목을 찾지 못한 경우에만 작업에 적용됩니다. 자세한 내용은 이 문서에서 [작업에 대한 스마트 할당 계산의 첫 번째 단계](#first-phase-of-smart-assignment-calculation-for-tasks) 섹션을 참조하십시오. 기본적으로 다음 기준은 항상 문제에 적용됩니다.

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
