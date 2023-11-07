---
content-type: api
navigation-topic: api-navigation-topic
title: 통합에서 API 버전 지정
description: 통합에서 API 버전 지정
author: Becky
feature: Workfront API
role: Developer
exl-id: 2971749d-1d34-42a4-9eda-411aa8c3a2ab
source-git-commit: 3e339e2bfb26e101f0305c05f620a21541394993
workflow-type: tm+mt
source-wordcount: '435'
ht-degree: 0%

---

# 통합에서 API 버전 지정

모든 Adobe Workfront URI는 URI의 &quot;attask/api&quot; 부분 뒤에 있는 특정 버전의 API를 참조해야 합니다. 다음 예제는 버전 15.0을 호출합니다.

`attask/api/v15.0/<objectName>/<objectId>`

모든 통합 호출이 현재 지원되는 Workfront API인지 확인하십시오.

## Workfront API의 릴리스 및 사용 중단 일정

API의 새 버전은 정기적으로(보통 1년에 두 번) 릴리스됩니다. 각 버전은 릴리스 날짜 이후 3년 동안 지원되며, 버전을 사용할 수 있지만 지원되지 않는 더 이상 사용되지 않는 상태에서 연도가 추가됩니다.

Workfront API의 릴리스 케이던스 및 사용 중단 일정에 대한 자세한 내용은 다음을 참조하십시오. [API 버전 관리 및 지원 일정](../../wf-api/api/api-version-support-schedule.md).

>[!IMPORTANT]
>
>* API의 기본 버전은 최신 버전으로 설정됩니다. 지정된 버전이 없는 모든 API 호출은 기본 버전을 사용합니다. Workfront이 새 버전의 API를 릴리스할 때마다 기본 버전이 최신 버전으로 업데이트됩니다. **따라서 새 버전의 Workfront API가 릴리스된 후 기본 버전을 사용하는 모든 API 호출은 기능이 계속 지원되는지 확인해야 합니다.**
>
>* 조직에서 현재 기본 API를 사용 중인 경우 Workfront 관리자가 기본 API에 대한 추가 지침이 포함된 공지 센터 메시지를 받았습니다.
>
>최신 버전의 API를 보려면 를 참조하십시오. [API 버전 관리 및 지원 일정](../../wf-api/api/api-version-support-schedule.md).


## 사용 중인 API 버전 확인

Workfront API로 전송된 HTTP 요청의 URI를 확인하여 사용 중인 API의 버전을 확인할 수 있습니다. 다음 예는 API 버전 15를 지정하는 Workfront 요청 URI를 보여 줍니다.

`https://<domainname>.my.workfront.com/attask/api/v15.0/proj/4c7c08b20000002de5ca1ebc19edf2d5`

URI에서 버전을 지정하지 않으면 다음 예와 같이 API의 기본 버전 을 사용합니다.

`https://<domainname>.my.workfront.com/attask/api/proj/4c7c08b20000002de5ca1ebc19edf2d5`

>[!IMPORTANT]
>
> URI에 API 버전을 지정하지 않는 통합은 자동으로 API 기본 버전으로 라우팅됩니다.

## 지원되는 API 버전을 사용하도록 통합 업데이트

Workfront 통합을 빌드하거나 유지 관리할 때 API 버전 및 변경될 수 있는 기타 속성(예: API 키)을 동적으로 업데이트하는 방법이 포함되어야 합니다.

통합 업데이트를 보다 효율적으로 수행하려면 통합 값을 기록하기 위해 다음 제안을 고려해야 합니다.

* 나중에 변경되는 속성 파일에 업데이트되는 값을 저장합니다.
* 실시간으로 속성을 관리할 웹 서비스 만들기
* 응용 프로그램에서 읽을 수 있는 데이터 저장소에 속성 값을 저장합니다.

이를 염두에 두고 Workfront 통합을 디자인하면 해당 값이 불가피하게 변경되는 경우 광범위한 개발 작업의 필요성이 줄어듭니다.
