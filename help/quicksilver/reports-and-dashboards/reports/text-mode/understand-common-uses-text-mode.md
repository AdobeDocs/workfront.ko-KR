---
product-area: reporting
navigation-topic: text-mode-reporting
title: 텍스트 모드의 일반적인 사용 개요
description: 텍스트 모드의 일반적인 사용 개요
author: Nolan
feature: Reports and Dashboards
exl-id: 81512837-1ec4-4dbc-ace4-bdf08fe667ce
source-git-commit: 9caac488522d2a12d3bdf4bf23ba7e44c6dbf7d2
workflow-type: tm+mt
source-wordcount: '762'
ht-degree: 0%

---

# 텍스트 모드의 일반적인 사용 개요

<!-- Audited: 1/2025 -->

<!--(NOTE: Alina: ***This is linked to Understanding Text Mode (article), and the TOC article for examples of various reporting elements)</p>-->

보고서 및 보고서 요소에서 텍스트 모드를 사용하여 보고 기능을 확장할 수 있습니다. 텍스트 모드 버전을 사용하여 보다 복잡한 계산된 사용자 정의 필드를 작성할 수도 있습니다. 텍스트 모드에 대한 자세한 내용은 [텍스트 모드 개요](../../../reports-and-dashboards/reports/text-mode/understand-text-mode.md)를 참조하십시오.

이 문서에서는 Adobe Workfront에서 보고 또는 계산된 사용자 정의 필드 기능을 확장하기 위해 텍스트 모드를 사용해야 하는 경우에 대한 몇 가지 일반적인 예를 간략하게 설명합니다. 보다 광범위한 예제 목록은 다음을 참조하십시오.

* [사용자 지정 보기, 필터 및 그룹화 샘플: 문서 인덱스](../../../reports-and-dashboards/reports/custom-view-filter-grouping-samples/custom-view-filter-grouping-samples.md)
* [보고서의 계산된 사용자 정의 데이터](../../../reports-and-dashboards/reports/calc-cstm-data-reports/calculated-custom-data-reports.md)

클래스, 비디오 및 튜토리얼을 포함하여 텍스트 모드를 사용하여 보고서를 만드는 방법에 대한 자세한 내용은 Adobe Experience League 사이트의 학습 섹션을 참조하십시오.

## 목록 및 보고서에서 텍스트 모드를 사용할 수 있는 인스턴스

보고서 및 목록 빌더를 사용하여 보기, 필터 및 그룹화를 빌드하는 것이 좋습니다. 그러나 텍스트 모드를 사용하여 보고서와 목록을 개선할 수 있는 인스턴스가 있습니다.

Workfront에서 다음을 달성하고자 할 때 텍스트 모드를 사용할 수 있습니다.

* 사용자 정의 양식에서 사용자 정의 계산된 사용자 정의 필드를 작성합니다.\
  계산된 사용자 지정 필드에 대한 자세한 내용은 이 문서의 [계산된 사용자 지정 필드에서 텍스트 모드 사용](#use-text-mode-in-calculated-custom-fields) 섹션을 참조하십시오.
* Report Builder에서 사용할 수 있는 것보다 필터, 보기 및 그룹화를 향상시킵니다. 필터, 보기 및 그룹화에 텍스트 모드를 사용하는 방법에 대한 자세한 내용은 이 문서의 다음 섹션을 참조하십시오.

   * [보기에서 텍스트 모드 사용](#use-text-mode-in-views)
   * [필터에서 텍스트 모드 사용](#use-text-mode-in-filters)
   * [그룹화에 텍스트 모드 사용](#use-text-mode-in-groupings)

* 사용자 지정 프롬프트를 만듭니다. 텍스트 모드를 사용하는 사용자 정의 프롬프트만 만들 수 있습니다.

  사용자 지정 프롬프트를 작성하는 방법에 대한 자세한 내용은 [보고서에 프롬프트 추가](../../../reports-and-dashboards/reports/creating-and-managing-reports/add-prompt-report.md)를 참조하십시오.

## 계산된 사용자 정의 필드에서 텍스트 모드 사용 {#use-text-mode-in-calculated-custom-fields}

텍스트 모드를 사용하여 계산된 사용자 정의 필드를 사용자 정의 양식에 추가할 수 있습니다.

사용자 정의 양식에 계산된 사용자 정의 필드를 추가하는 방법에 대한 자세한 내용은 [사용자 정의 양식 만들기](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/form-designer/design-a-form/design-a-form.md)를 참조하십시오.

텍스트 모드에서 계산된 사용자 지정 필드를 만드는 방법에 대한 자세한 내용은 [양식에 계산된 필드 추가](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/form-designer/design-a-form/add-a-calculated-field.md)를 참조하십시오.

예를 들어, 항목이 [진행 중]으로 표시된 순간의 시간 및 날짜 스탬프를 표시하는 계산된 사용자 정의 필드를 추가할 수 있습니다. 다른 상태에 대해 이 계산을 사용할 수 있습니다.

자세한 내용은 [계산된 사용자 정의 필드 예: 사용자 정의 양식에 상태 타임스탬프 표시](../../../reports-and-dashboards/reports/calc-cstm-data-reports/example-status-timestamp-in-calculated-field.md)를 참조하십시오.

## 보기에서 텍스트 모드 사용 {#use-text-mode-in-views}

뷰에서 텍스트 모드를 사용하여 뷰에 표시할 수 있는 필드 및 객체를 확장할 수 있습니다.

보기에서 텍스트 모드를 사용하는 가장 일반적인 이유에 대한 예는 다음 문서를 참조하십시오.

* [보기: 표준 인터페이스에 포함되지 않은 개체를 표시합니다](../../../reports-and-dashboards/reports/custom-view-filter-grouping-samples/view-display-objects-not-in-standard-interface.md)
* [보기: 열에 있는 두 필드 간의 계산 결과를 표시합니다](../../../reports-and-dashboards/reports/custom-view-filter-grouping-samples/view-calculation-between-two-fields.md)
* [보기: 열의 너비를 영구적으로 편집](../../../reports-and-dashboards/reports/custom-view-filter-grouping-samples/view-edit-column-width-permanently.md)
* [보기: 하나의 공유 열에 있는 여러 열의 정보를 병합합니다](../../../reports-and-dashboards/reports/custom-view-filter-grouping-samples/view-merge-columns.md)
* [보기: 열의 개체에 대한 링크를 제거합니다](../../../reports-and-dashboards/reports/custom-view-filter-grouping-samples/view-remove-link-to-object.md)
* [보고서에서 컬렉션 참조](../../../reports-and-dashboards/reports/text-mode/reference-collections-report.md)
* [보기: 열의 내용을 숨깁니다](../../../reports-and-dashboards/reports/custom-view-filter-grouping-samples/view-hide-column-content.md)
* [보기: 열에 문자열 대신 이미지를 표시합니다](../../../reports-and-dashboards/reports/custom-view-filter-grouping-samples/view-display-image-in-view.md)
* [보기: 작업 목록에 작업 들여쓰기를 표시합니다](../../../reports-and-dashboards/reports/custom-view-filter-grouping-samples/view-display-task-identations.md)
* [보기: 시간 및 날짜 차이 계산](../../../reports-and-dashboards/reports/custom-view-filter-grouping-samples/view-calculate-time-and-date-differences.md)

## 필터에서 텍스트 모드 사용 {#use-text-mode-in-filters}

필터 작성 시 텍스트 모드를 사용하여 필터링할 수 있는 필드 및 개체에서 확장할 수 있습니다.

필터에서 텍스트 모드를 사용하는 가장 일반적인 이유에 대한 예는 다음 문서를 참조하십시오.

* [필터: 동일한 필드(&quot;AND&quot; 문)를 참조하는 필터 규칙을 여러 개 만듭니다.](../../../reports-and-dashboards/reports/custom-view-filter-grouping-samples/filter-refrence-the-same-field-multiple-times.md)
* [필터: 승인 상태의 항목만 표시](../../../reports-and-dashboards/reports/custom-view-filter-grouping-samples/filter-for-items-in-approval-status.md)
* [필터: 상태가 다른 그룹과 연결되어 있을 때 같은 이름 상태로 항목을 표시합니다](../../../reports-and-dashboards/reports/custom-view-filter-grouping-samples/filter-same-name-statuses-from-different-groups.md)
* [필터: 두 필드를 비교하여 목록에 있는 항목을 제거합니다.](../../../reports-and-dashboards/reports/custom-view-filter-grouping-samples/filter-items-by-comparing-two-fields.md)
* 문서 [EXISTS 문을 사용하여 복잡한 텍스트 모드 필터 만들기](../../../reports-and-dashboards/reports/text-mode/create-complex-text-mode-filters-using-exists-statements.md)의 섹션 [개체 계층에서 여러 수준에 걸쳐 있는 텍스트 모드 필터의 예](../../../reports-and-dashboards/reports/text-mode/create-complex-text-mode-filters-using-exists-statements.md#examples)
* 문서 [EXISTS 문을 사용하여 복합 텍스트 모드 필터 만들기](../../../reports-and-dashboards/reports/text-mode/create-complex-text-mode-filters-using-exists-statements.md)의 섹션 [누락된 개체에 대한 복합 텍스트 모드 필터 만들기](../../../reports-and-dashboards/reports/text-mode/create-complex-text-mode-filters-using-exists-statements.md#missing-object-filters)

## 그룹화에 텍스트 모드 사용 {#use-text-mode-in-groupings}

그룹화를 작성할 때 텍스트 모드를 사용하여 목록 및 보고서에서 그룹화할 수 있는 필드 및 개체를 확장할 수 있습니다.

그룹화에서 텍스트 모드를 사용하는 가장 일반적인 이유에 대한 예는 다음 문서를 참조하십시오.

* [그룹화: 그룹화에 있는 모든 개체에 공통되는 계산된 값으로 목록 결과를 구성합니다](../../../reports-and-dashboards/reports/custom-view-filter-grouping-samples/grouping-by-calculated-common-values.md)
* [그룹화: 네 번째 그룹화를 목록에 추가](../../../reports-and-dashboards/reports/custom-view-filter-grouping-samples/grouping-add-fourth-grouping.md)
* [그룹화: 그룹화에서 표시 이름을 편집합니다](../../../reports-and-dashboards/reports/custom-view-filter-grouping-samples/grouping-rename-grouping.md)
* [그룹화: 텍스트 모드를 사용하여 그룹화 결과를 축소할지 또는 확장할지 여부를 나타냅니다.](../../../reports-and-dashboards/reports/custom-view-filter-grouping-samples/grouping-collapsed-or-expanded-results.md)
