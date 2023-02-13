---
content-type: api;tips-tricks-troubleshooting
navigation-topic: tips-tricks-and-troubleshooting-workfront-api
title: 통화가 null일 때 프로젝트에 대한 통화 정보를 검색합니다
description: 통화가 null일 때 프로젝트에 대한 통화 정보를 검색합니다
author: Becky
feature: Workfront API
source-git-commit: a9af457793e123a60172fe4baf5ae5def472b026
workflow-type: tm+mt
source-wordcount: '121'
ht-degree: 0%

---

# 통화가 null(지정되지 않음)인 경우 프로젝트에 대한 통화 정보를 검색합니다.

통화 필드가 있는 프로젝트 개체는 다음 요청을 사용하여 검색할 수 있습니다.

```
GET /attask/api-internal/project/{{projectID}}?fields=currency
```

이렇게 하면 다음 응답 본문이 반환됩니다.

```
{
{
"data": {
"ID": "some_project_id",
"name": "some_project_name",
"objCode": "PROJ",
"currency": "EUR"
}
}
}
```

프로젝트에 대해 통화가 설정되지 않은 경우 이 응답에는 값이 있는 통화가 포함됩니다 `null`:

```
{
{
"data": {
"ID": "some_project_id",
"name": "some_project_name",
"objCode": "PROJ",
"currency": null
}
}
}
```

프로젝트에 대한 통화가 필요한 경우(예: 계산용) 고객에 대한 기본 통화를 검색할 수 있습니다.

`GET /attask/api-internal/CUST/currentCustomer?fields=currency`

응답에는 통화 세트가 없는 해당 고객에 대한 모든 프로젝트에서 사용되는, 사용자가 기본값으로 설정한 통화가 포함됩니다.

```
{
"data": [
{
"ID": "some_customer_id,
"name": "some_customer_name",
"objCode": "CUST",
"currency": "USD"
}
]
}
```
