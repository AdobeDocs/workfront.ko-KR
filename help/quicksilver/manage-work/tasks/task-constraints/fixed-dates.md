---
content-type: reference;how-to-procedural
product-area: projects
navigation-topic: task-constraints
title: '작업 제한 개요: 고정 날짜'
description: 작업의 정확한 시작 날짜와 종료 날짜를 알려면 고정 날짜 작업 제한 사항을 사용할 수 있습니다. 작업 제한에 대한 자세한 내용은 작업 제한 개요를 참조하십시오.
author: Alina
feature: Work Management
exl-id: 084f54a6-e757-405c-b388-5d5f61608e71
source-git-commit: 7427706f6ce6cad3370b91269c1b4e7a10ed09f9
workflow-type: tm+mt
source-wordcount: '437'
ht-degree: 0%

---

# 작업 제한 개요: 고정 날짜

작업의 정확한 시작 날짜와 종료 날짜를 알려면 고정 날짜 작업 제한 사항을 사용할 수 있습니다. 작업 제한에 대한 자세한 내용은 [작업 제한 개요](../../../manage-work/tasks/task-constraints/task-constraint-overview.md)를 참조하십시오.

## 고정 날짜 제한 개요

고정 날짜 제약 조건을 사용할 때는 다음 사항을 고려하십시오.

* 고정 일자(FIXT) 작업 제한을 선택할 경우 작업의 계획된 시작 일자와 계획된 완료 일자를 지정해야 합니다. 이 경우 작업의 전임 작업 관계는 무시됩니다.
* FIXT 제약 조건을 사용할 때는 작업의 기간 필드를 편집할 수 없습니다. 기간은 작업의 계획된 시작 일자와 계획된 완료 일자 간의 차이로 계산됩니다.
* 작업의 기간 유형이 작업량 기준인 경우 작업의 할당자 수는 작업 기간에도 영향을 줍니다.
* FIXT 제한 사항이 있는 작업을 다른 프로젝트로 이동하거나 복사하는 경우 제한 일자가 무엇이고 프로젝트의 시작 및 완료 일자가 무엇인지에 따라 작업 제한 사항이나 프로젝트 일자가 변경될 수 있습니다. 다음과 같은 시나리오가 있습니다.

   * 대상 프로젝트가 시작부터 예약된 경우:

      * 작업의 제한 일자가 프로젝트 시작 일자보다 이전인 경우 작업 제한 사항이 가능한 한 빨리 로 변경됩니다.
      * 작업의 제한 일자 중 하나 또는 둘 다가 프로젝트의 계획된 완료 일자보다 늦으면 프로젝트의 계획된 완료 일자가 작업의 완료 제한 일자와 일치하도록 변경됩니다.

   * 대상 프로젝트가 완료부터 예약된 경우:

      * 작업의 제한 일자가 프로젝트 완료 일자보다 늦으면 작업 제한 사항이 가능한 한 늦게 변경됩니다.
      * 작업의 제한 일자 중 하나 또는 둘 다가 프로젝트의 계획된 시작 일자보다 이전인 경우 프로젝트의 계획된 시작 일자가 작업의 시작 제한 일자와 일치하도록 변경됩니다.

   * 프로젝트의 일정에 관계없이 작업의 제한 일자가 프로젝트의 시작 및 완료 일자 내에 있으면 작업 제한 일자 또는 프로젝트 일자에 변경 사항이 없습니다.

  작업 이동에 대한 자세한 내용은 [작업 이동](../../../manage-work/tasks/manage-tasks/move-tasks.md)을 참조하십시오. 작업 복사에 대한 자세한 내용은 [작업 복사 및 복제](../../../manage-work/tasks/manage-tasks/copy-and-duplicate-tasks.md)를 참조하십시오.

작업에 대한 작업 제한을 업데이트하는 방법에 대한 자세한 내용은 [작업의 작업 제한 업데이트](../../../manage-work/tasks/task-constraints/update-task-constraint-of-task.md)를 참조하십시오.

<!--
<div data-mc-conditions="QuicksilverOrClassic.Draft mode">
<h2>Use the Fixed Dates Task Constraint</h2>
<p>(NOTE:&nbsp;replaced with new article linked above) </p>
<p>To update the Task Constraint to Finish No Later Than:</p>
<ol>
<li value="1">Go to a task whose Task Constraint you want to update.</li>
<li value="2"> <p data-mc-conditions="QuicksilverOrClassic.Quicksilver">Click the <strong>More</strong> icon <img src="assets/qs-more-icon-on-an-object.png"> next to the task name, then click <strong>Edit</strong>.</p> </li>
<li value="3">In the <strong>Overview</strong> section, expand the <strong>Task Constraint</strong> drop-down menu.</li>
<li value="4"> <p>Select <strong>Fixed Dates</strong>.</p> </li>
<li value="5"> <p>Specify a <strong>Planned Start Date</strong>.</p> <p>The task must start on this date. </p> </li>
<li value="6"> <p>Specify a <strong>Planned Completion Date</strong>.</p> <p>The task must complete on this date. </p> </li>
<li value="7">Click <strong>Save Changes</strong>.</li>
</ol>
</div>
-->
