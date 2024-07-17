---
content-type: api;tips-tricks-troubleshooting
navigation-topic: tips-tricks-and-troubleshooting-workfront-api
title: API 오류 메시지 400 잘못된 요청
description: API 오류 메시지 400 잘못된 요청
author: Becky
feature: Workfront API
role: Developer
exl-id: ab7c76a9-16ce-41f9-b7af-5943eb2dfdff
source-git-commit: 14ff8da8137493e805e683e5426ea933f56f8eb8
workflow-type: tm+mt
source-wordcount: '93'
ht-degree: 0%

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
