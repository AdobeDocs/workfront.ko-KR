---
content-type: api
product-area: documents
navigation-topic: documents-webhooks-api
title: 문서 웹후크로 폴더 만들기
description: 문서 웹후크로 폴더 만들기
author: Becky
feature: Workfront API
role: Developer
exl-id: 50905915-58c9-4b50-b8a1-133833884a88
source-git-commit: 14ff8da8137493e805e683e5426ea933f56f8eb8
workflow-type: tm+mt
source-wordcount: '66'
ht-degree: 9%

---


# 문서 웹후크로 폴더 만들기

특정 디렉터리에 폴더를 만듭니다.

## URL

POST /createFolder

## 쿼리 매개변수

| **이름** | **설명** |
|---|---|
| parentId  | 폴더를 만들어야 하는 폴더 ID |
| 이름  | 새 폴더의 이름 |




**응답**

/metadata 끝점에 정의된 대로 새로 생성된 폴더의 메타데이터입니다.

## 예

```
POST https://www.acme.com/api/createFolder
­­­­­­­­­­­­­­­­­­­­­­­­­­­­­­­-------------------------------
parentId=1234
name=New Folder 
-------------------------------
```

반환

```
{title:"New Folder",br /> kind:"folder"
 id":"5678",
 viewLink:"",
 downloadLink:"",
 mimeType:"",
 dateModified:"2014­06­05T17:39:45.251Z"
 size: ""
 }
```
