---
content-type: api
navigation-topic: api-navigation-topic
title: API를 통해 파일 업로드
description: API를 통해 파일 업로드
author: Becky
feature: Workfront API
role: Developer
exl-id: 4e0b73b6-0d6d-4971-a87a-dfec85fb031a
TQID: https://experienceleague.adobe.com/Yd7byYJ1pYDXwdKvINXh4fKy-pWoEiNMj345jr1HHNs
product_v2: id: c4a86a5d-6562-4fc6-aa00-bfa25833aed9
feature_v2: id: b58ad82f-df6b-4b01-81a3-3a02ab9567a0
role_v2: id: ff6a42d2-313e-452e-93a6-792e4fad9ff8
source-git-commit: 55a9d9feae8cc1128e3427a8874414ba734dd467
workflow-type: tm+mt
source-wordcount: 176
ht-degree: 0%

---

# API를 통해 파일 업로드

Postman과 같은 API 도구 또는 간단한 cURL 명령을 사용하여 Workfront API를 사용하여 파일을 업로드할 수 있습니다.

문서를 업로드하려면 Workfront [게시물 동작](/help/quicksilver/wf-api/general/api-basics.md#post-behavior)에서 **문서 업로드**&#x200B;에 대한 지침을 참조하십시오. cURL 요청에 대해서도 동일한 지침을 사용할 수 있습니다.

**API 도구를 사용하여 파일을 업로드할 때 다음 지침을 따르십시오.**

* API 도구 옵션을 사용하여 파일을 업로드하십시오. 요청 화면에 **파일 선택** 단추가 있는 경우가 많습니다.

* POST HTTP 메서드를 사용하여 파일 업로드를 요청합니다.

* 요청에 따라 핸들 값이 포함된 응답이 생성되어야 합니다.

* 후속 호출을 수행하려면 JSON 페이로드의 objID에 대한 핸들 값, 개체 유형 및 GUID 값을 사용하십시오. 다음 예제와 같이 파일에 대한 개체를 만들기 위한 것입니다.

```
{
"name": "TestPDF",
"handle": "7af257e64aba4a22c33ccdfc40bbb87",
"docObjCode": "PROJ",
"objID": "0398450f8345980843445534354",
"currentVersion": {"version": "1", "fileName" : "TestPDF"},
}
```

응답에서 개체의 ID를 받아야 합니다.

자세한 내용은 사용 중인 특정 API 도구의 도움말을 참조하십시오.
