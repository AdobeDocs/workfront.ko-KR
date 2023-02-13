---
product-previous: workfront-goals
navigation-topic: old-workfront-goals-articles
title: Adobe Workfront 목표에서 목표 삭제 및 비활성화
description: 목표 작업을 시작할 때 조직에서 관련이 없게 되면 삭제하는 대신 비활성화하는 것이 좋습니다. 목표를 비활성화하면 이전 정보가 보존되고 나중에 다시 활성화할 수 있습니다. 하지만 목표를 삭제하는 것이 적절할 수 있으므로 목표 목록을 정확하게 유지하는 경우도 있습니다.
author: Alina
feature: Workfront Goals
exl-id: 3089adeb-3e56-492a-82fe-536f57079b73
source-git-commit: 1d221d10e5845e477dff825f853330b9b4df0adf
workflow-type: tm+mt
source-wordcount: '652'
ht-degree: 0%

---

# Adobe Workfront 목표에서 목표 삭제 및 비활성화

목표 작업을 시작할 때 조직에서 관련이 없게 되면 삭제하는 대신 비활성화하는 것이 좋습니다. 목표를 비활성화하면 이전 정보가 보존되고 나중에 다시 활성화할 수 있습니다. 하지만 목표를 삭제하는 것이 적절할 수 있으므로 목표 목록을 정확하게 유지하는 경우도 있습니다.

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
   <td> <p>목표 이상에 대한 액세스 편집</p> <p><b>메모</b>

<p>여전히 액세스 권한이 없는 경우 Workfront 관리자에게 액세스 수준에서 추가 제한 사항을 설정하는지 문의하십시오. Workfront 관리자가 액세스 수준을 변경하는 방법에 대한 자세한 내용은 다음을 참조하십시오.</p> 
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

&#42;어떤 계획, 라이선스 유형 또는 액세스 권한을 보유하고 있는지 알아보려면 Workfront 관리자에게 문의하십시오.

## 전제 조건

시작하려면 먼저 다음을 수행해야 합니다.

* 기본 메뉴의 목표 영역을 포함하는 레이아웃 템플릿.

## 목표 비활성화

더 이상 관련이 없고 나중에 다시 활성화하려는 목표를 비활성화할 수 있습니다.

* [목표 비활성화 시 고려 사항](#considerations-when-deactivating-goals)
* [목표 비활성화](#deactivate-goals)

### 목표 비활성화 시 고려 사항

목표를 비활성화할 때에는 다음 사항을 기억하십시오.

* 활성 상태에서만 목표를 비활성화할 수 있습니다. 목표 활성화에 대한 자세한 내용은 [Adobe Workfront 목표에서 목표 활성화](../../workfront-goals/goal-management/activate-goals.md).

   >[!TIP]
   >
   >초안 상태에서는 목표를 비활성화할 수 없습니다.

* Workfront은 비활성화된 목표의 진행 상태 계산을 중지합니다.
* 비활성 목표가 더 이상 Workfront 목표에 표시되거나 목표 의 그래프 섹션에 고려되지 않습니다. Workfront 목표 그래프에 대한 자세한 내용은 [Adobe Workfront 목표의 목표 진행 상황을 이해하려면 그래프를 검토하십시오](../../workfront-goals/goal-review-and-workfront-goals-sections/review-goal-graphs.md).

   <!--* The Check-in section. For information about the Check-in page, see [Update goal progress in Adobe Workfront Goals](../../workfront-goals/goal-review-and-workfront-goals-sections/check-in-goals.md). -->

* 더 이상 비활성화된 목표에 대해 업데이트할 수 없습니다.
* 목표 및 목표에 대한 정보를 편집할 수 있습니다.
* 이전에 비활성화된 목표를 다시 활성화할 수 있습니다.

### 목표 비활성화

<!--
Deactivating goals differs depending on which environment you use.

### Deactivate goals in the Production environment


1. Go to the goal that you want to deactivate.

   For example, go to the Goal List and click the name of a goal.

   The Goal Details panel opens on the right.

   >[!TIP]
   >
   >You can open goals from any sections of Workfront Goals.

1. Click the **More icon** ![](assets/more-icon.png), then click **Deactivate**.

   ![](assets/deactivate-goal-highlighted.png)

   The goal status changes to Inactive. 

1. Click the **X** icon in the upper-right to close Goal Details.
-->

1. 을(를) 클릭합니다. **기본 메뉴** 아이콘 ![](assets/main-menu-icon.png) 오른쪽 상단 모서리에서 을(를) 클릭하고 **목표**.

   목표 목록이 표시됩니다.

   <!-- Add this when Shell is available to all: or (if available), click the **Main Menu** icon ![Main menu icon](../goal-management/assets/three-line-main-menu-icon.png) in the upper-left corner)
   -->

1. (선택 사항) 활성 상태인 목표만 표시하도록 필터를 수정합니다.

   Workfront 목표의 정보 필터링에 대한 자세한 내용은 [Adobe Workfront 목표에서 정보 필터링](../goal-management/filter-information-wf-goals.md).

1. 활성 목표를 클릭합니다.

   목표 페이지가 열립니다.

   ![](assets/goal-page-unshimmed.png)

1. 을(를) 클릭합니다. **자세히** 메뉴 ![](assets/more-icon.png) 목표 이름의 오른쪽에 있는 를 클릭한 다음 **비활성화**.

1. 목표가 비활성화되고 상태가 비활성으로 바뀝니다.

## 목표 삭제

더 이상 관련성이 없거나 중요하지 않은 목표를 삭제할 수 있습니다.

* [목표 삭제 시 고려 사항](#considerations-when-deleting-goals)
* [목표 삭제](#delete-goals)

### 목표 삭제 시 고려 사항 {#considerations-when-deleting-goals}

* 닫힌 목표를 포함하여 모든 상태에서 목표를 삭제할 수 있습니다.
* 삭제된 목표를 복구할 수 없습니다.
* 목표에 첨부된 결과 및 수동 진행률 표시줄 활동도 삭제됩니다.
* 목표와 연결된 프로젝트는 삭제되지 않지만 목표와의 연관성은 제거됩니다.

### 목표 삭제

<!--
Deleting  goals differs depending on which environment you use.

#### Delete goals in the Production environment

1. Go to the goal that you want to delete.

   For example, go to the Goal List and click a goal.

   The Goal Details panel opens on the right. 

1. Click the **More icon** ![](assets/more-icon.png), then click **Delete**.

   ![](assets/delete-goal-highlighted.png)

1. Click **Yes, delete**.

   The goal is removed from the Goal List and cannot be recovered.
-->

1. Main Menu 아이콘을 클릭합니다. ![](assets/main-menu-icon.png) 오른쪽 상단 모서리에서 을(를) 클릭하고 **목표**.

   목표 목록이 표시됩니다.

   <!-- Add this when Shell is available to all: or (if available), click the **Main Menu** icon ![Main menu icon](../goal-management/assets/three-line-main-menu-icon.png) in the upper-left corner)
   -->
1. 목표 이름을 클릭합니다. 목표 페이지가 열립니다.
1. 을(를) 클릭합니다. **자세히** 메뉴 ![](assets/more-icon.png) 목표 이름의 오른쪽에 있는 를 클릭한 다음 **목표 삭제**, 그런 다음 **삭제**.

   목표 및 해당 활동 및 결과도 삭제되며 복구할 수 없습니다. 목표 또는 하위 목표와 연관된 프로젝트는 삭제되지 않습니다.


