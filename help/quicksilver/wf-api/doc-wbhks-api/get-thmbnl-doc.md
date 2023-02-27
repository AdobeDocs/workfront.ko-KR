---
content-type: api
product-area: documents
navigation-topic: documents-webhooks-api
title: 문서의 축소판 그림 가져오기
description: 문서의 축소판 그림 가져오기
author: Becky
feature: Workfront API
exl-id: 31960689-1811-4ba7-a63d-0842caedf3ea
source-git-commit: f050c8b95145552c9ed67b549608c16115000606
workflow-type: tm+mt
source-wordcount: '54'
ht-degree: 7%

---


# 문서의 축소판 그림 가져오기

문서에 대한 원시 축소판 바이트를 반환합니다.

**URL**

GET /축소판

## 쿼리 매개 변수

| 이름  | 설명 |
|---|---|
| id  | 문서 ID입니다. |
| 크기  |  축소판의 폭입니다. |


## 응답

원시 축소판 바이트

**예:**: https://www.acme.com/api/thumbnail?id=123456
