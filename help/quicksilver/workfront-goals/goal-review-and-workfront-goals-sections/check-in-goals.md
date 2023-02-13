---
product-previous: workfront-goals
navigation-topic: goal-review-and-sections
title: Adobe Workfront 목표에서 목표 진행 상태 업데이트
description: 목표를 주기적으로 검토하고 목표를 달성하지 못할 위험에 빠지지 않도록 진행 상황을 업데이트해야 합니다.
author: Alina
feature: Workfront Goals
exl-id: 5092f508-e52c-4934-a8c1-d0be04ecce13
source-git-commit: afc2124a7fd0d9d52c04be1c174fdba314beec7a
workflow-type: tm+mt
source-wordcount: '659'
ht-degree: 0%

---

# Adobe Workfront 목표에서 목표 진행 상태 업데이트

목표를 주기적으로 검토하고 목표를 달성하지 못할 위험에 빠지지 않도록 진행 상황을 업데이트해야 합니다.

<!--And: take this last sentence ^^ out when you update this for goal redesign production.-->

## 액세스 요구 사항

<!--drafted for P&P release:

You must have the following: 

<table style="table-layout:auto">
 <col>
 </col>
 <col>
 </col>
 <tbody>
  <tr>
   <td role="rowheader">Adobe Workfront plan*</td>
   <td>
   <p>Current plan: Select or higher</p>
   Or
   <p>Legacy plan: Pro or higher</p>
   
   </td>
  </tr>
  <tr>
   <td role="rowheader">Adobe Workfront license*</td>
   <td>
   <p>Current license: Contributor or higher</p>
   Or
   <p>Legacy license: Request or higher</p> <p>For more information, see <a href="../../administration-and-setup/add-users/access-levels-and-object-permissions/wf-licenses.md" class="MCXref xref">Adobe Workfront licenses overview</a>.</p> </td>
  </tr>
  <tr>
   <td role="rowheader">Product</td>
   <td>
   <p> Current product requirement: If you have the Select or Prime Adobe Workfront plan, you must also buy an additional Adobe Workfront Goals license.  Workfront Goals are included in the Ultimate Workfront Plan.</p>
   Or
   <p>Legacy product requirement: You must purchase an additional license for the Adobe Workfront Goals to access functionality described in this article. </p> <p>For information, see <a href="../../workfront-goals/goal-management/access-needed-for-wf-goals.md" class="MCXref xref">Requirements to use Workfront Goals</a>. </p> </td>
  </tr>
  <tr>
   <td role="rowheader">Access level*</td>
   <td> <p>Edit access to Goals</p> <p><b>NOTE</b><p>If you still don't have access, ask your Workfront administrator if they set additional restrictions in your access level. For information on how a Workfront administrator can change your access level, see:</p>
     <ul>
      <li> <p><a href="../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Create or modify custom access levels</a> </p> </li>
      <li> <p><span href="../../administration-and-setup/add-users/configure-and-grant-access/grant-access-goals.md"><a href="../../administration-and-setup/add-users/configure-and-grant-access/grant-access-goals.md" class="MCXref xref">Grant access to Adobe Workfront Goals</a></span> </p> </li>
     </ul> </p> </td>
  </tr>
  <tr data-mc-conditions="">
   <td role="rowheader">Object permissions</td>
   <td>
    <div>
     <p>View or higher permissions to the goal to view it</p>
     <p>Manage permissions to the goal to edit it</p>
     <p>For information about sharing goals, see <a href="../../workfront-goals/workfront-goals-settings/share-a-goal.md" class="MCXref xref">Share a goal in Workfront Goals</a>. </p>
    </div> </td>
  </tr>
 </tbody>
</table>

-->

다음 항목이 있어야 합니다.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront 플랜*</td> 
   <td> <p>Pro 이상</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront 라이선스*</td> 
   <td> <p>요청 이상</p> <p>자세한 내용은 <a href="../../administration-and-setup/add-users/access-levels-and-object-permissions/wf-licenses.md" class="MCXref xref">Adobe Workfront 라이선스 개요</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">제품</td> 
   <td> <p>이 문서에 설명된 기능에 액세스하려면 Adobe Workfront 목표에 대한 추가 라이센스를 구매해야 합니다. </p> <p>자세한 내용은 <a href="../../workfront-goals/goal-management/access-needed-for-wf-goals.md" class="MCXref xref">Workfront 목표 사용 요구 사항</a>. </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">액세스 수준 구성*</td> 
   <td> <p>목표 이상에 대한 액세스 편집</p> <p><b>메모</b><p>여전히 액세스 권한이 없는 경우 Workfront 관리자에게 액세스 수준에서 추가 제한 사항을 설정하는지 문의하십시오. Workfront 관리자가 액세스 수준을 변경하는 방법에 대한 자세한 내용은 다음을 참조하십시오.</p> 
     <ul> 
      <li> <p><a href="../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">사용자 정의 액세스 수준 만들기 또는 수정</a> </p> </li> 
      <li> <p><span href="../../administration-and-setup/add-users/configure-and-grant-access/grant-access-goals.md"><a href="../../administration-and-setup/add-users/configure-and-grant-access/grant-access-goals.md" class="MCXref xref">Adobe Workfront 목표에 대한 액세스 권한 부여</a></span> </p> </li> 
     </ul> </p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader">개체 권한</td> 
   <td> 
    <div> 
     <p>목표에 대한 권한 관리</p> 
     <p>목표 공유에 대한 자세한 내용은 <a href="../../workfront-goals/workfront-goals-settings/share-a-goal.md" class="MCXref xref">Workfront 목표에서 목표 공유</a>. </p> 
    </div> </td> 
  </tr> 
 </tbody> 
</table>

*보유하고 있는 플랜, 라이선스 유형 또는 액세스를 알아보려면 Workfront 관리자에게 문의하십시오.

## 전제 조건

시작하려면 먼저 다음을 수행해야 합니다.

* 기본 메뉴의 목표 영역을 포함하는 레이아웃 템플릿.
* 능동적인 목표. 초안, 비활성 또는 닫힌 목표에 대한 진행 상황을 업데이트할 수 없습니다.

## 목표 업데이트를 위한 고려 사항

목표에 대한 진행 상황을 업데이트할 때는 다음 사항을 고려하십시오.

* Workfront 목표는 목표 진행 상태 표시기의 진행 상황을 업데이트할 때 자동으로 목표 진행 상황을 계산합니다.

   >[!TIP]
   >
   >목표에 대한 진행 상황을 직접 업데이트할 수는 없습니다. 목표의 진행 상태 지표(활동, 결과, 연결된 프로젝트)의 진행 상황을 업데이트해야 목표의 진행 상태가 업데이트됩니다. 프로젝트의 진행 상태를 업데이트하려면 프로젝트의 작업을 업데이트해야 합니다.

   다음 문서를 참조하십시오.

   * 목표에 활동 추가에 대한 자세한 내용은 [Adobe Workfront 목표의 목표에 활동 추가](../../workfront-goals/results-and-activities/add-activities-to-goals.md).
   * 목표에 결과 추가에 대한 자세한 내용은 [Adobe Workfront 목표에 결과 추가](../../workfront-goals/results-and-activities/add-results-to-goals.md).
   * Workfront 목표가 목표에 대한 진행 상황을 계산하는 방법에 대한 자세한 내용은 다음을 참조하십시오 [Adobe Workfront 목표의 목표 진행 및 조건 개요](../../workfront-goals/goal-management/calculate-goal-progress.md).

* 진행 상황을 업데이트하려면 먼저 목표를 만들고 이를 활성화해야 합니다.

   다음 문서를 참조하십시오.

   * 목표 만들기에 대한 내용은 [Adobe Workfront 목표에서 목표 만들기](../../workfront-goals/goal-management/create-goals.md).
   * 목표 활성화에 대한 자세한 내용은 [Adobe Workfront 목표에서 목표 활성화](../../workfront-goals/goal-management/activate-goals.md).

   >[!IMPORTANT]
   >
   >초안, 종료 또는 비활성 상태의 목표 진행 상태는 업데이트할 수 없습니다.

* 사용자나 다른 사람이 목표에 대한 결과 또는 활동의 진행 상황을 처음 업데이트하면 새 목표와 Workfront 목표에 대한 진행 상태 업데이트 및 진행 상태 업데이트를 목표에 기록하기 시작합니다.

<!--

## Update goal progress by using Check-in in the Production environment

>[!IMPORTANT]
>
> <span class="preview"> The Check-in functionality has been removed from the Preview environment and will be removed from Workfront Goals with the 23.1 release. See the [Update goal progress in the Preview environment](#update-goal-progress-in-the-preview-environment) section in this article to update goal progress in Preview. </span>


You can check in on goals at the individual goal level, or you can check in on multiple goals from the Check-in section of Workfront Goals.

* [Update individual goals](#update-individual-goals) 
* [Update goals in the Check-in section](#update-goals-in-the-check-in-section)

### Update individual goals {#update-individual-goals}

When you check in on a goal at the goal level, you can update the progress of the results and activities that are assigned to you or other users.

For information about how to update additional information about results and activities, see [Edit results and activities in Adobe Workfront Goals](../../workfront-goals/results-and-activities/edit-results-and-activities.md).

1. Click the **Main Menu** icon ![](assets/main-menu-icon.png) > **Goals** in the upper-right corner.

   (!-- Add this when Shell is available to all: or (if available), click the **Main Menu** icon ![Main menu icon](../goal-review-and-workfront-goals-sections/assets/three-line-main-menu-icon.png) in the upper-left corner)
   --)

   This opens the Workfront Goals area.

   All goals display by default. 

1. (Optional) Click any of the following sections in the left panel to access a list of goals:

   * Goal Alignment 
   * Pulse 
   * Check-in

   Or

   From the Goal List, click the name of a goal to open the **Goal Details** panel on the right.

   >[!TIP]
   >
   >You must have Edit access to Goals in your Access Level to view the Check-in section or the Check in button.

1. Click **Check in**.

   ![](assets/check-in-link-inside-goal-details-highlighted-350x156.png)

   The progress of results and activities becomes editable.

1. Update the current progress on each of the results. Depending on what type of result you selected, you can do one of the following:

   * Update the quantity 
   * Update the currency amount
   * Update the percent complete

1. Update the percent complete on the Manual progress bar activity.

   >[!TIP]
   >
   >When you add projects as activities to your goals, you cannot manually update projects at the goal level. Workfront automatically updates project progress based on the project of their tasks. When the project percent complete updates in Workfront, the goal progress associated with the project also updates automatically.

1. Click **Back to Summary** to return to the Goal Details panel.

   Your goal progress updates as you update the results and activities of your goal. 

1. Click the **X icon** in the upper-right corner of the Goal Details panel to close it.

### Update goals in the Check-in section {#update-goals-in-the-check-in-section}

You can use the Check-in section to check in on goals when you want to quickly provide updates for several goals at the same time.

>[!TIP]
>
>You can access the Check-in section from any of the following sections:
>
>* Goal List 
>* Goal Alignment 
>* Pulse 
>

When you check in on a goal in the Check-in section, you can update the progress of the results and activities that are assigned only to you. You cannot update the progress of results and activities that are assigned to other users in this section.

1. Click the **Main Menu** icon ![](assets/main-menu-icon.png) > **Goals** in the upper-right corner.

   (!-- Add this when Shell is available to all: or (if available), click the **Main Menu** icon ![Main menu icon](../goal-review-and-workfront-goals-sections/assets/three-line-main-menu-icon.png) in the upper-left corner)
   --)

   This opens the Workfront Goals area and the Goal List section displays by default. 

1. Click Check-in in the left panel.

   Or

   (Conditional) If you are in the Goal List, Goal Alignment, or Pulse sections, click the **Check in** button in the upper-right of the screen. This opens the Check-in section.

   ![](assets/check-in-button-highlighted-350x102.png)

   Goals display in a list and results and activities are listed under each goal.

   ![](assets/check-in-page-with-show-all-aligned-goals-link-350x178.png)

1. (Optional) Click **Show all results**, **Show all activities**, or **Show all aligned goals** to the far right of the goal name to display all results, activities, and aligned goals of a goal whose progress you want to update.

   >[!CAUTION]
   >
   >You cannot directly update aligned goals, but you can update their results and activities.

1. Update the current progress on each of the results assigned to you. Depending on what type of result you selected, you can do one of the following:

   * Update the quantity 
   * Update the currency amount
   * Update the percent complete

   The result and the goal progress updated automatically and you receive a confirmation of your changes.

1. Update the percent complete on your Manual progress bar activity.

   >[!TIP]
   >
   >When you add projects as activities to your goals, you cannot manually update projects at the goal level. Workfront automatically updates project progress based on the project of their tasks. When the project percent complete updates in Workfront, the goal progress associated with the project also updates automatically.

   The activity and the goal progress updated automatically and you receive a confirmation of your changes.

1. (Optional) Add a comment for your goal, then click **Post** to save your comment.

-->

목표에 대한 진행 상황을 업데이트하려면

1. 을(를) 클릭합니다. **기본 메뉴** 아이콘 ![](assets/main-menu-icon.png) > **목표** 오른쪽 상단 모서리에서

   <!-- Add this when Shell is available to all: or (if available), click the **Main Menu** icon ![Main menu icon](../goal-review-and-workfront-goals-sections/assets/three-line-main-menu-icon.png) in the upper-left corner)
   -->

   그러면 목표 목록이 열립니다. 기본적으로 볼 수 있는 액세스 권한이 있는 모든 목표가 표시됩니다.

   또는 왼쪽 패널에서 목표 정렬 을 클릭할 수 있습니다.

1. 목표 목록에서 목표 페이지를 열 목표 이름을 클릭합니다.
1. 클릭 **진행률 표시기** 왼쪽 패널에 표시됩니다.

   진행 지표 목록에는 선택한 목표에 대한 모든 진행 상태 표시기가 표시됩니다.

   >[!NOTE]
   >
   >  * 결과 및 활동만 업데이트할 수 있습니다.
   >  * 하위 목표에 대한 진행 상태를 표시하려면 하위 목표의 진행 상태 표시기를 업데이트해야 합니다.
   >  * 프로젝트에 대한 진행 상황을 표시하려면 연결된 프로젝트의 작업을 업데이트해야 합니다.

      >   
      >    결과적으로 하위 목표의 진행 상황과 프로젝트 진행이 선택한 목표의 진행 상황을 이끌게 됩니다.



1. 결과 또는 활동의 진행 상황을 업데이트하려면 **실제 진행률** 결과 또는 활동의 열을 입력하고 값을 업데이트할 숫자를 입력한 다음 Enter 키를 누릅니다.

   ![](assets/actual-progress-result-updating-highlighted-unshimmed.png)

   진행률 열의 진행률 표시기에 대한 진행률 표시기와 목표 헤더에서 목표 진행 상태가 즉시 업데이트됩니다.

