---
content-type: overview
product-area: projects
navigation-topic: financials
title: 청구 및 수익 개요
description: 프로젝트 관리자는 청구 비율을 사용하여 프로젝트에서 수익을 캡처할 수 있습니다.
author: Alina
feature: Work Management
exl-id: 400abcde-e368-4a70-89a9-05027900ab81
source-git-commit: 518a552845598a30fd547d432aa9d22dfef6ec8e
workflow-type: tm+mt
source-wordcount: '3313'
ht-degree: 0%

---

# 청구 및 수익 개요

프로젝트 관리자는 청구 비율을 사용하여 프로젝트에서 수익을 캡처할 수 있습니다.

이 문서에서는 프로젝트에 대한 추적 매출에 대해 설명합니다. 매출은 활용률 보고서에서 다르게 계산됩니다. 활용률 보고서의 수익 계산에 대한 자세한 내용은 [자원 사용률 정보 보기](../../../resource-mgmt/resource-utilization/view-utilization-information.md).

## 청구 비율 개요

청구 단가 작업 시 다음 사항을 고려하십시오.

* 청구 비율을 관리하려면 재무 데이터에 대한 편집 액세스 권한이 있는 계획 라이센스가 필요합니다.\
   재무 데이터에 대한 액세스 권한 부여에 대한 자세한 내용은 [재무 데이터에 대한 액세스 권한 부여](../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-financial.md).

* 청구 비율은 작업 역할이나 사용자와 연관된 작업 단위당 수익 금액입니다.

   작업에 사용한 시간을 곱하면 프로젝트에 대한 수익이 생성됩니다.

* 청구 비율을 설정한 후 청구 레코드를 생성하여 청구되지 않은 청구 레코드를 기록함으로써 수익을 추적할 수 있습니다.

   >[!TIP]
   >
   >청구 레코드를 청구됨으로 표시하면 편집할 수 없습니다. 이는 요금이 다르며 프로젝트에 대한 매출 및 비용 정보를 잠그려는 경우에 중요합니다. 청구 레코드에 추가하고 청구됨으로 표시하면 시스템에서 요금이 업데이트될 때 업데이트되지 않습니다.

   청구 레코드 생성에 대한 자세한 내용은 문서를 참조하십시오 [청구 레코드 만들기](../../../manage-work/projects/project-finances/create-billing-records.md).

* 사용자, Job 역할에 대한 청구 비율을 생성하거나 프로젝트 또는 작업에 대해 1회 청구 비율을 가질 수 있습니다.

>[!IMPORTANT]
>
>수입을 계산하는 비율은 시간을 기록하는 사용자 또는 해당 작업 역할에 속하는 것입니다.

* [사용자 청구 비율](#user-billing-rates)
* [직무 역할 청구 비율](#job-role-billing-rates)
* [프로젝트 또는 작업에 대한 고정 청구 비율](#fixed-billing-rates-for-projects-or-tasks)
* [청구 비율 대체](#override-billing-rates)

### 사용자 청구 비율 {#user-billing-rates}

사용자 관리자는 사용자를 생성할 때 해당 프로필의 시간당 청구 필드에 값을 지정하여 사용자를 청구 요율과 연관시킬 수 있습니다.\
사용자 만들기에 대한 자세한 내용은 문서를 참조하십시오 [사용자 추가](../../../administration-and-setup/add-users/create-and-manage-users/add-users.md)

![](assets/qs-user-edit-ui-with-rp-and-billing-per-hour-field-1-350x152.png)

### 직무 역할 청구 비율 {#job-role-billing-rates}

Adobe Workfront 관리자는 작업 역할을 생성할 때 청구/시간 필드에 값을 지정하여 청구 비율에 연결할 수 있습니다.

Workfront 시스템의 기본 통화를 사용하거나 다른 사용자 지정 통화를 사용하여 작업 역할 청구 비율 값을 정의할 수 있습니다.

Job 역할 생성 및 해당 통화 대체에 대한 자세한 내용은 문서를 참조하십시오 [작업 역할 만들기 및 관리](../../../administration-and-setup/set-up-workfront/organizational-setup/create-manage-job-roles.md)

![](assets/billing-rate-for-role-1-350x294.png)

### 프로젝트 또는 작업에 대한 고정 청구 비율 {#fixed-billing-rates-for-projects-or-tasks}

사용자 및 작업 역할 시간별 요금 외에도 다음과 같은 고정 청구 요금이 있을 수 있습니다.

* 고정된 시간별 수익 유형에 대한 고정 금액
* 고정 수익 유형에 대한 고정 금액

고정 청구 비율을 사용하여 수익을 계산하는 방법에 대한 자세한 내용은 [작업 매출 유형 개요](#overview-of-task-revenue-types).

### 청구 비율 대체 {#override-billing-rates}

>[!IMPORTANT]
>
>직무 역할과 연관된 청구 비율을 대체할 수 있습니다. 사용자 청구 단가 또는 고정 요금을 대체할 수 없습니다.

다음 작업에 대해 직무 역할 청구 비율을 대체할 수 있습니다.

* 특정 회사

   특정 회사에 대한 Job 역할 청구 단가 생성에 대한 자세한 내용은 [회사 만들기 및 편집](../../../administration-and-setup/set-up-workfront/organizational-setup/create-and-edit-companies.md).

* 특정 프로젝트

   프로젝트별 Job 역할 청구 단가 생성에 대한 자세한 내용은 문서를 참조하십시오 [Job 역할 청구 비율 대체 및 프로젝트에 대한 수익 계산 개요](../../../manage-work/projects/project-finances/override-role-billing-rates-and-calculate-project-revenue.md).

## 매출 금액 추적

Workfront은 작업의 계획 시간을 기반으로 작업을 생성할 때 자동으로 계획 매출을 추적할 수 있습니다.

또한 실제 시간이 작업, 문제 및 프로젝트에 기록되면 실제 수익을 자동으로 추적할 수도 있습니다.

다음 표에는 작업, 문제 및 프로젝트와 관련된 매출 유형이 나와 있습니다.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">계획된 수익</td> 
   <td> <p>작업의 경우, 작업 계획 시간과 연관된 수익입니다. 모든 태스크의 계획 시간은 프로젝트 계획 시간 계산에 기여하기 위해 프로젝트의 계획 시간으로 롤업됩니다. </p> <p>Workfront에서 계획된 시간에 대한 자세한 내용은 <a href="../../../manage-work/tasks/task-information/planned-hours.md" class="MCXref xref">계획 시간 개요</a>. </p> <p>Workfront은 다음 공식을 사용하여 작업 및 프로젝트에 대한 계획 수익을 계산합니다.</p> <p><code>Task Planned Revenue = Planned Hours * Billing hourly rate</code> </p> <p><code>Project Planned Revenue = SUM (All tasks Planned Revenue) +&nbsp;Fixed Revenue</code> </p> 
   <p><b>메모</b>

<p>프로젝트 상세내역 영역 및 프로젝트 보고서에 표시되는 프로젝트 계획 수익은 활용률 보고서에 표시되는 계획 수익과 다릅니다. </p> <p>프로젝트 상세내역 영역의 계획 수익은 태스크 계획 시간과 프로젝트의 고정 수익과 연관된 태스크 수익을 반영합니다. 가동률 보고서의 계획 수익에는 프로젝트의 태스크 지정에서 계획된 시간에만 연관된 계획 수익이 표시됩니다. </p> 
     <div class="example" data-mc-autonum="<b>Example: </b>"> 
      <p>프로젝트에 10시간의 작업이 있고 $20 시간별 비율을 갖는 컨설턴트에 지정되며 프로젝트에 $100 고정 수익이 있는 경우, 가동률 보고서에는 계획 수익(태스크 시간과 연관된 계획 수익)에 대해 $200가 표시됩니다. 프로젝트 상세내역 섹션에는 $300(태스크의 계획 수익 및 프로젝트의 고정 수익)이 표시됩니다. </p> 
     </div> </p> <p>작업 계획 수익은 태스크에 지정된 사용자 또는 작업 역할의 청구 시간별 비율을 사용하여 계산됩니다. 작업의 수익 유형은 계획 수익 계산에 사용되는 비율(사용자 또는 역할)에 영향을 줍니다. 자세한 내용은 이 문서에서 다음 섹션을 참조하십시오.</p> 
    <ul> 
     <li> <p><a href="#overview-of-task-revenue-types" class="MCXref xref">작업 매출 유형 개요</a> </p> </li> 
     <li> <p><a href="#revenue-calculations-for-tasks-based-on-user-and-role-assignments" class="MCXref xref">사용자 및 역할 할당을 기반으로 작업에 대한 매출 계산</a> </p> </li> 
    </ul> <p>활용률 보고서의 계획 수익 계산에 대한 자세한 내용은 <a href="../../../resource-mgmt/resource-utilization/view-utilization-information.md" class="MCXref xref">자원 사용률 정보 보기 </a>. </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">실제 수익*</td> 
   <td> <p>작업, 문제 및 프로젝트의 실제 시간과 연관됩니다. </p> <p>일반적으로 Workfront은 다음 공식을 사용하여 실제 매출을 계산합니다.</p> <p><code>Planned Revenue = Planned Hours * Billing rate</code> </p> <p>활용률 보고서의 실제 수익 계산에 대한 자세한 내용은 <a href="../../../resource-mgmt/resource-utilization/view-utilization-information.md" class="MCXref xref">자원 사용률 정보 보기 </a>. </p> <p><b>팁</b>

문제 수준에서는 실제 수익을 볼 수 없지만 문제에 대한 실제 시간과 연관된 수익은 프로젝트의 실제 매출에 기여합니다. </p> </td>
</tr> 
 </tbody> 
</table>

*실제 시간의 경우 사용자 비율은 항상 시간 또는 작업 역할의 비율을 기록하는 사용자를 의미합니다. Workfront이 사용자의 비율을 사용하는 시기와 작업 역할의 비율을 사용하는 경우에 대한 자세한 내용은 [매출 계산](#revenue-calculations) 섹션에 자세히 설명되어 있습니다.

<!--Note from the table for Planned Revenue line: 
     <p data-mc-conditions="QuicksilverOrClassic.Draft mode">(the note below is duplicated in this article: /Content/Resource Mgmt/Resource utilization/view-utilization-information.htm and in the glossary)</p>
    -->

예를 들어, 사용자 시간별 매출 유형을 사용하는 작업이 2시간 걸리도록 계획되어 있고 사용자에게 할당된 사용자가 시간당 $30인 경우, 작업의 계획 수익은 $60입니다. 작업이 완료되면 사용자가 작업을 완료하는 데 걸린 실제 시간으로 1.5시간만 기록하면 실제 매출액은 45달러입니다. 작업에 할당되지 않은 다른 사용자가 시간을 기록하는 경우 실제 매출은 해당 사용자의 청구 비율을 기반으로 계산됩니다.

다음과 같은 방법으로 매출을 기록할 수 있습니다.

* 작업의 수익 유형을 정의하고 작업 항목에 지정된 사용자 또는 역할을 청구 요율과 연관시킴으로써, 이는 작업 품목의 계획 또는 실제 시간 금액으로 수익을 계산합니다. 상한선을 시간별 요금에 대해 부과되는 최대 금액으로 설정할 수 있습니다.\
   작업의 매출 유형 지정에 대한 자세한 내용은 문서를 참조하십시오 [작업 편집](../../../manage-work/tasks/manage-tasks/edit-tasks.md).

* 작업 또는 프로젝트에 대한 고정 수익 비율을 청구하여\
   고정 수익 태스크가 있는 경우 고정 수익 금액이 태스크 또는 프로젝트의 계획 수익으로 추가되고, 태스크 계획 수익이 고정 수익으로 청구 레코드에 추가할 수 있습니다.
* 프로젝트에 대한 고정 청구 고정 수익 비율을 설정한 다음 프로젝트 내의 작업에 대한 시간별 비율을 설정합니다. Workfront은 작업에 대한 시간별 요금을 프로젝트 단가에 추가합니다.\
   예를 들어, Workfront을 사용하는 정비사는 프로젝트에 대한 고정 수익으로 부품 비용을 입력한 다음, 자동차를 고정하는 데 사용한 시간에 대해 시간별로 청구할 수 있습니다. 프로젝트 또는 작업에 대한 고정 수익은 완료 시 실현됩니다.

태스크를 &quot;청구 불능&quot;으로 표시할 수도 있습니다. 이 경우 태스크와 연관된 계획 또는 실제 수익이 없습니다.

## 작업 매출 유형 개요 {#overview-of-task-revenue-types}

기본적으로 모든 새 작업의 매출 유형은 Workfront 또는 그룹 관리자가 지정한 작업 및 문제 환경 설정에 따라 설정됩니다.\
Workfront 인스턴스에 대한 작업 및 문제 환경 설정 정의에 대한 자세한 내용은 문서를 참조하십시오 [시스템 전체 작업 및 문제 환경 설정 구성](../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-task-issue-preferences.md).

프로젝트 소유자는 프로젝트의 매출 유형 및 고정 수익을 수정할 수 있습니다.\
프로젝트의 고정 수익 지정에 대한 자세한 내용은 문서를 참조하십시오 [프로젝트 편집](../../../manage-work/projects/manage-projects/edit-projects.md).\
작업의 매출 유형 지정에 대한 자세한 내용은 문서를 참조하십시오 [작업 편집](../../../manage-work/tasks/manage-tasks/edit-tasks.md).

작업 또는 프로젝트에 다음 매출 유형을 적용할 수 있습니다.

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
   <td> <p>이 유형은 프로젝트 및 작업에 사용할 수 있습니다. </p> <p>템플릿을 프로젝트에 첨부할 때 템플릿의 고정 수익이 프로젝트의 고정 수익에 추가됩니다. 자세한 내용은 <a href="../../../manage-work/projects/create-and-manage-templates/attach-template-to-project-overview.md" class="MCXref xref">프로젝트에 템플릿 첨부 개요</a>. </p> <p>태스크의 경우 태스크 지정에 관계없이 항상 태스크에 지정된 고정 금액을 사용하여 태스크 수익이 계산됩니다. </p> <p>1차 하위 구성요소 작업의 고정 수익은 상위 작업의 수입, 그 다음 프로젝트의 수익으로 올림됩니다. 상위 태스크 및/또는 프로젝트에 고정 금액이 정의된 경우, 금액은 하위 태스크에서 롤업된 계획 매출에 추가됩니다.</p> <p>태스크에 대한 고정 수익 금액은 프로젝트의 청구 레코드에 포함될 수 있습니다.</p> </td> 
  </tr> 
  <tr> 
   <td> <p>시간별 사용자</p> </td> 
   <td> <p>이 유형은 작업에만 사용할 수 있습니다. </p> <p>특정 사용자에 대해 설정한 청구 비율에 해당 작업에 대한 계획 시간 수를 곱한 값이 태스크의 계획 수익 금액이 됩니다. 특정 사용자에 대해 설정한 청구 비율과 작업에 대해 사용자가 로그하는 시간 수를 곱한 값은 작업의 실제 수익 금액입니다. <br>예를 들어, 사용자를 만들고 [시간당 청구] 필드에 대해 $20를 설정한 경우, 사용자가 작업표에서 작업에 대해 5시간을 제출하면 작업의 실제 청구 금액은 $100입니다.</p> <p><b>팁</b>

작업을 만들 때 기본 매출 유형입니다.</p> </td>
</tr> 
  <tr> 
   <td> <p>시간별 역할</p> </td> 
   <td> <p>이 유형은 작업에만 사용할 수 있습니다.</p> <p>이 유형은 시간별 사용자 와 비슷하지만 사용자 비율보다는 작업 역할 비율을 사용합니다.</p> </td> 
  </tr> 
  <tr> 
   <td> <p>캡이 있는 시간별 사용자</p> </td> 
   <td> <p>이 유형은 작업에만 사용할 수 있습니다.</p> <p>작업은 시간별로 청구되지만 지정할 수 있는 최대 상한 금액이 있습니다. <br>예를 들어, 사용자의 청구 비율이 $25이지만 작업의 상한 금액이 $20이고 사용자가 1시간을 기록하면, 작업의 실제 매출은 $20입니다. </p> </td> 
  </tr> 
  <tr> 
   <td> <p>캡을 사용한 시간별 역할</p> </td> 
   <td> <p>이 유형은 작업에만 사용할 수 있습니다.</p> <p>이 유형은 Cap가 있는 사용자 시간별 과 유사하지만 사용자 비율보다는 작업 역할 비율을 사용합니다. </p> </td> 
  </tr> 
  <tr> 
   <td> <p>시간별 + 고정 사용자</p> </td> 
   <td> <p>이 유형은 작업에만 사용할 수 있습니다. </p> <p>작업은 시간별로 청구되지만 사용자 비율에 추가할 수 있는 고정 금액이 있습니다. 태스크에 지정된 고정 금액은 프로젝트에 대한 청구 레코드에 포함할 수 있습니다. 고정 금액에 작업 시간을 곱하지 않습니다. 사용자 청구율만 수행합니다. </p> </td> 
  </tr> 
  <tr> 
   <td> <p>시간별 + 고정 역할</p> </td> 
   <td> <p>이 유형은 작업에만 사용할 수 있습니다. </p> <p>작업은 시간별로 청구되지만 역할율에 추가할 수 있는 추가 고정 금액이 있습니다. 태스크에 지정된 고정 금액은 프로젝트에 대한 청구 레코드에 포함할 수 있습니다. 고정 금액에 작업 시간을 곱하지 않습니다. 작업 역할 청구 비율만 수행합니다. </p> </td> 
  </tr> 
  <tr> 
   <td> <p>고정 시간별</p> </td> 
   <td> <p>이 유형은 작업에만 사용할 수 있습니다.</p> <p>작업에 대해 설정한 상한 또는 고정 금액과 작업에 대해 입력한 시간 수(사용자 또는 해당 직무 역할과 관계없이)를 곱합니다.</p> </td> 
  </tr> 
  <tr> 
   <td> <p>청구 불가</p> </td> 
   <td> <p>이 유형은 작업에만 사용할 수 있습니다.</p> <p>이 매출 유형은 매출에 영향을 주지 않습니다. </p> <p>상위 객체에 이 설정이 있는 경우 청구 유형이 있는 하위 작업은 여전히 정상적으로 적용됩니다.</p> <p>재무 데이터에 액세스할 수 없는 사용자 또는 템플릿에 대한 재무 권한이 없는 사용자가 해당 템플릿에서 프로젝트를 생성하는 경우, 이는 프로젝트의 작업에 대한 기본 수익 유형입니다.</p> <p>재무 데이터 액세스에 대한 자세한 내용은 문서를 참조하십시오 <a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-financial.md" class="MCXref xref">재무 데이터에 대한 액세스 권한 부여</a>.<br>객체에 대한 재무 권한에 대한 자세한 내용은 문서를 참조하십시오 <a href="../../../workfront-basics/grant-and-request-access-to-objects/sharing-permissions-on-objects-overview.md" class="MCXref xref">개체에 대한 권한 공유 개요</a>.<br>템플릿에서 프로젝트 만들기에 대한 자세한 내용은 문서를 참조하십시오 <a href="../../../manage-work/projects/create-projects/create-project-from-template.md" class="MCXref xref">템플릿을 사용하여 프로젝트 만들기</a>. </p> </td> 
  </tr> 
 </tbody> 
</table>

## 상위 작업의 매출 개요

청구 정보가 있는 독립형 태스크를 상위로 변경하면, 신규 상위 태스크는 이전에 적용된 청구 정보와 함께 이전에 적용된 청구 정보를 그대로 유지합니다. 1차 하위 구성요소 작업에 기록된 시간에서 나오는 모든 청구 정보는 새 상위 태스크에 실제 수익으로 롤업됩니다.

1차 하위 구성요소 태스크에서 계획된 수익도 상위 태스크로 롤업됩니다.

## 문제에 대한 수입 개요

문제에는 계획됨 또는 실제 수익 금액이 없지만 실제 원가가 있을 수 있습니다.

문제에 대해 시간을 기록하고 &quot;매출로 계산&quot;으로 표시된 시간 유형을 사용하는 경우, Workfront은 해당 시간에 로그인하는 사용자의 비율에 따라 실제 비용 금액을 계산합니다. 이 숫자는 프로젝트의 실제 원가에 추가됩니다. 시간은 청구 레코드에도 포함될 수 있습니다.

비용 추적에 대한 자세한 내용은 문서를 참조하십시오 [비용 추적](../../../manage-work/projects/project-finances/track-costs.md).

시간 유형에 대한 자세한 내용은 문서를 참조하십시오 [시간 유형 관리](../../../administration-and-setup/set-up-workfront/configure-timesheets-schedules/hour-types.md).

## 매출 계산

* [사용자 및 역할 할당을 기반으로 작업에 대한 매출 계산](#revenue-calculations-for-tasks-based-on-user-and-role-assignments)

### 사용자 및 역할 할당을 기반으로 작업에 대한 매출 계산 {#revenue-calculations-for-tasks-based-on-user-and-role-assignments}

작업에 대한 수익을 계산할 때 다음 사항을 고려하십시오.

* 사용자 또는 작업 역할이 $0.00를 표시하는 경우 Workfront은 이를 유효한 금액으로 읽으며 이 금액에 작업의 시간 수에 곱하여 수입을 계산합니다. 작업에 대한 수익을 표시하지 않으려면 사용자 또는 작업 역할에 대한 청구 비율 필드가 비어 있는지 확인하십시오.
* 작업 역할 청구 비율이 적용되면, Workfront은 프로젝트에 대체 비율이 있을 때마다 시스템 수준에서 정의된 해당 역할에 대한 청구 비율 대신 프로젝트 수준에서 대체 비율을 사용합니다.
* 작업에 대해 여러 직원이 있는 경우 아래 요약된 시나리오는 각 할당자에 대해 적용됩니다.

태스크 지정에 따라 수익 계산에 사용되는 비율이 계층입니다.

Workfront 관리자가 **작업 역할을 시간 항목에 수동으로 할당** 작업표 및 시간 기본 설정 영역에서 설정하고, 프로젝트에 대한 사용자 로깅 시간이 이 시간과 연결할 다른 역할을 선택하면 작업 또는 프로젝트의 실제 수익이 항상 시간 항목과 연관된 역할을 기준으로 계산됩니다. 특정 작업 역할에 대한 로깅 시간을 활성화하는 방법에 대한 내용은 문서를 참조하십시오 [작업표 및 시간 기본 설정](../../../administration-and-setup/set-up-workfront/configure-timesheets-schedules/timesheet-and-hour-preferences.md).

수익 유형 및 태스크 지정 특성을 기반으로 태스크 수익을 계산할 때 다음 시나리오가 있습니다.

* **작업의 매출 유형은 시간별 사용자입니다**

   <table style="table-layout:auto"> 
   <col> 
   <col> 
   <col> 
   <col> 
   <tbody> 
    <tr> 
     <td role="rowheader">시간당 요금 청구</td> 
     <td>할당 없음</td> 
     <td>사용자 할당</td> 
     <td>작업 역할 할당</td> 
    </tr> 
    <tr> 
     <td role="rowheader">계획 매출에 대한 시간당 청구 비율</td> 
     <td>$0.00</td> 
     <td> 사용자가 프로파일에 청구 비율이 있는 경우 해당 비율을 사용하여 계획 수익을 계산합니다. 그렇지 않으면 기본 직무 역할의 시스템 청구 비율이 사용됩니다. <br><p><b>참고</b>  사용자는 보조 작업 역할 중 하나를 사용하여 작업에 할당할 수 있지만 기본 작업 역할의 비율은 여기에서 대신 사용됩니다.</p></td> 
     <td>작업에 지정된 작업 역할의 시스템 청구 비율은 계획 수익을 계산하는 데 사용됩니다. </td> 
    </tr> 
    <tr> 
     <td role="rowheader">실제 매출에 대한 시간당 청구 비율</td> 
     <td>시간을 기록하는 사용자가 프로필에 청구 비율이 있는 경우 해당 비율이 사용됩니다. <br>그렇지 않으면 기본 Job 역할의 청구 비율이 사용됩니다. 사용자 또는 사용자의 기본 역할과 연관된 청구 비율이 없는 경우 실제 매출액은 $0.00입니다. <br><p><b>메모</b>

   다른 사용자가 작업에 할당되더라도 시간 기록 사용자와 관련된 비율만 계산에 고려됩니다.</p></td>
   <td>시간을 기록하는 사용자가 프로필에 청구 비율이 있는 경우 해당 비율이 사용됩니다. <br>그렇지 않으면 기본 Job 역할의 청구 비율이 사용됩니다. 사용자 또는 사용자의 기본 역할과 연관된 청구 비율이 없는 경우 실제 매출액은 $0.00입니다. <br><p><b>메모</b>

   다른 사용자가 작업에 할당되더라도 시간 기록 사용자와 관련된 비율만 계산에 고려됩니다.</p></td>
   <td>시간을 기록하는 사용자가 프로필에 청구 비율이 있는 경우 해당 비율이 사용됩니다. 그렇지 않으면 기본 Job 역할의 청구 비율이 사용됩니다.<br><p><b>메모</b>

   사용자 로깅 시간에 연관된 청구 비율이 없고 Job 역할이나 Job 역할에 대한 청구 비율이 없는 경우 해당 작업과 연관된 Job 역할의 비율이 사용됩니다. 이 역할에 대한 청구 비율이 없는 경우 수입은 $0.00입니다</p></td>
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
     <td role="rowheader">시간당 요금 청구</td> 
     <td>할당 없음</td> 
     <td>사용자 할당</td> 
     <td>작업 역할 할당</td> 
    </tr> 
    <tr> 
     <td role="rowheader">계획 매출에 대한 시간당 청구 비율</td> 
     <td>$0.00</td> 
     <td>Workfront은 사용자가 작업에서 충족한 작업 역할을 보고 계획된 수입을 계산합니다. <br>사용자가 작업의 역할과 연관되지 않은 경우 수입은 $0.00입니다. </td> 
     <td>태스크에 지정된 작업 역할의 청구 비율은 계획 수익을 계산하는 데 사용됩니다.</td> 
    </tr> 
    <tr> 
     <td role="rowheader">실제 매출에 대한 시간당 청구 비율</td> 
     <td>Workfront에서는 시간을 기록하는 사용자의 기본 작업 역할의 청구 비율을 사용합니다. <br>시간을 기록하는 사용자에게 연관된 작업 역할이 없거나 기본 작업 역할에 청구 비율이 없는 경우 실제 수익은 $0.00입니다. </td> 
     <td> 시간을 기록하는 사용자가 작업에 할당되면 작업의 사용자와 연관된 작업 역할의 청구 비율이 실제 수익을 계산하는 데 사용됩니다. 그렇지 않으면 기본 Job 역할의 청구 비율이 사용됩니다. 사용자에게 기본 Job 역할이 없거나 기본 Job 역할에 청구 비율이 없는 경우 실제 수익은 $0.00입니다. </td> 
     <td>시간을 기록하는 사용자의 작업 역할 중 하나가 작업에 할당되면 해당 작업 역할 비율이 사용됩니다. 작업에 지정된 작업 역할이 시간을 기록하는 사용자와 연관되지 않으면 사용자의 기본 역할의 청구 비율이 실제 수익을 계산하는 데 사용됩니다. 사용자에게 작업 역할이 없거나 기본 작업 역할과 연관된 비율이 없는 경우 작업에 할당된 작업 역할의 비율이 사용됩니다. </td> 
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

### 프로젝트에 대한 매출 계산

프로젝트에 대해 다음 매출 유형을 추적할 수 있습니다.

* 프로젝트에 대한 계획 수익은 다음 공식으로 계산됩니다.

   ```
   Project Planned Revenue = SUM(Task Planned Revenue)+ Fixed Revenue
   ```

   태스크 계획 수익 계산 방법에 대한 자세한 내용은 [사용자 및 역할 할당을 기반으로 작업에 대한 매출 계산](#revenue-calculations-for-tasks-based-on-user-and-role-assignments) 섹션에 자세히 설명되어 있습니다.

* 프로젝트에 대한 실제 수익은 다음 공식으로 계산됩니다.

   ```
   Project Actual Revenue = SUM (Task Actual Revenue) + (Hours logged for the project x User Billing per Hour Rate) + SUM (Hours logged for the issues x User Billing per Hour rate)
   ```

태스크 실제 수익 계산 방법에 대한 자세한 내용은 [사용자 및 역할 할당을 기반으로 작업에 대한 매출 계산](#revenue-calculations-for-tasks-based-on-user-and-role-assignments) 섹션에 자세히 설명되어 있습니다.

프로젝트에 직접 로그인한 시간 또는 문제와 연결된 실제 매출에 대해, Workfront에서는 프로젝트에서 시간을 기록하는 사용자의 청구 비율을 사용합니다. 사용자에게 프로필과 연관된 청구 비율이 없는 경우 Workfront은 기본 Job 역할의 청구 비율을 사용합니다. 두 비율이 모두 0이면 프로젝트에서 로그온한 시간 또는 문제와 연관된 실제 매출이 0입니다.
