---
content-type: api
product-area: user-management
navigation-topic: general-api
title: API를 통해 사용자 비활성화
description: API를 통해 사용자 비활성화
author: John
feature: Workfront API
exl-id: 45b06cce-4622-4739-b9f3-2edb9101c099
source-git-commit: 50675b7af3fcd2188a18391732a93a7b67454db9
workflow-type: tm+mt
source-wordcount: '199'
ht-degree: 0%

---


# API를 통해 사용자 비활성화

사용자가 조직을 떠날 때 사용자를 비활성화하여 다른 사용자가 해당 Adobe Workfront 라이센스를 사용할 수 있게 하고 해당 사용자에게 실수로 작업이 할당되지 않도록 할 수 있습니다. 사용자를 비활성화하면 작업 지정과 노트, 시간 및 문서와의 연관성을 포함하여 작업 기록이 유지됩니다.

사용자 비활성화에 대한 자세한 내용은 &quot; [사용자 비활성화 또는 다시 활성화](../../administration-and-setup/add-users/create-and-manage-users/deactivate-a-user.md).

핵심 API 사용에 대한 자세한 내용은 [API 기본 사항](../../wf-api/general/api-basics.md).

API를 통해 사용자를 비활성화하려면:

1. 다음 API 요청을 사용하여 API 키를 생성합니다.

```
<domain>.my.workfront.com/attask/api/v7.0/user?action=generateApiKey&username=`username`&password=`password`&method=PUT`
```

1. 비활성화할 사용자의 GUID를 찾습니다.

   1. 다음 API 요청을 사용하여 시스템의 모든 사용자에 대한 GUID를 검색합니다. **isActive** 필드 표시 **true** 현재 활성 상태이고 **false** 비활성화된 사용자:

```
<domain>`.my.workfront.com/attask/api/v7.0/USER/search?fields=isActive
```

1. 비활성화할 사용자의 GUID를 찾으려면 다음을 사용하십시오 **PUT** 사용자의 변경 요청 **isActive** 필드 값 **false**:

```
<domain>`.my.workfront.com/attask/api/v7.0/USER/`<user's GUID>`?updates={"isActive":"false"}&method=put&apiKey=`<apiKey>`&fields=isActive
```

1. 응답에는 **isActive** 필드 값이 **true** to **false**&#x200B;사용자가 비활성화되었음을 나타냅니다.

<!-- [Copy](javascript:void(0);) -->
<pre></pre>
