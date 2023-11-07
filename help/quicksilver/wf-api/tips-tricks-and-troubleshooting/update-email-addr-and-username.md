---
content-type: api;tips-tricks-troubleshooting
navigation-topic: workfront-api
title: emailAddr으로 업데이트해도 사용자 이름이 업데이트되지 않음
description: 이메일 주소 업데이트로 사용자 이름이 업데이트되지 않음
author: Becky
feature: Workfront API
role: Developer
exl-id: 2d24d1b8-9504-484f-9cc0-d2f1abd6391a
source-git-commit: 14ff8da8137493e805e683e5426ea933f56f8eb8
workflow-type: tm+mt
source-wordcount: '231'
ht-degree: 0%

---


# emailAddr으로 업데이트해도 사용자 이름이 업데이트되지 않음

## 문제

일반적으로, `emailAddr` 및 `username` 는 동일한 속성입니다. 따라서 사용자의 `emailAddr` 속성, `username` 속성은 일치하도록 자동으로 업데이트됩니다.

다음의 경우 `username` 이(가) 와(과) 일치하지 않음 `emailAddr`, 업데이트 `emailAddr` 을(를) 업데이트하지 않습니다. `username` 자동으로 표시됩니다. 이는 두 가지 모두에 해당됩니다 `emailAddr` 는 사용자 인터페이스 및 API를 통해 변경됩니다.

## 원인

불일치는 다음과 같은 여러 가지 방법으로 만들 수 있습니다.

* 동기화 규칙이 존재하기 전에 생성된 사용자입니다. 매우 오래된 사용자 계정에는 이러한 속성이 동기화되지 않을 수 있습니다.

* Workfront의 emailAddr이 대소문자를 구분했을 때 SSO를 통해 생성된 사용자입니다. SSO 자동 프로비저닝 옵션은 ID 공급자의 사용자 속성을 기반으로 사용자에 대해 대/소문자 검사를 실행합니다. 정확히 일치하는 항목이 없으면 자동 프로비저닝 서비스에서 새 사용자를 만듭니다. 사용자가 이미 있는 경우 사용자 이름과 `emailAddr` 는 동일한 케이스가 없습니다.

* 을(를) 가진 사용자 `username` API를 통해 직접 업데이트된 속성 및 해당 `emailAddr` 업데이트되지 않았습니다. 다음 `username` 및 `emailAddr` 일치하지 않을 수 있습니다.

## 솔루션

API를 사용하여 `username` 속성이 과 동일해야 함 `emailAddr`. 속성을 동기화한 후 `emailAddr` 은(는) 도 업데이트합니다. `username` 일치하는 사용자 이름 필드가 업데이트에 포함되지 않은 경우.
