---
content-type: api
navigation-topic: api-navigation-topic
title: 기본 API 버전 관리를 사용하는 통합 업데이트
description: 기본 API 버전 관리를 사용하는 통합 업데이트
author: Becky
feature: Workfront API
role: Developer
exl-id: ac394b41-63cb-481a-a858-30d8d7f840bb
source-git-commit: 3e339e2bfb26e101f0305c05f620a21541394993
workflow-type: tm+mt
source-wordcount: '632'
ht-degree: 0%

---

# 기본 API 버전 관리를 사용하는 통합 업데이트

당사는 2년 단위로 새로운 버전의 Adobe Workfront API를 출시합니다. 각 버전은 릴리스 이후 3년 동안 지원되며 버전을 사용할 수 있지만 지원되지 않는 더 이상 사용되지 않는 상태에서 연도가 추가됩니다.

URI에 API 버전을 지정하지 않는 통합은 자동으로 기본값으로 라우팅됩니다. API 호출이 API의 특정 버전을 사용하도록 하려면 Workfront API 요청에 해당 버전을 지정해야 합니다.

>[!NOTE]
>
>조직에서 현재 기본 API를 사용 중인 경우 Workfront 관리자가 기본 API에 대한 추가 지침이 포함된 공지 센터 메시지를 받았습니다.

API 요청에서 버전을 지정하는 방법에 대한 자세한 내용은 [통합에서 API 버전 지정](../../wf-api/api/specify-api-version-integrations.md).

## 기본 API 사용 시 고려 사항

Workfront 기본 API로 작업할 때 다음 사항을 고려하십시오.

* API의 기본 버전 및 최신 버전입니다. 지정된 버전이 없는 모든 API 호출은 기본 버전을 사용합니다. Workfront이 새 버전의 API를 릴리스할 때마다 기본 버전이 최신 버전으로 업데이트됩니다. **따라서 새 버전의 Workfront API가 릴리스된 후 기본 버전을 사용하는 모든 API 호출은 기능이 계속 지원되는지 확인해야 합니다**.
* 조직에서 현재 더 이상 사용되지 않는 이전 기본 API를 사용하는 경우 Workfront 관리자가 기본 API에 대한 추가 지침과 함께 공지 센터 메시지를 받았습니다.

최신 버전의 API를 보려면 를 참조하십시오. [API 버전 관리 및 지원 일정](../../wf-api/api/api-version-support-schedule.md).

## 지원되는 API 버전에 대한 통합 업데이트

Workfront API 요청에 버전이 지정되지 않은 경우 기본값 을 사용합니다. 지원되는 API 버전, 가급적 지원되는 최신 API를 지정하기 위해 API 요청을 사용하는 것이 좋습니다.

예를 들어 다음 Workfront API 요청은 API 버전을 지정하지 않습니다.

`https://davidwhite.my.workfront.com/attask/api/project/metadata`

이 요청이 이루어지면 Workfront 인스턴스의 데이터를 지정하는 JSON 인코딩 텍스트가 있는 응답을 받게 됩니다. 이 URI에 지정된 API 버전이 없으므로 호출이 기본값으로 이동합니다.

기본 API 요청을 버전 관리 API 요청으로 전환하려면 지원되는 API 버전을 호출하면 됩니다. 예를 들어 다음 URI는 버전 15를 요청합니다.

`https://davidwhite.my.workfront.com/attask/api/`**v15.0**`/project/metadata`

Workfront API 요청을 업데이트할 때 지원되는 모든 API 버전을 지정할 수 있습니다. 특정 API 참조에 대한 자세한 내용은 [통합에서 API 버전 지정](../../wf-api/api/specify-api-version-integrations.md).

최대 지원 기간을 보장하려면 최신 버전을 호출해야 합니다. 에서 지원되는 API 목록을 찾을 수 있습니다. [API 버전 관리 및 지원 일정](../../wf-api/api/api-version-support-schedule.md).

## API 기본 버전 내역

&quot;기본 API&quot; 또는 Default의 원래 목적은 이 API를 Workfront API의 최신 버전에 매핑하는 것이었습니다. 이렇게 하면 Default라고 하는 기본 통합을 사용하는 고객이 API 요청을 업데이트할 필요가 없습니다.

2011년 Workfront은 API 버전 3.0을 릴리스했습니다. 기본값이 버전 3.0으로 자동 이동되었으므로, 업데이트하지 않고 버전 3.0을 사용하기에는 너무 복잡한 고객 통합이 많이 끊어졌습니다. 그 결과 Workfront은 이 변경 사항을 롤백하고 기본 버전을 버전 2에 남겨두었습니다.

2011년 이후 Workfront은 API 기능을 크게 늘렸습니다. 이러한 이유로 더 이상 사용되지 않는 이전 버전의 API가 있습니다. 2017년에는 Default를 업데이트하기보다는 Default 버전의 개념을 완전히 제거했습니다. 이는 고객이 안정적인 버전의 API를 사용하고 최대 3년 주기로 통합을 유지할 수 있도록 하기 위한 것이었습니다.

Workfront이 이제 기본 API 버전을 복원합니다. 기본 API는 Workfront API의 최신 버전으로 설정되어 있으며, 새 버전이 릴리스될 때마다 최신 버전으로 업데이트됩니다.

