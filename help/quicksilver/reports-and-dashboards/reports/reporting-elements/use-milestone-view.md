---
product-area: reporting
navigation-topic: reporting-elements
title: 마일스톤 보기 사용
description: 마일스톤 보기를 프로젝트 목록 또는 보고서에 적용할 수 있습니다. 마일스톤 보기를 사용하여 보고 있는 프로젝트 내에서 작업과 관련된 모든 마일스톤을 볼 수 있습니다.
author: Courtney, Alina
feature: Reports and Dashboards
exl-id: c55e53b5-5559-4b6a-a8d7-5028be6af30f
source-git-commit: d7af8c5888147e847b4e239b629373b4b72541f7
workflow-type: tm+mt
source-wordcount: '1420'
ht-degree: 1%

---

# 마일스톤 보기 사용

<!-- Audited: 11/2024 -->

<!--remove Preview and Production mentions from the article when this comes out live-->

<!--
<div class="preview"> 

The highlighted information on this page refers to functionality not yet generally available. It is available only in the Preview environment for all customers. The same features will also be available in the Production environment for all customers after a week from the Preview release.      

For more information, see [Interface modernization](/help/quicksilver/product-announcements/product-releases/interface-modernization/interface-modernization.md).  

</div> 
-->

마일스톤 보기를 프로젝트 목록 또는 보고서에 적용할 수 있습니다. 마일스톤 보기를 사용하여 보고 있는 프로젝트 내에서 작업과 관련된 모든 마일스톤을 볼 수 있습니다.

마일스톤 보기를 사용하려면 다음 요소가 있어야 합니다.

* 마일스톤 경로가 구성됩니다. 자세한 내용은 [마일스톤 경로 만들기](../../../administration-and-setup/customize-workfront/configure-approval-milestone-processes/create-milestone-path.md)를 참조하세요.
* 마일스톤 경로를 프로젝트에 추가해야 합니다. 자세한 내용은 [프로젝트 편집](/help/quicksilver/manage-work/projects/manage-projects/edit-projects.md)을 참조하세요.
* 이정표는 작업과 연결됩니다. 자세한 내용은 [작업과 마일스톤 연결](../../../manage-work/tasks/manage-tasks/associate-milestones-with-tasks.md)을 참조하세요.

마일스톤 보기는 프로젝트 목록이나 프로젝트 보고서를 볼 때 사용할 수 있습니다. 다음 섹션에서는 마일스톤 보기를 보고 사용하는 방법에 대해 설명합니다.

## 액세스 요구 사항

+++ 을 확장하여 이 문서의 기능에 대한 액세스 요구 사항을 봅니다.

이 문서의 단계를 수행하려면 다음 액세스 권한이 있어야 합니다.

<table style="table-layout:auto"> 
 <col> 
 </col> 
 <col> 
 </col> 
 <tbody> 
  <tr> 
   <td role="rowheader"><strong>Adobe Workfront 플랜</strong></td> 
   <td> <p>임의</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>Adobe Workfront 라이선스</strong></td> 
   <td> 
      <p>신규:</p>
         <ul>
         <li><p>표준</p></li>
         </ul>
      <p>현재:</p>
         <ul>
         <li><p>작업 이상</p></li>
         </ul>
   </td>
  </tr> 
  <tr> 
   <td role="rowheader"><strong>액세스 수준 구성*</strong></td> 
   <td> <p>보고서, 대시보드, 캘린더에 대한 보기 또는 상위 액세스 권한</p></td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>개체 권한</strong></td> 
   <td> <p>마일스톤 보기를 보고서에 적용하려면 프로젝트 보고서에 대한 권한을 봅니다.</p> </td> 
  </tr> 
 </tbody> 
</table>

이 표의 정보에 대한 자세한 내용은 [Workfront 설명서의 액세스 요구 사항](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)을 참조하십시오.

+++

## 마일스톤 보기로 전환 {#switch-to-the-milestone-view}

{{step1-to-projects}}

1. **보기** 드롭다운 메뉴를 클릭한 다음 **마일스톤**&#x200B;을 클릭합니다.

   목록 또는 보고서가 마일스톤 보기에 표시됩니다.

   마일스톤 보기에 대한 자세한 내용은 이 문서의 [마일스톤 보기 개요](#milestone-view-overview) 섹션을 참조하십시오.

## 마일스톤 보기 개요 {#milestone-view-overview}

마일스톤 보기는 프로젝트 목록 및 프로젝트 보고서에서 사용할 수 있습니다. 보고 있는 프로젝트 내의 작업과 관련된 모든 이정표를 빠르게 볼 수 있습니다.


>[!NOTE]
>
>다음 영역에서는 마일스톤 보기를 사용할 수 없습니다.
>
>* 타임시트, 프로젝트 추가 시 프로젝트 목록

마일스톤 보기로 전환하는 방법에 대한 자세한 내용은 이 문서의 [마일스톤 보기로 전환](#switch-to-the-milestone-view) 섹션을 참조하십시오.

<!--add new screen shot for preview or production release-->

마일스톤 보기가 있는 ![프로젝트](assets/project-with-milestone-view-with-complete.png)

### 마일스톤 보기 섹션

마일스톤 보기를 프로젝트 목록에 적용하면 프로젝트가 다음 섹션에 표시됩니다.

* 마일스톤 경로와 연관된 프로젝트가 먼저 해당 마일스톤 경로의 이름 아래에 나열됩니다.

  Workfront은 첫 번째 섹션의 프로젝트를 다음 기준에 따라 이 순서로 정렬합니다.

   1. 마일스톤 경로 ID. 마일스톤 경로 보고서에서 마일스톤 경로 ID를 볼 수 있습니다.

   2. 마일스톤 보기를 선택하기 전에 프로젝트 목록에 이전에 적용된 보기에서 프로젝트 목록의 첫 번째 정렬 필드로 선택된 필드입니다.

* 마일스톤 경로와 연관되지 않은 프로젝트가 미할당 섹션 옆에 표시됩니다. Workfront은 마일스톤 보기를 선택하기 전에 프로젝트 목록에 이전에 적용된 보기에서 프로젝트 목록의 첫 번째 정렬 필드로 선택된 필드를 기준으로 미할당 섹션의 프로젝트를 정렬합니다.

### 마일스톤 보기의 프로젝트 정보

마일스톤 보기에서 프로젝트 목록 또는 프로젝트 보고서를 볼 때 다음 정보를 사용할 수 있습니다.

* **계획된 일자 또는 예상 일자:** 마일스톤 보기에서 계획된 일자 또는 예상 일자를 표시할지 여부를 지정합니다.\
  프로젝트의 시작 및 완료 날짜와 마일스톤 경로의 각 마일스톤 작업의 완료 날짜에 대한 날짜가 표시됩니다.

  예상 일자를 보는 경우에는 일자를 편집할 수 없습니다. 예상 날짜는 Workfront에 의해 계산되며 수동으로 변경할 수 없습니다.

  계획된 일자를 보고 프로젝트에 대한 관리 액세스 권한도 있는 경우 마일스톤 보기에서 직접 다음 일자를 편집할 수 있습니다.

   * **프로젝트 시작 날짜:** 프로젝트가 시작 날짜부터 예약된 경우 프로젝트의 계획된 시작 날짜를 수동으로 변경할 수 있으며 계획된 완료 날짜가 계산됩니다.
   * **프로젝트 완료 일자:** 프로젝트가 계획된 완료 일자부터 예약된 경우 프로젝트의 계획된 완료 일자를 수동으로 변경할 수 있으며 계획된 시작 일자가 계산됩니다.
   * **작업 완료 날짜:** 마일스톤 보기에서 직접 작업의 계획된 완료 날짜를 수동으로 업데이트할 수 있습니다.

* **완료율:** 각 작업 및 프로젝트의 완료율을 표시합니다.

  이 문서의 [마일스톤 보기에 표시되는 정보 구성](#configure-what-information-displays-in-the-milestone-view) 섹션에 설명된 대로 완료 비율이 표시되지 않도록 할 수 있습니다.

  이 문서의 [마일스톤 보기에서 작업에 대한 완료율 조정](#adjust-percent-complete-for-tasks-in-the-milestone-view) 섹션에 설명된 대로 마일스톤 보기에서 직접 완료율을 조정할 수 있습니다.

* **작업 진행 상태 아이콘:** 마일스톤 보기에서 각 프로젝트 및 작업 옆에 상태 아이콘이 표시됩니다. <!--get new screen shots or hide them for preview or production - could not display all in devtest; idea: use color dots from Task Details tab - New status is blue; Some concerns condition is yellow etc-->

  <!--A progress status icon in the shape of a colored circle displays next to each project and task in the Milestone view. The possible statuses and circle colors are: 
   * On Time - green
   * Behind - yellow
   * At Risk - blue
   * Late - red-->


   * 정시\
     ![시간 아이콘](assets/gantt-ontime.png)

   * 지연됨\
     ![뒤로 아이콘](assets/gantt-behind.png)

   * 위험 상태\
     ![위험 상태 아이콘](assets/gantt-atrisk.png)

   * 지연\
     ![지연 아이콘](assets/gantt-late.png)

  이 문서의 [마일스톤 보기에 표시되는 정보 구성](#configure-what-information-displays-in-the-milestone-view) 섹션에 설명된 대로 이러한 상태 아이콘이 표시되지 않도록 할 수 있습니다.

  각 상태 유형에 대한 자세한 내용은 문서 [작업 진행 상태 개요](../../../manage-work/tasks/task-information/task-progress-status.md)를 참조하십시오.

* **완료된 작업에 대한 작업 상태 음영**: 작업이 완료로 표시된 후 작업이 정시에 완료되었는지 또는 늦게 완료되었는지 여부를 나타내는 마일스톤 보기에서 작업 배경이 음영으로 표시됩니다.

   * **작업 열의 빨간색 음영**: 진행 상태가 **지연**&#x200B;인 경우 작업 배경이 빨간색입니다.

   * **작업 열의 녹색 음영**: 진행 상태가 **설정 시간**&#x200B;일 때 작업 배경이 녹색입니다.

* **프로젝트 시작 및 완료 열에 대한 프로젝트 상태 음영**:

   * **프로젝트 시작 열**: 실제 시작 날짜가 채워진 경우에만 프로젝트 시작 열의 배경이 빨간색 또는 녹색입니다.

      * **프로젝트 시작 열의 빨간색 음영**: 프로젝트의 진행 상태가 **지연**&#x200B;인 경우 프로젝트 시작 열의 배경이 빨간색입니다.

      * **프로젝트 시작 열의 녹색 음영**: 프로젝트의 진행 상태가 **설정 시간**&#x200B;일 때 프로젝트 시작 열의 배경이 녹색입니다.

     >[!TIP]
     >
     >프로젝트의 실제 시작 일자를 보려면 프로젝트 세부 정보 페이지로 이동해야 합니다.

   * **프로젝트 완료 열**: 실제 완료 날짜가 채워진 경우에만 프로젝트 완료 열의 배경이 빨간색 또는 녹색으로 표시됩니다.

      * **프로젝트 완료 열의 빨간색 음영**: 프로젝트의 진행 상태가 **지연**&#x200B;인 경우 프로젝트 완료 열의 배경이 빨간색입니다.

      * **프로젝트 완료 열의 녹색 음영**: 프로젝트의 진행 상태가 **설정 시간**&#x200B;일 때 프로젝트 완료 열의 배경이 녹색입니다.

     >[!TIP]
     >
     >프로젝트의 실제 완료 일자를 보려면 프로젝트 세부 정보 페이지로 이동해야 합니다.

   * 작업의 진행 상태가 위험 또는 지연이면 시작 및 완료 열에 색상 음영이 할당되지 않습니다.

  <!--add new screen shot for preview or production release-->

  ![음영이 있는 마일스톤 보기](assets/milestone-view-with-shading.png)

* **프로젝트 이름**: 프로젝트 이름이 프로젝트에 대한 링크와 함께 표시됩니다.
* **프로젝트 상태 아이콘**: 프로젝트 이름 옆에 프로젝트의 상태를 나타내는 아이콘이 표시됩니다.

  <!--
   <div class="preview">
   A condition icon in the shape of a colored circle displays next to each project in the Milestone view. The possible project conditions and circle colors are: 
   * On Target - green
   * At Risk - yellow
   * In Trouble - red
   </div>
   -->

  프로젝트의 상태는 다음 중 하나일 수 있습니다.

   * 대상
   * 위험 상태
   * 문제 발생

## 마일스톤 보기에 표시되는 정보 구성 {#configure-what-information-displays-in-the-milestone-view}

마일스톤 보기에 다음 요소가 표시되는지 여부를 구성할 수 있습니다.

* 진행 상태 아이콘
* 프로젝트 및 작업 완료율

기본적으로 프로젝트 및 작업의 진행 상태 아이콘 및 완료율이 표시됩니다.

이러한 옵션에 대한 변경 내용은 귀하에게만 적용되며 다른 사용자는 영향을 받지 않습니다. 변경 사항은 다음에 Workfront에 로그인할 때 유지됩니다.

프로젝트의 프로젝트 상태 아이콘 및 완료 비율을 표시할지 여부를 구성하려면 다음 작업을 수행하십시오.

{{step1-to-projects}}

1. **보기** 드롭다운 메뉴를 클릭한 다음 **마일스톤**&#x200B;을 클릭합니다.
   <!--No longer available: If you are viewing a list of projects inside a Portfolio or a Program, select the **Milestone** subtab.  -->

1. &#x200B;<!--In the Production environment,--> 마일스톤 보기의 오른쪽 상단 모서리에서 **옵션**&#x200B;을 클릭합니다.

   <!--<div class="preview">In the Preview environment, select from the options in the next step, from the upper-right corner of the Milestone view.</div>-->

   <!--at Production release, replace this screen shot and adjust the Production/ Preview text above-->

   ![milestone_view_options.png](assets/milestone-view-options-350x141.png)

1. 다음 옵션 중에서 선택합니다.

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">진행 상태</td> 
      <td> <p>각 프로젝트 및 작업 옆에 진행 상태 아이콘을 표시하려면 이 옵션을 선택하십시오.</p> <p>이 옵션은 기본적으로 활성화되어 있습니다.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">완료율</td> 
      <td> <p>각 프로젝트 및 작업 옆에 완료율을 표시하려면 이 옵션을 선택합니다.</p> <p>이 옵션은 기본적으로 활성화되어 있습니다.</p> </td> 
     </tr> 
    </tbody> 
   </table>

## 마일스톤 보기에서 작업의 완료율 조정 {#adjust-percent-complete-for-tasks-in-the-milestone-view}

마일스톤 보기에서 작업에 대한 완료율을 조정할 수 있습니다. 상위 작업(하위 작업이 포함된 작업) 또는 프로젝트에 대해서는 완료율을 조정할 수 없습니다.

마일스톤 보기에서 작업에 대한 완료율을 조정하려면 다음을 수행합니다.

{{step1-to-projects}}

1. **보기** 드롭다운 메뉴를 클릭한 다음 **마일스톤**&#x200B;을 클릭합니다.

1. (조건부) 마일스톤 보기에 현재 완료율이 표시되지 않는 경우 이 문서의 [마일스톤 보기에 표시되는 정보 구성](#configure-what-information-displays-in-the-milestone-view)에 설명된 대로 작업 및 프로젝트의 완료율 보기를 활성화합니다.

1. &#x200B;<!--In the Production environment,--> 작업 아래의 완료 백분율을 클릭하고 새 백분율을 지정한 다음 Enter 키를 누릅니다.

   <!--<div class="preview">In the Preview environment, move the Percent Complete slide to the new percent complete to update it. </div>-->
