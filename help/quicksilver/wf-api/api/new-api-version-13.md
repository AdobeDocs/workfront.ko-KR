---
content-type: api
navigation-topic: api-navigation-topic
title: API 버전 13의 새로운 기능
description: Adobe Workfront은 2021년 4월 22일에 API 버전 13을 출시했습니다. API 버전 13에는 버전 12의 다음 변경 사항이 포함되어 있습니다.
author: Becky
feature: Workfront API
role: Developer
exl-id: afbc986e-8b5c-40bc-9120-e8d34e0f7004
source-git-commit: 3e339e2bfb26e101f0305c05f620a21541394993
workflow-type: tm+mt
source-wordcount: '1064'
ht-degree: 2%

---

# API 버전 13의 새로운 기능

Adobe Workfront은 2021년 4월 22일에 API 버전 13을 출시했습니다. API 버전 13에는 버전 12의 다음 변경 사항이 포함되어 있습니다.

## 추가된 리소스

API 버전 13에 대해 추가된 리소스가 없습니다.

## 제거된 리소스

API 버전 13에 대해 제거된 리소스가 없습니다.

## 수정된 리소스

API 버전 13에 대해 다음 리소스가 수정되었습니다.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td> 
    <ul> 
     <li> <p><a href="#accesslevel" class="MCXref xref">AccessLevel</a> </p> </li> 
     <li> <p><a href="#breadcrumb" class="MCXref xref">빵 부스러기</a> </p> </li> 
     <li> <p><a href="#burndownevent" class="MCXref xref">번다운 이벤트</a> </p> </li> 
     <li> <p><a href="#customerpreferences" class="MCXref xref">고객 환경 설정</a> </p> </li> 
     <li> <p><a href="#documentversion" class="MCXref xref">DocumentVersion</a> </p> </li> 
     <li> <p><a href="#group" class="MCXref xref">그룹 </a> </p> </li> 
     <li> <p><a href="#journalentry" class="MCXref xref">저널 게시물</a> </p> </li> 
     <li> <p><a href="#layouttemplate" class="MCXref xref">레이아웃 템플릿</a> </p> </li> 
     <li> <p><a href="#linkedfolder" class="MCXref xref">LinkedFolder</a> </p> </li> 
     <li> <p><a href="#optask" class="MCXref xref">OpTask</a> </p> </li> 
    </ul> </td> 
   <td> 
    <ul> 
     <li> <p><a href="#project" class="MCXref xref">프로젝트</a> </p> </li> 
     <li> <p><a href="#proofapproval" class="MCXref xref">ProofApproval</a> </p> </li> 
     <li> <p><a href="#queuedef" class="MCXref xref">QueueDef</a> </p> </li> 
     <li> <p><a href="#task" class="MCXref xref">작업</a> </p> </li> 
     <li> <p><a href="#team" class="MCXref xref">팀</a> </p> </li> 
     <li> <p><a href="#timesheet" class="MCXref xref">타임시트</a> </p> </li> 
     <li> <p><a href="#timesheetprofile" class="MCXref xref">타임시트 프로필</a> </p> </li> 
     <li> <p><a href="#uitemplate" class="MCXref xref">UITemplate</a> </p> </li> 
     <li> <p><a href="#userdelegation" class="MCXref xref">사용자 위임</a> </p> </li> 
     <li> <p><a href="#work" class="MCXref xref">작업 </a> </p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

### AccessLevel {#accesslevel}

AccessLevel 개체는 사용자와 연결되어 있으며 사용자가 액세스할 수 있는 항목을 결정하는 AccessLevelPermissions 집합에 대해 설명합니다.

액세스 수준에 대한 자세한 내용은 [액세스 수준 작동 방식](../../administration-and-setup/add-users/access-levels-and-object-permissions/access-levels.md).

<table style="table-layout:auto"> 
 <col data-mc-conditions=""> 
 <col data-mc-conditions=""> 
 <tbody> 
  <tr> 
   <td> <p>직접 필드</p> </td> 
   <td> 
    <ul> 
     <li> <p><b>설명</b> </p> <p>설명의 길이가 4000자를 넘지 않도록 지정하는 유효성 검사기 MAX_LENGTH가 추가되었습니다.</p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

### 빵 부스러기 {#breadcrumb}

BreadCrumb 개체는 Workfront 작업 항목의 상위/하위 계층 구조에 있는 요소를 나타냅니다. 이동 경로는 작업 항목이 더 큰 구조의 Portfolio, 프로젝트, 프로젝트 및 작업에 어떻게 적합한지 나타냅니다.

이동 경로에 대한 자세한 내용은 [새로운 Adobe Workfront 경험의 탐색 표시 개요](../../workfront-basics/the-new-workfront-experience/breadcrumb-overview.md)

<table style="table-layout:auto"> 
 <col data-mc-conditions=""> 
 <col data-mc-conditions=""> 
 <tbody> 
  <tr> 
   <td> <p>직접 필드</p> </td> 
   <td> 
    <ul> 
     <li> <p><b>objCode</b> </p> <p>개체 코드는 다음에서 찾을 수 있습니다. <a href="../../wf-api/general/api-explorer.md" class="MCXref xref">API 탐색기</a>.</p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

### 번다운 이벤트 {#burndownevent}

BurndownEvent 객체는 이터레이션의 번다운을 변경하는 객체를 나타냅니다.

번다운에 대한 자세한 내용은 [번다운](../../agile/use-scrum-in-an-agile-team/burndown/burndown.md).

<table style="table-layout:auto"> 
 <col data-mc-conditions=""> 
 <col data-mc-conditions=""> 
 <tbody> 
  <tr> 
   <td> <p>직접 필드</p> </td> 
   <td> <p>다음 필드에서 NOT_GROUPABLE 플래그가 제거되었습니다. </p> 
    <ul> 
     <li> <p>applyDate</p> </li> 
     <li> <p>entryDate</p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

### 고객 환경 설정 {#customerpreferences}

CustomerPreferences 객체는 고객이 Workfront 인스턴스에 대해 설정한 환경 설정 집합을 나타냅니다.

<table style="table-layout:auto"> 
 <col data-mc-conditions=""> 
 <col data-mc-conditions=""> 
 <tbody> 
  <tr> 
   <td>직접 필드</td> 
   <td> 
    <ul> 
     <li style="font-weight: bold;"> <p>이름</p> <p style="font-weight: normal;">가능한 값이 추가되었습니다.</p> 
      <ul> 
       <li style="font-weight: normal;">암호:aemAPIKey (config.general.aem.apikey)</li> 
       <li style="font-weight: normal;"> 암호:aemAADomain (config.general.aem.aadomain) </li> 
       <li style="font-weight: normal;">암호:aemIntegrationEnabled (config.general.aem.enabled)</li> 
       <li style="font-weight: normal;">password:aemHost (config.general.aem.host)</li> 
       <li style="font-weight: normal;">타임시트:default.timesheet.restrict.timesheet.edit.owners.admins (config.timesheet.restrict.timesheet.edit.owners.admins)</li> 
      </ul> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>액션</td> 
   <td> <p>다음 작업이 CustomerPreferences 리소스에 추가되었습니다.</p> 
    <ul> 
     <li> <p><b>getTimesheetPreferences</b> </p> </li> 
     <li> <p><b>타임시트 환경 설정 지정</b> </p> <p>인수를 사용합니다.</p> 
      <ul> 
       <li> <p>환경 설정(맵)</p> </li> 
      </ul> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

### DocumentVersion {#documentversion}

DocumentVersion 개체는 작성된 자료, 이미지 또는 다른 형태의 정보 등 파일의 특정 버전을 나타냅니다.

문서 버전에 대한 자세한 내용은 [새 문서 버전 업로드](../../documents/managing-documents/upload-new-document-version.md).

<table style="table-layout:auto"> 
 <col data-mc-conditions=""> 
 <col data-mc-conditions=""> 
 <tbody> 
  <tr> 
   <td> <p>직접 필드</p> </td> 
   <td> 
    <ul> 
     <li> <p><b>externalIntegrationType</b> </p> <p>추가된 가능한 값:</p> 
      <ul> 
       <li> <p>AEM(Adobe Experience Manager)</p> </li> 
      </ul> </li> 
    </ul> 
    <ul> 
     <li> <p><b>proofID</b> </p> <p>NOT_FILTERABLE 플래그가 추가되었습니다.</p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

### 그룹  {#group}

Group 객체는 사용자 및 팀 집합을 나타냅니다. 그룹은 종종 부서 구조를 나타냅니다.

그룹에 대한 자세한 내용은 [Adobe Workfront의 그룹과 팀 비교](../../people-teams-and-groups/work-with-groups-and-teams/understanding-differences-and-similarities-between-groups-and-teams.md).

<table style="table-layout:auto"> 
 <col data-mc-conditions=""> 
 <col data-mc-conditions=""> 
 <tbody> 
  <tr> 
   <td> <p>액션</p> </td> 
   <td> 
    <ul> 
     <li> <p><b>getParents</b> </p> <p>이 작업은 그룹의 상위 그룹(지정된 그룹이 의 하위 그룹인 그룹) 배열을 반환합니다.</p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

### 저널 게시물 {#journalentry}

JournalEntry 개체는 특정 개체 필드에 대한 정보를 해당 필드가 수정될 때마다 기록하도록 설정할 수 있습니다. 필드가 저널 게시물 개체의 일부로 기록되도록 설정되면 해당 필드를 수정할 때마다 해당 저널 게시물이 만들어집니다.

JournalEntry 리소스가 REPORTABLE 플래그를 추가했습니다.

<table style="table-layout:auto"> 
 <col data-mc-conditions=""> 
 <col data-mc-conditions=""> 
 <tbody> 
  <tr> 
   <td> <p>직접 필드</p> </td> 
   <td> <p>다음 필드에서 플래그 NOT_GROUPABLE을 제거했습니다.</p> 
    <ul> 
     <li> <p><b>changeType</b> </p> </li> 
     <li> <p><b>entryDate</b> </p> </li> 
     <li> <p><b>fieldName</b> </p> </li> 
     <li> <p><b>objObjCode</b> </p> </li> 
    </ul> <p>다음 필드에 NOT_FILTERABLE 플래그가 추가되었습니다.</p> 
    <ul> 
     <li> <p><b>subObjCode</b> </p> </li> 
     <li> <p><b>subObjId</b> </p> </li> 
     <li> <p><b>topObjCode</b> </p> </li> 
     <li> <p><b>topObjID</b> </p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

### 레이아웃 템플릿 {#layouttemplate}

Adobe Workfront 관리자 또는 그룹 관리자는 템플릿을 만들어 Adobe Workfront의 레이아웃 요소를 사용자 정의할 수 있습니다. LayoutTemplate 개체는 Adobe Workfront Classic에 따라 다릅니다.

새 Adobe Workfront 경험에서 레이아웃 템플릿을 나타내는 오브젝트에 대해서는 다음을 참조하십시오. [UITemplate](#uitemplate)

<table style="table-layout:auto"> 
 <col data-mc-conditions=""> 
 <col data-mc-conditions=""> 
 <tbody> 
  <tr> 
   <td> <p>직접 필드</p> </td> 
   <td> 
    <ul> 
     <li> <p><b>설명</b> </p> <p>설명의 길이가 4000자를 넘지 않도록 지정하는 유효성 검사기 MAX_LENGTH가 추가되었습니다.</p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

### LinkedFolder {#linkedfolder}

LinkedFolder 개체는 Google 드라이브 또는 Dropbox과 같은 외부 문서 공급자로부터 연결된 폴더를 나타냅니다.

연결된 폴더에 대한 자세한 내용은 [외부 애플리케이션에서 문서 연결](../../documents/adding-documents-to-workfront/link-documents-from-external-apps.md).

<table style="table-layout:auto"> 
 <col data-mc-conditions=""> 
 <col data-mc-conditions=""> 
 <tbody> 
  <tr> 
   <td> <p>직접 필드</p> </td> 
   <td> 
    <ul> 
     <li> <p><b>externalIntegrationType</b> </p> <p>추가된 가능한 값:</p> 
      <ul> 
       <li> <p>AEM(Adobe Experience Manager)</p> </li> 
      </ul> </li> 
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
   <td> <p>필드 검색</p> </td> 
   <td> 
    <ul> 
     <li> <p><b>favortedByUsersMM</b> </p> </li> 
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
   <td> <p>직접 필드</p> </td> 
   <td> 
    <ul> 
     <li> <p><b>convertedOpTaskOriginatorID</b> </p> <!--
       <p data-mc-conditions="QuicksilverOrClassic.Draft mode">Removed flag NOT&nbsp;FILTERABLE</p>
      --> </li> 
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
   <td> <p>직접 필드</p> </td> 
   <td> <p>다음 필드가 ProofApproval 리소스에 추가되었습니다.</p> 
    <ul> 
     <li> <p><b>approverStage</b> </p> </li> 
     <li> <p><b>결정 날짜</b> </p> </li> 
     <li> <p><b>workflowTemplate</b> </p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

### QueueDef {#queuedef}

QueueDef 개체는 사용자가 문제를 제출할 수 있도록 헬프 데스크 영역에 게시된 프로젝트인 Queue를 나타냅니다.

요청 대기열에 대한 자세한 내용은 [요청 대기열 만들기](../../manage-work/requests/create-and-manage-request-queues/create-request-queue.md).

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">직접 필드</td> 
   <td> 
    <ul> 
     <li> <p><b>documentPosition</b> </p> <p>추가됨. 가능한 값:</p> 
      <ul> 
       <li> <p>0(사용자 정의 양식 후)</p> </li> 
       <li> <p>1(사용자 정의 양식 전)</p> </li> 
      </ul> </li> 
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
   <td> <p>필드 검색</p> </td> 
   <td> 
    <ul> 
     <li> <p><b>favortedByUsersMM</b> </p> </li> 
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

### 타임시트 {#timesheet}

타임시트 오브젝트는 사용자가 작업, 프로젝트 및 오버헤드 시간 유형에 대한 실제 작업 시간을 입력할 수 있는 가상 타임카드를 나타냅니다.

<table style="table-layout:auto"> 
 <col data-mc-conditions=""> 
 <col data-mc-conditions=""> 
 <tbody> 
  <tr> 
   <td>직접 필드</td> 
   <td> 
    <ul> 
     <li> <p><b>isOvertimeDisabled</b> </p> <p>추가됨</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>코어 필드</td> 
   <td> 
    <ul> 
     <li> <p><b>objCode</b> </p> <p>제거됨</p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

### 타임시트 프로필 {#timesheetprofile}

타임시트 오브젝트는 사용자가 작업, 프로젝트 및 오버헤드 시간 유형에 대한 실제 작업 시간을 입력할 수 있는 가상 타임카드를 나타냅니다.

<table style="table-layout:auto"> 
 <col data-mc-conditions=""> 
 <col data-mc-conditions=""> 
 <tbody> 
  <tr> 
   <td>직접 필드</td> 
   <td> 
    <ul> 
     <li> <p><b>isOvertimeDisabled</b> </p> <p>추가됨</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>기본 필드</td> 
   <td> 
    <ul> 
     <li> <p><b>isOvertimeDisabled</b> </p> <p>추가됨</p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

### UITemplate {#uitemplate}

Adobe Workfront 관리자 또는 그룹 관리자는 템플릿을 만들어 Adobe Workfront의 레이아웃 요소를 사용자 정의할 수 있습니다. UITemplate 개체는 새로운 Adobe Workfront 환경에 따라 다릅니다.

Adobe Workfront Classic의 레이아웃 템플릿을 나타내는 오브젝트에 대해서는 다음을 참조하십시오. [레이아웃 템플릿](#layouttemplate).

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">액션</td> 
   <td> <p>다음 작업이 UITemplate 리소스에 추가되었습니다.</p> 
    <ul> 
     <li> <p><b>migrateCustomersAllLayoutTemplates</b> </p> <p>인수를 사용합니다.</p> 
      <ul> 
       <li> <p>overrideIfExists (부울)</p> </li> 
      </ul> </li> 
     <li> <p><b>migrateLayoutTemplates</b> </p> <p>인수를 사용합니다.</p> 
      <ul> 
       <li> <p>layoutTemplateIDs (string[])</p> </li> 
       <li> <p>overrideIfExists (부울)</p> </li> 
      </ul> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

### 사용자 위임 {#userdelegation}

UserDelegation 개체는 특정 시간 동안 한 사용자가 다른 사용자에게 작업을 위임하는 행위를 나타냅니다.

UserDelegation 개체가 REPORTABLE 플래그를 추가했습니다.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">직접 필드</td> 
   <td> <p>다음 필드에서 NOT_GROUPABLE 플래그가 제거되었습니다.</p> 
    <ul> 
     <li> <p><b>endDate</b> </p> </li> 
     <li> <p><b>startDate</b> </p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">기본 필드</td> 
   <td> <p>다음 필드가 추가되었습니다.</p> 
    <ul> 
     <li> <p><b>endDate</b> </p> </li> 
     <li> <p><b>startDate</b> </p> </li> 
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
   <td> <p>필드 검색</p> </td> 
   <td> 
    <ul> 
     <li> <p><b>favortedByUsersMM</b> </p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>
