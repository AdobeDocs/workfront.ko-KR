---
content-type: reference;how-to-procedural
product-area: projects
navigation-topic: task-constraints
title: '작업 제한 개요: 다음 이후에 완료:'
description: 다음보다 이전 완료(FNET)는 지정한 날짜 이후에 작업을 완료하도록 예약하는 작업 제한 사항입니다.
author: Alina
feature: Work Management
exl-id: b1dbf5c9-34b6-4c25-b582-ce9454501e03
source-git-commit: 7427706f6ce6cad3370b91269c1b4e7a10ed09f9
workflow-type: tm+mt
source-wordcount: '389'
ht-degree: 0%

---

# 작업 제한 개요: 다음 이후에 완료:

다음보다 이전 완료(FNET)는 지정한 날짜 이후에 작업을 완료하도록 예약하는 작업 제한 사항입니다.

## 다음 이후에 완료 제한 개요

다음 이후에 완료(FNET) 제한 사항을 작업에 사용할 때는 다음 사항을 고려하십시오.

* 프로젝트가 완료 일자부터 예약된 경우 이 제한을 사용해야 합니다. 이 경우 다른 종속 작업이 위험 상태로 표시되기 전에 작업에 대한 소프트 제한을 제공할 수 있습니다.
* 예약된 프로젝트&#x200B;**시작 날짜부터**&#x200B;에서 FNET을 사용하면 가능한 한 빨리 제한이 설정된 경우 제한 사항이 작업을 예약하는 것처럼 작업을 예약합니다.
* FNET 제한 사항이 있는 작업을 다른 프로젝트로 이동하거나 복사하는 경우 제한 일자가 무엇이고 프로젝트의 시작 및 완료 일자가 무엇인지에 따라 작업 제한 사항이나 프로젝트 일자가 변경될 수 있습니다. 다음과 같은 시나리오가 있습니다.

   * 대상 프로젝트가 시작부터 예약된 경우:

      * 작업의 제한 일자가 프로젝트 계획 시작 일자보다 빠를 경우 작업 제한 사항은 가능한 한 빨리 로 변경됩니다.
      * 작업의 제한 일자가 프로젝트 계획 완료 일자보다 늦으면 프로젝트 계획 완료 일자가 작업의 완료 제한 일자와 일치하도록 변경됩니다.

   * 대상 프로젝트가 완료부터 예약된 경우:

      * 작업의 제한 일자가 프로젝트 완료 일자보다 늦으면 작업 제한 사항이 가능한 한 늦게 변경됩니다.
      * 작업의 제한 일자가 프로젝트의 계획된 시작 일자보다 빠를 경우 프로젝트의 계획된 시작 일자가 작업의 시작 제한 일자와 일치하도록 변경됩니다.

   * 프로젝트의 일정에 관계없이 작업의 제한 일자가 프로젝트의 시작 및 완료 일자 내에 있으면 작업 제한 일자 또는 프로젝트 일자에 대한 변경 사항이 없습니다.

  작업 이동에 대한 자세한 내용은 [작업 이동](../../../manage-work/tasks/manage-tasks/move-tasks.md)을 참조하십시오. 작업 복사에 대한 자세한 내용은 [작업 복사 및 복제](../../../manage-work/tasks/manage-tasks/copy-and-duplicate-tasks.md)를 참조하십시오.

  작업에 대한 작업 제한을 업데이트하는 방법에 대한 자세한 내용은 [작업의 작업 제한 업데이트](../../../manage-work/tasks/task-constraints/update-task-constraint-of-task.md)를 참조하십시오.

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
