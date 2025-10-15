---
product-previous: workfront-goals
navigation-topic: goal-alignment
title: Adobe Workfront 목표에서 목표 정렬 제거
description: 더 이상 연결할 수 없는 경우 두 목표 간의 정렬을 제거할 수 있습니다.
author: Alina
feature: Workfront Goals
exl-id: a6196356-ca11-4759-9cff-64850a60208e
source-git-commit: 4ef71db5d93e314b746e8acdbf90fd041c6e71ae
workflow-type: tm+mt
source-wordcount: '428'
ht-degree: 1%

---

# Adobe Workfront 목표에서 목표 정렬 제거

<!--Audited P&P only: 4/2025-->

더 이상 연결할 수 없는 경우 두 목표 간의 정렬을 제거할 수 있습니다.

목표 정렬에 대한 자세한 내용은 다음 문서를 참조하십시오.

* [Adobe Workfront 목표에서 연결하여 목표 정렬](../../workfront-goals/goal-alignment/align-goals-by-connecting-them.md)
* [결과 및 활동을 목표로 변환하여 목표 정렬](../../workfront-goals/goal-alignment/align-goals-by-converting-results-activities.md)

## 액세스 요구 사항

>[!NOTE]
>
>이전에 이 패키지를 구입한 경우 귀사에서 Adobe Workfront 목표를 계속 사용하도록 선택할 수 있습니다. 자세한 내용은 계정 담당자에게 문의하십시오.
>
>Adobe Workfront 목표를 더 이상 구매할 수 없습니다.

+++ 을 확장하여 이 문서의 기능에 대한 액세스 요구 사항을 봅니다. 

<table style="table-layout:auto">
<col>
</col>
<col>
</col>
<tbody>
 <tr>
  <td> <p>Adobe Workfront 패키지</p> </td> 
   <td> 
   <p>Adobe Workfront Ultimate</p>
   </td> 
  </tr> 
 <tr>
 <td role="rowheader">Adobe Workfront 라이선스</td>
 <td>
 <p>기여자 이상</p>
 <p>요청 이상</p> </td>
 </tr>
  <tr>
 <td role="rowheader">액세스 수준</td>
 <td> <p>목표에 대한 액세스 편집</p> </td>
 </tr>
 <tr>
 <td role="rowheader">개체 권한</td>
 <td>
  <p>목표에 대한 또는 그 이상의 권한에 대한 보기</p>
  <p>편집할 목표에 대한 권한 관리</p>

</td>
 </tr>
   <td role="rowheader"><p>레이아웃 템플릿</p></td>
   <td> <p>시스템 관리자를 포함한 모든 사용자에게는 기본 메뉴의 목표 영역을 포함하는 레이아웃 템플릿을 할당해야 합니다. </p>  
</td>
  </tr>
</tbody>
</table>

자세한 내용은 [Workfront 설명서의 액세스 요구 사항](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)을 참조하십시오.

+++
<!--Old:
<table style="table-layout:auto">
<col>
</col>
<col>
</col>
<tbody>
 <tr>
 <td role="rowheader">Adobe Workfront plan*</td>
 <td> 
   <p>For the new plan and license structure:
  <ul><li>An Ultimate plan </li></ul>
   </p>
<p>For the current plan and license structure: 
<ul><li> A Pro or higher </li>
  <li>An Adobe Workfront Goals license in addition to a Workfront license.</li></ul></p>
   </td> 
 </tr>
 <tr>
 <td role="rowheader">Adobe Workfront license*</td>
 <td>
 <p>New license: Contributor or higher</p>
 Or
 <p>Current license: Request or higher</p> </td>
 </tr>
 <tr>
 <td role="rowheader">Product*</td>
 <td>
   <p> New product requirement: Workfront</p>
   Or
   <p>Current product requirement: In addition to a Workfront license, you must purchase a license for Adobe Workfront Goals. </p> <p>For information, see <a href="../../workfront-goals/goal-management/access-needed-for-wf-goals.md" class="MCXref xref">Requirements to use Workfront Goals</a>. </p> </td>
 </tr>
 <tr>
 <td role="rowheader">Access level</td>
 <td> <p>Edit access to Goals</p> </td>
 </tr>
 <tr data-mc-conditions="">
 <td role="rowheader">Object permissions</td>
 <td>
  <p>View or higher permissions to the goal to view it</p>
  <p>Manage permissions to the goal to edit it</p>
  <p>For information about sharing goals, see <a href="../../workfront-goals/workfront-goals-settings/share-a-goal.md" class="MCXref xref">Share a goal in Workfront Goals</a>. </p>
  </td>
 </tr>
   <td role="rowheader"><p>Layout template</p></td>
   <td> <p>All users, including Workfront administrators,  must be assigned a layout template that includes the Goals area in the Main Menu. </p>  
</td>
  </tr>
</tbody>
</table>-->

## 전제 조건

시작하려면 먼저 다음 항목이 있어야 합니다.

* 하나 이상의 하위 목표가 연결된 상위 목표입니다. 어린이 목표는 목표의 진행 지표입니다.

## 목표 정렬 제거에 대한 고려 사항

두 목표 간의 정렬을 제거할 때 다음 사항을 고려하십시오.

* 상위 목표에 다른 목표, 활동 또는 결과가 연결되어 있어야 활성 상태를 유지할 수 있습니다.
* 상위 목표의 유일한 진행 표시기인 경우 상위 목표에서 정렬된 하위 목표를 제거할 수 없습니다.
* 상위 목표에 대한 정렬을 제거하면 하위 목표가 독립형 목표가 됩니다.

## 목표 정렬 제거

<!--
Removing goal alignment differs depending on which environment you use.

### Remove goal alignment in the Production environment


1. Go to a child goal aligned to a parent goal. 
1. Click the goal name to open the **Goal Details** panel. 
1. Click the **gear icon** ![Gear icon](assets/gear-icon-settings.png) next to the parent goal, then click **Remove alignment**.

   ![Reove alignment](assets/edit-remove-alignment-350x88.png)

   The goal becomes a standalone goal and its progress no longer influences the progress of the original parent goal. 

1. (Optional) Click **Undo** in the lower-left corner of the screen if you want to revert this change and keep the goals aligned. 
1. (Optional) Add activities and results to either goals to indicate their progress. For information about adding activities and results, see the following articles:

   * [Add activities to goals in Adobe Workfront Goals](../../workfront-goals/results-and-activities/add-activities-to-goals.md) 
   * [Add results to goals in Adobe Workfront Goals](../../workfront-goals/results-and-activities/add-results-to-goals.md)
-->

1. Workfront의 **목표** 영역에 액세스하고 목표의 이름을 클릭하여 목표의 페이지를 엽니다.
1. 상위 목표의 목표 페이지에서 왼쪽 패널의 **진행 표시기**&#x200B;를 클릭합니다.

   ![목표 정렬 다시 이동](assets/remove-goal-alignment-from-list-unshimmed.png)

1. **유형: 목표** 그룹화에서 목표를 선택한 다음 목록 맨 위에 있는 **연결 끊기** 아이콘 ![연결 끊기 아이콘](assets/disconnect-goal-to-remove-alignment-icon-unshimmed.png)을 클릭합니다.

   연결 해제 상자가 표시됩니다.

1. **연결 끊기**&#x200B;를 클릭하여 선택한 목표를 부모와 연결 끊습니다.

   목표가 독립형 목표가 되고 더 이상 원래 목표의 진행 표시기로 나열되지 않습니다. 단절된 목표의 진행은 더 이상 원래 목표의 진행에 영향을 주지 않는다.

   페이지 오른쪽 상단에 목표 연결이 끊겼음을 확인하는 성공 메시지가 표시됩니다.
