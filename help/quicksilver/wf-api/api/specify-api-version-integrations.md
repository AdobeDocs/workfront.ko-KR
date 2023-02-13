---
content-type: api
navigation-topic: api-navigation-topic
title: 통합에서 API 버전 지정
description: 통합에서 API 버전 지정
author: John
feature: Workfront API
exl-id: 2971749d-1d34-42a4-9eda-411aa8c3a2ab
source-git-commit: 183f7b766fd6f02b51625778e380cf00c5ecf61f
workflow-type: tm+mt
source-wordcount: '394'
ht-degree: 0%

---

# 통합에서 API 버전 지정

URI의 &quot;attask/api&quot; 부분 뒤에 특정 버전의 API를 참조하려면 모든 Adobe Workfront URI가 필요합니다. 다음 예에서는 버전 7.0을 호출합니다.
`attask/api/v7.0/<objectName>/<objectId>` 모든 통합 호출이 현재 지원되는 Workfront API인지 확인하십시오.

## Workfront API의 릴리스 및 사용 중단 일정

API의 새 버전은 6~8개월마다 2년마다 릴리스됩니다. 각 버전은 릴리스 날짜 이후 3년 동안 지원되며, 버전은 사용 가능하지만 지원되지 않는 더 이상 사용되지 않는 상태에서 추가 연도를 사용할 수 있습니다.

Workfront API의 릴리스 주기 및 사용 중단 예약에 대한 자세한 내용은 [API 버전 관리 및 지원 예약](../../wf-api/api/api-version-support-schedule.md).

Workfront은 2017년 7월부터 API의 기본 버전을 사용 중단했습니다. 즉, Workfront은 더 이상 API의 특정 버전을 기본 버전으로 지정하지 않습니다. 모든 향후 API URI가 유효하려면 API 버전을 지정해야 합니다.

>[!IMPORTANT]
>
> 기본 API 버전을 사용하는 모든 통합은 2018년 7월 1일까지 특정 지원되는 API 버전을 호출하도록 업데이트해야 합니다.

## 사용 중인 API 버전 확인

Workfront API로 전송된 HTTP 요청의 URI를 확인하여 사용 중인 API 버전을 확인할 수 있습니다. 다음 예는 API의 버전 7을 지정하는 Workfront 요청 URI를 보여줍니다.

`https://<domainname>.my.workfront.com/attask/api/v7.0/proj/4c7c08b20000002de5ca1ebc19edf2d5`

URI가 버전을 지정하지 않는 경우 다음 예와 같이 API의 기본 버전을 사용합니다.

`https://<domainname>.my.workfront.com/attask/api/proj/4c7c08b20000002de5ca1ebc19edf2d5`

>[!IMPORTANT]
>
> URI에서 API 버전을 지정하지 않는 통합은 자동으로 API의 기본 버전으로 라우팅되며 2018년 7월 1일 이후에는 작동하지 않습니다.

## 지원되는 API 버전을 사용하도록 통합 업데이트

Workfront 통합을 작성하거나 유지 관리할 때 API 버전 및 변경할 수 있는 기타 속성(예: API 키)을 동적으로 업데이트하는 방법을 포함해야 합니다.

통합을 보다 효율적으로 업데이트하려면 통합 값을 기록하기 위해 다음 제안을 고려해야 합니다.

* 업데이트한 상태로 유지하는 속성 파일에 향후 변경 사항에 따라 값을 저장합니다
* 속성을 실시간으로 관리하는 웹 서비스 만들기
* 애플리케이션이 읽을 수 있는 데이터 저장소에 속성 값을 저장합니다

이러한 값을 염두에 두고 Workfront 통합을 디자인하면 이러한 값이 필연적으로 변경될 때 광범위한 개발 작업이 필요합니다.
