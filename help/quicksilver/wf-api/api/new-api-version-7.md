---
content-type: api
navigation-topic: api-navigation-topic
title: API 버전 7의 새로운 기능
description: 컬렉션
author: Becky
feature: Workfront API
role: Developer
exl-id: 8c575251-677b-474d-84aa-02b637ef7760
source-git-commit: 3e339e2bfb26e101f0305c05f620a21541394993
workflow-type: tm+mt
source-wordcount: '498'
ht-degree: 43%

---

# API 버전 7의 새로운 기능

## 새 개체

### 증명 빈

| 필드 | 참조 | 컬렉션 | 검색 | 액션 | 쿼리 | 작업 |
|---|---|---|---|---|---|---|
| ID |   |   |   |   |   | 검색 |
| deadLine |   |   |   |   |   |   |
| 이름 |   |   |   |   |   |   |

{style="table-layout:auto"}

### 문서 메타데이터 링크

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <col> 
 <col> 
 <col> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th>필드</th> 
   <th>참조</th> 
   <th> <p data-sheets-value="{&quot;1&quot;:2,&quot;2&quot;:&quot;Type&quot;}">컬렉션</p> <p data-sheets-value="{&quot;1&quot;:2,&quot;2&quot;:&quot;Type&quot;}">+++++++++++ </p> </th> 
   <th>검색</th> 
   <th>액션</th> 
   <th>쿼리</th> 
   <th>작업</th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td>ID</td> 
   <td> </td> 
   <td> </td> 
   <td> </td> 
   <td> </td> 
   <td> </td> 
   <td>추가</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td> </td> 
   <td> </td> 
   <td> </td> 
   <td> </td> 
   <td>카운트 </td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td> </td> 
   <td> </td> 
   <td> </td> 
   <td> </td> 
   <td>삭제 </td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td> </td> 
   <td> </td> 
   <td> </td> 
   <td> </td> 
   <td>Get  </td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td> </td> 
   <td> </td> 
   <td> </td> 
   <td> </td> 
   <td>보고서 </td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td> </td> 
   <td> </td> 
   <td> </td> 
   <td> </td> 
   <td>검색 </td> 
  </tr> 
 </tbody> 
</table>

### 문서 메타데이터 링크 그룹

| 필드 | 참조 | 컬렉션 | 검색 | 액션 | 쿼리 | 작업 |
|---|---|---|---|---|---|---|
| ID |   |   |   |   |   | 추가 |
|   |   |   |   |   |   | 개수 |
|   |   |   |   |   |   | 삭제 |
|   |   |   |   |   |   | Get |
|   |   |   |   |   |   | 보고서 |
|   |   |   |   |   |   | 검색 |

{style="table-layout:auto"}

### ProofApproval

| 필드 | 참조 | 컬렉션 | 검색 | 액션 | 쿼리 | 작업 |
|---|---|---|---|---|---|---|
| ID |   |   |   |   |   | 개수 |
|   |   |   |   |   |   | Get |
|   |   |   |   |   |   | 보고서 |
|   |   |   |   |   |   | 검색 |

{style="table-layout:auto"}

 

### 리소스 윤곽선

| 필드 | 참조 | 컬렉션 | 검색 | 액션 | 쿼리 | 작업 |
|---|---|---|---|---|---|---|
| ID |   |   |   |   |   | 추가 |
|   |   |   |   |   |   | 개수 |
|   |   |   |   |   |   | 삭제 |
|   |   |   |   |   |   | 편집 |
|   |   |   |   |   |   | Get |
|   |   |   |   |   |   | 보고서 |
|   |   |   |   |   |   | 검색 |

{style="table-layout:auto"}

 

### 사용자 그룹

| 필드 | 참조 | 컬렉션 | 검색 | 액션 | 쿼리 | 작업 |
|---|---|---|---|---|---|---|
| groupID | 그룹 |   |   |   |   |   |
| isOwner  | 사용자  |   |   |   |   |   |
| userID  |   |   |   |   |   |   |

{style="table-layout:auto"}

 

### 타임시트 프로필

| 필드 | 참조 | 컬렉션 | 검색 | 액션 | 쿼리 | 작업 |
|---|---|---|---|---|---|---|
| ID |   |  hourType |   |   |   | 추가 |
| 이름 |   |   |   |   |   | 복사 |
|   |   |   |   |   |   | 개수 |
|   |   |   |   |   |   | 삭제 |
|   |   |   |   |   |   | 편집 |
|   |   |   |   |   |   | Get |
|   |   |   |   |   |   | 보고서 |
|   |   |   |   |   |   | 검색 |
|   |   |   |   |   |   | 바꾸기 |

{style="table-layout:auto"}

 

### RsrcPool

| 필드 | 참조 | 컬렉션 | 검색 | 액션 | 쿼리 | 작업 |
|---|---|---|---|---|---|---|
| ID | 고객 | 사용자 |   |   |   | 추가 |
| customerID  | 입력한 사람  |   |   |   |   | 개수 |
| 설명  | lastUpdatedBy  |   |   |   |   | 삭제 |
| 입력자 ID  |   |   |   |   |   | 편집 |
| entryDate  |   |   |   |   |   | Get |
| extRefID  |   |   |   |   |   | 보고서 |
| 마지막 업데이트 날짜 |   |   |   |   |   | 검색 |
| lastUpdateById |   |   |   |   |   |   |
| 이름 |   |   |   |   |   |   |

{style="table-layout:auto"}

 

### 문서 메타데이터 링크 그룹

| 필드 | 참조 | 컬렉션 | 검색 | 액션 | 쿼리 | 작업 |
|---|---|---|---|---|---|---|
| ID |   |   |   |   |   | 개수 |
| articleName  |   |   |   |   |   | Get |
| pageID  |   |   |   |   |   | 보고서 |
| url  |   |   |   |   |   | 검색 |

{style="table-layout:auto"}

 

 

 

## 업데이트된 개체

기존 객체에 대한 변경 사항: 추가는 간단히 나열되고, 제거는 취소선이 있으며, 기존 객체에 대한 변경 사항은 테이블 뒤에 메모가 첨부되어 있습니다

### UpdateBean

| 필드 | 참조 | 컬렉션 | 검색 | 액션 | 쿼리 | 작업 |
|---|---|---|---|---|---|---|
| updateType<sup>1</sup> |   |   |   |   |   |   |

{style="table-layout:auto"}

가능한 값에 대한 <sup>1</sup> 변경 

 

### ApprovalServiceObject

| 필드 | 참조 | 컬렉션 | 검색 | 액션 | 쿼리 | 작업 |
|---|---|---|---|---|---|---|
| approvalCompleteDate |   |   |   |   |   |   |
| 승인 시작 날짜<sup>1</sup> |   |   |   |   |   |   |
| 일별 작업 목록 |   |   |   |   |   |    |

{style="table-layout:auto"}

 

### AccessRule<sup>1</sup>

<sup>1</sup>이(가) 보고 가능한 것으로 표시됨

 

### 승인 진행

| 필드 | 참조 | 컬렉션 | 검색 | 액션 | 쿼리 | 작업 |
|---|---|---|---|---|---|---|
|   |   | `AttachedApprovalPaths`  |   |   |   |   |

{style="table-layout:auto"}

  

### 승인 경로<sup>1</sup>

| 필드 | 참조 | 컬렉션 | 검색 | 액션 | 쿼리 | 작업 |
|---|---|---|---|---|---|---|
|   |   |   |   |   |   | `Add` |
|   |   |   |   |   |   | `Delete` |
|   |   |   |   |   |   | `Edit` |

{style="table-layout:auto"}

<sup>1</sup> 보고 가능 플래그가 제거됨

 

### 작업 서비스 개체

| 필드 | 참조 | 컬렉션 | 검색 | 액션 | 쿼리 | 작업 |
|---|---|---|---|---|---|---|
| approvalCompleteDate |   |   |   |   |   |   |
| approvalStartDate |   |   |   |   |   |   |
| 일별 작업 목록 |   |   |   |   |   |   |

{style="table-layout:auto"}

<sup>1</sup> 날짜 유효성 검사 추가됨

<sup>2</sup> Not_Filterable 플래그가 추가됨

 

### 할당

| 필드 | 참조 | 컬렉션 | 검색 | 액션 | 쿼리 | 작업 |
|---|---|---|---|---|---|---|
|  일별 작업 목록 |   |   |   | assignUserToRoleOnProjects<sup>1</sup> |   |   |
|   |   |   |   | swapUsersOnProjects<sup>1</sup> |   |   |
|   |   |   |   | 프로젝트 할당 해제<sup>1</sup> |   |   |

{style="table-layout:auto"}

<sup>1</sup> 추가된 필드 includeIssues

 

### 고객 

| 필드 | 참조 | 컬렉션 | 검색 | 액션 | 쿼리 | 작업 |
|---|---|---|---|---|---|---|
| bizRuleExclusions<sup>1</sup> |   |   |   |   |   |   |

{style="table-layout:auto"}

가능한 값에 대한 <sup>1</sup> 변경 

 

### 사용자 정의 열거형 

| 필드 | 참조 | 컬렉션 | 검색 | 액션 | 쿼리 | 작업 |
|---|---|---|---|---|---|---|
| groupID  |   |   |   |   |   |   |

{style="table-layout:auto"}

 

### 문서 

| 필드 | 참조 | 컬렉션 | 검색 | 액션 | 쿼리 | 작업 |
|---|---|---|---|---|---|---|
| checkOutTimestamp |   |   |   |  createProof |   |   |

{style="table-layout:auto"}

 

### DocumentVersion 

| 필드 | 참조 | 컬렉션 | 검색 | 액션 | 쿼리 | 작업 |
|---|---|---|---|---|---|---|
|   |   |   |   |  getProofingTokens |   |   |

{style="table-layout:auto"}

 

### 그룹

| 필드 | 참조 | 컬렉션 | 검색 | 액션 | 쿼리 | 작업 |
|---|---|---|---|---|---|---|
| isPublic |  layoutTemplate | 사용자 그룹  |   |   |   |   |
| 레이아웃 템플릿 ID |   |   |   |   |   |   |

{style="table-layout:auto"}

<sup>1</sup>이(가) PRECISION 유효성 검사기를 8에서 9로 변경했습니다.

 

### HourType

| 필드 | 참조 | 컬렉션 | 검색 | 액션 | 쿼리 | 작업 |
|---|---|---|---|---|---|---|
|   |   |   |   |   | defaultOpTaskHourType |   |
|   |   |   |   |   | defaultProjectHourType |   |
|   |   |   |   |   | defaultTaskHourType  |   |
|   |   |   |   |   | globalHourTypes  |   |
|   |   |   |   |   | objectHourTypes  |   |

{style="table-layout:auto"}

 

### 저널 항목

| 필드 | 참조 | 컬렉션 | 검색 | 액션 | 쿼리 | 작업 |
|---|---|---|---|---|---|---|
| changeType<sup>1</sup> |   |   |   |   |   |   |

{style="table-layout:auto"}

가능한 값에 대한 <sup>1</sup> 변경

 

### Optask(문제)

| 필드 | 참조 | 컬렉션 | 검색 | 액션 | 쿼리 | 작업 |
|---|---|---|---|---|---|---|
| approvalCompleteDate |   |   |   |  assignMultiple |   |   |
| approvalStartDate |   |   |   |   |   |   |

{style="table-layout:auto"}

 

 

### 프로젝트

| 필드 | 참조 | 컬렉션 | 검색 | 액션 | 쿼리 | 작업 |
|---|---|---|---|---|---|---|
| approvalCompleteDate |   |   |   |   |   |   |
| approvalStartDate |   |   |   |   |   |   |

{style="table-layout:auto"}

 

 

### QueueDef

| 필드 | 참조 | 컬렉션 | 검색 | 액션 | 쿼리 | 작업 |
|---|---|---|---|---|---|---|
| allowedLegacyQueueTopicIDs |  |  |  | getQueueDefTree |   |   |

{style="table-layout:auto"}

 

### 대기열 주제

| 필드 | 참조 | 컬렉션 | 검색 | 액션 | 쿼리 | 작업 |
|---|---|---|---|---|---|---|
|   |   |   |   |   |  대기열 주제 ID |   |

{style="table-layout:auto"}

 

### 최근 항목

| 필드 | 참조 | 컬렉션 | 검색 | 액션 | 쿼리 | 작업 |
|---|---|---|---|---|---|---|
|   |   |   |   |  updateLastViewsObject |   |   |

{style="table-layout:auto"}

 

### 작업

| 필드 | 참조 | 컬렉션 | 검색 | 액션 | 쿼리 | 작업 |
|---|---|---|---|---|---|---|
| approvalCompleteDate |   |   |   | assignMultiple  |   |   |
| approvalStartDate |   |   |   |   |   |   |
| 일별 작업 목록 |   |   |   |   |   |   |

{style="table-layout:auto"}

 

### TemplateTask

| 필드 | 참조 | 컬렉션 | 검색 | 액션 | 쿼리 | 작업 |
|---|---|---|---|---|---|---|
| 작업 필요<sup>1</sup> |   |   |   |   |   |   |

{style="table-layout:auto"}

<sup>1</sup> 형식이 Int에서 Double로 변경됨 

 

### 사용자

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <col> 
 <col> 
 <col> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th>필드</th> 
   <th>참조</th> 
   <th>컬렉션</th> 
   <th>검색</th> 
   <th>액션</th> 
   <th>쿼리</th> 
   <th>작업</th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td>
    <code>lastWhatsNew</code> </td> 
   <td> </td> 
   <td>
    <code>roles</code> </td> 
   <td> 역할</td> 
   <td>add모바일 장치</td> 
   <td> </td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td> <span data-sheets-value="{&quot;1&quot;:2,&quot;2&quot;:&quot;scheduleDeactivationDate&quot;}" data-sheets-userformat="{&quot;2&quot;:8707,&quot;3&quot;:{&quot;1&quot;:0},&quot;4&quot;:{&quot;1&quot;:2,&quot;2&quot;:14277081},&quot;12&quot;:0,&quot;16&quot;:10}">scheduleDeactivationDate</span></td> 
   <td> </td> 
   <td><span data-sheets-value="{&quot;1&quot;:2,&quot;2&quot;:&quot;timesheetProfileHourTypes&quot;}" data-sheets-userformat="{&quot;2&quot;:8707,&quot;3&quot;:{&quot;1&quot;:0},&quot;4&quot;:{&quot;1&quot;:2,&quot;2&quot;:14277081},&quot;12&quot;:0,&quot;16&quot;:10}">timesheetProfileHourTypes</span> </td> 
   <td> </td> 
   <td>getAvailableActions</td> 
   <td> </td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td> </td> 
   <td> </td> 
   <td>hasAnyAccess</td> 
   <td> </td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td> </td> 
   <td> </td> 
   <td>isUserTermActive</td> 
   <td> </td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td> </td> 
   <td> </td> 
   <td> <p>removeMobileDevice</p> </td> 
   <td> </td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td> </td> 
   <td> </td> 
   <td>showShouldProofHQNavButton</td> 
   <td> </td> 
   <td>  </td> 
  </tr> 
 </tbody> 
</table>

### 사용자 메모

| 필드 | 참조 | 컬렉션 | 검색 | 액션 | 쿼리 | 작업 |
|---|---|---|---|---|---|---|
| `acknowledgedmentIDs` |   |   |   |  unackknowledgeMany |   |   |
| 날짜 |   |   |   |   |   |   |
| ackType |   |   |   |   |   |   |

{style="table-layout:auto"}

 

 

### CustomerPrefObject

| 필드 | 참조 | 컬렉션 | 검색 | 액션 | 쿼리 | 작업 |
|---|---|---|---|---|---|---|
|  이름 |   |   |   |   |   |   |

{style="table-layout:auto"}

가능한 값에 대한 <sup>1</sup> 변경
