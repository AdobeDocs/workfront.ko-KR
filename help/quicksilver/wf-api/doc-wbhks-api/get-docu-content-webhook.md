---
content-type: api
product-area: documents
navigation-topic: documents-webhooks-api
title: Webhooks를 통해 문서 컨텐츠 가져오기
description: 문서에 대한 원시 바이트 반환
author: Becky
feature: Workfront API, Digital Content and Documents
exl-id: 0f0b5af7-f276-4856-852c-e976fa491f83
source-git-commit: f050c8b95145552c9ed67b549608c16115000606
workflow-type: tm+mt
source-wordcount: '53'
ht-degree: 7%

---

# Webhooks를 통해 문서 컨텐츠 가져오기

문서에 대한 원시 바이트 반환

## URL

GET /다운로드

## 쿼리 매개 변수

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
   <td> <p>id</p> </td> 
   <td> 문서 ID입니다.</td> 
  </tr> 
 </tbody> 
</table>

## 응답

문서의 원시 바이트입니다.

**예:**:  [https://www.acme.com/api/download?id=123456](https://www.acme.com/api/download?id=123456)
