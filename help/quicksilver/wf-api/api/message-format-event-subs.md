---
content-type: api
navigation-topic: api-navigation-topic
title: 이벤트 구독에 대한 아웃바운드 메시지 형식
description: 이벤트 구독에 대한 아웃바운드 메시지 형식
author: Becky
feature: Workfront API
role: Developer
exl-id: addcf5bc-a101-4bb0-93a6-46b4af67c848
source-git-commit: 3e339e2bfb26e101f0305c05f620a21541394993
workflow-type: tm+mt
source-wordcount: '255'
ht-degree: 0%

---

# 이벤트 구독에 대한 아웃바운드 메시지 형식

Adobe Workfront 2017.3 릴리스에서는 이벤트 구독에 대한 아웃바운드 메시지 형식이 변경되어 통합을 위한 이벤트 구독의 성능 향상 및 더 나은 사용을 허용합니다.

## 아웃바운드 메시지 형식 업데이트

아웃바운드 메시지 형식이 다음과 같이 변경됩니다.

* 아웃바운드 메시지에는 Workfront 리소스에 대한 oldState 및 newState가 포함됩니다.

  이 값은 Workfront의 이벤트로 인해 객체가 변경된 사항을 보여 줍니다.

* eventTime 메타데이터 필드가 모든 아웃바운드 메시지에 추가됩니다.

  이 필드는 이벤트가 발생한 시간을 Nanoseconds 및 EpochSeconds로 표시합니다. 통합에서 처리한 이벤트를 정렬할 때 eventTime을 사용합니다.

* NOTE 리소스의 owner:companyID 참조 필드가 제거됩니다.
* CurrentVersion 참조된 objectDOCU(문서) 리소스에서 제거됩니다.

현재 Workfront 이벤트 구독을 사용하는 경우 이러한 변경 사항을 적용하려면 2017.3 릴리스 전에 Workfront 통합을 업데이트해야 합니다.

이벤트 구독에 대한 자세한 내용은 [이벤트 구독 API](../../wf-api/general/event-subs-api.md)를 참조하세요.

## 이전 및 새 메시지 형식 샘플

다음 이전 형식의 CREATE 메시지는 2017.3 릴리스 이후 더 이상 사용되지 않습니다.

```
{
  "eventType": "CREATE",
  "subscriptionId": "8a0d839d5ef32c9a015ef33064b00001",
  "fields": {
     "ID": "59d7db3c0000014b05536251b669a3e4",
     "name": "EventSub Test 53350c27-ce58-40e9-af75-a2d45ff13046",
     "objCode": "PROJ",
     "entryDate": "2017-10-06T13:36:28.722-0600",
     "accessorIDs": ["544820df0000142362741fc0c368de19"],
     "lastUpdateDate": "2017-10-06T13:36:28.785-0600",
     "groupID": "544820df0000140f6a9c1faa7cacadd3",
     "sponsorID": null,
     "description": null,
     "plannedCompletionDate": "2017-10-06T09:00:00.000-0600",
     "enteredByID": "544820df0000142362741fc0c368de19",
     "ownerID": "544820df0000142362741fc0c368de19",
     "templateID": null,
     "priority": 0,
     "companyID": null,
     "portfolioID": null,
     "referenceNumber": 1891,
     "lastUpdatedByID": "544820df0000142362741fc0c368de19",
     "customerID": "544820df0000135b7719dcca654391f6",
     "currency": null,
     "categoryID": null,
     "status": "CUR",
     "parameterValues": {}
  }
}
```

다음 새 형식 CREATE 메시지는 2017.3 릴리스 이후에 사용됩니다.

```
{
   "eventType": "CREATE",
   "subscriptionId": "8a0d839d5ef32c9a015ef32e2cde0000",
   "eventTime": {
      "nano": 414000000,
      "epochSecond": 1507318444
   },
   "newState": {
     "ID": "59d7daab0000011b8faebf0f60d25d08",
     "name": "EventSub Test 3700e224-0ef7-4571-b200-09109712152c",
     "objCode": "PROJ",
     "entryDate": "2017-10-06T13:34:03.562-0600",
     "accessorIDs": ["544820df0000142362741fc0c368de19"],
     "lastUpdateDate": "2017-10-06T13:34:04.000-0600",
     "groupID": "544820df0000140f6a9c1faa7cacadd3",
     "sponsorID": null,
     "description": null,
     "plannedCompletionDate": "2017-10-06T09:00:00.000-0600",
     "enteredByID": "544820df0000142362741fc0c368de19",
     "ownerID": "544820df0000142362741fc0c368de19",
     "templateID": null,
     "priority": 0,
     "companyID": null,
     "portfolioID": null,
     "referenceNumber": 1890,
     "lastUpdatedByID": "544820df0000142362741fc0c368de19",
     "customerID": "544820df0000135b7719dcca654391f6",
     "currency": null,
     "categoryID": null,
     "status": "CUR",
     "parameterValues": {}
   },
   "oldState": {}
```

다음 이전 형식의 UPDATE 메시지는 2017.3 릴리스 이후 더 이상 사용되지 않습니다.

```
{
     "eventType": "UPDATE",
     "subscriptionId": "8a0d839d5ef32c9a015ef336a5ed0002",
     "fields": {
     "ID": "59d7dcde000001b2330bda8ac63fee16",
     "name": "EventSub Test updated",
     "objCode": "PROJ",
     "entryDate": "2017-10-06T13:43:26.305-0600",<
     "accessorIDs": [
        "544820df0000142362741fc0c368de19"
     ],
     "lastUpdateDate": "2017-10-06T13:43:49.265-0600",
     "groupID": "544820df0000140f6a9c1faa7cacadd3",
     "sponsorID": null,
     "description": null,
     "plannedCompletionDate": "2017-10-06T09:00:00.000-0600",
     "enteredByID": "544820df0000142362741fc0c368de19",
     "ownerID": "544820df0000142362741fc0c368de19",
     "templateID": null,
     "priority": 0,
     "companyID": null,
     "portfolioID": null,
     "referenceNumber": 1892,
     "lastUpdatedByID": "544820df0000142362741fc0c368de19",
     "customerID": "544820df0000135b7719dcca654391f6",
     "currency": null,
     "categoryID": null,
     "status": "CUR",
     "parameterValues": {}
   }
 }
```

다음 새 형식 UPDATE 메시지는 2017.3 릴리스 이후에 사용됩니다.

```
{
   "eventType": "UPDATE",
   "subscriptionId": "8a0d839d5ef32c9a015ef336a5ed0002",
   "eventTime": {
     "nano": 998000000,
     "epochSecond": 1507319336
   },
   "newState": {
     "ID": "59d7ddf7000002322d791eb08bafddfb",
     "name": "EventSub Test updated",
     "objCode": "PROJ",
     "entryDate": "2017-10-06T13:48:07.776-0600",
     "accessorIDs": [
        "544820df0000142362741fc0c368de19"
     ],
     "lastUpdateDate": "2017-10-06T13:48:56.980-0600",
     "groupID": "544820df0000140f6a9c1faa7cacadd3",
     "sponsorID": null,
     "description": null,
     "plannedCompletionDate": "2017-10-06T09:00:00.000-0600",
     "enteredByID": "544820df0000142362741fc0c368de19",
     "ownerID": "544820df0000142362741fc0c368de19",
     "templateID": null,
     "priority": 0,
     "companyID": null,
     "portfolioID": null,
     "referenceNumber": 1894,
     "lastUpdatedByID": "544820df0000142362741fc0c368de19",
     "customerID": "544820df0000135b7719dcca654391f6",
     "currency": null,
     "categoryID": null,
     "status": "CUR",
     "parameterValues": {}
  },
  "oldState": {
     "ID": "59d7ddf7000002322d791eb08bafddfb",
     "name": "EventSub Test 180fd595-63fb-4fa9-bd47-58bf6e53d964",
     "objCode": "PROJ",
     "entryDate": "2017-10-06T13:48:07.776-0600",
     "accessorIDs": [
        "544820df0000142362741fc0c368de19"
     ],
     "lastUpdateDate": "2017-10-06T13:48:07.792-0600",
     "groupID": "544820df0000140f6a9c1faa7cacadd3",
     "sponsorID": null,
     "description": null,
     "plannedCompletionDate": "2017-10-06T09:00:00.000-0600",
     "enteredByID": "544820df0000142362741fc0c368de19",
     "ownerID": "544820df0000142362741fc0c368de19"
     "templateID": null,
     "priority": 0,
     "companyID": null,
     "portfolioID": null,
     "referenceNumber": 1894,
     "lastUpdatedByID": "544820df0000142362741fc0c368de19",
     "customerID": "544820df0000135b7719dcca654391f6",
     "currency": null,
     "categoryID": null,
     "status": "CUR",
     "parameterValues": {}
  }
}
```
