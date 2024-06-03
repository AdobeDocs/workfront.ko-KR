---
product-previous: workfront-goals
navigation-topic: goal-alignment
title: Adobe Workfront 목표에서 연결하여 목표 정렬
description: 개인 목표가 있는 개별 기여자의 경우 조직의 전략의 더 큰 컨텍스트에서 자체 목표의 진행 상황을 효과적으로 표시하기 위해 목표를 팀의 목표에 맞출 수 있습니다.
author: Alina
feature: Workfront Goals
exl-id: 4276f1c9-2ee9-4f74-b011-ae1e19fefe35
source-git-commit: 330ee20ad14ea7409db1c6f627ed6aa0e0c5c014
workflow-type: tm+mt
source-wordcount: '765'
ht-degree: 1%

---

# Adobe Workfront 목표에서 연결하여 목표 정렬

개인 목표가 있는 개별 기여자의 경우 조직의 전략의 더 큰 컨텍스트에서 자체 목표의 진행 상황을 효과적으로 표시하기 위해 목표를 팀의 목표에 맞출 수 있습니다.

조직의 모든 구성원이 조직의 목표에 맞게 목표를 수립한 경우 개별 기여와 팀의 노력이 회사 수준의 더 큰 우선순위에서 바늘을 향해 나아가는 데 어떻게 도움이 되는지 명확하게 확인할 수 있습니다. 목표 정렬을 위한 모범 사례에 대한 자세한 내용은 다음을 참조하십시오. [Adobe Workfront 목표의 목표 정렬 개요](../../workfront-goals/goal-alignment/goal-alignment-overview.md).

Adobe Workfront 목표에는 두 가지 접근 방식으로 목표를 연결할 수 있습니다.

* 목표를 서로 연결하여 목표 간의 정렬을 만들 수 있습니다.

* 두 목표를 수동으로 정렬하거나 기존 목표의 결과 및 활동을 다른 목표로 변환할 수 있습니다. 전환된 결과나 활동이 원래 목표의 하위 목표가 됩니다.

>[!IMPORTANT]
>
>목표는 총 1000개의 진행 표시기를 가질 수 있습니다.

이 문서에서는 목표를 서로 연결하여 정렬하는 방법을 설명합니다. 결과 및 활동을 목표로 변환하여 목표를 정렬하는 방법에 대한 자세한 내용은 다음을 참조하십시오. [결과 및 활동을 목표로 변환하여 목표 정렬](../../workfront-goals/goal-alignment/align-goals-by-converting-results-activities.md).

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
 <p>현재 라이선스: 요청 이상</p> </td>
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
 <tr>
 <td role="rowheader">개체 권한</td>
 <td>

<p>목표에 대한 또는 그 이상의 권한에 대한 보기</p>
  <p>편집할 목표에 대한 권한 관리</p>
  <p>목표 공유에 대한 자세한 내용은 <a href="../../workfront-goals/workfront-goals-settings/share-a-goal.md" class="MCXref xref">Workfront 목표에서 목표 공유</a>. </p>
   </td>
 </tr>
<tr>
   <td role="rowheader"><p>레이아웃 템플릿</p></td>
   <td> <p>Workfront 관리자를 포함한 모든 사용자에게 메인 메뉴의 목표 영역을 포함하는 레이아웃 템플릿을 할당해야 합니다. </p>  
</td>
  </tr>
</tbody>
</table>

*자세한 내용은 [Workfront 설명서의 액세스 요구 사항](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

## 목표를 서로 연결하여 정렬

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
1. 조정할 두 가지 목표를 만듭니다. 목표 작성에 대한 자세한 내용은 [Adobe Workfront 목표에서 목표 만들기](../../workfront-goals/goal-management/create-goals.md).
1. (선택 사항) 정렬하려는 목표를 활성화합니다. 초안, 활성 또는 비활성 상태인 목표를 정렬할 수 있습니다. 목표 활성화에 대한 자세한 내용은 다음을 참조하십시오. [Adobe Workfront 목표에서 목표 활성화](../../workfront-goals/goal-management/activate-goals.md).
1. (하위 목표)를 다른 목표 (상위 목표)에 정렬하려는 목표로 이동한 다음 해당 이름을 클릭하여 목표 페이지를 엽니다.

   >[!INFO]
   >
   >예를 들어 목표 2가 목표 1의 진행 상황에 영향을 미치도록 하려면 목표 2로 이동해야 합니다.

1. 클릭 **목표 세부 정보** 왼쪽 패널에서

1. 다음에서 **상위 목표 정보** 영역, 클릭 **추가** 다음에서 **상위 목표** 필드: 상위 목표가 없으면

   또는

   상위 목표의 이름을 클릭하여 다른 목표를 선택합니다.

1. 에 기존 목표의 이름을 입력하십시오. **상위 목표** 필드를 선택한 다음 목록에 나타나면 선택합니다. 동일한 기간 또는 미래 기간의 목표만 목록에 표시됩니다.

1. **변경 내용 저장**&#x200B;을 클릭합니다.

   (목표 2)로 시작한 목표가 (목표 1)로 정렬한 상위 목표의 하위 목표입니다.\
   정렬된 목표는 목표 1에 대한 보조로 목표 2를 사용하여 목표 정렬 섹션에 연결됩니다.
하위 목표가 상위 목표의 진행 상황을 업데이트할 때 상위 목표의 진행 상황 표시기 섹션에 표시됩니다.

   ![](assets/goal-1-and-2-aligned-cards-350x427.png)

1. (선택 사항) 목표 정렬 섹션에서 목표를 보려면 Workfront의 목표 영역으로 이동한 다음, **목표 정렬** 왼쪽 패널의 섹션입니다. 목표 정렬 섹션에 대한 자세한 내용은 [Adobe Workfront 목표의 목표 정렬 섹션 탐색](../../workfront-goals/goal-alignment/navigate-goal-alignment-chart.md).

1. (선택 사항) 두 목표 중 하나에 활동 및 결과를 추가하여 진행 상황을 나타냅니다. 활동 및 결과 추가에 대한 자세한 내용은 다음 문서를 참조하십시오.

   * [Adobe Workfront 목표의 목표에 활동 추가](../../workfront-goals/results-and-activities/add-activities-to-goals.md)
   * [Adobe Workfront 목표의 목표에 결과 추가](../../workfront-goals/results-and-activities/add-results-to-goals.md)

1. (선택 사항) 조직의 전체 전략과 더 이상 관련이 없다고 고려할 때 두 목표 간의 정렬을 제거합니다. 목표 간 정렬 제거에 대한 자세한 내용은 [Adobe Workfront 목표에서 목표 정렬 제거](../../workfront-goals/goal-alignment/remove-goal-alignment.md).

