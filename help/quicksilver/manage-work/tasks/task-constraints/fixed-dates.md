---
content-type: reference;how-to-procedural
product-area: projects
navigation-topic: task-constraints
title: '작업 제한 개요: 고정 날짜'
description: 작업의 정확한 시작 날짜 및 종료 날짜에 대해 구체화하려는 경우 고정 날짜 작업 제한을 사용할 수 있습니다. 작업 제약 조건에 대한 자세한 내용은 작업 제한 개요를 참조하십시오.
author: Alina
feature: Work Management
exl-id: 084f54a6-e757-405c-b388-5d5f61608e71
source-git-commit: f2f825280204b56d2dc85efc7a315a4377e551c7
workflow-type: tm+mt
source-wordcount: '437'
ht-degree: 0%

---

# 작업 제한 개요: 고정 날짜

작업의 정확한 시작 날짜 및 종료 날짜에 대해 구체화하려는 경우 고정 날짜 작업 제한을 사용할 수 있습니다. 작업 제한에 대한 자세한 내용은 [작업 제한 개요](../../../manage-work/tasks/task-constraints/task-constraint-overview.md).

## 고정 날짜 제한 개요

고정 날짜 제한을 사용할 때는 다음 사항을 고려하십시오.

* 고정 일자(FIXT) 태스크 제약 조건을 선택하는 경우, 태스크의 계획 시작 일자 및 계획 완료 일자를 지정해야 합니다. 이 경우 작업의 이전 관계는 무시됩니다.
* FIXT 제약 조건을 사용할 때는 작업의 기간 필드를 편집할 수 없습니다. 기간은 작업의 계획 시작 일자와 계획 완료 일자 간의 차이로 계산됩니다.
* 작업의 기간 유형이 작업 제어인 경우, 작업의 담당자 수도 작업 기간에 영향을 줍니다.
* FIXT 제약 조건이 있는 작업을 다른 프로젝트에 이동하거나 복사하면 제한 날짜가 무엇이고 프로젝트의 시작 날짜와 완료 날짜가 무엇인지에 따라 작업의 제한이나 프로젝트 날짜가 변경될 수 있습니다. 다음 시나리오가 있습니다.

   * 대상 프로젝트를 시작 날짜부터 예약하면:

      * 작업의 제한 날짜가 프로젝트 시작 날짜보다 이전이면 작업 제약 조건이 가능한 한 빨리 로 변경됩니다.
      * 작업의 제한조건 일자가 프로젝트 계획 완료 일자보다 늦으면 프로젝트 계획 완료 일자가 태스크의 완료 제한조건 일자와 일치하도록 변경됩니다.
   * 대상 프로젝트가 완료 후 예약되는 경우:

      * 작업의 제한 날짜가 프로젝트 완료 날짜보다 늦은 경우 작업 제약 조건이 가능한 한 늦음으로 변경됩니다.
      * 태스크의 제약 일자가 프로젝트 계획 시작 일자보다 이전이면 프로젝트 계획 시작 일자가 태스크의 시작 제한 일자와 일치하도록 변경됩니다.
   * 프로젝트 일정에 관계없이 작업의 제한 날짜가 프로젝트의 시작 및 완료 날짜 내에 있으면 작업 제한이나 프로젝트 날짜에 대한 변경 사항이 없습니다.

   작업 이동에 대한 자세한 내용은 [작업 이동](../../../manage-work/tasks/manage-tasks/move-tasks.md). 작업 복사에 대한 자세한 내용은 [작업 복사 및 복제](../../../manage-work/tasks/manage-tasks/copy-and-duplicate-tasks.md).

작업에 대한 작업 제약 조건을 업데이트하는 방법에 대한 자세한 내용은 [작업의 작업 제약 조건 업데이트](../../../manage-work/tasks/task-constraints/update-task-constraint-of-task.md).

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
