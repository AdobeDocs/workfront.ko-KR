---
content-type: api
navigation-topic: api-navigation-topic
title: API 버전 14의 새로운 기능
description: Adobe Workfront은 2021년 9월 9일에 API 버전 14를 릴리스했습니다. API 버전 14는 버전 14에서 다음과 같은 변경 사항을 제공합니다.
author: John
feature: Workfront API
exl-id: eca5d1cc-6348-445c-be84-c0a29f15980d
source-git-commit: f2f825280204b56d2dc85efc7a315a4377e551c7
workflow-type: tm+mt
source-wordcount: '881'
ht-degree: 2%

---

# API 버전 14의 새로운 기능

Adobe Workfront은 2021년 9월 9일에 API 버전 14를 릴리스했습니다. API 버전 14는 버전 14에서 다음과 같은 변경 사항을 제공합니다.

## 리소스를 추가했습니다.

API 버전 14에 대한 리소스가 추가되지 않았습니다.

## 제거된 리소스

API 버전 14에 대해 제거된 리소스가 없습니다.

## 수정된 리소스

다음 리소스가 API 버전 14에 대해 수정되었습니다.

* [청구 레코드(BOM)](#billingrecord-bill)
* [카테고리(CTGY)](#category-ctgy)
* [CustomEnum(CSTEM)](#customenum-cstem)
* [고객(CUST)](#customer-cust)
* [고객 기본 설정(CUSTOMER)](#customerpreferences-custpr)
* [DocumentVersion(DOCV)](#documentversion-docv)
* [그룹(그룹)](#group-group)
* [참고 태그(NTAG)](#notetag-ntag)
* [프로젝트(PROJ)](#project-proj)
* [QueueDef(QUED)](#queuedef-qued)
* [리소스 할당(RSALLO)](#resource-allocation-rsallo)
* [역할(역할)](#role-role)
* [템플릿(TMPL)](#template-tmpl)
* [작업표(TSHET)](#timesheet-tshet)

### 청구 레코드(BOM) {#billingrecord-bill}

BillingRecord 개체는 청구할 수 있는 수익, 시간 또는 비용을 기록합니다. 이 정보는 외부 회계 시스템에서 송장을 생성하는 데 사용할 수 있습니다.

청구 레코드에 대한 자세한 내용은 [청구 레코드 만들기](../../manage-work/projects/project-finances/create-billing-records.md).

BillingRecord 개체가 플래그를 추가했습니다. **DATA_EXTENSION**.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <p role="rowheader">직접 필드</p> </td> 
   <td> 
    <ul> 
     <li> <p><b>categoryID</b> </p> <p>추가됨. 카테고리는 사용자 지정 양식입니다. 이 매개 변수는 BillingRecord 개체에 사용자 지정 Forms을 추가하는 기능을 지원하기 위해 추가되었습니다.</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">참조 필드</td> 
   <td> 
    <ul> 
     <li> <p><b>카테고리</b> </p> <p>추가됨. 카테고리는 사용자 지정 양식입니다. 이 매개 변수는 BillingRecord 개체에 사용자 지정 양식을 추가하는 기능을 지원하기 위해 추가되었습니다.</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">컬렉션 필드</td> 
   <td> 
    <ul> 
     <li> <p><b>objectCategories</b> </p> <p>추가됨. 이는 BillingRecord 개체와 연결된 카테고리(사용자 지정 양식)의 컬렉션을 나타냅니다.</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">액션</td> 
   <td> 
    <ul> 
     <li> <p><b>calculateDataExtension</b> </p> <p>추가됨. 이 작업은 사용자 지정 양식 필드의 표현식을 다시 계산합니다.</p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

### 카테고리(CTGY) {#category-ctgy}

Category 개체는 사용자 지정 양식입니다.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">직접 필드</td> 
   <td> 
    <ul> 
     <li> <p><b>catObjCode</b> </p> <p>가능한 값을 추가했습니다.</p> 
      <ul> 
       <li> <p> 청구(청구 레코드)</p> </li> 
      </ul> <p>이 값은 BillingRecord 개체에 사용자 지정 양식을 추가하는 기능을 지원하기 위해 추가되었습니다.</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">액션</td> 
   <td> 
    <ul> 
     <li> <p><b>isObjectFroundInPendingApprovalStatus</b> </p> <p>이 작업은 매개 변수 objID 및 objCode를 가져와 부울을 반환합니다.</p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

### CustomEnum(CSTEM) {#customenum-cstem}

CustomEnum 개체는 상태 코드를 사람이 읽을 수 있는 텍스트로 변환하는 데 도움이 됩니다.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">쿼리</td> 
   <td> 
    <ul> 
     <li> <p><b>getGroupStatus</b> </p> <p>추가됨. 이 쿼리는 그룹 및 하위 그룹의 상태를 만들고 관리하는 기능을 지원합니다. </p> <p>자세한 내용은 <a href="../../administration-and-setup/manage-groups/manage-group-statuses/manage-group-statuses.md" class="MCXref xref">그룹 상태 관리</a>.</p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

### 고객(CUST) {#customer-cust}

고객 개체는 Workfront 인스턴스를 사용하는 조직을 나타냅니다.

내부 개체입니다.

### 고객 기본 설정(CUSTOMER) {#customerpreferences-custpr}

CustomerPreferences 개체는 고객이 Workfront 인스턴스에 대해 설정한 환경 설정 집합을 나타냅니다.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">직접 필드</td> 
   <td> 
    <ul> 
     <li> <p><b>이름</b> </p> <p>가능한 값을 추가했습니다.</p> 
      <ul> 
       <li> <p>사용자가 업데이트에서 이미지를 추가할 수 있도록 허용(업데이트:images.toggle)</p> </li> 
      </ul> <p>이 매개 변수는 작업 항목 업데이트에 이미지를 추가하는 기능을 지원합니다. </p> <p>자세한 내용은 <a href="../../workfront-basics/updating-work-items-and-viewing-updates/update-work.md" class="MCXref xref">작업 업데이트</a>.</p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

### DocumentVersion(DOCV) {#documentversion-docv}

DocumentVersion 개체는 파일(예: 문서 자료, 이미지 또는 기타 정보 형식)의 특정 버전을 나타냅니다.

문서 버전에 대한 자세한 내용은 [문서의 새 버전 업로드](../../documents/managing-documents/upload-new-document-version.md).

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">직접 필드</td> 
   <td> 
    <ul> 
     <li> <p><b>lastCallbackDate</b> </p> <p>추가됨. 이 필드는 버전이 증명과 연관된 경우 Workfront 증명의 마지막 콜백의 날짜 및 시간을 기록합니다.</p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

### 그룹(그룹) {#group-group}

그룹 개체는 사용자 및 팀 집합을 나타냅니다. 그룹은 종종 부서별 구조를 나타냅니다.

그룹에 대한 자세한 내용은 [Adobe Workfront의 그룹과 팀](../../people-teams-and-groups/work-with-groups-and-teams/understanding-differences-and-similarities-between-groups-and-teams.md).

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">액션</td> 
   <td> 
    <ul> 
     <li> <p><b>addSubgroups</b> </p> <p>추가됨. 이 작업은 그룹 ID 배열을 취하여 해당 그룹을 지정된 그룹에 하위 그룹으로 추가합니다.</p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

### 참고 태그(NTAG) {#notetag-ntag}

NoteTag 개체는 작업 항목에 대한 업데이트에서 사용자 또는 팀에 태깅하는 작업을 나타냅니다.

업데이트에서의 태깅에 대한 자세한 내용은 [업데이트에 다른 사용자에게 태그 지정](../../workfront-basics/updating-work-items-and-viewing-updates/tag-others-on-updates.md).

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">작업</td> 
   <td> <p>다음 작업이 NoteTag 개체에 추가되었습니다.</p> 
    <ul> 
     <li> <p><b>카운트</b> </p> </li> 
     <li> <p><b>GET</b> </p> </li> 
     <li> <p><b>보고서</b> </p> </li> 
     <li> <p><b>검색</b> </p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

### 프로젝트(PROJ) {#project-proj}

프로젝트는 Workfront 내의 작업 항목이며, Workfront이 사람들이 작업을 수행하는 데 도움이 되는 기본 빌딩 블록입니다. 프로젝트 객체는 공통, 특정 목표를 가진 작업 그룹을 나타냅니다.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">액션</td> 
   <td> 
    <ul> 
     <li> <p><b>updateBusinessCaseSource</b> </p> <p>추가됨.</p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

### QueueDef(QUED) {#queuedef-qued}

QueueDef 개체는 사용자가 문제를 해당 대기열에 제출할 수 있도록 도움말 데스크 영역에 게시된 프로젝트인 Queue를 나타냅니다.

요청 큐에 대한 자세한 내용은 [요청 큐 만들기](../../manage-work/requests/create-and-manage-request-queues/create-request-queue.md).

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">액션</td> 
   <td> 
    <ul> 
     <li> <p><b>searchByPath</b> </p> <p>추가됨. 이 작업은 요청 큐 및 주제 그룹을 통해 경로를 사용하여 요청을 찾는 기능을 지원합니다.</p> <p>경로별 요청 큐 검색에 대한 자세한 내용은 <a href="../../manage-work/requests/create-requests/create-submit-requests.md#create-requests-in-the-web-app" class="MCXref xref">Workfront 웹 앱에서 요청 만들기 및 초안 생성</a> in <a href="../../manage-work/requests/create-requests/create-submit-requests.md" class="MCXref xref">Adobe Workfront 요청 만들기 및 제출</a>.</p> </li> 
    </ul> <p> </p> </td> 
  </tr> 
 </tbody> 
</table>

### 리소스 할당(RSALLO) {#resource-allocation-rsallo}

리소스 할당 개체는 주어진 프로젝트에 필요한 예상 리소스를 나타냅니다. 이 객체는 레거시 리소스 계획자에서만 사용됩니다. 새 자원 계획자의 해당 필드에 대해 BGHR(예산책정된 시간)을 사용합니다.

리소스 할당 개체가 플래그를 제거했습니다. **REPORTTABLE**.

### 역할(역할) {#role-role}

역할 객체(작업 역할)는 사용자가 채울 수 있는 기능 능력 또는 기술 세트(예: 디자이너 또는 제품 관리자)를 나타냅니다.

작업 역할에 대한 자세한 내용은 [작업 역할 개요](../../administration-and-setup/set-up-workfront/organizational-setup/job-role-overview.md).

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">직접 필드</td> 
   <td> 
    <ul> 
     <li style="font-weight: bold;"> <p>isActive</p> <p style="font-weight: normal;">추가됨. 객체가 활성 상태인 경우 true 값을 갖는 부울 매개 변수입니다. 그렇지 않은 경우 false 값을 갖습니다. 활성(Active)으로 설정된 객체는 드롭다운 메뉴 및 미리 입력 필드에 표시되며 다른 객체에 첨부할 수 있습니다.</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">기본 필드</td> 
   <td> 
    <ul> 
     <li style="font-weight: bold;"> <p>isActive</p> <p style="font-weight: normal;">추가됨</p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

### 템플릿(TMPL) {#template-tmpl}

Template 객체는 프로젝트의 패턴을 나타냅니다. 템플릿을 통해 프로젝트를 만들어 시간을 절약할 수 있습니다. 템플릿에는 팀 및 작업이 포함되어 있으며, 이 작업은 템플릿에서 만든 프로젝트에 복사됩니다.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">직접 필드</td> 
   <td> 
    <ul> 
     <li style="font-weight: bold;"> <p>groupID</p> <p style="font-weight: normal;">추가됨. 이 필드는 그룹과 템플릿을 연결하는 기능을 지원하기 위해 추가되었습니다.</p> <p style="font-weight: normal;">자세한 내용은 <a href="../../manage-work/projects/create-and-manage-templates/edit-templates.md" class="MCXref xref">프로젝트 템플릿 편집</a>.</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">참조 필드</td> 
   <td> 
    <ul> 
     <li style="font-weight: bold;"> <p>그룹</p> <p style="font-weight: normal;">추가됨. 이 필드는 그룹과 템플릿을 연결하는 기능을 지원하기 위해 추가되었습니다.</p> <p style="font-weight: normal;">자세한 내용은 <a href="../../manage-work/projects/create-and-manage-templates/edit-templates.md" class="MCXref xref">프로젝트 템플릿 편집</a>.</p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

<!--
<div data-mc-conditions="QuicksilverOrClassic.Draft mode">
<p><strong>Timesheet (TSHET)</strong></p>
<p>A&nbsp;Timesheet object represents a virtual timecard that allows users to enter actual hours worked for tasks, projects, and overhead hour types.</p>
<p>For more information, see <a href="../../timesheets/timesheets/timesheets-overview.md" class="MCXref xref">Timesheets overview</a>.</p>
<table style="table-layout:auto">
<col>
<col>
<tbody>
<tr>
<td role="rowheader">Core Fields</td>
<td>
<ul>
<li> <p><b>objCode</b> </p> <p>Removed.</p> </li>
</ul> </td>
</tr>
</tbody>
</table>
</div>
-->
