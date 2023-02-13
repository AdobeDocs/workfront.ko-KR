---
filename: api-changes-search
content-type: api
keywords: 개체,상태,검색,우수 사례,응답
navigation-topic: api-navigation-topic
title: '''핵심 API 변경 사항: 상태 검색 응답'
description: Workfront이 상태 개체를 저장하는 방식의 변경.
exl-id: 322f1525-d1d5-4845-a590-e34eb94ccdc2
source-git-commit: f2f825280204b56d2dc85efc7a315a4377e551c7
workflow-type: tm+mt
source-wordcount: '446'
ht-degree: 1%

---

# 핵심 API 변경 사항: 상태 검색 응답

Workfront에서 상태 개체를 저장하는 방식이 변경되었습니다. 이러한 변경 사항은 상태 검색 요청의 수행 방법에는 영향을 주지 않지만, 불완전한 그룹 상태 목록을 반환하여 상태 개체 검색을 포함하는 API 요청에서 반환되는 응답에 영향을 줍니다.

## 우수 사례

그룹에 사용 가능한 상태 전체 목록을 안정적으로 가져오기 위해 다음 요청을 모범 사례로 간주됩니다.

>[!NOTE]
>
>클러스터의 상태 검색 변경 여부에 관계없이 이러한 요청 구조가 모든 사용자에게 권장됩니다.

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

이 세 가지 종단점은 모두 **includeHidden=true** 지정된 그룹의 숨겨진 프로젝트/작업/문제 상태를 가져오기 위한 매개 변수입니다. 이러한 우수 사례 이후에 상태 검색 쿼리를 모델링하면 모든 그룹 상태 정보가 각 응답에 포함되도록 할 수 있습니다.

다음은 시스템 수준의 잠금 상태를 포함하는 작업 그룹에 대해 수행되는 상태 검색 쿼리의 예입니다 **Custom_1** 및 잠금 해제된 상태 **Custom_2**:

>**예:**

```
/attask/api/<VERSION>/CSTEM/taskGroupStatuses?groupID=602d286d000004fc8f53942de697a868
```

이 형식을 사용하면 응답에 다음 내용이 모두 포함됩니다.

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

## 기존 상태 검색 쿼리에 대한 변경 내용 이해

레거시 시스템 아래에 상태 검색 쿼리는 쿼리에 포함된 모든 그룹에 사용할 수 있는 모든 시스템 상태를 복사합니다. 그러면 레거시 응답에는 쿼리의 각 그룹에 대해 사용할 수 있는 모든 시스템 상태와 그룹 수준 상태가 포함됩니다.

예를 들어, 이 쿼리(현재 권장되는 우수 사례를 따르지 않음)는 다음과 같습니다.

>**예:**

```
/attask/api/<VERSION>/CSTEM/search?groupID=602d27640000bb3b779f770d5fb95d6d&enumClass=STATUS_TASK
```

레거시 시스템 아래에 모든 개체 상태를 포함하는 다음 응답이 있을 것입니다.

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

그러나 상태를 저장 및 사용하는 방법에 대한 업데이트 후에 상태는 그룹에 대해 복사되지 않으며 시스템 수준의 각 그룹에 의해 상속됩니다. 그 결과, 검색 API 쿼리는 특정 그룹과 직접 연결된 상태만 읽으므로, 응답에는 시스템 잠금 및 잠금 해제 상태가 포함되지만, 해당 상태가 추가된 후에 생성된 그룹에 대해서만 포함됩니다.

레거시 시스템을 업데이트한 후 상태 검색 쿼리를 만드는 업데이트된 모범 사례 메서드를 사용하지 않으면 응답에서 불완전한 그룹 상태 목록이 반환됩니다.

다음은 이전 시스템이 업데이트된 후 이러한 오래된 요청 구조가 반환하는 결과의 예입니다.

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
