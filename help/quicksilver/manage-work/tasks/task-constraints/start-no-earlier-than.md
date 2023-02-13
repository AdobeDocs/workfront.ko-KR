---
content-type: reference;how-to-procedural
product-area: projects
navigation-topic: task-constraints
title: '작업 제한 개요: 보다 일찍 시작'
description: SNET(Start No Early To) 작업 제약 조건을 사용하여 지정한 날짜 이후에 작업을 시작하도록 예약합니다.
author: Alina
feature: Work Management
exl-id: 857859fb-87ee-4397-b292-239ed9dc8281
source-git-commit: f2f825280204b56d2dc85efc7a315a4377e551c7
workflow-type: tm+mt
source-wordcount: '491'
ht-degree: 0%

---

# 작업 제한 개요: 보다 일찍 시작

SNET(Start No Early To) 작업 제약 조건을 사용하여 지정한 날짜 이후에 작업을 시작하도록 예약합니다.

## 작업 제한보다 이전 시작 번호 개요

작업 제한보다 이전 시작 번호 를 사용할 때는 다음 사항을 고려하십시오.

* 프로젝트가 시작 날짜로부터 예약되어 있는 경우 보다 이전 시작 없음 제한을 사용해야 합니다. 이 경우 다른 종속 작업이 위험 상태로 표시되기 전에 작업에 소프트 제한을 제공할 수 있습니다.
* 시작 일자: 부터 프로젝트를 예약하고 신규 작업에 대한 시스템 또는 그룹 기본 시작 일자를 오늘로 설정한 경우, 이전 시작 일자는 기본 제한입니다. 작업의 기본값 구성에 대한 내용은 [시스템 전체 작업 및 문제 환경 설정 구성](../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-task-issue-preferences.md).

* 프로젝트 시작 일자부터 일정을 예약하고 신규 태스크에 대한 시스템 기본 시작 일자를 프로젝트 계획 일자 기준으로 설정하면 신규 태스크에 대한 기본 제약 조건은 가능한 한 빨리 입니다.
* 프로젝트 완료 일자부터 프로젝트를 예약하고 신규 작업에 대한 시스템 기본 시작 날짜를 오늘로 설정한 경우, 시작 초과 제한 조건은 가능한 한 지연 태스크처럼 작업을 스케줄링합니다.
* SNET 제약 조건이 있는 작업을 다른 프로젝트에 이동하거나 복사하면 제한 날짜가 무엇이고 프로젝트의 시작 날짜와 완료 날짜가 무엇인지에 따라 작업 또는 프로젝트 날짜가 변경될 수 있습니다. 다음 시나리오가 있습니다.

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
<h2>Use the Start No Earlier Than Task Constraint</h2>
<p>(NOTE:&nbsp;replaced with new article linked above)&nbsp;</p>
<p>To update the Task Constraint to Start No Later Than:</p>
<ol>
<li value="1">Go to a task whose Task Constraint you want to update.</li>
<li value="2"> <p data-mc-conditions="QuicksilverOrClassic.Quicksilver">Click the <strong>More</strong> icon <img src="assets/qs-more-icon-on-an-object.png"> next to the task name, then click <strong>Edit</strong>.</p> </li>
<li value="3">In the <strong>Overview</strong> section, expand the <strong>Task Constraint</strong> drop-down menu.</li>
<li value="4"> <p>Select <strong>Start No Earlier Than</strong>.</p> </li>
<li value="5"> <p>Specify a <strong>Planned Start Date</strong>.</p> <p>This is the date by which the task must start, and not earlier than this date. </p> </li>
<li value="6">Click <strong>Save Changes</strong>.</li>
</ol>
</div>
-->
