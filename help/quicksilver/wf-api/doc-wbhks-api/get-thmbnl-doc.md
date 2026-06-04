---
content-type: api
product-area: documents
navigation-topic: documents-webhooks-api
title: 문서에 대한 썸네일 가져오기
description: 문서에 대한 썸네일 가져오기
author: Becky
feature: Workfront API
role: Developer
exl-id: 31960689-1811-4ba7-a63d-0842caedf3ea
TQID: https://experienceleague.adobe.com/-LE1gxQ9aViRNuN0sI14HlZaIcLc6Mmm8XmS1zaRCFQ
product_v2:
  - id: c4a86a5d-6562-4fc6-aa00-bfa25833aed9
role_v2:
  - id: ff6a42d2-313e-452e-93a6-792e4fad9ff8
source-git-commit: 55a9d9feae8cc1128e3427a8874414ba734dd467
workflow-type: tm+mt
source-wordcount: 55
ht-degree: 12%

---

# 문서에 대한 썸네일 가져오기

문서에 대한 원시 썸네일 바이트를 반환합니다.

**URL**

GET /thumbnail

## 쿼리 매개변수

| 이름  | 설명 |
|---|---|
| ID  | 문서 ID. |
| 크기  |  썸네일의 너비입니다. |


## 응답

원시 썸네일 바이트.

**예:**: https://www.acme.com/api/thumbnail?id=123456
