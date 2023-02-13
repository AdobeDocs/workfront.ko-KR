---
product-previous: workfront-goals
navigation-topic: goal-review-and-sections
title: Adobe Workfront 목표의 목표 진행 상황을 이해하려면 그래프를 검토하십시오
description: Adobe Workfront 목표 의 그래프 섹션에서 목표의 전체 상태와 진행 상황을 확인할 수 있습니다. 이 섹션의 차트는 각 목표의 진행 상태를 분류하지 않지만, 대신 지정된 기간 동안의 진행 상황과 모든 목표의 진행 상태에 대한 전체적인 스냅샷을 제공합니다.
author: Alina
feature: Workfront Goals
exl-id: 8d5f3617-c7bf-44ce-99b0-d4ebda106f25
source-git-commit: 3989903687f2ea64ebd5ad754119ce1a9d70b9f3
workflow-type: tm+mt
source-wordcount: '951'
ht-degree: 0%

---

# Adobe Workfront 목표의 목표 진행 상황을 이해하려면 그래프를 검토하십시오

<!-- drafted mostly for P&P release-->

Adobe Workfront 목표 의 그래프 섹션에서 목표의 전체 상태와 진행 상황을 확인할 수 있습니다. 이 섹션의 차트는 각 목표의 진행 상태를 분류하지 않지만, 대신 지정된 기간 동안의 진행 상황과 모든 목표의 진행 상태에 대한 전체적인 스냅샷을 제공합니다.

>[!IMPORTANT]
>
>선택한 기간 동안 그래프 섹션에서 목표에 대한 총 개수를 확인할 수 있습니다. 그러나 Workfront 목표는 전체 목표 진행 상태 및 완료율을 계산할 때 활성 및 종료됨 상태의 목표만 고려합니다.

## 액세스 요구 사항

<!--drafted for P&P release: 

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

이 문서에 설명된 작업을 수행하려면 다음 액세스 권한이 있어야 합니다.

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
   <td role="rowheader">액세스 수준*</td> 
   <td> <p>목표에 대한 액세스 권한 보기 이상</p> <p><b>메모</b><p>여전히 액세스 권한이 없는 경우 Workfront 관리자에게 액세스 수준에서 추가 제한 사항을 설정하는지 문의하십시오. Workfront 관리자가 액세스 수준을 변경하는 방법에 대한 자세한 내용은 다음을 참조하십시오.</p> 
     <ul> 
      <li> <p><a href="../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">사용자 정의 액세스 수준 만들기 또는 수정</a> </p> </li> 
      <li> <p><span href="../../administration-and-setup/add-users/configure-and-grant-access/grant-access-goals.md"><a href="../../administration-and-setup/add-users/configure-and-grant-access/grant-access-goals.md" class="MCXref xref">Adobe Workfront 목표에 대한 액세스 권한 부여</a></span> </p> </li> 
     </ul> </p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader">개체 권한</td> 
   <td> 
    <div> 
     <p>목표에 대한 권한 보기 이상</p> 
     <p>목표 공유에 대한 자세한 내용은 <a href="../../workfront-goals/workfront-goals-settings/share-a-goal.md" class="MCXref xref">Workfront 목표에서 목표 공유</a>. </p> 
    </div> </td> 
  </tr> 
 </tbody> 
</table>

*보유하고 있는 플랜, 라이선스 유형 또는 액세스를 알아보려면 Workfront 관리자에게 문의하십시오.

## 전제 조건

시작하려면 먼저 다음을 수행해야 합니다.

* 기본 메뉴의 목표 영역을 포함하는 레이아웃 템플릿.

## Workfront 목표에 있는 그래프 유형

그래프 섹션이나 Workfront 목표에 다음 차트를 사용할 수 있습니다.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">목표 상태 차트</td> 
   <td> <p>다음을 표시하는 계기 차트입니다.</p> 
    <ul> 
     <li>선택한 기간에 대한 총 목표 수입니다. 어떤 상태든 목표를 고려합니다. </li> 
     <li>상태가 활성 및 종료인 목표의 진행 상태입니다.</li> 
    </ul> <p>Workfront 목표가 진행 상태를 계산하는 방법에 대한 자세한 내용은 <a href="../../workfront-goals/goal-management/calculate-goal-progress.md" class="MCXref xref">Adobe Workfront 목표의 목표 진행 및 조건 개요</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">목표 진행률 차트</td> 
   <td> <p>목표에 대한 업데이트를 목표에 대한 기간 동안 주별 단위로 표시하는 라인 차트입니다. 목표 진행 차트에는 다음과 같은 내용이 표시됩니다.</p> 
    <ul> 
     <li>선택한 기간의 모든 활성 및 마감된 목표에 대한 평균 예상 완료율과 실제 완료율. 완료율 진행률은 노드에 의해 표시된 매주 증분으로 분할됩니다. </li> 
     <li>이전 주 이후 활성 목표 및 닫힌 목표에 대한 전체 평균 진행 비율입니다. </li> 
    </ul> <p>팁: 선택한 기간 이외의 목표에 대한 업데이트가 있을 때 목표 진행 차트에는 정보가 표시되지 않을 수 있습니다. </p> </td> 
  </tr> 
 </tbody> 
</table>

## 그래프에서 목표 진행 상태 검토

1. 을(를) 클릭합니다. **기본 메뉴** 아이콘 ![](assets/main-menu-icon.png) > **목표** 오른쪽 상단 모서리에서

   <!-- Add this when Shell is available to all: or (if available), click the **Main Menu** icon ![Main menu icon](../goal-review-and-workfront-goals-sections/assets/three-line-main-menu-icon.png) in the upper-left corner)
   -->

   이렇게 하면 Workfront 목표 영역이 열립니다.

1. 클릭 **그래프** 왼쪽 패널에 표시됩니다.

   ![](assets/graphs-in-left-panel.png)

   그래프 섹션이 표시됩니다.

   기본적으로 그래프 섹션에 표시되는 목표는 다음 기준으로 제한됩니다.

   * 그래프 영역에 적용된 필터.
   * 활성 및 초안 상태에 있는 목표.

1. (선택 사항) 그래프 섹션의 오른쪽 위 모서리에서 필터를 업데이트하여 표시할 정보 유형을 선택합니다.

   필터링 목표에 대한 자세한 내용은 [Adobe Workfront 목표에서 정보 필터링](../../workfront-goals/goal-management/filter-information-wf-goals.md).

   >[!TIP]
   두 개 이상의 기간을 표시하도록 선택한 경우 각 기간 동안 상태 차트(계기)와 진행 차트(라인)가 표시됩니다.

1. 목표 상태 차트를 검토할 때 아래 표에 있는 정보를 검토하십시오.

   ![](assets/gauge-graph-wf-align-350x230.png)

   | 총 목표 수 | 차트 하단의 숫자는 선택한 모든 상태에서 선택한 기간의 모든 목표 수를 나타냅니다. |
   |---|---|
   | 평균 완료율 | 차트 상단에서 이 숫자는 선택한 기간 동안 활성 및 마감된 목표에 대한 평균 완료 퍼센트를 나타냅니다. |
   | 목표 및 진행 상황 | 마우스로 차트의 세그먼트를 가리키면 각 진행률 상태 세그먼트에 대한 목표 수가 표시됩니다. 활성 또는 닫힌 상태의 목표만 세그먼트에서 계산됩니다. |


1. 목표 진행 차트를 검토할 때 아래 표의 정보를 검토하십시오.

   ![](assets/line-graph-wf-align-350x161.png)

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td>기준선 진행</td> 
      <td>녹색 기울기 선은 선택한 기간 동안 활성 및 닫힌 목표에 대한 예상 전체 완료율 평균을 나타냅니다. 기간 내의 모든 목표는 완료되어야 하므로 기간 종료 시 기본 진행 상태는 항상 100%입니다. </td> 
     </tr> 
     <tr> 
      <td>실제 진행률</td> 
      <td> <p>파란색 선은 선택한 기간(주별 증가)에 대해 활성 및 닫힌 목표의 실제 전체 백분율 완료 평균을 나타냅니다. 목표의 기간 동안 매주 라인 내의 노드에 의해 표시됩니다. </p> </td> 
     </tr> 
    </tbody> 
   </table>

1. 목표 진행 차트에서 주 노드를 마우스로 가리킨 다음 다음을 검토합니다.

   * **주 날짜**: 선택한 주의 월, 일 및 연도입니다.
   * **진행률**: 선택한 주에 대한 모든 목표에 대한 실제 완료율의 평균입니다.
   * **기준선**: 선택한 주의 모든 목표에 대한 예상 완료율의 평균입니다.

1. (선택 사항) **진행률** 진행 차트 하단에서 실제 전체 진행 라인을 제거하려면

   또는

   클릭 **기준선** 진행률 차트 하단에서 예상되는 진행 상황을 차트에서 제거합니다.

 
