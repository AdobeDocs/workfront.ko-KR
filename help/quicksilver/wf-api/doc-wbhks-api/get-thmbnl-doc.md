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
source-git-commit: 14ff8da8137493e805e683e5426ea933f56f8eb8
workflow-type: tm+mt
source-wordcount: '50'
ht-degree: 6%

---


# 문서에 대한 썸네일 가져오기

문서에 대한 원시 썸네일 바이트를 반환합니다.

**URL**

GET /thumbnail

## 쿼리 매개변수

| 이름  | 설명 |
|---|---|
| id  | 문서 ID. |
| 크기  |  썸네일의 너비입니다. |


## 응답

원시 썸네일 바이트.

**예:**: https://www.acme.com/api/thumbnail?id=123456
