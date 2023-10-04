---
content-type: api
navigation-topic: api-navigation-topic
title: 이벤트 구독 리소스 필드
description: 이벤트 구독 리소스 필드
author: Becky
feature: Workfront API
exl-id: 54859930-7619-4b93-8dff-29b10e43d6d5
source-git-commit: 012d53d4773ea8fa377ea7c65cea6cc411ef5321
workflow-type: tm+mt
source-wordcount: '633'
ht-degree: 10%

---

# 이벤트 구독 리소스 필드

이벤트 구독 리소스 필드는 구성된 끝점에 아웃바운드 메시지를 전송하는 이벤트 구독을 발생시키는 이벤트에 대한 트리거를 나타냅니다. 리소스 필드를 편집하면 UPDATE 이벤트가 트리거됩니다.

다음 표에는 이벤트 구독 리소스에 사용할 수 있는 필드가 나열되어 있습니다.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th>리소스</th> 
   <th>objCode</th> 
   <th>필드</th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td>할당</td> 
   <td>ASSIGN</td> 
   <td>실제 작업 완료</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>actualWorkPerDayStartDate</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>assignedByID</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>assignedToID</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td> assignmentPercent </td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td> avgWorkperDay </td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td> 분류자 ID </td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td> customerID </td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td> ID </td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>isPrimary</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td> isTeamAssignment </td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td> objCode </td> 
  </tr> 
  <tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td> opTaskId </td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td> 예상 평균 작업 시간(일) </td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td> projectedUserAllocationPercentage </td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td> projectID </td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>roleID</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td> 보안 루트 ID </td> 
  </tr> 
  <tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>상태</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>taskID</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>teamID</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>작업</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>작업 날짜</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>일별 작업 목록</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>작업 필요</td> 
  </tr> 
  <tr> 
   <td>회사</td> 
   <td>지저분해</td> 
   <td>범주 ID</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>customerID</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>입력자 ID</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td> ID </td> 
  </tr> 
  <tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td> extRefID </td> 
  </tr> 
  <tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td> groupID </td> 
  </tr> 
  <tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>마지막 업데이트 날짜</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>lastUpdatedByID</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>이름</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td> objCode </td> 
  </tr> 
  <tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td> 매개 변수 값 </td> 
  </tr> 
  <tr> 
  <tr> 
   <td>대시보드</td> 
   <td>PTLTAB</td> 
   <td>접근자 ID</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>customerID</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>설명</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>docID</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>extRefID</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>ID</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td> <p>마지막 업데이트 날짜</p> <p>참고: LastUpdateDate는 각 날 동안 처음 업데이트되는 이벤트만 트리거합니다. </p> </td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>lastUpdatedByID</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>이름</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>objCode</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>포털 프로필 ID</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>userID</td> 
  </tr> 
  <tr> 
   <td>문서</td> 
   <td>도쿠</td> 
   <td>접근자 ID</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>범주 ID</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>현재 버전 ID</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>customer:isAdvancedDocMgmtEnabled</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>customerID</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>설명</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>문서 요청 ID</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>extRefID</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>그룹</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>ID</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>반복 ID</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>마지막 메모 ID</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>마지막 업데이트 날짜</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td> lastUpdatedByID </td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>이름</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>메모 ID</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>objCode</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>objID</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>opTaskId</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>소유자 ID</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>매개 변수 값</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>포트폴리오 ID</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>programID</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>projectID</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td> <p>referenceNumber</p> </td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>referenceObjID</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>릴리스 버전 ID</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>보안 루트 ID</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>taskID</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>templateID</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>템플릿 작업 ID</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>topObjID</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>userID</td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td><span>DocumentVersion</span> </td> 
   <td><span>DOCV</span> </td> 
   <td><span>접근자 ID</span> </td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>active증명 단계</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>customerID</td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> </td> 
   <td> </td> 
   <td><span>documentID</span> </td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>문서 공급자 ID</td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> </td> 
   <td> </td> 
   <td><span>docSize</span> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> </td> 
   <td> </td> 
   <td><span>entryDate</span> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> </td> 
   <td> </td> 
   <td><span>입력자 ID</span> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> </td> 
   <td> </td> 
   <td><span>ext</span> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> </td> 
   <td> </td> 
   <td><span>externalIntegrationType</span> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> </td> 
   <td> </td> 
   <td><span>외부 스토리지 ID</span> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> </td> 
   <td> </td> 
   <td><span>fileName</span> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> </td> 
   <td> </td> 
   <td><span>fileType</span> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> </td> 
   <td> </td> 
   <td><span>ID</span> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> </td> 
   <td> </td> 
   <td><span>위치</span> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> </td> 
   <td> </td> 
   <td><span>objCode</span> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> </td> 
   <td> </td> 
   <td><span>proofApprovalStatusID</span> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> </td> 
   <td> </td> 
   <td><span>proofedByUserID</span> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> </td> 
   <td> </td> 
   <td><span>proofDeadlineDate</span> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> </td> 
   <td> </td> 
   <td><span>증명 결정</span> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> </td> 
   <td> </td> 
   <td><span>proofID</span> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> </td> 
   <td> </td> 
   <td><span>proofName</span> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> </td> 
   <td> </td> 
   <td><span>proofOwnerID</span> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> </td> 
   <td> </td> 
   <td><span>증명 페이지</span> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> </td> 
   <td> </td> 
   <td><span>증명 진행</span> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> </td> 
   <td> </td> 
   <td><span>증명 단계 ID</span> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> </td> 
   <td> </td> 
   <td><span>버전</span> </td> 
  </tr> 
  <tr> 
   <td>경비</td> 
   <td>확장</td> 
   <td> 실제 금액 </td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td> 실제 단위 금액 </td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td> billingRecordID </td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td> 범주 ID </td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>customerID</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>사용자 정의 양식 ID</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>설명</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>유효 날짜</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>입력자 ID</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>entryDate</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>expObjCode</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>경비 유형 ID</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>extRefID</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>ID </td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>isBillable</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td> isRevisable </td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td> isRepared </td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>마지막 업데이트 날짜</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>lastUpdatedByID</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>objCode</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>objectCategors</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>objID</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>parameterValues*</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>계획된 금액</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>plannedDate</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>plannedUnitMount</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>projectID</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>referenceObjCode</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>referenceObjID</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>referenceObjectName</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>보안 루트 ID </td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>taskID</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>templateID </td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>템플릿 작업 ID </td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>topObjCode</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>topObjID</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>topReferenceObjCode</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>topReferenceObjID</td> 
  </tr> 
  <tr> 
   <td>시간</td> 
   <td>시간</td> 
   <td>접근자 ID</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td> 실제 비용 </td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>승인자 ID</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>approveOnDate</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>billingRecordID</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>customerID</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>설명</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>dupID</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>entryDate</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>외부 타임시트 ID</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>extRefID</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>시간</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>hourTypeId</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>ID</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>마지막 업데이트 날짜</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>lastUpdatedByID</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>objCode</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>opTaskId</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>소유자 ID</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>projectID</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>프로젝트 오버헤드 ID</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>referenceObjCode</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>referenceObjID</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>roleID</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>보안 루트 ID</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>상태</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>taskID</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>타임시트 ID</td> 
  </tr> 
  <tr> 
   <td>문제</td> 
   <td>OPTASK</td> 
   <td>접근자 ID</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>승인 프로세스 ID</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>assignedToID</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>범주 ID</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>현재 승인 단계 ID</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>customerID</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>설명</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>입력자 ID</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>entryDate</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>extRefID</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>groupID</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>ID</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>반복 ID</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>칸반 보드 ID</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>lastConditionNoteID</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>마지막 메모 ID</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>마지막 업데이트 날짜</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>lastUpdatedByID</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>이름</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>objCode</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>소유자 ID</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>parameterValues*</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>계획된 완료 일자</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>우선 순위</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>projectID</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>queueDefID</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>대기열 주제 ID</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>referenceNumber</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>referenceObjID</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>거부 문제 ID</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>resolveOpTaskID</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>resolveProjectId</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>resolveTaskId</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>resolingObjID</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>roleID</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>루트 그룹 ID</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>보안 루트 ID</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>sourceObjID</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>sourceTaskId</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>상태</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>submittedByID</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>teamID</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>workflowAutomationid</td> 
  </tr> 
  <tr> 
   <td>참고</td> 
   <td>메모</td> 
   <td>접근자 ID</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>문서 ID 첨부</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>attachobjID</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>attachopTaskID</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>attachWorkID</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>attachWorkUserID</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>감사 레코드 ID</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>customerID</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>documentID</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>entryDate</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>외부 서비스 ID</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>extRefID</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>ID</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>반복 ID</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>메모 텍스트</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>objCode</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>objID</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>opTaskId</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>소유자 ID</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>parentAuthorizationID</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>parentJournalEntryID</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>상위 메모 ID</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>포트폴리오 ID</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>programID</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>projectID</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>증명 작업 ID</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>리치 텍스트 메모 ID</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>보안 루트 ID</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>제목</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>taskID</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>templateID</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>템플릿 작업 ID</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>threadID</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>타임시트 ID</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>topObjID</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>userID</td> 
  </tr> 
  <tr> 
   <td>포트폴리오</td> 
   <td>포트</td> 
   <td>접근자 ID</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>정렬 점수 카드 ID</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>범주 ID</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>customerID</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>설명</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>입력자 ID</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>entryDate</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>extRefID</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>groupID</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>ID</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>마지막 업데이트 날짜</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>lastUpdatedByID</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>이름</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>objCode</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>소유자 ID</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>parameterValues*</td> 
  </tr> 
  <tr> 
   <td>프로그램</td> 
   <td>PRGM</td> 
   <td>접근자 ID</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>범주 ID</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>customerID</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>설명</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>입력자 ID</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>extRefID</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>groupID</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>ID</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>마지막 업데이트 날짜</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>lastUpdatedByID</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>이름</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>objCode</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>소유자 ID</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>parameterValues*</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>포트폴리오 ID</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>보안 루트 ID</td> 
  </tr> 
  <tr> 
   <td>프로젝트</td> 
   <td>프로젝트</td> 
   <td>접근자 ID</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>정렬 점수 카드 ID</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>승인 프로세스 ID</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>attachedRateCardID </td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>범주 ID</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>companyID</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>convertedOpTaskID</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>convertedOpTaskOriginatorID</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>통화</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>현재 승인 단계 ID</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>customerID</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>deliverableScore카드 ID</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>설명</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>입력자 ID</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>entryDate</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>extRefID</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>groupID</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>ID</td> 
  </tr> 
    <tr> 
   <td> </td> 
   <td> </td> 
   <td>issueWorkflowAutomationid</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>lastConditionNoteID</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>마지막 메모 ID</td> 
  </tr> 
<tr> 
   <td> </td> 
   <td> </td> 
   <td>마지막 업데이트 날짜</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>lastUpatedByID</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>마일스톤 경로 ID</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>이름</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>objCode</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>소유자 ID</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>parameterValues*</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>계획된 완료 일자</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>popAccountID</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>우선 순위</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>programID</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>queueDefID</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>referenceNumber</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>거부 문제 ID</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>리소스 풀 ID</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>루트 그룹 ID</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>일정 ID</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>스폰서 ID</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>상태</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>submittedByID</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>작업 워크플로 자동화 ID</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>teamID</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>templateID</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>workflowAutomationid</td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td><span>ProofApproval</span> </td> 
   <td><span>PRFAPL</span> </td> 
   <td><span>접근자 ID</span> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> </td> 
   <td> </td> 
   <td><span>승인자 결정</span> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> </td> 
   <td> </td> 
   <td><span>approverID</span> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> </td> 
   <td> </td> 
   <td><span>customerID</span> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> </td> 
   <td> </td> 
   <td><span>documentID</span> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> </td> 
   <td> </td> 
   <td><span>문서 버전 ID</span> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> </td> 
   <td> </td> 
   <td><span>ID</span> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> </td> 
   <td> </td> 
   <td><span>isAwaitingDecision</span> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> </td> 
   <td> </td> 
   <td><span>objCode</span> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> </td> 
   <td> </td> 
   <td><span>증명 생성 날짜</span> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> </td> 
   <td> </td> 
   <td><span>requesterID</span> </td> 
  </tr> 
  <tr> 
   <td>보고서</td> 
   <td>PTLSEC</td> 
   <td>접근자 ID</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>appGlobalID</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>customerID</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>설명</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>입력자 ID</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>extRefID</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>filterID</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>groupByID</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>ID</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>마지막 업데이트 날짜</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>lastUpdatedByID</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>lastViewedByID</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>이름</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>objCode</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>objID</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>preferenceID</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>publicRunAsUserid</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>보고서 폴더 ID</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>실행 사용자 ID</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>예약된 보고서 ID</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>보안 루트 ID</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>uiObjCode</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>viewID</td> 
  </tr> 
  <tr> 
   <td>작업</td> 
   <td>작업</td> 
   <td>접근자 ID</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>승인 프로세스 ID</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>assignedToID</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>billingRecordID</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>범주 ID</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>convertedOpTaskID</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>convertedOpTaskOriginatorID</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>현재 승인 단계 ID</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>customerID</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>설명</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>입력자 ID</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>entryDate</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>마지막 업데이트 날짜</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>extRefID</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>groupID</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>ID</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>반복 ID</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>칸반 보드 ID</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>lastConditionNoteID</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>마지막 메모 ID</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>마지막 업데이트 날짜</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>lastUpdatedByID</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>이정표 ID</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>이름</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>objCode</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>parameterValues*</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>parentID</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>계획된 완료 일자</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>우선 순위</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>projectID</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>자동연장 규칙 ID</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>referenceNumber</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>거부 문제 ID</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>roleID</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>루트 그룹 ID</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>보안 루트 ID</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>상태</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>submittedByID</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>teamID</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>템플릿 작업 ID</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>workflowAutomationid</td> 
  </tr> 
  <tr> 
   <td>템플릿</td> 
   <td>템플릿</td> 
   <td>접근자 ID</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>승인 프로세스 ID</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>범주 ID</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>companyID</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>deliverableScore카드 ID</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>customerID</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>설명</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>입력자 ID</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>entryDate</td> 
  </tr> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>extRefID</td> 
  </tr> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>groupID</td> 
  </tr> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>ID</td> 
  </tr> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>issueWorkflowAutomationid</td> 
  </tr> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>마지막 메모 ID</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>마지막 업데이트 날짜</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>lastUpdatedByID</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>마일스톤 경로 ID</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>이름</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>objCode</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>소유자 ID</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>parameterValues*</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>우선 순위</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>programID</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>queueDefID</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>포트폴리오 ID</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>referenceNumber</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>일정 ID</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>스폰서 ID</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>작업 워크플로 자동화 ID</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>teamID</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>workflowAutomationid</td> 
  </tr> 
  <tr> 
   <td>타임시트</td> 
   <td>체트</td> 
   <td>approverID</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>approversListString</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>customerID</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>displayName</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>endDate </td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>extRefID</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>hasNotes</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>ID</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>hoursDuration</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>isEdit</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>마지막 메모 ID</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>마지막 업데이트 날짜</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>lastUpdatedByID</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>objCode</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>초과 작업 시간</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>regularHour</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>startDate </td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>상태</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>타임시트 프로필 ID</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>totalHours</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>userID</td> 
  </tr> 
  <tr> 
   <td>사용자</td> 
   <td>사용자</td> 
   <td>액세스 수준 ID</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>범주 ID</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>companyID</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>customerID</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>기본 시간 유형 ID</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>위임 대상 ID</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>eauthUserID</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>이메일 주소</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>입력자 ID</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>extRefID</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>홈 그룹 ID</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>홈 팀 ID</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>ID</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>활성</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>lastEnteredNoteID</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>lastLoginDate</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>마지막 메모 ID</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>마지막 업데이트 날짜</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>lastUpdatedByID</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>latestUpdateNoteID</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>레이아웃 템플릿 ID</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>logTimeInDays</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>managerID</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>이름</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>objCode</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>parameterValues*</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>포털 프로필 ID</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>리소스 풀 ID</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>roleID</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>일정 ID</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>타임시트 프로필 ID</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>title</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>uiTemplateID</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>uumUserID</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>workHoursPerDay </td> 
  </tr> 
 </tbody> 
</table>

&#42;parameterValue는 다양한 Workfront 리소스(또는 개체)와 연결된 사용자 지정 필드 값입니다. 이벤트 구독 아웃바운드 메시지에는 채워진 parameterValues(사용자 정의 필드)의 전체 목록이 포함됩니다.
