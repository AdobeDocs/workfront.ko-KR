---
content-type: api;tips-tricks-troubleshooting
navigation-topic: tips-tricks-and-troubleshooting-workfront-api
title: API에서 쿼리 결과 정렬
description: API에서 쿼리 결과 정렬
author: Becky
feature: Workfront API
role: Developer
exl-id: f001adb8-6295-4646-b9f1-78244a8c44a6
source-git-commit: 14ff8da8137493e805e683e5426ea933f56f8eb8
workflow-type: tm+mt
source-wordcount: '60'
ht-degree: 0%

---


# API에서 쿼리 결과 정렬

다음 내용을 API 호출에 추가하면 필드를 기준으로 결과를 정렬할 수 있습니다.

```
&entryDate_Sort=asc
```

예를 들어, 작업 계획 시작 일자별로 정렬하려면 다음을 제거합니다. `entryDate` 바꿀 내용: `plannedCompletionDate`.

Adobe Workfront의 대부분의 필드에 적용됩니다.
