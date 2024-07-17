---
content-type: api
product-area: user-management
navigation-topic: general-api
title: API를 통해 사용자 비활성화
description: API를 통해 사용자 비활성화
author: Becky
feature: Workfront API
role: Developer
exl-id: 45b06cce-4622-4739-b9f3-2edb9101c099
source-git-commit: 14ff8da8137493e805e683e5426ea933f56f8eb8
workflow-type: tm+mt
source-wordcount: '199'
ht-degree: 0%

---


# API를 통해 사용자 비활성화

사용자가 조직을 떠나면 사용자를 비활성화하여 다른 사용자가 Adobe Workfront 라이선스를 사용할 수 있도록 하고 실수로 작업을 할당받지 않도록 할 수 있습니다. 사용자를 비활성화하면 작업 할당과 메모, 시간 및 문서와의 연관을 포함하여 작업 기록이 유지됩니다.

사용자 비활성화에 대한 자세한 내용은 &quot; [사용자 비활성화 또는 다시 활성화](../../administration-and-setup/add-users/create-and-manage-users/deactivate-a-user.md)를 참조하세요.

Core API 사용에 대한 자세한 내용은 [API 기본 사항](../../wf-api/general/api-basics.md)을 참조하세요.

API를 통해 사용자를 비활성화하려면 다음을 수행하십시오.

1. 다음 API 요청을 사용하여 API 키를 생성합니다.

```
<domain>.my.workfront.com/attask/api/v15.0/user?action=generateApiKey&username=`username`&password=`password`&method=PUT`
```

1. 비활성화할 사용자의 GUID를 찾습니다.

   1. 다음 API 요청을 사용하여 시스템의 모든 사용자에 대한 GUID를 검색하십시오. **isActive** 필드는 현재 활성 상태인 사용자의 경우 **true**&#x200B;을(를), 비활성화되었던 사용자의 경우 **false**&#x200B;을(를) 표시합니다.

```
<domain>`.my.workfront.com/attask/api/v15.0/USER/search?fields=isActive
```

1. 비활성화할 사용자에 대한 GUID를 찾은 다음 **PUT** 요청을 사용하여 사용자의 **isActive** 필드 값을 **false**(으)로 변경하십시오.

```
<domain>`.my.workfront.com/attask/api/v15.0/USER/`<user's GUID>`?updates={"isActive":"false"}&method=put&apiKey=`<apiKey>`&fields=isActive
```

1. 응답이 **isActive** 필드 값이 **true**&#x200B;에서 **false**(사용자가 비활성화되었음을 나타냄)로 변경되었음을 보여 줍니다.

<!-- [Copy](javascript:void(0);) -->
<pre><code>{<br>&nbsp;&nbsp;&nbsp;&nbsp;data:&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;<br>&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;{&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;<br>&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;ID:&nbsp;"592125e60089b88fae8b51c08383e144",<br>&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;name:&nbsp;"Tyler Reid",<br>&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;objCode:&nbsp;"USER",<br>&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;isActive:&nbsp;false&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;<br>&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;}<br>}<br></code></pre>
