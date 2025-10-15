---
content-type: overview
product-area: projects
navigation-topic: plan-a-project
title: 프로젝트 기간 개요
description: Adobe Workfront은 가장 빠른 작업의 시작 일자와 가장 최근 작업의 완료 일자를 고려하여 프로젝트의 기간을 계산하고 두 일자 사이의 일수를 계산합니다.
author: Alina
feature: Work Management
exl-id: b558eaad-669b-4079-b61a-07df227edfa2
source-git-commit: 5bc7a1c00b72cfc07270cafee5bf753989b48d33
workflow-type: tm+mt
source-wordcount: '253'
ht-degree: 0%

---

# 프로젝트 기간 개요

Adobe Workfront은 가장 빠른 작업의 시작 일자와 가장 최근 작업의 완료 일자를 고려하여 프로젝트의 기간을 계산하고 두 일자 사이의 일수를 계산합니다.

## 프로젝트 기간

프로젝트 기간은 다음 공식에 의해 계산됩니다.

```
Project Duration = Completion Date of the latest task - Start Date of the earliest task
```

>[!NOTE]
>
>프로젝트에 대한 문제 기간은 프로젝트 기간에 영향을 주지 않습니다.

프로젝트 기간은 프로젝트와 연결된 일정 또는 작업에 할당된 사용자를 기준으로 두 작업 날짜 사이의 일 수를 계산합니다. Workfront에서 기간을 계산하는 데 사용하는 일정에 대한 자세한 내용은 [일정 개요](../../../administration-and-setup/set-up-workfront/configure-timesheets-schedules/schedules-overview.md)를 참조하십시오.

## 프로젝트 기간 유형

프로젝트 기간 및 Workfront에서 계산하는 공식에는 두 가지 유형이 있습니다.

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

## 프로젝트 기간 찾기

Workfront의 다음 영역에서 프로젝트 계획 기간 및 실제 기간을 찾을 수 있습니다.

* . 프로젝트 세부 정보 영역의 개요 섹션에서 확인할 수 있습니다.

  프로젝트의 개요 하위 탭에 대한 자세한 내용은 문서 [프로젝트 개요 영역의 정보 관리](../../../manage-work/projects/manage-projects/understand-project-overview-area.md)를 참조하십시오.

* 기간 또는 실제 기간 필드를 보고서에 포함하여 프로젝트 보고서에서

  보고서 만들기에 대한 자세한 내용은 문서 [사용자 지정 보고서 만들기](../../../reports-and-dashboards/reports/creating-and-managing-reports/create-custom-report.md)를 참조하세요.
