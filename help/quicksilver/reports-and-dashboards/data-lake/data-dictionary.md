---
content-type: reference
product-area: reports and dashboards
navigation-topic: data connect
title: Workfront Data Connect 데이터 사전
description: 이 페이지에는 Workfront Data Connect의 데이터 구조 및 내용에 대한 정보가 포함되어 있습니다.
author: Nolan
feature: Reports and Dashboards
exl-id: 57985404-554e-4289-b871-b02d3427aa5c
source-git-commit: 9caac488522d2a12d3bdf4bf23ba7e44c6dbf7d2
workflow-type: tm+mt
source-wordcount: '4609'
ht-degree: 4%

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

<table>
  <thead>
    <tr>
        <th>Workfront 엔티티 이름</th>
        <th>인터페이스 참조</th>
        <th>API 참조 | 레이블</th>
        <th>데이터 레이크 테이블</th>
        <th>관계 필드</th>
        <th>관계 테이블 및 필드</th>
    </tr>
  </thead>
  <tbody>
    <tr>
        <td>액세스 수준</td>
        <td>액세스 수준</td>
        <td>ACSLVL | 액세스 수준</td>
        <td>ACCESSLEVELS_CURRENT<br>ACCESSLEVELS_DAILY_HISTORY<br>ACCESSLEVELS_EVENT</td>
        <td>ACCESSLEVELID(자체)<br>APPGLOBALID<br>LASTUPDATEDBYID<br>LEGACYACCESSLEVELID<br>OBJID<br>SYSID</td>
        <td>자체<br>관계가 아님, 내부 응용 프로그램 용도로 사용됨<br>USER_CURRENT | USERID<br>관계가 없음, 내부 응용 프로그램 용도로 사용<br>OBJCODE 필드에서 식별된 개체의 ID<br>관계가 없음, 내부 응용 프로그램 용도로 사용</td>
    </tr>
    <tr>
        <td>액세스 규칙</td>
        <td>공유</td>
        <td>ACSRUL | 공유</td>
        <td>ACCESSRULES_CURRENT<br>ACCESSRULES_DAILY_HISTORY<br>ACCESSRULES_EVENT</td>
        <td>ACCESSORID <br>ACCESSRULEID(자체) <br>ANCESTORID <br>LASTUPDATEDBYID <br>SECURITYOBJID <br>SYSID</td>
        <td>ACCESSOROBJCODE 필드에서 식별된 개체의 ID<br>자체<br>ANCESTOROBJCODE 필드에서 식별된 개체의 ID<br>USERS_CURRENT | USERID<br>SECURITYOBJCODE 필드에서 식별된 개체의 ID<br>관계가 없습니다. 내부 응용 프로그램 용도로 사용됩니다.</td>
    </tr>
    <tr>
        <td>승인 경로</td>
        <td>승인 경로</td>
        <td>ARVPTH | 승인</td>
        <td>APPROVALPATHS_CURRENT<br>APPROVALPATHS_DAILY_HISTORY<br>APPROVALPATHS_EVENT</td>
        <td>APPROVALPATHID(자체) <br>APPROVALPROCESSID <br>ENTEREDBYID <br>GLOBALPATHID <br>LASTUPDATEDBYID <br>SYSID</td>
        <td>자체<br>APPROVALPROCESSES_CURRENT | APPROVALPROCESSID<br>USERS_CURRENT | USERID<br>관계가 아님, 내부 응용 프로그램 용도로 사용됨<br>USERS_CURRENT | USERID<br>관계가 아님, 내부 응용 프로그램 용도로 사용됨</td>
    </tr>
    <tr>
        <td>승인 진행</td>
        <td>승인 진행</td>
        <td>ARVPRC | 승인 진행</td>
        <td>APPROVALPROCESSES_CURRENT<br>APPROVALPROCESSES_DAILY_HISTORY<br>APPROVALPROCESSES_EVENT</td>
        <td>APPROVALPROCESSID(자체) <br>ENTEREDBYID <br>LASTUPDATEDBYID<br>SYSID</td>
        <td>자체<br>사용자_현재 | USERID<br>USERS_CURRENT | USERID<br>관계가 아님, 내부 응용 프로그램 용도로 사용됨</td>
    </tr>
    <tr>
        <td>승인 단계</td>
        <td>승인 단계</td>
        <td>ARVSTP | 승인 단계</td>
        <td>APPROVALSTEPS_CURRENT<br>APPROVALSTEPS_DAILY_HISTORY<br>APPROVALSTEPS_EVENT</td>
        <td>APPROVALPATHID <br>APPROVALSTEPID(자체) <br>SYSID</td>
        <td>APPROVALPATHS_CURRENT | APPROVALPATHID<br>자체<br>관계가 아님, 내부 응용 프로그램 용도로 사용됨</td>
    </tr>
    <tr>
        <td>승인자 상태</td>
        <td>승인자 상태</td>
        <td>아르브스트 | 승인자 상태</td>
        <td>APPROVERSTATUSES_CURRENT<br>APPROVERSTATUSES_DAILY_HISTORY<br>APPROVERSTATUSES_EVENT</td>
        <td>APPROVERSTATUSID(자체)<br>APPROVABLEOBJID<br>APPROVALSTEPID<br>APPROVEDBYID <br>DELEGATEUSERID<br>LASTUPDATEDBYID <br>OPTASKID<br>OVERRIDDENUSERID<br>PROJECTID<br>STEAPPROVERID<br>SYSID<br>TASKID<br>WILDCARDUSERID</td>
        <td>자체<br>APPROVABLEOBJCODE 필드에서 식별된 개체의 ID<br>APPROVALSTEPS_CURRENT | APPROVALSTEPID<br>USERS_CURRENT | USERID <br>USERS_CURRENT | USERID<br>USERS_CURRENT | 사용자 ID <br>OPTASKS_CURRENT | OPTASKID<br>USERS_CURRENT | USERID<br>PROJECTS_CURRENT | PROJECTID<br>USERS_CURRENT | USERID<br>관계가 아님, 내부 응용 프로그램 용도로 사용됨<br>TASKS_CURRENT | TASKID<br>USERS_CURRENT | 사용자 ID</td>
    </tr>
    <tr>
        <td>할당</td>
        <td>할당</td>
        <td>ASSIGN | 할당</td>
        <td>ASSIGNMENTS_CURRENT<br>ASSIGNMENTS_DAILY_HISTORY<br>ASSIGNMENTS_EVENT</td>
        <td>ASSIGNEDBYID<br>ASSIGNEDTOID<br>ASSIGNMENTID(자체)<br>CATEGORYID<br>CLASSIFIERID<br>OPTASKID<br>PRIVATERATECARDID<br>PROJECTID<br>ROLEID<br>TASKID<br>TEAMID</td>
        <td>USER_CURRENT | USERID<br>USER_CURRENT | USERID<br>자체<br>범주_현재 | CATEGORYID<br>분류자 테이블이 현재 지원되지 않음<br>OPTASK_CURRENT | OPTASKID<br>RATECARD_CURRENT | RATECARDID<br>PROJECT_CURRENT | PROJECTID<br>ROLE_CURRENT | ROLEID<br>TASK_CURRENT | TASKID<br>TEAM_CURRENT | 티미드</td>
    </tr>
    <tr>
        <td>승인 대기 중</td>
        <td>승인 대기 중</td>
        <td>AWAPVL | 승인 대기 중</td>
        <td>AWAITINGAPPROVALS_CURRENT<br>AWAITINGAPPROVALS_DAILY_HISTORY<br>AWAITINGAPPROVALS_EVENT</td>
        <td>ACCESSREQUESTID<br>APPROVABLEID <br>APPROVERID <br>AWAITINGAPPROVALID(자체) <br>DOCUMENTID <br>DOCUMENTVERSIONID<br>OPTASKID <br>PROJECTID <br>ROLEID <br>SUBMITTEDBYID <br>SYSID<br>TASKID <br>TEAMID <br>TIMESHEETID<br>USERID</td>
        <td>액세스 요청 테이블이 현재 지원되지 않음<br>관계가 아님, 내부 응용 프로그램 용도로 사용됨<br>USERS_CURRENT | USERID<br>자체<br>DOCUMENTS_CURRENT | DOCUMENTID<br>DOCUMENTVERSIONS_CURRENT | DOCUMENTVERSIONID<br>OPTASKS_CURRENT | OPTASKID<br>PROJECTS_CURRENT | PROJECTID<br>ROLES_CURRENT | ROLEID<br>USERS_CURRENT | USERID<br>관계가 아님, 내부 응용 프로그램 용도로 사용됨<br>TASKS_CURRENT | TASKID<br>TEAMS_CURRENT | TEAMID<br>TIMESHEETS_CURRENT | TIMESHEETID<br>USERS_CURRENT | 사용자 ID</td>
    </tr>
    <tr>
        <td>기준선</td>
        <td>기준선</td>
        <td>블린 | 기준선</td>
        <td>BASELINES_CURRENT<br>BASELINES_DAY_HISTORY<br>BASELINES_EVENT</td>
        <td>BASELINEID(자체)<br>EXCHANGERATEID <br>PROJECTID <br>SYSID</td>
        <td>자체<br>EXCHANGERATES_CURRENT | EXCHANGERATEID<br>PROJECTS_CURRENT | PROJECTID<br>관계가 아닙니다. 내부 응용 프로그램 용도로 사용됩니다.</td>
    </tr>
    <tr>
        <td>기준선 작업</td>
        <td>기준선 작업</td>
        <td>BSTSK | 기준선 작업</td>
        <td>BASELINETTASKS_CURRENT<br>BASELINETTASKS_DAILY_HISTORY<br>BASELINETTASKS_EVENT</td>
        <td>BASELINEID<br>BASELINETASKID(자체) <br>EXCHANGERATEID <br>PROJECTID <br>SYSID<br>TASKID</td>
        <td>BASELINES_CURRENT | BASELINEID<br>자체<br>EXCHANGERATES_CURRENT | EXCHANGERATEID<br>PROJECTS_CURRENT | PROJECTID<br>관계가 아님, 내부 응용 프로그램 용도로 사용됨<br>TASKS_CURRENT | TASKID</td>
    </tr>
    <tr>
        <td>청구 요금</td>
        <td>비율 또는 재정의 비율</td>
        <td>비율 | 청구 요금</td>
        <td>RATES_CURRENT<br>RATES_DAILY_HISTORY<br>RATES_EVENT</td>
        <td>ASSIGNMENTID<br>CLASSIFIERID<br>EXCHANGERATEID<br>NLBRCATEGORYID<br>NONLABORRESOURCEID<br>OBJID<br>PROJECTID <br>RATECARDID<br>RATEID(자체)<br>ROLEID <br>SOURCERATECARDID <br>SYSID <br>TEMPLATEID<br>USERID</td>
        <td>ASSIGNMENTS_CURRENT | ASSIGNMENTID<br>분류자 테이블이 현재 지원되지 않음<br>EXCHANGERATES_CURRENT | EXCHANGERATEID<br>비인적 자원 범주 테이블은 현재 지원되지 않습니다<br>NONLABORRESOURCES_CURRENT | NONLABORRESOURCEID<br>OBJCODE 필드에서 식별된 개체의 ID<br>PROJECTS_CURRENT | PROJECTID <br>RATECARD_CURRENT | RATECARDID<br>Self<br>ROLES_CURRENT | ROLEID <br>RATECARD_CURRENT | RATECARDID <br>관계가 아닙니다. 내부 응용 프로그램 용도로 사용됩니다. <br>TEMPLATES_CURRENT | TEMPLATEID<br>USERS_CURRENT | 사용자 ID</td>
    </tr>
    <tr>
        <td>청구 기록</td>
        <td>청구 기록</td>
        <td>청구서 | 청구 기록</td>
        <td>BILLINGRECORDS_CURRENT<br>BILLINGRECORDS_DAILY_HISTORY<br>BILLINGRECORDS_EVENT</td>
        <td>BILLINGRECORDID(자체)<br>CATEGORYID<br>EXCHANGERATEID <br>INVOICID <br>LASTUPDATEDBYID <br>PROJECTID <br>SYSID</td>
        <td>자체<br>범주_현재 | CATEGORYID<br>EXCHANGERATES_CURRENT | EXCHANGERATEID <br>현재 <br>USERS_CURRENT의 송장 테이블이 지원되지 않습니다. | 사용자 ID <br>PROJECTS_CURRENT | PROJECTID   <br>관계가 아닙니다. 내부 응용 프로그램 용도로 사용됩니다.</td>
    </tr>
    <tr>
        <td>예약</td>
        <td>예약</td>
        <td>예약 | 예약</td>
        <td>BOOKINGS_CURRENT<br>BOOKINGS_DAILY_HISTORY<br>BOOKINGS_EVENT</td>
        <td>BOOKINGID(자체)<br>ENTEREDBYID<br>LASTUPDATEDBYID<br>NLBRCATEGORYID<br>NONLABORRESOURCEID<br>OBJID<br>PROJECTID<br>SYSID<br>TASKID<br>TEMPLATEID<br>TEMPLATETASKID<br>TOPOBJID</td>
        <td>자체<br>사용자_현재 | USERID<br>USERS_CURRENT | USERID<br>비인적 자원 범주 테이블은 현재 지원되지 않음<br>NONLABORRESOURCES_CURRENT | NONLABORRESOURCEID<br>OBJOBJCODE 필드에서 식별된 개체의 ID<br>PROJECTS_CURRENT | PROJECTID <br>관계가 아님, 내부 응용 프로그램 용도로 사용됨<br>TASKS_CURRENT | TASKID<br>TEMPLATES_CURRENT | TEMPLATEID<br>TEMPLATETASKS_CURRENT | TEMPLATETASKID<br>TOPOBJCODE 필드에서 식별된 개체의 ID입니다</td>
    </tr>
    <tr>
        <td>비즈니스 프로필</td>
        <td>비즈니스 프로필</td>
        <td>BSNPRF | 비즈니스 프로필</td>
        <td>BUSINESSPROFILE_CURRENT<br>BUSINESSPROFILE_DAILY_HISTORY<br>BUSINESSPROFILE_EVENT</td>
        <td>ACCESSLEVELID<br>BUSINESSPROFILEID(자체)<br>ENTEREDBYID<br>GROUPID<br>LASTUPDATEDBYID<br>SYSID</td>
        <td>ACCESSLEVELS_CURRENT | ACCESSLEVELID<br>자체<br>사용자_현재 | USERID<br>GROUPS_CURRENT | GROUPID<br>USERS_CURRENT | USERID<br>관계가 아님, 내부 응용 프로그램 용도로 사용됨</td>
    </tr>
    <tr>
        <td>비즈니스 규칙</td>
        <td>비즈니스 규칙</td>
        <td>BSNRUL | 비즈니스 규칙</td>
        <td>BUSINESSRULE_CURRENT<br>BUSINESSRULE_DAILY_HISTORY<br>BUSINESSRULE_EVENT</td>
        <td>BUSINESSRULEID(자체)<br>ENTEREDBYID<br>LASTUPDATEDBYID<br>SYSID</td>
        <td>자체<br>사용자_현재 | USERID<br>USERS_CURRENT | USERID<br>관계가 아님, 내부 응용 프로그램 용도로 사용됨</td>
    </tr>
    <tr>
        <td>범주</td>
        <td>사용자 정의 양식</td>
        <td>CTGY | 범주</td>
        <td>CATEGORIES_CURRENT<br>CATEGORIES_DAILY_HISTORY<br>CATEGORIES_EVENT</td>
        <td>CATEGORYID(자체)<br>ENTEREDBYID<br>GROUPPID<br>LASTUPDATEDBYID<br>SYSID</td>
        <td>자체<br>사용자_현재 | USERID<br>GROUPS_CURRENT | GROUPID<br>USERS_CURRENT | USERID<br>관계가 아님, 내부 응용 프로그램 용도로 사용됨</td>
    </tr>
    <tr>
        <td>범주 매개변수</td>
        <td>사용자 정의 양식 필드</td>
        <td>CTGYA | 범주 매개변수</td>
        <td>CATEGORIESPARAMETERS_CURRENT<br>CATEGORIESPARAMETERS_DAILY_HISTORY<br>CATEGORIESPARAMETERS_EVENT</td>
        <td>CATEGORIESPARAMETERID(자체)<br>CATEGORYID<br>PARAMETERGROUPID<br>PARAMETERID<br>SYSID</td>
        <td>자체<br>범주_현재 | CATEGORYID<br>현재 지원되지 않는 매개변수 그룹 테이블<br>PARAMETERS_CURRENT | 매개 변수화    <br>관계가 아닙니다. 내부 응용 프로그램 용도로 사용됩니다.</td>
    </tr>
    <tr>
        <td>분류자</td>
        <td>위치</td>
        <td>CLSF | 위치</td>
        <td>CLASSIFIER_CURRENT<br>CLASSIFIER_DAILY_HISTORY<br>CLASSIFIER_EVENT</td>
        <td>CLASSIFIERID(자체)<br>ENTEREDBYID<br>LASTUPDATEDBYID<br>PARENTID<br>SYSID</td>
        <td>자체<br>사용자_현재 | USERID<br>USERS_CURRENT | USERID<br>CLASSIFIER_CURRENT | CLASSIFIERID<br>관계가 아님, 내부 응용 프로그램 용도로 사용됨</td>
    </tr>
    <tr>
        <td>회사</td>
        <td>회사</td>
        <td>지저분해 | 회사</td>
        <td>COMPANIES_CURRENT<br>COMPANIES_DAILY_HISTORY<br>COMPANIES_EVENT</td>
        <td>CATEGORYID<br>COMPANYID(자체)<br>ENTEREDBYID<br>GROUPID<br>LASTUPDATEDBYID<br>PRIVATERATECARDID<br>SYSID</td>
        <td>CATEGORS_CURRENT | CATEGORYID<br>Self<br>USERS_CURRENT | 사용자 ID <br>GROUPS_CURRENT | GROUPID<br>USERS_CURRENT | 사용자 ID <br>RATECARD_CURRENT | RATECARDID<br>관계가 아닙니다. 내부 응용 프로그램 용도로 사용됩니다.</td>
    </tr>
    <tr>
        <td>사용자 정의 분기</td>
        <td>사용자 정의 분기</td>
        <td>CSTQRT | 사용자 정의 영역</td>
        <td>CUSTOMQUARTERS_CURRENT<br>CUSTOMQUARTERS_DAILY_HISTORY<br>CUSTOMQUARTERS_EVENT</td>
        <td>CUSTOMQUARTERID(자체) <br>SYSID</td>
        <td>자체<br>관계가 아님, 내부 응용 프로그램 용도로 사용됨</td>
    </tr>
    <tr>
        <td>CustomEnum</td>
        <td>상태, 우선 순위, 심각도, 상태</td>
        <td>CSTEM | 사용자 정의 열거형</td>
        <td>CUSTOMENUMS_CURRENT<br>CUSTOMENUMS_DAILY_HISTORY<br>CUSTOMENUMS_EVENT<br>* 레코드 유형은 'enumClass' 속성을 통해 식별됩니다. 다음은 예상 유형입니다.<br>CONDITION_OPTASK<br>CONDITION_PROJ<br>CONDITION_TASK<br>PRIORITY_OPTASK<br>PRIORITY_PROJ<br>PRIORITY_TASK<br>SEVERITY_OPTASK<br>STATUS_OPTASK<br>STATUS_PROJ<br>STATUS_TASK</td>
        <td>ENTEREDBYID<br>GROUPID</td>
        <td>USER_CURRENT | USERID<br>GROUP_CURRENT | GROUPID</td>
    </tr>
    <tr>
        <td>문서</td>
        <td>문서</td>
        <td>도쿠 | 문서</td>
        <td>DOCUMENTS_CURRENT<br>DOCUMENTS_DAILY_HISTORY<br>DOCUMENTS_EVENT<br>DOCUMENTS_CUSTOM_VALUE_CURRENT<br>DOCUMENTS_CUSTOM_VALUE_DAILY_HISTORY<br>DOCUMENTS_CUSTOM_VALUE_EVENT</td>
        <td>CATEGORYID<br>CHECKEDOUTBYID<br>DOCUMENTID<br>DOCUMENTREQUESTID<br>EXCHANGERATEID<br>ITERATIONID<br>LASTNOTEID<br>LASTUPDATEDBYID<br>NOTEID<br>OBJID<br>OPTASKID<br>OWNERID<br>PORTFOLIOID<br>PROGRAMID<br>PROJECTID<br>RELEASEVERSIONID<br>TASKID<br>TEMPLATEID<br>TEMPLATEKID<br>USERID<br></td>
        <td>CATEGORS_CURRENT | CATEGORYID<br>USER_CURRENT | USERID<br>자체<br>문서 요청 테이블이 현재 지원되지 않음<br>EXCHANGERATES_CURRENT | EXCHANGERATEID<br>ITERATIONS_CURRENT | ITERATIONID<br>NOTE_CURRENT | NOTEID<br>USER_CURRENT | USERID<br>NOTE_CURRENT | NOTEID<br>DOCOBJCODE 값에 따라 변수<br>OPTASK_CURRENT | OPTASKID<br>USER_CURRENT | USERID<br>PORTFOLIO_현재 | 포트폴리오<br>PROGRAM_CURRENT | PROGRAMID<br>PROJECT_CURRENT | PROJECTID<br>릴리스 버전 테이블이 현재 지원되지 않음<br>TASK_CURRENT | TASKID<br>TEMPLATES_CURRENT | TEMPLATEID<br>TEMPLATETASKS_CURRENT | TEMPLATETASKID<br>TOPOBJCODE 값에 따라 변수<br>USER_CURRENT | 사용자 ID</td>
    </tr>
    <tr>
        <td>문서 승인</td>
        <td>문서 승인</td>
        <td>DOCAPL | 문서 승인</td>
        <td>DOCAPPROVALS_CURRENT<br>DOCAPPROVALS_DAILY_HISTORY<br>DOCAPPROVALS_EVENT</td>
        <td>APPROVERID<br>DOCAPPROVALID(자체)<br>DOCUMENTID<br>NOTEID<br>REQUESTORID<br>SYSID</td>
        <td>USERS_CURRENT | USERID <br>Self<br>DOCUMENTS_CURRENT | DOCUMENTID<br>NOTES_CURRENT | NOTEID<br>USERS_CURRENT | USERID <br>관계가 아닙니다. 내부 응용 프로그램 용도로 사용됩니다.</td>
    </tr>
    <tr>
        <td>문서 폴더</td>
        <td>문서 폴더</td>
        <td>DOCFLD | 문서 폴더</td>
        <td>DOCTFOLDERS_CURRENT<br>DOCTFOLDERS_DAILY_HISTORY<br>DOCTFOLDERS_EVENT</td>
        <td>DOCFOLDERID(자체)<br>ENTEREDBYID<br>ISSUEID<br>ITERATIONID    <br>LINKEDFOLDERID<br>PARENTID<br>PORTFOLIOID <br>PROGRAMID    <br>PROJECTID<br>SYSID<br>TASKID     <br>TEMPLATEID<br>TEMPLATETASKID<br>USERID</td>
        <td>자체<br>사용자_현재 | USERID<br>OPTASKS_CURRENT | OPTASKID<br>ITERATIONS_CURRENT | ITERATIONID<br>LINKEDFOLDERS_CURRENT | LINKEDFOLDERID<br>DOCTFOLDERS_CURRENT | DOCFOLDERID<br>PORTFOLIO_CURRENT | 포트폴리오 <br>PROGRAM_CURRENT | PROGRAMID    <br>프로젝트_CURRENT | PROJECTID <br>관계가 아님, 내부 응용 프로그램 용도로 사용됨<br>TASKS_CURRENT | TASKID     <br>TEMPLATES_CURRENT | TEMPLATEID<br>TEMPLATETASKS_CURRENT | TEMPLATETASKID<br>USERS_CURRENT | 사용자 ID</td>
    </tr>
    <tr>
        <td>DocumentProviderMetadata</td>
        <td>문서 제공 메타데이터</td>
        <td>문서 | 문서 공급자 메타데이터</td>
        <td>DOCTPROVIDERMETA_CURRENT<br>DOCTPROVIDERMETA_DAILY_HISTORY<br>DOCTPROVIDERMETA_EVENT</td>
        <td>DOCPROVIDERMETAID(자체) <br>SYSID</td>
        <td>자체<br>관계가 아님, 내부 응용 프로그램 용도로 사용됨</td>
    </tr>
    <tr>
        <td>DocumentProvider</td>
        <td>문서 공급자</td>
        <td>DOCPRO | 문서 공급자</td>
        <td>DOCPROVIDERS_CURRENT<br>DOCPROVIDERS_DAILY_HISTORY<br>DOCPROVIDERS_EVENT</td>
        <td>DOCTPROVIDERCONFIGID<br>DOCTPROVIDERID(자체)<br>OWNERID    <br>SYSID</td>
        <td>DOCPROVIDERCONFIG_CURRENT | DOCTPROVIDERCONFIGID<br>자체<br>USERS_CURRENT | 사용자 ID    <br>관계가 아닙니다. 내부 응용 프로그램 용도로 사용됩니다.</td>
    </tr>
    <tr>
        <td>DocumentProviderConfig</td>
        <td>문서 공급자 구성</td>
        <td>DOCCFG | DocumentProviderConfig</td>
        <td>DOCTPROVIDERCONFIG_CURRENT<br>DOCTPROVIDERCONFIG_DAILY_HISTORY<br>DOCTPROVIDERCONFIG_EVENT</td>
        <td>DOCTPROVIDERCONFIGID(self)<br>SYSID</td>
        <td>자체<br>관계가 아님, 내부 응용 프로그램 용도로 사용됨</td>
    </tr>
    <tr>
        <td>DocumentVersion</td>
        <td>문서 버전</td>
        <td>DOCV | 문서 버전</td>
        <td>DOCUMENTVERSIONS_CURRENT<br>DOCUMENTVERSIONS_DAILY_HISTORY<br>DOCUMENTVERSIONS_EVENT</td>
        <td>DOCUMENTID<br>DOCUMENTPROVIDERID<br>DOCUMENTVERSIONID<br>ENTEREDBYID<br>EXTERNALSTORAGEID<br>PROOFAPPROVALSTATUSID<br>PROOFFEDBYUSERID<br>PROOFID<br>PROOFOWNERID<br>PROOFSTAGEID</td>
        <td>DOCUMENT_CURRENT | DOCUMENTID<br>DOCPROVIDERS_CURRENT | DOCUMENTPROVIDERID<br>Self<br>USER_CURRENT | USERID<br>외부 ID<br>증명 승인 상태 테이블이 현재 지원되지 않음<br>USER_CURRENT | USERID<br>증명 테이블이 현재 지원되지 않음<br>USER_CURRENT | USERID<br>증명 단계 테이블이 현재 지원되지 않음</td>
    </tr>
    <tr>
        <td>환율</td>
        <td>환율</td>
        <td>EXRATE | 환율</td>
        <td>EXCHANGERATES_CURRENT<br>EXCHANGERATES_DAILY_HISTORY<br>EXCHANGERATES_EVENT</td>
        <td>EXCHANGERATEID(자체)<br>PROJECTID<br>SYSID <br>TEMPLATEID  </td>
        <td>자체<br>프로젝트_현재 | PROJECTID <br>관계가 아닙니다. 내부 응용 프로그램 용도로 사용됩니다. <br>TEMPLATES_CURRENT | TEMPLATEID  </td>
    </tr>
    <tr>
        <td>경비</td>
        <td>경비</td>
        <td>확장 | 경비</td>
        <td>EXPENSES_CURRENT<br>EXPENSES_DAILY_HISTORY<br>EXPENSES_EVENT</td>
        <td>BILLINGRECORDID<br>CATEGORYID<br>ENTEREDBYID<br>EXCHANGERATEID <br>EXPENSEID(자체) <br>EXPENSETYPEID <br>LASTUPDATEDBYID <br>OBJID <br>PROJECTID<br>SYSID<br>TASKID<br>TEMPLATEID<br>TEMPLATETASKID<br>TOPOBJID</td>
        <td>BILLINGRECORDS_CURRENT | BILLINGRECORDID<br>CATEGORIES_CURRENT | CATEGORYID<br>USERS_CURRENT | USERID<br>EXCHANGERATES_CURRENT | EXCHANGERATEID <br>자체 <br>EXPENSETYPES_CURRENT | EXPENSETYPEID <br>USERS_CURRENT | USERID <br>OBJCODE 필드 <br>PROJECTS_CURRENT에서 식별된 개체의 ID | PROJECTID <br>관계가 아님, 내부 응용 프로그램 용도로 사용됨<br>TASKS_CURRENT | TASKID<br>TEMPLATES_CURRENT | TEMPLATEID<br>TEMPLATETASKS_CURRENT | TEMPLATETASKID<br>TOPOBJCODE 필드에서 식별된 개체의 ID입니다</td>
    </tr>
    <tr>
        <td>경비 유형</td>
        <td>경비 유형</td>
        <td>EXPTYP | 경비 유형</td>
        <td>EXPENSETYPES_CURRENT<br>EXPENSETYPES_DAILY_HISTORY<br>EXPENSETYPES_EVENT</td>
        <td>APPGLOBALID<br>EXPENSETYPEID(자체)<br>OBJID <br>SYSID  </td>
        <td>관계가 아닙니다. 내부 응용 프로그램 용도로 사용됩니다<br>자체<br>OBJCODE 필드에서 식별된 개체의 ID <br>관계가 아닙니다. 내부 응용 프로그램 용도로 사용됩니다.  </td>
    </tr>
    <tr>
        <td>그룹</td>
        <td>그룹</td>
        <td>그룹 | 그룹</td>
        <td>GROUPS_CURRENT<br>GROUPS_DAILY_HISTORY<br>GROUPS_EVENT</td>
        <td>BUSINESLEADERID<br>CATEGORYID<br>ENTEREDBYID<br>GROUPID<br>LAYOUTTEMPLATEID<br>PARENTID<br>ROOTID<br>UITEMPLATEID</td>
        <td>USER_CURRENT | USERID<br>CATEGORIES_CURRENT | CATEGORYID<br>USER_CURRENT | USERID<br>자체<br>레이아웃 템플릿 테이블이 지원되지 않습니다.<br>GROUP_CURRENT | GROUPID<br>GROUP_CURRENT | GROUPID<br>UITEMPLATES_CURRENT | UITEMPLATEID</td>
    </tr>
    <tr>
        <td>시간</td>
        <td>시간</td>
        <td>시간 | 시간</td>
        <td>HOURS_CURRENT<br>HOURS_DAILY_HISTORY<br>HOURS_EVENT</td>
        <td>APPROVEDBYID<br>BILLINGRECORDID<br>CATEGORYID<br>CLASSIFIERID<br>DUPID<br>EXCHANGERATEID<br>EXTERNALTIMESHEETID<br>HOURTYPEID<br>LASTUPDATEDBYID<br>OPTASKID<br>OWNERID<br>PROJECTID<br>PROJECTTOVERHEADID<br>ROLEID<br>TASKID<br>TIMESHEETID<br></td>
        <td>USER_CURRENT | USERID<br>BILLINGRECORDS_CURRENT | BILLINGRECORDID<br>CATEGORIES_CURRENT | CATEGORYID<br>분류자 테이블이 현재 지원되지 않음<br>관계가 없음, 내부 응용 프로그램 용도로 사용됨<br>EXCHANGERATES_CURRENT | EXCHANGERATEID<br>Workfront 관계가 아님, 외부 시스템과의 통합에 사용됨<br>Self<br>HOURTYPE_CURRENT | HOURTYPEID<br>USER_CURRENT | USERID<br>OPTASK_CURRENT | OPTASKID<br>USER_CURRENT | USERID<br>PROJECT_CURRENT | PROJECTID<br>관계가 아님, 내부 응용 프로그램 용도로 사용됨<br>ROLE_CURRENT | ROLEID<br>TASK_CURRENT | TASKID<br>TIMESHEET_CURRENT | TIMESHEETID</td>
    </tr>
    <tr>
        <td>시간 유형</td>
        <td>시간 유형</td>
        <td>시간 | 시간 유형</td>
        <td>HOURTYPES_CURRENT</td>
        <td>APPGLOBALID<br>HOURTYPEID<br>OBJID</td>
        <td>관계가 아닙니다. 내부 응용 프로그램 용도로 사용됩니다<br>자체<br>관계가 아닙니다. 내부 응용 프로그램 용도로 사용됩니다.</td>
    </tr>
    <tr>
        <td>반복</td>
        <td>반복</td>
        <td>ITRN | 반복</td>
        <td>ITERATIONS_CURRENT<br>ITERATIONS_DAILY_HISTORY<br>ITERATIONS_EVENT</td>
        <td>CATEGORYID<br>ENTEREDBYID<br>ITERATIONID(자체)<br>LASTUPDATEDBYID<br>OWNERID<br>SYSID<br>TEAMID</td>
        <td>CATEGORS_CURRENT | CATEGORYID<br>USERS_CURRENT | 사용자 ID <br>자체<br>사용자_현재 | USERID <br>USERS_CURRENT | 사용자 ID <br>관계가 아님, 내부 응용 프로그램 용도로 사용됨<br>TEAMS_CURRENT | 티미드</td>
    </tr>
    <tr>
        <td>저널 항목</td>
        <td>저널 항목</td>
        <td>JRNLE | 저널 게시물</td>
        <td>JOURNALENTRIES_CURRENT<br>JOURNALENTRIES_DAILY_HISTORY<br>JOURNALENTRIES_EVENT</td>
        <td>APPROVERSTATUSID<br>ASSIGNMENTID<br>AUDITRECORDID<br>BASELINEID <br>BILLINGRECORDID<br>COMPANYID <br>DOCUMENTID <br>DOCUMENTSHAREID <br>EDITEDBYID<br>EXPENSEID<br>HOURID<br>INITIATIVEID<br>JOURNALENTRIEID(자체)<br>OBJID<br>OPTASKID<br>PORTFOLIOID<br>PROGRAMID<br>PROJECTID<br>SUBOBJID<br>SUBSCBEID<br>SYSID <br>TASKID<br>TEMPLATEID<br>TIMESHEETID<br>TOPOBJID<br>USERID</td>
        <td>APPROVERSTATUSES_CURRENT | APPROVERSTATUSID<br>ASSIGNMENTS_CURRENT | ASSIGNMENTID<br>감사 레코드 테이블이 현재 지원되지 않음<br>BASELINES_CURRENT | BASELINEID <br>BILLINGRECORDS_CURRENT | BILLINGRECORDID<br>COMPANIES_CURRENT | COMPANYID <br>DOCUMENTS_CURRENT | DOCUMENTID <br>문서 공유 테이블은 현재 <br>USERS_CURRENT에서 지원되지 않습니다. | USERID<br>EXPENSES_CURRENT | EXPENSEID<br>HOURS_CURRENT | HOURID<br>이니셔티브 테이블이 현재 지원되지 않음<br>자체<br>OBJCODE 필드에서 식별된 개체의 ID<br>OPTASKS_CURRENT | OPTASKID<br>PORTFOLIO_CURRENT | 포트폴리오<br>PROGRAM_CURRENT | PROGRAMID<br>PROJECTS_CURRENT | PROJECTID <br>SUBOBJCODE 필드에서 식별된 개체의 ID<br>구독 테이블이 현재 지원되지 않음<br>관계가 없음, 내부 응용 프로그램 용도로 사용됨<br>TASKS_CURRENT | TASKID<br>TEMPLATES_CURRENT | TEMPLATEID<br>TIMESHEETS_CURRENT | TIMESHEETID<br>TOPOBJCODE 필드에서 식별된 개체의 ID<br>USERS_CURRENT | 사용자 ID</td>
    </tr>
    <tr>
        <td>LinkedFolder</td>
        <td>LinkedFolder</td>
        <td>LNKFDR | LinkedFolder</td>
        <td>LINKEDFOLDERS_CURRENT<br>LINKEDFOLDERS_DAILY_HISTORY<br>LINKEDFOLDERS_EVENT</td>
        <td>DOCUMENTPROVIDERID<br>EXTERNALSTORAGEID<br>FOLDERID<br>LINKEDBYID<br>LINKEDFOLDERID(자체)<br>SYSID</td>
        <td>DOCPROVIDERS_CURRENT | DOCTPROVIDERID<br>외부 ID<br>DOCTFOLDERS_CURRENT | DOCFOLDERID<br>USERS_CURRENT | USERID <br>Self<br>관계가 아님, 내부 응용 프로그램 용도로 사용됨  </td>
    </tr>
    <tr>
        <td>마일스톤</td>
        <td>마일스톤</td>
        <td>마일 | 마일스톤</td>
        <td>MILESTONES_CURRENT<br>MILESTONES_DAILY_HISTORY<br>MILESTONES_EVENT</td>
        <td>LASTUPDATEDBYID<br>MILESTONEID<br>MILESTONEPATHID</td>
        <td>USER_CURRENT | USERID<br>자체<br>마일스톤 경로_현재 | 마일스톤ID</td>
    </tr>
    <tr>
        <td>마일스톤 경로</td>
        <td>마일스톤 경로</td>
        <td>MPATH | 마일스톤 경로</td>
        <td>MILESTONEPATHS_CURRENT<br>MILESTONEPATHS_DAILY_HISTORY<br>MILESTONEPATHS_EVENT</td>
        <td>ENTEREDBYID<br>LASTUPDATEDBYID<br>MILESTONEPATHID</td>
        <td>USER_CURRENT | USERID<br>USER_CURRENT | USERID<br>Self</td>
    </tr>
    <tr>
        <td>NonLaborResource</td>
        <td>비노동 리소스</td>
        <td>NLBR | 비인적 자원</td>
        <td>NONLABORRESOURCES_CURRENT<br>NONLABORRESOURCES_DAILY_HISTORY<br>NONLABORRESOURCES_EVENT</td>
        <td>CATEGORYID<br>NONLABORRESOURCEID(자체)<br>ENTEREDBYID<br>HOMEGROUPPID<br>LASTUPDATEDBYID<br>NONLABORRESOURCECATEGORYID<br>SYSID  </td>
        <td>CATEGORS_CURRENT | CATEGORYID<br>Self<br>USERS_CURRENT | USERID<br>GROUPS_CURRENT | GROUPID<br>USERS_CURRENT | USERID<br>비인적 자원 범주 테이블은 현재 지원되지 않음<br>관계가 없음, 내부 응용 프로그램 용도로 사용됨</td>
    </tr>
    <tr>
        <td>비노동 리소스 범주</td>
        <td>비노동 리소스 범주</td>
        <td>NLBRCY | 비인적 자원 범주</td>
        <td>NLBRCATEGORIES_CURRENT<br>NLBRCATEGORIES_DAILY_HISTORY<br>NLBRCATEGORIES_EVENT</td>
        <td>CATEGORYID<br>ENTEREDBYID<br>LASTUPDATEDBYID<br>NLBRCATEGORYID(자체)<br>PRIVATERATECARDID<br>SCHEDULEID<br>SYSID</td>
        <td>CATEGORS_CURRENT | CATEGORYID<br>USERS_CURRENT | USERID<br>USERS_CURRENT | USERID<br>Self<br>RATECARD_CURRENT | RATECARDID<br>USERS_CURRENT | USERID<br>관계가 아님, 내부 응용 프로그램 용도로 사용됨</td>
    </tr>
    <tr>
        <td>비근무일</td>
        <td>일정 예외</td>
        <td>NONWKD | 비근무일</td>
        <td>NONWORKDAYS_CURRENT<br>NONWORKDAYS_DAILY_HISTORY<br>NONWORKDAYS_EVENT</td>
        <td>NONWORKDAYID(자체)<br>OBJID <br>SCHEDULEID <br>SYSID <br>USERID  </td>
        <td>Self<br>OBJCODE 필드 <br>SCHEDULES_CURRENT에서 식별된 개체의 ID | 일정 ID <br>관계가 아닙니다. 내부 응용 프로그램 용도로 사용됩니다. <br>USERS_CURRENT | 사용자 ID  </td>
    </tr>
    <tr>
        <td>참고</td>
        <td>참고</td>
        <td>참고 | 참고</td>
        <td>NOTES_CURRENT<br>NOTES_DAILY_HISTORY<br>NOTES_EVENT</td>
        <td>ATTACHDOCUMENTID<br>ATTACHOBJID<br>ATTACHOPTASKID<br>ATTACHWORKID<br>ATTACHWORKUSERID<br>AUDITRECORDID<br>COMPANYID<br>DOCUMENTID<br>EXTERNALSERVICID<br>ITERATIONID<br>NOTEID<br>OBJID<br>OPTASKID<br>OWNERID<br>PARENTENDORSEMENTID<br>PARENTJOURALENTRYID<br>PARENTNOTEID<br>PORTFOLIOID<br>PROGRAMID<br>PROJECTID<br>PROOFATIONFACID <br>PROFID<br>RICHTEXTNOTEID<br>TASKID<br>TEMPLATEID<br>TEMPLATETASKID<br>THREADID<br>TIMESHEETID<br>TOPOBJID<br>USERID</td>
        <td>DOCUMENT_CURRENT | DOCUMENTID<br>ATTACHOBJCODE에 따른 변수<br>OPTASK_CURRENT | OPTASKID<br>WORKITEMS_CURRENT<br>USER_CURRENT | USERID<br>감사 레코드 테이블이 현재 지원되지 않음<br>COMPANIES_CURRENT | COMPANYID <br>DOCUMENT_CURRENT | DOCUMENTID<br>Workfront 관계가 아님, 외부 시스템과의 통합에 사용됨<br>ITERATIONS_CURRENT | ITERATIONID<br>Self<br>NOTEOBJCODE<br>OPTASK_CURRENT에 따른 변수 | OPTASKID<br>USER_CURRENT | USERID<br>보증 테이블이 현재 지원되지 않음<br>JOURNALENTRIES_CURRENT | JOURNALENTRYID<br>NOTE_CURRENT | NOTEID<br>PORTFOLIO_CURRENT | 포트폴리오<br>PROGRAM_CURRENT | PROGRAMID<br>PROJECT_CURRENT | PROJECTID<br>증명 작업 테이블이 현재 지원되지 않음<br>증명 테이블이 현재 지원되지 않음<br>RESERVEDTEXTNOTES_CURRENT | RICHTEXTNOTEID<br>TASK_CURRENT | TASKID<br>TEMPLATES_CURRENT | TEMPLATEID<br>TEMPLATETASKS_CURRENT | TEMPLATETASKID<br>NOTE_CURRENT | NOTEID<br>TIMESHEET_CURRENT | TIMESHEETID<br>TOPOBJCODE에 따른 변수<br>USER_CURRENT | 사용자 ID</td>
    </tr>
    <tr>
        <td>오브젝트 통합</td>
        <td>오브젝트 통합</td>
        <td>오브젝트 | 오브젝트 통합</td>
        <td>OBJECTINTEGRATION_CURRENT<br>OBJECTINTEGRATION_DAILY_HISTORY<br>OBJECTINTEGRATION_EVENT</td>
        <td>LINKEDOBJECTID<br>OBJECTINTEGRATIONID   (self)<br>OBJID <br>SYSID  </td>
        <td>LINKEDOBJECTCODE 필드에서 식별된 개체의 ID <br>자체<br>OBJCODE 필드에서 식별된 개체의 ID <br>관계가 아닙니다. 내부 응용 프로그램 용도로 사용됩니다.  </td>
    </tr>
    <tr>
        <td>오브젝트 범주</td>
        <td>오브젝트 범주</td>
        <td>OBJCAT | 오브젝트 범주</td>
        <td>OBJECTSCATEGORIES_CURRENT<br>OBJECTSCATEGORIES_DAILY_HISTORY<br>OBJECTSCATEGORIES_EVENT</td>
        <td>CATEGORYID<br>OBJECTSCATEGORYID(자체)<br>OBJID <br>SYSID  </td>
        <td>CATEGORS_CURRENT | CATEGORYID<br>Self<br>OBJCODE 필드에서 식별된 개체의 ID <br>관계가 아닙니다. 내부 응용 프로그램 용도로 사용됩니다.  </td>
    </tr>
    <tr>
        <td>OpTask</td>
        <td>문제, 요청</td>
        <td>OPTASK | 문제</td>
        <td>OPTASKS_CURRENT<br>OPTASKS_DAILY_HISTORY<br>OPTASKS_EVENT<br>OPTASKS_CUSTOM_VALUE_CURRENT<br>OPTASKS_CUSTOM_VALUE_DAILY_HISTORY<br>OPTASKS_CUSTOM_VALUE_EVENT</td>
        <td>APPROVALPROCESSID<br>ASSIGNEUTTOID<br>CATEGORYID<br>CURRENTAPPROVALSTEPID<br>ENTEREDBYID<br>EXCHANGERATEID<br>ITERATIONID<br>KANBANBOARDID<br>LASTCONDITIONNOTEID<br>LASTNOTEID<br>LASTUPDATEDBYID<br>OPTASKID<br>OWNERID<br>PROJECTID<br>QUEUEDEFID<br>QUEUETOPICID<br>RESOLVEOPTASKID<br>RESOLVETID<br>RESOLVEETASKID <br>RESOLVINGOBJID<br>ROLEID<br>SOURCEOBJID<br>SOURCETASKID<br>SUBMITTEDBYID<br>TEAMID</td>
        <td>APPROVALPROCESSES_CURRENT | APPROVALPROCESSID<br>USER_CURRENT | USERID<br>CATEGORIES_CURRENT | CATEGORYID<br>APPROVALSTEPS_CURRENT | APPROVALSTEPID<br>USER_CURRENT | USERID<br>EXCHANGERATES_CURRENT | EXCHANGERATEID<br>ITERATIONS_CURRENT | ITERATIONID<br>Kanban 보드 테이블이 현재 지원되지 않음<br>NOTE_CURRENT | NOTEID<br>NOTE_CURRENT | NOTEID<br>USER_CURRENT | USERID<br>자체<br>USER_CURRENT | USERID<br>PROJECT_CURRENT | PROJECTID<br>큐 정의 테이블이 현재 지원되지 않음<br>큐 주제 테이블이 현재 지원되지 않음<br>OPTASK_CURRENT | OPTASKID<br>PROJECT_CURRENT | PROJECTID<br>TASK_CURRENT | TASKID<br>RESOLVINGOBJCODE에 따른 변수<br>ROLE_CURRENT | ROLEID<br>SOURCEOBJCODE에 따른 변수<br>TASK_CURRENT | TASKID<br>USER_CURRENT | USERID<br>TEAM_CURRENT | 티미드</td>
    </tr>
    <tr>
        <td>매개변수</td>
        <td>사용자 정의 필드</td>
        <td>매개 변수 | 매개 변수</td>
        <td>PARAMETERS_CURRENT<br>PARAMETERS_DAILY_HISTORY<br>PARAMETERS_EVENT</td>
        <td>LASTUPDATEDBYID<br>PARAMETERFILTERID<br>PARAMETERID(자체)<br>SYSID  </td>
        <td>USERS_CURRENT | USERID<br>매개 변수 필터 테이블이 현재 지원되지 않음<br>자체<br>관계가 없음, 내부 응용 프로그램 용도로 사용됨  </td>
    </tr>
    <tr>
        <td>매개변수 옵션</td>
        <td>매개변수 옵션</td>
        <td>POPT | 매개변수 옵션</td>
        <td>PARAMETEROPTIONS_CURRENT<br>PARAMETEROPTIONS_DAILY_HISTORY<br>PARAMETEROPTIONS_EVENT</td>
        <td>PARAMETERID<br>PARAMETERATIONID(자체) <br>SYSID  </td>
        <td>PARAMETERS_CURRENT | PARAMETERID <br>자체 <br>관계가 없습니다. 내부 응용 프로그램 용도로 사용됩니다.  </td>
    </tr>
    <tr>
        <td>포털 섹션</td>
        <td>보고서</td>
        <td>PTLSEC | 보고서</td>
        <td>PORTALSECTIONS_CURRENT<br>PORTALSECTIONS_DAILY_HISTORY<br>PORTALSECTIONS_EVENT</td>
        <td>APPGLOBALID<br>ENTEREDBYID<br>FILTERID<br>GROUPBYID<br>LASTUPDATEDBYID<br>LASTVIEWEDBYID<br>OBJID<br>PORTALSECTIONID(자체)<br>PREFERENCEID<br>PUBLICRUNASUSERID<br>REPORTFOLDERID<br>RUNASUSERID<br>SCHEDULEDREPORTID<br>SYSID<br>VIEWID</td>
        <td>관계가 아닙니다. 내부 응용 프로그램 용도로 사용됩니다. <br>USERS_CURRENT | 사용자 ID <br>UIFILTERS_CURRENT | FILTERID<br>UIGROUPYS_CURRENT | GROUPBYID<br>USERS_CURRENT | USERID <br>USERS_CURRENT | USERID <br>OBJOBJCODE 필드에서 식별된 개체의 ID<br>Self<br>PREFERENCES_CURRENT | PREFERENCEID<br>USERS_CURRENT | 사용자 ID <br>REPORTFOLDERS_CURRENT | REPORTFOLDERID<br>USERS_CURRENT | USERID <br>예약된 보고서 테이블이 현재 지원되지 않음<br>관계가 없음. 내부 응용 프로그램 용도로 사용됨 <br>UIVIEWS_CURRENT | VIEWID</td>
    </tr>
    <tr>
        <td>포털 탭</td>
        <td>대시보드</td>
        <td>PTLTAB | 대시보드</td>
        <td>PORTALTAB_CURRENT<br>PORTALTAB_DAILY_HISTORY<br>PORTALTAB_EVENT</td>
        <td>DOCID<br>LASTUPDATEDBYID<br>PORTALPROFILEID<br>PORTALTABID(자체)<br>SYSID<br>USERID</td>
        <td>관계가 아닙니다. 내부 응용 프로그램 용도로 사용됩니다. <br>USERS_CURRENT | USERID <br>포털 프로필 테이블이 지원되지 않습니다. <br>자체<br>관계가 없습니다. 내부 응용 프로그램 용도로 사용됨 <br>USERS_CURRENT | 사용자 ID  </td>
    </tr>
    <tr>
        <td>포털 탭 섹션</td>
        <td>대시보드 섹션</td>
        <td>PRTBSC | 포털 탭 섹션</td>
        <td>PORTALTABSPORTALSECTIONS_CURRENT<br>PORTALTABSPORTALSECTIONS_DAILY_HISTORY<br>PORTALTABSPORTALSECTIONS_EVENT</td>
        <td>CALENDARPORTALSECTIONID<br>EXTERNALSECTIONID<br>INTERNALSECTIONID <br>PORTALSECTIONOBJID <br>PORTALTABID<br>PORTALTABSECTIONID(자체)<br>SYSID</td>
        <td>일정 포털 섹션이 현재 지원되지 않음<br>외부 섹션 테이블이 현재 지원되지 않음<br>PORTALSECTIONS_CURRENT | PORTALSECTIONID <br>PORTALSECTIONOBJCODE 필드에서 식별된 개체의 ID<br>PORTALTAB_CURRENT | PORTALTABID<br>자체<br>관계가 아님, 내부 응용 프로그램 용도로 사용됨</td>
    </tr>
    <tr>
        <td>포털 섹션 마지막 뷰어</td>
        <td>마지막 뷰어 보고서</td>
        <td>PLSLSV | 포털 섹션 마지막 뷰어</td>
        <td>REPORTLASTVIEWERS_CURRENT<br>REPORTLASTVIEWERS_DAILY_HISTORY<br>REPORTLASTVIEWERS_EVENT</td>
        <td>REPORTID<br>REPORTLASTVIEWERID(자체)<br>SYSID<br>VIEWERID</td>
        <td>PORTALSECTIONS_CURRENT | PORTALSECTIONID <br>REPORTLASTVIEWERID(자체)<br>관계가 없음, 내부 응용 프로그램 용도로 사용됨<br>USERS_CURRENT | 사용자 ID  </td>
    </tr>
    <tr>
        <td>포트폴리오</td>
        <td>포트폴리오</td>
        <td>포트 | Portfolio</td>
        <td>PORTFOLIO_CURRENT<br>PORTFOLIO_DAILY_HISTORY<br>PORTFOLIO_EVENT<br>PORTFOLIO_CUSTOM_VALUE_CURRENT<br>PORTFOLIO_CUSTOM_VALUE_DAILY_HISTORY<br>PORTFOLIO_CUSTOM_VALUE_EVENT</td>
        <td>ALIGNMENTSCORECARDID<br>CATEGORYID<br>ENTEREDBYID<br>GROUPID<br>LASTUPDATEDBYID<br>OWNERID<br>PORTFOLIOID</td>
        <td>스코어카드 테이블은 현재 지원되지 않습니다<br>CATEGORIES_CURRENT | CATEGORYID<br>USER_CURRENT | USERID<br>GROUP_CURRENT | GROUPID<br>USER_CURRENT | USERID<br>USER_CURRENT | USERID<br>Self</td>
    </tr>
    <tr>
        <td>환경 설정</td>
        <td>보기, 필터링, 그룹화, 보고서 정의</td>
        <td>PROSET | 환경 설정</td>
        <td>PREFERENCES_CURRENT<br>PREFERENCES_DAILY_HISTORY<br>PREFERENCES_EVENT</td>
        <td>APPGLOBALID<br>PREFERENCEID(자체) <br>SYSID  </td>
        <td>관계가 아닙니다. 내부 응용 프로그램 용도로 사용됩니다<br>자체 <br>관계가 아닙니다. 내부 응용 프로그램 용도로 사용됩니다.  </td>
    </tr>
    <tr>
        <td>프로그램</td>
        <td>프로그램</td>
        <td>PRGM | 프로그램</td>
        <td>PROGRAMS_CURRENT<br>PROGRAMS_DAILY_HISTORY<br>PROGRAMS_EVENT<br>PROGRAMS_CUSTOM_VALUE_CURRENT<br>PROGRAMS_CUSTOM_VALUE_DAILY_HISTORY<br>PROGRAMS_CUSTOM_VALUE_EVENT</td>
        <td>CATEGORYID<br>ENTEREDBYID<br>GROUPID<br>LASTUPDATEDBYID<br>OWNERID<br>PORTFOLIOID<br>PROGRAMID</td>
        <td>CATEGORS_CURRENT | CATEGORYID<br>USER_CURRENT | USERID<br>GROUP_CURRENT | GROUPID<br>USER_CURRENT | USERID<br>USER_CURRENT | USERID<br>PORTFOLIO_CURRENT | 포트폴리오<br>자가</td>
    </tr>
    <tr>
        <td>프로젝트</td>
        <td>프로젝트</td>
        <td>프로젝트 | 프로젝트</td>
        <td>PROJECTS_CURRENT<br>PROJECTS_DAILY_HISTORY<br>PROJECTS_EVENT<br>PROJECTS_CUSTOM_VALUE_CURRENT<br>PROJECTS_CUSTOM_VALUE_DAILY_HISTORY<br>PROJECTS_CUSTOM_VALUE_EVENT</td>
        <td>AEMNATIVEFOLDERTREESREFID<br>ALIGNMENTSCORECARDID<br>APPROVALPROCESID<br>ATTACHEDRATECARDID<br>CATEGORYID<br>COMPANYID<br>CONVERTEDOPTASKID<br>CONVERTEDOPTASKORIDATORID<br>CURRENTAPPROVALSTEPID<br>DELIVERABLESCORECARDID<br>ENTEREDBYID<br>GROUPID<br>LASTCONDITIONNOTEID<br>LASTNOTEID<br>LASTUPTEDBYID<br>MILESTONEPATHID<br>OWNERID<br>POPACCOUNTID <br>PORTFOLIOID<br>PRIVATERATECARDID<br>PROGRAMID<br>PROJECTID<br>QUEUEDEFID<br>REJECTIONISSUEID<br>RESOURCEPOOID<br>SCHEDULEID<br>SPONSORID<br>SUBMITTEDBYID<br>TEMAMID<br>TEMPLATEID</td>
        <td>Workfront 관계가 아닙니다. 외부 시스템과의 통합에 사용됩니다.<br>현재 스코어카드 테이블이 지원되지 않습니다.<br>APPROVALPROCESSES_CURRENT | APPROVALPROCESSID<br>RATECARD_CURRENT | RATECARDID<br>CATEGORIES_CURRENT | CATEGORYID<br>COMPANIES_CURRENT | COMPANYID <br>OPTASK_CURRENT | OPTASKID<br>USER_CURRENT | USERID<br>APPROVALSTEPS_CURRENT | APPROVALSTEPID<br>스코어카드 테이블이 현재 지원되지 않음<br>USER_CURRENT | USERID<br>GROUP_CURRENT | GROUPID<br>NOTE_CURRENT | NOTEID<br>NOTE_CURRENT | NOTEID<br>USER_CURRENT | USERID<br>MILESTONEPATH_CURRENT | 마일스톤 경로 ID<br>USER_CURRENT | USERID<br>현재 POP 계정 테이블이 지원되지 않음<br>PORTFOLIO_현재 | 포트폴리오<br>RATECARD_CURRENT | RATECARDID<br>PROGRAM_CURRENT | PROGRAMID<br>Self<br>큐 정의 테이블이 현재 지원되지 않음<br>OPTASK_CURRENT | OPTASKID<br>RESOURCEPOOLS_CURRENT | RESOURCEPOOLID<br>SCHEDULE_CURRENT | 예약 ID<br>USER_CURRENT | USERID<br>USER_CURRENT | USERID<br>TEAM_CURRENT | TEAMID<br>TEMPLATES_CURRENT | TEMPLATEID</td>
    </tr>
    <tr>
        <td>프로젝트 팀 사용자</td>
        <td>프로젝트 팀 사용자</td>
        <td>PRTU | 프로젝트 사용자</td>
        <td>PROJECTSUSERS_CURRENT<br>PROJECTSUSERS_DAILY_HISTORY<br>PROJECTSUSERS_EVENT</td>
        <td>PROJECTID<br>PROJECTSUSERID(자체)<br>SYSID<br>TMPUSERID<br>USERID</td>
        <td>PROJECTS_CURRENT | PROJECTID<br>자체<br>관계가 아님, 내부 응용 프로그램 용도로 사용됨<br>TEMPLATES_CURRENT | TEMPLATEID<br>USERS_CURRENT | 사용자 ID</td>
    </tr>
    <tr>
        <td>프로젝트 팀 사용자 역할</td>
        <td>프로젝트 팀 사용자 역할</td>
        <td>TEAM | 프로젝트 사용자 역할</td>
        <td>PROJECTSUSERSROLES_CURRENT<br>PROJECTSUSERSROLES_DAILY_HISTORY<br>PROJECTSUSERSROLES_EVENT</td>
        <td>PROJECTID<br>PROJECTSUSERSROLEID(자체)<br>ROLEID<br>SYSID<br>USERID</td>
        <td>PROJECTS_CURRENT | PROJECTID<br>Self<br>ROLES_CURRENT | ROLEID<br>관계가 아님, 내부 응용 프로그램 용도로 사용됨<br>USERS_CURRENT | 사용자 ID</td>
    </tr>
    <tr>
        <td>카드 속도</td>
        <td>요율 카드</td>
        <td>RTCRD |등급 카드</td>
        <td>RATECARD_CURRENT<br>RATECARD_DAILY_HISTORY<br>RATECARD_EVENT</td>
        <td>CATEGORYID<br>ENTEREDBYID<br>LASTUPDATEDBYID <br>RATECARDID(자체) <br>SECURITYROOTID <br>SOURCEID<br>SYSID</td>
        <td>CATEGORYID<br>USERS_CURRENT | USERID <br>USERS_CURRENT | 사용자 ID    <br>자체<br>SECURITYOBJCODE 필드에서 식별된 개체의 ID <br>SOURCEOBJCODE 필드에서 식별된 개체의 ID<br>관계가 아닙니다. 내부 응용 프로그램 용도로 사용됩니다  </td>
    </tr>
    <tr>
        <td>보고서 폴더</td>
        <td>보고서 폴더</td>
        <td>RPTFDR | 보고서 폴더</td>
        <td>REPORTFOLDERS_CURRENT<br>REPORTFOLDERS_DAILY_HISTORY<br>REPORTFOLDERS_EVENT</td>
        <td>REPORTFOLDERID(자체)<br>SYSID</td>
        <td>자체<br>관계가 아님, 내부 응용 프로그램 용도로 사용됨</td>
    </tr>
    <tr>
        <td>보고서 보기 통계 수</td>
        <td>보고서 보기 통계 수</td>
        <td>PLSVST | PortalSectionStatisticInfo</td>
        <td>REPORTVIEWSTATICCOUNTS_CURRENT<br>REPORTVIEWSTATICCOUNTS_DAILY_HISTORY<br>REPORTVIEWSTATICCOUNTS_EVENT</td>
        <td>REPORTID<br>REPORTVIEWSTATICCOUNTID(자체)<br>SYSID</td>
        <td>PORTALSECTIONS_CURRENT | PORTALSECTIONID<br>Self<br>관계가 아님, 내부 응용 프로그램 용도로 사용됨</td>
    </tr>
    <tr>
        <td>보고 가능한 예산 시간</td>
        <td>보고 가능한 예산 시간</td>
        <td>RPBGHR | 예산 시간</td>
        <td>REPORTABLEBUDGETEDHOURS_CURRENT<br>REPORTABLEBUDGETEDHOURS_DAILY_HISTORY<br>REPORTABLEBUDGETEDHOURS_EVENT</td>
        <td>PROJECTID<br>REPORTABLEBUDGETEDHOURID(자체)<br>ROLEID<br>SYSID<br>USERID</td>
        <td>PROJECTS_CURRENT | PROJECTID<br>Self<br>ROLES_CURRENT | ROLEID<br>관계가 아님, 내부 응용 프로그램 용도로 사용됨<br>USERS_CURRENT | 사용자 ID</td>
    </tr>
    <tr>
        <td>예약된 시간</td>
        <td>(개인) 휴무</td>
        <td>REVT | 휴무</td>
        <td>RESERVEDTIMES_CURRENT<br>RESERVEDTIMES_DAILY_HISTORY<br>RESERVEDTIMES_EVENT</td>
        <td>RESERVEDTIMEID(자체)<br>SYSID<br>TASKID<br>USERID</td>
        <td>자체<br>관계가 아님, 내부 응용 프로그램 용도로 사용됨<br>TASKS_CURRENT | TASKID<br>USERS_CURRENT | 사용자 ID</td>
    </tr>
    <tr>
        <td>리소스 관리자</td>
        <td>리소스 관리자</td>
        <td>RESMGR | 리소스 관리자</td>
        <td>RESOURCEMANAGERS_CURRENT<br>RESOURCEMANAGERS_DAILY_HISTORY<br>RESOURCEMANAGERS_EVENT</td>
        <td>ID(자체)<br>PROJECTID<br>RESOURCEMANAGERID<br>SYSID<br>TEMPLATEID</td>
        <td>자체<br>프로젝트_현재 | PROJECTID<br>USERS_CURRENT | USERID<br>관계가 아님, 내부 응용 프로그램 용도로 사용됨<br>TEMPLATES_CURRENT | TEMPLATEID</td>
    </tr>
    <tr>
        <td>리소스 풀</td>
        <td>리소스 풀</td>
        <td>RSPL | 리소스 풀</td>
        <td>RSRCPOOLS_CURRENT<br>RSRCPOOLS_DAILY_HISTORY<br>RSRCPOOLS_EVENT</td>
        <td>ENTEREDBYID<br>LASTUPDATEDBYID <br>RESOURCEPOOLID(자체)<br>SYSID  </td>
        <td>USERS_CURRENT | USERID <br>USERS_CURRENT | USERID <br>Self<br>관계가 아님, 내부 응용 프로그램 용도로 사용됨  </td>
    </tr>
    <tr>
        <td>서식 있는 텍스트 메모</td>
        <td>서식 있는 텍스트 메모</td>
        <td>RHNOTE | 서식 있는 텍스트 메모</td>
        <td>RESERVEDTEXTNOTES_CURRENT<br>RESERVEDTEXTNOTES_DAILY_HISTORY<br>RESERVEDTEXTNOTES_EVENT</td>
        <td>RICHTEXTNOTEID(자체)<br>SYSID</td>
        <td>자체<br>관계가 아님, 내부 응용 프로그램 용도로 사용됨</td>
    </tr>
    <tr>
        <td>리치 텍스트 매개 변수 값</td>
        <td>리치 텍스트 매개 변수 값</td>
        <td>RCHVAL | 리치 텍스트 매개 변수 값</td>
        <td>RICHTEXTPARAMETERVALUES_CURRENT<br>RICHTEXTPARAMETERVALUES_DAILY_HISTORY<br>RICHTEXTPARAMETERVALUES_EVENT</td>
        <td>PARAMETERVALUEID<br>RICHTEXTPARAMETERVALUEID(자체) <br>SYSID  </td>
        <td>매개 변수 값 테이블이 현재 지원되지 않음<br>자체 <br>관계가 아님, 내부 응용 프로그램 용도로 사용됨  </td>
    </tr>
    <tr>
        <td>위험</td>
        <td>위험</td>
        <td>위험 | 위험</td>
        <td>RISK_CURRENT<br>RISK_DAILY_HISTORY<br>RISK_EVENT</td>
        <td>ENTEREDBYID<br>EXCHANGERATEID<br>LASTUPDATEDBYID <br>PROJECTID <br>RISKID(자체)<br>RISKTYPEID<br>SYSID<br>TEMPLATEID</td>
        <td>USERS_CURRENT | USERID<br>EXCHANGERATES_CURRENT | EXCHANGERATEID<br>USERS_CURRENT | 사용자 ID <br>PROJECTS_CURRENT | PROJECTID   <br>자체<br>RISKTYPES_CURRENT | RISKTYPEID<br>관계가 아닙니다. 내부 응용 프로그램 용도로 사용됩니다.<br>TEMPLATES_CURRENT | TEMPLATEID</td>
    </tr>
    <tr>
        <td>위험 유형</td>
        <td>위험 유형</td>
        <td>RSKTYP | 위험 유형</td>
        <td>RISKTYPES_CURRENT<br>RISKTYPES_DAILY_HISTORY<br>RISKTYPES_EVENT</td>
        <td>RISKTYPEID<br>SYSID</td>
        <td>자체<br>관계가 아님, 내부 응용 프로그램 용도로 사용됨</td>
    </tr>
    <tr>
        <td>역할</td>
        <td>작업 역할</td>
        <td>역할 | 작업 역할</td>
        <td>ROLES_CURRENT<br>ROLES_DAILY_HISTORY<br>ROLES_EVENT</td>
        <td>ENTEREDBYID<br>LAYOUTTEMPLATEID<br>PRIVATERATECARDID<br>ROLEID<br>UITEMPLATEID</td>
        <td>USER_CURRENT | USERID<br>레이아웃 템플릿 테이블이 지원되지 않습니다<br>RATECARD_CURRENT | RATECARDID<br>Self<br>UITEMPLATES_CURRENT |UITEMPLATEID</td>
    </tr>
    <tr>
        <td>예약</td>
        <td>예약</td>
        <td>일정 조정됨 | 예약</td>
        <td>SCHEDULES_CURRENT<br>SCHEDULES_DAILY_HISTORY<br>SCHEDULES_EVENT</td>
        <td>ENTEREDBYID<br>GROUPID<br>HOMEGROUPID<br>SCHEDULEID</td>
        <td>USER_CURRENT | USERID<br>GROUP_CURRENT | GROUPID<br>GROUP_CURRENT | GROUPID<br>Self</td>
    </tr>
    <tr>
        <td>단계 승인자</td>
        <td>단계 승인자</td>
        <td>SPAPVR | 단계 승인자</td>
        <td>STEPAPPROVERS_CURRENT<br>STEPAPPROVERS_DAILY_HISTORY<br>STEPAPPROVERS_EVENT</td>
        <td>APPROVALSTEPID<br>ROLEID<br>STEPAPPROVERID(자체)<br>SYSID <br>TEAMID<br>USERID</td>
        <td>APPROVALSTEPS_CURRENT | APPROVALSTEPID<br>ROLES_CURRENT | ROLEID<br>자체<br>관계가 아님, 내부 응용 프로그램 용도로 사용됨 <br>TEAMS_CURRENT | TEAMID<br>USERS_CURRENT | 사용자 ID</td>
    </tr>
    <tr>
        <td>작업</td>
        <td>작업</td>
        <td>작업 | 작업</td>
        <td>TASKS_CURRENT<br>TASKS_DAILY_HISTORY<br>TASKS_EVENT<br>TASKS_CUSTOM_VALUE_CURRENT<br>TASKS_CUSTOM_VALUE_DAILY_HISTORY<br>TASKS_CUSTOM_VALUE_EVENT</td>
        <td>APPROVALPROCESSID<br>ASSIGNEDTOID<br>BILLINGRECORDID<br>CATEGORYID<br>CONVERTEDOPTASKID<br>CONVERTEDOPTASKORIATORID<br>CURRENTAPPROVALSTEPID<br>ENTEREDBYID<br>EXCHANGERATEID<br>GROUPID<br>ITERATIONID<br>KANBANBOARDID<br>LASTCONDITIONNOTEID<br>LASTNOTEID<br>LASTUPDATEDBYID<br>MILESTONEID<br>PARENTID<br>PROJECTID<br>RECURRENUCERENUCERENULEULEULEULEULEID<br>ID}ID}ID}ID rejectionissuid<br>RESERVEDTIMEID<br>ROLEID<br>SUBMITTEDBYID<br>TASKID<br>TEAMID<br>TEMPLATETASKID</td>
        <td>APPROVALPROCESSES_CURRENT | APPROVALPROCESSID<br>USER_CURRENT | USERID<br>BILLINGRECORDS_CURRENT | BILLINGRECORDID<br>CATEGORIES_CURRENT | CATEGORYID<br>OPTASK_CURRENT | OPTASKID<br>USER_CURRENT | USERID<br>APPROVALSTEPS_CURRENT | APPROVALSTEPID<br>USER_CURRENT | USERID<br>EXCHANGERATES_CURRENT | EXCHANGERATEID<br>GROUP_CURRENT | GROUPID<br>ITERATIONS_CURRENT | ITERATIONID<br>Kanban 보드 테이블이 현재 지원되지 않음<br>NOTE_CURRENT | NOTEID<br>NOTE_CURRENT | NOTEID<br>USER_CURRENT | USERID<br>MILESTONE_CURRENT | MILESTONEID<br>TASK_CURRENT | TASKID<br>PROJECT_CURRENT | PROJECTID<br>반복 규칙 테이블이 현재 지원되지 않음<br>OPTASK_CURRENT | OPTASKID<br>RESERVEDTIMES_CURRENT | RESERVEDTIMEID<br>ROLE_CURRENT | ROLEID<br>USER_CURRENT | USERID<br>자체<br>팀_현재 | TEAMID<br>TEMPLATETASKS_CURRENT | TEMPLATETASKID</td>
    </tr>
    <tr>
        <td>작업 전임 작업</td>
        <td>전임 작업</td>
        <td>PRED | 전임 작업</td>
        <td>PREDECESSORS_CURRENT<br>PREDECESSORS_DAILY_HISTORY<br>PREDECESSORS_EVENT</td>
        <td>ID(자체)<br>PREDECESSORID<br>SUCCESSORID <br>SYSID</td>
        <td>자체<br>TASKS_CURRENT | TASKID<br>TASKS_CURRENT | TASKID <br>관계가 아닙니다. 내부 응용 프로그램 용도로 사용됩니다.</td>
    </tr>
    <tr>
        <td>팀</td>
        <td>팀</td>
        <td>TEAOB | 팀</td>
        <td>TEAMS_CURRENT<br>TEAMS_DAILY_HISTORY<br>TEAMS_EVENT</td>
        <td>ENTEREDBYID<br>GROUPID<br>LAYOUTTEMPLATEID<br>MYWORKVIEWID<br>OWNERID<br>REQUESTSVIEWID<br>SCHEDULEID<br>TEAMID<br>UITEMPLATEID</td>
        <td>USER_CURRENT | USERID<br>GROUP_CURRENT | GROUPID<br>레이아웃 템플릿 테이블이 지원되지 않습니다.<br>UIVIEWS_CURRENT | UIVIEWID<br>USER_CURRENT | USERID<br>UIVIEWS_CURRENT | UIVIEWID<br>SCHEDULE_CURRENT | 예약 ID<br>자체<br>UITEMPLATES_CURRENT |UITEMPLATEID</td>
    </tr>
    <tr>
        <td>팀원</td>
        <td>기타 팀, 팀원</td>
        <td>TEAMMB | 팀원</td>
        <td>TEAMMEMBERS_CURRENT<br>TEAMMEMBERS_DAILY_HISTORY<br>TEAMMEMBERS_EVENT</td>
        <td>SYSID <br>TEAMID<br>TEAMMEMBERID(자체)<br>USERID</td>
        <td>관계가 아닙니다. 내부 응용 프로그램 용도로 사용됩니다. <br>TEAMS_CURRENT | TEAMID<br>자체<br>사용자_현재 | 사용자 ID</td>
    </tr>
    <tr>
        <td>팀멤버역할</td>
        <td>팀원 역할</td>
        <td>팀 | 팀원 역할</td>
        <td>TEAMMEMBERROLES_CURRENT<br>TEAMMEMBERROLES_DAILY_HISTORY<br>TEAMMEMBERROLES_EVENT</td>
        <td>ROLEID <br>TEAMID<br>TEAMMEMBERROLEID(자체)<br>USERID</td>
        <td>ROLES_CURRENT | ROLEID <br>TEAMS_CURRENT | TEAMID<br>자체<br>사용자_현재 | 사용자 ID</td>
    </tr>
    <tr>
        <td>템플릿</td>
        <td>템플릿</td>
        <td>템플릿 | 템플릿</td>
        <td>TEMPLATES_CURRENT<br>TEMPLATES_DAILY_HISTORY<br>TEMPLATES_EVENT</td>
        <td>APPROVALPROCESSID<br>CATEGORYID<br>COMPANYID <br>DELIVERABLESCORECARDID <br>ENTEREDBYID<br>GROUPID<br>LASTNOTEID<br>LASTUPDATEDBYID<br>MILESTONEPATHID <br>OWNERID <br>PRIVATERATECARDID<br>PROGRAMID<br>QUEUEDEFID<br>SCHEDULEID <br>SYSID <br>TEMAMID<br>TEMPLATEID(자체)</td>
        <td>APPROVALPROCESSES_CURRENT | APPROVALPROCESSID<br>CATEGORIES_CURRENT | CATEGORYID<br>COMPANIES_CURRENT | COMPANYID   <br>DELIVERABLESCORECARDID <br>USERS_CURRENT | USERID<br>GROUPS_CURRENT | GROUPID<br>NOTES_CURRENT | NOTEID<br>USERS_CURRENT | USERID<br>MILESTONEPATH_CURRENT | 마일스톤 경로 ID <br>USERS_CURRENT | USERID <br>RATECARD_CURRENT | RATECARDID<br>PROGRAM_CURRENT | PROGRAMID<br>큐 정의 테이블이 현재 지원되지 않음<br>SCHEDULES_CURRENT | 일정 ID <br>관계가 아닙니다. 내부 응용 프로그램 용도로 사용됩니다. <br>TEAMS_CURRENT | TEAMID<br>자체</td>
    </tr>
    <tr>
        <td>템플릿 할당</td>
        <td>템플릿 할당</td>
        <td>작업 | 템플릿 할당</td>
        <td>TEMPLATEASSIGNMENTS_CURRENT<br>TEMPLATEASSIGNMENTS_DAILY_HISTORY<br>TEMPLATEASSIGNMENTS_EVENT</td>
        <td>ASSIGNEDTOID<br>CATEGORYID<br>LASTUPDATEDBYID<br>OBJID<br>ROLEID<br>SYSID<br>TEAMID<br>TEAMELELINEABLEID<br>TEMPLATEASSIGNMENTID(자체)<br>TEMPLATETASKID</td>
        <td>USERS_CURRENT | USERID<br>CATEGORIES_CURRENT | CATEGORYID<br>USERS_CURRENT | USERID<br>OBJCODE 필드에서 식별된 개체의 ID<br>ROLES_CURRENT | ROLEID<br>관계가 아님, 내부 응용 프로그램 용도로 사용됨<br>TEAMS_CURRENT | TEAMID<br>팀 타임라인 가능 테이블은 현재 지원되지 않음<br>자체<br>TEMPLATETASKS_CURRENT |TEMPLATETASKID</td>
    </tr>
    <tr>
        <td>템플릿 작업</td>
        <td>템플릿 작업</td>
        <td>TTSK | 템플릿 작업</td>
        <td>TEMPLATETASKS_CURRENT<br>TEMPLATETASKS_DAILY_HISTORY<br>TEMPLATETASKS_EVENT</td>
        <td>APPROVALPROCESSID<br>ASSIGNEEDTOID<br>CATEGORYID<br>ENTEREDBYID<br>EXCHANGERATEID<br>LASTNOTEID<br>LASTUDATEDBYID<br>MILESTONEID<br>PARENTID<br>RECURRENCERULEID<br>ROLEID<br>SYSID<br>TEAMID<br>TEAMID<br>TEMPLATEID<br>TEMPLATETASKID(자체)</td>
        <td>APPROVALPROCESSES_CURRENT | APPROVALPROCESSID<br>USERS_CURRENT | USERID<br>CATEGORIES_CURRENT | CATEGORYID<br>USERS_CURRENT | USERID<br>EXCHANGERATES_CURRENT | EXCHANGERATEID<br>NOTES_CURRENT | NOTEID<br>USERS_CURRENT | USERID<br>MILESTONE_CURRENT | MILESTONEID<br>TEMPLATETASKS_CURRENT |TEMPLATETASKID<br>반복 규칙 테이블이 현재 지원되지 않음<br>ROLES_CURRENT | ROLEID<br>관계가 아님, 내부 응용 프로그램 용도로 사용됨<br>TEAMS_CURRENT | TEAMID<br>팀 타임라인 가능 테이블은 현재 지원되지 않음<br>TEMPLATES_CURRENT | TEMPLATEID<br>Self</td>
    </tr>
    <tr>
        <td>템플릿 작업 전임 작업</td>
        <td>템플릿 전임 작업</td>
        <td>TPRED | 전임 작업</td>
        <td>TEMPLATEPREDECESSORS_CURRENT<br>TEMPLATEPREDECESSORS_DAILY_HISTORY<br>TEMPLATEPREDECESSORS_EVENT</td>
        <td>PREDECESSORID<br>SUCCESSORID <br>TEMPLATEPREDECESSORID(자체)<br>SYSID</td>
        <td>TEMPLATETASKS_CURRENT |TEMPLATETASKID<br>TEMPLATETASKS_CURRENT |TEMPLATETASKID <br>자체<br>관계가 없습니다. 내부 응용 프로그램 용도로 사용됩니다.</td>
    </tr>
    <tr>
        <td>타임시트</td>
        <td>타임시트</td>
        <td>체트 | 타임시트</td>
        <td>TIMESHEETS_CURRENT<br>TIMESHEETS_DAILY_HISTORY<br>TIMESHEETS_EVENT</td>
        <td>APPROVERID<br>LASTNOTEID<br>LASTUPDATEDBYID<br>TIMESHEETID<br>TIMESHEETPROFILEID<br>USERID</td>
        <td>USER_CURRENT | USERID<br>NOTE_CURRENT | NOTEID<br>USER_CURRENT | USERID<br>자체<br>타임시트 프로필_현재 | TIMESHEETPROFILEID<br>USER_CURRENT | 사용자 ID</td>
    </tr>
    <tr>
        <td>타임시트 프로필</td>
        <td>타임시트 프로필</td>
        <td>TSPRO | 타임시트 프로필</td>
        <td>TIMESHEETPROFILES_CURRENT<br>TIMESHEETPROFILES_DAILY_HISTORY<br>TIMESHEETPROFILES_EVENT</td>
        <td>APPROVERID<br>ENTEREDBYID <br>GROUPID<br>SYSID<br>TIMESHEETPROFILEID(자체)</td>
        <td>USERS_CURRENT | USERID<br>USERS_CURRENT | 사용자 ID <br>GROUPS_CURRENT | GROUPID<br>관계가 아님, 내부 응용 프로그램 용도로 사용됨<br>자체</td>
    </tr>
    <tr>
        <td>UI 필터</td>
        <td>필터</td>
        <td>UIFT | 필터</td>
        <td>UIFILTERS_CURRENT<br>UIFILTERS_DAILY_HISTORY<br>UIFILTERS_EVENT</td>
        <td>APPGLOBALID<br>ENTEREDBYID <br>LASTUPDATEDBYID <br>OBJID<br>PREFERENCEID<br>SYSID <br>UIFILTERID(자체)</td>
        <td>관계가 아닙니다. 내부 응용 프로그램 용도로 사용됩니다<br>USERS_CURRENT | USERID <br>USERS_CURRENT | USERID <br>OBJCODE 필드에서 식별된 개체의 ID<br>PREFERENCES_CURRENT | PREFERENCEID<br>관계가 아닙니다. 내부 응용 프로그램 용도로 사용됩니다. <br>자체</td>
    </tr>
    <tr>
        <td>UI 그룹 기준</td>
        <td>그룹화</td>
        <td>UIGB | 그룹화</td>
        <td>UIGROUPYS_CURRENT<br>UIGROUPYS_DAILY_HISTORY<br>UIGROPBYS_EVENT</td>
        <td>ENTEREDBYID<br>GROUPID <br>LASTUPDATEDBYID <br>SYSID <br>UITEMPLATEID(자체)</td>
        <td>USERS_CURRENT | USERID<br>GROUPS_CURRENT | GROUPID <br>USERS_CURRENT | USERID <br>관계가 아님, 내부 응용 프로그램 용도로 사용됨 <br>자체</td>
    </tr>
    <tr>
        <td>UI 템플릿</td>
        <td>레이아웃 템플릿</td>
        <td>UITMPL | 레이아웃 템플릿</td>
        <td>UITEMPLATES_CURRENT<br>UITEMPLATES_DAILY_HISTORY<br>UITEMPLATES_EVENT</td>
        <td>APPGLOBALID<br>ENTEREDBYID <br>LASTUPDATEDBYID <br>OBJID<br>PREFERENCEID<br>SYSID <br>UIGROUPBYID(자체)</td>
        <td>관계가 아닙니다. 내부 응용 프로그램 용도로 사용됩니다<br>USERS_CURRENT | USERID <br>USERS_CURRENT | USERID <br>OBJCODE 필드에서 식별된 개체의 ID<br>PREFERENCES_CURRENT | PREFERENCEID<br>관계가 아닙니다. 내부 응용 프로그램 용도로 사용됩니다. <br>자체</td>
    </tr>
    <tr>
        <td>UI 보기</td>
        <td>보기</td>
        <td>UIVIEW | 보기</td>
        <td>UIVIEWS_CURRENT<br>UIVIEWS_DAILY_HISTORY<br>UIVIEWS_EVENT</td>
        <td>APPGLOBALID<br>ENTEREDBYID <br>LASTUPDATEDBYID <br>OBJID<br>PREFERENCEID<br>SYSID <br>UIVIEWID(자체)</td>
        <td>관계가 아닙니다. 내부 응용 프로그램 용도로 사용됩니다<br>USERS_CURRENT | USERID <br>USERS_CURRENT | USERID <br>OBJCODE 필드에서 식별된 개체의 ID<br>PREFERENCES_CURRENT | PREFERENCEID<br>관계가 아닙니다. 내부 응용 프로그램 용도로 사용됩니다. <br>자체</td>
    </tr>
    <tr>
        <td>사용자</td>
        <td>사용자</td>
        <td>사용자 | 사용자</td>
        <td>USERS_CURRENT<br>USERS_DAILY_HISTORY<br>USERS_EVENT<br>USERS_CUSTOM_VALUE_CURRENT<br>USERS_CUSTOM_VALUE_DAILY_HISTORY<br>USERS_CUSTOM_VALUE_EVENT</td>
        <td>ACCESSLEVELID<br>CATEGORYID<br>COMPANYID<br>DEFAULTHORTYPEID<br>DELEGATIONTOID<br>EAUTHUSERID<br>ENTEREDBYID<br>HOMEGROUPID<br>HOMETEMAID<br>LATESTUREDNOTEID<br>LASTUPDATEDBYID<br>LATESTUPDATENOTEID<br>LAYOUTTEMPLATEID<br>MANAGERID<br>PORTALPROFILEID<br>PREFUIID<br>PRIVATERATECARDID<br>RESOURCEOLIPOD<br>ROLEID <br>SCHEDULEID<br>TIMESHEETPROFILEID<br>UITEMPLATEID<br>USERID<br>UUSERID</td>
        <td>ACCESSLEVELS_CURRENT |ACCESSLEVELID<br>CATEGORIES_CURRENT | CATEGORYID<br>COMPANIES_CURRENT | COMPANYID <br>HOURTYPE_CURRENT | HOURTYPEID<br>USER_CURRENT | USERID<br>관계가 아님, 내부 응용 프로그램 용도로 사용됨<br>USER_CURRENT | USERID<br>GROUP_CURRENT | GROUPID<br>TEAM_CURRENT | TEAMID<br>NOTE_CURRENT | NOTEID<br>USER_CURRENT | USERID<br>NOTE_CURRENT | NOTEID<br>레이아웃 템플릿 테이블이 지원되지 않습니다<br>USER_CURRENT | USERID<br>포털 프로필 테이블이 지원되지 않습니다<br>관계가 없습니다. 내부 응용 프로그램 용도로 사용됨<br>RATECARD_CURRENT | RATECARDID<br>RESOURCEPOOLS_CURRENT | RESOURCEPOOLID<br>ROLE_CURRENT | ROLEID<br>SCHEDULE_CURRENT | SCHEDULEID<br>TIMESHEETPROFILES_CURRENT | TIMESHEETPROFILEID<br>UITEMPLATES_CURRENT |UITEMPLATEID<br>자체<br>관계가 아닙니다. 내부 응용 프로그램 용도로 사용됩니다.</td>
    </tr>
    <tr>
        <td>사용자 위임</td>
        <td>사용자 위임</td>
        <td>우르델 | 사용자 위임</td>
        <td>USERDELEGATIONS_CURRENT<br>USERDELEGATIONS_DAILY_HISTORY<br>USERDELEGATIONS_EVENT</td>
        <td>FROMUSERID<br>SYSID <br>TOUSERID <br>USERDELEGATIONID(자체)</td>
        <td>USERS_CURRENT | USERID<br>관계가 아님, 내부 응용 프로그램 용도로 사용됨 <br>USERS_CURRENT | 사용자 ID <br>Self</td>
    </tr>
    <tr>
        <td>사용자 그룹</td>
        <td>기타 그룹</td>
        <td>USRGPS | 사용자 그룹</td>
        <td>USERSGROUPS_CURRENT<br>USERSGROUPS_DAILY_HISTORY<br>USERSGROUPS_EVENT</td>
        <td>GROUPID <br>SYSID<br>사용자 ID <br>사용자 GROUPID(자체)</td>
        <td>GROUPS_CURRENT | GROUPID <br>관계가 아님, 내부 응용 프로그램 용도로 사용됨<br>USERS_CURRENT | 사용자 ID <br>Self</td>
    </tr>
    <tr>
        <td>사용자 위치</td>
        <td>사용자 위치</td>
        <td>USRLOC | 사용자 위치</td>
        <td>USERLOCATIONS_CURRENT<br>USERLOCATIONS_DAILY_HISTORY<br>USERLOCATIONS_EVENT</td>
        <td>CLASSIFIERID<br>SYSID<br>USERID<br>USERLOCATIONID(자체)</td>
        <td>CLASSIFIER_CURRENT | CLASSIFIERID<br>관계가 아님, 내부 응용 프로그램 용도로 사용됨<br>USERS_CURRENT | USERID<br>Self</td>
    </tr>
    <tr>
        <td>사용자 역할</td>
        <td>기타 역할</td>
        <td>USRROL | 사용자 역할</td>
        <td>USERSROLES_CURRENT<br>USERSROLES_DAILY_HISTORY<br>USERSROLES_EVENT</td>
        <td>ROLEID <br>SYSID<br>사용자 ID    <br>USERROLESEID<br>USERSROLEID(자체)</td>
        <td>ROLES_CURRENT | ROLEID <br>관계가 아님, 내부 응용 프로그램 용도로 사용됨<br>USERS_CURRENT | 사용자 ID    <br>USERROLESET_CURRENT | USERROLESETID<br>자가</td>
    </tr>
    <tr>
        <td>UserPrefValue</td>
        <td>UserPrefValue</td>
        <td>USERPF | 사용자 환경 설정</td>
        <td>USERPREFVALUES_CURRENT<br>USERPREFVALUES_DAILY_HISTORY<br>USERPREFVALUES_EVENT</td>
        <td>SYSID    <br>USERID <br>USERPREFVALUEID(자체)</td>
        <td>관계가 아닙니다. 내부 응용 프로그램 용도로 사용됩니다<br>USERS_CURRENT | 사용자 ID    <br>자가</td>
    </tr>
    <tr>
        <td>사용자 역할 집합</td>
        <td>사용자 역할 집합</td>
        <td>URSET | 사용자 역할 집합</td>
        <td>USERROLESET_CURRENT<br>USERROLESET_DAILY_HISTORY<br>USERROLESET_EVENT</td>
        <td>PRIMARYROLEID <br>SYSID<br>사용자 ID    <br>USERROLESEID(자체)</td>
        <td>ROLES_CURRENT | ROLEID <br>관계가 아님, 내부 응용 프로그램 용도로 사용됨<br>USERS_CURRENT | 사용자 ID <br>Self</td>
    </tr>
    <tr>
        <td>사용자 결정</td>
        <td>사용자 결정</td>
        <td>USRDEC | 사용자 의사 결정</td>
        <td>USERSDECISIONS_CURRENT<br>USERSDECISIONS_DAILY_HISTORY<br>USERSDECISIONS_EVENT</td>
        <td>USERDECISIONID(자체)<br>SYSID <br>USERID  </td>
        <td>자체<br>관계가 아님, 내부 응용 프로그램 용도로 사용됨 <br>USERS_CURRENT | 사용자 ID </td>
    </tr>
    <tr>
        <td>작업 항목</td>
        <td>작업 항목</td>
        <td>WRKITM | 작업 항목</td>
        <td>WORKITEMS_CURRENT<br>WORKITEMS_DAILY_HISTORY<br>WORKITEMS_EVENT</td>
        <td>ASSIGNMENTID <br>OBJID<br>OPTASKID    <br>PROJECTID <br>SYSID<br>TASKID    <br>USERID <br>WORKITEMID(자체)</td>
        <td>ASSIGNMENTS_CURRENT | ASSIGNMENTID <br>OBJOBJCODE 필드에서 식별된 개체의 ID<br>OPTASK_CURRENT | OPTASKID    <br>PROJECTS_CURRENT | PROJECTID <br>관계가 아님, 내부 응용 프로그램 용도로 사용됨<br>TASKS_CURRENT | TASKID    <br>USERS_CURRENT | 사용자 ID    <br>자가 </td>
    </tr>
  </tbody>
</table>
