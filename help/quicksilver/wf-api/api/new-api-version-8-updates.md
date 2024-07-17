---
content-type: api
navigation-topic: api-navigation-topic
title: API 버전 8 업데이트
description: API 버전 8에 대한 업데이트를 봅니다.
author: Becky
feature: Workfront API
role: Developer
exl-id: c6d7d2d2-cd21-4ca8-a5a0-afe3669dc959
source-git-commit: ae80999fc7ea7e35097560aa99baa435bcd31b74
workflow-type: tm+mt
source-wordcount: '537'
ht-degree: 31%

---

# API 버전 8 업데이트

## 업데이트된 리소스

다음 기존 리소스가 Adobe Workfront API의 이번 릴리스로 업데이트되었습니다. 버전 8의 새로운 리소스를 보려면 [API 버전 8의 새로운 기능](../../wf-api/api/new-api-version-8.md)을 참조하세요. 리소스에 대한 변경 사항은 다음 방법으로 표시됩니다.

* 추가 사항은 간단히 나열되어 있습니다
* 제거는 취소선 텍스트로 표시됩니다
* 변경 사항은 표 뒤에 있는 메모에 명시되어 있습니다

### AccessRequest

| 필드 | 참조 | 컬렉션 | 검색 | 액션 | 쿼리 | 작업 |
|---|---|---|---|---|---|---|
| 작업<sup>1</sup>  |   |   |   |   |   |   |

{style="table-layout:auto"}

가능한 값에 대한 <sup>1</sup> 변경

### AccessRule<sup>1</sup> 

| 필드 | 참조 | 컬렉션 | 검색 | 액션 | 쿼리 | 작업 |
|---|---|---|---|---|---|---|
| coreAction<sup>2</sup>  |   |   |   |   |   |   |
| forbiddenActions<sup>2</sup> |   |   |   |   |   |   |
| secondaryActions<sup>2</sup> |   |   |   |   |   |   |

{style="table-layout:auto"}

<sup>1</sup> 플래그 제거됨: 보고 가능\
가능한 값에 대한 <sup>2</sup> 변경

### 승인

| 필드 | 참조 | 컬렉션 | 검색 | 액션 | 쿼리 | 작업 |
|---|---|---|---|---|---|---|
| auditTypes<sup>1</sup> | 애자일 작업  | 리소스 풀 |   |   |   |   |
| backlogOrder<sup>2</sup> | kanbanBoard  |   |   |   |   |   |
| 백로그 상위 |   |   |   |   |   |   |
| 칸반 보드 ID |   |   |   |   |   |   |

{style="table-layout:auto"}

<sup>1</sup>가능한 값에 대한 변경 내용\
<sup>2</sup>추가된 플래그: DYNAMIC, LAZY_READ 및 NOT_GROUPABLE

### 할당

|   |   |   |   | 필드 | 참조 | 컬렉션 | 검색 | 액션 | 쿼리 | 작업 |
|---|---|---|---|---|---|---|---|---|---|---|
|   |   |   |   | assignUserToRoleOntasks | getAssignAssignmentsForTasks  |   |   |   |   |   |
|   |   |   |   | swapUserOnTasks | getUnassignAssignmentsForTasks |   |   |   |   |   |
|   |   |   |   | unassignUserFromTasks |   |   |   |   |   |   |

{style="table-layout:auto"}

### 고객

| 필드 | 참조 | 컬렉션 | 검색 | 액션 | 쿼리 | 작업 |
|---|---|---|---|---|---|---|
| bizRuleExclusions<sup>1</sup> |   |   |   | getPackagingOptionValue |   |   |
| proofPlan<sup>1</sup> |   |   |   | isPackagingOptionEnabled |   |   |

{style="table-layout:auto"}

<sup>1</sup>가능한 값에 대한 변경 내용

### 고객 환경 설정

| 필드 | 참조 | 컬렉션 | 검색 | 액션 | 쿼리 | 작업 |
|---|---|---|---|---|---|---|
| 이름<sup>1</sup> |   |   |   |   |   |   |

{style="table-layout:auto"}

<sup>1</sup>가능한 값에 대한 변경 내용

### DocumentApproval

| 필드 | 참조 | 컬렉션 | 검색 | 액션 | 쿼리 | 작업 |
|---|---|---|---|---|---|---|
| ID<sup>1</sup> |   |   |   |   |   |   |

{style="table-layout:auto"}

<sup>1</sup>플래그 추가됨: NOT_FILTERABLE

### DocumentVersion

| 필드 | 참조 | 컬렉션 | 검색 | 액션 | 쿼리 | 작업 |
|---|---|---|---|---|---|---|
| active증명 단계 |   |   |   |   |   |   |

{style="table-layout:auto"}

### 그룹

| 필드 | 참조 | 컬렉션 | 검색 | 액션 | 쿼리 | 작업 |
|---|---|---|---|---|---|---|
|   |   | 소유자 |   |   |   |   |

{style="table-layout:auto"}

### HourType

| 필드 | 참조 | 컬렉션 | 검색 | 액션 | 쿼리 | 작업 |
|---|---|---|---|---|---|---|
| appGlobalID<sup>1</sup> |   |   |   |   |   |   |

{style="table-layout:auto"}

<sup>1</sup>플래그 추가됨: NOT_FILTERABLE

### 반복

| 필드 | 참조 | 컬렉션 | 검색 | 액션 | 쿼리 | 작업 |
|---|---|---|---|---|---|---|
|   |   |   |   | moveStories |   |   |

{style="table-layout:auto"}

### 좋아요

| 필드 | 참조 | 컬렉션 | 검색 | 액션 | 쿼리 | 작업 |
|---|---|---|---|---|---|---|
| `endorsementID` | `endorsement` |   |   |   |   |   |

{style="table-layout:auto"}

### 참고

| 필드 | 참조 | 컬렉션 | 검색 | 액션 | 쿼리 | 작업 |
|---|---|---|---|---|---|---|
| auditType<sup>1</sup> |   |   |   |   |   |   |

{style="table-layout:auto"}

<sup>1</sup>가능한 값에 대한 변경 내용

### OpTask

| 필드 | 참조 | 컬렉션 | 검색 | 액션 | 쿼리 | 작업 |
|---|---|---|---|---|---|---|
| auditTypes<sup>1</sup> | 애자일 작업  |   |   |   | defaultShownTimesheetIssues  |   |
| backlogOrder | 반복 |   |   |   |   |   |
| 백로그 상위 |   |   |   |   |   |   |
| 예상 |   |   |   |   |   |   |
| 반복 ID |   |   |   |   |   |   |

{style="table-layout:auto"}

<sup>1</sup>가능한 값에 대한 변경 내용

### Portfolio

| 필드 | 참조 | 컬렉션 | 검색 | 액션 | 쿼리 | 작업 |
|---|---|---|---|---|---|---|
| auditTypes<sup>1</sup> |   |   |   |   |   |   |

{style="table-layout:auto"}

<sup>1</sup>가능한 값에 대한 변경 내용

### 프로그램

| 필드 | 참조 | 컬렉션 | 검색 | 액션 | 쿼리 | 작업 |
|---|---|---|---|---|---|---|
| auditTypes<sup>1</sup> |   |   |   |   |   |   |

{style="table-layout:auto"}

<sup>1</sup>가능한 값에 대한 변경 내용

### 프로젝트

| 필드 | 참조 | 컬렉션 | 검색 | 액션 | 쿼리 | 작업 |
|---|---|---|---|---|---|---|
| auditTypes<sup>1</sup> |   | 리소스 풀 |   |   | defaultShownTimesheetProjects |   |

{style="table-layout:auto"}

<sup>1</sup>가능한 값에 대한 변경 내용

### ProofApproval

| 필드 | 참조 | 컬렉션 | 검색 | 액션 | 쿼리 | 작업 |
|---|---|---|---|---|---|---|
| approverID | 승인자 |   |   |   |   |   |
| 문서 버전 ID | documentVersion |   |   |   |   |   |
| ID<sup>1</sup> |   |   |   |   |   |   |
| 증명 생성 날짜 |   |   |   |   |   |   |

{style="table-layout:auto"}

<sup>1</sup>플래그 추가됨: NOT_FILTERABLE

### QueueDef

| 필드 | 참조 | 컬렉션 | 검색 | 액션 | 쿼리 | 작업 |
|---|---|---|---|---|---|---|
| requestorCoreAction<sup>1</sup> |   |   |   |   |   |   |
| requestorForbiddenActions<sup>1</sup> |   |   |   |   |   |   |

{style="table-layout:auto"}

<sup>1</sup>가능한 값에 대한 변경 내용

### 요금

| 필드 | 참조 | 컬렉션 | 검색 | 액션 | 쿼리 | 작업 |
|---|---|---|---|---|---|---|
| endDate |   |   |   | setRatesForRole  |   |   |
| 이름 |   |   |   |   |   |   |
| startDate |   |   |   |   |   |   |

{style="table-layout:auto"}

### 예약된 시간

| 필드 | 참조 | 컬렉션 | 검색 | 액션 | 쿼리 | 작업 |
|---|---|---|---|---|---|---|
| extRefID |   |   |   |   |   |   |

{style="table-layout:auto"}

### 리소스 관리자

| 필드 | 참조 | 컬렉션 | 검색 | 액션 | 쿼리 | 작업 |
|---|---|---|---|---|---|---|
| projectPriority |   |   |   |   |   |   |

{style="table-layout:auto"}

### 작업

| 필드 | 참조 | 컬렉션 | 검색 | 액션 | 쿼리 | 작업 |
|---|---|---|---|---|---|---|
| auditTypes<sup>1</sup> | 애자일 작업  |   |   |   | 모든 작업 반복  |   |
| 백로그 상위 | kanbanBoard |   |   |   | defaultShownTimesheetTasks |   |
| 칸반 보드 ID |   |   |   |   |   |   |

{style="table-layout:auto"}

<sup>1</sup>가능한 값에 대한 변경 내용

### 팀

| 필드 | 참조 | 컬렉션 | 검색 | 액션 | 쿼리 | 작업 |
|---|---|---|---|---|---|---|
| 애자일 방법론 |   |   |   |   |   |   |
| autoAdd다음 스토리 |   |   |   |   |   |   |
| includeIssues |   |   |   |   |   |   |
| teamStoryBoardIssueStates |   |   |   |   |   |   |
| wipLimit |   |   |   |   |   |   |

{style="table-layout:auto"}

### 템플릿

| 필드 | 참조 | 컬렉션 | 검색 | 액션 | 쿼리 | 작업 |
|---|---|---|---|---|---|---|
|   |   | 리소스 풀 |   |   |   |   |

{style="table-layout:auto"}

### TemplateTask

| 필드 | 참조 | 컬렉션 | 검색 | 액션 | 쿼리 | 작업 |
|---|---|---|---|---|---|---|
| auditTypes<sup>1</sup> |   |   |   |   |   |   |

{style="table-layout:auto"}

<sup>1</sup>가능한 값에 대한 변경 내용

업데이트

| 필드 | 참조 | 컬렉션 | 검색 | 액션 | 쿼리 | 작업 |
|---|---|---|---|---|---|---|
| updateType<sup>1</sup> | `updateEndorsement` |   |   |   |   |   |

{style="table-layout:auto"}

<sup>1</sup>가능한 값에 대한 변경 내용

### 사용자

|   |   | 필드 | 참조 | 컬렉션 | 검색 | 액션 | 쿼리 | 작업 |
|---|---|---|---|---|---|---|---|---|
|   |   | 리소스 풀 |   |   |   |   |   |   |
|   |   | 사용자 그룹 |   |   |   |   |   |   |
|   |   | userRoles |   |   |   |   |   |   |

{style="table-layout:auto"}

### UserNote

| 필드 | 참조 | 컬렉션 | 검색 | 액션 | 쿼리 | 작업 |
|---|---|---|---|---|---|---|
| `endorsementID` | `endorsement` |   |   |   |   |   |
| `endorsementShareID` | `endorsementShare` |   |   |   |   |   |
| eventType<sup>1</sup> |   |   |   |   |   |   |

{style="table-layout:auto"}

<sup>1</sup>가능한 값에 대한 변경 내용

### 작업

| 필드 | 참조 | 컬렉션 | 검색 | 액션 | 쿼리 | 작업 |
|---|---|---|---|---|---|---|
| auditTypes<sup>1</sup> | 애자일 작업  |   |   |   |   |   |
| backlogOrder<sup>2</sup> | kanbanBoard  |   |   |   |   |   |
| 백로그 상위  |   |   |   |   |   |   |
| 칸반 보드 ID |   |   |   |   |   |   |

{style="table-layout:auto"}

<sup>1</sup>가능한 값에 대한 변경 내용\
<sup>2</sup>추가된 플래그: DYNAMIC, LAZY_READ 및 NOT_GROUPABLE
