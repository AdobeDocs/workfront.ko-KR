---
content-type: overview
product-area: reporting
navigation-topic: calculate-custom-data-reports
title: IF 문 개요
description: 일반 프로그래밍 언어에서 "IF" 문을 사용할 수 있습니다. Adobe Workfront에서 "IF" 문을 사용하면 보고 및 사용자 지정 데이터 목적을 위해 데이터 필드를 비교, 서식 지정 및 함께 문자열이 될 수 있습니다. 또한, "IF" 문에 대해 수학적으로 생각하는 것은 표현식에 대한 변수가 일반적으로 사용되므로 더 나은 개념적 이해로 이어집니다.
author: Nolan
feature: Reports and Dashboards
exl-id: 090a85fd-fdbe-4507-8bad-ce8c29bf8fc9
source-git-commit: 54f4c136cfaaaaaa90a4fc64d3ffd06816cff9cb
workflow-type: tm+mt
source-wordcount: '928'
ht-degree: 0%

---

# &quot;IF&quot; 문 개요

일반 프로그래밍 언어에서 &quot;IF&quot; 문을 사용할 수 있습니다. Adobe Workfront에서 &quot;IF&quot; 문을 사용하면 보고 및 사용자 지정 데이터 목적을 위해 데이터 필드를 비교, 서식 지정 및 함께 문자열이 될 수 있습니다. 또한, &quot;IF&quot; 문에 대해 수학적으로 생각하는 것은 표현식에 대한 변수가 일반적으로 사용되므로 더 나은 개념적 이해로 이어집니다.

## &quot;IF&quot; 문에 대한 Recommendations

&quot;IF&quot; 문을 만들기 전에 다음 사항을 고려하십시오.

* 일반적인 프로그래밍 언어에 대한 기본적인 이해를 권장하지만 이 안내서에서는 필요하지 않습니다.
* Workfront 텍스트 모드 구문에 대한 고급 이해가 필요합니다. 이렇게 하면 Workfront API의 용어를 이해하고 이러한 특정 형식의 사용자 지정 데이터 구문을 이해하는 데 도움이 됩니다.

   Workfront API에 대한 자세한 내용은 [API 기본 사항](../../../wf-api/general/api-basics.md).

   텍스트 모드 사용에 대한 자세한 내용은 [텍스트 모드 개요](../../../reports-and-dashboards/reports/text-mode/understand-text-mode.md).

* 다음 Workfront 요소에 대해 &quot;IF&quot; 문을 작성할 수 있습니다.

   * 조회수
   * 그룹화
   * 계산된 사용자 지정 필드

* 필터에 대해 &quot;IF&quot; 문을 작성할 수 없습니다. 이로 인해 Workfront에 &quot;Whoops&quot; 오류가 발생합니다.
* 지원 팀은 사용자 지정 데이터를 작성하는 데 도움이 되지 않습니다. 사용자 지정 필드 또는 열을 작성하고 원하는 결과가 표시되지 않으면 지원 팀에 문의할 수 있습니다. 표현식을 작성하는 데 도움이 필요하면 계정 담당자에게 연락하여 컨설팅 옵션에 대해 문의하십시오.
* 이렇게 하면 Workfront에 나타나는 것보다 데이터를 보다 명확하게 볼 수 있으므로 Giabliant 또는 Visual Studio Code와 같이 텍스트 편집기에 이러한 표현식을 먼저 작성하는 것이 좋습니다.

## &quot;IF&quot; 문의 구성 요소

다음 형식을 사용하여 Workfront에서 &quot;IF&quot; 문을 작성할 수 있습니다.
<pre>IF(Condition,True 표현식,False 표현식)</pre>"IF" 문의 구성 요소는 다음과 같습니다.

* **IF**= &quot;함수&quot;에 대한 Workfront 계산된 데이터 표현식입니다. SUM 및 PROD 표현식과 마찬가지로, 먼저 함수를 &quot;IF&quot; 문으로 이해하도록 시스템에 지시합니다. 이 문에서 항상 &quot;IF&quot;에 대문자를 사용하십시오.\
   모든 계산된 데이터 표현식 목록이 필요하면 를 참조하십시오 [계산된 데이터 표현식](../../../reports-and-dashboards/reports/calc-cstm-data-reports/calculated-data-expressions.md).

* **조건**= Workfront 변수가 충족되어야 하는 조건이며 이 방정식의 기반입니다. 나중에 방정식에서 지정할 수 있는 모든 것은 조건에 따라 다릅니다. 여러 참조, 비교 또는 수학 표현식을 사용하여 방정식을 시작할 수 있습니다. 조건의 일부 예는 다음과 같습니다.

   * 날짜가 지정된 개체의 다른 날짜보다 큽니다.
   * 상태는 지정된 개체에서 사용 가능한 상태 중 하나와 같습니다.
   * 작업의 완료율이 특정 백분율보다 작거나 같습니다.

* **조건 연산자** = &quot;IF&quot; 문의 조건을 작성하는 데 도움이 되는 연산자입니다. 예를 들어 &quot;is equal to&quot; 또는 &quot;is greater than&quot;은 조건 연산자입니다. 문에서 사용할 수 있는 조건 연산자 목록은 다음을 참조하십시오 [계산된 사용자 지정 표현식의 조건 연산자](../../../reports-and-dashboards/reports/calc-cstm-data-reports/condition-operators-calculated-custom-expressions.md).

* **True****Expression**= &quot;True&quot; 변수입니다. 이 변수는 조건의 기준이 충족되면 표시할 지표(true 지표)를 지정합니다.

* **False 표현식**= &quot;False&quot; 변수입니다. 이 변수는 조건의 기준이 충족되지 않을 때 표시할 지표를 지정합니다(false 표시기).

다음 예제에서 원래 문 형식은 &quot;IF&quot; 문에 대해 간단한 데이터 표현식을 작성하는 데 사용됩니다. 표현식은 Workfront의 두 개의 서로 다른 날짜 필드를 비교하고 True/False 결과를 데이터 문자열로 비교합니다.

```
IF({projectedCompletionDate}>{plannedCompletionDate},"Off Track","On Track")
```

매일 하는 연설에서, 이 진술은 다음을 의미할 것입니다. 내 객체의 예상 완료 일자가 동일한 객체의 계획 완료 일자에서 &quot;보다 큼&quot;인 경우 이 필드에 &quot;Off Track&quot;이라는 단어를 표시합니다. 없는 경우 &quot;On Track&quot;이라는 단어를 표시합니다.

## &quot;IF&quot; 문을 사용하여 사용자 지정 양식 또는 사용자 지정 열에 계산된 필드를 작성합니다

사용자 지정 양식 또는 사용자 지정 열의 계산된 필드에 &quot;IF&quot; 문을 작성할 수 있습니다.

계산된 사용자 지정 양식에서 사용하는 구문과 계산된 사용자 지정 열에서 차이가 있습니다. 다음 예를 참조하십시오.

* [단일 &quot;IF&quot; 문](#single-if-statements)
* [여러 &quot;IF&quot; 문](#multiple-if-statements)

### 단일 &quot;IF&quot; 문 {#single-if-statements}

다음은 &quot;IF&quot; 문을 사용하는 계산된 사용자 지정 필드 및 해당 열의 예입니다.

* 계산된 사용자 지정 필드:

사용자 지정 필드를 작성할 때는 &quot;IF&quot; 문에 다음 구문을 사용합니다.

```
IF({Projected Completion Date}>{Planned Completion Date},"Off Track","On Track")
```

* 계산된 사용자 지정 열:

사용자 지정 열을 작성할 때는 값 표현식 라인의 &quot;IF&quot; 문에 다음 구문을 사용해야 합니다.

```
valueexpression=IF({projectedCompletionDate}>{plannedCompletionDate},"Off Track","On Track")
```

### 여러 &quot;IF&quot; 문 {#multiple-if-statements}

다음 문과 함께 여러 &quot;IF&quot; 문을 결합하여 보다 복잡하고 동적 표현식을 작성할 수 있습니다.

<pre>IF(Condition1,True Expression,IF(Condition2,True Expression,False Expression))</pre>주목하십시오. 이제 첫 번째 "IF"에 대한 false 문은 없습니다. 대신 두 번째 "IF"의 시작으로 대체했습니다.

다음은 여러 &quot;IF&quot; 문을 사용하는 계산된 사용자 지정 필드 및 해당 사용자 지정 열의 예입니다.

* 계산된 사용자 지정 필드:

   ```
   IF({projectedCompletionDate}>{plannedCompletionDate},"Off Track",IF({plannedCompletionDate}>{projectedCompletionDate},"Off Track","On Track"))
   ```

* 계산된 사용자 지정 열:

```
valueexpression=IF({"projectedCompletionDate"}>{"plannedCompletionDate"},"Off Track",IF({plannedCompletionDate}>{projectedCompletionDate},"Off Track","On Track"))
```

이 예에서, 두 개의 서로 다른 기준 변수를 함께 사용함으로써 동일한 작업을 수행할 수 있었습니다.\
사용자 환경에서 이러한 예를 다시 빌드하여 이러한 옵션을 추가로 탐색할 수 있습니다.

이를 학습하는 가장 좋은 방법은 다양한 필드와 시나리오를 이용하는 것입니다. 또한 API 탐색기에 익숙해지십시오. 그러면 사용할 수 있는 필드 이름이 표시됩니다. API 탐색기에 대한 자세한 내용은 [API 탐색기](../../../wf-api/general/api-explorer.md).

계산된 데이터 표현식의 Workfront 구문에 대한 자세한 내용은 [계산된 데이터 표현식](../../../reports-and-dashboards/reports/calc-cstm-data-reports/calculated-data-expressions.md).
