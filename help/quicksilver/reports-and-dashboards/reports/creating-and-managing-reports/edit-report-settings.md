---
product-area: reporting
navigation-topic: create-and-manage-reports
title: 보고서 설정 편집
description: 보고서의 설정을 편집하여 다른 사용자에게 표시되는 방법이나 사용자가 보고서를 실행하기 전에 어떤 정보를 묻는 메시지를 표시할 수 있는지 정의할 수 있습니다.
author: Courtney
feature: Reports and Dashboards
exl-id: 6fbbc557-65da-4ffe-968a-9c8db6a45811
source-git-commit: 6a6d3d47ed5741e3202c44b7240a2e67b687ea95
workflow-type: tm+mt
source-wordcount: '612'
ht-degree: 9%

---

# 보고서 설정 편집

<!-- Audited: 11/2024 -->

보고서의 설정을 편집하여 다른 사용자에게 표시되는 방법이나 사용자가 보고서를 실행하기 전에 어떤 정보를 묻는 메시지를 표시할 수 있는지 정의할 수 있습니다.

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
   <td> <p>보고서, 대시보드, 캘린더에 대한 액세스 편집</p> <p>필터, 보기, 그룹화에 대한 액세스 편집</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">개체 권한</td> 
 <td> <p>보고서에 대한 권한 관리</p></td>  
  </tr> 
 </tbody> 
</table>

이 표의 정보에 대한 자세한 내용은 [Workfront 설명서의 액세스 요구 사항](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)을 참조하십시오.

+++

## 방법 단계

1. Start creating a report by going to the **Main menu** > **Reports**, then select the object of your report.

   또는

   Open an existing report, then click **Report Actions** > **Edit**.

1. Click **Report Settings** in the upper-right corner of the report builder.
1. Configure the following report settings:

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">보고서 제목</td> 
      <td>보고서 제목을 지정합니다.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">설명</td> 
      <td>보고서의 목적 및 용도를 설명하는 문을 지정합니다.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Run this report with the Access Rights of</td> 
      <td>Select the user whose access rights you want this report to use when displaying for other users. For more information about running a report with the access rights of another user, see the article <a href="../../../reports-and-dashboards/reports/creating-and-managing-reports/run-deliver-report-access-rights-another-user.md" class="MCXref xref">Run and deliver a report with the access rights of another user</a>.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">When the Report loads, show the</td> 
      <td>Select the default tab that is displayed for all users when the report loads.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">When the report loads on a dashboard, show ... items</td> 
      <td>Specify the number of items that are displayed for all users when the report loads on a dashboard. 기본값은 15개 항목이며 최대 항목 수는 200개입니다.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">세부 정보 탭에서 리소스 그리드 보기 표시</td> 
      <td> <p>(사용자 보고서만 해당) 이 옵션을 선택하면 보고서의 세부 정보 탭에 리소스 그리드가 표시됩니다.</p> <p>참고: 사용자 보고서에 리소스 그리드 보기를 적용하면 보고서에는 현재 상태에 있는 프로젝트만 표시됩니다. 다른 상태에서 프로젝트를 보려면 전역 탐색 막대의 사람 영역에서 사용자 활용성 탭을 사용하여 리소스 그리드 보기를 적용할 수 있습니다. <!--
         <MadCap:conditionalText data-mc-conditions="QuicksilverOrClassic.Draft mode">
          For more information about using the Resource Grid, see the article Overview of the Resource Grid . (drafted because this article is drafted also: Article is in draft Feb 1, 2021)
         </MadCap:conditionalText>
        --></p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Show a special view on the Details tab</td> 
      <td>(Project Report Only) Specify the type of view users will see when they access this information on the Details tab. For example, you can select a Milestone or Gantt view.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">기본으로 간트 보기에서 이 보고서 표시</td> 
      <td>(Project Report and Task Report Only) Select this option to have the Gantt view automatically enabled when users view the Details tab in this report.<br>For more information about viewing the Gantt chart in project reports and task reports, see the section "View task information in the project list Gantt Chart" in the article <a href="../../../manage-work/gantt-chart/use-the-gantt-chart/view-info-in-gantt.md" class="MCXref xref">View information in the Gantt Chart </a>.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">보고서에서 보기 변경 가능</td> 
      <td>Select this option to allow users to change the View when running the report.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">보고서에서 그룹 변경 가능</td> 
      <td>보고서를 실행할 때 사용자가 그룹을 변경할 수 있도록 하려면 이 옵션을 선택하십시오.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">보고서에서 필터를 변경할 수 있도록 허용</td> 
      <td>사용자가 보고서를 실행할 때 필터를 변경할 수 있도록 하려면 이 옵션을 선택합니다.</td> 
     </tr> 
    </tbody> 
   </table>

1. Click **Report Prompts** to set up any prompts for the report.\
   보고서에 프롬프트를 추가하는 방법에 대한 자세한 내용은 문서 [보고서에 프롬프트 추가](../../../reports-and-dashboards/reports/creating-and-managing-reports/add-prompt-report.md)를 참조하십시오.

1. **완료,**&#x200B;를 클릭한 다음 **저장 + 닫기**&#x200B;를 클릭합니다.

## 추가 정보

다음도 참조하십시오.

<!--outdated: * [Basic Report Creation Program for the new Workfront experience](https://one.workfront.com/s/basic-report-creation-program) -->
* [보고서 시작](../../../reports-and-dashboards/reports/reporting/get-started-reports-workfront.md)
* [Use Adobe Workfront built-in reports](../../../reports-and-dashboards/reports/using-built-in-reports/use-workfront-built-in-reports.md)
* [사용자 지정 보고서 만들기](../../../reports-and-dashboards/reports/creating-and-managing-reports/create-custom-report.md)
