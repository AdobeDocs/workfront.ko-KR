---
content-type: api;tips-tricks-troubleshooting
navigation-topic: tips-tricks-and-troubleshooting-workfront-api
title: OPTASK copyIssue에 대한 옵션 구성
description: copyIssue 끝점에 필요한 정수 값에 대한 설명입니다.
author: Becky
feature: Workfront API
role: Developer
exl-id: a2b8ef01-1c14-47a5-8b0a-550b17b526ff
TQID: https://experienceleague.adobe.com/9cDJFoKl6zqpaAvqzpGqzflcbGZNrAWvEnUAFuqD-Rc
product_v2:
  - id: c4a86a5d-6562-4fc6-aa00-bfa25833aed9
feature_v2:
  - id: b58ad82f-df6b-4b01-81a3-3a02ab9567a0
role_v2:
  - id: ff6a42d2-313e-452e-93a6-792e4fad9ff8
topic_v2:
  - id: c1579802-ddd4-4214-8a91-97b2066abe11
source-git-commit: 55a9d9feae8cc1128e3427a8874414ba734dd467
workflow-type: tm+mt
source-wordcount: 122
ht-degree: 8%

---

# OPTASK copyIssue에 대한 옵션 구성


copyIssue API 호출에 대한 속성 중 하나는 이름이 `options`인 필드입니다. 이 필드에는 정수가 필요합니다.

다음 옵션 중 하나를 포함하려면 일치하는 정수를 입력합니다. 두 개 이상의 옵션을 포함하려면 일치하는 정수의 합계를 입력합니다.

| 옵션 | 값* |
|---|---|
| 할당 지우기 | 2 |
| 진행 상황 지우기 | 4 |
| 문서 지우기 | 128 |
| 업데이트 지우기 | 65536 |
| 권한 지우기 | 524288 |
| 사용자 정의 데이터 지우기 | 1048576 |

*모든 값은 2의 거듭제곱입니다.

예:

* 문제를 복사할 때 진행 상황을 지우려면 `4`의 `options` 값을 입력하십시오.

* 진행률과 문서를 모두 지우려면 `132`의 `options` 값을 입력하십시오.

  진행 상황 지우기 = 4

  문서 지우기 = 128

  4 + 128 = 132
