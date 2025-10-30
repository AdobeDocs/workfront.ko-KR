---
user-type: administrator
product-area: system-administration;user-management
navigation-topic: organization-setup
title: 작업 역할 만들기 및 관리
description: ' [!DNL Adobe Workfront] 관리자 또는 작업 역할에 대한 관리 액세스 권한이 있는 사용자는 사용자에게 할당할 수 있는 작업 역할을 만들고 조직과 관련이 없는 기본 작업 역할을 삭제할 수 있습니다.'
author: Lisa
feature: System Setup and Administration
role: Admin
exl-id: 664fb2fe-ff7e-4807-9a43-b37e7d5d57eb
source-git-commit: e5416fab4f4ad1f2c31edf962554ddd6a4c2f1e5
workflow-type: tm+mt
source-wordcount: '1165'
ht-degree: 0%

---

# 작업 역할 만들기 및 관리

<!-- Audited: 1/2024 -->

<!--DON'T DELETE, DRAFT OR HIDE THIS ARTICLE. IT IS LINKED TO THE PRODUCT, THROUGH THE CONTEXT SENSITIVE HELP LINKS.-->

>[!IMPORTANT]
>
>25.11 릴리스에서는 작업 역할에 대한 통화 재정의가 프로덕션에서 더 이상 사용되지 않습니다. (사용 중단은 미리보기 환경에서 10월 30일에 수행됩니다.) 기본 통화와 대체 통화를 사용하는 대신 작업 역할에 하나의 통화를 사용할 수 있으며 해당 통화를 사용하여 비용 및 청구 요금이 정의됩니다.

[!DNL Adobe Workfront] 관리자 또는 작업 역할에 대한 관리 액세스 권한이 있는 사용자는 사용자에게 할당할 수 있는 작업 역할을 만들고 조직과 관련이 없는 기본 작업 역할을 삭제할 수 있습니다. [!DNL Workfront]의 관리 액세스에 대한 자세한 내용은 [특정 영역에 대한 관리 액세스 권한 부여](../../../administration-and-setup/add-users/configure-and-grant-access/grant-users-admin-access-certain-areas.md)를 참조하십시오.

## 액세스 요구 사항

+++ 을 확장하여 이 문서의 기능에 대한 액세스 요구 사항을 봅니다.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!DNL Adobe Workfront] 패키지</td> 
   <td><p>임의</p></td> 
  </tr> 
  <tr> 
   <td>[!DNL Adobe Workfront] 라이센스</td> 
   <td><p>[!UICONTROL Standard]</p>
       <p>[!UICONTROL 계획]</p></td>
  </tr> 
  <tr> 
   <td>액세스 수준 구성</td> 
   <td>작업 역할에 대한 관리 액세스</td>
  </tr> 
 </tbody> 
</table>

자세한 내용은 [Workfront 설명서의 액세스 요구 사항](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)을 참조하십시오.

+++

## 작업 역할 만들기

작업 역할을 생성하려면 다음을 수행합니다.

{{step-1-to-setup}}

1. 왼쪽 패널에서 **[!UICONTROL &#x200B;작업 역할].**&#x200B;을 클릭합니다.
1. **[!UICONTROL 새 작업 역할]을 클릭합니다.**
1. 다음 필드를 구성합니다.

   * **이름**: 작업 역할의 이름을 나타냅니다. Workfront에서 작업 역할 필드가 표시되는 모든 위치에 표시되는 이름입니다.

     >[!TIP]
     >
     >작업 역할의 이름은 최대 255자를 포함할 수 있습니다. 그러나 Workfront의 특정 영역에서 더 긴 이름이 잘릴 수 있습니다.

   * **설명**: 역할에 대한 고유한 설명을 입력하십시오.
   * **활성 상태**: 역할을 활성화하여 Workfront의 모든 곳에서 사용자, 작업 항목 등과 연결할 수 있도록 하려면 **예**&#x200B;를 선택합니다. 역할을 비활성화하고 사용자, 작업 항목 등에 할당할 수 없도록 하려면 **아니요**&#x200B;를 선택하십시오.

     작업 역할 비활성화에 대한 자세한 내용은 [작업 역할 비활성화](/help/quicksilver/administration-and-setup/set-up-workfront/organizational-setup/deactivate-job-roles.md)를 참조하십시오.

   * **기본 통화**: Workfront 관리자가 설정 영역에서 설정한 기본 통화입니다. 자세한 내용은 [환율 설정](/help/quicksilver/administration-and-setup/manage-workfront/exchange-rates/set-up-exchange-rates.md)을 참조하세요.

     >[!TIP]
     >
     >작업 역할 수준에서 기본 통화를 편집할 수 없습니다. 이 필드는 흐리게 표시되어 시스템의 기본 통화에 대한 미리 알림 역할을 합니다.

   * **비용 비율**: 작업 역할의 시간당 비용 비율입니다. 이 값은 역할과 관련된 작업 및 문제의 계획 및 실제 비용과 궁극적으로 프로젝트의 계획 및 실제 비용을 계산합니다. 기준 통화를 사용하여 환율을 입력합니다.

     날짜 유효 비용 요율을 보려면 **요율 추가**&#x200B;를 클릭하십시오. 기간에 대한 비용/시간 값을 입력하고 필요에 따라 시작 일자와 종료 일자를 지정합니다. 첫 번째 원가에는 시작 일자가 없고 마지막 원가에는 종료 일자가 없습니다.

     일부 날짜는 자동으로 추가됩니다. 예를 들어, 첫 번째 원가율에 종료 일자가 없고 시작 일자가 2025년 5월 1일인 두 번째 원가율을 추가하면, 종료 일자가 2025년 4월 30일인 첫 번째 원가율에 추가되므로 공백이 없습니다.

     >[!TIP]
     >
     >기존 작업 역할을 편집할 때 **시작 날짜별로 정렬**&#x200B;을 선택하여 요금 목록의 맨 위에 가장 최근 시작 날짜를 표시할 수 있습니다.

   * **청구 요금**: 작업 역할의 시간당 청구 요금입니다. 이 값은 역할과 관련된 작업 및 문제의 계획 및 실제 수익과 궁극적으로 프로젝트의 계획 및 실제 수익을 계산합니다. 기준 통화를 사용하여 환율을 입력합니다.

     날짜 유효 청구 요금을 보려면 **요금 추가**&#x200B;를 클릭하십시오. 기간에 대한 청구/시간의 값을 입력하고 필요에 따라 시작 일자와 종료 일자를 지정합니다. 첫 번째 청구 요금에 시작 일자가 없고 마지막 청구 요금에 종료 일자가 없습니다.

     일부 날짜는 자동으로 추가됩니다. 예를 들어 첫 번째 청구 요금에 종료 일자가 없고 시작 일자가 2025년 5월 1일인 두 번째 청구액을 추가한 경우, 간격이 없도록 종료 일자가 2025년 4월 30일인 첫 번째 청구 요금에 추가됩니다.

     >[!TIP]
     >
     >기존 작업 역할을 편집할 때 **시작 날짜별로 정렬**&#x200B;을 선택하여 요금 목록의 맨 위에 가장 최근 시작 날짜를 표시할 수 있습니다.

   * **통화 재정의**: 이 작업 역할과 연결된 통화를 선택합니다. Workfront이 이 작업 역할과 연결된 비용 및 수익을 계산하는 데 사용하는 통화입니다.

     이는 Workfront 관리자가 설정 영역에서 설정한 기본 통화와 다르며, 프로젝트와 연관된 통화와 다를 수 있습니다.

     >[!TIP]
     >
     >시스템의 환율 영역에서 사용할 수 있는 통화만 이 필드에서 사용할 수 있습니다. 통화를 하나만 설정한 경우 이 필드가 표시되지 않습니다.

     Workfront에서 기본 통화 설정에 대한 자세한 내용은 [환율 설정](/help/quicksilver/administration-and-setup/manage-workfront/exchange-rates/set-up-exchange-rates.md)을 참조하십시오.

     프로젝트 통화 변경에 대한 자세한 내용은 [프로젝트 통화 변경](/help/quicksilver/manage-work/projects/project-finances/change-project-currency.md)을 참조하십시오.

   * **통화 대체 비용 비율**: 선택한 통화 재정의를 사용하는 작업 역할의 시간당 비용 비율입니다. Workfront은 이 값을 사용하여 작업 역할과 관련된 작업 및 문제의 계획 및 실제 비용을 계산합니다.

     위에 지정된 통화 재정의 환율을 입력합니다. 기본 통화를 사용할 때 이 작업 역할의 비용 비율도 업데이트됩니다.

     Workfront에서 비용을 계산하는 방법에 대한 자세한 내용은 [비용 추적](/help/quicksilver/manage-work/projects/project-finances/track-costs.md)을 참조하십시오.

     >[!TIP]
     >
     >이미 비용 환율이 연결된 기존 작업 역할을 업데이트할 때 Workfront은 시스템의 전환율을 기반으로 통화 대체 환율을 계산합니다. 대체 통화 원가율을 갱신하면 작업 역할의 원가율도 자동으로 갱신됩니다.

   * **통화 대체 청구 요금**: 선택한 통화 재정의를 사용하는 작업 역할의 시간당 청구 요금입니다. Workfront은 이 값을 사용하여 작업 역할과 관련된 작업 및 문제의 계획 및 실제 매출을 계산합니다.

     위에 지정된 통화 재정의 환율을 입력합니다. 또한 기본 통화를 사용할 때 이 작업 역할에 대한 청구 요금이 업데이트됩니다.

     Workfront이 매출을 계산하는 방법에 대한 자세한 내용은 [청구 및 매출 개요](/help/quicksilver/manage-work/projects/project-finances/billing-and-revenue-overview.md)를 참조하십시오.

     >[!TIP]
     >
     >이미 청구 요금이 연계된 기존 작업 역할을 업데이트할 때 Workfront은 시스템의 전환율을 기반으로 통화 대체 요금을 계산합니다. 통화 대체 청구 단가를 갱신하면 작업 역할의 청구 단가도 자동으로 갱신됩니다.

<!--
   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">[!UICONTROL Name]</td> 
      <td> <p>Indicate a name for the job role. This is the name that displays everywhere in [!DNL Workfront] where the [!UICONTROL Job Role] field displays. </p> <p>Tip: The name of a job role may contain up to 255 characters. However, longer names might be truncated in certain areas of [!DNL Workfront]. </p> </td> 
     </tr>
     <tr> 
      <td role="rowheader">[!UICONTROL Description]</td> 
      <td>Enter a description for the role that indicates what is unique about it. </td> 
     </tr> 
     <tr data-mc-conditions=""> 
      <td role="rowheader"><span>[!UICONTROL Is Active]</span> </td> 
      <td> 
       <ul> 
        <li> <p>Select <b>[!UICONTROL Yes]</b> if you want the role to be active and available everywhere in [!DNL Workfront] to be associated with users, work items, etc. </p> </li> 
        <li> <p>Select <b>[!UICONTROL No]</b>, if you want the role to be deactivated and not available to assign to users, work items, etc. </p> </li> 
       </ul> <p><span>For information about deactivating job roles, see</span> <a href="../../../administration-and-setup/set-up-workfront/organizational-setup/deactivate-job-roles.md" class="MCXref xref">Deactivate job roles</a>. </p> </td> 
     </tr>
     <tr data-mc-conditions=""> 
      <td role="rowheader"><span>[!UICONTROL Base Currency]</span> </td> 
      <td> <p><span>This is the [!UICONTROL Base Currency], as set in the [!UICONTROL Setup] area by your Workfront administrator. For information, see</span> <a href="../../../administration-and-setup/manage-workfront/exchange-rates/set-up-exchange-rates.md" class="MCXref xref">Set up exchange rates</a> .</p> <p>Tip: <span>You cannot edit the [!UICONTROL Base Currency] at the job role level. This field is dimmed and serves as a reminder for what the base currency is for your system.</span> </p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL Cost Rate]</td> 
      <td><p>This is the cost per hour rate of the job role. This value calculates the planned and the actual costs of tasks and issues associated with the role, and ultimately the planned and actual costs of the projects. Enter the rate using the [!UICONTROL Base Currency].</p> 
      <p>For date effective cost rates, click <strong>[!UICONTROL Add Rate]</strong>. Enter the value of the cost/hour for the time period, and assign a [!UICONTROL Start Date] and [!UICONTROL End Date] as needed. The first cost rate will not have a start date and the last cost rate will not have an end date.</p> <p>Some dates are added automatically. For example, if the first cost rate does not have an end date, and you add a second cost rate with a start date of May 1, 2023, an end date of April 30, 2023 is added to the first cost rate so that no gaps exist.</p> <p>Tip: When editing an existing job role, you can select <strong>Sort by start date</strong> to see the most recent start date at the top of the rate list.</p></td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL Billing Rate] </td> 
      <td><p>This is the billing per hour rate of the job role. This value calculates the planned and actual revenues of tasks and issues associated with the role, and ultimately the planned and actual revenues of the projects. Enter the rate using the [!UICONTROL Base Currency].</p> <p>For date effective billing rates, click <strong>[!UICONTROL Add Rate]</strong>. Enter the value of the billing/hour for the time period, and assign a [!UICONTROL Start Date] and [!UICONTROL End Date] as needed. The first billing rate will not have a start date and the last billing rate will not have an end date.</p> <p>Some dates are added automatically. For example, if the first billing rate does not have an end date, and you add a second with a start date of May 1, 2023, an end date of April 30, 2023 is added to the first billing rate so that no gaps exist.</p> <p>Tip: When editing an existing job role, you can select <strong>Sort by start date</strong> to see the most recent start date at the top of the rate list.</p> </td> 
     </tr> 
     <tr data-mc-conditions=""> 
      <td role="rowheader"><span>[!UICONTROL Override Currency]</span> </td> 
      <td>
        <p>Select a currency associated with this job role. This is the currency that [!DNL Workfront] uses for calculating costs and revenue associated with this job role. </p> 
        <p><span>This is different than the [!UICONTROL Base Currency] set up by your [!DNL Workfront] administrator in the [!UICONTROL Setup] area, and can be different than the currency associated with a project.</span> </p> 
        <p>Tip: Only currencies available in the [!UICONTROL Exchange Rates] area in your system are available in this field. If you only have one currency set up, this field is does not appear.</p> 
       <p><span>For information about setting up the [!UICONTROL Base Currency] in [!DNL Workfront], see</span> <a href="../../../administration-and-setup/manage-workfront/exchange-rates/set-up-exchange-rates.md" class="MCXref xref">Set up exchange rates</a>.</p> <p><span>For information about changing the currency of a project, see</span> <a href="../../../manage-work/projects/project-finances/change-project-currency.md" class="MCXref xref">Change the project currency</a>.</p> </td> 
     </tr> 
     <tr data-mc-conditions=""> 
      <td role="rowheader"><span>[!UICONTROL Override Currency Cost Rate]</span> </td> 
      <td>
        <p>This is the cost per hour rate of the job role using the selected [!UICONTROL Override Currency]. [!DNL Workfront] uses this value to calculate the planned and the actual costs of tasks and issues associated with the job role. </p> 
        <p><span>Enter the rate in the [!UICONTROL Override Currency] specified above. This also updates the Cost Rate for this job role when using the [!UICONTROL Base Currency].</span> </p> 
        <p>For information about how [!DNL Workfront] calculates cost, see <a href="../../../manage-work/projects/project-finances/track-costs.md" class="MCXref xref">Track costs</a>.</p> 
       <p>Tip: When updating an existing job role that already has a Cost Rate associated with it, [!DNL Workfront] calculates the [!UICONTROL Override Currency] rate based on the conversion rate in your system. If you update the [!UICONTROL Override Currency Cost Rate], the Cost Rate of the job role also updates automatically.</p> </td> 
     </tr> 
     <tr data-mc-conditions=""> 
      <td role="rowheader"><span>[!UICONTROL Override Currency Billing Rate]</span> </td> 
      <td>
        <p>This is the billing per hour rate of the job role using the selected [!UICONTROL Override Currency]. [!DNL Workfront] uses this value to calculate the planned and the actual revenue of tasks and issues associated with the job role. </p>
        <p><span>Enter the rate in the [!UICONTROL Override Currency] specified above. This also updates the Billing Rateate for this job role when using the [!UICONTROL Base Currency].</span> </p>
        <p>For information about how [!DNL Workfront] calculates revenue, see <a href="../../../manage-work/projects/project-finances/billing-and-revenue-overview.md" class="MCXref xref">Overview of Billing and Revenue</a>.</p>
        <p>Tip: When updating an existing job role that already has a Billing Rate associated with it, [!DNL Workfront] calculates the Override Currency rate based on the conversion rate in your system. If you update the Override Currency Billing Rate, the Billing Rate of the job role also updates automatically. </p>
       </td>
     </tr> 
    </tbody> 
   </table>
-->

>[!TIP]
>
>작업 역할은 리소스 관리의 필수적인 부분입니다. 자원 계획 도구를 사용하려면 작업 역할에 연관된 비용 및 청구 요금이 필요합니다. 자세한 내용은 [리소스 관리 시작](../../../resource-mgmt/resource-mgmt-overview/get-started-resource-management.md)을 참조하세요.

1. **[!UICONTROL 작업 역할 만들기]**&#x200B;를 클릭합니다. 이제 작업 역할을 작업, 문제, 승인에 할당하거나 레이아웃 템플릿 또는 다른 개체를 공유할 수 있습니다. [!DNL Workfront]의 모든 작업 역할 사용에 대한 자세한 내용은 [작업 역할 개요](../../../administration-and-setup/set-up-workfront/organizational-setup/job-role-overview.md)를 참조하십시오. 작업 역할 삭제에 대한 자세한 내용은 [작업 역할 삭제](../../../administration-and-setup/set-up-workfront/organizational-setup/delete-job-roles.md)를 참조하십시오.

<!--
<div data-mc-conditions="QuicksilverOrClassic.Draft mode">
<h2>Delete a job role</h2>
<ol data-mc-continue="false">
<li value="1">Click the <strong>Main Menu</strong> icon <img src="assets/main-menu-icon.png"> in the upper-right corner of Adobe Workfront, then click <strong>Setup</strong> <img src="assets/gear-icon-settings.png">.</li>
<li value="2">Click<strong>Job Roles.</strong></li>
<li value="3">Select the job role that you want to delete, then click <strong>Delete.</strong></li>
<li value="4">If there are any objects (users, tasks, issues) that are assigned to the job role, do one of the following:<br>
<ul>
<li><p><strong>Replace the job role with a different job role:</strong> Select the new job role from the drop-down list.</p><p>Any current and past resource allocations that are associated with the deleted job role are transferred to the job role that you select.</p><p>Users who have only one job role assigned to them are reassigned to the job role that you select; users who have a secondary job role assigned to them are not reassigned to the job role that you select.</p></li>
<li><p><strong>Delete the job role and its resource allocation:</strong> Select<strong>None</strong> from the drop-down list.</p><note type="important">
Deleting a job role deletes all current and past resource allocation related to that job role for all projects.
</note><p>​For example, if a task or issue is assigned to only that job role, the task or issue is unassigned after the job role is deleted.</p></li>
</ul></li>
<li value="5">Click  <strong>Yes, Delete It</strong>. </li>
</ol>
</div>
-->
