---
user-type: administrator
product-area: system-administration;projects
navigation-topic: configure-system-defaults
title: 사용자 정의 영역 활성화
description: '조직의 분기가 달력 날짜(예: 업무일 또는 쇼핑일) 이외의 특정 기준을 기반으로 하는 경우, 보고를 위해 사용자 정의 분기를 만들 수 있습니다.'
author: Lisa
feature: System Setup and Administration
role: Admin
exl-id: 0f643d36-6235-4fd3-b6d3-54fbd03c9b33
last-update: 2026-04-01T18:03:50.000Z
git-commit-file: b03dbe8e217593e0f3a6fcd522148dcd8b7670b8
TQID: https://experienceleague.adobe.com/8kRfZ17zcgN0-hlc16wh328YGRjTlzuI3LAe-Yjj25s
product_v2:
  - id: c4a86a5d-6562-4fc6-aa00-bfa25833aed9
feature_v2:
  - id: d968a1bc-9a90-4926-a531-bcf272c32aad
role_v2:
  - id: c66ffd68-0f65-42bb-aa23-b4020f12e0bd
topic_v2:
  - id: aa2f3246-cb95-4b30-8899-fdf7d73550cc
  - id: eddd9b14-83bd-4ff4-9072-54a4a484abb7
source-git-commit: 85c9f757134bc84e4b5038e4001f9a9fe1430f2a
workflow-type: tm+mt
source-wordcount: 376
ht-degree: 4%

---

# 사용자 정의 영역 활성화

<!--Audited: 03/2026-->

<!--
<span class="preview">The highlighted information on this page refers to functionality not yet generally available. It is available only in the Preview environment for all customers. After the monthly releases to Production, the same features are also available in the Production environment for customers who enabled fast releases. </span>   

<span class="preview">For information about fast releases, see [Enable or disable fast releases for your organization](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/enable-fast-release-process.md). </span>
-->

조직의 분기가 달력 날짜(예: 업무일 또는 쇼핑일) 이외의 특정 기준을 기반으로 하는 경우, 보고를 위해 사용자 정의 분기를 만들 수 있습니다.

회사에서 구매한 제품에 따라 Workfront 설정 영역에서 다음 분기 수를 구성할 수 있습니다.

* [!DNL Workfront]만 구입한 고객은 [!DNL Adobe Workfront] 시스템에 대해 최대 8개의 사용자 정의 분기를 구성할 수 있습니다.
* [!DNL Workfront] 및 [!DNL Workfront Planning]을(를) 구매한 고객은 [!DNL Planning]에서도 사용할 수 있는 [!DNL Workfront] 시스템에 대해 최대 100분기를 구성할 수 있습니다.

<!--
<div class="preview">
* Customers who purchased [!DNL Workfront] and [!DNL Workfront Planning], can configure custom weeks for each custom quarter which are visible in the [!DNL Planning] timeline views. 
</div>
-->


## 액세스 요구 사항

+++ 이 문서의 기능에 대한 액세스 요구 사항을 보려면 확장하십시오.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!DNL Adobe Workfront] 패키지</td> 
   <td><p>Any</p></td> 
  </tr> 
  <tr> 
   <td>[!DNL Adobe Workfront] 라이센스</td> 
   <td><p>[!UICONTROL Workflow Standard] 또는 [!UICONTROL Workfront Plan] 라이선스</p>
       <p></p></td>
  </tr> 
  <tr> 
   <td>액세스 수준 구성</td> 
   <td>[!UICONTROL 시스템 관리자]</td> 
  </tr> 
 </tbody> 
</table>

자세한 내용은 [Workfront 설명서의 액세스 요구 사항](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)을 참조하십시오.

+++

<!--
When we release fiscal weeks, replace the table above with this:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!DNL Adobe Workfront] package</td> 
   <td>
   <ul>
   <li><p>To configure custom quarters:</p>
   <p>Any Workfront or Workflow package</p></li>
   <li>
   <div class="preview">
   <p>To configure custom weeks:</p>
   <p>Any Planning package, including Planning as a standalone product</p>
   </div>
   </li>
   </ul>
   </td> 
  </tr> 
  <tr> 
   <td>[!DNL Adobe Workfront] license</td> 
   <td>
   
   <ul>
   <li><p>To configure custom quarters:</p>
   <p>[!UICONTROL Workflow Standard] or [!UICONTROL Workfront Plan] license</p></li>
   <li>
   <div class="preview">
   <p>To configure custom weeks:</p>
   <p>A [!UICONTROL Planning Standard] license, in addition to a Workfront or a Workflow license</p>
   </div>
   </li>
   </ul>
    </td>
  </tr> 
  <tr> 
   <td>Access level configurations</td> 
   <td>[!UICONTROL System Administrator]</td> 
  </tr> 
 </tbody> 
</table>

-->


## [!DNL Workfront] 시스템에 대한 사용자 정의 영역 설정

<!--
Setting up custom quarters differs depending on which environment you use. 

### Set up custom quarters for your [!DNL Workfront] system in the Production environment
-->

{{step-1-to-setup}}

1. **[!UICONTROL 사용자 지정 분기]**&#x200B;를 클릭합니다.

1. **[!UICONTROL 사용자 정의 영역 사용]**&#x200B;을 선택합니다.

1. 사용자 정의 분기의 이름을 입력합니다(예: &quot;2021년 1분기 회계&quot;).
1. 사용자 정의 분기의 시작 및 종료 날짜를 선택합니다.

   ![사용자 지정 분기](assets/custom-quarters-nwe.png)

1. (선택 사항) 시스템에 사용자 정의 영역을 추가하려면 **[!UICONTROL 사용자 정의 영역 추가]**&#x200B;를 클릭합니다.

   >[!IMPORTANT]
   >
   > 회사에서 [!DNL Workfront Planning]을(를) 구입한 경우 분기 간에 차이가 있거나 중복되는 경우 사용자 정의 분기를 저장할 수 없습니다.
   >![겹침 경고가 있는 사용자 지정 분기](assets/custom-quarters-with-overlap-warning.png)
   >[!DNL Workfront]명의 고객에게만 분기 간 간격 및 중복이 허용됩니다.

1. (선택 사항 및 조건부) 회사에서 [!DNL Workfront Planning] 없이 [!DNL Workfront]만 구입한 경우 회계 분기를 참조하는 보고 요소를 만듭니다.

   **예:** [!UICONTROL 프로젝트] 목록에 대한 필터를 만들고 사용자 정의 분기를 참조하는 프로젝트의 계획된 완료 날짜를 포함합니다.

   ![사용자 지정 분기가 있는 프로젝트 필터](assets/example-of-project-filter-with-custom-quarters.png)

   &quot;이번 분기&quot;, &quot;다음 분기&quot; 및 &quot;지난 분기&quot;에 대한 참조가 사용자 정의 분기에 대한 새 참조로 대체됩니다.

   보고 요소에 대한 자세한 내용은 [보고 요소: 필터, 보기 및 그룹화](../../../reports-and-dashboards/reports/reporting-elements/reporting-elements-filters-views-groupings.md)를 참조하십시오.

   필터 만들기에 대한 자세한 내용은 [필터 만들기 또는 편집 [!DNL Adobe Workfront]](../../../reports-and-dashboards/reports/reporting-elements/create-filters.md)을 참조하세요.
1. (선택 사항 및 조건부) 회사에서 Workfront Planning을 구입하고 [!DNL Workfront Planning]에 대한 액세스 권한이 있는 경우 레코드 유형 페이지로 이동하여 타임라인 보기를 엽니다. 보기에 새 사용자 정의 분기가 표시됩니다.
자세한 내용은 [타임라인 보기 관리](/help/quicksilver/planning/views/manage-the-timeline-view.md)를 참조하십시오.

<!--
<div class="preview">

### Set up custom quarters for your [!DNL Workfront] system in the Preview environment

>[!NOTE]
>
>If your organization purchased a Planning package in addition to a Workflow package, or if they purchased  Workfront Planning as a standalone package, you can configure custom weeks, in addition to custom quarters. 
> 
>Custom weeks are not available for Workfront reports and lists. 

{{step-1-to-setup}}

1. Click **[!UICONTROL Custom Quarters]**.

1. Select **[!UICONTROL Enable Custom Quarters]**.

1. Type a name for the custom quarter. For example, "Fiscal Q1 2021."
1. Select start and end dates for the custom quarter.

1. (Optional) Select the **Starts a new custom week sequence** option. 

    When selected, this option sets the start of the custom quarter as the start of the first custom week of the quarter in the Planning timeline view. 
1. (Optional) In the **Custom week label format** area, choose the **Format** for the custom week labels. Choose from the following options:

    * **W1, W2, W3 ...** . This is the default format.
    * **FW1, FW2, FW3 ...**
    * **Week1, Week 2, Week 3, ...**
    * **Custom**

1. (Conditional) If you selected **Custom** for the **Format** field, type a **Custom label** to identify the custom weeks.  

    Custom weeks display in Planning timeline views. 

    >[!TIP]
    >
    >When adding a custom label, you can type up to 100 characters. 
    >
    >You may indicate the name of the first week, and the following weeks will use the same label followed by a sequential number. 
    >
    >For example, a **Custom label** of "Fiscal week" will add the labels of "Fiscal week 1, Fiscal week 2, Fiscal week 3 ..." to the rest of the weeks in the sequence. 

1. (Optional) Click **[!UICONTROL Add Custom Quarter]** to add additional custom quarters to the system.

      >[!IMPORTANT]
      >
      > If your company purchased [!DNL Workfront Planning], you cannot save your custom quarters if there are gaps or overlaps between the quarters. 
      >![Custom quarters with overlap warning](assets/custom-quarters-with-overlap-warning-red-outline.png)
      >Gaps and overlaps between the quarters are allowed for [!DNL Workfront] only customers. 

1. (Optional and conditional) To view the custom quarters in Workfront, create a reporting element that refers to the custom quarters.

   **Example:** Create a filter for a [!UICONTROL project] list and include the Planned Completion Date of a project referencing the custom quarters.

   ![Project filter with custom quarters](assets/example-of-project-filter-with-custom-quarters.png)

   The references to "This Quarter", "Next Quarter", and "Last Quarter" are replaced with new references to the custom quarters.

   For information about reporting elements, see [Reporting elements: filters, views, and groupings](../../../reports-and-dashboards/reports/reporting-elements/reporting-elements-filters-views-groupings.md).

   For information about creating filters, see [Create or edit filters in [!DNL Adobe Workfront]](../../../reports-and-dashboards/reports/reporting-elements/create-filters.md).
1. (Optional and conditional) To view custom quarters and weeks in Workfront Planning, go to a record type page and open a timeline view. The view displays the new custom quarters and weeks. 

For information, see [Manage the timeline view](/help/quicksilver/planning/views/manage-the-timeline-view.md). 

</div>
-->