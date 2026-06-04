---
content-type: api;tips-tricks-troubleshooting
navigation-topic: tips-tricks-and-troubleshooting-workfront-api
title: API 오류 메시지 400 잘못된 요청
description: API 오류 메시지 400 잘못된 요청
author: Becky
feature: Workfront API
role: Developer
exl-id: ab7c76a9-16ce-41f9-b7af-5943eb2dfdff
TQID: https://experienceleague.adobe.com/19PIdv4u8de0BlasXD0Yy6GssO3vv6Jt8BzcljB-m1w
product_v2: id: c4a86a5d-6562-4fc6-aa00-bfa25833aed9
feature_v2: id: b58ad82f-df6b-4b01-81a3-3a02ab9567a0
role_v2: id: ff6a42d2-313e-452e-93a6-792e4fad9ff8
topic_v2: id: c1579802-ddd4-4214-8a91-97b2066abe11
source-git-commit: 55a9d9feae8cc1128e3427a8874414ba734dd467
workflow-type: tm+mt
source-wordcount: 93
ht-degree: 2%

---

# API 오류: &quot;원격 서버가 오류(400) 잘못된 요청을 반환했습니다.&quot;

## 문제

API를 사용하여 사용자 정의 필드를 문제로 가져오는 도중 다음 오류가 발생했습니다.

`The remote server returned an error: (400) Bad Request`

## 원인

이 오류는 큐 주제와 연결된 사용자 정의 양식이 없는 프로젝트에서 API를 통해 사용자 정의 필드를 가져오려고 할 때 발생합니다.

## 솔루션

대기열 주제에 올바른 사용자 정의 양식을 추가합니다.

대기열 주제에 대한 자세한 내용은 [대기열 주제 만들기](../../manage-work/requests/create-and-manage-request-queues/create-queue-topics.md)를 참조하십시오.
