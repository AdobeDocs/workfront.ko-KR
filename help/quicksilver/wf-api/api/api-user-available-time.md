---
content-type: api
navigation-topic: wf-api
title: 사용자 사용 가능한 시간 API 가져오기
description: 사용자 사용 가능한 시간 API 가져오기
author: John
feature: Workfront API
exl-id: fa37920a-c08b-4af3-9896-7e4044834860
source-git-commit: aea37c1d200dfadf9ccbb7b36145eb04d5ab4b6d
workflow-type: tm+mt
source-wordcount: '94'
ht-degree: 7%

---

# 사용 가능한 시간 API 사용자

**URI: attask/api/v15.0/user/getUsersAvailableTime**

사용 가능한 시간 끝점은 사용자가 사용 가능한 시간에 데이터를 검색합니다. 이를 통해 사용자 특성 및 시간 간격에 따라 데이터를 수집할 수 있습니다.

## 요청 예

`curl -XPUT /attask/api/v15.0/user/getUsersAvailableTime`

## 요청 매개 변수

* **userIDs**: 문자열의 배열입니다. 필수. 예: `"61a9cc0500002f9fdaa7a6f824f557e1"`.

* **fromDate**: datetime. 문자열. 필수. 예:  `"2022-07-10T00:00:00"`.

* **toDate**: datetime. 문자열. 필수. 예 `"2022-07-20T23:59:59"`.

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

* **AVL**: 실제 사용 가능 시간 숫자 배열입니다.
* **PAVL**: 비근무 일수 또는 사용자 타임오프가 포함되지 않는 예약에 사용할 수 있는 순수 시간입니다. 문자열.
