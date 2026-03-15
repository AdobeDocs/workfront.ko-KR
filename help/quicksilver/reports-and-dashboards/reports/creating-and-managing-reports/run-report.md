---
product-area: reporting
navigation-topic: create-and-manage-reports
title: 보고서 실행
description: You can run any report that you have access to View.
author: Courtney
feature: Reports and Dashboards
exl-id: bd2202a7-040c-4291-ad02-ba8929a37e2b
source-git-commit: 6a6d3d47ed5741e3202c44b7240a2e67b687ea95
workflow-type: tm+mt
source-wordcount: '497'
ht-degree: 4%

---


# 보고서 실행

보기에 액세스할 수 있는 모든 보고서를 실행할 수 있습니다.

<!-- Audited: 11/2024 -->

<!--
NOTE: ***Linked to Getting Started with Reporting.***This information is obsolete, because asynchronous timeline is not enabled for all customers (used to be included in the "Viewing a Cached Report" section): Some reports in Workfront can take a significant time to load. If your report takes longer than 30 seconds to load, your report is cached after it is finished loading, and a message is displayed in the upper-right corner of the page indicating that the report being viewed is a saved report from a specific time.

After a report is cached, it is available for the next 12 hours. Any user who runs the report (as described in "Running a Report") sees the cached report.)
-->

## 액세스 요구 사항

+++ 이 문서의 기능에 대한 액세스 요구 사항을 보려면 확장하십시오. 

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront 패키지</td> 
   <td> <p>Any</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront 라이선스</td> 
   <td> 
      <p>표준</p>
      <p>플랜</p>
   </td>
  </tr> 
  <tr> 
   <td role="rowheader">액세스 수준 구성</td> 
   <td> <p>View access to Reports, Dashboards, Calendars</p></td> 
  </tr> 
  <tr> 
   <td role="rowheader">개체 권한</td> 
     <td> <p>보고서에 대한 권한 보기</p></td> 
  </tr> 
 </tbody> 
</table>

이 표의 정보에 대한 자세한 내용은 [Workfront 설명서의 액세스 요구 사항](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)을 참조하십시오.

+++

## 보고서 실행

1. Adobe Workfront의 오른쪽 상단에 있는 **[!UICONTROL 주 메뉴]** 아이콘 ![주 메뉴](/help/_includes/assets/main-menu-icon.png)을 클릭하거나(가능한 경우) 왼쪽 상단에 있는 **[!UICONTROL 주 메뉴]** 아이콘 ![주 메뉴](/help/_includes/assets/main-menu-icon-left-nav.png)을 클릭한 다음 **[!UICONTROL 보고서]**&#x200B;를 클릭합니다.

1. 다음 옵션 중에서 선택합니다.

   * **My Reports:** Reports that you have created.
   * **Shared With Me:** Reports that other users have shared with you.
   * **All Reports:** All reports in the system that you have access to.

1. Click the name of the report that you want to run.\
   또는\
   프롬프트를 사용하여 보고서를 만든 경우 드롭다운 메뉴에서 적절한 정보를 선택한 다음 **보고서 실행**&#x200B;을 클릭합니다.\
   프롬프트에 대한 자세한 내용은 [보고서에 프롬프트 추가](../../../reports-and-dashboards/reports/creating-and-managing-reports/add-prompt-report.md)를 참조하십시오.\
   보고서의 콘텐츠는 보고서를 실행한 사용자의 컨텍스트에서 보고서를 실행한 날짜, 시간 및 시간대를 포함하는 타임스탬프와 함께 보고서의 오른쪽 위 모서리에 표시됩니다.

1. (Optional) Click the **Reload icon** ![Reload icon](assets/unshimmed-report-refresh-icon.png) to refresh the results in a report if the report has been displayed in your browser for a while.

1. (Conditional) If the report uses filters or prompts, click **Show Filters and Prompts** to display a list of filters and prompts that are being used on the report you are viewing. If the report contains only filters or only prompts, **Show Filters** or **Show Prompts** appears instead.

   ![Show filters and prompts](assets/unshimmed-show-filters-and-prompts.png)

   Information displays below the report name on the left side of the page. For prompts, this is information about the prompt selections made at the time the report was run, as described in Step 3.

1. If you are using Custom Prompts, they do not display. Only the system prompts display. Custom Filters always display.

## 캐시된 보고서 보기

보고서가 잠시 동안 브라우저에 표시되면 캐시될 수 있습니다. 다음 작업을 수행하면 캐시된 보고서가 다시 로드됩니다.

* 보고서 설정을 편집하고 보고서를 저장합니다.
* Change the View, Group, or Filter.
* Click the **Reload icon** ![Reload icon](assets/unshimmed-report-refresh-icon.png)
This option is available in the upper-right corner of the page within the message box that indicates the time that the report was saved, or it is available in the upper-right corner of the dashboard that the report is placed on. For more information about reloading dashboards, see the section &quot;Display Dashboards&quot; in the article [Get started with dashboards](../../../reports-and-dashboards/dashboards/understanding-dashboards/get-started-dashboards.md).

* Access any page of the report beyond the first page by navigating to the Summary, Matrix, or Chart tabs.
