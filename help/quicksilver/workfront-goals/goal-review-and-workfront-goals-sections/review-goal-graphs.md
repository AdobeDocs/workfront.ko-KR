---
product-previous: workfront-goals
navigation-topic: goal-review-and-sections
title: 그래프를 검토하여 Adobe Workfront 목표의 목표 진행 트렌드를 파악합니다
description: Adobe Workfront 목표의 그래프 섹션에서 목표의 전반적인 상태와 목표 진행률 추세를 시간별로 볼 수 있습니다. 이 섹션의 차트는 각 목표의 진행 상황을 분류하지 않고 대신 모든 목표의 진행 상태와 지정된 기간 동안의 진행 추세에 대한 전체적인 스냅샷을 제공합니다.
author: Alina
feature: Workfront Goals
exl-id: 8d5f3617-c7bf-44ce-99b0-d4ebda106f25
source-git-commit: dbc4404501e20b3f1905a5eebd13734a65db27ae
workflow-type: tm+mt
source-wordcount: '899'
ht-degree: 2%

---

# 그래프를 검토하여 Adobe Workfront 목표의 목표 진행 트렌드를 파악합니다

<!--Audited for P&P only: 4/2025-->

Adobe Workfront 목표의 그래프 섹션에서 목표의 전반적인 상태와 목표 진행률 추세를 시간별로 볼 수 있습니다. 이 섹션의 차트는 각 목표의 진행 상황을 분류하지 않고 대신 모든 목표의 진행 상태와 지정된 기간 동안의 진행 추세에 대한 전체적인 스냅샷을 제공합니다.

>[!IMPORTANT]
>
>선택한 기간 동안의 그래프 섹션에서 목표에 대한 총 개수를 볼 수 있습니다. 그러나 Workfront 목표는 전체 목표 진행 상태 및 완료율을 계산할 때 활성 및 마감됨 상태의 목표만 고려합니다.

## 액세스 요구 사항

>[!NOTE]
>
>이전에 이 패키지를 구입한 경우 귀사에서 Adobe Workfront 목표를 계속 사용하도록 선택할 수 있습니다. 자세한 내용은 계정 담당자에게 문의하십시오.
>
>Adobe Workfront 목표를 더 이상 구매할 수 없습니다.

+++ 이 문서의 기능에 대한 액세스 요구 사항을 보려면 확장하십시오. 

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
<p>요청 이상</p></td>
 </tr>
  <tr>
 <td role="rowheader">액세스 수준 구성</td>
 <td> <p>목표에 대한 액세스 편집</p> </td>
 </tr>
 <tr data-mc-conditions="">
 <td role="rowheader">개체 권한</td>
 <td>
  <div>
  <p>목표에 대한 또는 그 이상의 권한에 대한 보기</p>
  <p>편집할 목표에 대한 권한 관리</p>
  </div> </td>
 </tr>
<tr>
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
 <p>Current license: Request or higher</p> <p>For more information, see <a href="../../administration-and-setup/add-users/access-levels-and-object-permissions/wf-licenses.md" class="MCXref xref">Adobe Workfront licenses overview</a>.</p> </td>
 </tr>
 <tr>
 <td role="rowheader">Product*</td>
 <td>
    <p> New product requirement: Workfront</p>
    Or
    <p>Current product requirement: In addition to a Workfront license, you must purchase a license for Adobe Workfront Goals. </p> <p>For information, see <a href="../../workfront-goals/goal-management/access-needed-for-wf-goals.md" class="MCXref xref">Requirements to use Workfront Goals</a>. </p> </td>
 </tr>
 <tr>
 <td role="rowheader"><p>Access level</p></td>
 <td> <p>Edit access to Goals</p> </td>
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
 <tr>
   <td role="rowheader"><p>Layout template</p></td>
   <td> <p>All users, including Workfront administrators,  must be assigned a layout template that includes the Goals area in the Main Menu. </p>  
</td>
  </tr>
</tbody>
</table>-->

## Workfront 목표의 그래프 유형

그래프 섹션 또는 Workfront 목표에서 다음 차트를 사용할 수 있습니다.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">목표 상태 차트</td> 
   <td> <p>다음을 표시하는 측정 차트:</p> 
    <ul> 
     <li>선택한 기간 동안의 총 목표 수입니다. 모든 상태의 목표를 고려합니다. </li> 
     <li>활성 및 마감됨 상태의 목표 진행 상태입니다.</li> 
    </ul> <p>Workfront Goals가 진행 상태를 계산하는 방법에 대한 자세한 내용은 <a href="../../workfront-goals/goal-management/calculate-goal-progress.md" class="MCXref xref">Adobe Workfront Goals의 목표 진행 및 상태 개요</a>를 참조하십시오.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">목표 진행률 차트</td> 
   <td> <p>목표 기간 동안 주간 단위로 목표에 대한 업데이트를 표시하는 라인 차트입니다. 목표 진행률 차트는 다음을 표시합니다.</p> 
    <ul> 
     <li>선택한 기간 내 모든 활성 및 마감된 목표의 평균 예상 및 실제 완료율. 완료율 진행률은 노드로 표시된 주별 증분으로 분류됩니다. </li> 
     <li>이전 주 이후 활성 및 마감된 목표에 대한 전체 평균 진행률. </li> 
    </ul> <p>팁: 목표 진행 차트는 선택한 기간 이외의 목표를 업데이트할 때 정보를 표시하지 않을 수 있습니다. </p> </td> 
  </tr> 
 </tbody> 
</table>

## 그래프로 목표 진행 상황 검토

{{step1-to-goals}}

그러면 Workfront 목표 영역이 열립니다.

1. 왼쪽 패널에서 **그래프**&#x200B;를 클릭합니다.

   왼쪽 패널의 ![그래프](assets/graphs-in-left-panel.png)

   그래프 섹션이 표시됩니다.

   그래프 섹션에 표시되는 목표는 기본적으로 다음 기준에 의해 제한됩니다.

   * 그래프 영역에 적용된 필터.
   * 활성 및 초안 상태의 목표입니다.

1. (선택 사항) 그래프 섹션의 오른쪽 상단에 있는 필터를 업데이트하여 표시할 정보 유형을 선택합니다.

   필터링 목표에 대한 자세한 내용은 [Adobe Workfront 목표의 정보 필터링](../../workfront-goals/goal-management/filter-information-wf-goals.md)을 참조하십시오.

   >[!TIP]
   >
   >두 개 이상의 기간을 표시하도록 선택한 경우 각 기간에 대해 상태 차트(측정)와 진행률 차트(선)가 표시됩니다.

1. 목표 상태 차트를 검토할 때 아래 표의 정보를 검토하십시오.

   ![게이지 그래프](assets/gauge-graph-wf-align-350x230.png)

   | 총 목표 수 | 차트 하단의 숫자는 선택한 모든 상태에서 선택한 기간의 모든 목표 수를 나타냅니다. |
   |---|---|
   | 평균 완료율 | 차트의 맨 위에 있는 이 숫자는 선택한 기간 동안 활성 목표와 마감된 목표의 평균 완료율을 나타냅니다. |
   | 목표 및 진행 상황 | 차트의 세그먼트 위로 마우스를 가져갈 때 각 진행 상태 세그먼트에 대한 목표 수입니다. 활성 또는 종료됨 상태의 목표만 세그먼트에서 계산됩니다. |


1. 목표 진행률 차트를 검토할 때 아래 표의 정보를 검토하십시오.

   ![선 그래프](assets/line-graph-wf-align-350x161.png)

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td>기준선 진행률</td> 
      <td>녹색 기울기 선은 선택한 기간 동안 활성 목표와 마감된 목표의 예상 전체 완료율 평균을 나타냅니다. 기간 내의 모든 목표가 완료되어야 하므로 기간이 끝나면 항상 기준선 진행률이 100%입니다. </td> 
     </tr> 
     <tr> 
      <td>실제 진행 상황</td> 
      <td> <p>파란색 선은 선택한 기간 동안 주별 증분으로 활성 및 마감된 목표의 실제 전체 완료 퍼센트 평균을 나타냅니다. 목표 기간 동안 매주 줄에 노드가 표시됩니다. </p> </td> 
     </tr> 
    </tbody> 
   </table>

1. 목표 진행률 차트에서 주 노드를 마우스로 가리키고 다음을 검토합니다.

   * **주 날짜**: 선택한 주의 월, 일, 년입니다.
   * **진행**: 선택한 주에 대한 모든 목표의 실제 완료율 평균입니다.
   * **기준선**: 선택한 주에 대한 모든 목표의 예상 완료율의 평균입니다.

1. (선택 사항) 진행률 차트의 맨 아래에 있는 **진행률**&#x200B;을 클릭하여 실제 전체 진행률을 제거합니다.

   또는

   진행률 차트의 맨 아래에 있는 **기준선**&#x200B;을 클릭하여 차트에서 예상되는 진행률을 제거합니다.


