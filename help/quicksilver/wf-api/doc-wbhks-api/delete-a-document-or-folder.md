---
content-type: api
product-area: documents
navigation-topic: documents-webhooks-api
title: 문서 또는 폴더 삭제
description: 문서 또는 폴더 삭제
author: Becky
feature: Workfront API
role: Developer
exl-id: b56ec13a-1ee1-4bef-b39b-e625d00e4952
source-git-commit: 14ff8da8137493e805e683e5426ea933f56f8eb8
workflow-type: tm+mt
source-wordcount: '82'
ht-degree: 8%

---


# 문서 또는 폴더 삭제(아직 구현되지 않음)

외부 시스템에서 특정 ID의 문서 또는 폴더를 삭제합니다. 폴더를 삭제하면 폴더 내용도 삭제됩니다.

## URL

PUT /삭제

## 쿼리 매개변수

| 이름  | 설명 |
|---|---|
| documentId  | 삭제할 문서 ID |
| folderId  |  삭제할 폴더 ID |



## 응답

아래 오류 처리 섹션에 지정된 대로 성공 또는 실패를 나타내는 JSON 문자열입니다.

### 예

PUT https://www.example.com/api/delete­­­­­­­­­­­­­­­­­­­­­­­­­­­­­id=1234
* 반환 `status: "success"`

* 반환 `status: "failure", error: "File not found"`
