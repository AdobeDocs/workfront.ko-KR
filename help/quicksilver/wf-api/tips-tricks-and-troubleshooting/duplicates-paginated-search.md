---
content-type: api;tips-tricks-troubleshooting
navigation-topic: tips-tricks-and-troubleshooting-workfront-api
title: 페이지가 매겨진 대규모 검색 중 중복이 반환됨
description: 페이지가 매겨진 대규모 검색 중 중복이 반환됨
author: Becky
feature: Workfront API
role: Developer
exl-id: 0359d6ba-b219-4d11-9f6f-cec2ff9ee058
TQID: https://experienceleague.adobe.com/1FXTHSro-rlUVHaajM1monR2Y-sxVHN6KIviogoXqRc
product_v2:
  - id: c4a86a5d-6562-4fc6-aa00-bfa25833aed9
feature_v2:
  - id: b58ad82f-df6b-4b01-81a3-3a02ab9567a0
role_v2:
  - id: ff6a42d2-313e-452e-93a6-792e4fad9ff8
topic_v2:
  - id: c1579802-ddd4-4214-8a91-97b2066abe11
source-git-commit: 55a9d9feae8cc1128e3427a8874414ba734dd467
workflow-type: tm+mt
source-wordcount: 111
ht-degree: 0%

---

# 페이지가 매겨진 대규모 검색 중 중복이 반환됨

## 문제

API에서 오브젝트에 대해 페이지가 매겨진 대규모 검색을 수행할 때 고객이 중복 항목을 받고 레코드가 누락되었습니다.

## 솔루션

순서가 공식적으로 정의되지 않으면 Oracle 데이터베이스에서 반환되는 행 순서에 의존하므로 결정론적 순서가 보장되지 않습니다. 예를 들어 동일한 쿼리를 사용하는 두 개의 연속 호출은 다른 순서로 행을 반환할 수 있습니다. 마찬가지로 페이징을 수행할 때 행이 다른 &quot;페이지&quot;에 임의로 할당되어 중복될 수 있습니다. 가장 간단한 솔루션은 ID별로 정렬을 추가하는 것입니다.

```
&ID_Sort=asc
```

