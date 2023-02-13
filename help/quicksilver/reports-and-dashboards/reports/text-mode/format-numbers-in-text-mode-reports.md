---
product-area: reporting
navigation-topic: text-mode-reporting
title: 텍스트 모드 보고서에서 숫자, 통화 및 백분율 값 형식 지정
description: 통화를 포함한 숫자 값은 Adobe Workfront의 보고서 및 목록에서 다양한 형식으로 표시되도록 구성할 수 있습니다.
author: Nolan
feature: Reports and Dashboards
exl-id: 965f5dcd-4844-4792-9fd0-a47814a325a4
source-git-commit: 54f4c136cfaaaaaa90a4fc64d3ffd06816cff9cb
workflow-type: tm+mt
source-wordcount: '154'
ht-degree: 7%

---

# 텍스트 모드 보고서에서 숫자, 통화 및 백분율 값 형식 지정

통화를 포함한 숫자 값은 Adobe Workfront의 보고서 및 목록에서 다양한 형식으로 표시되도록 구성할 수 있습니다.

숫자 값의 형식을 수정하려면 **value 형식** 열의 행.

예를 들어 예산 열을 $1000로 표시하려면 값 형식 라인이 다음과 같습니다.

```
valueformat=currencyStringCurrencyRounded
valuefield=budget
```

Workfront 보고서 및 텍스트 모드를 사용한 목록에서 조건부 서식을 적용하는 방법에 대한 자세한 내용은 [텍스트 모드에서 조건부 서식 사용](../../../reports-and-dashboards/reports/text-mode/use-conditional-formatting-text-mode.md).

다음 값을 사용하여 숫자 서식을 지정할 수 있습니다 `valueformat` 열 줄:

| 예 | `valueformat=` |
|---|---|
| 1234 | <pre>doubleAsString</pre> <br>또는 <br><pre>int</pre> |
| 1,234 | <pre>doubleAsInt</pre> |
| $1,234 | <pre>currencyStringCurrencyRounded</pre> |
| 1234.56 | <pre>doubleAsDouble</pre> |
| $1,234.56 | <pre>currencyStringCurrency</pre> |
| 12% | <pre>doubleAsPercentRounded</pre> |
| 12.34% | <pre>doubleAsPercent</pre> |
| (1,234.56) | <pre>doubleAsFinancial</pre> |
| (1,234) | <pre>doubleAsFinancialRounded</pre> |
