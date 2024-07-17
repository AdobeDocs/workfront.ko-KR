---
content-type: api
navigation-topic: api-navigation-topic
title: API 버전 11의 새로운 기능
description: ReportableBudgedHour가 보고를 위한 리소스로 Adobe Workfront API에 추가되었습니다. 여기에는 BudgetedHour에 없는 참조 필드, 핵심 필드 및 기본 필드가 포함되어 있습니다.
author: Becky
feature: Workfront API
role: Developer
exl-id: b8826dc6-9791-49f6-923d-5a0c5392a8b0
source-git-commit: 3e339e2bfb26e101f0305c05f620a21541394993
workflow-type: tm+mt
source-wordcount: '3573'
ht-degree: 2%

---

# API 버전 11의 새로운 기능

* [추가된 리소스](#added-resources)
* [제거된 리소스](#removed-resources)
* [수정된 리소스](#modified-resources)

## 추가된 리소스 {#added-resources}

<!--
  <li data-mc-conditions="QuicksilverOrClassic.Draft mode"><a href="#loginasaccessrule" class="MCXref xref">LoginAsAccessRule</a> </li>
  -->

<!--
  <li data-mc-conditions="QuicksilverOrClassic.Draft mode"><a href="#loginasadditionalrule" class="MCXref xref">LoginAsAdditionalRule</a> </li>
  -->

<!--
  <li data-mc-conditions="QuicksilverOrClassic.Draft mode"><a href="#loginassettings" class="MCXref xref">LoginAsSettings</a> </li>
  -->

* [ReportableBudgetHour](#reportablebudgetedhour)

<!--
<h3 data-mc-conditions="QuicksilverOrClassic.Draft mode" id="loginasaccessrule">LoginAsAccessRule</h3>
-->

<table style="table-layout:auto"> <!--
  <col data-mc-conditions="QuicksilverOrClassic.Draft mode">
 --> <!--
  <col data-mc-conditions="QuicksilverOrClassic.Draft mode">
 --> 
 <tbody> 
  <tr> 
   <td>직접 필드</td> 
   <td> 
    <ul> 
     <li style="font-weight: bold;">accessExpirationDate</li> 
     <li style="font-weight: bold;">접근자 ID</li> 
     <li style="font-weight: bold;">customerID</li> 
     <li style="font-weight: bold;">ID</li> 
     <li style="font-weight: bold;">userID</li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>참조 필드</td> 
   <td> 
    <ul> 
     <li style="font-weight: bold;">접근자</li> 
     <li style="font-weight: bold;">고객</li> 
     <li style="font-weight: bold;">사용자  </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>코어 필드</td> 
   <td> 
    <ul> 
     <li style="font-weight: bold;">ID</li> 
     <li style="font-weight: bold;">objCode</li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

<!--
<h3 data-mc-conditions="QuicksilverOrClassic.Draft mode" id="loginasadditionalrule">LoginAsAdditionalRule</h3>
-->

<table style="table-layout:auto"> <!--
  <col data-mc-conditions="QuicksilverOrClassic.Draft mode">
 --> <!--
  <col data-mc-conditions="QuicksilverOrClassic.Draft mode">
 --> 
 <tbody> 
  <tr> 
   <td>직접 필드</td> 
   <td> 
    <ul> 
     <li style="font-weight: bold;">customerID</li> 
     <li style="font-weight: bold;">ID</li> 
     <li style="font-weight: bold;">loginAsSettingsID</li> 
     <li style="font-weight: bold;">objID</li> 
     <li style="font-weight: bold;">objObjCode  </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>참조 필드</td> 
   <td> 
    <ul> 
     <li style="font-weight: bold;">고객  </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>코어 필드</td> 
   <td> 
    <ul> 
     <li style="font-weight: bold;">ID</li> 
     <li style="font-weight: bold;">objCode</li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

<!--
<h3 data-mc-conditions="QuicksilverOrClassic.Draft mode" id="loginassettings">LoginAsSettings</h3>
-->

<table style="table-layout:auto"> <!--
  <col data-mc-conditions="QuicksilverOrClassic.Draft mode">
 --> <!--
  <col data-mc-conditions="QuicksilverOrClassic.Draft mode">
 --> 
 <tbody> 
  <tr> 
   <td>직접 필드</td> 
   <td> 
    <ul> 
     <li style="font-weight: bold;">customerID</li> 
     <li style="font-weight: bold;">licenseType</li> 
     <li style="font-weight: bold;">ID</li> 
     <li style="font-weight: bold;">restrictedLoginAs  </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>참조 필드</td> 
   <td> 
    <ul> 
     <li style="font-weight: bold;">고객  </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>컬렉션 필드</td> 
   <td> 
    <ul> 
     <li style="font-weight: bold;">additionalRules</li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>코어 필드</td> 
   <td> 
    <ul> 
     <li style="font-weight: bold;">ID</li> 
     <li style="font-weight: bold;">objCode</li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

### ReportableBudgetHour {#reportablebudgetedhour}

ReportableBudgedHour가 보고를 위한 리소스로 Adobe Workfront API에 추가되었습니다. 여기에는 BudgetedHour에 없는 참조 필드, 핵심 필드 및 기본 필드가 포함되어 있습니다.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>직접 필드</td> 
   <td> 
    <ul> 
     <li> <p style="font-weight: bold;">allocationDate </p> <p>할당 일자는 리소스 플래너에서 시간을 예산 설정한 주의 첫 번째 날(일요일)입니다.</p> </li> 
     <li> <p style="font-weight: bold;">budgetHours </p> <p>예산 시간은 프로젝트에서 자원이 완료해야 하는 작업에 대해 자원 관리자가 예산을 책정하는 시간입니다</p> </li> 
     <li> <p style="font-weight: bold;">ID </p> <p>특정 보고 가능한 예산 시간 오브젝트에 할당된 고유한 Workfront ID입니다.</p> </li> 
     <li style="font-weight: bold;">plannedBudgetHours </li> 
     <li> <p style="font-weight: bold;">projectID </p> <p>특정 프로젝트에 할당된 고유한 Workfront ID입니다.</p> </li> 
     <li> <p style="font-weight: bold;">roleID</p> <p>특정 작업 역할에 할당된 고유한 Workfront ID입니다.</p> </li> 
     <li> <p style="font-weight: bold;">userID</p> <p>특정 사용자에게 할당된 고유한 Workfront ID입니다.</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>참조 필드</td> 
   <td> 
    <ul> 
     <li> <p style="font-weight: bold;">프로젝트</p> <p>ReportableBudgetedHour가 연결된 프로젝트입니다.</p> </li> 
     <li> <p style="font-weight: bold;">역할</p> <p>ReportableBudgetedHour가 연결된 작업 역할입니다.</p> </li> 
     <li> <p style="font-weight: bold;">사용자</p> <p>ReportableBudgetedHour와 연결된 사용자입니다.</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>코어 필드</td> 
   <td> 
    <ul> 
     <li style="font-weight: bold;">ID</li> 
     <li style="font-weight: bold;">이름</li> 
     <li style="font-weight: bold;">objCode</li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>기본 필드</td> 
   <td> 
    <ul> 
     <li style="font-weight: bold;">이름</li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>작업</td> 
   <td> 
    <ul> 
     <li style="font-weight: bold;">수</li> 
     <li style="font-weight: bold;">GET</li> 
     <li style="font-weight: bold;">보고서 </li> 
     <li style="font-weight: bold;">검색</li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

## 제거된 리소스 {#removed-resources}

API v11에 대해 제거된 리소스가 없습니다.

## 수정된 리소스 {#modified-resources}

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td> 
    <ul> 
     <li><a href="#accesslevelpermissions" class="MCXref xref">AccessLevelPermissions</a> </li> 
     <li><a href="#accessrequest" class="MCXref xref">AccessRequest</a> </li> 
     <li><a href="#accessrule" class="MCXref xref">AccessRule</a> </li> 
     <li><a href="#approval" class="MCXref xref">승인</a> </li> 
     <li><a href="#approvalpath" class="MCXref xref">승인 경로</a> </li> 
     <li><a href="#approvalprocess" class="MCXref xref">ApprovalProcess</a> </li> 
     <li><a href="#assignment" class="MCXref xref">할당</a> </li> 
     <li><a href="#baselinetask" class="MCXref xref">기준선 작업</a> </li> 
     <li><a href="#category" class="MCXref xref">범주</a> </li> 
     <li><a href="#company" class="MCXref xref">회사</a> </li> 
     <li><a href="#customenum" class="MCXref xref">CustomEnum</a> </li> 
     <li><a href="#customer" class="MCXref xref">고객</a> </li> 
     <li><a href="#customerpreferences" class="MCXref xref">CustomerPreferences</a> </li> 
    </ul> </td> 
   <td> 
    <ul> 
     <li><a href="#docmetadatalinkgroup" class="MCXref xref">DocMetadataLinkGroup</a> </li> 
     <li><a href="#document" class="MCXref xref">문서</a> </li> 
     <li><a href="#iteration" class="MCXref xref">반복</a> </li> 
     <li><a href="#layout-template" class="MCXref xref">레이아웃 템플릿</a> </li> 
     <li><a href="#milestonepath" class="MCXref xref">마일스톤 경로</a> </li> 
     <li><a href="#note" class="MCXref xref">참고</a> </li> 
     <li><a href="#optask" class="MCXref xref">OpTask</a> </li> 
     <li><a href="#parameter" class="MCXref xref">매개 변수</a> </li> 
     <li><a href="#portfolio" class="MCXref xref">Portfolio</a> </li> 
     <li><a href="#program" class="MCXref xref">프로그램</a> </li> 
     <li><a href="#project" class="MCXref xref">프로젝트</a> </li> 
     <li><a href="#proofapproval" class="MCXref xref">ProofApproval</a> </li> 
     <li><a href="#queuedef" class="MCXref xref">QueueDef</a> </li> 
     <li><a href="#reservedtime" class="MCXref xref">예약된 시간</a> </li> 
    </ul> </td> 
   <td> 
    <ul> 
     <li><a href="#resourceplannerfilter" class="MCXref xref">ResourcePlannerFilter</a> </li> 
     <li><a href="#risk" class="MCXref xref">위험</a> </li> 
     <li><a href="#scheduledreport" class="MCXref xref">예약된 보고서</a> </li> 
     <li><a href="#scorecardquestion" class="MCXref xref">ScoreCardQuestion</a> </li> 
     <li><a href="#task" class="MCXref xref">작업</a> </li> 
     <li><a href="#team" class="MCXref xref">팀</a> </li> 
     <li><a href="#template" class="MCXref xref">템플릿</a> </li> 
     <li><a href="#templateassignment" class="MCXref xref">TemplateAssignment</a> </li> 
     <li><a href="#templatetask" class="MCXref xref">TemplateTask</a> </li> 
     <li><a href="#timesheet" class="MCXref xref">타임시트</a> </li> 
     <li><a href="#update" class="MCXref xref">업데이트</a> </li> <!--
      <li data-mc-conditions="QuicksilverOrClassic.Draft mode"><a href="#user" class="MCXref xref">User</a> </li>
     --> 
     <li><a href="#usernote" class="MCXref xref">사용자 메모</a> </li> 
     <li><a href="#work" class="MCXref xref">작업 </a> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

 

### 액세스 수준 권한 {#accesslevelpermissions}

AccessLevelPermissions 개체는 권한 집합을 나타냅니다. 그런 다음 이 권한 집합을 액세스 수준과 연결할 수 있습니다.

<table style="table-layout:auto"> 
 <col data-mc-conditions=""> 
 <col data-mc-conditions=""> 
 <tbody> 
  <tr> 
   <td>직접 필드</td> 
   <td> <p>다음 필드에 가능한 BUDGETING_INFORMATION 값이 추가되었습니다. 이를 통해 권한이 있는 사용자는 플래너에서 우선 순위 및 예산 시간을 편집할 수 있습니다.</p> 
    <ul> 
     <li style="font-weight: bold;">coreAction</li> 
     <li style="font-weight: bold;">forbiddenActions</li> 
     <li style="font-weight: bold;">secondaryActions  </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

### AccessRequest {#accessrequest}

사용자에게 Workfront의 필요한 오브젝트에 대한 액세스 권한이 없는 경우 해당 오브젝트에 대한 액세스를 요청할 수 있습니다. AccessRequest 개체는 이 요청을 나타냅니다.

<table style="table-layout:auto"> 
 <col data-mc-conditions=""> 
 <col data-mc-conditions=""> 
 <tbody> 
  <tr> 
   <td>직접 필드</td> 
   <td> 
    <ul> 
     <li> <p style="font-weight: bold;">작업</p> <p>가능한 값 BUDGETING_INFORMATION이 추가되었습니다. 이를 통해 권한이 있는 사용자는 플래너에서 우선 순위 및 예산 시간을 편집할 수 있습니다.  </p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

### AccessRule {#accessrule}

AccessRule 개체는 사용자가 만드는 프로젝트를 공유할 수 있는 방법을 결정하는 사용자 지정 액세스 수준에 설정된 규칙을 나타냅니다.

<table style="table-layout:auto"> 
 <col data-mc-conditions=""> 
 <col data-mc-conditions=""> 
 <tbody> 
  <tr> 
   <td>직접 필드</td> 
   <td> <p>다음 필드에 가능한 BUDGETING_INFORMATION 값이 추가되었습니다. 이를 통해 권한이 있는 사용자는 플래너에서 우선 순위 및 예산 시간을 편집할 수 있습니다.</p> 
    <ul> 
     <li style="font-weight: bold;">coreAction</li> 
     <li style="font-weight: bold;">forbiddenActions</li> 
     <li style="font-weight: bold;">secondaryActions  </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

### 승인 {#approval}

작업, 문서 또는 타임시트와 같은 특정 작업 항목에서는 감독자 또는 다른 사용자가 해당 작업 항목을 승인해야 할 수 있습니다. 승인 오브젝트는 작업 항목에 대한 사인오프 작업을 나타냅니다.

<table style="table-layout:auto"> 
 <col data-mc-conditions=""> 
 <col data-mc-conditions=""> 
 <tbody> 
  <tr> 
   <td colspan="2">직접 필드<p style="font-weight: normal;">다음 필드에는 AT_DATE_BEFORE_YEAR 및 AT_DATE_AFTER_YEAR 유효성 검사기가 추가되었습니다. 이러한 유효성 검사기는 연결된 오브젝트의 날짜를 1900년 이전 또는 2200년 이후로 설정할 수 없도록 지정합니다.</p>
    <ul>
     <li style="font-weight: bold;">실제 완료 일자</li>
     <li style="font-weight: bold;">actualStartDate</li>
     <li style="font-weight: bold;">constraintDate</li>
     <li style="font-weight: bold;">계획된 완료 일자</li>
     <li style="font-weight: bold;">plannedStartDate</li>
    </ul><p style="font-weight: normal;">EAC(완료 시 추정) 계산의 투명성을 위해 공개 API에 다음 필드가 추가되었습니다.</p>
    <ul>
     <li><p style="font-weight: bold;">bcwp</p><p style="font-weight: normal;">성과 값이라고도 하는 BCWP(수행된 작업의 예산 비용)는 이 지표가 계산될 때 실제로 완료된 작업 금액의 예산 비용을 나타내는 프로젝트 성과 지표입니다. 작업의 경우 BCWP = 실제 완료율 x 작업 예산. 프로젝트의 경우 BCWP = SUM(모든 상위 및 개별 작업의 BCWP 값).</p></li>
     <li><p style="font-weight: bold;">bcws</p><p style="font-weight: normal;">계획된 값이라고도 하는 BCWS(Budgeted Cost of Work Scheduled)는 이 지표가 계산되는 시점에 완료해야 하는 작업 금액의 예산 비용을 나타내는 프로젝트 성과 지표입니다. 작업의 경우 BCWS = 계획된 완료율 x 작업 예산. 프로젝트의 경우 BCWS = SUM(모든 상위 및 개별 작업의 BCWS 값).</p></li>
    </ul><p style="font-weight: normal;">다음 필드에 가능한 값 ET가 추가되었습니다. 이 값은 경과된 시간(월) 단위를 나타내며, 주말이나 공휴일에 관계없이 월을 나타냅니다.</p>
    <ul>
     <li style="font-weight: bold;">durationUnit</li>
     <li style="font-weight: bold;">workUnit</li>
    </ul><p style="font-weight: normal;">다음 필드에 CURRENCY 플래그가 추가되었습니다</p>
    <ul>
     <li style="font-weight: bold;">projectBudgetCost</li>
     <li style="font-weight: bold;">프로젝트 순 가치</li>
    </ul><p style="font-weight: normal;">다음 필드가 승인 오브젝트에서 제거되었습니다.</p>
    <ul>
     <li style="font-weight: bold;">예약된 시간 ID</li>
     <li style="font-weight: bold;">timelineExceptionInfo</li>
    </ul><p style="font-weight: normal;">다음 필드가 승인 개체에 추가되었습니다.</p>
    <ul>
     <li style="font-weight: bold;">storypoints</li>
    </ul></td> 
  </tr> 
  <tr> 
   <td>참조 필드</td> 
   <td> 
    <ul> 
     <li style="font-weight: bold;"> <p>reservedTime</p> <p style="font-weight: normal;">승인 오브젝트에서 제거됨  </p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>컬렉션 필드</td> 
   <td> 
    <ul> 
     <li style="font-weight: bold;"> <p>allConditions</p> <p style="font-weight: normal;">이(가) 승인 개체에 추가되었습니다.</p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

### 승인 경로 {#approvalpath}

ApprovalPath 개체는 승인 프로세스 내의 분기입니다. 승인 경로는 승인 프로세스와 연결된 오브젝트의 상태를 기반으로 합니다.

<table style="table-layout:auto"> 
 <col data-mc-conditions=""> 
 <col data-mc-conditions=""> 
 <tbody> 
  <tr> 
   <td>직접 필드</td> 
   <td> 
    <ul> 
     <li style="font-weight: bold;"> <p>durationUnit </p> <p style="font-weight: normal;">가능한 값 ET가 추가되었습니다. 이 값은 경과된 시간(월) 단위를 나타내며, 주말이나 공휴일에 관계없이 월을 나타냅니다.  </p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

### 승인 프로세스 {#approvalprocess}

ApprovalProcess 개체는 프로젝트, 작업 또는 문제와 연결할 수 있는 여러 단계 승인입니다.

<table style="table-layout:auto"> 
 <col data-mc-conditions=""> 
 <col data-mc-conditions=""> 
 <tbody> 
  <tr> 
   <td>직접 필드</td> 
   <td> 
    <ul> 
     <li style="font-weight: bold;"> <p>활성</p> <p style="font-weight: normal;">이 필드가 추가되었으며, 개체가 활성 상태이면 true 값을 갖고, 그렇지 않으면 false 값을 갖는 부울 매개 변수입니다. 활성으로 설정된 객체는 드롭다운 메뉴와 앞에 입력 필드에 나타나며 다른 객체에 첨부할 수 있습니다. 활성으로 설정되지 않은 객체는 다른 객체에 첨부할 드롭다운 메뉴와 자동 입력 필드에 표시되지 않습니다.  </p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>기본 필드</td> 
   <td> 
    <ul> 
     <li style="font-weight: bold;"> <p>활성</p> <p style="font-weight: normal;">추가됨</p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

### 할당 {#assignment}

할당 개체는 작업 항목과 작업 항목에 할당된 사용자, 팀 또는 그룹 간의 연결을 나타냅니다.

<table style="table-layout:auto"> 
 <col data-mc-conditions=""> 
 <col data-mc-conditions=""> 
 <tbody> 
  <tr> 
   <td>직접 필드</td> 
   <td> 
    <ul> 
     <li style="font-weight: bold;"> <p>workUnit </p> <p style="font-weight: normal;">가능한 값 ET가 추가되었습니다. 이 값은 경과된 시간(월) 단위를 나타내며, 주말이나 공휴일에 관계없이 월을 나타냅니다.  </p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

### 기준선 작업 {#baselinetask}

기준선은 특정 시점의 프로젝트 성능에 대한 스냅샷입니다. 여기에는 주요 날짜, 진행 상황, 비용 및 수익 값과 같은 프로젝트에 대한 주요 정보가 저장됩니다. 베이스라인을 생성하면 작업 정보가 해당 베이스라인의 베이스라인 작업에도 캡처됩니다.

<table style="table-layout:auto"> 
 <col data-mc-conditions=""> 
 <col data-mc-conditions=""> 
 <tbody> 
  <tr> 
   <td>직접 필드</td> 
   <td> 
    <ul> 
     <li style="font-weight: bold;"> <p>durationUnit </p> <p style="font-weight: normal;">가능한 값 ET가 추가되었습니다. 이 값은 경과된 시간(월) 단위를 나타내며, 주말이나 공휴일에 관계없이 월을 나타냅니다.  </p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

### 범주 {#category}

Category 객체는 사용자 정의 양식입니다. 이 개체에 대한 보고서를 작성하고 다른 개체 보고서에도 표시할 수 있습니다.

<table style="table-layout:auto"> 
 <col data-mc-conditions=""> 
 <col data-mc-conditions=""> 
 <tbody> 
  <tr> 
   <td>직접 필드</td> 
   <td> 
    <ul> 
     <li style="font-weight: bold;"> <p>활성</p> <p style="font-weight: normal;">이 필드가 추가되었으며, 개체가 활성 상태이면 true 값을 갖고, 그렇지 않으면 false 값을 갖는 부울 매개 변수입니다. 활성으로 설정된 객체는 드롭다운 메뉴와 앞에 입력 필드에 나타나며 다른 객체에 첨부할 수 있습니다. 활성으로 설정되지 않은 객체는 다른 객체에 첨부할 드롭다운 메뉴와 자동 입력 필드에 표시되지 않습니다.  </p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>기본 필드</td> 
   <td> 
    <ul> 
     <li style="font-weight: bold;"> <p>활성</p> <p style="font-weight: normal;">추가됨</p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

### 회사 {#company}

Company 객체는 사람들의 컬렉션으로 구성된 조직을 나타냅니다. 회사는 사용자 또는 프로젝트와 연결됩니다.

<table style="table-layout:auto"> 
 <col data-mc-conditions=""> 
 <col data-mc-conditions=""> 
 <tbody> 
  <tr> 
   <td>직접 필드</td> 
   <td> 
    <ul> 
     <li style="font-weight: bold;"> <p>활성</p> <p style="font-weight: normal;">이 필드가 추가되었으며, 개체가 활성 상태이면 true 값을 갖고, 그렇지 않으면 false 값을 갖는 부울 매개 변수입니다. 활성으로 설정된 객체는 드롭다운 메뉴와 앞에 입력 필드에 나타나며 다른 객체에 첨부할 수 있습니다. 활성으로 설정되지 않은 객체는 다른 객체에 첨부할 드롭다운 메뉴와 자동 입력 필드에 표시되지 않습니다.  </p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>기본 필드</td> 
   <td> 
    <ul> 
     <li style="font-weight: bold;"> <p>활성</p> <p style="font-weight: normal;">추가됨</p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

### CustomEnum {#customenum}

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">A CustomEnum object is an enumeration that is created in Workfront to be used in objects and fields throughout Workfront.</p>
-->

<table style="table-layout:auto"> 
 <col data-mc-conditions=""> 
 <col data-mc-conditions=""> 
 <tbody> 
  <tr> 
   <td>액션</td> 
   <td> <p style="font-weight: normal;">다음 작업이 CustomEnum 개체에 추가되었습니다</p> 
    <ul> 
     <li style="font-weight: bold;">getDefaultOpTaskConditionEnum</li> 
     <li style="font-weight: bold;">getDefaultProjectConditionEnum</li> 
     <li style="font-weight: bold;">getDefaultTaskConditionEnum</li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>쿼리</td> 
   <td> <p>다음 쿼리가 CustomEnum 개체에 추가되었습니다.</p> 
    <ul> 
     <li style="font-weight: bold;">opTaskConditions</li> 
     <li style="font-weight: bold;">projectConditions</li> 
     <li style="font-weight: bold;">작업 조건</li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

### 고객 {#customer}

Customer 개체는 Workfront 인스턴스를 사용하는 조직을 나타냅니다.

<table style="table-layout:auto"> 
 <col data-mc-conditions=""> 
 <col data-mc-conditions=""> 
 <tbody> 
  <tr data-mc-conditions=""> 
   <td>직접 필드</td> 
   <td> 
    <ul> 
     <li style="font-weight: bold;"> <p>사용자 정의 열거형 유형</p> <p style="font-weight: normal;">가능한 값이 추가되었습니다. </p> 
      <ul> 
       <li style="font-weight: normal;">CONDITION_PROJECT (프로젝트 상태)</li> 
       <li style="font-weight: normal;">CONDITION_TASK(작업 조건)</li> 
       <li style="font-weight: normal;">CONDITION_OPTASK (문제 상태)  </li> 
      </ul> </li> 
    </ul> </td> 
  </tr> <!--
   <tr data-mc-conditions="QuicksilverOrClassic.Draft mode"> 
    <td>Reference Fields</td> 
    <td> 
     <ul> 
      <li style="font-weight: bold;"> <p>loginAsSettings</p> <p style="font-weight: normal;">Added. &nbsp;</p> </li> 
     </ul> </td> 
   </tr>
  --> 
  <tr> 
   <td>액션</td> 
   <td> <p style="font-weight: normal;">다음 작업이 Customer 개체에 추가되었습니다</p> 
    <ul> 
     <li style="font-weight: bold;">goalsEnabled</li> 
     <li style="font-weight: bold;">updateLoginAsSettings</li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

### 고객 환경 설정 {#customerpreferences}

CustomerPreferences 객체는 고객이 Workfront 인스턴스에 대해 설정한 환경 설정 집합을 나타냅니다.

<table style="table-layout:auto"> <!--
  <col data-mc-conditions="QuicksilverOrClassic.Draft mode">
 --> <!--
  <col data-mc-conditions="QuicksilverOrClassic.Draft mode">
 --> 
 <tbody> 
  <tr> 
   <td>직접 필드</td> 
   <td> 
    <ul> 
     <li style="font-weight: bold;"> <p>이름</p> <p style="font-weight: normal;">가능한 값이 추가되었습니다.</p> 
      <ul> 
       <li style="font-weight: normal;">password:password.eauthPolicy(암호 복잡성 요구 사항)</li> 
       <li style="font-weight: normal;"> password:password.minimumLength (최소 암호 길이)</li> 
       <li style="font-weight: normal;">암호:mobileSessionTimeout (모바일 세션 시간 초과)</li> 
       <li style="font-weight: normal;"> project.mgmt:default.project.usertimeoff (사용자 휴무)</li> 
       <li style="font-weight: normal;">타임시트:default.timesheet.manual 역할(수동 제어 역할)</li> 
       <li style="font-weight: normal;">proof:defaultNonRecipientRole (config.proofhq.defaultnonrecipientrole) </li> 
       <li style="font-weight: normal;">proof:defaultNonRecipientGuestRole(config.proofhq.defaultnonrecipientguestrole)  </li> 
      </ul> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

### 문서 메타데이터 링크 그룹 {#docmetadatalinkgroup}

<table style="table-layout:auto"> 
 <col data-mc-conditions=""> 
 <col data-mc-conditions=""> 
 <tbody> 
  <tr> 
   <td>액션</td> 
   <td> 
    <ul> 
     <li style="font-weight: bold;"> <p>getMetadataDetailsForDocument</p> <p style="font-weight: normal;">추가됨</p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

### 문서 {#document}

Document 객체는 파일(예: 작성된 자료, 이미지 또는 기타 정보 형식)을 나타냅니다.

<table style="table-layout:auto"> 
 <col data-mc-conditions=""> 
 <col data-mc-conditions=""> 
 <tbody> 
  <tr> 
   <td>액션</td> 
   <td> <p>Document 객체에 다음과 같은 작업이 추가되었습니다.</p> 
    <ul> 
     <li style="font-weight: bold;">completeLargeDocument</li> 
     <li style="font-weight: bold;">createLargeDocument</li> 
     <li style="font-weight: bold;">createProofRest</li> 
     <li style="font-weight: bold;">getDocumentProofTemplate</li> 
     <li style="font-weight: bold;">getProofRecipients</li> 
     <li style="font-weight: bold;">getProofStages</li> 
     <li style="font-weight: bold;">getProofTemplate</li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

### 반복 {#iteration}

Iteration 객체는 단일 애자일 반복을 나타냅니다. 반복은 애자일 스토리를 계획하고 완료하는 데 사용되는 이산 기간입니다.

<table style="table-layout:auto"> 
 <col data-mc-conditions=""> 
 <col data-mc-conditions=""> 
 <tbody> 
  <tr> 
   <td>직접 필드</td> 
   <td> <p>다음 필드가 Iteration 개체에 추가되었습니다.</p> 
    <ul> 
     <li style="font-weight: bold;">원래 총점 수</li> 
     <li style="font-weight: bold;">포인트 완료됨</li> 
     <li style="font-weight: bold;">합계 포인트  </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

### 레이아웃 템플릿 {#layout-template}

레이아웃 템플릿 개체는 주 메뉴, 탐색 패널 또는 홈 영역과 같은 레이아웃 요소의 특정 배열을 나타냅니다. 레이아웃 템플릿을 사용자, 팀, 그룹 또는 작업 역할에 할당할 수 있습니다.

<table style="table-layout:auto"> 
 <col data-mc-conditions=""> 
 <col data-mc-conditions=""> 
 <tbody> 
  <tr> 
   <td>직접 필드</td> 
   <td> 
    <ul> 
     <li style="font-weight: bold;"> <p>showHomeTimestamp </p> <p style="font-weight: normal;">이 필드가 추가되었으며, 레이아웃 템플릿 이 작업 목록 및 달력의 기한 타임스탬프를 표시하도록 설정된 경우 true 값을 갖고, 타임스탬프를 숨기도록 설정된 경우 false 값을 갖는 부울 매개 변수입니다.  </p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>기본 필드</td> 
   <td> 
    <ul> 
     <li style="font-weight: bold;"> <p>showHomeTimestamp</p> <p style="font-weight: normal;">추가됨</p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

### 마일스톤 경로 {#milestonepath}

마일스톤은 프로젝트의 요점임을 나타내는 작업 표시의 표식입니다. 일반적으로 는 프로젝트의 단계 또는 중요한 활동 세트와 같은 중요한 이벤트를 표시하는 데 사용됩니다. MilestonePath 개체는 마일스톤의 컬렉션입니다.

<table style="table-layout:auto"> 
 <col data-mc-conditions=""> 
 <col data-mc-conditions=""> 
 <tbody> 
  <tr> 
   <td>직접 필드</td> 
   <td> 
    <ul> 
     <li style="font-weight: bold;"> <p>활성</p> <p style="font-weight: normal;">이 필드가 추가되었으며, 개체가 활성 상태이면 true 값을 갖고, 그렇지 않으면 false 값을 갖는 부울 매개 변수입니다. 활성으로 설정된 객체는 드롭다운 메뉴와 앞에 입력 필드에 나타나며 다른 객체에 첨부할 수 있습니다. 활성으로 설정되지 않은 객체는 다른 객체에 첨부할 드롭다운 메뉴와 자동 입력 필드에 표시되지 않습니다.  </p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>기본 필드</td> 
   <td> 
    <ul> 
     <li style="font-weight: bold;"> <p>활성</p> <p style="font-weight: normal;">추가됨</p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

### 참고 {#note}

Note 객체는 Workfront 객체에 대한 댓글 또는 업데이트입니다.

<table style="table-layout:auto"> 
 <col data-mc-conditions=""> 
 <col data-mc-conditions=""> 
 <tbody> 
  <tr> 
   <td>직접 필드</td> 
   <td> <p>Note 개체에 다음 필드가 추가되었습니다.</p> 
    <ul> 
     <li style="font-weight: bold;">proofID  </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>컬렉션 필드</td> 
   <td> 
    <ul> 
     <li style="font-weight: bold;"> <p>좋아요 수</p> <p style="font-weight: normal;">추가됨</p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

### OpTask {#optask}

OpTask 객체를 일반적으로 문제라고 합니다. 문제는 일반적으로 작업 또는 프로젝트의 완료를 방해하는 문제가 있음을 나타내는 작업 항목입니다. 문제는 헬프 데스크 요청일 수도 있습니다. 변경 주문, 요청 및 버그도 문제가 됩니다.

<table style="table-layout:auto"> 
 <col data-mc-conditions=""> 
 <col data-mc-conditions=""> 
 <tbody> 
  <tr> 
   <td colspan="2">직접 필드<p style="font-weight: normal;">다음 필드에는 AT_DATE_BEFORE_YEAR 및 AT_DATE_AFTER_YEAR 유효성 검사기가 추가되었습니다. 이러한 유효성 검사기는 연결된 오브젝트의 날짜를 1900년 이전 또는 2200년 이후로 설정할 수 없도록 지정합니다.</p>
    <ul>
     <li style="font-weight: bold;">실제 완료 일자</li>
     <li style="font-weight: bold;">actualStartDate</li>
     <li style="font-weight: bold;">계획된 완료 일자</li>
     <li style="font-weight: bold;">plannedStartDate</li>
    </ul><p style="font-weight: normal;">다음 필드가 OpTask에 추가되었습니다.</p>
    <ul>
     <li style="font-weight: bold;"><p>칸반 보드 ID </p><p style="font-weight: normal;">칸반 보드 개체의 고유한 Workfront ID입니다.</p></li>
     <li style="font-weight: bold;"><p>percentComplete</p><p style="font-weight: normal;">완료율은 완료된 문제 금액을 백분율로 반환하는 매개 변수입니다.</p></li>
     <li style="font-weight: bold;">storypoints</li>
     <li style="font-weight: bold;">작업  </li>
    </ul></td> 
  </tr> 
  <tr> 
   <td>컬렉션 필드</td> 
   <td> 
    <ul> 
     <li style="font-weight: bold;"> <p>allConditions</p> <p style="font-weight: normal;">추가됨</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>필드 검색</td> 
   <td> 
    <ul> 
     <li style="font-weight: bold;"> <p>작업</p> <p style="font-weight: normal;">제거됨</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>기본 필드</td> 
   <td> 
    <ul> 
     <li style="font-weight: bold;"> <p>percentComplete</p> <p style="font-weight: normal;">추가됨</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>액션</td> 
   <td> <p>다음 작업이 OpTask 개체에 추가되었습니다</p> 
    <ul> 
     <li style="font-weight: bold;">일괄 이동</li> 
     <li style="font-weight: bold;">copyIssue</li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

### 매개변수 {#parameter}

Parameter 개체는 사용자 지정 필드입니다.

<table style="table-layout:auto"> 
 <col data-mc-conditions=""> 
 <col data-mc-conditions=""> 
 <tbody> 
  <tr> 
   <td>직접 필드</td> 
   <td> 
    <ul> 
     <li style="font-weight: bold;"> <p>displayType</p> <p style="font-weight: normal;">가능한 값 TYAH(Typeahead)가 추가되었습니다.</p> </li> 
     <li style="font-weight: bold;"> <p>refObjCode </p> <p style="font-weight: normal;">이 필드가 추가되었으며 참조된 개체의 개체 코드를 참조합니다. 모든 개체의 개체 코드는 <a href="../../wf-api/general/api-explorer.md" class="MCXref xref">API 탐색기</a>에서 찾을 수 있습니다.  </p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

### Portfolio {#portfolio}

Portfolio 객체는 동일한 리소스(일반적으로 돈 또는 완료하는 사람)에 대해 경쟁하는 프로젝트의 컬렉션입니다.

<table style="table-layout:auto"> 
 <col data-mc-conditions=""> 
 <col data-mc-conditions=""> 
 <tbody> 
  <tr> 
   <td>직접 필드</td> 
   <td> 
    <ul> 
     <li style="font-weight: bold;"> <p>설명</p> <p style="font-weight: normal;">설명의 길이가 4000자를 넘지 않도록 지정하는 유효성 검사기 MAX_LENGTH가 추가되었습니다.</p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

### 프로그램 {#program}

프로그램 객체는 유사한 프로젝트를 함께 그룹화할 수 있는 포트폴리오 내의 하위 집합입니다.

<table style="table-layout:auto"> 
 <col data-mc-conditions=""> 
 <col data-mc-conditions=""> 
 <tbody> 
  <tr> 
   <td>직접 필드</td> 
   <td> 
    <ul> 
     <li style="font-weight: bold;"> <p>설명</p> <p style="font-weight: normal;">설명의 길이가 4000자를 넘지 않도록 지정하는 유효성 검사기 MAX_LENGTH가 추가되었습니다.</p> </li> 
     <li style="font-weight: bold;"> <p>활성</p> <p style="font-weight: normal;">이 필드가 추가되었으며, 개체가 활성 상태이면 true 값을 갖고, 그렇지 않으면 false 값을 갖는 부울 매개 변수입니다. 활성으로 설정된 객체는 드롭다운 메뉴와 앞에 입력 필드에 나타나며 다른 객체에 첨부할 수 있습니다. 활성으로 설정되지 않은 객체는 다른 객체에 첨부할 드롭다운 메뉴와 자동 입력 필드에 표시되지 않습니다.  </p> </li> 
     <li style="font-weight: bold;"> <p>이름 </p> <p style="font-weight: normal;">이름의 길이가 255자를 넘지 않도록 지정하는 유효성 검사기 MAX_LENGTH가 추가되었습니다.  </p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>기본 필드</td> 
   <td> 
    <ul> 
     <li style="font-weight: bold;"> <p>활성</p> <p style="font-weight: normal;">추가됨</p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

### 프로젝트 {#project}

프로젝트는 Workfront 내의 작업 항목이며 Workfront이 작업을 수행하는 데 도움을 주는 방식의 주요 빌딩 블록입니다. Project 개체는 일반적인 특정 목표를 가진 작업 그룹을 나타냅니다.

<table style="table-layout:auto"> 
 <col data-mc-conditions=""> 
 <col data-mc-conditions=""> 
 <tbody> 
  <tr> 
   <td colspan="2">직접 필드<p style="font-weight: normal;">다음 필드에는 AT_DATE_BEFORE_YEAR 및 AT_DATE_AFTER_YEAR 유효성 검사기가 추가되었습니다. 이러한 유효성 검사기는 연결된 오브젝트의 날짜를 1900년 이전 또는 2200년 이후로 설정할 수 없도록 지정합니다.</p>
    <ul>
     <li style="font-weight: bold;">실제 완료 일자</li>
     <li style="font-weight: bold;">actualStartDate</li>
     <li style="font-weight: bold;">계획된 완료 일자</li>
     <li style="font-weight: bold;">plannedStartDate</li>
    </ul><p style="font-weight: normal;">EAC(완료 시 추정) 계산의 투명성을 위해 공개 API에 다음 필드가 추가되었습니다.</p>
    <ul>
     <li><p style="font-weight: bold;">bcwp</p><p style="font-weight: normal;">성과 값이라고도 하는 BCWP(수행된 작업의 예산 비용)는 이 지표가 계산될 때 실제로 완료된 작업 금액의 예산 비용을 나타내는 프로젝트 성과 지표입니다. 작업의 경우 BCWP = 실제 완료율 x 작업 예산. 프로젝트의 경우 BCWP = SUM(모든 상위 및 개별 작업의 BCWP 값).</p></li>
     <li><p style="font-weight: bold;">bcws</p><p style="font-weight: normal;">계획된 값이라고도 하는 BCWS(Budgeted Cost of Work Scheduled)는 이 지표가 계산되는 시점에 완료해야 하는 작업 금액의 예산 비용을 나타내는 프로젝트 성과 지표입니다. 작업의 경우 BCWS = 계획된 완료율 x 작업 예산. 프로젝트의 경우 BCWS = SUM(모든 상위 및 개별 작업의 BCWS 값).</p></li>
    </ul><p style="font-weight: normal;">다음 필드에 CURRENCY 플래그가 추가되었습니다</p>
    <ul>
     <li style="font-weight: bold;">projectBudgetCost</li>
     <li style="font-weight: bold;">프로젝트 순 가치</li>
    </ul><p style="font-weight: normal;">다음 필드가 프로젝트 개체에서 제거되었습니다.</p>
    <ul>
     <li style="font-weight: bold;">timelineExceptionInfo</li>
    </ul></td> 
  </tr> 
  <tr> 
   <td>컬렉션 필드</td> 
   <td> 
    <ul> 
     <li style="font-weight: bold;"> <p>allConditions</p> <p style="font-weight: normal;">추가됨</p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

### ProofApproval {#proofapproval}

ProofApproval 객체는 증명에 직접 연결된 승인을 나타냅니다.

<table style="table-layout:auto"> 
 <col data-mc-conditions=""> 
 <col data-mc-conditions=""> 
 <tbody> 
  <tr> 
   <td>직접 필드</td> 
   <td> 
    <ul> 
     <li style="font-weight: bold;"> <p>isAwaitingDecision</p> <p style="font-weight: normal;">이 필드가 추가되었으며, 증명이 결정을 기다리는 경우 true 값을 갖고, 그렇지 않은 경우 false 값을 갖는 부울 매개 변수입니다.  </p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

### QueueDef {#queuedef}

QueueDef 개체는 사용자가 문제를 제출할 수 있도록 헬프 데스크 영역에 게시된 프로젝트인 Queue를 나타냅니다.

<table style="table-layout:auto"> 
 <col data-mc-conditions=""> 
 <col data-mc-conditions=""> 
 <tbody> 
  <tr> 
   <td>직접 필드</td> 
   <td> <p>다음 필드에 가능한 BUDGETING_INFORMATION 값이 추가되었습니다. 이를 통해 권한이 있는 사용자는 플래너에서 우선 순위 및 예산 시간을 편집할 수 있습니다.</p> 
    <ul> 
     <li style="font-weight: bold;">requestorCoreAction</li> 
     <li style="font-weight: bold;">requestorForbiddenActions</li> 
    </ul>  </td> 
  </tr> 
 </tbody> 
</table>

### 예약된 시간 {#reservedtime}

ReservedTime 개체는 사용자의 개인 시간에 지정된 일을 나타내며, 사용자가 작업에 사용할 수 없음을 나타냅니다.

ReservedTime 리소스가 REPORTABLE 플래그를 추가했습니다.

<table style="table-layout:auto"> 
 <col data-mc-conditions=""> 
 <col data-mc-conditions=""> 
 <tbody> 
  <tr> 
   <td>직접 필드</td> 
   <td> <p>다음 필드에서 NOT_GROUPABLE 플래그가 제거되었습니다.</p> 
    <ul> 
     <li style="font-weight: bold;">endDate</li> 
     <li style="font-weight: bold;">extRefID</li> 
     <li style="font-weight: bold;">startDate </li> 
    </ul> <p>다음 필드가 ReservedTime 개체에서 제거되었습니다.</p> 
    <ul> 
     <li style="font-weight: bold;">taskID</li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>참조 필드</td> 
   <td> 
    <ul> 
     <li style="font-weight: bold;"> <p>작업</p> <p style="font-weight: normal;">제거됨  </p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>작업</td> 
   <td> 
    <ul> 
     <li style="font-weight: bold;"> <p>편집</p> <p style="font-weight: normal;">추가됨</p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

### 리소스 플래너 필터 {#resourceplannerfilter}

ResourcePlannerFilter 객체는 리소스 플래너에 표시할 항목을 결정하는 규칙 세트입니다.

ResourcePlannerFilter 리소스가 SHARABLE 플래그를 추가했습니다. 오브젝트에 다른 변경 사항이 없습니다.

### 위험 {#risk}

위험 개체는 프로젝트가 정시 또는 예산 내에서 완료되지 않을 수 있는 가능한 이벤트를 나타냅니다. 작업 승인 전에 잠재적인 장애 요소를 식별하기 위해 계획 단계에서 프로젝트에 위험이 추가됩니다.

<table style="table-layout:auto"> 
 <col data-mc-conditions=""> 
 <col data-mc-conditions=""> 
 <tbody> 
  <tr> 
   <td>직접 필드</td> 
   <td> <p>위험 개체에 다음 필드가 추가되었습니다.</p> 
    <ul> 
     <li style="font-weight: bold;"> <p>입력자 ID</p> <p style="font-weight: normal;">원래 개체를 만든 사용자의 ID입니다.</p> </li> 
     <li> <p style="font-weight: bold;">entryDate</p> <p>Workfront에서 사용자가 개체를 제출한 날짜입니다.</p> </li> 
     <li> <p style="font-weight: bold;">마지막 업데이트 날짜</p> <p>마지막 업데이트 날짜 매개 변수는 개체에 마지막으로 업데이트한 날짜,</p> </li> 
     <li> <p style="font-weight: bold;">lastUpdatedByID </p> <p>Last Updated By ID는 개체를 업데이트한 마지막 사용자의 사용자 ID를 반환하는 매개 변수입니다.  </p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>참조 필드</td> 
   <td> <p style="font-weight: normal;">다음 참조 필드가 RIsk 개체에 추가되었습니다.</p> 
    <ul> 
     <li style="font-weight: bold;">입력한 사람</li> 
     <li style="font-weight: bold;">lastUpdatedBy  </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

### 예약된 보고서 {#scheduledreport}

ScheduledReport 개체는 전송을 위해 예약되도록 구성된 보고서를 나타냅니다.

<table style="table-layout:auto"> 
 <col data-mc-conditions=""> 
 <col data-mc-conditions=""> 
 <tbody> 
  <tr> 
   <td>직접 필드</td> 
   <td> 
    <ul> 
     <li style="font-weight: bold;"> <p>pageSize</p> <p style="font-weight: normal;">다음과 같은 가능한 값이 추가되었습니다.</p> 
      <ul> 
       <li style="font-weight: normal;">A2</li> 
       <li style="font-weight: normal;">A1</li> 
       <li style="font-weight: normal;">A0  </li> 
      </ul> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

### 스코어카드 질문 {#scorecardquestion}

ScoreCardQuestion 객체는 스코어카드에 추가된 질문을 나타냅니다. 이러한 질문은 일반적으로 Portfolio 관리자가 결정하며, 관리자는 이에 대한 답변을 통해 프로젝트가 포트폴리오의 목표에 얼마나 잘 부합하는지 파악할 수 있습니다.

<table style="table-layout:auto"> 
 <col data-mc-conditions=""> 
 <col data-mc-conditions=""> 
 <tbody> 
  <tr> 
   <td>직접 필드</td> 
   <td> 
    <ul> 
     <li style="font-weight: bold;"> <p>displayType</p> <p style="font-weight: normal;">가능한 값 TYAH(Typeahead)가 추가되었습니다.  </p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

### 작업 {#task}

작업 객체는 최종 목표 달성(프로젝트 완료)을 위한 단계로 수행해야 하는 작업 항목을 나타냅니다.

<table style="table-layout:auto"> 
 <col data-mc-conditions=""> 
 <col data-mc-conditions=""> 
 <tbody> 
  <tr> 
   <td colspan="2">직접 필드<p style="font-weight: normal;">다음 필드에는 AT_DATE_BEFORE_YEAR 및 AT_DATE_AFTER_YEAR 유효성 검사기가 추가되었습니다. 이러한 유효성 검사기는 연결된 오브젝트의 날짜를 1900년 이전 또는 2200년 이후로 설정할 수 없도록 지정합니다.</p>
    <ul>
     <li style="font-weight: bold;">실제 완료 일자</li>
     <li style="font-weight: bold;">actualStartDate</li>
     <li style="font-weight: bold;">constraintDate</li>
     <li style="font-weight: bold;">계획된 완료 일자</li>
     <li style="font-weight: bold;">plannedStartDate</li>
    </ul><p style="font-weight: normal;">EAC(완료 시 추정) 계산의 투명성을 위해 공개 API에 다음 필드가 추가되었습니다.</p>
    <ul>
     <li><p style="font-weight: bold;">bcwp</p><p style="font-weight: normal;">성과 값이라고도 하는 BCWP(수행된 작업의 예산 비용)는 이 지표가 계산될 때 실제로 완료된 작업 금액의 예산 비용을 나타내는 프로젝트 성과 지표입니다. 작업의 경우 BCWP = 실제 완료율 x 작업 예산. 프로젝트의 경우 BCWP = SUM(모든 상위 및 개별 작업의 BCWP 값).</p></li>
     <li><p style="font-weight: bold;">bcws</p><p style="font-weight: normal;">계획된 값이라고도 하는 BCWS(Budgeted Cost of Work Scheduled)는 이 지표가 계산되는 시점에 완료해야 하는 작업 금액의 예산 비용을 나타내는 프로젝트 성과 지표입니다. 작업의 경우 BCWS = 계획된 완료율 x 작업 예산. 프로젝트의 경우 BCWS = SUM(모든 상위 및 개별 작업의 BCWS 값).</p></li>
    </ul><p style="font-weight: normal;">다음 필드에 가능한 값 ET가 추가되었습니다. 이 값은 경과된 시간(월) 단위를 나타내며, 주말이나 공휴일에 관계없이 월을 나타냅니다.</p>
    <ul>
     <li style="font-weight: bold;">durationUnit</li>
     <li style="font-weight: bold;">workUnit</li>
    </ul><p style="font-weight: normal;">다음 필드가 작업 개체에서 제거되었습니다.</p>
    <ul>
     <li style="font-weight: bold;">예약된 시간 ID</li>
    </ul><p style="font-weight: normal;">다음 필드가 작업 개체에 추가되었습니다.</p>
    <ul>
     <li style="font-weight: bold;">storypoints</li>
    </ul></td> 
  </tr> 
  <tr> 
   <td>참조 필드</td> 
   <td> 
    <ul> 
     <li style="font-weight: bold;"> <p>reservedTime</p> <p style="font-weight: normal;">제거됨  </p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>컬렉션 필드</td> 
   <td> 
    <ul> 
     <li style="font-weight: bold;"> <p>allConditions</p> <p style="font-weight: normal;">추가됨</p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

### 팀 {#team}

팀 개체는 작업 항목에 할당할 수 있는 사용자 컬렉션입니다.

<table style="table-layout:auto"> 
 <col data-mc-conditions=""> 
 <col data-mc-conditions=""> 
 <tbody> 
  <tr> 
   <td>직접 필드</td> 
   <td> 
    <ul> 
     <li style="font-weight: bold;"> <p>애자일 견적 유형 </p> <p style="font-weight: normal;">이 필드는 팀 개체에 추가되었습니다. 애자일 예상 유형은 스토리의 작업 로드가 어떻게 추정되는지 결정합니다. 시간 단위로 예상하면 스토리에 추가되는 계획된 시간 수입니다. 포인트로 예상되는 경우 각 포인트는 포인트 설정 방법에 따라 스토리에 계획된 시간 수를 추가합니다(기본값은 8시간). 애자일 예상 유형의 가능한 값은 다음과 같습니다.</p> 
      <ul> 
       <li style="font-weight: normal;"> STORY_POINTS(스토리 포인트)</li> 
       <li style="font-weight: normal;">시간(시간)</li> 
       <li style="font-weight: normal;">LEGACY_POINTS(시간을 포인트로)  </li> 
      </ul> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

### 템플릿 {#template}

Template 객체는 프로젝트의 패턴을 나타냅니다. 템플릿에서 프로젝트를 생성하여 시간을 절약할 수 있습니다. 템플릿에는 팀 및 작업이 포함되어 있으며, 이 작업은 템플릿을 사용할 때 프로젝트에 복사됩니다.

<table style="table-layout:auto"> 
 <col data-mc-conditions=""> 
 <col data-mc-conditions=""> 
 <tbody> 
  <tr> 
   <td>직접 필드</td> 
   <td> 
    <ul> 
     <li style="font-weight: bold;"> <p>활성</p> <p style="font-weight: normal;">이 필드가 추가되었으며, 개체가 활성 상태이면 true 값을 갖고, 그렇지 않으면 false 값을 갖는 부울 매개 변수입니다. 활성으로 설정된 객체는 드롭다운 메뉴와 앞에 입력 필드에 나타나며 다른 객체에 첨부할 수 있습니다. 활성으로 설정되지 않은 객체는 다른 객체에 첨부할 드롭다운 메뉴와 자동 입력 필드에 표시되지 않습니다.  </p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>컬렉션 필드</td> 
   <td> 
    <ul> 
     <li style="font-weight: bold;"> <p>allPriorities</p> <p style="font-weight: normal;">추가됨</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>기본 필드</td> 
   <td> 
    <ul> 
     <li style="font-weight: bold;"> <p>활성</p> <p style="font-weight: normal;">추가됨</p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

### 템플릿 할당 {#templateassignment}

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">A TemplateAssignment object represents the connection between a Template and the User, Team, or Group it is assigned to.</p>
-->

<table style="table-layout:auto"> 
 <col data-mc-conditions=""> 
 <col data-mc-conditions=""> 
 <tbody> 
  <tr> 
   <td>직접 필드</td> 
   <td> 
    <ul> 
     <li style="font-weight: bold;"> <p>workUnit</p> <p style="font-weight: normal;">가능한 값 ET가 추가되었습니다. 이 값은 경과된 시간(월) 단위를 나타내며, 주말이나 공휴일에 관계없이 월을 나타냅니다.  </p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

### TemplateTask {#templatetask}

TemplateTask 개체는 Template의 일부인 작업을 나타냅니다. 템플릿 작업은 템플릿이 사용되는 프로젝트의 작업이 됩니다.

<table style="table-layout:auto"> 
 <col data-mc-conditions=""> 
 <col data-mc-conditions=""> 
 <tbody> 
  <tr> 
   <td>직접 필드</td> 
   <td> <p style="font-weight: normal;">다음 필드에 가능한 값 ET가 추가되었습니다. 이 값은 경과된 시간(월) 단위를 나타내며, 주말이나 공휴일에 관계없이 월을 나타냅니다.</p> 
    <ul> 
     <li style="font-weight: bold;">durationUnit</li> 
     <li style="font-weight: bold;">workUnit</li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>컬렉션 필드</td> 
   <td> 
    <ul> 
     <li style="font-weight: bold;"> <p>allPriorities</p> <p style="font-weight: normal;">추가됨</p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

### 타임시트 {#timesheet}

타임시트 오브젝트는 사용자가 작업, 프로젝트 및 오버헤드 시간 유형에 대한 실제 작업 시간을 입력할 수 있는 가상 타임카드를 나타냅니다.

<table style="table-layout:auto"> 
 <col data-mc-conditions=""> 
 <col data-mc-conditions=""> 
 <tbody> 
  <tr> 
   <td>코어 필드</td> 
   <td> 
    <ul> 
     <li style="font-weight: bold;"> <p>objCode</p> <p style="font-weight: normal;">제거됨</p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

### 업데이트 {#update}

Workfront의 작업 항목을 업데이트하여 사용자에게 현재 상태를 알릴 수 있습니다. Update 개체는 이러한 업데이트 중 하나를 나타냅니다. 업데이트는 사용자가 입력하거나 Workfront 시스템에서 만들 수 있습니다.

<table style="table-layout:auto"> 
 <col data-mc-conditions=""> 
 <col data-mc-conditions=""> 
 <tbody> 
  <tr> 
   <td>직접 필드</td> 
   <td> 
    <ul> 
     <li style="font-weight: bold;"> <p>updateType</p> <p style="font-weight: normal;">가능한 값 referenceObjectCustomData(enum.updatetypeenum.referenceobjectcustomdata)가 추가되었습니다.  </p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>쿼리</td> 
   <td> <p style="font-weight: normal;">다음 쿼리가 Update 개체에 추가되었습니다.</p> 
    <ul> 
     <li style="font-weight: bold;">objectUpdateMobile</li> 
     <li style="font-weight: bold;">updateThreadMobile</li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

<!--
<h3 data-mc-conditions="QuicksilverOrClassic.Draft mode" id="user">User</h3>
-->

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">A User object represents a person with an account in Workfront that can log in and interact with the system.</p>
-->

<table style="table-layout:auto"> <!--
  <col data-mc-conditions="QuicksilverOrClassic.Draft mode">
 --> <!--
  <col data-mc-conditions="QuicksilverOrClassic.Draft mode">
 --> 
 <tbody> 
  <tr> 
   <td>컬렉션 필드</td> 
   <td> 
    <ul> 
     <li style="font-weight: bold;"> <p>loginAs액세스 규칙</p> <p style="font-weight: normal;">추가됨</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>액션</td> 
   <td> <p style="font-weight: normal;">다음 작업이 User 개체에 추가되었습니다.</p> 
    <ul> 
     <li style="font-weight: bold;">hasGrantLoginAsAccess</li> 
     <li style="font-weight: bold;">isUseradmin</li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>쿼리</td> 
   <td> 
    <ul> 
     <li style="font-weight: bold;"> <p>userAdmin</p> <p style="font-weight: normal;">추가됨</p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

### UserNote {#usernote}

<table style="table-layout:auto"> 
 <col data-mc-conditions=""> 
 <col data-mc-conditions=""> 
 <tbody> 
  <tr> 
   <td>액션</td> 
   <td> <p style="font-weight: normal;">다음 작업이 User 개체에 추가되었습니다.</p> 
    <ul> 
     <li style="font-weight: bold;">acknowledgementMyNotifications</li> 
     <li style="font-weight: bold;">unacknowledgedAllObjectsTypeCount  </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>쿼리</td> 
   <td> 
    <ul> 
     <li style="font-weight: bold;"> <p>myAllObjectTypesUnreadNotifications</p> <p style="font-weight: normal;">추가됨</p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

### 작업  {#work}

Work 개체는 Task와 OpTask가 모두 상속하는 공통 인터페이스이며 두 개체 간에 공통 코드를 공유합니다.

<table style="table-layout:auto"> 
 <col data-mc-conditions=""> 
 <col data-mc-conditions=""> 
 <tbody> 
  <tr> 
   <td colspan="2">직접 필드<p style="font-weight: normal;">다음 필드에는 AT_DATE_BEFORE_YEAR 및 AT_DATE_AFTER_YEAR 유효성 검사기가 추가되었습니다. 이러한 유효성 검사기는 연결된 오브젝트의 날짜를 1900년 이전 또는 2200년 이후로 설정할 수 없도록 지정합니다.</p>
    <ul>
     <li style="font-weight: bold;">실제 완료 일자</li>
     <li style="font-weight: bold;">actualStartDate</li>
     <li style="font-weight: bold;">constraintDate</li>
     <li style="font-weight: bold;">계획된 완료 일자</li>
     <li style="font-weight: bold;">plannedStartDate</li>
    </ul><p style="font-weight: normal;">EAC(완료 시 추정) 계산의 투명성을 위해 공개 API에 다음 필드가 추가되었습니다.</p>
    <ul>
     <li><p style="font-weight: bold;">bcwp</p><p style="font-weight: normal;">성과 값이라고도 하는 BCWP(수행된 작업의 예산 비용)는 이 지표가 계산될 때 실제로 완료된 작업 금액의 예산 비용을 나타내는 프로젝트 성과 지표입니다. 작업의 경우 BCWP = 실제 완료율 x 작업 예산. 프로젝트의 경우 BCWP = SUM(모든 상위 및 개별 작업의 BCWP 값).</p></li>
     <li><p style="font-weight: bold;">bcws</p><p style="font-weight: normal;">계획된 값이라고도 하는 BCWS(Budgeted Cost of Work Scheduled)는 이 지표가 계산되는 시점에 완료해야 하는 작업 금액의 예산 비용을 나타내는 프로젝트 성과 지표입니다. 작업의 경우 BCWS = 계획된 완료율 x 작업 예산. 프로젝트의 경우 BCWS = SUM(모든 상위 및 개별 작업의 BCWS 값).</p></li>
    </ul><p style="font-weight: normal;">다음 필드에 가능한 값 ET가 추가되었습니다. 이 값은 경과된 시간(월) 단위를 나타내며, 주말이나 공휴일에 관계없이 월을 나타냅니다.</p>
    <ul>
     <li style="font-weight: bold;">durationUnit</li>
     <li style="font-weight: bold;">workUnit</li>
    </ul><p style="font-weight: normal;">다음 필드가 작업 오브젝트에서 제거되었습니다.</p>
    <ul>
     <li style="font-weight: bold;">예약된 시간 ID</li>
    </ul><p style="font-weight: normal;">다음 필드가 Work 개체에 추가되었습니다.</p>
    <ul>
     <li style="font-weight: bold;">storypoints</li>
    </ul></td> 
  </tr> 
  <tr> 
   <td>참조 필드</td> 
   <td> 
    <ul> 
     <li style="font-weight: bold;"> <p>reservedTime</p> <p style="font-weight: normal;">제거됨  </p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>컬렉션 필드</td> 
   <td> 
    <ul> 
     <li style="font-weight: bold;"> <p>allConditions</p> <p style="font-weight: normal;">추가됨</p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>
