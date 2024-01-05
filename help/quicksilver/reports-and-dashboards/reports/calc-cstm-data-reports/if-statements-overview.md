---
content-type: overview
product-area: reporting
navigation-topic: calculate-custom-data-reports
title: IF 문 개요
description: 일반 프로그래밍 언어에서 "IF" 문을 사용할 수 있습니다. Adobe Workfront에서 "IF" 문을 사용하면 보고 및 사용자 지정 데이터 목적 모두에 대해 데이터 필드를 비교하고, 형식을 지정하며, 함께 문자열을 지정할 수 있습니다. 또한, "IF" 문장에 대해 수학적으로 생각하는 것은 표현에 대한 변수들이 일반적으로 사용되기 때문에 더 나은 개념 이해로 이어진다.
author: Nolan
feature: Reports and Dashboards
exl-id: 090a85fd-fdbe-4507-8bad-ce8c29bf8fc9
source-git-commit: 23b5ba9564b514e11c1ca9d5cca276238ef11066
workflow-type: tm+mt
source-wordcount: '925'
ht-degree: 0%

---

# &quot;IF&quot; 문 개요

<!-- Audited: 1/2024 -->

일반 프로그래밍 언어에서 &quot;IF&quot; 문을 사용할 수 있습니다. Adobe Workfront에서 &quot;IF&quot; 문을 사용하면 보고 및 사용자 지정 데이터 목적 모두에 대해 데이터 필드를 비교하고, 형식을 지정하며, 함께 문자열을 지정할 수 있습니다. 또한, &quot;IF&quot; 문장에 대해 수학적으로 생각하는 것은 표현에 대한 변수들이 일반적으로 사용되기 때문에 더 나은 개념 이해로 이어진다.

## Recommendations for &quot;IF&quot; 문

&quot;IF&quot; 문을 생성하기 전에 다음 사항을 고려하십시오.

* 이 안내서에서는 모든 일반 프로그래밍 언어에 대한 기본 이해를 권장하지만 반드시 필요한 것은 아닙니다.
* Workfront 텍스트 모드 구문에 대한 고급 이해가 필요합니다. 이렇게 하면 Workfront API의 용어를 이해하고 이러한 특정 형식의 사용자 지정 데이터 구문을 이해하는 데 도움이 됩니다.

  Workfront API에 대한 자세한 내용은 [API 기본 사항](../../../wf-api/general/api-basics.md).

  텍스트 모드 사용에 대한 자세한 내용은 [텍스트 모드 개요](../../../reports-and-dashboards/reports/text-mode/understand-text-mode.md).

* 다음 Workfront 요소에 대해 &quot;IF&quot; 문을 작성할 수 있습니다.

   * 조회수
   * 그룹화
   * 계산된 사용자 정의 필드

* 필터에 대해 &quot;IF&quot; 문을 작성할 수 없습니다. 그 결과 Workfront에서 &quot;죄송합니다&quot; 오류가 발생합니다.
* 지원 팀은 사용자 정의 데이터를 작성하는 데 도움이 되지 않습니다. 사용자 정의 필드 또는 열을 빌드했지만 원하는 결과가 표시되지 않는 경우 지원 팀에 문의할 수 있습니다. 표현식 작성에 도움이 필요하면 계정 담당자에게 문의하여 컨설팅 옵션에 대해 문의하십시오.
* Sublime 또는 Visual Studio Code와 같이 Workfront에 표시되는 것보다 더 명확하게 데이터를 볼 수 있도록 텍스트 편집기에서 이러한 표현식을 먼저 작성하는 것이 좋습니다.

## &quot;IF&quot; 문의 구성 요소

다음 형식을 사용하여 Workfront에서 &quot;IF&quot; 문을 작성할 수 있습니다.
<pre>IF(Condition,True 표현식,False 표현식)</pre>"IF" 문의 구성 요소는 다음과 같습니다.

* **IF** = &quot;function&quot;에 대한 Workfront 계산된 데이터 표현식입니다. SUM 및 PROD 표현식과 마찬가지로 이 표현식은 먼저 시스템에 함수를 &quot;IF&quot; 문으로 이해하도록 지시합니다. 이 문에서 &quot;IF&quot;에는 항상 대문자를 사용하십시오.\
  모든 계산된 데이터 표현식의 목록은 다음을 참조하십시오 [계산된 데이터 표현식 개요](../../../reports-and-dashboards/reports/calc-cstm-data-reports/calculated-data-expressions.md).

* **조건** = Workfront 변수가 충족해야 하는 조건이며 이 방정식의 기초입니다. 방정식에서 나중에 지정할 수 있는 모든 것은 조건에 따라 달라진다. 여러 참조, 비교 또는 수학 표현식을 사용하여 방정식을 시작할 수 있습니다. 조건의 일부 예는 다음과 같습니다.

   * 날짜가 지정된 개체의 다른 날짜보다 이후입니다.
   * 상태는 지정된 오브젝트에서 사용 가능한 상태 중 하나와 같습니다.
   * 작업 완료율이 특정 비율보다 작거나 더 큽니다.

* **조건 연산자** = &quot;IF&quot; 문의 조건을 작성하는 데 도움이 되는 연산자입니다. 예를 들어 &quot;다음과 같음&quot; 또는 &quot;다음보다 큼&quot;은 조건 연산자입니다. 문에서 사용할 수 있는 조건 연산자 목록은 다음을 참조하십시오. [계산된 사용자 정의 표현식의 조건 연산자](../../../reports-and-dashboards/reports/calc-cstm-data-reports/condition-operators-calculated-custom-expressions.md).

* ****** 표현식** = &quot;True&quot; 변수로, 조건 기준이 충족되면 어떤 지표를 표시할지 방정식에 알려줍니다(True 지표).

* **False 표현식** = 조건 기준이 충족되지 않을 때 표시할 지표(거짓 지표)를 방정식에 알려 주는 &quot;False&quot; 변수입니다.

다음 예제에서는 원래 문 형식을 사용하여 &quot;IF&quot; 문에 대한 간단한 데이터 표현식을 작성합니다. 이 표현식은 Workfront의 두 개의 서로 다른 날짜 필드와 True/False 결과를 데이터 문자열로 비교합니다.

```
IF({projectedCompletionDate}>{plannedCompletionDate},"Off Track","On Track")
```

일상 대화에서 이 명령문은 다음과 같은 의미입니다. 내 객체의 예상 완료 일자가 동일한 객체의 계획된 완료 일자보다 &quot;큼&quot;인 경우 이 필드에 &quot;트랙외&quot;라는 단어를 표시합니다. 그렇지 않으면 &quot;추적 중&quot;이라는 단어를 표시합니다.

## &quot;IF&quot; 문을 사용하여 사용자 정의 양식 또는 사용자 정의 열에서 계산된 필드 작성

사용자 정의 양식 또는 사용자 정의 열에서 계산된 필드에 &quot;IF&quot; 문을 작성할 수 있습니다.

계산된 사용자 정의 양식과 계산된 사용자 정의 열에서 사용하는 구문은 차이가 있습니다. 다음 예를 참조하십시오.

* [단일 &quot;IF&quot; 문](#single-if-statements)
* [여러 &quot;IF&quot; 문](#multiple-if-statements)

### 단일 &quot;IF&quot; 문 {#single-if-statements}

다음은 &quot;IF&quot; 문을 사용하는 계산된 사용자 정의 필드 및 해당 열의 예입니다.

* 계산된 사용자 정의 필드:

사용자 지정 필드를 작성할 때 &quot;IF&quot; 문에 다음 구문을 사용합니다.

```
IF({Projected Completion Date}>{Planned Completion Date},"Off Track","On Track")
```

* 계산된 사용자 정의 열:

사용자 지정 열을 작성할 때는 값 표현식 라인의 &quot;IF&quot; 문에 다음 구문을 사용해야 합니다.

```
valueexpression=IF({projectedCompletionDate}>{plannedCompletionDate},"Off Track","On Track")
```

### 여러 &quot;IF&quot; 문 {#multiple-if-statements}

다음 문으로 여러 &quot;IF&quot; 문을 결합하여 보다 복잡하고 동적인 표현식을 작성할 수 있습니다.

<pre>IF(Condition1,True 표현식,IF(Condition2,True 표현식,False 표현식))</pre>이제 첫 번째 "IF"에 대해 잘못된 설명이 없습니다. 대신 두 번째 "IF"의 시작으로 대체했습니다.

다음은 여러 &quot;IF&quot; 문을 사용하는 계산된 사용자 정의 필드 및 해당 사용자 정의 열의 예입니다.

* 계산된 사용자 정의 필드:

  ```
  IF({projectedCompletionDate}>{plannedCompletionDate},"Off Track",IF({plannedCompletionDate}>{projectedCompletionDate},"Off Track","On Track"))
  ```

* 계산된 사용자 정의 열:

```
valueexpression=IF({"projectedCompletionDate"}>{"plannedCompletionDate"},"Off Track",IF({plannedCompletionDate}>{projectedCompletionDate},"Off Track","On Track"))
```

이 예에서는 서로 다른 두 기준 변수를 함께 적용하여 동일한 작업을 수행했습니다.\
이러한 예제를 사용자 환경에 다시 빌드하여 이러한 옵션을 추가로 탐색할 수 있습니다.

이를 학습하는 가장 좋은 방법은 다양한 분야와 시나리오를 실험하는 것이다. 또한 사용할 수 있는 필드 이름이 표시되는 API 탐색기에 익숙해지십시오. API 탐색기에 대한 자세한 내용은 [API 탐색기](../../../wf-api/general/api-explorer.md).

계산된 데이터 표현식의 Workfront 구문에 대한 자세한 내용은 [계산된 데이터 표현식 개요](../../../reports-and-dashboards/reports/calc-cstm-data-reports/calculated-data-expressions.md).
