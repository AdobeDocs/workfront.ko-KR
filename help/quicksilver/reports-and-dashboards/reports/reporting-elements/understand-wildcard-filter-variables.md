---
content-type: overview
product-area: reporting
navigation-topic: reporting-elements
title: 와일드카드 필터 변수
description: 필터에서 와일드카드를 사용하면 특정 사용자 또는 날짜 대신 일반 사용자 또는 날짜를 참조할 수 있습니다. 이러한 방식으로 빌드하는 요소는 동적이며 사용되는 컨텍스트에 따라 결과가 변경됩니다.
author: Nolan
feature: Reports and Dashboards
exl-id: f99cd99e-c4c1-471d-8428-c680f0e73336
source-git-commit: 548e713700fda79070f59f3dc3457410d2c50133
workflow-type: tm+mt
source-wordcount: '1446'
ht-degree: 1%

---

# 와일드카드 필터 변수 개요

<!-- Audited: 12/2023 -->

<!--
<div data-mc-conditions="QuicksilverOrClassic.Draft mode">
<p>(NOTE: This article is linked to the training self-serve promted articles for user-based and date-based widlcards (how-to articles). This serves as the "overview/ reference" article for those articles. Consider renaming this when that is allowed.) </p>
<p>(NOTE: Alina: ***&gt;&gt;Linked in other articles - do not move/ delete.</p>
<p>&gt;&gt;This was included but it is not supported???:</p>
<p>The $$USER.roleIDs variable refers to all the job roles that are associated with the logged-in user. Using this variable, you can&nbsp; items assigned to all of the job roles associated with the logged-in user.</p>
<p>For example, if you want to display tasks assigned to any of the job roles associated with the logged-in user, you can use the following filter rule in a task filter:</p>
<p>AssignedToID Equals $$USER.roleIDs.)</p>
</div>
-->

와일드카드를 사용하면 특정 사용자 또는 날짜 대신 일반 사용자 또는 날짜를 참조할 수 있습니다. 이러한 방식으로 빌드하는 요소는 동적입니다. 결과는 사용되는 컨텍스트에 따라 달라집니다.

예를 들어 프로젝트 보고서에서 $$USER.homeGroupID에 대한 필터링은 로그인한 사용자의 홈 그룹과 관련된 프로젝트만 검색합니다.

다음 요소를 작성할 때 필터 변수(와일드카드라고도 함)를 사용할 수 있습니다.

<table>
    <tr>
        <td>목록, 보고서 및 리소스 플래너의 필터</td>
        <td>Workfront 필터에 대한 자세한 내용은 문서 를 참조하십시오 <a href="../../../reports-and-dashboards/reports/reporting-elements/filters-overview.md">필터 개요</a>.
</td>
    </tr>
    <tr>
        <td>고급 검색</td>
        <td>고급 검색에 대한 자세한 내용은 섹션을 참조하십시오 <a href="../../../workfront-basics/navigate-workfront/search/search-workfront.md#using-advanced-search">고급 검색 사용</a> 이 문서에서 <a href="../../../workfront-basics/navigate-workfront/search/search-workfront.md">Adobe Workfront 검색</a>.
    </tr>
    <tr>
        <td>보기의 계산된 열</td>
        <td></td>
    </tr>
    <tr>
        <td>보기의 조건부 서식</td>
        <td>조건부 서식에 대한 자세한 내용은 문서를 참조하십시오 <a href="../../../reports-and-dashboards/reports/reporting-elements/use-conditional-formatting-views.md">보기에서 조건부 서식 사용</a>.
    </tr>
    <tr>
        <td>계산된 사용자 정의 필드</td>
        <td>계산된 열에서 중첩된 컬렉션을 참조할 때는 와일드카드 필터 변수가 지원되지 않습니다.

계산된 사용자 정의 필드 및 열에 대한 자세한 내용은 문서 를 참조하십시오 <a hreft="../../../reports-and-dashboards/reports/calc-cstm-data-reports/calculated-custom-fields-calculated-columns.md">계산된 사용자 정의 필드와 계산된 열 비교</a>.
</td>
    </tr>
</table>

## 날짜 기반 와일드카드 필터 변수

날짜 기반 와일드카드 옵션은 모든 날짜 필터 속성과 함께 사용할 수 있습니다. 보고서에 날짜 기반 와일드카드를 추가하는 방법에 대한 자세한 내용은 문서를 참조하십시오 [날짜 기반 와일드카드를 사용하여 보고서를 일반화합니다.](../../../reports-and-dashboards/reports/reporting-elements/use-date-based-wildcards-generalize-reports.md).

>[!NOTE]
>
>시간 부분을 포함하지 않거나 날짜 와일드카드 $$TODAY 또는 $$NOW를 사용하는 날짜 및 시간 계산을 만드는 경우, 시스템은 현지 시간대가 아닌 UTC(협정 세계시) 시간대에 따라 날짜를 사용합니다. 이로 인해 예상치 못한 날짜 결과가 발생할 수 있습니다.

다음 날짜 기반 와일드카드 중에서 선택할 수 있습니다.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr valign="top"> 
   <td width="100" role="rowheader"> <p><strong>$$오늘</strong> </p> </td> 
   <td> <p>내일, 다음 주 또는 다음 달에 필터를 다시 빌드하지 않도록 이 와일드카드를 사용하여 날짜 구분 필터를 빌드하는 것이 좋습니다.</p> <p>예를 들어 오늘 전에 마감된 모든 작업을 표시하려는 경우 작업 필터에서 다음 규칙을 사용할 수 있습니다. <em>계획된 시작 일자가 오늘 $$보다 작음</em>.</p> <p>$$TODAY는 현재 날짜의 자정과 항상 같습니다.</p> </td> 
  </tr> 
  <tr valign="top"> 
   <td width="100" role="rowheader"> <p><strong>$$NOW</strong> </p> </td> 
   <td> <p>$$TODAY 와일드카드와 유사하지만 현재 날짜 및 시간을 포함합니다. $$NOW는 현재 날짜 및 시간과 같습니다.</p> <p>예를 들어 현재 시간까지 제공된 모든 시간 항목을 표시하려면 시간 필터에서 다음 규칙을 사용하여 이 작업을 수행할 수 있습니다. <em>계획된 시작 일자가 $$NOW 미만임</em>.</p> <p>참고: 이 와일드카드는 리소스 플래너에서 지원되지 않습니다.</p> </td> 
  </tr> 
 </tbody> 
</table>

다양한 기간 및 다양한 시점(미래 또는 과거)을 나타내기 위해 위의 와일드카드를 다음과 결합할 수 있습니다.

| 속성 |   |
|---|---|
| **q** | 달력 분기 |
| **h** | 시간 |
| **d** | 일 |
| **w** | 주 |
| **m** | 개월 |
| **y** | 년 |

{style="table-layout:auto"}

| **한정자** | |
|---|---|
| **b** | 주 시작(일요일) |
| **e** | 주의 끝(토요일) |

{style="table-layout:auto"}

| **연산자** | |
|---|---|
| **+** | 와일드카드 값에 값 추가 |
| **-** | 와일드카드 값에서 값 빼기 |

{style="table-layout:auto"}

예: 와일드카드 `$$TODAYb+2w` 는 &quot;이번 주 초부터 2주&quot;를 나타냅니다. 와일드카드 *`$$NOW+2h` 는 &quot;지금부터 2시간 후&quot;를 나타냅니다.

## 사용자 기반 와일드카드 필터 변수

>[!IMPORTANT]
>
>필터나 보고서에 사용자 기반 와일드카드 필터 변수가 포함되어 있으면 결과는 항상 현재 로그인한 사용자가 필터링한 정보를 표시합니다. 이러한 필터 또는 보고서를 다른 사용자와 공유할 때 와일드카드는 보고서를 보는 사용자에 대한 정보를 검색합니다. 두 사용자에게 서로 다른 결과가 표시됩니다.
>
>사용자 기반 와일드카드를 보고서에 추가하는 방법에 대한 자세한 내용은 문서를 참조하십시오 [사용자 기반 와일드카드를 사용하여 보고서 일반화](../../../reports-and-dashboards/reports/reporting-elements/use-user-based-wildcards-generalize-reports.md).

다음 사용자 기반 변수 중에서 선택할 수 있습니다.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr valign="top"> 
   <td width="200" role="rowheader"> <p><strong>$$USER.ID</strong> </p> </td> 
   <td> <!--
     <p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: : should these be formatted with code?!) </p>
    --> <p>가장 일반적인 사용자 기반 변수는 $$USER.ID입니다. 로그인된 사용자의 ID가 항상 반환됩니다. 각 개체와 작업 할당을 만든 사용자를 식별하는 데 사용되는 ID입니다.</p> <p>보고서에서 사용할 경우 이 와일드카드는 시스템에서 만들어야 하는 보고서 수를 줄입니다. 하나의 보고서를 만들어 여러 사용자와 공유할 수 있으며, 결과는 로그인한 사용자와 보고서를 보고 있는 사용자에 따라 변경됩니다.</p> <p>예를 들어 로그인한 사용자에게 할당된 모든 문제에 대한 보고서를 작성하려면 문제 필터에서 다음 규칙을 사용할 수 있습니다. <em>할당 대상 ID가 $$USER.ID와 같음</em>.</p> <p>Workfront은 다음의 기본 제공 필터에서 이 변수를 사용합니다.</p> 
    <ul> 
     <li>내 보고서</li> 
     <li>내 프로젝트</li> 
     <li>내 작업</li> 
     <li>내 문제</li> 
     <li>내 시간</li> 
    </ul> </td> 
  </tr> 
  <tr valign="top"> 
   <td width="200" role="rowheader"> <p><strong>$$USER.categoryID</strong> </p> </td> 
   <td> <p>$$USER.categoryID 변수는 로그인한 사용자와 관련된 특정 사용자 정의 양식을 참조합니다.</p> </td> 
  </tr> 
  <tr valign="top"> 
   <td role="rowheader"> <p><strong>$$USER.accessLevelID</strong> </p> </td> 
   <td> <p>$$USER.accessLevelID 변수는 로그인한 사용자와 연결된 액세스 수준의 ID를 나타냅니다.</p> </td> 
  </tr> 
  <tr valign="top"> 
   <td role="rowheader"> <p><strong>$$USER.accessLevelRank</strong> </p> </td> 
   <td> <p>$$USER.accessLevelRank 변수는 로그인한 사용자와 관련된 액세스 수준 등급을 나타냅니다.</p> </td> 
  </tr> 
  <tr valign="top"> 
   <td role="rowheader"> <p><strong>$$USER.companyID</strong> </p> </td> 
   <td> <p>$$USER.companyID 변수는 로그인한 사용자와 연결된 회사를 참조합니다.</p> </td> 
  </tr> 
  <tr valign="top"> 
   <td role="rowheader"> <p><strong>$$USER.customerID</strong> </p> </td> 
   <td> <p>$$USER.customerID 변수는 환경과 연결된 고객 계정의 ID를 나타냅니다. 사용자 환경의 경우 이 변수에 사용할 수 있는 값은 하나이며, 일반적으로 API를 통해 통합을 구축할 때만 사용됩니다.</p> </td> 
  </tr> 
  <tr valign="top"> 
   <td role="rowheader"> <p><strong>$$USER.name</strong> </p> </td> 
   <td> <p>$$USER.firstName 변수는 로그인한 사용자의 이름을 나타냅니다.</p> </td> 
  </tr> 
  <tr valign="top"> 
   <td role="rowheader"> <p><strong>$$USER.lastName</strong> </p> </td> 
   <td> <p>$$USER.lastName 변수는 로그인한 사용자의 성을 나타냅니다.</p> </td> 
  </tr> 
  <tr valign="top"> 
   <td role="rowheader"> <p><strong>$$USER.name</strong> </p> </td> 
   <td> <p>$$USER.name 변수는 로그인한 사용자의 전체 이름을 나타냅니다.</p> <p>참고:   <p>이 와일드카드 변수는 텍스트 모드에서 필터를 수정하는 경우에만 작동합니다. 텍스트 모드를 지원하지 않는 필터에서는 이 와일드카드를 사용할 수 없습니다. 예를 들어 다음 영역의 필터에서는 이 와일드카드를 사용할 수 없습니다.</p> 
     <ul> 
      <li> <p>리소스 플래너</p> </li> 
      <li> <p>워크로드 밸런서</p> </li> 
      <li> <p>분석</p> </li> 
     </ul> </p> </td> 
  </tr> 
  <tr valign="top"> 
   <td role="rowheader"> <p><strong>$$USER.homeGroupID</strong> </p> </td> 
   <td> <p>$$USER.homeGroupID 변수는 로그인한 사용자의 홈 그룹 ID를 참조합니다. 그룹 관리자는 이 변수를 사용하여 홈 그룹의 사용자에 속하는 항목에 대해서만 필터링할 수 있습니다.</p> <p>예를 들어 재무 그룹의 프로젝트에서 미완료 태스크를 모두 보려면 태스크 필터에서 다음 필터 규칙을 사용합니다.<br><em>프로젝트: 그룹 ID가 $$USER.homeGroupID와 같음 </em><br><em>완료율이 100보다 작음</em></p> <p>로그인한 사용자의 홈 그룹인 특정 그룹의 개인에게 할당된 모든 미완료 작업을 보려면 작업 필터에서 다음 필터 규칙을 사용합니다.</p> <p><em>할당 대상: 그룹 ID가 $$USER.homeGroupID와 같음<br>완료율이 100보다 작음</em> </p> </td> 
  </tr> 
  <tr valign="top"> 
   <td role="rowheader"> <p><strong>$$USER.otherGroupIDs</strong> </p> </td> 
   <td> <p>$$USER.otherGroupIDs 변수는 로그인한 사용자의 프로필과 관련된 모든 그룹(홈 그룹 포함)을 참조합니다.</p> <p>이 변수의 기능은 로그인한 사용자와 관련된 그룹에 속한 사용자에 대한 정보가 결과에 표시된다는 점을 제외하면 $$USER.homeGroupID 변수의 기능과 유사합니다.</p> </td> 
  </tr> 
  <tr valign="top"> 
   <td role="rowheader"> <p><strong>$$USER.homeTeamID</strong> </p> </td> 
   <td> <p>$$USER.homeTeamID 변수는 로그인한 사용자의 홈 팀 ID를 나타냅니다. 팀 관리자는 이 변수를 사용하여 홈 팀의 사용자에 속하는 항목에 대해서만 필터링할 수 있습니다.</p> </td> 
  </tr> 
  <tr valign="top"> 
   <td role="rowheader"> <p><strong>$$USER.teamIDs</strong> </p> </td> 
   <td> <p>$$USER.teamIDs 변수는 로그인한 사용자와 연결된 모든 팀의 목록을 반환합니다.</p> <p>이 변수의 기능은 필터에서 식별된 팀에 속하는 사용자에 대한 정보를 표시하는 결과를 제외하면 $$USER.homeTeamID 변수의 기능과 유사합니다.</p> </td> 
  </tr> 
  <tr valign="top"> 
   <td role="rowheader"> <p><strong>$$USER.roleID</strong> </p> </td> 
   <td> <p>$$USER.roleID 변수는 로그인한 사용자의 기본 역할을 참조합니다. 이 변수를 사용하면 특정 작업 역할에 할당된 작업 또는 문제에 대해 보고할 수 있습니다.</p> <p>예를 들어 로그인한 사용자의 기본 역할에 할당된 모든 작업을 보려면 작업 필터에서 다음 필터 규칙을 사용할 수 있습니다.</p> <p><em>작업: 역할 ID가 $$USER.roleID와 같음.</em> </p> </td> 
  </tr> 
  <tr valign="top"> 
   <td role="rowheader"><p><strong>$$USER.roleIDs</strong></p></td> 
   <td> <p>$$USER.roleIDs 변수는 로그인한 사용자와 관련된 모든 작업 역할을 참조합니다. 이 변수를 사용하면 로그인한 사용자와 관련된 모든 작업 역할에 할당된 작업 또는 문제에 대해 보고할 수 있습니다. </p> <p>예를 들어 로그인한 사용자와 연관된 역할에 할당된 모든 작업을 보려면 작업 필터에서 다음 필터 규칙을 사용할 수 있습니다.</p> <p><i>작업: 역할 ID가 $$USERID.roleIDs와 같음<br></i> </p> <p>팁: <i>작업: 역할 ID가 $$USERID.roleIDs와 같음</i> 필터 규칙은 내 역할의 기본 제공 필터 미할당 작업 및 내 역할의 미할당 문제에 있습니다. </p> </td> 
  </tr> 
 </tbody> 
</table>

## 개체 기반 와일드카드 필터 변수

다음 개체 기반 와일드카드 중에서 선택할 수 있습니다.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"><b>$$OBJCODE</b> </td> 
   <td> 
    <div> 
     <p>$$OBJCODE 변수는 개체의 유형을 참조합니다. </p> 
     <p>사용자 정의 양식에서, 양식의 선택된 객체 유형이 계산된 사용자 정의 필드에서 참조된 필드와 호환되지 않을 경우, 이 와일드카드를 사용하여 해당 객체 유형에 대한 중복 양식을 생성하는 문제를 방지할 수 있습니다.</p> 
     <p>계산된 사용자 정의 필드에서는 IF 표현식에 와일드카드를 포함하여 계산에서 양식의 각 객체 유형에 대해 서로 다른 값을 출력할 수 있도록 이 작업을 수행합니다. </p> 
     <p>자세한 내용 및 예제는 섹션을 참조하십시오 <a href="../../../administration-and-setup/customize-workfront/create-manage-custom-forms/add-calculated-data-to-custom-form.md#calculat" class="MCXref xref">다중 오브젝트 사용자 정의 양식의 계산된 사용자 정의 필드</a> 이 문서에서 <a href="../../../administration-and-setup/customize-workfront/create-manage-custom-forms/add-calculated-data-to-custom-form.md" class="MCXref xref">사용자 정의 양식에 계산된 데이터 추가</a>.</p> 
    </div> </td> 
  </tr> 
 </tbody> 
</table>
