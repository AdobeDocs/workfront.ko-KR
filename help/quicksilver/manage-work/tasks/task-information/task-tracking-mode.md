---
content-type: overview
product-area: projects
navigation-topic: task-information
title: 작업 추적 모드 개요
description: 작업을 만들거나 편집할 때 작업의 추적 모드 설정을 조정하여 작업의 진행 상태 표시기가 표시되는 방식과 시기를 제어할 수 있습니다. Adobe Workfront은 작업의 진행 상황을 추적하기 위해 특정 설정을 구성할 때 진행 상태 플래그를 표시합니다.
author: Alina
feature: Work Management
exl-id: 397b5593-ac01-40cf-b683-fcf671a53d26
source-git-commit: 7427706f6ce6cad3370b91269c1b4e7a10ed09f9
workflow-type: tm+mt
source-wordcount: '646'
ht-degree: 3%

---

# 작업 추적 모드 개요

<!-- Audited: 01/2024 -->

작업을 만들거나 편집할 때 작업의 추적 모드 설정을 조정하여 작업의 진행 상태 표시기가 표시되는 방식과 시기를 제어할 수 있습니다. Adobe Workfront은 작업의 진행 상황을 추적하기 위해 특정 설정을 구성할 때 진행 상태 플래그를 표시합니다.

작업의 진행 상태에 대한 자세한 내용은 [작업 진행 상태 개요](../../../manage-work/tasks/task-information/task-progress-status.md)를 참조하십시오.

<!--
<div data-mc-conditions="QuicksilverOrClassic.Draft mode">
<h2>Set Tracking Mode for tasks</h2>
<p>(NOTE: drafted, because we created a new article and linked it below. Left this article as a "Overview" article only.) </p>
<p>To set the tracking mode:</p>
<ol>
<li value="1">Go to the task you want to set the tracking mode for.</li>
<li value="2"> <p data-mc-conditions="QuicksilverOrClassic.Quicksilver">Click the <strong>More</strong> icon <img src="assets/qs-more-icon-on-an-object.png">next to the name of the task, then click&nbsp;<strong>Edit</strong>.</p> <p>The Edit Task dialog box opens. </p> </li>
<li value="3"> <p>In the&nbsp;<strong>Settings</strong> section, use the&nbsp;<strong>Tracking Mode</strong> drop-down menu to select the Tracking Mode for the task.</p> <p>For more information about the tracking mode options, see the <a href="#tracking-mode-options" class="MCXref xref" xrefformat="{para}">Tracking Mode options</a> section in this article. </p> </li>
<li value="4">Click&nbsp;<strong>Save Changes.</strong></li>
</ol>
</div>
-->

## 추적 모드 옵션 {#tracking-mode-options}

작업 소유자 또는 프로젝트 관리자는 Workfront이 각 작업의 진행 상태를 표시하는 방법을 선택할 수 있습니다. 작업에 대한 추적 모드를 설정하는 방법에 대한 자세한 내용은 [작업에 대한 추적 모드 설정](../../../manage-work/tasks/task-information/set-tracking-mode-for-tasks.md)을 참조하십시오.

다음 옵션 중에서 선택할 수 있습니다.

* [사용자가 업데이트해야 함](#user-must-update)
* [정시 가정](#assume-on-time)
* [지연 경고 무시](#ignore-late-warnings)
* [자동 완성](#auto-complete)
* [전임 작업](#predecessor)

### 사용자는 업데이트해야 합니다. {#user-must-update}

이 옵션을 선택하면 Workfront에서는 작업의 완료율 및 기록된 실제 시간을 사용하여 작업의 진행 상태를 확인합니다. 기본 옵션입니다.

### 정시 추정 {#assume-on-time}

Workfront에서는 현재 완료 상태에 관계없이 작업이 정시에 완료된다고 가정합니다. 작업이 정시에 완료되지 않으면(계획된 완료 일자에) Workfront은 자동으로 계획된 완료 일자를 다음 근무일로 가정합니다. 작업이 완료되는 시기를 표시해야 합니다. 사용자가 작업을 정기적으로 업데이트하지 않을 때 이 옵션을 사용합니다.

### 지연 경고 무시 {#ignore-late-warnings}

작업 진행 상태는 늦어질 때까지 정시에 표시됩니다. 예를 들어 작업을 10일 동안 수행하도록 예약하고 완료되는 날짜에 작업이 완료되도록 예약하면 작업의 완료율이 60%로 표시되면 Workfront이 4일을 추가하여 예상 완료 일자를 업데이트하고 작업의 진행 상태가 지연됩니다.

### 자동 완성 {#auto-complete}

Workfront에서는 작업이 예약된 대로 완료된다고 가정하고 기한 또는 계획된 완료 일자에 완료된 것으로 표시합니다. 그때까지 Workfront은 완료율 및 기록된 실제 시간을 사용하여 진행 상태를 확인합니다. 그러나 예약된 완료 일자 이전의 진행 상태에 관계없이 Workfront은 여전히 작업을 완료로 표시합니다.

다음과 같은 예외가 있습니다.

* 작업에 완료되지 않은 전임 작업이 있는 경우 해당 전임 작업이 모두 완료될 때까지 작업이 자동으로 완료되지 않습니다. 전임 작업은 강제 적용되어야 합니다.
* 작업에 고정 일자 제한이 있는 경우 선행 작업의 완료 여부에 관계없이 작업은 항상 계획된 완료 일자에 완료됩니다.

>[!IMPORTANT]
>
>작업을 자동으로 완료하도록 선택하면 프로젝트 시간이 다시 계산될 때 작업이 완료로 표시됩니다. 프로젝트의 업데이트 유형 이 자동 또는 자동으로 설정되고 변경 시 프로젝트 타임라인이 매일 계산됩니다. 프로젝트의 타임라인 다시 계산에 대한 자세한 내용은 [프로젝트 타임라인 다시 계산](../../../manage-work/projects/manage-projects/recalculate-project-timeline.md)을 참조하세요.
>
>실제 완료 일자의 시간은 타임라인이 자동으로 계산되는 날의 자정입니다. 이 타임스탬프를 생성하는 데 사용되는 시간은 Workfront 관리자가 설정의 고객 정보 섹션에서 정의한 시스템의 시간대입니다. 시스템의 표준 시간대 설정에 대한 자세한 내용은 [시스템에 대한 기본 정보 구성](../../../administration-and-setup/get-started-wf-administration/configure-basic-info.md)을 참조하십시오.

### 전임 작업 {#predecessor}

Workfront은 전임 작업 관계에 따라 작업의 예상 완료 일자를 예측합니다. 작업의 진행 상태는 이 예측에 따라 결정됩니다. 예를 들어 작업 B의 기간은 1일이며 전임 작업 A보다 2일 후인 5일이 소요될 예정입니다. 그런 다음 사용자는 작업 B를 50% 완료로 업데이트하지만 전임 작업 A는 아직 시작되지 않았습니다. Workfront은 전임 작업 시작일로부터 6일 후에 종속 작업 B를 완료하도록 예약하여 작업 A의 경우 5일, 작업 B의 경우 1일을 허용합니다.
