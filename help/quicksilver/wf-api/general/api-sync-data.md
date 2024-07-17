---
content-type: api
keywords: API,data,sync,journal,entry,object
navigation-topic: general-api
title: API를 사용하여 프로그램 및 서비스에 대한 데이터를 동기화합니다
description: API를 사용하여 프로그램 및 서비스에 대한 데이터를 동기화합니다
author: Becky
feature: Workfront API
role: Developer
exl-id: 1d0583fc-1573-4279-a3fa-a912d9a4213c
source-git-commit: 14ff8da8137493e805e683e5426ea933f56f8eb8
workflow-type: tm+mt
source-wordcount: '471'
ht-degree: 0%

---


# API를 사용하여 프로그램 및 서비스의 데이터 동기화

다음은 프로그램 및 서비스의 데이터를 동기화하기 위해 API를 활용하는 몇 가지 일반적인 방법입니다.

## 거의 실시간 업데이트

Adobe Workfront은 &quot;이벤트 구독&quot;(일반적으로 웹후크라고도 함)을 사용하여 API를 통해 지원되는 개체 및 작업에 대한 근거리 실시간 업데이트를 원하는 끝점으로 보냅니다. 새 오브젝트 및 작업에 대한 업데이트를 5초 이내에 받을 것으로 예상할 수 있지만 평균 업데이트는 약 1초 후에 도착합니다. 지원되는 개체 유형, 지원되는 작업 유형, 기술 세부 정보 및 이벤트 구독을 설정하는 방법에 대한 예제에 대한 자세한 내용은 [이벤트 구독 API](../../wf-api/general/event-subs-api.md) 및 [이벤트 구독 배달 요구 사항](../../wf-api/general/setup-event-sub-endpoint.md)을 참조하십시오.

## 일괄 업데이트

일괄 업데이트 는 Workfront 서버에 정기적으로 요청하여 업데이트할 시스템을 구성하는 방법입니다. 이렇게 하는 방법에는 여러 가지가 있지만 일반적으로 프로세스에서는 서비스가 Workfront API 서버에 요청을 하도록 하고 마지막 요청 호출 이후 생성 또는 수정된 개체를 검색하는 것으로 구성됩니다. 잠재적 요청 호출 및 유용한 매개 변수에 대한 자세한 내용은 [API 기본 사항](../../wf-api/general/api-basics.md) 문서의 [GET 동작](../../wf-api/general/api-basics.md#get-behavior) 섹션을 참조하십시오.

배치 업데이트를 위한 서비스를 설정하는 동안 몇 가지 중요한 사항을 염두에 두어야 합니다.

### 시작 날짜

시작 날짜는 ISO 8601 형식을 사용하여 저장됩니다. 이 표준에는 날짜, 시간 및 시간대 정보가 포함됩니다.

**예:** ISO 8601 날짜 형식

<!-- [Copy](javascript:void(0);) -->
 
<pre><code>2020-05-18T17:00:00:000-0600</code></pre> 

객체가 작성된 날짜와 객체가 수정된 마지막 날짜가 모두 각각 &quot;entryDate&quot; 및 &quot;lastUpdateDate&quot;로 저장됩니다. Workfront 개체, 관련 필드 및 필드 이름에 대한 자세한 내용은 [API 탐색기](../../wf-api/general/api-explorer.md)를 참조하십시오. 개체를 수정할 때마다 lastUpdatedDate가 변경되는 경우 지정된 Workfront 개체의 entryDate는 변경되지 않습니다.

**예:** **lastUpdateDate** 필드를 활용하여 문제 개체에 대한 GET 요청입니다. 이 요청은 지정된 날짜 이후 업데이트된 모든 문제를 반환합니다.

<!-- [Copy](javascript:void(0);) -->
 

```
GET
https://<domain>.my.workfront.com/attask/api/v15.0/OPTASK/search?fields=ID,name,lastUpdateDate&$$LIMIT=200&lastUpdateDate=2020-05-13T18:18:37.255Z&lastUpdateDate_Mod=gte
```

### 저널 게시물 개체

객체의 특정 필드에 대한 변경 사항을 얻고자 하는 경우 &quot;분개 기입&quot; 객체를 질의할 수 있습니다. 해당 필드를 수정할 때마다 특정 개체 필드에 대한 정보를 기록하도록 Workfront 저널 항목 개체를 설정할 수 있습니다. 자세한 내용은 [시스템 업데이트 구성](../../administration-and-setup/set-up-workfront/system-tracked-update-feeds/configure-system-updates.md)을 참조하십시오.

필드를 저널 게시물 개체의 일부로 기록하도록 설정하면 해당 필드가 수정될 때마다 해당 저널 게시물이 만들어집니다. 그런 다음 다음과 유사한 API 호출을 사용하여 분개 기입 객체를 질의할 수 있습니다.

<!-- [Copy](javascript:void(0);) -->

<pre><code>GET https://&#123;&#123;domain&#125;&#125;.my.workfront.com/attask/api/v15.0/JRNLE/search?fields=newTextVal,oldTextVal,newDateVal,oldDateVal,newNumberVal,oldNumberVal,entryDate,objObjCode,objID,fieldName&fieldName=name&objObjCode=OPTASK&entryDate=2020-05-13T18:18:37.255Z&entryDate_Mod=gte</code></pre>

>[!NOTE]
>
>entryDate는 변경된 객체 자체를 보는 것과 대조적으로 변경 내용의 분개 입력을 보는 데 사용됩니다.
