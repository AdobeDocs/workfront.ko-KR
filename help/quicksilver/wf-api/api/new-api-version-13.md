---
content-type: api
navigation-topic: api-navigation-topic
title: API 버전 13의 새로운 기능
description: Adobe Workfront은 2021년 4월 22일에 API 버전 13을 릴리스했습니다. API 버전 13은 버전 12에서 다음과 같은 변경 사항을 제공합니다.
author: Becky
feature: Workfront API
exl-id: afbc986e-8b5c-40bc-9120-e8d34e0f7004
source-git-commit: f050c8b95145552c9ed67b549608c16115000606
workflow-type: tm+mt
source-wordcount: '1064'
ht-degree: 2%

---

# API 버전 13의 새로운 기능

Adobe Workfront은 2021년 4월 22일에 API 버전 13을 릴리스했습니다. API 버전 13은 버전 12에서 다음과 같은 변경 사항을 제공합니다.

## 리소스를 추가했습니다.

API 버전 13에 대한 리소스가 추가되지 않았습니다.

## 제거된 리소스

API 버전 13에 대해 제거된 리소스가 없습니다.

## 수정된 리소스

다음 리소스가 API 버전 13에 대해 수정되었습니다.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td> 
    <ul> 
     <li> <p><a href="#accesslevel" class="MCXref xref">AccessLevel</a> </p> </li> 
     <li> <p><a href="#breadcrumb" class="MCXref xref">BreadCrumb</a> </p> </li> 
     <li> <p><a href="#burndownevent" class="MCXref xref">BurndownEvent</a> </p> </li> 
     <li> <p><a href="#customerpreferences" class="MCXref xref">고객 기본 설정</a> </p> </li> 
     <li> <p><a href="#documentversion" class="MCXref xref">DocumentVersion</a> </p> </li> 
     <li> <p><a href="#group" class="MCXref xref">그룹 </a> </p> </li> 
     <li> <p><a href="#journalentry" class="MCXref xref">분개 입력</a> </p> </li> 
     <li> <p><a href="#layouttemplate" class="MCXref xref">레이아웃 템플릿</a> </p> </li> 
     <li> <p><a href="#linkedfolder" class="MCXref xref">LinkedFolder</a> </p> </li> 
     <li> <p><a href="#optask" class="MCXref xref">OpTask</a> </p> </li> 
    </ul> </td> 
   <td> 
    <ul> 
     <li> <p><a href="#project" class="MCXref xref">프로젝트</a> </p> </li> 
     <li> <p><a href="#proofapproval" class="MCXref xref">증명 승인</a> </p> </li> 
     <li> <p><a href="#queuedef" class="MCXref xref">QueueDef</a> </p> </li> 
     <li> <p><a href="#task" class="MCXref xref">작업</a> </p> </li> 
     <li> <p><a href="#team" class="MCXref xref">팀</a> </p> </li> 
     <li> <p><a href="#timesheet" class="MCXref xref">타임시트</a> </p> </li> 
     <li> <p><a href="#timesheetprofile" class="MCXref xref">작업표 프로필</a> </p> </li> 
     <li> <p><a href="#uitemplate" class="MCXref xref">UITemplate</a> </p> </li> 
     <li> <p><a href="#userdelegation" class="MCXref xref">사용자 위임</a> </p> </li> 
     <li> <p><a href="#work" class="MCXref xref">작업 </a> </p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

### AccessLevel {#accesslevel}

AccessLevel 개체는 사용자와 연결되며 사용자가 액세스할 수 있는 항목을 결정하는 AccessLevelPermissions 집합을 설명합니다.

액세스 수준에 대한 자세한 내용은 [액세스 수준 작동 방식](../../administration-and-setup/add-users/access-levels-and-object-permissions/access-levels.md).

<table style="table-layout:auto"> 
 <col data-mc-conditions=""> 
 <col data-mc-conditions=""> 
 <tbody> 
  <tr> 
   <td> <p>직접 필드</p> </td> 
   <td> 
    <ul> 
     <li> <p><b>설명</b> </p> <p>설명 길이가 4000자를 넘지 않도록 지정하는 유효성 검사기 MAX_LENGTH가 추가되었습니다.</p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

### BreadCrumb {#breadcrumb}

BreadCrumb 개체는 Workfront 작업 항목의 부모/자식 계층에 있는 요소를 나타냅니다. 탐색 표시는 작업 항목이 Portfolio, 프로젝트, 프로젝트 및 작업의 더 큰 구조에 어떻게 적합한지 나타냅니다.

탐색 표시에 대한 자세한 내용은 [새 Adobe Workfront 경험의 탐색 표시 개요](../../workfront-basics/the-new-workfront-experience/breadcrumb-overview.md)

<table style="table-layout:auto"> 
 <col data-mc-conditions=""> 
 <col data-mc-conditions=""> 
 <tbody> 
  <tr> 
   <td> <p>직접 필드</p> </td> 
   <td> 
    <ul> 
     <li> <p><b>objCode</b> </p> <p>개체 코드는 <a href="../../wf-api/general/api-explorer.md" class="MCXref xref">API 탐색기</a>.</p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

### BurndownEvent {#burndownevent}

BurndownEvent 개체는 반복의 번다운을 변경하는 개체를 나타냅니다.

번다운에 대한 자세한 내용은 [번다운](../../agile/use-scrum-in-an-agile-team/burndown/burndown.md).

<table style="table-layout:auto"> 
 <col data-mc-conditions=""> 
 <col data-mc-conditions=""> 
 <tbody> 
  <tr> 
   <td> <p>직접 필드</p> </td> 
   <td> <p>다음 필드에서 NOT_GROUPABLE 플래그를 제거했습니다. </p> 
    <ul> 
     <li> <p>applyDate</p> </li> 
     <li> <p>entryDate</p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

### 고객 기본 설정 {#customerpreferences}

CustomerPreferences 개체는 고객이 Workfront 인스턴스에 대해 설정한 환경 설정 집합을 나타냅니다.

<table style="table-layout:auto"> 
 <col data-mc-conditions=""> 
 <col data-mc-conditions=""> 
 <tbody> 
  <tr> 
   <td>직접 필드</td> 
   <td> 
    <ul> 
     <li style="font-weight: bold;"> <p>이름</p> <p style="font-weight: normal;">가능한 값을 추가했습니다.</p> 
      <ul> 
       <li style="font-weight: normal;">암호:aemAPIKey(config.general.aem.apikey)</li> 
       <li style="font-weight: normal;"> 암호:aemAADomain(config.general.aem.aadomain) </li> 
       <li style="font-weight: normal;">암호:aemIntegrationEnabled(config.general.aem.enabled)</li> 
       <li style="font-weight: normal;">암호:aemHost (config.general.aem.host)</li> 
       <li style="font-weight: normal;">작업표:default.작업표.restrict.작업표.edit.owners.admins (config.작업표.restrict.workbench.edit.owners.admins)</li> 
      </ul> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>액션</td> 
   <td> <p>다음 작업이 CustomerPreferences 리소스에 추가되었습니다.</p> 
    <ul> 
     <li> <p><b>getTimesetPreferences</b> </p> </li> 
     <li> <p><b>setTimesetPreferences</b> </p> <p>인수를 수행합니다.</p> 
      <ul> 
       <li> <p>환경 설정(맵)</p> </li> 
      </ul> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

### DocumentVersion {#documentversion}

DocumentVersion 개체는 파일(예: 문서 자료, 이미지 또는 기타 정보 형식)의 특정 버전을 나타냅니다.

문서 버전에 대한 자세한 내용은 [문서의 새 버전 업로드](../../documents/managing-documents/upload-new-document-version.md).

<table style="table-layout:auto"> 
 <col data-mc-conditions=""> 
 <col data-mc-conditions=""> 
 <tbody> 
  <tr> 
   <td> <p>직접 필드</p> </td> 
   <td> 
    <ul> 
     <li> <p><b>externalIntegrationType</b> </p> <p>가능한 값을 추가했습니다.</p> 
      <ul> 
       <li> <p>AEM (Adobe Experience Manager)</p> </li> 
      </ul> </li> 
    </ul> 
    <ul> 
     <li> <p><b>proofID</b> </p> <p>NOT_FILTERABLE 플래그가 추가되었습니다.</p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

### 그룹  {#group}

그룹 개체는 사용자 및 팀 집합을 나타냅니다. 그룹은 종종 부서별 구조를 나타냅니다.

그룹에 대한 자세한 내용은 [Adobe Workfront의 그룹과 팀](../../people-teams-and-groups/work-with-groups-and-teams/understanding-differences-and-similarities-between-groups-and-teams.md).

<table style="table-layout:auto"> 
 <col data-mc-conditions=""> 
 <col data-mc-conditions=""> 
 <tbody> 
  <tr> 
   <td> <p>액션</p> </td> 
   <td> 
    <ul> 
     <li> <p><b>getParent</b> </p> <p>이 작업은 그룹의 상위 그룹(해당 그룹이 의 하위 그룹인 그룹)의 배열을 반환합니다.</p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

### 분개 입력 {#journalentry}

JournalEntry 개체는 해당 필드가 수정될 때마다 특정 개체 필드에 대한 정보를 기록하도록 설정할 수 있습니다. 필드를 분개 입력 객체의 일부로 기록하도록 설정하면 해당 필드가 수정될 때마다 해당 분개 항목이 생성됩니다.

JournalEntry 리소스가 REPORTABLE 플래그를 추가했습니다.

<table style="table-layout:auto"> 
 <col data-mc-conditions=""> 
 <col data-mc-conditions=""> 
 <tbody> 
  <tr> 
   <td> <p>직접 필드</p> </td> 
   <td> <p>다음 필드에서 NOT_GROUPABLE 플래그를 제거했습니다.</p> 
    <ul> 
     <li> <p><b>changeType</b> </p> </li> 
     <li> <p><b>entryDate</b> </p> </li> 
     <li> <p><b>fieldName</b> </p> </li> 
     <li> <p><b>objObjCode</b> </p> </li> 
    </ul> <p>다음 필드에 NOT_FILTERABLE 플래그가 추가되었습니다.</p> 
    <ul> 
     <li> <p><b>subObjCode</b> </p> </li> 
     <li> <p><b>subObjID</b> </p> </li> 
     <li> <p><b>topObjCode</b> </p> </li> 
     <li> <p><b>topObjID</b> </p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

### 레이아웃 템플릿 {#layouttemplate}

Adobe Workfront 관리자 또는 그룹 관리자는 템플릿을 만들어 Adobe Workfront의 레이아웃 요소를 사용자 지정할 수 있습니다. LayoutTemplate 개체는 Adobe Workfront Classic에만 해당됩니다.

새 Adobe Workfront 경험의 레이아웃 템플릿을 나타내는 개체의 경우 [UITemplate](#uitemplate)

<table style="table-layout:auto"> 
 <col data-mc-conditions=""> 
 <col data-mc-conditions=""> 
 <tbody> 
  <tr> 
   <td> <p>직접 필드</p> </td> 
   <td> 
    <ul> 
     <li> <p><b>설명</b> </p> <p>설명 길이가 4000자를 넘지 않도록 지정하는 유효성 검사기 MAX_LENGTH가 추가되었습니다.</p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

### LinkedFolder {#linkedfolder}

LinkedFolder 개체는 Google 드라이브나 Dropbox과 같은 외부 문서 공급자에서 연결된 폴더를 나타냅니다.

링크된 폴더에 대한 자세한 내용은 [외부 응용 프로그램에서 문서 연결](../../documents/adding-documents-to-workfront/link-documents-from-external-apps.md).

<table style="table-layout:auto"> 
 <col data-mc-conditions=""> 
 <col data-mc-conditions=""> 
 <tbody> 
  <tr> 
   <td> <p>직접 필드</p> </td> 
   <td> 
    <ul> 
     <li> <p><b>externalIntegrationType</b> </p> <p>가능한 값을 추가했습니다.</p> 
      <ul> 
       <li> <p>AEM (Adobe Experience Manager)</p> </li> 
      </ul> </li> 
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
   <td> <p>필드 검색</p> </td> 
   <td> 
    <ul> 
     <li> <p><b>favoritedByUsersMM</b> </p> </li> 
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

### 증명 승인 {#proofapproval}

ProofApproval 개체는 증명에 직접 연결된 승인을 나타냅니다.

<table style="table-layout:auto"> 
 <col data-mc-conditions=""> 
 <col data-mc-conditions=""> 
 <tbody> 
  <tr> 
   <td> <p>직접 필드</p> </td> 
   <td> <p>다음 필드가 ProofApproval 리소스에 추가되었습니다.</p> 
    <ul> 
     <li> <p><b>승인자 단계</b> </p> </li> 
     <li> <p><b>의사 결정 날짜</b> </p> </li> 
     <li> <p><b>workflowTemplate</b> </p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

### QueueDef {#queuedef}

QueueDef 개체는 사용자가 문제를 해당 항목에 제출할 수 있도록 도움말 데스크 영역에 게시된 프로젝트인 Queue를 나타냅니다.

요청 큐에 대한 자세한 내용은 [요청 큐 만들기](../../manage-work/requests/create-and-manage-request-queues/create-request-queue.md).

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">직접 필드</td> 
   <td> 
    <ul> 
     <li> <p><b>documentPosition</b> </p> <p>추가됨. 가능한 값은 다음과 같습니다.</p> 
      <ul> 
       <li> <p>0(사용자 지정 양식 후)</p> </li> 
       <li> <p>1(사용자 지정 양식 전)</p> </li> 
      </ul> </li> 
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
   <td> <p>필드 검색</p> </td> 
   <td> 
    <ul> 
     <li> <p><b>favoritedByUsersMM</b> </p> </li> 
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

### 타임시트 {#timesheet}

작업표 개체는 사용자가 작업, 프로젝트 및 오버헤드 시간 유형에 대해 실제 작업 시간을 입력할 수 있도록 하는 가상 타임카드를 나타냅니다.

<table style="table-layout:auto"> 
 <col data-mc-conditions=""> 
 <col data-mc-conditions=""> 
 <tbody> 
  <tr> 
   <td>직접 필드</td> 
   <td> 
    <ul> 
     <li> <p><b>isTimeoutDisabled</b> </p> <p>추가됨</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>핵심 필드</td> 
   <td> 
    <ul> 
     <li> <p><b>objCode</b> </p> <p>제거됨</p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

### 작업표 프로필 {#timesheetprofile}

작업표 개체는 사용자가 작업, 프로젝트 및 오버헤드 시간 유형에 대해 실제 작업 시간을 입력할 수 있도록 하는 가상 타임카드를 나타냅니다.

<table style="table-layout:auto"> 
 <col data-mc-conditions=""> 
 <col data-mc-conditions=""> 
 <tbody> 
  <tr> 
   <td>직접 필드</td> 
   <td> 
    <ul> 
     <li> <p><b>isTimeoutDisabled</b> </p> <p>추가됨</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>기본 필드</td> 
   <td> 
    <ul> 
     <li> <p><b>isTimeoutDisabled</b> </p> <p>추가됨</p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

### UITemplate {#uitemplate}

Adobe Workfront 관리자 또는 그룹 관리자는 템플릿을 만들어 Adobe Workfront의 레이아웃 요소를 사용자 지정할 수 있습니다. LayoutTemplate 개체는 새 Adobe Workfront 경험에만 해당됩니다.

Adobe Workfront Classic의 레이아웃 템플릿을 나타내는 개체의 경우 [레이아웃 템플릿](#layouttemplate).

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">액션</td> 
   <td> <p>다음 작업이 UITemplate 리소스에 추가되었습니다.</p> 
    <ul> 
     <li> <p><b>migrateCustomersAllLayoutTemplates</b> </p> <p>인수를 수행합니다.</p> 
      <ul> 
       <li> <p>overrideIfExists(부울)</p> </li> 
      </ul> </li> 
     <li> <p><b>migrateLayoutTemplates</b> </p> <p>인수를 사용합니다.</p> 
      <ul> 
       <li> <p>layoutTemplateIDs (string[])</p> </li> 
       <li> <p>overrideIfExists(부울)</p> </li> 
      </ul> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

### 사용자 위임 {#userdelegation}

UserDelegation 개체는 특정 기간 동안 한 사용자로부터 다른 사용자로 작업을 위임하는 동작을 나타냅니다.

UserDelegation 개체가 REPORTABLE 플래그를 추가했습니다.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">직접 필드</td> 
   <td> <p>다음 필드에서 NOT_GROUPABLE 플래그를 제거했습니다.</p> 
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

작업 개체는 Task 및 OpTask가 모두 상속하고 두 Task 간에 공통 코드를 공유하는 공통 인터페이스입니다.

<table style="table-layout:auto"> 
 <col data-mc-conditions=""> 
 <col data-mc-conditions=""> 
 <tbody> 
  <tr> 
   <td> <p>필드 검색</p> </td> 
   <td> 
    <ul> 
     <li> <p><b>favoritedByUsersMM</b> </p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>
