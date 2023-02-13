---
product-previous: workfront-goals
navigation-topic: goal-management
title: Adobe Workfront 목표 의 목표 세부 사항 패널에서 목표 업데이트
description: 목표 세부 사항 패널에 액세스하여 개별 목표에 대한 정보를 업데이트할 수 있습니다.
author: Alina
feature: Workfront Goals
exl-id: e9df0d98-05a1-4977-b7f1-426b8f5b3eae
source-git-commit: 1d221d10e5845e477dff825f853330b9b4df0adf
workflow-type: tm+mt
source-wordcount: '614'
ht-degree: 1%

---

# Adobe Workfront 목표의 목표 세부 사항 섹션에서 목표 업데이트

<!--drafted for the goal redesign:
- change the title for Production to Update goals in the Goal details section in Adobe Workfront Goals. 
- update the description in the metadata above
-->

목표 세부 사항 패널에 액세스하여 개별 목표에 대한 정보를 업데이트할 수 있습니다.

>[!NOTE]
>
>상태가 닫됨인 목표는 업데이트할 수 없습니다.


## 액세스 요구 사항

<!--drafted for P&P release: replace the existing requirements with this:

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

## 목표 세부 사항 섹션에서 목표 업데이트

목표 목록에서 개별 목표에 액세스할 수 있습니다.

<!--

Updating goals in the Goal Details panel differs depending on where you access the goal from. 

### Update goals in the Goal Details panel in the Production environment

1. Click the **Main Menu** icon ![](assets/main-menu-icon.png) > **Goals** in the upper-right corner.

   (!-- Add this when Shell is available to all: or (if available), click the **Main Menu** icon ![Main menu icon](../goal-management/assets/three-line-main-menu-icon.png) in the upper-left corner)
   --)

   This opens the Goals area in Workfront. 

1. Click the name of a goal in the Goal List, then click the name of a goal.

   This opens the Goal Details panel on the right.
   ![](assets/goal-details-summary-tab-350x294.png)

   >[!TIP]
   >
   >You can also click the name of a goal in the Goal Alignment, Check-in, or Pulse sections. 
   >
   ><!-- drafted for goal redesign:
   >Add this to the TIP above with goal redesign: 
   >
   >The Check-in and Pulse sections have been removed from the Preview environment.
   >

1. On the Summary tab, click the **More icon** ![](assets/more-icon.png), then click any of the following options:

   1. **Edit**. For information about editing goals, see [Edit goals in Adobe Workfront Goals](../../workfront-goals/goal-management/edit-goals.md).
   1. **Copy**. For information about copying goals, see [Copy goals in Adobe Workfront Goals](../../workfront-goals/goal-management/copy-goals.md).
   1. **Activate**. This option is available only for drafted and inactive goals.

      For information about activating goals, see [Access and open goals in Adobe Workfront Goals](../../workfront-goals/goal-management/access-goals-in-wf-goals.md). 
   
   1. **Close**, then click**Close Goal**. This option is available only for active goals.

      For information about closing goals, see [Close and reopen goals in Adobe Workfront Goals](../../workfront-goals/goal-management/close-and-reopen-goals.md). 
   
   1. **Deactivate**. This option is available only for active goals. This deactivates the goal immediately.

      For information about deactivating goals, see [Delete and deactivate goals in Adobe Workfront Goals](../../workfront-goals/goal-management/delete-and-deactivate-goals.md).
   
   1. **Delete**, then click **Yes, Delete**.

      For information about deleting goals, see [Delete and deactivate goals in Adobe Workfront Goals](../../workfront-goals/goal-management/delete-and-deactivate-goals.md).

      >[!NOTE]
      >
      >Deleted goals cannot be recovered.

   1. **Reopen**, then click **Reopen**. This option is available only for closed goals that are from a current time period.

      For information about reopening goals, see [Close and reopen goals in Adobe Workfront Goals](../../workfront-goals/goal-management/close-and-reopen-goals.md). 
   
   1. (Conditional) If you clicked any of the options between steps a-i above except Delete or Reopen, click **Save**.    
   
      (!--ensure this is accurate)--)

1. Click **Align to another goal** in the upper-right of the Summary tab, then specify the name of a goal in the **Align to** **another goal** field that you want to align the current goal to. The current goal becomes the child of the goal you align it to. For information about child and parent goals, see [Align goals by connecting them in Adobe Workfront Goals](../../workfront-goals/goal-alignment/align-goals-by-connecting-them.md). 
1. Click **Add results**. Results drive the progress of your goal. For information about adding results, see [Add results to goals in Adobe Workfront Goals](../../workfront-goals/results-and-activities/add-results-to-goals.md).

1. Click **Add activities**. Activities drive the progress of your goal. For information about adding activities, see [Add activities to goals in Adobe Workfront Goals](../../workfront-goals/results-and-activities/add-activities-to-goals.md). 

1. Click the **Updates** tab. Here, you can view goal comments and review the entire editing history of the goal, activities, and results, to understand who changed what and when.

   ![](assets/goal-details-updates-tab-350x280.png)

1. (Optional) Deselect any of the following options if you want to not display them in the Updates tab.&nbsp;They are selected by default: 

   | Option |Description  |
   |---|---|
   | Progress Updates |Displays information about the history of progress updates on results and activities.  |
   | Comments |Displays comments made by users on the goal.  |
   | Editing History |Displays information about creating and updating the goal, results, and activities.  |

1. (Optional) Click **Details** under a progress or an editing history update to display additional information about the update.

   ![](assets/update-details-in-updates-tab-expanded-highlighted-350x139.png)

-->



1. 목표 목록에서 목표 이름을 클릭한 다음 목표 이름을 클릭합니다.

   이렇게 하면 **목표 세부 사항** 섹션에 있습니다.

   ![](assets/goal-page-unshimmed.png)

1. 을(를) 클릭합니다. **편집 아이콘** ![](assets/edit-icon.png) 오른쪽 위 모서리에서 을(를) 클릭하고 **모두 편집** 또는 **개요**

   또는

   목표 세부 사항 섹션의 편집 가능한 필드 중 하나에 정보 입력을 시작합니다. 섹션을 편집할 수 있습니다.

   >[!IMPORTANT]
   >
   >목표 세부 사항 섹션에 표시되는 일부 필드는 편집할 수 없습니다. Workfront은 일부 필드를 계산하며 읽기 전용입니다.

1. 다음 필드를 업데이트하거나 검토합니다.

   * **설명**: 목표에 대한 정보를 추가하거나 업데이트합니다.
   * **진행률**: 지금까지 완료되는 목표 비율을 나타냅니다. 목표 진행 상태는 수동으로 업데이트할 수 없습니다. 목표 진행 상태는 모든 진행 상태 표시기를 계산하는 것입니다.
   * **조건**: 목표가 새로운 것인지, 아직 업데이트되지 않았는지, 제시간에 완료되는 것이 목표인지, 아니면 후행인지를 나타냅니다. 목표 조건은 업데이트할 수 없습니다. 목표의 조건은 Workfront에 의해 자동으로 계산됩니다.\
      목표 조건 및 진행률에 대한 자세한 내용은
      [Adobe Workfront 목표의 목표 진행 및 조건 개요](../goal-management/calculate-goal-progress.md).
   * **상태**: 목표의 상태는 수동으로 업데이트할 수 없습니다. 자세한 내용은 [Adobe Workfront 목표의 목표 상태 개요](../goal-management/goal-status-overview.md).
   * **목표 소유자**: 을(를) 클릭하여 목표 소유자의 이름을 업데이트합니다. 사용자, 팀, 그룹 또는 조직 이름을 입력하기 시작한 다음 목록에 표시될 때 선택합니다. 한 골대에 한 명의 소유자만 있을 수 있습니다.
   * **상위 목표**: 선택한 목표의 상위로 설정할 목표 이름을 입력하기 시작합니다. 선택한 목표의 진행 상태는 상위 목표의 진행 상태를 자동으로 업데이트합니다.

      >[!TIP]
      >
      >상위 목표에 대한 다음 정보는 업데이트할 수 없습니다.
      >    * 상위 목표 기간
      >    * 상위 목표 진행 상황
      >    * 상위 목표 소유자.

      >      
      >상위 목표 자체에 대한 이 정보를 업데이트해야 합니다.

   * **기간**: 목표를 위한 기간을 업데이트하려면 을(를) 클릭합니다\
      또는\
      선택 **사용자 지정 날짜 활성화** 목표의 날짜를 지정하려면 **시작** 및 **종료 날짜**.
   * **닫기 참고 사항**: 이 필드는 상태가 닫힌 목표에만 표시됩니다. 닫힌 목표는 편집할 수 없습니다. 닫힌 목표를 영구적으로 다시 열면 닫는 메모가 영구적으로 삭제됩니다.


