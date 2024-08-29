---
product-previous: workfront-goals
product-area: projects
navigation-topic: results-and-activities
title: Adobe Workfront 목표의 목표에서 진행 표시기 제거
description: 결과, 활동 및 프로젝트가 더 이상 관련이 없을 때 Adobe Workfront 목표의 목표에서 제거할 수 있습니다.
author: Alina
feature: Workfront Goals
exl-id: 0e064dbd-6168-47b4-98ab-b5c0481e839e
source-git-commit: d7dd5ab4e3041a100b13c5bf169747f58db0ea39
workflow-type: tm+mt
source-wordcount: '732'
ht-degree: 0%

---

# Adobe Workfront 목표의 목표에서 진행 표시기 제거

<!-- for goal redesign PRODUCTION RELEASE: Should this article be called "Remove or disconnect progress indicators from goals" when this is available to ALL progress indicators (including "disconnect goals")-- if yes, updte the title everywhere else where this is linked?
-->

결과, 활동 및 프로젝트가 더 이상 관련이 없는 경우 목표에서 제거할 수 있습니다.

목표 생성, 결과 및 활동에 대한 자세한 내용은 다음 문서를 참조하십시오.

* [Adobe Workfront 목표에서 목표 만들기](../../workfront-goals/goal-management/create-goals.md)
* [Adobe Workfront 목표의 목표에 활동 추가](../../workfront-goals/results-and-activities/add-activities-to-goals.md)
* [Adobe Workfront 목표의 목표에 결과 추가](../../workfront-goals/results-and-activities/add-results-to-goals.md)
* [Adobe Workfront 목표에서 결과 및 활동 편집](../../workfront-goals/results-and-activities/edit-results-and-activities.md)

목표는 또한 부모 목표와 일치하여 자식 목표가 될 수 있습니다. 하위 목표도 상위 목표의 진행 지표이다.

목표 사이의 연결을 제거하여 목표 사이의 정렬을 제거할 수 있습니다. 자세한 내용은 [Adobe Workfront 목표에서 목표 정렬 제거](../goal-alignment/remove-goal-alignment.md)를 참조하십시오.

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
  <ul><li>궁극적인 플랜 </li></ul>
   </p>
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

## 전제 조건

결과, 활동 또는 프로젝트와 관련된 목표가 있어야 합니다.

## 결과, 활동 제거 및 목표에서 프로젝트 연결 해제에 대한 고려 사항

* 활성 목표에서만 결과 및 활동을 제거할 수 있습니다.
* 결과 및 활동을 삭제하여 목표에서 제거할 수 있습니다. 삭제된 결과 및 활동은 복구할 수 없습니다.
* 목표에서 결과나 활동을 제거하면 제거된 결과나 활동의 진행 상황이 목표의 전체 진행 상황에 영향을 줍니다.
* 목표에서 프로젝트를 삭제할 수는 없지만 목표에서 연결을 끊을 수는 있습니다. 목표에서 프로젝트의 연결을 해제하면 프로젝트의 완료율이 더 이상 목표의 진행에 영향을 주지 않습니다.

  프로젝트가 목표 진행에 미치는 영향에 대한 자세한 내용은 [Adobe Workfront 목표의 목표에 프로젝트 추가](../../workfront-goals/results-and-activities/connect-projects-to-goals-overview.md)를 참조하십시오.

* 목표에서 결과나 활동을 제거할 수 없으며, 목표에 대한 마지막 진행 표시자인 경우 하위 목표나 프로젝트의 연결을 끊을 수 없습니다.
* 프로젝트가 프로젝트 영역에서 삭제되고 목표의 마지막 진행 표시기이면 목표가 비활성 상태가 됩니다.

## 목표에서 결과 및 활동 삭제

결과 및 활동을 삭제하면 목표에서 제거됩니다. 목표에서 결과 및 활동을 삭제하는 것은 동일합니다.

<!--
How you delete results and activities differs depending on the environment you use.

### Delete results and activities in the Production environment


1. Click the **Main Menu** icon ![](assets/main-menu-icon.png) > **Goals** in the upper-right corner.

   (!-- Add this when Shell is available to all: or (if available), click the **Main Menu** icon ![Main menu icon](../results-and-activities/assets/three-line-main-menu-icon.png) in the upper-left corner)
   --)

   This opens the Workfront Goals area and the Goal List displays by default. 

1. Click the name of a goal you want to remove results and activities from.

   This opens the Goal Details panel on the right.

1. Click **Results** to remove results or **Activities** to remove activities. 

1. Click the **gear icon** ![](assets/settings-gear-icon.png) to the right of the result or activity name, then click **Delete** > **Yes, delete**.

   ![](assets/delete-result-goal-details-350x108.png)

   The result or activity is deleted and cannot be recovered. The percent complete of the goal updates to exclude the deleted activity or result.

-->

1. 오른쪽 상단의 **주 메뉴** 아이콘 ![](assets/main-menu-icon.png)을(를) 클릭한 다음 **목표**&#x200B;를 클릭합니다.

   <!-- Add this when Shell is available to all: or (if available), click the **Main Menu** icon ![Main menu icon](../results-and-activities/assets/three-line-main-menu-icon.png) in the upper-left corner)
   -->
   이렇게 하면 Workfront 목표 영역이 열리고 기본적으로 목표 목록이 표시됩니다.

1. 결과 및 활동을 제거할 목표의 이름을 클릭합니다.

   목표 페이지가 열립니다.

1. 왼쪽 패널에서 **진행률 표시기**&#x200B;를 클릭합니다.

1. 결과 또는 활동을 선택한 다음 목록 맨 위에 있는 **삭제** 아이콘 ![](assets/delete-icon.png)을(를) 클릭합니다.

1. **삭제**&#x200B;를 클릭하여 삭제를 확인합니다. 결과 또는 활동이 삭제되며 복구할 수 없습니다. 목표 완료율이 업데이트되어 삭제된 활동 또는 결과가 제외됩니다.


## 목표에서 프로젝트 제거

<!--
Dsconnecting projects from goals differs depending on the environment you use.

### Disconnect projects from goals in the Production environment


1. Click the **Main Menu** icon ![](assets/main-menu-icon.png) > **Goals** in the upper-right corner.

   (!-- Add this when Shell is available to all: or (if available), click the **Main Menu** icon ![Main menu icon](../results-and-activities/assets/three-line-main-menu-icon.png) in the upper-left corner)
   --)

   This opens the Workfront Goals area and the Goal List displays by default. 

1. Click the name of a goal you want to remove results and activities from.

   This opens the Goal Details panel on the right.

1. Click the **right-pointing arrow** to the left of the Activities sections to expand it. 
1. Click the **gear icon** ![](assets/settings-gear-icon.png) to the right of the project name, then click **Disconnect**.

   ![](assets/disconnect-project-goal-details-350x94.png)

   The project is disconnected from the goal. The percent complete of the goal updates to exclude the percent complete of the disconnected project.
-->


1. 오른쪽 상단의 **주 메뉴** 아이콘을 클릭한 다음 **목표**&#x200B;를 클릭합니다.

   <!-- Add this when Shell is available to all: or (if available), click the **Main Menu** icon ![Main menu icon](../results-and-activities/assets/three-line-main-menu-icon.png) in the upper-left corner)
   -->

   이렇게 하면 Workfront 목표 영역이 열리고 기본적으로 목표 목록이 표시됩니다.

1. 결과 및 활동을 제거할 목표의 이름을 클릭합니다.

   목표 페이지가 열립니다.
1. 왼쪽 패널에서 **진행률 표시기**&#x200B;를 클릭합니다.
1. 프로젝트를 선택한 다음 목록 맨 위에 있는 **연결 끊기** 아이콘 ![](assets/disconnect-icon.png)을(를) 클릭합니다.
1. 확인하려면 **연결 끊기**&#x200B;를 클릭하세요.

   프로젝트가 더 이상 목표에 연결되지 않습니다. 연결이 끊어진 프로젝트를 제외하기 위한 목표 업데이트의 완료율입니다.

