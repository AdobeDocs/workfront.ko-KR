---
content-type: reference;how-to-procedural
product-area: projects
navigation-topic: task-constraints
title: '작업 제한 개요: 사용 가능한 최신 시간'
description: 최근 사용 가능한 시간(LAT)은 Adobe Workfront의 작업 제한 유형입니다.
author: Alina
feature: Work Management
exl-id: acf55004-9424-4e24-9ff5-90f6fd7f72a6
source-git-commit: 7427706f6ce6cad3370b91269c1b4e7a10ed09f9
workflow-type: tm+mt
source-wordcount: '334'
ht-degree: 0%

---

# 작업 제한 개요: 사용 가능한 최신 시간

최근 사용 가능한 시간(LAT)은 Adobe Workfront의 작업 제한 유형입니다.

## 사용 가능한 최신 시간 작업 제한 사용

프로젝트의 전임 작업-후임 작업 관계를 고려한 후 가장 늦은 사용 가능한 시간에 작업을 시작하도록 예약하려는 경우 LAT 제한 사항을 사용할 수 있습니다.

이 제한은 전임 작업 또는 후임 작업의 일정을 강제로 조정하지 않는다는 점에서 가능한 한 빨리 와 다릅니다. 대신 연결된 작업의 일정에만 영향을 주고 다른 작업과의 관계를 기반으로 사용 가능한 최신 시간으로 설정합니다.

작업에 대한 작업 제한을 업데이트하는 방법에 대한 자세한 내용은 [작업의 작업 제한 업데이트](../../../manage-work/tasks/task-constraints/update-task-constraint-of-task.md)를 참조하십시오.

<!--
<div data-mc-conditions="QuicksilverOrClassic.Draft mode">
<p>To update the Task Constraint to Latest Available Time:</p>
<p>(NOTE: replaced with new article linked above) </p>
<ol>
<li value="1">Go to a task whose Task Constraint you want to update.</li>
<li value="2"> <p data-mc-conditions="QuicksilverOrClassic.Quicksilver">Click the <strong>More</strong> icon <img src="assets/qs-more-icon-on-an-object.png"> next to the task name, then click <strong>Edit</strong>.</p> </li>
<li value="3">In the <strong>Overview</strong> section, expand the <strong>Task Constraint</strong> drop-down menu.</li>
<li value="4"> <p>Select <strong>Latest Available Time</strong>.</p> </li>
<li value="5">Click <strong>Save Changes</strong>.</li>
</ol>
</div>
-->

## 최근 사용 가능한 시간과 가능한 한 늦게 사용 가능한 시간의 차이

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: [! This section is duplicated in "As Late As Possible"] - inserted snippet in both (Alina)) </p>
-->

다음 기준이 있는 경우 최근 가용 시간 제약조건이 가능한 한 늦게 제약조건과 다릅니다.

* 프로젝트가 시작 날짜부터 예약됩니다.
* 프로젝트의 작업에 전임 작업 관계가 있습니다.
* 후속 작업의 작업 제한 사항이 유연합니다.

이 경우:

* **최근 사용 가능한 시간:** 전임 작업에 대해 최근 사용 가능한 시간 제한을 사용하면 후임 작업의 유연한 제한에 우선 순위를 둘 수 있습니다.

  **예:** 예를 들어 작업 A는 작업 B의 전임자입니다. 작업 A는 사용 가능한 최신 시간 제약 조건을 가지며 작업 B는 가능한 한 빨리 제한 조건을 갖습니다. 이러한 상황에서 작업 A는 가능한 프로젝트 시작에 가깝게 일정이 잡힌다.

  ![](assets/latest-available-time-task-constraint-in-task-list-350x116.png)

* **가능한 한 늦게:** 이 시나리오에서는 전임 작업에 가능한 한 늦게 제한을 사용하면 전임 작업에 우선 순위가 부여됩니다.

  **예:** 예를 들어 작업 A는 작업 B의 전임자입니다. 작업 A에는 가능한 한 늦게 제한이 있고 작업 B에는 가능한 한 빨리 제한이 있습니다. 이러한 상황에서 작업 A는 가능한 프로젝트 종료에 임박하여 예정되어 있다.

  ![](assets/as-late-as-possible-task-constraint-in-task-list-350x104.png)

<!--
<div data-mc-conditions="QuicksilverOrClassic.Draft mode">
<p>(NOTE: this content was here before but it was wrong - according to this issue in Hub, per Dev, the correct functionality is in the snippet above: https://hub.workfront.com/task/6193c6910004bce9de07cda7757f3ce8/updates?email-source=subscribedCommunication) </p>
<p>The Latest Available Time constraint differs from the As Late As Possible constraint when the following criteria exist:</p>
<ul>
<li> The project is scheduled From Completion </li>
<li> Tasks in the project have a predecessor relationship </li>
<li> The predecessor task has a flexible task constraint </li>
</ul>
<p> In this situation: </p>
<ul>
<li> <p><strong>Latest Available Time:</strong> Using the Latest Available Time constraint on the successor task gives priority to flexible constraint of the predecessor.</p> <p>For example, Task A is a predecessor to Task B. Task B has the Latest Available Time constraint and Task A has the As Soon As Possible constraint. In this situation, Task B is scheduled as close to the start of the project as possible.</p> </li>
<li> <p><strong>As Late As Possible:</strong> In this scenario, using the As Late As Possible constraint on the successor task gives the priority to the successor task.</p> <p>For example, Task A is a predecessor to Task B. Task B has the As Late As Possible constraint and Task A has the As Soon As Possible constraint. In this situation, Task B is scheduled as close to the end of the project as possible.</p> </li>
</ul>
</div>
-->
