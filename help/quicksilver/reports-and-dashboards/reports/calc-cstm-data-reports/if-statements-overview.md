---
content-type: overview
product-area: reporting
navigation-topic: calculate-custom-data-reports
title: IF 문 개요
description: 일반 프로그래밍 언어에서 "IF" 문을 사용할 수 있습니다. Adobe Workfront에서 "IF" 문을 사용하면 보고 및 사용자 지정 데이터 목적 모두에 대해 데이터 필드를 비교, 형식 지정 및 문자열로 연결할 수 있습니다. 또한, "IF" 문장에 대해 수학적으로 생각하면 표현에 대한 변수가 일반적으로 사용되기 때문에 개념적 이해가 더 잘 된다.
author: Courtney
feature: Reports and Dashboards
exl-id: 090a85fd-fdbe-4507-8bad-ce8c29bf8fc9
source-git-commit: 4261febe4af8628508083fa18e4767e3fd3e1136
workflow-type: tm+mt
source-wordcount: '925'
ht-degree: 0%

---

# &quot;IF&quot; 문 개요

<!-- Audited: 1/2024 -->

일반 프로그래밍 언어에서는 &quot;IF&quot; 문을 사용할 수 있습니다. Adobe Workfront에서 &quot;IF&quot; 문을 사용하면 보고 및 사용자 지정 데이터 목적 모두에 대해 데이터 필드를 비교, 형식 지정 및 문자열로 연결할 수 있습니다. 또한 &quot;IF&quot; 문에 대해 수학적으로 생각하면 표현식에 대한 변수가 일반적으로 사용되기 때문에 더 나은 개념적 이해로 이어집니다.

## &quot;IF&quot; 문에 대한 권장 사항

&quot;IF&quot; 문을 만들기 전에 다음 사항을 고려하십시오.

* 모든 일반 프로그래밍 언어에 대한 기본적인 이해를 권장하지만 이 안내서에서는 필요하지 않습니다.
* Workfront 텍스트 모드 구문에 대한 고급 이해가 필요합니다. 이렇게 하면 Workfront API의 용어를 파악하고 이러한 특정 형식의 사용자 지정 데이터 구문을 이해하는 데 도움이 됩니다.

  Workfront API에 대한 자세한 내용은 [API 기본 사항](../../../wf-api/general/api-basics.md)을 참조하세요.

  For information about using text mode, see [Text Mode overview](../../../reports-and-dashboards/reports/text-mode/understand-text-mode.md).

* You can build &quot;IF&quot; statements for the following Workfront elements:

   * 보기 횟수
   * 그룹화
   * 계산된 사용자 정의 필드

* 필터에 대해서는 &quot;IF&quot; 문을 빌드할 수 없습니다. 이러면 Workfront에서 &quot;Whops&quot; 오류가 발생합니다.
* 지원 팀은 사용자 정의 데이터 작성에 도움을 주지 않습니다. You can contact the Support Team after you build the custom fields or columns and you are not seeing the desired results. For help building an expression, please contact your Account Executive to inquire about our consulting options.
* We recommend writing these expressions in a text editor first, such as Sublime or Visual Studio Code, because this helps you see data more clearly than would appear in Workfront.

## IF 문의 구성 요소

다음 형식을 사용하여 Workfront에서 &quot;IF&quot; 문을 작성할 수 있습니다.
<pre>IF(Condition,True Expression,False Expression)</pre>"IF" 문의 구성 요소는 다음과 같습니다.

* **IF** = &quot;function&quot;에 대한 Workfront 계산 데이터 식입니다. SUM 및 PROD 표현식과 마찬가지로 이 표현식은 먼저 &quot;IF&quot; 문으로 함수를 이해하도록 시스템에 지시합니다. 이 문에서 &quot;IF&quot;에는 항상 대문자를 사용하십시오.\
  모든 계산된 데이터 식의 목록은 [계산된 데이터 식의 개요](../../../reports-and-dashboards/reports/calc-cstm-data-reports/calculated-data-expressions.md)를 참조하십시오.

* **조건** = Workfront 변수가 충족해야 하는 조건이며 이 방정식의 기초입니다. 나중에 방정식에서 지정할 수 있는 모든 것은 조건에 따라 다릅니다. 여러 참조, 비교 또는 수학 표현식을 사용하여 방정식을 시작할 수 있습니다. 조건의 몇 가지 예는 다음과 같습니다.

   * 날짜가 지정된 개체의 다른 날짜보다 이후입니다.
   * 상태는 지정된 객체에서 사용 가능한 상태 중 하나와 같습니다.
   * Percent complete of a task is lesser than or greater than a certain percentage.

* **Condition Operator** = this is the operator that helps you build the condition of your &quot;IF&quot; statement. For example, &quot;is equal to&quot; or &quot;is greater than&quot; are condition operators. For a list of condition operators that you can use in statements, see [Condition operators in calculated custom expressions](../../../reports-and-dashboards/reports/calc-cstm-data-reports/condition-operators-calculated-custom-expressions.md).

* **True****Expression** = This is the &quot;True&quot; variable, which tells the equation which indicator to display once the criteria of the condition are met (true indicators).

* **False Expression** = This is the &quot;False&quot; variable, which tells the equation which indicator to display when the criteria of the condition are not met (false indicators).

다음 예제에서는 &quot;IF&quot; 문에 대한 간단한 데이터 표현식을 작성하는 데 원본 문 형식을 사용합니다. 이 표현식은 Workfront의 서로 다른 두 날짜 필드와 True/False 결과를 데이터 문자열로 비교합니다.

```
IF({projectedCompletionDate}>{plannedCompletionDate},"Off Track","On Track")
```

In everyday speech, this statement would mean: If the Projected Completion Date of my object is &quot;Greater Than&quot; the Planned Completion Date of my same object, then display the words &quot;Off Track&quot; in this field. If not, display the words &quot;On Track.&quot;

## Build calculated fields in custom forms or custom columns using &quot;IF&quot; statements

You can build &quot;IF&quot; statements in a calculated field either in a custom form, or in a custom column.

There is a difference in the syntax you use in a calculated custom form vs a calculated custom column. 다음 예를 참조하십시오.

* [단일 &quot;IF&quot; 문](#single-if-statements)
* [여러 &quot;IF&quot; 문](#multiple-if-statements)

### 단일 &quot;IF&quot; 문 {#single-if-statements}

다음은 &quot;IF&quot; 문을 사용하는 계산된 사용자 정의 필드 및 해당 열의 예입니다.

* 계산된 사용자 정의 필드:

When building a custom field, use the following syntax for an &quot;IF&quot; statement:

```
IF({Projected Completion Date}>{Planned Completion Date},"Off Track","On Track")
```

* Calculated custom column:

When building a custom column, you should use the following syntax for the &quot;IF&quot; statement in the value expression line:

```
valueexpression=IF({projectedCompletionDate}>{plannedCompletionDate},"Off Track","On Track")
```

### Multiple &quot;IF&quot; statements {#multiple-if-statements}

You can put together multiple &quot;IF&quot; statements with the following statement to build a more complex and dynamic expression:

<pre>IF(Condition1,True 표현식,IF(Condition2,True 표현식,False 표현식))</pre>이제 첫 번째 "IF"에 대한 거짓 진술이 없습니다. 대신, 우리는 그것을 두 번째 "IF"의 시작으로 대체했다.

다음은 여러 &quot;IF&quot; 문을 사용하는 계산된 사용자 정의 필드와 해당 사용자 정의 열의 예입니다.

* 계산된 사용자 정의 필드:

  ```
  IF({projectedCompletionDate}>{plannedCompletionDate},"Off Track",IF({plannedCompletionDate}>{projectedCompletionDate},"Off Track","On Track"))
  ```

* Calculated custom column:

```
valueexpression=IF({"projectedCompletionDate"}>{"plannedCompletionDate"},"Off Track",IF({plannedCompletionDate}>{projectedCompletionDate},"Off Track","On Track"))
```

이 예에서 동일한 작업은 두 개의 다른 기준 변수를 함께 배치함으로써 수행되었습니다.\
이러한 예제를 사용자 환경에서 다시 빌드하여 이러한 옵션을 추가로 탐색할 수 있습니다.

이를 배우는 가장 좋은 방법은 다양한 분야와 시나리오를 실험하는 것입니다. 또한 API 탐색기를 숙지하여 사용할 수 있는 필드 이름을 표시합니다. API 탐색기에 대한 자세한 내용은 [API 탐색기](../../../wf-api/general/api-explorer.md)를 참조하십시오.

계산된 데이터 식의 Workfront 구문에 대한 자세한 내용은 [계산된 데이터 식의 개요](../../../reports-and-dashboards/reports/calc-cstm-data-reports/calculated-data-expressions.md)를 참조하십시오.
