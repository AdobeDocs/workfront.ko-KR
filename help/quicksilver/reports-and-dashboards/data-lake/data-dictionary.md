---
content-type: reference
product-area: reports and dashboards
navigation-topic: data connect
title: Workfront Data Connect 데이터 사전
description: 이 페이지에는 Workfront Data Connect의 데이터 구조 및 내용에 대한 정보가 포함되어 있습니다.
author: Nolan
feature: Reports and Dashboards
exl-id: 57985404-554e-4289-b871-b02d3427aa5c
source-git-commit: 44342db0a473eac70212d08cedf9ac0f571cda0b
workflow-type: tm+mt
source-wordcount: '8129'
ht-degree: 7%

---

# Workfront Data Connect 데이터 사전

이 페이지에는 Workfront Data Connect의 데이터 구조 및 내용에 대한 정보가 포함되어 있습니다.

>[!NOTE]
>
>Data Connect의 데이터는 4시간마다 새로 고침되므로 최근 변경 사항이 즉시 반영되지 않을 수 있습니다.

## 테이블 유형

Data Connect에서 최대한 통찰력을 제공하는 방식으로 Workfront 데이터를 보기 위해 활용할 수 있는 다양한 테이블 유형이 있습니다.

* **현재 테이블**

  현재 테이블은 모든 개체 및 현재 상태의 Workfront에 존재하는 것과 유사하게 데이터를 반영합니다. 하지만 Workfront 내에서보다 훨씬 짧은 지연 시간으로 탐색할 수 있습니다.

* **이벤트 테이블**

  이벤트 테이블은 Workfront의 모든 변경 레코드를 추적합니다. 즉, 객체가 상태를 변경할 때마다 변경 발생 시간, 변경한 사람 및 변경된 내용을 표시하는 레코드가 만들어집니다. 따라서 이 표는 시점 비교에 유용합니다. 이 표에는 지난 3년간의 기록만 포함되어 있습니다.

* **일별 기록 테이블**

  일별 내역 테이블은 각 개별 이벤트가 발생한 시점이 아니라 매일 각 객체의 상태를 표시한다는 점에서 이벤트 테이블의 축약된 버전을 제공합니다. 따라서 이 표는 추세 분석에 유용합니다.

<!-- Custom table -->

## 엔티티 관계 다이어그램

Workfront의 개체(및 따라서 Data Connect 데이터 레이크)는 개별 값뿐만 아니라 다른 개체와의 관계에 의해서도 정의됩니다. 아래의 엔티티 관계 다이어그램은 Data Connect에서 개체 관계의 높은 수준 매핑을 제공합니다. 다음 링크를 사용하여 다이어그램을 보고 다운로드할 수 있습니다.

[Data Connect 엔티티 관계 다이어그램](/help/quicksilver/reports-and-dashboards/data-lake/assets/Workfront-data-lake_entity-relationship-diagram.pdf)

>[!IMPORTANT]
>
>엔티티 관계 다이어그램은 진행 중인 작업입니다. 따라서 참조용으로만 사용되며 변경될 수 있습니다.

## 날짜 유형

특정 이벤트가 발생하는 시기에 대한 정보를 제공하는 다양한 날짜 개체가 있습니다.

* `DL_LOAD_TIMESTAMP`: 이 날짜는 내부 참조에 사용되며 데이터가 Current, Event 또는 Daily History 테이블에 로드된 시기를 반영합니다. 이 날짜는 데이터 분석에 사용되어서는 안 되며 Workfront 데이터 레이크의 베타 단계 동안 제거될 계획입니다.
* `CALENDAR_DATE`: 이 날짜는 [일별 기록] 테이블에만 있습니다. 이 테이블은 `CALENDAR_DATE`에 지정된 각 날짜에 대해 11:59 UTC에 데이터가 어떻게 보이는지에 대한 기록을 제공합니다.
* `BEGIN_EFFECTIVE_TIMESTAMP`: 이 날짜는 이벤트 및 일별 기록 테이블 모두에 있으며 레코드가 현재 행에 있는 값을 _to_(으)로 변경한 시기를 정확하게 기록합니다.
* `END_EFFECTIVE_TIMESTAMP`: 이 날짜는 이벤트 및 일일 기록 테이블 모두에 있으며 레코드가 현재 행의 값을 _부터_&#x200B;까지 다른 행의 값으로 변경한 정확한 시점을 기록합니다. `BEGIN_EFFECTIVE_TIMESTAMP`과(와) `END_EFFECTIVE_TIMESTAMP`의 쿼리 사이에 을(를) 허용하려면 새 값이 없어도 이 값은 null이 아닙니다. 레코드가 여전히 유효한 경우(즉, 값이 변경되지 않은 경우) `END_EFFECTIVE_TIMESTAMP`의 값은 2300-01-01입니다.

## 용어 표

다음 표는 Workfront의 개체 이름(인터페이스 및 API의 이름)과 Data Connect의 해당 이름을 상호 연결합니다.

### 액세스 수준

<table>
    <thead>
        <tr>
            <th>Workfront 엔티티 이름</th>
            <th>인터페이스 참조</th>
            <th>API 참조</th>
            <th>API 레이블</th>
            <th>데이터 레이크 보기</th>
        </tr>
      </thead>
      <tbody>
        <tr>
            <td>액세스 수준</td>
            <td>액세스 수준</td>
            <td>ACSLVL</td>
            <td>액세스 수준</td>
            <td>ACCESSLEVELS_CURRENT<br>ACCESSLEVELS_DAILY_HISTORY<br>ACCESSLEVELS_EVENT</td>
        </tr>
      </tbody>
</table>
<table>
    <thead>
        <tr>
            <th>기본/외래 키</th>
            <th>유형</th>
            <th>관련 테이블</th>
            <th>관련 필드</th>
        </tr>
    </thead>
    <tbody>
        <tr>
             <td>ACCESSLEVELID</td>
             <td>PK</td>
             <td>-</td>
             <td>-</td>
        </tr>
        <tr>
             <td>APPGLOBALID</td>
             <td>-</td>
             <td colspan="2">관계가 아닙니다. 내부 응용 프로그램 용도로 사용됩니다.</td>
        </tr>
        <tr>
             <td>LASTUPDATEDBYID</td>
             <td>FK</td>
             <td>USERS_CURRENT</td>
             <td>사용자 ID</td>
        </tr>
        <tr>
             <td>LEGACYACCESSLEVELID</td>
             <td>-</td>
             <td colspan="2">관계가 아닙니다. 내부 응용 프로그램 용도로 사용됩니다.</td>
        </tr>
        <tr>
             <td>OBJID</td>
             <td>FK</td>
             <td>변수, OBJCODE 기반</td>
             <td>OBJCODE 필드에서 식별된 객체의 기본 키/ID</td>
        </tr>
        <tr>
             <td>SYSID</td>
             <td>-</td>
             <td colspan="2">관계가 아닙니다. 내부 응용 프로그램 용도로 사용됩니다.</td>
        </tr>
    </tbody>
</table>

### 액세스 규칙

<table>
    <thead>
        <tr>
            <th>Workfront 엔티티 이름</th>
            <th>인터페이스 참조</th>
            <th>API 참조</th>
            <th>API 레이블</th>
            <th>데이터 레이크 보기</th>
        </tr>
      </thead>
      <tbody>
        <tr>
            <td>액세스 규칙</td>
            <td>공유</td>
            <td>ACSRUL</td>
            <td>공유</td>
            <td>ACCESSRULES_CURRENT<br>ACCESSRULES_DAILY_HISTORY<br>ACCESSRULES_EVENT</td>
        </tr>
      </tbody>
</table>
<table>
    <thead>
        <tr>
            <th>기본/외래 키</th>
            <th>유형</th>
            <th>관련 테이블</th>
            <th>관련 필드</th>
        </tr>
    </thead>
    <tbody>
        <tr>
             <td>접근자 ID</td>
             <td>FK</td>
             <td>변수, ACCESSOROBJCODE 기반</td>
             <td>ACCESSOROBJCODE 필드에서 식별된 개체의 기본 키/ID</td>
        </tr>
        <tr>
             <td>접근성 ID</td>
             <td>PK</td>
             <td>-</td>
             <td>-</td>
        </tr>
        <tr>
             <td>ANCESTORID</td>
             <td>PK</td>
             <td>변수, ANCESTOROBJCODE 기반</td>
             <td>ANCESTOROBJCODE 필드에서 식별된 객체의 기본 키/ID</td>
        </tr>
        <tr>
             <td>LASTUPDATEDBYID</td>
             <td>FK</td>
             <td>USERS_CURRENT</td>
             <td>사용자 ID</td>
        </tr>
        <tr>
             <td>SECURITYOBJID</td>
             <td>FK</td>
             <td>변수, SECURITYOBJCODE 기반</td>
             <td>SECURITYOBJCODE 필드에서 식별된 객체의 기본 키/ID</td>
        </tr>
        <tr>
             <td>SYSID</td>
             <td>-</td>
             <td colspan="2">관계가 아닙니다. 내부 응용 프로그램 용도로 사용됩니다.</td>
        </tr>
    </tbody>
</table>

### 승인 경로

<table>
    <thead>
        <tr>
            <th>Workfront 엔티티 이름</th>
            <th>인터페이스 참조</th>
            <th>API 참조</th>
            <th>API 레이블</th>
            <th>데이터 레이크 보기</th>
        </tr>
      </thead>
      <tbody>
        <tr>
            <td>승인 경로</td>
            <td>승인 경로</td>
            <td>ARVPTH</td>
            <td>승인</td>
            <td>APPROVALPATHS_CURRENT<br>APPROVALPATHS_DAILY_HISTORY<br>APPROVALPATHS_EVENT</td>
        </tr>
      </tbody>
</table>
<table>
    <thead>
        <tr>
            <th>기본/외래 키</th>
            <th>유형</th>
            <th>관련 테이블</th>
            <th>관련 필드</th>
        </tr>
    </thead>
    <tbody>
        <tr>
             <td>APPROVALPATHID</td>
             <td>PK</td>
             <td>-</td>
             <td>-</td>
        </tr>
        <tr>
             <td>APPROVALPROCESSID</td>
             <td>FK</td>
             <td>APPROVALPROCESSES_CURRENT</td>
             <td>APPROVALPROCESSID</td>
        </tr>
        <tr>
             <td>ENTEREDBYID</td>
             <td>FK</td>
             <td>USERS_CURRENT</td>
             <td>사용자 ID</td>
        </tr>
        <tr>
             <td>GLOBALPATHID</td>
             <td>-</td>
             <td colspan="2">관계가 아닙니다. 내부 응용 프로그램 용도로 사용됩니다.</td>
        </tr>
        <tr>
             <td>LASTUPDATEDBYID</td>
             <td>FK</td>
             <td>USERS_CURRENT</td>
             <td>사용자 ID</td>
        </tr>
        <tr>
             <td>SYSID</td>
             <td>-</td>
             <td colspan="2">관계가 아닙니다. 내부 응용 프로그램 용도로 사용됩니다.</td>
        </tr>
    </tbody>
</table>

### 승인 진행

<table>
    <thead>
        <tr>
            <th>Workfront 엔티티 이름</th>
            <th>인터페이스 참조</th>
            <th>API 참조</th>
            <th>API 레이블</th>
            <th>데이터 레이크 보기</th>
        </tr>
      </thead>
      <tbody>
        <tr>
            <td>승인 진행</td>
            <td>승인 진행</td>
            <td>ARVPRC</td>
            <td>승인 진행</td>
            <td>APPROVALPROCESSES_CURRENT<br>APPROVALPROCESSES_DAILY_HISTORY<br>APPROVALPROCESSES_EVENT</td>
        </tr>
      </tbody>
</table>
<table>
    <thead>
        <tr>
            <th>기본/외래 키</th>
            <th>유형</th>
            <th>관련 테이블</th>
            <th>관련 필드</th>
        </tr>
    </thead>
    <tbody>
        <tr>
             <td>APPROVALPROCESSID</td>
             <td>PK</td>
             <td>-</td>
             <td>-</td>
        </tr>
        <tr>
             <td>ENTEREDBYID</td>
             <td>FK</td>
             <td>USERS_CURRENT</td>
             <td>사용자 ID</td>
        </tr>
        <tr>
             <td>LASTUPDATEDBYID</td>
             <td>FK</td>
             <td>USERS_CURRENT</td>
             <td>사용자 ID</td>
        </tr>
        <tr>
             <td>SYSID</td>
             <td>-</td>
             <td colspan="2">관계가 아닙니다. 내부 응용 프로그램 용도로 사용됩니다.</td>
        </tr>
    </tbody>
</table>

### 승인 단계

<table>
    <thead>
        <tr>
            <th>Workfront 엔티티 이름</th>
            <th>인터페이스 참조</th>
            <th>API 참조</th>
            <th>API 레이블</th>
            <th>데이터 레이크 보기</th>
        </tr>
      </thead>
      <tbody>
        <tr>
            <td>승인 단계</td>
            <td>승인 단계</td>
            <td>ARVSTP</td>
            <td>승인 단계</td>
            <td>APPROVALSTEPS_CURRENT<br>APPROVALSTEPS_DAILY_HISTORY<br>APPROVALSTEPS_EVENT</td>
        </tr>
      </tbody>
</table>
<table>
    <thead>
        <tr>
            <th>기본/외래 키</th>
            <th>유형</th>
            <th>관련 테이블</th>
            <th>관련 필드</th>
        </tr>
    </thead>
    <tbody>
        <tr>
             <td>APPROVALPATHID</td>
             <td>FK</td>
             <td>APPROVALPATHS_CURRENT</td>
             <td>APPROVALPATHID</td>
        </tr>
        <tr>
             <td>승인스테피드</td>
             <td>PK</td>
             <td>-</td>
             <td>-</td>
        </tr>
        <tr>
             <td>SYSID</td>
             <td>-</td>
             <td colspan="2">관계가 아닙니다. 내부 응용 프로그램 용도로 사용됩니다.</td>
        </tr>
    </tbody>
</table>

### 승인자 상태

<table>
    <thead>
        <tr>
            <th>Workfront 엔티티 이름</th>
            <th>인터페이스 참조</th>
            <th>API 참조</th>
            <th>API 레이블</th>
            <th>데이터 레이크 보기</th>
        </tr>
      </thead>
      <tbody>
        <tr>
            <td>승인자 상태</td>
            <td>승인자 상태</td>
            <td>아르브스트</td>
            <td>승인자 상태</td>
            <td>APPROVERSTATUSES_CURRENT<br>APPROVERSTATUSES_DAILY_HISTORY<br>APPROVERSTATUSES_EVENT</td>
        </tr>
      </tbody>
</table>
<table>
    <thead>
        <tr>
            <th>기본/외래 키</th>
            <th>유형</th>
            <th>관련 테이블</th>
            <th>관련 필드</th>
        </tr>
    </thead>
    <tbody>
        <tr>
             <td>APPROVERSTATUSID</td>
             <td>PK</td>
             <td>-</td>
             <td>-</td>
        </tr>
        <tr>
             <td>APPROVABLEOBJID</td>
             <td>FK</td>
             <td>변수, APPROVABLEOBJCODE 기반</td>
             <td>APPROVABLEOBJCODE 필드에서 식별된 객체의 기본 키/ID</td>
        </tr>
        <tr>
             <td>승인스테피드</td>
             <td>FK</td>
             <td>APPROVALSTEPS_CURRENT</td>
             <td>승인스테피드</td>
        </tr>
        <tr>
             <td>APPROVEDBYID</td>
             <td>FK</td>
             <td>USERS_CURRENT</td>
             <td>사용자 ID</td>
        </tr>
        <tr>
             <td>DELEGATEUSERID</td>
             <td>FK</td>
             <td>USERS_CURRENT</td>
             <td>사용자 ID</td>
        </tr>
        <tr>
             <td>LASTUPDATEDBYID</td>
             <td>FK</td>
             <td>USERS_CURRENT</td>
             <td>사용자 ID</td>
        </tr>
        <tr>
             <td>OPTASKID</td>
             <td>FK</td>
             <td>OPTASKS_CURRENT</td>
             <td>OPTASKID</td>
        </tr>
        <tr>
             <td>OVERRIDDENUSERID</td>
             <td>FK</td>
             <td>USERS_CURRENT</td>
             <td>사용자 ID</td>
        </tr>
        <tr>
             <td>PROJECTID</td>
             <td>FK</td>
             <td>PROJECTS_CURRENT</td>
             <td>PROJECTID</td>
        </tr>
        <tr>
             <td>STEAPPROVERID</td>
             <td>FK</td>
             <td>USERS_CURRENT</td>
             <td>사용자 ID</td>
        </tr>
        <tr>
             <td>시시드</td>
             <td>-</td>
             <td colspan="2">관계가 아닙니다. 내부 응용 프로그램 용도로 사용됩니다.</td>
        </tr>
        <tr>
             <td>TASKID</td>
             <td>FK</td>
             <td>TASKS_CURRENT</td>
             <td>TASKID</td>
        </tr>
        <tr>
             <td>와일드카드 사용자 ID</td>
             <td>FK</td>
             <td>USERS_CURRENT</td>
             <td>사용자 ID</td>
        </tr>
    </tbody>
</table>

### 할당

<table>
    <thead>
        <tr>
            <th>Workfront 엔티티 이름</th>
            <th>인터페이스 참조</th>
            <th>API 참조</th>
            <th>API 레이블</th>
            <th>데이터 레이크 보기</th>
        </tr>
      </thead>
      <tbody>
        <tr>
            <td>할당</td>
            <td>할당</td>
            <td>ASSIGN</td>
            <td>할당</td>
            <td>ASSIGNMENTS_CURRENT<br>ASSIGNMENTS_DAILY_HISTORY<br>ASSIGNMENTS_EVENT</td>
        </tr>
      </tbody>
</table>
<table>
    <thead>
        <tr>
            <th>기본/외래 키</th>
            <th>유형</th>
            <th>관련 테이블</th>
            <th>관련 필드</th>
        </tr>
    </thead>
    <tbody>
        <tr>
             <td>ASSIGNEDBYID</td>
             <td>FK</td>
             <td>USERS_CURRENT</td>
             <td>사용자 ID</td>
        </tr>
        <tr>
             <td>ASSIGNEDTOID</td>
             <td>FK</td>
             <td>USERS_CURRENT</td>
             <td>사용자 ID</td>
        </tr>
        <tr>
             <td>ASSIGNMENTID</td>
             <td>PK</td>
             <td>-</td>
             <td>-</td>
        </tr>
        <tr>
             <td>범주 ID</td>
             <td>FK</td>
             <td>CATEGORS_CURRENT</td>
             <td>범주 ID</td>
        </tr>
        <tr>
             <td>분류자</td>
             <td>FK</td>
             <td>CLASSIFIER_CURRENT</td>
             <td>분류자</td>
        </tr>
        <tr>
             <td>OPTASKID</td>
             <td>FK</td>
             <td>OPTASKS_CURRENT</td>
             <td>OPTASKID</td>
        </tr>
        <tr>
             <td>PRIVATERATECARDID</td>
             <td>FK</td>
             <td>RATECARD_CURRENT</td>
             <td>RATECARDID</td>
        </tr>
        <tr>
             <td>PROJECTID</td>
             <td>FK</td>
             <td>PROJECTS_CURRENT</td>
             <td>PROJECTID</td>
        </tr>
        <tr>
             <td>장미모양-</td>
             <td>FK</td>
             <td>ROLES_CURRENT</td>
             <td>장미모양-</td>
        </tr>
        <tr>
             <td>TASKID</td>
             <td>FK</td>
             <td>TASKS_CURRENT</td>
             <td>TASKID</td>
        </tr>
        <tr>
             <td>티미드</td>
             <td>FK</td>
             <td>TEAMS_CURRENT</td>
             <td>티미드</td>
        </tr>
    </tbody>
</table>

### 승인 대기 중

<table>
    <thead>
        <tr>
            <th>Workfront 엔티티 이름</th>
            <th>인터페이스 참조</th>
            <th>API 참조</th>
            <th>API 레이블</th>
            <th>데이터 레이크 보기</th>
        </tr>
      </thead>
      <tbody>
        <tr>
            <td>승인 대기 중</td>
            <td>승인 대기 중</td>
            <td>AWAPVL</td>
            <td>승인 대기 중</td>
            <td>AWAITINGAPPROVALS_CURRENT<br>AWAITINGAPPROVALS_DAILY_HISTORY<br>AWAITINGAPPROVALS_EVENT</td>
        </tr>
      </tbody>
</table>
<table>
    <thead>
        <tr>
            <th>기본/외래 키</th>
            <th>유형</th>
            <th>관련 테이블</th>
            <th>관련 필드</th>
        </tr>
    </thead>
    <tbody>
        <tr>
             <td>ACCESSREQUESTID</td>
             <td>-</td>
             <td colspan="2">액세스 요청 테이블은 현재 지원되지 않습니다.</td>
        </tr>
        <tr>
             <td>APPROVABLEID</td>
             <td>FK</td>
             <td>-</td>
             <td colspan="2">관계가 아닙니다. 내부 응용 프로그램 용도로 사용됩니다.</td>
        </tr>
        <tr>
             <td>승인자 ID</td>
             <td>FK</td>
             <td>USERS_CURRENT</td>
             <td>사용자 ID</td>
        </tr>
        <tr>
             <td>AWAITINGAPPROVALID</td>
             <td>PK</td>
             <td>-</td>
             <td>-</td>
        </tr>
        <tr>
             <td>DOCUMENTID</td>
             <td>FK</td>
             <td>DOCUMENTS_CURRENT</td>
             <td>DOCUMENTID</td>
        </tr>
        <tr>
             <td>DOCUMENTVERSIONID</td>
             <td>FK</td>
             <td>DOCUMENTVERSIONS_CURRENT</td>
             <td>DOCUMENTVERSIONID</td>
        </tr>
        <tr>
             <td>OPTASKID</td>
             <td>FK</td>
             <td>OPTASKS_CURRENT</td>
             <td>OPTASKID</td>
        </tr>
        <tr>
             <td>PROJECTID</td>
             <td>FK</td>
             <td>PROJECTS_CURRENT</td>
             <td>PROJECTID</td>
        </tr>
        <tr>
             <td>장미모양-</td>
             <td>FK</td>
             <td>ROLES_CURRENT</td>
             <td>장미모양-</td>
        </tr>
        <tr>
             <td>SUBMITTEDBYID</td>
             <td>FK</td>
             <td>USERS_CURRENT</td>
             <td>사용자 ID</td>
        </tr>
        <tr>
             <td>SYSID</td>
             <td>-</td>
             <td colspan="2">관계가 아닙니다. 내부 응용 프로그램 용도로 사용됩니다.</td>
        </tr>
        <tr>
             <td>TASKID</td>
             <td>FK</td>
             <td>TASKS_CURRENT</td>
             <td>TASKID</td>
        </tr>
        <tr>
             <td>티미드</td>
             <td>FK</td>
             <td>TEAMS_CURRENT</td>
             <td>티미드</td>
        </tr>
        <tr>
             <td>TIMESHEETID</td>
             <td>FK</td>
             <td>TIMESHEETS_CURRENT</td>
             <td>TIMESHEETID</td>
        </tr>
        <tr>
             <td>사용자 ID</td>
             <td>FK</td>
             <td>USERS_CURRENT</td>
             <td>사용자 ID</td>
        </tr>
    </tbody>
</table>

### 기준선

<table>
    <thead>
        <tr>
            <th>Workfront 엔티티 이름</th>
            <th>인터페이스 참조</th>
            <th>API 참조</th>
            <th>API 레이블</th>
            <th>데이터 레이크 보기</th>
        </tr>
      </thead>
      <tbody>
        <tr>
            <td>기준선</td>
            <td>기준선</td>
            <td>블린</td>
            <td>기준선</td>
            <td>BASELINES_CURRENT<br>BASELINES_DAY_HISTORY<br>BASELINES_EVENT</td>
        </tr>
      </tbody>
</table>
<table>
    <thead>
        <tr>
            <th>기본/외래 키</th>
            <th>유형</th>
            <th>관련 테이블</th>
            <th>관련 필드</th>
        </tr>
    </thead>
    <tbody>
        <tr>
             <td>BASELINEID</td>
             <td>PK</td>
             <td>-</td>
             <td>-</td>
        </tr>
        <tr>
             <td>EXCHANGERATEID</td>
             <td>FK</td>
             <td>EXCHANGE_CURRENT</td>
             <td>EXCHANGERATEID</td>
        </tr>
        <tr>
             <td>PROJECTID</td>
             <td>FK</td>
             <td>PROJECTS_CURRENT</td>
             <td>PROJECTID</td>
        </tr>
        <tr>
             <td>SYSID</td>
             <td>-</td>
             <td colspan="2">관계가 아닙니다. 내부 응용 프로그램 용도로 사용됩니다.</td>
        </tr>
    </tbody>
</table>

### 기준선 작업

<table>
    <thead>
        <tr>
            <th>Workfront 엔티티 이름</th>
            <th>인터페이스 참조</th>
            <th>API 참조</th>
            <th>API 레이블</th>
            <th>데이터 레이크 보기</th>
        </tr>
      </thead>
      <tbody>
        <tr>
            <td>기준선 작업</td>
            <td>기준선 작업</td>
            <td>BSTSK</td>
            <td>기준선 작업</td>
            <td>BASELINETTASKS_CURRENT<br>BASELINETTASKS_DAILY_HISTORY<br>BASELINETTASKS_EVENT</td>
        </tr>
      </tbody>
</table>
<table>
    <thead>
        <tr>
            <th>기본/외래 키</th>
            <th>유형</th>
            <th>관련 테이블</th>
            <th>관련 필드</th>
        </tr>
    </thead>
    <tbody>
        <tr>
             <td>BASELINEID</td>
             <td>FK</td>
             <td>BASELINES_CURRENT</td>
             <td>BASELINEID</td>
        </tr>
        <tr>
             <td>BASELINETASKID</td>
             <td>PK</td>
             <td>-</td>
             <td>-</td>
        </tr>
        <tr>
             <td>EXCHANGERATEID</td>
             <td>FK</td>
             <td>EXCHANGE_CURRENT</td>
             <td>EXCHANGERATEID</td>
        </tr>
        <tr>
             <td>PROJECTID</td>
             <td>FK</td>
             <td>PROJECTS_CURRENT</td>
             <td>PROJECTID</td>
        </tr>
        <tr>
             <td>SYSID</td>
             <td>-</td>
             <td colspan="2">관계가 아닙니다. 내부 응용 프로그램 용도로 사용됩니다.</td>
        </tr>
        <tr>
             <td>TASKID</td>
             <td>FK</td>
             <td>TASKS_CURRENT</td>
             <td>TASKID</td>
        </tr>
    </tbody>
</table>

### 청구 요금

<table>
    <thead>
        <tr>
            <th>Workfront 엔티티 이름</th>
            <th>인터페이스 참조</th>
            <th>API 참조</th>
            <th>API 레이블</th>
            <th>데이터 레이크 보기</th>
        </tr>
      </thead>
      <tbody>
        <tr>
            <td>청구 요금</td>
            <td>비율 또는 재정의 비율</td>
            <td>비율</td>
            <td>청구 요금</td>
            <td>RATES_CURRENT<br>RATES_DAILY_HISTORY<br>RATES_EVENT</td>
        </tr>
      </tbody>
</table>
<table>
    <thead>
        <tr>
            <th>기본/외래 키</th>
            <th>유형</th>
            <th>관련 테이블</th>
            <th>관련 필드</th>
        </tr>
    </thead>
    <tbody>
        <tr>
             <td>ASSIGNMENTID</td>
             <td>FK</td>
             <td>ASSIGNMENTS_CURRENT</td>
             <td>ASSIGNMENTID</td>
        </tr>
        <tr>
             <td>분류자</td>
             <td>FK</td>
             <td>CLASSIFIER_CURRENT</td>
             <td>분류자</td>
        </tr>
        <tr>
             <td>EXCHANGERATEID</td>
             <td>FK</td>
             <td>EXCHANGE_CURRENT</td>
             <td>EXCHANGERATEID</td>
        </tr>
        <tr>
             <td>NLBRCATEGORYID</td>
             <td>FK</td>
             <td>NLBRCATEGORIES_CURRENT</td>
             <td>NLBRCATEGORYID</td>
        </tr>
        <tr>
             <td>NONLABORRESOURCEID</td>
             <td>FK</td>
             <td>NONLABORRESOURCES_CURRENT</td>
             <td>NONLABORRESOURCEID</td>
        </tr>
        <tr>
             <td>OBJID</td>
             <td>FK</td>
             <td>변수, OBJCODE 기반</td>
             <td>OBJCODE 필드에서 식별된 객체의 기본 키/ID</td>
        </tr>
        <tr>
             <td>PROJECTID</td>
             <td>FK</td>
             <td>PROJECTS_CURRENT</td>
             <td>PROJECTID</td>
        </tr>
        <tr>
             <td>RATECARDID</td>
             <td>FK</td>
             <td>RATECARD_CURRENT</td>
             <td>RATECARDID</td>
        </tr>
        <tr>
             <td>RATEID</td>
             <td>PK</td>
             <td>-</td>
             <td>-</td>
        </tr>
        <tr>
             <td>장미모양-</td>
             <td>FK</td>
             <td>ROLES_CURRENT</td>
             <td>장미모양-</td>
        </tr>
        <tr>
             <td>SOURCERATECARDID</td>
             <td>FK</td>
             <td>RATECARD_CURRENT</td>
             <td>RATECARDID</td>
        </tr>
        <tr>
             <td>SYSID</td>
             <td>-</td>
             <td colspan="2">관계가 아닙니다. 내부 응용 프로그램 용도로 사용됩니다.</td>
        </tr>
        <tr>
             <td>TEMPLATEID</td>
             <td>FK</td>
             <td>TEMPLATES_CURRENT</td>
             <td>TEMPLATEID</td>
        </tr>
        <tr>
             <td>사용자 ID</td>
             <td>FK</td>
             <td>USERS_CURRENT</td>
             <td>사용자 ID</td>
        </tr>
    </tbody>
</table>

### 청구 기록

<table>
    <thead>
        <tr>
            <th>Workfront 엔티티 이름</th>
            <th>인터페이스 참조</th>
            <th>API 참조</th>
            <th>API 레이블</th>
            <th>데이터 레이크 보기</th>
        </tr>
      </thead>
      <tbody>
        <tr>
            <td>청구 기록</td>
            <td>청구 기록</td>
            <td>청구서</td>
            <td>청구 기록</td>
            <td>BILLINGRECORDS_CURRENT<br>BILLINGRECORDS_DAILY_HISTORY<br>BILLINGRECORDS_EVENT</td>
        </tr>
      </tbody>
</table>
<table>
    <thead>
        <tr>
            <th>기본/외래 키</th>
            <th>유형</th>
            <th>관련 테이블</th>
            <th>관련 필드</th>
        </tr>
    </thead>
    <tbody>
        <tr>
             <td>빌링레코디드</td>
             <td>PK</td>
             <td>-</td>
             <td>-</td>
        </tr>
        <tr>
             <td>범주 ID</td>
             <td>FK</td>
             <td>CATEGORS_CURRENT</td>
             <td>범주 ID</td>
        </tr>
        <tr>
             <td>EXCHANGERATEID</td>
             <td>FK</td>
             <td>EXCHANGE_CURRENT</td>
             <td>EXCHANGERATEID</td>
        </tr>
        <tr>
             <td>INVOICID</td>
             <td>-</td>
             <td colspan="2">송장 테이블이 현재 지원되지 않음</td>
        </tr>
        <tr>
             <td>LASTUPDATEDBYID</td>
             <td>FK</td>
             <td>USERS_CURRENT</td>
             <td>사용자 ID</td>
        </tr>
        <tr>
             <td>PROJECTID</td>
             <td>FK</td>
             <td>PROJECTS_CURRENT</td>
             <td>PROJECTID</td>
        </tr>
        <tr>
             <td>SYSID</td>
             <td>-</td>
             <td colspan="2">관계가 아닙니다. 내부 응용 프로그램 용도로 사용됩니다.</td>
        </tr>
    </tbody>
</table>

### 예약

<table>
    <thead>
        <tr>
            <th>Workfront 엔티티 이름</th>
            <th>인터페이스 참조</th>
            <th>API 참조</th>
            <th>API 레이블</th>
            <th>데이터 레이크 보기</th>
        </tr>
      </thead>
      <tbody>
        <tr>
            <td>예약</td>
            <td>예약</td>
            <td>예약</td>
            <td>예약</td>
            <td>BOOKINGS_CURRENT<br>BOOKINGS_DAILY_HISTORY<br>BOOKINGS_EVENT</td>
        </tr>
      </tbody>
</table>
<table>
    <thead>
        <tr>
            <th>기본/외래 키</th>
            <th>유형</th>
            <th>관련 테이블</th>
            <th>관련 필드</th>
        </tr>
    </thead>
    <tbody>
        <tr>
             <td>BOOKINGID</td>
             <td>PK</td>
             <td>-</td>
             <td>-</td>
        </tr>
        <tr>
             <td>ENTEREDBYID</td>
             <td>FK</td>
             <td>USERS_CURRENT</td>
             <td>사용자 ID</td>
        </tr>
        <tr>
             <td>LASTUPDATEDBYID</td>
             <td>FK</td>
             <td>USERS_CURRENT</td>
             <td>사용자 ID</td>
        </tr>
        <tr>
             <td>NLBRCATEGORYID</td>
             <td>FK</td>
             <td>NLBRCATEGORIES_CURRENT</td>
             <td>NLBRCATEGORYID</td>
        </tr>
        <tr>
             <td>NONLABORRESOURCEID</td>
             <td>FK</td>
             <td>NONLABORRESOURCES_CURRENT</td>
             <td>NONLABORRESOURCEID</td>
        </tr>
        <tr>
             <td>OBJID</td>
             <td>FK</td>
             <td>변수, OBJCODE 기반</td>
             <td>OBJCODE 필드에서 식별된 객체의 기본 키/ID</td>
        </tr>
        <tr>
             <td>PROJECTID</td>
             <td>FK</td>
             <td>PROJECTS_CURRENT</td>
             <td>PROJECTID</td>
        </tr>
        <tr>
             <td>SYSID</td>
             <td>-</td>
             <td colspan="2">관계가 아닙니다. 내부 응용 프로그램 용도로 사용됩니다.</td>
        </tr>
        <tr>
             <td>TASKID</td>
             <td>FK</td>
             <td>TASKS_CURRENT</td>
             <td>TASKID</td>
        </tr>
        <tr>
             <td>TEMPLATEID</td>
             <td>FK</td>
             <td>TEMPLATES_CURRENT</td>
             <td>TEMPLATEID</td>
        </tr>
        <tr>
             <td>TEMPLATETASKID</td>
             <td>FK</td>
             <td>TEMPLATETASKS_CURRENT</td>
             <td>TEMPLATETASKID</td>
        </tr>
        <tr>
             <td>TOPOBJID</td>
             <td>FK</td>
             <td>변수, TOPOBJCODE 기반</td>
             <td>TOPOBJCODE 필드에서 식별된 객체의 기본 키/ID</td>
        </tr>
    </tbody>
</table>

### 비즈니스 프로필

<table>
    <thead>
        <tr>
            <th>Workfront 엔티티 이름</th>
            <th>인터페이스 참조</th>
            <th>API 참조</th>
            <th>API 레이블</th>
            <th>데이터 레이크 보기</th>
        </tr>
      </thead>
      <tbody>
        <tr>
            <td>비즈니스 프로필</td>
            <td>비즈니스 프로필</td>
            <td>BSNPRF</td>
            <td>비즈니스 프로필</td>
            <td>BUSINESSPROFILE_CURRENT<br>BUSINESSPROFILE_DAILY_HISTORY<br>BUSINESSPROFILE_EVENT</td>
        </tr>
      </tbody>
</table>
<table>
    <thead>
        <tr>
            <th>기본/외래 키</th>
            <th>유형</th>
            <th>관련 테이블</th>
            <th>관련 필드</th>
        </tr>
    </thead>
    <tbody>
        <tr>
             <td>ACCESSLEVELID</td>
             <td>FK</td>
             <td>ACCESSLEVELS_CURRENT</td>
             <td>ACCESSLEVELID</td>
        </tr>
        <tr>
             <td>BUSINESSPROFILEID</td>
             <td>PK</td>
             <td>-</td>
             <td>-</td>
        </tr>
        <tr>
             <td>ENTEREDBYID</td>
             <td>FK</td>
             <td>USERS_CURRENT</td>
             <td>사용자 ID</td>
        </tr>
        <tr>
             <td>GROUPID</td>
             <td>FK</td>
             <td>GROUPS_CURRENT</td>
             <td>GROUPID</td>
        </tr>
        <tr>
             <td>LASTUPDATEDBYID</td>
             <td>FK</td>
             <td>USERS_CURRENT</td>
             <td>사용자 ID</td>
        </tr>
        <tr>
             <td>SYSID</td>
             <td>-</td>
             <td colspan="2">관계가 아닙니다. 내부 응용 프로그램 용도로 사용됩니다.</td>
        </tr>
    </tbody>
</table>

### 비즈니스 규칙

<table>
    <thead>
        <tr>
            <th>Workfront 엔티티 이름</th>
            <th>인터페이스 참조</th>
            <th>API 참조</th>
            <th>API 레이블</th>
            <th>데이터 레이크 보기</th>
        </tr>
      </thead>
      <tbody>
        <tr>
            <td>비즈니스 규칙</td>
            <td>비즈니스 규칙</td>
            <td>BSNRUL</td>
            <td>비즈니스 규칙</td>
            <td>BUSINESSRULE_CURRENT<br>BUSINESSRULE_DAILY_HISTORY<br>BUSINESSRULE_EVENT</td>
        </tr>
      </tbody>
</table>
<table>
    <thead>
        <tr>
            <th>기본/외래 키</th>
            <th>유형</th>
            <th>관련 테이블</th>
            <th>관련 필드</th>
        </tr>
    </thead>
    <tbody>
        <tr>
             <td>BUSINESSRULEID</td>
             <td>PK</td>
             <td>-</td>
             <td>-</td>
        </tr>
        <tr>
             <td>ENTEREDBYID</td>
             <td>FK</td>
             <td>USERS_CURRENT</td>
             <td>사용자 ID</td>
        </tr>
        <tr>
             <td>LASTUPDATEDBYID</td>
             <td>FK</td>
             <td>USERS_CURRENT</td>
             <td>사용자 ID</td>
        </tr>
        <tr>
             <td>SYSID</td>
             <td>-</td>
             <td colspan="2">관계가 아닙니다. 내부 응용 프로그램 용도로 사용됩니다.</td>
        </tr>
    </tbody>
</table>

### 카테고리

<table>
    <thead>
        <tr>
            <th>Workfront 엔티티 이름</th>
            <th>인터페이스 참조</th>
            <th>API 참조</th>
            <th>API 레이블</th>
            <th>데이터 레이크 보기</th>
        </tr>
      </thead>
      <tbody>
        <tr>
            <td>카테고리</td>
            <td>사용자 정의 양식</td>
            <td>CTGY</td>
            <td>카테고리</td>
            <td>CATEGORIES_CURRENT<br>CATEGORIES_DAILY_HISTORY<br>CATEGORIES_EVENT</td>
        </tr>
      </tbody>
</table>
<table>
    <thead>
        <tr>
            <th>기본/외래 키</th>
            <th>유형</th>
            <th>관련 테이블</th>
            <th>관련 필드</th>
        </tr>
    </thead>
    <tbody>
        <tr>
             <td>범주 ID</td>
             <td>PK</td>
             <td>-</td>
             <td>-</td>
        </tr>
        <tr>
             <td>ENTEREDBYID</td>
             <td>FK</td>
             <td>USERS_CURRENT</td>
             <td>사용자 ID</td>
        </tr>
        <tr>
             <td>GROUPID</td>
             <td>FK</td>
             <td>GROUPS_CURRENT</td>
             <td>GROUPID</td>
        </tr>
        <tr>
             <td>LASTUPDATEDBYID</td>
             <td>FK</td>
             <td>USERS_CURRENT</td>
             <td>사용자 ID</td>
        </tr>
        <tr>
             <td>SYSID</td>
             <td>-</td>
             <td colspan="2">관계가 아닙니다. 내부 응용 프로그램 용도로 사용됩니다.</td>
        </tr>
    </tbody>
</table>

### 범주 매개변수

<table>
    <thead>
        <tr>
            <th>Workfront 엔티티 이름</th>
            <th>인터페이스 참조</th>
            <th>API 참조</th>
            <th>API 레이블</th>
            <th>데이터 레이크 보기</th>
        </tr>
      </thead>
      <tbody>
        <tr>
            <td>범주 매개변수</td>
            <td>사용자 정의 양식 필드</td>
            <td>CTGYA</td>
            <td>범주 매개변수</td>
            <td>CATEGORIESPARAMETERS_CURRENT<br>CATEGORIESPARAMETERS_DAILY_HISTORY<br>CATEGORIESPARAMETERS_EVENT</td>
        </tr>
      </tbody>
</table>
<table>
    <thead>
        <tr>
            <th>기본/외래 키</th>
            <th>유형</th>
            <th>관련 테이블</th>
            <th>관련 필드</th>
        </tr>
    </thead>
    <tbody>
        <tr>
             <td>CATEGORIESPARAMETERID</td>
             <td>PK</td>
             <td>-</td>
             <td>-</td>
        </tr>
        <tr>
             <td>범주 ID</td>
             <td>FK</td>
             <td>CATEGORS_CURRENT</td>
             <td>범주 ID</td>
        </tr>
        <tr>
             <td>PARAMETERGROUPID</td>
             <td>FK</td>
             <td>PARAMETERGROUPS_CURRENT</td>
             <td>PARAMETERGROUPID</td>
        </tr>
        <tr>
             <td>매개 변수화</td>
             <td>FK</td>
             <td>PARAMETERS_CURRENT</td>
             <td>매개 변수화</td>
        </tr>
        <tr>
             <td>SYSID</td>
             <td>-</td>
             <td colspan="2">관계가 아닙니다. 내부 응용 프로그램 용도로 사용됩니다.</td>
        </tr>
    </tbody>
</table>

### 분류자

<table>
    <thead>
        <tr>
            <th>Workfront 엔티티 이름</th>
            <th>인터페이스 참조</th>
            <th>API 참조</th>
            <th>API 레이블</th>
            <th>데이터 레이크 보기</th>
        </tr>
      </thead>
      <tbody>
        <tr>
            <td>분류자</td>
            <td>위치</td>
            <td>CLSF</td>
            <td>위치</td>
            <td>CLASSIFIER_CURRENT<br>CLASSIFIER_DAILY_HISTORY<br>CLASSIFIER_EVENT</td>
        </tr>
      </tbody>
</table>
<table>
    <thead>
        <tr>
            <th>기본/외래 키</th>
            <th>유형</th>
            <th>관련 테이블</th>
            <th>관련 필드</th>
        </tr>
    </thead>
    <tbody>
        <tr>
             <td>분류자</td>
             <td>PK</td>
             <td>-</td>
             <td>-</td>
        </tr>
        <tr>
             <td>ENTEREDBYID</td>
             <td>FK</td>
             <td>USERS_CURRENT</td>
             <td>사용자 ID</td>
        </tr>
        <tr>
             <td>LASTUPDATEDBYID</td>
             <td>FK</td>
             <td>USERS_CURRENT</td>
             <td>사용자 ID</td>
        </tr>
        <tr>
             <td>괄호 ID</td>
             <td>FK</td>
             <td>CLASSIFIER_CURRENT</td>
             <td>분류자</td>
        </tr>
        <tr>
             <td>SYSID</td>
             <td>-</td>
             <td colspan="2">관계가 아닙니다. 내부 응용 프로그램 용도로 사용됩니다.</td>
        </tr>
    </tbody>
</table>

### 회사

<table>
    <thead>
        <tr>
            <th>Workfront 엔티티 이름</th>
            <th>인터페이스 참조</th>
            <th>API 참조</th>
            <th>API 레이블</th>
            <th>데이터 레이크 보기</th>
        </tr>
      </thead>
      <tbody>
        <tr>
            <td>회사</td>
            <td>회사</td>
            <td>지저분해</td>
            <td>회사</td>
            <td>COMPANIES_CURRENT<br>COMPANIES_DAILY_HISTORY<br>COMPANIES_EVENT</td>
        </tr>
      </tbody>
</table>
<table>
    <thead>
        <tr>
            <th>기본/외래 키</th>
            <th>유형</th>
            <th>관련 테이블</th>
            <th>관련 필드</th>
        </tr>
    </thead>
    <tbody>
        <tr>
             <td>범주 ID</td>
             <td>FK</td>
             <td>CATEGORS_CURRENT</td>
             <td>범주 ID</td>
        </tr>
        <tr>
             <td>COMPANYID</td>
             <td>PK</td>
             <td>-</td>
             <td>-</td>
        </tr>
        <tr>
             <td>ENTEREDBYID</td>
             <td>FK</td>
             <td>USERS_CURRENT</td>
             <td>사용자 ID</td>
        </tr>
        <tr>
             <td>GROUPID</td>
             <td>FK</td>
             <td>GROUPS_CURRENT</td>
             <td>GROUPID</td>
        </tr>
        <tr>
             <td>LASTUPDATEDBYID</td>
             <td>FK</td>
             <td>USERS_CURRENT</td>
             <td>사용자 ID</td>
        </tr>
        <tr>
             <td>PRIVATERATECARDID</td>
             <td>FK</td>
             <td>RATECARD_CURRENT</td>
             <td>RATECARDID</td>
        </tr>
        <tr>
             <td>SYSID</td>
             <td>-</td>
             <td colspan="2">관계가 아닙니다. 내부 응용 프로그램 용도로 사용됩니다.</td>
        </tr>
    </tbody>
</table>

### 사용자 정의 분기

<table>
    <thead>
        <tr>
            <th>Workfront 엔티티 이름</th>
            <th>인터페이스 참조</th>
            <th>API 참조</th>
            <th>API 레이블</th>
            <th>데이터 레이크 보기</th>
        </tr>
      </thead>
      <tbody>
        <tr>
            <td>사용자 정의 분기</td>
            <td>사용자 정의 분기</td>
            <td>CSTQRT</td>
            <td>사용자 정의 분기</td>
            <td>CUSTOMQUARTERS_CURRENT<br>CUSTOMQUARTERS_DAILY_HISTORY<br>CUSTOMQUARTERS_EVENT</td>
        </tr>
      </tbody>
</table>
<table>
    <thead>
        <tr>
            <th>기본/외래 키</th>
            <th>유형</th>
            <th>관련 테이블</th>
            <th>관련 필드</th>
        </tr>
    </thead>
    <tbody>
        <tr>
             <td>CUSTOMQUARTERID</td>
             <td>PK</td>
             <td>-</td>
             <td>-</td>
        </tr>
        <tr>
             <td>SYSID</td>
             <td>-</td>
             <td colspan="2">관계가 아닙니다. 내부 응용 프로그램 용도로 사용됩니다.</td>
        </tr>
    </tbody>
</table>

### 사용자 정의 열거형

<table>
    <thead>
        <tr>
            <th>Workfront 엔티티 이름</th>
            <th>인터페이스 참조</th>
            <th>API 참조</th>
            <th>API 레이블</th>
            <th>데이터 레이크 보기</th>
        </tr>
      </thead>
      <tbody>
        <tr>
            <td>CustomEnum</td>
            <td>상태, 우선 순위, 심각도, 상태</td>
            <td>CSTEM</td>
            <td>사용자 정의 열거형</td>
            <td>CUSTOMENUMS_CURRENT<br>CUSTOMENUMS_DAILY_HISTORY<br>CUSTOMENUMS_EVENT</td>
        </tr>
      </tbody>
</table>
<table>
    <thead>
        <tr>
            <th>기본/외래 키</th>
            <th>유형</th>
            <th>관련 테이블</th>
            <th>관련 필드</th>
        </tr>
    </thead>
    <tbody>
        <tr>
             <td>CUSTOMENUMID</td>
             <td>PK</td>
             <td>-</td>
             <td>-</td>
        </tr>
        <tr>
             <td>ENTEREDBYID</td>
             <td>FK</td>
             <td>USERS_CURRENT</td>
             <td>사용자 ID</td>
        </tr>
        <tr>
             <td>GROUPID</td>
             <td>FK</td>
             <td>GROUPS_CURRENT</td>
             <td>GROUPID</td>
        </tr>
        <tr>
             <td>LASTUPDATEDBYID</td>
             <td>FK</td>
             <td>USERS_CURRENT</td>
             <td>사용자 ID</td>
        </tr>
        <tr>
             <td>SYSID</td>
             <td>-</td>
             <td colspan="2">관계가 아닙니다. 내부 응용 프로그램 용도로 사용됩니다.</td>
        </tr>
    </tbody>
</table>
<div>* 레코드 유형은 'enumClass' 속성을 통해 식별됩니다. 다음은 예상 형식입니다.<br>
<ul><li>CONDITION_OPTASK</li>
<li>CONDITION_PROJ</li>
<li>CONDITION_TASK</li>
<li>PRIORITY_OPTASK</li>
<li>PRIORITY_PROJECT</li>
<li>PRIORITY_TASK</li>
<li>SEVERITY_OPTASK</li>
<li>STATUS_OPTASK</li>
<li>STATUS_PROJECT</li>
<li>STATUS_TASK</li></ul></div>

### 문서

<table>
    <thead>
        <tr>
            <th>Workfront 엔티티 이름</th>
            <th>인터페이스 참조</th>
            <th>API 참조</th>
            <th>API 레이블</th>
            <th>데이터 레이크 보기</th>
        </tr>
      </thead>
      <tbody>
        <tr>
            <td>문서</td>
            <td>문서</td>
            <td>도쿠</td>
            <td>문서</td>
            <td>DOCUMENTS_CURRENT<br>DOCUMENTS_DAILY_HISTORY<br>DOCUMENTS_EVENT</td>
        </tr>
      </tbody>
</table>
<table>
    <thead>
        <tr>
            <th>기본/외래 키</th>
            <th>유형</th>
            <th>관련 테이블</th>
            <th>관련 필드</th>
        </tr>
    </thead>
    <tbody>
        <tr>
             <td>범주 ID</td>
             <td>FK</td>
             <td>CATEGORS_CURRENT</td>
             <td>범주 ID</td>
        </tr>
        <tr>
             <td>CHECKEDOUTBYID</td>
             <td>FK</td>
             <td>USERS_CURRENT</td>
             <td>사용자 ID</td>
        </tr>
        <tr>
             <td>DOCUMENTID</td>
             <td>PK</td>
             <td>-</td>
             <td>-</td>
        </tr>
        <tr>
             <td>DOCUMENTREQUESTID</td>
             <td>-</td>
             <td colspan="2">문서 요청 테이블은 현재 지원되지 않습니다.</td>
        </tr>
        <tr>
             <td>EXCHANGERATEID</td>
             <td>FK</td>
             <td>EXCHANGE_CURRENT</td>
             <td>EXCHANGERATEID</td>
        </tr>
        <tr>
             <td>ITERATIONID</td>
             <td>FK</td>
             <td>ITERATIONS_CURRENT</td>
             <td>ITERATIONID</td>
        </tr>
        <tr>
             <td>LASTNOTEID</td>
             <td>FK</td>
             <td>NOTES_CURRENT</td>
             <td>NOTEID</td>
        </tr>
        <tr>
             <td>LASTUPDATEDBYID</td>
             <td>FK</td>
             <td>USERS_CURRENT</td>
             <td>사용자 ID</td>
        </tr>
        <tr>
             <td>NOTEID</td>
             <td>FK</td>
             <td>NOTES_CURRENT</td>
             <td>NOTEID</td>
        </tr>
        <tr>
             <td>OBJID</td>
             <td>FK</td>
             <td>변수, OBJCODE 기반</td>
             <td>OBJCODE 필드에서 식별된 객체의 기본 키/ID</td>
        </tr>
        <tr>
             <td>OPTASKID</td>
             <td>FK</td>
             <td>OPTASKS_CURRENT</td>
             <td>OPTASKID</td>
        </tr>
        <tr>
             <td>소유자 ID</td>
             <td>FK</td>
             <td>USERS_CURRENT</td>
             <td>사용자 ID</td>
        </tr>
        <tr>
             <td>포트폴리오</td>
             <td>FK</td>
             <td>포트폴리오_현재</td>
             <td>포트폴리오</td>
        </tr>
        <tr>
             <td>PROGRAMID</td>
             <td>FK</td>
             <td>PROGRAMS_CURRENT</td>
             <td>PROGRAMID</td>
        </tr>
        <tr>
             <td>PROJECTID</td>
             <td>FK</td>
             <td>PROJECTS_CURRENT</td>
             <td>PROJECTID</td>
        </tr>
        <tr>
             <td>RELEASEVERSIONID</td>
             <td>-</td>
             <td colspan="2">릴리스 버전 테이블은 현재 지원되지 않습니다.</td>
        </tr>
        <tr>
             <td>SYSID</td>
             <td>-</td>
             <td colspan="2">관계가 아닙니다. 내부 응용 프로그램 용도로 사용됩니다.</td>
        </tr>
        <tr>
             <td>TASKID</td>
             <td>FK</td>
             <td>TASKS_CURRENT</td>
             <td>TASKID</td>
        </tr>
        <tr>
             <td>TEMPLATEID</td>
             <td>FK</td>
             <td>TEMPLATES_CURRENT</td>
             <td>TEMPLATEID</td>
        </tr>
        <tr>
             <td>TEMPLATETASKID</td>
             <td>FK</td>
             <td>TEMPLATETASKS_CURRENT</td>
             <td>TEMPLATETASKID</td>
        </tr>
        <tr>
             <td>TOPOBJID</td>
             <td>FK</td>
             <td>변수, TOPOBJCODE 기반</td>
             <td>TOPOBJCODE 필드에서 식별된 객체의 기본 키/ID</td>
        </tr>
        <tr>
             <td>사용자 ID</td>
             <td>FK</td>
             <td>USERS_CURRENT</td>
             <td>사용자 ID</td>
        </tr>
    </tbody>
</table>

### 문서 승인

<table>
    <thead>
        <tr>
            <th>Workfront 엔티티 이름</th>
            <th>인터페이스 참조</th>
            <th>API 참조</th>
            <th>API 레이블</th>
            <th>데이터 레이크 보기</th>
        </tr>
      </thead>
      <tbody>
        <tr>
            <td>문서 승인</td>
            <td>문서 승인</td>
            <td>DOCAPL</td>
            <td>문서 승인</td>
            <td>DOCAPPROVALS_CURRENT<br>DOCAPPROVALS_DAILY_HISTORY<br>DOCAPPROVALS_EVENT</td>
        </tr>
      </tbody>
</table>
<table>
    <thead>
        <tr>
            <th>기본/외래 키</th>
            <th>유형</th>
            <th>관련 테이블</th>
            <th>관련 필드</th>
        </tr>
    </thead>
    <tbody>
        <tr>
             <td>승인자 ID</td>
             <td>FK</td>
             <td>USERS_CURRENT</td>
             <td>사용자 ID</td>
        </tr>
        <tr>
             <td>DOCAPPROVALID</td>
             <td>PK</td>
             <td>-</td>
             <td>-</td>
        </tr>
        <tr>
             <td>DOCUMENTID</td>
             <td>FK</td>
             <td>DOCUMENTS_CURRENT</td>
             <td>DOCUMENTID</td>
        </tr>
        <tr>
             <td>NOTEID</td>
             <td>FK</td>
             <td>NOTES_CURRENT</td>
             <td>NOTEID</td>
        </tr>
        <tr>
             <td>REQUESTORID</td>
             <td>FK</td>
             <td>USERS_CURRENT</td>
             <td>사용자 ID</td>
        </tr>
        <tr>
             <td>SYSID</td>
             <td>-</td>
             <td colspan="2">관계가 아닙니다. 내부 응용 프로그램 용도로 사용됩니다.</td>
        </tr>
    </tbody>
</table>

### 문서 승인(신규)

제한된 고객 가용성

<table>
    <thead>
        <tr>
            <th>Workfront 엔티티 이름</th>
            <th>인터페이스 참조</th>
            <th>API 참조</th>
            <th>API 레이블</th>
            <th>데이터 레이크 보기</th>
        </tr>
      </thead>
      <tbody>
        <tr>
            <td>문서 승인</td>
            <td>승인</td>
            <td>해당 사항 없음</td>
            <td>해당 사항 없음</td>
            <td>APPROVAL_CURRENT<br>APPROVAL_DAILY_HISTORY<br>APPROVAL_EVENT</td>
        </tr>
      </tbody>
</table>
<table>
    <thead>
        <tr>
            <th>기본/외래 키</th>
            <th>유형</th>
            <th>관련 테이블</th>
            <th>관련 필드</th>
        </tr>
    </thead>
    <tbody>
        <tr>
             <td class="key">승인 가능하</td>
             <td>PK</td>
             <td>-</td>
             <td>참고: 승인과 연결된 DOCUMENTVERSION 개체의 ID이기도 합니다.</td>
        </tr>
        <tr>
             <td class="key">ASSETID</td>
             <td>FK</td>
             <td>변수, ASSETTYPE 기반</td>
             <td>ASSETTYPE 필드에서 식별된 객체의 기본 키/ID</td>
        </tr>
        <tr>
             <td class="key">크리토이드</td>
             <td>FK</td>
             <td>USERS_CURRENT</td>
             <td>사용자 ID</td>
        </tr>
        <tr>
             <td class="key">이우테난티드</td>
             <td>-</td>
             <td colspan="2">관계가 아닙니다. 내부 응용 프로그램 용도로 사용됩니다.</td>
        </tr>
        <tr>
             <td class="key">PRODUCTID</td>
             <td>-</td>
             <td colspan="2">관계가 아닙니다. 내부 응용 프로그램 용도로 사용됩니다.</td>
        </tr>
        <tr>
             <td class="key">REALCREATORID</td>
             <td>FK</td>
             <td>USERS_CURRENT</td>
             <td>사용자 ID</td>
        </tr>
    </tbody>
</table>

### 문서 승인 단계(신규)

제한된 고객 가용성

<table>
    <thead>
        <tr>
            <th>Workfront 엔티티 이름</th>
            <th>인터페이스 참조</th>
            <th>API 참조</th>
            <th>API 레이블</th>
            <th>데이터 레이크 보기</th>
        </tr>
      </thead>
      <tbody>
        <tr>
            <td>문서 승인 단계</td>
            <td>승인 단계</td>
            <td>해당 사항 없음</td>
            <td>해당 사항 없음</td>
            <td>APPROVAL_STAGE_CURRENT<br>APPROVAL_STAGE_DAILY_HISTORY<br>APPROVAL_STAGE_EVENT</td>
        </tr>
      </tbody>
</table>
<table>
    <thead>
        <tr>
            <th>기본/외래 키</th>
            <th>유형</th>
            <th>관련 테이블</th>
            <th>관련 필드</th>
        </tr>
    </thead>
    <tbody>
        <tr>
             <td class="key">승인 가능하</td>
             <td>FK</td>
             <td>APPROVAL_CURRENT</td>
             <td>승인 가능하</td>
        </tr>
        <tr>
             <td class="key">APPROVALSTAGEID</td>
             <td>PK</td>
             <td>-</td>
             <td>-</td>
        </tr>
        <tr>
             <td class="key">크리토이드</td>
             <td>FK</td>
             <td>USERS_CURRENT</td>
             <td>사용자 ID</td>
        </tr>
        <tr>
             <td class="key">OBJID</td>
             <td class="type">FK</td>
             <td class="relatedtable">변수, OBJCODE 기반</td>
             <td>OBJCODE 필드에서 식별된 객체의 기본 키/ID</td>
        </tr>
    </tbody>
</table>

### 문서 승인 단계 참가자(신규)

제한된 고객 가용성

<table>
    <thead>
        <tr>
            <th>Workfront 엔티티 이름</th>
            <th>인터페이스 참조</th>
            <th>API 참조</th>
            <th>API 레이블</th>
            <th>데이터 레이크 보기</th>
        </tr>
      </thead>
      <tbody>
        <tr>
            <td>문서 승인 단계 참가자</td>
            <td>승인 결정</td>
            <td>해당 사항 없음</td>
            <td>해당 사항 없음</td>
            <td>APPROVAL_STAGE_PARTICIPANT_CURRENT<br>APPROVAL_STAGE_PARTICIPANT_DAILY_HISTORY<br>APPROVAL_STAGE_PARTICIPANT_EVENT</td>
        </tr>
      </tbody>
</table>
<table>
    <thead>
        <tr>
            <th>기본/외래 키</th>
            <th>유형</th>
            <th>관련 테이블</th>
            <th>관련 필드</th>
        </tr>
    </thead>
    <tbody>
        <tr>
             <td class="key">승인 가능하</td>
             <td>FK</td>
             <td>APPROVAL_CURRENT</td>
             <td>승인 가능하</td>
        </tr>
        <tr>
             <td class="key">APPROVALSTAGEPARTICIPANTID/td&gt;
             <td>PK</td>
             <td>-</td>
             <td>-</td>
        </tr>
        <tr>
             <td class="key">ASSETID</td>
             <td>FK</td>
             <td>변수, ASSETTYPE 기반</td>
             <td>ASSETTYPE 필드에서 식별된 객체의 기본 키/ID</td>
        </tr>
        <tr>
             <td class="key">DECISIONUSERID</td>
             <td>FK</td>
             <td>USERS_CURRENT</td>
             <td>사용자 ID</td>
        </tr>
        <tr>
             <td class="key">OBJID</td>
             <td class="type">FK</td>
             <td class="relatedtable">변수, OBJCODE 기반</td>
             <td>OBJCODE 필드에서 식별된 객체의 기본 키/ID</td>
        </tr>
        <tr>
             <td class="key">입천장염-</td>
             <td>FK</td>
             <td class="relatedtable">변수, PARTICIPANTTYPE 기반</td>
             <td>PARTICIPANTTYPE 필드에서 식별된 객체의 기본 키/ID</td>
        </tr>
        <tr>
             <td class="key">REALREQUESTORID</td>
             <td>FK</td>
             <td>USERS_CURRENT</td>
             <td>사용자 ID</td>
        </tr>
        <tr>
             <td class="key">REALUSERID</td>
             <td>FK</td>
             <td>USERS_CURRENT</td>
             <td>사용자 ID</td>
        </tr>
        <tr>
             <td class="key">REQUESTORID</td>
             <td>FK</td>
             <td>USERS_CURRENT</td>
             <td>사용자 ID</td>
        </tr>
        <tr>
             <td class="key">STAGID</td>
             <td>FK</td>
             <td>APPROVAL_STAGE_CURRENT</td>
             <td>STAGID</td>
        </tr>
    </tbody>
</table>

### 문서 폴더

<table>
    <thead>
        <tr>
            <th>Workfront 엔티티 이름</th>
            <th>인터페이스 참조</th>
            <th>API 참조</th>
            <th>API 레이블</th>
            <th>데이터 레이크 보기</th>
        </tr>
      </thead>
      <tbody>
        <tr>
            <td>문서 폴더</td>
            <td>문서 폴더</td>
            <td>DOCFLD</td>
            <td>문서 폴더</td>
            <td>DOCTFOLDERS_CURRENT<br>DOCTFOLDERS_DAILY_HISTORY<br>DOCTFOLDERS_EVENT</td>
        </tr>
      </tbody>
</table>
<table>
    <thead>
        <tr>
            <th>기본/외래 키</th>
            <th>유형</th>
            <th>관련 테이블</th>
            <th>관련 필드</th>
        </tr>
    </thead>
    <tbody>
        <tr>
             <td>DOCFOLDERID</td>
             <td>PK</td>
             <td>-</td>
             <td>-</td>
        </tr>
        <tr>
             <td>ENTEREDBYID</td>
             <td>FK</td>
             <td>USERS_CURRENT</td>
             <td>사용자 ID</td>
        </tr>
        <tr>
             <td>ISSUEID</td>
             <td>FK</td>
             <td>OPTASKS_CURRENT</td>
             <td>OPTASKID</td>
        </tr>
        <tr>
             <td>ITERATIONID</td>
             <td>FK</td>
             <td>ITERATIONS_CURRENT</td>
             <td>ITERATIONID</td>
        </tr>
        <tr>
             <td>LINKEDFOLDERID</td>
             <td>FK</td>
             <td>LINKEDFOLDERS_CURRENT</td>
             <td>LINKEDFOLDERID</td>
        </tr>
        <tr>
             <td>괄호 ID</td>
             <td>FK</td>
             <td>DOCFOLDERS_CURRENT</td>
             <td>DOCFOLDERID</td>
        </tr>
        <tr>
             <td>포트폴리오</td>
             <td>FK</td>
             <td>포트폴리오_현재</td>
             <td>포트폴리오</td>
        </tr>
        <tr>
             <td>PROGRAMID</td>
             <td>FK</td>
             <td>PROGRAMS_CURRENT</td>
             <td>PROGRAMID</td>
        </tr>
        <tr>
             <td>PROJECTID</td>
             <td>FK</td>
             <td>PROJECTS_CURRENT</td>
             <td>PROJECTID</td>
        </tr>
        <tr>
             <td>SYSID</td>
             <td>-</td>
             <td colspan="2">관계가 아닙니다. 내부 응용 프로그램 용도로 사용됩니다.</td>
        </tr>
        <tr>
             <td>TASKID</td>
             <td>FK</td>
             <td>TASKS_CURRENT</td>
             <td>TASKID</td>
        </tr>
        <tr>
             <td>TEMPLATEID</td>
             <td>FK</td>
             <td>TEMPLATES_CURRENT</td>
             <td>TEMPLATEID</td>
        </tr>
        <tr>
             <td>TEMPLATETASKID</td>
             <td>FK</td>
             <td>TEMPLATETASKS_CURRENT</td>
             <td>TEMPLATETASKID</td>
        </tr>
        <tr>
             <td>사용자 ID</td>
             <td>FK</td>
             <td>USERS_CURRENT</td>
             <td>사용자 ID</td>
        </tr>
    </tbody>
</table>

### 문서 공급자 메타데이터

<table>
    <thead>
        <tr>
            <th>Workfront 엔티티 이름</th>
            <th>인터페이스 참조</th>
            <th>API 참조</th>
            <th>API 레이블</th>
            <th>데이터 레이크 보기</th>
        </tr>
      </thead>
      <tbody>
        <tr>
            <td>문서 공급자 메타데이터</td>
            <td>문서 공급자 메타데이터</td>
            <td>문서</td>
            <td>문서 공급자 메타데이터</td>
            <td>DOCTPROVIDERMETA_CURRENT<br>DOCTPROVIDERMETA_DAILY_HISTORY<br>DOCTPROVIDERMETA_EVENT</td>
        </tr>
      </tbody>
</table>
<table>
    <thead>
        <tr>
            <th>기본/외래 키</th>
            <th>유형</th>
            <th>관련 테이블</th>
            <th>관련 필드</th>
        </tr>
    </thead>
    <tbody>
        <tr>
             <td>DOCPROVIDERMETAID</td>
             <td>PK</td>
             <td>-</td>
             <td>-</td>
        </tr>
        <tr>
             <td>SYSID</td>
             <td>-</td>
             <td colspan="2">관계가 아닙니다. 내부 응용 프로그램 용도로 사용됩니다.</td>
        </tr>
    </tbody>
</table>

### 문서 공급자

<table>
    <thead>
        <tr>
            <th>Workfront 엔티티 이름</th>
            <th>인터페이스 참조</th>
            <th>API 참조</th>
            <th>API 레이블</th>
            <th>데이터 레이크 보기</th>
        </tr>
      </thead>
      <tbody>
        <tr>
            <td>문서 공급자</td>
            <td>문서 공급자</td>
            <td>DOCPRO</td>
            <td>문서 공급자</td>
            <td>DOCPROVIDERS_CURRENT<br>DOCPROVIDERS_DAILY_HISTORY<br>DOCPROVIDERS_EVENT</td>
        </tr>
      </tbody>
</table>
<table>
    <thead>
        <tr>
            <th>기본/외래 키</th>
            <th>유형</th>
            <th>관련 테이블</th>
            <th>관련 필드</th>
        </tr>
    </thead>
    <tbody>
        <tr>
             <td>DOCTPROVIDERCONFIGID</td>
             <td>FK</td>
             <td>DOCPROVIDERCONFIG_CURRENT</td>
             <td>DOCTPROVIDERCONFIGID</td>
        </tr>
        <tr>
             <td>DOCPROVIDERID</td>
             <td>PK</td>
             <td>-</td>
             <td>-</td>
        </tr>
        <tr>
             <td>소유자 ID</td>
             <td>FK</td>
             <td>USERS_CURRENT</td>
             <td>사용자 ID</td>
        </tr>
        <tr>
             <td>SYSID</td>
             <td>-</td>
             <td colspan="2">관계가 아닙니다. 내부 응용 프로그램 용도로 사용됩니다.</td>
        </tr>
    </tbody>
</table>

### 문서 공급자 구성

<table>
    <thead>
        <tr>
            <th>Workfront 엔티티 이름</th>
            <th>인터페이스 참조</th>
            <th>API 참조</th>
            <th>API 레이블</th>
            <th>데이터 레이크 보기</th>
        </tr>
      </thead>
      <tbody>
        <tr>
            <td>문서 공급자 구성</td>
            <td>문서 공급자 구성</td>
            <td>DOCCFG</td>
            <td>DocumentProviderConfig</td>
            <td>DOCTPROVIDERCONFIG_CURRENT<br>DOCTPROVIDERCONFIG_DAILY_HISTORY<br>DOCTPROVIDERCONFIG_EVENT</td>
        </tr>
      </tbody>
</table>
<table>
    <thead>
        <tr>
            <th>기본/외래 키</th>
            <th>유형</th>
            <th>관련 테이블</th>
            <th>관련 필드</th>
        </tr>
    </thead>
    <tbody>
        <tr>
             <td>DOCTPROVIDERCONFIGID</td>
             <td>PK</td>
             <td>-</td>
             <td>-</td>
        </tr>
        <tr>
             <td>SYSID</td>
             <td>-</td>
             <td colspan="2">관계가 아닙니다. 내부 응용 프로그램 용도로 사용됩니다.</td>
        </tr>
    </tbody>
</table>

### 문서 버전

<table>
    <thead>
        <tr>
            <th>Workfront 엔티티 이름</th>
            <th>인터페이스 참조</th>
            <th>API 참조</th>
            <th>API 레이블</th>
            <th>데이터 레이크 보기</th>
        </tr>
      </thead>
      <tbody>
        <tr>
            <td>문서 버전</td>
            <td>문서 버전</td>
            <td>DOCV</td>
            <td>문서 버전</td>
            <td>DOCUMENTVERSIONS_CURRENT<br>DOCUMENTVERSIONS_DAILY_HISTORY<br>DOCUMENTVERSIONS_EVENT</td>
        </tr>
      </tbody>
</table>
<table>
    <thead>
        <tr>
            <th>기본/외래 키</th>
            <th>유형</th>
            <th>관련 테이블</th>
            <th>관련 필드</th>
        </tr>
    </thead>
    <tbody>
        <tr>
             <td>DOCUMENTID</td>
             <td>FK</td>
             <td>DOCUMENTS_CURRENT</td>
             <td>DOCUMENTID</td>
        </tr>
        <tr>
             <td>DOCUMENTPROVIDERID</td>
             <td>FK</td>
             <td>DOCPROVIDERS_CURRENT</td>
             <td>DOCUMENTPROVIDERID</td>
        </tr>
        <tr>
             <td>DOCUMENTVERSIONID</td>
             <td>PK</td>
             <td>-</td>
             <td>-</td>
        </tr>
        <tr>
             <td>ENTEREDBYID</td>
             <td>FK</td>
             <td>USERS_CURRENT</td>
             <td>사용자 ID</td>
        </tr>
        <tr>
             <td>EXTERNALSTORAGEID</td>
             <td>-</td>
             <td colspan="2">외부 스토리지 시스템의 외부 ID</td>
        </tr>
        <tr>
             <td>PROOFAPPROVALSTATUSID</td>
             <td>-</td>
             <td colspan="2">증명 승인 상태 테이블은 현재 지원되지 않음</td>
        </tr>
        <tr>
             <td>PROFEDBYUSERID</td>
             <td>FK</td>
             <td>USERS_CURRENT</td>
             <td>사용자 ID</td>
        </tr>
        <tr>
             <td>PROFID</td>
             <td>-</td>
             <td colspan="2">증명 테이블은 현재 지원되지 않음</td>
        </tr>
        <tr>
             <td>PROOFOWNERID</td>
             <td>FK</td>
             <td>USERS_CURRENT</td>
             <td>사용자 ID</td>
        </tr>
        <tr>
             <td>PROOFSTAGID</td>
             <td>FK</td>
             <td>-</td>
             <td colspan="2">증명 단계 테이블은 현재 지원되지 않음</td>
        </tr>
        <tr>
             <td>SYSID</td>
             <td>-</td>
             <td colspan="2">관계가 아닙니다. 내부 응용 프로그램 용도로 사용됩니다.</td>
        </tr>
    </tbody>
</table>

### 환율

<table>
    <thead>
        <tr>
            <th>Workfront 엔티티 이름</th>
            <th>인터페이스 참조</th>
            <th>API 참조</th>
            <th>API 레이블</th>
            <th>데이터 레이크 보기</th>
        </tr>
      </thead>
      <tbody>
        <tr>
            <td>환율</td>
            <td>환율</td>
            <td>EXRATE</td>
            <td>환율</td>
            <td>EXCHANGERATES_CURRENT<br>EXCHANGERATES_DAILY_HISTORY<br>EXCHANGERATES_EVENT</td>
        </tr>
      </tbody>
</table>
<table>
    <thead>
        <tr>
            <th>기본/외래 키</th>
            <th>유형</th>
            <th>관련 테이블</th>
            <th>관련 필드</th>
        </tr>
    </thead>
    <tbody>
        <tr>
             <td>EXCHANGERATEID</td>
             <td>PK</td>
             <td>-</td>
             <td>-</td>
        </tr>
        <tr>
             <td>PROJECTID</td>
             <td>FK</td>
             <td>PROJECTS_CURRENT</td>
             <td>PROJECTID</td>
        </tr>
        <tr>
             <td>SYSID</td>
             <td>-</td>
             <td colspan="2">관계가 아닙니다. 내부 응용 프로그램 용도로 사용됩니다.</td>
        </tr>
        <tr>
             <td>TEMPLATEID</td>
             <td>FK</td>
             <td>TEMPLATES_CURRENT</td>
             <td>TEMPLATEID</td>
        </tr>
    </tbody>
</table>

### 경비

<table>
    <thead>
        <tr>
            <th>Workfront 엔티티 이름</th>
            <th>인터페이스 참조</th>
            <th>API 참조</th>
            <th>API 레이블</th>
            <th>데이터 레이크 보기</th>
        </tr>
      </thead>
      <tbody>
        <tr>
            <td>경비</td>
            <td>경비</td>
            <td>확장</td>
            <td>경비</td>
            <td>EXPENSES_CURRENT<br>EXPENSES_DAILY_HISTORY<br>EXPENSES_EVENT</td>
        </tr>
      </tbody>
</table>
<table>
    <thead>
        <tr>
            <th>기본/외래 키</th>
            <th>유형</th>
            <th>관련 테이블</th>
            <th>관련 필드</th>
        </tr>
    </thead>
    <tbody>
        <tr>
             <td>빌링레코디드</td>
             <td>FK</td>
             <td>BILLINGRECORDS_CURRENT</td>
             <td>빌링레코디드</td>
        </tr>
        <tr>
             <td>범주 ID</td>
             <td>FK</td>
             <td>CATEGORS_CURRENT</td>
             <td>범주 ID</td>
        </tr>
        <tr>
             <td>ENTEREDBYID</td>
             <td>FK</td>
             <td>USERS_CURRENT</td>
             <td>사용자 ID</td>
        </tr>
        <tr>
             <td>EXCHANGERATEID</td>
             <td>FK</td>
             <td>EXCHANGE_CURRENT</td>
             <td>EXCHANGERATEID</td>
        </tr>
        <tr>
             <td>경비 ID</td>
             <td>PK</td>
             <td>-</td>
             <td>-</td>
        </tr>
        <tr>
             <td>EXPENSETYPEID</td>
             <td>FK</td>
             <td>EXPENSETYPES_CURRENT</td>
             <td>EXPENSETYPEID</td>
        </tr>
        <tr>
             <td>LASTUPDATEDBYID</td>
             <td>FK</td>
             <td>USERS_CURRENT</td>
             <td>사용자 ID</td>
        </tr>
        <tr>
             <td>OBJID</td>
             <td>FK</td>
             <td>변수, OBJCODE 기반</td>
             <td>OBJCODE 필드에서 식별된 객체의 기본 키/ID</td>
        </tr>
        <tr>
             <td>PROJECTID</td>
             <td>FK</td>
             <td>PROJECTS_CURRENT</td>
             <td>PROJECTID</td>
        </tr>
        <tr>
             <td>SYSID</td>
             <td>-</td>
             <td colspan="2">관계가 아닙니다. 내부 응용 프로그램 용도로 사용됩니다.</td>
        </tr>
        <tr>
             <td>TASKID</td>
             <td>FK</td>
             <td>TASKS_CURRENT</td>
             <td>TASKID</td>
        </tr>
        <tr>
             <td>TEMPLATEID</td>
             <td>FK</td>
             <td>TEMPLATES_CURRENT</td>
             <td>TEMPLATEID</td>
        </tr>
        <tr>
             <td>TEMPLATETASKID</td>
             <td>FK</td>
             <td>TEMPLATETASKS_CURRENT</td>
             <td>TEMPLATETASKID</td>
        </tr>
        <tr>
             <td>TOPOBJID</td>
             <td>FK</td>
             <td>변수, TOPBJCODE 기반</td>
             <td>TOPBJCODE 필드에서 식별된 객체의 기본 키/ID</td>
        </tr>
    </tbody>
</table>

### 경비 유형

<table>
    <thead>
        <tr>
            <th>Workfront 엔티티 이름</th>
            <th>인터페이스 참조</th>
            <th>API 참조</th>
            <th>API 레이블</th>
            <th>데이터 레이크 보기</th>
        </tr>
      </thead>
      <tbody>
        <tr>
            <td>경비 유형</td>
            <td>경비 유형</td>
            <td>EXPTYP</td>
            <td>경비 유형</td>
            <td>EXPENSETYPES_CURRENT<br>EXPENSETYPES_DAILY_HISTORY<br>EXPENSETYPES_EVENT</td>
        </tr>
      </tbody>
</table>
<table>
    <thead>
        <tr>
            <th>기본/외래 키</th>
            <th>유형</th>
            <th>관련 테이블</th>
            <th>관련 필드</th>
        </tr>
    </thead>
    <tbody>
        <tr>
             <td>APPGLOBALID</td>
             <td>-</td>
             <td colspan="2">관계가 아닙니다. 내부 응용 프로그램 용도로 사용됩니다.</td>
        </tr>
        <tr>
             <td>EXPENSETYPEID</td>
             <td>PK</td>
             <td>-</td>
             <td>-</td>
        </tr>
        <tr>
             <td>OBJID</td>
             <td>FK</td>
             <td>변수, OBJCODE 기반</td>
             <td>OBJCODE 필드에서 식별된 객체의 기본 키/ID</td>
        </tr>
        <tr>
             <td>SYSID</td>
             <td>-</td>
             <td colspan="2">관계가 아닙니다. 내부 응용 프로그램 용도로 사용됩니다.</td>
        </tr>
    </tbody>
</table>

### 그룹

<table>
    <thead>
        <tr>
            <th>Workfront 엔티티 이름</th>
            <th>인터페이스 참조</th>
            <th>API 참조</th>
            <th>API 레이블</th>
            <th>데이터 레이크 보기</th>
        </tr>
      </thead>
      <tbody>
        <tr>
            <td>그룹</td>
            <td>그룹</td>
            <td>그룹</td>
            <td>그룹</td>
            <td>GROUPS_CURRENT<br>GROUPS_DAILY_HISTORY<br>GROUPS_EVENT</td>
        </tr>
      </tbody>
</table>
<table>
    <thead>
        <tr>
            <th>기본/외래 키</th>
            <th>유형</th>
            <th>관련 테이블</th>
            <th>관련 필드</th>
        </tr>
    </thead>
    <tbody>
        <tr>
             <td>BUSINESSLEADERID</td>
             <td>FK</td>
             <td>USERS_CURRENT</td>
             <td>사용자 ID</td>
        </tr>
        <tr>
             <td>범주 ID</td>
             <td>FK</td>
             <td>CATEGORS_CURRENT</td>
             <td>범주 ID</td>
        </tr>
        <tr>
             <td>ENTEREDBYID</td>
             <td>FK</td>
             <td>USERS_CURRENT</td>
             <td>사용자 ID</td>
        </tr>
        <tr>
             <td>GROUPID</td>
             <td>PK</td>
             <td>-</td>
             <td>-</td>
        </tr>
        <tr>
             <td>LAYOUTTEMPLATEID</td>
             <td>-</td>
             <td colspan="2">관계가 아닙니다. 내부 응용 프로그램 용도로 사용됩니다.</td>
        </tr>
        <tr>
             <td>괄호 ID</td>
             <td>FK</td>
             <td>GROUPS_CURRENT</td>
             <td>GROUPID</td>
        </tr>
        <tr>
             <td>ROOTID</td>
             <td>FK</td>
             <td>GROUPS_CURRENT</td>
             <td>GROUPID</td>
        </tr>
        <tr>
             <td>SYSID</td>
             <td>-</td>
             <td colspan="2">관계가 아닙니다. 내부 응용 프로그램 용도로 사용됩니다.</td>
        </tr>
        <tr>
             <td>UITEMPLATEID</td>
             <td>FK</td>
             <td>UITEMPLATES_CURRENT</td>
             <td>UITEMPLATEID</td>
        </tr>
    </tbody>
</table>

### 시간

<table>
    <thead>
        <tr>
            <th>Workfront 엔티티 이름</th>
            <th>인터페이스 참조</th>
            <th>API 참조</th>
            <th>API 레이블</th>
            <th>데이터 레이크 보기</th>
        </tr>
      </thead>
      <tbody>
        <tr>
            <td>시간</td>
            <td>시간</td>
            <td>시간</td>
            <td>시간</td>
            <td>HOURS_CURRENT<br>HOURS_DAILY_HISTORY<br>HOURS_EVENT</td>
        </tr>
      </tbody>
</table>
<table>
    <thead>
        <tr>
            <th>기본/외래 키</th>
            <th>유형</th>
            <th>관련 테이블</th>
            <th>관련 필드</th>
        </tr>
    </thead>
    <tbody>
        <tr>
             <td>APPROVEDBYID</td>
             <td>FK</td>
             <td>USERS_CURRENT</td>
             <td>사용자 ID</td>
        </tr>
        <tr>
             <td>빌링레코디드</td>
             <td>FK</td>
             <td>BILLINGRECORDS_CURRENT</td>
             <td>빌링레코디드</td>
        </tr>
        <tr>
             <td>범주 ID</td>
             <td>FK</td>
             <td>CATEGORS_CURRENT</td>
             <td>범주 ID</td>
        </tr>
        <tr>
             <td>분류자</td>
             <td>FK</td>
             <td>CLASSIFIER_CURRENT</td>
             <td>분류자</td>
        </tr>
        <tr>
             <td>더피</td>
             <td>-</td>
             <td colspan="2">관계가 아닙니다. 내부 응용 프로그램 용도로 사용됩니다.</td>
        </tr>
        <tr>
             <td>EXCHANGERATEID</td>
             <td>FK</td>
             <td>EXCHANGE_CURRENT</td>
             <td>EXCHANGERATEID</td>
        </tr>
        <tr>
             <td>EXTERNALTIMESHEETID</td>
             <td>-</td>
             <td colspan="2">Workfront 관계가 아닙니다. 외부 시스템과의 통합에 사용됩니다.
자가</td>
        </tr>
        <tr>
             <td>야우리</td>
             <td>PK</td>
             <td>-</td>
             <td>-</td>
        </tr>
        <tr>
             <td>HOURTYPEID</td>
             <td>FK</td>
             <td>HOURTYPES_CURRENT</td>
             <td>HOURTYPEID</td>
        </tr>
        <tr>
             <td>LASTUPDATEDBYID</td>
             <td>FK</td>
             <td>USERS_CURRENT</td>
             <td>사용자 ID</td>
        </tr>
        <tr>
             <td>OPTASKID</td>
             <td>FK</td>
             <td>OPTASKS_CURRENT</td>
             <td>OPTASKID</td>
        </tr>
        <tr>
             <td>소유자 ID</td>
             <td>FK</td>
             <td>USERS_CURRENT</td>
             <td>사용자 ID</td>
        </tr>
        <tr>
             <td>PROJECTID</td>
             <td>FK</td>
             <td>PROJECTS_CURRENT</td>
             <td>PROJECTID</td>
        </tr>
        <tr>
             <td>PROJECTTOVERHEADID</td>
             <td>-</td>
             <td colspan="2">관계가 아닙니다. 내부 응용 프로그램 용도로 사용됩니다.</td>
        </tr>
        <tr>
             <td>장미모양-</td>
             <td>FK</td>
             <td>ROLES_CURRENT</td>
             <td>장미모양-</td>
        </tr>
        <tr>
             <td>SYSID</td>
             <td>-</td>
             <td colspan="2">관계가 아닙니다. 내부 응용 프로그램 용도로 사용됩니다.</td>
        </tr>
        <tr>
             <td>TASKID</td>
             <td>FK</td>
             <td>TASKS_CURRENT</td>
             <td>TASKID</td>
        </tr>
        <tr>
             <td>TIMESHEETID</td>
             <td>FK</td>
             <td>TIMESHEETS_CURRENT</td>
             <td>TIMESHEETID</td>
        </tr>
    </tbody>
</table>

### 시간 유형

<table>
    <thead>
        <tr>
            <th>Workfront 엔티티 이름</th>
            <th>인터페이스 참조</th>
            <th>API 참조</th>
            <th>API 레이블</th>
            <th>데이터 레이크 보기</th>
        </tr>
      </thead>
      <tbody>
        <tr>
            <td>시간 유형</td>
            <td>시간 유형</td>
            <td>시간</td>
            <td>시간 유형</td>
            <td>HOURTYPES_CURRENT<br>HOURTYPES_DAILY_HISTORY<br>HOURTYPES_EVENT</td>
        </tr>
      </tbody>
</table>
<table>
    <thead>
        <tr>
            <th>기본/외래 키</th>
            <th>유형</th>
            <th>관련 테이블</th>
            <th>관련 필드</th>
        </tr>
    </thead>
    <tbody>
        <tr>
             <td>APPGLOBALID</td>
             <td>-</td>
             <td colspan="2">관계가 아닙니다. 내부 응용 프로그램 용도로 사용됩니다.</td>
        </tr>
        <tr>
             <td>HOURTYPEID</td>
             <td>PK</td>
             <td>-</td>
             <td>-</td>
        </tr>
        <tr>
             <td>OBJID</td>
             <td>FK</td>
             <td>변수, OBJCODE 기반</td>
             <td>OBJCODE 필드에서 식별된 객체의 기본 키/ID</td>
        </tr>
        <tr>
             <td>SYSID</td>
             <td>-</td>
             <td colspan="2">관계가 아닙니다. 내부 응용 프로그램 용도로 사용됩니다.</td>
        </tr>
    </tbody>
</table>

### 반복

<table>
    <thead>
        <tr>
            <th>Workfront 엔티티 이름</th>
            <th>인터페이스 참조</th>
            <th>API 참조</th>
            <th>API 레이블</th>
            <th>데이터 레이크 보기</th>
        </tr>
      </thead>
      <tbody>
        <tr>
            <td>반복</td>
            <td>반복</td>
            <td>ITRN</td>
            <td>반복</td>
            <td>ITERATIONS_CURRENT<br>ITERATIONS_DAILY_HISTORY<br>ITERATIONS_EVENT</td>
        </tr>
      </tbody>
</table>
<table>
    <thead>
        <tr>
            <th>기본/외래 키</th>
            <th>유형</th>
            <th>관련 테이블</th>
            <th>관련 필드</th>
        </tr>
    </thead>
    <tbody>
        <tr>
             <td>범주 ID</td>
             <td>FK</td>
             <td>CATEGORS_CURRENT</td>
             <td>범주 ID</td>
        </tr>
        <tr>
             <td>ENTEREDBYID</td>
             <td>FK</td>
             <td>USERS_CURRENT</td>
             <td>사용자 ID</td>
        </tr>
        <tr>
             <td>ITERATIONID</td>
             <td>PK</td>
             <td>-</td>
             <td>-</td>
        </tr>
        <tr>
             <td>LASTUPDATEDBYID</td>
             <td>FK</td>
             <td>USERS_CURRENT</td>
             <td>사용자 ID</td>
        </tr>
        <tr>
             <td>소유자 ID</td>
             <td>FK</td>
             <td>USERS_CURRENT</td>
             <td>사용자 ID</td>
        </tr>
        <tr>
             <td>SYSID</td>
             <td>-</td>
             <td colspan="2">관계가 아닙니다. 내부 응용 프로그램 용도로 사용됩니다.</td>
        </tr>
        <tr>
             <td>티미드</td>
             <td>FK</td>
             <td>TEAMS_CURRENT</td>
             <td>티미드</td>
        </tr>
    </tbody>
</table>

### 저널 항목

<table>
    <thead>
        <tr>
            <th>Workfront 엔티티 이름</th>
            <th>인터페이스 참조</th>
            <th>API 참조</th>
            <th>API 레이블</th>
            <th>데이터 레이크 보기</th>
        </tr>
      </thead>
      <tbody>
        <tr>
            <td>저널 항목</td>
            <td>저널 항목</td>
            <td>JRNLE</td>
            <td>저널 항목</td>
            <td>JOURNALENTRIES_CURRENT<br>JOURNALENTRIES_DAILY_HISTORY<br>JOURNALENTRIES_EVENT</td>
        </tr>
      </tbody>
</table>
<table>
    <thead>
        <tr>
            <th>기본/외래 키</th>
            <th>유형</th>
            <th>관련 테이블</th>
            <th>관련 필드</th>
        </tr>
    </thead>
    <tbody>
        <tr>
             <td>APPROVERSTATUSID</td>
             <td>FK</td>
             <td>APPROVERSTATUSES_CURRENT</td>
             <td>APPROVERSTATUSID</td>
        </tr>
        <tr>
             <td>ASSIGNMENTID</td>
             <td>FK</td>
             <td>ASSIGNMENTS_CURRENT</td>
             <td>ASSIGNMENTID</td>
        </tr>
        <tr>
             <td>AUDITRECORDID</td>
             <td>-</td>
             <td colspan="2">감사 레코드 테이블이 현재 지원되지 않음</td>
        </tr>
        <tr>
             <td>BASELINEID</td>
             <td>FK</td>
             <td>BASELINES_CURRENT</td>
             <td>BASELINEID</td>
        </tr>
        <tr>
             <td>빌링레코디드</td>
             <td>FK</td>
             <td>BILLINGRECORDS_CURRENT</td>
             <td>빌링레코디드</td>
        </tr>
        <tr>
             <td>COMPANYID</td>
             <td>FK</td>
             <td>COMPANIES_CURRENT</td>
             <td>COMPANYID</td>
        </tr>
        <tr>
             <td>DOCUMENTID</td>
             <td>FK</td>
             <td>DOCUMENTS_CURRENT</td>
             <td>DOCUMENTID</td>
        </tr>
        <tr>
             <td>DOCUMENTSHAREID</td>
             <td>-</td>
             <td colspan="2">문서 공유 테이블은 현재 지원되지 않습니다.</td>
        </tr>
        <tr>
             <td>EDITEDBYID</td>
             <td>FK</td>
             <td>USERS_CURRENT</td>
             <td>사용자 ID</td>
        </tr>
        <tr>
             <td>경비 ID</td>
             <td>FK</td>
             <td>EXPENSES_CURRENT</td>
             <td>경비 ID</td>
        </tr>
        <tr>
             <td>야우리</td>
             <td>FK</td>
             <td>HOURS_CURRENT</td>
             <td>야우리</td>
        </tr>
        <tr>
             <td>INITIATIVEID</td>
             <td>-</td>
             <td colspan="2">이니셔티브 테이블은 현재 지원되지 않습니다.</td>
        </tr>
        <tr>
             <td>JOURNALENTRIESID</td>
             <td>PK</td>
             <td>-</td>
             <td>-</td>
        </tr>
        <tr>
             <td>OBJID</td>
             <td>FK</td>
             <td>변수, OBJCODE 기반</td>
             <td>OBJCODE 필드에서 식별된 객체의 기본 키/ID</td>
        </tr>
        <tr>
             <td>OPTASKID</td>
             <td>FK</td>
             <td>OPTASKS_CURRENT</td>
             <td>OPTASKID</td>
        </tr>
        <tr>
             <td>포트폴리오</td>
             <td>FK</td>
             <td>포트폴리오_현재</td>
             <td>포트폴리오</td>
        </tr>
        <tr>
             <td>PROGRAMID</td>
             <td>FK</td>
             <td>PROGRAMS_CURRENT</td>
             <td>PROGRAMID</td>
        </tr>
        <tr>
             <td>PROJECTID</td>
             <td>FK</td>
             <td>PROJECTS_CURRENT</td>
             <td>PROJECTID</td>
        </tr>
        <tr>
             <td>SUBOBJID</td>
             <td>FK</td>
             <td>변수, SUBOBJCODE 기반</td>
             <td>SUBOBJCODE 필드에서 식별된 객체의 기본 키/ID</td>
        </tr>
        <tr>
             <td>구독 ID</td>
             <td>-</td>
             <td colspan="2">관계가 아닙니다. 내부 응용 프로그램 용도로 사용됩니다.</td>
        </tr>
        <tr>
             <td>SYSID</td>
             <td>-</td>
             <td colspan="2">관계가 아닙니다. 내부 응용 프로그램 용도로 사용됩니다.</td>
        </tr>
        <tr>
             <td>TASKID</td>
             <td>FK</td>
             <td>TASKS_CURRENT</td>
             <td>TASKID</td>
        </tr>
        <tr>
             <td>TEMPLATEID</td>
             <td>FK</td>
             <td>TEMPLATES_CURRENT</td>
             <td>TEMPLATEID</td>
        </tr>
        <tr>
             <td>TIMESHEETID</td>
             <td>FK</td>
             <td>TIMESHEETS_CURRENT</td>
             <td>TIMESHEETID</td>
        </tr>
        <tr>
             <td>TOPOBJID</td>
             <td>FK</td>
             <td>변수, TOPOBJCODE 기반</td>
             <td>TOPOBJCODE 필드에서 식별된 객체의 기본 키/ID</td>
        </tr>
        <tr>
             <td>사용자 ID</td>
             <td>FK</td>
             <td>USERS_CURRENT</td>
             <td>사용자 ID</td>
        </tr>
    </tbody>
</table>

### 연결된 폴더

<table>
    <thead>
        <tr>
            <th>Workfront 엔티티 이름</th>
            <th>인터페이스 참조</th>
            <th>API 참조</th>
            <th>API 레이블</th>
            <th>데이터 레이크 보기</th>
        </tr>
      </thead>
      <tbody>
        <tr>
            <td>연결된 폴더</td>
            <td>연결된 폴더</td>
            <td>LNKFDR</td>
            <td>LinkedFolder</td>
            <td>LINKEDFOLDERS_CURRENT<br>LINKEDFOLDERS_DAILY_HISTORY<br>LINKEDFOLDERS_EVENT</td>
        </tr>
      </tbody>
</table>
<table>
    <thead>
        <tr>
            <th>기본/외래 키</th>
            <th>유형</th>
            <th>관련 테이블</th>
            <th>관련 필드</th>
        </tr>
    </thead>
    <tbody>
        <tr>
             <td>DOCUMENTPROVIDERID</td>
             <td>FK</td>
             <td>DOCPROVIDERS_CURRENT</td>
             <td>DOCUMENTPROVIDERID</td>
        </tr>
        <tr>
             <td>EXTERNALSTORAGEID</td>
             <td>-</td>
             <td colspan="2">외부 스토리지 시스템의 외부 ID</td>
        </tr>
        <tr>
             <td>폴더 ID</td>
             <td>FK</td>
             <td>DOCFOLDERS_CURRENT</td>
             <td>폴더 ID</td>
        </tr>
        <tr>
             <td>LINKEDBYID</td>
             <td>FK</td>
             <td>USERS_CURRENT</td>
             <td>사용자 ID</td>
        </tr>
        <tr>
             <td>LINKEDFOLDERID</td>
             <td>PK</td>
             <td>-</td>
             <td>-</td>
        </tr>
        <tr>
             <td>SYSID</td>
             <td>-</td>
             <td colspan="2">관계가 아닙니다. 내부 응용 프로그램 용도로 사용됩니다.</td>
        </tr>
    </tbody>
</table>

### 마일스톤

<table>
    <thead>
        <tr>
            <th>Workfront 엔티티 이름</th>
            <th>인터페이스 참조</th>
            <th>API 참조</th>
            <th>API 레이블</th>
            <th>데이터 레이크 보기</th>
        </tr>
      </thead>
      <tbody>
        <tr>
            <td>마일스톤</td>
            <td>마일스톤</td>
            <td>마일</td>
            <td>마일스톤</td>
            <td>MILESTONES_CURRENT<br>MILESTONES_DAILY_HISTORY<br>MILESTONES_EVENT</td>
        </tr>
      </tbody>
</table>
<table>
    <thead>
        <tr>
            <th>기본/외래 키</th>
            <th>유형</th>
            <th>관련 테이블</th>
            <th>관련 필드</th>
        </tr>
    </thead>
    <tbody>
        <tr>
             <td>LASTUPDATEDBYID</td>
             <td>FK</td>
             <td>USERS_CURRENT</td>
             <td>사용자 ID</td>
        </tr>
        <tr>
             <td>마일스톤ID</td>
             <td>PK</td>
             <td>-</td>
             <td>-</td>
        </tr>
        <tr>
             <td>마일스톤 경로 ID</td>
             <td>FK</td>
             <td>MILESTONEPATHS_CURRENT</td>
             <td>마일스톤 경로 ID</td>
        </tr>
        <tr>
             <td>SYSID</td>
             <td>-</td>
             <td colspan="2">관계가 아닙니다. 내부 응용 프로그램 용도로 사용됩니다.</td>
        </tr>
    </tbody>
</table>

### 마일스톤 경로

<table>
    <thead>
        <tr>
            <th>Workfront 엔티티 이름</th>
            <th>인터페이스 참조</th>
            <th>API 참조</th>
            <th>API 레이블</th>
            <th>데이터 레이크 보기</th>
        </tr>
      </thead>
      <tbody>
        <tr>
            <td>마일스톤 경로</td>
            <td>마일스톤 경로</td>
            <td>MPATH</td>
            <td>마일스톤 경로</td>
            <td>MILESTONEPATHS_CURRENT<br>MILESTONEPATHS_DAILY_HISTORY<br>MILESTONEPATHS_EVENT</td>
        </tr>
      </tbody>
</table>
<table>
    <thead>
        <tr>
            <th>기본/외래 키</th>
            <th>유형</th>
            <th>관련 테이블</th>
            <th>관련 필드</th>
        </tr>
    </thead>
    <tbody>
        <tr>
             <td>ENTEREDBYID</td>
             <td>FK</td>
             <td>USERS_CURRENT</td>
             <td>사용자 ID</td>
        </tr>
        <tr>
             <td>LASTUPDATEDBYID</td>
             <td>FK</td>
             <td>USERS_CURRENT</td>
             <td>사용자 ID</td>
        </tr>
        <tr>
             <td>마일스톤 경로 ID</td>
             <td>PK</td>
             <td>-</td>
             <td>-</td>
        </tr>
        <tr>
             <td>SYSID</td>
             <td>-</td>
             <td colspan="2">관계가 아닙니다. 내부 응용 프로그램 용도로 사용됩니다.</td>
        </tr>
    </tbody>
</table>

### 비노동 리소스

<table>
    <thead>
        <tr>
            <th>Workfront 엔티티 이름</th>
            <th>인터페이스 참조</th>
            <th>API 참조</th>
            <th>API 레이블</th>
            <th>데이터 레이크 보기</th>
        </tr>
      </thead>
      <tbody>
        <tr>
            <td>비노동 리소스</td>
            <td>비노동 리소스</td>
            <td>NLBR</td>
            <td>비노동 리소스</td>
            <td>NONLABORRESOURCES_CURRENT<br>NONLABORRESOURCES_DAILY_HISTORY<br>NONLABORRESOURCES_EVENT</td>
        </tr>
      </tbody>
</table>
<table>
    <thead>
        <tr>
            <th>기본/외래 키</th>
            <th>유형</th>
            <th>관련 테이블</th>
            <th>관련 필드</th>
        </tr>
    </thead>
    <tbody>
        <tr>
             <td>범주 ID</td>
             <td>FK</td>
             <td>CATEGORS_CURRENT</td>
             <td>범주 ID</td>
        </tr>
        <tr>
             <td>NONLABORRESOURCEID</td>
             <td>PK</td>
             <td>-</td>
             <td>-</td>
        </tr>
        <tr>
             <td>ENTEREDBYID</td>
             <td>FK</td>
             <td>USERS_CURRENT</td>
             <td>사용자 ID</td>
        </tr>
        <tr>
             <td>HOMEGROUPID</td>
             <td>FK</td>
             <td>GROUPS_CURRENT</td>
             <td>GROUPID</td>
        </tr>
        <tr>
             <td>LASTUPDATEDBYID</td>
             <td>FK</td>
             <td>USERS_CURRENT</td>
             <td>사용자 ID</td>
        </tr>
        <tr>
             <td>NONLABORRESOURCECATEGORYID</td>
             <td>FK</td>
             <td>NLBRCATEGORIES_CURRENT</td>
             <td>NLBRCATEGORYID</td>
        </tr>
        <tr>
             <td>SYSID</td>
             <td>-</td>
             <td colspan="2">관계가 아닙니다. 내부 응용 프로그램 용도로 사용됩니다.</td>
        </tr>
    </tbody>
</table>

### 비노동 리소스 범주

<table>
    <thead>
        <tr>
            <th>Workfront 엔티티 이름</th>
            <th>인터페이스 참조</th>
            <th>API 참조</th>
            <th>API 레이블</th>
            <th>데이터 레이크 보기</th>
        </tr>
      </thead>
      <tbody>
        <tr>
            <td>비노동 리소스 범주</td>
            <td>비노동 리소스 범주</td>
            <td>NLBRCY</td>
            <td>비노동 리소스 범주</td>
            <td>NLBRCATEGORIES_CURRENT<br>NLBRCATEGORIES_DAILY_HISTORY<br>NLBRCATEGORIES_EVENT</td>
        </tr>
      </tbody>
</table>
<table>
    <thead>
        <tr>
            <th>기본/외래 키</th>
            <th>유형</th>
            <th>관련 테이블</th>
            <th>관련 필드</th>
        </tr>
    </thead>
    <tbody>
        <tr>
             <td>범주 ID</td>
             <td>FK</td>
             <td>CATEGORS_CURRENT</td>
             <td>범주 ID</td>
        </tr>
        <tr>
             <td>ENTEREDBYID</td>
             <td>FK</td>
             <td>USERS_CURRENT</td>
             <td>사용자 ID</td>
        </tr>
        <tr>
             <td>LASTUPDATEDBYID</td>
             <td>FK</td>
             <td>USERS_CURRENT</td>
             <td>사용자 ID</td>
        </tr>
        <tr>
             <td>NLBRCATEGORYID</td>
             <td>PK</td>
             <td>-</td>
             <td>-</td>
        </tr>
        <tr>
             <td>PRIVATERATECARDID</td>
             <td>FK</td>
             <td>RATECARD_CURRENT</td>
             <td>RATECARDID</td>
        </tr>
        <tr>
             <td>예약 ID</td>
             <td>FK</td>
             <td>SCHEDULES_CURRENT</td>
             <td>예약 ID</td>
        </tr>
        <tr>
             <td>SYSID</td>
             <td>-</td>
             <td colspan="2">관계가 아닙니다. 내부 응용 프로그램 용도로 사용됩니다.</td>
        </tr>
    </tbody>
</table>

### 비근무일

<table>
    <thead>
        <tr>
            <th>Workfront 엔티티 이름</th>
            <th>인터페이스 참조</th>
            <th>API 참조</th>
            <th>API 레이블</th>
            <th>데이터 레이크 보기</th>
        </tr>
      </thead>
      <tbody>
        <tr>
            <td>비근무일</td>
            <td>일정 예외</td>
            <td>NONWKD</td>
            <td>비근무일</td>
            <td>NONWORKDAYS_CURRENT<br>NONWORKDAYS_DAILY_HISTORY<br>NONWORKDAYS_EVENT</td>
        </tr>
      </tbody>
</table>
<table>
    <thead>
        <tr>
            <th>기본/외래 키</th>
            <th>유형</th>
            <th>관련 테이블</th>
            <th>관련 필드</th>
        </tr>
    </thead>
    <tbody>
        <tr>
             <td>NONWORKDAYID</td>
             <td>PK</td>
             <td>-</td>
             <td>-</td>
        </tr>
        <tr>
             <td>OBJID</td>
             <td>FK</td>
             <td>변수, OBJCODE 기반</td>
             <td>OBJCODE 필드에서 식별된 객체의 기본 키/ID</td>
        </tr>
        <tr>
             <td>예약 ID</td>
             <td>FK</td>
             <td>SCHEDULES_CURRENT</td>
             <td>예약 ID</td>
        </tr>
        <tr>
             <td>SYSID</td>
             <td>-</td>
             <td colspan="2">관계가 아닙니다. 내부 응용 프로그램 용도로 사용됩니다.</td>
        </tr>
        <tr>
             <td>사용자 ID</td>
             <td>FK</td>
             <td>USERS_CURRENT</td>
             <td>사용자 ID</td>
        </tr>
    </tbody>
</table>

### 참고

<table>
    <thead>
        <tr>
            <th>Workfront 엔티티 이름</th>
            <th>인터페이스 참조</th>
            <th>API 참조</th>
            <th>API 레이블</th>
            <th>데이터 레이크 보기</th>
        </tr>
      </thead>
      <tbody>
        <tr>
            <td>참고</td>
            <td>참고</td>
            <td>메모</td>
            <td>참고</td>
            <td>NOTES_CURRENT<br>NOTES_DAILY_HISTORY<br>NOTES_EVENT</td>
        </tr>
      </tbody>
</table>
<table>
    <thead>
        <tr>
            <th>기본/외래 키</th>
            <th>유형</th>
            <th>관련 테이블</th>
            <th>관련 필드</th>
        </tr>
    </thead>
    <tbody>
        <tr>
             <td>ATTACHDOCUMENTID</td>
             <td>FK</td>
             <td>DOCUMENTS_CURRENT</td>
             <td>DOCUMENTID</td>
        </tr>
        <tr>
             <td>ATTACHOBJID</td>
             <td>FK</td>
             <td>변수, ATTACHOBJCODE 기반</td>
             <td>OBJCODE ATTACHOBJCODE에서 식별된 객체의 기본 키/ID</td>
        </tr>
        <tr>
             <td>ATTACHOPTASKID</td>
             <td>FK</td>
             <td>OPTASKS_CURRENT</td>
             <td>OPTASKID</td>
        </tr>
        <tr>
             <td>ATTACHWORKID</td>
             <td>FK</td>
             <td>WORKITEMS_CURRENT</td>
             <td>WORKITEMID</td>
        </tr>
        <tr>
             <td>ATTACHWORKUSERID</td>
             <td>FK</td>
             <td>USERS_CURRENT</td>
             <td>사용자 ID</td>
        </tr>
        <tr>
             <td>AUDITRECORDID</td>
             <td>-</td>
             <td colspan="2">감사 레코드 테이블이 현재 지원되지 않음</td>
        </tr>
        <tr>
             <td>COMPANYID</td>
             <td>FK</td>
             <td>COMPANIES_CURRENT</td>
             <td>COMPANYID</td>
        </tr>
        <tr>
             <td>DOCUMENTID</td>
             <td>FK</td>
             <td>DOCUMENTS_CURRENT</td>
             <td>DOCUMENTID</td>
        </tr>
        <tr>
             <td>EXTERNALSERVICEID</td>
             <td>-</td>
             <td colspan="2">Workfront 관계가 아닙니다. 외부 시스템과의 통합에 사용됩니다.</td>
        </tr>
        <tr>
             <td>ITERATIONID</td>
             <td>FK</td>
             <td>ITERATIONS_CURRENT</td>
             <td>ITERATIONID</td>
        </tr>
        <tr>
             <td>NOTEID</td>
             <td>PK</td>
             <td>-</td>
             <td>-</td>
        </tr>
        <tr>
             <td>OBJID</td>
             <td>FK</td>
             <td>변수, NOTEOBJCODE 기반</td>
             <td>NOTEOBJCODE 필드에서 식별된 객체의 기본 키/ID</td>
        </tr>
        <tr>
             <td>OPTASKID</td>
             <td>FK</td>
             <td>OPTASKS_CURRENT</td>
             <td>OPTASKID</td>
        </tr>
        <tr>
             <td>소유자 ID</td>
             <td>FK</td>
             <td>USERS_CURRENT</td>
             <td>사용자 ID</td>
        </tr>
        <tr>
             <td>비실어샘체</td>
             <td>-</td>
             <td colspan="2">보증 테이블은 현재 지원되지 않습니다.</td>
        </tr>
        <tr>
             <td>PARENTJOURNALENTRYID</td>
             <td>FK</td>
             <td>JOURNALENTRIES_CURRENT</td>
             <td>JOURNALENTRYID</td>
        </tr>
        <tr>
             <td>PARENTNOTEID</td>
             <td>FK</td>
             <td>NOTES_CURRENT</td>
             <td>NOTEID</td>
        </tr>
        <tr>
             <td>포트폴리오</td>
             <td>FK</td>
             <td>포트폴리오_현재</td>
             <td>포트폴리오</td>
        </tr>
        <tr>
             <td>PROGRAMID</td>
             <td>FK</td>
             <td>PROGRAMS_CURRENT</td>
             <td>PROGRAMID</td>
        </tr>
        <tr>
             <td>PROJECTID</td>
             <td>FK</td>
             <td>PROJECTS_CURRENT</td>
             <td>PROJECTID</td>
        </tr>
        <tr>
             <td>PROFACATIONID</td>
             <td>-</td>
             <td colspan="2">증명 작업 테이블은 현재 지원되지 않음</td>
        </tr>
        <tr>
             <td>PROFID</td>
             <td>-</td>
             <td colspan="2">증명 테이블은 현재 지원되지 않음</td>
        </tr>
        <tr>
             <td>RICHTEXTNOTEID</td>
             <td>FK</td>
             <td>RESERVEDTEXTNOTES_CURRENT</td>
             <td>RICHTEXTNOTEID</td>
        </tr>
        <tr>
             <td>SYSID</td>
             <td>-</td>
             <td colspan="2">관계가 아닙니다. 내부 응용 프로그램 용도로 사용됩니다.</td>
        </tr>
        <tr>
             <td>TASKID</td>
             <td>FK</td>
             <td>TASKS_CURRENT</td>
             <td>TASKID</td>
        </tr>
        <tr>
             <td>TEMPLATEID</td>
             <td>FK</td>
             <td>TEMPLATES_CURRENT</td>
             <td>TEMPLATEID</td>
        </tr>
        <tr>
             <td>TEMPLATETASKID</td>
             <td>FK</td>
             <td>TEMPLATETASKS_CURRENT</td>
             <td>TEMPLATETASKID</td>
        </tr>
        <tr>
             <td>스레디드</td>
             <td>FK</td>
             <td>NOTES_CURRENT</td>
             <td>NOTEID</td>
        </tr>
        <tr>
             <td>TIMESHEETID</td>
             <td>FK</td>
             <td>TIMESHEETS_CURRENT</td>
             <td>TIMESHEETID</td>
        </tr>
        <tr>
             <td>TOPOBJID</td>
             <td>FK</td>
             <td>변수, TOPOBJCODE 기반</td>
             <td>TOPOBJCODE 필드에서 식별된 객체의 기본 키/ID</td>
        </tr>
        <tr>
             <td>사용자 ID</td>
             <td>FK</td>
             <td>USERS_CURRENT</td>
             <td>사용자 ID</td>
        </tr>


    &lt;/tbody>
</table>

### 오브젝트 통합

<table>
    <thead>
        <tr>
            <th>Workfront 엔티티 이름</th>
            <th>인터페이스 참조</th>
            <th>API 참조</th>
            <th>API 레이블</th>
            <th>데이터 레이크 보기</th>
        </tr>
      </thead>
      <tbody>
        <tr>
            <td>오브젝트 통합</td>
            <td>오브젝트 통합</td>
            <td>오브젝트</td>
            <td>오브젝트 통합</td>
            <td>OBJECTINTEGRATION_CURRENT<br>OBJECTINTEGRATION_DAILY_HISTORY<br>OBJECTINTEGRATION_EVENT</td>
        </tr>
      </tbody>
</table>
<table>
    <thead>
        <tr>
            <th>기본/외래 키</th>
            <th>유형</th>
            <th>관련 테이블</th>
            <th>관련 필드</th>
        </tr>
    </thead>
    <tbody>
        <tr>
             <td>LINKEDOBJECTID</td>
             <td>FK</td>
             <td>변수, LINKEDOBJECTCODE 기반</td>
             <td>LINKEDOBJECTCODE 필드에서 식별된 객체의 기본 키/ID</td>
        </tr>
        <tr>
             <td>OBJECTINTEGRATIONID</td>
             <td>PK</td>
             <td>-</td>
             <td>-</td>
        </tr>
        <tr>
             <td>OBJID</td>
             <td>FK</td>
             <td>변수, OBJCODE 기반</td>
             <td>OBJCODE 필드에서 식별된 객체의 기본 키/ID</td>
        </tr>
        <tr>
             <td>SYSID</td>
             <td>-</td>
             <td colspan="2">관계가 아닙니다. 내부 응용 프로그램 용도로 사용됩니다.</td>
        </tr>

    &lt;/tbody>
</table>

### 오브젝트 범주

<table>
    <thead>
        <tr>
            <th>Workfront 엔티티 이름</th>
            <th>인터페이스 참조</th>
            <th>API 참조</th>
            <th>API 레이블</th>
            <th>데이터 레이크 보기</th>
        </tr>
      </thead>
      <tbody>
        <tr>
            <td>오브젝트 범주</td>
            <td>오브젝트 범주</td>
            <td>OBJCAT</td>
            <td>오브젝트 범주</td>
            <td>OBJECTSCATEGORIES_CURRENT<br>OBJECTSCATEGORIES_DAILY_HISTORY<br>OBJECTSCATEGORIES_EVENT</td>
        </tr>
      </tbody>
</table>
<table>
    <thead>
        <tr>
            <th>기본/외래 키</th>
            <th>유형</th>
            <th>관련 테이블</th>
            <th>관련 필드</th>
        </tr>
    </thead>
    <tbody>
        <tr>
             <td>범주 ID</td>
             <td>FK</td>
             <td>CATEGORS_CURRENT</td>
             <td>범주 ID</td>
        </tr>
        <tr>
             <td>OBJECTSCATEGORYID</td>
             <td>PK</td>
             <td>-</td>
             <td>-</td>
        </tr>
        <tr>
             <td>OBJID</td>
             <td>FK</td>
             <td>변수, OBJCODE 기반</td>
             <td>OBJCODE 필드에서 식별된 객체의 기본 키/ID</td>
        </tr>
        <tr>
             <td>SYSID</td>
             <td>-</td>
             <td colspan="2">관계가 아닙니다. 내부 응용 프로그램 용도로 사용됩니다.</td>
        </tr>
    </tbody>
</table>

### OpTask / 문제

<table>
    <thead>
        <tr>
            <th>Workfront 엔티티 이름</th>
            <th>인터페이스 참조</th>
            <th>API 참조</th>
            <th>API 레이블</th>
            <th>데이터 레이크 보기</th>
        </tr>
      </thead>
      <tbody>
        <tr>
            <td>OpTask</td>
            <td>문제, 요청</td>
            <td>OPTASK</td>
            <td>문제</td>
            <td>OPTASKS_CURRENT<br>OPTASKS_DAILY_HISTORY<br>OPTASKS_EVENT</td>
        </tr>
      </tbody>
</table>
<table>
    <thead>
        <tr>
            <th>기본/외래 키</th>
            <th>유형</th>
            <th>관련 테이블</th>
            <th>관련 필드</th>
        </tr>
    </thead>
    <tbody>
        <tr>
             <td>APPROVALPROCESSID</td>
             <td>FK</td>
             <td>APPROVALPROCESSES_CURRENT</td>
             <td>APPROVALPROCESSID</td>
        </tr>
        <tr>
             <td>ASSIGNEDTOID</td>
             <td>FK</td>
             <td>USERS_CURRENT</td>
             <td>사용자 ID</td>
        </tr>
        <tr>
             <td>범주 ID</td>
             <td>FK</td>
             <td>CATEGORS_CURRENT</td>
             <td>범주 ID</td>
        </tr>
        <tr>
             <td>CURRENTAPPROVALSTEPID</td>
             <td>FK</td>
             <td>APPROVALSTEPS_CURRENT</td>
             <td>승인스테피드</td>
        </tr>
        <tr>
             <td>ENTEREDBYID</td>
             <td>FK</td>
             <td>USERS_CURRENT</td>
             <td>사용자 ID</td>
        </tr>
        <tr>
             <td>EXCHANGERATEID</td>
             <td>FK</td>
             <td>EXCHANGE_CURRENT</td>
             <td>EXCHANGERATEID</td>
        </tr>
        <tr>
             <td>ITERATIONID</td>
             <td>FK</td>
             <td>ITERATIONS_CURRENT</td>
             <td>ITERATIONID</td>
        </tr>
        <tr>
             <td>칸반보드</td>
             <td>-</td>
             <td colspan="2">칸반 보드 테이블은 현재 지원되지 않습니다.</td>
        </tr>
        <tr>
             <td>LASTCONDITIONNOTEID</td>
             <td>FK</td>
             <td>NOTES_CURRENT</td>
             <td>NOTEID</td>
        </tr>
        <tr>
             <td>LASTNOTEID</td>
             <td>FK</td>
             <td>NOTES_CURRENT</td>
             <td>NOTEID</td>
        </tr>
        <tr>
             <td>LASTUPDATEDBYID</td>
             <td>FK</td>
             <td>USERS_CURRENT</td>
             <td>사용자 ID</td>
        </tr>
        <tr>
             <td>OPTASKID</td>
             <td>PK</td>
             <td>-</td>
             <td>-</td>
        </tr>
        <tr>
             <td>소유자 ID</td>
             <td>FK</td>
             <td>USERS_CURRENT</td>
             <td>사용자 ID</td>
        </tr>
        <tr>
             <td>PROJECTID</td>
             <td>FK</td>
             <td>PROJECTS_CURRENT</td>
             <td>PROJECTID</td>
        </tr>
        <tr>
             <td>QUEUEDEFID</td>
             <td>-</td>
             <td colspan="2">대기열 정의 테이블은 현재 지원되지 않습니다.</td>
        </tr>
        <tr>
             <td>QUEUETOPICID</td>
             <td>-</td>
             <td colspan="2">대기열 주제 테이블은 현재 지원되지 않습니다.</td>
        </tr>
        <tr>
             <td>RESOLVEOPTASKID</td>
             <td>FK</td>
             <td>OPTASKS_CURRENT</td>
             <td>OPTASKID</td>
        </tr>
        <tr>
             <td>RESOLVEPROJECTID</td>
             <td>FK</td>
             <td>PROJECTS_CURRENT</td>
             <td>PROJECTID</td>
        </tr>
        <tr>
             <td>RESOLVETASKID</td>
             <td>FK</td>
             <td>TASKS_CURRENT</td>
             <td>TASKID</td>
        </tr>
        <tr>
             <td>RESOLVINGOBJID</td>
             <td>FK</td>
             <td>변수, RESOLVINGOBJCODE 기반</td>
             <td>RESOLVINGOBJCODE 필드에서 식별된 개체의 기본 키/ID입니다</td>
        </tr>
        <tr>
             <td>장미모양-</td>
             <td>FK</td>
             <td>ROLES_CURRENT</td>
             <td>장미모양-</td>
        </tr>
        <tr>
             <td>SOURCEOBJID</td>
             <td>FK</td>
             <td>변수, SOURCEOBJCODE 기반</td>
             <td>SOURCEOBJCODE 필드에서 식별된 객체의 기본 키/ID</td>
        </tr>
        <tr>
             <td>SOURCETASKID</td>
             <td>FK</td>
             <td>TASKS_CURRENT</td>
             <td>TASKID</td>
        </tr>
        <tr>
             <td>SUBMITTEDBYID</td>
             <td>FK</td>
             <td>USERS_CURRENT</td>
             <td>사용자 ID</td>
        </tr>
        <tr>
             <td>SYSID</td>
             <td>-</td>
             <td colspan="2">관계가 아닙니다. 내부 응용 프로그램 용도로 사용됩니다.</td>
        </tr>
        <tr>
             <td>티미드</td>
             <td>FK</td>
             <td>TEAMS_CURRENT</td>
             <td>티미드</td>
        </tr>
    </tbody>
</table>

### 매개변수

<table>
    <thead>
        <tr>
            <th>Workfront 엔티티 이름</th>
            <th>인터페이스 참조</th>
            <th>API 참조</th>
            <th>API 레이블</th>
            <th>데이터 레이크 보기</th>
        </tr>
      </thead>
      <tbody>
        <tr>
            <td>매개변수</td>
            <td>사용자 정의 필드</td>
            <td>매개 변수</td>
            <td>매개변수</td>
            <td>PARAMETERS_CURRENT<br>PARAMETERS_DAILY_HISTORY<br>PARAMETERS_EVENT</td>
        </tr>
      </tbody>
</table>
<table>
    <thead>
        <tr>
            <th>기본/외래 키</th>
            <th>유형</th>
            <th>관련 테이블</th>
            <th>관련 필드</th>
        </tr>
    </thead>
    <tbody>
        <tr>
             <td>LASTUPDATEDBYID</td>
             <td>FK</td>
             <td>USERS_CURRENT</td>
             <td>사용자 ID</td>
        </tr>
        <tr>
             <td>PARAMETERFILTERID</td>
             <td>-</td>
             <td colspan="2">매개변수 필터 테이블은 현재 지원되지 않습니다.</td>
        </tr>
        <tr>
             <td>매개 변수화</td>
             <td>PK</td>
             <td>-</td>
             <td>-</td>
        </tr>
        <tr>
             <td>SYSID</td>
             <td>-</td>
             <td colspan="2">관계가 아닙니다. 내부 응용 프로그램 용도로 사용됩니다.</td>
        </tr>
    </tbody>
</table>

### 매개변수 그룹

<table>
    <thead>
        <tr>
            <th>Workfront 엔티티 이름</th>
            <th>인터페이스 참조</th>
            <th>API 참조</th>
            <th>API 레이블</th>
            <th>데이터 레이크 보기</th>
        </tr>
      </thead>
      <tbody>
        <tr>
            <td>매개변수 그룹</td>
            <td>양식 섹션</td>
            <td>매개 변수</td>
            <td>매개변수 그룹</td>
            <td>PARAMETERGROUPS_CURRENT<br>PARAMETERGROUPS_DAILY_HISTORY<br>PARAMETERGROUPS_EVENT</td>
        </tr>
      </tbody>
</table>
<table>
    <thead>
        <tr>
            <th>기본/외래 키</th>
            <th>유형</th>
            <th>관련 테이블</th>
            <th>관련 필드</th>
        </tr>
    </thead>
    <tbody>
        <tr>
             <td>LASTUPDATEDBYID</td>
             <td>FK</td>
             <td>USERS_CURRENT</td>
             <td>사용자 ID</td>
        </tr>
        <tr>
             <td>PARAMETERGROUPID</td>
             <td>PK</td>
             <td>-</td>
             <td>-</td>
        </tr>
        <tr>
             <td>SYSID</td>
             <td>-</td>
             <td colspan="2">관계가 아닙니다. 내부 응용 프로그램 용도로 사용됩니다.</td>
        </tr>
    </tbody>
</table>

### 매개변수 옵션

<table>
    <thead>
        <tr>
            <th>Workfront 엔티티 이름</th>
            <th>인터페이스 참조</th>
            <th>API 참조</th>
            <th>API 레이블</th>
            <th>데이터 레이크 보기</th>
        </tr>
      </thead>
      <tbody>
        <tr>
            <td>매개변수 옵션</td>
            <td>매개변수 옵션</td>
            <td>POPT</td>
            <td>매개변수 옵션</td>
            <td>PARAMETEROPTIONS_CURRENT<br>PARAMETEROPTIONS_DAILY_HISTORY<br>PARAMETEROPTIONS_EVENT</td>
        </tr>
      </tbody>
</table>
<table>
    <thead>
        <tr>
            <th>기본/외래 키</th>
            <th>유형</th>
            <th>관련 테이블</th>
            <th>관련 필드</th>
        </tr>
    </thead>
    <tbody>
        <tr>
             <td>매개 변수화</td>
             <td>FK</td>
             <td>PARAMETERS_CURRENT</td>
             <td>매개 변수화</td>
        </tr>
        <tr>
             <td>PARAMETEROPATIONID</td>
             <td>PK</td>
             <td>-</td>
             <td>-</td>
        </tr>
        <tr>
             <td>SYSID</td>
             <td>-</td>
             <td colspan="2">관계가 아닙니다. 내부 응용 프로그램 용도로 사용됩니다.</td>
        </tr>
    </tbody>
</table>

### 포털 섹션 / 보고서

<table>
    <thead>
        <tr>
            <th>Workfront 엔티티 이름</th>
            <th>인터페이스 참조</th>
            <th>API 참조</th>
            <th>API 레이블</th>
            <th>데이터 레이크 보기</th>
        </tr>
      </thead>
      <tbody>
        <tr>
            <td>포털 섹션</td>
            <td>보고서</td>
            <td>PTLSEC</td>
            <td>보고서</td>
            <td>PORTALSECTIONS_CURRENT<br>PORTALSECTIONS_DAILY_HISTORY<br>PORTALSECTIONS_EVENT</td>
        </tr>
      </tbody>
</table>
<table>
    <thead>
        <tr>
            <th>기본/외래 키</th>
            <th>유형</th>
            <th>관련 테이블</th>
            <th>관련 필드</th>
        </tr>
    </thead>
    <tbody>
        <tr>
             <td>APPGLOBALID</td>
             <td>-</td>
             <td colspan="2">관계가 아닙니다. 내부 응용 프로그램 용도로 사용됩니다.</td>
        </tr>
        <tr>
             <td>ENTEREDBYID</td>
             <td>FK</td>
             <td>USERS_CURRENT</td>
             <td>사용자 ID</td>
        </tr>
        <tr>
             <td>여과물</td>
             <td>FK</td>
             <td>UIFILTERS_CURRENT</td>
             <td>여과물</td>
        </tr>
        <tr>
             <td>GROUPBYID</td>
             <td>FK</td>
             <td>UIGROUPYS_CURRENT</td>
             <td>GROUPBYID</td>
        </tr>
        <tr>
             <td>LASTUPDATEDBYID</td>
             <td>FK</td>
             <td>USERS_CURRENT</td>
             <td>사용자 ID</td>
        </tr>
        <tr>
             <td>LASTVIEWEDBYID</td>
             <td>FK</td>
             <td>USERS_CURRENT</td>
             <td>사용자 ID</td>
        </tr>
        <tr>
             <td>OBJID</td>
             <td>FK</td>
             <td>변수, OBJCODE 기반</td>
             <td>OBJCODE 필드에서 식별된 객체의 기본 키/ID</td>
        </tr>
        <tr>
             <td>PORTALSECTIONID</td>
             <td>PK</td>
             <td>-</td>
             <td>-</td>
        </tr>
        <tr>
             <td>PREFERENCEID</td>
             <td>FK</td>
             <td>PREFERENCES_CURRENT</td>
             <td>PREFERENCEID</td>
        </tr>
        <tr>
             <td>PUBLRUNASUSERID</td>
             <td>FK</td>
             <td>USERS_CURRENT</td>
             <td>사용자 ID</td>
        </tr>
        <tr>
             <td>REPORTFOLDERID</td>
             <td>FK</td>
             <td>REPORTFOLDERS_CURRENT</td>
             <td>REPORTFOLDERID</td>
        </tr>
        <tr>
             <td>RUNASUSERID</td>
             <td>FK</td>
             <td>USERS_CURRENT</td>
             <td>사용자 ID</td>
        </tr>
        <tr>
             <td>SCHEDULEDREPORTID</td>
             <td>-</td>
             <td colspan="2">예약된 보고서 테이블은 현재 지원되지 않습니다.</td>
        </tr>
        <tr>
             <td>SYSID</td>
             <td>-</td>
             <td colspan="2">관계가 아닙니다. 내부 응용 프로그램 용도로 사용됩니다.</td>
        </tr>
        <tr>
             <td>VIEWID</td>
             <td>FK</td>
             <td>UIVIEWS_CURRENT</td>
             <td>VIEWID</td>
        </tr>
    </tbody>
</table>

### 포털 탭/대시보드

<table>
    <thead>
        <tr>
            <th>Workfront 엔티티 이름</th>
            <th>인터페이스 참조</th>
            <th>API 참조</th>
            <th>API 레이블</th>
            <th>데이터 레이크 보기</th>
        </tr>
      </thead>
      <tbody>
        <tr>
            <td>포털 탭</td>
            <td>대시보드</td>
            <td>PTLTAB</td>
            <td>대시보드</td>
            <td>PORTALTAB_CURRENT<br>PORTALTAB_DAILY_HISTORY<br>PORTALTAB_EVENT</td>
        </tr>
      </tbody>
</table>
<table>
    <thead>
        <tr>
            <th>기본/외래 키</th>
            <th>유형</th>
            <th>관련 테이블</th>
            <th>관련 필드</th>
        </tr>
    </thead>
    <tbody>
        <tr>
             <td>DOCID</td>
             <td>-</td>
             <td colspan="2">관계가 아닙니다. 내부 응용 프로그램 용도로 사용됩니다.</td>
        </tr>
        <tr>
             <td>LASTUPDATEDBYID</td>
             <td>FK</td>
             <td>USERS_CURRENT</td>
             <td>사용자 ID</td>
        </tr>
        <tr>
             <td>PORTALPROFILEID</td>
             <td>-</td>
             <td colspan="2">관계가 아닙니다. 내부 응용 프로그램 용도로 사용됩니다.</td>
        </tr>
        <tr>
             <td>PORTALTABID</td>
             <td>PK</td>
             <td>-</td>
             <td>-</td>
        </tr>
        <tr>
             <td>SYSID</td>
             <td>-</td>
             <td colspan="2">관계가 아닙니다. 내부 응용 프로그램 용도로 사용됩니다.</td>
        </tr>
        <tr>
             <td>사용자 ID</td>
             <td>FK</td>
             <td>USERS_CURRENT</td>
             <td>사용자 ID</td>
        </tr>
    </tbody>
</table>

### 포털 탭 섹션

<table>
    <thead>
        <tr>
            <th>Workfront 엔티티 이름</th>
            <th>인터페이스 참조</th>
            <th>API 참조</th>
            <th>API 레이블</th>
            <th>데이터 레이크 보기</th>
        </tr>
      </thead>
      <tbody>
        <tr>
            <td>포털 탭 섹션</td>
            <td>대시보드 섹션</td>
            <td>PRTBSC</td>
            <td>포털 탭 섹션</td>
            <td>PORTALTABSPORTALSECTIONS_CURRENT<br>PORTALTABSPORTALSECTIONS_DAILY_HISTORY<br>PORTALTABSPORTALSECTIONS_EVENT</td>
        </tr>
      </tbody>
</table>
<table>
    <thead>
        <tr>
            <th>기본/외래 키</th>
            <th>유형</th>
            <th>관련 테이블</th>
            <th>관련 필드</th>
        </tr>
    </thead>
    <tbody>
        <tr>
             <td>CALENDARPORTALSECTIONID</td>
             <td>-</td>
             <td colspan="2">달력 포털 섹션은 현재 지원되지 않습니다.</td>
        </tr>
        <tr>
             <td>EXTERNALSECTIONID</td>
             <td>-</td>
             <td colspan="2">현재 외부 섹션 테이블이 지원되지 않음</td>
        </tr>
        <tr>
             <td>INTERNALSECTIONID</td>
             <td>FK</td>
             <td>PORTALSECTIONS_CURRENT</td>
             <td>PORTALSECTIONID</td>
        </tr>
        <tr>
             <td>PORTALSECTIONOBJID</td>
             <td>FK</td>
             <td>변수, PORTALSECTIONOBJCODE 기반</td>
             <td>PORTALSECTIONOBJCODE 필드에서 식별된 개체의 기본 키/ID</td>
        </tr>
        <tr>
             <td>PORTALTABID</td>
             <td>FK</td>
             <td>PORTALTAB_CURRENT</td>
             <td>PORTALTABID</td>
        </tr>
        <tr>
             <td>PORTALTABSECTIONID</td>
             <td>PK</td>
             <td>-</td>
             <td>-</td>
        </tr>
        <tr>
             <td>SYSID</td>
             <td>-</td>
             <td colspan="2">관계가 아닙니다. 내부 응용 프로그램 용도로 사용됩니다.</td>
        </tr>
    </tbody>
</table>

### 포털 섹션 마지막 뷰어

<table>
    <thead>
        <tr>
            <th>Workfront 엔티티 이름</th>
            <th>인터페이스 참조</th>
            <th>API 참조</th>
            <th>API 레이블</th>
            <th>데이터 레이크 보기</th>
        </tr>
      </thead>
      <tbody>
        <tr>
            <td>포털 섹션 마지막 뷰어</td>
            <td>마지막 뷰어 보고서</td>
            <td>PLSLSV</td>
            <td>포털 섹션 마지막 뷰어</td>
            <td>REPORTLASTVIEWERS_CURRENT<br>REPORTLASTVIEWERS_DAILY_HISTORY<br>REPORTLASTVIEWERS_EVENT</td>
        </tr>
      </tbody>
</table>
<table>
    <thead>
        <tr>
            <th>기본/외래 키</th>
            <th>유형</th>
            <th>관련 테이블</th>
            <th>관련 필드</th>
        </tr>
    </thead>
    <tbody>
        <tr>
             <td>REPORTID</td>
             <td>FK</td>
             <td>PORTALSECTIONS_CURRENT</td>
             <td>REPORTID</td>
        </tr>
        <tr>
             <td>REPORTLASTVIEWERID</td>
             <td>PK</td>
             <td>-</td>
             <td>-</td>
        </tr>
        <tr>
             <td>SYSID</td>
             <td>-</td>
             <td colspan="2">관계가 아닙니다. 내부 응용 프로그램 용도로 사용됩니다.</td>
        </tr>
        <tr>
             <td>VIEWERID</td>
             <td>FK</td>
             <td>USERS_CURRENT</td>
             <td>사용자 ID</td>
        </tr>
    </tbody>
</table>

### 포트폴리오

<table>
    <thead>
        <tr>
            <th>Workfront 엔티티 이름</th>
            <th>인터페이스 참조</th>
            <th>API 참조</th>
            <th>API 레이블</th>
            <th>데이터 레이크 보기</th>
        </tr>
      </thead>
      <tbody>
        <tr>
            <td>포트폴리오</td>
            <td>포트폴리오</td>
            <td>포트</td>
            <td>포트폴리오</td>
            <td>PORTFOLIOS_CURRENT<br>PORTFOLIOS_DAILY_HISTORY<br>포트폴리오_이벤트</td>
        </tr>
      </tbody>
</table>
<table>
    <thead>
        <tr>
            <th>기본/외래 키</th>
            <th>유형</th>
            <th>관련 테이블</th>
            <th>관련 필드</th>
        </tr>
    </thead>
    <tbody>
        <tr>
             <td>ALIGNMENTSCORECARDID</td>
             <td>-</td>
             <td colspan="2">스코어카드 테이블은 현재 지원되지 않습니다.</td>
        </tr>
        <tr>
             <td>범주 ID</td>
             <td>FK</td>
             <td>CATEGORS_CURRENT</td>
             <td>범주 ID</td>
        </tr>
        <tr>
             <td>ENTEREDBYID</td>
             <td>FK</td>
             <td>USERS_CURRENT</td>
             <td>사용자 ID</td>
        </tr>
        <tr>
             <td>GROUPID</td>
             <td>FK</td>
             <td>GROUPS_CURRENT</td>
             <td>GROUPID</td>
        </tr>
        <tr>
             <td>LASTUPDATEDBYID</td>
             <td>FK</td>
             <td>USERS_CURRENT</td>
             <td>사용자 ID</td>
        </tr>
        <tr>
             <td>소유자 ID</td>
             <td>FK</td>
             <td>USERS_CURRENT</td>
             <td>사용자 ID</td>
        </tr>
        <tr>
             <td>포트폴리오</td>
             <td>PK</td>
             <td>-</td>
             <td>-</td>
        </tr>
        <tr>
             <td>SYSID</td>
             <td>-</td>
             <td colspan="2">관계가 아닙니다. 내부 응용 프로그램 용도로 사용됩니다.</td>
        </tr>
    </tbody>
</table>

### 환경 설정

<table>
    <thead>
        <tr>
            <th>Workfront 엔티티 이름</th>
            <th>인터페이스 참조</th>
            <th>API 참조</th>
            <th>API 레이블</th>
            <th>데이터 레이크 보기</th>
        </tr>
      </thead>
      <tbody>
        <tr>
            <td>환경 설정</td>
            <td>보기, 필터링, 그룹화, 보고서 정의</td>
            <td>PROSET</td>
            <td>환경 설정</td>
            <td>PREFERENCES_CURRENT<br>PREFERENCES_DAILY_HISTORY<br>PREFERENCES_EVENT</td>
        </tr>
      </tbody>
</table>
<table>
    <thead>
        <tr>
            <th>기본/외래 키</th>
            <th>유형</th>
            <th>관련 테이블</th>
            <th>관련 필드</th>
        </tr>
    </thead>
    <tbody>
        <tr>
             <td>APPGLOBALID</td>
             <td>-</td>
             <td colspan="2">관계가 아닙니다. 내부 응용 프로그램 용도로 사용됩니다.</td>
        </tr>
        <tr>
             <td>PREFERENCEID</td>
             <td>PK</td>
             <td>-</td>
             <td>-</td>
        </tr>
        <tr>
             <td>SYSID</td>
             <td>-</td>
             <td colspan="2">관계가 아닙니다. 내부 응용 프로그램 용도로 사용됩니다.</td>
        </tr>
    </tbody>
</table>

### 프로그램

<table>
    <thead>
        <tr>
            <th>Workfront 엔티티 이름</th>
            <th>인터페이스 참조</th>
            <th>API 참조</th>
            <th>API 레이블</th>
            <th>데이터 레이크 보기</th>
        </tr>
      </thead>
      <tbody>
        <tr>
            <td>프로그램</td>
            <td>프로그램</td>
            <td>PRGM</td>
            <td>프로그램</td>
            <td>PROGRAMS_CURRENT<br>PROGRAMS_DAILY_HISTORY<br>PROGRAMS_EVENT</td>
        </tr>
      </tbody>
</table>
<table>
    <thead>
        <tr>
            <th>기본/외래 키</th>
            <th>유형</th>
            <th>관련 테이블</th>
            <th>관련 필드</th>
        </tr>
    </thead>
    <tbody>
        <tr>
             <td>범주 ID</td>
             <td>FK</td>
             <td>CATEGORS_CURRENT</td>
             <td>범주 ID</td>
        </tr>
        <tr>
             <td>ENTEREDBYID</td>
             <td>FK</td>
             <td>USERS_CURRENT</td>
             <td>사용자 ID</td>
        </tr>
        <tr>
             <td>GROUPID</td>
             <td>FK</td>
             <td>GROUPS_CURRENT</td>
             <td>GROUPID</td>
        </tr>
        <tr>
             <td>LASTUPDATEDBYID</td>
             <td>FK</td>
             <td>USERS_CURRENT</td>
             <td>사용자 ID</td>
        </tr>
        <tr>
             <td>소유자 ID</td>
             <td>FK</td>
             <td>USERS_CURRENT</td>
             <td>사용자 ID</td>
        </tr>
        <tr>
             <td>포트폴리오</td>
             <td>FK</td>
             <td>포트폴리오_현재</td>
             <td>포트폴리오</td>
        </tr>
        <tr>
             <td>PROGRAMID</td>
             <td>PK</td>
             <td>-</td>
             <td>-</td>
        </tr>
        <tr>
             <td>SYSID</td>
             <td>-</td>
             <td colspan="2">관계가 아닙니다. 내부 응용 프로그램 용도로 사용됩니다.</td>
        </tr>
    </tbody>
</table>

### 프로젝트

<table>
    <thead>
        <tr>
            <th>Workfront 엔티티 이름</th>
            <th>인터페이스 참조</th>
            <th>API 참조</th>
            <th>API 레이블</th>
            <th>데이터 레이크 보기</th>
        </tr>
      </thead>
      <tbody>
        <tr>
            <td>프로젝트</td>
            <td>프로젝트</td>
            <td>프로젝트</td>
            <td>프로젝트</td>
            <td>PROJECTS_CURRENT<br>PROJECTS_DAILY_HISTORY<br>PROJECTS_EVENT</td>
        </tr>
      </tbody>
</table>
<table>
    <thead>
        <tr>
            <th>기본/외래 키</th>
            <th>유형</th>
            <th>관련 테이블</th>
            <th>관련 필드</th>
        </tr>
    </thead>
    <tbody>
        <tr>
             <td>AEMNATIVEFOLDERTREESREFID</td>
             <td>-</td>
             <td colspan="2">관계가 아닙니다. 내부 응용 프로그램 용도로 사용됩니다.</td>
        </tr>
        <tr>
             <td>ALIGNMENTSCORECARDID</td>
             <td>-</td>
             <td colspan="2">스코어카드 테이블은 현재 지원되지 않습니다.</td>
        </tr>
        <tr>
             <td>APPROVALPROCESSID</td>
             <td>FK</td>
             <td>APPROVALPROCESSES_CURRENT</td>
             <td>APPROVALPROCESSID</td>
        </tr>
        <tr>
             <td>ATTACHEDATECARDID</td>
             <td>FK</td>
             <td>RATECARD_CURRENT</td>
             <td>RATECARDID</td>
        </tr>
        <tr>
             <td>범주 ID</td>
             <td>FK</td>
             <td>CATEGORS_CURRENT</td>
             <td>범주 ID</td>
        </tr>
        <tr>
             <td>COMPANYID</td>
             <td>FK</td>
             <td>COMPANIES_CURRENT</td>
             <td>COMPANYID</td>
        </tr>
        <tr>
             <td>CONVERTEDOPTASKID</td>
             <td>FK</td>
             <td>OPTASKS_CURRENT</td>
             <td>OPTASKID</td>
        </tr>
        <tr>
             <td>CONVERTEDOPTASKORIGINATORID</td>
             <td>FK</td>
             <td>USERS_CURRENT</td>
             <td>사용자 ID</td>
        </tr>
        <tr>
             <td>CURRENTAPPROVALSTEPID</td>
             <td>FK</td>
             <td>APPROVALSTEPS_CURRENT</td>
             <td>승인스테피드</td>
        </tr>
        <tr>
             <td>DELIVERABLESCORECARDID</td>
             <td>-</td>
             <td colspan="2">스코어카드 테이블은 현재 지원되지 않습니다.</td>
        </tr>
        </tr>
        <tr>
             <td>ENTEREDBYID</td>
             <td>FK</td>
             <td>USERS_CURRENT</td>
             <td>사용자 ID</td>
        </tr>
        <tr>
             <td>GROUPID</td>
             <td>FK</td>
             <td>GROUPS_CURRENT</td>
             <td>GROUPID</td>
        </tr>
        <tr>
             <td>LASTCONDITIONNOTEID</td>
             <td>FK</td>
             <td>NOTES_CURRENT</td>
             <td>NOTEID</td>
        </tr>
        <tr>
             <td>LASTNOTEID</td>
             <td>FK</td>
             <td>NOTES_CURRENT</td>
             <td>NOTEID</td>
        </tr>
        <tr>
             <td>LASTUPDATEDBYID</td>
             <td>FK</td>
             <td>USERS_CURRENT</td>
             <td>사용자 ID</td>
        </tr>
        <tr>
             <td>마일스톤 경로 ID</td>
             <td>FK</td>
             <td>MILESTONEPATHS_CURRENT</td>
             <td>마일스톤 경로 ID</td>
        </tr>
        <tr>
             <td>소유자 ID</td>
             <td>FK</td>
             <td>USERS_CURRENT</td>
             <td>사용자 ID</td>
        </tr>
        <tr>
             <td>POPACCOUNTID</td>
             <td>-</td>
             <td colspan="2">Pop 계정 테이블은 현재 지원되지 않습니다.</td>
        </tr>
        <tr>
             <td>포트폴리오</td>
             <td>FK</td>
             <td>포트폴리오_현재</td>
             <td>포트폴리오</td>
        </tr>
        <tr>
             <td>PRIVATERATECARDID</td>
             <td>FK</td>
             <td>RATECARD_CURRENT</td>
             <td>RATECARDID</td>
        </tr>
        <tr>
             <td>PROGRAMID</td>
             <td>FK</td>
             <td>PROGRAMS_CURRENT</td>
             <td>PROGRAMID</td>
        </tr>
        <tr>
             <td>PROJECTID</td>
             <td>PK</td>
             <td>-</td>
             <td>-</td>
        </tr>
        <tr>
             <td>QUEUEDEFID</td>
             <td>-</td>
             <td colspan="2">대기열 정의 테이블은 현재 지원되지 않습니다.</td>
        </tr>
        <tr>
             <td>REJECTIONISSUEID</td>
             <td>FK</td>
             <td>OPTASKS_CURRENT</td>
             <td>OPTASKID</td>
        </tr>
        <tr>
             <td>RESOURCEPOOLID</td>
             <td>FK</td>
             <td>RESOURCEPOOL_CURRENT</td>
             <td>RESOURCEPOOLID</td>
        </tr>
        <tr>
             <td>예약 ID</td>
             <td>FK</td>
             <td>SCHEDULES_CURRENT</td>
             <td>예약 ID</td>
        </tr>
        <tr>
             <td>스폰소이드</td>
             <td>FK</td>
             <td>USERS_CURRENT</td>
             <td>사용자 ID</td>
        </tr>
        <tr>
             <td>SUBMITTEDBYID</td>
             <td>FK</td>
             <td>USERS_CURRENT</td>
             <td>사용자 ID</td>
        </tr>
        <tr>
             <td>SYSID</td>
             <td>-</td>
             <td colspan="2">관계가 아닙니다. 내부 응용 프로그램 용도로 사용됩니다.</td>
        </tr>
        <tr>
             <td>티미드</td>
             <td>FK</td>
             <td>TEAMS_CURRENT</td>
             <td>티미드</td>
        </tr>
        <tr>
             <td>TEMPLATEID</td>
             <td>FK</td>
             <td>TEMPLATES_CURRENT</td>
             <td>TEMPLATEID</td>
        </tr>
    </tbody>
</table>

### 프로젝트 팀 사용자

<table>
    <thead>
        <tr>
            <th>Workfront 엔티티 이름</th>
            <th>인터페이스 참조</th>
            <th>API 참조</th>
            <th>API 레이블</th>
            <th>데이터 레이크 보기</th>
        </tr>
      </thead>
      <tbody>
        <tr>
            <td>프로젝트 팀 사용자</td>
            <td>프로젝트 팀 사용자</td>
            <td>PRTU</td>
            <td>프로젝트 사용자</td>
            <td>PROJECTSUSERS_CURRENT<br>PROJECTSUSERS_DAILY_HISTORY<br>PROJECTSUSERS_EVENT</td>
        </tr>
      </tbody>
</table>
<table>
    <thead>
        <tr>
            <th>기본/외래 키</th>
            <th>유형</th>
            <th>관련 테이블</th>
            <th>관련 필드</th>
        </tr>
    </thead>
    <tbody>
        <tr>
             <td>PROJECTID</td>
             <td>FK</td>
             <td>PROJECTS_CURRENT</td>
             <td>PROJECTID</td>
        </tr>
        <tr>
             <td>PROJECTSUSERID</td>
             <td>PK</td>
             <td>-</td>
             <td>-</td>
        </tr>
        <tr>
             <td>SYSID</td>
             <td>-</td>
             <td colspan="2">관계가 아닙니다. 내부 응용 프로그램 용도로 사용됩니다.</td>
        </tr>
        <tr>
             <td>TMPUSERID</td>
             <td>-</td>
             <td colspan="2">관계가 아닙니다. 내부 응용 프로그램 용도로 사용됩니다.</td>
        </tr>
        <tr>
             <td>사용자 ID</td>
             <td>FK</td>
             <td>USERS_CURRENT</td>
             <td>사용자 ID</td>
        </tr>
    </tbody>
</table>

### 프로젝트 팀 사용자 역할

<table>
    <thead>
        <tr>
            <th>Workfront 엔티티 이름</th>
            <th>인터페이스 참조</th>
            <th>API 참조</th>
            <th>API 레이블</th>
            <th>데이터 레이크 보기</th>
        </tr>
      </thead>
      <tbody>
        <tr>
            <td>프로젝트 팀 사용자 역할</td>
            <td>프로젝트 팀 사용자 역할</td>
            <td>TEAM</td>
            <td>프로젝트 사용자 역할</td>
            <td>PROJECTSUSERSROLES_CURRENT<br>PROJECTSUSERSROLES_DAILY_HISTORY<br>PROJECTSUSERSROLES_EVENT</td>
        </tr>
      </tbody>
</table>
<table>
    <thead>
        <tr>
            <th>기본/외래 키</th>
            <th>유형</th>
            <th>관련 테이블</th>
            <th>관련 필드</th>
        </tr>
    </thead>
    <tbody>
        <tr>
             <td>PROJECTID</td>
             <td>FK</td>
             <td>PROJECTS_CURRENT</td>
             <td>PROJECTID</td>
        </tr>
        <tr>
             <td>PROJECTSUSERSROLEID</td>
             <td>PK</td>
             <td>-</td>
             <td>-</td>
        </tr>
        <tr>
             <td>장미모양-</td>
             <td>FK</td>
             <td>ROLES_CURRENT</td>
             <td>장미모양-</td>
        </tr>
        <tr>
             <td>SYSID</td>
             <td>-</td>
             <td colspan="2">관계가 아닙니다. 내부 응용 프로그램 용도로 사용됩니다.</td>
        </tr>
        <tr>
             <td>사용자 ID</td>
             <td>FK</td>
             <td>USERS_CURRENT</td>
             <td>사용자 ID</td>
        </tr>
    </tbody>
</table>

### 요율 카드

<table>
    <thead>
        <tr>
            <th>Workfront 엔티티 이름</th>
            <th>인터페이스 참조</th>
            <th>API 참조</th>
            <th>API 레이블</th>
            <th>데이터 레이크 보기</th>
        </tr>
      </thead>
      <tbody>
        <tr>
            <td>요율 카드</td>
            <td>요율 카드</td>
            <td>RTCRD</td>
            <td>요율 카드</td>
            <td>RATECARD_CURRENT<br>RATECARD_DAILY_HISTORY<br>RATECARD_EVENT</td>
        </tr>
      </tbody>
</table>
<table>
    <thead>
        <tr>
            <th>기본/외래 키</th>
            <th>유형</th>
            <th>관련 테이블</th>
            <th>관련 필드</th>
        </tr>
    </thead>
    <tbody>
        <tr>
             <td>범주 ID</td>
             <td>FK</td>
             <td>CATEGORS_CURRENT</td>
             <td>범주 ID</td>
        </tr>
        <tr>
             <td>ENTEREDBYID</td>
             <td>FK</td>
             <td>USERS_CURRENT</td>
             <td>사용자 ID</td>
        </tr>
        <tr>
             <td>LASTUPDATEDBYID</td>
             <td>FK</td>
             <td>USERS_CURRENT</td>
             <td>사용자 ID</td>
        </tr>
        <tr>
             <td>RATECARDID</td>
             <td>PK</td>
             <td>-</td>
             <td>-</td>
        </tr>
        <tr>
             <td>SECURITYROOTID</td>
             <td>FK</td>
             <td>변수, SECURITYOBJCODE 기반</td>
             <td>SECURITYOBJCODE 필드에서 식별된 객체의 기본 키/ID</td>
        </tr>
        <tr>
             <td>SOURCEID</td>
             <td>FK</td>
             <td>변수, SOURCEOBJCODE 기반</td>
             <td>SOURCEOBJCODE 필드에서 식별된 객체의 기본 키/ID</td>
        </tr>
        <tr>
             <td>SYSID</td>
             <td>-</td>
             <td colspan="2">관계가 아닙니다. 내부 응용 프로그램 용도로 사용됩니다.</td>
        </tr>

    &lt;/tbody>
</table>

### 보고서 폴더

<table>
    <thead>
        <tr>
            <th>Workfront 엔티티 이름</th>
            <th>인터페이스 참조</th>
            <th>API 참조</th>
            <th>API 레이블</th>
            <th>데이터 레이크 보기</th>
        </tr>
      </thead>
      <tbody>
        <tr>
            <td>보고서 폴더</td>
            <td>보고서 폴더</td>
            <td>RPTFDR</td>
            <td>보고서 폴더</td>
            <td>REPORTFOLDERS_CURRENT<br>REPORTFOLDERS_DAILY_HISTORY<br>REPORTFOLDERS_EVENT</td>
        </tr>
      </tbody>
</table>
<table>
    <thead>
        <tr>
            <th>기본/외래 키</th>
            <th>유형</th>
            <th>관련 테이블</th>
            <th>관련 필드</th>
        </tr>
    </thead>
    <tbody>
        <tr>
             <td>REPORTFOLDERID</td>
             <td>PK</td>
             <td>-</td>
             <td>-</td>
        </tr>
        <tr>
             <td>SYSID</td>
             <td>-</td>
             <td colspan="2">관계가 아닙니다. 내부 응용 프로그램 용도로 사용됩니다.</td>
        </tr>
    </tbody>
</table>

### 보고서 보기 통계 수

<table>
    <thead>
        <tr>
            <th>Workfront 엔티티 이름</th>
            <th>인터페이스 참조</th>
            <th>API 참조</th>
            <th>API 레이블</th>
            <th>데이터 레이크 보기</th>
        </tr>
      </thead>
      <tbody>
        <tr>
            <td>보고서 보기 통계 수</td>
            <td>보고서 보기 통계 수</td>
            <td>PLSVST</td>
            <td>PortalSectionStatisticInfo</td>
            <td>REPORTVIEWSTATICCOUNTS_CURRENT<br>REPORTVIEWSTATICCOUNTS_DAILY_HISTORY<br>REPORTVIEWSTATICCOUNTS_EVENT</td>
        </tr>
      </tbody>
</table>
<table>
    <thead>
        <tr>
            <th>기본/외래 키</th>
            <th>유형</th>
            <th>관련 테이블</th>
            <th>관련 필드</th>
        </tr>
    </thead>
    <tbody>
        <tr>
             <td>REPORTID</td>
             <td>FK</td>
             <td>PORTALSECTIONS_CURRENT</td>
             <td>PORTALSECTIONID</td>
        </tr>
        <tr>
             <td>REPORTVIEWSTATICCOUNTID</td>
             <td>PK</td>
             <td>-</td>
             <td>-</td>
        </tr>
        <tr>
             <td>SYSID</td>
             <td>-</td>
             <td colspan="2">관계가 아닙니다. 내부 응용 프로그램 용도로 사용됩니다.</td>
        </tr>
    </tbody>
</table>

### 보고 가능한 예산 시간

<table>
    <thead>
        <tr>
            <th>Workfront 엔티티 이름</th>
            <th>인터페이스 참조</th>
            <th>API 참조</th>
            <th>API 레이블</th>
            <th>데이터 레이크 보기</th>
        </tr>
      </thead>
      <tbody>
        <tr>
            <td>보고 가능한 예산 시간</td>
            <td>보고 가능한 예산 시간</td>
            <td>RPBGHR</td>
            <td>예산 시간</td>
            <td>REPORTABLEBUDGETEDHOURS_CURRENT<br>REPORTABLEBUDGETEDHOURS_DAILY_HISTORY<br>REPORTABLEBUDGETEDHOURS_EVENT</td>
        </tr>
      </tbody>
</table>
<table>
    <thead>
        <tr>
            <th>기본/외래 키</th>
            <th>유형</th>
            <th>관련 테이블</th>
            <th>관련 필드</th>
        </tr>
    </thead>
    <tbody>
        <tr>
             <td>PROJECTID</td>
             <td>FK</td>
             <td>PROJECTS_CURRENT</td>
             <td>PROJECTID</td>
        </tr>
        <tr>
             <td>REPORTABLEBUDGETEDHOURID</td>
             <td>PK</td>
             <td>-</td>
             <td>-</td>
        </tr>
        <tr>
             <td>장미모양-</td>
             <td>FK</td>
             <td>ROLES_CURRENT</td>
             <td>장미모양-</td>
        </tr>
        <tr>
             <td>SYSID</td>
             <td>-</td>
             <td colspan="2">관계가 아닙니다. 내부 응용 프로그램 용도로 사용됩니다.</td>
        </tr>
        <tr>
             <td>사용자 ID</td>
             <td>FK</td>
             <td>USERS_CURRENT</td>
             <td>사용자 ID</td>
        </tr>
    </tbody>
</table>

### 예약 시간/PTO

<table>
    <thead>
        <tr>
            <th>Workfront 엔티티 이름</th>
            <th>인터페이스 참조</th>
            <th>API 참조</th>
            <th>API 레이블</th>
            <th>데이터 레이크 보기</th>
        </tr>
      </thead>
      <tbody>
        <tr>
            <td>예약된 시간</td>
            <td>(개인) 휴무</td>
            <td>REVT</td>
            <td>휴무</td>
            <td>RESERVEDTIMES_CURRENT<br>RESERVEDTIMES_DAILY_HISTORY<br>RESERVEDTIMES_EVENT</td>
        </tr>
      </tbody>
</table>
<table>
    <thead>
        <tr>
            <th>기본/외래 키</th>
            <th>유형</th>
            <th>관련 테이블</th>
            <th>관련 필드</th>
        </tr>
    </thead>
    <tbody>
        <tr>
             <td>RESERVEDTIMEID</td>
             <td>PK</td>
             <td>-</td>
             <td>-</td>
        </tr>
        <tr>
             <td>SYSID</td>
             <td>-</td>
             <td colspan="2">관계가 아닙니다. 내부 응용 프로그램 용도로 사용됩니다.</td>
        </tr>
        <tr>
             <td>TASKID</td>
             <td>FK</td>
             <td>TASKS_CURRENT</td>
             <td>TASKID</td>
        </tr>
        <tr>
             <td>사용자 ID</td>
             <td>FK</td>
             <td>USERS_CURRENT</td>
             <td>사용자 ID</td>
        </tr>
    </tbody>
</table>

### 리소스 관리자

<table>
    <thead>
        <tr>
            <th>Workfront 엔티티 이름</th>
            <th>인터페이스 참조</th>
            <th>API 참조</th>
            <th>API 레이블</th>
            <th>데이터 레이크 보기</th>
        </tr>
      </thead>
      <tbody>
        <tr>
            <td>리소스 관리자</td>
            <td>리소스 관리자</td>
            <td>RESMGR</td>
            <td>리소스 관리자</td>
            <td>RESOURCEMANAGERS_CURRENT<br>RESOURCEMANAGERS_DAILY_HISTORY<br>RESOURCEMANAGERS_EVENT</td>
        </tr>
      </tbody>
</table>
<table>
    <thead>
        <tr>
            <th>기본/외래 키</th>
            <th>유형</th>
            <th>관련 테이블</th>
            <th>관련 필드</th>
        </tr>
    </thead>
    <tbody>
        <tr>
             <td>ID</td>
             <td>PK</td>
             <td>-</td>
             <td>-</td>
        </tr>
        <tr>
             <td>PROJECTID</td>
             <td>FK</td>
             <td>PROJECTS_CURRENT</td>
             <td>PROJECTID</td>
        </tr>
        <tr>
             <td>RESOURCEMANAGERID</td>
             <td>FK</td>
             <td>USERS_CURRENT</td>
             <td>사용자 ID</td>
        </tr>
        <tr>
             <td>SYSID</td>
             <td>-</td>
             <td colspan="2">관계가 아닙니다. 내부 응용 프로그램 용도로 사용됩니다.</td>
        </tr>
        <tr>
             <td>TEMPLATEID</td>
             <td>FK</td>
             <td>TEMPLATES_CURRENT</td>
             <td>TEMPLATEID</td>
        </tr>
    </tbody>
</table>

### 리소스 풀

<table>
    <thead>
        <tr>
            <th>Workfront 엔티티 이름</th>
            <th>인터페이스 참조</th>
            <th>API 참조</th>
            <th>API 레이블</th>
            <th>데이터 레이크 보기</th>
        </tr>
      </thead>
      <tbody>
        <tr>
            <td>리소스 풀</td>
            <td>리소스 풀</td>
            <td>RSPL</td>
            <td>리소스 풀</td>
            <td>RSRCPOOLS_CURRENT<br>RSRCPOOLS_DAILY_HISTORY<br>RSRCPOOLS_EVENT</td>
        </tr>
      </tbody>
</table>
<table>
    <thead>
        <tr>
            <th>기본/외래 키</th>
            <th>유형</th>
            <th>관련 테이블</th>
            <th>관련 필드</th>
        </tr>
    </thead>
    <tbody>
        <tr>
             <td>ENTEREDBYID</td>
             <td>FK</td>
             <td>USERS_CURRENT</td>
             <td>사용자 ID</td>
        </tr>
        <tr>
             <td>LASTUPDATEDBYID</td>
             <td>FK</td>
             <td>USERS_CURRENT</td>
             <td>사용자 ID</td>
        </tr>
        <tr>
             <td>RESOURCEPOOLID</td>
             <td>PK</td>
             <td>-</td>
             <td>-</td>
        </tr>
        <tr>
             <td>SYSID</td>
             <td>-</td>
             <td colspan="2">관계가 아닙니다. 내부 응용 프로그램 용도로 사용됩니다.</td>
        </tr>
    </tbody>
</table>

### 서식 있는 텍스트 메모

<table>
    <thead>
        <tr>
            <th>Workfront 엔티티 이름</th>
            <th>인터페이스 참조</th>
            <th>API 참조</th>
            <th>API 레이블</th>
            <th>데이터 레이크 보기</th>
        </tr>
      </thead>
      <tbody>
        <tr>
            <td>서식 있는 텍스트 메모</td>
            <td>서식 있는 텍스트 메모</td>
            <td>RHNOTE</td>
            <td>서식 있는 텍스트 메모</td>
            <td>RESERVEDTEXTNOTES_CURRENT<br>RESERVEDTEXTNOTES_DAILY_HISTORY<br>RESERVEDTEXTNOTES_EVENT</td>
        </tr>
      </tbody>
</table>
<table>
    <thead>
        <tr>
            <th>기본/외래 키</th>
            <th>유형</th>
            <th>관련 테이블</th>
            <th>관련 필드</th>
        </tr>
    </thead>
    <tbody>
        <tr>
             <td>RICHTEXTNOTEID</td>
             <td>PK</td>
             <td>-</td>
             <td>-</td>
        </tr>
        <tr>
             <td>SYSID</td>
             <td>-</td>
             <td colspan="2">관계가 아닙니다. 내부 응용 프로그램 용도로 사용됩니다.</td>
        </tr>
    </tbody>
</table>

### 리치 텍스트 매개 변수 값

<table>
    <thead>
        <tr>
            <th>Workfront 엔티티 이름</th>
            <th>인터페이스 참조</th>
            <th>API 참조</th>
            <th>API 레이블</th>
            <th>데이터 레이크 보기</th>
        </tr>
      </thead>
      <tbody>
        <tr>
            <td>리치 텍스트 매개 변수 값</td>
            <td>리치 텍스트 매개 변수 값</td>
            <td>RCHVAL</td>
            <td>리치 텍스트 매개 변수 값</td>
            <td>RICHTEXTPARAMETERVALUES_CURRENT<br>RICHTEXTPARAMETERVALUES_DAILY_HISTORY<br>RICHTEXTPARAMETERVALUES_EVENT</td>
        </tr>
      </tbody>
</table>
<table>
    <thead>
        <tr>
            <th>기본/외래 키</th>
            <th>유형</th>
            <th>관련 테이블</th>
            <th>관련 필드</th>
        </tr>
    </thead>
    <tbody>
        <tr>
             <td>PARAMETERVALUEID</td>
             <td>-</td>
             <td colspan="2">매개변수 값 테이블은 현재 지원되지 않습니다.</td>
        </tr>
        <tr>
             <td>RICHTEXTPARAMETERVALUEID</td>
             <td>PK</td>
             <td>-</td>
             <td>-</td>
        </tr>
        <tr>
             <td>SYSID</td>
             <td>-</td>
             <td colspan="2">관계가 아닙니다. 내부 응용 프로그램 용도로 사용됩니다.</td>
        </tr>
    </tbody>
</table>

### 위험

<table>
    <thead>
        <tr>
            <th>Workfront 엔티티 이름</th>
            <th>인터페이스 참조</th>
            <th>API 참조</th>
            <th>API 레이블</th>
            <th>데이터 레이크 보기</th>
        </tr>
      </thead>
      <tbody>
        <tr>
            <td>위험</td>
            <td>위험</td>
            <td>위험</td>
            <td>위험</td>
            <td>RISK_CURRENT<br>RISK_DAILY_HISTORY<br>RISK_EVENT</td>
        </tr>
      </tbody>
</table>
<table>
    <thead>
        <tr>
            <th>기본/외래 키</th>
            <th>유형</th>
            <th>관련 테이블</th>
            <th>관련 필드</th>
        </tr>
    </thead>
    <tbody>
        <tr>
             <td>ENTEREDBYID</td>
             <td>FK</td>
             <td>USERS_CURRENT</td>
             <td>사용자 ID</td>
        </tr>
        <tr>
             <td>EXCHANGERATEID</td>
             <td>FK</td>
             <td>EXCHANGE_CURRENT</td>
             <td>EXCHANGERATEID</td>
        </tr>
        <tr>
             <td>LASTUPDATEDBYID</td>
             <td>FK</td>
             <td>USERS_CURRENT</td>
             <td>사용자 ID</td>
        </tr>
        <tr>
             <td>PROJECTID</td>
             <td>FK</td>
             <td>PROJECTS_CURRENT</td>
             <td>PROJECTID</td>
        </tr>
        <tr>
             <td>위험하</td>
             <td>PK</td>
             <td>-</td>
             <td>-</td>
        </tr>
        <tr>
             <td>RISKTYPEID</td>
             <td>FK</td>
             <td>RISKTYPES_CURRENT</td>
             <td>RISKTYPEID</td>
        </tr>
        <tr>
             <td>SYSID</td>
             <td>-</td>
             <td colspan="2">관계가 아닙니다. 내부 응용 프로그램 용도로 사용됩니다.</td>
        </tr>
        <tr>
             <td>TEMPLATEID</td>
             <td>FK</td>
             <td>TEMPLATES_CURRENT</td>
             <td>TEMPLATEID</td>
        </tr>
    </tbody>
</table>

### 위험 유형

<table>
    <thead>
        <tr>
            <th>Workfront 엔티티 이름</th>
            <th>인터페이스 참조</th>
            <th>API 참조</th>
            <th>API 레이블</th>
            <th>데이터 레이크 보기</th>
        </tr>
      </thead>
      <tbody>
        <tr>
            <td>위험 유형</td>
            <td>위험 유형</td>
            <td>RSKTYP</td>
            <td>위험 유형</td>
            <td>RISKTYPES_CURRENT<br>RISKTYPES_DAILY_HISTORY<br>RISKTYPES_EVENT</td>
        </tr>
      </tbody>
</table>
<table>
    <thead>
        <tr>
            <th>기본/외래 키</th>
            <th>유형</th>
            <th>관련 테이블</th>
            <th>관련 필드</th>
        </tr>
    </thead>
    <tbody>
        <tr>
             <td>RISKTYPEID</td>
             <td>PK</td>
             <td>-</td>
             <td>-</td>
        </tr>
        <tr>
             <td>SYSID</td>
             <td>-</td>
             <td colspan="2">관계가 아닙니다. 내부 응용 프로그램 용도로 사용됩니다.</td>
        </tr>
    </tbody>
</table>

### 역할

<table>
    <thead>
        <tr>
            <th>Workfront 엔티티 이름</th>
            <th>인터페이스 참조</th>
            <th>API 참조</th>
            <th>API 레이블</th>
            <th>데이터 레이크 보기</th>
        </tr>
      </thead>
      <tbody>
        <tr>
            <td>역할</td>
            <td>작업 역할</td>
            <td>역할</td>
            <td>작업 역할</td>
            <td>ROLES_CURRENT<br>ROLES_DAILY_HISTORY<br>ROLES_EVENT</td>
        </tr>
      </tbody>
</table>
<table>
    <thead>
        <tr>
            <th>기본/외래 키</th>
            <th>유형</th>
            <th>관련 테이블</th>
            <th>관련 필드</th>
        </tr>
    </thead>
    <tbody>
        <tr>
             <td>ENTEREDBYID</td>
             <td>FK</td>
             <td>USERS_CURRENT</td>
             <td>사용자 ID</td>
        </tr>
        <tr>
             <td>LAYOUTTEMPLATEID</td>
             <td>-</td>
             <td colspan="2">레이아웃 템플릿 테이블은 지원되지 않습니다.</td>
        </tr>
        <tr>
             <td>PRIVATERATECARDID</td>
             <td>FK</td>
             <td>RATECARD_CURRENT</td>
             <td>RATECARDID</td>
        </tr>
        <tr>
             <td>장미모양-</td>
             <td>PK</td>
             <td>-</td>
             <td>-</td>
        </tr>
        <tr>
             <td>SYSID</td>
             <td>-</td>
             <td colspan="2">관계가 아닙니다. 내부 응용 프로그램 용도로 사용됩니다.</td>
        </tr>
        <tr>
             <td>UITEMPLATEID</td>
             <td>FK</td>
             <td>UITEMPLATES_CURRENT</td>
             <td>UITEMPLATEID</td>
        </tr>
    </tbody>
</table>

### 예약

<table>
    <thead>
        <tr>
            <th>Workfront 엔티티 이름</th>
            <th>인터페이스 참조</th>
            <th>API 참조</th>
            <th>API 레이블</th>
            <th>데이터 레이크 보기</th>
        </tr>
      </thead>
      <tbody>
        <tr>
            <td>예약</td>
            <td>예약</td>
            <td>일정 조정됨</td>
            <td>예약</td>
            <td>SCHEDULES_CURRENT<br>SCHEDULES_DAILY_HISTORY<br>SCHEDULES_EVENT</td>
        </tr>
      </tbody>
</table>
<table>
    <thead>
        <tr>
            <th>기본/외래 키</th>
            <th>유형</th>
            <th>관련 테이블</th>
            <th>관련 필드</th>
        </tr>
    </thead>
    <tbody>
        <tr>
             <td>ENTEREDBYID</td>
             <td>FK</td>
             <td>USERS_CURRENT</td>
             <td>사용자 ID</td>
        </tr>
        <tr>
             <td>GROUPID</td>
             <td>FK</td>
             <td>GROUPS_CURRENT</td>
             <td>GROUPID</td>
        </tr>
        <tr>
             <td>HOMEGROUPID</td>
             <td>FK</td>
             <td>GROUPS_CURRENT</td>
             <td>GROUPID</td>
        </tr>
        <tr>
             <td>예약 ID</td>
             <td>PK</td>
             <td>-</td>
             <td>-</td>
        </tr>
        <tr>
             <td>SYSID</td>
             <td>-</td>
             <td colspan="2">관계가 아닙니다. 내부 응용 프로그램 용도로 사용됩니다.</td>
        </tr>
    </tbody>
</table>

### 단계 승인자

<table>
    <thead>
        <tr>
            <th>Workfront 엔티티 이름</th>
            <th>인터페이스 참조</th>
            <th>API 참조</th>
            <th>API 레이블</th>
            <th>데이터 레이크 보기</th>
        </tr>
      </thead>
      <tbody>
        <tr>
            <td>단계 승인자</td>
            <td>단계 승인자</td>
            <td>SPAPVR</td>
            <td>단계 승인자</td>
            <td>STEPAPPROVERS_CURRENT<br>STEPAPPROVERS_DAILY_HISTORY<br>STEPAPPROVERS_EVENT</td>
        </tr>
      </tbody>
</table>
<table>
    <thead>
        <tr>
            <th>기본/외래 키</th>
            <th>유형</th>
            <th>관련 테이블</th>
            <th>관련 필드</th>
        </tr>
    </thead>
    <tbody>
        <tr>
             <td>승인스테피드</td>
             <td>FK</td>
             <td>APPROVALSTEPS_CURRENT</td>
             <td>승인스테피드</td>
        </tr>
        <tr>
             <td>장미모양-</td>
             <td>FK</td>
             <td>ROLES_CURRENT</td>
             <td>장미모양-</td>
        </tr>
        <tr>
             <td>STEAPPROVERID</td>
             <td>PK</td>
             <td>-</td>
             <td>-</td>
        </tr>
        <tr>
             <td>SYSID</td>
             <td>-</td>
             <td colspan="2">관계가 아닙니다. 내부 응용 프로그램 용도로 사용됩니다.</td>
        </tr>
        <tr>
             <td>티미드</td>
             <td>FK</td>
             <td>TEAMS_CURRENT</td>
             <td>티미드</td>
        </tr>
        <tr>
             <td>사용자 ID</td>
             <td>FK</td>
             <td>USERS_CURRENT</td>
             <td>사용자 ID</td>
        </tr>
    </tbody>
</table>

### 작업

<table>
    <thead>
        <tr>
            <th>Workfront 엔티티 이름</th>
            <th>인터페이스 참조</th>
            <th>API 참조</th>
            <th>API 레이블</th>
            <th>데이터 레이크 보기</th>
        </tr>
      </thead>
      <tbody>
        <tr>
            <td>작업</td>
            <td>작업</td>
            <td>작업</td>
            <td>작업</td>
            <td>TASKS_CURRENT<br>TASKS_DAILY_HISTORY<br>TASKS_EVENT</td>
        </tr>
      </tbody>
</table>
<table>
    <thead>
        <tr>
            <th>기본/외래 키</th>
            <th>유형</th>
            <th>관련 테이블</th>
            <th>관련 필드</th>
        </tr>
    </thead>
    <tbody>
        <tr>
             <td>APPROVALPROCESSID</td>
             <td>FK</td>
             <td>APPROVALPROCESSES_CURRENT</td>
             <td>APPROVALPROCESSID</td>
        </tr>
        <tr>
             <td>ASSIGNEDTOID</td>
             <td>FK</td>
             <td>USERS_CURRENT</td>
             <td>사용자 ID</td>
        </tr>
        <tr>
             <td>빌링레코디드</td>
             <td>FK</td>
             <td>BILLINGRECORDS_CURRENT</td>
             <td>빌링레코디드</td>
        </tr>
        <tr>
             <td>범주 ID</td>
             <td>FK</td>
             <td>CATEGORS_CURRENT</td>
             <td>범주 ID</td>
        </tr>
        <tr>
             <td>CONVERTEDOPTASKID</td>
             <td>FK</td>
             <td>OPTASKS_CURRENT</td>
             <td>OPTASKID</td>
        </tr>
        <tr>
             <td>CONVERTEDOPTASKORIGINATORID</td>
             <td>FK</td>
             <td>USERS_CURRENT</td>
             <td>사용자 ID</td>
        </tr>
        <tr>
             <td>CURRENTAPPROVALSTEPID</td>
             <td>FK</td>
             <td>APPROVALSTEPS_CURRENT</td>
             <td>승인스테피드</td>
        </tr>
        <tr>
             <td>ENTEREDBYID</td>
             <td>FK</td>
             <td>USERS_CURRENT</td>
             <td>사용자 ID</td>
        </tr>
        <tr>
             <td>EXCHANGERATEID</td>
             <td>FK</td>
             <td>EXCHANGE_CURRENT</td>
             <td>EXCHANGERATEID</td>
        </tr>
        <tr>
             <td>GROUPID</td>
             <td>FK</td>
             <td>GROUPS_CURRENT</td>
             <td>GROUPID</td>
        </tr>
        <tr>
             <td>ITERATIONID</td>
             <td>FK</td>
             <td>ITERATIONS_CURRENT</td>
             <td>ITERATIONID</td>
        </tr>
        <tr>
             <td>칸반보드</td>
             <td>-</td>
             <td colspan="2">칸반 보드 테이블은 현재 지원되지 않습니다.</td>
        </tr>
        <tr>
             <td>LASTCONDITIONNOTEID</td>
             <td>FK</td>
             <td>NOTES_CURRENT</td>
             <td>NOTEID</td>
        </tr>
        <tr>
             <td>LASTNOTEID</td>
             <td>FK</td>
             <td>NOTES_CURRENT</td>
             <td>NOTEID</td>
        </tr>
        <tr>
             <td>LASTUPDATEDBYID</td>
             <td>FK</td>
             <td>USERS_CURRENT</td>
             <td>사용자 ID</td>
        </tr>
        <tr>
             <td>마일스톤ID</td>
             <td>FK</td>
             <td>마일스톤_현재</td>
             <td>마일스톤ID</td>
        </tr>
        <tr>
             <td>괄호 ID</td>
             <td>FK</td>
             <td>TASKS_CURRENT</td>
             <td>TASKID</td>
        </tr>
        <tr>
             <td>PROJECTID</td>
             <td>FK</td>
             <td>PROJECTS_CURRENT</td>
             <td>PROJECTID</td>
        </tr>
        <tr>
             <td>재귀결핵-</td>
             <td>-</td>
             <td colspan="2">반복 규칙 테이블은 현재 지원되지 않습니다.</td>
        </tr>
        <tr>
             <td>REJECTIONISSUEID</td>
             <td>FK</td>
             <td>OPTASKS_CURRENT</td>
             <td>OPTASKID</td>
        </tr>
        <tr>
             <td>RESERVEDTIMEID</td>
             <td>FK</td>
             <td>RESERVEDTIMES_CURRENT</td>
             <td>RESERVEDTIMEID</td>
        </tr>
        <tr>
             <td>장미모양-</td>
             <td>FK</td>
             <td>ROLES_CURRENT</td>
             <td>장미모양-</td>
        </tr>
        <tr>
             <td>SUBMITTEDBYID</td>
             <td>FK</td>
             <td>USERS_CURRENT</td>
             <td>SUBMITTEDBYID</td>
        </tr>
        <tr>
             <td>SYSID</td>
             <td>-</td>
             <td colspan="2">관계가 아닙니다. 내부 응용 프로그램 용도로 사용됩니다.</td>
        </tr>
        <tr>
             <td>TASKID</td>
             <td>PK</td>
             <td>-</td>
             <td>-</td>
        </tr>
        <tr>
             <td>티미드</td>
             <td>FK</td>
             <td>TEAMS_CURRENT</td>
             <td>티미드</td>
        </tr>
        <tr>
             <td>TEMPLATETASKID</td>
             <td>FK</td>
             <td>TEMPLATETASKS_CURRENT</td>
             <td>TEMPLATETASKID</td>
        </tr>
    </tbody>
</table>

### 작업 전임 작업

<table>
    <thead>
        <tr>
            <th>Workfront 엔티티 이름</th>
            <th>인터페이스 참조</th>
            <th>API 참조</th>
            <th>API 레이블</th>
            <th>데이터 레이크 보기</th>
        </tr>
      </thead>
      <tbody>
        <tr>
            <td>작업 전임 작업</td>
            <td>전임 작업</td>
            <td>PRED</td>
            <td>전임 작업</td>
            <td>PREDECESSORS_CURRENT<br>PREDECESSORS_DAILY_HISTORY<br>PREDECESSORS_EVENT</td>
        </tr>
      </tbody>
</table>
<table>
    <thead>
        <tr>
            <th>기본/외래 키</th>
            <th>유형</th>
            <th>관련 테이블</th>
            <th>관련 필드</th>
        </tr>
    </thead>
    <tbody>
        <tr>
             <td>ID</td>
             <td>PK</td>
             <td>-</td>
             <td>-</td>
        </tr>
        <tr>
             <td>PREDECESSORID</td>
             <td>FK</td>
             <td>TASKS_CURRENT</td>
             <td>TASKID</td>
        </tr>
        <tr>
             <td>SUCCESSORID</td>
             <td>FK</td>
             <td>TASKS_CURRENT</td>
             <td>TASKID</td>
        </tr>
        <tr>
             <td>SYSID</td>
             <td>-</td>
             <td colspan="2">관계가 아닙니다. 내부 응용 프로그램 용도로 사용됩니다.</td>
        </tr>
    </tbody>
</table>

### 팀

<table>
    <thead>
        <tr>
            <th>Workfront 엔티티 이름</th>
            <th>인터페이스 참조</th>
            <th>API 참조</th>
            <th>API 레이블</th>
            <th>데이터 레이크 보기</th>
        </tr>
      </thead>
      <tbody>
        <tr>
            <td>팀</td>
            <td>팀</td>
            <td>TEAOB</td>
            <td>팀</td>
            <td>TEAMS_CURRENT<br>TEAMS_DAILY_HISTORY<br>TEAMS_EVENT</td>
        </tr>
      </tbody>
</table>
<table>
    <thead>
        <tr>
            <th>기본/외래 키</th>
            <th>유형</th>
            <th>관련 테이블</th>
            <th>관련 필드</th>
        </tr>
    </thead>
    <tbody>
        <tr>
             <td>ENTEREDBYID</td>
             <td>FK</td>
             <td>USERS_CURRENT</td>
             <td>사용자 ID</td>
        </tr>
        <tr>
             <td>GROUPID</td>
             <td>FK</td>
             <td>GROUPS_CURRENT</td>
             <td>GROUPID</td>
        </tr>
        <tr>
             <td>LAYOUTTEMPLATEID</td>
             <td>-</td>
             <td colspan="2">레이아웃 템플릿 테이블은 지원되지 않습니다.</td>
        </tr>
        <tr>
             <td>MYWORKVIEWID</td>
             <td>FK</td>
             <td>UIVIEWS_CURRENT</td>
             <td>UIVIEWID</td>
        </tr>
        <tr>
             <td>소유자 ID</td>
             <td>FK</td>
             <td>USERS_CURRENT</td>
             <td>사용자 ID</td>
        </tr>
        <tr>
             <td>REQUESTSVIEWID</td>
             <td>FK</td>
             <td>UIVIEWS_CURRENT</td>
             <td>UIVIEWID</td>
        </tr>
        <tr>
             <td>예약 ID</td>
             <td>FK</td>
             <td>SCHEDULES_CURRENT</td>
             <td>예약 ID</td>
        </tr>
        <tr>
             <td>티미드</td>
             <td>PK</td>
             <td>-</td>
             <td>-</td>
        </tr>
        <tr>
             <td>SYSID</td>
             <td>-</td>
             <td colspan="2">관계가 아닙니다. 내부 응용 프로그램 용도로 사용됩니다.</td>
        </tr>
        <tr>
             <td>UITEMPLATEID</td>
             <td>FK</td>
             <td>UITEMPLATES_CURRENT</td>
             <td>UITEMPLATEID</td>
        </tr>
    </tbody>
</table>

### 팀원

<table>
    <thead>
        <tr>
            <th>Workfront 엔티티 이름</th>
            <th>인터페이스 참조</th>
            <th>API 참조</th>
            <th>API 레이블</th>
            <th>데이터 레이크 보기</th>
        </tr>
      </thead>
      <tbody>
        <tr>
            <td>팀원</td>
            <td>기타 팀, 팀원</td>
            <td>TEAMMB</td>
            <td>팀원</td>
            <td>TEAMMEMBERS_CURRENT<br>TEAMMEMBERS_DAILY_HISTORY<br>TEAMMEMBERS_EVENT</td>
        </tr>
      </tbody>
</table>
<table>
    <thead>
        <tr>
            <th>기본/외래 키</th>
            <th>유형</th>
            <th>관련 테이블</th>
            <th>관련 필드</th>
        </tr>
    </thead>
    <tbody>
        <tr>
             <td>SYSID</td>
             <td>-</td>
             <td colspan="2">관계가 아닙니다. 내부 응용 프로그램 용도로 사용됩니다.</td>
        </tr>
        <tr>
             <td>티미드</td>
             <td>FK</td>
             <td>TEAMS_CURRENT</td>
             <td>티미드</td>
        </tr>
        <tr>
             <td>TEAMMEMBERID</td>
             <td>PK</td>
             <td>-</td>
             <td>-</td>
        </tr>
        <tr>
             <td>사용자 ID</td>
             <td>FK</td>
             <td>USERS_CURRENT</td>
             <td>사용자 ID</td>
        </tr>
    </tbody>
</table>

### 팀원 역할

<table>
    <thead>
        <tr>
            <th>Workfront 엔티티 이름</th>
            <th>인터페이스 참조</th>
            <th>API 참조</th>
            <th>API 레이블</th>
            <th>데이터 레이크 보기</th>
        </tr>
      </thead>
      <tbody>
        <tr>
            <td>팀원 역할</td>
            <td>팀원 역할</td>
            <td>팀</td>
            <td>팀원 역할</td>
            <td>TEAMMEMBERROLES_CURRENT<br>TEAMMEMBERROLES_DAILY_HISTORY<br>TEAMMEMBERROLES_EVENT</td>
        </tr>
      </tbody>
</table>
<table>
    <thead>
        <tr>
            <th>기본/외래 키</th>
            <th>유형</th>
            <th>관련 테이블</th>
            <th>관련 필드</th>
        </tr>
    </thead>
    <tbody>
        <tr>
             <td>장미모양-</td>
             <td>FK</td>
             <td>ROLES_CURRENT</td>
             <td>장미모양-</td>
        </tr>
        <tr>
             <td>SYSID</td>
             <td>-</td>
             <td colspan="2">관계가 아닙니다. 내부 응용 프로그램 용도로 사용됩니다.</td>
        </tr>
        <tr>
             <td>티미드</td>
             <td>FK</td>
             <td>TEAMS_CURRENT</td>
             <td>티미드</td>
        </tr>
        <tr>
             <td>TEAMMEMBERROLEID</td>
             <td>PK</td>
             <td>-</td>
             <td>-</td>
        </tr>
        <tr>
             <td>사용자 ID</td>
             <td>FK</td>
             <td>USERS_CURRENT</td>
             <td>사용자 ID</td>
        </tr>
    </tbody>
</table>

### 템플릿

<table>
    <thead>
        <tr>
            <th>Workfront 엔티티 이름</th>
            <th>인터페이스 참조</th>
            <th>API 참조</th>
            <th>API 레이블</th>
            <th>데이터 레이크 보기</th>
        </tr>
      </thead>
      <tbody>
        <tr>
            <td>템플릿</td>
            <td>템플릿, 프로젝트 템플릿</td>
            <td>템플릿</td>
            <td>템플릿</td>
            <td>TEMPLATES_CURRENT<br>TEMPLATES_DAILY_HISTORY<br>TEMPLATES_EVENT</td>
        </tr>
      </tbody>
</table>
<table>
    <thead>
        <tr>
            <th>기본/외래 키</th>
            <th>유형</th>
            <th>관련 테이블</th>
            <th>관련 필드</th>
        </tr>
    </thead>
    <tbody>
        <tr>
             <td>APPROVALPROCESSID</td>
             <td>FK</td>
             <td>APPROVALPROCESSES_CURRENT</td>
             <td>APPROVALPROCESSID</td>
        </tr>
        <tr>
             <td>범주 ID</td>
             <td>FK</td>
             <td>CATEGORS_CURRENT</td>
             <td>범주 ID</td>
        </tr>
        <tr>
             <td>COMPANYID</td>
             <td>FK</td>
             <td>COMPANIES_CURRENT</td>
             <td>COMPANYID</td>
        </tr>
        <tr>
             <td>DELIVERABLESCORECARDID</td>
             <td>-</td>
             <td colspan="2">결과물 스코어카드 테이블은 현재 지원되지 않습니다.</td>
        </tr>
        <tr>
             <td>ENTEREDBYID</td>
             <td>FK</td>
             <td>USERS_CURRENT</td>
             <td>사용자 ID</td>
        </tr>
        <tr>
             <td>GROUPID</td>
             <td>FK</td>
             <td>GROUPS_CURRENT</td>
             <td>GROUPID</td>
        </tr>
        <tr>
             <td>LASTNOTEID</td>
             <td>FK</td>
             <td>NOTES_CURRENT</td>
             <td>NOTEID</td>
        </tr>
        <tr>
             <td>LASTUPDATEDBYID</td>
             <td>FK</td>
             <td>USERS_CURRENT</td>
             <td>사용자 ID</td>
        </tr>
        <tr>
             <td>마일스톤 경로 ID</td>
             <td>FK</td>
             <td>MILESTONEPATHS_CURRENT</td>
             <td>마일스톤 경로 ID</td>
        </tr>
        <tr>
             <td>소유자 ID</td>
             <td>FK</td>
             <td>USERS_CURRENT</td>
             <td>사용자 ID</td>
        </tr>
        <tr>
             <td>PRIVATERATECARDID</td>
             <td>FK</td>
             <td>RATECARD_CURRENT</td>
             <td>RATECARDID</td>
        </tr>
        <tr>
             <td>PROGRAMID</td>
             <td>FK</td>
             <td>PROGRAMS_CURRENT</td>
             <td>PROGRAMID</td>
        </tr>
        <tr>
             <td>QUEUEDEFID</td>
             <td>-</td>
             <td colspan="2">대기열 정의 테이블은 현재 지원되지 않습니다.</td>
        </tr>
        <tr>
             <td>예약 ID</td>
             <td>FK</td>
             <td>SCHEDULES_CURRENT</td>
             <td>예약 ID</td>
        </tr>
        <tr>
             <td>SYSID</td>
             <td>-</td>
             <td colspan="2">관계가 아닙니다. 내부 응용 프로그램 용도로 사용됩니다.</td>
        </tr>
        <tr>
             <td>티미드</td>
             <td>FK</td>
             <td>TEAMS_CURRENT</td>
             <td>티미드</td>
        </tr>
        <tr>
             <td>TEMPLATEID</td>
             <td>PK</td>
             <td>-</td>
             <td>-</td>
        </tr>
    </tbody>
</table>

### 템플릿 작업 할당

<table>
    <thead>
        <tr>
            <th>Workfront 엔티티 이름</th>
            <th>인터페이스 참조</th>
            <th>API 참조</th>
            <th>API 레이블</th>
            <th>데이터 레이크 보기</th>
        </tr>
      </thead>
      <tbody>
        <tr>
            <td>템플릿 작업 할당</td>
            <td>템플릿 할당</td>
            <td>작업</td>
            <td>템플릿 할당</td>
            <td>TEMPLATEASSIGNMENTS_CURRENT<br>TEMPLATEASSIGNMENTS_DAILY_HISTORY<br>TEMPLATEASSIGNMENTS_EVENT</td>
        </tr>
      </tbody>
</table>
<table>
    <thead>
        <tr>
            <th>기본/외래 키</th>
            <th>유형</th>
            <th>관련 테이블</th>
            <th>관련 필드</th>
        </tr>
    </thead>
    <tbody>
        <tr>
             <td>ASSIGNEDTOID</td>
             <td>FK</td>
             <td>USERS_CURRENT</td>
             <td>사용자 ID</td>
        </tr>
        <tr>
             <td>범주 ID</td>
             <td>FK</td>
             <td>CATEGORS_CURRENT</td>
             <td>범주 ID</td>
        </tr>
        <tr>
             <td>LASTUPDATEDBYID</td>
             <td>FK</td>
             <td>USERS_CURRENT</td>
             <td>사용자 ID</td>
        </tr>
        <tr>
             <td>OBJID</td>
             <td>FK</td>
             <td>변수, OBJCODE 기반</td>
             <td>OBJCODE 필드에서 식별된 객체의 기본 키/ID</td>
        </tr>
        <tr>
             <td>장미모양-</td>
             <td>FK</td>
             <td>ROLES_CURRENT</td>
             <td>장미모양-</td>
        </tr>
        <tr>
             <td>SYSID</td>
             <td>-</td>
             <td colspan="2">관계가 아닙니다. 내부 응용 프로그램 용도로 사용됩니다.</td>
        </tr>
        <tr>
             <td>티미드</td>
             <td>FK</td>
             <td>TEAMS_CURRENT</td>
             <td>티미드</td>
        </tr>
        <tr>
             <td>TEAMTIMELINEABLEID</td>
             <td>-</td>
             <td colspan="2">팀 타임라인 가능 테이블은 현재 지원되지 않습니다.</td>
        </tr>
        <tr>
             <td>TEMPLATEASSIGNMENTID</td>
             <td>PK</td>
             <td>-</td>
             <td>-</td>
        </tr>
        <tr>
             <td>TEMPLATETASKID</td>
             <td>FK</td>
             <td>TEMPLATETASKS_CURRENT</td>
             <td>TEMPLATETASKID</td>
        </tr>
    </tbody>
</table>

### 템플릿 작업

<table>
    <thead>
        <tr>
            <th>Workfront 엔티티 이름</th>
            <th>인터페이스 참조</th>
            <th>API 참조</th>
            <th>API 레이블</th>
            <th>데이터 레이크 보기</th>
        </tr>
      </thead>
      <tbody>
        <tr>
            <td>템플릿 작업</td>
            <td>템플릿 작업</td>
            <td>TTSK</td>
            <td>템플릿 작업</td>
            <td>TEMPLATETASKS_CURRENT<br>TEMPLATETASKS_DAILY_HISTORY<br>TEMPLATETASKS_EVENT</td>
        </tr>
      </tbody>
</table>
<table>
    <thead>
        <tr>
            <th>기본/외래 키</th>
            <th>유형</th>
            <th>관련 테이블</th>
            <th>관련 필드</th>
        </tr>
    </thead>
    <tbody>
        <tr>
             <td>APPROVALPROCESSID</td>
             <td>FK</td>
             <td>APPROVALPROCESSES_CURRENT</td>
             <td>APPROVALPROCESSID</td>
        </tr>
        <tr>
             <td>ASSIGNEDTOID</td>
             <td>FK</td>
             <td>USERS_CURRENT</td>
             <td>사용자 ID</td>
        </tr>
        <tr>
             <td>범주 ID</td>
             <td>FK</td>
             <td>CATEGORS_CURRENT</td>
             <td>범주 ID</td>
        </tr>
        <tr>
             <td>ENTEREDBYID</td>
             <td>FK</td>
             <td>USERS_CURRENT</td>
             <td>사용자 ID</td>
        </tr>
        <tr>
             <td>EXCHANGERATEID</td>
             <td>FK</td>
             <td>EXCHANGE_CURRENT</td>
             <td>EXCHANGERATEID</td>
        </tr>
        <tr>
             <td>LASTNOTEID</td>
             <td>FK</td>
             <td>NOTES_CURRENT</td>
             <td>NOTEID</td>
        </tr>
        <tr>
             <td>LASTUPDATEDBYID</td>
             <td>FK</td>
             <td>USERS_CURRENT</td>
             <td>사용자 ID</td>
        </tr>
        <tr>
             <td>마일스톤ID</td>
             <td>FK</td>
             <td>마일스톤_현재</td>
             <td>마일스톤ID</td>
        </tr>
        <tr>
             <td>괄호 ID</td>
             <td>FK</td>
             <td>TEMPLATETASKS_CURRENT</td>
             <td>TEMPLATETASKID</td>
        </tr>
        <tr>
             <td>재귀결핵-</td>
             <td>-</td>
             <td colspan="2">반복 규칙 테이블은 현재 지원되지 않습니다.</td>
        </tr>
        <tr>
             <td>장미모양-</td>
             <td>FK</td>
             <td>ROLES_CURRENT</td>
             <td>장미모양-</td>
        </tr>
        <tr>
             <td>SYSID</td>
             <td>-</td>
             <td colspan="2">관계가 아닙니다. 내부 응용 프로그램 용도로 사용됩니다.</td>
        </tr>
        <tr>
             <td>티미드</td>
             <td>FK</td>
             <td>TEAMS_CURRENT</td>
             <td>티미드</td>
        </tr>
        <tr>
             <td>TEAMTIMELINEABLEID</td>
             <td>-</td>
             <td colspan="2">팀 타임라인 가능 테이블은 현재 지원되지 않습니다.</td>
        </tr>
        <tr>
             <td>TEMPLATEID</td>
             <td>FK</td>
             <td>TEMPLATES_CURRENT</td>
             <td>TEMPLATEID</td>
        </tr>
        <tr>
             <td>TEMPLATETASKID</td>
             <td>PK</td>
             <td>-</td>
             <td>-</td>
        </tr>
    </tbody>
</table>

### 템플릿 작업 전임 작업

<table>
    <thead>
        <tr>
            <th>Workfront 엔티티 이름</th>
            <th>인터페이스 참조</th>
            <th>API 참조</th>
            <th>API 레이블</th>
            <th>데이터 레이크 보기</th>
        </tr>
      </thead>
      <tbody>
        <tr>
            <td>템플릿 작업 전임 작업</td>
            <td>템플릿 전임 작업</td>
            <td>TPRED</td>
            <td>전임 작업</td>
            <td>TEMPLATEPREDECESSORS_CURRENT<br>TEMPLATEPREDECESSORS_DAILY_HISTORY<br>TEMPLATEPREDECESSORS_EVENT</td>
        </tr>
      </tbody>
</table>
<table>
    <thead>
        <tr>
            <th>기본/외래 키</th>
            <th>유형</th>
            <th>관련 테이블</th>
            <th>관련 필드</th>
        </tr>
    </thead>
    <tbody>
        <tr>
             <td>PREDECESSORID</td>
             <td>FK</td>
             <td>TEMPLATETASKS_CURRENT</td>
             <td>TEMPLATETASKID</td>
        </tr>
        <tr>
             <td>SUCCESSORID</td>
             <td>FK</td>
             <td>TEMPLATETASKS_CURRENT</td>
             <td>TEMPLATETASKID</td>
        </tr>
        <tr>
             <td>TEMPLATEPREDECESSORID</td>
             <td>PK</td>
             <td>-</td>
             <td>-</td>
        </tr>
        <tr>
             <td>SYSID</td>
             <td>-</td>
             <td colspan="2">관계가 아닙니다. 내부 응용 프로그램 용도로 사용됩니다.</td>
        </tr>
    </tbody>
</table>

### 시간 단계별 KPI 통화

제한된 고객 가용성

<table>
    <thead>
        <tr>
            <th>Workfront 엔티티 이름</th>
            <th>인터페이스 참조</th>
            <th>API 참조</th>
            <th>API 레이블</th>
            <th>데이터 레이크 보기</th>
        </tr>
      </thead>
      <tbody>
        <tr>
            <td>시간 단계별 KPI 통화</td>
            <td>시간별 KPI</td>
            <td>TMPH</td>
            <td>TimePhasedKPI</td>
            <td>TIMEPHASED_CURRENCY_CURRENT<br>TIMEPHASED_CURRENCY_DAILY_HISTORY<br>TIMEPHASED_CURRENCY_EVENT</td>
        </tr>
      </tbody>
</table>
<table>
    <thead>
        <tr>
            <th>기본/외래 키</th>
            <th>유형</th>
            <th>관련 테이블</th>
            <th>관련 필드</th>
        </tr>
    </thead>
    <tbody>
        <tr>
             <td>ASSIGNMENTID</td>
             <td>FK</td>
             <td>ASSIGNMENTS_CURRENT</td>
             <td>ASSIGNMENTID</td>
        </tr>
        <tr>
             <td>GROUPID</td>
             <td>FK</td>
             <td>GROUPS_CURRENT</td>
             <td>GROUPID</td>
        </tr>
        <tr>
             <td>위치 ID</td>
             <td>FK</td>
             <td>CLASSIFIER_CURRENT</td>
             <td>분류자</td>
        </tr>
        <tr>
             <td>OPTASKID</td>
             <td>FK</td>
             <td>OPTASKS_CURRENT</td>
             <td>OPTASKID</td>
        </tr>
        <tr>
             <td>포트폴리오</td>
             <td>FK</td>
             <td>포트폴리오_현재</td>
             <td>포트폴리오</td>
        </tr>
        <tr>
             <td>PROGRAMID</td>
             <td>FK</td>
             <td>PROGRAMS_CURRENT</td>
             <td>PROGRAMID</td>
        </tr>
        <tr>
             <td>PROJECTID</td>
             <td>FK</td>
             <td>PROJECTS_CURRENT</td>
             <td>PROJECTID</td>
        </tr>
        <tr>
             <td>참조 ID</td>
             <td>FK</td>
             <td>변수, OBJCODE 기반</td>
             <td>OBJCODE 필드에서 식별된 객체의 기본 키/ID</td>
        </tr>
        <tr>
             <td>장미모양-</td>
             <td>FK</td>
             <td>ROLES_CURRENT</td>
             <td>장미모양-</td>
        </tr>
        <tr>
             <td>SCHEMAID</td>
             <td>FK</td>
             <td>곧 추가될 예정입니다.</td>
             <td>SCHEMAID</td>
        </tr>
        <tr>
             <td>SOURCETASKID</td>
             <td>FK</td>
             <td>TASKS_CURRENT</td>
             <td>TASKID</td>
        </tr>
        <tr>
             <td>SYSID</td>
             <td>-</td>
             <td colspan="2">관계가 아닙니다. 내부 응용 프로그램 용도로 사용됩니다.</td>
        </tr>
        <tr>
             <td>TASKID</td>
             <td>FK</td>
             <td>TASKS_CURRENT</td>
             <td>TASKID</td>
        </tr>
        <tr>
             <td>TIMEPHASEDCURRENCYID</td>
             <td>PK</td>
             <td>-</td>
             <td>-</td>
        </tr>
        <tr>
             <td>사용자 ID</td>
             <td>FK</td>
             <td>USERS_CURRENT</td>
             <td>사용자 ID</td>
        </tr>
    </tbody>
</table>

### 시간 단계별 KPI 기간

제한된 고객 가용성

<table>
    <thead>
        <tr>
            <th>Workfront 엔티티 이름</th>
            <th>인터페이스 참조</th>
            <th>API 참조</th>
            <th>API 레이블</th>
            <th>데이터 레이크 보기</th>
        </tr>
      </thead>
      <tbody>
        <tr>
            <td>시간 단계별 KPI 기간</td>
            <td>시간별 KPI</td>
            <td>TMPH</td>
            <td>TimePhasedKPI</td>
            <td>TIMEPHASED_DURATION_CURRENT<br>TIMEPHASED_DURATION_DAILY_HISTORY<br>TIMEPHASED_DURATION_EVENT</td>
        </tr>
      </tbody>
</table>
<table>
    <thead>
        <tr>
            <th>기본/외래 키</th>
            <th>유형</th>
            <th>관련 테이블</th>
            <th>관련 필드</th>
        </tr>
    </thead>
    <tbody>
        <tr>
             <td>ASSIGNMENTID</td>
             <td>FK</td>
             <td>ASSIGNMENTS_CURRENT</td>
             <td>ASSIGNMENTID</td>
        </tr>
        <tr>
             <td>GROUPID</td>
             <td>FK</td>
             <td>GROUPS_CURRENT</td>
             <td>GROUPID</td>
        </tr>
        <tr>
             <td>위치 ID</td>
             <td>FK</td>
             <td>CLASSIFIER_CURRENT</td>
             <td>분류자</td>
        </tr>
        <tr>
             <td>OPTASKID</td>
             <td>FK</td>
             <td>OPTASKS_CURRENT</td>
             <td>OPTASKID</td>
        </tr>
        <tr>
             <td>포트폴리오</td>
             <td>FK</td>
             <td>포트폴리오_현재</td>
             <td>포트폴리오</td>
        </tr>
        <tr>
             <td>PROGRAMID</td>
             <td>FK</td>
             <td>PROGRAMS_CURRENT</td>
             <td>PROGRAMID</td>
        </tr>
        <tr>
             <td>PROJECTID</td>
             <td>FK</td>
             <td>PROJECTS_CURRENT</td>
             <td>PROJECTID</td>
        </tr>
        <tr>
             <td>참조 ID</td>
             <td>FK</td>
             <td>변수, OBJCODE 기반</td>
             <td>OBJCODE 필드에서 식별된 객체의 기본 키/ID</td>
        </tr>
        <tr>
             <td>장미모양-</td>
             <td>FK</td>
             <td>ROLES_CURRENT</td>
             <td>장미모양-</td>
        </tr>
        <tr>
             <td>SCHEMAID</td>
             <td>FK</td>
             <td>곧 추가될 예정입니다.</td>
             <td>SCHEMAID</td>
        </tr>
        <tr>
             <td>SOURCETASKID</td>
             <td>FK</td>
             <td>TASKS_CURRENT</td>
             <td>TASKID</td>
        </tr>
        <tr>
             <td>SYSID</td>
             <td>-</td>
             <td colspan="2">관계가 아닙니다. 내부 응용 프로그램 용도로 사용됩니다.</td>
        </tr>
        <tr>
             <td>TASKID</td>
             <td>FK</td>
             <td>TASKS_CURRENT</td>
             <td>TASKID</td>
        </tr>
        <tr>
             <td>TIMEPHASEDDURATIONID</td>
             <td>PK</td>
             <td>-</td>
             <td>-</td>
        </tr>
        <tr>
             <td>사용자 ID</td>
             <td>FK</td>
             <td>USERS_CURRENT</td>
             <td>사용자 ID</td>
        </tr>
    </tbody>
</table>

### 타임시트

<table>
    <thead>
        <tr>
            <th>Workfront 엔티티 이름</th>
            <th>인터페이스 참조</th>
            <th>API 참조</th>
            <th>API 레이블</th>
            <th>데이터 레이크 보기</th>
        </tr>
      </thead>
      <tbody>
        <tr>
            <td>타임시트</td>
            <td>타임시트</td>
            <td>체트</td>
            <td>타임시트</td>
            <td>TIMESHEETS_CURRENT<br>TIMESHEETS_DAILY_HISTORY<br>TIMESHEETS_EVENT</td>
        </tr>
      </tbody>
</table>
<table>
    <thead>
        <tr>
            <th>기본/외래 키</th>
            <th>유형</th>
            <th>관련 테이블</th>
            <th>관련 필드</th>
        </tr>
    </thead>
    <tbody>
        <tr>
             <td>승인자 ID</td>
             <td>FK</td>
             <td>USERS_CURRENT</td>
             <td>사용자 ID</td>
        </tr>
        <tr>
             <td>LASTNOTEID</td>
             <td>FK</td>
             <td>NOTES_CURRENT</td>
             <td>NOTEID</td>
        </tr>
        <tr>
             <td>LASTUPDATEDBYID</td>
             <td>FK</td>
             <td>USERS_CURRENT</td>
             <td>사용자 ID</td>
        </tr>
        <tr>
             <td>SYSID</td>
             <td>-</td>
             <td colspan="2">관계가 아닙니다. 내부 응용 프로그램 용도로 사용됩니다.</td>
        </tr>
        <tr>
             <td>TIMESHEETID</td>
             <td>PK</td>
             <td>-</td>
             <td>-</td>
        </tr>
        <tr>
             <td>TIMESHEETPROFILEID</td>
             <td>FK</td>
             <td>TIMESHEETPROFILES_CURRENT</td>
             <td>TIMESHEETPROFILEID</td>
        </tr>
        <tr>
             <td>사용자 ID</td>
             <td>FK</td>
             <td>USERS_CURRENT</td>
             <td>사용자 ID</td>
        </tr>
    </tbody>
</table>

### 타임시트 프로필

<table>
    <thead>
        <tr>
            <th>Workfront 엔티티 이름</th>
            <th>인터페이스 참조</th>
            <th>API 참조</th>
            <th>API 레이블</th>
            <th>데이터 레이크 보기</th>
        </tr>
      </thead>
      <tbody>
        <tr>
            <td>타임시트 프로필</td>
            <td>타임시트 프로필</td>
            <td>TSPRO</td>
            <td>타임시트 프로필</td>
            <td>TIMESHEETPROFILES_CURRENT<br>TIMESHEETPROFILES_DAILY_HISTORY<br>TIMESHEETPROFILES_EVENT</td>
        </tr>
      </tbody>
</table>
<table>
    <thead>
        <tr>
            <th>기본/외래 키</th>
            <th>유형</th>
            <th>관련 테이블</th>
            <th>관련 필드</th>
        </tr>
    </thead>
    <tbody>
        <tr>
             <td>승인자 ID</td>
             <td>FK</td>
             <td>USERS_CURRENT</td>
             <td>사용자 ID</td>
        </tr>
        <tr>
             <td>ENTEREDBYID</td>
             <td>FK</td>
             <td>USERS_CURRENT</td>
             <td>사용자 ID</td>
        </tr>
        <tr>
             <td>GROUPID</td>
             <td>FK</td>
             <td>GROUPS_CURRENT</td>
             <td>GROUPID</td>
        </tr>
        <tr>
             <td>SYSID</td>
             <td>-</td>
             <td colspan="2">관계가 아닙니다. 내부 응용 프로그램 용도로 사용됩니다.</td>
        </tr>
        <tr>
             <td>TIMESHEETPROFILEID</td>
             <td>PK</td>
             <td>-</td>
             <td>-</td>
        </tr>
    </tbody>
</table>

### UI 필터

<table>
    <thead>
        <tr>
            <th>Workfront 엔티티 이름</th>
            <th>인터페이스 참조</th>
            <th>API 참조</th>
            <th>API 레이블</th>
            <th>데이터 레이크 보기</th>
        </tr>
      </thead>
      <tbody>
        <tr>
            <td>UI 필터</td>
            <td>필터</td>
            <td>UIFT</td>
            <td>필터</td>
            <td>UIFILTERS_CURRENT<br>UIFILTERS_DAILY_HISTORY<br>UIFILTERS_EVENT</td>
        </tr>
      </tbody>
</table>
<table>
    <thead>
        <tr>
            <th>기본/외래 키</th>
            <th>유형</th>
            <th>관련 테이블</th>
            <th>관련 필드</th>
        </tr>
    </thead>
    <tbody>
        <tr>
             <td>APPGLOBALID</td>
             <td>-</td>
             <td colspan="2">관계가 아닙니다. 내부 응용 프로그램 용도로 사용됩니다.</td>
        </tr>
        <tr>
             <td>ENTEREDBYID</td>
             <td>FK</td>
             <td>USERS_CURRENT</td>
             <td>사용자 ID</td>
        </tr>
        <tr>
             <td>LASTUPDATEDBYID</td>
             <td>FK</td>
             <td>USERS_CURRENT</td>
             <td>사용자 ID</td>
        </tr>
        <tr>
             <td>OBJID</td>
             <td>FK</td>
             <td>변수, OBJCODE 기반</td>
             <td>OBJCODE 필드에서 식별된 객체의 기본 키/ID</td>
        </tr>
        <tr>
             <td>PREFERENCEID</td>
             <td>FK</td>
             <td>PREFERENCES_CURRENT</td>
             <td>PREFERENCEID</td>
        </tr>
        <tr>
             <td>SYSID</td>
             <td>-</td>
             <td colspan="2">관계가 아닙니다. 내부 응용 프로그램 용도로 사용됩니다.</td>
        </tr>
        <tr>
             <td>우이필테르</td>
             <td>PK</td>
             <td>-</td>
             <td>-</td>
        </tr>
    </tbody>
</table>

### UI 그룹 기준

<table>
    <thead>
        <tr>
            <th>Workfront 엔티티 이름</th>
            <th>인터페이스 참조</th>
            <th>API 참조</th>
            <th>API 레이블</th>
            <th>데이터 레이크 보기</th>
        </tr>
      </thead>
      <tbody>
        <tr>
            <td>UI 그룹 기준</td>
            <td>그룹화</td>
            <td>UIGB</td>
            <td>그룹화</td>
            <td>UIGROUPYS_CURRENT<br>UIGROUPYS_DAILY_HISTORY<br>UIGROPBYS_EVENT</td>
        </tr>
      </tbody>
</table>
<table>
    <thead>
        <tr>
            <th>기본/외래 키</th>
            <th>유형</th>
            <th>관련 테이블</th>
            <th>관련 필드</th>
        </tr>
    </thead>
    <tbody>
        <tr>
             <td>APPGLOBALID</td>
             <td>-</td>
             <td colspan="2">관계가 아닙니다. 내부 응용 프로그램 용도로 사용됩니다.</td>
        </tr>
        <tr>
             <td>ENTEREDBYID</td>
             <td>FK</td>
             <td>USERS_CURRENT</td>
             <td>사용자 ID</td>
        </tr>
        <tr>
             <td>LASTUPDATEDBYID</td>
             <td>FK</td>
             <td>USERS_CURRENT</td>
             <td>사용자 ID</td>
        </tr>
        <tr>
             <td>OBJID</td>
             <td>FK</td>
             <td>변수, OBJCODE 기반</td>
             <td>OBJCODE 필드에서 식별된 객체의 기본 키/ID</td>
        </tr>
        <tr>
             <td>PREFERENCEID</td>
             <td>FK</td>
             <td>PREFERENCES_CURRENT</td>
             <td>PREFERENCEID</td>
        </tr>
        <tr>
             <td>SYSID</td>
             <td>-</td>
             <td colspan="2">관계가 아닙니다. 내부 응용 프로그램 용도로 사용됩니다.</td>
        </tr>
        <tr>
             <td>UIGROUPBYID</td>
             <td>PK</td>
             <td>-</td>
             <td>-</td>
        </tr>
    </tbody>
</table>

### UI 템플릿

<table>
    <thead>
        <tr>
            <th>Workfront 엔티티 이름</th>
            <th>인터페이스 참조</th>
            <th>API 참조</th>
            <th>API 레이블</th>
            <th>데이터 레이크 보기</th>
        </tr>
      </thead>
      <tbody>
        <tr>
            <td>UI 템플릿</td>
            <td>레이아웃 템플릿</td>
            <td>UITMPL</td>
            <td>레이아웃 템플릿</td>
            <td>UITEMPLATES_CURRENT<br>UITEMPLATES_DAILY_HISTORY<br>UITEMPLATES_EVENT</td>
        </tr>
      </tbody>
</table>
<table>
    <thead>
        <tr>
            <th>기본/외래 키</th>
            <th>유형</th>
            <th>관련 테이블</th>
            <th>관련 필드</th>
        </tr>
    </thead>
    <tbody>
        <tr>
             <td>ENTEREDBYID</td>
             <td>FK</td>
             <td>USERS_CURRENT</td>
             <td>사용자 ID</td>
        </tr>
        <tr>
             <td>GROUPID</td>
             <td>FK</td>
             <td>GROUPS_CURRENT</td>
             <td>GROUPID</td>
        </tr>
        <tr>
             <td>LASTUPDATEDBYID</td>
             <td>FK</td>
             <td>USERS_CURRENT</td>
             <td>사용자 ID</td>
        </tr>
        <tr>
             <td>SYSID</td>
             <td>-</td>
             <td colspan="2">관계가 아닙니다. 내부 응용 프로그램 용도로 사용됩니다.</td>
        </tr>
        <tr>
             <td>UITEMPLATEID</td>
             <td>PK</td>
             <td>-</td>
             <td>-</td>
        </tr>
    </tbody>
</table>

### UI 보기

<table>
    <thead>
        <tr>
            <th>Workfront 엔티티 이름</th>
            <th>인터페이스 참조</th>
            <th>API 참조</th>
            <th>API 레이블</th>
            <th>데이터 레이크 보기</th>
        </tr>
      </thead>
      <tbody>
        <tr>
            <td>UI 보기</td>
            <td>보기</td>
            <td>UIVIEW</td>
            <td>보기</td>
            <td>UIVIEWS_CURRENT<br>UIVIEWS_DAILY_HISTORY<br>UIVIEWS_EVENT</td>
        </tr>
      </tbody>
</table>
<table>
    <thead>
        <tr>
            <th>기본/외래 키</th>
            <th>유형</th>
            <th>관련 테이블</th>
            <th>관련 필드</th>
        </tr>
    </thead>
    <tbody>
        <tr>
             <td>APPGLOBALID</td>
             <td>-</td>
             <td colspan="2">관계가 아닙니다. 내부 응용 프로그램 용도로 사용됩니다.</td>
        </tr>
        <tr>
             <td>ENTEREDBYID</td>
             <td>FK</td>
             <td>USERS_CURRENT</td>
             <td>사용자 ID</td>
        </tr>
        <tr>
             <td>LASTUPDATEDBYID</td>
             <td>FK</td>
             <td>USERS_CURRENT</td>
             <td>사용자 ID</td>
        </tr>
        <tr>
             <td>OBJID</td>
             <td>FK</td>
             <td>변수, OBJCODE 기반</td>
             <td>OBJCODE 필드에서 식별된 객체의 기본 키/ID</td>
        </tr>
        <tr>
             <td>PREFERENCEID</td>
             <td>FK</td>
             <td>PREFERENCES_CURRENT</td>
             <td>PREFERENCEID</td>
        </tr>
        <tr>
             <td>SYSID</td>
             <td>-</td>
             <td colspan="2">관계가 아닙니다. 내부 응용 프로그램 용도로 사용됩니다.</td>
        </tr>
        <tr>
             <td>UIVIEWID</td>
             <td>PK</td>
             <td>-</td>
             <td>-</td>
        </tr>
    </tbody>
</table>

### 사용자

<table>
    <thead>
        <tr>
            <th>Workfront 엔티티 이름</th>
            <th>인터페이스 참조</th>
            <th>API 참조</th>
            <th>API 레이블</th>
            <th>데이터 레이크 보기</th>
        </tr>
      </thead>
      <tbody>
        <tr>
            <td>사용자</td>
            <td>사용자</td>
            <td>사용자</td>
            <td>사용자</td>
            <td>USERS_CURRENT<br>USERS_DAILY_HISTORY<br>USERS_EVENT</td>
        </tr>
      </tbody>
</table>
<table>
    <thead>
        <tr>
            <th>기본/외래 키</th>
            <th>유형</th>
            <th>관련 테이블</th>
            <th>관련 필드</th>
        </tr>
    </thead>
    <tbody>
        <tr>
             <td>ACCESSLEVELID</td>
             <td>FK</td>
             <td>ACCESSLEVELS_CURRENT</td>
             <td>ACCESSLEVELID</td>
        </tr>
        <tr>
             <td>범주 ID</td>
             <td>FK</td>
             <td>CATEGORS_CURRENT</td>
             <td>범주 ID</td>
        </tr>
        <tr>
             <td>COMPANYID</td>
             <td>FK</td>
             <td>COMPANIES_CURRENT</td>
             <td>COMPANYID</td>
        </tr>
        <tr>
             <td>DEFAULTHOURTYPEID</td>
             <td>FK</td>
             <td>HOURTYPES_CURRENT</td>
             <td>HOURTYPEID</td>
        </tr>
        <tr>
             <td>DELEGATIONTOID</td>
             <td>FK</td>
             <td>USERS_CURRENT</td>
             <td>사용자 ID</td>
        </tr>
        <tr>
             <td>EAUTHUSERID</td>
             <td>-</td>
             <td colspan="2">관계가 아닙니다. 내부 응용 프로그램 용도로 사용됩니다.</td>
        </tr>
        <tr>
             <td>ENTEREDBYID</td>
             <td>FK</td>
             <td>USERS_CURRENT</td>
             <td>사용자 ID</td>
        </tr>
        <tr>
             <td>HOMEGROUPID</td>
             <td>FK</td>
             <td>GROUPS_CURRENT</td>
             <td>GROUPID</td>
        </tr>
        <tr>
             <td>홈메팀</td>
             <td>FK</td>
             <td>TEAMS_CURRENT</td>
             <td>티미드</td>
        </tr>
        <tr>
             <td>LASTENTEREDNOTEID</td>
             <td>FK</td>
             <td>NOTES_CURRENT</td>
             <td>NOTEID</td>
        </tr>
        <tr>
             <td>LASTUPDATEDBYID</td>
             <td>FK</td>
             <td>USERS_CURRENT</td>
             <td>사용자 ID</td>
        </tr>
        <tr>
             <td>LATESTUPDATENOTEID</td>
             <td>FK</td>
             <td>NOTES_CURRENT</td>
             <td>NOTEID</td>
        </tr>
        <tr>
             <td>LAYOUTTEMPLATEID</td>
             <td>-</td>
             <td colspan="2">레이아웃 템플릿 테이블은 지원되지 않습니다.</td>
        </tr>
        <tr>
             <td>MANAGERID</td>
             <td>FK</td>
             <td>USERS_CURRENT</td>
             <td>사용자 ID</td>
        </tr>
        <tr>
             <td>PORTALPROFILEID</td>
             <td>-</td>
             <td colspan="2">포털 프로필 테이블이 지원되지 않습니다.</td>
        </tr>
        <tr>
             <td>PREFUID</td>
             <td>-</td>
             <td colspan="2">관계가 아닙니다. 내부 응용 프로그램 용도로 사용됩니다.</td>
        </tr>
        <tr>
             <td>PRIVATERATECARDID</td>
             <td>FK</td>
             <td>RATECARD_CURRENT</td>
             <td>RATECARDID</td>
        </tr>
        <tr>
             <td>RESOURCEPOOLID</td>
             <td>FK</td>
             <td>RESOURCEPOOL_CURRENT</td>
             <td>RESOURCEPOOLID</td>
        </tr>
        <tr>
             <td>장미모양-</td>
             <td>FK</td>
             <td>ROLES_CURRENT</td>
             <td>장미모양-</td>
        </tr>
        <tr>
             <td>예약 ID</td>
             <td>FK</td>
             <td>SCHEDULES_CURRENT</td>
             <td>예약 ID</td>
        </tr>
        <tr>
             <td>SYSID</td>
             <td>-</td>
             <td colspan="2">관계가 아닙니다. 내부 응용 프로그램 용도로 사용됩니다.</td>
        </tr>
        <tr>
             <td>TIMESHEETPROFILEID</td>
             <td>FK</td>
             <td>TIMESHEETPROFILES_CURRENT</td>
             <td>TIMESHEETPROFILEID</td>
        </tr>
        <tr>
             <td>UITEMPLATEID</td>
             <td>FK</td>
             <td>UITEMPLATES_CURRENT</td>
             <td>UITEMPLATEID</td>
        </tr>
        <tr>
             <td>사용자 ID</td>
             <td>PK</td>
             <td>-</td>
             <td>-</td>
        </tr>
        <tr>
             <td>유무세리드</td>
             <td>-</td>
             <td colspan="2">관계가 아닙니다. 내부 응용 프로그램 용도로 사용됩니다.</td>
        </tr>
    </tbody>
</table>

### 사용자 위임

<table>
    <thead>
        <tr>
            <th>Workfront 엔티티 이름</th>
            <th>인터페이스 참조</th>
            <th>API 참조</th>
            <th>API 레이블</th>
            <th>데이터 레이크 보기</th>
        </tr>
      </thead>
      <tbody>
        <tr>
            <td>사용자 위임</td>
            <td>사용자 위임</td>
            <td>우르델</td>
            <td>사용자 위임</td>
            <td>USERDELEGATIONS_CURRENT<br>USERDELEGATIONS_DAILY_HISTORY<br>USERDELEGATIONS_EVENT</td>
        </tr>
      </tbody>
</table>
<table>
    <thead>
        <tr>
            <th>기본/외래 키</th>
            <th>유형</th>
            <th>관련 테이블</th>
            <th>관련 필드</th>
        </tr>
    </thead>
    <tbody>
        <tr>
             <td>프로무세라드</td>
             <td>FK</td>
             <td>USERS_CURRENT</td>
             <td>사용자 ID</td>
        </tr>
        <tr>
             <td>SYSID</td>
             <td>-</td>
             <td colspan="2">관계가 아닙니다. 내부 응용 프로그램 용도로 사용됩니다.</td>
        </tr>
        <tr>
             <td>TOUSERID</td>
             <td>FK</td>
             <td>USERS_CURRENT</td>
             <td>사용자 ID</td>
        </tr>
        <tr>
             <td>USERDELEGATIONID</td>
             <td>PK</td>
             <td>-</td>
             <td>-</td>
        </tr>
    </tbody>
</table>

### 사용자 그룹

<table>
    <thead>
        <tr>
            <th>Workfront 엔티티 이름</th>
            <th>인터페이스 참조</th>
            <th>API 참조</th>
            <th>API 레이블</th>
            <th>데이터 레이크 보기</th>
        </tr>
      </thead>
      <tbody>
        <tr>
            <td>사용자 그룹</td>
            <td>기타 그룹</td>
            <td>USRGPS</td>
            <td>사용자 그룹</td>
            <td>USERSGROUPS_CURRENT<br>USERSGROUPS_DAILY_HISTORY<br>USERSGROUPS_EVENT</td>
        </tr>
      </tbody>
</table>
<table>
    <thead>
        <tr>
            <th>기본/외래 키</th>
            <th>유형</th>
            <th>관련 테이블</th>
            <th>관련 필드</th>
        </tr>
    </thead>
    <tbody>
        <tr>
             <td>GROUPID</td>
             <td>FK</td>
             <td>GROUPS_CURRENT</td>
             <td>GROUPID</td>
        </tr>
        <tr>
             <td>SYSID</td>
             <td>-</td>
             <td colspan="2">관계가 아닙니다. 내부 응용 프로그램 용도로 사용됩니다.</td>
        </tr>
        <tr>
             <td>사용자 ID</td>
             <td>FK</td>
             <td>USERS_CURRENT</td>
             <td>사용자 ID</td>
        </tr>
        <tr>
             <td>USERSGROUPID</td>
             <td>PK</td>
             <td>-</td>
             <td>-</td>
        </tr>
    </tbody>
</table>

### 사용자 위치

<table>
    <thead>
        <tr>
            <th>Workfront 엔티티 이름</th>
            <th>인터페이스 참조</th>
            <th>API 참조</th>
            <th>API 레이블</th>
            <th>데이터 레이크 보기</th>
        </tr>
      </thead>
      <tbody>
        <tr>
            <td>사용자 위치</td>
            <td>사용자 위치</td>
            <td>USRLOC</td>
            <td>사용자 위치</td>
            <td>USERLOCATIONS_CURRENT<br>USERLOCATIONS_DAILY_HISTORY<br>USERLOCATIONS_EVENT</td>
        </tr>
      </tbody>
</table>
<table>
    <thead>
        <tr>
            <th>기본/외래 키</th>
            <th>유형</th>
            <th>관련 테이블</th>
            <th>관련 필드</th>
        </tr>
    </thead>
    <tbody>
        <tr>
             <td>분류자</td>
             <td>FK</td>
             <td>CLASSIFIER_CURRENT</td>
             <td>분류자</td>
        </tr>
        <tr>
             <td>SYSID</td>
             <td>-</td>
             <td colspan="2">관계가 아닙니다. 내부 응용 프로그램 용도로 사용됩니다.</td>
        </tr>
        <tr>
             <td>사용자 ID</td>
             <td>FK</td>
             <td>USERS_CURRENT</td>
             <td>사용자 ID</td>
        </tr>
        <tr>
             <td>USERLOCATIONID</td>
             <td>PK</td>
             <td>-</td>
             <td>-</td>
        </tr>
    </tbody>
</table>

### 사용자 역할

<table>
    <thead>
        <tr>
            <th>Workfront 엔티티 이름</th>
            <th>인터페이스 참조</th>
            <th>API 참조</th>
            <th>API 레이블</th>
            <th>데이터 레이크 보기</th>
        </tr>
      </thead>
      <tbody>
        <tr>
            <td>사용자 역할</td>
            <td>기타 역할</td>
            <td>USRROL</td>
            <td>사용자 역할</td>
            <td>USERSROLES_CURRENT<br>USERSROLES_DAILY_HISTORY<br>USERSROLES_EVENT</td>
        </tr>
      </tbody>
</table>
<table>
    <thead>
        <tr>
            <th>기본/외래 키</th>
            <th>유형</th>
            <th>관련 테이블</th>
            <th>관련 필드</th>
        </tr>
    </thead>
    <tbody>
        <tr>
             <td>장미모양-</td>
             <td>FK</td>
             <td>ROLES_CURRENT</td>
             <td>장미모양-</td>
        </tr>
        <tr>
             <td>SYSID</td>
             <td>-</td>
             <td colspan="2">관계가 아닙니다. 내부 응용 프로그램 용도로 사용됩니다.</td>
        </tr>
        <tr>
             <td>사용자 ID</td>
             <td>FK</td>
             <td>USERS_CURRENT</td>
             <td>사용자 ID</td>
        </tr>
        <tr>
             <td>USERROLESETID</td>
             <td>FK</td>
             <td>USERROLESET_CURRENT</td>
             <td>USERROLESETID</td>
        </tr>
        <tr>
             <td>USERLOCATIONID</td>
             <td>PK</td>
             <td>-</td>
             <td>-</td>
        </tr>
    </tbody>
</table>

### 사용자 환경 설정 값

<table>
    <thead>
        <tr>
            <th>Workfront 엔티티 이름</th>
            <th>인터페이스 참조</th>
            <th>API 참조</th>
            <th>API 레이블</th>
            <th>데이터 레이크 보기</th>
        </tr>
      </thead>
      <tbody>
        <tr>
            <td>사용자 환경 설정 값</td>
            <td>사용자 환경 설정</td>
            <td>USERPF</td>
            <td>사용자 환경 설정</td>
            <td>USERPREFVALUES_CURRENT<br>USERPREFVALUES_DAILY_HISTORY<br>USERPREFVALUES_EVENT</td>
        </tr>
      </tbody>
</table>
<table>
    <thead>
        <tr>
            <th>기본/외래 키</th>
            <th>유형</th>
            <th>관련 테이블</th>
            <th>관련 필드</th>
        </tr>
    </thead>
    <tbody>
        <tr>
             <td>SYSID</td>
             <td>-</td>
             <td colspan="2">관계가 아닙니다. 내부 응용 프로그램 용도로 사용됩니다.</td>
        </tr>
        <tr>
             <td>사용자 ID</td>
             <td>FK</td>
             <td>USERS_CURRENT</td>
             <td>사용자 ID</td>
        </tr>
        <tr>
             <td>USERPREFVALUEID</td>
             <td>PK</td>
             <td>-</td>
             <td>-</td>
        </tr>
    </tbody>
</table>

### 사용자 역할 집합

<table>
    <thead>
        <tr>
            <th>Workfront 엔티티 이름</th>
            <th>인터페이스 참조</th>
            <th>API 참조</th>
            <th>API 레이블</th>
            <th>데이터 레이크 보기</th>
        </tr>
      </thead>
      <tbody>
        <tr>
            <td>사용자 역할 집합</td>
            <td>사용자 역할 집합</td>
            <td>URSET</td>
            <td>사용자 역할 집합</td>
            <td>USERROLESET_CURRENT<br>USERROLESET_DAILY_HISTORY<br>USERROLESET_EVENT</td>
        </tr>
      </tbody>
</table>
<table>
    <thead>
        <tr>
            <th>기본/외래 키</th>
            <th>유형</th>
            <th>관련 테이블</th>
            <th>관련 필드</th>
        </tr>
    </thead>
    <tbody>
        <tr>
             <td>프리마리롤리드</td>
             <td>FK</td>
             <td>ROLES_CURRENT</td>
             <td>장미모양-</td>
        </tr>
        <tr>
             <td>SYSID</td>
             <td>-</td>
             <td colspan="2">관계가 아닙니다. 내부 응용 프로그램 용도로 사용됩니다.</td>
        </tr>
        <tr>
             <td>사용자 ID</td>
             <td>FK</td>
             <td>USERS_CURRENT</td>
             <td>사용자 ID</td>
        </tr>
        <tr>
             <td>USERROLESETID</td>
             <td>PK</td>
             <td>-</td>
             <td>-</td>
        </tr>
    </tbody>
</table>

### 사용자 결정

<table>
    <thead>
        <tr>
            <th>Workfront 엔티티 이름</th>
            <th>인터페이스 참조</th>
            <th>API 참조</th>
            <th>API 레이블</th>
            <th>데이터 레이크 보기</th>
        </tr>
      </thead>
      <tbody>
        <tr>
            <td>사용자 결정</td>
            <td>사용자 결정</td>
            <td>USRDEC</td>
            <td>사용자 결정</td>
            <td>USERSDECISIONS_CURRENT<br>USERSDECISIONS_DAILY_HISTORY<br>USERSDECISIONS_EVENT</td>
        </tr>
      </tbody>
</table>
<table>
    <thead>
        <tr>
            <th>기본/외래 키</th>
            <th>유형</th>
            <th>관련 테이블</th>
            <th>관련 필드</th>
        </tr>
    </thead>
    <tbody>
        <tr>
             <td>USERDECISIONID</td>
             <td>PK</td>
             <td>-</td>
             <td>-</td>
        </tr>
        <tr>
             <td>SYSID</td>
             <td>-</td>
             <td colspan="2">관계가 아닙니다. 내부 응용 프로그램 용도로 사용됩니다.</td>
        </tr>
        <tr>
             <td>사용자 ID</td>
             <td>FK</td>
             <td>USERS_CURRENT</td>
             <td>사용자 ID</td>
        </tr>
    </tbody>
</table>

### 작업 항목

<table>
    <thead>
        <tr>
            <th>Workfront 엔티티 이름</th>
            <th>인터페이스 참조</th>
            <th>API 참조</th>
            <th>API 레이블</th>
            <th>데이터 레이크 보기</th>
        </tr>
      </thead>
      <tbody>
        <tr>
            <td>작업 항목</td>
            <td>작업 항목</td>
            <td>WRKITM</td>
            <td>작업 항목</td>
            <td>WORKITEMS_CURRENT<br>WORKITEMS_DAILY_HISTORY<br>WORKITEMS_EVENT</td>
        </tr>
      </tbody>
</table>
<table>
    <thead>
        <tr>
            <th>기본/외래 키</th>
            <th>유형</th>
            <th>관련 테이블</th>
            <th>관련 필드</th>
        </tr>
    </thead>
    <tbody>
        <tr>
             <td>ASSIGNMENTID</td>
             <td>FK</td>
             <td>ASSIGNMENTS_CURRENT</td>
             <td>ASSIGNMENTID</td>
        </tr>
        <tr>
             <td>OBJID</td>
             <td>FK</td>
             <td>변수, OBJCODE 기반</td>
             <td>OBJCODE 필드에서 식별된 객체의 기본 키/ID</td>
        </tr>
        <tr>
             <td>OPTASKID</td>
             <td>FK</td>
             <td>OPTASKS_CURRENT</td>
             <td>OPTASKID</td>
        </tr>
        <tr>
             <td>PROJECTID</td>
             <td>FK</td>
             <td>PROJECTS_CURRENT</td>
             <td>PROJECTID</td>
        </tr>
        <tr>
             <td>SYSID</td>
             <td>-</td>
             <td colspan="2">관계가 아닙니다. 내부 응용 프로그램 용도로 사용됩니다.</td>
        </tr>
        <tr>
             <td>TASKID</td>
             <td>FK</td>
             <td>TASKS_CURRENT</td>
             <td>TASKID</td>
        </tr>
        <tr>
             <td>사용자 ID</td>
             <td>FK</td>
             <td>USERS_CURRENT</td>
             <td>사용자 ID</td>
        </tr>
        <tr>
             <td>WORKITEMID</td>
             <td>PK</td>
             <td>-</td>
             <td>-</td>
        </tr>
    </tbody>
</table>
