---
product-area: resource-management
navigation-topic: resource-utilization
title: 자원 사용률 정보 보기
description: 활용률 보고서를 사용하여 자원 활용률을 볼 수 있습니다.
author: Alina
feature: Resource Management
exl-id: 785ee3e9-1b2d-4180-bc78-c41e71c5244d
source-git-commit: a55041ad5a6cd41cd11ec3ade27bf5227ae0ac47
workflow-type: tm+mt
source-wordcount: '7758'
ht-degree: 0%

---

# 자원 사용률 정보 보기

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE:&nbsp;this is linked to the UI from the Utilization report. ALWAYS keep this information. DO NOT DELETE!!)</p>
-->

활용률 보고서를 사용하여 자원 활용률을 볼 수 있습니다.

<!--
<div data-mc-conditions="QuicksilverOrClassic.Draft mode">
<p>(NOTE: Vazgen's response about these hours ie below and he asked us to NOT document them:</p>
<p>It queries Assignments first to get the tasks, issues, projects to display in the view. And then from those gets the hours.</p>
<p>In some cases, like for Planned Hours, it takes them from Assignments</p>
<p>But Budgeted Hours come from projects.</p>
<p>And Actual Hours are their own object - Hour)</p>
</div>
-->

<!--
<p style="color: #dc143c;" data-mc-conditions="QuicksilverOrClassic.Draft mode">This report displays information about the assignments on work items for projects in your environment, like Planned, Actual, and Budgeted Hours, FTE, or Cost.&nbsp;These are hours,&nbsp;FTE, or costs associated with the assignments and not with the tasks and issues themselves.(PRIVATE NOTE:&nbsp;Vazgen's response about these hours: It queries Assignments first to get the tasks, issues, projects to display in the view. And then from those gets the hours. In some cases, like for Planned Hours, it takes them from Assignments; But Budgeted Hours come from projects. And Actual Hours are their own object - Hour.)</p>
-->

## 액세스 요구 사항

활용률 보고서에 액세스하려면 다음 사항이 있어야 합니다.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront 플랜*</td> 
   <td> <p>Pro 이상</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront 라이선스*</td> 
   <td> <p>플랜 </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">액세스 수준 구성*</td> 
   <td> <p>다음 항목에 대한 액세스 권한 보기 이상:</p> 
    <ul> 
     <li> <p>리소스 관리 </p> </li> 
     <li> <p>프로젝트</p> </li> 
     <li> <p>포트폴리오</p> </li> 
     <li> <p>프로그램</p> </li> 
     <li> <p>비용별로 정보를 보려는 경우 재무 데이터</p> </li> 
    </ul> <p><b>메모</b>

여전히 액세스 권한이 없는 경우 Workfront 관리자에게 액세스 수준에서 추가 제한 사항을 설정하는지 문의하십시오. Workfront 관리자가 액세스 수준을 변경하는 방법에 대한 자세한 내용은 <a href="../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">사용자 정의 액세스 수준 만들기 또는 수정</a>.</p> </td>
</tr> 
  <tr> 
   <td role="rowheader">개체 권한</td> 
   <td> <p>프로젝트, 포트폴리오 및 프로그램에 대한 액세스를 보고 리소스 영역에서 활용률 섹션에 액세스합니다</p> <p data-mc-conditions="QuicksilverOrClassic.Quicksilver"> <img src="assets/nwe-utilization-section-highloighted-350x145.png" style="width: 350;height: 145;"> </p> <p>프로젝트에 대한 액세스를 관리하여 프로젝트의 활용률 섹션에 액세스합니다</p> <p data-mc-conditions="QuicksilverOrClassic.Quicksilver"> <img src="assets/nwe-utilization-section-on-project-highloighted-350x289.png" style="width: 350;height: 289;"> </p> <p>추가 액세스 요청에 대한 자세한 내용은 <a href="../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">개체에 대한 액세스 요청 </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

*보유하고 있는 플랜, 라이선스 유형 또는 액세스를 알아보려면 Workfront 관리자에게 문의하십시오.

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">You must have View access to the projects you want to view utilization information for as described in this section. If you are still unable to access this information, contact your Workfront administrator. (NOTE:&nbsp;replaced with above table)</p>
-->

다음 섹션에서는 활용률 정보를 보고 사용하는 방법에 대해 설명합니다.

<!--
<div data-mc-conditions="QuicksilverOrClassic.Draft mode">
<h2>Prerequisites for accessing utilization information</h2>
<p>(NOTE: drafted, replaced with above table)</p>
<p>To access utilization information as described in this section, ensure that the following conditions are met:</p>
<ul>
<li>You have at least&nbsp;View access to the project, program, or portfolio for which you want to view the utilization information.</li>
<li>Your Workfront administrator must grant you at least View access to&nbsp;Financial&nbsp;Data in your Access Level to be able to view cost and revenue information in the Utilization report. The Workfront administrator must enable both View Role Billing & Cost Rates as well as View User Billing &&nbsp;Cost Rates when they grant you the View access to Financial Data. For information about granting access to&nbsp;Financial&nbsp;Data, see <a href="../../administration-and-setup/add-users/configure-and-grant-access/grant-access-financial.md" class="MCXref xref">Grant access to financial data</a>. </li>
<li>
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE:&nbsp;drafted. No longer the case.) </p>
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">The Utilization tab is included on any layout template that is assigned to you and that is applied to either the projects you view or to the Reporting area. </p>
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">The Utilization section is included on any layout template that is assigned to you and that is applied to either the projects you view or to the Resourcing area. </p>
</li>
<li>
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">The Utilization tab is available by default in the Reporting area if the system administrator has not assigned a custom layout template to you. </p>
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">The Utilization section is available by default in the Resourcing area if the system administrator has not assigned a custom layout template to you. </p>
</li>
</ul>
</div>
-->

## 활용률 보고서 개요 {#overview-of-the-utilization-report}

활용률 보고서를 사용하여 프로젝트, 프로그램 또는 포트폴리오의 진행 상황, 원가 또는 수익을 단일 보고서에 표시할 수 있습니다. 매출과 비용을 비교할 수도 있습니다.

자원 영역에서 활용률 보고서를 보고 여러 프로젝트에 걸쳐 활용률을 표시하거나 한 프로젝트 레벨에서 보고 해당 프로젝트와 연관된 개별 자원(작업 역할 및 사용자)에 대한 활용률을 표시할 수 있습니다.

활용률 보고서 액세스 및 사용에 대한 자세한 내용은 [활용률 보고서를 사용하여 진행 상황, 비용 및 수익 추적](#track-progress-cost-and-revenue-with-the-utilization-report) 섹션에 자세히 설명되어 있습니다.

* [추적 시간(진행)](#track-hours-progress)
* [비용 추적](#track-cost)
* [매출 추적](#track-revenue)
* [매출과 계획 및 실제 원가 비교](#compare-revenue-against-planned-and-actual-costs)

### 추적 시간(진행) {#track-hours-progress}

예산책정된 시간과 계획된 시간을 실제 시간과 비교하는 방법을 보고 진행을 추적할 수 있습니다.

프로젝트, 프로그램 또는 포트폴리오의 진행 상황을 추적할 때 작업 및 문제에 대한 진행 상태가 활용률 보고서에 포함됩니다.

시간 추적 시 사용률 보고서에서 다음 정보를 확인할 수 있습니다.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th><strong>시간 표시 시 열 제목</strong> </th> 
   <th><strong>함수</strong> </th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td scope="col"><strong>예산 시간</strong> </td> 
   <td scope="col"> <p>포함된 프로젝트에 대한 총 예산책정 시간입니다. 포함된 프로젝트의 전체 기간에 대한 총 예산책정된 시간을 보거나 지정된 일자 범위에 대해서만 총 예산책정된 시간을 조회할 수 있습니다(개별 주 또는 월을 지정할 수 있음). </p> <p>예산책정된 시간은 업무 사례 또는 자원 계획자의 신규 자원 예산 계획 영역에서 사용할 수 있는 정보로 채워집니다<em>.</em></p> <p>예산책정된 시간은 다음 행 중 하나에 있는 가동률 보고서에 나타납니다.</p> 
    <ul> 
     <li> 예산책정된 시간은 다음과 같이 Utilization 보고서에서 Job 역할 및 개별 사용자별로 요약됩니다.<br><strong>개별 사용자:</strong> 예산책정된 시간은 활용률 보고서에서 각 사용자에 대해 요약됩니다. 이 예산책정된 시간은 포함된 프로젝트에서 사용자가 지정되는 태스크 및 문제와 연관됩니다. (해당 작업 역할의 행을 확장하여 해당 작업 역할이 있는 사용자 목록을 볼 수 있습니다.)<br><strong>작업 역할:</strong> 예산책정된 시간은 활용률 보고서에서 Job 역할별로 요약됩니다.<br>예산책정된 시간은 다음 시나리오의 결과로 특정 Job 역할에 나타납니다. 
     <li>작업 역할은 작업 또는 예산책정된 시간이 연관된 문제에 지정된 사용자의 기본 작업 역할로 정의됩니다. </li> 
       <li>단일 프로젝트에 대한 활용률 정보를 볼 때, 작업 또는 문제에 할당이 없거나, 작업 역할 할당이 없는 다른 사용자에게 할당되거나, 다른 사용자에게 다른 작업 역할이 할당되거나, 다른 팀이 할당되는지 여부에 관계없이 시간이 지정된 사용자의 작업 역할이 사용됩니다.</li> 
       <li>여러 프로젝트, 프로그램 또는 포트폴리오에 대한 활용률 정보를 볼 때 해당 시간을 지정한 사용자의 작업 역할은 프로젝트에서 작업이나 문제에 대해 역할이 지정된 경우에만 사용됩니다. </li> 
       <li>작업 역할은 예산책정된 시간이 연관된 작업이나 문제에 할당되며, 작업이나 문제에 지정된 사용자에게 시스템에 정의된 작업 역할이 없습니다.</li> 
      </ul></li> 
    </ul> 
    <ul> 
     <li> <p><strong>할당되지 않은 시간</strong>: 예산책정된 시간은 작업 또는 문제와 연관되어 있고 작업이나 문제에 지정된 사용자 또는 역할이 없는 경우 미할당 시간 섹션의 가동률 보고서에 표시됩니다.<br>이 섹션은 이 설명과 일치하는 프로젝트 시간이 있을 때와 프로젝트별 또는 프로젝트에서 활용률 보고서를 볼 때만 나타납니다. </p> <p>이 섹션은 이 설명과 일치하는 프로젝트 시간이 있을 때와 프로젝트별 또는 프로젝트에서 활용률 보고서를 볼 때만 나타납니다. </p> </li> 
    </ul> <p>예산책정된 시간에 대한 자세한 내용은 <a href="../../manage-work/projects/project-finances/budgeted-labor-cost.md" class="MCXref xref">프로젝트에 대한 예산책정된 노무비 및 예산책정 시간 이해</a> 문서.</p> </td> 
  </tr> 
  <tr> 
   <td scope="col"><strong>계획된 시간</strong> </td> 
   <td scope="col"> <!-- Yay, no errors, warnings, or alerts! -->

<p>
각 태스크 및 문제에 대한 지정과 연관된 포함된 프로젝트의 계획 시간 포함된 프로젝트의 전체 수명 동안 프로젝트에 있는 모든 발령의 총 계획 시간을 보거나 지정된 날짜 범위에 대해서만 총 계획 시간을 조회할 수 있습니다(개별 주 또는 월을 지정할 수 있음). 
</p>
<p>
<strong>팁 </strong>
</p>
<p>
기간이 0인 품목의 계획 시간은 고려되지 않습니다. 
</p>
<p>
가동률 보고서의 계획시간은 작업 또는 문제의 기간에 걸쳐 계획시간을 다시 할당했는지 여부를 고려합니다. 
</p>
<p>
작업 로드 밸런서를 사용하여 시간 동안의 사용자 일별 할당이 수정된 경우 사용률 보고서에서 선택한 날짜에 작업 또는 문제 기간 중 일부만 포함되어 있으면 사용률 보고서의 데이터에 영향을 줄 수 있습니다. 
</p>
<p>
사용자의 할당 수정에 대한 자세한 내용은 <a href="../workload-balancer/manage-user-allocations-workload-balancer.md">작업 로드 밸런서에서 사용자 할당 관리</a>.


</p>
<p>
계획 시간은 다음 행 중 하나로 활용률 보고서에 나타납니다.
</p>
<ul>

<li>계획 시간은 다음과 같이, 작업 역할 및 활용률 보고서에서 개별 사용자에 의해 요약됩니다. 
<ul>

<li><strong>개별 사용자</strong>: 계획 시간은 활용률 보고서에서 각 사용자에 대해 요약됩니다. 이러한 계획 시간은 포함된 프로젝트에서 사용자가 지정되는 작업 및 문제와 연관됩니다. (해당 작업 역할의 행을 확장하여 해당 작업 역할이 있는 사용자 목록을 볼 수 있습니다.)

<li><strong>작업 역할</strong>: 계획 시간은 단일 프로젝트의 활용률 보고서에서 Job 역할별로 요약됩니다.<br>계획 시간은 다음 시나리오의 결과로 특정 작업 역할에 나타납니다.  
<ul>

<li>작업 롤은 작업 또는 계획 시간과 연관된 문제에 지정된 사용자의 기본 작업 롤로 정의됩니다.

<li>단일 프로젝트에 대한 활용률 정보를 볼 때 다음 시나리오에서 작업 역할과 연관된 시간은 작업 역할에 대해 표시되지 않습니다.   
<ul>

<li>작업이나 문제에 할당이 없습니다

<li>사용자에게 작업 역할 할당이 없습니다.

<li>사용자에게 다른 작업 역할이 할당됩니다

<li>팀이 작업 또는 문제에 할당됨
</li>   
</ul>

<li>여러 프로젝트, 프로그램 또는 포트폴리오에 대한 활용률 정보를 볼 때 해당 시간을 지정한 사용자의 작업 역할은 프로젝트에서 작업이나 문제에 대해 역할이 지정된 경우에만 사용됩니다. 여러 프로젝트에 대한 활용률 보고서를 볼 때 작업 역할 시간이 별도로 표시되지 않습니다.

<li>작업 역할은 계획됨 시간이 연관된 작업이나 문제에 할당되며, 작업이나 문제에 지정된 사용자에게 시스템에 정의된 작업 역할이 없습니다.
</li>  
</ul>

<li><strong>할당되지 않은 시간</strong>: 계획 시간은 작업 또는 문제와 연관되고 작업이나 문제에 지정된 사용자 또는 역할이 없는 경우 할당되지 않은 시간 섹션의 가동률 보고서에 표시됩니다. 이 섹션은 이 설명과 일치하는 프로젝트 시간이 있고 단일 프로젝트에 대한 가동률 보고서를 볼 때만 나타납니다. <br>계획된 시간에 대한 자세한 내용은 <a href="../../manage-work/tasks/task-information/planned-hours.md">계획 시간 개요</a>.
</li> 
</ul>
</li> 
</ul> </td> 
  </tr> 
  <tr> 
   <td><strong>실제 근로시간</strong> </td> 
   <td> <p> 작업, 문제, <span>그리고 프로젝트에서</span> 포함된 프로젝트에 대해 설명합니다. 포함된 프로젝트의 전체 수명 동안 총 실제 시간을 보거나 지정된 날짜 범위에 대해서만 총 실제 시간을 볼 수 있습니다(개별 주 또는 월을 지정할 수 있음). </p> <p>경고: 활용률 보고서에는 하나 이상의 할당이 있는 프로젝트, 1차 하위 구성요소 작업, 문제 및 상위 작업에 기록된 시간이 포함됩니다. 할당 없이 상위 작업에 기록된 시간이 포함되지 않습니다. 상위 작업을 작업 작업으로 사용하지 않고 리소스에 하위 작업만 할당하는 것이 좋습니다. </p> <p>실제 시간은 다음 행 중 하나로 활용률 보고서에 나타납니다.</p> 
    <ul> 
     <li> 실제 시간은 다음과 같이 프로젝트의 활용률 보고서에서 작업 역할 및 개별 사용자에 의해 요약됩니다.<br><strong>개별 사용자:</strong> 실제 시간은 시간을 기록한 사용자 행의 활용률 보고서에 표시됩니다. (해당 작업 역할의 행을 확장하여 해당 작업 역할이 기록된 시간 목록을 볼 수 있습니다.)<br><strong>작업 역할:</strong> 해당 역할과 연관된 사용자가 로그한 실제 시간은 해당 작업 역할 행의 활용률 보고서에 요약됩니다.<br>실제 시간은 다음 시나리오의 결과로 특정 작업 역할에 나타납니다. 
      <ul> 
       <li>작업 역할은 시간을 기록한 사용자의 기본 작업 역할로 정의됩니다.</li> 
       <li>작업이나 문제에 할당이 없습니다</li> 
       <li>다른 사용자가 작업 역할 할당 없이 할당됨</li> 
       <li>다른 사용자에게 다른 작업 역할이 할당됩니다</li> 
       <li> <p>팀이 할당되었습니다.</p> </li> 
      </ul></li>  
     <p>시간을 로깅하는 사용자에게 해당 프로필과 연관된 작업 역할이 없는 경우 사용률 보고서에 사용된 작업 역할은 작업에 할당된 작업 역할이거나, 시간이 기록되거나 작업 또는 문제의 주 소유자와 연관된 작업 역할입니다. </p> 
     <li><strong>기타 시간:</strong> 실제 시간은 시간에 로그인한 사용자 행의 기타 시간 섹션의 활용률 보고서에 표시됩니다.<br>시간을 기록한 사용자에게 시스템에 정의된 작업 역할이 없을 때 이 섹션에 시간이 표시됩니다.<br>이 섹션은 이 설명과 일치하는 프로젝트 시간이 있을 때만 나타납니다. </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td><strong>예산책정된 차이(시간)</strong> </td> 
   <td> <p>총 예산책정된 시간에서 포함된 프로젝트의 총 실제 시간을 뺀 것입니다. 포함된 프로젝트의 전체 기간에 대한 총 예산책정 편차를 보거나 지정된 일자 범위에 대해서만 총 예산책정 편차를 조회할 수 있습니다(개별 주 또는 월을 지정할 수 있음). </p> <p>값이 양수이면 녹색으로 표시됩니다. 이것은 총 예산책정된 시간이 실제 시간보다 크다는 것을 나타냅니다.</p> <p>값이 음수이면 빨간색으로 표시됩니다. 이것은 총 예산책정된 시간이 실제 시간보다 적음을 나타냅니다.</p> <p> <img src="assets/utilization-variance-budgeted-350x96.png" style="width: 350;height: 96;"> </p> </td> 
  </tr> 
  <tr> 
   <td><strong>계획 차이(시간)</strong> </td> 
   <td> <p>포함된 프로젝트의 총 실제 시간을 뺀 총 계획 시간입니다. 포함된 프로젝트의 전체 수명 동안 총 계획 편차를 보거나 지정된 일자 범위에 대해서만 총 계획 편차를 조회할 수 있습니다(개별 주 또는 월을 지정할 수 있음).</p> <p>값이 양수이면 녹색으로 표시됩니다. 이것은 총 계획 시간이 실제 시간보다 더 크다는 것을 나타냅니다.</p> <p>값이 음수이면 빨간색으로 표시됩니다. 이것은 총 계획 시간이 실제 시간보다 적음을 나타냅니다.</p> </td> 
  </tr> 
 </tbody> 
</table>

### 비용 추적 {#track-cost}

예산책정된 원가 및 계획 원가와 실제 원가가 어떻게 비교되는지 확인하여 원가를 추적할 수 있습니다.

프로젝트, 프로그램 또는 포트폴리오의 비용을 추적할 때 활용률 보고서의 정보는 작업에서 가져옵니다. 작업의 비용 정보는 항상 활용률 보고서에서 사용할 수 있습니다. 작업의 비용은 작업의 비용 유형에 따라 계산됩니다. 작업의 원가 유형에 대한 자세한 내용은 [비용 추적](../../manage-work/projects/project-finances/track-costs.md).

다음과 같은 방법으로 활용률 보고서에 원가 정보를 표시할 수 있습니다.

* 특정 주 또는 월 동안 또는 전체 프로젝트, 프로그램 또는 포트폴리오에 대해
* 역할 또는 개인별, 프로젝트

활용률 보고서에 사용된 통화는 프로젝트에서 설정된 통화로 결정됩니다. 프로젝트 통화를 조정하는 방법에 대한 자세한 내용은 [프로젝트 통화 변경](../../manage-work/projects/project-finances/change-project-currency.md).

원가를 추적할 때 활용률 보고서에서 다음 정보를 사용할 수 있습니다.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th><strong>원가 조회 시 열 제목</strong> </th> 
   <th> <p><strong>함수</strong> </p> </th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td scope="col"><strong>예산 비용</strong> </td> 
   <td scope="col"> <p>포함된 프로젝트에 대한 예산책정 원가. 포함된 프로젝트의 전체 기간에 대한 총 예산책정된 원가를 조회하거나 지정된 일자 범위에 대해서만 총 예산책정된 원가를 조회할 수 있습니다(개별 주 또는 월을 지정할 수 있음).</p> <p>활용률 보고서의 예산책정된 원가는 역할별 원가에 집중되므로, 계산은 Workfront의 다른 영역 내의 예산책정된 노무비와 동일합니다. 예산책정된 노무비 계산 방법에 대한 자세한 내용은 <a href="../../manage-work/projects/project-finances/budgeted-labor-cost.md" class="MCXref xref">프로젝트에 대한 예산책정된 노무비 및 예산책정 시간 이해</a>.</p> </td> 
  </tr> 
  <tr> 
   <td scope="col"><strong>계획된 비용</strong> </td> 
   <td scope="col"> <p>포함된 프로젝트의 총 계획 원가. 포함된 프로젝트의 전체 기간에 대한 총 계획 원가를 보거나 지정된 일자 범위에 대해서만 총 계획 원가를 조회할 수 있습니다(개별 주 또는 월을 지정할 수 있음).</p> <p>프로젝트에 대한 계획 원가를 계산하는 방법에 대한 자세한 내용은 문서의 "Workfront이 계획, 예산 및 실제 비용을 계산하는 방법" 섹션을 참조하십시오 <a href="../../manage-work/projects/project-finances/track-costs.md" class="MCXref xref">비용 추적</a>.</p> </td> 
  </tr> 
  <tr> 
   <td scope="col"><strong>실제 비용</strong> </td> 
   <td scope="col"> <p>포함된 프로젝트의 총 실제 원가 포함된 프로젝트의 전체 기간에 대한 총 실제 비용을 보거나 지정된 날짜 범위에 대해서만 총 실제 비용을 조회할 수 있습니다(개별 주 또는 월을 지정할 수 있음).</p> <p>프로젝트에 대한 실제 원가를 계산하는 방법에 대한 자세한 내용은 문서의 "Workfront이 계획, 예산 및 실제 비용을 계산하는 방법" 섹션을 참조하십시오 <a href="../../manage-work/projects/project-finances/track-costs.md" class="MCXref xref">비용 추적</a>.</p> </td> 
  </tr> 
  <tr> 
   <td><strong>예산책정된 차이(비용)</strong> </td> 
   <td scope="col"> <p>총 예산책정된 비용에서 포함된 프로젝트의 총 실제 비용을 뺀 것입니다. 포함된 프로젝트의 전체 기간에 대한 총 예산책정 편차를 보거나 지정된 일자 범위에 대해서만 총 예산책정 편차를 조회할 수 있습니다(개별 주 또는 월을 지정할 수 있음).</p> <p>값이 양수이면 녹색으로 표시됩니다. 이는 총 예산책정된 비용이 실제 원가보다 크다는 것을 나타냅니다.</p> <p>값이 음수이면 빨간색으로 표시됩니다. 이는 총 예산책정된 비용이 실제 원가보다 적음을 나타냅니다.</p> </td> 
  </tr> 
  <tr> 
   <td><strong>계획 차이(비용)</strong> </td> 
   <td> <p>총 계획 원가에서 포함된 프로젝트의 총 실제 원가를 뺀 것입니다. 포함된 프로젝트의 전체 수명 동안 총 계획 편차를 보거나 지정된 일자 범위에 대해서만 총 계획 편차를 조회할 수 있습니다(개별 주 또는 월을 지정할 수 있음). </p> <p>값이 양수이면 녹색으로 표시됩니다. 이는 총 계획 원가가 실제 원가보다 크다는 것을 나타냅니다.</p> <p>값이 음수이면 빨간색으로 표시됩니다. 이는 총 계획 원가가 실제 원가보다 적음을 나타냅니다.</p> </td> 
  </tr> 
 </tbody> 
</table>

### 매출 추적 {#track-revenue}

예산책정된 매출과 계획된 수익이 실제 매출과 비교하는 방식을 보고 수익을 추적할 수 있습니다.

프로젝트, 프로그램 또는 포트폴리오의 수익을 추적할 때 작업의 수익만 활용률 보고서에 포함됩니다.

다음 표의 정보는 수익을 추적할 때 활용률 보고서에서 확인할 수 있습니다.

특정 필드 및 Workfront에서 이러한 필드를 계산하는 방법에 대한 자세한 내용은 다음 문서를 참조하십시오.

* [비용 추적](../../manage-work/projects/project-finances/track-costs.md)
* [청구 및 수익 개요](../../manage-work/projects/project-finances/billing-and-revenue-overview.md)

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th><strong>수입을 볼 때 열 제목</strong> </th> 
   <th> <strong>함수</strong></th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td scope="col"><strong>예산 수익</strong> </td> 
   <td scope="col"> <p>포함된 프로젝트에 대한 역할 청구 비율을 곱한 총 예산 시간 포함된 프로젝트의 전체 수명 동안 총 예산책정된 수익을 조회하거나 지정된 일자 범위에 대해서만 총 예산책정된 수익을 조회할 수 있습니다(개별 주 또는 월을 지정할 수 있음).</p> </td> 
  </tr> 
  <tr> 
   <td scope="col"><strong>계획된 수익</strong> </td> 
   <td scope="col"> <p>활용률 보고서의 계획 수익은 프로젝트의 태스크에 지정된 자원에 할당된 계획 시간과 연관된 수익입니다.</p> <p>Workfront은 다음 공식을 사용하여 가동률 보고서에 대한 프로젝트 계획 수익을 계산합니다.</p> <p><code>Project Planned Revenue = SUM&nbsp;(All Tasks Planned Revenue)</code> </p> 
   <p><b>메모</b>
   <p>활용률 보고서에 표시되는 프로젝트 계획 수익은 프로젝트 상세내역 영역 및 프로젝트 보고서에 표시되는 계획 수익과 다릅니다. </p> <p>프로젝트 상세내역 영역의 계획 수익은 프로젝트의 고정 수익뿐만 아니라 태스크 수익도 반영합니다. 활용률 보고서의 계획 수익에는 프로젝트의 태스크에만 연관된 계획 수익이 표시됩니다. </p> 
     <div class="example" data-mc-autonum="<b>Example: </b>">  
      <p>프로젝트에 10시간의 작업이 있고 $20 시간별 비율을 갖는 컨설턴트에 지정되며 프로젝트에 $100 고정 수익이 있는 경우, 가동률 보고서에는 계획 수익(태스크 시간과 연관된 계획 수익)에 대해 $200가 표시됩니다. 프로젝트 상세내역 섹션에는 $300(태스크의 계획 수익 및 프로젝트의 고정 수익)이 표시됩니다. </p> 
     </div> <p>활용률 보고서 외부의 태스크 및 프로젝트 계획 수익에 대한 자세한 내용은 <a href="../../manage-work/projects/project-finances/billing-and-revenue-overview.md" class="MCXref xref">청구 및 수익 개요</a>.</p> </p> <p>가동률 보고서가 포함된 프로젝트에 대한 계획 수익을 계산하고 표시하는 방법은 태스크에 설정된 수익 유형을 고려합니다. </p> <p>프로젝트에 있는 각 작업의 매출 유형에 따라 다음 시나리오가 존재합니다. </p> <p><strong>고정 매출:</strong> 태스크 지정에 관계없이 항상 태스크에 지정된 고정 금액을 사용하여 태스크 수익을 계산합니다.</p> <p><b>중요 사항</b>

Workfront의 다른 영역과는 달리, 활용률 보고서는 고정 수익(Fixed Revenue)을 작업의 계획 시간(Planning Hours) 수로 균등하게 나누어 고정 수익 작업에 대한 계획 수익(Planning Revenue)을 계산합니다. </p> <p>예를 들어, 작업의 매출액은 $200입니다. 작업에 4시간의 계획 시간이 있는 경우 1시간에 50달러가 됩니다. 사용자 및 역할 수준에서 배포됩니다. 이 배포는 활용률 보고서에 고유합니다.</p> <p><b>메모</b>

고정 수익 태스크가 있고 태스크에 대한 계획 시간이 없는 경우, 해당 작업을 시간에 분배할 방법이 없으므로 수익이 활용률 보고서에 표시되지 않습니다. 고정 수익과 지정 없는 태스크에 대한 계획 시간이 있는 경우, 수익이 미할당 수입으로 표시됩니다. </p> <p><strong>시간별 역할:</strong> 태스크 수익은 특정 역할에 대해 설정된 청구율 세트를 사용하여 계산되며 해당 역할과 연관된 계획 시간 수를 곱합니다. Workfront에서는 다음 공식을 사용합니다.</p> <p>역할 시간별 계획 수익 = SUM(모든 작업의 역할에서 계획된 시간) * 역할 청구 비율</code></p> <p><strong>시간별 사용자:</strong> 작업의 수익은 특정 사용자에 대해 설정된 청구 단가 세트와 해당 사용자와 연관된 계획 시간 수를 사용하여 계산됩니다. Workfront에서는 다음 공식을 사용합니다.</p> <p>사용자 시간별 계획 수익 = SUM(모든 태스크에서 사용자의 계획 시간) * 사용자 청구 비율</code> </p> <p><b>시간별 또는 사용자 시간별 플러스 고정 역할</b> </p> <p><b>중요 사항</b>

Workfront의 다른 영역과 달리 활용률 보고서는 고정 수익을 태스크의 계획 시간 수로 균등하게 나누어 계획 수익을 계산합니다. </p> <p>다음과 같은 경우가 있습니다. </p>
<ul>
<li> <p><strong>시간별 역할 더하기 고정:</strong> 태스크 수익은 특정 역할에 대해 설정된 청구율을 사용하여 계산되며 역할과 연관된 계획 시간 수를 곱합니다. 또한 작업에 지정된 고정 금액이 역할율에 추가됩니다. Workfront에서는 다음 공식을 사용합니다.</p> <p>역할 시간별 + 고정 계획 수익 = [SUM(모든 작업의 역할에서 계획된 시간) * 역할 청구 비율] + SUM(작업의 상한 또는 고정 금액 / 작업의 계획 시간)</code> </p> </li>
</ul>
<ul>
<li> <p><strong>사용자 시간별 + 고정:</strong> 특정 사용자에 대해 설정된 청구 비율에 해당 사용자의 작업에 대한 계획 시간 수를 곱합니다. 또한 작업에 지정된 고정 금액이 사용자 비율에 추가됩니다. Workfront에서는 다음 공식을 사용합니다.</p> <p>사용자 시간별 + 고정 계획 수익 = [SUM(모든 작업의 사용자로부터 계획된 시간) * 사용자 청구 비율] + SUM(작업의 상한 또는 고정 금액 / 작업의 계획 시간)</code> </p> </li>
</ul> <p><b>역할 또는 사용자 시간별(상한 포함)</b> </p> <p><b>중요 사항</b>

Workfront의 다른 영역과 달리, 계획 수익이 상한선을 초과하는 경우 상한 금액 초과 금액은 고정 수입으로 간주됩니다. 계획 수익은 고정 수익을 작업의 계획 시간 수로 균등하게 나눈 다음, 상한 금액 및 역할이나 사용자 시간별 매출에 추가하여 계산합니다. <br></p> <p>다음과 같은 경우가 있습니다. </p>
<ul>
<li> <p><strong>시간별(상한 포함) 역할:</strong> 작업은 시간별로 청구되지만 역할 시간별로 최대 상한 금액이 있습니다. Workfront에서는 다음 공식을 사용합니다.</p> <p>역할 시간별 상한 계획 수익 = [SUM(모든 태스크 및 문제에 대한 역할에서 계획된 시간) * 역할 청구 비율] + 태스크 상한 금액 + SUM(상한 금액 초과 금액 / 태스크 계획 시간)</code> </p> </li>
</ul>
<ul>
<li> <p><strong>사용자 시간별(상한 포함):</strong> 작업은 시간별로 청구되지만 지정할 수 있는 최대 상한 금액이 있습니다. Workfront에서는 다음 공식을 사용합니다. </p> <p>상한 계획 수익을 포함하는 사용자 시간별 = [SUM(모든 작업의 사용자로부터 계획된 시간) * 사용자 청구 비율] + 태스크 상한 금액 + SUM(상한 금액 초과 금액 / 태스크 계획 시간)</code> </p> </li>
</ul> <p>계획 수익을 계산할 때 고려되는 역할이나 사용자에 대한 자세한 내용은 <a href="../../manage-work/projects/project-finances/billing-and-revenue-overview.md" class="MCXref xref">청구 및 수익 개요</a>.</p> </td>
</tr> 
  <tr> 
   <td><strong>실제 수익</strong> </td> 
   <td> <p>실제 매출액은 작업의 실제 시간과 연관된 수익입니다 <span>및</span>. 실제 매출에 대한 자세한 내용은 문서의 "매출 금액 추적" 섹션을 참조하십시오 <a href="../../manage-work/projects/project-finances/billing-and-revenue-overview.md" class="MCXref xref">청구 및 수익 개요</a>.</p>

<p>가동률 보고서가 포함된 프로젝트의 실제 수익을 계산하는 방법은 다음과 같이 태스크에 설정된 수익 유형에 따라 다릅니다.</p> <p><strong>고정 매출:</strong> 태스크 지정에 관계없이 항상 태스크에 지정된 고정 금액을 사용하여 태스크 수익을 계산합니다.</p> <p><b>중요 사항</b>

Workfront의 다른 영역과 달리 활용률 보고서는 고정 수익을 작업에 로그온한 시간 수로 균등하게 나누어 실제 매출액을 계산합니다. </p> <p> </p> <p>예를 들어, 작업의 실제 매출액은 $200입니다. 작업에 4시간의 실제 시간이 있는 경우 한 시간에 50달러가 됩니다. 사용자 및 역할 수준에서 배포됩니다. 이 배포는 활용률 보고서에 고유합니다.</p> <p><b>메모</b>

고정 수익 태스크가 있고 태스크에 실제 시간이 없는 경우, 시간을 분배할 방법이 없으므로 실제 수익이 가동률 보고서에 표시되지 않습니다. </p> <p><strong>시간별 역할:</strong> 태스크 수익은 특정 역할에 대해 설정된 청구 단가 세트와 계획 시간 수를 사용하여 계산됩니다.</p> <p>Workfront에서는 다음 공식을 사용합니다.</p> <p>역할 시간별 실제 수익 = SUM(모든 작업의 역할에서 실제 시간) * 역할 청구 비율</code> </p> <p><strong>시간별 사용자:</strong> 작업의 수익은 특정 사용자에 대해 설정된 청구율과 해당 사용자의 작업에 대해 로그된 시간 수를 곱한 값을 사용하여 계산됩니다. Workfront에서는 다음 공식을 사용합니다.</p> <p>사용자 시간별 실제 수익 = SUM(모든 태스크에서 사용자의 실제 시간) * 사용자 청구 비율</code></p> <p><b>역할 또는 사용자 시간별 + 고정</b> </p> <p><b>중요 사항</b>

Workfront의 다른 영역과 달리 활용률 보고서는 고정 수익을 작업에 로그온한 시간 수로 균등하게 나누어 실제 매출액을 계산합니다. </p> <p>다음과 같은 경우가 있습니다. </p>
<ul>
<li> <p><strong>시간별 역할 더하기 고정:</strong> 특정 역할에 대해 설정된 청구 비율에 해당 역할을 가진 사용자의 작업에 대해 기록된 시간을 곱합니다. 또한 작업에 지정된 고정 금액이 역할율에 추가됩니다. </p> <p>Workfront에서는 다음 공식을 사용합니다.</p> <p>역할 시간별 + 고정 실제 매출 = [SUM(모든 작업의 역할에서 실제 시간) * 역할 청구 비율] + SUM(작업의 상한 또는 고정 금액 / 작업의 실제 시간)</code> </p> </li>
</ul>
<ul>
<li> <p><strong>사용자 시간별 + 고정:</strong> 특정 사용자에 대해 설정된 청구 비율에 해당 사용자의 작업에 대해 기록된 시간을 곱합니다. 또한 작업에 지정된 고정 금액이 사용자 비율에 추가됩니다. </p> <p>Workfront에서는 다음 공식을 사용합니다.</p> <p>사용자 시간별 + 고정 실제 매출 = [SUM(모든 작업의 역할에서 실제 시간) * 사용자 청구 비율] + SUM(작업의 상한 또는 고정 금액 / 작업의 사용자 시간)</code> </p> </li>
</ul> <p><b>역할 또는 사용자 시간별(상한 포함)</b> </p> <p><b>중요 사항</b>

Workfront의 다른 영역과 달리, 계획 수익이 상한선을 초과하는 경우 상한 금액 초과 금액은 고정 수입으로 간주됩니다. 계획 수익은 고정 수익을 작업의 계획 시간 수로 균등하게 나눈 다음, 상한 금액 및 역할이나 사용자 시간별 매출에 추가하여 계산합니다. <br></p> <p>다음 시나리오가 있습니다.</p>
<ul>
<li> <p><strong>시간별(상한 포함) 역할:</strong> 작업은 시간별로 청구되지만 역할 시간별로 최대 상한 금액이 있습니다. Workfront에서는 다음 공식을 사용합니다.</p> <p>역할 시간별 상한 실제 매출 = [SUM(모든 태스크 및 문제에 대한 역할에서 실제 시간) * 역할 청구 비율] + 작업의 상한 금액 + SUM(상한 금액 초과 금액 / 작업의 실제 시간)</code></p> </li>
</ul>
<ul>
<li> <p><strong>사용자 시간별(상한 포함):</strong> 작업은 시간별로 청구되지만 지정할 수 있는 최대 상한 금액이 있습니다.</p> <p> Workfront에서는 다음 공식을 사용합니다.</p> <p>상한액을 사용하는 사용자 시간별 실제 매출 = [SUM(모든 작업 및 문제에 대한 역할에서 실제 시간) * 사용자 청구 비율] + 작업의 상한 금액 + SUM(상한 금액 초과 금액 / 작업의 실제 시간)</code> </p> </li>
</ul>
<div>
<p><strong>프로젝트 매출</strong>: 프로젝트에 로그온한 시간과 연관된 수익은 시간을 기록하는 사용자의 기본 작업 역할의 시간당 청구 금액을 고려하여 계산됩니다. 프로젝트에서 로깅 시간을 기록하지 않는 것이 좋습니다. </p>
<p><b>메모</b>

사용자가 Job 역할과 연관되지 않았거나 기본 역할의 시간당 청구가 0인 경우 Workfront은 사용자에 대한 시간당 청구 금액을 사용하여 실제 수익을 계산합니다. 프로필에 시간당 청구 금액이 없는 경우 실제 매출은 0입니다. </p>
</div> </td>
</tr> 
  <tr> 
   <td><strong>예산책정된 차이(수익용)</strong> </td> 
   <td> <p>포함된 프로젝트에 대한 총 매출에서 예산 수익을 뺀 금액입니다.<br>포함된 프로젝트의 전체 기간에 대한 총 예산책정 편차를 보거나 지정된 일자 범위에 대해서만 총 예산책정 편차를 조회할 수 있습니다(개별 주 또는 월을 지정할 수 있음).</p> <p>값이 양수이면 녹색으로 표시됩니다. 이는 총 예산 수익이 실제 수익보다 큰 것을 나타냅니다.</p> <p>값이 음수이면 빨간색으로 표시됩니다. 이는 총 예산 수익이 실제 수익보다 작음을 나타냅니다.</p> </td> 
  </tr> 
  <tr> 
   <td><strong>계획 차이(매출용)</strong> </td> 
   <td> <p>총 실제 수입에서 포함된 프로젝트의 총 계획 수익을 뺀 것입니다.<br>포함된 프로젝트의 전체 수명 동안 총 계획 편차를 보거나 지정된 일자 범위에 대해서만 총 계획 편차를 조회할 수 있습니다(개별 주 또는 월을 지정할 수 있음). </p> <p>값이 양수이면 녹색으로 표시됩니다. 이는 총 계획 수익이 실제 수익보다 크다는 것을 나타냅니다.</p> <p>값이 음수이면 빨간색으로 표시됩니다. 이는 총 계획 수익이 실제 수익보다 작음을 나타냅니다.</p> </td> 
  </tr> 
 </tbody> 
</table>

<!--Note from the table about Actual revenue: 
     <p>Actual Revenue is displayed in the Utilization report only after the task is marked as Complete or Done (or a status that equates with Complete).</p>
    -->

<!--More notes from the table: 
     <p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE:&nbsp;the note below is duplicated in this article: /Content/Manage work/Projects/Project Finances/billing-and-revenue-overview.html and in the glossary)</p>
   -->

### 매출과 계획 및 실제 원가 비교 {#compare-revenue-against-planned-and-actual-costs}

계획 수익 및 실제 원가를 계획 매출과 함께 조회할 수 있습니다. 마진(%)도 표시됩니다(마진은 매출 - 비용/매출로 계산됨).

수익과 계획 및 실제 원가를 비교할 때 활용률 보고서에서 다음 정보를 사용할 수 있습니다.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th><strong>매출과 원가 조회 시 열 제목(계획됨)</strong> </th> 
   <th> <strong>함수</strong></th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td scope="col"><strong>계획된 비용</strong> </td> 
   <td scope="col"> 포함된 프로젝트의 총 계획 원가. 포함된 프로젝트의 전체 기간에 대한 총 계획 원가를 보거나 지정된 일자 범위에 대해서만 총 계획 원가를 조회할 수 있습니다(개별 주 또는 월을 지정할 수 있음). </td> 
  </tr> 
  <tr> 
   <td scope="col"><strong>계획된 수익</strong> </td> 
   <td scope="col"> <p>계획 매출액은 작업의 계획 시간과 연관된 수익입니다. </p> <p>활용률 보고서가 포함된 프로젝트에 대한 계획 수익을 계산하고 표시하는 방식은 <a href="#track-revenue" class="MCXref xref">매출 추적</a> 섹션에 자세히 설명되어 있습니다.</p> </td> 
  </tr> 
  <tr> 
   <td scope="col"><strong>여백</strong> </td> 
   <td scope="col"> <p>순익 퍼센트는 다음과 같이 계산됩니다.</p> <p><code>Planned Revenue - Planned Cost / Planned Revenue * 100. </code></p> <p><b>메모</b>

계획 수익이 0인 경우 마진이 0으로 표시됩니다. </p> </td>
</tr> 
  <tr> 
   <td scope="col"> <p scope="col"><strong>매출과 비용을 볼 때 열 제목(실제)</strong> </p>  </td> 
   <td scope="col"><p><strong>함수</strong></p></td> 
  </tr> 
  <tr> 
   <td scope="col"><strong>실제 비용</strong> </td> 
   <td scope="col"> <p>포함된 프로젝트의 총 실제 원가 포함된 프로젝트의 전체 기간에 대한 총 실제 비용을 보거나 지정된 날짜 범위에 대해서만 총 실제 비용을 조회할 수 있습니다(개별 주 또는 월을 지정할 수 있음).</p> </td> 
  </tr> 
  <tr> 
   <td scope="col"><strong>실제 수익</strong> </td> 
   <td> <p>실제 매출액은 작업의 실제 시간과 연관된 수익입니다.</p> <p>작업이 완료 또는 완료(또는 완료와 동일한 상태)로 표시된 후에만 실제 수익이 활용률 보고서에 표시됩니다.</p> <p>활용률 보고서가 포함된 프로젝트의 실제 수익을 계산하는 방법은 작업에 설정된 수익 유형에 따라 다릅니다. <a href="#track-revenue" class="MCXref xref">매출 추적</a> 섹션에 자세히 설명되어 있습니다. </p> </td> 
  </tr> 
  <tr> 
   <td scope="col"><strong>여백</strong> </td> 
   <td> <p>순익 퍼센트는 다음과 같이 계산됩니다.</p> <p>실제 수익 - 실제 원가/실제 수익 * 100개. </p> <p><b>메모</b>

실제 수익이 0인 경우 마진이 0으로 표시됩니다. </p> </td>
</tr> 
 </tbody> 
</table>

<!--Note from the table from above "Function" header in the middle of the table; right after the "Planned Revenue"/"Margin" definition: 
     <p scope="col" data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: This needs to be either split in two tables of formatted differently)</p>
    -->

## 활용률 보고서를 사용하여 진행 상황, 비용 및 수익 추적 {#track-progress-cost-and-revenue-with-the-utilization-report}

프로젝트, 프로그램 또는 포트폴리오의 진행 또는 비용을 추적할 수 있습니다.

주어진 주 또는 월의 활용률 보고서 또는 프로젝트의 전체 수명 정보를 표시할 수 있습니다.

활용률 보고서를 사용하여 하나 이상의 프로젝트의 진행 또는 비용을 추적하려면

1. 개별 프로젝트, 여러 프로젝트, 프로그램 또는 포트폴리오의 활용률 정보를 보고 있는지 여부에 따라 다음 중 하나를 수행합니다.

   * 단일 프로젝트에 대한 활용률 정보를 조회하려면

      1. 활용률 정보를 보려는 프로젝트로 이동한 다음 **자세히 표시> 활용률**.
      1. 개별 프로젝트를 볼 때 활용률 정보가 자동으로 표시되며 필터를 적용할 필요는 없습니다.\
         활용률 보고서를 필터링하려면 필터를 적용한 다음 **실행**.\
         활용률 보고서를 필터링하는 방법에 대한 자세한 내용은 섹션을 참조하십시오 [사용률 정보 필터링](#filter-utilization-information) 참조하십시오.\
         개별 사용자 및 역할에 대한 활용률 정보가 표시됩니다(사용자는 연관된 역할 내에 그룹화됨).
   * 복수 프로젝트에 대한 활용률 정보를 조회하려면

      1. 을(를) 클릭합니다. **기본 메뉴** 아이콘 ![](assets/main-menu-icon.png) Workfront의 오른쪽 위 모서리에서 을(를) 클릭하고 **리소스**, 그런 다음 **활용** 왼쪽 패널에 표시됩니다.
      1. 사용률 보고서에 필터를 적용한 다음 **실행**.\
         활용률 보고서를 실행하기 전에 필터에 하나 이상의 프로젝트를 지정해야 합니다. 활용률 보고서를 필터링하는 방법에 대한 자세한 내용은 섹션을 참조하십시오 [사용률 정보 필터링](#filter-utilization-information) 참조하십시오.\
         개별 역할 및 프로젝트에 대한 활용률 정보가 표시됩니다(역할은 관련 프로젝트 내에 그룹화됨).
   * 프로그램에 대한 활용률 정보를 조회하려면

      1. 을(를) 클릭합니다. **기본 메뉴** 아이콘 ![](assets/main-menu-icon.png) Workfront의 오른쪽 위 모서리에서 을(를) 클릭하고 **리소스**, 그런 다음 **활용** 왼쪽 패널에서 **표시**>**프로그램**.
      1. 사용률 보고서에 필터를 적용한 다음 **실행**.\
         활용률 보고서를 실행하기 전에 필터에 하나 이상의 프로그램을 지정해야 합니다. 활용률 보고서를 필터링하는 방법에 대한 자세한 내용은 섹션을 참조하십시오 [사용률 정보 필터링](#filter-utilization-information) 참조하십시오.\
         개별 프로젝트 및 프로그램에 대해 활용률 정보가 표시됩니다(프로젝트는 관련 프로그램 내에 그룹화됨).
   * 포트폴리오의 활용률 정보를 보려면

      1. 을(를) 클릭합니다. **기본 메뉴** 아이콘 ![](assets/main-menu-icon.png) Workfront의 오른쪽 위 모서리에서 을(를) 클릭하고 **리소스**, 그런 다음 **활용** 왼쪽 패널에서 **표시**>**Portfolio**.
      1. 사용률 보고서에 필터를 적용한 다음 **실행**.\
         활용률 보고서를 실행하기 전에 필터에 하나 이상의 포트폴리오를 지정해야 합니다. 활용률 보고서를 필터링하는 방법에 대한 자세한 내용은 섹션을 참조하십시오 [사용률 정보 필터링](#filter-utilization-information) 참조하십시오.\
         개별 프로젝트, 프로그램 및 포트폴리오에 대해 활용률 정보가 표시됩니다(프로젝트는 관련 프로그램 내에서 그룹화되고 프로그램은 관련 포트폴리오 내에서 그룹화됨).




1. 활용률 보고서의 오른쪽 위 모서리에서 **보기** 드롭다운 메뉴에서 다음 중에서 선택합니다.

   * **비용**
   * **시간**
   * **수익**
   * **수익 대 비용(계획)**
   * **매출과 비용(실제)**.

   선택하는 옵션에 따라 보고서에서 사용할 수 있는 열과 정보가 결정됩니다. 각 열에서 사용할 수 있는 정보에 대한 자세한 내용은 5단계의 테이블을 참조하십시오.\
   ![](assets/utilization-view-dropdown.png)

1. (선택 사항) 활용률 정보가 표시되는 날짜 범위를 선택합니다. 특정 주 또는 달의 정보를 **전체** 열. 전체 프로젝트, 프로그램 또는 포트폴리오에 대한 정보는 항상 **전체** 열.\
   자세한 내용은 섹션을 참조하십시오 [정보가 표시되는 날짜 범위를 조정합니다](#adjust-the-date-range-for-which-information-is-displayed) 참조하십시오.

1. (선택 사항) 임의의 열 제목을 눌러 해당 열의 정보별로 활용률 보고서를 정렬합니다. 정렬은 보고서에 여러 항목을 포함하는 경우에만 작동합니다. 예를 들어 두 개 이상의 프로젝트(또는 포트폴리오 또는 프로그램)를 볼 때 보고서 결과를 정렬할 수 있습니다. 한 번에 하나의 프로젝트(또는 하나의 포트폴리오 또는 프로그램)만 보는 경우에는 결과를 정렬할 수 없습니다.
1. 섹션의 정보를 사용합니다 [활용률 보고서 개요](#overview-of-the-utilization-report) 이 문서에서 활용률 보고서의 각 열에 대해 알아보십시오.

## 사용률 정보 필터링 {#filter-utilization-information}

프로젝트의 활용률 보고서에 표시되는 컨텐츠를 필터링할 수 있습니다. 작업, 문제, 역할 및 사용자 지정 데이터를 필터링할 수 있습니다. 활용률 보고서에 필터를 적용하면 활용률 보고서에는 선택한 기준에 따른 정보가 포함됩니다.

필터를 만들거나 이전에 만든 필터를 적용할 수 있습니다.

* [필터 만들기 또는 수정](#create-or-modify-a-filter)
* [저장된 필터 적용](#apply-a-saved-filter)
* [필터 복제](#duplicate-a-filter)
* [필터 이름 바꾸기](#rename-a-filter)
* [필터 삭제](#delete-a-filter)

### 필터 만들기 또는 수정 {#create-or-modify-a-filter}

필터를 만들면 사용률 보고서에 액세스할 수 있는 모든 Workfront 사용자도 사용자가 만드는 필터에 액세스할 수 있습니다. 마찬가지로, 기존 필터를 수정할 때 사용률 보고서에 액세스할 수 있는 모든 사용자에 대해 필터가 수정됩니다.

필터를 만들거나 수정하려면 다음을 수행합니다.

1. 단일 프로젝트에 대한 활용률 정보를 필터링하려면 활용률 정보를 필터링할 프로젝트로 이동한 다음 **자세히 보기>활용률** 왼쪽 패널에 표시됩니다.

   또는

   여러 프로젝트, 프로그램 또는 포트폴리오의 활용률 정보를 필터링하려면 기본 메뉴 아이콘을 누릅니다 ![](assets/main-menu-icon.png) Workfront의 오른쪽 위 모서리에서 **리소스**, **활용** 왼쪽 패널에서 **표시**>**프로그램** 또는 **Portfolio** 또는&#x200B;**프로젝트**.

1. 을(를) 클릭합니다. **필터** 아이콘을 클릭하여 필터 옵션을 표시합니다.

1. (조건부) 기존 필터를 수정하려면 **필터** 드롭다운 메뉴에서 수정할 필터를 선택합니다.
1. 필터를 만들거나 수정하려면 다음 정보를 지정하십시오.

   * **Portfolio:** 활용률 보고서에 포함할 정보가 포함된 포트폴리오의 이름을 입력한 다음 드롭다운 메뉴에 해당 이름이 표시되면 이름을 클릭합니다.\
      활용률 보고서에 여러 포트폴리오의 정보를 포함하려면 이 프로세스를 반복합니다.\
      필터에 시스템의 모든 포트폴리오를 포함하려면 **모두 추가**. (시스템에 포트폴리오가 10개 미만인 경우에만 이 옵션을 사용할 수 있습니다.)

   * **프로그램:** 활용률 보고서에 포함할 정보가 포함된 프로그램의 이름을 입력하고 드롭다운 메뉴에 나타나는 이름을 클릭합니다.\
      활용률 보고서에 여러 작업의 정보를 포함하려면 이 프로세스를 반복합니다.\
      필터에 이미 포트폴리오를 지정한 경우 지정한 프로그램은 필터에 이미 포함된 포트폴리오에서 지정되어야 합니다. 그렇지 않으면 프로그램의 데이터가 활용률 보고서에 포함되지 않습니다.\
      필터에 시스템의 모든 프로그램을 포함하려면 **모두 추가**. (시스템에 프로그램이 20개 미만인 경우에만 이 옵션을 사용할 수 있습니다.)

   * **프로젝트:** 사용률 보고서에 포함할 정보가 포함된 프로젝트의 이름을 입력하고 드롭다운 메뉴에 나타나는 이름을 클릭합니다.\
      활용률 보고서에 여러 프로젝트의 정보를 포함하려면 이 프로세스를 반복합니다.\
      필터에 이미 포트폴리오나 프로그램을 지정한 경우 지정한 프로젝트는 이미 필터에 포함된 포트폴리오 또는 프로그램 중 하나여야 합니다. 그렇지 않으면 프로젝트의 데이터가 활용률 보고서에 포함되지 않습니다.\
      필터에 시스템의 모든 프로젝트를 포함하려면 **모두 추가**. (시스템에 프로젝트가 250개 미만인 경우에만 이 옵션을 사용할 수 있습니다.)

   * **작업:** 사용률 보고서에 포함할 정보가 포함된 작업의 이름을 입력하고 드롭다운 메뉴에 나타나는 이름을 클릭합니다.\
      활용률 보고서에 여러 작업의 정보를 포함하려면 이 프로세스를 반복합니다.\
      필터에 이미 포트폴리오, 프로그램 또는 프로젝트를 지정한 경우 지정한 작업은 해당 필터에 이미 포함된 포트폴리오, 프로그램 또는 프로젝트 중 하나여야 합니다. 그렇지 않으면 작업의 데이터가 활용률 보고서에 포함되지 않습니다.

   * **문제:** 사용률 보고서에 포함할 정보가 포함된 문제 이름을 입력하고 드롭다운 메뉴에 나타나는 이름을 클릭합니다.\
      활용률 보고서에 여러 문제의 정보를 포함하려면 이 프로세스를 반복합니다.\
      이미 필터에 포트폴리오, 프로그램 또는 프로젝트를 지정한 경우 지정한 문제는 필터에 이미 포함된 포트폴리오, 프로그램 또는 프로젝트 중 하나여야 합니다. 그렇지 않으면 문제의 데이터가 활용률 보고서에 포함되지 않습니다.\
      문제에 대한 비용 정보가 항상 활용률 보고서에 포함되는 것은 아닙니다. 문제에 대한 비용 정보가 활용률 보고서에 포함되는 경우에 대한 자세한 내용은 섹션을 참조하십시오 [활용률 보고서를 사용하여 진행 상황, 비용 및 수익 추적](#track-progress-cost-and-revenue-with-the-utilization-report) 참조하십시오.

   * **역할:** 활용률 보고서에 나타낼 역할의 이름을 입력하고 드롭다운 메뉴에 표시될 이름을 클릭합니다. 추가 역할을 포함하려면 이 프로세스를 반복합니다.\
      활용률 보고서에는 지정한 역할에 대한 정보만 포함됩니다. 예를 들어, 작업에 10시간의 실제 시간이 포함됩니다. 이 중 6시간은 디자이너 역할이며 4시간은 개발자 역할입니다. 디자이너의 역할별로 활용률 보고서를 필터링하면 개발자 역할에서 나오는 4시간이 보고서에서 제외됩니다.

   * **필터 규칙 추가:** 클릭 **필터 규칙 추가**&#x200B;첫 번째 필드를 클릭한 다음 필터링할 필드 이름을 입력하기 시작합니다. 필드를 사용할 수 있으면 필드를 연결할 수 있는 각 개체에 대해 채워집니다. 필드 이름을 클릭하여 필터에 추가합니다.

      >[!IMPORTANT]
      >
      >필드 레이블이 아니라 필드 이름을 입력해야 합니다. 필드 레이블은 개체에 첨부된 사용자 지정 양식에 표시됩니다. 레이블과 사용자 지정 필드 이름의 차이에 대한 자세한 내용은  [사용자 지정 양식 만들기 또는 편집](../../administration-and-setup/customize-workfront/create-manage-custom-forms/create-or-edit-a-custom-form.md).

      열에 표시되는 필드에 대한 자세한 내용은 [Adobe Workfront 용어 설명](../../workfront-basics/navigate-workfront/workfront-navigation/workfront-terminology-glossary.md).\
      필터에 대한 필터 및 조건 한정자를 선택합니다. 사용 가능한 수정자는 [필터 및 조건 수정자](../../reports-and-dashboards/reports/reporting-elements/filter-condition-modifiers.md).

1. 새 필터를 만들려면 **필터 저장**.\
   또는\
   기존 필터를 수정하려면 **필터 저장** 단추를 클릭한 다음 **새 필터 저장**.\
   에서 **필터 이름** 필드에서 필터 이름을 지정한 다음 **저장**.\
   활용률 영역은 필터에 포함된 정보로 필터링됩니다.

### 저장된 필터 적용 {#apply-a-saved-filter}

1. 단일 프로젝트에 대한 활용률 보고서에 필터를 적용하려면 필터링할 프로젝트로 이동한 다음 **자세히 보기>활용률** 왼쪽 패널에 표시됩니다.

   또는

   여러 프로젝트, 프로그램 또는 포트폴리오의 활용률 보고서에 필터를 적용하려면 **기본 메뉴** 아이콘 ![](assets/main-menu-icon.png) Workfront의 오른쪽 위 모서리에서 **리소스**, **활용** 왼쪽 패널에서 **표시**>**프로그램** 또는&#x200B;**Portfolio** 또는&#x200B;**프로젝트**.

1. 클릭 **저장한 필터**&#x200B;을 클릭한 다음 드롭다운 메뉴에서 적용할 필터를 선택합니다.

### 필터 복제 {#duplicate-a-filter}

1. 단일 프로젝트에 대한 활용률 보고서에서 필터를 복제하려면 필터를 복제할 프로젝트로 이동한 다음 를 클릭합니다 **자세히 보기>활용률** 왼쪽 패널에 표시됩니다.

   또는

   여러 프로젝트, 프로그램 또는 포트폴리오의 활용률 보고서에서 필터를 복제하려면 **기본 메뉴** 아이콘 ![](assets/main-menu-icon.png) Workfront의 오른쪽 위 모서리에서 을(를) 클릭하고 **리소스**, 그런 다음 **활용** 왼쪽 패널에 표시됩니다.

1. 클릭 **저장한 필터**&#x200B;을 클릭하고 드롭다운 메뉴에서 복제할 필터 위로 마우스를 가져간 다음 **복제** 아이콘.

   ![](assets/utilization-filter-duplicate.png)\
   필터 복제 대화 상자가 표시됩니다.

1. 에서 **필터 이름** 필드에서 새 필터의 이름을 지정한 다음 **저장**.

### 필터 이름 바꾸기 {#rename-a-filter}

필터 이름을 바꾸면 사용률 보고서에 액세스할 수 있는 모든 Workfront 사용자가 선택한 새 이름을 확인합니다.

필터 이름을 변경하려면:

1. 단일 프로젝트에 대한 활용률 보고서에서 필터 이름을 변경하려면 필터 이름을 바꿀 프로젝트로 이동한 다음 **자세히 보기>활용률** 왼쪽 패널에 표시됩니다.

   또는

   여러 프로젝트, 프로그램 또는 포트폴리오의 활용률 보고서에서 필터 이름을 변경하려면 **기본 메뉴** 아이콘 ![](assets/main-menu-icon.png) Workfront의 오른쪽 위 모서리에서 을(를) 클릭하고 **리소스**, 그런 다음 **활용** 왼쪽 패널에 표시됩니다.

1. 클릭 **저장한 필터**&#x200B;을 클릭하고 드롭다운 메뉴에서 복제할 필터 위로 마우스를 가져간 다음 **이름 변경** 아이콘.\
   ![](assets/utilization-filter-rename.png)\
   필터 이름 변경 대화 상자가 표시됩니다.

1. 에서 **필터 이름** 필드에서 새 필터의 이름을 지정한 다음 **저장**.

### 필터 삭제 {#delete-a-filter}

필터를 삭제하면 사용률 보고서에 액세스할 수 있는 모든 Workfront 사용자에 대해 필터가 삭제됩니다.

필터를 삭제하려면 다음을 수행하십시오.

1. 단일 프로젝트에 대한 활용률 보고서에서 필터를 삭제하려면 필터를 삭제할 프로젝트로 이동한 다음 를 클릭합니다 **자세히 보기>활용률** 왼쪽 패널에 표시됩니다.

   또는

   여러 프로젝트, 프로그램 또는 포트폴리오의 활용률 보고서에서 필터를 삭제하려면 **기본 메뉴** 아이콘 ![](assets/main-menu-icon.png) Workfront의 오른쪽 위 모서리에서 을(를) 클릭하고 **리소스**, 그런 다음 **활용** 왼쪽 패널에 표시됩니다.

1. 클릭 **저장한 필터**&#x200B;을 클릭하고 드롭다운 메뉴에서 복제할 필터 위로 마우스를 가져간 다음 **삭제** 아이콘.

   ![](assets/utilization-filter-delete.png)

1. 클릭 **삭제** 필터를 삭제할지 여부를 묻는 메시지가 표시되면

## 정보가 표시되는 날짜 범위를 조정합니다 {#adjust-the-date-range-for-which-information-is-displayed}

활용률 정보가 표시되는 날짜 범위를 조정할 수 있습니다. 과거 또는 미래 날짜를 선택할 수 있습니다. 변경한 내용은 사용자에게만 표시됩니다.

1. 단일 프로젝트에 대한 활용률 보고서의 날짜 범위를 조정하려면 날짜 범위를 조정할 프로젝트로 이동한 다음 를 클릭합니다 **자세히 보기>활용률** 왼쪽 패널에 표시됩니다.

   또는

   여러 프로젝트, 프로그램 또는 포트폴리오에 대해 활용률 보고서의 날짜 범위를 조정하려면 **기본 메뉴** 아이콘 ![](assets/main-menu-icon.png) Workfront의 오른쪽 위 모서리에서 을(를) 클릭하고 **리소스**, 그런 다음 **활용** 왼쪽 패널에 표시됩니다.

1. 다음 옆에 있는 날짜 범위를 클릭합니다. **내보내기** 버튼을 클릭합니다.

   기본적으로 현재 주가 선택됩니다.

1. 다음 옵션 중에서 선택합니다.

   * **주:** 주어진 주(일요일부터 토요일)를 선택하려면 이 옵션을 선택합니다.
   * **월:** 지정된 월을 선택하려면 이 옵션을 선택합니다.

   선택한 날짜 범위가 활용률 보고서에 표시되며, **전체** 열.\
   Workfront은 1주일 또는 1개월 보기를 표시할지 여부를 기억합니다. 다음에 활용률 보고서에 액세스할 때 선택한 옵션에 따라 현재 주 또는 이번 달이 표시됩니다.

## 활용률 정보 내보내기

Workfront에서 프로젝트, 프로그램 또는 포트폴리오의 활용률 정보를 내보낼 수 있습니다. 정보는 XLSX, TSV 및 PDF 형식으로만 내보낼 수 있습니다.

Microsoft Excel에서 보면 음수 숫자가 괄호 안에 표시됩니다.

활용률 정보를 익스포트하려면

1. 단일 프로젝트에 대한 활용률 정보를 내보내려면 활용률 정보를 내보낼 프로젝트로 이동한 다음 **활용** 탭(레이아웃 설정에 따라 다름) **자세히** 탭).

   또는

   여러 프로젝트, 프로그램 또는 포트폴리오의 활용률 정보를 내보내려면 **기본 메뉴** 아이콘 ![](assets/main-menu-icon.png) Workfront의 오른쪽 위 모서리에서 을(를) 클릭하고 **리소스**, 그런 다음 **활용** 왼쪽 패널에 표시됩니다.

1. 클릭 **내보내기**&#x200B;의 왼쪽 위 모서리에 있습니다. **활용** 탭.

1. 다음 옵션 중에서 선택합니다.

   * **PDF:** 보고서를 PDF 형식으로 내보냅니다. 보고서를 인쇄하려는 경우 권장되는 형식입니다.\
      다음 중 하나를 선택합니다 **편지 - 세로**, **편지 - 가로**, 또는 **기타 크기** (법어(8.5인치 x 14인치), 원장(11인치 x 17인치) 및 A4에서 내보내기 옵션을 제공합니다.)\
      사용하는 운영 체제에 따라 파일을 열거나 저장하는 옵션이 있을 수 있습니다. 연결된 응용 프로그램이 있는 파일을 열거나 하드 드라이브에 저장합니다.

   * **Excel:** 보고서를 XLSX 형식으로 내보냅니다. Excel에서 데이터를 추가로 분석하려는 경우 권장되는 형식입니다.\
      사용하는 운영 체제에 따라 파일을 열거나 저장하는 옵션이 있을 수 있습니다. 연결된 응용 프로그램이 있는 파일을 열거나 하드 드라이브에 저장합니다.

   * **탭으로 구분:** 보고서를 TSV 형식으로 내보냅니다. 추가적인 분석을 위해 데이터를 타사 소프트웨어로 가져오려는 경우 권장되는 형식입니다.\
      사용하는 운영 체제에 따라 파일을 열거나 저장하는 옵션이 있을 수 있습니다. 연결된 응용 프로그램이 있는 파일을 열거나 하드 드라이브에 저장합니다.

1. 문서의 정보 읽기 [데이터 내보내기](../../reports-and-dashboards/reports/creating-and-managing-reports/export-data.md) 내보낸 파일을 사용하는 방법을 이해합니다.

## 차트에서 활용률 정보 보기

차트 보기에서 사용률 보고서의 데이터를 시각화할 수 있습니다.

1. 차트 형식의 단일 프로젝트에 대한 활용률 보고서를 보려면 보려는 프로젝트로 이동한 다음 **자세히 표시> 활용률** 왼쪽 패널에 표시됩니다.

   또는

   여러 프로젝트, 프로그램 또는 포트폴리오의 차트 형식으로 활용률 보고서를 보려면 **보고** 전역 탐색 막대에서 보고 영역으로 이동한 다음 **활용** 탭.

1. 활용률 보고서의 오른쪽 위 모서리에서 **차트** 아이콘.\
   ![](assets/utilization-chart.png)\
   활용률 보고서가 차트 뷰에 표시됩니다.

1. (선택 사항)에서 적절한 옵션을 선택하여 프로젝트, 프로그램 또는 Portfolio을 표시하도록 구성합니다 **표시** 드롭다운 메뉴
1. (선택 사항) 보고서에서 특정 시점으로 마우스를 가져가 해당 시점의 데이터를 확인합니다.

   ![](assets/utilization-chart-hover-350x176.png)

1. (선택 사항) 필터를 조정하여 차트에 표시할 정보를 결정합니다. 필터 조정에 대한 자세한 내용은 섹션을 참조하십시오 [사용률 정보 필터링](#filter-utilization-information) 참조하십시오.
1. (선택 사항) 섹션에 설명된 대로 차트 보고서의 기간을 구성합니다 [정보가 표시되는 날짜 범위를 조정합니다](#adjust-the-date-range-for-which-information-is-displayed) 참조하십시오.
