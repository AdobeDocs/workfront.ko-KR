---
content-type: api
product-area: documents
navigation-topic: documents-webhooks-api
title: 문서 웹 후크 오류 처리
description: 문서 웹 후크 오류 처리
author: John
feature: Workfront API
exl-id: 6e0f3be7-5321-44bd-a404-d5bef1462d82
source-git-commit: 338cc745a7660ffed8e4d44e19dcadfdc13bc345
workflow-type: tm+mt
source-wordcount: '119'
ht-degree: 0%

---

# 문서 웹 후크 오류 처리

API 요청을 처리할 때 문제가 발생할 수 있습니다. 모든 API 엔드포인트에서 일관되게 처리되어야 합니다. 오류가 발생하면 웹 후크 공급자에 응답 헤더에 오류 코드가 포함되어야 합니다. 오류 코드는 다음과 같습니다.

* 403 - 금지. 요청 토큰이 없거나 잘못되었거나 토큰과 연결된 자격 증명에 지정된 리소스에 대한 액세스 권한이 없음을 나타냅니다. OAuth 기반 웹 후크 공급자의 경우 Adobe Workfront은 새 액세스 토큰을 검색하려고 합니다.

* 404 - 없음. 지정한 파일 또는 폴더가 없음을 나타냅니다.

* 500 - 내부 서버 오류 다른 유형의 오류입니다.

* 다음 형식을 사용하여 응답 본문에 있는 오류에 대한 설명입니다.

   ```
   {status: “error”
    error: “Sample error message”}
   ```
