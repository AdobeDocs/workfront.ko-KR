---
content-type: api
navigation-topic: api-navigation-topic
title: API-Internal 사용 중단
description: API-Internal 사용 중단
author: Becky
feature: Workfront API
exl-id: 45b42fe8-7ce3-441d-8fbc-b8db7f9b254e
source-git-commit: f050c8b95145552c9ed67b549608c16115000606
workflow-type: tm+mt
source-wordcount: '218'
ht-degree: 0%

---

# API-Internal 사용 중단

API-Internal은 Adobe Workfront API의 디자인과 목적 때문에 지원되지 않는 버전입니다. Workfront API에 대한 최신 업데이트를 포함하지만 예고 없이 변경될 수 있으므로 프로덕션 통합에서 신중하게 사용해야 합니다. Workfront은 모든 API-내부 통합을 버전이 지정된 API로 업데이트할 것을 강력히 권장합니다.

Workfront API의 지원되는 버전에 대한 자세한 내용은 [API 버전 관리 및 지원 예약](../../wf-api/api/api-version-support-schedule.md).

**API 사용 - 지원되지 않음**

버전에서 관리되는 API에서 사용할 수 없는 기능이 통합되어야 하는 경우 API-Unsupported를 사용하는 것이 좋습니다. API-Internal과 유사한 API-Unsupported는 지원되지 않습니다. API-Unsupported에는 Workfront API의 최신 변경 사항이 포함되어 있으며 예고 없이 변경될 수 있습니다. Workfront에서는 새로운 기능을 탐색하고 API에 버그가 없는지 확인할 수 있는 테스트 환경에서 API-Unsupported를 사용할 것을 권장합니다.

**사용 중인 API 버전 확인**

REST 를 사용하여 HTTPS를 통해 Workfront에 호출을 전송하는 URI를 구성한 다음 JSON 응답을 반환하여 통합에 사용하는 API 버전을 확인할 수 있습니다.

다음 예는 API-Internal을 호출하는 URI를 보여줍니다.

```
https://<domainname>.my.workfront.com/attask/api/api-internal/proj/4c70…
```

다음 예제에서는 API-Unsupported를 호출하는 URI를 보여 줍니다.

```
https://<domainname>.my.workfront.com/attask/api/api-unsupported/proj/4c70...
```

다음 예는 API의 버전 15.0을 호출하는 URI를 보여줍니다.

```
https://<domainname>.my.workfront.com/attask/api/v15.0/proj/4c70…
```
