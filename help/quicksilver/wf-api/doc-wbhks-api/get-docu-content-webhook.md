---
content-type: api
product-area: documents
navigation-topic: documents-webhooks-api
title: 웹후크를 통해 문서 콘텐츠 가져오기
description: 문서에 대한 원시 바이트 반환
author: Becky
feature: Workfront API, Digital Content and Documents
exl-id: 0f0b5af7-f276-4856-852c-e976fa491f83
source-git-commit: 54d1753b9062b6d4910e4478c1f072b7fedc87eb
workflow-type: tm+mt
source-wordcount: '43'
ht-degree: 16%

---

# 웹후크를 통해 문서 콘텐츠 가져오기

문서에 대한 원시 바이트 반환

## URL

GET /다운로드

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
   <td> <p>id</p> </td> 
   <td> 문서 ID.</td> 
  </tr> 
 </tbody> 
</table>

## 응답

문서의 원시 바이트입니다.

**예**:  `https://www.acme.com/api/download?id=123456`
