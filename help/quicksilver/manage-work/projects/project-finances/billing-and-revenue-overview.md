---
content-type: overview
product-area: projects
navigation-topic: financials
title: 청구 및 수익 개요
description: 프로젝트 관리자는 청구 요금을 사용하여 프로젝트의 매출을 캡처할 수 있습니다.
author: Lisa
feature: Work Management
exl-id: 400abcde-e368-4a70-89a9-05027900ab81
source-git-commit: dbc4404501e20b3f1905a5eebd13734a65db27ae
workflow-type: tm+mt
source-wordcount: '3691'
ht-degree: 0%

---

# 청구 및 수익 개요

<!-- Audited: 1/2024 -->

{{highlighted-preview}}

프로젝트 관리자는 청구 요금을 사용하여 프로젝트의 매출을 캡처할 수 있습니다.

이 문서에서는 프로젝트의 매출 추적에 대해 설명합니다. 매출은 활용성 보고서에서 다르게 계산됩니다. 사용률 보고서의 수익 계산에 대한 자세한 내용은 [리소스 사용률 정보 보기](../../../resource-mgmt/resource-utilization/view-utilization-information.md)를 참조하십시오.

## 청구 요금 개요

청구 요율을 사용할 때는 다음 사항을 고려하십시오.

* 청구 요율을 관리하려면 재무 데이터에 대한 편집 액세스 권한이 있는 플랜 또는 표준 라이센스가 필요합니다.\
  재무 데이터에 대한 액세스 권한을 부여하는 방법에 대한 자세한 내용은 [재무 데이터에 대한 액세스 권한 부여](../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-financial.md)를 참조하십시오.

* 청구 요금은 작업 역할 또는 사용자와 연결된 작업 단위당 매출액입니다.

  요율에 작업 시간을 곱하면 프로젝트의 수익이 생성됩니다.

* 청구 요율을 설정한 후 청구 기록을 생성하여 청구된 항목과 청구되지 않은 항목을 기록하여 매출을 추적할 수 있습니다.

  >[!TIP]
  >
  >청구 기록을 청구됨으로 표시하면 절대 편집할 수 없습니다. 이는 요금이 다르고 프로젝트에 대한 수입 및 경비 정보를 잠그려는 경우에 중요합니다. 청구 기록에 추가하고 청구됨으로 표시하면 시스템에서 요금이 업데이트될 때 업데이트되지 않습니다.

  청구 기록 만들기에 대한 자세한 내용은 문서 [청구 기록 만들기](../../../manage-work/projects/project-finances/create-billing-records.md)를 참조하십시오.

* 사용자, 작업 역할에 대한 청구 요율을 생성하거나 프로젝트나 작업에 대한 일회성 청구 요율을 가질 수 있습니다.

>[!IMPORTANT]
>
>매출을 계산하는 비율은 시간을 기록하는 사용자 또는 해당 작업 역할에 속합니다.

* [사용자 청구 요금](#user-billing-rates)
* [작업 역할 청구 요금](#job-role-billing-rates)
* [프로젝트 또는 작업에 대한 고정 청구 요금](#fixed-billing-rates-for-projects-or-tasks)
* [청구 요금 재정의](#override-billing-rates)

### 사용자 청구 요금 {#user-billing-rates}

사용자 관리자는 사용자를 생성할 때 시간당 청구 필드에 대한 값과 요금에 대한 일자를 지정하여 이 사용자를 일자 유효 청구 요금과 연관시킬 수 있습니다.

사용자 만들기에 대한 자세한 내용은 문서 [사용자 추가](../../../administration-and-setup/add-users/create-and-manage-users/add-users.md)를 참조하십시오.

![사용자 비용 및 청구 요금 편집](assets/edit-user-cost-billing-rate-1.png)

### 작업 역할 청구 요금 {#job-role-billing-rates}

Adobe Workfront 관리자는 작업 역할을 생성할 때 시간당 청구 필드에 대한 값과 청구 요금에 대한 날짜를 지정하여 이 역할을 날짜 유효 청구 요금과 연결할 수 있습니다.

Workfront 시스템의 기본 통화 또는 다른 사용자 지정 통화를 사용하여 작업 역할 청구 요금의 값을 정의할 수 있습니다.

작업 역할을 만들고 통화를 재정의하는 방법에 대한 자세한 내용은 문서 [작업 역할 만들기 및 관리](../../../administration-and-setup/set-up-workfront/organizational-setup/create-manage-job-roles.md)를 참조하십시오.

![작업 역할 비용 및 청구 요금 편집](assets/edit-job-role-multiple-billing-rates-new.png)

### 프로젝트 또는 작업에 대한 고정 청구 요금 {#fixed-billing-rates-for-projects-or-tasks}

사용자 및 작업 역할 시간당 요금 외에도 다음과 같은 고정 청구 요금이 있을 수 있습니다.

* 고정 시간당 수익 유형에 대한 고정 금액
* 고정 수익 유형에 대한 고정 금액

고정 청구 요금을 사용하여 수익을 계산하는 방법에 대한 자세한 내용은 [작업 수익 유형 개요](#overview-of-task-revenue-types)를 참조하십시오.

### 청구 요금 재정의 {#override-billing-rates}

>[!IMPORTANT]
>
>작업 역할과 연관된 청구 요율을 대체할 수 있습니다. 사용자 청구 요금 또는 고정 요금은 재정의할 수 없습니다.

다음에 대한 작업 역할 청구 요율을 재정의할 수 있습니다.

* 특정 회사

  회사별 작업 역할 청구 요율을 만드는 방법에 대한 자세한 내용은 [회사 만들기 및 편집](../../../administration-and-setup/set-up-workfront/organizational-setup/create-and-edit-companies.md)을 참조하십시오.

* 특정 프로젝트

  프로젝트에 대한 작업 역할 청구 요율을 만드는 방법에 대한 자세한 내용은 문서 [작업 역할 청구 요율 재정의 개요 및 프로젝트의 수익 계산](../../../manage-work/projects/project-finances/override-role-billing-rates-and-calculate-project-revenue.md)을 참조하십시오.

## 수익 금액 추적

Workfront은 작업의 계획된 시간을 기반으로 작업이 생성될 때 계획된 수익을 자동으로 추적할 수 있습니다.

또한 작업, 문제 및 프로젝트에 실제 시간이 기록될 때 실제 수익을 자동으로 추적할 수도 있습니다.

다음 표는 작업, 문제 및 프로젝트와 관련된 수익 유형을 보여 줍니다.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">계획된 수익</td> 
   <td> <p>작업의 경우 계획된 작업 시간과 관련된 매출입니다. 모든 작업의 계획된 시간은 프로젝트 계획된 시간 계산에 기여하기 위해 프로젝트의 계획된 시간으로 롤업됩니다. </p> <p>Workfront의 계획된 시간에 대한 자세한 내용은 <a href="../../../manage-work/tasks/task-information/planned-hours.md" class="MCXref xref">계획된 시간 개요</a>를 참조하십시오. </p> <ul><li><p>Workfront은 다음 공식을 사용하여 작업에 대한 계획된 수익을 계산합니다.</p>
   <p><code>Task Planned Revenue = Planned Hours * Billing hourly rate</code><p> <p><strong>참고</strong></br> 공식의 청구 시간당 요금은 날짜 대비 요금의 변경 사항을 고려합니다.</p> </li><li><p>Workfront은 다음 공식을 사용하여 프로젝트의 계획된 수익을 계산합니다.</p> <p><code>Project Planned Revenue = SUM (All tasks Planned Revenue) + Fixed Revenue</code></p>
   <p><b>메모</b>

<p>프로젝트 세부 정보 영역 및 프로젝트 보고서에 표시되는 프로젝트 계획 수익이 활용률 보고서에 표시되는 계획 수익과 다릅니다. </p></li></ul> <p>프로젝트 세부 정보 영역의 계획된 수익에는 프로젝트의 고정 수익뿐만 아니라 작업 계획 시간과 연관된 작업 수익이 반영됩니다. 활용성 보고서의 계획된 수익에는 프로젝트에 대한 태스크 지정의 계획된 시간에만 연관된 계획된 수익이 표시됩니다. </p> 
     <div class="example" data-mc-autonum="<b>Example: </b>"> 
      <p>프로젝트에 10시간의 작업이 1개 있고 시간당 비율이 $20인 컨설턴트에게 할당되어 있으며 프로젝트에 $100의 고정 수익이 있는 경우, 활용률 보고서에는 계획된 수익(작업의 시간과 연결된 계획된 수익)에 대해 $200가 표시됩니다. 프로젝트 세부 정보 섹션에는 $300(작업의 계획된 수익 및 프로젝트에 대한 고정 수익)이 표시됩니다. </p> 
     </div> </p> <p>작업 계획 매출은 작업에 할당된 사용자 또는 작업 역할의 청구 시간당 요금을 사용하여 계산됩니다. 작업의 수익 유형은 계획된 수익 계산에 사용되는 비율(사용자 또는 역할)에 영향을 줍니다. 자세한 내용은 이 문서의 다음 섹션을 참조하십시오.</p> 
    <ul> 
     <li> <p><a href="#overview-of-task-revenue-types" class="MCXref xref">작업 수익 유형 개요</a> </p> </li> 
     <li> <p><a href="#revenue-calculations-for-tasks-based-on-user-and-role-assignments" class="MCXref xref">사용자 및 역할 할당에 따른 작업에 대한 수익 계산</a> </p> </li> 
    </ul> <p>사용률 보고서의 계획된 수익 계산에 대한 자세한 내용은 <a href="../../../resource-mgmt/resource-utilization/view-utilization-information.md" class="MCXref xref">리소스 사용률 정보 보기</a>를 참조하십시오. </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">실제 수익*</td> 
   <td> <p>작업, 문제 및 프로젝트의 실제 시간과 관련된 매출입니다. </p> <p>일반적으로 Workfront은 다음 공식을 사용하여 실제 매출을 계산합니다.</p> <p><code>Actual Revenue = Actual Hours * Billing rate</code> </p> <p><strong>참고</strong></br> 공식의 청구 시간당 요금은 날짜 대비 요금의 변경 사항을 고려합니다.</p> <p>사용률 보고서의 실제 수익 계산에 대한 자세한 내용은 <a href="../../../resource-mgmt/resource-utilization/view-utilization-information.md" class="MCXref xref">리소스 사용률 정보 보기</a>를 참조하십시오. </p> <p><b>팁</b>

문제 수준에서 실제 수익을 볼 수 없지만 문제의 실제 시간과 연결된 수익이 프로젝트의 실제 수익에 기여합니다. </p> </td>
</tr> 
 </tbody> 
</table>

*실제 사용 시간의 경우 사용자 비율은 항상 시간을 기록하는 사용자 또는 작업 역할 비율을 나타냅니다. Workfront에서 사용자 비율을 사용하는 시점과 작업 역할 비율을 사용하는 시점에 대한 자세한 내용은 이 문서의 [매출 계산](#revenue-calculations) 섹션을 참조하십시오.

<!--Note from the table for Planned Revenue line: 
     <p data-mc-conditions="QuicksilverOrClassic.Draft mode">(the note below is duplicated in this article: /Content/Resource Mgmt/Resource utilization/view-utilization-information.htm and in the glossary)</p>
    -->

예를 들어, 사용자 시간당 수익 유형의 작업이 2시간 소요되도록 계획되고 여기에 할당된 사용자의 시간당 비율이 $30인 경우 작업의 계획된 수익은 $60입니다. 작업이 완료되면 사용자가 작업을 완료하는 데 걸린 실제 시간으로 1.5시간만 기록하면 실제 매출액은 $45입니다. 작업에 할당되지 않은 다른 사용자가 시간을 기록하는 경우 실제 매출은 해당 사용자의 청구 요금을 기반으로 계산됩니다.

다음과 같은 방법으로 매출을 기록할 수 있습니다.

* 작업의 수익 유형을 정의하고 작업 항목에 지정된 사용자 또는 역할을 청구 요금과 연관시켜. 작업 항목에 대한 계획된 시간 또는 실제 시간의 양별로 매출을 계산합니다. 시간당 요금에 대해 부과되는 최대 금액으로 상한을 설정할 수 있습니다.\
  작업의 매출 유형 지정에 대한 자세한 내용은 문서 [작업 편집](../../../manage-work/tasks/manage-tasks/edit-tasks.md)을 참조하십시오.

* 작업 또는 프로젝트에 대한 고정 수입 요금을 청구하여.\
  고정 수익이 있는 작업이 있는 경우 고정 수익 금액은 작업 또는 프로젝트의 계획 수익으로 추가되며 작업의 계획 수익은 고정 수익으로 청구 기록에 추가할 수 있습니다.
* 프로젝트에 대한 고정 청구 고정 수익 요금을 설정한 다음 프로젝트 내 작업에 대한 시간당 요금을 설정합니다. Workfront은 작업의 시간당 요금을 프로젝트의 고정 요금에 추가합니다.\
  예를 들어, Workfront을 사용하는 정비사가 프로젝트의 고정 수입으로 부품 비용을 입력한 다음, 차를 고치는 데 걸린 시간을 시간별로 청구할 수 있습니다. 프로젝트 또는 작업에 대한 고정 수익이 완료 시 실현됩니다.

작업을 &quot;청구 불가&quot;로 표시할 수도 있습니다. 이 경우 작업과 연결된 계획된 수익 또는 실제 수익이 없습니다.

## 작업 수익 유형 개요 {#overview-of-task-revenue-types}

기본적으로 모든 새 작업의 매출 유형은 Workfront 또는 그룹 관리자가 지정한 작업 및 문제 환경 설정에 따라 설정됩니다.\
Workfront 인스턴스의 작업 및 문제 환경 설정을 정의하는 방법에 대한 자세한 내용은 [시스템 전체 작업 및 문제 환경 설정 구성](../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-task-issue-preferences.md) 문서를 참조하십시오.

프로젝트 소유자는 작업의 수익 유형과 프로젝트의 고정 수익을 수정할 수 있습니다.\
프로젝트의 고정 수익 지정에 대한 자세한 내용은 [프로젝트 편집](../../../manage-work/projects/manage-projects/edit-projects.md) 문서를 참조하십시오.\
작업의 매출 유형 지정에 대한 자세한 내용은 문서 [작업 편집](../../../manage-work/tasks/manage-tasks/edit-tasks.md)을 참조하십시오.

작업 또는 프로젝트에 다음 수익 유형을 적용할 수 있습니다.

<table border="1" cellspacing="15"> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th> <p><strong>수익 유형</strong> </p> </th> 
   <th> <p><strong>설명</strong> </p> </th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td> <p>고정 수입</p> </td> 
   <td> <p>이 유형은 프로젝트 및 작업과 함께 사용할 수 있습니다. </p> <p>템플릿을 프로젝트에 첨부할 때 템플릿의 고정 수익이 프로젝트의 고정 수익에 추가됩니다. 자세한 내용은 <a href="../../../manage-work/projects/create-and-manage-templates/attach-template-to-project-overview.md" class="MCXref xref">프로젝트에 템플릿을 첨부하는 개요</a>를 참조하십시오. </p> <p>태스크의 경우 태스크 지정에 관계없이 태스크의 수익은 항상 태스크에 지정된 고정 금액을 사용하여 계산됩니다. </p> <p>하위 작업의 고정 수익은 상위 작업의 수익으로 적상된 다음 프로젝트의 수익으로 적상됩니다. 상위 작업 및/또는 프로젝트에 고정 금액이 정의된 경우 금액은 하위 작업에서 롤업된 계획된 수익에 추가됩니다.</p> <p>작업의 고정 매출액은 프로젝트의 청구 기록에 포함될 수 있습니다.</p> </td> 
  </tr> 
  <tr> 
   <td> <p>시간별 사용자</p> </td> 
   <td> <p>이 유형은 작업에만 사용할 수 있습니다. </p> <p>특정 사용자에 대해 설정한 청구 요금에 해당 작업의 계획된 시간을 곱한 값이 작업의 계획된 수익 금액이 됩니다. 특정 사용자에 대해 설정한 청구 요금에 사용자가 작업에 대해 기록한 시간을 곱한 값이 작업의 실제 수익 금액입니다. <br>예를 들어 사용자를 만들고 시간당 청구 필드에 $20를 설정하면 사용자가 타임시트의 작업에 대해 5시간을 제출하면 작업의 실제 청구 금액은 $100입니다.</p>
   <p>사용자 프로필에는 유효 일자가 있는 여러 청구 요금이 포함될 수 있습니다. 예를 들어 $20의 첫 번째 사용자 청구 요금은 2023년 4월 30일에 종료되고 $25의 두 번째 사용자 청구 요금은 2023년 5월 1일에 시작됩니다. 사용자가 작업에 대해 4월 28일에 2시간, 5월 2일에 3시간을 제출한 경우 작업의 실제 청구 금액은 $40 + $75 = $115입니다.</p>
   <p><b>팁</b>

작업을 만들 때 기본 수익 유형입니다.</p> </td>
</tr> 
  <tr> 
   <td> <p>시간별 역할</p> </td> 
   <td> <p>이 유형은 작업에만 사용할 수 있습니다.</p> <p>이 유형은 시간별 사용자 수와 유사하지만 사용자 요금이 아닌 작업 역할 요금을 사용합니다.</p> <p><strong>참고</strong><br>작업 역할에는 유효 날짜가 포함된 청구 요금이 여러 개 있을 수도 있습니다.</p></td> 
  </tr> 
  <tr> 
   <td> <p>시간별 사용자(상한 포함)</p> </td> 
   <td> <p>이 유형은 작업에만 사용할 수 있습니다.</p> <p>작업은 시간별 사용자에서와 같이 시간별로 청구되지만 지정할 수 있는 최대 한도 금액이 있습니다. <br>예를 들어, 사용자의 청구 요금이 $25이지만 작업의 상한 금액이 $20이고 사용자가 1시간 동안 기록하는 경우 작업의 실제 매출은 $20입니다. </p> </td> 
  </tr> 
  <tr> 
   <td> <p>시간별 역할(상한 포함)</p> </td> 
   <td> <p>이 유형은 작업에만 사용할 수 있습니다.</p> <p>이 유형은 상한이 있는 시간별 사용자 와 유사하지만 사용자 요금이 아닌 작업 역할 요금을 사용합니다. </p> </td> 
  </tr> 
  <tr> 
   <td> <p>시간별 + 고정 사용자</p> </td> 
   <td> <p>이 유형은 작업에만 사용할 수 있습니다. </p> <p>작업은 시간별 사용자에서와 같이 시간별로 청구되지만 사용자 요금에 추가할 수 있는 고정 금액이 있습니다. 작업에 지정된 고정 금액은 프로젝트의 청구 기록에 포함될 수 있습니다. 고정 금액에 작업의 시간을 곱하지 않습니다. 사용자 청구 요금만 해당됩니다. </p> </td> 
  </tr> 
  <tr> 
   <td> <p>시간별 + 고정 역할</p> </td> 
   <td> <p>이 유형은 작업에만 사용할 수 있습니다. </p> <p>작업은 시간별 역할에서처럼 시간별로 청구되지만 역할 요금에 추가할 수 있는 추가 고정 금액이 있습니다. 작업에 지정된 고정 금액은 프로젝트의 청구 기록에 포함될 수 있습니다. 고정 금액에 작업의 시간을 곱하지 않습니다. 작업 역할 청구 요금만 해당됩니다. </p> </td> 
  </tr> 
  <tr> 
   <td> <p>고정 시간별</p> </td> 
   <td> <p>이 유형은 작업에만 사용할 수 있습니다.</p> <p>태스크에 대해 설정한 상한 또는 고정 금액에 태스크에 대해 입력된 시간 수(사용자 또는 해당 작업 역할에 관계 없음)를 곱한 금액이 청구 금액입니다.</p> </td> 
  </tr> 
  <tr> 
   <td> <p>과금 불가</p> </td> 
   <td> <p>이 유형은 작업에만 사용할 수 있습니다.</p> <p>이 수익 유형은 수익에 영향을 주지 않습니다. </p> <p>상위 오브젝트에 이 설정이 있는 경우 청구 유형의 하위 작업이 여전히 정상적으로 적용됩니다.</p> <p>재무 데이터에 대한 액세스 권한이 없는 사용자 또는 템플릿에 대한 재무 권한이 없는 사용자가 해당 템플릿에서 프로젝트를 만들 때 프로젝트의 작업에 대한 기본 수익 유형이 됩니다.</p> <p>재무 데이터에 대한 액세스 정보는 문서 <a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-financial.md" class="MCXref xref">재무 데이터에 대한 액세스 권한 부여</a>를 참조하십시오.<br>개체에 대한 재무 사용 권한에 대한 자세한 내용은 <a href="../../../workfront-basics/grant-and-request-access-to-objects/sharing-permissions-on-objects-overview.md" class="MCXref xref">개체에 대한 공유 권한 개요</a> 문서를 참조하십시오.<br>템플릿으로 프로젝트를 만드는 방법에 대한 자세한 내용은 문서 <a href="../../../manage-work/projects/create-projects/create-project-from-template.md" class="MCXref xref">템플릿을 사용하여 프로젝트 만들기</a>를 참조하십시오. </p> </td> 
  </tr> 
 </tbody> 
</table>

## 상위 작업의 수익 개요

청구 정보가 있는 독립형 태스크를 상위로 변경하면 신규 상위 태스크에는 이전에 적용된 시간과 함께 이전에 적용된 청구 정보가 유지됩니다. 하위 작업에 기록된 시간에서 오는 모든 청구 정보는 새 상위 작업에 실제 수익으로 적상됩니다.

하위 작업의 계획된 수익도 상위 작업에 롤업됩니다.

## 문제에 대한 수익 개요

문제에는 계획된 또는 실제 수익 금액이 없지만 실제 비용이 있을 수 있습니다.

문제에 대한 시간을 기록하고 &quot;수익으로 계산&quot;으로 표시된 시간 유형을 사용하는 경우, Workfront은 해당 시간에 로그인하는 사용자의 비율에 따라 실제 비용 금액을 계산합니다. 이 숫자는 프로젝트의 실제 비용에 추가됩니다. 청구 기록에 시간을 포함할 수도 있습니다.

비용 추적에 대한 자세한 내용은 문서 [비용 추적](../../../manage-work/projects/project-finances/track-costs.md)을 참조하세요.

시간 유형에 대한 자세한 내용은 문서 [시간 유형 관리](../../../administration-and-setup/set-up-workfront/configure-timesheets-schedules/hour-types.md)를 참조하십시오.

## 수익 계산

* [사용자 및 역할 할당을 기반으로 한 작업에 대한 수익 계산](#revenue-calculations-for-tasks-based-on-user-and-role-assignments)

### 사용자 및 역할 할당을 기반으로 한 작업에 대한 수익 계산 {#revenue-calculations-for-tasks-based-on-user-and-role-assignments}

작업에 대한 매출을 계산할 때 다음 사항을 고려하십시오.

* 사용자 또는 작업 역할에 $0.00 비율이 표시되면 Workfront은 해당 금액을 유효한 금액으로 읽고 해당 금액에 작업의 시간을 곱하여 수익을 계산합니다. 작업에 대한 매출을 표시하지 않으려면 사용자 또는 작업 역할에 대한 청구 요금에 대한 필드가 비어 있는지 확인합니다.
* 작업 역할 청구 요금이 적용되면 Workfront은 프로젝트에 오버라이드 요금이 있을 때마다 시스템 수준에서 정의된 해당 역할에 대한 청구 요금 대신 프로젝트 수준에서 오버라이드 요금을 사용합니다.
* 실제 매출의 경우, 사용자 또는 작업 역할에 유효 일자가 있는 청구 요금이 여러 개 있는 경우 작업 매출은 사용자가 시간을 기록한 각 기간의 매출의 합계입니다. 계획된 수익은 기간에 대한 계획된 시간을 기반으로 합니다.
* 작업에 여러 명의 할당자가 있는 경우 아래 설명된 시나리오가 각 할당자에 적용됩니다.

태스크 지정을 기준으로 수익 계산에 사용되는 비율이 있는 계층이 있습니다.

Workfront 관리자가 [타임시트 및 시간 환경 설정] 영역에서 **시간 항목에 수동으로 작업 역할 할당** 설정을 활성화했으며 프로젝트의 사용자 로깅 시간이 이 시간과 연결할 다른 역할을 선택한 경우 작업 또는 프로젝트의 실제 매출은 항상 시간 항목과 연결된 역할을 기반으로 계산됩니다. 특정 작업 역할에 대한 로깅 시간 활성화에 대한 자세한 내용은 문서 [타임시트 및 시간 환경 설정 구성](../../../administration-and-setup/set-up-workfront/configure-timesheets-schedules/timesheet-and-hour-preferences.md)을 참조하십시오.

수익 유형 및 태스크 지정의 특성에 따라 태스크 수익을 계산할 때 다음과 같은 시나리오가 있습니다.

* **작업의 매출 유형은 시간별 사용자입니다**

  <table style="table-layout:auto"> 
   <col> 
   <col> 
   <col> 
   <col> 
   <tbody> 
    <tr> 
     <td role="rowheader">시간당 청구 요금</td> 
     <td>할당 없음</td> 
     <td>사용자 할당</td> 
     <td>작업 역할 할당</td> 
    </tr> 
    <tr> 
     <td role="rowheader">계획된 수익에 대한 시간당 청구 요금</td> 
     <td>US$0.00</td> 
     <td> 사용자가 프로필에 청구 요금이 있는 경우 해당 요금이 계획된 수익을 계산하는 데 사용됩니다. 그렇지 않으면 기본 작업 역할의 시스템 청구 요금이 사용됩니다. <br><p><b>참고</b> 사용자는 보조 작업 역할 중 하나를 사용하여 작업에 할당할 수 있지만 기본 작업 역할의 비율이 대신 여기에 사용됩니다.</p><p>할당 중에 사용자의 역할이 변경된 경우 프로젝트 재정이 다시 계산될 때 정확한 비율이 적용됩니다.</p></td> 
     <td><p><span class="preview">비율 카드가 프로젝트에 첨부된 경우 계획된 수익은 비율 카드의 작업 역할을 기준으로 계산됩니다.</span></p> <p><span class="preview">프로젝트 수준에서 청구 요금이 재정의될 수 있습니다.</span></p></td> 
    </tr> 
    <tr> 
     <td role="rowheader">실제 매출에 대한 시간당 청구 요금</td> 
     <td>시간을 기록하는 사용자가 프로필에 청구 요금이 있는 경우 해당 요금이 사용됩니다. 
     <br><span class="preview">고급 할당에서 위치별 할당이 있는 사용자 또는 역할에 대해 시간이 기록되면 해당 위치의 비율이 사용됩니다.</span>
     <br>그렇지 않으면 기본 작업 역할의 청구 요금이 사용됩니다. 사용자 또는 기본 역할과 연결된 청구 요금이 없는 경우 실제 매출은 $0.00입니다. <br><p><b>메모</b>

  다른 사용자가 작업에 할당된 경우에도 시간을 기록한 사용자와 관련된 비율만 계산에 고려됩니다.</p></td>
  <td>시간을 기록하는 사용자가 프로필에 청구 요금이 있는 경우 해당 요금이 사용됩니다. <br><span class="preview">고급 할당에서 위치별 할당이 있는 사용자 또는 역할에 대해 시간이 기록되면 해당 위치의 비율이 사용됩니다.</span><br>그렇지 않으면 기본 작업 역할의 청구 요금이 사용됩니다. 사용자 또는 기본 역할과 연결된 청구 요금이 없는 경우 실제 매출은 $0.00입니다. <br><p><b>메모</b>

  다른 사용자가 작업에 할당된 경우에도 시간을 기록한 사용자와 관련된 비율만 계산에 고려됩니다.</p></td>
  <td>시간을 기록하는 사용자가 프로필에 청구 요금이 있는 경우 해당 요금이 사용됩니다. 그렇지 않으면 기본 작업 역할의 청구 요금이 사용됩니다.<br><p><b>메모</b>

  사용자 로깅 시간에 연결된 청구 요금이 없고 작업 역할이나 작업 역할에 대한 청구 요금이 없는 경우 작업과 연결된 작업 역할의 요금이 사용됩니다. 이 역할에 대한 청구 요금이 없는 경우 매출은 $0.00입니다.</p></td>
  </tr> 
   </tbody> 
  </table>

* **작업의 매출 유형은 시간별 역할입니다**

  <table style="table-layout:auto"> 
   <col> 
   <col> 
   <col> 
   <col> 
   <tbody> 
    <tr> 
     <td role="rowheader">시간당 청구 요금</td> 
     <td>할당 없음</td> 
     <td>사용자 할당</td> 
     <td>작업 역할 할당</td> 
    </tr> 
    <tr> 
     <td role="rowheader">계획된 수익에 대한 시간당 청구 요금</td> 
     <td>US$0.00</td> 
     <td><p>Workfront은 사용자가 계획된 수익을 계산하기 위해 작업을 수행하는 작업 역할을 봅니다. <br>사용자가 작업에 연결된 역할이 없으면 매출은 $0.00입니다.</p> <p><strong>참고</strong><br>할당 중에 사용자 역할이 변경된 경우 프로젝트 재무 정보가 다시 계산되면 올바른 비율이 적용됩니다.</p> </td> 
     <td><p><span class="preview">비율 카드가 프로젝트에 첨부된 경우 계획된 수익은 비율 카드의 작업 역할을 기준으로 계산됩니다.</span></p> <p><span class="preview">프로젝트 수준에서 청구 요금이 재정의될 수 있습니다.</span></p></td> 
    </tr> 
    <tr> 
     <td role="rowheader">실제 매출에 대한 시간당 청구 요금</td> 
     <td>Workfront은 시간을 기록하는 사용자의 기본 작업 역할에 대한 청구 요금을 사용합니다. <br><span class="preview">고급 할당에서 위치별 할당이 있는 사용자 또는 역할에 대해 시간이 기록되면 해당 위치의 비율이 사용됩니다.</span> <br>시간을 기록하는 사용자에게 연결된 작업 역할이 없거나 기본 작업 역할에 청구 요금이 없는 경우 실제 매출은 $0.00입니다. </td> 
     <td> 시간을 기록한 사용자가 작업에 할당된 경우 작업에 대한 사용자와 연결된 작업 역할의 청구 요금이 실제 수익을 계산하는 데 사용됩니다. <br><span class="preview">고급 할당에서 위치별 할당이 있는 사용자 또는 역할에 대해 시간이 기록되면 해당 위치의 비율이 사용됩니다.</span> <br>그렇지 않으면 기본 작업 역할의 청구 요금이 사용됩니다. 사용자에게 기본 작업 역할이 없거나 기본 작업 역할에 청구 요금이 없는 경우 실제 매출은 $0.00입니다. </td> 
     <td>시간을 기록하는 사용자의 작업 역할 중 하나가 작업에 할당되면 해당 작업 역할 비율이 사용됩니다. 작업에 할당된 작업 역할이 시간을 기록하는 사용자와 연결되어 있지 않으면 사용자의 기본 역할에 대한 청구 요금을 사용하여 실제 수익을 계산합니다. 사용자에게 작업 역할이 없거나 기본 작업 역할과 연결된 비율이 없는 경우 작업에 할당된 작업 역할의 비율이 사용됩니다. </td> 
    </tr> 
   </tbody> 
  </table>

<!--
<div data-mc-conditions="QuicksilverOrClassic.Draft mode">
<p>Ideal table but does not come across Markdown</p>
<table style="table-layout:auto">
<col>
<col>
<col>
<col>
<col>
<col>
<col>
<tbody>
<tr>
<td colspan="3">Revenue Type = User Hourly</td>
<td colspan="4">Revenue Type = Role Hourly</td>
</tr>
<tr>
<td> <p> </p> </td>
<td> <p><strong>No Assignment</strong> </p> </td>
<td> <p><strong>User Assignment</strong> </p> </td>
<td> <p><strong>Job Role Assignment</strong> </p> </td>
<td> <p><strong>No Assignment</strong> </p> </td>
<td> <p><strong>User Assignment</strong> </p> </td>
<td> <p><strong>Job Role Assignment</strong> </p> </td>
</tr>
<tr>
<td> <p><strong>Billing per hour rate for Planned Revenue</strong> </p> </td>
<td> <p>$0.00</p> </td>
<td> <p> If a user has a billing rate in their profile, then that rate is used to calculate Planned Revenue. Otherwise, the system billing rate of their primary job role is used. <br><note type="note">
The user can be assigned to the task with one of their secondary job roles, but the rate of the primary job role is used here instead.
</note></p> </td>
<td> <p> The system billing rate of the job role assigned to the task is used to calculate Planned Revenue. </p> </td>
<td> <p>$0.00</p> </td>
<td> <p>Workfront looks at the job role that the user fulfills on the task to calculate the Planned Revenue. <br>If the user is not associated with any role on the task, the Revenue is $0.00. </p> </td>
<td> <p>The billing rate of the job role assigned to the task is used to calculate Planned Revenue. </p> <p> </p> <p> </p> </td>
</tr>
<tr>
<td> <p><strong>Billing per hour rate for Actual Revenue</strong> </p> </td>
<td colspan="2"> <p>If the user logging the hours has a billing rate in their profile, that rate is used. <br>Otherwise, the billing rate of their primary job role is used. If there is no billing rate associated with the user or their primary role, the Actual Revenue is $0.00. <br><note type="note">
Only the rates associated with the user logging the time are taken into account for the calculation, even when another user is assigned to the task.
</note></p> </td>
<td> If the user logging the hours has a billing rate in their profile, that rate is used. Otherwise, the billing rate of their primary job role is used.<br><note type="note">
If the user logging time has no billing rate associated with them, and they do not have a job role or a billing rate for their job role, then the rate from the job role associated with the task is used. If there is no billing rate for this role, the revenue is $0.00
</note></td>
<td> <p>Workfront uses the billing rate of the primary job role of the user logging the time. <br>If the user logging the time has no job role associated with them, or if the primary job role has no billing rate, the Actual Revenue is $0.00. </p> </td>
<td> <p> If the user logging the time is assigned to the task, the billing rate of the job role associated with the user on the task is used to calculate the Actual Revenue. Otherwise, the billing rate of their primary job role is used. If the user has no primary job role or if their primary job role has no billing rate, the Actual Revenue is $0.00. </p> </td>
<td> <p>If one of the job roles of the user logging the time is assigned to the task, that job role rate is used. If the job role assigned to the task is not associated with the user logging the time, then the billing rate of the primary role of the user is used to calculate the Actual Revenue. If the user does not have a job role or there is no rate associated with their primary job role, then the rate of the job role assigned to the task is used. </p> </td>
</tr>
</tbody>
</table>
</div>
-->

### 프로젝트에 대한 수익 계산

프로젝트에 대한 다음 수익 유형을 추적할 수 있습니다.

* 프로젝트의 계획된 수익은 다음 공식에 의해 계산됩니다.

  `Project Planned Revenue = SUM(Task Planned Revenue)+ Fixed Revenue`

  작업 계획 수익 계산 방법에 대한 자세한 내용은 이 문서의 [사용자 및 역할 할당에 따른 작업에 대한 수익 계산](#revenue-calculations-for-tasks-based-on-user-and-role-assignments) 섹션을 참조하십시오.

* 프로젝트의 실제 매출은 다음 공식에 의해 계산됩니다.

  `Project Actual Revenue = SUM (Task Actual Revenue) + (Hours logged for the project x User Billing per Hour Rate) + SUM (Hours logged for the issues x User Billing per Hour rate)`

작업 실제 수익 계산 방법에 대한 자세한 내용은 이 문서의 [사용자 및 역할 할당에 따른 작업에 대한 수익 계산](#revenue-calculations-for-tasks-based-on-user-and-role-assignments) 섹션을 참조하십시오.

프로젝트에 직접 기록된 시간 또는 문제와 관련된 실제 매출의 경우 Workfront에서는 프로젝트에 시간을 기록한 사용자의 청구 요금을 사용합니다. 사용자에게 프로필과 연결된 청구 요금이 없는 경우 Workfront은 기본 작업 역할의 청구 요금을 사용합니다. 두 비율이 모두 0인 경우 프로젝트에 기록된 시간 또는 문제와 관련된 실제 매출은 0입니다.
