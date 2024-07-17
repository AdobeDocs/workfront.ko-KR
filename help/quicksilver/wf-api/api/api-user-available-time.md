---
content-type: api
navigation-topic: wf-api
title: 사용 가능한 시간 API 사용자 가져오기
description: 사용 가능한 시간 API 사용자 가져오기
author: Becky
feature: Workfront API
role: Developer
exl-id: fa37920a-c08b-4af3-9896-7e4044834860
source-git-commit: 3e339e2bfb26e101f0305c05f620a21541394993
workflow-type: tm+mt
source-wordcount: '94'
ht-degree: 0%

---

# 사용자 사용 가능 시간 API

**URI: attask/api/v15.0/user/getUsersAvailableTime**

사용자 사용 가능한 시간 엔드포인트는 사용자의 사용 가능한 시간에 대한 데이터를 검색합니다. 이를 통해 사용자 특성 및 시간 간격에 따른 데이터 집계를 위한 통합이 가능합니다.

## 요청 예

`curl -XPUT /attask/api/v15.0/user/getUsersAvailableTime`

## 요청 매개 변수

* **userIDs**: 문자열 배열입니다. 필수. 예: `"61a9cc0500002f9fdaa7a6f824f557e1"`

* **fromDate**: datetime. 문자열. 필수. 예: `"2022-07-10T00:00:00"`

* **toDate**: 날짜/시간입니다. 문자열. 필수. 예 `"2022-07-20T23:59:59"`.

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
