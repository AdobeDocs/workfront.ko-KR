---
content-type: faq
product-area: reporting
navigation-topic: tips-tricks-and-troubleshooting-reports
title: 공유 열의 데이터가 대시보드 보고서에 표시되지 않음
description: Data from shared columns does not display when the report is placed in a multiple column dashboard layout, but it does display on a single column layout. Line breaks are also overridden.
author: Courtney
feature: Reports and Dashboards
exl-id: b8307182-3ec1-4f16-8427-48ef7a65f969
source-git-commit: 6a6d3d47ed5741e3202c44b7240a2e67b687ea95
workflow-type: tm+mt
source-wordcount: '162'
ht-degree: 1%

---

# 공유 열의 데이터가 대시보드 보고서에 표시되지 않음

## 문제

Data from shared columns does not display when the report is placed in a multiple column dashboard layout, but it does display on a single column layout. Line breaks are also overridden.

## 원인

Only columns marked as

```
shortview=true
```

are included in the dashboard view of the report when the dashboard layout has the left/right split or the left/middle/right split set up.

## 솔루션

Access the view used in the report and open text mode. (For more information, see [Edit a view using text mode](../../../reports-and-dashboards/reports/text-mode/edit-text-mode-in-view.md).) Label all columns in the report, including the columns used in a shared/merged column, with

```
shortview=true
```

. The report columns will then display properly in the dashboard.
