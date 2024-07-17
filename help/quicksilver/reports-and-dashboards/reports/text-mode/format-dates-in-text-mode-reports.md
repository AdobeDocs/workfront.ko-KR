---
product-area: reporting
navigation-topic: text-mode-reporting
title: 텍스트 모드 보고서에서 날짜 형식 지정
description: Adobe Workfront의 보고서와 목록에 날짜를 다양한 형식으로 표시하도록 구성할 수 있습니다. 날짜 형식을 설정하려면 열에서 텍스트 모드 코드의 valueformat 라인을 수정해야 합니다.
author: Nolan
feature: Reports and Dashboards
exl-id: ff0686aa-b306-4954-8f9b-3e98bf8cff22
source-git-commit: 54f4c136cfaaaaaa90a4fc64d3ffd06816cff9cb
workflow-type: tm+mt
source-wordcount: '198'
ht-degree: 0%

---

# 텍스트 모드 보고서에서 날짜 형식 지정

Adobe Workfront의 보고서와 목록에 날짜를 다양한 형식으로 표시하도록 구성할 수 있습니다. 날짜 형식을 설정하려면 열에서 텍스트 모드 코드의 `valueformat` 줄을 수정해야 합니다.

`valueformat= [new date format]` 예를 들어, 예상 완료 일자를 MM/DD/YY로 표시하려는 경우 코드는 다음과 같습니다.

```
valueformat=atDate
valuefield=projectedCompletionDate
```

계획된 완료 일자를 *월, DD, 연도*(으)로 표시하려면 코드가 다음과 같습니다.

```
valueformat=mediumAtdate
valuefield=plannedCompletionDate
```

텍스트 모드를 사용하여 Workfront 보고서 및 목록에서 조건부 서식을 적용하는 방법에 대한 자세한 내용은 [텍스트 모드에서 조건부 서식 사용](../../../reports-and-dashboards/reports/text-mode/use-conditional-formatting-text-mode.md)을 참조하십시오.

다음을 사용하여 날짜 형식을 지정할 수 있습니다

```
valueformat
```

 텍스트 모드 값:

| **형식** | 예  | ***valueformat=*** |
|---|---|---|
| MM/DD/YY | 10/11/18 | `atDate` |
| MM/DD/YY 시간 | 10/11/18 12:00pm | `longAtDate` |
| MM/DD/YY | 10/11/18 | `shortAtDate` |
| 월, DD, 연도 | 2018년 10월 11일 | `mediumAtDate` |
| DW, 월, 일, 년 | 2018년 10월 11일 월요일 | `partialAtDate` |
| DW, 월, 일, 연도 시간 | 2018년 10월 11일 월요일 오후 12:00 | `fullAtDate` |
