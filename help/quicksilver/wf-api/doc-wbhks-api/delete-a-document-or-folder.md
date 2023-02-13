---
content-type: api
product-area: documents
navigation-topic: documents-webhooks-api
title: 문서 또는 폴더 삭제
description: 문서 또는 폴더 삭제
author: John
feature: Workfront API
exl-id: b56ec13a-1ee1-4bef-b39b-e625d00e4952
source-git-commit: 9de8ee7fad2a3cb67c4fc6bfdff4d6ce50f15afd
workflow-type: tm+mt
source-wordcount: '82'
ht-degree: 6%

---


# 문서 또는 폴더 삭제(아직 구현되지 않음)

외부 시스템에서 해당 ID가 있는 문서 또는 폴더를 삭제합니다. 폴더를 삭제하면 폴더 내용도 삭제됩니다.

## URL

PUT/삭제

## 쿼리 매개 변수

| 이름  | 설명 |
|---|---|
| documentId  | 삭제할 문서 ID |
| folderId  |  삭제할 폴더 ID |



## 응답

아래 오류 처리 섹션에 지정된 대로 성공 또는 실패를 나타내는 JSON 문자열입니다.

### 예

PUT https://www.example.com/api/deleteid=1234
* 반환 `status: “success”`

* 반환 `status: “failure”, error: “File not found”`
