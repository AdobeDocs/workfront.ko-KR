---
product-previous: workfront-goals
navigation-topic: goal-alignment
title: Adobe Workfront 목표에 연결하여 목표 정렬
description: 개인 목표를 가진 개별 기여자인 경우 조직의 전략의 큰 컨텍스트에서 자신의 목표의 진행 상황을 효과적으로 표시하기 위해 해당 목표를 팀의 목표에 맞게 조정할 수 있습니다.
author: Alina
feature: Workfront Goals
exl-id: 4276f1c9-2ee9-4f74-b011-ae1e19fefe35
source-git-commit: 1d221d10e5845e477dff825f853330b9b4df0adf
workflow-type: tm+mt
source-wordcount: '770'
ht-degree: 0%

---

# Adobe Workfront 목표에 연결하여 목표 정렬


개인 목표를 가진 개별 기여자인 경우 조직의 전략의 큰 컨텍스트에서 자신의 목표의 진행 상황을 효과적으로 표시하기 위해 해당 목표를 팀의 목표에 맞게 조정할 수 있습니다.

조직의 모든 구성원이 조직의 목표에 맞는 목표를 가지고 있을 경우 개별 기여와 팀 노력이 더 큰 회사 수준의 우선 순위에 따라 전진하는 데 어떻게 도움이 되는지 명확히 알 수 있습니다. 목표 정렬을 위한 우수 사례에 대한 자세한 내용은 다음을 참조하십시오 [Adobe Workfront 목표의 목표 정렬 개요](../../workfront-goals/goal-alignment/goal-alignment-overview.md).

Adobe Workfront 목표에는 두 가지 방법으로 목표를 연결할 수 있습니다.

* 목표를 서로 연결하여 목표 간 정렬을 만들 수 있습니다.

* 두 개의 목표를 수동으로 맞추거나 기존 목표의 결과와 활동을 다른 목표로 전환할 수 있습니다. 변환된 결과 또는 활동이 원래 목표의 하위 목표가 됩니다.

>[!IMPORTANT]
>
>목표에는 총 1000개의 진행률 표시기가 있을 수 있습니다.

이 문서에서는 목표를 서로 연결하여 맞추는 방법을 설명합니다. 결과와 활동을 목표로 전환하여 목표를 정렬하는 방법에 대한 자세한 내용은 [결과 및 활동을 목표로 변환하여 목표 정렬](../../workfront-goals/goal-alignment/align-goals-by-converting-results-activities.md).

## 액세스 요구 사항

<!--drfated for the P&P release: 

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
   <td> <p>목표에 대한 액세스 편집</p> <p><b>메모</b>

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

*보유하고 있는 플랜, 라이선스 유형 또는 액세스를 알아보려면 Workfront 관리자에게 문의하십시오.

## 전제 조건

시작하려면 먼저 다음을 수행해야 합니다.

* 기본 메뉴의 목표 영역을 포함하는 레이아웃 템플릿.

## 목표를 서로 연결하여 맞춤

<!--
Aligning goals by connecting them differs depending on what environment you use. 

### Align goals by connecting them in the Production environment

1. Create two goals that you want to align. For information about creating goals, see [Create goals in Adobe Workfront Goals](../../workfront-goals/goal-management/create-goals.md).
1. (Optional) Activate the goals that you want to align. You can align goals that have a Draft, Active, or Inactive status. For information about activating goals, see [Activate goals in Adobe Workfront Goals](../../workfront-goals/goal-management/activate-goals.md).
1. Go to the goal that you want to align (child goal) to another goal (parent goal) and click its name to open the **Goal Details** panel.

   For example, if you want Goal 2 to influence the progress of Goal 1, you must go to Goal 2. 

1. Click **Align to another goal** in the upper-right corner of the right panel.

   ![](assets/align-to-another-goal-link-highlighted-350x128.png)

1. Start typing the name of an existing goal or the name of an owner in the **Align to another goal** field, then select it when it appears in the list. Only goals that are from the same or future periods display in the list. 
1. Click **Save**.

   The goal you started with (Goal 2) is now the child goal of the goal you aligned it with (Goal 1).   
   The aligned goals display connected in the Goal Alignment section with Goal 2 as secondary to Goal 1.

   ![](assets/goal-1-and-2-aligned-cards-350x427.png)

1. (Optional) To view the goals in the Goal Alignment section, do one of the following:

   * Click the Goal Alignment section in the left panel and find the goals by applying the correct filter. For information about filtering information in Workfront Goals, see [Filter information in Adobe Workfront Goals](../../workfront-goals/goal-management/filter-information-wf-goals.md).
   * Click the Goal List, Check-in, or Pulse sections in the left panel and find one of the goals, then click the **Alignment icon** ![](assets/align-icon.png) next to the goal name to go directly to the goal in the Goal Alignment section.

   For information about the Goal Alignment section, see [Navigate the Goal Alignment section in Adobe Workfront Goals](../../workfront-goals/goal-alignment/navigate-goal-alignment-chart.md). 

1. (Optional) Add activities and results to either goal to indicate their progress. For information about adding activities and results, see the following articles:

   * [Add activities to goals in Adobe Workfront Goals](../../workfront-goals/results-and-activities/add-activities-to-goals.md) 
   * [Add results to goals in Adobe Workfront Goals](../../workfront-goals/results-and-activities/add-results-to-goals.md)

1. (Optional) Remove the alignment between two goals, when you consider that no longer is relevant to your organization's overall strategy For information about removing alignment between goals, see [Remove goal alignment in Adobe Workfront Goals](../../workfront-goals/goal-alignment/remove-goal-alignment.md).

-->
1. 정렬할 두 개의 목표를 만듭니다. 목표 만들기에 대한 내용은 [Adobe Workfront 목표에서 목표 만들기](../../workfront-goals/goal-management/create-goals.md).
1. (선택 사항) 정렬할 목표를 활성화합니다. 초안, 활성 또는 비활성 상태인 목표를 정렬할 수 있습니다. 목표 활성화에 대한 자세한 내용은 [Adobe Workfront 목표에서 목표 활성화](../../workfront-goals/goal-management/activate-goals.md).
1. 다른 목표(상위 목표)에 맞게(하위 목표)를 맞추려는 목표로 이동하고 해당 이름을 클릭하여 목표 페이지를 엽니다.

   >[!INFO]
   >
   >예를 들어, 목표 2가 목표 1의 진행 상태에 영향을 미치도록 하려면 목표 2로 이동해야 합니다.

1. 클릭 **목표 세부 사항** 왼쪽 패널에 표시됩니다.

1. 에서 **상위 목표 정보** 영역을 클릭합니다. **추가** 에서 **상위 목표** 상위 목표가 없으면,

   또는

   다른 목표를 선택하려면 상위 목표 이름을 클릭하십시오.

1. 에 기존 목표의 이름을 입력합니다. **상위 목표** 필드를 선택한 다음 목록에 표시될 때 선택합니다. 동일하거나 미래 기간에 있는 목표만 목록에 표시됩니다.

1. 클릭 **변경 내용 저장**.

   시작한 목표(목표 2)가 이제 목표(목표 1)와 정렬한 상위 목표의 하위 목표입니다.\
   정렬된 목표들은 목표 정렬 섹션에 목표 2와 목표 1의 2차 요소로 연결됩니다.
진행률이 상위 목표의 진행 상황을 업데이트하면 하위 목표가 상위 목표의 진행 상태 표시기 섹션에 표시됩니다.

   ![](assets/goal-1-and-2-aligned-cards-350x427.png)

1. (선택 사항) 목표 정렬 섹션에서 목표를 보려면 Workfront의 목표 영역으로 이동한 다음 **목표 정렬** 왼쪽 패널의 섹션에 있습니다. 목표 정렬 섹션에 대한 자세한 내용은 [Adobe Workfront 목표의 목표 정렬 섹션으로 이동합니다](../../workfront-goals/goal-alignment/navigate-goal-alignment-chart.md).

1. (선택 사항) 활동 및 결과를 목표에 추가하여 진행 상황을 나타냅니다. 활동 및 결과 추가에 대한 자세한 내용은 다음 문서를 참조하십시오.

   * [Adobe Workfront 목표의 목표에 활동 추가](../../workfront-goals/results-and-activities/add-activities-to-goals.md)
   * [Adobe Workfront 목표에 결과 추가](../../workfront-goals/results-and-activities/add-results-to-goals.md)

1. (선택 사항) 더 이상 조직의 전체 전략과 관련이 없다고 고려할 때 두 목표 간의 정렬을 제거합니다. 목표 간 정렬 제거에 대한 자세한 내용은 [Adobe Workfront 목표에서 목표 정렬 제거](../../workfront-goals/goal-alignment/remove-goal-alignment.md).

