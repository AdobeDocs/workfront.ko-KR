---
product-area: reporting
navigation-topic: text-mode-reporting
title: 텍스트 모드 보고서에서 숫자, 통화 및 백분율 값 서식 지정
description: 통화를 포함한 숫자 값을 Adobe Workfront의 보고서 및 목록에 다양한 형식으로 표시하도록 구성할 수 있습니다.
author: Nolan
feature: Reports and Dashboards
exl-id: 965f5dcd-4844-4792-9fd0-a47814a325a4
source-git-commit: 9caac488522d2a12d3bdf4bf23ba7e44c6dbf7d2
workflow-type: tm+mt
source-wordcount: '145'
ht-degree: 6%

---

# 텍스트 모드 보고서에서 숫자, 통화 및 백분율 값 서식 지정

<!-- Audited: 1/2025 -->

통화를 포함한 숫자 값을 Adobe Workfront의 보고서 및 목록에 다양한 형식으로 표시하도록 구성할 수 있습니다.

숫자 값의 형식을 수정하려면 열의 **valueformat** 줄을 편집해야 합니다.

예를 들어 예산 열을 $1000로 표시하려는 경우 값 형식 라인은 다음과 같습니다.

```
valueformat=currencyStringCurrencyRounded
valuefield=budget
```

텍스트 모드를 사용하여 Workfront 보고서 및 목록에서 조건부 서식을 적용하는 방법에 대한 자세한 내용은 [텍스트 모드에서 조건부 서식 사용](../../../reports-and-dashboards/reports/text-mode/use-conditional-formatting-text-mode.md)을 참조하십시오.

열의 `valueformat` 행에 대해 다음 값을 사용하여 숫자의 서식을 지정할 수 있습니다.

| 예 | `valueformat=` |
|---|---|
| 1234 | `doubleAsString`<br>또는<br>`int` |
| 1,234 | `doubleAsInt` |
| $1,234 | `currencyStringCurrencyRounded` |
| 1234.56 | `doubleAsDouble` |
| $1,234.56 | `currencyStringCurrency` |
| 12% | `doubleAsPercentRounded` |
| 12.34% | `doubleAsPercent` |
| (1,234.56) | `doubleAsFinancial` |
| (1,234) | `doubleAsFinancialRounded` |

