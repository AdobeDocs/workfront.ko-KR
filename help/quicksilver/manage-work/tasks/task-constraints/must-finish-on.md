---
content-type: reference;how-to-procedural
product-area: projects
navigation-topic: task-constraints
title: '작업 제한 개요: 다음 일자에 완료되어야 함'
description: MFO(완료 시 필수) 작업 제한 사항을 사용하여 특정 날짜에 작업이 종료되도록 예약할 수 있습니다.
author: Alina
feature: Work Management
exl-id: 9e546a0f-7f7a-4f1c-9d9d-aa3cea377fdf
source-git-commit: dbc4404501e20b3f1905a5eebd13734a65db27ae
workflow-type: tm+mt
source-wordcount: '395'
ht-degree: 0%

---

# 작업 제한 개요: 다음 일자에 완료되어야 함

MFO(완료 시 필수) 작업 제한 사항을 사용하여 특정 날짜에 작업이 종료되도록 예약할 수 있습니다.

Must Finish On 제약 조건은 **계획된 완료 일자** 필드에 지정한 시간과 날짜에 정확히 작업을 완료하도록 예약합니다.

>[!TIP]
>
>작업의 계획된 완료 일자를 수동으로 업데이트하면 작업의 제한이 다음까지 완료되어야 합니다.

## 작업 제한 시 완료해야 함 개요

Must Finish On 제약 조건이 있는 작업을 예약할 때 다음 사항을 고려하십시오.

* 전임 작업 관계는 작업의 일정을 강제로 조정하지 않습니다. Adobe Workfront은 기본적으로 전임 작업 관계를 무시합니다.
* 전임 작업이 지연되거나 지연되면 작업이 **위험 상태**(으)로 표시됩니다.

* MFO 제한이 있는 작업을 다른 프로젝트로 이동하거나 복사할 때 제한 일자가 무엇인지와 프로젝트의 시작 및 완료 일자가 무엇인지에 따라 작업 제한 또는 프로젝트 일자가 변경될 수 있습니다. 다음과 같은 시나리오가 있습니다.

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
