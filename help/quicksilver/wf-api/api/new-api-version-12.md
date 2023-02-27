---
content-type: api
navigation-topic: api-navigation-topic
title: API 버전 12의 새로운 기능
description: Workfront은 2020년 11월 12일에 API 버전 12를 릴리스했습니다. API 버전 12는 버전 11에서 다음과 같은 변경 사항을 제공합니다
author: Becky
feature: Workfront API
exl-id: 1ffba3b5-ab24-4ca2-a1ef-f7e5b77e776c
source-git-commit: f050c8b95145552c9ed67b549608c16115000606
workflow-type: tm+mt
source-wordcount: '2516'
ht-degree: 2%

---

# API 버전 12의 새로운 기능

Workfront은 2020년 11월 12일에 API 버전 12를 릴리스했습니다. API 버전 12는 버전 11에서 다음과 같은 변경 사항을 제공합니다

## 추가된 리소스

Workfront API 버전 12의 새로운 리소스는 다음과 같습니다.

* [BreadCrumb](#breadcrumb)
* [RichTextParameterValue](#richtextparametervalue)

### BreadCrumb {#breadcrumb}

BreadCrumb 개체는 Adobe Workfront 작업 항목의 부모/자식 계층에 있는 요소를 나타냅니다. 탐색 표시는 작업 항목이 Portfolio, 프로젝트, 프로젝트 및 작업의 더 큰 구조에 어떻게 적합한지 나타냅니다.

Workfront의 탐색 표시에 대한 자세한 내용은 [새 Adobe Workfront 경험의 탐색 표시 개요](../../workfront-basics/the-new-workfront-experience/breadcrumb-overview.md)

<table style="table-layout:auto"> <!--
  <col data-mc-conditions="QuicksilverOrClassic.Draft mode">
 --> <!--
  <col data-mc-conditions="QuicksilverOrClassic.Draft mode">
 --> 
 <tbody> 
  <tr> 
   <td>개 액션</td> 
   <td> 
    <ul> 
     <li style="font-weight: bold;">getObjectHierarchy</li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

### RichTextParameterValue {#richtextparametervalue}

이제 더 많은 개체에서 리치 텍스트 필드를 사용할 수 있습니다. 이 가용성을 지원하기 위해 RichTextParameterValue 개체가 Workfront에 추가되었습니다.

자세한 내용은 [Adobe Workfront API의 리치 텍스트 필드](../../wf-api/general/rich-text-field-api.md).

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
     <li style="font-weight: bold;">ID</li> 
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

## 제거된 리소스

API 버전 12에 대해 제거된 리소스가 없습니다.

## 수정된 리소스

Workfront API 버전 12에 대해 다음 리소스가 수정되었습니다.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"> 
    <ul> 
     <li> <p><a href="#accesslevel" class="MCXref xref">AccessLevel</a> </p> </li> 
     <li> <p><a href="#accesslevelpermissions" class="MCXref xref">AccessLevelPermissions</a> </p> </li> 
     <li> <p><a href="#accessrequest" class="MCXref xref">AccessRequest</a> </p> </li> 
     <li> <p><a href="#accessrule" class="MCXref xref">AccessRule</a> </p> </li> 
     <li> <p><a href="#activitylog" class="MCXref xref">ActivityLog</a> </p> </li> 
     <li> <p><a href="#announcementattachment" class="MCXref xref">공지 첨부 파일</a> </p> </li> 
     <li> <p><a href="#approval" class="MCXref xref">승인</a> </p> </li> 
     <li> <p><a href="#calendarsection" class="MCXref xref">CalendarSection</a> </p> </li> 
     <li> <p><a href="#company" class="MCXref xref">회사</a> </p> </li> 
     <li> <p><a href="#customer" class="MCXref xref">고객</a> </p> </li> 
    </ul> </td> 
   <td> 
    <ul> 
     <li> <p><a href="#customerpreferences" class="MCXref xref">고객 기본 설정</a> </p> </li> 
     <li> <p><a href="#document" class="MCXref xref">문서</a> </p> </li> 
     <li> <p><a href="#documentversion" class="MCXref xref">DocumentVersion</a> </p> </li> 
     <li> <p><a href="#group" class="MCXref xref">그룹 </a> </p> </li> 
     <li> <p><a href="#linkedfolder" class="MCXref xref">LinkedFolder</a> </p> </li> 
     <li> <p><a href="#optask" class="MCXref xref">OpTask</a> </p> </li> 
     <li> <p><a href="#parameter" class="MCXref xref">매개변수</a> </p> </li> 
     <li> <p><a href="#portfolio" class="MCXref xref">포트폴리오</a> </p> </li> 
     <li> <p><a href="#program" class="MCXref xref">프로그램</a> </p> </li> 
    </ul> </td> 
   <td> 
    <ul> 
     <li> <p><a href="#queuedef" class="MCXref xref">QueueDef</a> </p> </li> 
     <li> <p><a href="#scheduledreport" class="MCXref xref">예약된 보고서</a> </p> </li> 
     <li> <p><a href="#scorecardquestion" class="MCXref xref">ScoreCardQuestion</a> </p> </li> 
     <li> <p><a href="#task" class="MCXref xref">작업</a> </p> </li> 
     <li> <p><a href="#team" class="MCXref xref">팀</a> </p> </li> 
     <li> <p><a href="#templatetask" class="MCXref xref">TemplateTask</a> </p> </li> 
     <li> <p><a href="#timesheet" class="MCXref xref">타임시트</a> </p> </li> 
     <li> <p><a href="#user" class="MCXref xref">사용자</a> </p> </li> 
     <li> <p><a href="#work" class="MCXref xref">작업 </a> </p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

 

### AccessLevel {#accesslevel}

AccessLevel 개체는 사용자와 연결되며 사용자가 액세스할 수 있는 항목을 결정하는 AccessLevelPermissions 집합을 설명합니다.

액세스 수준에 대한 자세한 내용은 [액세스 수준 작동 방식](../../administration-and-setup/add-users/access-levels-and-object-permissions/access-levels.md).

<table style="table-layout:auto"> <!--
  <col data-mc-conditions="QuicksilverOrClassic.Draft mode">
 --> <!--
  <col data-mc-conditions="QuicksilverOrClassic.Draft mode">
 --> 
 <tbody> 
  <tr> <!--
    <td data-mc-conditions="QuicksilverOrClassic.Draft mode">Direct Fields</td>
   --> 
   <td> 
    <ul> 
     <li style="font-weight: bold;"> <!--
       <p data-mc-conditions="QuicksilverOrClassic.Draft mode">fieldAccessPrivileges</p>
      --> <!--
       <p style="font-weight: normal;" data-mc-conditions="QuicksilverOrClassic.Draft mode">Added the possible value CPJ (Copy). This allows Users with Planner Access Level to copy Projects.</p>
      --> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

### AccessLevelPermissions {#accesslevelpermissions}

AccessLevelPermissions 개체는 Workfront 개체에 액세스, 만들기 또는 수정하기 위한 특정 권한을 나타냅니다. 그런 다음 액세스 수준과 연결할 수 있습니다.

<table style="table-layout:auto"> 
 <col data-mc-conditions=""> 
 <col data-mc-conditions=""> 
 <tbody> 
  <tr> 
   <td>직접 필드</td> 
   <td> 
    <ul> 
     <li> <p><strong>coreAction</strong> </p> <p>다음 possibleValues가 추가되었습니다.</p> 
      <ul> 
       <li> <p>PLANNING_HOURS_CONTOLING </p> <p>이 권한을 포함하는 액세스 수준을 가진 사용자는 작업 로드 밸런서에서 계획 시간을 업데이트할 수 있습니다.</p> <p>자세한 내용은 <a href="../../resource-mgmt/workload-balancer/manage-user-allocations-workload-balancer.md#update" class="MCXref xref">사용자 할당을 관리할 때 작업 계획 시간 업데이트</a> in <a href="../../resource-mgmt/workload-balancer/manage-user-allocations-workload-balancer.md" class="MCXref xref">작업 로드 밸런서에서 사용자 할당 관리</a>.</p> </li> 
       <li> <p>ADD_TO_CUSTOM_FORMS. </p> <p>이 권한을 포함하는 액세스 수준을 가진 사용자는 사용자 지정 양식에 필드를 추가할 수 있습니다.</p> <p>자세한 내용은 <a href="../../administration-and-setup/customize-workfront/create-manage-custom-forms/create-or-edit-a-custom-form.md#add2" class="MCXref xref"></a> in <a href="../../administration-and-setup/customize-workfront/create-manage-custom-forms/create-or-edit-a-custom-form.md" class="MCXref xref">사용자 지정 양식 만들기 또는 편집</a>.</p> </li> 
       <li> <p>EDIT_SYSTEMWIDE </p> <p>이 권한을 포함하는 액세스 수준을 가진 사용자는 사용자 정의 필드 시스템 전체를 삭제 액세스와 공유할 수 있습니다.</p> <p>자세한 내용은 <a href="../../administration-and-setup/customize-workfront/create-manage-custom-forms/configure-sharing-for-a-custom-field.md" class="MCXref xref">사용자 지정 필드 및 위젯에 대한 공유 구성</a>.</p> </li> 
      </ul> </li> 
     <li> <p><strong>forbiddenActions</strong> </p> <p>다음 possibleValues가 추가되었습니다.</p> 
      <ul> 
       <li> <p>PLANNING_HOURS_CONTOLING </p> </li> 
       <li> <p>ADD_TO_CUSTOM_FORMS. </p> </li> 
       <li> <p>EDIT_SYSTEMWIDE </p> </li> 
      </ul> </li> 
     <li> <p><strong>secondaryActions</strong> </p> <p>다음 possibleValues가 추가되었습니다.</p> 
      <ul> 
       <li> <p>PLANNING_HOURS_CONTOLING </p> </li> 
       <li> <p>ADD_TO_CUSTOM_FORMS. </p> </li> 
       <li> <p>EDIT_SYSTEMWIDE </p> </li> 
      </ul> </li> 
    </ul> <!--
     <p data-mc-conditions="QuicksilverOrClassic.Draft mode">OR</p>
    --> <!--
     <p data-mc-conditions="QuicksilverOrClassic.Draft mode">The following fields added the possible value PLANNED_HOURS_CONTOURING, which allows a user to update planned hours in the Workload Balancer</p>
    --> 
    <ul> 
     <li> <!--
       <p data-mc-conditions="QuicksilverOrClassic.Draft mode">coreAction</p>
      --> </li> 
     <li> <!--
       <p data-mc-conditions="QuicksilverOrClassic.Draft mode">forbiddenActions</p>
      --> </li> 
     <li> <!--
       <p data-mc-conditions="QuicksilverOrClassic.Draft mode">secondaryActions</p>
      --> </li> 
    </ul> <!--
     <p data-mc-conditions="QuicksilverOrClassic.Draft mode">The following fields added the possible value ADD_TO_CUSTOM_FORMS, which allows a user to add fields to custom forms.</p>
    --> 
    <ul> 
     <li> <!--
       <p data-mc-conditions="QuicksilverOrClassic.Draft mode">coreAction</p>
      --> </li> 
     <li> <!--
       <p data-mc-conditions="QuicksilverOrClassic.Draft mode">forbiddenActions</p>
      --> </li> 
     <li> <!--
       <p data-mc-conditions="QuicksilverOrClassic.Draft mode">secondaryActions</p>
      --> </li> 
    </ul> <!--
     <p data-mc-conditions="QuicksilverOrClassic.Draft mode">The following fields added the possible value EDIT_SYSTEMWIDE, which allows a user to share a custom field system-wide with Delete access. </p>
    --> <!--
     <ul data-mc-conditions="QuicksilverOrClassic.Draft mode"> 
      <li> <p>coreAction</p> </li> 
      <li> <p>forbiddenActions</p> </li> 
      <li> <p>secondaryActions</p> </li> 
     </ul>
    --> </td> 
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
     <li> <p style="font-weight: bold;">작업</p> <p>다음 possibleValues가 추가되었습니다.</p> 
      <ul> 
       <li> <p>PLANNING_HOURS_CONTOLING </p> <p>이 권한을 포함하는 액세스 수준을 가진 사용자는 작업 로드 밸런서에서 계획 시간을 업데이트할 수 있습니다.</p> <p>자세한 내용은 <a href="../../resource-mgmt/workload-balancer/manage-user-allocations-workload-balancer.md#update" class="MCXref xref">사용자 할당을 관리할 때 작업 계획 시간 업데이트</a> in <a href="../../resource-mgmt/workload-balancer/manage-user-allocations-workload-balancer.md" class="MCXref xref">작업 로드 밸런서에서 사용자 할당 관리</a>.</p> </li> 
       <li> <p>ADD_TO_CUSTOM_FORMS. </p> <p>이 권한을 포함하는 액세스 수준을 가진 사용자는 사용자 지정 양식에 필드를 추가할 수 있습니다.</p> <p>자세한 내용은 <a href="../../administration-and-setup/customize-workfront/create-manage-custom-forms/create-or-edit-a-custom-form.md#add2" class="MCXref xref"></a> in <a href="../../administration-and-setup/customize-workfront/create-manage-custom-forms/create-or-edit-a-custom-form.md" class="MCXref xref">사용자 지정 양식 만들기 또는 편집</a>.</p> </li> 
       <li> <p>EDIT_SYSTEMWIDE </p> <p>이 권한을 포함하는 액세스 수준을 가진 사용자는 사용자 정의 필드 시스템 전체를 삭제 액세스와 공유할 수 있습니다.</p> <p>자세한 내용은 <a href="../../administration-and-setup/customize-workfront/create-manage-custom-forms/configure-sharing-for-a-custom-field.md" class="MCXref xref">사용자 지정 필드 및 위젯에 대한 공유 구성</a>.</p> </li> 
      </ul> </li> 
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
   <td> 
    <ul> 
     <li><strong>coreAction</strong> <p>다음 possibleValues가 추가되었습니다.</p> 
      <ul> 
       <li> <p>PLANNING_HOURS_CONTOLING </p> <p>이 권한을 포함하는 액세스 수준을 가진 사용자는 작업 로드 밸런서에서 계획 시간을 업데이트할 수 있습니다.</p> <p>자세한 내용은 <a href="../../resource-mgmt/workload-balancer/manage-user-allocations-workload-balancer.md#update" class="MCXref xref">사용자 할당을 관리할 때 작업 계획 시간 업데이트</a> in <a href="../../resource-mgmt/workload-balancer/manage-user-allocations-workload-balancer.md" class="MCXref xref">작업 로드 밸런서에서 사용자 할당 관리</a>.</p> </li> 
       <li> <p>ADD_TO_CUSTOM_FORMS. </p> <p>이 권한을 포함하는 액세스 수준을 가진 사용자는 사용자 지정 양식에 필드를 추가할 수 있습니다.</p> <p>자세한 내용은 <a href="../../administration-and-setup/customize-workfront/create-manage-custom-forms/create-or-edit-a-custom-form.md#add2" class="MCXref xref"></a> in <a href="../../administration-and-setup/customize-workfront/create-manage-custom-forms/create-or-edit-a-custom-form.md" class="MCXref xref">사용자 지정 양식 만들기 또는 편집</a>.</p> </li> 
       <li> <p>EDIT_SYSTEMWIDE </p> <p>이 권한을 포함하는 액세스 수준을 가진 사용자는 사용자 정의 필드 시스템 전체를 삭제 액세스와 공유할 수 있습니다.</p> <p>자세한 내용은 <a href="../../administration-and-setup/customize-workfront/create-manage-custom-forms/configure-sharing-for-a-custom-field.md" class="MCXref xref">사용자 지정 필드 및 위젯에 대한 공유 구성</a>.</p> </li> 
      </ul> </li> 
     <li> <p><strong>forbiddenActions</strong> </p> <p>다음 possibleValues가 추가되었습니다.</p> 
      <ul> 
       <li> <p>PLANNING_HOURS_CONTOLING </p> </li> 
       <li> <p>ADD_TO_CUSTOM_FORMS. </p> </li> 
       <li> <p>EDIT_SYSTEMWIDE </p> </li> 
      </ul> </li> 
     <li> <p><strong>secondaryActions</strong> </p> <p>다음 possibleValues가 추가되었습니다.</p> 
      <ul> 
       <li> <p>PLANNING_HOURS_CONTOLING </p> </li> 
       <li> <p>ADD_TO_CUSTOM_FORMS. </p> </li> 
       <li> <p>EDIT_SYSTEMWIDE </p> </li> 
      </ul> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

### ActivityLog {#activitylog}

ActivityLog 개체는 지정된 Workfront 증명 계정에서 발생한 모든 활동의 전체 목록입니다.

<table style="table-layout:auto"> 
 <col data-mc-conditions=""> 
 <col data-mc-conditions=""> 
 <tbody> 
  <tr> 
   <td> <p>작업</p> </td> 
   <td> <p>ActivityLog 개체에서 다음 작업이 제거되었습니다.</p> 
    <ul> 
     <li> <p><strong>추가</strong> </p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

### 공지 첨부 파일 {#announcementattachment}

AnnouncementAttachment 개체는 Workfront 공지에 첨부된 파일을 나타냅니다.

발표 첨부 파일에 대한 자세한 내용은 [공지 보내기](../../administration-and-setup/get-started-wf-administration/view-send-announcements.md)

<table style="table-layout:auto"> 
 <col data-mc-conditions=""> 
 <col data-mc-conditions=""> 
 <tbody> 
  <tr> 
   <td> <p>직접 필드</p> </td> 
   <td> 
    <ul> 
     <li> <p><strong>fileExtension</strong> </p> <p>가능한 값을 추가했습니다.</p> 
      <ul> 
       <li> <p>qdoc(enum.fileextension.qdoc)</p> </li> 
       <li> <p>qslides(enum.fileextension.qslids)</p> </li> 
       <li> <p>qsheet(enum.fileextension.qsheet)</p> </li> 
      </ul> </li> 
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
   <td>직접 필드</td> 
   <td> 
    <ul> 
     <li> <p><strong>backlogOrder</strong> </p> <p>다음 플래그를 제거했습니다.</p> 
      <ul> 
       <li> <p>동적,</p> </li> 
       <li> <p>LAZY_READ,</p> </li> 
       <li> <p>NOT_GROUPABLE</p> </li> 
      </ul> </li> 
     <li> <p><strong>groupID</strong> </p> <p>다음 플래그가 추가되었습니다</p> 
      <ul> 
       <li> <p>AUTO_LOAD,</p> </li> 
       <li> <p>동적,</p> </li> 
       <li> <p>READ_ONLY</p> </li> 
      </ul> </li> 
     <li> <p><strong>workFuture</strong> </p> <p>이 필드가 추가되었으며 작업을 완료하는 데 사용자에게 작은 작업, 중간 작업 또는 많은 양의 노력이 필요하는지 여부를 나타냅니다. 가능한 값은 다음과 같습니다.</p> 
      <ul> 
       <li> <p>1 (작음)</p> </li> 
       <li> <p>2(중간)</p> </li> 
       <li> <p>3(큰)</p> </li> 
      </ul> <p>Workfront의 작업 수행에 대한 자세한 내용은 <a href="../../manage-work/tasks/task-information/work-effort.md" class="MCXref xref">작업 시간 개요</a>.</p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

### CalendarSection {#calendarsection}

달력 섹션은 달력 보고서입니다.

달력 보고서에 대한 자세한 내용은 [달력 보고서 개요](../../reports-and-dashboards/reports/calendars/calendar-reports-overview.md).

<table style="table-layout:auto"> 
 <col data-mc-conditions=""> 
 <col data-mc-conditions=""> 
 <tbody> 
  <tr> 
   <td>직접 필드</td> 
   <td> <p style="font-weight: normal;">달력 보고서에서 사용자 지정 날짜를 사용하는 새 기능을 지원하기 위해 다음 필드가 CalendarSection 개체에 추가되었습니다. </p> <p style="font-weight: normal;">자세한 내용은 <a href="../../reports-and-dashboards/reports/calendars/use-custom-dates.md" class="MCXref xref">달력 보고서에서 사용자 지정 날짜 필드 사용</a>.</p> 
    <ul> 
     <li> <p style="font-weight: normal;">customDate</p> </li> 
     <li> <p style="font-weight: normal;">customEndDateParameterID</p> </li> 
     <li> <p style="font-weight: normal;">customStartDateParameterID</p> </li> 
     <li> <p style="font-weight: normal;">ignoreActualDate</p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

### 회사 {#company}

회사 객체는 사람 컬렉션으로 구성된 조직을 나타냅니다.

회사에 대한 자세한 내용은 [회사 만들기 및 편집](../../administration-and-setup/set-up-workfront/organizational-setup/create-and-edit-companies.md).

<table style="table-layout:auto"> 
 <col data-mc-conditions=""> 
 <col data-mc-conditions=""> 
 <tbody> 
  <tr> 
   <td>직접 필드</td> 
   <td> 
    <ul> 
     <li style="font-weight: bold;"> <p>groupID</p> <p style="font-weight: normal;">회사가 연결된 그룹의 ID입니다.</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>참조 필드</td> 
   <td> 
    <ul> 
     <li style="font-weight: bold;"> <p>그룹</p> <p style="font-weight: normal;">회사가 연관된 그룹입니다. 회사를 그룹에 연결하면 그룹 관리자가 그룹 액세스 및 권한을 회사에 확장할 수 있습니다.</p> </li> 
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
  <tr> 
   <td>액션</td> 
   <td> 
    <ul> 
     <li> <p style="font-weight: normal;"><strong>productEnabled</strong> </p> <p style="font-weight: normal;">이 작업은 CustomerProductTypeEnum 인수를 사용하고 해당 고객에게 해당 제품에 대한 계정이 있는지 여부를 나타내는 부울을 반환합니다. </p> </li> 
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
       <li style="font-weight: normal;">password:zoomIntegrationEnabled(업데이트 스트림에서 확대/축소 통합 사용)</li> 
       <li style="font-weight: normal;"> password:quipIntegrationEnabled(config.general.quip.enabled)  </li> 
      </ul> </li> 
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
   <td> 
    <ul> 
     <li style="font-weight: bold;"> <p>createLinkedProofVersion</p> <p style="font-weight: normal;">추가됨</p> </li> 
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
   <td>직접 필드</td> 
   <td> 
    <ul> 
     <li style="font-weight: bold;"> <p>externalIntegrationType</p> <p style="font-weight: normal;">가능한 값이 제거됨:</p> 
      <ul> 
       <li style="font-weight: normal;">QUIP(Quip)</li> 
      </ul> </li> 
    </ul> 
    <ul> 
     <li> <p style="font-weight: normal;"><strong>proofDecision</strong> </p> <p>추가됨</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>액션</td> 
   <td> <p>다음 작업이 Document 객체에 추가되었습니다.</p> 
    <ul> 
     <li> <p style="font-weight: bold;">getDocumentReviewerDecision</p> <p style="font-weight: normal;">이 작업은 documentVersionID 인수(문자열)를 취하여 검토자의 결정을 나타내는 맵을 반환합니다.</p> </li> 
     <li style="font-weight: bold;"> <p>setDocumentReviewerDecision</p> <p style="font-weight: normal;">이 작업은 다음 인수를 사용합니다.</p> 
      <ul style="font-weight: normal;"> 
       <li> <p>documentVersionID(문자열)</p> </li> 
       <li> <p>reviewerDecision(문자열)</p> </li> 
       <li> <p>주석(문자열)</p> </li> 
      </ul> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

### 그룹  {#group}

그룹 개체는 사용자 및 팀 집합을 나타냅니다. 그룹은 종종 부서별 구조를 나타냅니다.

<table style="table-layout:auto"> 
 <col data-mc-conditions=""> 
 <col data-mc-conditions=""> 
 <tbody> 
  <tr> 
   <td>직접 필드</td> 
   <td> 
    <ul> 
     <li style="font-weight: bold;"> <p>businessLeaderID</p> <p style="font-weight: normal;">그룹에 지정된 비즈니스 리더의 ID입니다.</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>참조 필드</td> 
   <td> 
    <ul> 
     <li style="font-weight: bold;"> <p>businessLeader</p> <p style="font-weight: normal;">그룹에 지정된 비즈니스 리더 비즈니스 리더는 그룹을 위한 비즈니스 결정을 내리는 사람이다.</p> <p style="font-weight: normal;">비즈니스 리더에 대한 자세한 내용은 <a href="../../administration-and-setup/manage-groups/group-roles/business-leader-overview.md" class="MCXref xref">비즈니스 리더 개요</a>.<br></p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>액션</td> 
   <td> 
    <ul> 
     <li> <p><strong>assignMultiple</strong> </p> <p>이 작업은 다음 인수를 사용합니다.</p> 
      <ul> 
       <li> <p>userIDs (string[])</p> </li> 
       <li> <p>roleIDs (string[])</p> </li> 
       <li> <p>teamID (문자열)</p> </li> 
      </ul> </li> 
     <li> <p><strong>getGroupMembers</strong> </p> </li> 
     <li> <p><strong>updateMembersList</strong> </p> <p>이 작업은 다음 인수를 사용합니다.</p> 
      <ul> 
       <li> <p>newMemberIDs(string[])</p> </li> 
       <li> <p>removedMemberDs(string[])</p> </li> 
      </ul> </li> 
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
     <li style="font-weight: bold;"> <p>externalIntegrationType</p> <p style="font-weight: normal;">가능한 값이 제거됨:</p> 
      <ul> 
       <li style="font-weight: normal;">QUIP(Quip)</li> 
      </ul> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

### OpTask {#optask}

일반적으로 OpTask 개체를 Issue라고 합니다. 문제는 일반적으로 작업 또는 프로젝트 완료를 방지하는 데 문제가 있음을 나타내는 작업 항목입니다. 헬프데스크 요청도 있습니다. 변경 주문, 요청 및 버그도 문제입니다.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <p>직접 필드</p> </td> 
   <td> 
    <ul> 
     <li> <p><strong>backlogOrder</strong> </p> <p>순서는 Agile 백로그에 대한 작업 또는 스토리의 위치를 나타냅니다.</p> <p>이 필드에서 다음 플래그가 제거되었습니다.
       <ul>
        <li>동적,</li>
        <li>LAZY_READ,</li>
        <li>NOT_GROUPABLE:</li>
       </ul></p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">액션</td> 
   <td> <p>이러한 작업으로 사용자가 단추를 클릭하여 해당 항목에서 작업을 시작했음을 나타내는 작업 항목의 상태를 변경하는 새 시작 단추 기능을 지원하도록 인수 상태가 추가되었습니다.</p> <p>자세한 내용은 <a href="../../people-teams-and-groups/create-and-manage-teams/work-on-it-button-to-start-button.md" class="MCXref xref">Work On It 단추를 시작 단추로 바꿉니다.</a>.</p> 
    <ul> 
     <li> <p><strong>acceptWork</strong> </p> </li> 
     <li> <p><strong>unacceptWork</strong> </p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

### 매개변수 {#parameter}

Parameter 개체는 사용자 지정 필드입니다.

매개 변수 리소스가 SHARABLE 플래그를 추가했습니다.

사용자 지정 필드에 대한 자세한 내용은 [사용자 지정 양식 만들기 또는 편집](../../administration-and-setup/customize-workfront/create-manage-custom-forms/create-or-edit-a-custom-form.md#create) in [사용자 지정 양식 만들기 또는 편집](../../administration-and-setup/customize-workfront/create-manage-custom-forms/create-or-edit-a-custom-form.md).

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">직접 필드</td> 
   <td> 
    <ul> 
     <li> <p><strong>dataType</strong> </p> <p>가능한 값을 추가했습니다.</p> 
      <ul> 
       <li> <p>리치(리치 텍스트)</p> <p>자세한 내용은 <a href="../../wf-api/general/rich-text-field-api.md" class="MCXref xref">Adobe Workfront API의 리치 텍스트 필드</a>.</p> </li> 
      </ul> </li> 
     <li> <p><strong>displayType</strong> </p> <p>가능한 값을 추가했습니다.</p> 
      <ul> 
       <li> <p>리치(서식이 있는 텍스트 필드)</p> <p>자세한 내용은 <a href="../../wf-api/general/rich-text-field-api.md" class="MCXref xref">Adobe Workfront API의 리치 텍스트 필드</a>.</p> </li> 
      </ul> </li> 
     <li> <p><strong>레이블</strong> </p> <p>추가됨</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">컬렉션 필드</td> 
   <td> 
    <ul> 
     <li> <p><strong>accessRules</strong> </p> <p>추가됨</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">기본 필드</td> 
   <td> 
    <ul> 
     <li> <p class="TableStyle-TableStyle-List-options-in-steps-BodyA-Column2-LightGray"><strong>레이블</strong> </p> <p>추가됨</p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

### 포트폴리오 {#portfolio}

Portfolio 객체는 일반적으로 동일한 리소스, 즉 완료 비용 또는 사람에 대해 경쟁하는 프로젝트 컬렉션입니다.

포트폴리오에 대한 자세한 내용은 [Adobe Workfront의 Portfolio 개요](../../manage-work/portfolios/portfolios-overview/portfolio-overview.md).

<table style="table-layout:auto"> 
 <col data-mc-conditions=""> 
 <col data-mc-conditions=""> 
 <tbody> 
  <tr> 
   <td>직접 필드</td> 
   <td> 
    <ul> 
     <li style="font-weight: bold;"> <p>groupID</p> <p style="font-weight: normal;">포트폴리오가 연결된 그룹의 ID입니다.</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>참조 필드</td> 
   <td> 
    <ul> 
     <li style="font-weight: bold;"> <p>그룹</p> <p style="font-weight: normal;">포트폴리오와 연결된 그룹입니다. </p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

### 프로그램 {#program}

프로그램 객체는 유사한 프로젝트를 함께 그룹화할 수 있는 포트폴리오 내의 프로젝트의 하위 집합입니다.

<table style="table-layout:auto"> 
 <col data-mc-conditions=""> 
 <col data-mc-conditions=""> 
 <tbody> 
  <tr> 
   <td>직접 필드</td> 
   <td> 
    <ul> 
     <li style="font-weight: bold;"> <p>groupID</p> <p style="font-weight: normal;">프로그램이 연결된 그룹의 ID입니다.</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>참조 필드</td> 
   <td> 
    <ul> 
     <li style="font-weight: bold;"> <p>그룹</p> <p style="font-weight: normal;">프로그램과 연결된 그룹입니다. </p> </li> 
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
     <li><strong>requestorCoreAction</strong> <p>다음 possibleValues가 추가되었습니다.</p> 
      <ul> 
       <li> <p>PLANNING_HOURS_CONTOLING </p> <p>이 권한을 포함하는 액세스 수준을 가진 사용자는 작업 로드 밸런서에서 계획 시간을 업데이트할 수 있습니다.</p> <p>자세한 내용은 <a href="../../resource-mgmt/workload-balancer/manage-user-allocations-workload-balancer.md#update" class="MCXref xref">사용자 할당을 관리할 때 작업 계획 시간 업데이트</a> in <a href="../../resource-mgmt/workload-balancer/manage-user-allocations-workload-balancer.md" class="MCXref xref">작업 로드 밸런서에서 사용자 할당 관리</a>.</p> </li> 
       <li> <p>ADD_TO_CUSTOM_FORMS. </p> <p>이 권한을 포함하는 액세스 수준을 가진 사용자는 사용자 지정 양식에 필드를 추가할 수 있습니다.</p> <p>자세한 내용은 <a href="../../administration-and-setup/customize-workfront/create-manage-custom-forms/create-or-edit-a-custom-form.md#add2" class="MCXref xref"></a> in <a href="../../administration-and-setup/customize-workfront/create-manage-custom-forms/create-or-edit-a-custom-form.md" class="MCXref xref">사용자 지정 양식 만들기 또는 편집</a>.</p> </li> 
       <li> <p>EDIT_SYSTEMWIDE </p> <p>이 권한을 포함하는 액세스 수준을 가진 사용자는 사용자 정의 필드 시스템 전체를 삭제 액세스와 공유할 수 있습니다.</p> <p>자세한 내용은 <a href="../../administration-and-setup/customize-workfront/create-manage-custom-forms/configure-sharing-for-a-custom-field.md" class="MCXref xref">사용자 지정 필드 및 위젯에 대한 공유 구성</a></p> </li> 
      </ul> <li> <p><strong>requestorForbiddenActions</strong> </p> <p>다음 possibleValues가 추가되었습니다.</p> 
       <ul> 
        <li> <p>PLANNING_HOURS_CONTOLING </p> </li> 
        <li> <p>ADD_TO_CUSTOM_FORMS. </p> </li> 
        <li> <p>EDIT_SYSTEMWIDE </p> </li> 
       </ul> </li> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

### 예약된 보고서 {#scheduledreport}

ScheduledReport 개체는 배달하도록 구성된 보고서를 나타냅니다.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">직접 필드</td> 
   <td> 
    <ul> 
     <li> <p><strong>포맷</strong> </p> <p>가능한 값을 추가했습니다.</p> 
      <ul> 
       <li> <p>qdoc(enum.fileextension.qdoc)</p> </li> 
       <li> <p>qslides(enum.fileextension.qslids)</p> </li> 
       <li> <p>qsheet(enum.fileextension.qsheet)</p> </li> 
      </ul> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

### ScoreCardQuestion {#scorecardquestion}

ScoreCardQuestion 개체는 스코어카드에 추가된 질문을 나타냅니다. 이러한 질문은 일반적으로 Portfolio 관리자에 의해 결정되며 관리자가 이러한 질문에 대한 답변을 통해 프로젝트가 포트폴리오의 목표에 얼마나 잘 부합하는지 이해할 수 있습니다.

스코어카드 질문에 대한 자세한 내용은 [스코어카드 만들기](../../administration-and-setup/set-up-workfront/configure-system-defaults/create-scorecard.md).

<table style="table-layout:auto"> 
 <col data-mc-conditions=""> 
 <col data-mc-conditions=""> 
 <tbody> 
  <tr> 
   <td>직접 필드</td> 
   <td> 
    <ul> 
     <li style="font-weight: bold;"> <p>displayType</p> <p style="font-weight: normal;">가능한 값 RICH(서식이 있는 텍스트 필드)가 추가되었습니다. </p> <p style="font-weight: normal;">자세한 내용은 <a href="../../wf-api/general/rich-text-field-api.md" class="MCXref xref">Adobe Workfront API의 리치 텍스트 필드</a>.  </p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

### 작업 {#task}

작업 객체는 최종 목표(프로젝트 완료)를 달성하는 단계로 수행되어야 하는 작업 항목을 나타냅니다.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">직접 필드</td> 
   <td> 
    <ul> 
     <li> <p><strong>workFuture</strong> </p> <p>이 필드가 추가되었으며 작업을 완료하는 데 사용자에게 작은 작업, 중간 작업 또는 많은 양의 노력이 필요하는지 여부를 나타냅니다. 가능한 값은 다음과 같습니다.</p> 
      <ul> 
       <li> <p>1 (작음)</p> </li> 
       <li> <p>2(중간)</p> </li> 
       <li> <p>3(큰)</p> </li> 
      </ul> <p>Workfront의 작업 수행에 대한 자세한 내용은 <a href="../../manage-work/tasks/task-information/work-effort.md" class="MCXref xref">작업 시간 개요</a>.</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">액션</td> 
   <td> <p>이러한 작업으로 사용자가 단추를 클릭하여 해당 항목에서 작업을 시작했음을 나타내는 작업 항목의 상태를 변경하는 새 시작 단추 기능을 지원하도록 인수 상태가 추가되었습니다.</p> <p>자세한 내용은 <a href="../../people-teams-and-groups/create-and-manage-teams/work-on-it-button-to-start-button.md" class="MCXref xref">Work On It 단추를 시작 단추로 바꿉니다.</a>.</p> 
    <ul> 
     <li> <p><strong>acceptWork</strong> </p> </li> 
     <li> <p><strong>unacceptWork</strong> </p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

### 팀 {#team}

팀 개체는 작업 항목에 지정할 수 있는 사용자 모음입니다.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">직접 필드</td> 
   <td> <p>다음 필드가 팀 리소스에 추가되었습니다.</p> 
    <ul> 
     <li> <p><strong>completeDaysOnKanbanBoard</strong> </p> <p>이 필드는 완료된 카드가 간판 보드에 남아 있는 일수를 나타냅니다.</p> <!--
       <p data-mc-conditions="QuicksilverOrClassic.Draft mode">For more information, see <a href="../../agile/get-started-with-agile-in-workfront/configure-kanban.md" class="MCXref xref">Configure Kanban</a>.</p>
      --> </li> 
     <li> <p><strong>groupID</strong> </p> <p>이 필드는 한 팀을 그룹과 연결합니다. 팀을 그룹의 일부로 식별하고 그룹 관리자가 팀을 관리할 수 있도록 합니다.</p> </li> 
     <li> <p><strong>workOnItStatusChange</strong> </p> <p>팀의 작업 중 단추가 시작 단추로 구성되었는지 여부를 나타내는 부울 매개 변수입니다. 팀 구성원이 시작 단추를 클릭하여 작업 항목에 대한 작업을 시작하면 항목의 상태가 새로 작성에서 팀 설정에 구성된 상태로 변경됩니다.</p> </li> 
     <li> <p>다음 필드를 사용하면 개별 작업 항목의 시작 단추에 대한 사용자 지정 상태를 지정할 수 있습니다.</p> 
      <ul> 
       <li> <p><strong>workOnItOpTaskBugReportStatus</strong> </p> </li> 
       <li> <p><strong>workOnItOpTaskChangeOrderStatus</strong> </p> </li> 
       <li> <p><strong>workOnItOpTaskIssueStats</strong> </p> </li> 
       <li> <p><strong>workOnItOpTaskRequestStatus</strong> </p> <p><strong>workOnItTaskStatus</strong> </p> </li> 
      </ul> <p>시작 단추에 대한 자세한 내용은 <a href="../../people-teams-and-groups/create-and-manage-teams/work-on-it-button-to-start-button.md" class="MCXref xref">Work On It 단추를 시작 단추로 바꿉니다.</a>.</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">참조 필드</td> 
   <td> <p>팀 리소스에 다음 필드가 추가되었습니다.</p> 
    <ul> 
     <li> <p><strong>그룹</strong> </p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

### TemplateTask {#templatetask}

TemplateTask 개체는 템플릿에 속하는 작업을 나타냅니다. 템플릿 작업은 템플릿이 사용되는 프로젝트에서 작업이 됩니다.

템플릿 작업에 대한 자세한 내용은 [템플릿 작업 편집](../../manage-work/projects/create-and-manage-templates/edit-template-task.md).

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">직접 필드</td> 
   <td> 
    <ul> 
     <li> <p><strong>workFuture</strong> </p> <p>이 필드가 추가되었으며 작업을 완료하는 데 사용자에게 작은 작업, 중간 작업 또는 많은 양의 노력이 필요하는지 여부를 나타냅니다. 가능한 값은 다음과 같습니다.</p> 
      <ul> 
       <li> <p>1 (작음)</p> </li> 
       <li> <p>2(중간)</p> </li> 
       <li> <p>3(큰)</p> </li> 
      </ul> <p>Workfront의 작업 수행에 대한 자세한 내용은 <a href="../../manage-work/tasks/task-information/work-effort.md" class="MCXref xref">작업 시간 개요</a>.</p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

### 타임시트 {#timesheet}

작업표 개체는 사용자가 작업, 프로젝트 및 오버헤드 시간 유형에 대해 실제 작업 시간을 입력할 수 있도록 하는 가상 타임카드를 나타냅니다.

작업표에 대한 자세한 내용은 [작업표 개요](../../timesheets/timesheets/timesheets-overview.md)

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">핵심 필드</td> 
   <td> <p>작업표 리소스에서 다음 필드가 제거되었습니다.</p> 
    <ul> 
     <li> <p><strong>개체 코드</strong> </p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

### 업데이트

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">직접 필드</td> 
   <td> 
    <ul> 
     <li> <p><strong>updateType</strong> </p> <p>다음 가능한 값을 추가했습니다.</p> 
      <ul> 
       <li> <p>initiativeAdd (enum.updatetime.initiativeadd)</p> </li> 
       <li> <p>initiativeEdit (enum.updatetime.initiativeedit)</p> </li> 
      </ul> <p data-mc-conditions="QuicksilverOrClassic.Quicksilver">이니셔티브에 대한 자세한 내용은 <a href="../../scenario-planner/initiatives-overview.md" class="MCXref xref">시나리오 플래너의 이니셔티브 개요</a>.</p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

### 사용자 {#user}

사용자 개체는 로그인하고 시스템과 상호 작용할 수 있는 Workfront에 계정이 있는 사람을 나타냅니다.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">직접 필드</td> 
   <td> <p>다음 필드가 사용자 리소스에 추가되었습니다.</p> 
    <ul> 
     <li> <p><strong>actualDeactivationDate</strong> </p> <p>사용자가 비활성화된 날짜 및 시간을 나타냅니다.</p> <p>비활성화된 사용자에 대한 자세한 내용은 <a href="../../administration-and-setup/add-users/create-and-manage-users/deactivate-a-user.md" class="MCXref xref">사용자 비활성화 또는 다시 활성화</a>.</p> </li> 
     <li> <p><strong>alignAccessType</strong> </p> <p>이 필드는 Workfront 목표에 대한 사용자의 액세스를 보여줍니다. 가능한 값은 다음과 같습니다.</p> 
      <ul> 
       <li> <p>액세스 권한 없음</p> </li> 
       <li> <p>보기</p> </li> 
       <li> <p>편집</p> </li> 
      </ul> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">액션</td> 
   <td> <p>다음 작업이 사용자 리소스에 추가되었습니다.</p> 
    <ul> 
     <li> <p><strong>getUserAccessPermissionsByObjCode</strong> </p> <p>이 작업은 다음 인수를 사용합니다</p> 
      <ul> 
       <li> <p>id(문자열)</p> </li> 
       <li> <p>objCode(문자열)</p> </li> 
      </ul> </li> 
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
   <td>직접 필드</td> 
   <td> 
    <ul> 
     <li> <p><strong>backlogOrder</strong> </p> <p>순서는 Agile 백로그에 대한 작업 또는 스토리의 위치를 나타냅니다.</p> <p>이 필드에서 다음 플래그가 제거되었습니다.</p> 
      <ul> 
       <li> <p>동적,</p> </li> 
       <li> <p>LAZY_READ,</p> </li> 
       <li> <p>NOT_GROUPABLE</p> </li> 
      </ul> </li> 
     <li> <p><strong>groupID</strong> </p> <p>이 필드에 다음 플래그가 추가되었습니다.</p> 
      <ul> 
       <li> <p>AUTO_LOAD,</p> </li> 
       <li> <p>동적,</p> </li> 
       <li> <p>READ_ONLY</p> </li> 
      </ul> </li> 
     <li> <p><strong>workFuture</strong> </p> <p>이 필드가 추가되었으며 작업을 완료하는 데 사용자에게 작은 작업, 중간 작업 또는 많은 양의 노력이 필요하는지 여부를 나타냅니다. 가능한 값은 다음과 같습니다.</p> 
      <ul> 
       <li> <p>1 (작음)</p> </li> 
       <li> <p>2(중간)</p> </li> 
       <li> <p>3(큰)</p> </li> 
      </ul> <p>Workfront의 작업 수행에 대한 자세한 내용은 <a href="../../manage-work/tasks/task-information/work-effort.md" class="MCXref xref">작업 시간 개요</a>.</p> </li> 
    </ul> <p style="font-weight: normal;">  </p> </td> 
  </tr> 
 </tbody> 
</table>
