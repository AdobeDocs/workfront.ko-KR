---
product-previous: workfront-goals
navigation-topic: goal-management
title: Adobe Workfront 목표에서 문제 해결 목표 검토
description: 문제가 진행 중인 목표 는 달성되지 못할 위험이 있으며 Adobe Workfront 목표의 빨간색 진행률 표시줄에 표시됩니다. 목표를 자주 검토하고 진행 상황이 느린 이유를 이해해야 합니다.
author: Alina
feature: Workfront Goals
exl-id: df2cdc12-9102-4759-9daa-1f8ae68f110b
source-git-commit: dbc4404501e20b3f1905a5eebd13734a65db27ae
workflow-type: tm+mt
source-wordcount: '748'
ht-degree: 2%

---

# Adobe Workfront 목표에서 문제 발생 목표 검토

<!--Audited: 4/2025-->

<!--
<p>(NOTE: the status of goals in "red" used to be called At Risk. Now, it is "in trouble") </p>
-->

문제가 진행 중인 목표는 달성되지 못할 위험이 있으며 Adobe Workfront 목표의 빨간색 진행률 표시줄이 표시됩니다. 목표를 자주 검토하고 진행 상황이 느린 이유를 이해해야 합니다. 목표 진행 상황에 대한 자세한 내용은 [Adobe Workfront 목표의 목표 진행 상황 및 상태 개요](../../workfront-goals/goal-management/calculate-goal-progress.md)를 참조하십시오.

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
 <td role="rowheader">Access level</td>
 <td> <p>Edit access to Goals</p></td>
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

## 목표 달성 시 문제 상황 진행에 도달하지 않도록 하기 위한 권장 사항

목표 진행 상황에 도달하기 전에 목표 진행 상황을 자주 모니터링하고 목표 진행 상황에 도달할 때 진행 상황을 조정할 수 있습니다. 위험에 처한 목표는 곤경에 빠질 위험이 있다. 목표 진행 상황에 대한 자세한 내용은 [Adobe Workfront 목표의 목표 진행 상황 및 상태 개요](../../workfront-goals/goal-management/calculate-goal-progress.md)를 참조하십시오.

목표 달성이 문제 상황으로 진행되기 전에 다음 사항을 권장합니다.

* 사용자에게 종종 할당된 위험 상태의 목표와 목표 진행에 영향을 받을 수 있는 팀, 그룹 또는 조직에 할당된 조직 목표를 검토하십시오. 위험에 처한 목표가 곤경에 처한 목표가 될 위험에 처해 있다. 위험 상태의 목표는 노란색 진행률 표시줄로 표시됩니다. 목표 목록을 사용하여 사용자, 팀, 그룹 또는 조직에 속한 목표를 봅니다.


## 목표 목록에서 문제 발생 목표 검토

Workfront 목표의 모든 섹션에서 목표를 검토할 수 있습니다. Workfront 목표 섹션에 대한 자세한 내용은 [Adobe Workfront 목표 섹션 개요](../../workfront-goals/goal-review-and-workfront-goals-sections/overview-of-wf-goals-sections.md)를 참조하십시오.

이 문서에서는 목표 목록에서 목표를 검토하는 방법을 설명합니다.

{{step1-to-goals}}

Workfront 목표 영역이 열리고 기본적으로 목표 목록 섹션이 표시됩니다.

1. (권장) 위험 상태의 목표를 검토하려면 목표 목록 영역에 대해 다음 필터를 조정합니다.

   * 조직, 팀, 그룹, 자신의 목표를 보려면 **회사**, **내 팀**, **내 그룹**, **개인** 목표를 클릭하십시오.

     >[!TIP]
     >
     >Adobe Workfront 목표에서 회사 필터는 조직이 소유자로 선택된 목표를 표시합니다.
     >
     >
     >이 필드를 사용하여 회사를 검색할 수 없습니다. Workfront 인스턴스의 소유자인 조직만 기본적으로 선택됩니다.

   * 위에서 선택한 각 조직 단위에 대해 **새 필터** > **진행** > **문제 발생** >**적용**&#x200B;을 클릭합니다.
   * (선택 사항) 목표를 보려는 기간을 선택합니다.

     진행률 표시줄 표시기는 목표 목록의 각 목표에 대해 빨간색으로 표시됩니다.

     오른쪽 패널의 다른 모든 기준을 사용하여 목표를 필터링하는 방법에 대한 자세한 내용은 [Adobe Workfront 목표의 정보 필터링](../../workfront-goals/goal-management/filter-information-wf-goals.md)을 참조하십시오.

1. 진행률 표시줄 표시기 위로 마우스를 가져가 실제 진행률 및 현재 날짜의 예상 값을 확인합니다.

   ![진행 상황 가리키기 세부 정보](assets/goal-progress-hover-over-detail-unshimmed.png)

1. (선택 사항) 필터를 사용하여 특정 소유자에게 속한 목표를 찾습니다.

   선택한 사용자의 문제 해결 목표가 목표 목록에 표시됩니다.

1. 목표 이름을 클릭하여 목표 페이지를 연 다음 왼쪽 패널에서 **진행 표시기**&#x200B;를 클릭합니다. 진행 표시기 목록의 **실제 진행** 열에서 목표가 지연되는 진행 표시기를 보고 표시기의 진행 상황을 인라인으로 업데이트합니다.

   결과 및 활동 업데이트에 대한 자세한 내용은 [Adobe Workfront 목표의 목표 진행률 업데이트](../goal-review-and-workfront-goals-sections/check-in-goals.md)를 참조하세요.

   ![실제 진행 상황](assets/actual-progress-editable-column-in-indicator-list-unshimmed.png)

   >[!NOTE]
   >
   >진행 표시기 목록의 결과 및 활동만 업데이트할 수 있습니다. 목표에 액세스하여 1차 하위 구성요소 목표의 진행률 지표를 갱신해야 하며, 연결된 프로젝트의 작업을 갱신하여 프로젝트의 진행률을 갱신해야 합니다.


