---
content-type: api
navigation-topic: api-navigation-topic
title: 통합에서 API 버전 지정
description: 통합에서 API 버전 지정
author: Becky
feature: Workfront API
exl-id: 2971749d-1d34-42a4-9eda-411aa8c3a2ab
source-git-commit: 2b9eacc9b2c8f499cdd1794a55879a56224051c8
workflow-type: tm+mt
source-wordcount: '0'
ht-degree: 0%

---

# 통합에서 API 버전을 지정합니다

모든 Adobe Workfront URI는 URI의 &quot;attask/api&quot; 부분 뒤에 특정 버전의 API를 참조해야 합니다. 다음 예에서는 버전 15.0을 호출합니다.

`attask/api/v15.0/<objectName>/<objectId>`

모든 통합 호출이 현재 지원되는 Workfront API인지 확인하십시오.

## Workfront API의 릴리스 및 사용 중단 일정

새로운 버전의 API는 일반적으로 1년에 두 번 정기적으로 릴리스됩니다. 각 버전은 릴리스 날짜 이후 3년 동안 지원되며, 버전은 사용 가능하지만 지원되지 않는 더 이상 사용되지 않는 상태에서 추가 연도를 사용할 수 있습니다.

Workfront API의 릴리스 주기 및 사용 중단 예약에 대한 자세한 내용은 [API 버전 관리 및 지원 예약](../../wf-api/api/api-version-support-schedule.md).

>[!IMPORTANT]
>
>* API의 기본 버전이 최신 버전으로 설정되어 있습니다. 지정된 버전이 없는 모든 API 호출은 기본 버전을 사용합니다. Workfront이 새로운 버전의 API를 릴리스할 때마다 기본 버전이 최신 버전으로 업데이트됩니다. **따라서 새 버전의 Workfront API가 릴리스된 후 기본 버전을 사용하는 모든 API 호출을 확인하여 기능이 계속 지원되는지 확인해야 합니다.**
>
>* 조직에서 현재 기본 API를 사용하고 있는 경우 Workfront 관리자가 기본 API에 대한 추가 지침이 포함된 공지 센터 메시지를 수신했습니다.
>
>최신 버전의 API를 보려면 [API 버전 관리 및 지원 예약](../../wf-api/api/api-version-support-schedule.md).


## 사용 중인 API 버전 확인

Workfront API로 전송된 HTTP 요청의 URI를 확인하여 사용 중인 API 버전을 확인할 수 있습니다. 다음 예는 API의 버전 15를 지정하는 Workfront 요청 URI를 보여줍니다.

`https://<domainname>.my.workfront.com/attask/api/v15.0/proj/4c7c08b20000002de5ca1ebc19edf2d5`

URI가 버전을 지정하지 않는 경우 다음 예와 같이 API의 기본 버전을 사용합니다.

`https://<domainname>.my.workfront.com/attask/api/proj/4c7c08b20000002de5ca1ebc19edf2d5`

>[!IMPORTANT]
>
> URI에서 API 버전을 지정하지 않는 통합은 자동으로 API의 기본 버전으로 라우팅됩니다.

## 지원되는 API 버전을 사용하도록 통합 업데이트

Workfront 통합을 작성하거나 유지 관리할 때 API 버전 및 변경할 수 있는 기타 속성(예: API 키)을 동적으로 업데이트하는 방법을 포함해야 합니다.

통합을 보다 효율적으로 업데이트하려면 통합 값을 기록하기 위해 다음 제안을 고려해야 합니다.

* 업데이트한 상태로 유지하는 속성 파일에 향후 변경 사항에 따라 값을 저장합니다
* 속성을 실시간으로 관리하는 웹 서비스 만들기
* 애플리케이션이 읽을 수 있는 데이터 저장소에 속성 값을 저장합니다

이러한 값을 염두에 두고 Workfront 통합을 디자인하면 이러한 값이 필연적으로 변경될 때 광범위한 개발 작업이 필요합니다.
