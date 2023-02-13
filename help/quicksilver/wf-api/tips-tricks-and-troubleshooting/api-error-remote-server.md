---
content-type: api;tips-tricks-troubleshooting
navigation-topic: tips-tricks-and-troubleshooting-workfront-api
title: API 오류 메시지 400 잘못된 요청
description: API 오류 메시지 400 잘못된 요청
author: John
feature: Workfront API
exl-id: ab7c76a9-16ce-41f9-b7af-5943eb2dfdff
source-git-commit: 368a634b09d38a5b61c3e320f3f72e896694eeb1
workflow-type: tm+mt
source-wordcount: '90'
ht-degree: 0%

---


# API 오류: &quot;원격 서버에서 오류(400) 잘못된 요청을 반환했습니다.&quot;

## 문제

API를 사용하여 사용자 지정 필드를 문제에 가져오려고 하면 다음 오류가 발생합니다.

`The remote server returned an error: (400) Bad Request`

## 원인

이 오류는 API를 통해 큐 항목과 연결된 사용자 지정 양식이 없는 프로젝트의 사용자 지정 필드를 가져오려고 할 때 발생합니다.

## 솔루션

큐 항목에 올바른 사용자 지정 양식을 추가합니다.

큐 항목에 대한 자세한 내용은 [큐 항목 만들기](../../manage-work/requests/create-and-manage-request-queues/create-queue-topics.md).
