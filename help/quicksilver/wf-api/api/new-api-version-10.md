---
content-type: api
navigation-topic: api-navigation-topic
title: API 버전 10의 새로운 기능
description: 업데이트된 리소스
author: John
feature: Workfront API
exl-id: 8ac384ae-5d65-4c0e-98c1-cf38cfbff460
source-git-commit: f2f825280204b56d2dc85efc7a315a4377e551c7
workflow-type: tm+mt
source-wordcount: '571'
ht-degree: 45%

---

# API 버전 10의 새로운 기능

* [새 리소스](#new-resources)
* [업데이트된 리소스](#updated-resources)
* [제거된 리소스](#removed-resources)

## 새 리소스 {#new-resources}

### ActivityLog

| 필드 | 참조 | 컬렉션 | 검색 | 액션 | 쿼리 | 작업 |
|---|---|---|---|---|---|---|
|   |   |   |   |   |   | 추가 |
|   |   |   |   |   |   | 카운트 |
|   |   |   |   |   |   | GET |
|   |   |   |   |   |   | 검색 |

{style=&quot;table-layout:auto&quot;}

### CalendarEntry

| 필드 | 참조 | 컬렉션 | 검색 | 액션 | 쿼리 | 작업 |
|---|---|---|---|---|---|---|
| ID |   |   |   |   |   | 추가 |
|   |   |   |   |   |   | 카운트  |
|   |   |   |   |   |   | DELETE  |
|   |   |   |   |   |   | 편집  |
|   |   |   |   |   |   | GET  |
|   |   |   |   |   |   | 보고서  |
|   |   |   |   |   |   | 검색 |

{style=&quot;table-layout:auto&quot;}

### CalendarEntryExternalReference

| 필드 | 참조 | 컬렉션 | 검색 | 액션 | 쿼리 | 작업 |
|---|---|---|---|---|---|---|
| ID |   |   |   |   |   | 카운트 |
|   |   |   |   |   |   | GET  |
|   |   |   |   |   |   | 보고서  |
|   |   |   |   |   |   | 검색  |

{style=&quot;table-layout:auto&quot;}

### ExternalAuthToken

| 필드 | 참조 | 컬렉션 | 검색 | 액션 | 쿼리 | 작업 |
|---|---|---|---|---|---|---|
| ID |   |   |   |   |   | 추가 |
|   |   |   |   |   |   | 카운트 |
|   |   |   |   |   |   | DELETE  |
|   |   |   |   |   |   | 편집  |
|   |   |   |   |   |   | GET  |
|   |   |   |   |   |   | 보고서  |
|   |   |   |   |   |   | 검색  |

{style=&quot;table-layout:auto&quot;}

### LicenseTypeGroupLimit

| 필드 | 참조 | 컬렉션 | 검색 | 액션 | 쿼리 | 작업 |
|---|---|---|---|---|---|---|
| customerID | 고객 |   |   |   |   |   |
| groupID | 그룹 |   |   |   |   |   |
| planLimit |   |   |   |   |   |   |
| usedLicenses |   |   |   |   |   |   |
| 작업량 제한 |   |   |   |   |   |   |
|   |   |   |   |   |   |   |
|   |   |   |   |   |   |   |

{style=&quot;table-layout:auto&quot;}

### UserHomeCalendarPreference

| 필드 | 참조 | 컬렉션 | 검색 | 액션 | 쿼리 | 작업 |
|---|---|---|---|---|---|---|
| customerID | 고객 |   |   |   |   | 추가 |
| edTime | 사용자 |   |   |   |   | 카운트 |
| firstDayOfWeek |   |   |   |   |   | DELETE |
| ID |   |   |   |   |   | 편집 |
| showPTO |   |   |   |   |   | GET |
| startTime |   |   |   |   |   | 보고서 |
| userID |   |   |   |   |   | 검색 |
| workDate |   |   |   |   |   |   |

{style=&quot;table-layout:auto&quot;}

**업데이트된 리소스**

다음 기존 리소스가 이 Workfront API 릴리스로 업데이트되었습니다. 리소스에 대한 변경 사항은 다음과 같이 표시됩니다.

* 추가는 단순히 나열됨
* 제거는 취소선 텍스트로 표시됩니다
* 변경 사항은 테이블 뒤에 메모에 나열됩니다

### 승인

| 필드 | 참조 | 컬렉션 | 검색 | 액션 | 쿼리 | 작업 |
|---|---|---|---|---|---|---|
| 간판 플래그 |  |  | pendingApproval `¹`   |   |   |   |
| `masterTaskID` |   |   |   |   |   |   |
| priorityColor  |   |   |   |   |   |   |
| projectBudgetCost  |   |   |   |   |   |   |
| projectNetValue  |   |   |   |   |   |   |
| projectRoi  |   |   |   |   |   |   |
| resourcePlannerScheduledLaborCost  |   |   |   |   |   |   |

{style=&quot;table-layout:auto&quot;}

`¹ Type changed from null to boolean`

### 할당

| 필드 | 참조 | 컬렉션 | 검색 | 액션 | 쿼리 | 작업 |
|---|---|---|---|---|---|---|
| assignmentPercent `¹` |   |   |   |   |   |   |
| viewedByAssignedToUser |   |   |   |   |   |   |

{style=&quot;table-layout:auto&quot;}

`¹`유효성 검사기 LESS_THAN_EQUAL가 추가되었습니다.

### 예산책정 시간

| 필드 | 참조 | 컬렉션 | 검색 | 액션 | 쿼리 | 작업 |
|---|---|---|---|---|---|---|
| ID |   |   |   |   |   |   |

{style=&quot;table-layout:auto&quot;}

 

### 고객 기본 설정

| 필드 | 참조 | 컬렉션 | 검색 | 액션 | 쿼리 | 작업 |
|---|---|---|---|---|---|---|
| 이름 `¹` |   |   |   |   |   |   |

{style=&quot;table-layout:auto&quot;}

¹ 가능한 값 변경

### DocMetadataLinkGroup

| 필드 | 참조 | 컬렉션 | 검색 | 액션 | 쿼리 | 작업 |
|---|---|---|---|---|---|---|
|   |   |   |   | getMetadataForDocument |   |   |

{style=&quot;table-layout:auto&quot;}

### 문서

| 필드 | 참조 | 컬렉션 | 검색 | 액션 | 쿼리 | 작업 |
|---|---|---|---|---|---|---|
| `masterTaskID` |  |  |  |  |  |  |

{style=&quot;table-layout:auto&quot;}

### DocumentRequest

| 필드 | 참조 | 컬렉션 | 검색 | 액션 | 쿼리 | 작업 |
|---|---|---|---|---|---|---|
| `masterTaskID` |  |  |  |  |  |  |

{style=&quot;table-layout:auto&quot;}

DocumentVersion

| 필드 | 참조 | 컬렉션 | 검색 | 액션 | 쿼리 | 작업 |
|---|---|---|---|---|---|---|
| externalIntegrationType ¹ |   |   |   |   |   |   |
|   |   |   |   |   |   |   |
|   |   |   |   |   |   |   |
|   |   |   |   |   |   |   |

{style=&quot;table-layout:auto&quot;}

¹ 가능한 값 변경

경비

| 필드 | 참조 | 컬렉션 | 검색 | 액션 | 쿼리 | 작업 |
|---|---|---|---|---|---|---|
| `masterTaskID` |   |   |   |   |   |   |

{style=&quot;table-layout:auto&quot;}

### 그룹

| 필드 | 참조 | 컬렉션 | 검색 | 액션 | 쿼리 | 작업 |
|---|---|---|---|---|---|---|
|   | licenseTypeLimit |   |   | addRemoveLicenseTypeLimits  |   |   |
|   |   |   |   | setLicenseTypeLimit |   |   |

{style=&quot;table-layout:auto&quot;}

### LinkedFolder

| 필드 | 참조 | 컬렉션 | 검색 | 액션 | 쿼리 | 작업 |
|---|---|---|---|---|---|---|
| externalIntegrationType¹ |  |  |  |  |  |  |

{style=&quot;table-layout:auto&quot;}

¹ 가능한 값 변경

### OpTask

| 필드 | 참조 | 컬렉션 | 검색 | 액션 | 쿼리 | 작업 |
|---|---|---|---|---|---|---|
| priorityColor |  |  | pendingApproval¹ |  |  |  |

{style=&quot;table-layout:auto&quot;}

¹ 유형이 null에서 부울로 변경됨

### 포털 섹션

| 필드 | 참조 | 컬렉션 | 검색 | 액션 | 쿼리 | 작업 |
|---|---|---|---|---|---|---|
|  |  |  | groupIDs |  |  |  |

{style=&quot;table-layout:auto&quot;}

### 포트폴리오

| 필드 | 참조 | 컬렉션 | 검색 | 액션 | 쿼리 | 작업 |
|---|---|---|---|---|---|---|
| portfolioNetValue |  |  |  |  |  |  |
| portfolioRoi |   |   |   |   |   |   |

{style=&quot;table-layout:auto&quot;}

### 프로젝트

| 필드 | 참조 | 컬렉션 | 검색 | 액션 | 쿼리 | 작업 |
|---|---|---|---|---|---|---|
| projectBudgetCost  |   |   |   | linkExternalObject  |   |   |
| projectNetValue |   |   |   | unlinkExternalObject |   |   |
| projectRoi |   |   |   |   |   |   |
| resourcePlannerScheduledLaborCost |   |   |   |   |   |   |

{style=&quot;table-layout:auto&quot;}

### 증명 승인

| 필드 | 참조 | 컬렉션 | 검색 | 액션 | 쿼리 | 작업 |
|---|---|---|---|---|---|---|
| 승인자 결정 |  |  |  |  |  |  |

{style=&quot;table-layout:auto&quot;}

### 요금

| 필드 | 참조 | 컬렉션 | 검색 | 액션 | 쿼리 | 작업 |
|---|---|---|---|---|---|---|
| rateValue ¹ |  |  |  |  |  |  |

{style=&quot;table-layout:auto&quot;}

¹유효성 검사기 통화가 추가되었습니다.

### 작업

| 필드 | 참조 | 컬렉션 | 검색 | 액션 | 쿼리 | 작업 |
|---|---|---|---|---|---|---|
| 간판 플래그 |   |   |   |   |   |   |
| `masterTaskID` |   |   |   |   |   |   |
| priorityColor  |   |   |   |   |   |   |

{style=&quot;table-layout:auto&quot;}

 

### 팀

| 필드 | 참조 | 컬렉션 | 검색 | 액션 | 쿼리 | 작업 |
|---|---|---|---|---|---|---|
| hoursPerPoint ¹ |   |   |   |   |   |   |

{style=&quot;table-layout:auto&quot;}

¹ 유효성 검사기 LESS_THAN 추가

### TeamAssignment

| 필드 | 참조 | 컬렉션 | 검색 | 액션 | 쿼리 | 작업 |
|---|---|---|---|---|---|---|
| `masterTaskID` |   |   |   |   |   |   |

{style=&quot;table-layout:auto&quot;}

### TeamTask

| 필드 | 참조 | 컬렉션 | 검색 | 액션 | 쿼리 | 작업 |
|---|---|---|---|---|---|---|
| `masterTaskID` |   |   |   |   |   |   |

{style=&quot;table-layout:auto&quot;}

### 타임시트

| 필드 | 참조 | 컬렉션 | 검색 | 액션 | 쿼리 | 작업 |
|---|---|---|---|---|---|---|
|   |   |   |   |   |   |   |

{style=&quot;table-layout:auto&quot;}

### 업데이트

| 필드 | 참조 | 컬렉션 | 검색 | 액션 | 쿼리 | 작업 |
|---|---|---|---|---|---|---|
| updateType `¹` |   |   |   |   |   | objectUpdatesWithNoteAndJournalEntryIndex  |

{style=&quot;table-layout:auto&quot;}

가능한 값 ¹ 변경

### 사용자

| 필드 | 참조 | 컬렉션 | 검색 | 액션 | 쿼리 | 작업 |
|---|---|---|---|---|---|---|
|   | accessLevel  |   |   |   |   |   |

{style=&quot;table-layout:auto&quot;}

### UserNote

| 필드 | 참조 | 컬렉션 | 검색 | 액션 | 쿼리 | 작업 |
|---|---|---|---|---|---|---|
| eventType ¹ |   |   |   |   |   |   |

{style=&quot;table-layout:auto&quot;}

가능한 값 ¹ 변경

### 작업

| 필드 | 참조 | 컬렉션 | 검색 | 액션 | 쿼리 | 작업 |
|---|---|---|---|---|---|---|
| 간판 플래그 |  |  | pendingApproval ¹  |   |   |   |
| `masterTaskID` |   |   |   |   |   |   |
| priorityColor  |   |   |   |   |   |   |

{style=&quot;table-layout:auto&quot;}

¹ 유형이 null에서 부울로 변경됨

## 제거된 리소스 {#removed-resources}

### 자원_예산책정된_시간

| 필드 | 참조 | 컬렉션 | 검색 | 액션 | 쿼리 | 작업 |
|---|---|---|---|---|---|---|
| allocationDate |   |   |   |   |   | 추가  |
| backgroundHours |   |   |   |   |   | 카운트  |
| ID |   |   |   |   |   | DELETE  |
| planningScheduledHours |   |   |   |   |   | 편집  |
| projectID |   |   |   |   |   | GET  |
| roleID |   |   |   |   |   | 보고서  |
| userID |   |   |   |   |   | 검색 |

{style=&quot;table-layout:auto&quot;}

 

 

 
