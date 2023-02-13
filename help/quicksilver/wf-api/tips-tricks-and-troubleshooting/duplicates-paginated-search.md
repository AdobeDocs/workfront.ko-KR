---
content-type: api;tips-tricks-troubleshooting
navigation-topic: tips-tricks-and-troubleshooting-workfront-api
title: 페이지를 매긴 검색 중에 반환된 중복
description: 페이지를 매긴 검색 중에 반환된 중복
author: John
feature: Workfront API
exl-id: 0359d6ba-b219-4d11-9f6f-cec2ff9ee058
source-git-commit: a939e14cbd6936bdd0c46c1ed641acdda497b8fc
workflow-type: tm+mt
source-wordcount: '111'
ht-degree: 0%

---


# 페이지를 매긴 검색 중에 반환된 중복

## 문제

API에서 개체에 대해 큰 페이지 매김 검색을 수행할 때 고객이 중복 항목을 수신하고 레코드가 누락됩니다.

## 솔루션

주문이 공식적으로 정의되지 않은 경우 Adobe에서는 Oracle 데이터베이스에서 반환한 행의 순서에 의존하여 결정론적 순서를 보장하지 않습니다. 예를 들어 동일한 쿼리를 사용하는 두 개의 연속 호출은 다른 순서로 행을 반환할 수 있습니다. 마찬가지로 페이징을 수행할 때 행이 임의로 다른 &quot;페이지&quot;에 할당되어 중복될 수 있습니다. 가장 간단한 방법은 ID별로 정렬을 추가하는 것입니다.

```
&ID_Sort=asc
```

