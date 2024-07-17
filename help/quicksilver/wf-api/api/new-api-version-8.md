---
content-type: api
navigation-topic: api-navigation-topic
title: API 버전 8의 새로운 기능
description: API 버전 9를 처음 사용하는 리소스 목록입니다. 버전 8의 리소스에 대한 업데이트 목록은 API 버전 8 업데이트 를 참조하십시오.
author: Becky
feature: Workfront API
role: Developer
exl-id: 90fefaa6-d387-4cdb-8aea-9a939fe2ac26
source-git-commit: 3e339e2bfb26e101f0305c05f620a21541394993
workflow-type: tm+mt
source-wordcount: '269'
ht-degree: 27%

---

# API 버전 8의 새로운 기능

## 새 리소스

API 버전 9를 처음 사용하는 리소스 목록입니다. 버전 8의 리소스에 대한 업데이트 목록을 보려면 [API 버전 8에 대한 업데이트](../../wf-api/api/new-api-version-8-updates.md)를 방문하십시오.

**AgileWork**

| 필드 | 참조 | 컬렉션 | 검색 | 액션 | 쿼리 | 작업 |
|---|---|---|---|---|---|---|
| backlogOrder | 고객 |   |   | bulkCopy  |   | 복사 |
| 색상 | 반복  |   |   |   |   | 수 |
| customerID | lastUpdatedBy |   |   |   |   | DELETE |
| 예상 | opTask |   |   |   |   | 편집 |
| ID | 프로젝트 |   |   |   |   | GET  |
| isReady | 스토리보드상위 |   |   |   |   | 보고서 |
| 반복 ID | 작업 |   |   |   |   | 검색 |
| 마지막 업데이트 날짜 | 팀 |   |   |   |   |   |
| lastUpdatedByID |   |   |   |   |   |   |
| 이름 |   |   |   |   |   |   |
| opTaskId |   |   |   |   |   |   |
| parentStoryBoardOrder |   |   |   |   |   |   |
| projectID |   |   |   |   |   |   |
| storyBoardOrder |   |   |   |   |   |   |
| storyBoardParentID |   |   |   |   |   |   |
| taskID  |   |   |   |   |   |   |
| teamID |   |   |   |   |   |   |
| 유형 |   |   |   |   |   |   |
| uiObjCode |   |   |   |   |   |   |
| uiObjectID |   |   |   |   |   |   |

{style="table-layout:auto"}

### APIVersionMetadata

| 필드 | 참조 | 컬렉션 | 검색 | 액션 | 쿼리 | 작업 |
|---|---|---|---|---|---|---|
| deprecationRelease |   |   |   |   |   | 수  |
| removalRelease |   |   |   |   |   | GET |
| versionName |   |   |   |   |   | 보고서 |
|   |   |   |   |   |   | 검색 |

{style="table-layout:auto"}

**KanbanBoard**

| 필드 | 참조 | 컬렉션 | 검색 | 액션 | 쿼리 | 작업 |
|---|---|---|---|---|---|---|
| ID |   |   |   |   |   | 추가 |
| 이름 |   |   |   |   |   | 수 |
|   |   |   |   |   |   | DELETE |
|   |   |   |   |   |   | 편집 |
|   |   |   |   |   |   | GET |
|   |   |   |   |   |   | 보고서 |
|   |   |   |   |   |   | 검색 |

{style="table-layout:auto"}

### ProofApprovalStatus

| 필드 | 참조 | 컬렉션 | 검색 | 액션 | 쿼리 | 작업 |
|---|---|---|---|---|---|---|
| ID |   |   |   |   |   |   |
| proofApprovalStatusID |   |   |   |   |   |   |
| proofApprovalStatusLabel |   |   |   |   |   |   |

{style="table-layout:auto"}

**ProofFileMeta**

| 필드 | 참조 | 컬렉션 | 검색 | 액션 | 쿼리 | 작업 |
|---|---|---|---|---|---|---|
| 문서 버전 ID | documentVersion |   |   |   |   |   |
| fileIndex |   |   |   |   |   |   |
| fileName |   |   |   |   |   |   |
| ID |   |   |   |   |   |   |
| isURL |   |   |   |   |   |   |

{style="table-layout:auto"}

**리소스 예산 시간**

| 필드 | 참조 | 컬렉션 | 검색 | 액션 | 쿼리 | 작업 |
|---|---|---|---|---|---|---|
| allocationDate |   |   |   |   |   | 추가 |
| budgetHours |   |   |   |   |   | 수 |
| plannedBudgetHours |   |   |   |   |   | DELETE |
| projectID |   |   |   |   |   | 편집 |
| roleID |   |   |   |   |   | GET |
| userID |   |   |   |   |   | 보고서 |
|   |   |   |   |   |   | 검색 |

{style="table-layout:auto"}

### 리소스 플래너 필터

| 필드 | 참조 | 컬렉션 | 검색 | 액션 | 쿼리 | 작업 |
|---|---|---|---|---|---|---|
| ID |   |   |   |   |   | 추가 |
| 이름 |   |   |   |   |   | 수 |
|   |   |   |   |   |   | DELETE |
|   |   |   |   |   |   | 편집 |
|   |   |   |   |   |   | GET |
|   |   |   |   |   |   | 보고서 |
|   |   |   |   |   |   | 검색 |

{style="table-layout:auto"}

**RichTextNote**

| 필드 | 참조 | 컬렉션 | 검색 | 액션 | 쿼리 | 작업 |
|---|---|---|---|---|---|---|
| ID |   |   |   |   |   | 수 |
|   |   |   |   |   |   | GET |
|   |   |   |   |   |   | 보고서 |
|   |   |   |   |   |   | 검색 |

{style="table-layout:auto"}

### 구독

| 필드 | 참조 | 컬렉션 | 검색 | 액션 | 쿼리 | 작업 |
|---|---|---|---|---|---|---|
|  ID |   |   |   | addSubscribers | 구독자 | 추가 |
|   |   |   |   | removeSubscribers |   | 수  |
|   |   |   |   | 구독 |   | DELETE |
|   |   |   |   | 구독 취소 |   | GET |
|   |   |   |   |   |   | 보고서 |
|   |   |   |   |   |   | 검색 |

{style="table-layout:auto"}

### 사용자 역할

| 필드 | 참조 | 컬렉션 | 검색 | 액션 | 쿼리 | 작업 |
|---|---|---|---|---|---|---|
| roleID | 역할 |   |   |   |   |   |
| timePercent | 사용자 |   |   |   |   |   |
| userID |   |   |   |   |   |   |
