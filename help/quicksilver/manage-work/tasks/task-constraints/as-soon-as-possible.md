---
content-type: reference;how-to-procedural
product-area: projects
navigation-topic: task-constraints
title: '작업 제한 개요: 가능한 한 빨리'
description: 가능한 한 빨리 는 작업 시작 시간을 프로젝트 시작 시간과 가깝게 배치하는 작업 제한 사항입니다.
author: Alina
feature: Work Management
exl-id: 9cb232fe-bc74-4433-afac-88be69514c88
source-git-commit: 7427706f6ce6cad3370b91269c1b4e7a10ed09f9
workflow-type: tm+mt
source-wordcount: '391'
ht-degree: 0%

---

# 작업 제한 개요: 가능한 한 빨리

가능한 한 빨리 는 작업 시작 시간을 프로젝트 시작 시간과 가깝게 배치하는 작업 제한 사항입니다.

## 가능한 한 빠른 시간 내에 를 사용하기 위한 고려 사항

* 프로젝트가 시작 날짜부터 일정 모드로 일정 모드를 사용하고 새 작업의 시스템 기본 시작 날짜가 프로젝트 계획 날짜에 따라 설정된 경우 가능한 한 빨리 기본 제한 사항이 됩니다.

* 프로젝트가 시작 일자부터 스케줄 모드를 사용하고 시스템 또는 그룹의 새 작업에 대한 기본 시작 일자가 오늘로 설정된 경우 기본 작업 제한은 시작 일자 이전입니다.

  새 작업의 기본 제한 사항을 설정할 위치에 대한 자세한 내용은 [시스템 전체 작업 및 문제 환경 설정 구성](../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-task-issue-preferences.md)을 참조하세요.

작업에 대한 작업 제한을 업데이트하는 방법에 대한 자세한 내용은 [작업의 작업 제한 업데이트](../../../manage-work/tasks/task-constraints/update-task-constraint-of-task.md)를 참조하십시오.

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

## 가능한 가장 빠른 시간과 가능한 빠른 시간의 차이

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: [! This section is duplicated in "Earliest Available Time"])&nbsp;</p>
-->

다음 기준이 모두 있는 경우 가장 빠른 가용 시간 제약조건이 가능한 한 빨리 제약조건과 다릅니다.

* 프로젝트가 완료부터 예약됩니다.
* 프로젝트의 작업에 전임 작업 관계가 있습니다.
* 전임 작업은 유연한 작업 제한 사항이 있습니다.

이 경우:

* **가장 빠른 사용 가능한 시간:** 후속 작업에 가장 빠른 사용 가능한 시간 제한을 사용하면 전임 작업의 유연한 제한 사항에 우선 순위를 둘 수 있습니다.

  예를 들어, 태스크 A가 태스크 B의 전임자라고 가정합니다. 태스크 B가 가장 빠른 가용 시간 제한을 가지며, 태스크 A가 가능한 한 늦은 시간 제한을 가진다고 가정합니다. 이러한 상황에서 가능한 한 프로젝트 완료에 가깝게 업무가 예정되어 있다.

* **가능한 한 빨리:** 이 시나리오에서는 후임 작업에 대해 가능한 한 빨리 제한을 사용하면 후임 작업에 우선 순위가 지정됩니다.

  예를 들어 작업 A가 작업 B의 전임자라고 가정해 보겠습니다. 작업 B에는 가능한 한 빨리 제한이 있고 작업 A에는 가능한 한 늦게 제한이 있습니다. 이러한 상황에서 작업은 가능한 프로젝트 시작에 가깝게 예약됩니다.
