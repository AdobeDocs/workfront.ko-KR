---
content-type: api;tips-tricks-troubleshooting
navigation-topic: tips-tricks-and-troubleshooting-workfront-api
title: OPTASK copyIssue에 대한 옵션 구성
description: copyIssue 끝점에 필요한 정수 값에 대한 설명입니다.
author: Becky
feature: Workfront API
exl-id: a2b8ef01-1c14-47a5-8b0a-550b17b526ff
source-git-commit: 93a67b3dbd59f188dad6b060ec93c3f137c981b2
workflow-type: tm+mt
source-wordcount: '117'
ht-degree: 6%

---

# OPTASK copyIssue에 대한 옵션 구성


copyIssue API 호출에 대한 속성 중 하나는 라는 필드입니다 `options`. 이 필드에는 정수가 필요합니다.

다음 옵션 중 하나를 포함하려면 일치하는 정수를 입력합니다. 두 개 이상의 옵션을 포함하려면 일치하는 정수의 합계를 입력합니다.

| 옵션 | value* |
|---|---|
| 지정 지우기 | 2 |
| 진행률 지우기 | 4 |
| 문서 지우기 | 128 |
| 업데이트 지우기 | 65536 |
| 권한 지우기 | 524288 |
| 사용자 지정 데이터 지우기 | 1048576 |

*모든 값은 2의 권력입니다.

예:

* 문제를 복사할 때 진행 상태를 지우려면 `options` 값 `4`.

* 진행 상황과 문서를 모두 지우려면 `options` 값 `132`.

   진행률 지우기 = 4

   문서 지우기 = 128

   4 + 128 = 132
