---
content-type: overview
product-area: projects
navigation-topic: plan-a-project
title: 프로젝트 기간 개요
description: Adobe Workfront은 가장 이른 작업의 시작 날짜와 최신 작업의 완료 날짜를 고려하여 프로젝트 기간을 계산하고 두 날짜 사이의 일 수를 계산합니다.
author: Alina
feature: Work Management
exl-id: b558eaad-669b-4079-b61a-07df227edfa2
source-git-commit: bbd64e9deed1b89d720272508b3562c354578704
workflow-type: tm+mt
source-wordcount: '253'
ht-degree: 2%

---

# 프로젝트 기간 개요

Adobe Workfront은 가장 이른 작업의 시작 날짜와 최신 작업의 완료 날짜를 고려하여 프로젝트 기간을 계산하고 두 날짜 사이의 일 수를 계산합니다.

## 프로젝트 기간

프로젝트 기간은 다음 공식으로 계산됩니다.

```
Project Duration = Completion Date of the latest task - Start Date of the earliest task
```

>[!NOTE]
>
>프로젝트의 문제 기간은 프로젝트 기간에 영향을 주지 않습니다.

프로젝트 기간은 프로젝트와 연결된 일정 또는 작업에 지정된 사용자를 기준으로 두 작업 날짜 사이의 일 수를 계산합니다. Workfront에서 지속 시간을 계산하는 데 사용하는 예약에 대한 자세한 내용은 [예약 개요](../../../administration-and-setup/set-up-workfront/configure-timesheets-schedules/schedules-overview.md).

## 프로젝트 기간 유형

프로젝트 지속 시간 과 Workfront에서 계산하는 수식의 두 가지 유형이 있습니다.

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: Check these formulas? Should they be divided by the hours per day?!) </p>
-->

* **계획된 기간**: 

   ```
   Project Planned Duration = Planned Completion Date of the latest task - Planned Start Date of the earliest task / Typical hour per day
   ```

* **실제 기간**: 

   ```
   Project Actual Duration = Actual Completion Date of the latest task - Actual Start Date of the earliest task / Typical hour per day
   ```

## 프로젝트 지속 시간 찾기

Workfront의 다음 영역에서 프로젝트 계획 및 실제 기간을 찾을 수 있습니다.

* . 프로젝트 세부 사항 영역의 개요 섹션에서

   프로젝트의 개요 하위 탭에 대한 자세한 내용은 문서를 참조하십시오 [프로젝트 개요 영역의 정보 관리](../../../manage-work/projects/manage-projects/understand-project-overview-area.md).

* 프로젝트 보고서에서 기간 또는 실제 기간 필드를 보고서에 포함하여 지정합니다.

   보고서 만들기에 대한 자세한 내용은 문서를 참조하십시오 [사용자 지정 보고서 만들기](../../../reports-and-dashboards/reports/creating-and-managing-reports/create-custom-report.md).
