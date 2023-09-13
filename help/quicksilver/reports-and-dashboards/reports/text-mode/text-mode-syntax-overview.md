---
product-area: reporting
navigation-topic: text-mode-reporting
title: 텍스트 모드 구문 개요
description: 텍스트 모드 인터페이스를 사용하여 목록 및 보고서에서 보다 복잡한 보기, 필터, 그룹화 및 사용자 지정된 프롬프트를 만들 수 있습니다. 텍스트 모드를 사용하면 표준 모드 인터페이스에서 사용할 수 없는 필드 및 해당 속성에 액세스할 수 있습니다.
author: Nolan
feature: Reports and Dashboards
role: User
exl-id: f24430e1-c5f7-4925-93df-0e956a03c863
source-git-commit: b774a74863bb35e3477a69ff11189c40a6d66437
workflow-type: tm+mt
source-wordcount: '1857'
ht-degree: 0%

---

# 텍스트 모드 구문 개요

텍스트 모드 인터페이스를 사용하여 목록 및 보고서에서 보다 복잡한 보기, 필터, 그룹화 및 사용자 지정된 프롬프트를 만들 수 있습니다. 텍스트 모드를 사용하면 표준 모드 인터페이스에서 사용할 수 없는 필드 및 해당 속성에 액세스할 수 있습니다.

시작하기 전에 텍스트 모드에 대한 정보 및 고려 사항은 다음을 참조하십시오. [텍스트 모드 개요](../../../reports-and-dashboards/reports/text-mode/understand-text-mode.md).

보고 가능한 모든 필드와 해당 속성에 대한 전체 목록은 다음을 참조하십시오. [API 탐색기](../../../wf-api/general/api-explorer.md).

클래스, 비디오 및 튜토리얼을 포함하여 텍스트 모드를 사용하여 보고서를 만드는 방법에 대한 자세한 내용은 Adobe Experience League 사이트의 학습 섹션을 참조하십시오.

## 텍스트 모드 구문에 대한 고려 사항

* 텍스트 모드에서 보고 요소 작성을 시작하려면 Adobe Workfront 구문을 이해해야 합니다. 텍스트 모드의 Workfront 구문은 이 애플리케이션에 고유하며 익숙해야 하는 고유한 특성을 가집니다.
* 보고서에서 텍스트 모드를 사용하기 전에 텍스트 모드 언어를 더 깊이 있게 이해할 수 있도록 고급 보고에 대한 강의를 수강하는 것이 좋습니다. <!--outdated link: For training materials on reporting see [Workfront Reports and Dashboards Learning Paths](https://one.workfront.com/s/learningpath2/workfront-reporting-20Y0z000000blhLEAQ).-->
* 표준 모드 인터페이스를 사용하여 보기, 필터 및 그룹화를 사용자 지정할 수 있습니다. 하지만 텍스트 모드만 사용하여 사용자 정의 프롬프트를 작성할 수 있습니다.

## 텍스트 모드에서 보고 요소를 작성하기 위한 일반적인 지침

다음은 텍스트 모드에서 보고 또는 목록 요소를 작성할 때의 일반적인 지침입니다.

* Workfront 데이터베이스의 개체 또는 특성을 참조할 때는 항상 카멜 표식을 사용하십시오.
* Workfront의 개체 계층 구조를 염두에 두십시오. 보기, 필터 및 그룹화 사이에는 다음과 같은 차이가 있습니다.

   * 뷰에서 보고서나 목록 객체에서 멀리 떨어진 세 개의 객체를 표시할 수 있습니다.
   * 그룹화, 필터 또는 사용자 지정 프롬프트에서 주 개체와 2개 이상의 개체를 참조할 수 없습니다.

  **예:** 작업 보기에 Portfolio 소유자의 이름 또는 GUID를 표시할 수 있습니다.


  `valuefield=project:portfolio:ownerID`

  작업 보기에서 Portfolio 소유자를 그룹화하거나 필터링하거나 프롬프트를 표시할 수 없습니다.

  `project:portfolio:ownerID=5808f4bc00790b270a9629dd128e63fa`


  이러한 예에서 Portfolio 소유자 ID는 목록의 객체에서 3개의 객체입니다.

  Workfront의 개체 계층 구조에 대한 자세한 내용은 다음을 참조하십시오.

   * [Adobe Workfront의 오브젝트 이해](../../../workfront-basics/navigate-workfront/workfront-navigation/understand-objects.md)
   * [API 탐색기](../../../wf-api/general/api-explorer.md)

* 가능한 경우 언제든지 와일드카드를 사용하여 보고서와 목록을 보다 동적이고 다양한 사용자 및 유사한 타임라인에 대해 중복을 피하십시오.

## 카멜 대/소문자 개요

텍스트 모드에서 Workfront 필드 또는 해당 속성을 참조할 때 Workfront에서는 카멜 표기법으로 해당 이름을 입력해야 합니다. 이 경우 단일 이름 필드는 소문자로 입력됩니다. 컴파운드 필드의 맞춤법은 다음 패턴에 따라 결정됩니다.

`camelCaseSyntax`

>[!IMPORTANT]
>
>모든 보고 요소는 이 케이싱 패턴을 따릅니다.

낙타 사례의 특징은 다음과 같습니다.

* 첫 번째 단어는 항상 소문자로 시작합니다.
* 다음 단어는 항상 대문자로 시작합니다.
* 단어 사이에 공백이 없습니다.

**예:** 프로젝트의 실제 완료 일자를 참조하기 위해 텍스트 모드 보고 요소를 작성할 때 사용할 필드의 이름은 입니다.

`actualCompletionDate`

## 다양한 보고 요소의 텍스트 모드 구문

텍스트 모드를 사용하여 생성할 때 아래 보고 요소 세트의 구문 사이에는 다음과 같은 유사성이 있습니다.

* 코드 및 구문 행은 보기 및 그룹화에서 유사합니다.

  텍스트 모드에서 뷰 및 그룹화를 작성할 때의 코드 키 행에 대한 자세한 내용은 다음을 참조하십시오.

   * [텍스트 모드를 사용하여 보기 편집](../../../reports-and-dashboards/reports/text-mode/edit-text-mode-in-view.md)
   * [그룹화에서 텍스트 모드 편집](../../../reports-and-dashboards/reports/text-mode/edit-text-mode-in-grouping.md)

* 코드 및 구문 행은 필터 및 사용자 지정 프롬프트에 대해 유사합니다.

  자세한 내용은 다음을 참조하십시오.

   * [텍스트 모드를 사용하여 필터 편집](../../../reports-and-dashboards/reports/text-mode/edit-text-mode-in-filter.md)
   * [보고서에 프롬프트 추가](../../../reports-and-dashboards/reports/creating-and-managing-reports/add-prompt-report.md)

### 보기 및 그룹화 구문

보기와 그룹화를 작성할 때 코드 줄이 비슷하다는 것을 알 수 있습니다.

보기 및 그룹화 만들기에 대한 자세한 내용은 다음 문서를 참조하십시오.

* [Adobe Workfront의 보기 개요](../../../reports-and-dashboards/reports/reporting-elements/views-overview.md)
* [Adobe Workfront의 그룹화 개요](../../../reports-and-dashboards/reports/reporting-elements/groupings-overview.md)

뷰 또는 그룹화에 대한 가장 중요한 코드 행은 뷰의 열 또는 그룹화에서 참조된 객체를 식별하는 행입니다. 이 필드가 Workfront 데이터베이스 필드에 대한 직접 참조인지 또는 여러 필드 간의 계산인지에 따라 코드 줄이 다음으로 시작될 수 있습니다. `valuefield` 또는 `valueexpression`

다음 표에는 뷰 또는 그룹화에서 가장 일반적인 코드 행이 나열되어 있습니다.

| 코드 라인 | 설명 |
|-----------------|------------------------------------------------------------------------------------------------------------------------------|
| `valuefield` | 보기의 열이나 그룹화에 참조된 개체를 식별합니다. 참조된 개체에 대한 직접 참조입니다. |
| `valueexpression` | 보기의 열이나 그룹화에 참조된 개체를 식별합니다. 여러 필드 간의 계산입니다. |
| `valueformat` | Workfront이 valuefield 또는 valueexpression 행에 지정된 값을 반환하는 형식을 식별합니다. |
| `width` | 열의 너비를 픽셀 단위로 식별합니다. |
| `stretch` | 보기에서 필요하지 않은 추가 공간을 차지하는 열을 식별합니다. |

>[!TIP]
>
>* 아래 예제의 코드 행은 보기 수와 그룹화 간에 유사하지만 그룹화에 대한 모든 코드 행은 그룹화 번호로 시작한다는 것을 항상 기억하십시오.
>
>  프로젝트 목록 또는 보고서에서 프로젝트 이름별로 그룹화하려면 첫 번째 계층 그룹화에 대해 다음 줄을 사용하십시오.
>
>  `group.0.valuefield=name`
>  
>* 공유 열의 경우와 마찬가지로 동일한 열의 보기에서 여러 열을 편집하는 경우 각 열의 모든 코드 행은 열 번호로 시작합니다.
>
>  다음 형식을 사용하여 보기의 첫 번째 열을 식별합니다.
>
>  `column.0.valuefield=name`
>  
>  열 공유에 대한 자세한 내용은 [보기: 여러 열의 정보를 하나의 공유 열에 병합](../../../reports-and-dashboards/reports/custom-view-filter-grouping-samples/view-merge-columns.md).
>

#### `Valuefield` 보기 및 그룹화에 대한 구문 개요

`Valuefield=` 는 직접 참조하는 개체를 식별하는 보기 및 그룹화의 주요 코드 행입니다.

필드를 직접 참조하는 구문은 그룹화 및 보기에 대해 동일합니다.

다음을 사용하여 Workfront 개체를 참조할 때 다음 규칙이 적용됩니다 `valuefield` 줄:

* 필드를 직접 참조하려면 카멜 표식을 사용하십시오.

  **예:** 태스크 뷰에서 태스크 실제 완료 일자를 참조하려면 다음 라인을 사용합니다.

  `valuefield=actualCompletionDate`

* 카멜 대/소문자와 콜론을 사용하여 동일한 오브젝트에 대해 서로 관련된 필드를 구분합니다.

  **예:** 작업 보기에서 프로젝트 계획 완료 일자를 참조하려면 다음 라인을 사용합니다.

  `valuefield=project:plannedCompletionDate`

  개체가 Workfront 데이터베이스에서 서로 참조하는 방법에 대한 자세한 내용은 [API 탐색기](../../../wf-api/general/api-explorer.md).

* 사용자 정의 필드를 참조할 때는 인터페이스에 표시되는 것과 정확히 동일한 필드의 이름을 사용하십시오.

  **예:** 작업 보기에서 추가 세부 정보 레이블이 지정된 프로젝트 사용자 정의 필드를 참조하려면 다음 줄을 사용하십시오.

  `valuefield=project:Additional Details`

#### `Valueexpression` 보기 및 그룹화에 대한 구문 개요

다음을 바꿀 수 있습니다. `valuefield=` 코드 줄 포함 `valueexpression=` 텍스트 모드에서 보기 및 그룹화를 작성할 때 2개 이상의 필드 간에 계산을 참조하려는 경우.

>[!TIP]
>
>보고서에 표시할 수 있는 계산된 필드를 작성할 수 있지만 계산된 보기 및 그룹화는 더 동적입니다. 보고서를 실행하거나 목록을 표시할 때마다 계산된 보기 및 그룹화가 새 정보로 새로 고쳐집니다.
>
>뷰에서 계산된 열을 만드는 방법에 대한 자세한 내용은 [계산된 사용자 정의 필드와 계산된 열 비교](../../../reports-and-dashboards/reports/calc-cstm-data-reports/calculated-custom-fields-calculated-columns.md).

계산된 그룹화를 작성하는 것은 뷰에서 계산된 열을 작성하는 것과 비슷합니다.

다음을 사용하여 Workfront 개체를 참조할 때 다음 규칙이 적용됩니다 `valueexpression` 줄:

* 필드를 직접 참조하고 각 필드를 중괄호로 묶으려면 카멜 대/소문자를 사용하십시오.

  **예:** 다음을 사용하여 작업 열에 작업 이름 필드를 표시하려면 `valueexpression`, 다음 줄을 사용하십시오.

  `valueexpression={name}`


* 카멜 대/소문자와 마침표를 사용하여 서로 관련된 필드를 구분합니다.

  **예:** 작업 보고서에 작업 이름과 연결된 프로젝트 이름을 표시하려면 다음 줄을 사용합니다.

   * 보기에서:

     `valueexpression=CONCAT({project}.{name},' - ',{name})`

   * 그룹화:

     `group.0.valueexpression=CONCAT({project}.{name},' - ',{name})`

  개체가 Workfront 데이터베이스에서 서로 참조하는 방법에 대한 자세한 내용은 [API 탐색기](../../../wf-api/general/api-explorer.md).

* 사용자 정의 필드를 참조할 때 다음 규칙을 사용합니다.

   * 인터페이스에 표시되는 것과 정확히 동일한 필드 이름을 사용합니다.
   * 필드 이름 앞에 &quot;DE:&quot;를 붙입니다.
   * 필드를 중괄호로 묶습니다.
   * 객체와 관련된 필드를 마침표로 구분합니다.

  **예:** Valueexpression 라인의 작업 보기에 추가 세부 정보 프로젝트 사용자 정의 필드를 표시하려면 다음 줄을 사용하십시오.

  `valueexpression={project}.{DE:Additional Details}`

* 다음에서 와일드카드를 사용할 수 있습니다. `valueexpression` 그러나 에는 없습니다. `valuefield` 줄.

  와일드카드에 대한 자세한 내용은 [와일드카드 필터 변수](../../../reports-and-dashboards/reports/reporting-elements/understand-wildcard-filter-variables.md).


#### `Valueformat` 보기 및 그룹화 개요

보기 또는 그룹화에서 두 번째로 중요한 코드 행은 `valueformat=` 줄. 이것은 Workfront에 지정하는 값을 반환할 형식을 알려줍니다.
`valuefield` 또는 valueexpression 행입니다. 에 다양한 형식을 사용할 수 있지만 `valueformat` 행, 을 사용할 때는 항상 다음 값을 사용하는 것이 좋습니다
`valueexpression`:

`valueformat=HTML`

추가 `valueformats` 값은 다음 문서를 참조하십시오.

* [텍스트 모드 보고서에서 날짜 형식 지정](../../reports/text-mode/format-dates-in-text-mode-reports.md)
* [텍스트 모드 보고서에서 숫자, 통화 및 백분율 값 서식 지정](../../reports/text-mode/format-numbers-in-text-mode-reports.md)

#### `width` 보기에 대한 개요

`width=` 는 각 열의 너비를 픽셀 단위로 지정할 수 있는 코드 행입니다. Workfront에서는 각 필드에 대해 제안된 너비를 제공하지만 필드 유형과 형식에 따라 조정할 수 있습니다.

추가 항목을 사용해야 합니다. `usewidths=true` 열에 지정된 너비를 적용하는 코드 줄입니다.

**예:** 너비가 80픽셀인 열을 표시하려면 다음 줄을 사용합니다.

`width=80`

`usewidths=true`

#### `stretch` 보기에 대한 개요

다음 `stretch` 는 보기에서 필요하지 않은 추가 공간을 차지하는 열을 식별하는 데 사용됩니다. 일반적인 사용자를 위한 작업 영역의 사용자 인터페이스 폭은 약 850픽셀이다. 즉, 보기가 850픽셀 중 600픽셀을 차지하는 4개의 열(각각 150픽셀)이 있는 보기입니다. UI에 250개의 추가 픽셀이 있으며, 이 픽셀은 스트레치 비율이 제공된 열에 추가됩니다.

추가 코드 행을 사용하면 열 스트레치가 적용됩니다. `usewidths=true` 뷰에 있는 하나 이상의 열에 대해 설명합니다.

**예:** 열에 보기에서 빈 공간의 70%를 사용할 수 있음을 나타내려면 다음 줄을 사용합니다.

`stretch=70`

`usewidths=true`

### 필터 및 사용자 지정 프롬프트 구문

필터를 만드는 구문은 사용자 지정 프롬프트를 만드는 구문과 유사합니다.

>[!TIP]
>
>먼저 프롬프트에 포함할 문에 대한 필터를 빌드하여 사용자 지정 프롬프트를 만들 수 있습니다. &quot;&amp;&quot;를 기준으로 필터에 있는 모든 코드 줄을 줄 사이에 공백 없이 연결하여 사용자 정의 프롬프트가 됩니다.

필터 빌드 및 사용자 지정 프롬프트에 대한 자세한 내용은 다음을 참조하십시오.

* [Adobe Workfront의 필터 개요](../../../reports-and-dashboards/reports/reporting-elements/filters-overview.md)
* [보고서에 프롬프트 추가](../../../reports-and-dashboards/reports/creating-and-managing-reports/add-prompt-report.md)

텍스트 모드에서 필터를 만드는 방법에 대한 자세한 내용은 [텍스트 모드를 사용하여 필터 편집](../../../reports-and-dashboards/reports/text-mode/edit-text-mode-in-filter.md).

다음 요소를 사용하여 텍스트 모드에서 필터와 사용자 지정 프롬프트를 작성할 수 있습니다.

* 필터 문의 개체를 참조하는 코드 줄입니다. 필터 개체에 카멜 대/소문자를 사용합니다.
* 필터 개체 및 필터 개체의 값에 대한 수정자를 참조하는 코드 줄입니다. 이 줄의 필터 개체에 대해 카멜 표식을 사용하십시오.

  >[!TIP]
  >
  >범위를 참조할 때 2개의 수정자 라인이 필요합니다.

* 여러 필터 문을 연결하는 문 커넥터:

   * 및

     필터 문 사이의 기본 커넥터입니다.

   * 또는

     >[!TIP]
     >
     >문 커넥터는 대소문자를 구분하며 항상 대문자입니다. 텍스트 모드에서 &quot;AND&quot;를 생략할 수 있습니다.

* 필터를 보다 동적으로 만들고 현재 시간 또는 로그인한 사용자에 대해 사용자 지정하는 와일드카드. 와일드카드에 대한 자세한 내용은 [와일드카드 필터 변수](../../../reports-and-dashboards/reports/reporting-elements/understand-wildcard-filter-variables.md).
