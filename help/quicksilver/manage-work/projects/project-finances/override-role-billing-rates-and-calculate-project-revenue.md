---
product-area: projects
navigation-topic: financials
title: 작업 역할 청구 요금 재정의 및 프로젝트의 수익 계산에 대한 개요
description: 프로젝트에 소요된 시간에 청구 요금을 곱하면 프로젝트의 수익을 계산하는 데 청구 요금을 사용할 수 있습니다. 청구 요금 및 수익에 대한 자세한 내용은 청구 및 수익 개요 문서를 참조하십시오.
author: Alina, Lisa
feature: Work Management
exl-id: 63ba6758-ba62-48b4-89f4-d784e32a1bfa
source-git-commit: 1517e3e28fe536a8a72d2802919c8b8819e9ea1a
workflow-type: tm+mt
source-wordcount: '3852'
ht-degree: 0%

---

# 작업 역할 청구 요금 재정의 및 프로젝트의 수익 계산에 대한 개요

{{highlighted-preview}}

프로젝트에 소요된 시간에 청구 요금을 곱하면 프로젝트의 수익을 계산하는 데 청구 요금을 사용할 수 있습니다. 청구 요금 및 매출에 대한 자세한 내용은 문서 를 참조하십시오 [청구 및 수익 개요](../../../manage-work/projects/project-finances/billing-and-revenue-overview.md).

<!--
<div data-mc-conditions="QuicksilverOrClassic.Draft mode">
<p>(NOTE: drafted because the only procedure here was moved to a different article.&nbsp;This stays as an overview)</p>
<h2>Access requirements</h2>
<p>You must have the following access to perform the steps in this article:</p>
<table style="table-layout:auto">
<col>
<col>
<tbody>
<tr>
<td role="rowheader">Adobe Workfront plan*</td>
<td> <p>Any</p> </td>
</tr>
<tr>
<td role="rowheader">Adobe Workfront license*</td>
<td> <p>Plan </p> </td>
</tr>
<tr>
<td role="rowheader">Access level configurations*</td>
<td> <p>Edit access to Projects and Financial&nbsp;Data</p> <note type="note">
If you still don't have access, ask your Workfront administrator if they set additional restrictions in your access level. For information on how a Workfront administrator can modify your access level, see
<a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Create or modify custom access levels</a>.
</note> </td>
</tr>
<tr>
<td role="rowheader">Object permissions</td>
<td> <p>Manage permissions to the project with permissions to Manage Finance</p> <p>For information on requesting additional access, see <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Request access to objects </a>.</p> </td>
</tr>
</tbody>
</table>
<p>*To find out what plan, license type, or access you have, contact your Workfront administrator.</p>
</div>
-->

## 작업 역할 청구 요금 및 역할 시간당 수익 유형 개요

Adobe Workfront 관리자는 청구 요금을 사용자 및 작업 역할에 모두 연결할 수 있습니다.\
사용자를 만들고 청구 요금과 연결하는 방법에 대한 자세한 내용은 문서를 참조하십시오 [사용자 추가](../../../administration-and-setup/add-users/create-and-manage-users/add-users.md). 작업 역할을 생성하고 청구 요금과 연관시키는 방법에 대한 자세한 내용은 문서를 참조하십시오 [작업 역할 만들기 및 관리](../../../administration-and-setup/set-up-workfront/organizational-setup/create-manage-job-roles.md).

사용자와 연결된 청구 요금은 재정의할 수 없습니다.

작업 역할과 연결된 청구 요금은 회사 또는 프로젝트 수준에서 재정의할 수 있습니다.

작업 역할의 청구 요율을 기반으로 프로젝트의 수익을 계산하려면 다음을 수행합니다. **수익 유형** 프로젝트의 작업 중 하나는 다음 중 하나여야 합니다.

* 시간별 역할
* 시간별 역할(수용작업량 포함)
* 시간별 + 고정 역할

에 대한 자세한 내용 **수익 유형** 및 청구 요금, 참조: [청구 및 수익 개요](../../../manage-work/projects/project-finances/billing-and-revenue-overview.md).

## 수익 계산 시 청구 요금 대체 계층

작업 역할에는 다음과 같은 방법으로 청구 요금이 연결될 수 있습니다.

* Workfront 관리자는 작업 역할을 생성할 때 해당 작업 역할과 연관된 시스템 수준 청구 요금을 정의할 수 있습니다.\
  작업 역할 생성에 대한 자세한 내용은 [작업 역할 만들기 및 관리](../../../administration-and-setup/set-up-workfront/organizational-setup/create-manage-job-roles.md).

* Workfront 관리자는 회사를 만들 때 동일한 작업 역할에 대한 회사 수준 청구 요금을 정의할 수 있습니다.\
  Workfront이 이 회사와 연결된 프로젝트의 수익을 계산할 때 이 작업 역할에 대한 시스템 수준 청구 요금 대신 작업이 할당되면 회사 청구 요금이 사용됩니다.\
  회사 수준에서 변경된 작업 역할 비율은 해당 회사와 관련된 모든 프로젝트에 영향을 줍니다.

  >[!NOTE]
  >
  >회사 청구 요금을 업데이트해야 하는 경우 프로젝트의 요금이 자동으로 업데이트되지 않습니다. 새 회사 요율이 프로젝트에 적용되기 전에 프로젝트에서 회사를 제거하고 회사에 대한 요율을 업데이트한 다음 회사를 프로젝트에 다시 첨부해야 합니다. 프로젝트에 회사를 첨부하는 방법에 대한 지침은 [프로젝트 편집](../../../manage-work/projects/manage-projects/edit-projects.md).

  회사별 작업 역할 청구 요금 생성에 대한 자세한 내용은 다음을 참조하십시오. [회사 만들기 및 편집](../../../administration-and-setup/set-up-workfront/organizational-setup/create-and-edit-companies.md).

* Workfront 관리자는 사용자가 프로젝트 재무 정보를 수동으로 다시 계산할 때 프로젝트를 편집할 때 회사 수준의 청구 요금에 변경 사항을 프로젝트에 적용하도록 옵션을 활성화할 수 있습니다.\
  자세한 내용은 [프로젝트 수준 청구 요율을 회사 수준 청구 요율로 재정의](../../../manage-work/projects/project-finances/override-project-level-with-company-level-billing-rates.md).

<div class="preview">

* Workfront 관리자는 위치 및 날짜에 따라 역할당 여러 청구 요금이 있는 요금 카드를 정의할 수 있습니다. 요금 카드가 프로젝트에 첨부된 경우 모든 역할(위치가 사용되는 경우 위치별)과 관련 청구 요금이 프로젝트의 청구 요금 섹션에 추가됩니다. 요금 카드를 첨부하면 프로젝트의 기존 청구 요금이 무시됩니다.

  자세한 내용은 [등급 카드 관리](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/manage-rate-cards.md) 및 [프로젝트에 요금 카드 첨부](/help/quicksilver/manage-work/projects/project-finances/attach-rate-card-to-project.md).

</div>

* 프로젝트 관리자는 프로젝트 수준에서 동일한 작업 역할에 대한 청구 요금을 정의할 수 있습니다.\
  프로젝트에서 변경된 작업 역할 비율은 해당 프로젝트에만 영향을 줍니다.

  프로젝트의 역할 비율 재정의에 대한 자세한 내용은 [프로젝트 수준에서 작업 역할 청구 요금 재정의](../../../manage-work/projects/project-finances/override-job-role-billing-rates-at-the-project-level.md).

>[!IMPORTANT]
>
>작업 역할이 시스템 수준, 회사 수준 및 프로젝트 수준의 청구 요금과 연결된 경우 Workfront은 작업 역할 요금을 사용할 때 프로젝트 수준의 작업 역할의 청구 요율을 사용하여 작업의 매출을 계산합니다. 모든 작업의 수익이 프로젝트 수익으로 적상됩니다.

## 프로젝트 수준에서 작업 역할 청구 요금 재정의

프로젝트 관리자는 특정 프로젝트의 작업 역할에 대한 청구 요금을 지정할 수 있습니다. 이 프로젝트 수준의 청구 요율은 이 작업 역할에 대한 시스템 수준의 청구 요율을 무시합니다. Workfront은 시스템 수준 청구 요금을 사용하는 대신 작업 역할의 프로젝트 수준 청구 요금을 사용하여 수익을 계산합니다.

<span class="preview">프로젝트에 요금 카드를 첨부할 수도 있습니다. 이 경우 요금 카드에서 프로젝트로 작업 역할 청구 요금을 가져옵니다.</span>

프로젝트 수준에서 작업 역할 청구 요율을 재정의하는 방법에 대한 자세한 내용은 다음을 참조하십시오. [프로젝트 수준에서 작업 역할 청구 요금 재정의](../../../manage-work/projects/project-finances/override-job-role-billing-rates-at-the-project-level.md).

프로젝트의 수익을 계산하는 데 사용되는 작업 역할에 대한 자세한 내용은 의 &quot;사용자 및 역할 할당에 따른 작업에 대한 수익 계산&quot; 섹션을 참조하십시오. [청구 및 수익 개요](../../../manage-work/projects/project-finances/billing-and-revenue-overview.md). <span class="preview">프로젝트에 비율 카드를 첨부하는 방법에 대한 자세한 내용은 [프로젝트에 요금 카드 첨부](/help/quicksilver/manage-work/projects/project-finances/attach-rate-card-to-project.md).</span>

>[!NOTE]
>
>실제 매출의 경우, 청구됨으로 표시된 청구 기록에 추가된 시간에 적용되는 청구 요금은 청구 기록이 청구된 후에 발생하는 청구 요금 무시의 영향을 받지 않아야 합니다.

<!--
<div data-mc-conditions="QuicksilverOrClassic.Draft mode">
<p>(NOTE: drafted and linked above to the stand-alone article for overriding billing rates on projects.)</p>
<p>You can override the billing rate of a job role on a project in the following ways:</p>
<ul>
<li>One time, by selecting a new rate for the job role.<br>The new rate is used for the entire duration of the project, to calculate revenue. </li>
</ul>
<ul>
<li>Several times, by selecting several new rates for specific date ranges. <br>A different rate can be used during each specified date range.</li>
</ul>
<p>To override a billing rate for a project:</p>
<ol>
<li value="1">Go to the project you want to override billing rates for.</li>
<li value="2"> <p data-mc-conditions="QuicksilverOrClassic.Quicksilver">Click <strong>Billing Rates</strong> in the left panel. You might have to first click <strong>Show More</strong>. </p> </li>
<li value="3"> <p>Click <strong>Add Billing Rate</strong> > <strong>New Billing Rate</strong>.</p> <p>The New Billing Rate box opens</p> <p> <img src="assets/override-billing-rate-on-project-nwe-350x310.png" style="width: 350;height: 310;"> </p> <p> <br>The <strong>Default Billing Rate</strong> field displays the system-level rate for this job role.</p> </li>
<li value="4">In the <strong>Job Role</strong> field, select the job role you want to change the billing rate for.<br></li>
<li value="5">In the <strong>Billing Rates 1</strong> field, enter the one time billing rate override, then click <strong>Save</strong> to override the billing rate one time, <br>Or Click <strong>Add Rate</strong> to add more billing rate overrides.</li>
<li value="6">(Conditional) If you are adding more than one billing rate override, specify the following information:<br>- <strong>Billing Rates 1</strong>: the value of the Billing Rate from the beginning of the project to the first date of the first override. This is typically the same amount as the <strong>Default Rate</strong>.<br>- <strong>Start Date</strong>: this is the date when the Default Rate ends.<br>- <strong>End Date</strong>: the date when the new billing rate override ends. <br>Workfront applies the override job role rate to the hours that occur during the time frames specified when calculating revenue on the project.<br>There should be no gaps between the time frames of two override rates. The <strong>Start Date</strong> of an override rate should be the day immediately following the <strong>End Date</strong> of the previous override date.<br><note type="note">
You cannot specify a
<strong>Start Date</strong> for the first override rate, nor an
<strong>End Date</strong> for the last override rate. We recommend that you use the Default Rate for the first override rate.
<br>Workfront assumes that the first override rate is applied for all hours with a date older than the
<strong>End Date</strong> of the first override, and that the last override rate is applied for all hours with a date newer than the
<strong>Start Date</strong> of the last override.
<br>If an hour is logged before the Planned Start Date of the project the very first billing rate is used.
<br>If an hour is logged after the Planned Completion Date of the project the very last billing rate is used.
</note><br></li>
<li value="7">Click <strong>Save</strong>.</li>
</ol>
</div>
-->

## 프로젝트의 청구 요금 섹션 개요

프로젝트와 연계된 작업 역할에 대한 대체 청구 요율을 지정한 후에는에서 모든 작업 역할과 해당 재정의를 볼 수 있습니다. **청구 요금** 프로젝트의 탭.

목록에 다음 정보가 표시됩니다. **청구 요금**:

* [작업 역할 그룹화](#job-role-grouping)
* [프로젝트 청구 요금 값](#project-billing-rate-value)
* [기본 청구 요금 값](#default-billing-rate-value)
* [회사 청구 요금 값](#company-billing-rate-value)
* [여러 청구 요금 값 및 일정](#multiple-billing-rate-values-and-timeframes)

### 작업 역할 그룹화 {#job-role-grouping}

청구 요금은 다음에 그룹화되어 있습니다. **청구 요금** 영역별로 지정합니다. <span class="preview">비율 카드가 프로젝트에 첨부된 경우 작업 역할도 비율 카드로 그룹화됩니다. 위치가 작업 역할에 적용되는 경우 위치 이름이 작업 역할 이름의 일부로 포함됩니다. 여러 위치에 대해 동일한 작업 역할이 나열될 수 있습니다.</span>

### 프로젝트 청구 요금 값 {#project-billing-rate-value}

작업 역할에 해당하는 그룹화 줄에서 의 프로젝트 수준에서 해당 작업 역할에 대한 청구 요금을 확인합니다. **프로젝트 청구 요금** 열. 작업 역할에 복수 대체 비율이 있는 경우 현재 날짜에 해당하는 대체 비율이 **프로젝트 청구 요금** 열.

### 기본 청구 요금 값 {#default-billing-rate-value}

작업 역할의 그룹화 줄에서 의 시스템 수준에서 해당 작업 역할에 대한 청구 요금을 확인합니다. **기본 청구 요금** 열.

>[!NOTE]
>
>작업 역할에 대한 프로젝트 청구 요금이 있는 경우 **기본 청구 요금** 은 프로젝트의 수익 계산에 적용되지 않습니다. 만 **프로젝트 청구 요금** 매출 계산에 적용됩니다.

### 회사 청구 요금 값 {#company-billing-rate-value}

작업 역할의 그룹화 줄에서 의 회사 수준에서 해당 작업 역할에 대한 청구 요금을 확인합니다. **회사 청구 요금** 열. 즉, 이 프로젝트와 연계된 회사가 있으며 이 작업 역할에는 해당 회사의 청구 요금이 다릅니다. 프로젝트 요금과 동일한 경우에도 회사의 청구 요금이 표시됩니다.

>[!NOTE]
>
><span class="preview">요금 카드가 프로젝트에 첨부된 경우 **회사 청구 요금** 청구 요금에 가져오지 않습니다. 이 계산은 작업 역할에 대한 비율 카드 비율 또는 회사 비율을 기반으로 합니다.</span>
>
>작업 역할에 대한 프로젝트 청구 요금이 있는 경우 **회사 청구 요금** 은 프로젝트의 매출 계산에 적용되지 않습니다. 만 **프로젝트 청구 요금** 매출 계산에 적용됩니다.

### 여러 청구 요금 값 및 일정 {#multiple-billing-rate-values-and-timeframes}

특정 작업 역할에 대해 여러 대체 청구 요금이 있는 경우 해당 작업 역할에 대한 그룹화 아래에 나열됩니다. 인라인 편집을 사용하여 재정의 비율과 **시작** **날짜** 및 **종료일** 이 탭의 청구 요금 재정의.

>[!NOTE]
>
>다음을 지정할 수 없습니다. **시작일** 첫 번째 재정의 비율의 경우 **종료일** 마지막 재정의 비율입니다. Workfront에서는 날짜가 다음보다 오래된 모든 시간에 대해 첫 번째 재정의 비율이 적용된다고 가정합니다. **종료일** 을 반환합니다. 마지막 재정의 비율은 다음 날짜 이후의 모든 시간에 적용됩니다. **시작일** 마지막 재정의\
>프로젝트의 계획된 시작 일자 전에 시간이 기록되는 경우 첫 번째 청구 요금이 사용됩니다.\
>프로젝트의 계획된 완료 일자 이후 시간이 기록된 경우 마지막 청구 요금이 사용됩니다.

## 계획된 수익 계산

* [일회성 청구 요금 재정의를 기반으로 계획된 수익 계산](#calculate-planned-revenue-based-on-a-one-time-billing-rate-override)
* [여러 청구 요금 재정의를 기반으로 계획된 수익 계산](#calculate-planned-revenue-based-on-multiple-billing-rate-overrides)
* [작업 기간 전체에 대한 계획된 시간 분포](#distribution-of-planned-hours-across-the-duration-of-a-task)

### 일회성 청구 요금 재정의를 기반으로 계획된 수익 계산 {#calculate-planned-revenue-based-on-a-one-time-billing-rate-override}

일회성 청구 요금 재정의를 기반으로 계획된 수익을 계산할 때 다음 사항을 고려하십시오.

* 다음의 경우 **수익 유형** 작업: **시간별 역할**, Workfront은 작업의 계획된 시간과 작업과 연결된 작업 역할의 청구 요금을 곱하여 작업의 계획된 수익을 계산합니다.

* 작업 역할의 청구 요금이 프로젝트 수준에서 재정의된 경우 Workfront은 프로젝트의 재정의 요금을 사용하여 계획 수익을 계산합니다.
* 작업에 할당이 여러 개 있는 경우 계획된 수익은 각 할당의 작업 역할과 해당 계획된 시간 할당에 대한 청구 요율을 곱하여 계산됩니다.

>[!NOTE]
>
>할당당 계획된 시간은 여러 할당의 경우 작업에 대한 계획된 시간과 다릅니다.

계획된 수익을 계산하는 데 사용되는 작업 역할에 대한 자세한 내용은 문서의 &quot;사용자 및 역할 할당에 따른 작업에 대한 수익 계산 이해&quot; 섹션을 참조하십시오 [청구 및 수익 개요](../../../manage-work/projects/project-finances/billing-and-revenue-overview.md).

### 여러 청구 요금 재정의를 기반으로 계획된 수익 계산 {#calculate-planned-revenue-based-on-multiple-billing-rate-overrides}

여러 청구 요금 재정의를 기반으로 계획된 수익을 계산할 때 다음 사항을 고려하십시오.

* 다음의 경우 **수익 유형** 작업: **시간별 역할**, Workfront은 작업의 계획된 시간과 작업과 연결된 작업 역할의 청구 요금을 곱하여 작업의 계획된 수익을 계산합니다.

  계획된 수익을 계산하는 데 사용되는 작업 역할에 대한 자세한 내용은 문서의 &quot;사용자 및 역할 할당에 따른 작업에 대한 수익 계산 이해&quot; 섹션을 참조하십시오 [청구 및 수익 개요](../../../manage-work/projects/project-finances/billing-and-revenue-overview.md).

* 여러 청구 요율 무시의 경우 작업 기간 동안 계획된 시간을 곱한 요율이 변경됩니다. 기본적으로 Workfront은 작업 기간 동안 계획된 시간을 균등하게 분배하여 작업의 각 날에 동일한 시간을 할당합니다. 계산할 때 **계획된 수익** 작업의 경우 Workfront은 일별 계획된 시간과 해당 날짜의 청구 요금을 곱합니다. 여러 청구 요금의 경우 매일 요금이 다를 수 있습니다.

  예를 들어 시간별 역할이 있는 작업이 있는 경우 **수익 유형**. 작업의 기간은 5일이며 계획된 시간 값은 40시간입니다. 일별 계획된 시간은 8시간입니다. 프로젝트 관리자 작업 역할을 작업에 할당하고 작업의 마지막 3일에 대해 이 작업 역할의 청구 요금을 재정의하면 이 작업 역할에 대해 처음 2일까지는 요율 1 청구 요율이 적용되고 나머지 3일까지는 요율 2 청구 요율이 적용됩니다.

  를 계산하는 공식 **계획된 수익** 이 작업 중:

  ```
  Planned Revenue = (Rate 1) * (Planned Hours for Day 1) + (Rate 1) * (Planned hours for Day 2) + (Rate 2) * (Planned hours for Day 3) + (Rate 2) * (Planned hours for Day 4) + (Rate 2) * (Planned hours for Day 5)
  ```

Workfront에서 일별 계획된 시간 금액을 찾는 방법에 대한 자세한 내용은 섹션 을 참조하십시오. [작업 기간 전체에 대한 계획된 시간 분포](#distribution-of-planned-hours-across-the-duration-of-a-task) 이 문서에서.

>[!NOTE]
>
>작업에 여러 명의 할당자가 있는 경우 계획된 시간의 양은 먼저 각 할당자에게 분배된 다음 작업 기간 동안 각 날짜로 분배됩니다. 이 경우, 계획된 수익은 각 피할당자에 대한 일일 시간 및 여러 청구 요금의 경우 작업 기간 동안 변경될 수 있는 각 작업 역할의 청구 요율을 고려하여 계산됩니다.

### 작업 기간 전체에 대한 계획된 시간 분포 {#distribution-of-planned-hours-across-the-duration-of-a-task}

작업 기간 동안 계획된 시간의 분포를 이해할 때는 다음 사항을 고려하십시오.

* 기본적으로 Workfront은 작업 기간 동안 계획된 시간을 균등하게 분배하며 프로젝트 일정의 가용성에 따라 작업의 각 날에 대해 동일한 수의 계획된 시간을 할당합니다.

  작업 기간 동안 계획된 시간의 분포를 이해하는 방법에 대한 자세한 내용은 문서의 &quot;작업 기간 동안 계획된 시간의 분포 이해&quot; 섹션을 참조하십시오 [계획된 시간 개요](../../../manage-work/tasks/task-information/planned-hours.md).

  >[!NOTE]
  >
  >일별 계획된 시간은 작업 기간 동안 각 날의 계획된 시간을 할당한 것입니다. 작업에 할당이 한 개 있는 경우 이 숫자는 할당당 하루 계획된 시간도 나타냅니다. 작업에 여러 개의 할당이 있는 경우 할당당 일별 계획된 시간이 작업에 대한 일별 계획된 시간과 다릅니다. 할당당 일별 계획된 시간 (일 기준), 여러 할당이 있는 작업에 대해서는 Workfront에 시각적으로 표시되지 않습니다.
  >
  >
  >일별 계획된 시간과 해당 일자의 작업에 할당된 작업 역할에 대한 청구 요금을 곱하여 해당 작업의 일별 계획된 수익을 계산합니다. 이 방법으로 계산된 모든 일일 계획 수익의 합은 해당 작업의 계획 수익과 같습니다.

## 실제 수익 계산

* [일회성 청구 요금 재정의를 기반으로 실제 수익 계산](#calculate-actual-revenue-based-on-a-one-time-billing-rate-override)
* [여러 청구 요금 재정의를 기반으로 실제 수익 계산](#calculate-actual-revenue-based-on-multiple-billing-rate-overrides)

### 일회성 청구 요금 재정의를 기반으로 실제 수익 계산 {#calculate-actual-revenue-based-on-a-one-time-billing-rate-override}

일회성 청구 요금 재정의를 기준으로 실제 수익을 계산할 때 다음 사항을 고려하십시오.

* 다음의 경우 **수익 유형** 작업: **시간별 역할**, Workfront은 **실제 근로시간** 계산할 작업에 연결된 작업 역할의 청구 요율별 작업 **실제 수익** 작업. 실제 시간은 작업에 직접 기록된 시간입니다.

  계산에 사용되는 작업 역할에 대한 자세한 정보 **실제 수익**&#x200B;이 문서에서 설명하는 &quot;사용자 및 역할 할당에 따른 작업에 대한 수익 계산 이해&quot; 섹션을 참조하십시오 [청구 및 수익 개요](../../../manage-work/projects/project-finances/billing-and-revenue-overview.md).

* 작업 역할의 청구 요금이 프로젝트 수준에서 재정의된 경우 Workfront은 프로젝트의 재정의 요금을 사용하여 실제 수익을 계산합니다. 프로젝트에서 작업 역할의 청구 요금을 재정의하는 경우 **실제 수익** 의 프로젝트가 새로 조정된 비율을 사용하여 자동으로 다시 계산됩니다.

  프로젝트의 역할 비율 재정의에 대한 자세한 내용은 [프로젝트 수준에서 작업 역할 청구 요금 재정의](../../../manage-work/projects/project-finances/override-job-role-billing-rates-at-the-project-level.md).

>[!NOTE]
>
>원래 요율로 청구된 원래 청구 요율을 재정의하기 전에 프로젝트에 이미 로그온한 시간을 유지하려면 해당 시간을 **청구 기록**, 그리고 다음을 표시해야 합니다. **청구 기록** 다음으로: **청구됨**. 그렇지 않으면 **실제 수익** 프로젝트에 대한 청구 요금이 재정의되기 전에 기록된 시간부터 프로젝트의 재정이 다시 계산되면 새 요금을 사용하여 다시 계산됩니다.\
>청구 기록에 시간을 포함하고 다음으로 표시하는 방법에 대한 자세한 정보 **청구됨**, 문서 참조 [청구 기록 만들기](../../../manage-work/projects/project-finances/create-billing-records.md).

### 여러 청구 요금 재정의를 기반으로 실제 수익 계산 {#calculate-actual-revenue-based-on-multiple-billing-rate-overrides}

여러 청구 요금 재정의를 기준으로 실제 수익을 계산할 때는 다음 사항을 고려하십시오.

* 다음의 경우 **수익 유형** 작업: **시간별 역할**, Workfront은 **실제 근로시간** 계산할 작업에 할당된 작업 역할의 청구 요금이 있는 작업 **실제 수익** 작업. 실제 시간은 작업에 직접 기록된 시간입니다.

* 여러 청구 요금이 무시되는 경우 **실제 근로시간** 곱하기 로 계산합니다. **실제 수익** 는 작업 기간 동안 변경될 수 있습니다. Workfront은 시간대가 과(와) 일치하는 작업 역할의 청구 요금을 사용합니다. **입력 일자** 계산할 작업에 기록된 시간 중 **실제 수익.**

  예를 들어 작업에는 **수익 유형** / **시간별 역할** 및 이 프로젝트 관리자의 작업 역할에 할당됩니다. 6월 19일부터 6월 25일 사이의 날짜에 대한 요금 1로 이 작업 역할의 청구 요금을 재정의합니다. 6월 26일부터 청구 요금을 요금 2로 재정의합니다. 6월 20일은 2시간, 6월 28일은 3시간을 기록하십시오.

  Workfront이 다음을 계산합니다. **실제 수익** 다음 공식을 사용하는 이 작업에 대해:

  ```
  Actual Revenue = 2 * Rate 1 + 3 * Rate 2
  ```

  계산에 사용되는 작업 역할에 대한 자세한 정보 **실제 수익**&#x200B;이 문서에서 설명하는 &quot;사용자 및 역할 할당에 따른 작업에 대한 수익 계산 이해&quot; 섹션을 참조하십시오 [청구 및 수익 개요](../../../manage-work/projects/project-finances/billing-and-revenue-overview.md).

## 여러 청구 요율을 기반으로 수익을 계산할 때 시간대가 미치는 영향

표준 시간대 차이가 Workfront의 다른 엔티티와 발생하는 경우 다른 사용자와 다른 사용자가 하루 계획된 시간을 다르게 볼 수 있습니다. 다음 시나리오는 다른 사용자에게 표시되는 내용에서 사용자에 대한 일별 계획된 시간 정보를 왜곡할 수 있습니다.

* 두 사용자는 서로 다른 두 시간대에 맞게 컴퓨터를 설정할 수 있습니다
* Workfront의 두 사용자 프로필은 서로 다른 두 시간대로 설정될 수 있습니다
* 사용자 프로필과 연결된 시간대는 Workfront의 시스템 시간대와 다를 수 있습니다
* 사용자 프로필과 연결된 시간대는 프로젝트 일정의 시간대와 다를 수 있습니다.

이러한 경우 시간대에 대해 동일한 설정을 공유하지 않는 두 사용자 간에 하루 계획된 시간 수가 다를 수 있습니다. 프로젝트에서 여러 청구 요금 무시를 사용할 때도 서로 다른 계획된 수익 번호가 표시됩니다.

* [다른 시간대의 사용자에 대한 계획된 수익 계산](#calculate-planned-revenue-for-users-in-different-time-zones)
* [다른 시간대의 사용자에 대한 실제 수익 계산](#calculate-actual-revenue-for-users-in-different-time-zones)

### 다른 시간대의 사용자에 대한 계획된 수익 계산 {#calculate-planned-revenue-for-users-in-different-time-zones}

>[!NOTE]
>
>다른 시간대의 사용자가 동일한 프로젝트에서 작업하고 있는 경우 주중 프로젝트에 대한 청구 요금 대체를 변경하지 않는 것이 좋습니다. 이렇게 하면 사용자의 일정에 있는 시간대와 Workfront 시스템 시간대 간의 시간 차이로 인해 프로젝트에 대한 잘못된 계획된 수익 금액이 표시될 수 있습니다. 대부분의 일정에서는 주말을 계획된 시간 계산에서 제외할 수 있습니다. 작업 역할의 청구 요금 재정의에 변경 사항이 발생하는 경우 작업 기간 중간에 해당할 수 있는 주중보다 주말에 발생하는 것이 좋습니다.

다른 시간대의 사용자에 대한 계획된 수익을 계산할 때 다음 사항을 고려하십시오.

* 이 있는 작업의 경우 **수익 유형** / **시간별 역할** 및 이(가) 작업 역할에 할당되었습니다. **계획된 수익** 는 다음을 곱하여 계산됩니다. **계획된 시간** 작업 역할의 청구 요율별 작업.

* 다음 **계획된 시간** 전체에 고르게 분포되어 있습니다. **기간** 작업.

* 다음 **기간** 다음 기간 사이의 기간입니다. **계획된 시작** **날짜** 및 **계획된 완료 일자** 작업. 이유:**계획된 시작 일자** 및 **계획된 완료 일자** 작업 중 은 작업을 보는 사용자의 시간대에 따라 다를 수 있으며, 다른 시간대에 있는 두 명의 사용자에 대해 일별 계획된 시간의 양이 다를 수 있습니다.

* 작업 역할의 청구 요금이 변경되지 않았거나 청구 요금 재정의가 한 개만 있는 경우 일별 계획된 시간의 양은 프로젝트의 계획된 수익을 변경하지 않습니다. 이 경우 서로 다른 두 시간대의 두 사용자에게 일별 계획된 시간이 다르더라도 프로젝트의 전체 계획된 수익은 두 사용자 간에 동일합니다.

  그러나 여러 청구 요금 무시의 경우 전체적으로 **계획된 수익** 은(는) 일별 계획된 시간 (두 명의 사용자에 대해 다를 수 있음)의 양과 청구 요금 재정의 (각 사용자가 고유한 시간대에서 작업을 볼 때 동일한 날에 대해 다를 수 있음)에 의존하므로, 두 명의 사용자가 서로 다른 시간대에 있는 이(가) 서로 다른 것처럼 보일 수 있습니다.

* 정확함 **계획된 수익** amount는 Workfront 인스턴스의 시간대와 동일한 시간대를 가진 사용자가 보는 값입니다. Workfront 관리자는 시스템 고객 정보 영역에서 Workfront 시간대를 정의합니다.\
  시스템의 시간대 정의에 대한 자세한 내용은 문서 를 참조하십시오 [시스템에 대한 기본 정보 구성](../../../administration-and-setup/get-started-wf-administration/configure-basic-info.md).

### 다른 시간대의 사용자에 대한 실제 수익 계산 {#calculate-actual-revenue-for-users-in-different-time-zones}

다른 시간대의 사용자에 대한 실제 매출을 계산할 때는 다음 사항을 고려하십시오.

* 다음의 경우 **수익 유형** 작업: **시간별 역할**, Workfront은 **실제 근로시간** (이)가 작업을 계산하기 위해 작업에 할당된 작업 역할의 청구 요금이 있는 작업에 대해 **실제 수익**. 실제 시간은 작업에 직접 기록된 시간입니다.

* 여러 청구 요금이 무시되는 경우 Workfront은 시간대가 다음과 일치하는 작업 역할의 청구 요금을 사용합니다. **입력 일자** 계산할 작업에 기록된 시간 중 **실제 수익**.

* 왜냐면 타임스탬프가 **입력 일자** 기록된 시간 및 여러 청구 요금 무시의 날짜 범위에 타임스탬프가 없는 경우 **실제 수익** 계산은 사용자와 연결된 시간대의 영향을 받지 않습니다.

계산에 사용되는 작업 역할에 대한 자세한 정보 **실제 수익**&#x200B;이 문서에서 설명하는 &quot;사용자 및 역할 할당에 따른 작업에 대한 수익 계산 이해&quot; 섹션을 참조하십시오 [청구 및 수익 개요](../../../manage-work/projects/project-finances/billing-and-revenue-overview.md).

## 프로젝트 재무 다시 계산

프로젝트에 기록된 시간이 변경될 때 프로젝트의 재정이 계산됩니다.

프로젝트의 수명 동안 비율이 변경된 경우 프로젝트의 재무 다시 계산 옵션을 사용하여 프로젝트의 비용 및 수익을 수동으로 다시 계산할 수 있습니다. 또한 일부 작업은 자동 재계산을 트리거합니다.

프로젝트 재무 다시 계산에 대한 자세한 내용은 문서 를 참조하십시오 [프로젝트 재무 다시 계산](../../../manage-work/projects/project-finances/recalculate-project-finances.md).

## API를 사용하여 새 청구 요금 추가

API를 사용하여 작업 역할에 대한 새 청구 요금을 추가하려면 다음을 수행합니다 *setRatesForRole* 에 대한 작업 **비율** 을 사용하는 개체 *PUT 방법*.
의 작업 및 날짜 필드 **비율** 개체는 API 버전 8.0에서 사용할 수 있습니다. 프로젝트의 작업 역할에 대해 이미 여러 청구 요금이 정의되어 있고 새 날짜 범위를 사용하여 새 청구 요금을 추가하려면 기존 요금과 추가할 요금을 동일한 API 호출에 모두 포함해야 합니다. 이는 개체에 대한 컬렉션을 업데이트하는 방법과 유사합니다.

다음 API 호출은 **attachableID** 은(는) **프로젝트 ID** 및 을(를) 추가하는 프로젝트의 **역할 ID** 은(는) **작업 역할 ID** 에 대해 새 청구 요금을 추가합니다.<pre>{</pre><pre>&quot;attachableID&quot;:&quot;593f01500000557d75fdd4fdfcc624f2&quot;,</pre><pre>&quot;attachableObjCode&quot;:&quot;PROJ&quot;,</pre><pre>&quot;roleID&quot;:&quot;544820df000014148cda5136d4b79d09&quot;, </pre><pre>&quot;비율&quot;:[</pre><pre>         {&quot;rateValue&quot;:&quot;0.00&quot;,&quot;startDate&quot;:null,&quot;endDate&quot;:&quot;2017-06-11&quot;},</pre><pre>         {&quot;rateValue&quot;:&quot;45.00&quot;,&quot;startDate&quot;:&quot;2017-06-12&quot;,&quot;endDate&quot;:&quot;2017-06-17&quot;},</pre><pre>         {&quot;rateValue&quot;:&quot;95.00&quot;,&quot;startDate&quot;:&quot;2017-06-21&quot;,&quot;endDate&quot;:null}</pre><pre>]</pre><pre>}</pre>Workfront API 사용에 대한 자세한 내용은 문서를 참조하십시오 [API 기본 사항](https://experience.workfront.com/s/article/API-Basics-638808549).
