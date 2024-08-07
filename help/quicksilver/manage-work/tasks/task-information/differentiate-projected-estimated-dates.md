---
content-type: overview
product-area: projects
navigation-topic: task-information
title: 예상 및 예상 일자 개요
description: 시작 가능한 시점과 완료 가능한 시점 사이의 작업 시간표를 표시하는 몇 가지 유형의 날짜가 있습니다.
author: Alina
feature: Work Management
exl-id: 7cc68fc4-5f79-4ce6-a404-737ea8959ec3
source-git-commit: 811d8076a0b344e863b25aa253a0fb1c102f0435
workflow-type: tm+mt
source-wordcount: '924'
ht-degree: 0%

---

# 예상 및 예상 일자 개요

<!--Audited: 07/2024-->

시작 가능한 시점과 완료 가능한 시점 사이의 작업 시간표를 표시하는 몇 가지 유형의 날짜가 있습니다. 다음은 작업 타임라인을 표시하는 일부 날짜입니다.

* 계획된 시작 및 계획된 완료 일자
* 예상 시작 및 예상 완료 일자
* 예상 시작 및 예상 기한
* 실제 시작 및 실제 완료 일자

이 문서에서는 프로젝트에 대한 예상 일자와 예상 일자의 차이점에 대해 설명합니다.

작업을 처음 만들 때 계획된 일자, 예상 일자 및 예상 일자가 일반적으로 일치해야 합니다. 일부 예외가 존재합니다.

Adobe Workfront의 프로젝트, 작업 및 문제 날짜에 대한 자세한 내용은 [Workfront의 프로젝트, 작업 및 문제 날짜 개요](../../../workfront-basics/navigate-workfront/workfront-navigation/definitions-pti-dates.md)를 참조하십시오.

## 계획된 일자 개요

계획된 일자는 프로젝트 소유자가 작업의 시작 및 종료 일자로 정의하는 일자입니다. 사용자 또는 프로젝트 소유자는 작업에 대한 계획된 일자를 수동으로 수정할 수 있습니다.

## 실제 일자 개요

작업을 처음 만들 때 아직 시작하지도 완료하지도 않았으므로 실제 날짜가 없습니다.

## 예상 및 예상 일자 개요

프로젝트 수명 동안에는 작업의 실제 시작 및 종료에 영향을 줄 수 있는 사항을 고려하므로 예상 및 예상 날짜는 프로젝트의 현실과 더 비슷합니다. 이렇게 하면 계획된 일자에서 변경됩니다.

작업에 대한 예상 및 예상 일자 작업을 수행할 때는 다음 사항을 고려하십시오.

* 작업의 예상 일자 또는 예상 일자를 수동으로 수정할 수 없습니다. 둘 다 Adobe Workfront에 의해 계산됩니다.
* 작업을 생성할 때 예상 날짜와 예상 날짜는 동일해야 하며 작업이 시작되거나 종료될 수 있는 실제 시간을 보여 주어야 합니다.\
  작업에 대해 수행하는 특정 업데이트는 예상 및 예상 일자의 값에 직접 영향을 줍니다.

  예를 들어 사용자가 작업을 시작하거나 완료하면 작업의 예상 및 예상 날짜에 영향을 주는 실제 시작 및 완료 날짜가 표시됩니다. 또한 작업의 할당자가 커밋 일자를 수정하는 경우 이 일자는 작업의 예상 일자에 영향을 줍니다.

## 예상 일자와 예상 일자의 차이

예상 일자와 예상 일자의 차이는 다음과 같습니다.

* 예상 날짜는 작업에 대해 다음과 같은 업데이트를 수행하는 사용자의 영향을 받습니다.

   * 고정 작업 제한 사항을 추가하여 제한 일자 추가
   * 커밋 일자 추가

* 예상 일자는 주어진 시점의 작업에 대한 실제 진행 상황만 고려합니다.

**예:** 작업의 계획된 시작 일자가 9월 20일이고 계획된 완료 일자가 9월 24일인 경우 제한 시 완료되어야 하며 예상 완료 일자는 9월 24일입니다. 이 작업의 기간은 4일입니다.

예상 완료 일자는 작업에 대한 현재 진행 상황을 기반으로 계산됩니다. 따라서 오늘이 9월 23일이고 작업이 아직 시작되지 않은 경우 예상 완료 일자는 9월 27일입니다(오늘 작업이 시작된다고 가정하고 4일 후에 완료되어야 함).

작업이 오늘 50% 완료된 경우 예상 완료 일자는 9월 25일입니다(작업 기간의 절반인 2일 후에 완료되어야 함).


### 작업에 대한 예상 일자가 업데이트되는 시기 이해 {#understand-when-projected-dates-update-on-tasks}

예상 날짜는 다른 작업 날짜와 일치하거나 작업의 실제 진행 상황을 고려하여 Workfront에서 수행한 계산입니다.

다음 목록에는 작업의 예상 일자가 작업의 실제 상황에 따라 프로젝트 기간 중에 변경되는 경우의 여러 시나리오가 표시됩니다.

* 작업이 완료로 표시되는 경우:

  `Projected Dates = Estimated Dates = Actual Dates`

* 작업에 실제 시작 일자가 있는 경우:

  `Projected Start Date = Estimated Start Date = Actual Start Date`

* 작업에 실제 시작 일자는 없지만 미래의 계획된 시작 일자(시작 일자에 시작 해야 함)에 대한 강제 제한이 있는 경우:

  `Projected Start Date = Constraint Date`

  제한 날짜에 대한 자세한 내용은 [Adobe Workfront 용어 용어집](../../../workfront-basics/navigate-workfront/workfront-navigation/workfront-terminology-glossary.md)을 참조하세요.

* 작업에 실제 시작 일자가 없고 작업에 강제 제한 일자가 없는 경우:

  `Projected Start Date = the next available date in the future that falls within working schedule`

* 피할당자가 커밋 일자를 업데이트할 때:

  `Projected Completion Date = Commit Date`

  커밋 날짜에 대한 자세한 내용은 [커밋 날짜 개요](../../../manage-work/projects/updating-work-in-a-project/overview-of-commit-dates.md)를 참조하십시오.

* 작업에 업데이트된 커밋 일자가 없고 작업에 미래의 계획된 완료 일자에 대한 강제 제한(다음까지 완료)이 있는 경우:

  `Projected Completion Date = Constraint Date`

* 작업에 업데이트된 커밋 일자, 강제 제한 일자가 미래의 경우 또는 제한 일자가 과거의 경우:

  `Projected Completion Date = system calculation for the Completion Date based on the current progress and the work left to be done`

### 작업에 대한 예상 일자 업데이트 시기 이해 {#understand-when-the-estimated-dates-update-on-tasks}

예상 날짜에 대해 위에 설명된 시나리오와 비교하여 예상 날짜는 제한 또는 커밋 날짜에 관계없이 작업이 시작되거나 완료되는 시기에 대한 Workfront의 실제 분석을 항상 반영합니다.

## 작업의 타임라인에 영향을 주는 것

다음은 작업의 실제 타임라인에 영향을 줄 수 있는 몇 가지 예입니다.

* 계획된 일자 및 현재 일자와 관련된 작업 진행
* 지금까지의 작업 완료율
* 전임 작업 관계
* 전임 작업 진행률
* 사용자 할당

  >[!NOTE]
  >
  >사용자 할당은 작업을 완료할 수 있는 속도에 영향을 주는 경우 작업의 예상 완료 날짜에 영향을 줄 수 있습니다. 예를 들어 작업 기간 유형이 작업량 고정 인 경우 피할당자를 추가하여 작업을 더 빨리 완료할 수 있습니다. 그 결과 예상 완료 일자가 변경됩니다.
