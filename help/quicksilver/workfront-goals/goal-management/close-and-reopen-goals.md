---
product-previous: workfront-goals
navigation-topic: goal-management
title: Adobe Workfront 목표의 목표 닫기 및 다시 열기
description: 목표를 완료했거나 더 이상 쓸모가 없어져 작업을 수행하지 않을 때 목표를 닫을 수 있습니다.
author: Alina
feature: Workfront Goals
exl-id: bbb549c1-aea6-4f5e-8a6b-01fc04cf06ef
source-git-commit: 09e34ecdfeec531ebbaaba4fb8682496c53d86bf
workflow-type: tm+mt
source-wordcount: '902'
ht-degree: 0%

---

# Adobe Workfront 목표의 목표 닫기 및 다시 열기

다음을 나타내고자 할 때 목표를 닫을 수 있습니다.

* 목표가 달성되었거나 기간이 경과했기 때문에 수행됩니다.
* 더 이상 이 작업을 수행하지 않으며 가까운 미래에도 그렇게 할 계획이 없습니다.

마감된 목표가 다시 관련이 있을 때 다시 열 수 있습니다.

## 액세스 요구 사항

다음 항목이 있어야 합니다.

<table style="table-layout:auto">
<col>
</col>
<col>
</col>
<tbody>
 <tr>
 <td role="rowheader">Adobe Workfront 플랜</td>
 <td>
 <p>임의</p>

</td>
 </tr>
 <tr>
 <td role="rowheader">Adobe Workfront 라이센스*</td>
 <td>
 <p>새 라이선스: 기여자 이상</p>
 또는
 <p>현재 라이선스: 요청 이상</p> <p>자세한 내용은 <a href="../../administration-and-setup/add-users/access-levels-and-object-permissions/wf-licenses.md" class="MCXref xref">Adobe Workfront 라이선스 개요</a>.</p> </td>
 </tr>
 <tr>
 <td role="rowheader">제품*</td>
 <td>
 <p> 다음 중 하나인 새 제품 요구 사항: </p>
<ul>
<li>Select 또는 Prime Adobe Workfront 플랜 및 추가 Adobe Workfront Goals 라이선스.</li>
<li>기본적으로 Workfront 목표를 포함하는 Ultimate Workfront 계획입니다. </li></ul>
 <p>또는</p>
 <p>현재 제품 요구 사항: Workfront 플랜 및 Adobe Workfront 목표에 대한 추가 라이선스. </p> <p>자세한 내용은 <a href="../../workfront-goals/goal-management/access-needed-for-wf-goals.md" class="MCXref xref">Workfront 목표 사용 요구 사항</a>. </p> </td>
 </tr>
 <td role="rowheader">액세스 수준</td>
 <td> <p>목표에 대한 액세스 편집</p> </td>
 </tr>
 <tr data-mc-conditions="">
 <td role="rowheader">개체 권한</td>
 <td>
  <div>
  <p>목표에 대한 또는 그 이상의 권한에 대한 보기</p>
  <p>편집할 목표에 대한 권한 관리</p>
  <p>목표 공유에 대한 자세한 내용은 <a href="../../workfront-goals/workfront-goals-settings/share-a-goal.md" class="MCXref xref">Workfront 목표에서 목표 공유</a>. </p>
  </div> </td>
 </tr>
<tr>
   <td role="rowheader"><p>레이아웃 템플릿</p></td>
   <td> <p>Workfront 관리자를 포함한 모든 사용자에게 메인 메뉴의 목표 영역을 포함하는 레이아웃 템플릿을 할당해야 합니다. </p>  
</td>
  </tr>
</tbody>
</table>

*자세한 내용은 [Workfront 설명서의 액세스 요구 사항](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

## 목표를 닫거나 다시 열 때의 고려 사항

* 목표를 닫았다가 다시 열려면 먼저 액세스 수준에서 목표 편집에 대한 액세스 권한이 있어야 합니다. 목표에 대한 액세스 권한 부여에 대한 자세한 내용은 을 참조하십시오. [Adobe Workfront 목표에 대한 액세스 권한 부여](../../administration-and-setup/add-users/configure-and-grant-access/grant-access-goals.md).
* 활성 목표만 닫을 수 있습니다. 초안 상태의 목표는 닫을 수 없습니다.

  목표 상태에 대한 자세한 내용은 [Adobe Workfront 목표의 목표 상태 개요](../../workfront-goals/goal-management/goal-status-overview.md).

* 목표를 닫으면 진행이 잠기고 목표를 달성한 정도를 평가할 수 있습니다.

  >[!CAUTION]
  >
  >활성 기여 목표가 있는 목표를 닫을 때 종료 후 진행 상태가 변경되어 기여 활성 목표의 진행 상황을 나타냅니다. 목표 정렬에 대한 자세한 내용은 [Adobe Workfront 목표에서 연결하여 목표 정렬](../../workfront-goals/goal-alignment/align-goals-by-connecting-them.md).

* 목표를 닫기 전에 목표의 진행 표시기를 업데이트하여 정확한 진행 값으로 목표가 닫히도록 합니다. 모든 진행 표시기가 달성된 경우 목표 완료율은 100%여야 하며 목표가 달성되었습니다. 목표 업데이트에 대한 자세한 내용은 [Adobe Workfront 목표의 목표 진행 상황 업데이트](../../workfront-goals/goal-review-and-workfront-goals-sections/check-in-goals.md).
* 마감한 목표에 대한 업데이트로 최종 주석을 남겨둡니다. 목표에 주석을 추가하는 방법에 대한 자세한 내용은 [Adobe Workfront 목표의 목표 주석 관리](../../workfront-goals/goal-management/manage-goal-comments.md).
* 닫은 목표에 대한 결과 및 활동의 진행 상황을 더 이상 업데이트할 수 없습니다.
* 마감된 목표를 계속 작업하려면 마감된 목표를 다시 열 수 있습니다.
* 목표를 달성하지 못한 경우 해당 정보의 대부분을 다음 기간(분기 또는 연도)에 복사하는 것이 좋습니다. 이는 한 기간에서 다음 기간까지 동일한 목표 또는 다음 기간에 달성하기 위해 여전히 작업해야 하는 목표에 적합한 옵션입니다. 목표 복사에 대한 자세한 내용은 [Adobe Workfront 목표의 목표 복사](../../workfront-goals/goal-management/copy-goals.md). 다른 기간에 복사하는 대신 목표의 기간을 업데이트할 수도 있습니다.
* Workfront은 닫힌 목표를 다시 열면 해당 목표의 주석을 삭제합니다. 주석을 유지해야 하는 경우에는 닫은 목표를 다시 열지 말고 연결된 결과를 포함하여 복사하는 것이 좋습니다.


## 목표 닫기

<!--
Closing goals differs depending on what environment you use. 

### Close goals in the Production environment

1. Click the **Main Menu** icon ![](assets/main-menu-icon.png) > **Goals** in the upper-right corner.

   (!-- Add this when Shell is available to all: or (if available), click the **Main Menu** icon ![Main menu icon](../goal-management/assets/three-line-main-menu-icon.png) in the upper-left corner)
   --)

   The Goal List opens. 

1. (Optional) Modify your filters to display only goals that are active.

   For information about filtering information in Workfront Goals, see [Filter information in Adobe Workfront Goals](../../workfront-goals/goal-management/filter-information-wf-goals.md). 

1. Click an active goal.

   The Goal Details panel displays on the right. 

1. (Optional and recommended) Click the **Updates** tab and add an update in the **Comment here** field about the reason you are closing the goal, then click **Post**. 

1. Click the **More icon** ![](assets/more-icon.png) to the right of the goal name, then click **Close** > **Close Goal**.

   This closes the goal and saves the current progress on the goal and its results and activities.

   >[!IMPORTANT]
   >
   >If the goal has contributing goals that are still active, the progress of the goal continues to update based on the progress of the aligned goals.
   >
   >
   >![](assets/closing-goals-with-active-aligned-goals-warning-350x71.png)   >
   >

1. (Optional) Modify your filters again to display only closed goals. The goals you closed display on the screen.
-->

1. 다음을 클릭합니다. **메인 메뉴** 아이콘 ![](assets/main-menu-icon.png) > **목표** 오른쪽 상단 모서리입니다.

   목표 목록이 열립니다.

   <!-- Add this when Shell is available to all: or (if available), click the **Main Menu** icon ![Main menu icon](../goal-management/assets/three-line-main-menu-icon.png) in the upper-left corner)
   -->

1. (선택 사항) 활성 상태인 목표만 표시하도록 필터를 수정합니다.

   Workfront 목표의 필터링 정보에 대한 자세한 내용은 다음을 참조하십시오. [Adobe Workfront 목표의 정보 필터링](../goal-management/filter-information-wf-goals.md).
1. 활성 목표를 클릭합니다.

   목표 페이지가 열립니다.

   ![](assets/goal-page-unshimmed.png)
1. 다음을 클릭합니다. **자세히** 메뉴 ![](assets/more-icon.png) 목표 이름의 오른쪽에 있는 을(를) 클릭합니다. **닫기**.

   목표가 닫히고 화면 오른쪽 상단에 확인 메시지가 표시됩니다.

   ![](assets/goal-close-confirmation-with-add-closing-notes-link.png)

1. (선택 사항) 확인란에서 **마감 메모 추가** 이 목표와 이 목표를 닫아야 하는 이유에 대한 설명을 추가합니다.
1. 닫기 메모를 추가한 다음 **메모 추가**.

   ![](assets/add-closing-notes-box-unshimmed.png)

   설명은 목표 페이지의 목표 세부 정보 섹션에 마감 메모 영역에 표시됩니다.

   >[!NOTE]
   >
   >나중에 닫힌 목표를 다시 열면 Workfront이 마감 메모를 삭제합니다.


## 목표 재개

마감된 목표가 다시 관련성이 있다고 판단되어 진행 상황을 계속 업데이트해야 하는 경우 마감된 목표를 다시 열 수 있습니다.

<!--
Reopening goals differs depending on what environment you use.

### Reopen goals in the Production environment

1. Click the **Main Menu** icon ![](assets/main-menu-icon.png) > **Goals** in the upper-right corner.

   (!-- Add this when Shell is available to all: or (if available), click the **Main Menu** icon ![Main menu icon](../goal-management/assets/three-line-main-menu-icon.png) in the upper-left corner)
   --)

   The Goal List opens. 

1. (Optional) Modify your filters to display only goals that are closed.

   For information about filtering information in Workfront Goals, see [Filter information in Adobe Workfront Goals](../../workfront-goals/goal-management/filter-information-wf-goals.md).


1. Click a closed goal.

   This opens the Goal Details panel on the right. 

1. Click the **More icon** ![](assets/more-icon.png) to the right of the goal name, then click **Reopen** > **Reopen**.

   This reopens the goal and places it in a status of Active. The progress of the goal is recalculated starting with the current date. 

1. (Optional) Modify your filters again to display only active goals. The goals you opened display on the screen.

-->

1. 다음을 클릭합니다. **메인 메뉴** 아이콘 ![](assets/main-menu-icon.png)> **목표** 오른쪽 상단 모서리입니다.

   목표 목록이 열립니다.

   <!-- Add this when Shell is available to all: or (if available), click the **Main Menu** icon ![Main menu icon](../goal-management/assets/three-line-main-menu-icon.png) in the upper-left corner)
   -->

1. (선택 사항) 닫힌 목표만 표시하도록 필터를 수정합니다.

   Workfront 목표의 필터링 정보에 대한 자세한 내용은 다음을 참조하십시오. [Adobe Workfront 목표의 정보 필터링](../goal-management/filter-information-wf-goals.md).
1. 마감된 목표의 이름을 클릭합니다.

   목표 페이지가 열립니다.
1. 다음을 클릭합니다. **자세히** 메뉴 ![](assets/more-icon.png) 목표 이름의 오른쪽에 있는 다음 **다시 열기** > **다시 열기**.

   다음과 같은 상황이 발생합니다.
   * 목표가 현재 열려 있고 활성 상태입니다.
   * 현재 날짜부터 목표 진행률이 다시 계산됩니다.
   * 모든 마감 메모는 목표 세부 사항 페이지에서 삭제됩니다. 삭제된 마감 메모는 복구할 수 없습니다.

1. (선택 사항) 활성 목표만 표시하도록 필터를 다시 수정합니다.

   연 목표가 화면에 표시됩니다.

