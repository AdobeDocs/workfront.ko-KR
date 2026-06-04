---
content-type: api
product-area: documents
navigation-topic: documents-webhooks-api
title: 웹후크를 통해 문서 콘텐츠 가져오기
description: 문서에 대한 원시 바이트 반환
author: Becky
feature: Workfront API, Digital Content and Documents
role: Developer
exl-id: 0f0b5af7-f276-4856-852c-e976fa491f83
TQID: https://experienceleague.adobe.com/AIN65ofKDJA95iMpvNwoe3oQapmyxzDC16dpf5ehwH0
product_v2: id: c4a86a5d-6562-4fc6-aa00-bfa25833aed9
role_v2: id: ff6a42d2-313e-452e-93a6-792e4fad9ff8
source-git-commit: 55a9d9feae8cc1128e3427a8874414ba734dd467
workflow-type: tm+mt
source-wordcount: 43
ht-degree: 16%

---

# 웹후크를 통해 문서 콘텐츠 가져오기

문서에 대한 원시 바이트 반환

## URL

GET /download

## 쿼리 매개변수

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th>이름 </th> 
   <th>설명</th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td> <p>ID</p> </td> 
   <td> 문서 ID.</td> 
  </tr> 
 </tbody> 
</table>

## 응답

문서의 원시 바이트입니다.

**예**: `https://www.acme.com/api/download?id=123456`
