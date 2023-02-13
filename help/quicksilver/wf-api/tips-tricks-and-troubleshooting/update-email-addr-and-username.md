---
content-type: api;tips-tricks-troubleshooting
navigation-topic: workfront-api
title: emailAddr로 업데이트해도 사용자 이름이 업데이트되지 않습니다
description: emailAddr로 업데이트해도 사용자 이름이 업데이트되지 않습니다
author: John
feature: Workfront API
exl-id: 2d24d1b8-9504-484f-9cc0-d2f1abd6391a
source-git-commit: a939e14cbd6936bdd0c46c1ed641acdda497b8fc
workflow-type: tm+mt
source-wordcount: '231'
ht-degree: 0%

---


# emailAddr로 업데이트해도 사용자 이름이 업데이트되지 않습니다

## 문제

보통 `emailAddr` 및 `username` 는 동일한 속성입니다. 따라서 사용자의 `emailAddr` 속성, `username` 속성이 일치하도록 자동으로 업데이트됩니다.

이 `username` 일치하지 않음 `emailAddr`, 및에 대한 업데이트 `emailAddr` 은 업데이트하지 않습니다 `username` 자동. 이것은 둘 다 사실이다 `emailAddr` 사용자 인터페이스 및 API를 통해 변경됩니다.

## 원인

일치하지 않는 항목은 여러 가지 방법으로 만들 수 있습니다.

* 동기화 규칙이 존재하기 전에 생성된 사용자입니다. 매우 오래된 사용자 계정에는 이러한 속성이 동기화되지 않을 수 있습니다.

* Workfront의 emailAddr이 대/소문자를 구분하던 시기에 SSO를 통해 만든 사용자입니다. SSO 자동 프로비저닝 옵션은 ID 공급자의 사용자 특성을 기반으로 사용자에 대해 대/소문자를 구분하는 검사를 실행합니다. 정확히 일치하는 항목이 없으면 자동 프로비저닝 서비스가 새 사용자를 만듭니다. 사용자가 이미 존재하는 경우 사용자 이름과 `emailAddr` 케이싱은 동일하지 않습니다.

* 가 있는 사용자 `username` api 및 해당 속성을 통해 직접 업데이트된 특성 `emailAddr` 이 업데이트되지 않았습니다. 다음 `username` 및 `emailAddr` 일치하지 않을 수도 있습니다.

## 솔루션

API를 사용하여 `username` 속성이 `emailAddr`. 속성을 동기화한 후에는 `emailAddr` 도 업데이트됩니다 `username` 일치시켜야 합니다(사용자 이름 필드가 업데이트에 포함되지 않은 경우).
