---
product-previous: workfront-goals
navigation-topic: goal-management
title: Adobe Workfront 목표에서 문제가 있는 목표 검토
description: 문제가 되는 진행 중인 도메인이 달성되지 못할 위험이 있으며, Adobe Workfront 목표에 있는 빨간색 진행률 표시줄로 표시됩니다. 목표를 자주 검토하고 진행이 지연된 이유를 이해해야 합니다.
author: Alina
feature: Workfront Goals
exl-id: df2cdc12-9102-4759-9daa-1f8ae68f110b
source-git-commit: 1d221d10e5845e477dff825f853330b9b4df0adf
workflow-type: tm+mt
source-wordcount: '794'
ht-degree: 0%

---

# Adobe Workfront 목표에서 문제가 있는 목표 검토

<!--
<p>(NOTE: the status of goals in "red" used to be called At Risk. Now, it is "in trouble") </p>
-->

문제가 되는 진행 중인 목표가 달성되지 못할 위험에 있으며, Adobe Workfront 목표에 빨간색 진행률 표시줄로 표시됩니다. 목표를 자주 검토하고 진행이 지연된 이유를 이해해야 합니다. 목표 진행에 대한 자세한 내용은 [Adobe Workfront 목표의 목표 진행 및 조건 개요](../../workfront-goals/goal-management/calculate-goal-progress.md).

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

&#42;어떤 계획, 라이선스 유형 또는 액세스 권한을 보유하고 있는지 알아보려면 Workfront 관리자에게 문의하십시오.

## 전제 조건

시작하려면 먼저 다음을 수행해야 합니다.

* 기본 메뉴의 목표 영역을 포함하는 레이아웃 템플릿.

## 문제의 진행 상황에 도달하는 목표를 방지하기 위한 Recommendations

목표가 문제 발생 단계에 도달하기 전에 이러한 목표를 자주 모니터링하고 위험 발생 시 진행 상황을 조정할 수 있습니다. 위험에 처한 목표들은 곤경에 빠질 위험에 처해 있다. 목표 진행에 대한 자세한 내용은 [Adobe Workfront 목표의 목표 진행 및 조건 개요](../../workfront-goals/goal-management/calculate-goal-progress.md)

목표가 문제 발생 단계에 도달하기 전에 다음 사항을 권장합니다.

* 위험 상태에 있는 목표 검토 및 목표 진행에 영향을 받을 수 있는 팀, 그룹 또는 조직에 할당된 조직 목표도 검토합니다. 위험에 처한 목표들이 곤경에 처한 목표가 될 위험에 처해 있다. 위험 발생 시 목표는 노란색 진행률 표시줄에 표시됩니다. 목표 목록을 사용하여 사용자, 팀, 그룹 또는 조직에 속한 목표를 봅니다.


## 목표 목록에서 문제 내 목표 검토

Workfront 목표 의 섹션에서 목표를 검토할 수 있습니다. Workfront 목표 섹션에 대한 자세한 내용은 [Adobe Workfront 목표 섹션 개요](../../workfront-goals/goal-review-and-workfront-goals-sections/overview-of-wf-goals-sections.md).

이 문서에서는 목표 목록에서 목표를 검토하는 방법을 설명합니다.

1. 을(를) 클릭합니다. **기본 메뉴** 아이콘 ![](assets/main-menu-icon.png) > **목표** 오른쪽 상단 모서리에서

   <!-- Add this when Shell is available to all: or (if available), click the **Main Menu** icon ![Main menu icon](../goal-management/assets/three-line-main-menu-icon.png) in the upper-left corner)
   -->

   이렇게 하면 Workfront 목표 영역이 열리고 목표 목록 섹션이 기본적으로 표시됩니다.

1. (권장) 목표 목록 영역에 대해 다음 필터를 조정하여 위험 시 목표를 검토합니다.

   * 클릭 **회사**, 그런 다음 **내 팀**, 그런 다음 **내 그룹**, 그런 다음 **개인** 조직의 목표, 팀, 그룹 및 목표에 속하는 목표를 보기 위해 이 목표를 사용합니다.

      >[!TIP]
      >
      >Adobe Workfront 목표에서 회사 필터는 조직이 소유자로 선택되는 목표를 표시합니다.
      >
      >
      >이 필드를 사용하여 회사를 검색할 수 없습니다. 기본적으로 Workfront 인스턴스의 소유자인 조직만 선택됩니다.

   * 위에서 선택하는 각 조직 단위에 대해 **새 필터** > **진행률** > **문제 발생** >**적용.**
   * (선택 사항) 목표를 보려는 기간을 선택합니다.

      진행률 표시줄 표시기는 목표 목록의 각 목표에 대해 빨간색으로 표시됩니다.

      오른쪽 패널에서 다른 모든 기준을 사용하여 목표를 필터링하는 방법에 대한 자세한 내용은 [Adobe Workfront 목표에서 정보 필터링](../../workfront-goals/goal-management/filter-information-wf-goals.md).

1. 진행률 표시줄 표시기 위로 마우스를 가져가면 실제 진행 비율이 무엇이고 현재 날짜에 대해 예상되는 값이 표시됩니다.

   ![](assets/goal-progress-hover-over-detail-unshimmed.png)

1. (선택 사항) 필터를 사용하여 특정 소유자에 속하는 목표를 찾습니다.

   선택한 사용자에 대한 문제 해결 목표가 목표 목록에 표시됩니다.

1. 목표 이름을 클릭하여 목표 페이지를 연 다음, **진행률 표시기** 왼쪽 패널에 표시됩니다. 목표가 뒤로 오는 진행률 표시기를 보고 인라인으로 표시되는 진행 상황을 업데이트합니다 **실제 진행률** 진행 표시기 목록의 열입니다.

   결과 및 활동 업데이트에 대한 자세한 내용은 [Adobe Workfront 목표에서 목표 진행 상태 업데이트](../goal-review-and-workfront-goals-sections/check-in-goals.md)

   ![](assets/actual-progress-editable-column-in-indicator-list-unshimmed.png)

   >[!NOTE]
   >
   >진행 지표 목록에서 결과와 활동만 업데이트할 수 있습니다. 목표에 액세스하여 하위 목표의 진행 상태 표시기를 업데이트해야 하며, 연결된 프로젝트의 작업을 갱신하여 프로젝트의 진행 상태를 업데이트해야 합니다.


