---
product-previous: workfront-goals
navigation-topic: goal-alignment
title: Adobe Workfront 목표의 목표 정렬 섹션 탐색
description: '[목표 정렬] 섹션을 사용하여 순서에서 전체 조직에 대한 목표 정렬을 전체적으로 볼 수 있습니다. 정렬된 목표는 계층 트리에서 상호 연결되는 카드에 표시됩니다.'
author: Alina
feature: Workfront Goals
exl-id: e79ced31-4680-4af7-b083-3d615c747af8
source-git-commit: 09e34ecdfeec531ebbaaba4fb8682496c53d86bf
workflow-type: tm+mt
source-wordcount: '921'
ht-degree: 1%

---

# Adobe Workfront 목표의 목표 정렬 섹션 탐색

[목표 정렬] 섹션을 사용하여 순서에서 전체 조직에 대한 목표 정렬을 전체적으로 볼 수 있습니다. 정렬된 목표는 계층 트리에서 상호 연결되는 카드에 표시됩니다.

목표 정렬 및 달성 방법에 대한 자세한 내용은 다음 문서를 참조하십시오.

* [Adobe Workfront 목표의 목표 정렬 개요](../../workfront-goals/goal-alignment/goal-alignment-overview.md)
* [Adobe Workfront 목표에서 연결하여 목표 정렬](../../workfront-goals/goal-alignment/align-goals-by-connecting-them.md)

## 액세스 요구 사항

이 문서에 설명된 활동을 수행하려면 다음이 있어야 합니다.

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
<p>현재 라이선스: 요청 이상</p>  </td>
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
<tr>
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

## 목표 정렬 섹션 탐색

1. 다음을 클릭합니다. **메인 메뉴** 아이콘 ![메인 메뉴 아이콘](../goal-alignment/assets/dots-main-menu-icon.png) 화면의 오른쪽 상단에서 을(를) 클릭한 다음 **목표**.
   <!-- Add this when Shell is available to all: or (if available), click the **Main Menu** icon ![Main menu icon](../goal-alignment/assets/three-line-main-menu-icon.png) in the upper-left corner)
   -->
1. 클릭 **목표 정렬** 왼쪽 패널에서
1. 정렬 차트의 오른쪽 위 모서리에 있는 필터를 사용하여 중요한 목표만 선택합니다. Workfront 목표에서 필터를 사용하는 방법에 대한 자세한 내용은 다음을 참조하십시오. [Adobe Workfront 목표의 정보 필터링](../../workfront-goals/goal-management/filter-information-wf-goals.md).

   필터와 일치하는 목표가 카드의 정렬 차트에 표시됩니다.

   목표 카드에 다음 정보가 표시됩니다.

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">기간 날짜 </td> 
      <td> <p>목표가 열려 있는 기간입니다. 목표는 기간 종료일까지 달성해야 합니다. Workfront 목표는 목표의 기간 및 현재 날짜를 기반으로 목표에 대한 진행률을 계산합니다.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">진행 표시기</td> 
      <td>목표에 대한 진행 표시기 수입니다. 진행률 지표는 목표, 결과 또는 활동에 정렬될 수 있습니다. </td> 
     </tr> 
     <tr> 
      <td role="rowheader">소유자 이름</td> 
      <td>목표 소유자로 지정된 사용자, 팀, 그룹 또는 조직의 이름입니다. </td> 
     </tr> 
     <tr> 
      <td role="rowheader">목표 이름</td> 
      <td>목표의 이름입니다. </td> 
     </tr> 
     <tr> 
      <td role="rowheader">목표 진행률 표시줄 <span>및 진행</span></td> 
      <td> <p>목표 진행률은 현재 얼마나 많은 목표를 달성했는지를 나타냅니다. 목표 기간 시작 이후 경과된 시간을 기준으로 목표에 대한 모든 정렬된 목표, 결과 및 활동의 진행 평균을 자동으로 계산합니다. 목표에 대한 진행률 계산에 대한 자세한 내용은 <a href="../../workfront-goals/goal-management/calculate-goal-progress.md" class="MCXref xref">Adobe Workfront 목표의 목표 진행 및 상태 개요</a>. </p> 
       <div> 
        <p>현재 날짜까지 목표의 실제 진행 상황입니다. 다음 진행률 값과 색상은 목표가 정시에 달성되는 정도를 나타냅니다. </p> 
        <ul> 
         <li><span>대상</span> (녹색 표시기): 목표는 정시에 달성되며 정시에 달성됩니다.</li> 
         <li> <span>위험 상태</span> (노란색 지표): 목표가 늦어지고 기한 내에 달성되지 않을 수 있습니다.</li> 
         <li> <span>문제 발생</span> (빨간색 표시기): 목표가 제때 달성되지 못할 위험이 있습니다. </li> 
        </ul> 
       </div> </td> 
     </tr> <!--
      <tr data-mc-conditions="QuicksilverOrClassic.Draft mode"> 
       <td role="rowheader">Updated on date </td> 
       <td> <p>The date when the goal was last updated</p> <p>(NOTE: drafted because I think this was removed with the alignment chart redesign - 21.1) </p> </td> 
      </tr>
     --> 
     <tr> 
      <td role="rowheader">상태</td> 
      <td><span>모든 상태의 목표가 목표 정렬 섹션에 표시됩니다.</span> </td> 
     </tr> 
    </tbody> 
   </table>

   다른 목표와 정렬된 목표에는 목표 카드 아래에 정렬된 목표의 수가 표시됩니다.

   ![](assets/alignment-chart-arrow-for-aligned-goals-highlighted-350x241.png)

1. 다음을 클릭합니다. **아래쪽 방향 화살표** 을 클릭하여 하위 목표를 더 확장하고 볼 수 있습니다.

   ![](assets/alignment-chart-arrow-for-aligned-goals-highlighted-350x241.png)

   >[!TIP]
   >
   >하위 목표가 정렬된 목표는 해당 카드 아래에 정렬된 목표의 수를 표시합니다.

1. (조건부) 현재 필터가 정렬에 참여하는 목표 중 일부를 제외하는 경우 일부 목표가 표시되지 않는다는 경고 메시지가 표시됩니다.

   ![](assets/parent-goal-excluded-by-filter-alignment-section-350x230.png)

1. 클릭 **해당 항목 표시** 현재 필터에서 제거된 목표를 표시합니다.

   정렬 차트에서 다음 변경 사항을 확인합니다.

   * 필터에서 이전에 제거한 연결된 목표가 이제 정렬 차트에 표시됩니다.
   * 오른쪽 위 모서리의 필터는 현재 적용되지 않았음을 나타내기 위해 노란색으로 윤곽선이 표시되어 있습니다.

     ![](assets/reapply-filter-link-and-yellow-filter-highlight-350x120.png)

     필터 이름 왼쪽에 필터 재적용 링크가 표시됩니다.

1. (선택 사항) **필터 다시 적용** 원래 결과로 돌아가서 목표 계층을 표시합니다.
1. (선택 사항) 진행 표시기 위로 마우스를 가져가면 현재 날짜의 목표 진행 상황을 파악할 수 있습니다.

   ![](assets/progress-mouse-over-alignment-chart-350x163.png)

   다음 정보가 표시됩니다.

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">오늘 기준</td> 
      <td>진행 상태는 항상 최신입니다. </td> 
     </tr> 
     <tr> 
      <td role="rowheader"><span>실제</span> </td> 
      <td>목표에 대한 모든 진행 표시기를 고려하여 계산된 현재 날짜별 목표의 실제 진행 상황(백분율)입니다. 목표 진행 지표는 정렬된 목표, 활동 및 결과입니다. </td> 
     </tr> 
     <tr> 
      <td role="rowheader">예상</td> 
      <td> <p>정시에 목표를 달성한다고 가정할 때 현재 날짜까지 목표의 예상 진행률(백분율)입니다.</p> </td> 
     </tr> 
    </tbody> 
   </table>

1. 목표 카드를 클릭하여 목표 페이지를 엽니다. 기존 목표 편집에 대한 자세한 내용은 [Adobe Workfront 목표의 목표 편집](../../workfront-goals/goal-management/edit-goals.md). 목표에 대한 진행률 업데이트에 대한 자세한 내용은 다음을 참조하십시오. [Adobe Workfront 목표의 목표 진행 상황 업데이트](../../workfront-goals/goal-review-and-workfront-goals-sections/check-in-goals.md).

1. 현재 수준 목표의 위쪽 방향 화살표를 클릭하여 차트의 계층에서 이전 수준으로 돌아갑니다.

   또는

   (선택 사항) **목표 계층 종료** 서로 간의 연결을 표시하지 않고 현재 필터와 일치하는 모든 목표의 카드를 표시합니다.


