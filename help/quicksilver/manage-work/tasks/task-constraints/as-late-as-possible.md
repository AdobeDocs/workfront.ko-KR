---
content-type: reference;how-to-procedural
product-area: projects
navigation-topic: task-constraints
title: '작업 제한 개요: 가능한 한 늦다'
description: ALAP(Late As Fluid As Possible)는 작업이 완료되는 시간을 가능한 한 프로젝트 끝에 가깝게 설정하는 Adobe Workfront 작업 제한입니다.
author: Alina
feature: Work Management
exl-id: 475427d0-020b-4851-a614-c9931659e07d
source-git-commit: f2f825280204b56d2dc85efc7a315a4377e551c7
workflow-type: tm+mt
source-wordcount: '368'
ht-degree: 0%

---

# 작업 제한 개요: 가능한 늦게

ALAP(Late As Fluid As Possible)는 작업이 완료되는 시간을 가능한 한 프로젝트 끝에 가깝게 설정하는 Adobe Workfront 작업 제한입니다.

이 제약 조건을 사용하면 선행 작업 또는 종속 작업의 일정이 조정될 수 있습니다.

이전 관계에 대한 자세한 내용은 [작업 선행 작업 사용](../../../manage-work/tasks/use-prdcssrs/use-task-predecessors.md).

프로젝트가 완료 날짜로부터 스케줄 모드의 스케줄 모드를 사용하고 작업의 시작 날짜에 대한 시스템 또는 그룹 기본값을 프로젝트 계획 날짜에 따라 사용하는 경우 가능한 지연 이 기본 제한입니다.

새 작업에 대한 기본 제약 조건을 설정할 위치에 대한 자세한 내용은 [시스템 전체 작업 및 문제 환경 설정 구성](../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-task-issue-preferences.md).

작업에 대한 작업 제약 조건을 업데이트하는 방법에 대한 자세한 내용은 [작업의 작업 제약 조건 업데이트](../../../manage-work/tasks/task-constraints/update-task-constraint-of-task.md).

<!--
<div data-mc-conditions="QuicksilverOrClassic.Draft mode">
<h2>Use the As Late As Possible Task Constraint</h2>
<p>(NOTE: replaced with new article linked above) </p>
<p>To update the Task Constraint to As Late As Possible:&nbsp;</p>
<ol>
<li value="1">Go to a task whose Task Constraint you want to update.</li>
<li value="2"> <p data-mc-conditions="QuicksilverOrClassic.Quicksilver">Click the <strong>More</strong> icon <img src="assets/qs-more-icon-on-an-object.png"> next to the task name, then click&nbsp;<strong>Edit</strong>.</p> </li>
<li value="3"> <p>In the&nbsp;<strong>Overview</strong>&nbsp;section, expand the&nbsp;<strong>Task Constraint</strong>&nbsp;drop-down menu.</p> </li>
<li value="4"> <p>Select&nbsp;<strong>As Late As Possible</strong>.</p> </li>
<li value="5">Click <strong>Save Changes</strong>.&nbsp;</li>
</ol>
</div>
-->

## 가능한 최신 사용 가능 시간과 지연 시간 간의 차이점

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE:&nbsp;[! This section is duplicated in "Latest Available Time"] - inserted a snippet for both articles (Alina)) </p>
-->

다음 기준이 있는 경우 사용 가능한 최신 시간 제약 조건은 가능한 한 늦게까지 제한과 다릅니다.

* 프로젝트가 시작 날짜부터 예약되었습니다.
* 프로젝트의 작업은 이전 관계가 있습니다
* 후속 작업에 유연한 작업 제약 조건이 있습니다

이 경우:

* **최신 사용 시간:** 이전 작업에 대해 사용 가능한 최신 시간 제약 조건을 사용하면 후임자의 유연한 제약 조건이 우선합니다.

   **예:** 예를 들어, 작업 A는 작업 B의 전임자입니다. 작업 A에는 사용 가능한 최신 시간 제한이 있고 작업 B에는 가능한 한 빨리 제약 조건이 있습니다. 이 경우 작업 A는 가능한 한 프로젝트 시작에 가깝게 예약됩니다.

   ![](assets/latest-available-time-task-constraint-in-task-list-350x116.png)

* **가능한 늦게:** 이 시나리오에서는 선행 작업에 대해 가능한 한 늦게까지 제약 조건을 사용하면 선행 작업에 우선 순위가 지정됩니다.

   **예:** 예를 들어, 작업 A는 작업 B의 전임자입니다. 작업 A는 가능한 한 늦으며 작업 B는 가능한 한 빨리 제약 조건을 가집니다. 이 경우 작업 A는 최대한 프로젝트 끝에 가깝게 예약됩니다.

   ![](assets/as-late-as-possible-task-constraint-in-task-list-350x104.png)

 

<!--
<div data-mc-conditions="QuicksilverOrClassic.Draft mode">
<p>(NOTE: this content was here before but it was wrong - according to this issue in Hub, per Dev, the correct functionality is in the snippet above: https://hub.workfront.com/task/6193c6910004bce9de07cda7757f3ce8/updates?email-source=subscribedCommunication) </p>
<p>The Latest&nbsp;Available Time constraint differs from the As Late&nbsp;As Possible constraint when the following criteria exist:</p>
<ul>
<li> The project is scheduled From Completion </li>
<li> Tasks in the project have a predecessor relationship </li>
<li> The predecessor task has a flexible task constraint </li>
</ul>
<p> In this situation: </p>
<ul>
<li> <p><strong>Latest Available Time:</strong> Using the Latest&nbsp;Available Time constraint on the successor task gives priority to flexible constraint of the predecessor.</p> <p>For example, Task A is a predecessor to Task B. Task B has the Latest&nbsp;Available Time constraint and Task A has the As Soon&nbsp;As Possible constraint. In this situation, the task is scheduled as close&nbsp;to the start&nbsp;of the project as possible.</p> </li>
<li> <p><strong>As Late As Possible:</strong> In this scenario, using the As Late&nbsp;As Possible constraint on the successor task gives the priority to the successor task.</p> <p>For example, Task A is a predecessor to Task B. Task B has the As Late&nbsp;As Possible&nbsp;constraint and Task A has the As Soon&nbsp;As Possible constraint. In this situation, the task is scheduled as close to the end&nbsp;of the project as possible.</p> </li>
</ul>
</div>
-->
