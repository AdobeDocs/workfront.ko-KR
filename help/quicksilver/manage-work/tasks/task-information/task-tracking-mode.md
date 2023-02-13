---
content-type: overview
product-area: projects
navigation-topic: task-information
title: 작업 추적 모드 개요
description: 작업을 만들거나 편집할 때 작업의 추적 모드 설정을 조정하여 작업의 진행 상태 표시기가 표시되는 방법과 시기를 제어할 수 있습니다. 작업 진행 상태 추적을 위한 특정 설정을 구성하면 Adobe Workfront에 진행 상태 플래그가 표시됩니다.
author: Alina
feature: Work Management
exl-id: 397b5593-ac01-40cf-b683-fcf671a53d26
source-git-commit: 6bb6b834c5af8ad48179fc0d60b184d083b360e4
workflow-type: tm+mt
source-wordcount: '626'
ht-degree: 3%

---

# 작업 추적 모드 개요

작업을 만들거나 편집할 때 작업의 추적 모드 설정을 조정하여 작업의 진행 상태 표시기가 표시되는 방법과 시기를 제어할 수 있습니다. 작업 진행 상태 추적을 위한 특정 설정을 구성하면 Adobe Workfront에 진행 상태 플래그가 표시됩니다.

작업의 진행 상태에 대한 자세한 내용은 [작업 진행 상태 개요](../../../manage-work/tasks/task-information/task-progress-status.md).

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

작업 소유자 또는 프로젝트 관리자는 Workfront이 각 작업의 진행 상태를 표시하는 방식을 선택할 수 있습니다. 작업에 대한 추적 모드를 설정하는 방법에 대한 자세한 내용은 [작업에 대한 추적 모드 설정](../../../manage-work/tasks/task-information/set-tracking-mode-for-tasks.md).

다음 옵션 중에서 선택할 수 있습니다.

* [사용자는 업데이트해야 합니다.](#user-must-update)
* [정시 추정](#assume-on-time)
* [지연 경고 무시](#ignore-late-warnings)
* [자동 완성](#auto-complete)
* [전임 작업](#predecessor)

### 사용자는 업데이트해야 합니다. {#user-must-update}

이 옵션을 선택하면 Workfront에서는 작업의 완료 비율 및 로그된 실제 시간을 사용하여 작업의 진행 상태를 확인합니다. 기본 옵션입니다.

### 정시 추정 {#assume-on-time}

Workfront에서는 현재 완료 상태에 관계없이 작업이 제시간에 완료된다고 가정합니다. 그렇지 않으면 Workfront에서 자동으로 다음 작업일의 계획된 완료 날짜를 가정합니다. 작업이 완료되는 시점을 표시해야 합니다. 사용자가 정기적으로 작업을 업데이트하지 않을 경우 이 옵션을 사용합니다.

### 지연 경고 무시 {#ignore-late-warnings}

작업의 진행 상태는 작업이 늦어질 때까지 정시에 표시됩니다. 예를 들어, 10일 동안 작업을 예약하고 작업이 완료되는 날에 완료율이 60%로 표시되면 Workfront은 4일을 추가하여 예상 완료일을 업데이트하며 작업의 진행 상태가 지연이 됩니다.

### 자동 완성 {#auto-complete}

Workfront은 작업이 예약됨으로 간주하여 기한 또는 계획 완료 날짜에 완료된 것으로 표시합니다. 그때까지 Workfront에서는 완료율 및 로그된 실제 시간을 사용하여 진행 상태를 확인합니다. 그러나 예약된 완료 날짜 이전의 진행 상태에 관계없이 Workfront에서는 여전히 작업이 완료되었음을 표시합니다.

다음과 같은 예외가 있습니다.

* 작업이 완료되지 않은 선행 작업이 있는 경우 선행 작업이 모두 완료될 때까지 자동으로 완료되지 않습니다.
* 작업에 고정 일자의 제약 조건이 있는 경우 선행 작업이 완료되었는지 여부에 관계없이 항상 계획 완료 날짜에 작업이 완료됩니다.

>[!IMPORTANT]
>
>작업을 자동으로 완료하도록 선택하면 프로젝트 시간이 재계산되면 작업이 완료됨으로 표시됩니다. 프로젝트의 업데이트 유형 이 자동 또는 자동 및 변경 시 로 설정되어 있으면 프로젝트 타임라인이 매일 계산됩니다. 프로젝트의 타임라인 재계산에 대한 자세한 내용은 다음을 참조하십시오 [프로젝트 타임라인 다시 계산](../../../manage-work/projects/manage-projects/recalculate-project-timeline.md).
>
>실제 완료 날짜 시간은 타임라인이 자동으로 계산되는 날의 자정입니다. 이 타임스탬프를 생성하는 데 사용되는 시간은 설정의 고객 정보 섹션에서 Workfront 관리자가 정의한 시스템의 시간대입니다. 시스템의 시간대 설정에 대한 자세한 내용은 [시스템에 대한 기본 정보 구성](../../../administration-and-setup/get-started-wf-administration/configure-basic-info.md).

### 전임 작업 {#predecessor}

Workfront은 이전 관계의 예상 작업 완료 날짜를 예측합니다. 작업의 진행 상태는 이 추정에 따라 결정됩니다. 예를 들어, 작업 B의 기간은 1일이며, 이전 작업 A의 작업 A 이후 2일 후에 완료되도록 예약되어 있으며, 이 작업은 5일이 소요됩니다. 사용자는 작업 B를 50%로 업데이트하지만 선행 작업 A는 아직 시작되지 않았습니다. Workfront은 종속 작업 B를 선행 작업의 시작 날짜 이후 6일 동안 스케줄링하여 작업 A의 경우 5일, 작업 B의 경우 1일을 허용합니다.
