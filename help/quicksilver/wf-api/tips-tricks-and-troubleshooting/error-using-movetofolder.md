---
content-type: api;tips-tricks-troubleshooting
navigation-topic: tips-tricks-and-troubleshooting-workfront-api
title: 문서 moveToFolder 작업이 작동하지 않음
description: Document moveToFolder 작업을 사용할 때 422 오류가 반환됩니다.
author: Becky
feature: Workfront API
role: Developer
exl-id: 811efabc-e101-4de5-a800-a1447654dc3e
TQID: https://experienceleague.adobe.com/UV4VnQEs-jGJau1UqXTLnp7Ak-cmKRpjuJqxgNTF5z8
product_v2:
  - id: c4a86a5d-6562-4fc6-aa00-bfa25833aed9
feature_v2:
  - id: b58ad82f-df6b-4b01-81a3-3a02ab9567a0
role_v2:
  - id: ff6a42d2-313e-452e-93a6-792e4fad9ff8
topic_v2:
  - id: c1579802-ddd4-4214-8a91-97b2066abe11
source-git-commit: 55a9d9feae8cc1128e3427a8874414ba734dd467
workflow-type: tm+mt
source-wordcount: 121
ht-degree: 1%

---

# 문서 moveToFolder 작업이 작동하지 않음

## 문제

문서 개체의 `moveToFolder` 작업을 사용하는 경우 422 오류가 반환됩니다.

또는

Workfront Fusion의 Adobe Authenticator 모듈을 통해 이 작업을 사용하는 경우 문서가 이동되지 않지만 오류가 표시되지는 않습니다. 오류는 동일하지만 Adobe Authenticator 모듈에 표시되지 않습니다.

## 솔루션

이 액션에 대한 422 오류의 한 가지 가능한 원인은 이 액션이 한 연결된 폴더에 있는 문서를 다른 연결된 폴더로 이동하려고 시도하기 때문입니다.

이동할 문서가 이미 연결된 폴더에 있는지 확인합니다.
