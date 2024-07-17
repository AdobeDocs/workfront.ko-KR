---
content-type: api
navigation-topic: api-navigation-topic
title: API 내부 사용 중단
description: API 내부 사용 중단
author: Becky
feature: Workfront API
role: Developer
exl-id: 45b42fe8-7ce3-441d-8fbc-b8db7f9b254e
source-git-commit: acc7414a9c6eef838147aee675603b6cc2566fb9
workflow-type: tm+mt
source-wordcount: '227'
ht-degree: 0%

---

# API 내부 사용 중단

API-Internal은 디자인 및 목적 때문에 지원되지 않는 Adobe Workfront API 버전입니다. 이 팩에는 Workfront API에 대한 최신 업데이트가 포함되어 있지만 예고 없이 변경될 수 있으므로 프로덕션 통합에서 주의해서 사용해야 합니다. Workfront은 모든 API-내부 통합을 버전이 지정된 API로 업데이트할 것을 강력히 권장합니다.

지원되는 Workfront API 버전에 대한 자세한 내용은 [API 버전 관리 및 지원 일정](../../wf-api/api/api-version-support-schedule.md)을 참조하세요.

**API 사용-지원되지 않음**

통합 시 버전 관리 API에서 사용할 수 없는 기능이 필요한 경우 Workfront에서는 API-Unsupported를 사용하는 것이 좋습니다. API-Internal과 마찬가지로 API-Unsupported는 지원되지 않습니다. API 미지원 은 또한 Workfront API에 대한 최신 변경 사항을 포함하며, 예고 없이 변경될 수 있습니다. Workfront에서는 새로운 기능을 탐색하고 API에 버그가 없는지 확인할 수 있도록 테스트 환경에서 API-Unsupported를 사용할 것을 권장합니다.

**사용 중인 API 버전 확인**

REST를 사용하여 HTTPS를 통해 Workfront으로 호출을 보낸 다음 JSON 응답을 반환하는 URI를 구성하여 통합에서 사용하는 API의 버전을 결정할 수 있습니다.

다음 예제는 API-Internal을 호출하는 URI를 보여 줍니다.

```
https://<domainname>.my.workfront.com/attask/api/api-internal/proj/4c70…
```

다음 예제는 API-Unsupported를 호출하는 URI를 보여 줍니다.

```
https://<domainname>.my.workfront.com/attask/api-unsupported/proj/4c70...
```

>[!NOTE]
>
>API가 지원되지 않는 호출에서는 URL의 `/api` 섹션을 생략합니다.

다음 예제는 API 버전 15.0을 호출하는 URI를 보여 줍니다.

```
https://<domainname>.my.workfront.com/attask/api/v15.0/proj/4c70…
```
