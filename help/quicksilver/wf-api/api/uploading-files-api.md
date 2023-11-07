---
content-type: api
navigation-topic: api-navigation-topic
title: API를 통해 파일 업로드
description: API를 통해 파일 업로드
author: Becky
feature: Workfront API
role: Developer
exl-id: 4e0b73b6-0d6d-4971-a87a-dfec85fb031a
source-git-commit: 3e339e2bfb26e101f0305c05f620a21541394993
workflow-type: tm+mt
source-wordcount: '176'
ht-degree: 0%

---

# API를 통해 파일 업로드

Postman과 같은 API 도구 또는 간단한 cURL 명령을 사용하여 Workfront API를 사용하여 파일을 업로드할 수 있습니다.

문서를 업로드하려면 다음 지침을 참조하십시오. **문서 업로드** Workfront에서 [게시물 비헤이비어](/help/quicksilver/wf-api/general/api-basics.md#post-behavior). cURL 요청에 대해서도 동일한 지침을 사용할 수 있습니다.

**API 도구를 사용하여 파일을 업로드할 때 다음 지침을 따르십시오.**

* API 도구 옵션을 사용하여 파일을 업로드하십시오. 이는 종종 다음과 같습니다. **파일 선택** 요청 화면의 버튼입니다.

* POST HTTP 메서드를 사용하여 파일 업로드를 요청합니다.

* 요청에 따라 핸들 값이 포함된 응답이 생성되어야 합니다.

* 후속 호출을 수행하려면 JSON 페이로드의 objID에 대한 핸들 값, 개체 유형 및 GUID 값을 사용하십시오. 다음 예제와 같이 파일에 대한 개체를 만들기 위한 것입니다.

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
