---
filename: api-changes-search
content-type: api
keywords: 오브젝트,상태,검색,우수 사례,응답
navigation-topic: api-navigation-topic
title: '핵심 API 변경: 상태 검색 응답'
description: Workfront이 상태 개체를 저장하는 방식의 변경 사항입니다.
feature: Workfront API
role: Developer
exl-id: 322f1525-d1d5-4845-a590-e34eb94ccdc2
source-git-commit: 3e339e2bfb26e101f0305c05f620a21541394993
workflow-type: tm+mt
source-wordcount: '441'
ht-degree: 0%

---

# 핵심 API 변경 사항: 상태 검색 응답

Workfront에서 상태 개체를 저장하는 방식이 변경되었습니다. 이러한 변경 사항은 상태 검색 요청이 수행되는 방식에는 영향을 주지 않지만, 불완전한 그룹 상태 목록을 반환하여 상태 오브젝트를 검색하는 것을 포함하는 API 요청에 의해 반환되는 응답에는 영향을 줍니다.

## 우수 사례

그룹에 사용할 수 있는 상태의 전체 목록을 안정적으로 가져오려면 다음 요청을 모범 사례로 간주합니다.

>[!NOTE]
>
>이러한 요청 구조는 클러스터에 대한 상태 검색 변경 여부와 관계없이 모든 사용자에게 권장됩니다.

프로젝트 그룹 상태의 경우:

>**예:**

```
/attask/api/<VERSION>/CSTEM/projectGroupStatuses?groupID=602d27640000bb3b779f770d5fb95d6d
```

작업 그룹 상태의 경우:

>**예:**

```
/attask/api/<VERSION>/CSTEM/taskGroupStatuses?groupID=602d27640000bb3b779f770d5fb95d6d
```

문제 그룹 상태의 경우:

>**예:**

```
/attask/api/<VERSION>/CSTEM/opTaskGroupStatuses?groupID=602d27640000bb3b779f770d5fb95d6d
```

이 세 끝점은 모두 **includeHidden=true** 매개 변수를 사용하여 주어진 그룹의 숨겨진 프로젝트/작업/문제 상태를 가져옵니다. 이러한 모범 사례 예제 후 상태 검색 쿼리를 모델링하면 모든 그룹 상태 정보가 각 응답에 포함됩니다.

다음은 시스템 수준 잠금 상태 **Custom_1**&#x200B;와 잠금 해제 상태 **Custom_2**&#x200B;를 포함하는 작업 그룹에 대해 수행되는 상태 검색 쿼리의 예입니다.

>**예:**

```
/attask/api/<VERSION>/CSTEM/taskGroupStatuses?groupID=602d286d000004fc8f53942de697a868
```

이 형식을 사용하면 응답에 다음 항목이 모두 포함됩니다.

```
{
    "data": [
        {
            "color": "1C68FF",
            "equatesWith": "NEW",
            "groupID": "602d27640000bb3b779f770d5fb95d6d",
            "label": "New",
            "objCode": "CSTEM",
            "value": "NEW"
        },
        {
            "color": "39FF39",
            "equatesWith": "INP",
            "groupID": "602d27640000bb3b779f770d5fb95d6d",
            "label": "In Progress",
            "objCode": "CSTEM",
            "value": "INP"
        },
        {
            "color": "FF3939",
            "equatesWith": "CPL",
            "groupID": "602d27640000bb3b779f770d5fb95d6d",
            "label": "Complete",
            "objCode": "CSTEM",
            "value": "CPL"
        },
        {
            "color": "8BC34A",
            "equatesWith": "NEW",
            "groupID": "602d27640000bb3b779f770d5fb95d6d",
            "label": "Custom_1",
            "objCode": "CSTEM",
            "value": "JET"
        },
        {
            "color": "8BC34A",
            "equatesWith": "NEW",
            "groupID": "602d27640000bb3b779f770d5fb95d6d",
            "label": "Custom_2",
            "objCode": "CSTEM",
            "value": "OGC"
        }
    ]
}
```

## 기존 상태 검색 쿼리에 대한 변경 사항 이해

기존 시스템에서 상태 검색 쿼리는 쿼리에 포함된 모든 그룹에 사용할 수 있는 모든 시스템 상태를 복사합니다. 그러면 이전 응답에는 쿼리의 각 그룹에 사용할 수 있는 모든 시스템 상태 및 그룹 수준 상태가 포함됩니다.

예를 들어 이 쿼리(현재 권장되는 모범 사례를 따르지 않음)는

>**예:**

```
/attask/api/<VERSION>/CSTEM/search?groupID=602d27640000bb3b779f770d5fb95d6d&enumClass=STATUS_TASK
```

모든 객체 상태를 포함하여 레거시 시스템에서 다음과 같은 응답을 받게 됩니다.

```
{
    "data": [
        {
            "color": "1C68FF",
            "equatesWith": "NEW",
            "groupID": "602d27640000bb3b779f770d5fb95d6d",
            "label": "New",
            "objCode": "CSTEM",
            "value": "NEW"
        },
        {
            "color": "39FF39",
            "equatesWith": "INP",
            "groupID": "602d27640000bb3b779f770d5fb95d6d",
            "label": "In Progress",
            "objCode": "CSTEM",
            "value": "INP"
        },
        {
            "color": "FF3939",
            "equatesWith": "CPL",
            "groupID": "602d27640000bb3b779f770d5fb95d6d",
            "label": "Complete",
            "objCode": "CSTEM",
            "value": "CPL"
        },
        {
            "color": "8BC34A",
            "equatesWith": "NEW",
            "groupID": "602d27640000bb3b779f770d5fb95d6d",
            "label": "Custom_1",
            "objCode": "CSTEM",
            "value": "JET"
        },
        {
            "color": "8BC34A",
            "equatesWith": "NEW",
            "groupID": "602d27640000bb3b779f770d5fb95d6d",
            "label": "Custom_2",
            "objCode": "CSTEM",
            "value": "OGC"
        }
    ]
}
```

그러나 상태가 저장되고 사용되는 방식에 대한 업데이트에 따라 그룹에 대해 상태가 복사되지 않고 시스템 수준에서 각 그룹에 의해 상속됩니다. 따라서 검색 API 쿼리는 특정 그룹과 직접 관련된 상태만 읽으므로, 응답에는 시스템 잠금 및 잠금 해제 상태가 포함되지만 해당 상태가 추가된 후 생성된 그룹에 대해서만 표시됩니다.

기존 시스템이 업데이트된 후 업데이트된 모범 사례 방법을 사용하여 상태 검색 쿼리를 만들지 않으면 응답에 그룹 상태의 불완전한 목록이 반환됩니다.

다음은 레거시 시스템이 업데이트된 후 이 오래된 요청 구조가 반환하는 것의 예입니다.

>**예:**

```
/attask/api/<VERSION>/CSTEM/search?groupID=602d27640000bb3b779f770d5fb95d6d&enumClass=STATUS_TASK
```

이 응답에는 그룹별 상태만 포함되며 시스템 수준에서 선언된 상태는 제외됩니다.

```
{
  "data": [
    {
      "color": "8BC34A",
      "equatesWith": "NEW",
      "groupID": "602d286d000004fc8f53942de697a868",
      "label": "Custom_2",
      "objCode": "CSTEM",
      "value": "MMI"
    }
  ]
}
```
