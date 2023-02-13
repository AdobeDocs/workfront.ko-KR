---
content-type: reference;how-to-procedural
product-area: projects
navigation-topic: task-constraints
title: '작업 제한 개요: 보다 빨리 완료'
description: FNET(Finish No Early To) 은 지정한 날짜 이후에 작업을 완료하도록 예약하는 작업 제한입니다.
author: Alina
feature: Work Management
exl-id: b1dbf5c9-34b6-4c25-b582-ce9454501e03
source-git-commit: f2f825280204b56d2dc85efc7a315a4377e551c7
workflow-type: tm+mt
source-wordcount: '389'
ht-degree: 0%

---

# 작업 제한 개요: 보다 빨리 완료

FNET(Finish No Early To) 은 지정한 날짜 이후에 작업을 완료하도록 예약하는 작업 제한입니다.

## Finish No Early 제한 개요

작업에 대해 FNET(Finish No Early Than) 제약 조건을 사용할 때는 다음 사항을 고려하십시오.

* 프로젝트가 완료 날짜로부터 예약된 경우 이 제한을 사용해야 합니다. 이 경우 다른 종속 작업에 위험 표시를 강제하기 전에 작업에 소프트 제한을 제공할 수 있습니다.
* 예약된 프로젝트에서 FNET을 사용하는 경우&#x200B;**시작 날짜부터**&#x200B;그런 다음 제약 조건이 가능한 한 빨리 지정되었을 경우 작업 일정을 예약합니다.
* FNET 제약 조건이 있는 작업을 다른 프로젝트에 이동하거나 복사하면 제한 날짜가 무엇이고 프로젝트의 시작 날짜와 완료 날짜가 무엇인지에 따라 작업 또는 프로젝트 날짜가 변경될 수 있습니다. 다음 시나리오가 있습니다.

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
<h2>Use the Finish No Earlier Than constraint</h2>
<p>(NOTE: replaced with new article linked above)&nbsp;</p>
<p>To update the Task Constraint to Finish No Earlier Than:</p>
<ol>
<li value="1">Go to a task whose Task Constraint you want to update.</li>
<li value="2"> <p data-mc-conditions="QuicksilverOrClassic.Quicksilver">Click the <strong>More</strong> icon <img src="assets/qs-more-icon-on-an-object.png"> next to the task name, then click <strong>Edit</strong>.</p> </li>
<li value="3"> <p>In the <strong>Overview</strong> section, expand the <strong>Task Constraint</strong> drop-down menu.</p> </li>
<li value="4"> <p>Select <strong>Finish No Earlier Than</strong>.</p> <p> <img src="assets/fnet-350x267.png" alt="FNET.png" style="width: 350;height: 267;"> </p> </li>
<li value="5"> <p>Specify a <strong>Planned Completion Date</strong>.</p> <p>The task must complete no earlier than this date. </p> </li>
<li value="6">Click <strong>Save Changes.</strong> </li>
</ol>
</div>
-->
