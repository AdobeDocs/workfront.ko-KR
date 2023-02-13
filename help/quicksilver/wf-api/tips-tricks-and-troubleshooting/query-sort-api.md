---
content-type: api;tips-tricks-troubleshooting
navigation-topic: tips-tricks-and-troubleshooting-workfront-api
title: API에서 쿼리 결과 정렬
description: API에서 쿼리 결과 정렬
author: John
feature: Workfront API
exl-id: f001adb8-6295-4646-b9f1-78244a8c44a6
source-git-commit: a939e14cbd6936bdd0c46c1ed641acdda497b8fc
workflow-type: tm+mt
source-wordcount: '60'
ht-degree: 0%

---


# API에서 쿼리 결과 정렬

API 호출에 다음을 추가한 경우 필드를 기준으로 결과를 정렬할 수 있습니다.

```
&entryDate_Sort=asc
```

예를 들어 계획 시작 일자별로 정렬하려면 다음을 제거합니다 `entryDate` 다음으로 바꾸십시오. `plannedCompletionDate`.

Adobe Workfront의 대부분의 필드에 대해 작동합니다.
