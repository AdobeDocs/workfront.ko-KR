---
content-type: api
navigation-topic: api-navigation-topic
title: API 버전 11의 새로운 기능
description: ReporttableBudgedHour가 Reporting을 위한 리소스로 Adobe Workfront API에 추가되었습니다. BudgetHour에 없는 참조 필드, 핵심 필드 및 기본 필드를 제공합니다.
author: John
feature: Workfront API
exl-id: b8826dc6-9791-49f6-923d-5a0c5392a8b0
source-git-commit: f2f825280204b56d2dc85efc7a315a4377e551c7
workflow-type: tm+mt
source-wordcount: '3600'
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

* [ReporttableScheduledHour](#reportablebudgetedhour)

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
     <li style="font-weight: bold;">accessorID</li> 
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
   <td>핵심 필드</td> 
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
   <td>핵심 필드</td> 
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
     <li style="font-weight: bold;">licenseTypes</li> 
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
   <td>핵심 필드</td> 
   <td> 
    <ul> 
     <li style="font-weight: bold;">ID</li> 
     <li style="font-weight: bold;">objCode</li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

### ReporttableScheduledHour {#reportablebudgetedhour}

ReporttableBudgedHour가 Reporting을 위한 리소스로 Adobe Workfront API에 추가되었습니다. BudgetHour에 없는 참조 필드, 핵심 필드 및 기본 필드를 제공합니다.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>직접 필드</td> 
   <td> 
    <ul> 
     <li> <p style="font-weight: bold;">allocationDate </p> <p>배부 일자는 Resource Planner에서 시간 예산을 책정한 주의 첫 번째 날(일요일)입니다.</p> </li> 
     <li> <p style="font-weight: bold;">backgroundHours </p> <p>예산책정된 시간은 자원 관리자가 프로젝트에서 자원을 완료해야 하는 작업에 대한 예산입니다</p> </li> 
     <li> <p style="font-weight: bold;">ID </p> <p>특정 Reportable Scheduled Hour 개체에 지정된 고유한 Workfront ID입니다.</p> </li> 
     <li style="font-weight: bold;">planningScheduledHours </li> 
     <li> <p style="font-weight: bold;">projectID </p> <p>특정 프로젝트에 지정된 고유한 Workfront ID입니다.</p> </li> 
     <li> <p style="font-weight: bold;">roleID</p> <p>특정 작업 역할에 지정된 고유한 Workfront ID입니다.</p> </li> 
     <li> <p style="font-weight: bold;">userID</p> <p>특정 사용자에게 할당된 고유한 Workfront ID입니다.</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>참조 필드</td> 
   <td> 
    <ul> 
     <li> <p style="font-weight: bold;">프로젝트</p> <p>ReportableScheduledHour가 연결된 프로젝트입니다.</p> </li> 
     <li> <p style="font-weight: bold;">역할</p> <p>ReportableScheduledHour가 연결된 작업 역할입니다.</p> </li> 
     <li> <p style="font-weight: bold;">사용자</p> <p>ReporttableScheduledHour가 연결된 사용자입니다.</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>핵심 필드</td> 
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
     <li style="font-weight: bold;">카운트</li> 
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
     <li><a href="#approvalpath" class="MCXref xref">ApprovalPath</a> </li> 
     <li><a href="#approvalprocess" class="MCXref xref">승인 프로세스</a> </li> 
     <li><a href="#assignment" class="MCXref xref">할당</a> </li> 
     <li><a href="#baselinetask" class="MCXref xref">초기 계획 작업</a> </li> 
     <li><a href="#category" class="MCXref xref">범주</a> </li> 
     <li><a href="#company" class="MCXref xref">회사</a> </li> 
     <li><a href="#customenum" class="MCXref xref">CustomEnum</a> </li> 
     <li><a href="#customer" class="MCXref xref">고객</a> </li> 
     <li><a href="#customerpreferences" class="MCXref xref">고객 기본 설정</a> </li> 
    </ul> </td> 
   <td> 
    <ul> 
     <li><a href="#docmetadatalinkgroup" class="MCXref xref">DocMetadataLinkGroup</a> </li> 
     <li><a href="#document" class="MCXref xref">문서</a> </li> 
     <li><a href="#iteration" class="MCXref xref">반복</a> </li> 
     <li><a href="#layout-template" class="MCXref xref">레이아웃 템플릿</a> </li> 
     <li><a href="#milestonepath" class="MCXref xref">이정표 경로</a> </li> 
     <li><a href="#note" class="MCXref xref">참고</a> </li> 
     <li><a href="#optask" class="MCXref xref">OpTask</a> </li> 
     <li><a href="#parameter" class="MCXref xref">매개변수</a> </li> 
     <li><a href="#portfolio" class="MCXref xref">포트폴리오</a> </li> 
     <li><a href="#program" class="MCXref xref">프로그램</a> </li> 
     <li><a href="#project" class="MCXref xref">프로젝트</a> </li> 
     <li><a href="#proofapproval" class="MCXref xref">증명 승인</a> </li> 
     <li><a href="#queuedef" class="MCXref xref">QueueDef</a> </li> 
     <li><a href="#reservedtime" class="MCXref xref">ReservedTime</a> </li> 
    </ul> </td> 
   <td> 
    <ul> 
     <li><a href="#resourceplannerfilter" class="MCXref xref">리소스 플래너필터</a> </li> 
     <li><a href="#risk" class="MCXref xref">위험</a> </li> 
     <li><a href="#scheduledreport" class="MCXref xref">예약된 보고서</a> </li> 
     <li><a href="#scorecardquestion" class="MCXref xref">ScoreCardQuestion</a> </li> 
     <li><a href="#task" class="MCXref xref">작업</a> </li> 
     <li><a href="#team" class="MCXref xref">팀</a> </li> 
     <li><a href="#template" class="MCXref xref">템플릿</a> </li> 
     <li><a href="#templateassignment" class="MCXref xref">TemplateAssignment</a> </li> 
     <li><a href="#templatetask" class="MCXref xref">TemplateTask</a> </li> 
     <li><a href="#timesheet" class="MCXref xref">타임시트</a> </li> 
     <li><a href="#update" class="MCXref xref"></a> 업데이트 </li> <!--
      <li data-mc-conditions="QuicksilverOrClassic.Draft mode"><a href="#user" class="MCXref xref">User</a> </li>
     --> 
     <li><a href="#usernote" class="MCXref xref">UserNote</a> </li> 
     <li><a href="#work" class="MCXref xref">작업 </a> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

 

### AccessLevelPermissions {#accesslevelpermissions}

AccessLevelPermissions 개체는 사용 권한 집합을 나타냅니다. 그런 다음 이 권한 집합을 액세스 수준과 연결할 수 있습니다.

<table style="table-layout:auto"> 
 <col data-mc-conditions=""> 
 <col data-mc-conditions=""> 
 <tbody> 
  <tr> 
   <td>직접 필드</td> 
   <td> <p>다음 필드에 가능한 값 BUDGETING_INFORMATION이 추가되었습니다. 이를 통해 사용자가 계획자에서 우선순위 및 예산 시간을 편집할 수 있습니다.</p> 
    <ul> 
     <li style="font-weight: bold;">coreAction</li> 
     <li style="font-weight: bold;">forbiddenActions</li> 
     <li style="font-weight: bold;">secondaryActions  </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

### AccessRequest {#accessrequest}

사용자에게 필요한 Workfront의 객체에 대한 액세스 권한이 없는 경우 해당 객체에 대한 액세스를 요청할 수 있습니다. AccessRequest 개체는 이 요청을 나타냅니다.

<table style="table-layout:auto"> 
 <col data-mc-conditions=""> 
 <col data-mc-conditions=""> 
 <tbody> 
  <tr> 
   <td>직접 필드</td> 
   <td> 
    <ul> 
     <li> <p style="font-weight: bold;">작업</p> <p>가능한 값 BUDGETING_INFORMATION을 추가했습니다. 이를 통해 사용자가 계획자에서 우선순위 및 예산 시간을 편집할 수 있습니다.  </p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

### AccessRule {#accessrule}

AccessRule 개체는 사용자가 만드는 프로젝트를 공유할 수 있는 방법을 결정하는 사용자 지정 액세스 수준의 규칙 세트를 나타냅니다.

<table style="table-layout:auto"> 
 <col data-mc-conditions=""> 
 <col data-mc-conditions=""> 
 <tbody> 
  <tr> 
   <td>직접 필드</td> 
   <td> <p>다음 필드에 가능한 값 BUDGETING_INFORMATION이 추가되었습니다. 이를 통해 사용자가 계획자에서 우선순위 및 예산 시간을 편집할 수 있습니다.</p> 
    <ul> 
     <li style="font-weight: bold;">coreAction</li> 
     <li style="font-weight: bold;">forbiddenActions</li> 
     <li style="font-weight: bold;">secondaryActions  </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

### 승인 {#approval}

작업, 문서 또는 작업표와 같은 특정 작업 항목에서는 감독자나 다른 사용자가 작업 항목에 대해 로그오프해야 할 수 있습니다. Approval 객체는 작업 항목에 대해 로그오프하는 작업을 나타냅니다.

<table style="table-layout:auto"> 
 <col data-mc-conditions=""> 
 <col data-mc-conditions=""> 
 <tbody> 
  <tr> 
   <td colspan="2">직접 필드<p style="font-weight: normal;">다음 필드에 AT_DATE_BEFORE_YEAR 및 AT_DATE_AFTER_YEAR가 추가되었습니다. 이러한 유효성 검사기는 연결된 개체의 날짜를 1900년 전이나 2200년 이후에 설정할 수 없도록 지정합니다.</p>
    <ul>
     <li style="font-weight: bold;">actualCompletionDate</li>
     <li style="font-weight: bold;">actualStartDate</li>
     <li style="font-weight: bold;">constraintDate</li>
     <li style="font-weight: bold;">planningCompletionDate</li>
     <li style="font-weight: bold;">planningStartDate</li>
    </ul><p style="font-weight: normal;">EAC(완료 시 예상) 계산을 수행할 때 투명성을 위해 공개 API에 다음 필드가 추가되었습니다.</p>
    <ul>
     <li><p style="font-weight: bold;">bwp</p><p style="font-weight: normal;">BCWP(Backed Cost of Work Performed)라고도 하는 Earned Value는 이 지표가 계산될 때 실제로 완료된 작업의 금액의 예산책정된 비용을 나타내는 프로젝트 성과 지표입니다. 작업의 경우 BCWP = 실제 완료 퍼센트 x 작업 예산입니다. 프로젝트의 경우 BCWP = SUM(모든 상위 및 개별 작업의 BCWP 값)입니다.</p></li>
     <li><p style="font-weight: bold;">bcws</p><p style="font-weight: normal;">계획 값이라고도 하는 BCWS(Scheduled Cost of Work Scheduled)는 이 지표가 계산될 때 완료했어야 하는 작업의 금액의 예산책정된 비용을 나타내는 프로젝트 성과 지표입니다. 작업의 경우 BCWS = 계획 완료 퍼센트 x 작업 예산입니다. 프로젝트의 경우 BCWS = SUM(모든 상위 작업과 개별 작업의 BCWS 값).</p></li>
    </ul><p style="font-weight: normal;">다음 필드에 가능한 값 ET가 추가되었습니다. 이 값은 주말 또는 휴일에 상관 없이 월을 참조하는 경과 개월 단위를 나타냅니다.</p>
    <ul>
     <li style="font-weight: bold;">durationUnit</li>
     <li style="font-weight: bold;">workUnit</li>
    </ul><p style="font-weight: normal;">다음 필드에 플래그 CURRENCY가 추가되었습니다</p>
    <ul>
     <li style="font-weight: bold;">projectBudgetCost</li>
     <li style="font-weight: bold;">projectNetValue</li>
    </ul><p style="font-weight: normal;">Approval 개체에서 다음 필드가 제거되었습니다.</p>
    <ul>
     <li style="font-weight: bold;">reservedTimeID</li>
     <li style="font-weight: bold;">timelineExceptionInfo</li>
    </ul><p style="font-weight: normal;">Approval 개체에 다음 필드가 추가되었습니다.</p>
    <ul>
     <li style="font-weight: bold;">storyPoints</li>
    </ul></td> 
  </tr> 
  <tr> 
   <td>참조 필드</td> 
   <td> 
    <ul> 
     <li style="font-weight: bold;"> <p>reservedTime</p> <p style="font-weight: normal;">Approval 개체에서 제거됨  </p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>컬렉션 필드</td> 
   <td> 
    <ul> 
     <li style="font-weight: bold;"> <p>allConditions</p> <p style="font-weight: normal;">승인 개체에 가 추가되었습니다.</p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

### ApprovalPath {#approvalpath}

ApprovalPath 객체는 승인 프로세스 내의 분기입니다. 승인 경로는 승인 프로세스와 연관된 객체의 상태를 기반으로 합니다.

<table style="table-layout:auto"> 
 <col data-mc-conditions=""> 
 <col data-mc-conditions=""> 
 <tbody> 
  <tr> 
   <td>직접 필드</td> 
   <td> 
    <ul> 
     <li style="font-weight: bold;"> <p>durationUnit </p> <p style="font-weight: normal;">가능한 값 ET가 추가되었습니다. 이 값은 주말 또는 휴일에 상관 없이 월을 참조하는 경과 개월 단위를 나타냅니다.  </p> </li> 
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
     <li style="font-weight: bold;"> <p>isActive</p> <p style="font-weight: normal;">이 필드가 추가되었으며 개체가 활성 상태인 경우 true 값을 가지는 부울 매개 변수입니다. 그렇지 않으면 false 값을 갖습니다. 활성(Active)으로 설정된 객체는 드롭다운 메뉴 및 미리 입력 필드에 표시되며 다른 객체에 첨부할 수 있습니다. 활성으로 설정되지 않은 객체는 드롭다운 메뉴에 표시되지 않으며 다른 객체에 첨부할 미리 입력 필드는 표시되지 않습니다.  </p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>기본 필드</td> 
   <td> 
    <ul> 
     <li style="font-weight: bold;"> <p>isActive</p> <p style="font-weight: normal;">추가됨</p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

### 할당 {#assignment}

할당 객체는 작업 항목과 작업 항목에 지정된 사용자, 팀 또는 그룹 간의 연결을 나타냅니다.

<table style="table-layout:auto"> 
 <col data-mc-conditions=""> 
 <col data-mc-conditions=""> 
 <tbody> 
  <tr> 
   <td>직접 필드</td> 
   <td> 
    <ul> 
     <li style="font-weight: bold;"> <p>workUnit </p> <p style="font-weight: normal;">가능한 값 ET가 추가되었습니다. 이 값은 주말 또는 휴일에 상관 없이 월을 참조하는 경과 개월 단위를 나타냅니다.  </p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

### 초기 계획 작업 {#baselinetask}

기준선은 주어진 순간에 프로젝트 성능이 어떻게 보였는지에 대한 스냅샷입니다. 주요 날짜, 진행 상황, 비용 및 수익 값과 같은 프로젝트 관련 주요 정보를 저장합니다. 베이스라인을 생성하면 해당 베이스라인의 베이스라인 작업에도 작업 정보가 캡처됩니다.

<table style="table-layout:auto"> 
 <col data-mc-conditions=""> 
 <col data-mc-conditions=""> 
 <tbody> 
  <tr> 
   <td>직접 필드</td> 
   <td> 
    <ul> 
     <li style="font-weight: bold;"> <p>durationUnit </p> <p style="font-weight: normal;">가능한 값 ET가 추가되었습니다. 이 값은 주말 또는 휴일에 상관 없이 월을 참조하는 경과 개월 단위를 나타냅니다.  </p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

### 범주 {#category}

Category 개체는 사용자 지정 양식입니다. 이 객체에 대한 보고서를 작성할 수 있으며, 다른 객체 보고서에도 표시할 수 있습니다.

<table style="table-layout:auto"> 
 <col data-mc-conditions=""> 
 <col data-mc-conditions=""> 
 <tbody> 
  <tr> 
   <td>직접 필드</td> 
   <td> 
    <ul> 
     <li style="font-weight: bold;"> <p>isActive</p> <p style="font-weight: normal;">이 필드가 추가되었으며 개체가 활성 상태인 경우 true 값을 가지는 부울 매개 변수입니다. 그렇지 않으면 false 값을 갖습니다. 활성(Active)으로 설정된 객체는 드롭다운 메뉴 및 미리 입력 필드에 표시되며 다른 객체에 첨부할 수 있습니다. 활성으로 설정되지 않은 객체는 드롭다운 메뉴에 표시되지 않으며 다른 객체에 첨부할 미리 입력 필드는 표시되지 않습니다.  </p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>기본 필드</td> 
   <td> 
    <ul> 
     <li style="font-weight: bold;"> <p>isActive</p> <p style="font-weight: normal;">추가됨</p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

### 회사 {#company}

회사 객체는 사람 컬렉션으로 구성된 조직을 나타냅니다. 회사는 사용자 또는 프로젝트와 연결됩니다.

<table style="table-layout:auto"> 
 <col data-mc-conditions=""> 
 <col data-mc-conditions=""> 
 <tbody> 
  <tr> 
   <td>직접 필드</td> 
   <td> 
    <ul> 
     <li style="font-weight: bold;"> <p>isActive</p> <p style="font-weight: normal;">이 필드가 추가되었으며 개체가 활성 상태인 경우 true 값을 가지는 부울 매개 변수입니다. 그렇지 않으면 false 값을 갖습니다. 활성(Active)으로 설정된 객체는 드롭다운 메뉴 및 미리 입력 필드에 표시되며 다른 객체에 첨부할 수 있습니다. 활성으로 설정되지 않은 객체는 드롭다운 메뉴에 표시되지 않으며 다른 객체에 첨부할 미리 입력 필드는 표시되지 않습니다.  </p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>기본 필드</td> 
   <td> 
    <ul> 
     <li style="font-weight: bold;"> <p>isActive</p> <p style="font-weight: normal;">추가됨</p> </li> 
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
   <td> <p>다음 쿼리가 CustomEnum 개체에 추가되었습니다</p> 
    <ul> 
     <li style="font-weight: bold;">opTaskConditions</li> 
     <li style="font-weight: bold;">projectConditions</li> 
     <li style="font-weight: bold;">taskConditions</li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

### 고객 {#customer}

고객 개체는 Workfront 인스턴스를 사용하는 조직을 나타냅니다.

<table style="table-layout:auto"> 
 <col data-mc-conditions=""> 
 <col data-mc-conditions=""> 
 <tbody> 
  <tr data-mc-conditions=""> 
   <td>직접 필드</td> 
   <td> 
    <ul> 
     <li style="font-weight: bold;"> <p>customEnumTypes</p> <p style="font-weight: normal;">가능한 값을 추가했습니다. </p> 
      <ul> 
       <li style="font-weight: normal;">CONDITION_PROJ(프로젝트 조건)</li> 
       <li style="font-weight: normal;">CONDITION_TASK(작업 조건)</li> 
       <li style="font-weight: normal;">CONDITION_OPTASK(문제 조건)  </li> 
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
   <td> <p style="font-weight: normal;">다음 작업이 고객 개체에 추가되었습니다</p> 
    <ul> 
     <li style="font-weight: bold;">goalsEnabled</li> 
     <li style="font-weight: bold;">updateLoginAsSettings</li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

### 고객 기본 설정 {#customerpreferences}

CustomerPreferences 개체는 고객이 Workfront 인스턴스에 대해 설정한 환경 설정 집합을 나타냅니다.

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
     <li style="font-weight: bold;"> <p>이름</p> <p style="font-weight: normal;">가능한 값을 추가했습니다.</p> 
      <ul> 
       <li style="font-weight: normal;">password:password.eauthPolicy(암호 복잡성 요구 사항)</li> 
       <li style="font-weight: normal;"> password:password.minimumLength(최소 암호 길이)</li> 
       <li style="font-weight: normal;">password:mobileSessionTimeout (모바일 세션 시간 초과)</li> 
       <li style="font-weight: normal;"> project.mgmt:default.project.usertimeoff(사용자 시간 초과)</li> 
       <li style="font-weight: normal;">작업표:default.작업표.manualrole(수동 제어 역할)</li> 
       <li style="font-weight: normal;">증명:defaultNonRecipientRole(config.proohq.defaultnonrecipientrole) </li> 
       <li style="font-weight: normal;">증명:defaultNonRecipientGuestRole(config.proohq.defaultnonrecipientguestrole)  </li> 
      </ul> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

### DocMetadataLinkGroup {#docmetadatalinkgroup}

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

Document 객체는 문서 자료, 이미지 또는 기타 정보 유형과 같은 파일을 나타냅니다.

<table style="table-layout:auto"> 
 <col data-mc-conditions=""> 
 <col data-mc-conditions=""> 
 <tbody> 
  <tr> 
   <td>액션</td> 
   <td> <p>다음 작업이 Document 객체에 추가되었습니다.</p> 
    <ul> 
     <li style="font-weight: bold;">completeLargeDocument</li> 
     <li style="font-weight: bold;">createLargeDocument</li> 
     <li style="font-weight: bold;">createProofRest</li> 
     <li style="font-weight: bold;">getDocumentProofTemplate</li> 
     <li style="font-weight: bold;">getProofRecipients</li> 
     <li style="font-weight: bold;">getProofStage</li> 
     <li style="font-weight: bold;">getProofTemplate</li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

### 반복 {#iteration}

반복 객체는 단일 애자일 반복을 나타냅니다. 반복은 Agile 스토리를 계획하고 완료하는 데 사용되는 개별 기간입니다.

<table style="table-layout:auto"> 
 <col data-mc-conditions=""> 
 <col data-mc-conditions=""> 
 <tbody> 
  <tr> 
   <td>직접 필드</td> 
   <td> <p>다음 필드가 반복 개체에 추가되었습니다.</p> 
    <ul> 
     <li style="font-weight: bold;">originalTotalPoints</li> 
     <li style="font-weight: bold;">완료됨</li> 
     <li style="font-weight: bold;">totalPoints  </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

### 레이아웃 템플릿 {#layout-template}

레이아웃 템플릿 개체는 기본 메뉴, 탐색 패널 또는 홈 영역과 같은 레이아웃 요소의 특정 배열을 나타냅니다. 레이아웃 템플릿은 사용자, 팀, 그룹 또는 작업 역할에 할당할 수 있습니다.

<table style="table-layout:auto"> 
 <col data-mc-conditions=""> 
 <col data-mc-conditions=""> 
 <tbody> 
  <tr> 
   <td>직접 필드</td> 
   <td> 
    <ul> 
     <li style="font-weight: bold;"> <p>showHomeTimestamps </p> <p style="font-weight: normal;">이 필드가 추가되었으며, 작업 목록 및 달력에 기한 날짜에 대한 타임스탬프를 표시하도록 레이아웃 템플릿을 설정하고 타임스탬프를 숨기도록 설정하면 false 값을 갖는 부울 매개 변수입니다.  </p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>기본 필드</td> 
   <td> 
    <ul> 
     <li style="font-weight: bold;"> <p>showHomeTimestamps</p> <p style="font-weight: normal;">추가됨</p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

### 이정표 경로 {#milestonepath}

이정표는 프로젝트에서 중요한 지점임을 나타내는 작업 표시에서의 마커입니다. 일반적으로 프로젝트의 단계 완료 또는 중요한 활동 세트와 같은 중요한 이벤트를 나타내는 데 사용됩니다. MilestonesPath 개체는 이정표의 컬렉션입니다.

<table style="table-layout:auto"> 
 <col data-mc-conditions=""> 
 <col data-mc-conditions=""> 
 <tbody> 
  <tr> 
   <td>직접 필드</td> 
   <td> 
    <ul> 
     <li style="font-weight: bold;"> <p>isActive</p> <p style="font-weight: normal;">이 필드가 추가되었으며 개체가 활성 상태인 경우 true 값을 가지는 부울 매개 변수입니다. 그렇지 않으면 false 값을 갖습니다. 활성(Active)으로 설정된 객체는 드롭다운 메뉴 및 미리 입력 필드에 표시되며 다른 객체에 첨부할 수 있습니다. 활성으로 설정되지 않은 객체는 드롭다운 메뉴에 표시되지 않으며 다른 객체에 첨부할 미리 입력 필드는 표시되지 않습니다.  </p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>기본 필드</td> 
   <td> 
    <ul> 
     <li style="font-weight: bold;"> <p>isActive</p> <p style="font-weight: normal;">추가됨</p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

### 참고 {#note}

Note 객체는 Workfront 객체에 대한 주석 또는 업데이트입니다.

<table style="table-layout:auto"> 
 <col data-mc-conditions=""> 
 <col data-mc-conditions=""> 
 <tbody> 
  <tr> 
   <td>직접 필드</td> 
   <td> <p>다음 필드가 Note 개체에 추가되었습니다.</p> 
    <ul> 
     <li style="font-weight: bold;">proofID  </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>컬렉션 필드</td> 
   <td> 
    <ul> 
     <li style="font-weight: bold;"> <p>좋아요</p> <p style="font-weight: normal;">추가됨</p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

### OpTask {#optask}

일반적으로 OpTask 개체를 Issue라고 합니다. 문제는 일반적으로 작업 또는 프로젝트 완료를 방지하는 데 문제가 있음을 나타내는 작업 항목입니다. 헬프데스크 요청도 있습니다. 변경 주문, 요청 및 버그도 문제입니다.

<table style="table-layout:auto"> 
 <col data-mc-conditions=""> 
 <col data-mc-conditions=""> 
 <tbody> 
  <tr> 
   <td colspan="2">직접 필드<p style="font-weight: normal;">다음 필드에 AT_DATE_BEFORE_YEAR 및 AT_DATE_AFTER_YEAR가 추가되었습니다. 이러한 유효성 검사기는 연결된 개체의 날짜를 1900년 전이나 2200년 이후에 설정할 수 없도록 지정합니다.</p>
    <ul>
     <li style="font-weight: bold;">actualCompletionDate</li>
     <li style="font-weight: bold;">actualStartDate</li>
     <li style="font-weight: bold;">planningCompletionDate</li>
     <li style="font-weight: bold;">planningStartDate</li>
    </ul><p style="font-weight: normal;">다음 필드가 OpTask에 추가되었습니다.</p>
    <ul>
     <li style="font-weight: bold;"><p>간판ID </p><p style="font-weight: normal;">간판 보드 객체의 고유한 Workfront ID입니다.</p></li>
     <li style="font-weight: bold;"><p>percentComplete</p><p style="font-weight: normal;">완료율은 완료된 문제 금액을 백분율로 반환하는 매개변수입니다.</p></li>
     <li style="font-weight: bold;">storyPoints</li>
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
     <li style="font-weight: bold;">bulkMove</li> 
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
     <li style="font-weight: bold;"> <p>refObjCode </p> <p style="font-weight: normal;">이 필드가 추가되었으며 참조된 개체의 개체 코드를 참조합니다. 모든 개체의 개체 코드는 <a href="../../wf-api/general/api-explorer.md" class="MCXref xref">API 탐색기</a>.  </p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

### 포트폴리오 {#portfolio}

Portfolio 객체는 일반적으로 동일한 리소스, 즉 완료 비용 또는 사람에 대해 경쟁하는 프로젝트 컬렉션입니다.

<table style="table-layout:auto"> 
 <col data-mc-conditions=""> 
 <col data-mc-conditions=""> 
 <tbody> 
  <tr> 
   <td>직접 필드</td> 
   <td> 
    <ul> 
     <li style="font-weight: bold;"> <p>설명</p> <p style="font-weight: normal;">설명 길이가 4000자를 넘지 않도록 지정하는 유효성 검사기 MAX_LENGTH가 추가되었습니다.</p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

### 프로그램 {#program}

Program 객체는 유사한 프로젝트를 함께 그룹화할 수 있는 포트폴리오 내의 하위 집합입니다.

<table style="table-layout:auto"> 
 <col data-mc-conditions=""> 
 <col data-mc-conditions=""> 
 <tbody> 
  <tr> 
   <td>직접 필드</td> 
   <td> 
    <ul> 
     <li style="font-weight: bold;"> <p>설명</p> <p style="font-weight: normal;">설명 길이가 4000자를 넘지 않도록 지정하는 유효성 검사기 MAX_LENGTH가 추가되었습니다.</p> </li> 
     <li style="font-weight: bold;"> <p>isActive</p> <p style="font-weight: normal;">이 필드가 추가되었으며 개체가 활성 상태인 경우 true 값을 가지는 부울 매개 변수입니다. 그렇지 않으면 false 값을 갖습니다. 활성(Active)으로 설정된 객체는 드롭다운 메뉴 및 미리 입력 필드에 표시되며 다른 객체에 첨부할 수 있습니다. 활성으로 설정되지 않은 객체는 드롭다운 메뉴에 표시되지 않으며 다른 객체에 첨부할 미리 입력 필드는 표시되지 않습니다.  </p> </li> 
     <li style="font-weight: bold;"> <p>이름 </p> <p style="font-weight: normal;">이름 길이가 255자를 넘지 않도록 지정하는 유효성 검사기 MAX_LENGTH가 추가되었습니다.  </p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>기본 필드</td> 
   <td> 
    <ul> 
     <li style="font-weight: bold;"> <p>isActive</p> <p style="font-weight: normal;">추가됨</p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

### 프로젝트 {#project}

프로젝트는 Workfront 내의 작업 항목이며, Workfront이 사람들이 작업을 수행하는 데 도움이 되는 기본 빌딩 블록입니다. 프로젝트 객체는 공통, 특정 목표를 가진 작업 그룹을 나타냅니다.

<table style="table-layout:auto"> 
 <col data-mc-conditions=""> 
 <col data-mc-conditions=""> 
 <tbody> 
  <tr> 
   <td colspan="2">직접 필드<p style="font-weight: normal;">다음 필드에 AT_DATE_BEFORE_YEAR 및 AT_DATE_AFTER_YEAR가 추가되었습니다. 이러한 유효성 검사기는 연결된 개체의 날짜를 1900년 전이나 2200년 이후에 설정할 수 없도록 지정합니다.</p>
    <ul>
     <li style="font-weight: bold;">actualCompletionDate</li>
     <li style="font-weight: bold;">actualStartDate</li>
     <li style="font-weight: bold;">planningCompletionDate</li>
     <li style="font-weight: bold;">planningStartDate</li>
    </ul><p style="font-weight: normal;">EAC(완료 시 예상) 계산을 수행할 때 투명성을 위해 공개 API에 다음 필드가 추가되었습니다.</p>
    <ul>
     <li><p style="font-weight: bold;">bwp</p><p style="font-weight: normal;">BCWP(Backed Cost of Work Performed)라고도 하는 Earned Value는 이 지표가 계산될 때 실제로 완료된 작업의 금액의 예산책정된 비용을 나타내는 프로젝트 성과 지표입니다. 작업의 경우 BCWP = 실제 완료 퍼센트 x 작업 예산입니다. 프로젝트의 경우 BCWP = SUM(모든 상위 및 개별 작업의 BCWP 값)입니다.</p></li>
     <li><p style="font-weight: bold;">bcws</p><p style="font-weight: normal;">계획 값이라고도 하는 BCWS(Scheduled Cost of Work Scheduled)는 이 지표가 계산될 때 완료했어야 하는 작업의 금액의 예산책정된 비용을 나타내는 프로젝트 성과 지표입니다. 작업의 경우 BCWS = 계획 완료 퍼센트 x 작업 예산입니다. 프로젝트의 경우 BCWS = SUM(모든 상위 작업과 개별 작업의 BCWS 값).</p></li>
    </ul><p style="font-weight: normal;">다음 필드에 플래그 CURRENCY가 추가되었습니다</p>
    <ul>
     <li style="font-weight: bold;">projectBudgetCost</li>
     <li style="font-weight: bold;">projectNetValue</li>
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

### 증명 승인 {#proofapproval}

ProofApproval 개체는 증명에 직접 연결된 승인을 나타냅니다.

<table style="table-layout:auto"> 
 <col data-mc-conditions=""> 
 <col data-mc-conditions=""> 
 <tbody> 
  <tr> 
   <td>직접 필드</td> 
   <td> 
    <ul> 
     <li style="font-weight: bold;"> <p>isWaitingDecision</p> <p style="font-weight: normal;">이 필드가 추가되었으며, 증명이 결정을 기다리는 경우 true 값을 가지는 부울 매개 변수이고 그렇지 않으면 false입니다.  </p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

### QueueDef {#queuedef}

QueueDef 개체는 사용자가 문제를 해당 항목에 제출할 수 있도록 도움말 데스크 영역에 게시된 프로젝트인 Queue를 나타냅니다.

<table style="table-layout:auto"> 
 <col data-mc-conditions=""> 
 <col data-mc-conditions=""> 
 <tbody> 
  <tr> 
   <td>직접 필드</td> 
   <td> <p>다음 필드에 가능한 값 BUDGETING_INFORMATION이 추가되었습니다. 이를 통해 사용자가 계획자에서 우선순위 및 예산 시간을 편집할 수 있습니다.</p> 
    <ul> 
     <li style="font-weight: bold;">requestorCoreAction</li> 
     <li style="font-weight: bold;">requestorForbiddenActions</li> 
    </ul>  </td> 
  </tr> 
 </tbody> 
</table>

### ReservedTime {#reservedtime}

ReservedTime 개체는 사용자가 작업에 사용할 수 없음을 나타내는 사용자의 개인 시간에 지정된 일을 나타냅니다.

ReservedTime 리소스가 REPORTABLE 플래그를 추가했습니다.

<table style="table-layout:auto"> 
 <col data-mc-conditions=""> 
 <col data-mc-conditions=""> 
 <tbody> 
  <tr> 
   <td>직접 필드</td> 
   <td> <p>다음 필드에서 NOT_GROUPABLE 플래그를 제거했습니다.</p> 
    <ul> 
     <li style="font-weight: bold;">endDate</li> 
     <li style="font-weight: bold;">extRefID</li> 
     <li style="font-weight: bold;">startDate </li> 
    </ul> <p>ReservedTime 개체에서 다음 필드가 제거되었습니다.</p> 
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

### 리소스 플래너필터 {#resourceplannerfilter}

ResourcePlannerFilter 객체는 리소스 계획자에 표시할 항목을 결정하는 규칙 세트입니다.

ResourcePlannerFilter 리소스가 SHARABLE 플래그를 추가했습니다. 객체에 다른 변경 사항이 없습니다.

### 위험 {#risk}

위험 객체는 프로젝트가 제 시간에 또는 예산 내에서 완료되지 못하도록 할 수 있는 가능한 이벤트를 나타냅니다. 작업 승인 전에 발생할 수 있는 장애물을 식별하기 위해 계획 단계의 프로젝트에 위험이 추가됩니다.

<table style="table-layout:auto"> 
 <col data-mc-conditions=""> 
 <col data-mc-conditions=""> 
 <tbody> 
  <tr> 
   <td>직접 필드</td> 
   <td> <p>위험 개체에 다음 필드가 추가되었습니다.</p> 
    <ul> 
     <li style="font-weight: bold;"> <p>enteredByID</p> <p style="font-weight: normal;">원래 개체를 만든 사용자의 ID입니다.</p> </li> 
     <li> <p style="font-weight: bold;">entryDate</p> <p>Workfront에서 사용자가 개체를 제출한 날짜입니다.</p> </li> 
     <li> <p style="font-weight: bold;">lastUpdateDate</p> <p>Last Update Date 매개 변수는 개체에 Last Update가 수행된 날짜를 반환합니다.</p> </li> 
     <li> <p style="font-weight: bold;">lastUpdatedByID </p> <p>Last Updated By ID는 개체를 업데이트한 마지막 사용자의 사용자 ID를 반환하는 매개 변수입니다.  </p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>참조 필드</td> 
   <td> <p style="font-weight: normal;">다음 참조 필드가 RIsk 개체에 추가되었습니다.</p> 
    <ul> 
     <li style="font-weight: bold;">enteredBy</li> 
     <li style="font-weight: bold;">lastUpdatedBy  </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

### 예약된 보고서 {#scheduledreport}

ScheduledReport 개체는 배달하도록 구성된 보고서를 나타냅니다.

<table style="table-layout:auto"> 
 <col data-mc-conditions=""> 
 <col data-mc-conditions=""> 
 <tbody> 
  <tr> 
   <td>직접 필드</td> 
   <td> 
    <ul> 
     <li style="font-weight: bold;"> <p>pageSize</p> <p style="font-weight: normal;">다음 가능한 값을 추가했습니다.</p> 
      <ul> 
       <li style="font-weight: normal;">A2</li> 
       <li style="font-weight: normal;">A1</li> 
       <li style="font-weight: normal;">A0  </li> 
      </ul> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

### ScoreCardQuestion {#scorecardquestion}

ScoreCardQuestion 개체는 스코어카드에 추가된 질문을 나타냅니다. 이러한 질문은 일반적으로 Portfolio 관리자에 의해 결정되며 관리자가 이러한 질문에 대한 답변을 통해 프로젝트가 포트폴리오의 목표에 얼마나 잘 부합하는지 이해할 수 있습니다.

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

작업 객체는 최종 목표(프로젝트 완료)를 달성하는 단계로 수행되어야 하는 작업 항목을 나타냅니다.

<table style="table-layout:auto"> 
 <col data-mc-conditions=""> 
 <col data-mc-conditions=""> 
 <tbody> 
  <tr> 
   <td colspan="2">직접 필드<p style="font-weight: normal;">다음 필드에 AT_DATE_BEFORE_YEAR 및 AT_DATE_AFTER_YEAR가 추가되었습니다. 이러한 유효성 검사기는 연결된 개체의 날짜를 1900년 전이나 2200년 이후에 설정할 수 없도록 지정합니다.</p>
    <ul>
     <li style="font-weight: bold;">actualCompletionDate</li>
     <li style="font-weight: bold;">actualStartDate</li>
     <li style="font-weight: bold;">constraintDate</li>
     <li style="font-weight: bold;">planningCompletionDate</li>
     <li style="font-weight: bold;">planningStartDate</li>
    </ul><p style="font-weight: normal;">EAC(완료 시 예상) 계산을 수행할 때 투명성을 위해 공개 API에 다음 필드가 추가되었습니다.</p>
    <ul>
     <li><p style="font-weight: bold;">bwp</p><p style="font-weight: normal;">BCWP(Backed Cost of Work Performed)라고도 하는 Earned Value는 이 지표가 계산될 때 실제로 완료된 작업의 금액의 예산책정된 비용을 나타내는 프로젝트 성과 지표입니다. 작업의 경우 BCWP = 실제 완료 퍼센트 x 작업 예산입니다. 프로젝트의 경우 BCWP = SUM(모든 상위 및 개별 작업의 BCWP 값)입니다.</p></li>
     <li><p style="font-weight: bold;">bcws</p><p style="font-weight: normal;">계획 값이라고도 하는 BCWS(Scheduled Cost of Work Scheduled)는 이 지표가 계산될 때 완료했어야 하는 작업의 금액의 예산책정된 비용을 나타내는 프로젝트 성과 지표입니다. 작업의 경우 BCWS = 계획 완료 퍼센트 x 작업 예산입니다. 프로젝트의 경우 BCWS = SUM(모든 상위 작업과 개별 작업의 BCWS 값).</p></li>
    </ul><p style="font-weight: normal;">다음 필드에 가능한 값 ET가 추가되었습니다. 이 값은 주말 또는 휴일에 상관 없이 월을 참조하는 경과 개월 단위를 나타냅니다.</p>
    <ul>
     <li style="font-weight: bold;">durationUnit</li>
     <li style="font-weight: bold;">workUnit</li>
    </ul><p style="font-weight: normal;">작업 개체에서 다음 필드가 제거되었습니다.</p>
    <ul>
     <li style="font-weight: bold;">reservedTimeID</li>
    </ul><p style="font-weight: normal;">작업 개체에 다음 필드가 추가되었습니다.</p>
    <ul>
     <li style="font-weight: bold;">storyPoints</li>
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

팀 개체는 작업 항목에 지정할 수 있는 사용자 모음입니다.

<table style="table-layout:auto"> 
 <col data-mc-conditions=""> 
 <col data-mc-conditions=""> 
 <tbody> 
  <tr> 
   <td>직접 필드</td> 
   <td> 
    <ul> 
     <li style="font-weight: bold;"> <p>agileEstimateType </p> <p style="font-weight: normal;">이 필드가 Team 개체에 추가되었습니다. Agile Estimate Type은 스토리의 작업 로드가 예상되는 방식을 결정합니다. 시간 단위로 추정하면 스토리에 추가된 계획 시간 수입니다. 포인트 단위로 추정하면 각 지점에 포인트가 설정되는 방식에 따라 스토리에 계획 시간 수가 추가됩니다(기본값은 8시간). 애자일 예상 유형에 가능한 값은 다음과 같습니다.</p> 
      <ul> 
       <li style="font-weight: normal;"> STORY_POINTS(스토리 지점)</li> 
       <li style="font-weight: normal;">시간(시간)</li> 
       <li style="font-weight: normal;">LEGACY_POINTS(Hours as Points)  </li> 
      </ul> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

### 템플릿 {#template}

Template 객체는 프로젝트에 대한 패턴을 나타냅니다. 시간을 절약하기 위해 템플릿에서 프로젝트를 만들 수 있습니다. 템플릿에는 팀 및 작업이 포함되어 있으며, 이 작업은 템플릿을 사용할 때 프로젝트에 복사됩니다.

<table style="table-layout:auto"> 
 <col data-mc-conditions=""> 
 <col data-mc-conditions=""> 
 <tbody> 
  <tr> 
   <td>직접 필드</td> 
   <td> 
    <ul> 
     <li style="font-weight: bold;"> <p>isActive</p> <p style="font-weight: normal;">이 필드가 추가되었으며 개체가 활성 상태인 경우 true 값을 가지는 부울 매개 변수입니다. 그렇지 않으면 false 값을 갖습니다. 활성(Active)으로 설정된 객체는 드롭다운 메뉴 및 미리 입력 필드에 표시되며 다른 객체에 첨부할 수 있습니다. 활성으로 설정되지 않은 객체는 드롭다운 메뉴에 표시되지 않으며 다른 객체에 첨부할 미리 입력 필드는 표시되지 않습니다.  </p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>컬렉션 필드</td> 
   <td> 
    <ul> 
     <li style="font-weight: bold;"> <p>allPriority</p> <p style="font-weight: normal;">추가됨</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>기본 필드</td> 
   <td> 
    <ul> 
     <li style="font-weight: bold;"> <p>isActive</p> <p style="font-weight: normal;">추가됨</p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

### TemplateAssignment {#templateassignment}

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
     <li style="font-weight: bold;"> <p>workUnit</p> <p style="font-weight: normal;">가능한 값 ET가 추가되었습니다. 이 값은 주말 또는 휴일에 상관 없이 월을 참조하는 경과 개월 단위를 나타냅니다.  </p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

### TemplateTask {#templatetask}

TemplateTask 개체는 템플릿에 속하는 작업을 나타냅니다. 템플릿 작업은 템플릿이 사용되는 프로젝트에서 작업이 됩니다.

<table style="table-layout:auto"> 
 <col data-mc-conditions=""> 
 <col data-mc-conditions=""> 
 <tbody> 
  <tr> 
   <td>직접 필드</td> 
   <td> <p style="font-weight: normal;">다음 필드에 가능한 값 ET가 추가되었습니다. 이 값은 주말 또는 휴일에 상관 없이 월을 참조하는 경과 개월 단위를 나타냅니다.</p> 
    <ul> 
     <li style="font-weight: bold;">durationUnit</li> 
     <li style="font-weight: bold;">workUnit</li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>컬렉션 필드</td> 
   <td> 
    <ul> 
     <li style="font-weight: bold;"> <p>allPriority</p> <p style="font-weight: normal;">추가됨</p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

### 타임시트 {#timesheet}

작업표 개체는 사용자가 작업, 프로젝트 및 오버헤드 시간 유형에 대해 실제 작업 시간을 입력할 수 있도록 하는 가상 타임카드를 나타냅니다.

<table style="table-layout:auto"> 
 <col data-mc-conditions=""> 
 <col data-mc-conditions=""> 
 <tbody> 
  <tr> 
   <td>핵심 필드</td> 
   <td> 
    <ul> 
     <li style="font-weight: bold;"> <p>objCode</p> <p style="font-weight: normal;">제거됨</p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

### 업데이트 {#update}

Workfront의 작업 항목을 업데이트하여 사용자에게 현재 상태에 대한 정보를 제공할 수 있습니다. Update 개체는 이러한 업데이트 중 하나를 나타냅니다. 업데이트는 사용자가 입력하거나 Workfront 시스템에서 만들 수 있습니다.

<table style="table-layout:auto"> 
 <col data-mc-conditions=""> 
 <col data-mc-conditions=""> 
 <tbody> 
  <tr> 
   <td>직접 필드</td> 
   <td> 
    <ul> 
     <li style="font-weight: bold;"> <p>updateType</p> <p style="font-weight: normal;">가능한 값 referenceObjectCustomData (enum.updatetime.referenceobjectcustomdata)를 추가했습니다.  </p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>쿼리</td> 
   <td> <p style="font-weight: normal;">다음 쿼리가 Update 개체에 추가되었습니다.</p> 
    <ul> 
     <li style="font-weight: bold;">objectUpdatesMobile</li> 
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
     <li style="font-weight: bold;"> <p>loginAsAccessRules</p> <p style="font-weight: normal;">추가됨</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>액션</td> 
   <td> <p style="font-weight: normal;">다음 작업이 사용자 개체에 추가되었습니다.</p> 
    <ul> 
     <li style="font-weight: bold;">hasGrantLoginAsAccess</li> 
     <li style="font-weight: bold;">isUserAdmin</li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>쿼리</td> 
   <td> 
    <ul> 
     <li style="font-weight: bold;"> <p>userAdmins</p> <p style="font-weight: normal;">추가됨</p> </li> 
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
   <td> <p style="font-weight: normal;">다음 작업이 사용자 개체에 추가되었습니다.</p> 
    <ul> 
     <li style="font-weight: bold;">acknowledgementMyNotifications</li> 
     <li style="font-weight: bold;">unacceptedAllObjectsTypeCount  </li> 
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

작업 개체는 Task 및 OpTask가 모두 상속하고 두 Task 간에 공통 코드를 공유하는 공통 인터페이스입니다.

<table style="table-layout:auto"> 
 <col data-mc-conditions=""> 
 <col data-mc-conditions=""> 
 <tbody> 
  <tr> 
   <td colspan="2">직접 필드<p style="font-weight: normal;">다음 필드에 AT_DATE_BEFORE_YEAR 및 AT_DATE_AFTER_YEAR가 추가되었습니다. 이러한 유효성 검사기는 연결된 개체의 날짜를 1900년 전이나 2200년 이후에 설정할 수 없도록 지정합니다.</p>
    <ul>
     <li style="font-weight: bold;">actualCompletionDate</li>
     <li style="font-weight: bold;">actualStartDate</li>
     <li style="font-weight: bold;">constraintDate</li>
     <li style="font-weight: bold;">planningCompletionDate</li>
     <li style="font-weight: bold;">planningStartDate</li>
    </ul><p style="font-weight: normal;">EAC(완료 시 예상) 계산을 수행할 때 투명성을 위해 공개 API에 다음 필드가 추가되었습니다.</p>
    <ul>
     <li><p style="font-weight: bold;">bwp</p><p style="font-weight: normal;">BCWP(Backed Cost of Work Performed)라고도 하는 Earned Value는 이 지표가 계산될 때 실제로 완료된 작업의 금액의 예산책정된 비용을 나타내는 프로젝트 성과 지표입니다. 작업의 경우 BCWP = 실제 완료 퍼센트 x 작업 예산입니다. 프로젝트의 경우 BCWP = SUM(모든 상위 및 개별 작업의 BCWP 값)입니다.</p></li>
     <li><p style="font-weight: bold;">bcws</p><p style="font-weight: normal;">계획 값이라고도 하는 BCWS(Scheduled Cost of Work Scheduled)는 이 지표가 계산될 때 완료했어야 하는 작업의 금액의 예산책정된 비용을 나타내는 프로젝트 성과 지표입니다. 작업의 경우 BCWS = 계획 완료 퍼센트 x 작업 예산입니다. 프로젝트의 경우 BCWS = SUM(모든 상위 작업과 개별 작업의 BCWS 값).</p></li>
    </ul><p style="font-weight: normal;">다음 필드에 가능한 값 ET가 추가되었습니다. 이 값은 주말 또는 휴일에 상관 없이 월을 참조하는 경과 개월 단위를 나타냅니다.</p>
    <ul>
     <li style="font-weight: bold;">durationUnit</li>
     <li style="font-weight: bold;">workUnit</li>
    </ul><p style="font-weight: normal;">다음 필드가 작업 개체에서 제거되었습니다.</p>
    <ul>
     <li style="font-weight: bold;">reservedTimeID</li>
    </ul><p style="font-weight: normal;">다음 필드가 작업 개체에 추가되었습니다.</p>
    <ul>
     <li style="font-weight: bold;">storyPoints</li>
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
