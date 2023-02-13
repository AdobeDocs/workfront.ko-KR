---
content-type: api
navigation-topic: api-navigation-topic
title: API를 통해 파일 업로드
description: API를 통해 파일 업로드
author: John
feature: Workfront API
exl-id: 4e0b73b6-0d6d-4971-a87a-dfec85fb031a
source-git-commit: 03df0ad329255e86780c03bbb4541e0a0a526381
workflow-type: tm+mt
source-wordcount: '188'
ht-degree: 0%

---

# API를 통해 파일 업로드

Postman과 같은 API 도구가 있는 Workfront API 또는 간단한 cURL 명령을 사용하여 파일을 업로드할 수 있습니다.

문서를 업로드하려면 다음 지침에 대해 **문서 업로드** Workfront [게시물 동작](https://one.workfront.com/s/document-item?bundleId=the-new-workfront-experience&amp;topicId=Content%2FWF_API%2FGeneral%2Fapi-basics.html). cURL 요청에 이와 동일한 지침을 사용할 수도 있습니다.

**API 도구를 사용하여 파일을 업로드할 때에는 다음 지침을 따르십시오.**

* API 도구 옵션을 사용하여 파일을 업로드합니다. 종종 **파일 선택** 단추를 클릭합니다.

* 파일 업로드를 요청하려면 POST HTTP 메서드를 사용합니다.

* 요청에 따라 해당 핸들에 대한 값이 포함된 응답이 발생합니다.

* JSON 페이로드에서 objID에 대한 핸들 값, 개체 유형 및 GUID 값을 사용하여 후속 호출을 수행하십시오. 다음 예와 같이 파일에 대한 개체를 만들기 위한 것입니다.

```
}
"name": "TestPDF",
"handle": "7af257e64aba4a22c33ccdfc40bbb87",
"docObjCode": "PROJ",
"objID": "0398450f8345980843445534354",
"currentVersion": {"version": "v1.0", "fileName" : "TestPDF"},
}
```

응답에서 개체의 ID를 받아야 합니다.

자세한 내용은 사용 중인 특정 API 도구의 도움말을 참조하십시오.
