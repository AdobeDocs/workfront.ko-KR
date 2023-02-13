---
product-area: projects
navigation-topic: financials
title: Job 역할 청구 비율 대체 및 프로젝트에 대한 수익 계산 개요
description: 청구 비율을 사용하여 프로젝트에서 사용한 시간 수에 프로젝트 수익을 곱할 때 프로젝트에서 수익을 계산할 수 있습니다. 청구 비율 및 매출에 대한 자세한 내용은 청구 및 수익 개요 문서를 참조하십시오.
author: Alina
feature: Work Management
exl-id: 63ba6758-ba62-48b4-89f4-d784e32a1bfa
source-git-commit: f2f825280204b56d2dc85efc7a315a4377e551c7
workflow-type: tm+mt
source-wordcount: '3644'
ht-degree: 0%

---

# Job 역할 청구 비율 대체 및 프로젝트에 대한 수익 계산 개요

청구 비율을 사용하여 프로젝트에서 사용한 시간 수에 프로젝트 수익을 곱할 때 프로젝트에서 수익을 계산할 수 있습니다. 청구 비율 및 매출에 대한 자세한 내용은 문서를 참조하십시오 [청구 및 수익 개요](../../../manage-work/projects/project-finances/billing-and-revenue-overview.md).

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

## 직무 역할 청구 비율 및 역할 시간별 수익 유형 개요

Adobe Workfront 관리자는 사용자 및 작업 역할 둘 다에 청구 비율을 연결할 수 있습니다.\
사용자 생성 및 이를 청구 요금과 연관시키는 방법에 대한 자세한 내용은 문서를 참조하십시오 [사용자 추가](../../../administration-and-setup/add-users/create-and-manage-users/add-users.md). Job 역할 생성 및 청구 단가 연관에 대한 자세한 내용은 문서를 참조하십시오 [작업 역할 만들기 및 관리](../../../administration-and-setup/set-up-workfront/organizational-setup/create-manage-job-roles.md).

사용자와 연결된 청구 비율은 대체할 수 없습니다.

직무 역할과 연관된 청구 비율은 회사 또는 프로젝트 레벨에서 대체할 수 있습니다.

Job 역할의 청구 비율을 기반으로 프로젝트에 대한 수익을 계산하려면 **매출 유형** 프로젝트에 대한 작업 중 하나는 다음 중 하나여야 합니다.

* 시간별 역할
* 시간별 역할(수용작업량 포함)
* 시간별 역할과 고정

에 대한 자세한 정보 **매출 유형** 및 청구 단가 [청구 및 수익 개요](../../../manage-work/projects/project-finances/billing-and-revenue-overview.md).

## 수익을 계산할 때 청구 비율 대체 계층

Job 역할에는 다음과 같은 방법으로 Job 역할과 연관된 청구 비율이 있을 수 있습니다.

* Workfront 관리자는 해당 작업 역할을 만들 때 작업 역할과 연관된 시스템 수준의 청구 비율을 정의할 수 있습니다.\
   작업 역할 만들기에 대한 자세한 내용은 [작업 역할 만들기 및 관리](../../../administration-and-setup/set-up-workfront/organizational-setup/create-manage-job-roles.md).

* Workfront 관리자는 회사를 생성할 때 동일한 Job 역할에 대해 회사 수준의 청구 비율을 정의할 수 있습니다.\
   Workfront이 이 회사와 연결된 프로젝트에 대한 수익을 계산할 때 이 Job 역할에 대한 시스템 수준 청구 비율 대신 역할이 태스크에 지정될 때 회사 청구 비율이 사용됩니다.\
   회사 수준에서 변경된 직무 역할율은 해당 회사와 연관된 모든 프로젝트에 영향을 줍니다.

   >[!NOTE]
   >
   >회사 청구 비율을 갱신해야 하는 경우 프로젝트의 요금이 자동으로 업데이트되지 않습니다. 프로젝트에서 회사를 제거하고 회사 비율을 갱신한 다음 프로젝트에 회사를 다시 첨부해야 새 회사 비율이 프로젝트에 적용됩니다. 프로젝트에 회사 첨부에 대한 지침은 [프로젝트 편집](../../../manage-work/projects/manage-projects/edit-projects.md).

   특정 회사에 대한 Job 역할 청구 단가 생성에 대한 자세한 내용은 [회사 만들기 및 편집](../../../administration-and-setup/set-up-workfront/organizational-setup/create-and-edit-companies.md).

* Workfront 관리자는 프로젝트를 편집할 때 사용자가 수동으로 프로젝트 재정을 재계산할 때 회사 수준 청구 비율에 변경 사항을 프로젝트에 적용하는 옵션을 활성화할 수 있습니다.\
   자세한 내용은 [회사 수준 청구 단가로 프로젝트 레벨 청구 비율 대체](../../../manage-work/projects/project-finances/override-project-level-with-company-level-billing-rates.md).

* 프로젝트 관리자는 프로젝트 레벨에서 동일한 작업 역할에 대한 청구 비율을 정의할 수 있습니다.\
   프로젝트에서 변경된 작업 역할 비율은 해당 프로젝트에만 영향을 줍니다.

   프로젝트의 역할 비율 재지정에 대한 자세한 내용은 [프로젝트 레벨에서 작업 역할 청구 비율 대체](../../../manage-work/projects/project-finances/override-job-role-billing-rates-at-the-project-level.md).

>[!IMPORTANT]
>
>작업 역할이 시스템 레벨, 회사 레벨 및 프로젝트 레벨에서 청구 비율에 연관된 경우, Workfront은 작업 역할 비율을 사용할 때 프로젝트 레벨에서 작업 역할의 청구 비율을 사용하여 태스크 수익을 계산합니다. 모든 작업의 수익은 프로젝트의 수익에 해당합니다.

## 프로젝트 레벨에서 작업 역할 청구 비율 대체

프로젝트 관리자는 특정 프로젝트에서 작업 역할에 대한 청구 비율을 지정할 수 있습니다. 이 프로젝트 레벨 청구 비율은 이 작업 역할에 대한 시스템 레벨에서 청구 비율을 대체합니다. Workfront은 시스템 수준 청구 비율을 사용하는 대신 작업 역할의 프로젝트 수준 청구 비율을 사용하여 수익을 계산합니다.

프로젝트 레벨에서 작업 역할 청구 비율을 무효화하는 방법에 대한 자세한 내용은 [프로젝트 레벨에서 작업 역할 청구 비율 대체](../../../manage-work/projects/project-finances/override-job-role-billing-rates-at-the-project-level.md).

프로젝트에서 수익을 계산하는 데 사용되는 작업 역할에 대한 자세한 내용은 의 &quot;사용자 및 역할 지정을 기반으로 한 작업에 대한 수익 계산&quot; 섹션을 참조하십시오 [청구 및 수익 개요](../../../manage-work/projects/project-finances/billing-and-revenue-overview.md).

>[!NOTE]
>
>실제 수익의 경우, 청구됨으로 표시된 청구 레코드에 추가된 시간에 적용되는 청구 비율은 청구 레코드가 청구된 후 발생하는 청구 비율 대체의 영향을 받지 않습니다.

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

## 프로젝트의 청구 비율 섹션 개요

프로젝트와 연관된 작업 역할에 대한 대체 청구 비율을 지정한 후에는 모든 작업 역할 및 그 대체값을 **청구 비율** 탭으로 이동합니다.

다음 정보를 **청구 비율**:

* [작업 역할 그룹화](#job-role-grouping)
* [프로젝트 청구 비율 값](#project-billing-rate-value)
* [기본 청구 비율 값](#default-billing-rate-value)
* [회사 청구 비율 값](#company-billing-rate-value)
* [복수 청구 비율 값 및 시간대](#multiple-billing-rate-values-and-timeframes)

### 작업 역할 그룹화 {#job-role-grouping}

청구 비율은 **청구 비율** 각 작업 역할별 영역.

### 프로젝트 청구 비율 값 {#project-billing-rate-value}

Job 역할에 해당하는 그룹핑 라인에서, **프로젝트 청구 비율** 열. 작업 롤에 복수 대체 비율이 있는 경우 현재 날짜에 해당하는 대체 비율이 의 그룹화 라인에 표시됩니다 **프로젝트 청구 비율** 열.

### 기본 청구 비율 값 {#default-billing-rate-value}

Job 역할의 그룹핑 라인에서 Job 역할에 대한 청구 비율을 시스템 레벨에서 확인합니다. **기본 청구 비율** 열.

>[!NOTE]
>
>Job 역할에 대한 프로젝트 청구 비율이 있는 경우 **기본 청구 비율** 이 프로젝트에 대한 매출 계산에는 적용되지 않습니다. 전용 **프로젝트 청구 비율** 이 적용되어 매출액을 계산합니다.

### 회사 청구 비율 값 {#company-billing-rate-value}

Job 역할의 그룹핑 라인에서 Job 역할에 대한 청구 비율을 회사 레벨에서 확인합니다. **회사 청구 비율** 열. 즉, 이 프로젝트와 연결된 회사가 있으며 이 Job 역할은 해당 회사에 대해 다른 청구 비율을 갖습니다. 프로젝트 비율과 동일한 경우에도 회사의 청구 비율이 표시됩니다.

>[!NOTE]
>
>Job 역할에 대한 프로젝트 청구 비율이 있는 경우 **회사 청구 비율** 이 프로젝트에 대한 매출 계산에는 적용되지 않습니다. 전용 **프로젝트 청구 비율** 이 적용되어 매출액을 계산합니다.

### 복수 청구 비율 값 및 시간대 {#multiple-billing-rate-values-and-timeframes}

특정 Job 역할에 대해 복수 대체 청구 비율이 있는 경우 해당 Job 역할에 대한 그룹핑 아래에 나열됩니다. 인라인 편집을 사용하여 재정의율과 **시작** **날짜** 및 **종료 날짜** 이 탭의 청구 요금 대체

>[!NOTE]
>
>을(를) 지정할 수 없습니다 **시작 날짜** 첫 번째 재지정 비율에 대해, **종료 날짜** 마지막 재정의 비율. Workfront에서는 보다 오래된 날짜가 있는 모든 시간에 대해 첫 번째 재정의 비율이 적용된다고 가정합니다 **종료 날짜** 첫 번째 재정의보다 최신 날짜가 있는 모든 시간에 대해 마지막 재지정 비율이 적용됩니다. **시작 날짜** 마지막 재정의입니다.\
>프로젝트의 계획 시작 일자 전에 시간이 기록되면 첫 번째 청구 비율이 사용됩니다.\
>프로젝트의 계획 완료 일자 이후에 시간이 기록되면 마지막 청구 비율이 사용됩니다.

## 계획 수익 계산

* [1회 청구 비율 대체를 기반으로 계획 수익 계산](#calculate-planned-revenue-based-on-a-one-time-billing-rate-override)
* [복수 청구 비율 대체를 기반으로 계획된 수익 계산](#calculate-planned-revenue-based-on-multiple-billing-rate-overrides)
* [작업 기간에 대한 계획 시간 배포](#distribution-of-planned-hours-across-the-duration-of-a-task)

### 1회 청구 비율 대체를 기반으로 계획 수익 계산 {#calculate-planned-revenue-based-on-a-one-time-billing-rate-override}

1회 청구 비율 대체를 기준으로 계획 수익을 계산할 때 다음 사항을 고려하십시오.

* 이 **매출 유형** 작업 **시간별 역할**, Workfront은 작업의 계획 시간 및 작업과 연관된 작업 역할의 청구 비율을 곱하여 작업에 대한 계획 수익을 계산합니다.

* 프로젝트 레벨에서 작업 역할의 청구 비율이 대체되면 Workfront은 프로젝트의 대체 비율을 사용하여 계획 수익을 계산합니다.
* 태스크에 여러 발령이 있는 경우 각 발령의 Job 역할에 대한 청구 단가 및 각 계획 시간 할당의 청구 비율을 곱하여 계획 수익을 계산합니다.

>[!NOTE]
>
>발령당 계획 시간은 여러 발령의 경우 태스크에 대한 계획 시간과 같지 않습니다.

계획 수익 계산에 사용되는 Job 역할에 대한 자세한 내용은 문서의 &quot;사용자 및 역할 지정을 기반으로 태스크에 대한 수익 계산 이해&quot; 섹션을 참조하십시오 [청구 및 수익 개요](../../../manage-work/projects/project-finances/billing-and-revenue-overview.md).

### 복수 청구 비율 대체를 기반으로 계획된 수익 계산 {#calculate-planned-revenue-based-on-multiple-billing-rate-overrides}

복수 청구 비율 대체를 기준으로 계획 수익을 계산할 때 다음 사항을 고려하십시오.

* 이 **매출 유형** 작업 **시간별 역할**, Workfront은 작업의 계획 시간 및 작업과 연관된 작업 역할의 청구 비율을 곱하여 작업에 대한 계획 수익을 계산합니다.

   계획 수익 계산에 사용되는 Job 역할에 대한 자세한 내용은 문서의 &quot;사용자 및 역할 지정을 기반으로 태스크에 대한 수익 계산 이해&quot; 섹션을 참조하십시오 [청구 및 수익 개요](../../../manage-work/projects/project-finances/billing-and-revenue-overview.md).

* 복수 청구 비율 대체의 경우 작업 기간 동안 계획된 시간을 곱하는 비율이 변경됩니다. 기본적으로 Workfront은 작업 기간에 걸쳐 계획된 시간을 균등하게 분배하여 작업 일마다 동일한 시간 수를 할당합니다. 계산할 때 **계획된 수익** 작업의 경우 Workfront은 일별 계획 시간과 해당 일의 청구 비율을 곱합니다. 여러 청구 비율의 경우 해당 비율은 매일 다를 수 있습니다.

   예를 들어 시간별 역할을 가진 작업이 있습니다 **매출 유형**. 작업의 기간은 5일이며 계획 시간 값은 40시간입니다. 일별 계획 시간은 8시간입니다. 작업에 프로젝트 관리자 작업 역할을 지정하고 작업의 마지막 3일 동안 이 작업 역할의 청구 비율을 대체하므로 처음 2일 동안 비율 1의 청구 비율이 있고 이 작업 역할에 대한 나머지 3일 동안 비율 2의 청구 비율이 지정됩니다.

   를 계산하는 공식입니다 **계획된 수익** 이 작업의 경우:

   ```
   Planned Revenue = (Rate 1) * (Planned Hours for Day 1) + (Rate 1) * (Planned hours for Day 2) + (Rate 2) * (Planned hours for Day 3) + (Rate 2) * (Planned hours for Day 4) + (Rate 2) * (Planned hours for Day 5)
   ```

Workfront에서 일별 계획 시간 금액을 찾는 방법에 대한 자세한 내용은 섹션을 참조하십시오 [작업 기간에 대한 계획 시간 배포](#distribution-of-planned-hours-across-the-duration-of-a-task) 참조하십시오.

>[!NOTE]
>
>작업에 여러 개의 담당자를 두고 있는 경우, 먼저 각 할당자에게 계획 시간 값이 분배되고, 작업 기간 동안 매일 분배됩니다. 이 경우, 계획 수익은 복수 청구 비율의 경우, 태스크 기간 동안 변경될 수 있는 각 직무 역할의 청구 비율을 고려하여 각 담당자에 대한 일별 시간을 계산합니다.

### 작업 기간에 대한 계획 시간 배포 {#distribution-of-planned-hours-across-the-duration-of-a-task}

작업 기간 동안 계획된 시간 분포를 이해할 때는 다음 사항을 고려하십시오.

* 기본적으로 Workfront은 작업 기간에 걸쳐 계획 시간을 균등하게 분배하여 프로젝트 예약의 가용성에 따라 각 작업 일마다 동일한 수의 계획 시간을 할당합니다.

   작업 기간 동안의 계획 시간 분포를 이해하는 방법에 대한 자세한 내용은 문서의 &quot;작업 기간 동안 계획된 시간 분포를 이해하는&quot; 섹션을 참조하십시오 [계획 시간 개요](../../../manage-work/tasks/task-information/planned-hours.md).

   >[!NOTE]
   >
   >일별 계획 시간은 태스크 기간 동안 각 일별 계획 시간 할당이 됩니다. 태스크에 하나의 발령이 있는 경우 이 숫자는 발령당 일별 계획 시간 도 나타냅니다. 작업에 여러 개의 할당이 있는 경우 발령당 하루 계획 시간은 태스크에 대한 하루 계획 시간과 다릅니다. Workfront에는 여러 개의 할당이 있는 작업의 경우 할당당 하루 계획 시간 수에 대한 시각적 표현이 없습니다.
   >
   >
   >일별 계획 시간 에는 해당 일별 계획 수익을 계산하기 위해 해당 일별 작업에 지정된 작업 역할에 대한 청구 비율을 곱합니다. 이 방법으로 계산된 모든 일별 계획 수익의 합계가 해당 태스크에 대한 계획 매출과 같습니다.

## 실제 매출 계산

* [1회 청구 비율 대체를 기반으로 실제 수익 계산](#calculate-actual-revenue-based-on-a-one-time-billing-rate-override)
* [복수 청구 비율 대체를 기반으로 실제 수익 계산](#calculate-actual-revenue-based-on-multiple-billing-rate-overrides)

### 1회 청구 비율 대체를 기반으로 실제 수익 계산 {#calculate-actual-revenue-based-on-a-one-time-billing-rate-override}

1회 청구 비율 대체를 기반으로 실제 수익을 계산할 때 다음 사항을 고려하십시오.

* 이 **매출 유형** 작업 **시간별 역할**, Workfront에 곱하기 **실제 시간** 작업 계산 작업과 연관된 작업 역할의 청구 비율에 따른 작업 **실제 매출** 작업 실제 시간은 작업에 직접 기록되는 시간입니다.

   계산하는 데 사용되는 작업 역할에 대한 자세한 정보 **실제 매출**&#x200B;의 경우 문서에서 &quot;사용자 및 역할 지정을 기반으로 한 작업에 대한 수익 계산 이해&quot; 섹션을 참조하십시오 [청구 및 수익 개요](../../../manage-work/projects/project-finances/billing-and-revenue-overview.md).

* 프로젝트 수준에서 작업 역할의 청구 비율이 대체된 경우 Workfront은 프로젝트의 대체 비율을 사용하여 실제 수입을 계산합니다. 프로젝트에서 작업 역할의 청구 비율을 무효화하면 **실제 매출** 새로 조정된 비율을 사용하여 프로젝트의 값이 자동으로 다시 계산됩니다.

   프로젝트의 역할 비율 재지정에 대한 자세한 내용은 [프로젝트 레벨에서 작업 역할 청구 비율 대체](../../../manage-work/projects/project-finances/override-job-role-billing-rates-at-the-project-level.md).

>[!NOTE]
>
>원래 비율로 청구되는 원래 청구 비율을 초과하기 전에 프로젝트에 이미 로그인한 시간을 유지하려면, 해당 시간을 **청구 레코드**, 및에 표시를 해야 합니다 **청구 레코드** 로서의 **청구됨**. 그렇지 않으면 **실제 매출** 프로젝트에 대한 청구 비율이 재정의되기 전에 기록된 시간부터 프로젝트의 재정이 재계산될 때 신규 비율을 사용하여 재계산됩니다.\
>청구 레코드에 시간을 포함하여 다음으로 표시하는 방법에 대한 자세한 정보 **청구됨**, 문서를 참조하십시오 [청구 레코드 만들기](../../../manage-work/projects/project-finances/create-billing-records.md).

### 복수 청구 비율 대체를 기반으로 실제 수익 계산 {#calculate-actual-revenue-based-on-multiple-billing-rate-overrides}

복수 청구 비율 대체를 기준으로 실제 수익을 계산할 때 다음 사항을 고려하십시오.

* 이 **매출 유형** 작업 **시간별 역할**, Workfront에 곱하기 **실제 시간** 작업 역할에 할당된 작업 역할의 청구 비율이 있는 작업에서 계산 **실제 매출** 작업 실제 시간은 작업에 직접 기록되는 시간입니다.

* 복수 청구 비율 대체의 경우 **실제 시간** 를 곱하여 계산합니다 **실제 매출** 작업 기간 동안 변경될 수 있습니다. Workfront에서는 시간대가 **시작 날짜** 작업 계산 시간이 기록된 시간 **실제 매출.**

   예를 들어, 작업에 **매출 유형** 의 **시간별 역할** 및 은 프로젝트 관리자의 작업 역할에 할당됩니다. 6월 19일부터 6월 25일 사이의 일자에 대해 이 Job 역할의 청구 비율을 비율 1로 대체합니다. 6월 26일부터 청구 비율을 2로 바꿉니다. 6월 20일에 2시간, 6월 28일에 3시간을 기록합니다.

   Workfront이 계산합니다 **실제 매출** 이 작업의 경우 다음 공식을 사용합니다.

   ```
   Actual Revenue = 2 * Rate 1 + 3 * Rate 2
   ```

   계산하는 데 사용되는 작업 역할에 대한 자세한 정보 **실제 매출**&#x200B;의 경우 문서에서 &quot;사용자 및 역할 지정을 기반으로 한 작업에 대한 수익 계산 이해&quot; 섹션을 참조하십시오 [청구 및 수익 개요](../../../manage-work/projects/project-finances/billing-and-revenue-overview.md).

## 복수 청구 비율을 기준으로 수익을 계산할 때 시간대가 미치는 영향

Workfront의 다른 엔티티와 표준 시간대 차이가 발생하는 경우 다른 사용자와 일별 계획 시간이 다르게 표시됩니다. 다음 시나리오는 다른 사용자가 보는 것과 비교하여 사용자에 대한 1일 기준 계획 시간 정보를 왜곡할 수 있습니다.

* 두 사용자는 서로 다른 두 시간대의 컴퓨터를 설정할 수 있습니다
* Workfront의 두 사용자 프로필은 서로 다른 두 시간대로 설정될 수 있습니다
* 사용자 프로필과 연결된 시간대는 Workfront의 시스템 시간대와 다를 수 있습니다
* 사용자 프로필과 연관된 시간대는 프로젝트 예약의 시간대와 다를 수 있습니다.

이러한 경우 시간대의 동일한 설정을 공유하지 않는 두 사용자 간에 일별 계획 시간 수가 다를 수 있습니다. 또한 프로젝트에서 복수 청구 비율 대체를 사용할 때 다른 계획 수익 번호를 볼 수 있습니다.

* [다른 시간대에 있는 사용자의 계획 수익 계산](#calculate-planned-revenue-for-users-in-different-time-zones)
* [다른 시간대에 있는 사용자의 실제 매출 계산](#calculate-actual-revenue-for-users-in-different-time-zones)

### 다른 시간대에 있는 사용자의 계획 수익 계산 {#calculate-planned-revenue-for-users-in-different-time-zones}

>[!NOTE]
>
>동일한 프로젝트에서 작업하는 다른 시간대에 있는 사용자가 있는 경우 해당 주 동안 프로젝트에 대한 청구 비율 대체를 변경하지 않는 것이 좋습니다. 이렇게 하면 사용자 예약의 시간대와 Workfront 시스템 시간대 간의 시간 차이로 인해 프로젝트에 대한 잘못된 계획 수익 금액이 표시될 수 있습니다. 대부분의 스케줄은 계획 시간 계산에서 주말을 제외할 수 있습니다. Job 역할의 청구 비율 재정의에 변경이 발생하면 작업 기간 중간에 일치할 수 있는 주 중보다 주말 동안 발생하는 것이 좋습니다.

다른 시간대에 있는 사용자의 계획 수익을 계산할 때 다음 사항을 고려하십시오.

* 가 있는 작업의 경우 **매출 유형** 의 **시간별 역할** 작업 역할에 할당되고 **계획된 수익** 은(는) **계획 시간** 작업 역할의 청구 비율에 의한 작업의 수입니다.

* 다음 **계획 시간** 는 **기간** Analytics JavaScript에서 액세스 권한을 부여합니다.

* 다음 **기간** 는 **계획된 시작** **날짜** 그리고 **계획 완료 일자** Analytics JavaScript에서 액세스 권한을 부여합니다. 왜냐하면&#x200B;**계획 시작 날짜** 및 **계획 완료 일자** 작업 중 작업은 작업을 보는 사용자의 시간대에 따라 다를 수 있으며, 두 개의 다른 시간대에 있는 두 사용자에게 일별 계획 시간 수가 다를 수 있습니다.

* Job 역할의 청구 비율이 변경되지 않았거나 청구 비율 대체가 하나만 있는 경우, 일별 계획 시간 금액은 프로젝트의 계획 수익을 변경하지 않습니다. 이 경우 서로 다른 두 시간대의 두 사용자가 서로 다른 하루 계획 시간을 보더라도 프로젝트의 전체 계획 수익은 두 사용자 간에 동일합니다.

   그러나 복수 청구 비율 대체의 경우 전체 **계획된 수익** 프로젝트 중 두 개의 다른 시간대에 있는 두 사용자에게 다르게 보일 수 있습니다. 이는 일별 계획 시간(두 사용자에게 다를 수 있음)의 양과 청구 비율 대체(각 사용자가 자신의 시간대에 있는 작업을 볼 때 같은 날에 대해 다를 수 있음)에 의존하기 때문입니다.

* 정확성 **계획된 수익** 금액은 Workfront 인스턴스의 시간대와 동일한 시간대를 가진 사용자가 보는 시간대입니다. Workfront 관리자는 시스템 고객 정보 영역에서 Workfront 시간대를 정의합니다.\
   시스템의 시간대 정의에 대한 자세한 내용은 문서를 참조하십시오 [시스템에 대한 기본 정보 구성](../../../administration-and-setup/get-started-wf-administration/configure-basic-info.md).

### 다른 시간대에 있는 사용자의 실제 매출 계산 {#calculate-actual-revenue-for-users-in-different-time-zones}

다른 시간대에 있는 사용자의 실제 매출액을 계산할 때 다음 사항을 고려하십시오.

* 이 **매출 유형** 작업 **시간별 역할**, Workfront에 곱하기 **실제 시간** 작업 역할에 할당된 작업 역할의 청구 비율이 있는 작업에서 다음을 계산하여 **실제 매출**. 실제 시간은 작업에 직접 기록되는 시간입니다.

* 복수 청구 비율 재정의의 경우 Workfront은 시간 프레임과 일치하는 작업 역할의 청구 비율을 사용합니다 **시작 날짜** 작업 계산 시간이 기록된 시간 **실제 매출**.

* 에 타임스탬프가 없으므로 **시작 날짜** 로그된 시간 및 복수 청구 비율 재정의의 날짜 범위에 타임스탬프가 없습니다. **실제 매출** 계산은 사용자와 연결된 표준 시간대의 영향을 받지 않습니다.

계산하는 데 사용되는 작업 역할에 대한 자세한 정보 **실제 매출**&#x200B;의 경우 문서에서 &quot;사용자 및 역할 지정을 기반으로 한 작업에 대한 수익 계산 이해&quot; 섹션을 참조하십시오 [청구 및 수익 개요](../../../manage-work/projects/project-finances/billing-and-revenue-overview.md).

## 프로젝트 재무 재계산

프로젝트 로그된 시간 내에 변경 사항이 발생할 경우 재정은 프로젝트에서 계산됩니다.

프로젝트 수명 동안 비율이 변경되면 프로젝트에서 재무 재계산 옵션을 사용하여 프로젝트의 비용과 수익을 수동으로 재계산할 수 있습니다. 또한 일부 작업은 자동 다시 계산을 트리거합니다.

프로젝트 재정 재계산에 대한 자세한 내용은 문서를 참조하십시오 [프로젝트 재무 재계산](../../../manage-work/projects/project-finances/recalculate-project-finances.md).

## API를 사용하여 새 청구 비율 추가

API를 사용하여 작업 역할에 대한 새 청구 비율을 추가하려면 *setRatesForRole* 작업 **비율** 개체를 사용하여 *PUT 메서드*.
작업 및 날짜 필드는 **비율** 객체는 API 버전 8.0에서 사용할 수 있습니다. 프로젝트에서 작업 역할에 대해 이미 몇 개의 청구 요금이 정의되어 있고 새 날짜 범위를 사용하여 새 청구 비율을 추가하려면 동일한 API 호출에 추가할 기존 비율과 비율을 모두 포함해야 합니다. 이는 개체의 컬렉션을 업데이트하는 방법과 유사합니다.

다음 API 호출이 **attachableID** 은 **프로젝트 ID** 비율을 추가하고 있는 프로젝트의 **RoleID** 은 **작업 역할 ID** 신규 청구 비율을 추가하는 경우.<pre>{</pre><pre>&quot;attachableID&quot;:&quot;593f01500000557d75fdd4fdfcc624f2&quot;,</pre><pre>&quot;attachableObjCode&quot;:&quot;PROJ&quot;,</pre><pre>&quot;roleID&quot;:&quot;544820df000014148cda5136d4b79d09&quot;, </pre><pre>&quot;rates&quot;:[</pre><pre>         {&quot;rateValue&quot;:&quot;0.00&quot;,&quot;startDate&quot;:null,&quot;endDate&quot;:&quot;2017-06-11&quot;},</pre><pre>         {&quot;rateValue&quot;:&quot;45.00&quot;,&quot;startDate&quot;:&quot;2017-06-12&quot;,&quot;endDate&quot;:&quot;2017-06-17&quot;},</pre><pre>         {&quot;rateValue&quot;:&quot;95.00&quot;,&quot;startDate&quot;:&quot;2017-06-21&quot;,&quot;endDate&quot;:null}</pre><pre>]</pre><pre>}</pre>Workfront API 사용에 대한 자세한 내용은 문서를 참조하십시오 [API 기본 사항](https://experience.workfront.com/s/article/API-Basics-638808549).
