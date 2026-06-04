---
content-type: api
product-area: documents
navigation-topic: documents-webhooks-api
title: 문서 웹후크 오류 처리
description: 문서 웹후크 오류 처리
author: Becky
feature: Workfront API
role: Developer
exl-id: 6e0f3be7-5321-44bd-a404-d5bef1462d82
TQID: https://experienceleague.adobe.com/KoMJXXZbDdywLGIwYTu7o8GigPxQ5RG6sNQpOTMHWY0
product_v2:
  - id: c4a86a5d-6562-4fc6-aa00-bfa25833aed9
role_v2:
  - id: ff6a42d2-313e-452e-93a6-792e4fad9ff8
source-git-commit: 55a9d9feae8cc1128e3427a8874414ba734dd467
workflow-type: tm+mt
source-wordcount: 123
ht-degree: 0%

---

# 문서 웹후크 오류 처리

API 요청을 처리할 때 문제가 발생할 수 있습니다. 모든 API 엔드포인트에서 일관된 방식으로 처리해야 합니다. 오류가 발생하면 웹후크 공급자는 응답 헤더에 오류 코드를 포함해야 합니다. 오류 코드는 다음과 같습니다.

* 403 - 사용할 수 없음. 요청 토큰이 누락되었거나 잘못되었거나 토큰과 연결된 자격 증명에 지정된 리소스에 대한 액세스 권한이 없음을 나타냅니다. OAuth 기반 웹후크 공급자의 경우 Adobe Workfront은 새 액세스 토큰 검색을 시도합니다.

* 404 - 찾을 수 없음. 지정한 파일 또는 폴더가 없음을 나타냅니다.

* 500 - 내부 서버 오류. 기타 모든 유형의 오류.

* 다음 형식을 사용하여 응답 본문의 오류에 대한 설명:

  ```
  {status: "error"
   error: "Sample error message"}
  ```
