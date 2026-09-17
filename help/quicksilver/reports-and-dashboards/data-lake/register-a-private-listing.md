---
content-type: reference
product-area: reports and dashboards
navigation-topic: data connect
title: Workfront Data Connect의 비공개 목록 등록
description: Snowflake 비공개 목록을 등록하여 Workfront Data Connect 데이터를 조직의 Snowflake 계정과 직접 공유합니다.
author: Courtney
feature: Reports and Dashboards
exl-id:
last-update: 2026-09-15T00:00:00.000Z
product_v2:
  - id: c4a86a5d-6562-4fc6-aa00-bfa25833aed9
    internal-label: Workfront
feature_v2:
  - id: d968a1bc-9a90-4926-a531-bcf272c32aad
    internal-label: Administration
role_v2:
  - id: b69b2659-1057-424e-8fc5-ed9e016dc554
    internal-label: User
topic_v2:
  - id: aa2f3246-cb95-4b30-8899-fdf7d73550cc
    internal-label: Reporting
  - id: eddd9b14-83bd-4ff4-9072-54a4a484abb7
    internal-label: Administration
source-git-commit: ed31fce397f9e99e7049d4f55eaca94f43dfcf5c
workflow-type: tm+mt
source-wordcount: '1060'
ht-degree: 1%
---
# Workfront Data Connect의 비공개 목록 등록

비공개 목록을 등록하여 Workfront Data Connect 데이터를 조직의 Snowflake 계정과 직접 공유할 수 있습니다. 이 연결 방법은 Snowflake의 비공개 목록 기능을 사용하여 데이터를 공개적으로 노출하지 않고 조직 간에 안전하게 공유하며 지역 및 호스팅 플랫폼에서 작동합니다.

비공개 목록은 Workfront 데이터를 엔터프라이즈 데이터 웨어하우스의 다른 데이터와 결합하려는 경우 유용합니다. 데이터가 고유한 Snowflake 계정에 저장되므로 나머지 데이터와 함께 쿼리할 수 있습니다.

## 액세스 요구 사항

+++ 를 확장하여 액세스 요구 사항을 확인합니다.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront 패키지</td> 
   <td><p>Ultimate</p>
    <p>워크플로 얼티밋</p>
   </td>
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront 라이선스</td> 
   <td>
   <p>표준</p>
   <p>플랜</p></td> 
  </tr> 
  <tr> 
   <td role="rowheader">액세스 수준 구성</td> 
   <td> <p>Workfront 관리자여야 합니다.</p></td> 
  </tr> 
 </tbody> 
</table>

이 표의 정보에 대한 자세한 내용은 [Workfront 설명서의 액세스 요구 사항](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)을 참조하십시오.

+++

또한 목록을 수락하고 데이터베이스를 만들 수 있는 권한이 있는 Snowflake 계정과 Workfront Data Connect 권한이 필요합니다.

## 비공개 목록이 공유하는 항목

비공개 목록을 통해 다음에 액세스할 수 있습니다.

* Workfront 개체에 대한 100개 이상의 데이터 보기. 각 보기에 대한 설명은 [Workfront Data Connect 데이터 사전](/help/quicksilver/reports-and-dashboards/data-lake/data-dictionary.md)을 참조하십시오.
* Data Connect 데이터 파이프라인에 전달된 각 변경 트랜잭션을 포함하는 `*_event` 데이터 보기입니다.
* 데이터 확장 가능 개체에 대한 사용자 지정 데이터 값입니다. 예를 들어 [Workfront Data Connect 쿼리 예제](/help/quicksilver/reports-and-dashboards/data-lake/basic-query-examples.md)에서 사용자 지정 데이터 쿼리 예제를 참조하십시오.

## 판독기 계정 연결과의 차이점

비공개 목록은 리더 계정 연결과 다른 보기 세트를 공유하며, 데이터는 다른 일정에 따라 도달합니다. 다음 차이점을 염두에 두십시오.

* 비공개 목록은 `*_event` 보기만 공유합니다. `*_current` 및 `*_daily_history` 보기는 Reader 계정을 통해 사용할 수 있지만 개인 목록을 통해서는 사용할 수 없습니다. 고유한 Snowflake 계정에서 빌드할 수 있습니다. 자세한 내용은 이 문서에서 [현재 및 일별 내역 보기 설정](#set-up-current-and-daily-history-views)을 참조하십시오.
* 비공개 목록에는 판독기 계정을 통해 사용할 수 있는 모든 보기가 포함되지 않을 수 있습니다. 공유되지 않는 보기의 예로는 Workfront Planning 개체 `MONITORING_DATA_REFRESHES`, `BOOKINGS` 및 `CLASSIFIER`이(가) 있습니다. 이 목록은 완전하지 않습니다.
* Data Connect는 4시간마다 변경 이벤트를 로드합니다. 비공개 목록에는 데이터를 표시하기 위해 추가 복제 단계가 필요하므로 데이터가 리더 계정을 통해 전송되는 것보다 약 1시간 더 걸릴 것으로 예상됩니다.
* 데이터 복제는 01:01, 05:01, 09:01, 13:01, 17:01 및 21:01 UTC에서 실행됩니다. 데이터는 일반적으로 각 실행 후 약 10분 내에 사용할 수 있습니다.
* `MONITORING_DATA_REFRESHES` 및 `JOB_HISTORY` 보기에는 비공개 목록을 통해 데이터를 사용할 수 있는 시간이 반영되지 않습니다. `JOB_HISTORY` 보기는 비공개 목록을 통해 공유되지만 실패한 작업을 더 빨리 식별하려면 판독기 계정을 통해 읽는 것이 좋습니다.

## 비공개 목록 등록

비공개 목록을 등록하려면 먼저 Snowflake 계정 세부 정보를 수집한 다음 Workfront에서 목록을 추가하십시오.

### Snowflake 계정 세부 정보 수집

Workfront은 Snowflake 계정 세부 사항을 사용하여 목록을 사용자 계정으로 타깃팅합니다. 다음 세부 정보를 수집합니다.

* 계정 로케이터
* 계정 URL
* 계정 조직
* 계정 이름

이러한 각 값은 Snowflake의 계정 세부 사항 모달에서 사용할 수 있습니다.

계정 세부 정보를 찾으려면

1. Snowflake 계정에 로그인하는 동안 왼쪽 하단의 사용자 메뉴를 클릭합니다.

1. 메뉴의 **계정** 섹션에서 계정을 선택합니다.

1. 해당 계정의 **계정 세부 정보 보기**&#x200B;를 클릭합니다.

1. 위에 나열된 각 값을 기록합니다.

또한 연결된 Workfront 데이터에 액세스할 데이터베이스의 이름도 결정합니다. 목록을 등록할 때 이 이름을 입력합니다.

### Workfront에서 비공개 목록 추가

Adobe Workfront 인터페이스를 통해 비공개 목록을 등록합니다.

>[!IMPORTANT]
>
>계정 로케이터당 하나의 비공개 목록만 만들 수 있습니다.

1. Adobe Workfront의 오른쪽 상단에 있는 **[!UICONTROL 주 메뉴]** 아이콘 ![주 메뉴](/help/_includes/assets/main-menu-icon.png)을 클릭하거나(가능한 경우) 왼쪽 상단에 있는 **[!UICONTROL 주 메뉴]** 아이콘 ![주 메뉴](/help/_includes/assets/main-menu-icon-left-nav.png)을 클릭한 다음 **설정**&#x200B;을 클릭합니다.

1. 왼쪽 패널에서 **시스템** > **데이터 연결**&#x200B;을 클릭합니다.

1. **Snowflake 연결** 탭을 클릭합니다.

1. **비공개 목록 추가**&#x200B;를 클릭합니다.

1. 기본 데이터베이스 이름을 포함하여 수집한 계정 세부 정보로 양식을 작성합니다.

1. **비공개 목록 추가**&#x200B;를 클릭합니다.

### Snowflake의 목록에 연결

Snowflake 계정에서 비공개 목록에 대한 연결을 외부 데이터 소스로 설정합니다. 그런 다음 나머지 데이터와 함께 Workfront 데이터를 쿼리할 수 있습니다.

## 현재 및 일별 내역 보기 설정

판독기 계정 연결은 각 개체 테이블에 대해 세 개의 데이터 보기를 제공합니다.

* **현재** — 원본 응용 프로그램에 있는 데이터의 대기 시간이 짧은 표현입니다.
* **일별 기록** — 매일 오후 11시 59분(UTC)에 있는 데이터를 나타냅니다.
* **이벤트** — Data Connect 데이터 파이프라인에 전달된 각 변경 트랜잭션입니다.

비공개 목록은 이벤트 보기만 공유합니다. 이 섹션에서는 SQL을 제공하여 현재, 일별 내역 및 이벤트 보기를 고유한 Snowflake 계정에서 작성합니다.

목록에 포함된 모든 이벤트 보기에는 아래 보기 논리에 필요한 필드가 있습니다. 이러한 예제에서는 대상 Snowflake 계정에서 선택한 새 데이터베이스 및 스키마를 만들었으며, `projects_event` 보기를 사용한다고 가정합니다. 각 예에서 `<listing_db>` 및 `<listing_schema>`을(를) 고유한 값으로 바꿉니다.

>[!TIP]
>
>`select *`을(를) 분석에 사용하는 열 목록으로 바꾸는 것이 좋습니다. `select *`을(를) 사용하고 열을 나중에 목록의 이벤트 보기에 추가하는 경우 새 열을 사용하려면 보기를 다시 만들어야 합니다.

### 현재 보기

개체의 현재 보기는 Data Connect에 저장된 마지막 변경 이벤트 레코드입니다. 마지막 레코드가 삭제된 상태이면 현재 보기에서 레코드가 생략됩니다. 모든 이벤트 보기의 구조는 동일합니다.

```sql
create or replace view projects_current copy grants
as
select *
from <listing_db>.<listing_schema>.projects_event
where end_effective_timestamp = '2300-01-01'::timestamp_ntz
 and nvl(deleted, 0) != 1;
```

현재 보기에서는 `deleted` 및 `end_effective_timestamp` 열이 필요하지 않습니다. 이 보기는 데이터를 단일 값으로 필터링하며 레코드가 삭제될 경우 레코드를 완전히 제거합니다.

### 일별 내역 보기

일별 내역 보기는 지정된 날짜의 23:59:59에 활성 상태인 변경 이벤트 레코드를 식별하므로 시간에 따른 레코드 상태의 트렌드를 표시할 수 있습니다. 다음 예제에서는 각 달력의 날짜가 끝날 때 프로젝트 레코드의 상태를 제공합니다.

```sql
create or replace view projects_daily_history copy grants
as
select d.calendardate as
 , p.*
from <listing_db>.<listing_schema>.calendar_dates d
join <listing_db>.<listing_schema>.projects_event p
 on p.begin_effective_timestamp <= d.calendareodtimestamp
and d.calendareodtimestamp < p.end_effective_timestamp
where d.calendareodtimestamp < current_date() - 1
 and nvl(deleted, 0) != 1;
```

### 이벤트 보기

일관성을 위해 목록 데이터베이스에서 이벤트 보기의 복사본을 만들고 현재 및 일일 기록 보기와 동일한 스키마에 배치하는 것이 좋습니다.

```sql
create or replace view projects_event copy grants
as
select *
from <listing_db>.<listing_schema>.projects_event;
```
