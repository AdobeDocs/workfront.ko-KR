---
content-type: api
navigation-topic: api-navigation-topic
title: API 버전 6의 새로운 기능
description: API 버전 6의 새로운 기능
author: Becky
feature: Workfront API
role: Developer
exl-id: e671a881-b8c2-4234-a3a0-76b1fbfafd32
source-git-commit: 3e339e2bfb26e101f0305c05f620a21541394993
workflow-type: tm+mt
source-wordcount: '495'
ht-degree: 38%

---

# API 버전 6의 새로운 기능

## 새 개체

### 리소스 관리자

| 필드 | 참조 | 컬렉션 | 검색 | 액션 | 쿼리 | 작업 |
|---|---|---|---|---|---|---|
| ID | 고객 |   |   |   |   | 추가 |
| customerID | 프로젝트 |   |   |   |   | 수 |
| projectID | resourceManager |   |   |   |   | 삭제 |
| 리소스 관리자 ID | 템플릿 |   |   |   |   | Get |
| templateID |   |   |   |   |   | 보고서  |
|   |   |   |   |   |   | 검색  |


### Ews

| 필드 | 참조 | 컬렉션 | 검색 | 액션 | 쿼리 | 작업 |
|---|---|---|---|---|---|---|
| fileName |   |   |   |   | 업로드 |   |
| 핸들 |   |   |   |   |   |   |
| objCode |   |   |   |   |   |   |


### 사용자 정의 레이블

| 필드 | 참조 | 컬렉션 | 검색 | 액션 | 쿼리 | 작업 |
|---|---|---|---|---|---|---|
| ID |   |   |   | checkDelete | 사용자 정의 레이블 | 추가 |
|   |   |   |   | inUseByOtherLayoutTemplate | 사용자 정의 레이블 | 수 |
|   |   |   |   | removeCustomLabel |   | 삭제 |
|   |   |   |   |   |   | Get |
|   |   |   |   |   |   | 보고서 |
|   |   |   |   |   |   | 검색 |


## 업데이트된 개체

기존 객체에 대한 변경 사항: 추가는 간단히 나열되고, 제거는 취소선이 있으며, 기존 객체에 대한 변경 사항은 테이블 뒤에 메모가 첨부되어 있습니다

### 업데이트

 

| 필드 | 참조 | 컬렉션 | 검색 | 액션 | 쿼리 | 작업 |
|---|---|---|---|---|---|---|
| updateType<sup>1</sup> |   |   |   |   | `sinceDate` |   |
|   |   |   |   |   | objectUpdatesByCommentID<sup>2</sup> |   |

{style="table-layout:auto"}

<sup>1</sup> 가능한 값 변경

<sup>2</sup> hasFilters 속성이 true로 변경됨

 

### 승인

| 필드 | 참조 | 컬렉션 | 검색 | 액션 | 쿼리 | 작업 |
|---|---|---|---|---|---|---|
| completedHours |   | resourceManager | resourceManagerID |   |   |   |
| constraintDate<sup>1</sup> |   |   |   |   |   |   |
| isOriginalPlannedHoursSet |   |   |   |   |   |   |
| syncBurndownDate |   |   |   |   |   |   |
| 작업 필요<sup>2</sup> |   |   |   |   |   |   |

{style="table-layout:auto"}

<sup>1</sup> 날짜 유효성 검사 추가됨

<sup>2</sup> NOT_FILTERABLE 플래그가 추가됨

 

### 승인 진행

|   | 필드 | 참조 | 컬렉션 | 검색 | 액션 | 쿼리 | 작업 |
|---|---|---|---|---|---|---|---|
|   |  | `attachedApprovalPaths` |   |   |   |   |   |

{style="table-layout:auto"}

 

### 승인 단계

 

| 필드 | 참조 | 컬렉션 | 검색 | 액션 | 쿼리 | 작업 |
|---|---|---|---|---|---|---|
| approvalType<sup>1</sup> |   |   |   |   |   |   |

{style="table-layout:auto"}

<sup>1</sup> 가능한 값 변경

 

### 승인 경로<sup>1</sup>

| 필드 | 참조 | 컬렉션 | 검색 | 액션 | 쿼리 | 작업 |
|---|---|---|---|---|---|---|
| approvedStatus |   |   |   |   |   | 추가 |
| approvedStatusLabel |   |   |   |   |   | 수 |
| 댓글 |   |   |   |   |   | 삭제 |
| 입력자 ID |   |   |   |   |   | 편집 |
| entryDate |   |   |   |   |   | Get |
| 글로벌 경로 ID |   |   |   |   |   | 보고서 |
| isPrivate |   |   |   |   |   | 검색 |
| 마지막 업데이트 날짜 |   |   |   |   |   |   |
| lastUpdateById |   |   |   |   |   |   |
| 이름<sup>2</sup> |   |   |   |   |   |   |

{style="table-layout:auto"}

<sup>1</sup> 보고 가능으로 변경됨

<sup>2</sup> 최대 길이 유효성 검사기가 추가되었습니다.

 

### 작업 서비스 개체

| 필드 | 참조 | 컬렉션 | 검색 | 액션 | 쿼리 | 작업 |
|---|---|---|---|---|---|---|
| constraintDate<sup>1</sup> |   |   |   | getMyWorkCountFiltered |   |   |
| 작업 필요<sup>2</sup> |   |   |   | 작업 항목 상태 레이블  |   |   |

{style="table-layout:auto"}

<sup>1</sup> 날짜 유효성 검사 추가됨

<sup>2</sup> Not_Filterable 플래그가 추가됨

 

### 할당

| 필드 | 참조 | 컬렉션 | 검색 | 액션 | 쿼리 | 작업 |
|---|---|---|---|---|---|---|
|   |   |   |   | assignUserToRoleOnprojects |   |   |
|   |   |   |   | swapUserOnProjects |   |   |
|   |   |   |   | 프로젝트에서 사용자 할당 해제 |   |   |

{style="table-layout:auto"}

 

### 기준선 

| 필드 | 참조 | 컬렉션 | 검색 | 액션 | 쿼리 | 작업 |
|---|---|---|---|---|---|---|
| 작업 필요<sup>1</sup> |   |   |   |   |   |   |

{style="table-layout:auto"}

<sup>1</sup> Not_Filterable 플래그가 추가됨

 

### 기준선 작업

| 필드 | 참조 | 컬렉션 | 검색 | 액션 | 쿼리 | 작업 |
|---|---|---|---|---|---|---|
| 작업 필요<sup>1</sup> |   |   |   |   |   |   |

{style="table-layout:auto"}

<sup>1</sup> Not_Filterable 플래그가 추가됨

 

### 청구 기록

| 필드 | 참조 | 컬렉션 | 검색 | 액션 | 쿼리 | 작업 |
|---|---|---|---|---|---|---|
| billingDate<sup>1</sup> |   |   |   |   |   |   |

{style="table-layout:auto"}

<sup>1</sup> no_TIME 필드 플래그가 추가되었습니다.

### 번다운 이벤트 

| 필드 | 참조 | 컬렉션 | 검색 | 액션 | 쿼리 | 작업 |
|---|---|---|---|---|---|---|
| eventInitiator |   |   |   |   |   | `ADD` |
|   |   |   |   |   |   | `DELETE` |

{style="table-layout:auto"}

 

### 범주 

| 필드 | 참조 | 컬렉션 | 검색 | 액션 | 쿼리 | 작업 |
|---|---|---|---|---|---|---|
|   |   |   |   | getCascadingRules |   |   |
|   |   |   |   | 카테고리 재정렬 |   |   |

{style="table-layout:auto"}

 

사용자 정의 열거형 

| 필드 | 참조 | 컬렉션 | 검색 | 액션 | 쿼리 | 작업 |
|---|---|---|---|---|---|---|
|   |   |   |   | getGroupDefaultProjectStatus | 작업 그룹 상태 |   |
|   |   |   |   | isPossibleToUnlockStatus | projectGroupStatus |   |
|   |   |   |   |   | 작업 그룹 상태 |   |

{style="table-layout:auto"}

 

문서 

| 필드 | 참조 | 컬렉션 | 검색 | 액션 | 쿼리 | 작업 |
|---|---|---|---|---|---|---|
| `checkedOutByID` | `checkedOutBy`  |   |  isDir |   |   |   |
| `isDir`  |   |   |   |   |   |   |

{style="table-layout:auto"}

 

환율 

| 필드 | 참조 | 컬렉션 | 검색 | 액션 | 쿼리 | 작업 |
|---|---|---|---|---|---|---|
| 비율<sup>1</sup> |   |   |   |   |   |   |

{style="table-layout:auto"}

<sup>1</sup> PRECISION 검사기를 8에서 9로 변경했습니다.

 

### 통합

| 필드 | 참조 | 컬렉션 | 검색 | 액션 | 쿼리 | 작업 |
|---|---|---|---|---|---|---|
| syncBurndownDate |   |   |   |   |   |   |

{style="table-layout:auto"}

 

### 저널 항목

| 필드 | 참조 | 컬렉션 | 검색 | 액션 | 쿼리 | 작업 |
|---|---|---|---|---|---|---|
| changeType<sup>1</sup> |   |   |   |   |   |   |

{style="table-layout:auto"}

<sup>1</sup> 가능한 값 변경

 

### Optask(문제)<sup>1</sup> 

| 필드 | 참조 | 컬렉션 | 검색 | 액션 | 쿼리 | 작업 |
|---|---|---|---|---|---|---|
| 작업 필요<sup>2</sup> |   |   |   |   |   |   |

{style="table-layout:auto"}

<sup>1</sup> 복원 가능으로 플래그 지정됨

<sup>2</sup> Not_Filterable 플래그가 추가됨

 

### 프로젝트<sup>1</sup> 

| 필드 | 참조 | 컬렉션 | 검색 | 액션 | 쿼리 | 작업 |
|---|---|---|---|---|---|---|
| completedHours |   | `openOpTasks` |  openOpTasks |   |   |   |
| isOriginalPlannedHoursSet |   | resourceManager | resourceManagerID  |   |   |   |
| originalWorkRequired |   |   | `work` |   |   |   |
| syncBurndownDate |   |   |   |   |   |   |
| 작업 |   |   |   |   |   |   |
| 작업 필요 |   |   |   |   |   |   |

{style="table-layout:auto"}

<sup>1</sup> 복원 가능 및 RESOURCE_MANAGABLE로 플래그가 지정됨

<sup>2</sup> Not_Filterable 플래그가 추가됨

 

### 작업<sup>1</sup>

| 필드 | 참조 | 컬렉션 | 검색 | 액션 | 쿼리 | 작업 |
|---|---|---|---|---|---|---|
| constraintDate<sup>2</sup> |   |   |   |   |   |   |
| 작업 필요<sup>3</sup> |   |   |   |   |   |   |

{style="table-layout:auto"}

<sup>1</sup> 복원 가능으로 플래그 지정됨

<sup>2</sup> AT_DATE_YEAR_BEFORE 유효성 검사기 추가됨

<sup>3</sup> Not_Filterable 플래그가 추가됨

 

### 팀

| 필드 | 참조 | 컬렉션 | 검색 | 액션 | 쿼리 | 작업 |
|---|---|---|---|---|---|---|
| `myWorkViewID` |  `myWorkView` |   |   |   |   |   |
| `requestsViewID`  | `myRequestsView`  |   |   |   |   |   |

{style="table-layout:auto"}

 

### 템플릿<sup>1</sup> 

| 필드 | 참조 | 컬렉션 | 검색 | 액션 | 쿼리 | 작업 |
|---|---|---|---|---|---|---|
|   |   | resourceManager | resourceManagerID |   |   |   |

{style="table-layout:auto"}

<sup>1</sup> 복원 가능 및 RESOURCE_MANAGABLE로 플래그가 지정됨

### 템플릿 작업<sup>1</sup> 

| 필드 | 참조 | 컬렉션 | 검색 | 액션 | 쿼리 | 작업 |
|---|---|---|---|---|---|---|
| 작업 필요<sup>2</sup> |   |   |   |   |   |   |

{style="table-layout:auto"}

<sup>1</sup> 복원 가능으로 플래그 지정됨

<sup>2</sup> Not_Filterable 플래그가 추가됨

 

### 사용자

| 필드 | 참조 | 컬렉션 | 검색 | 액션 | 쿼리 | 작업 |
|---|---|---|---|---|---|---|
| myInfo<sup>1</sup> |   |   |   |   |   |   |

{style="table-layout:auto"}

<sup>1</sup> MAX_LENGTH 위반

 

### 사용자 메모

| 필드 | 참조 | 컬렉션 | 검색 | 액션 | 쿼리 | 작업 |
|---|---|---|---|---|---|---|
| eventType<sup>1</sup> |   |   |   |   | 내 알림<sup>2</sup> |   |

{style="table-layout:auto"}

<sup>1</sup> 가능한 값이 변경됨

<sup>2</sup> 이(가) 다음으로 필터 변경됨: `[true]`

 

### 공지

| 필드 | 참조 | 컬렉션 | 검색 | 액션 | 쿼리 | 작업 |
|---|---|---|---|---|---|---|
|   |   |   |   | `fileHandle` |   |   |
|   |   |   |   | `zipAnnouncementAttachments`  |   |   |
