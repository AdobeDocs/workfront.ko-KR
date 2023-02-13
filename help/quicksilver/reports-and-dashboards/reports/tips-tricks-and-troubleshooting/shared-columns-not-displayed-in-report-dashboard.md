---
content-type: faq
product-area: reporting
navigation-topic: tips-tricks-and-troubleshooting-reports
title: 공유 열의 데이터는 대시보드 보고서에 표시되지 않습니다
description: 보고서가 여러 열 대시보드 레이아웃에 배치되면 공유 열의 데이터가 표시되지 않지만 단일 열 레이아웃에 표시됩니다. 줄 바꿈이 재정의됩니다.
author: Nolan
feature: Reports and Dashboards
exl-id: b8307182-3ec1-4f16-8427-48ef7a65f969
source-git-commit: 54f4c136cfaaaaaa90a4fc64d3ffd06816cff9cb
workflow-type: tm+mt
source-wordcount: '162'
ht-degree: 0%

---

# 공유 열의 데이터는 대시보드 보고서에 표시되지 않습니다

## 문제

보고서가 여러 열 대시보드 레이아웃에 배치되면 공유 열의 데이터가 표시되지 않지만 단일 열 레이아웃에 표시됩니다. 줄 바꿈이 재정의됩니다.

## 원인

로 표시된 열만

```
shortview=true
```

대시보드 레이아웃에 왼쪽/오른쪽 분할이나 왼쪽/중간/오른쪽 분할이 설정되어 있을 경우 보고서의 대시보드 보기에 포함됩니다.

## 솔루션

보고서에 사용된 보기에 액세스하고 텍스트 모드를 엽니다. (자세한 내용은 [텍스트 모드를 사용하여 보기 편집](../../../reports-and-dashboards/reports/text-mode/edit-text-mode-in-view.md)) 공유/병합된 열에 사용된 열을 포함하여 보고서의 모든 열에 레이블을 지정합니다.

```
shortview=true
```

. 그러면 보고서 열이 대시보드에 제대로 표시됩니다.
