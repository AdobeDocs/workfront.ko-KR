---
content-type: api
product-area: documents
navigation-topic: documents-webhooks-api
title: 문서 또는 폴더 이름 바꾸기(아직 구현되지 않음)
description: 문서 또는 폴더 이름 바꾸기
author: Becky
feature: Workfront API, Digital Content and Documents
exl-id: 5b1a4a02-a7fd-41f2-9adb-74b40606270b
source-git-commit: f050c8b95145552c9ed67b549608c16115000606
workflow-type: tm+mt
source-wordcount: '81'
ht-degree: 6%

---


# 문서 또는 폴더 이름 바꾸기(아직 구현되지 않음)

외부 시스템에서 지정된 ID로 문서 또는 폴더의 이름을 변경합니다.

**URL**

PUT/이름 바꾸기

## 쿼리 매개 변수

| 이름  | 설명 |
|---|---|
| id | 이름을 바꿀 문서 또는 폴더 ID |
| 이름  | 문서 또는 폴더의 새 이름 |


## 응답

아래 오류 처리 섹션에 지정된 대로 성공 또는 실패를 나타내는 JSON 문자열입니다.

**예:** PUT https://www.acme.com/api/rename

```
-------------------------------

id=1234

name=Folder B ­­­­­­­­­­­­­­­­­­­­­­­­­­­­­­­­­­­­

-------------------------------
```

반환

```
{status: “success”
 }returns
 {
 status: “failure”, error: “Folder cannot be renamed because a folder with that name already exists.”
 }
```
