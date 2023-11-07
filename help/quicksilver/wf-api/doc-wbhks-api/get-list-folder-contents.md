---
content-type: api
product-area: documents
navigation-topic: documents-webhooks-api
title: 파일 또는 폴더의 메타데이터 나열
description: 파일 또는 폴더의 메타데이터 나열
author: Becky
feature: Workfront API
role: Developer
exl-id: 9c9f9222-59ac-4643-8297-d4939bec7e64
source-git-commit: 14ff8da8137493e805e683e5426ea933f56f8eb8
workflow-type: tm+mt
source-wordcount: '100'
ht-degree: 7%

---


# 폴더 컨텐츠의 항목 목록 가져오기

지정된 폴더의 파일 및 폴더에 대한 메타데이터를 나열합니다.

**URL**

GET /files

## 쿼리 매개변수

| 이름  | 설명 |
|---|---|
| parentId  | 폴더 ID입니다. 루트 디렉토리의 메타데이터를 가져오려면 값 &#39;/&#39;를 사용합니다. |
| 최대  | 반환할 최대 항목 수입니다. 페이지 매김에 사용됩니다. |
| offset  |  &#39;max&#39;와 함께 사용되는 페이지 오프셋입니다. |


## 응답

파일 및 폴더 목록이 포함된 JSON. 각 항목에 대한 메타데이터는 /metadata 끝점에서 반환되는 메타데이터와 동일합니다.

**예:** https://www.acme.com/api/files?parentId=123456

```
[ 
{
title:"Folder A",
kind:"folder"
id":"2lj23lkj",
viewLink:" https://www.acme.com/viewDocument?id=2lj23lkj ",
downloadLink:"https://www.acme.com/downloadDocument?id=2lj23lkj",
mimeType:"",
dateModified:"2014­06­05T17:39:45.251Z"
size: ""
},
{
title:"My Document",
kind:"file"
id":"da8cj234",
viewLink:" https://www.acme.com/viewDocument?id=da8cj234 ",
downloadLink:"https://www.acme.com/downloadDocument?id=da8cj234",
mimeType:"image/png",
dateModified:"2014­06­05T17:39:45.251Z"
size: "32554694"
}
]
```
