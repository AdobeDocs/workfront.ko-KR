---
product-previous: workfront-goals
navigation-topic: goal-review-and-sections
title: 그래프를 검토하여 Adobe Workfront 목표의 목표 진행 트렌드를 파악합니다
description: Adobe Workfront 목표의 그래프 섹션에서 목표의 전반적인 상태와 목표 진행률 추세를 시간별로 볼 수 있습니다. 이 섹션의 차트는 각 목표의 진행 상황을 분류하지 않고 대신 모든 목표의 진행 상태와 지정된 기간 동안의 진행 추세에 대한 전체적인 스냅샷을 제공합니다.
author: Alina
feature: Workfront Goals
exl-id: 8d5f3617-c7bf-44ce-99b0-d4ebda106f25
source-git-commit: 024c612d46848c55529e902a00d481588d261584
workflow-type: tm+mt
source-wordcount: '992'
ht-degree: 0%

---

# 그래프를 검토하여 Adobe Workfront 목표의 목표 진행 트렌드를 파악합니다

<!-- drafted mostly for P&P release-->

Adobe Workfront 목표의 그래프 섹션에서 목표의 전반적인 상태와 목표 진행률 추세를 시간별로 볼 수 있습니다. 이 섹션의 차트는 각 목표의 진행 상황을 분류하지 않고 대신 모든 목표의 진행 상태와 지정된 기간 동안의 진행 추세에 대한 전체적인 스냅샷을 제공합니다.

>[!IMPORTANT]
>
>선택한 기간 동안의 그래프 섹션에서 목표에 대한 총 개수를 볼 수 있습니다. 그러나 Workfront 목표는 전체 목표 진행 상태 및 완료율을 계산할 때 활성 및 마감됨 상태의 목표만 고려합니다.

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
 <td role="rowheader"><p>액세스 수준</p></td>
 <td> <p>목표에 대한 액세스 편집</p> </td>
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

1. 오른쪽 상단의 **주 메뉴** 아이콘 ![](assets/main-menu-icon.png) > **목표**&#x200B;를 클릭합니다.

   <!-- Add this when Shell is available to all: or (if available), click the **Main Menu** icon ![Main menu icon](../goal-review-and-workfront-goals-sections/assets/three-line-main-menu-icon.png) in the upper-left corner)
   -->

   그러면 Workfront 목표 영역이 열립니다.

1. 왼쪽 패널에서 **그래프**&#x200B;를 클릭합니다.

   ![](assets/graphs-in-left-panel.png)

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

   ![](assets/gauge-graph-wf-align-350x230.png)

   | 총 목표 수 | 차트 하단의 숫자는 선택한 모든 상태에서 선택한 기간의 모든 목표 수를 나타냅니다. |
   |---|---|
   | 평균 완료율 | 차트의 맨 위에 있는 이 숫자는 선택한 기간 동안 활성 목표와 마감된 목표의 평균 완료율을 나타냅니다. |
   | 목표 및 진행 상황 | 차트의 세그먼트 위로 마우스를 가져갈 때 각 진행 상태 세그먼트에 대한 목표 수입니다. 활성 또는 종료됨 상태의 목표만 세그먼트에서 계산됩니다. |


1. 목표 진행률 차트를 검토할 때 아래 표의 정보를 검토하십시오.

   ![](assets/line-graph-wf-align-350x161.png)

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

 
