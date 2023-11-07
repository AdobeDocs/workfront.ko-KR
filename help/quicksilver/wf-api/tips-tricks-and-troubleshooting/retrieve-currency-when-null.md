---
content-type: api;tips-tricks-troubleshooting
navigation-topic: tips-tricks-and-troubleshooting-workfront-api
title: 통화가 null일 때 프로젝트에 대한 통화 정보 검색
description: 통화가 null일 때 프로젝트에 대한 통화 정보 검색
author: Becky
feature: Workfront API
role: Developer
exl-id: 31ed533b-be19-4ccb-aad4-7c78e008b3e9
source-git-commit: 14ff8da8137493e805e683e5426ea933f56f8eb8
workflow-type: tm+mt
source-wordcount: '121'
ht-degree: 0%

---

# 통화가 null(지정되지 않음)인 경우 프로젝트에 대한 통화 정보 검색

통화 필드가 있는 프로젝트 개체는 다음 요청을 사용하여 검색할 수 있습니다.

```
GET /attask/api-internal/project/{{projectID}}?fields=currency
```

그러면 다음 응답 본문이 반환됩니다.

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

프로젝트(예: 계산)에 통화가 필요한 경우 고객에 대한 기본 통화를 검색할 수 있습니다.

`GET /attask/api-internal/CUST/currentCustomer?fields=currency`

응답에는 사용자가 기본값으로 설정한 통화가 포함되며, 이 통화는 설정된 통화가 없는 고객을 위한 프로젝트에서 사용됩니다.

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
