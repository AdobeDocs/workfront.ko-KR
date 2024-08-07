---
content-type: api
product-area: documents
navigation-topic: documents-webhooks-api
title: 문서 웹후크를 통해 검색
description: 문서 웹후크를 통해 검색
author: Becky
feature: Workfront API, Digital Content and Documents
role: Developer
exl-id: 8a3bf0c4-4a20-4311-8c05-15f4ef3a1d42
source-git-commit: 14ff8da8137493e805e683e5426ea933f56f8eb8
workflow-type: tm+mt
source-wordcount: '154'
ht-degree: 3%

---

# 문서 웹후크를 통해 검색

검색에서 반환된 파일 및 폴더에 대한 메타데이터를 반환합니다. 전체 텍스트 검색이나 일반 데이터베이스 쿼리로 구현할 수 있습니다. Adobe Workfront은 사용자가 외부 파일 브라우저에서 검색을 수행할 때 /search 끝점을 호출합니다.

## URL

GET /search

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
   <td>쿼리</td> 
   <td>검색어 또는 구.</td> 
  </tr> 
  <tr> 
   <td>parentId</td> 
   <td> <p>(선택 사항) 검색이 실행되는 폴더 ID입니다. 참고: Workfront의 향후 기능을 위한 자리 표시자입니다. 현재 Workfront는 이 매개 변수를 전달하지 않습니다. </p> </td> 
  </tr> 
  <tr> 
   <td>최대</td> 
   <td>반환할 최대 항목 수입니다. 페이지 매김에 사용됩니다.</td> 
  </tr> 
  <tr> 
   <td>offset</td> 
   <td> 'max'와 함께 사용되는 페이지 오프셋입니다.</td> 
  </tr> 
 </tbody> 
</table>

 

## 응답

쿼리와 일치하는 파일 및 폴더에 대한 메타데이터 목록이 포함된 JSON입니다. &quot;일치&quot;를 구성하는 것은 웹후크 공급자에 의해 결정됩니다. 이상적으로는 전체 텍스트 검색을 수행해야 합니다. 파일 이름 기반 검색도 작동합니다.

**예:**

예: `https://www.acme.com/api/search?query=test-query`

```
[ 
{ File/Folder Metadata },
{ File/Folder Metadata } 
]
```
