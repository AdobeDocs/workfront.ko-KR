---
product-area: reporting
navigation-topic: text-mode-reporting
title: 텍스트 모드 개요
description: 보고서나 목록을 구성하는 요소를 만들 때 표준 또는 텍스트 모드 인터페이스를 사용하여 Adobe Workfront에서 보고서나 목록을 빌드할 수 있습니다.
author: Nolan
feature: Reports and Dashboards
exl-id: 8be8cbd0-da1b-4e90-a52e-dc352f646d18
source-git-commit: 9caac488522d2a12d3bdf4bf23ba7e44c6dbf7d2
workflow-type: tm+mt
source-wordcount: '798'
ht-degree: 0%

---

# 텍스트 모드 개요

<!-- Audited: 1/2025 -->

<!--(NOTE: Linked to the UI (for the areas mentioned in the comments below and the new NWE filters as well))-->

<!--(NOTE: Alina: ***Linked to other articles. Do not move, rename or change url.Linked to the product, in the report builder, when using a field that is not recognized in standard mode.)-->

<!--(NOTE: This will be linked to the Ninja feature about adding a filter to the User typeahead field (which originally is open only for text mode filters). Update the Context Sensitive sheet at release time)-->

보고서나 목록을 구성하는 요소를 만들 때 표준 또는 텍스트 모드 인터페이스를 사용하여 Adobe Workfront에서 보고서나 목록을 빌드할 수 있습니다.

표준 인터페이스를 사용하면 Workfront 인터페이스에서 쉽게 사용할 수 있는 필드 및 해당 속성을 참조할 수 있습니다.

텍스트 모드를 사용하면 표준 모드에서는 사용할 수 없지만 Workfront 데이터베이스에서는 사용할 수 있는 필드 및 속성을 참조할 수 있습니다.

클래스, 비디오 및 튜토리얼을 포함하여 텍스트 모드를 사용하여 보고서를 만드는 방법에 대한 자세한 내용은 Adobe Experience League 사이트의 학습 섹션을 참조하십시오.

## 텍스트 모드 사용 전 고려 사항

>[!TIP]
>
>사용자 정의 필드에 대한 텍스트 모드 버전을 사용하여 계산된 사용자 정의 필드의 기능을 확장할 수도 있습니다. 계산된 사용자 정의 필드를 만들기 위한 구문 및 규칙은 보고서 및 목록에서 사용하는 구문 및 규칙과 다릅니다. 계산된 사용자 지정 필드를 추가하는 방법에 대한 자세한 내용은 [양식에 계산된 필드 추가](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/form-designer/design-a-form/add-a-calculated-field.md)를 참조하십시오.

* 보고서에서 텍스트 모드를 사용하기 전에 텍스트 모드 언어를 더 깊이 있게 이해할 수 있도록 고급 보고에 대한 강의를 수강하는 것이 좋습니다.
* Workfront 소프트웨어가 업데이트될 때 만드는 보고서가 그대로 유지되도록 표준 모드를 사용하는 것이 좋습니다. 텍스트 모드를 사용하면 더 복잡한 보기, 필터 및 그룹화를 만들 수 있지만, 유지 관리가 더 복잡하고 Workfront 소프트웨어가 업데이트될 때 보장되지 않습니다.
* 항상 표준 인터페이스의 모든 보고 요소를 빌드하고 몇 가지 조정만 하기 위해 텍스트 모드 빌더로 전환하는 것이 좋습니다.

  >[!TIP]
  >
  >표준 빌더를 사용하면 텍스트 모드에서 코드를 수정할 때 사용할 수 있는 중요한 구성 요소와 코드 패턴을 얻을 수 있습니다.

* 텍스트 모드에서 보고서와 목록을 성공적으로 작성하기 위해 사용해야 하는 규칙 세트와 고유한 구문이 있습니다. 시작하기 전에 텍스트 모드의 Workfront 구문을 잘 알고 있는지 확인합니다.

  텍스트 모드 사용 구문 및 규칙에 대한 자세한 내용은 [텍스트 모드 구문 개요](../../../reports-and-dashboards/reports/text-mode/text-mode-syntax-overview.md)를 참조하십시오.

* 텍스트 모드에서 보고 요소를 사용자 지정한 후 보기에서 표준 모드로 다시 전환하지 못하거나 만든 요소의 코드가 필터 및 그룹화에서 삭제될 수 있습니다. 텍스트 모드에서 지원되는 모든 필드가 표준 모드에서 지원되는 것은 아니기 때문입니다.

## 표준 모드 인터페이스

표준 모드 인터페이스에는 보고서나 목록에 표시할 응용 프로그램 요소를 매핑하는 필드가 표시됩니다. 표준 모드 인터페이스는 보고서나 목록에 표시할 필드를 선택할 수 있는 드롭다운 메뉴 세트입니다.

표준 모드 인터페이스에 대한 자세한 내용과 보고서나 목록을 만드는 방법에 대한 자세한 내용은 다음을 참조하십시오.

* [사용자 지정 보고서를 만듭니다](../../../reports-and-dashboards/reports/creating-and-managing-reports/create-custom-report.md).
* [보고 요소: 필터, 보기 및 그룹화](../../../reports-and-dashboards/reports/reporting-elements/reporting-elements-filters-views-groupings.md)

## 텍스트 모드 인터페이스

텍스트 모드를 사용하면 표준 모드 인터페이스에서 사용할 수 없는 필드를 사용할 수 있으므로 더 복잡한 보기, 필터, 그룹화 및 프롬프트를 만들 수 있습니다. Workfront 텍스트 모드는 보고서나 목록에 표시할 객체를 나타내는 코딩된 명령문 모음입니다.

보고 가능한 모든 필드의 전체 목록을 보려면 [API 탐색기](../../../wf-api/general/api-explorer.md)를 참조하십시오.

>[!NOTE]
>
>API를 통해 사용할 수 있는 일부 필드는 텍스트 모드 인터페이스를 통해 사용할 수 없습니다. 텍스트 모드 코드에서 올바른 필드를 사용하고 예상한 결과를 표시하지 않는 경우 필드는 API를 통해서만 보고할 수 있습니다.

## 보고 요소 액세스 및 텍스트 모드 편집 {#access-reporting-elements-and-edit-text-mode}

텍스트 모드 인터페이스에 액세스하는 방법은 보고서나 목록에서 텍스트 모드 인터페이스에 액세스할 때 보기, 그룹화 및 필터와 유사합니다.

보기, 필터 및 그룹화에서 텍스트 모드를 사용하는 방법에 대한 자세한 내용은 다음을 참조하십시오.

* [텍스트 모드를 사용하여 보기 편집](../../../reports-and-dashboards/reports/text-mode/edit-text-mode-in-view.md)
* [텍스트 모드를 사용하여 필터 편집](../../../reports-and-dashboards/reports/text-mode/edit-text-mode-in-filter.md)
* [텍스트 모드를 사용하여 그룹화 편집](../../../reports-and-dashboards/reports/text-mode/edit-text-mode-in-grouping.md)

사용자 지정 프롬프트는 텍스트 모드에서만 편집할 수 있습니다. 보고서에서 프롬프트에 대해서만 액세스할 수 있습니다.

사용자 지정 프롬프트의 텍스트 모드 인터페이스에 액세스하는 방법에 대한 자세한 내용은 [보고서에 프롬프트 추가](../../../reports-and-dashboards/reports/creating-and-managing-reports/add-prompt-report.md)를 참조하십시오.

## 텍스트 모드를 사용하는 일반적인 이유 {#common-reasons-to-use-text-mode}

텍스트 모드를 사용해서만 구성할 수 있는 사용자 지정 프롬프트를 만드는 것 외에 Report Builder를 사용하여 보기, 필터 및 그룹화를 빌드하는 것이 좋습니다. 그러나 텍스트 모드를 사용하여 보고서와 목록을 개선할 수 있는 인스턴스가 있습니다.

텍스트 모드의 일반적인 사용에 대한 자세한 내용은 [텍스트 모드의 일반적인 사용 개요](../../../reports-and-dashboards/reports/text-mode/understand-common-uses-text-mode.md)를 참조하십시오.
