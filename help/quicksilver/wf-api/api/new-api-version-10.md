---
content-type: api
navigation-topic: api-navigation-topic
title: API 버전 10의 새로운 기능
description: 업데이트된 리소스
author: Becky
feature: Workfront API
role: Developer
exl-id: 8ac384ae-5d65-4c0e-98c1-cf38cfbff460
source-git-commit: 3e339e2bfb26e101f0305c05f620a21541394993
workflow-type: tm+mt
source-wordcount: '487'
ht-degree: 39%

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
|   |   |   |   |   |   | 수 |
|   |   |   |   |   |   | GET |
|   |   |   |   |   |   | 검색 |

{style="table-layout:auto"}

### CalendarEntry

| 필드 | 참조 | 컬렉션 | 검색 | 액션 | 쿼리 | 작업 |
|---|---|---|---|---|---|---|
| ID |   |   |   |   |   | 추가 |
|   |   |   |   |   |   | 수  |
|   |   |   |   |   |   | DELETE  |
|   |   |   |   |   |   | 편집  |
|   |   |   |   |   |   | GET  |
|   |   |   |   |   |   | 보고서  |
|   |   |   |   |   |   | 검색 |

{style="table-layout:auto"}

### CalendarEntryExternalReference

| 필드 | 참조 | 컬렉션 | 검색 | 액션 | 쿼리 | 작업 |
|---|---|---|---|---|---|---|
| ID |   |   |   |   |   | 수 |
|   |   |   |   |   |   | GET  |
|   |   |   |   |   |   | 보고서  |
|   |   |   |   |   |   | 검색  |

{style="table-layout:auto"}

### ExternalAuthToken

| 필드 | 참조 | 컬렉션 | 검색 | 액션 | 쿼리 | 작업 |
|---|---|---|---|---|---|---|
| ID |   |   |   |   |   | 추가 |
|   |   |   |   |   |   | 수 |
|   |   |   |   |   |   | DELETE  |
|   |   |   |   |   |   | 편집  |
|   |   |   |   |   |   | GET  |
|   |   |   |   |   |   | 보고서  |
|   |   |   |   |   |   | 검색  |

{style="table-layout:auto"}

### 라이선스 유형 그룹 제한

| 필드 | 참조 | 컬렉션 | 검색 | 액션 | 쿼리 | 작업 |
|---|---|---|---|---|---|---|
| customerID | 고객 |   |   |   |   |   |
| groupID | 그룹 |   |   |   |   |   |
| planLimit |   |   |   |   |   |   |
| usedLicenses |   |   |   |   |   |   |
| 작업 제한 |   |   |   |   |   |   |
|   |   |   |   |   |   |   |
|   |   |   |   |   |   |   |

{style="table-layout:auto"}

### UserHomeCalendarPreference

| 필드 | 참조 | 컬렉션 | 검색 | 액션 | 쿼리 | 작업 |
|---|---|---|---|---|---|---|
| customerID | 고객 |   |   |   |   | 추가 |
| edTime | 사용자 |   |   |   |   | 수 |
| firstDayOfWeek |   |   |   |   |   | DELETE |
| ID |   |   |   |   |   | 편집 |
| showPTO |   |   |   |   |   | GET |
| startTime |   |   |   |   |   | 보고서 |
| userID |   |   |   |   |   | 검색 |
| 작업 날짜 |   |   |   |   |   |   |

{style="table-layout:auto"}

**업데이트된 리소스**

다음 기존 리소스가 Workfront API의 이번 릴리스로 업데이트되었습니다. 리소스에 대한 변경 사항은 다음과 같이 표시됩니다.

* 추가 사항은 간단히 나열되어 있습니다
* 제거는 취소선 텍스트로 표시됩니다
* 변경 사항은 표 뒤에 있는 메모에 나열되어 있습니다

### 승인

| 필드 | 참조 | 컬렉션 | 검색 | 액션 | 쿼리 | 작업 |
|---|---|---|---|---|---|---|
| kanbanbflag |  |  | 승인 보류 중 `<sup>1</sup>`   |   |   |   |
| `masterTaskID` |   |   |   |   |   |   |
| priorityColor  |   |   |   |   |   |   |
| projectBudgetCost  |   |   |   |   |   |   |
| 프로젝트 순 가치  |   |   |   |   |   |   |
| projectRoi  |   |   |   |   |   |   |
| resourcePlannerBudgetedLaborCost  |   |   |   |   |   |   |

{style="table-layout:auto"}

`<sup>1</sup> Type changed from null to boolean`

### 할당

| 필드 | 참조 | 컬렉션 | 검색 | 액션 | 쿼리 | 작업 |
|---|---|---|---|---|---|---|
| assignmentPercent `<sup>1</sup>` |   |   |   |   |   |   |
| viewedByAssignedToUser |   |   |   |   |   |   |

{style="table-layout:auto"}

`<sup>1</sup>`검사기 LESS_THAN_EQUAL 추가됨

### BudgetedHour

| 필드 | 참조 | 컬렉션 | 검색 | 액션 | 쿼리 | 작업 |
|---|---|---|---|---|---|---|
| ID |   |   |   |   |   |   |

{style="table-layout:auto"}

 

### 고객 환경 설정

| 필드 | 참조 | 컬렉션 | 검색 | 액션 | 쿼리 | 작업 |
|---|---|---|---|---|---|---|
| 이름 `<sup>1</sup>` |   |   |   |   |   |   |

{style="table-layout:auto"}

possibleValues에 대한 <sup>1</sup> 변경 사항

### 문서 메타데이터 링크 그룹

| 필드 | 참조 | 컬렉션 | 검색 | 액션 | 쿼리 | 작업 |
|---|---|---|---|---|---|---|
|   |   |   |   | getMetadataForDocument |   |   |

{style="table-layout:auto"}

### 문서

| 필드 | 참조 | 컬렉션 | 검색 | 액션 | 쿼리 | 작업 |
|---|---|---|---|---|---|---|
| `masterTaskID` |  |   |   |   |   |   |

{style="table-layout:auto"}

### DocumentRequest

| 필드 | 참조 | 컬렉션 | 검색 | 액션 | 쿼리 | 작업 |
|---|---|---|---|---|---|---|
| `masterTaskID` |   |   |   |   |   |   |

{style="table-layout:auto"}

DocumentVersion

| 필드 | 참조 | 컬렉션 | 검색 | 액션 | 쿼리 | 작업 |
|---|---|---|---|---|---|---|
| 외부 통합 유형 <sup>1</sup> |   |   |   |   |   |   |
|   |   |   |   |   |   |   |
|   |   |   |   |   |   |   |
|   |   |   |   |   |   |   |

{style="table-layout:auto"}

possibleValues에 대한 <sup>1</sup> 변경 사항

경비

| 필드 | 참조 | 컬렉션 | 검색 | 액션 | 쿼리 | 작업 |
|---|---|---|---|---|---|---|
| `masterTaskID` |   |   |   |   |   |   |

{style="table-layout:auto"}

### 그룹

| 필드 | 참조 | 컬렉션 | 검색 | 액션 | 쿼리 | 작업 |
|---|---|---|---|---|---|---|
|   | licenseTypeLimit |   |   | addRemoveLicenseTypeLimits  |   |   |
|   |   |   |   | setLicenseTypeLimit |   |   |

{style="table-layout:auto"}

### LinkedFolder

| 필드 | 참조 | 컬렉션 | 검색 | 액션 | 쿼리 | 작업 |
|---|---|---|---|---|---|---|
| 외부 통합 유형<sup>1</sup> |  |  |  |  |   |   |

{style="table-layout:auto"}

possibleValues에 대한 <sup>1</sup> 변경 사항

### OpTask

| 필드 | 참조 | 컬렉션 | 검색 | 액션 | 쿼리 | 작업 |
|---|---|---|---|---|---|---|
| priorityColor |   |  | pendingApproval<sup>1</sup> |   |   |   |

{style="table-layout:auto"}

<sup>1</sup> 형식이 null에서 부울로 변경됨

### PortalSection

| 필드 | 참조 | 컬렉션 | 검색 | 액션 | 쿼리 | 작업 |
|---|---|---|---|---|---|---|
|   |  |   | groupIDs |   |   |   |

{style="table-layout:auto"}

### Portfolio

| 필드 | 참조 | 컬렉션 | 검색 | 액션 | 쿼리 | 작업 |
|---|---|---|---|---|---|---|
| portfolioNetValue |   |   |   |  |  |   |
| portfolioRoi |   |   |   |   |   |   |

{style="table-layout:auto"}

### 프로젝트

| 필드 | 참조 | 컬렉션 | 검색 | 액션 | 쿼리 | 작업 |
|---|---|---|---|---|---|---|
| projectBudgetCost  |   |   |   | linkExternalObject  |   |   |
| 프로젝트 순 가치 |   |   |   | 외부 개체 연결 해제 |   |   |
| projectRoi |   |   |   |   |   |   |
| resourcePlannerBudgetedLaborCost |   |   |   |   |   |   |

{style="table-layout:auto"}

### ProofApproval

| 필드 | 참조 | 컬렉션 | 검색 | 액션 | 쿼리 | 작업 |
|---|---|---|---|---|---|---|
| 승인자 결정 |   |   |   |   |   |   |

{style="table-layout:auto"}

### 요금

| 필드 | 참조 | 컬렉션 | 검색 | 액션 | 쿼리 | 작업 |
|---|---|---|---|---|---|---|
| rateValue <sup>1</sup> |  |  |  |  |  |   |

{style="table-layout:auto"}

<sup>1</sup>유효성 검사기 통화 추가됨

### 작업

| 필드 | 참조 | 컬렉션 | 검색 | 액션 | 쿼리 | 작업 |
|---|---|---|---|---|---|---|
| kanbanbflag |   |   |   |   |   |   |
| `masterTaskID` |   |   |   |   |   |   |
| priorityColor  |   |   |   |   |   |   |

{style="table-layout:auto"}

 

### 팀

| 필드 | 참조 | 컬렉션 | 검색 | 액션 | 쿼리 | 작업 |
|---|---|---|---|---|---|---|
| hoursPerPoint <sup></sup> |   |   |   |   |   |   |

{style="table-layout:auto"}

<sup>1</sup> 검사기 LESS_THAN 추가됨

### 팀 할당

| 필드 | 참조 | 컬렉션 | 검색 | 액션 | 쿼리 | 작업 |
|---|---|---|---|---|---|---|
| `masterTaskID` |   |   |   |   |   |   |

{style="table-layout:auto"}

### TeamTask

| 필드 | 참조 | 컬렉션 | 검색 | 액션 | 쿼리 | 작업 |
|---|---|---|---|---|---|---|
| `masterTaskID` |   |   |   |   |   |   |

{style="table-layout:auto"}

### 타임시트

| 필드 | 참조 | 컬렉션 | 검색 | 액션 | 쿼리 | 작업 |
|---|---|---|---|---|---|---|
|   |   |   |   |   |   |   |

{style="table-layout:auto"}

### 업데이트

| 필드 | 참조 | 컬렉션 | 검색 | 액션 | 쿼리 | 작업 |
|---|---|---|---|---|---|---|
| updateType `<sup>1</sup>` |   |   |   |   |   | objectUpdatesWithNoteAndJournalEntryIndex  |

{style="table-layout:auto"}

possibleValues에 대한 <sup>1</sup> 변경 사항

### 사용자

| 필드 | 참조 | 컬렉션 | 검색 | 액션 | 쿼리 | 작업 |
|---|---|---|---|---|---|---|
|   | 액세스 수준  |   |   |   |   |   |

{style="table-layout:auto"}

### UserNote

| 필드 | 참조 | 컬렉션 | 검색 | 액션 | 쿼리 | 작업 |
|---|---|---|---|---|---|---|
| eventType <sup>1</sup> |   |   |   |   |   |   |

{style="table-layout:auto"}

possibleValues에 대한 <sup>1</sup> 변경 사항

### 작업

| 필드 | 참조 | 컬렉션 | 검색 | 액션 | 쿼리 | 작업 |
|---|---|---|---|---|---|---|
| kanbanbflag |  |  | 승인 보류 중 <sup>1</sup>  |   |   |   |
| `masterTaskID` |   |   |   |   |   |   |
| priorityColor  |   |   |   |   |   |   |

{style="table-layout:auto"}

<sup>1</sup> 형식이 null에서 부울로 변경됨

## 제거된 리소스 {#removed-resources}

### 리소스 예산 시간

| 필드 | 참조 | 컬렉션 | 검색 | 액션 | 쿼리 | 작업 |
|---|---|---|---|---|---|---|
| allocationDate |   |   |   |   |   | 추가  |
| budgetHours |   |   |   |   |   | 수  |
| ID |   |   |   |   |   | DELETE  |
| plannedBudgetHours |   |   |   |   |   | 편집  |
| projectID |   |   |   |   |   | GET  |
| roleID |   |   |   |   |   | 보고서  |
| userID |   |   |   |   |   | 검색 |

{style="table-layout:auto"}

 

 

 
