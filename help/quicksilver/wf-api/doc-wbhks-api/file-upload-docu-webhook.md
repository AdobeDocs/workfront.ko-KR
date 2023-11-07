---
content-type: api
product-area: documents
navigation-topic: documents-webhooks-api
title: 문서 웹후크를 통한 파일 업로드
description: 문서 웹후크를 통한 파일 업로드
author: Becky
feature: Workfront API
role: Developer
exl-id: 2c5727ee-bf8f-4664-a9b1-c5da356d94f5
source-git-commit: 14ff8da8137493e805e683e5426ea933f56f8eb8
workflow-type: tm+mt
source-wordcount: '261'
ht-degree: 5%

---


# 문서 웹후크를 통한 파일 업로드

문서 스토리지 공급자에 파일을 업로드하는 것은 두 개의 개별 API 끝점이 필요한 두 단계 프로세스입니다. Adobe Workfront은 /uploadInit 를 호출하여 업로드 프로세스를 시작합니다. 이 끝점은 문서 ID를 반환하고 문서 바이트를 업로드할 때 /upload에 전달됩니다. 기본 문서 스토리지 시스템에 따라 길이가 0인 문서를 만든 다음 나중에 문서 내용을 업데이트해야 할 수 있습니다.

이 사양의 버전 1.1에 추가된 문서 ID 및 문서 버전 ID를 사용하여 Workfront에서 추가 정보를 검색할 수 있습니다.

**예:** 문서 관리 시스템에서 문서에 대한 추가 정보를 원하는 경우 웹후크 구현 코드는 문서 ID를 사용하여 Workfront의 RESTful API를 사용하여 해당 정보를 검색할 수 있습니다. 문서의 사용자 정의 데이터 필드에서 가져온 이 정보에는 작업, 문제 또는 프로젝트가 포함되어 있는 것이 좋습니다.

## POST 방법

**URL**

POST /uploadInit

### 쿼리 매개변수

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
   <td>parentId </td> 
   <td>웹후크 공급자가 참조하는 상위 폴더 ID입니다.</td> 
  </tr> 
  <tr> 
   <td>파일 이름 </td> 
   <td>문서 이름</td> 
  </tr> 
  <tr> 
   <td>documentId</td> 
   <td> <p>Workfront 문서 ID(버전 1.1에 추가됨)</p> <p> </p> </td> 
  </tr> 
  <tr> 
   <td>documentVersionId </td> 
   <td>Workfront 문서 버전 ID(버전 1.1에 추가됨) </td> 
  </tr> 
 </tbody> 
</table>

## 응답

/metadata 끝점에 정의된 파일의 메타데이터입니다. 여기에는 공급자가 사용하는 문서 ID가 포함됩니다.

**예:**

```
https://www.acme.com/api/uploadInit?parentId=12345&filename=new-file.png&documentId=511ea6e000023edb38d2effb2f4e6e3b&documentVersionId=511ea6e000023edb38d2e ffb2f4e6e3b
```

## PUT 방법

문서의 바이트를 웹후크 공급자에 업로드합니다.

**URL**

PUT /업로드

## 쿼리 매개변수

| 이름  | 설명 |
|---|---|
| id  |  방금 만든 문서 ID입니다. |


**요청 본문**

문서에 대한 원시 콘텐츠 바이트입니다.

**응답**

```
{
result: "success"
}
```

또는

```
{
result: "fail"
}
```

**예**

`https://www.acme.com/api/upload?id=1234 [document bytes included in update stream]`

응답

```
{
result:"success"
}
```
