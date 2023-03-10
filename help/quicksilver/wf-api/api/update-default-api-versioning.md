---
content-type: api
navigation-topic: api-navigation-topic
title: 기본 API 버전 관리를 사용하는 통합 업데이트
description: 기본 API 버전 관리를 사용하는 통합 업데이트
author: Becky
feature: Workfront API
exl-id: ac394b41-63cb-481a-a858-30d8d7f840bb
source-git-commit: f050c8b95145552c9ed67b549608c16115000606
workflow-type: tm+mt
source-wordcount: '693'
ht-degree: 0%

---

# 기본 API 버전 관리를 사용하는 통합 업데이트

<!-- This article is going to need a complete revamp or to be removed-->

<span class="preview">이 페이지에서 강조 표시된 정보는 아직 일반적으로 사용할 수 없는 기능을 참조합니다. 미리 보기 샌드박스 환경에서만 사용할 수 있습니다.</span>

Adobe에서는 2년마다 Adobe Workfront API의 새로운 버전을 릴리스합니다. 각 버전은 릴리스 후 3년 동안 지원되며, 버전은 사용 가능하지만 지원되지 않는 추가 연도 상태로 제공됩니다.

URI에서 API 버전을 지정하지 않는 통합은 자동으로 기본값으로 라우팅됩니다. API 호출에서 특정 버전의 API를 사용하려면 Workfront API 요청에 해당 버전을 지정해야 합니다.

>[!NOTE]
>
>조직에서 현재 기본 API를 사용하고 있는 경우 Workfront 관리자가 기본 API에 대한 추가 지침이 포함된 공지 센터 메시지를 수신했습니다.


<!--
Integrations that do not specify a version of the API in the URI are automatically routed to Default, which has been deprecated. In order for your Workfront integrations to be valid, you must specify a supported API version in your Workfront API requests.
-->

API 요청에서 버전을 지정하는 방법에 대한 자세한 내용은 [통합에서 API 버전 지정](../../wf-api/api/specify-api-version-integrations.md).

## 기본 API를 사용할 때의 고려 사항

Workfront 기본 API 작업 시 다음 사항을 고려하십시오.

* 23.2 릴리스 이후 API의 기본 버전은 최신 버전으로 설정됩니다. 지정된 버전이 없는 모든 API 호출은 기본 버전을 사용합니다. Workfront이 새로운 버전의 API를 릴리스할 때마다 기본 버전이 최신 버전으로 업데이트됩니다. **따라서 새 버전의 Workfront API가 릴리스된 후에는 기본 버전을 사용하는 모든 API 호출을 확인하여 기능이 계속 지원되는지 확인해야 합니다**.
* 조직에서 현재 더 이상 사용되지 않는 기본 API를 사용하는 경우 Workfront 관리자가 기본 API에 대한 추가 지침이 포함된 공지 센터 메시지를 수신했습니다.
* <span class="preview">미리 보기 환경의 기본 API가 현재 최신 버전으로 설정되어 있습니다. 프로덕션 환경의 기본 API는 23.2 릴리스 이후 가장 최신 버전으로 설정됩니다.</span>

최신 버전의 API를 보려면 [API 버전 관리 및 지원 예약](../../wf-api/api/api-version-support-schedule.md).

<!--

## Deprecating Default

In an effort to improve the Workfront API, we are in the process of removing older API versions that have exceeded our support window of three years. One of these versions is Version 2, to which Default is mapped. This version was released in 2010, and much of the logic supported in the Attask/Workfront application at that time either no longer exists or has substantially changed.

We deprecated Default in July 2017, and we will no longer designate a specific version of the API to be the default version. Instead, all Workfront API requests must specify a specific API version.

>[!IMPORTANT]
>
> By July 1, 2018 all of your Workfront integrations that use Default must be updated to call a specific supported API version. After that date, all of your Workfront API requests used by integrations that do not specify a version will fail.

To learn about the Workfront deprecation cadence, see [API versioning and support schedule](../../wf-api/api/api-version-support-schedule.md).

-->

## 지원되는 API 버전으로 통합 업데이트

Workfront API 요청에 버전을 지정하지 않는 경우 기본값을 사용합니다. API 요청에서 지원되는 API 버전(가급적 최신 지원 API)을 지정하는 것이 좋습니다.

예를 들어 다음 Workfront API 요청은 API 버전을 지정하지 않습니다.

`https://davidwhite.my.workfront.com/attask/api/project/metadata`

이 요청이 수행되면 Workfront 인스턴스의 데이터를 지정하는 JSON 인코딩 텍스트가 있는 응답을 받게 됩니다. 이 URI에 지정된 API 버전이 없으므로 호출이 Default로 이동합니다.

기본 API 요청을 버전이 지정된 API 요청으로 전환하려면 지원되는 API 버전을 호출하면 됩니다. 예를 들어 다음 URI가 버전 15를 요청합니다.

`https://davidwhite.my.workfront.com/attask/api/`**v15.0**`/project/metadata`

Workfront API 요청을 업데이트할 때 지원되는 API 버전을 지정할 수 있습니다. 특정 API 참조에 대한 자세한 내용은 [통합에서 API 버전 지정](../../wf-api/api/specify-api-version-integrations.md).

최대 지원 기간을 확인하려면 최신 버전을 호출해야 합니다. 에서 지원되는 API 목록을 찾을 수 있습니다 [API 버전 관리 및 지원 예약](../../wf-api/api/api-version-support-schedule.md).

## API의 기본 버전 기록

기본 API 또는 Default의 원래 목적은 최신 버전의 Workfront API에 매핑하는 것이었습니다. 이렇게 하면 Default라는 기본 통합을 사용하는 고객이 API 요청을 업데이트할 필요가 없습니다.

2011년에 Workfront은 API의 버전 3.0을 릴리스했습니다. 기본값이 버전 3.0으로 자동으로 이동되었으므로, 이 버전 3.0은 업데이트되지 않고 버전 3.0을 활용하기에 너무 복잡한 고객 통합이 중단되었습니다. 그 결과 Workfront은 이 변경 사항을 롤백하고 기본 버전을 버전 2에서 남겼습니다.

2011년 이후 Workfront은 API 기능을 크게 늘렸습니다. 이러한 이유로 이전 버전의 API는 더 이상 사용되지 않습니다. 2017년, 기본값 업데이트 대신 기본 버전의 개념을 완전히 제거했습니다. 이는 고객이 안정적인 버전의 API를 사용하고 최대 3년 주기로 통합을 유지하도록 독려하기 위한 것입니다.

Workfront이 이제 기본 API 버전을 재설치하고 있습니다. 기본 API는 Workfront API의 최신 버전으로 설정되며, 새 버전이 릴리스될 때마다 최신 버전으로 업데이트됩니다.

