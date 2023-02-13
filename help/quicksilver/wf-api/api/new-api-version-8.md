---
content-type: api
navigation-topic: api-navigation-topic
title: API 버전 8의 새로운 기능
description: API 버전 9를 처음 사용하는 리소스 목록입니다. 버전 8 리소스에 대한 업데이트 목록을 보려면 API 버전 8 업데이트 를 참조하십시오.
author: John
feature: Workfront API
exl-id: 90fefaa6-d387-4cdb-8aea-9a939fe2ac26
source-git-commit: f2f825280204b56d2dc85efc7a315a4377e551c7
workflow-type: tm+mt
source-wordcount: '288'
ht-degree: 31%

---

# API 버전 8의 새로운 기능

## 새 리소스

API 버전 9를 처음 사용하는 리소스 목록입니다. 버전 8 리소스에 대한 업데이트 목록을 보려면 을 참조하십시오. [API 버전 8 업데이트](../../wf-api/api/new-api-version-8-updates.md)

**AgileWork**

| 필드 | 참조 | 컬렉션 | 검색 | 액션 | 쿼리 | 작업 |
|---|---|---|---|---|---|---|
| backlogOrder | 고객 |   |   | bulkCopy  |   | 복사 |
| 색상 | 반복  |   |   |   |   | 카운트 |
| customerID | lastUpdatedBy |   |   |   |   | DELETE |
| 예상 | opTask |   |   |   |   | 편집 |
| ID | 프로젝트 |   |   |   |   | GET  |
| isReady | storyboardParent |   |   |   |   | 보고서 |
| iterationID | 작업 |   |   |   |   | 검색 |
| lastUpdateDate | 팀 |   |   |   |   |   |
| lastUpdatedByID |   |   |   |   |   |   |
| 이름 |   |   |   |   |   |   |
| opTaskID |   |   |   |   |   |   |
| parentStoryBoardOrder |   |   |   |   |   |   |
| projectID |   |   |   |   |   |   |
| storyBoardOrder |   |   |   |   |   |   |
| storyBoardParentID |   |   |   |   |   |   |
| taskID  |   |   |   |   |   |   |
| teamID |   |   |   |   |   |   |
| 유형 |   |   |   |   |   |   |
| uiObjCode |   |   |   |   |   |   |
| uiObjectID |   |   |   |   |   |   |

{style=&quot;table-layout:auto&quot;}

### APIVersionMetadata

| 필드 | 참조 | 컬렉션 | 검색 | 액션 | 쿼리 | 작업 |
|---|---|---|---|---|---|---|
| deprecationRelease |   |   |   |   |   | 카운트  |
| removalRelease |   |   |   |   |   | GET |
| versionName |   |   |   |   |   | 보고서 |
|   |   |   |   |   |   | 검색 |

{style=&quot;table-layout:auto&quot;}

**간판 보드**

| 필드 | 참조 | 컬렉션 | 검색 | 액션 | 쿼리 | 작업 |
|---|---|---|---|---|---|---|
| ID |   |   |   |   |   | 추가 |
| 이름 |   |   |   |   |   | 카운트 |
|   |   |   |   |   |   | DELETE |
|   |   |   |   |   |   | 편집 |
|   |   |   |   |   |   | GET |
|   |   |   |   |   |   | 보고서 |
|   |   |   |   |   |   | 검색 |

{style=&quot;table-layout:auto&quot;}

### 증명 승인 상태

| 필드 | 참조 | 컬렉션 | 검색 | 액션 | 쿼리 | 작업 |
|---|---|---|---|---|---|---|
| ID |   |   |   |   |   |   |
| proofApprovalStatusID |   |   |   |   |   |   |
| proofApprovalStatusLabel |   |   |   |   |   |   |

{style=&quot;table-layout:auto&quot;}

**ProofFileMetadata**

| 필드 | 참조 | 컬렉션 | 검색 | 액션 | 쿼리 | 작업 |
|---|---|---|---|---|---|---|
| documentVersionID | documentVersion |   |   |   |   |   |
| fileIndex |   |   |   |   |   |   |
| fileName |   |   |   |   |   |   |
| ID |   |   |   |   |   |   |
| isURL |   |   |   |   |   |   |

{style=&quot;table-layout:auto&quot;}

**자원_예산책정된_시간**

| 필드 | 참조 | 컬렉션 | 검색 | 액션 | 쿼리 | 작업 |
|---|---|---|---|---|---|---|
| allocationDate |   |   |   |   |   | 추가 |
| backgroundHours |   |   |   |   |   | 카운트 |
| planningScheduledHours |   |   |   |   |   | DELETE |
| projectID |   |   |   |   |   | 편집 |
| roleID |   |   |   |   |   | GET |
| userID |   |   |   |   |   | 보고서 |
|   |   |   |   |   |   | 검색 |

{style=&quot;table-layout:auto&quot;}

### 리소스 플래너필터

| 필드 | 참조 | 컬렉션 | 검색 | 액션 | 쿼리 | 작업 |
|---|---|---|---|---|---|---|
| ID |   |   |   |   |   | 추가 |
| 이름 |   |   |   |   |   | 카운트 |
|   |   |   |   |   |   | DELETE |
|   |   |   |   |   |   | 편집 |
|   |   |   |   |   |   | GET |
|   |   |   |   |   |   | 보고서 |
|   |   |   |   |   |   | 검색 |

{style=&quot;table-layout:auto&quot;}

**RichTextNote**

| 필드 | 참조 | 컬렉션 | 검색 | 액션 | 쿼리 | 작업 |
|---|---|---|---|---|---|---|
| ID |   |   |   |   |   | 카운트 |
|   |   |   |   |   |   | GET |
|   |   |   |   |   |   | 보고서 |
|   |   |   |   |   |   | 검색 |

{style=&quot;table-layout:auto&quot;}

### 구독

| 필드 | 참조 | 컬렉션 | 검색 | 액션 | 쿼리 | 작업 |
|---|---|---|---|---|---|---|
|  ID |   |   |   | addSubscribers | 가입자 | 추가 |
|   |   |   |   | removeSubscribers |   | 카운트  |
|   |   |   |   | 가입 |   | DELETE |
|   |   |   |   | 가입 해지 |   | GET |
|   |   |   |   |   |   | 보고서 |
|   |   |   |   |   |   | 검색 |

{style=&quot;table-layout:auto&quot;}

### UserRole

| 필드 | 참조 | 컬렉션 | 검색 | 액션 | 쿼리 | 작업 |
|---|---|---|---|---|---|---|
| roleID | 역할 |   |   |   |   |   |
| timePercentage | 사용자 |   |   |   |   |   |
| userID |   |   |   |   |   |   |
