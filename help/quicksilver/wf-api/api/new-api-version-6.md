---
content-type: api
navigation-topic: api-navigation-topic
title: API 버전 6의 새로운 기능
description: API 버전 6의 새로운 기능
author: Becky
feature: Workfront API
exl-id: e671a881-b8c2-4234-a3a0-76b1fbfafd32
source-git-commit: f050c8b95145552c9ed67b549608c16115000606
workflow-type: tm+mt
source-wordcount: '570'
ht-degree: 42%

---

# API 버전 6의 새로운 기능

## 새 개체

### 리소스 관리자

| 필드 | 참조 | 컬렉션 | 검색 | 액션 | 쿼리 | 작업 |
|---|---|---|---|---|---|---|
| ID | 고객 |   |   |   |   | 추가 |
| customerID | 프로젝트 |   |   |   |   | 수 |
| projectID | resourceManager |   |   |   |   | 삭제 |
| resourceManagerID | 템플릿 |   |   |   |   | Get |
| templateID |   |   |   |   |   | 보고서  |
|   |   |   |   |   |   | 검색  |


### Ews

| 필드 | 참조 | 컬렉션 | 검색 | 액션 | 쿼리 | 작업 |
|---|---|---|---|---|---|---|
| fileName |   |   |   |   | 업로드 |   |
| 핸들 |   |   |   |   |   |   |
| objCode |   |   |   |   |   |   |


### 사용자 지정 레이블

| 필드 | 참조 | 컬렉션 | 검색 | 액션 | 쿼리 | 작업 |
|---|---|---|---|---|---|---|
| ID |   |   |   | checkDelete | customLabels | 추가 |
|   |   |   |   | inUseByOtherLayoutTemplate | userCustomLabels | 수 |
|   |   |   |   | removeCustomLabel |   | 삭제 |
|   |   |   |   |   |   | Get |
|   |   |   |   |   |   | 보고서 |
|   |   |   |   |   |   | 검색 |


## 업데이트된 개체

기존 객체에 대한 변경 사항: 추가 항목을 간단히 나열하거나, 제거 시 취소가 있고, 기존 변경 사항에 대한 표 뒤에 메모가 첨부되어 있습니다.

### 업데이트

 

| 필드 | 참조 | 컬렉션 | 검색 | 액션 | 쿼리 | 작업 |
|---|---|---|---|---|---|---|
| updateType¹ |   |   |   |   | `sinceDate` |   |
|   |   |   |   |   | objectUpdatesByCommentID² |   |

{style=&quot;table-layout:auto&quot;}

¹ 가능한 값 변경

² hasFilters 속성이 true로 변경됨

 

### 승인

| 필드 | 참조 | 컬렉션 | 검색 | 액션 | 쿼리 | 작업 |
|---|---|---|---|---|---|---|
| completedHours |   | resourceManager | resourceManagerIDs |   |   |   |
| constraintDate¹ |   |   |   |   |   |   |
| isOriginalPlanningHoursSet |   |   |   |   |   |   |
| syncBurndownDate |   |   |   |   |   |   |
| workRequired² |   |   |   |   |   |   |

{style=&quot;table-layout:auto&quot;}

¹ 날짜 유효성 검사 추가

² NOT_FILTERABLE 플래그가 추가되었습니다.

 

### 승인 진행

|   | 필드 | 참조 | 컬렉션 | 검색 | 액션 | 쿼리 | 작업 |
|---|---|---|---|---|---|---|---|
|  |  | `attachedApprovalPaths` |   |   |   |   |   |

{style=&quot;table-layout:auto&quot;}

 

### 승인 단계

 

| 필드 | 참조 | 컬렉션 | 검색 | 액션 | 쿼리 | 작업 |
|---|---|---|---|---|---|---|
| approvalType¹ |   |   |   |   |   |   |

{style=&quot;table-layout:auto&quot;}

¹ 가능한 값 변경

 

### 승인 경로¹

| 필드 | 참조 | 컬렉션 | 검색 | 액션 | 쿼리 | 작업 |
|---|---|---|---|---|---|---|
| approvedStatus |   |   |   |   |   | 추가 |
| approvedStatusLabel |   |   |   |   |   | 수 |
| 개의 주석 |   |   |   |   |   | 삭제 |
| enteredByID |   |   |   |   |   | 편집 |
| entryDate |   |   |   |   |   | Get |
| globalPathID |   |   |   |   |   | 보고서 |
| isPrivate |   |   |   |   |   | 검색 |
| lastUpdateDate |   |   |   |   |   |   |
| lastUpdateByID |   |   |   |   |   |   |
| 이름² |   |   |   |   |   |   |

{style=&quot;table-layout:auto&quot;}

¹ Reporttable로 변경됨

² 최대 길이 유효성 검사기를 추가했습니다.

 

### 작업 서비스 개체

| 필드 | 참조 | 컬렉션 | 검색 | 액션 | 쿼리 | 작업 |
|---|---|---|---|---|---|---|
| constraintDate¹ |   |   |   | getMyWorkCountFiltered |   |   |
| workRequired² |   |   |   | workItemStatusLabels  |   |   |

{style=&quot;table-layout:auto&quot;}

¹ 추가된 날짜 유효성 검사

² Not_Filterable 플래그가 추가됨

 

### 할당

| 필드 | 참조 | 컬렉션 | 검색 | 액션 | 쿼리 | 작업 |
|---|---|---|---|---|---|---|
|   |   |   |   | assignUserToRoleOnProjects |   |   |
|   |   |   |   | swapUsersOnProjects |   |   |
|   |   |   |   | unassignUserFromProjects |   |   |

{style=&quot;table-layout:auto&quot;}

 

### 기준선 

| 필드 | 참조 | 컬렉션 | 검색 | 액션 | 쿼리 | 작업 |
|---|---|---|---|---|---|---|
| workRequired¹ |   |   |   |   |   |   |

{style=&quot;table-layout:auto&quot;}

¹ Not_Filterable 플래그가 추가됨

 

### 기준선 작업

| 필드 | 참조 | 컬렉션 | 검색 | 액션 | 쿼리 | 작업 |
|---|---|---|---|---|---|---|
| workRequired¹ |   |   |   |   |   |   |

{style=&quot;table-layout:auto&quot;}

¹ Not_Filterable 플래그가 추가됨

 

### 청구 기록

| 필드 | 참조 | 컬렉션 | 검색 | 액션 | 쿼리 | 작업 |
|---|---|---|---|---|---|---|
| billingDate¹ |   |   |   |   |   |   |

{style=&quot;table-layout:auto&quot;}

¹ NO_TIME 필드 플래그가 추가되었습니다.

### 번다운 이벤트 

| 필드 | 참조 | 컬렉션 | 검색 | 액션 | 쿼리 | 작업 |
|---|---|---|---|---|---|---|
| eventInitiator |   |   |   |   |   | `ADD` |
|   |   |   |   |   |   | `DELETE` |

{style=&quot;table-layout:auto&quot;}

 

### 범주 

| 필드 | 참조 | 컬렉션 | 검색 | 액션 | 쿼리 | 작업 |
|---|---|---|---|---|---|---|
|   |   |   |   | getCascadingRules |   |   |
|   |   |   |   | reorderCategories |   |   |

{style=&quot;table-layout:auto&quot;}

 

사용자 정의 열거형 

| 필드 | 참조 | 컬렉션 | 검색 | 액션 | 쿼리 | 작업 |
|---|---|---|---|---|---|---|
|   |   |   |   | getGroupDefaultProjectStatus | opTaskGroupStatus |   |
|   |   |   |   | isPossibleToUnlockStatus | projectGroupStatus |   |
|   |   |   |   |   | taskGroupStatus |   |

{style=&quot;table-layout:auto&quot;}

 

문서 

| 필드 | 참조 | 컬렉션 | 검색 | 액션 | 쿼리 | 작업 |
|---|---|---|---|---|---|---|
| `checkedOutByID` | `checkedOutBy`  |   |  isDir |   |   |   |
| `isDir`  |   |   |   |   |   |   |

{style=&quot;table-layout:auto&quot;}

 

환율 

| 필드 | 참조 | 컬렉션 | 검색 | 액션 | 쿼리 | 작업 |
|---|---|---|---|---|---|---|
| rate¹ |   |   |   |   |   |   |

{style=&quot;table-layout:auto&quot;}

¹ 8용 PRECISION 유효성 검사기를 9로 변경했습니다.

 

### 통합

| 필드 | 참조 | 컬렉션 | 검색 | 액션 | 쿼리 | 작업 |
|---|---|---|---|---|---|---|
| syncBurndownDate |   |   |   |   |   |   |

{style=&quot;table-layout:auto&quot;}

 

### 저널 항목

| 필드 | 참조 | 컬렉션 | 검색 | 액션 | 쿼리 | 작업 |
|---|---|---|---|---|---|---|
| changeType¹ |   |   |   |   |   |   |

{style=&quot;table-layout:auto&quot;}

¹ 가능한 값 변경

 

### Optask(문제)¹ 

| 필드 | 참조 | 컬렉션 | 검색 | 액션 | 쿼리 | 작업 |
|---|---|---|---|---|---|---|
| workRequired² |   |   |   |   |   |   |

{style=&quot;table-layout:auto&quot;}

¹ 복원 가능 플래그가 지정됨

² Not_Filterable 플래그가 추가됨

 

### 프로젝트¹ 

| 필드 | 참조 | 컬렉션 | 검색 | 액션 | 쿼리 | 작업 |
|---|---|---|---|---|---|---|
| completedHours |   | `openOpTasks` |  openOpTasks |   |   |   |
| isOriginalPlanningHoursSet |   | resourceManager | resourceManagerIDs  |   |   |   |
| originalWorkRequired |   |   | `work` |   |   |   |
| syncBurndownDate |   |   |   |   |   |   |
| 작업 |   |   |   |   |   |   |
| workRequired |   |   |   |   |   |   |

{style=&quot;table-layout:auto&quot;}

¹ 복원 가능 및 자원 관리 가능

² Not_Filterable 플래그가 추가됨

 

### 작업¹

| 필드 | 참조 | 컬렉션 | 검색 | 액션 | 쿼리 | 작업 |
|---|---|---|---|---|---|---|
| constraintDate² |   |   |   |   |   |   |
| workRequired³ |   |   |   |   |   |   |

{style=&quot;table-layout:auto&quot;}

¹ 복원 가능 플래그가 지정됨

² AT_DATE_YEAR_BEFORE 유효성 검사기가 추가되었습니다.

³ Not_Filterable 플래그가 추가됨

 

### 팀

| 필드 | 참조 | 컬렉션 | 검색 | 액션 | 쿼리 | 작업 |
|---|---|---|---|---|---|---|
| `myWorkViewID` |  `myWorkView` |   |   |   |   |   |
| `requestsViewID`  | `myRequestsView`  |   |   |   |   |   |

{style=&quot;table-layout:auto&quot;}

 

### 템플릿¹ 

| 필드 | 참조 | 컬렉션 | 검색 | 액션 | 쿼리 | 작업 |
|---|---|---|---|---|---|---|
|   |   | resourceManager | resourceManagerIDs |   |   |   |

{style=&quot;table-layout:auto&quot;}

¹ 복원 가능 및 자원 관리 가능

### 템플릿 작업¹ 

| 필드 | 참조 | 컬렉션 | 검색 | 액션 | 쿼리 | 작업 |
|---|---|---|---|---|---|---|
| workRequired² |   |   |   |   |   |   |

{style=&quot;table-layout:auto&quot;}

¹ 복원 가능 플래그가 지정됨

² Not_Filterable 플래그가 추가됨

 

### 사용자

| 필드 | 참조 | 컬렉션 | 검색 | 액션 | 쿼리 | 작업 |
|---|---|---|---|---|---|---|
| myInfo¹ |   |   |   |   |   |   |

{style=&quot;table-layout:auto&quot;}

¹ MAX_LENGTH 위반자

 

### 사용자 참고

| 필드 | 참조 | 컬렉션 | 검색 | 액션 | 쿼리 | 작업 |
|---|---|---|---|---|---|---|
| eventType¹ |   |   |   |   | myNotifications² |   |

{style=&quot;table-layout:auto&quot;}

¹ 가능한 값이 변경됨

²에 필터가 `[true]`

 

### 공지

| 필드 | 참조 | 컬렉션 | 검색 | 액션 | 쿼리 | 작업 |
|---|---|---|---|---|---|---|
|   |   |   |   | `fileHandle` |   |   |
|   |   |   |   | `zipAnnouncementAttachments`  |   |   |
