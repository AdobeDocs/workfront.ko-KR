---
product-previous: workfront-goals
navigation-topic: goal-management
title: Adobe Workfront 목표의 목표 편집
description: 모든 기간 및 상태에서 기존 목표를 편집할 수 있습니다.
author: Alina
feature: Workfront Goals
exl-id: 74db534c-6897-40c2-bea9-a9d30a40f61c
source-git-commit: 024c612d46848c55529e902a00d481588d261584
workflow-type: tm+mt
source-wordcount: '647'
ht-degree: 1%

---

# Adobe Workfront 목표의 목표 편집

모든 기간 및 상태에서 기존 목표를 편집할 수 있습니다.

## 액세스 요구 사항

다음 항목이 있어야 합니다.

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
 <td role="rowheader">액세스 수준</td>
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

## 목표 편집에 대한 고려 사항

* 마감 상태의 목표는 편집할 수 없습니다.
* 모든 기간의 목표를 편집할 수 있습니다.

  과거 목표에 대한 다음 정보를 편집할 수 있습니다.

   * 이름
   * 기간
   * 상태

     >[!TIP]
     >
     >목표가 마감된 경우 다시 열면 진행률 완료율이 다시 계산됩니다. 마감된 목표는 편집할 수 없습니다.

   * 설명
   * 결과 및 활동

## 목표 편집

<!--
Editing goals differs depending on what environment you use.

### Edit goals in the Production environment

1. Go to a goal that you want to edit and click the goal name to open the **Goal Details** panel. 
1. Click the **More icon** ![](assets/more-icon.png), then click **Edit**.

   ![](assets/edit-goal-highlighted.png)

1. Update the name of the goal in the **Goal** field. 
1. Select a time period when the goal should be completed.

   Select from the following predefined options:

   * The current year
   * The quarters of the current year
   * The next two years
   * The quarters of the next two years

   Or

   Click **Define custom dates** to select a custom time frame. 

1. (Conditional) Select a start and an end date for your goal, if you clicked **Define custom dates**.

   
   <p>(NOTE: these fields don't yet have a name) </p>
   

   >[!CAUTION]
   >
   >You cannot create a goal with custom dates in the past.

1. (Optional) Click **Reset custom dates** to return to the predefined options.

   >[!TIP]
   >
   >We recommend that everyone in your organization selects the same time frames for similar goals or goals that are aligned. This provides better alignment between goals and ensures that everyone's work supports your larger organization-wide strategy.

1. Click the **Owner** field and select a new owner for the goal, if you want to indicate someone else as the owner of the goal. 
1. (Conditional) Start typing the name of a user, team, group, or the name of your organization in the **Owner** field, then select it when it displays in the list. You can have only one owner for a goal. 
1. Update the **Description** of the goal, then click **Save**.

-->

1. **주 메뉴** 아이콘 ![](assets/main-menu-icon.png)을(를) 클릭한 다음 **목표**&#x200B;를 클릭합니다.\
   목표 목록이 표시됩니다.
1. 목표를 클릭합니다.\
   목표 페이지가 표시됩니다.

   ![](assets/goal-page-unshimmed.png)

1. 다음 중 하나를 수행하여 목표에 대한 정보를 편집합니다.
   * 목표 헤더에 표시되는 필드를 클릭하여 업데이트합니다. 헤더의 일부 필드를 편집할 수 있는 것은 아닙니다.
   * 목표 이름의 오른쪽에 있는 **자세히 아이콘** ![](assets/more-icon.png)을 클릭한 다음 **편집**&#x200B;을 클릭합니다.
   * 왼쪽 패널에서 **목표 세부 사항**&#x200B;을 클릭하고 오른쪽 상단에서 **편집 아이콘** ![](assets/edit-icon.png)을 클릭한 다음 **모두 편집**&#x200B;을 클릭합니다. 목표 세부 사항 섹션의 필드 업데이트를 시작합니다.

     >[!IMPORTANT]
     >
     >위에서 언급한 영역에 표시되는 모든 필드를 편집할 수는 없습니다. Workfront은 일부 필드를 계산하며 읽기 전용입니다.

1. (조건부) 이전 단계에서 선택한 항목에 따라 목표에 대한 다음 정보를 업데이트합니다.

   * 목표 헤더에서 다음 정보를 업데이트한 다음 Enter 키를 눌러 변경 사항을 저장합니다.
      * **목표 이름**: 목표 이름을 클릭하고 새 이름을 입력하세요.
      * **소유자**: 소유자 이름을 클릭하고 사용자, 팀, 그룹 또는 회사의 이름을 입력한 다음 목록에 표시될 때 선택합니다. 목표에 대해 소유자는 한 명만 있을 수 있습니다.
   * 목표 편집 상자에서 다음 정보를 업데이트한 다음 **저장**&#x200B;을 클릭합니다.
      * **목표 이름**
      * **기간**: 목표의 기간을 업데이트하려면 클릭하십시오.\
        또는\
        목표의 **시작** 및 **종료 날짜**&#x200B;에 대한 날짜를 지정하려면 **사용자 지정 날짜 사용**&#x200B;을 선택하세요.

        >[!TIP]
        >
        >목표의 원래 기간으로 돌아가려면 **사용자 지정 날짜 사용**&#x200B;을 선택 취소하십시오.

      * **목표 소유자**
      * **설명**: 목표에 대한 정보를 추가하거나 업데이트합니다.
   * 목표 세부 사항 섹션에서 정보를 업데이트하거나 검토합니다. 자세한 내용은 [Adobe Workfront 목표의 목표 세부 정보 섹션에서 목표 업데이트](../goal-management/update-goals-in-goal-details-panel.md)를 참조하십시오.

   <!-- (should you update the title here after changing it at production??? - change it to Update goals in the goal Details section)-->

1. (선택 사항) 목표에 결과, 활동 또는 프로젝트를 추가하려면 왼쪽 패널의 **진행 표시기**를 클릭합니다. 진행 표시기를 추가하면 목표의 진행 상황을 추적할 수 있습니다.
자세한 내용은 다음 문서를 참조하십시오.
   * [Adobe Workfront 목표의 목표에 활동 추가](../results-and-activities/add-activities-to-goals.md)
   * [Adobe Workfront 목표의 목표에 결과 추가](../results-and-activities/add-results-to-goals.md).
   * [Adobe Workfront 목표의 목표에 프로젝트 추가](../results-and-activities/connect-projects-to-goals-overview.md).

</div>
