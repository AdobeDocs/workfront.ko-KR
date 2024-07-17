---
content-type: api
navigation-topic: api-navigation-topic
title: API 버전 15의 새로운 기능
description: Adobe Workfront은 2022년 6월 14일에 API 버전 14를 출시했습니다. API 버전 15에는 버전 14의 다음 변경 사항이 포함되어 있습니다.
author: Becky
feature: Workfront API
role: Developer
exl-id: 1cfdc136-f3b4-4beb-b58b-f546a5510e6d
source-git-commit: 3e339e2bfb26e101f0305c05f620a21541394993
workflow-type: tm+mt
source-wordcount: '2286'
ht-degree: 0%

---

# API 버전 15의 새로운 기능

Adobe Workfront은 2022년 6월 14일에 API 버전 15를 출시했습니다. API 버전 15에는 버전 14의 다음 변경 사항이 포함되어 있습니다.

## 추가된 리소스

* [이니셔티브(INITIV)](#Initiati)

* [IssueDef (ISSDEF)](#IssueDef)

* [ObjectIntegration(OBJINT)](#ObjectIn)

* [RichTextGroupParameterValue(GRCVAL)](#RichText)

* [TaskDef(TSKDEF)](#TaskDef)

* [UserApproval (USPRAPV)](#UserAppr)

### 이니셔티브(INITIV)

이 이니셔티브 오브젝트는 Workfront 시나리오 플래너에서 작업 역할의 종류와 수, 고정 비용 및 계획된 혜택에 대한 예상치를 생성합니다.

이니셔티브에 대한 자세한 내용은 시나리오 플래너의 [이니셔티브 개요](../../scenario-planner/initiatives-overview.md)를 참조하십시오.

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">직접 필드</td>
      <td>
        <ul>
          <li>
            <p><b>customerID</b>
            </p>
            <p>내부 개체입니다.</p>
          </li>
          <li>
            <p><b>기간</b>
            </p>
            <p>endDate와 startDate 사이의 시간입니다.</p>
          </li>
          <li>
            <p><b>endDate</b>
            </p>
            <p>이니셔티브의 계획된 완료 일자.</p>
          </li>
          <li>
            <p><b>enteredByID</b>
            </p>
            <p>요청을 제출한 사용자와 연계된 ID.</p>
          </li>
          <li>
            <p><b>ID</b>
            </p>
            <p>작업과 연결된 ID</p>
          </li>
          <li>
            <p><b>initiativeID</b>
            </p>
            <p>이니셔티브와 연계된 ID.</p>
          </li>
          <li>
            <p><b>lastPublishedDate</b>
            </p>
            <p>Workfront 시나리오 플래너에 이니셔티브가 마지막으로 게시된 날짜입니다.</p>
          </li>
          <li>
            <p><b>이름</b>
            </p>
            <p>이니셔티브 이름</p>
          </li>
          <li>
            <p><b>planID</b>
            </p>
            <p>이니셔티브와 연계된 플랜의 ID.</p>
          </li>
          <li>
            <p><b>planName</b>
            </p>
            <p>이니셔티브와 연계된 플랜의 이름입니다.</p>
          </li>
          <li>
            <p><b>projectID</b>
            </p>
            <p>이니셔티브와 연계된 프로젝트의 ID.</p>
          </li>
          <li>
            <p><b>scenarioID</b>
            </p>
            <p>이니셔티브와 연결된 Workfront 시나리오 플래너에 있는 시나리오의 ID입니다.</p>
          </li>
          <li>
            <p><b>startDate</b>
            </p>
            <p>이니셔티브의 계획된 시작 일자입니다.</p>
          </li>
        </ul>
      </td>
    </tr>
    <tr>
      <td role="rowheader">참조 필드</td>
      <td >
        <ul>
          <li>
            <p><b>고객</b>
            </p>
          </li>
          <li>
            <p><b>입력한 사람</b>
            </p>
          </li>
          <li>
            <p><b>프로젝트</b>
            </p>
          </li>
        </ul>
      </td>
    </tr>
    <tr>
      <td role="rowheader">코어 필드</td>
      <td>
        <ul>
          <li>
            <p><b>ID</b>
            </p>
          </li>
          <li>
            <p><b>이름</b>
            </p>
          </li>
          <li>
            <p><b>objCode</b>
            </p>
          </li>
        </ul>
      </td>
    </tr>
    <tr>
      <td role="rowheader">작업</td>
      <td>
        <ul>
          <li>
            <p><b>COUNT</b>
            </p>
          </li>
          <li>
            <p><b>GET</b>
            </p>
          </li>
          <li>
            <p><b>보고서 </b>
            </p>
          </li>
          <li>
            <p><b>검색</b>
            </p>
          </li>
        </ul>
      </td>
    </tr>
  </tbody>
</table>

### IssueDef (ISSDEF)

IssueDef 개체는 문제 형식과 관련된 데이터 집합을 나타냅니다. 이 개체는 프로젝트 또는 템플릿에 첨부할 수 있으며, 해당 프로젝트 또는 템플릿에 추가된 문제에 영향을 줍니다.

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">직접 필드</td>
      <td>
        <ul>
          <li>
            <p><b>ID</b>
            </p>
          </li>
          <li>
            <p><b>isInlineAddEnabled</b>
            </p>
          </li>
        </ul>
      </td>
    </tr>
    <tr>
      <td role="rowheader">코어 필드</td>
      <td>
        <ul>
          <li>
            <p><b>ID</b>
            </p>
          </li>
          <li>
            <p><b>objCode</b>
            </p>
          </li>
        </ul>
      </td>
    </tr>
  </tbody>
</table>

### ObjectIntegration(OBJINT)

경우에 따라 Workfront 작업 항목을 외부 소프트웨어 제품의 개체에 직접 연결할 수 있습니다. ObjectIntegration 개체는 이 링크를 나타냅니다.

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">직접 필드</td>
      <td>
        <ul>
          <li>
            <p><b>customerID</b>
            </p>
            <p>내부 개체입니다.</p>
          </li>
          <li>
            <p><b>entryDate</b>
            </p>
            <p>ObjectIntegration이 Workfront 시스템에 입력된 날짜 및 시간입니다.</p>
          </li>
          <li>
            <p><b>ID</b>
            </p>
            <p>특정 ObjectIntegration 개체의 고유한 Workfront ID입니다.</p>
          </li>
          <li>
            <p><b>integrationType</b>
            </p>
            <p>ObjectIntegration 개체가 링크를 만드는 외부 소프트웨어입니다. 가능한 값:</p>
            <ul>
              <li>
                <p>JRA</p>
              </li>
              <li>
                <p>SALESFORCE</p>
              </li>
              <li>
                <p>ANAPLAN</p>
              </li>
            </ul>
          </li>
          <li>
            <p><b>linkedObjectID</b>
            </p>
          </li>
          <li>
            <p><b>objID</b>
            </p>
            <p>ObjectIntegration이 연결된 Workfront의 개체입니다.</p>
          </li>
          <li>
            <p><b>objObjCode</b>
            </p>
            <p>ObjectIntegration이 연결된 Workfront에 있는 객체의 객체 코드입니다.</p>
          </li>
          <li>
            <p><b>param1</b>
            </p>
          </li>
          <li>
            <p><b>param2</b>
            </p>
          </li>
          <li>
            <p style="font-weight: bold;">param3</p>
          </li>
          <li>
            <p><b>URL</b>
            </p>
          </li>
        </ul>
      </td>
    </tr>
    <tr>
      <td role="rowheader">참조 필드</td>
      <td >
        <ul>
          <li>
            <p><b>고객</b>
            </p>
          </li>
        </ul>
      </td>
    </tr>
    <tr>
      <td role="rowheader">코어 필드</td>
      <td>
        <ul>
          <li>
            <p><b>ID</b>
            </p>
          </li>
          <li>
            <p><b>objCode</b>
            </p>
          </li>
        </ul>
      </td>
    </tr>
  </tbody>
</table>

### TaskDef(TSKDEF)

TaskDef 개체는 작업 형식에 대한 데이터 집합을 나타냅니다. 이 개체는 프로젝트 또는 템플릿에 첨부할 수 있으며, 해당 프로젝트 또는 템플릿에 추가된 작업에 영향을 줍니다.

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">직접 필드</td>
      <td>
        <ul>
          <li>
            <p><b>autoCalcPlannedHours </b>
            </p>
          </li>
          <li>
            <p><b>ID</b>
            </p>
          </li>
        </ul>
      </td>
    </tr>
    <tr>
      <td role="rowheader">참조 필드</td>
      <td >
        <ul>
          <li>
            <p><b>defaultApprovalProcess </b>
            </p>
          </li>
        </ul>
      </td>
    </tr>
    <tr>
      <td role="rowheader">컬렉션 필드</td>
      <td>
        <ul>
          <li>
            <p><b>개체 범주
</b>
            </p>
          </li>
        </ul>
      </td>
    </tr>
    <tr>
      <td role="rowheader">코어 필드</td>
      <td>
        <ul>
          <li>
            <p><b>ID</b>
            </p>
          </li>
          <li>
            <p><b>objCode</b>
            </p>
          </li>
        </ul>
      </td>
    </tr>
  </tbody>
</table>

### UserApproval (USPRAPV)

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">직접 필드 </td>
      <td>
        <ul>
          <li>
            <p><b>approverID</b>
            </p>
          </li>
          <li>
            <p><b>customerID</b>
            </p>
          </li>
          <li>
            <p><b>ID</b>
            </p>
          </li>
          <li>
            <p><b>requestedDate</b>
            </p>
          </li>
          <li>
            <p><b>요청자 ID</b>
            </p>
          </li>
          <li>
            <p><b>상태</b>
            </p>
          </li>
          <li>
            <p><b>사용자 ID</b>
            </p>
          </li>
        </ul>
      </td>
    </tr>
    <tr>
      <td role="rowheader">참조 필드</td>
      <td >
        <ul>
          <li>
            <p><b>승인자</b>
            </p>
          </li>
          <li>
            <p><b>고객</b>
            </p>
          </li>
          <li>
            <p><b>요청자</b>
            </p>
          </li>
          <li>
            <p><b>사용자</b>
            </p>
          </li>
        </ul>
      </td>
    </tr>
    <tr>
      <td role="rowheader">코어 필드</td>
      <td>
        <ul>
          <li>
            <p><b>ID</b>
            </p>
          </li>
          <li>
            <p><b>objCode</b>
            </p>
          </li>
        </ul>
      </td>
    </tr>
    <tr>
      <td role="rowheader">기본 필드</td>
      <td >
        <ul>
          <li>
            <p><b>approverID</b>
            </p>
          </li>
          <li>
            <p><b>요청자 ID</b>
            </p>
          </li>
          <li>
            <p><b>상태</b>
            </p>
          </li>
          <li>
            <p><b>사용자 ID</b>
            </p>
          </li>
        </ul>
      </td>
    </tr>
    <tr>
      <td role="rowheader">액션</td>
      <td>
        <ul>
          <li>
            <p><b>승인</b>
            </p>
          </li>
          <li>
            <p><b>거부</b>
            </p>
          </li>
        </ul>
      </td>
    </tr>
    <tr>
      <td role="rowheader">작업</td>
      <td>
        <ul>
          <li>
            <p><b>추가</b>
            </p>
          </li>
          <li>
            <p><b>COUNT</b>
            </p>
          </li>
          <li>
            <p><b>DELETE</b>
            </p>
          </li>
          <li>
            <p><b>GET</b>
            </p>
          </li>
          <li>
            <p><b>보고서</b>
            </p>
          </li>
          <li>
            <p><b>검색</b>
            </p>
          </li>
        </ul>
      </td>
    </tr>
  </tbody>
</table>

## 제거된 리소스

API 버전 15에 대해 제거된 리소스가 없습니다.

## 수정된 리소스

* [액세스 수준(ACSLVL)](#AccessLe)

* [AccessLevelPermissions(ALVPER)](#AccessLe2)

* [AccessRequest(ACSREQ)](#AccessRe)

* [AccessRule(ACSRUL)](#AccessRu)

* [승인(승인)](#Approval)

* [범주(CTGY)](#Category)

* [CategoryParameter(CTGAA)](#Category2)

* [CustomerPreferences (CUSTPR)](#Customer)

* [DocumentFolder(DOCFDR)](#Document)

* [DocumentVersion (DOCV)](#Document2)

* [그룹(그룹)](#Group)

* [저널 게시물(JRNL)](#JournalE)

* [LinkedFolder(LNKFDR)](#LinkedFo)

* [OpTask / 문제 (OPTASK)](#OpTask)

* [매개 변수(매개 변수)](#Paramete)

* [Portfolio(포트)](#Portfoli)

* [프로그램(PRGM)](#Program)

* [프로젝트(프로젝트)](#Project)

* [QueueDef(QUED)](#QueueDef)

* [ScoreCardQuestion(SCORREQ)](#ScoreCar)

* [작업(작업)](#Task)

* [템플릿(TMPL)](#Template)

* [타임시트(세트)](#Timeshee)

* [보기(UIVIEW)](#View)

* [업데이트(업데이트)](#Update)

* [사용자(사용자)](#User)

* [UserNote(USRNOT)](#UserNote)

* [작업(작업)](#Work)

### 액세스 수준(ACSLVL)

AccessLevel 개체는 사용자와 연결되어 있으며 사용자가 액세스할 수 있는 항목을 결정하는 AccessLevelPermissions 집합에 대해 설명합니다.

액세스 수준에 대한 자세한 내용은 [액세스 수준](../../administration-and-setup/add-users/access-levels-and-object-permissions/access-levels.md)을 참조하세요.

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">직접 필드</td>
      <td>
        <ul>
          <li>
            <p><b>fieldAccessPrivileges</b>(string[])</p>
            <p>다음과 같은 가능한 값이 추가되었습니다.</p>
            <ul>
              <li>
                <p>VTMAWMG(내 그룹과 관련된 팀 보기)</p>
              </li>
              <li>
                <p>VALLTM (모든 팀 보기)</p>
              </li>
            </ul>
          </li>
        </ul>
      </td>
    </tr>
  </tbody>
</table>

### AccessLevelPermissions(ALVPER)

AccessLevelPermissions 개체는 Workfront 개체에 액세스, 만들기 또는 수정할 수 있는 특정 권한을 나타냅니다. 그런 다음 이러한 권한을 액세스 수준과 연결할 수 있습니다.

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">직접 필드</td>
      <td>
        <ul>
          <li>
            <p><b>coreAction</b>(string[])</p>
            <p>다음과 같은 가능한 값이 추가되었습니다.</p>
            <ul>
              <li>
                <p>EDIT_TEAMS_I_AM_ON(내가 속한 팀 편집)</p>
              </li>
              <li>
                <p>EDIT_TEAMS_I_GROUP_ADMIN(내가 관리하는 그룹의 팀 편집(그룹 관리자만))</p>
              </li>
            </ul>
          </li>
          <li>
            <p><b>forbiddenActions</b>(문자열[])</p>
            <p>다음과 같은 가능한 값이 추가되었습니다.</p>
            <ul>
              <li>
                <p>EDIT_TEAMS_I_AM_ON(내가 속한 팀 편집)</p>
              </li>
              <li>
                <p>EDIT_TEAMS_I_GROUP_ADMIN(내가 관리하는 그룹의 팀 편집(그룹 관리자만))</p>
              </li>
            </ul>
          </li>
          <li>
            <p><b>secondaryActions</b>(string[])</p>
            <p>다음과 같은 가능한 값이 추가되었습니다.</p>
            <ul>
              <li>
                <p>EDIT_TEAMS_I_AM_ON(내가 속한 팀 편집)</p>
              </li>
              <li>
                <p>EDIT_TEAMS_I_GROUP_ADMIN(내가 관리하는 그룹의 팀 편집(그룹 관리자만))</p>
              </li>
            </ul>
          </li>
        </ul>
      </td>
    </tr>
  </tbody>
</table>

### AccessRequest(ACSREQ)

사용자에게 Workfront의 필요한 오브젝트에 대한 액세스 권한이 없는 경우 해당 오브젝트에 대한 액세스를 요청할 수 있습니다. AccessRequest 개체는 이 요청을 나타냅니다.

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">직접 필드</td>
      <td>
        <ul>
          <li>
            <p><b>action</b>(문자열)</p>
            <p>다음과 같은 가능한 값이 추가되었습니다.</p>
            <ul>
              <li>
                <p>EDIT_TEAMS_I_AM_ON(내가 속한 팀 편집)</p>
              </li>
              <li>
                <p>EDIT_TEAMS_I_GROUP_ADMIN(내가 관리하는 그룹의 팀 편집(그룹 관리자만))</p>
              </li>
            </ul>
          </li>
          <li>
            <p><b>autoShareAction</b>(문자열)</p>
            <p>다음과 같은 가능한 값이 추가되었습니다.</p>
            <ul>
              <li>
                <p>WDL</p>
              </li>
            </ul>
          </li>
        </ul>
      </td>
    </tr>
  </tbody>
</table>

### AccessRule(ACSRUL)

AccessRule 개체는 사용자가 만드는 프로젝트를 공유할 수 있는 방법을 결정하는 사용자 지정 액세스 수준에 설정된 규칙을 나타냅니다.

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">직접 필드</td>
      <td>
        <ul>
          <li>
            <p><b>coreAction</b>(string[])</p>
            <p>다음과 같은 가능한 값이 추가되었습니다.</p>
            <ul>
              <li>
                <p>EDIT_TEAMS_I_AM_ON(내가 속한 팀 편집)</p>
              </li>
              <li>
                <p>EDIT_TEAMS_I_GROUP_ADMIN(내가 관리하는 그룹의 팀 편집(그룹 관리자만))</p>
              </li>
            </ul>
          </li>
          <li>
            <p><b>forbiddenActions</b>(문자열[])</p>
            <p>다음과 같은 가능한 값이 추가되었습니다.</p>
            <ul>
              <li>
                <p>EDIT_TEAMS_I_AM_ON(내가 속한 팀 편집)</p>
              </li>
              <li>
                <p>EDIT_TEAMS_I_GROUP_ADMIN(내가 관리하는 그룹의 팀 편집(그룹 관리자만))</p>
              </li>
            </ul>
          </li>
          <li>
            <p><b>secondaryActions</b>(string[])</p>
            <p>다음과 같은 가능한 값이 추가되었습니다.</p>
            <ul>
              <li>
                <p>EDIT_TEAMS_I_AM_ON(내가 속한 팀 편집)</p>
              </li>
              <li>
                <p>EDIT_TEAMS_I_GROUP_ADMIN(내가 관리하는 그룹의 팀 편집(그룹 관리자만))</p>
              </li>
            </ul>
          </li>
        </ul>
      </td>
    </tr>
  </tbody>
</table>

### 승인(승인)

작업, 문서 또는 타임시트와 같은 특정 작업 항목에서는 감독자 또는 다른 사용자가 해당 작업 항목을 승인해야 할 수 있습니다. 승인 오브젝트는 작업 항목에 대한 사인오프 작업을 나타냅니다.

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">직접 필드</td>
      <td>
        <ul>
          <li>
            <p><b>resourcePlannerBudgetedHours </b>
            </p>
          </li>
        </ul>
      </td>
    </tr>
    <tr>
      <td role="rowheader">참조 필드</td>
      <td >
        <ul>
          <li>
            <p><b>이니셔티브</b>
            </p>
            <p>추가됨.</p>
            <p>이 이니셔티브 오브젝트는 Workfront 시나리오 플래너에서 작업 역할의 종류와 수, 고정 비용 및 계획된 혜택에 대한 예상치를 생성합니다. </p>
          </li>
          <li>
            <p><b>issueDef</b>
            </p>
            <p>추가됨.</p>
          </li>
          <li>
            <p><b>taskDef</b>
            </p>
            <p>추가됨.</p>
          </li>
        </ul>
      </td>
    </tr>
    <tr>
      <td role="rowheader">컬렉션 필드</td>
      <td>
        <ul>
          <li>
            <p style="font-weight: bold;"><b>objectIntegration
</b>
            </p>
            <p style="font-weight: normal;">추가됨.</p>
            <p>경우에 따라 Workfront 작업 항목을 외부 소프트웨어 제품의 개체에 직접 연결할 수 있습니다. ObjectIntegration 개체는 이 링크를 나타냅니다.</p>
          </li>
        </ul>
      </td>
    </tr>
  </tbody>
</table>

### 범주(CTGY)

Category 객체는 사용자 정의 양식입니다.

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">직접 필드</td>
      <td>
        <ul>
          <li>
            <p><b>catObjCode</b>(문자열)</p>
            <p>다음과 같은 가능한 값이 추가되었습니다.</p>
            <ul>
              <li>
                <p>GROUP(그룹)</p>
              </li>
            </ul>
          </li>
          <li>
            <p><b>objTypes</b> (string[])</p>
            <p>추가됨.</p>
            <p style="font-weight: normal;">이 매개 변수는 사용자 정의 양식을 첨부할 수 있는 가능한 객체의 배열입니다. 여러 유형의 오브젝트에 사용자 정의 양식을 첨부할 수 있는 기능을 지원하기 위해 추가되었습니다.</p>
            <p>가능한 값: </p>
            <p>CMPY, 포트, PRGM, 프로젝트, 작업, OPTASK, 사용자, DOCU, EXPNS, ITRN, BILL, 그룹</p>
          </li>
        </ul>
      </td>
    </tr>
    <tr>
      <td role="rowheader">컬렉션 필드</td>
      <td>
        <ul>
          <li>
            <p><b>objTypes</b> (string[])</p>
            <p>추가됨.</p>
            <p style="font-weight: normal;">이 매개 변수는 사용자 정의 양식을 첨부할 수 있는 가능한 객체의 배열입니다. 여러 유형의 오브젝트에 사용자 정의 양식을 첨부할 수 있는 기능을 지원하기 위해 추가되었습니다.</p>
            <p>가능한 값: </p>
            <p>CMPY, 포트, PRGM, 프로젝트, 작업, OPTASK, 사용자, DOCU, EXPNS, ITRN, BILL, 그룹</p>
          </li>
        </ul>
      </td>
    </tr>
  </tbody>
</table>

### CategoryParameter(CTGAA)

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">직접 필드</td>
      <td>
        <ul>
          <li>
            <p><b>hideFormulaFromDescription</b>
            </p>
            <p>추가됨.</p>
          </li>
          <li>
            <p><b>journaledObjCodes</b>
            </p>
            <p>추가됨.</p>
          </li>
          <li>
            <p><b>rawCustomExpression</b>
            </p>
            <p>추가됨.</p>
          </li>
        </ul>
      </td>
    </tr>
  </tbody>
</table>

### CustomerPreferences (CUSTPR)

CustomerPreferences 객체는 고객이 Workfront 인스턴스에 대해 설정한 환경 설정 집합을 나타냅니다.

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">직접 필드</td>
      <td>
        <ul>
          <li>
            <p><b>이름</b>
            </p>
            <p>다음 값이 추가되었습니다.</p>
            <ul>
              <li>
                <p><code>password:sharePointV2IntegrationEnabled</code> (SharePoint(Graph API) 통합 활성화됨)</p>
                <p>이 값은 업데이트된 Sharepoint 통합을 지원합니다.</p>
              </li>
              <li>
                <p><code>project.mgmt:default.project.allowcreatewithouttemplate</code> (사용자가 템플릿을 사용하지 않고 프로젝트를 만들 수 있도록 허용)</p>
              </li>
              <li>
                <p><code>project.mgmt:taskissue.delegate</code> (config.taskissue.delegate)</p>
              </li>
            </ul>
          </li>
        </ul>
      </td>
    </tr>
  </tbody>
</table>

### DocumentFolder(DOCFDR)

문서를 폴더로 구성할 수 있습니다. 개인 문서 영역에 개인 폴더를 만들 수 있습니다. DocumentFolder 개체는 이러한 폴더 중 하나를 나타냅니다.

DocumentFolder 개체가 `SHARABLE` 플래그를 추가했습니다.

### DocumentVersion (DOCV)

DocumentVersion 개체는 작성된 자료, 이미지 또는 다른 형태의 정보 등 파일의 특정 버전을 나타냅니다.

문서 버전에 대한 자세한 내용은 [새 문서 버전 업로드](../../documents/managing-documents/upload-new-document-version.md)를 참조하십시오.

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">직접 필드</td>
      <td>
        <ul>
          <li>
            <p><b>externalIntegrationType</b>
            </p>
            <p>다음 값이 추가되었습니다. </p>
            <ul>
              <li>
                <p><code>SHAREPOINT_V2</code> (SharePoint (Graph API))</p>
                <p>이 값은 업데이트된 Sharepoint 통합을 지원합니다.</p>
              </li>
            </ul>
          </li>
        </ul>
      </td>
    </tr>
  </tbody>
</table>

### 그룹(그룹)

Group 객체는 사용자 및 팀 집합을 나타냅니다. 그룹은 종종 부서 구조를 나타냅니다.

그룹에 대한 자세한 내용은 그룹 및 팀 을 참조하십시오.

Group 개체가 `DATA_EXTENDIBLE` 플래그를 추가했습니다.

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">직접 필드</td>
      <td>
        <p>다음 필드가 추가되었습니다.</p>
        <ul>
          <li>
            <p><b>categoryID</b>
            </p>
            <p>범주는 사용자 정의 양식입니다. 이 매개 변수는 그룹 개체에 사용자 지정 Forms을 추가하는 기능을 지원하기 위해 추가되었습니다. </p>
          </li>
          <li>
            <p><b>isActive</b>
            </p>
            <p>객체가 활성이면 true 값을 갖고 그렇지 않으면 false 값을 갖는 부울 매개변수입니다. 활성으로 설정된 객체는 드롭다운 메뉴와 앞에 입력 필드에 나타나며 다른 객체에 첨부할 수 있습니다.</p>
          </li>
        </ul>
      </td>
    </tr>
    <tr>
      <td role="rowheader">참조 필드</td>
      <td >
        <p>다음 필드가 추가되었습니다.</p>
        <ul>
          <li>
            <p><b>승인자</b>
            </p>
          </li>
          <li>
            <p><b>고객</b>
            </p>
          </li>
          <li>
            <p><b>요청자</b>
            </p>
          </li>
          <li>
            <p><b>사용자</b>
            </p>
          </li>
        </ul>
      </td>
    </tr>
    <tr>
      <td role="rowheader">컬렉션 필드</td>
      <td>
        <p>다음 필드가 추가되었습니다.</p>
        <ul>
          <li>
            <p><b>개체 범주</b>
            </p>
          </li>
          <li>
            <p><b>objectIntegrations</b>
            </p>
            <p>경우에 따라 Workfront 작업 항목을 외부 소프트웨어 제품의 개체에 직접 연결할 수 있습니다. ObjectIntegration 개체는 이 링크를 나타냅니다.</p>
          </li>
        </ul>
      </td>
    </tr>
    <tr>
      <td role="rowheader">기본 필드</td>
      <td >
        <p>다음 필드가 추가되었습니다.</p>
        <ul>
          <li>
            <p><b>isActive</b>
            </p>
            <p>객체가 활성이면 true 값을 갖고 그렇지 않으면 false 값을 갖는 부울 매개변수입니다. 활성으로 설정된 객체는 드롭다운 메뉴와 앞에 입력 필드에 나타나며 다른 객체에 첨부할 수 있습니다.</p>
          </li>
        </ul>
      </td>
    </tr>
    <tr>
      <td role="rowheader">액션</td>
      <td>
        <p>다음 필드가 추가되었습니다.</p>
        <ul>
          <li>
            <p><b>calculateDataExtension</b>
            </p>
            <p>이 작업은 사용자 정의 양식 필드의 표현식을 다시 계산합니다.</p>
          </li>
          <li>
            <p><b>completeGroupInfo</b>
            </p>
          </li>
          <li>
            <p><b>linkExternalObject</b>
            </p>
          </li>
          <li>
            <p><b>unlinkExternalObject</b>
            </p>
          </li>
        </ul>
      </td>
    </tr>
  </tbody>
</table>

### 저널 게시물(JRNL)

JournalEntry 개체는 특정 개체 필드에 대한 정보를 해당 필드가 수정될 때마다 기록하도록 설정할 수 있습니다. 필드가 저널 게시물 개체의 일부로 기록되도록 설정되면 해당 필드를 수정할 때마다 해당 저널 게시물이 만들어집니다.

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">직접 필드</td>
      <td>
        <p><b>changeType</b>
        </p>
        <p>다음 값이 추가되었습니다. </p>
        <ul>
          <li>
            <p>DW(다운로드)</p>
          </li>
        </ul>
      </td>
    </tr>
  </tbody>
</table>

### LinkedFolder(LNKFDR)

LinkedFolder 개체는 Google 드라이브 또는 Dropbox과 같은 외부 문서 공급자로부터 연결된 폴더를 나타냅니다.

연결된 폴더에 대한 자세한 내용은 외부 응용 프로그램에서 문서 연결을 참조하십시오.

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">직접 필드</td>
      <td>
        <ul>
          <li>
            <p><b>externalIntegrationType</b>
            </p>
            <p>다음 값이 추가되었습니다. </p>
            <ul>
              <li>
                <p><code>SHAREPOINT_V2</code> (SharePoint (Graph API))</p>
                <p>이 값은 업데이트된 Sharepoint 통합을 지원합니다.</p>
              </li>
            </ul>
          </li>
        </ul>
      </td>
    </tr>
  </tbody>
</table>

### OpTask / 문제 (OPTASK)

OpTask 객체를 일반적으로 문제라고 합니다. 문제는 일반적으로 작업 또는 프로젝트의 완료를 방해하는 문제가 있음을 나타내는 작업 항목입니다. 문제는 헬프 데스크 요청일 수도 있습니다. 변경 주문, 요청 및 버그도 문제가 됩니다.

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">액션</td>
      <td>
        <p>다음 작업이 추가되었습니다.</p>
        <ul>
          <li>
            <p><b>bulkMoveWithOptions</b>
            </p>
          </li>
          <li>
            <p><b>getRequestPath</b>
            </p>
          </li>
        </ul>
        <p>다음 작업이 수정되었습니다.</p>
        <ul>
          <li>
            <p><b>복사 문제</b>
            </p>
            <p>추가된 필드 <code>parentID</code></p>
          </li>
        </ul>
      </td>
    </tr>
  </tbody>
</table>

### 매개 변수(매개 변수)

Parameter 개체는 사용자 지정 필드입니다.

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">직접 필드</td>
      <td>
        <p>다음 필드가 추가되었습니다.</p>
        <ul>
          <li>
            <p><b>fieldDefinition</b>
            </p>
          </li>
        </ul>
        <p>다음 필드가 수정되었습니다.</p>
        <ul>
          <li>
            <p><b>dataType</b>
            </p>
            <p>가능한 값 <code>WIDGET </code>(위젯)이(가) 추가되었습니다. </p>
            <p>이 값은 사용자 정의 양식에서 이미지 사용을 지원합니다.</p>
          </li>
          <li>
            <p><b>displayType</b>
            </p>
            <p>가능한 값 <code>WIDGET </code>(위젯)이(가) 추가되었습니다.</p>
            <p>이 값은 사용자 정의 양식에서 이미지 사용을 지원합니다.</p>
          </li>
        </ul>
      </td>
    </tr>
  </tbody>
</table>

### Portfolio(포트)

Portfolio 객체는 동일한 리소스(일반적으로 돈 또는 완료하는 사람)에 대해 경쟁하는 프로젝트의 컬렉션입니다.

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">컬렉션 필드</td>
      <td>
        <ul>
          <li>
            <p><b>objectIntegrations</b>
            </p>
          </li>
        </ul>
      </td>
    </tr>
    <tr>
      <td role="rowheader">액션</td>
      <td>
        <ul>
          <li>
            <p><b>linkExternalObject</b>
            </p>
          </li>
          <li>
            <p><b>unlinkExternalObject</b>
            </p>
          </li>
        </ul>
      </td>
    </tr>
  </tbody>
</table>

### 프로그램(PRGM)

프로그램 객체는 유사한 프로젝트를 함께 그룹화할 수 있는 포트폴리오 내의 프로젝트 하위 집합입니다.

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">컬렉션 필드</td>
      <td>
        <ul>
          <li>
            <p><b>objectIntegrations</b>
            </p>
          </li>
        </ul>
      </td>
    </tr>
    <tr>
      <td role="rowheader">액션</td>
      <td>
        <ul>
          <li>
            <p><b>linkExternalObject</b>
            </p>
          </li>
          <li>
            <p><b>unlinkExternalObject</b>
            </p>
          </li>
        </ul>
      </td>
    </tr>
  </tbody>
</table>

### 프로젝트(프로젝트)

프로젝트는 Workfront 내의 작업 항목이며 Workfront이 작업을 수행하는 데 도움을 주는 방식의 주요 빌딩 블록입니다. Project 개체는 일반적인 특정 목표를 가진 작업 그룹을 나타냅니다.

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">직접 필드</td>
      <td>
        <ul>
          <li>
            <p><b>resourcePlannerBudgetHours</b>
            </p>
          </li>
        </ul>
      </td>
    </tr>
    <tr>
      <td role="rowheader">참조 필드</td>
      <td >
        <ul>
          <li>
            <p><b>이니셔티브</b>
            </p>
            <p>이 이니셔티브 오브젝트는 Workfront 시나리오 플래너에서 작업 역할의 종류와 수, 고정 비용 및 계획된 혜택에 대한 예상치를 생성합니다. </p>
          </li>
          <li>
            <p><b>issueDef</b>
            </p>
          </li>
          <li>
            <p><b>taskDef</b>
            </p>
          </li>
        </ul>
      </td>
    </tr>
    <tr>
      <td role="rowheader">컬렉션 필드</td>
      <td>
        <ul>
          <li>
            <p><b>objectIntegrations</b>
            </p>
            <p>경우에 따라 Workfront 작업 항목을 외부 소프트웨어 제품의 개체에 직접 연결할 수 있습니다. ObjectIntegration 개체는 이 링크를 나타냅니다.</p>
          </li>
        </ul>
      </td>
    </tr>
  </tbody>
</table>

### QueueDef(QUED)

QueueDef 개체는 사용자가 문제를 제출할 수 있도록 헬프 데스크 영역에 게시된 프로젝트인 Queue를 나타냅니다.

요청 대기열에 대한 자세한 내용은 [요청 대기열 만들기](../../manage-work/requests/create-and-manage-request-queues/create-request-queue.md)를 참조하십시오.

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">직접 필드</td>
      <td>
        <ul>
          <li>
            <p><b>requestorCoreAction</b>
            </p>
            <p>다음과 같은 가능한 값이 추가되었습니다.</p>
            <ul>
              <li>
                <p>EDIT_TEAMS_I_AM_ON(내가 속한 팀 편집)</p>
              </li>
              <li>
                <p>EDIT_TEAMS_I_GROUP_ADMIN(내가 관리하는 그룹의 팀 편집(그룹 관리자만))</p>
              </li>
            </ul>
          </li>
          <li>
            <p><b>requestorForbiddenActions</b>
            </p>
            <p>다음과 같은 가능한 값이 추가되었습니다.</p>
            <ul>
              <li>
                <p>EDIT_TEAMS_I_AM_ON(내가 속한 팀 편집)</p>
              </li>
              <li>
                <p>EDIT_TEAMS_I_GROUP_ADMIN(내가 관리하는 그룹의 팀 편집(그룹 관리자만))</p>
              </li>
            </ul>
          </li>
        </ul>
      </td>
    </tr>
  </tbody>
</table>

### ScoreCardQuestion(SCORREQ)

ScoreCardQuestion 객체는 스코어카드에 추가된 질문을 나타냅니다. 이러한 질문은 일반적으로 Portfolio 관리자가 결정하며, 관리자는 이에 대한 답변을 통해 프로젝트가 포트폴리오의 목표에 얼마나 잘 부합하는지 파악할 수 있습니다.

스코어카드 질문에 대한 자세한 내용은 [스코어카드 만들기](../../administration-and-setup/set-up-workfront/configure-system-defaults/create-scorecard.md)를 참조하십시오.

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">직접 필드</td>
      <td>
        <ul>
          <li>
            <p><b>displayType</b>
            </p>
            <p>가능한 값 <code>WIDGET </code>(위젯)이(가) 추가되었습니다.</p>
          </li>
        </ul>
      </td>
    </tr>
  </tbody>
</table>

### 작업(작업)

작업 객체는 최종 목표 달성(프로젝트 완료)을 위한 단계로 수행해야 하는 작업 항목을 나타냅니다.

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">컬렉션 필드</td>
      <td>
        <ul>
          <li>
            <p><b>objectIntegrations</b>
            </p>
            <p>경우에 따라 Workfront 작업 항목을 외부 소프트웨어 제품의 개체에 직접 연결할 수 있습니다. ObjectIntegration 개체는 이 링크를 나타냅니다.</p>
          </li>
        </ul>
      </td>
    </tr>
  </tbody>
</table>

### 템플릿(TMPL)

Template 객체는 프로젝트의 패턴을 나타냅니다. 템플릿에서 프로젝트를 생성하여 시간을 절약할 수 있습니다. 템플릿에는 팀과 작업이 포함되어 있으며, 이 작업은 템플릿에서 만든 프로젝트에 복사됩니다.

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">참조 필드</td>
      <td>
        <ul>
          <li>
            <p><b>issueDef</b>
            </p>
          </li>
          <li>
            <p><b>taskDef</b>
            </p>
          </li>
        </ul>
      </td>
    </tr>
  </tbody>
</table>

### 타임시트(세트)

타임시트 오브젝트는 사용자가 작업, 프로젝트 및 오버헤드 시간 유형에 대한 실제 작업 시간을 입력할 수 있는 가상 타임카드를 나타냅니다.

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">코어 필드</td>
      <td>
        <p>다음 필드가 제거되었습니다.</p>
        <ul>
          <li>
            <p><b>objCode</b>
            </p>
          </li>
        </ul>
      </td>
    </tr>
  </tbody>
</table>

### 보기(UIVIEW)

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">직접 필드</td>
      <td>
        <ul>
          <li>
            <p><b>uiviewType</b>
            </p>
            <p>다음 가능한 값이 제거되었습니다.</p>
            <ul>
              <li>
                <p><code>FOUR_COL</code> (4열 레이아웃)</p>
              </li>
              <li>
                <p><code>UPDATES</code> (업데이트)</p>
              </li>
              <li>
                <p><code>UPDATESTOOLBAR_FEED</code> (업데이트)</p>
              </li>
              <li>
                <p><code>WORKINGON</code> (처리 중)</p>
              </li>
              <li>
                <p><code>CUSTOMDATA</code> (사용자 정의 데이터)</p>
              </li>
              <li>
                <p><code>CUSTOMDATA_UPDATE</code> (사용자 정의 데이터 업데이트)</p>
              </li>
              <li>
                <p><code>STATUS_UPDATE</code> (상태 업데이트)</p>
              </li>
              <li>
                <p><code>OPTASK_STATUS_UPDATE</code> (상태 업데이트)</p>
              </li>
              <li>
                <p><code>PROJ_STATUS_UPDATE</code> (상태 업데이트)</p>
              </li>
              <li>
                <p><code>PROJECT_TIMEENTRY</code> (상태 업데이트)</p>
              </li>
              <li>
                <p><code>DLIST</code> (세부 사항 목록)</p>
              </li>
              <li>
                <p><code>DLIST_SECTION</code> (세부 목록 섹션)</p>
              </li>
            </ul>
          </li>
        </ul>
      </td>
    </tr>
  </tbody>
</table>

### 업데이트(업데이트)

Workfront의 작업 항목을 업데이트하여 사용자에게 현재 상태를 알릴 수 있습니다. Update 개체는 이러한 업데이트 중 하나를 나타냅니다. 업데이트는 사용자가 입력하거나 Workfront 시스템에서 만들 수 있습니다.

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">직접 필드</td>
      <td>
        <ul>
          <li>
            <p><b>updateType</b>
            </p>
            <p>가능한 값 <code>documentVersionDownload </code>(enum.updatetypeenum.documentversiondownload)이(가) 추가되었습니다.</p>
          </li>
        </ul>
      </td>
    </tr>
  </tbody>
</table>

### 사용자(사용자)

사용자 개체는 로그인하여 시스템과 상호 작용할 수 있는 Workfront의 계정을 가진 사용자를 나타냅니다.

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">참조 필드</td>
      <td>
        <ul>
          <li>
            <p><b>userApproval</b>
            </p>
          </li>
        </ul>
      </td>
    </tr>
    <tr>
      <td role="rowheader">액션</td>
      <td>
        <ul>
          <li>
            <p><b>getUsersAvailableTime</b>
            </p>
          </li>
          <li>
            <p><b>resetRopgPassword</b>
            </p>
          </li>
        </ul>
      </td>
    </tr>
  </tbody>
</table>

### UserNote(USRNOT)

UserNote 객체는 알림입니다.

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">직접 필드</td>
      <td>
        <ul>
          <li>
            <p><b>eventType</b>
            </p>
            <p>다음과 같은 가능한 값이 추가되었습니다.</p>
            <ul>
              <li>
                <p><code>DUP </code>(문서 증명을 요청함)</p>
              </li>
              <li>
                <p><code>DUV </code>(문서를 볼 수 있음)</p>
              </li>
            </ul>
          </li>
        </ul>
      </td>
    </tr>
  </tbody>
</table>

### 작업(작업)

Work 개체는 Task와 OpTask가 모두 상속하는 공통 인터페이스이며 두 개체 간에 공통 코드를 공유합니다.

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">컬렉션 필드</td>
      <td>
        <ul>
          <li>
            <p><b>objectIntegrations</b>
            </p>
            <p>경우에 따라 Workfront 작업 항목을 외부 소프트웨어 제품의 개체에 직접 연결할 수 있습니다. ObjectIntegration 개체는 이 링크를 나타냅니다.</p>
          </li>
        </ul>
      </td>
    </tr>
  </tbody>
</table>
