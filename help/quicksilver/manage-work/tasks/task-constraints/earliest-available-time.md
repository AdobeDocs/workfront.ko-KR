---
content-type: reference;how-to-procedural
product-area: projects
navigation-topic: task-constraints
title: '작업 제한 개요: 가장 빠른 사용 시간'
description: 가장 빠른 사용 가능 시간은 선행 관계를 고려하여 가능한 가장 이른 시간에 작업이 시작되도록 예약하는 작업 제한입니다.
author: Alina
feature: Work Management
exl-id: 9c01e4bd-c6ca-4540-a0f1-ecdd44df84e0
source-git-commit: f2f825280204b56d2dc85efc7a315a4377e551c7
workflow-type: tm+mt
source-wordcount: '299'
ht-degree: 0%

---

# 작업 제한 개요: 가장 이른 가용 시간

가장 빠른 사용 가능 시간은 선행 관계를 고려하여 가능한 가장 이른 시간에 작업이 시작되도록 예약하는 작업 제한입니다.

작업에 대한 작업 제약 조건을 업데이트하는 방법에 대한 자세한 내용은 [작업의 작업 제약 조건 업데이트](../../../manage-work/tasks/task-constraints/update-task-constraint-of-task.md).

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: replaced with new article linked above) </p>
-->

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">To update the Task Constraint to Earliest Available Time:</p>
-->

<!--
   <li value="1" data-mc-conditions="QuicksilverOrClassic.Draft mode">Go to a task whose constraint you want to modify. </li>
   -->

<!--
   <p data-mc-conditions="QuicksilverOrClassic.Draft mode">Click <strong>Edit Task</strong>.</p>
   -->

<!--
   <p data-mc-conditions="QuicksilverOrClassic.Draft mode">Click the <strong>More</strong> icon <img src="assets/qs-more-icon-on-an-object.png"> next to the task name, then click <strong>Edit</strong>.</p>
   -->

<!--
   <p data-mc-conditions="QuicksilverOrClassic.Draft mode">In the <strong>Overview</strong> section, expand the <strong>Task Constraint</strong> drop-down menu.</p>
   -->

<!--
   <p data-mc-conditions="QuicksilverOrClassic.Draft mode">Select <strong>Earliest Available Time</strong>.</p>
   -->

<!--
   <li value="5" data-mc-conditions="QuicksilverOrClassic.Draft mode">Click <strong>Save Changes</strong>.</li>
   -->

## 가능한 한 빨리 가능한 가장 빠른 시간 및 간격

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: [! This section is duplicated in "Earliest Available Time"])</p>
-->

사용 가능한 가장 이른 시간 제약 조건은 다음 기준이 모두 있을 때 가능한 한 빨리 제한과 다릅니다.

* 프로젝트가 완료 후 예약되었습니다.
* 프로젝트의 작업은 이전 관계가 있습니다
* 이전 작업의 작업 제약 조건이 유연합니다.

이 경우:

* **사용 가능한 가장 이른 시간:** 후속 작업에 대해 사용 가능한 가장 이른 시간 제약 조건을 사용하면 선행 작업의 유연한 제약 조건에 우선 순위가 지정됩니다.

   **예:** 작업 A는 작업 B의 전임자입니다. 작업 B는 사용 가능한 가장 이른 시간 제약 조건을 가지고 있으며 작업 A는 가능한 한 늦습니다. 이 경우 작업 B는 최대한 프로젝트 완료에 가깝게 예약됩니다.

   ![작업에 프로젝트의 완료 날짜에 가까운 날짜가 있는 경우 사용 가능한 가장 빠른 시간 제한](assets/earliest-available-constraint-dates-closer-to-project-completion-350x137.png)

* **가능한 한 빨리:** 이 시나리오에서는 후속 작업에 대해 가능한 한 빨리 제약 조건을 사용하여 후속 작업에 우선 순위를 제공합니다.

   **예:**  작업 A는 작업 B의 전임자입니다. 작업 B는 가능한 한 빨리 제한되고 작업 A는 가능한 한 늦습니다. 이 경우 작업 B가 최대한 프로젝트 시작에 가깝게 예약됩니다.

   ![작업이 프로젝트의 시작 날짜에 가까운 날짜가 있는 경우 가능한 한 빨리 제한](assets/as-soon-as-possible-dates-closer-to-project-start-350x126.png)
