---
content-type: api
navigation-topic: api-navigation-topic
title: API 버전 8 업데이트
description: 다음 기존 리소스가 이 Adobe Workfront API 릴리스로 업데이트되었습니다. 버전 8의 새로운 리소스를 보려면 API 버전 8의 새로운 기능 을 참조하십시오. 리소스에 대한 변경 사항은 다음 방법으로 표시됩니다. EDIT ME.
author: John
feature: Workfront API
exl-id: c6d7d2d2-cd21-4ca8-a5a0-afe3669dc959
source-git-commit: f2f825280204b56d2dc85efc7a315a4377e551c7
workflow-type: tm+mt
source-wordcount: '619'
ht-degree: 37%

---

# API 버전 8 업데이트

## 업데이트된 리소스

다음 기존 리소스가 이 Adobe Workfront API 릴리스로 업데이트되었습니다. 버전 8의 새로운 리소스를 보려면 [API 버전 8의 새로운 기능](../../wf-api/api/new-api-version-8.md). 리소스에 대한 변경 사항은 다음과 같은 방식으로 표시됩니다.

* 추가는 단순히 나열됨
* 제거는 취소선 텍스트로 표시됩니다
* 변경 사항은 표 뒤에 메모에 기록됩니다

### AccessRequest

| 필드 | 참조 | 컬렉션 | 검색 | 액션 | 쿼리 | 작업 |
|---|---|---|---|---|---|---|
| action¹  |   |   |   |   |   |   |

{style=&quot;table-layout:auto&quot;}

¹ 가능한 값 변경

### AccessRule¹ 

| 필드 | 참조 | 컬렉션 | 검색 | 액션 | 쿼리 | 작업 |
|---|---|---|---|---|---|---|
| coreAction²  |   |   |   |   |   |   |
| forbiddenActions² |   |   |   |   |   |   |
| secondaryActions² |   |   |   |   |   |   |

{style=&quot;table-layout:auto&quot;}

¹ 플래그가 제거됨: REPORTTABLE\
² 가능한 값 변경

### 승인

| 필드 | 참조 | 컬렉션 | 검색 | 액션 | 쿼리 | 작업 |
|---|---|---|---|---|---|---|
| auditTypes¹ | agileWork  | resourcePools |   |   |   |   |
| backlogOrder² | 간판  |   |   |   |   |   |
| backlogParent |   |   |   |   |   |   |
| 간판ID |   |   |   |   |   |   |

{style=&quot;table-layout:auto&quot;}

¹가능한 값에 대한 변경 사항\
²추가된 플래그: DYNAMIC, LAZY_READ 및 NOT_GROUPABLE

### 할당

|   |   |   |   | 필드 | 참조 | 컬렉션 | 검색 | 액션 | 쿼리 | 작업 |
|---|---|---|---|---|---|---|---|---|---|---|
|   |   |   |   | assignUserToRoleOnTasks | getAssignAssignmentsForTasks  |   |   |   |   |   |
|   |   |   |   | swapUsersOnTasks | getUnassignmentForTasks |   |   |   |   |   |
|   |   |   |   | unassignUserFromTasks |   |   |   |   |   |   |

{style=&quot;table-layout:auto&quot;}

### 고객

| 필드 | 참조 | 컬렉션 | 검색 | 액션 | 쿼리 | 작업 |
|---|---|---|---|---|---|---|
| bizRuleExclusions¹ |   |   |   | getPackagingOptionValue |   |   |
| proofPlan¹ |   |   |   | isPackagingOptionEnabled |   |   |

{style=&quot;table-layout:auto&quot;}

¹가능한 값에 대한 변경 사항

### 고객 기본 설정

| 필드 | 참조 | 컬렉션 | 검색 | 액션 | 쿼리 | 작업 |
|---|---|---|---|---|---|---|
| 이름¹ |   |   |   |   |   |   |

{style=&quot;table-layout:auto&quot;}

¹가능한 값에 대한 변경 사항

### DocumentApproval

| 필드 | 참조 | 컬렉션 | 검색 | 액션 | 쿼리 | 작업 |
|---|---|---|---|---|---|---|
| ID¹ |   |   |   |   |   |   |

{style=&quot;table-layout:auto&quot;}

¹추가된 플래그: NOT_FILTERABLE

### DocumentVersion

| 필드 | 참조 | 컬렉션 | 검색 | 액션 | 쿼리 | 작업 |
|---|---|---|---|---|---|---|
| activeProofStage |   |   |   |   |   |   |

{style=&quot;table-layout:auto&quot;}

### 그룹

| 필드 | 참조 | 컬렉션 | 검색 | 액션 | 쿼리 | 작업 |
|---|---|---|---|---|---|---|
|   |   | 소유자 |   |   |   |   |

{style=&quot;table-layout:auto&quot;}

### HourType

| 필드 | 참조 | 컬렉션 | 검색 | 액션 | 쿼리 | 작업 |
|---|---|---|---|---|---|---|
| appGlobalID¹ |   |   |   |   |   |   |

{style=&quot;table-layout:auto&quot;}

¹추가된 플래그: NOT_FILTERABLE

### 반복

| 필드 | 참조 | 컬렉션 | 검색 | 액션 | 쿼리 | 작업 |
|---|---|---|---|---|---|---|
|   |   |   |   | moveStories |   |   |

{style=&quot;table-layout:auto&quot;}

### 좋아요

| 필드 | 참조 | 컬렉션 | 검색 | 액션 | 쿼리 | 작업 |
|---|---|---|---|---|---|---|
| `endorsementID` | `endorsement` |   |   |   |   |   |

{style=&quot;table-layout:auto&quot;}

### 참고

| 필드 | 참조 | 컬렉션 | 검색 | 액션 | 쿼리 | 작업 |
|---|---|---|---|---|---|---|
| auditType¹ |   |   |   |   |   |   |

{style=&quot;table-layout:auto&quot;}

¹가능한 값에 대한 변경 사항

### OpTask

| 필드 | 참조 | 컬렉션 | 검색 | 액션 | 쿼리 | 작업 |
|---|---|---|---|---|---|---|
| auditTypes¹ | agileWork  |   |   |   | default표시된 작업표Issues  |   |
| backlogOrder | 반복 |   |   |   |   |   |
| backlogParent |   |   |   |   |   |   |
| 예상 |   |   |   |   |   |   |
| iterationID |   |   |   |   |   |   |

{style=&quot;table-layout:auto&quot;}

¹가능한 값에 대한 변경 사항

### 포트폴리오

| 필드 | 참조 | 컬렉션 | 검색 | 액션 | 쿼리 | 작업 |
|---|---|---|---|---|---|---|
| auditTypes¹ |   |   |   |   |   |   |

{style=&quot;table-layout:auto&quot;}

¹가능한 값에 대한 변경 사항

### 프로그램

| 필드 | 참조 | 컬렉션 | 검색 | 액션 | 쿼리 | 작업 |
|---|---|---|---|---|---|---|
| auditTypes¹ |   |   |   |   |   |   |

{style=&quot;table-layout:auto&quot;}

¹가능한 값에 대한 변경 사항

### 프로젝트

| 필드 | 참조 | 컬렉션 | 검색 | 액션 | 쿼리 | 작업 |
|---|---|---|---|---|---|---|
| auditTypes¹ |   | resourcePools |   |   | defaultShowTimesetProjects |   |

{style=&quot;table-layout:auto&quot;}

¹가능한 값에 대한 변경 사항

### 증명 승인

| 필드 | 참조 | 컬렉션 | 검색 | 액션 | 쿼리 | 작업 |
|---|---|---|---|---|---|---|
| 승인자 ID | 승인자 |   |   |   |   |   |
| documentVersionID | documentVersion |   |   |   |   |   |
| ID¹ |   |   |   |   |   |   |
| proofCreationDate |   |   |   |   |   |   |

{style=&quot;table-layout:auto&quot;}

¹추가된 플래그: NOT_FILTERABLE

### QueueDef

| 필드 | 참조 | 컬렉션 | 검색 | 액션 | 쿼리 | 작업 |
|---|---|---|---|---|---|---|
| requestorCoreAction¹ |   |   |   |   |   |   |
| requestorForbiddenActions¹ |   |   |   |   |   |   |

{style=&quot;table-layout:auto&quot;}

¹가능한 값에 대한 변경 사항

### 요금

| 필드 | 참조 | 컬렉션 | 검색 | 액션 | 쿼리 | 작업 |
|---|---|---|---|---|---|---|
| endDate |   |   |   | setRatesForRole  |   |   |
| 이름 |   |   |   |   |   |   |
| startDate |   |   |   |   |   |   |

{style=&quot;table-layout:auto&quot;}

### ReservedTime

| 필드 | 참조 | 컬렉션 | 검색 | 액션 | 쿼리 | 작업 |
|---|---|---|---|---|---|---|
| extRefID |   |   |   |   |   |   |

{style=&quot;table-layout:auto&quot;}

### 리소스 관리자

| 필드 | 참조 | 컬렉션 | 검색 | 액션 | 쿼리 | 작업 |
|---|---|---|---|---|---|---|
| projectPriority |   |   |   |   |   |   |

{style=&quot;table-layout:auto&quot;}

### 작업

| 필드 | 참조 | 컬렉션 | 검색 | 액션 | 쿼리 | 작업 |
|---|---|---|---|---|---|---|
| auditTypes¹ | agileWork  |   |   |   | allTasksOnIterations  |   |
| backlogParent | 간판 |   |   |   | defaultShowTimesetTasks |   |
| 간판ID |   |   |   |   |   |   |

{style=&quot;table-layout:auto&quot;}

¹가능한 값에 대한 변경 사항

### 팀

| 필드 | 참조 | 컬렉션 | 검색 | 액션 | 쿼리 | 작업 |
|---|---|---|---|---|---|---|
| agileMethodology |   |   |   |   |   |   |
| autoAddNextStory |   |   |   |   |   |   |
| includeIssues |   |   |   |   |   |   |
| teamStoryBoardIssueStatus |   |   |   |   |   |   |
| wipLimit |   |   |   |   |   |   |

{style=&quot;table-layout:auto&quot;}

### 템플릿

| 필드 | 참조 | 컬렉션 | 검색 | 액션 | 쿼리 | 작업 |
|---|---|---|---|---|---|---|
|   |   | resourcePools |   |   |   |   |

{style=&quot;table-layout:auto&quot;}

### TemplateTask

| 필드 | 참조 | 컬렉션 | 검색 | 액션 | 쿼리 | 작업 |
|---|---|---|---|---|---|---|
| auditTypes¹ |   |   |   |   |   |   |

{style=&quot;table-layout:auto&quot;}

¹가능한 값에 대한 변경 사항

업데이트

| 필드 | 참조 | 컬렉션 | 검색 | 액션 | 쿼리 | 작업 |
|---|---|---|---|---|---|---|
| updateType¹ | `updateEndorsement` |   |   |   |   |   |

{style=&quot;table-layout:auto&quot;}

¹가능한 값에 대한 변경 사항

### 사용자

|   |   | 필드 | 참조 | 컬렉션 | 검색 | 액션 | 쿼리 | 작업 |
|---|---|---|---|---|---|---|---|---|
|   |   | resourcePools |   |   |   |   |   |   |
|   |   | userGroups |   |   |   |   |   |   |
|   |   | userRoles |   |   |   |   |   |   |

{style=&quot;table-layout:auto&quot;}

### UserNote

| 필드 | 참조 | 컬렉션 | 검색 | 액션 | 쿼리 | 작업 |
|---|---|---|---|---|---|---|
| `endorsementID` | `endorsement` |   |   |   |   |   |
| `endorsementShareID` | `endorsementShare` |   |   |   |   |   |
| eventType¹ |   |   |   |   |   |   |

{style=&quot;table-layout:auto&quot;}

¹가능한 값에 대한 변경 사항

### 작업

| 필드 | 참조 | 컬렉션 | 검색 | 액션 | 쿼리 | 작업 |
|---|---|---|---|---|---|---|
| auditTypes¹ | agileWork  |   |   |   |   |   |
| backlogOrder² | 간판  |   |   |   |   |   |
| backlogParent  |   |   |   |   |   |   |
| 간판ID |   |   |   |   |   |   |

{style=&quot;table-layout:auto&quot;}

¹가능한 값에 대한 변경 사항\
²추가된 플래그: DYNAMIC, LAZY_READ 및 NOT_GROUPABLE
