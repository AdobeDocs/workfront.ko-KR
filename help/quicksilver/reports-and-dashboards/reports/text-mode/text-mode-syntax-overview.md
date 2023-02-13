---
product-area: reporting
navigation-topic: text-mode-reporting
title: 텍스트 모드 구문 개요
description: 텍스트 모드 인터페이스를 사용하여 목록 및 보고서에서 더 복잡한 보기, 필터, 그룹화 및 사용자 지정 프롬프트를 만들 수 있습니다. 텍스트 모드를 사용하면 표준 모드 인터페이스에서 사용할 수 없는 필드 및 속성에 액세스할 수 있습니다.
author: Nolan
feature: Reports and Dashboards
exl-id: f24430e1-c5f7-4925-93df-0e956a03c863
source-git-commit: 54f4c136cfaaaaaa90a4fc64d3ffd06816cff9cb
workflow-type: tm+mt
source-wordcount: '1498'
ht-degree: 0%

---

# 텍스트 모드 구문 개요

텍스트 모드 인터페이스를 사용하여 목록 및 보고서에서 더 복잡한 보기, 필터, 그룹화 및 사용자 지정 프롬프트를 만들 수 있습니다. 텍스트 모드를 사용하면 표준 모드 인터페이스에서 사용할 수 없는 필드 및 속성에 액세스할 수 있습니다.

시작하기 전에 텍스트 모드에 대한 정보 및 고려 사항은 [텍스트 모드 개요](../../../reports-and-dashboards/reports/text-mode/understand-text-mode.md).

모든 보고 가능 필드 및 해당 속성의 전체 목록은 [API 탐색기](../../../wf-api/general/api-explorer.md).

## 텍스트 모드 구문에 대한 고려 사항

* 텍스트 모드에서 보고 요소 작성을 시작하려면 먼저 Adobe Workfront 구문을 이해해야 합니다. 텍스트 모드에 대한 Workfront 구문은 이 응용 프로그램에 고유하며 익숙해야 하는 고유한 특성이 있습니다.
* 보고서에서 텍스트 모드를 사용하기 전에 고급 보고에 대한 클래스를 수강하여 텍스트 모드 언어를 더 잘 이해할 것을 강력히 권장합니다. 보고에 대한 교육 자료는 [Workfront 보고서 및 대시보드 학습 경로](https://one.workfront.com/s/learningpath2/workfront-reporting-20Y0z000000blhLEAQ).
* 표준 모드 인터페이스를 사용하여 보기, 필터 및 그룹화를 사용자 지정할 수 있습니다. 그러나 텍스트 모드만 사용하여 사용자 정의 프롬프트를 작성할 수 있습니다.

## 텍스트 모드에서 보고 요소를 빌드하기 위한 일반적인 지침

다음은 텍스트 모드에서 보고 또는 목록 요소를 작성할 때의 일반적인 지침입니다.

* Workfront 데이터베이스의 개체나 특성을 참조할 때에는 항상 카멜 표기법을 사용하십시오.
* Workfront에서 개체의 계층 구조를 기억하십시오. 보기, 필터 및 그룹화 간에 다음과 같은 차이가 있습니다.

   * 한 보기에서 보고서 또는 목록 객체에서 떨어져 있는 객체를 표시할 수 있습니다.
   * 그룹화, 필터 또는 사용자 정의 프롬프트에서 기본 객체로부터 2개 이상의 개체를 참조할 수 없습니다.

   **예:** 작업 보기에 Portfolio 소유자의 이름 또는 GUID를 표시할 수 있습니다.

   ```
   valuefield=project:portfolio:ownerID
   ```

   작업 보기에서 Portfolio 소유자를 그룹화, 필터링 또는 표시할 수 없습니다.

   ```
   project:portfolio:ownerID=5808f4bc00790b270a9629dd128e63fa
   ```

   이러한 예에서 Portfolio 소유자 ID는 목록 객체에서 세 개의 객체입니다.

   Workfront의 객체 계층에 대한 자세한 내용은 다음을 참조하십시오.

   * [Adobe Workfront의 개체 이해](../../../workfront-basics/navigate-workfront/workfront-navigation/understand-objects.md)
   * [API 탐색기](../../../wf-api/general/api-explorer.md)


* 가능한 경우 와일드카드를 사용하여 보고서를 동적으로 만들고 목록이 다른 사용자 및 유사한 타임라인에 대해 중복되지 않도록 합니다.

## 카멜 사례 개요

텍스트 모드에서 Workfront 필드 또는 해당 속성을 참조할 때 Workfront에서 해당 이름을 카멜 표기법으로 입력해야 합니다. 이 경우 단일 이름 필드의 맞춤은 소문자로 표시됩니다. 복합 필드는 다음 패턴에 따라 맞춤됩니다.

```
camelCaseSyntax
```

>[!IMPORTANT]
>
>모든 보고 요소는 이 케이싱 패턴을 따릅니다.

낙타 케이스의 특징은 다음과 같습니다.

* 첫 번째 단어는 항상 소문자로 시작합니다.
* 다음 단어는 항상 대문자로 시작합니다.
* 단어 사이에 공백이 없습니다.

**예:** 프로젝트의 실제 완료 날짜를 참조하려면 텍스트 모드 보고 요소를 작성할 때 사용할 필드의 이름이 입니다

```
actualCompletionDate
```

.

## 다양한 보고 요소에 대한 텍스트 모드 구문

텍스트 모드를 사용하여 보고 요소를 만들 때 아래 보고 요소 세트의 구문 간에 다음과 같은 유사성이 있습니다.

* 코드 및 구문 줄은 보기 및 그룹화에 대해 유사합니다.

   텍스트 모드에서 보기 및 그룹화를 작성할 때의 코드 주요 줄에 대한 자세한 내용은 다음을 참조하십시오.

   * [텍스트 모드를 사용하여 보기 편집](../../../reports-and-dashboards/reports/text-mode/edit-text-mode-in-view.md)
   * [그룹화 시 텍스트 모드 편집](../../../reports-and-dashboards/reports/text-mode/edit-text-mode-in-grouping.md)

* 코드 및 구문 줄은 필터 및 사용자 지정 프롬프트에 유사합니다.

   자세한 내용은 다음을 참조하십시오.

   * [텍스트 모드를 사용하여 필터 편집](../../../reports-and-dashboards/reports/text-mode/edit-text-mode-in-filter.md)
   * [보고서에 프롬프트 추가](../../../reports-and-dashboards/reports/creating-and-managing-reports/add-prompt-report.md)

### 보기 및 그룹화에 대한 구문

보기 및 그룹화를 작성할 때의 코드 줄이 비슷하다는 것을 알 수 있습니다.

보기 및 그룹화를 만드는 방법에 대한 자세한 내용은 다음 문서를 참조하십시오.

* [Adobe Workfront의 보기 개요](../../../reports-and-dashboards/reports/reporting-elements/views-overview.md)
* [Adobe Workfront의 그룹화 개요](../../../reports-and-dashboards/reports/reporting-elements/groupings-overview.md)

보기나 그룹화에 가장 중요한 코드 줄은 뷰의 열 또는 그룹화에서 참조되는 개체를 식별하는 라인입니다. 이 필드가 Workfront 데이터베이스 필드에 대한 직접 참조인지 또는 여러 필드 간의 계산인지에 따라 코드 행이 다음으로 시작될 수 있습니다.

```
valuefield
```

또는

```
valueexpression
```

.

* [보기 및 그룹화에 대한 값 필드 구문 개요](#valuefield-syntax-overview-for-views-and-groupings)
* [보기 및 그룹화에 대한 값 표현식 구문 개요](#valueexpression-syntax-overview-for-views-and-groupings)

>[!TIP]
>
>* 아래 예제의 코드 행은 보기와 그룹화 간에 유사하지만 그룹화 방법에 대한 모든 코드 줄은 항상 그룹화 번호로 시작됩니다.
>
>  프로젝트 목록이나 보고서에서 프로젝트 이름별로 그룹화하려면 첫 번째 계층 그룹화에 다음 라인을 사용합니다.
>
>  
```>
>  group.0.valuefield=name
>  ```>
>* If you edit multiple columns in a view in the same column (as it is the case of shared columns), remember that every line of code for each column starts with the column number. 
>
>  
Use the following format to identify the first column of a view: 
>
>  
```>
>  column.0.valuefield=name
>  ```>
>  For information about sharing columns, see [View: merge information from multiple columns in one shared column](../../../reports-and-dashboards/reports/custom-view-filter-grouping-samples/view-merge-columns.md). 
>



```
Valuefield
```

보기 및 그룹화에 대한 구문 개요 {#valuefield-syntax-overview-for-views-and-groupings}

```
Valuefield=
```

는 직접 참조하는 개체를 식별하는 보기 및 그룹의 코드 핵심 줄입니다.

필드를 직접 참조하는 구문은 그룹화 및 보기에 대해 동일합니다.

다음 규칙은

```
valuefield
```

줄:

* 필드를 직접 참조하려면 카멜 케이스를 사용하십시오.

   **예:** 태스크 뷰에서 태스크 실제 완료 일자를 참조하려면 다음 라인을 사용합니다.

   ```
   valuefield=actualCompletionDate
   ```

* 동일한 개체에 대해 서로 관련된 필드를 구분하려면 카멜 케이스 및 콜론을 사용하십시오.

   **예:** 태스크 뷰에서 프로젝트 계획 완료 일자를 참조하려면 다음 라인을 사용합니다.

   ```
   valuefield=project:plannedCompletionDate
   ```

   Workfront 데이터베이스에서 개체가 서로 참조하는 방법에 대한 자세한 내용은 [API 탐색기](../../../wf-api/general/api-explorer.md).

* 사용자 지정 필드를 참조할 때 인터페이스에 표시된 대로 필드의 이름을 사용합니다.

   **예:** 작업 보기에서 추가 세부 정보라는 프로젝트 사용자 지정 필드를 참조하려면 다음 행을 사용하십시오.

   ```
   valuefield=project:Additional Details
   ```

 

```
Valueexpression
```

보기 및 그룹화에 대한 구문 개요 {#valueexpression-syntax-overview-for-views-and-groupings}

을 대체할 수 있습니다

```
valuefield=
```

코드 줄

```
valueexpression=
```

둘 이상의 필드 사이의 계산을 참조하려는 경우 텍스트 모드에서 보기 및 그룹화를 작성할 때.

>[!TIP]
>
>보고서에 표시할 수 있는 계산된 필드를 작성할 수 있지만 계산된 보기 및 그룹화는 더 동적입니다. 보고서를 실행하거나 목록을 표시할 때마다 계산된 보기 및 그룹화가 새로운 정보로 새로 고침됩니다.
>
>보기에서 계산된 열 만들기에 대한 자세한 내용은 [계산된 사용자 지정 필드와 계산된 열](../../../reports-and-dashboards/reports/calc-cstm-data-reports/calculated-custom-fields-calculated-columns.md).

계산된 그룹을 작성하는 것은 보기에서 계산된 열을 작성하는 것과 비슷합니다.

다음 규칙은

```
valueexpression
```

줄:

* 카멜 대/소문자를 사용하여 필드를 직접 참조하고 각 필드를 중괄호로 묶습니다.

   **예:** 작업 열에 작업 이름 필드를 표시하려면

   ```
   valueexpression
   ```

   를 채울 때는 다음 줄을 사용하십시오.

   ```
   valueexpression={name}
   ```

* 서로 관련된 필드를 구분하려면 카멜 표기법 및 마침표를 사용하십시오.

   **예:** 작업 보고서에서 작업 이름과 연결된 프로젝트의 이름을 표시하려면 다음 행을 사용하십시오.

   * 보기에서:

      ```
      valueexpression=CONCAT({project}.{name},' - ',{name})
      ```

   * 그룹화:

      ```
      group.0.valueexpression=CONCAT({project}.{name},' - ',{name})
      ```
   Workfront 데이터베이스에서 개체가 서로 참조하는 방법에 대한 자세한 내용은 [API 탐색기](../../../wf-api/general/api-explorer.md).

* 사용자 지정 필드를 참조할 때에는 다음 규칙을 사용하십시오.

   * 인터페이스에 표시되는 필드의 이름을 그대로 사용합니다.
   * 필드의 이름 앞에 &quot;DE:&quot;를 입력합니다.
   * 필드를 중괄호로 묶습니다.
   * 개체와 관련된 필드를 마침표로 구분합니다.

   **예:** 값 표현식 라인의 작업 뷰에 추가 세부 정보 프로젝트 사용자 정의 필드를 표시하려면 다음 라인을 사용합니다.

   ```
   valueexpression={project}.{DE:Additional Details}
   ```

* 와일드카드를 사용할 수 있습니다

   ```
   valueexpression
   ```

   하지만

   ```
   valuefield
   ```

   줄.

   와일드카드에 대한 자세한 내용은 [와일드카드 필터 변수](../../../reports-and-dashboards/reports/reporting-elements/understand-wildcard-filter-variables.md).

```
Valueformat
```

개요

보기 또는 그룹에서 두 번째로 중요한 코드 줄은 다음과 같습니다

```
valueformat=
```

줄. 이렇게 하면 Workfront에서 지정한 값을 반환할 형식으로 표시됩니다.

```
valuefield
```

또는 값 표현식 라인. 다양한 형식의

```
valueformat
```

라인,

```
valueexpression
```

:

```
valueformat=HTML
```

### 필터 및 사용자 지정 프롬프트 구문

필터를 만드는 구문은 사용자 정의 프롬프트를 만드는 구문과 유사합니다.

>[!TIP]
>
>먼저 프롬프트에 포함할 문에 대한 필터를 작성하여 사용자 지정 프롬프트를 생성할 수 있습니다. 줄 사이의 공백 없이 &quot;&amp;&quot;로 필터에 있는 모든 코드 줄을 사용자 지정 프롬프트가 되는 방식으로 연결합니다.

필터 작성 및 사용자 정의 프롬프트에 대한 자세한 내용은 다음을 참조하십시오.

* [Adobe Workfront의 필터 개요](../../../reports-and-dashboards/reports/reporting-elements/filters-overview.md)
* [보고서에 프롬프트 추가](../../../reports-and-dashboards/reports/creating-and-managing-reports/add-prompt-report.md)

텍스트 모드에서 필터 만들기에 대한 내용은 [텍스트 모드를 사용하여 필터 편집](../../../reports-and-dashboards/reports/text-mode/edit-text-mode-in-filter.md).

다음 요소를 사용하여 텍스트 모드에서 필터 및 사용자 정의 프롬프트를 작성할 수 있습니다.

* filter 문의 개체를 참조하는 코드 줄 필터 개체에 Camel 대/소문자를 사용하십시오.
* 필터 개체 및 필터 개체 값의 한정자를 참조하는 코드 줄. 이 행의 필터 개체에 대해 카멜 표기법을 사용하십시오.

   >[!TIP]
   >
   >범위를 참조할 때는 2개의 수정자 라인이 필요합니다.

* 여러 필터 문을 연결하는 문 커넥터입니다.

   * 및

      필터 문 간의 기본 커넥터입니다.

   * 또는

      >[!TIP]
      >
      >문 커넥터는 대/소문자를 구분하며 항상 대문자입니다. &quot;AND&quot;는 텍스트 모드에서 생략할 수 있습니다.

* 필터를 보다 동적으로 만들고 현재 시간 또는 로그인한 사용자에 대해 사용자 지정하는 와일드카드를 사용할 수 있습니다. 와일드카드에 대한 자세한 내용은 [와일드카드 필터 변수](../../../reports-and-dashboards/reports/reporting-elements/understand-wildcard-filter-variables.md).
