---
content-type: api;tips-tricks-troubleshooting
navigation-topic: tips-tricks-and-troubleshooting-workfront-api
title: API에서 쿼리 결과 정렬
description: API에서 쿼리 결과 정렬
author: Becky
feature: Workfront API
role: Developer
exl-id: f001adb8-6295-4646-b9f1-78244a8c44a6
source-git-commit: 5936982217adc6cfcaf9e400bfff67a1496d3a78
workflow-type: tm+mt
source-wordcount: '60'
ht-degree: 0%

---


# API에서 쿼리 결과 정렬

다음 내용을 API 호출에 추가하면 필드를 기준으로 결과를 정렬할 수 있습니다.

```
&entryDate_Sort=asc
```

예를 들어 작업 계획 완료 날짜별로 정렬하려면 `entryDate`을(를) 제거하고 `plannedCompletionDate`(으)로 바꾸십시오.

```
&plannedCompletionDate_Sort=asc
```

Adobe Workfront의 대부분의 필드에 적용됩니다.
