---
content-type: reference;how-to-procedural
product-area: projects
navigation-topic: task-constraints
title: '작업 제한 개요: 가능한 한 빨리'
description: 가능한 한 빨리 는 작업 시작 시간을 프로젝트 시작 부분에 최대한 가깝게 배치하는 작업 제한입니다.
author: Alina
feature: Work Management
exl-id: 9cb232fe-bc74-4433-afac-88be69514c88
source-git-commit: f2f825280204b56d2dc85efc7a315a4377e551c7
workflow-type: tm+mt
source-wordcount: '391'
ht-degree: 0%

---

# 작업 제한 개요: 가능한 한 빨리

가능한 한 빨리 는 작업 시작 시간을 프로젝트 시작 부분에 최대한 가깝게 배치하는 작업 제한입니다.

## 가능한 한 빨리 제약 조건을 사용하기 위한 고려 사항

* 프로젝트가 시작 날짜로부터 스케줄의 스케줄 모드를 사용하고 신규 태스크에 대한 시스템 기본 시작 일자가 프로젝트 계획 일자 기준으로 설정된 경우 가능한 한 빨리 기본 제한조건이 됩니다.

* 프로젝트가 시작 날짜부터 스케줄 모드를 사용하고 새 작업에 대한 시스템 또는 그룹 기본 시작 날짜를 오늘로 설정한 경우 기본 작업 제약 조건은 시작 아니오입니다.

   새 작업에 대한 기본 제약 조건을 설정할 위치에 대한 자세한 내용은 [시스템 전체 작업 및 문제 환경 설정 구성](../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-task-issue-preferences.md).

작업에 대한 작업 제약 조건을 업데이트하는 방법에 대한 자세한 내용은 [작업의 작업 제약 조건 업데이트](../../../manage-work/tasks/task-constraints/update-task-constraint-of-task.md).

<!--
<div data-mc-conditions="QuicksilverOrClassic.Draft mode">
<p>(NOTE: replaced with new article linked above) </p>
<p>To update the Task Constraint to As Soon As Possible: </p>
<ol>
<li value="1">Go to a task whose Task Constraint you want to update.</li>
<li value="2"> <p data-mc-conditions="QuicksilverOrClassic.Quicksilver">Click the <strong>More</strong> icon <img src="assets/qs-more-icon-on-an-object.png"> next to the task name, then click <strong>Edit</strong>.</p> </li>
<li value="3"> <p>In the <strong>Overview</strong> section, expand the <strong>Task Constraint</strong> drop-down menu.</p> </li>
<li value="4"> <p>Select <strong>As Soon As Possible</strong>.</p> </li>
<li value="5">Click <strong>Save Changes</strong>. </li>
</ol>
</div>
-->

## 가능한 한 빨리 가능한 가장 빠른 시간 및 간격

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: [! This section is duplicated in "Earliest Available Time"])&nbsp;</p>
-->

사용 가능한 가장 이른 시간 제약 조건은 다음 기준이 모두 있을 때 가능한 한 빨리 제한과 다릅니다.

* 프로젝트가 완료로 예약되었습니다.
* 프로젝트의 작업은 이전 관계가 있습니다.
* 이전 작업의 작업 제약 조건이 유연합니다.

이 경우:

* **사용 가능한 가장 이른 시간:** 후속 작업에 대해 사용 가능한 가장 이른 시간 제약 조건을 사용하면 선행 작업의 유연한 제약 조건에 우선 순위가 지정됩니다.

   예를 들어 작업 A가 작업 B의 전임자라고 가정합니다. 작업 B는 사용 가능한 가장 이른 시간 제약 조건을 가지고 작업 A는 가능한 한 늦습니다. 이 경우 작업은 가능한 한 프로젝트 완료에 가깝게 예약됩니다.

* **가능한 한 빨리:** 이 시나리오에서는 후속 작업에 대해 가능한 한 빨리 제약 조건을 사용하여 후속 작업에 우선 순위를 제공합니다.

   예를 들어 작업 A가 작업 B의 전임자라고 가정합니다. 작업 B는 가능한 한 빨리 제약 조건을 가지고 작업 A는 가능한 한 늦습니다. 이 경우 작업은 가능한 한 프로젝트 시작에 가깝게 예약됩니다.
