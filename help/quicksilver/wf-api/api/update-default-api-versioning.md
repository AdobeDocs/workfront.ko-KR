---
content-type: api
navigation-topic: api-navigation-topic
title: 기본 API 버전 관리를 사용하는 통합 업데이트
description: 기본 API 버전 관리를 사용하는 통합 업데이트
author: John
feature: Workfront API
exl-id: ac394b41-63cb-481a-a858-30d8d7f840bb
source-git-commit: 183f7b766fd6f02b51625778e380cf00c5ecf61f
workflow-type: tm+mt
source-wordcount: '670'
ht-degree: 0%

---

# 기본 API 버전 관리를 사용하는 통합 업데이트

Adobe에서는 2년마다 Adobe Workfront API의 새로운 버전을 릴리스합니다. 각 버전은 릴리스 후 3년 동안 지원되며, 버전은 사용 가능하지만 지원되지 않는 추가 연도 상태로 제공됩니다.

URI에서 API 버전을 지정하지 않는 통합은 더 이상 사용되지 않는 기본값으로 자동 라우팅됩니다. Workfront 통합이 유효하려면 Workfront API 요청에서 지원되는 API 버전을 지정해야 합니다.

API 요청에서 버전을 지정하는 방법에 대한 자세한 내용은 [통합에서 API 버전 지정](../../wf-api/api/specify-api-version-integrations.md).

## API의 기본 버전 이해

기본 API 또는 Default의 원래 목적은 최신 버전의 Workfront API에 매핑하는 것이었습니다. 이렇게 하면 Default라는 기본 통합을 사용하는 고객이 API 요청을 업데이트할 필요가 없습니다.

2011년에 Workfront은 API의 버전 3.0을 릴리스했습니다. 기본값이 버전 3.0으로 자동으로 이동되었으므로, 이 버전 3.0은 업데이트되지 않고 버전 3.0을 활용하기에 너무 복잡한 고객 통합이 중단되었습니다. 그 결과 Workfront은 이 변경 사항을 롤백하고 기본 버전을 버전 2에서 남겼습니다.

안타깝게도 이 항목은 다시 방문되지 않았고, 이제 API 기능을 크게 늘리려고 하므로 Default를 포함한 이전 버전의 API를 함께 설치해야 합니다. 의심할 여지 없이 더 많은 통합을 중단시키는 기본값 업데이트 대신, 기본 버전의 개념을 완전히 제거하고 있습니다. 고객이 안정적인 버전의 API를 사용하고 최대 3년의 주기를 통해 통합을 유지하도록 독려하기 위한 것입니다.

## 기본값 사용 안 함

Workfront API를 향상시키기 위해 지원 기간을 3년을 초과한 이전 API 버전을 제거하는 중입니다. 이러한 버전 중 하나는 버전 2이며, 이 버전은 기본값이 매핑됩니다. 이 버전은 2010년에 출시되었으며, 이 시점에 Attask/Workfront 애플리케이션에서 지원되는 대부분의 로직은 더 이상 존재하지 않거나 크게 변경되었습니다.

2017년 7월부터 기본값이 사용되지 않으며, 더 이상 API의 특정 버전을 기본 버전으로 지정하지 않습니다. 대신, 모든 Workfront API 요청은 특정 API 버전을 지정해야 합니다.

>[!IMPORTANT]
>
> 2018년 7월 1일까지 Default를 사용하는 모든 Workfront 통합을 업데이트하여 특정 지원되는 API 버전을 호출해야 합니다. 해당 날짜 이후, 버전을 지정하지 않은 통합에 사용된 모든 Workfront API 요청이 실패합니다.

Workfront 사용 중단 케이스에 대한 자세한 내용은 [API 버전 관리 및 지원 예약](../../wf-api/api/api-version-support-schedule.md).

## 지원되는 API 버전으로 통합 업데이트

Workfront API 요청에 버전을 지정하지 않는 경우 기본값을 사용합니다. 지원되는 API 버전을 최신 지원 API로 지정하려면 API 요청을 업데이트해야 합니다.

예를 들어 다음 Workfront API 요청은 API 버전을 지정하지 않습니다.

`https://davidwhite.my.workfront.com/attask/api/project/metadata`

이 요청이 수행되면 Workfront 인스턴스의 데이터를 지정하는 JSON 인코딩 텍스트가 있는 응답을 받게 됩니다. 이 URI에 지정된 API 버전이 없으므로 호출이 Default로 이동합니다.

기본 API 요청을 버전이 지정된 API 요청으로 전환하려면 지원되는 API 버전을 호출하면 됩니다. 예를 들어 다음 URI가 버전 9를 요청합니다.

`https://davidwhite.my.workfront.com/attask/api/`**v9.0**`/project/metadata`

Workfront API 요청을 업데이트할 때 지원되는 API 버전을 지정할 수 있습니다. 특정 API 참조에 대한 자세한 내용은 [통합에서 API 버전 지정](../../wf-api/api/specify-api-version-integrations.md).

최대 지원 기간을 확인하려면 최신 버전(버전 9)을 호출해야 합니다. 에서 지원되는 API 목록을 찾을 수 있습니다 [API 버전 관리 및 지원 예약](../../wf-api/api/api-version-support-schedule.md).

기본값을 사용하는 통합을 업데이트해야 합니다. 현재 버전을 지정하지 않는 통합이 있는 경우 Workfront 영업 사원, 고객 성공 관리자, 지원 담당자 또는 공지 센터 메시지로부터 알림을 받을 수 있습니다.

가능한 한 빨리, 지원되는 버전의 API를 호출하도록 통합이 업데이트되는지 확인하십시오.
