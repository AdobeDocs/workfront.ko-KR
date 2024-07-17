---
product-previous: workfront-goals
navigation-topic: goal-review-and-sections
title: Adobe Workfront 목표의 목표 목록에서 목표 관리
description: 귀하 또는 다른 사용자가 목표를 만든 후 목표 목록에서 진행 상황과 정보를 검토할 수 있습니다. 목표 만들기에 대한 자세한 내용은 Adobe Workfront 목표에서 목표 만들기 를 참조하십시오.
author: Alina
feature: Workfront Goals
exl-id: 2a2c1240-f796-4cb8-b8a6-2ad5853916b9
source-git-commit: 024c612d46848c55529e902a00d481588d261584
workflow-type: tm+mt
source-wordcount: '819'
ht-degree: 2%

---

# Adobe Workfront 목표의 목표 목록에서 목표 관리

<!-- printing or exporting goals is no longer possible, but see if they add it later-->

귀하 또는 다른 사용자가 목표를 만든 후 목표 목록에서 진행 상황과 정보를 검토할 수 있습니다. 목표 만들기에 대한 자세한 내용은 [Adobe Workfront 목표에서 목표 만들기](../../workfront-goals/goal-management/create-goals.md)를 참조하십시오.

## 액세스 요구 사항

이 문서에 설명된 작업을 수행하려면 다음 액세스 권한이 있어야 합니다.

<table style="table-layout:auto">
<col>
</col>
<col>
</col>
<tbody>
 <tr> 
   <td role="rowheader">Adobe Workfront 플랜*</td> 
   <td> 
   <p>새 플랜 및 라이선스 구조의 경우:
  <ul><li>궁극적인 플랜 </li>
  또는
  <li>Prime 또는 Select Adobe Workfront 플랜에 대한 Adobe Workfront Goals에 대한 추가 라이센스입니다. </li></ul> </p>
<p>현재 플랜 및 라이선스 구조의 경우: 
<ul><li> Pro 이상 </li>
  <li>Workfront 라이선스 외에 Adobe Workfront Goals 라이선스.</li></ul></p>
   </td> 
  </tr>
 <tr>
 <td role="rowheader">Adobe Workfront 라이센스*</td>
 <td>
 <p>새 라이선스: 기여자 이상</p>
 또는
 <p>현재 라이선스: 요청 이상</p> <p>자세한 내용은 <a href="../../administration-and-setup/add-users/access-levels-and-object-permissions/wf-licenses.md" class="MCXref xref">Adobe Workfront 라이선스 개요</a>를 참조하십시오.</p> </td>
 </tr>
 <tr>
 <td role="rowheader">제품*</td>
 <td>
 <p> 다음 중 하나인 새 제품 요구 사항: </p>
<ul>
<li>Select 또는 Prime Adobe Workfront 플랜 및 추가 Adobe Workfront Goals 라이선스.</li>
<li>기본적으로 Workfront 목표를 포함하는 Ultimate Workfront 계획입니다. </li></ul>
 <p>또는</p>
 <p>현재 제품 요구 사항: Workfront 플랜 및 Adobe Workfront 목표에 대한 추가 라이선스. </p> <p>자세한 내용은 <a href="../../workfront-goals/goal-management/access-needed-for-wf-goals.md" class="MCXref xref">Workfront 목표를 사용하기 위한 요구 사항</a>을 참조하십시오. </p> </td>
 </tr>
 <tr>
 <td role="rowheader">액세스 수준</td>
 <td> <p>목표에 대한 액세스 편집</p>  </td>
 </tr>
 <tr data-mc-conditions="">
 <td role="rowheader">개체 권한</td>
 <td>
  <div>
  <p>목표에 대한 또는 그 이상의 권한에 대한 보기</p>
  <p>편집할 목표에 대한 권한 관리</p>
  <p>목표 공유에 대한 자세한 내용은 <a href="../../workfront-goals/workfront-goals-settings/share-a-goal.md" class="MCXref xref">Workfront 목표에서 목표 공유</a>를 참조하십시오. </p>
  </div> </td>
 </tr>
 <tr>
   <td role="rowheader"><p>레이아웃 템플릿</p></td>
   <td> <p>Workfront 관리자를 포함한 모든 사용자에게 메인 메뉴의 목표 영역을 포함하는 레이아웃 템플릿을 할당해야 합니다. </p>  
</td>
  </tr>
</tbody>
</table>

*자세한 내용은 [Workfront 설명서의 액세스 요구 사항](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)을 참조하십시오.

## 목표 목록의 목표 관리

Workfront 목표의 다음 섹션에서 목표를 보고 관리할 수 있습니다.

* 목표 목록
* 목표 정렬

각 섹션에는 목표가 약간 다른 형식으로 표시됩니다. 사용할 섹션은 목표 작업을 수행할 때 달성하고자 하는 목적에 따라 다릅니다.

자세한 내용은 [Adobe Workfront 목표 섹션 개요](../../workfront-goals/goal-review-and-workfront-goals-sections/overview-of-wf-goals-sections.md)를 참조하십시오.

이 문서에서는 목표 목록에서 목표를 검토하는 방법을 설명합니다.

목표 목록을 검토할 때 다음 사항을 고려하십시오.

* 나 또는 조직의 다른 사람이 목표 목록에서 만든 목표를 볼 수 있습니다. 목표를 편집하려면 목표에 대한 관리 권한이 있어야 합니다.

<!--

### Manage the Goal List in the Production environment

1. Click the **Main Menu** icon ![](assets/main-menu-icon.png) in the upper-right corner, then click **Goals**.

   (!-- Add this when Shell is available to all: or (if available), click the **Main Menu** icon ![Main menu icon](../goal-review-and-workfront-goals-sections/assets/three-line-main-menu-icon.png) in the upper-left corner)
   --)

   The Goal List section displays by default. You can view goals regardless of their status, period, or owner, by default.

   The list of goals contains the following columns with information about each goal, result, or activity: 

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader"> 
       <div> 
        <p role="rowheader">Name </p> 
       </div> </td> 
      <td>The name of the goal, result, or activity.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Owner</td> 
      <td>The name of the goal, result, or activity owner. </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Period</td> 
      <td>The time period for which the goal is scheduled.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Progress </td> 
      <td> <p>The progress indicator for the goal includes the following:</p> 
       <ul> 
      <li> <p>The progress label. </p> <p>For information, see <a href="../../workfront-goals/goal-management/calculate-goal-progress.md" class="MCXref xref">Overview of goal progress and condition in Adobe Workfront Goals</a>. </p> </li> 
      <li> <p>The percent complete of the goal, activity, or result. </p> </li> 
       </ul> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"> <p>Status (includes alignment icon)</p> <p> <img src="assets/alignment-icon-large.png"> </p> </td> 
      <td> <p>The status of the goal which can be one of the following:</p> 
       <ul> 
        <li>Active</li> 
        <li>Draft</li> 
        <li>Inactive</li> 
        <li>Closed</li> 
       </ul> <p>For information about goal status, see <a href="../../workfront-goals/goal-management/goal-status-overview.md" class="MCXref xref">Goal status overview in Adobe Workfront Goals</a>. </p> <p>The alignment icon appears on goals that are aligned to other goals. For information about aligning goals, see <a href="../../workfront-goals/goal-alignment/align-goals-by-connecting-them.md" class="MCXref xref">Align goals by connecting them in Adobe Workfront Goals</a>.</p> </td> 
     </tr> 
    </tbody> 
   </table>

1. Use the filters in the upper-right corner of the goal list to select only goals that are important to you. For information about using filters in Workfront Goals, see [Filter information in Adobe Workfront Goals](../../workfront-goals/goal-management/filter-information-wf-goals.md)
1. Click any of the fields in the column headers to sort it by that field.

   An arrow displays to the right of the field by which the list is sorted.

   ![](assets/goal-list-with-goal-expanded-+-result-+-activity-350x117.png)

1. (Optional) Click the field in the column again to sort the same column in a descending order. 
1. Click the right-pointing arrow to the left of the goal name to expand a goal

   Or

   Click the right-pointing arrow ![](assets/right-pointing-arrow.png) in the header of the list to expand all the goals in the list and view additional information about each goal, including any of the following:

   * Results names, owners, and progress

     For information about results, see [Add results to goals in Adobe Workfront Goals](../../workfront-goals/results-and-activities/add-results-to-goals.md).
   
   * Activity names, owners, and progress

     For information about activities, see [Add activities to goals in Adobe Workfront Goals](../../workfront-goals/results-and-activities/add-activities-to-goals.md).

1. Click the name of a goal to open the **Goal Details** panel on the right and review more information about the goal as well as manage it. For information about reviewing individual goals, see [Update goals in the Goal details section in Adobe Workfront Goals](../../workfront-goals/goal-management/update-goals-in-goal-details-panel.md).
1. (Optional) Expand the **Goals per page** drop-down menu and select from the following options to display additional goals:

   * 20  
      
      This is the default selection. 
   * 50
   * 100

1. Click **Print** to export a list of goals, results, and activities to a .pdf file.

   >[!TIP]
   >
   >* When printing a list of goals, the file produced contains only the information displayed on the screen. Items eliminated by filtering a list of goals do not display in the .pdf file.
   >* When you do not expand the goals in the list before printing the list, the .pdf file displays only goals without their results and activities.

   For more information, see [Print the Goal List in Adobe Workfront Goals](../../workfront-goals/goal-management/print-the-goal-list.md). 

1. Click the **Alignment icon** ![](assets/align-icon.png) next to an aligned to open the goal's card in the Goal Alignment section. For more information, see [Navigate the Goal Alignment section in Adobe Workfront Goals](../../workfront-goals/goal-alignment/navigate-goal-alignment-chart.md).
-->

목표 목록에서 목표를 관리하려면 다음을 수행하십시오.

1. 오른쪽 상단의 **주 메뉴** 아이콘 ![](assets/main-menu-icon.png)을(를) 클릭한 다음 **목표**&#x200B;를 클릭합니다.

   <!-- Add this when Shell is available to all: or (if available), click the **Main Menu** icon ![Main menu icon](../goal-review-and-workfront-goals-sections/assets/three-line-main-menu-icon.png) in the upper-left corner)
   -->

   기본적으로 목표 목록 섹션이 표시됩니다. 기본적으로 상태, 기간 또는 소유자에 관계없이 목표를 볼 수 있습니다.

   목표 목록에는 각 목표에 대한 정보와 함께 다음 필드가 포함되어 있습니다.

   * **이름**: 목표의 이름입니다.
   * **소유자**: 목표 소유자의 이름입니다.
   * **기간**: 목표가 예약되는 기간입니다.
   * **상태**: 목표의 상태는 다음 중 하나일 수 있습니다.
      * 활성
      * 초안
      * 비활성
      * 마감됨

     목표 상태에 대한 자세한 내용은 [Adobe Workfront 목표의 목표 상태 개요](../goal-management/goal-status-overview.md)를 참조하십시오.

     정렬 아이콘은 다른 목표에 정렬된 목표에 표시됩니다. 목표 정렬에 대한 자세한 내용은 [Adobe Workfront 목표에서 연결하여 목표 정렬](../goal-alignment/align-goals-by-connecting-them.md)을 참조하십시오.

   * **조건**: 목표를 완료하는 데 할당된 기간 내에 목표가 어떻게 진행되고 있는지 시각적으로 표시합니다.

     목표의 조건은 다음 중 하나일 수 있습니다.

      * 신규
      * 대상
      * 위험 상태
      * 문제 발생

     목표 조건에 대한 자세한 내용은 [Adobe Workfront 목표의 목표 진행 상황 및 상태 개요](../goal-management/calculate-goal-progress.md)를 참조하십시오.

   * **진행**: 목표의 진행 표시기를 백분율 값으로 사용합니다. 진행 표시기의 색상이 목표 조건의 색상과 일치합니다.

     자세한 내용은 [Adobe Workfront 목표의 목표 진행률 계산](../goal-management/calculate-goal-progress.md)을 참조하십시오.

1. 목표 목록의 오른쪽 상단에 있는 필터 아이콘 ![](assets/filter-icon.png)을(를) 클릭하고 필터를 적용하여 중요한 목표만 표시합니다.

   Workfront 목표에서 필터를 사용하는 방법에 대한 자세한 내용은 [Adobe Workfront 목표의 필터 정보](../goal-management/filter-information-wf-goals.md)를 참조하십시오.

1. 해당 필드를 기준으로 목록을 정렬하려면 열 머리글에 있는 필드를 클릭하십시오.
목록이 정렬되는 기준 필드 오른쪽에 화살표가 표시됩니다.

1. (선택 사항) 동일한 열을 내림차순으로 정렬하려면 열의 필드를 다시 클릭합니다.
1. 목표의 이름을 클릭하여 목표의 페이지를 엽니다.
1. 목록에서 목표를 한 개 선택한 다음 목록 맨 위에서 다음 옵션 중 하나를 클릭합니다.
   * 목표에 대한 정보를 편집하려면 **편집** 아이콘 ![](assets/edit-icon.png)을(를) 사용하십시오. 자세한 내용은 [Adobe Workfront 목표의 목표 편집](../goal-management/edit-goals.md)을 참조하십시오.
   * **공유** 아이콘 ![](assets/share-icon.png)을(를) 통해 다른 사람과 목표를 공유할 수 있습니다. 자세한 내용은 [Adobe Workfront 목표에서 목표 공유](../workfront-goals-settings/share-a-goal.md)를 참조하십시오.
   * **정렬 열기** 아이콘 ![](assets/align-icon-unshimmed.png)을 클릭하여 목표 정렬 영역을 엽니다. 이 옵션은 선택한 목표가 다른 목표에 맞춰진 경우에만 표시됩니다.
   * **삭제** 아이콘 ![](assets/delete-icon.png)을(를) 클릭하여 목표를 삭제한 다음 **삭제**&#x200B;를 클릭하여 확인합니다.  자세한 내용은 [Adobe Workfront 목표에서 목표 삭제 및 비활성화](../goal-management/delete-and-deactivate-goals.md)를 참조하십시오.





