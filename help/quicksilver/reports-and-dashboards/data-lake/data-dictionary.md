---
content-type: reference
product-area: reports and dashboards
navigation-topic: data connect
title: Workfront Data Connect 데이터 사전
description: 이 페이지에는 Workfront Data Connect의 데이터 구조 및 내용에 대한 정보가 포함되어 있습니다.
author: Nolan
feature: Reports and Dashboards
recommendations: noDisplay, noCatalog
exl-id: 57985404-554e-4289-b871-b02d3427aa5c
source-git-commit: 16809b2d1801dd7aa4ab1f452e4687601fc1ac59
workflow-type: tm+mt
source-wordcount: '726'
ht-degree: 5%

---

# Workfront Data Connect 데이터 사전

이 페이지에는 Workfront Data Connect의 데이터 구조 및 내용에 대한 정보가 포함되어 있습니다.

>[!NOTE]
>
>Data Connect의 데이터는 4시간마다 새로 고침되므로 최근 변경 사항이 즉시 반영되지 않을 수 있습니다.

## 테이블 유형

Data Connect에서 최대한 통찰력을 제공하는 방식으로 Workfront 데이터를 보기 위해 활용할 수 있는 다양한 테이블 유형이 있습니다.

* **현재 테이블**

  현재 테이블은 모든 개체 및 현재 상태의 Workfront에 존재하는 것과 유사하게 데이터를 반영합니다. 하지만 Workfront 내에서보다 훨씬 짧은 지연 시간으로 탐색할 수 있습니다.

* **이벤트 테이블**

  이벤트 테이블은 Workfront의 모든 변경 레코드를 추적합니다. 즉, 객체가 상태를 변경할 때마다 변경 발생 시간, 변경한 사람 및 변경된 내용을 표시하는 레코드가 만들어집니다. 따라서 이 표는 시점 비교에 유용합니다. 이 표에는 지난 3년간의 기록만 포함되어 있습니다.

* **일별 기록 테이블**

  일별 내역 테이블은 각 개별 이벤트가 발생한 시점이 아니라 매일 각 객체의 상태를 표시한다는 점에서 이벤트 테이블의 축약된 버전을 제공합니다. 따라서 이 표는 추세 분석에 유용합니다.

<!-- Custom table -->

## 엔티티 관계 다이어그램

Workfront의 개체(및 따라서 Data Connect 데이터 레이크)는 개별 값뿐만 아니라 다른 개체와의 관계에 의해서도 정의됩니다. 아래의 엔티티 관계 다이어그램은 Data Connect에서 개체 관계의 높은 수준 매핑을 제공합니다. 다음 링크를 사용하여 다이어그램을 보고 다운로드할 수 있습니다.

[Data Connect 엔티티 관계 다이어그램](/help/quicksilver/reports-and-dashboards/data-lake/assets/Workfront-data-lake_entity-relationship-diagram.pdf)

>[!IMPORTANT]
>
>엔티티 관계 다이어그램은 진행 중인 작업입니다. 따라서 참조용으로만 사용되며 변경될 수 있습니다.

## 날짜 유형

특정 이벤트가 발생하는 시기에 대한 정보를 제공하는 다양한 날짜 개체가 있습니다.

* `DL_LOAD_TIMESTAMP`: 이 날짜는 내부 참조에 사용되며 데이터가 Current, Event 또는 Daily History 테이블에 로드된 시기를 반영합니다. 이 날짜는 데이터 분석에 사용되어서는 안 되며 Workfront 데이터 레이크의 베타 단계 동안 제거될 계획입니다.
* `CALENDAR_DATE`: 이 날짜는 [일별 기록] 테이블에만 있습니다. 이 테이블은 `CALENDAR_DATE`에 지정된 각 날짜에 대해 11:59 UTC에 데이터가 어떻게 보이는지에 대한 기록을 제공합니다.
* `BEGIN_EFFECTIVE_TIMESTAMP`: 이 날짜는 이벤트 및 일별 기록 테이블 모두에 있으며 레코드가 현재 행에 있는 값을 _to_(으)로 변경한 시기를 정확하게 기록합니다.
* `END_EFFECTIVE_TIMESTAMP`: 이 날짜는 이벤트 및 일일 기록 테이블 모두에 있으며 레코드가 현재 행의 값을 _부터_&#x200B;까지 다른 행의 값으로 변경한 정확한 시점을 기록합니다. `BEGIN_EFFECTIVE_TIMESTAMP`과(와) `END_EFFECTIVE_TIMESTAMP`의 쿼리 사이에 을(를) 허용하려면 새 값이 없어도 이 값은 null이 아닙니다. 레코드가 여전히 유효한 경우(즉, 값이 변경되지 않은 경우) `END_EFFECTIVE_TIMESTAMP`의 값은 2300-01-01입니다.

## 용어 표

다음 표는 Workfront의 개체 이름(인터페이스 및 API의 이름)과 Data Connect의 해당 이름을 상호 연결합니다.

<table>
<thead>
  <tr>
    <th>Workfront 엔티티 이름</th>
    <th>인터페이스 참조</th>
    <th>API 참조 | 레이블</th>
    <th>데이터 레이크 테이블</th>
    <th>메모</th>
  </tr>
</thead>
<tbody>
  <tr>
    <td>할당</td>
    <td>할당</td>
    <td>ASSIGN | 할당</td>
    <td>ASSIGNMENTS_CURRENT<br>ASSIGNMENTS_DAILY_HISTORY<br>ASSIGNMENTS_EVENT</td>
    <td></td>
  </tr>
  <tr>
    <td>CustomEnum</td>
    <td>상태, 우선 순위, 심각도, 상태</td>
    <td>CSTEM | 사용자 정의 열거형</td>
    <td>CUSTOMENUMS_CURRENT<br>CUSTOMENUMS_DAILY_HISTORY<br>CUSTOMENUMS_EVENT</td>
    <td>레코드 유형은 'enumClass' 속성을 통해 식별됩니다. 다음은 예상 유형입니다.<br>CONDITION_OPTASK<br>CONDITION_PROJ<br>CONDITION_TASK<br>PRIORITY_OPTASK<br>PRIORITY_PROJ<br>PRIORITY_TASK<br>SEVERITY_OPTASK<br>STATUS_OPTASK<br>STATUS_PROJ<br>STATUS_TASK</td>
  </tr>
  <tr>
    <td>문서</td>
    <td>문서</td>
    <td>도쿠 | 문서</td>
    <td>DOCUMENTS_CURRENT<br>DOCUMENTS_DAILY_HISTORY<br>DOCUMENTS_EVENT<br><br>DOCUMENTS_CUSTOM_VALUE_CURRENT<br>DOCUMENTS_CUSTOM_VALUE_DAILY_HISTORY<br>DOCUMENTS_CUSTOM_VALUE_EVENT</td>
    <td></td>
  </tr>
  <tr>
    <td>DocumentVersion</td>
    <td>문서 버전</td>
    <td>DOCV | 문서 버전</td>
    <td>DOCUMENTVERSIONS_CURRENT<br>DOCUMENTVERSIONS_DAILY_HISTORY<br>DOCUMENTVERSIONS_EVENT</td>
    <td></td>
  </tr>
  <tr>
    <td>그룹</td>
    <td>그룹</td>
    <td>그룹 | 그룹</td>
    <td>GROUPS_CURRENT<br>GROUPS_DAILY_HISTORY<br>GROUPS_EVENT</td>
    <td></td>
  </tr>
  <tr>
    <td>시간</td>
    <td>시간</td>
    <td>시간 | 시간</td>
    <td>HOURS_CURRENT<br>HOURS_DAILY_HISTORY<br>HOURS_EVENT</td>
    <td></td>
  </tr>
  <tr>
    <td>시간 유형</td>
    <td>시간 유형</td>
    <td>시간 | 시간 유형</td>
    <td>HOURTYPES_CURRENT</td>
    <td></td>
  </tr>
  <tr>
    <td>마일스톤</td>
    <td>마일스톤</td>
    <td>마일 | 마일스톤</td>
    <td>MILESTONES_CURRENT<br>MILESTONES_DAILY_HISTORY<br>MILESTONES_EVENT</td>
    <td></td>
  </tr>
  <tr>
    <td>마일스톤 경로</td>
    <td>마일스톤 경로</td>
    <td>MPATH | 마일스톤 경로</td>
    <td>MILESTONEPATHS_CURRENT<br>MILESTONEPATHS_DAILY_HISTORY<br>MILESTONEPATHS_EVENT</td>
    <td></td>
  </tr>
  <tr>
    <td>참고</td>
    <td>참고</td>
    <td>참고 | 참고</td>
    <td>NOTES_CURRENT<br>NOTES_DAILY_HISTORY<br>NOTES_EVENT</td>
    <td></td>
  </tr>
  <tr>
    <td>OpTask</td>
    <td>문제, 요청</td>
    <td>OPTASK | 문제</td>
    <td>OPTASKS_CURRENT<br>OPTASKS_DAILY_HISTORY<br>OPTASKS_EVENT<br><br>OPTASKS_CUSTOM_VALUE_CURRENT<br>OPTASKS_CUSTOM_VALUE_DAILY_HISTORY<br>OPTASKS_CUSTOM_VALUE_EVENT</td>
    <td></td>
  </tr>
  <tr>
    <td>Portfolio</td>
    <td>Portfolio</td>
    <td>포트 | Portfolio</td>
    <td>PORTFOLIO_CURRENT<br>PORTFOLIO_DAILY_HISTORY<br>PORTFOLIO_EVENT<br><br>PORTFOLIO_CUSTOM_VALUE_CURRENT<br>PORTFOLIO_CUSTOM_VALUE_DAILY_HISTORY<br>PORTFOLIO_CUSTOM_VALUE_EVENT</td>
    <td></td>
  </tr>
  <tr>
    <td>프로그램</td>
    <td>프로그램</td>
    <td>PRGM | 프로그램</td>
    <td>PROGRAMS_CURRENT<br>PROGRAMS_DAILY_HISTORY<br>PROGRAMS_EVENT<br><br>PROGRAMS_CUSTOM_VALUE_CURRENT<br>PROGRAMS_CUSTOM_VALUE_DAILY_HISTORY<br>PROGRAMS_CUSTOM_VALUE_EVENT</td>
    <td></td>
  </tr>
  <tr>
    <td>프로젝트</td>
    <td>프로젝트</td>
    <td>프로젝트 | 프로젝트</td>
    <td>PROJECTS_CURRENT<br>PROJECTS_DAILY_HISTORY<br>PROJECTS_EVENT<br><br>PROJECTS_CUSTOM_VALUE_CURRENT<br>PROJECTS_CUSTOM_VALUE_DAILY_HISTORY<br>PROJECTS_CUSTOM_VALUE_EVENT</td>
    <td></td>
  </tr>
  <tr>
    <td>역할</td>
    <td>작업 역할</td>
    <td>역할 | 작업 역할</td>
    <td>ROLES_CURRENT<br>ROLES_DAILY_HISTORY<br>ROLES_EVENT</td>
    <td></td>
  </tr>
  <tr>
    <td>예약</td>
    <td>예약</td>
    <td>일정 조정됨 | 예약</td>
    <td>SCHEDULES_CURRENT<br>SCHEDULES_DAILY_HISTORY<br>SCHEDULES_EVENT</td>
    <td></td>
  </tr>
  <tr>
    <td>작업</td>
    <td>작업</td>
    <td>작업 | 작업</td>
    <td>TASKS_CURRENT<br>TASKS_DAILY_HISTORY<br>TASKS_EVENT<br><br>TASKS_CUSTOM_VALUE_CURRENT<br>TASKS_CUSTOM_VALUE_DAILY_HISTORY<br>TASKS_CUSTOM_VALUE_EVENT</td>
    <td></td>
  </tr>
  <tr>
    <td>팀</td>
    <td>팀</td>
    <td>TEAOB | 팀</td>
    <td>TEAMS_CURRENT<br>TEAMS_DAILY_HISTORY<br>TEAMS_EVENT</td>
    <td></td>
  </tr>
  <tr>
    <td>타임시트</td>
    <td>타임시트</td>
    <td>체트 | 타임시트</td>
    <td>TIMESHEETS_CURRENT<br>TIMESHEETS_DAILY_HISTORY<br>TIMESHEETS_EVENT</td>
    <td></td>
  </tr>
  <tr>
    <td>사용자</td>
    <td>사용자</td>
    <td>사용자 | 사용자</td>
    <td>USERS_CURRENT<br>USERS_DAILY_HISTORY<br>USERS_EVENT<br><br>USERS_CUSTOM_VALUE_CURRENT<br>USERS_CUSTOM_VALUE_DAILY_HISTORY<br>USERS_CUSTOM_VALUE_EVENT</td>
    <td></td>
  </tr>
</tbody>
</table>
