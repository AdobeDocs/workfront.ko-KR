---
content-type: api
navigation-topic: api-navigation-topic
title: API 버전 9 업데이트
description: 업데이트된 리소스
author: Becky
feature: Workfront API
role: Developer
exl-id: 51892846-d93f-4363-8416-4118fb2ef84d
TQID: https://experienceleague.adobe.com/JAoiJn1kNmwFsYKeuSU67f43wBsgMXCgnMDbcOM-5Kg
product_v2:
  - id: c4a86a5d-6562-4fc6-aa00-bfa25833aed9
role_v2:
  - id: ff6a42d2-313e-452e-93a6-792e4fad9ff8
source-git-commit: 55a9d9feae8cc1128e3427a8874414ba734dd467
workflow-type: tm+mt
source-wordcount: 257
ht-degree: 56%

---

# API 버전 9 업데이트

## 업데이트된 리소스

다음 기존 리소스가 Adobe Workfront API의 이번 릴리스로 업데이트되었습니다. 버전 9의 새로운 리소스를 보려면 [API 버전 9의 새로운 기능](../../wf-api/api/new-api-version-9.md) 및 [API 버전 9의 새로운 기능(계속)](../../wf-api/api/new-api-version-9-continue.md)을 방문하세요. 리소스에 대한 변경 사항은 다음 방법으로 표시됩니다.

* 추가 사항은 간단히 나열되어 있습니다
* 제거는 취소선 텍스트로 표시됩니다
* 변경 사항은 표 뒤에 있는 메모에 명시되어 있습니다

### AgileWork

| 필드 | 참조 | 컬렉션 | 검색 | 액션 | 쿼리 | 작업 |
|---|---|---|---|---|---|---|
| `opTaskID`<sup>2</sup> |  |   |  |   |   |  |
| `taskID`<sup>2</sup> |   |   |  |  |  |  |

{style="table-layout:auto"}

<sup>1</sup> 플래그 제거됨: 보고 가능\
<sup>2</sup> 플래그 제거됨: NOT_GROUPABLE

### 승인

| 필드 | 참조 | 컬렉션 | 검색 | 액션 | 쿼리 | 작업 |
|---|---|---|---|---|---|---|
| `storyBoardOrder` | `agileWork` |   |   |   |   |   |

{style="table-layout:auto"}

할당

| 필드 | 참조 | 컬렉션 | 검색 | 액션 | 쿼리 | 작업 |
|---|---|---|---|---|---|---|
| |   |  |  | `assignUserToRoleOnProjects`<sup>1</sup> |   |   |
|   |   |   |   | `assignUserToRoleOnTasks`<sup>1</sup> |   |   |
|   |   |   |   | `swapUsersOnProjects`<sup>1</sup> |   |   |
|   |   |   |   | `swapUsersOnTasks`<sup>1</sup> |   |   |

{style="table-layout:auto"}

<sup>1</sup> 추가된 필드: lockToRole

### 고객 환경 설정

| 필드 | 참조 | 컬렉션 | 검색 | 액션 | 쿼리 | 작업 |
|---|---|---|---|---|---|---|
| `name`<sup>1</sup> |   |   |   |   |   |   |

{style="table-layout:auto"}

possibleValues에 대한 <sup>1</sup> 변경 사항

### 시간

| 필드 | 참조 | 컬렉션 | 검색 | 액션 | 쿼리 | 작업 |
|---|---|---|---|---|---|---|
| `days` |   |   |   |   |   |   |
| `workHoursPerDay` |   |   |   |   |   |   |

{style="table-layout:auto"}

### 반복

| 필드 | 참조 | 컬렉션 | 검색 | 액션 | 쿼리 | 작업 |
|---|---|---|---|---|---|---|
|   |   |   |   | `moveIssues` |   |   |

{style="table-layout:auto"}

### 레이아웃 템플릿

| 필드 | 참조 | 컬렉션 | 검색 | 액션 | 쿼리 | 작업 |
|---|---|---|---|---|---|---|
| `groupID` | `group` |   |   |   |   |   |

{style="table-layout:auto"}

### 메모

| 필드 | 참조 | 컬렉션 | 검색 | 액션 | 쿼리 | 작업 |
|---|---|---|---|---|---|---|
| `html` |   |   |   |   |   |   |
| `json` |   |   |   |   |   |   |
| `richTextNoteID` |   |   |   |   |   |   |

{style="table-layout:auto"}

### OpTask

| 필드 | 참조 | 컬렉션 | 검색 | 액션 | 쿼리 | 작업 |
|---|---|---|---|---|---|---|
| `color` | `agileWork` |   |   | `convertToProject` |   |   |
| `isReady` |   |   |   | `convertToTask` |   |   |
| `storyBoardOrder` |   |   |   | `linkExternalObject` |   |   |
|   |   |   |   | `unlinkExternalObject` |   |   |

{style="table-layout:auto"}

### 리소스 예산

| 필드 | 참조 | 컬렉션 | 검색 | 액션 | 쿼리 | 작업 |
|---|---|---|---|---|---|---|
| `ID` |   |   |   |   |   |   |

{style="table-layout:auto"}

<sup>1</sup> 플래그 제거됨: 보고 가능

### 예약

| 필드 | 참조 | 컬렉션 | 검색 | 액션 | 쿼리 | 작업 |
|---|---|---|---|---|---|---|
| `homeGroupID` | `homeGroup` |   |   |   |   |   |

{style="table-layout:auto"}

### 작업

| 필드 | 참조 | 컬렉션 | 검색 | 액션 | 쿼리 | 작업 |
|---|---|---|---|---|---|---|
|   | `agileWork` |   |   | `convertToProject` |   |   |
|   |   |   |   | `linkExternalObject` |   |   |
|   |   |   |   | `unlinkExternalObject` |   |   |

{style="table-layout:auto"}

### 팀

| 필드 | 참조 | 컬렉션 | 검색 | 액션 | 쿼리 | 작업 |
|---|---|---|---|---|---|---|
| `includeIssues` |   |   |   |   |   |   |

{style="table-layout:auto"}

### 타임시트 프로필

| 필드 | 참조 | 컬렉션 | 검색 | 액션 | 쿼리 | 작업 |
|---|---|---|---|---|---|---|
| `groupID` | `group` |   |   |   |   |   |

{style="table-layout:auto"}

### UIFilter

| 필드 | 참조 | 컬렉션 | 검색 | 액션 | 쿼리 | 작업 |
|---|---|---|---|---|---|---|
|   |   |   |   |   | `filtersForObjCode` |   |

{style="table-layout:auto"}

### UIView

| 필드 | 참조 | 컬렉션 | 검색 | 액션 | 쿼리 | 작업 |
|---|---|---|---|---|---|---|
|   |   |   |   |   | `viewsForObjCode` |   |

{style="table-layout:auto"}

### 사용자

| 필드 | 참조 | 컬렉션 | 검색 | 액션 | 쿼리 | 작업 |
|---|---|---|---|---|---|---|
| `logTimeInDays` |   |   |   |   |   |   |
| `workHoursPerDay` |   |   |   |   |   |   |

{style="table-layout:auto"}

### 작업

| 필드 | 참조 | 컬렉션 | 검색 | 액션 | 쿼리 | 작업 |
|---|---|---|---|---|---|---|
| `storyBoardOrder` | `agileWork` |   |   | `getWFHomeObjects` |   |   |
