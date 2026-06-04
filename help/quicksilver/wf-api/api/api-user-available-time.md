---
content-type: api
navigation-topic: wf-api
title: 사용 가능한 시간 API 사용자 가져오기
description: 사용 가능한 시간 API 사용자 가져오기
author: Becky
feature: Workfront API
role: Developer
exl-id: fa37920a-c08b-4af3-9896-7e4044834860
TQID: https://experienceleague.adobe.com/JPvalH2RQRfMeqbYyWXyjyXCx-bdaZwRoR6WDRerZ5U
product_v2:
  - id: c4a86a5d-6562-4fc6-aa00-bfa25833aed9
feature_v2:
  - id: f48b5020-b9cd-4d99-bc6e-42c35e90c1f8
role_v2:
  - id: ff6a42d2-313e-452e-93a6-792e4fad9ff8
source-git-commit: 55a9d9feae8cc1128e3427a8874414ba734dd467
workflow-type: tm+mt
source-wordcount: 95
ht-degree: 4%

---

# 사용자 사용 가능 시간 API

**URI: attask/api/v15.0/user/getUsersAvailableTime**

사용자 사용 가능한 시간 엔드포인트는 사용자의 사용 가능한 시간에 대한 데이터를 검색합니다. 이를 통해 사용자 특성 및 시간 간격에 따른 데이터 집계를 위한 통합이 가능합니다.

## 요청 예

`curl -XPUT /attask/api/v15.0/user/getUsersAvailableTime`

## 요청 매개 변수

* **userIDs**: 문자열 배열입니다. 필수 여부. 예: `"61a9cc0500002f9fdaa7a6f824f557e1"`.

* **fromDate**: datetime. 문자열. 필수 여부. 예: `"2022-07-10T00:00:00"`

* **toDate**: 날짜/시간입니다. 문자열. 필수 여부. 예 `"2022-07-20T23:59:59"`.

## 응답 예:

```
{
    "data": {
        "result": {
            "PAVL": {
                "61a9cc0500002f9fdaa7a6f824f557e1": [
                    0.0,
                    480.0,
                    480.0,
                    480.0,
                    480.0,
                    480.0,
                    0.0,
                    0.0,
                    480.0,
                    480.0,
                    480.0
                ]
            },
            "AVL": {
                "61a9cc0500002f9fdaa7a6f824f557e1": [
                    0.0,
                    480.0,
                    480.0,
                    480.0,
                    480.0,
                    0.0,
                    480.0,
                    0.0,
                    480.0,
                    480.0,
                    480.0
                ]
            }
        }
    }
}
```

## 응답 매개 변수

* **AVL**: 실제 사용 가능한 시간. 숫자 배열.
* **PAVL**: 휴무일 또는 사용자 휴무를 포함하지 않는 예약에 사용 가능한 시간입니다. 문자열.
