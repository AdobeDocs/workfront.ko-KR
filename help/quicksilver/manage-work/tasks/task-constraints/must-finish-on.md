---
content-type: reference;how-to-procedural
product-area: projects
navigation-topic: task-constraints
title: '''작업 제한 개요: '' 작업을 완료해야 함'
description: MFO(Must Finish On) 작업 제약 조건을 사용하여 특정 날짜에 작업을 종료하도록 예약할 수 있습니다.
author: Alina
feature: Work Management
exl-id: 9e546a0f-7f7a-4f1c-9d9d-aa3cea377fdf
source-git-commit: f2f825280204b56d2dc85efc7a315a4377e551c7
workflow-type: tm+mt
source-wordcount: '395'
ht-degree: 0%

---

# 작업 제한 개요: 다음 작업을 완료해야 함

MFO(Must Finish On) 작업 제약 조건을 사용하여 특정 날짜에 작업을 종료하도록 예약할 수 있습니다.

Must Finish On 제약 조건에서는 Target에서 지정한 시간 및 날짜에 작업을 정확히 완료하도록 예약합니다. **계획 완료 일자** 필드.

>[!TIP]
>
>작업의 계획 완료 날짜를 수동으로 업데이트하면 작업 제한이 반드시 완료 상태로 변경됩니다.

## 작업 제약 조건에 대한 완료 필수 개요

제약 조건이 있는 작업을 예약할 때 다음을 고려하십시오.

* 전임자 관계는 작업 일정을 조정하도록 강요하지 않습니다. Adobe Workfront은 기본적으로 이전 관계를 무시합니다.
* 작업이 다음과 같이 표시됩니다. **위험** 과거 정권들이 뒤쫓기 시작했거나 늦게 온다면.

* MFO 제약 조건이 있는 작업을 다른 프로젝트에 이동하거나 복사하면 제한 날짜가 무엇이고 프로젝트의 시작 날짜와 완료 날짜가 무엇인지에 따라 작업 또는 프로젝트 날짜가 달라질 수 있습니다. 다음 시나리오가 있습니다.

   * 대상 프로젝트를 시작 날짜부터 예약하면:

      * 작업의 제한 날짜가 프로젝트 계획 시작 날짜보다 이전이면 작업 제약 조건이 가능한 한 빨리 로 변경됩니다.
      * 태스크의 제약 일자가 프로젝트 계획 완료 일자보다 늦으면 프로젝트 계획 완료 일자가 태스크의 완료 제한 일자와 일치하도록 변경됩니다.

      * 대상 프로젝트가 완료 후 예약되는 경우:

         * 작업의 제한 날짜가 프로젝트 완료 날짜보다 늦으면 작업 제약 조건이 가능한 한 늦음으로 변경됩니다.
         * 태스크의 제약 일자가 프로젝트의 계획 시작 일자보다 이전인 경우 프로젝트의 계획 시작 일자가 태스크의 시작 제한 일자와 일치하도록 변경됩니다.
      * 프로젝트 일정에 관계없이 작업의 제한 날짜가 프로젝트의 시작 및 완료 날짜 내에 있으면 작업 제한이나 프로젝트 날짜에 대한 변경 사항이 없습니다.

   작업 이동에 대한 자세한 내용은 [작업 이동](../../../manage-work/tasks/manage-tasks/move-tasks.md). 작업 복사에 대한 자세한 내용은 [작업 복사 및 복제](../../../manage-work/tasks/manage-tasks/copy-and-duplicate-tasks.md).

작업에 대한 작업 제약 조건을 업데이트하는 방법에 대한 자세한 내용은 [작업의 작업 제약 조건 업데이트](../../../manage-work/tasks/task-constraints/update-task-constraint-of-task.md).

<!--
<div data-mc-conditions="QuicksilverOrClassic.Draft mode">
<h2>Use the Must Finish On Task Constraint</h2>
<p>To update the Task Constraint to Must Finish On:</p>
<ol>
<li value="1">Go to a task whose Task Constraint you want to update.</li>
<li value="2"> <p data-mc-conditions="QuicksilverOrClassic.Quicksilver">Click the <strong>More</strong> icon <img src="assets/qs-more-icon-on-an-object.png"> next to the task name, then click <strong>Edit</strong>.</p> </li>
<li value="3">In the <strong>Overview</strong> section, expand the <strong>Task Constraint</strong> drop-down menu.</li>
<li value="4"> <p>Select <strong>Must Finish On</strong>.</p> </li>
<li value="5"> <p>Specify a <strong>Planned Completion Date</strong>.</p> <p>The task must complete by this date, and no later than this date. </p> </li>
<li value="6">Click <strong>Save Changes</strong>. </li>
</ol>
</div>
-->
