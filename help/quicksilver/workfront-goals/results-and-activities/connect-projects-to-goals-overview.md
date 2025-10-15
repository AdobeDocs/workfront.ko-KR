---
content-type: overview
product-previous: workfront-goals
product-area: projects
navigation-topic: results-and-activities
title: Adobe Workfront 목표의 목표에 프로젝트 추가
description: 프로젝트를 목표에 연결하여 프로젝트의 실제 진행 상황에 따라 목표가 어떻게 진행되는지 나타낼 수 있습니다. 프로젝트가 목표에 대한 진행 표시기가 됩니다.
author: Alina
feature: Workfront Goals
exl-id: 683c9cd9-6c7b-4d50-b326-b4000c9863e8
source-git-commit: 4ef71db5d93e314b746e8acdbf90fd041c6e71ae
workflow-type: tm+mt
source-wordcount: '865'
ht-degree: 1%

---

# Adobe Workfront 목표의 목표에 프로젝트 추가

<!--Audited for P&P only: 10/2025-->

프로젝트를 목표에 연결하여 프로젝트의 실제 진행 상황에 따라 목표가 어떻게 진행되는지 나타낼 수 있습니다. 프로젝트가 목표에 대한 진행 표시기가 됩니다.

프로젝트를 목표에 연결함으로써 조직의 전략 계획(목표)을 직원들이 매일 수행하고 완료하는 실제 작업(프로젝트)에 연결할 수 있습니다.

>[!IMPORTANT]
>
>프로젝트의 비즈니스 사례 영역에서 생성된 프로젝트 수준 목표는 Workfront 목표에서 생성된 전략적 목표와 연결되지 않습니다. 비즈니스 사례 프로젝트 목표에 대한 자세한 내용은 [비즈니스 사례 목표 만들기](../../manage-work/projects/define-a-business-case/create-business-case-goals.md)를 참조하십시오.


## 액세스 요구 사항

>[!NOTE]
>
>이전에 이 패키지를 구입한 경우 귀사에서 Adobe Workfront 목표를 계속 사용하도록 선택할 수 있습니다. 자세한 내용은 계정 담당자에게 문의하십시오.
>
>Adobe Workfront 목표를 더 이상 구매할 수 없습니다.

+++ 을 확장하여 이 문서의 기능에 대한 액세스 요구 사항을 봅니다. 

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
 <p> New product requirement, one of the following: </p>
<ul>
<li>A Select or Prime Adobe Workfront plan and an additional Adobe Workfront Goals license.</li>
<li>An Ultimate Workfront plan which includes Workfront Goals by default. </li></ul>
 <p>Or</p>
 <p>Current product requirement: A Workfront plan and an additional license for Adobe Workfront Goals. </p> <p>For information, see <a href="../../workfront-goals/goal-management/access-needed-for-wf-goals.md" class="MCXref xref">Requirements to use Workfront Goals</a>. </p> </td>
 </tr>
 <tr>
 <td role="rowheader">Access level</td>
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

## 프로젝트를 목표에 연결하는 것에 대한 고려 사항

* 다음 기준을 충족하는 프로젝트를 목표에 추가할 수 있습니다.

   * 적어도 볼 수 있는 권한이 있어야 합니다.

     >[!NOTE]
     >
     >프로젝트를 목표에 첨부한 후에 프로젝트를 볼 수 있는 권한이 상실되면 목표에 대한 프로젝트 정보를 계속 볼 수 있지만, 더 이상 프로젝트에 액세스할 수 없습니다.

   * 프로젝트가 중단 상태가 아니어야 합니다.

* 여러 프로젝트를 목표와 연결할 수 있습니다.
* 동일한 프로젝트를 여러 목표와 연결할 수 있습니다.
* 프로젝트가 첨부된 목표에서는 프로젝트의 진행 상황을 수동으로 업데이트할 수 없습니다. 대신 Workfront은 프로젝트의 완료율을 계산하고 Workfront 목표는 이 완료율을 사용하여 목표 진행률을 계산합니다. 이렇게 하면 프로젝트 백분율이 업데이트된 후 목표가 실시간으로 업데이트됩니다.
* 프로젝트 기간은 목표의 기간을 벗어날 수 있습니다. 프로젝트가 목표의 마감일보다 오래 지속되는 경우 목표를 닫고 완료된 것으로 간주할 수 있지만 목표 완료율은 100%가 되지 않습니다. 프로젝트의 완료율이 목표에 대해 더 이상 업데이트되지 않습니다.

<!--this is no longer visible in the new redesigned interface for goals: logged a bug for this: https://experience.adobe.com/#/@adobeinternalworkfront/so:hub-Hub/workfront/issue/63ceb049000080d30022aab9a359f6f1/updates - but confirmed that this will not be brought back at least for now - Jan 2023. 

There is an indication on the goal list that the project no longer updates progress for the goal.

  ![Goal closed](assets/goal-closed-project-active-warning-goal-list-350x94.png)
-->

* 목표에 첨부된 프로젝트를 삭제하면 프로젝트도 목표에서 삭제됩니다.

  >[!CAUTION]
  >
  >프로젝트를 삭제하기 전에 목표가 활성 상태이고 목표에 다른 진행 표시기가 없는 경우 목표가 비활성 상태가 됩니다.


## 목표에 프로젝트 추가

1. **주 메뉴** ![주 메뉴 아이콘](assets/main-menu-icon.png)(셸에 대한 초안: 또는 왼쪽 위 모서리에 있는 **주 메뉴** ![주 메뉴 줄](assets/three-line-main-menu-icon.png)(사용 가능한 경우)을 클릭한 다음 **목표**&#x200B;를 클릭합니다.
1. 목표 목록에서 목표 이름을 클릭하여 목표 페이지를 엽니다.
1. 왼쪽 패널에서 **진행률 표시기**&#x200B;를 클릭합니다.
1. **새 진행률 표시기** 드롭다운 메뉴에서 **기존 프로젝트 추가**&#x200B;를 클릭합니다.

   목표에 프로젝트 추가 상자가 표시됩니다.
1. (선택 사항) 프로젝트 목록이 표시되는 방식을 수정하려면 목록의 오른쪽 상단에 있는 각 아이콘을 클릭하여 **보기**, **필터** 또는 **그룹화**&#x200B;를 업데이트합니다.
1. (선택 사항) **검색** 아이콘 ![검색 아이콘](assets/search-icon.png)을 클릭하고 프로젝트 이름을 입력하여 목록에서 빠르게 찾을 수 있습니다.
1. 목표에 추가할 프로젝트를 선택한 다음 **추가**&#x200B;를 클릭합니다.

   선택한 프로젝트가 목표에 추가되고 **프로젝트** 그룹화 아래 목표 페이지의 진행 표시기 섹션에 표시됩니다.

   목표를 활성화하면 프로젝트 진행 상황이 업데이트될 때 목표의 진행 상황이 자동으로 업데이트됩니다. 목표 활성화에 대한 자세한 내용은 [Adobe Workfront 목표에서 목표 활성화](../goal-management/activate-goals.md)를 참조하십시오.

## 목표에 대한 프로젝트 정보 찾기

<p>
다음 프로젝트 정보는 목표 페이지의 진행 표시기 섹션에 목표 수준에서 표시됩니다.

</p>

<table>
  <tr>
   <td>프로젝트 이름
   </td>
   <td>프로젝트 이름의 모든 변경 사항은 연결된 프로젝트에도 반영됩니다.
   </td>
  </tr>
  <tr>
   <td>프로젝트 소유자
   </td>
   <td>프로젝트 소유자의 모든 변경 사항은 연결된 프로젝트에도 반영됩니다.
   </td>
  </tr>
    <tr>
   <td>실제 진행 상황
   </td>
   <td> <p>프로젝트의 완료율입니다. 목표에서 프로젝트 완료율을 수동으로 업데이트할 수 없습니다. Workfront은 작업 완료율을 기반으로 자동으로 계산됩니다. </p>
   </td>
  </tr>
  <tr>
   <td>진행
   </td>
   <td>막대로 표시되는 프로젝트의 완료율입니다. 프로젝트의 완료율을 변경하면 목표가 종료되지 않는 한 목표 진행률이 자동으로 업데이트됩니다.
   </td>
  </tr>

</table>

## 프로젝트에서 목표 정보 찾기

프로젝트 목록 또는 보고서에 다음 목표 정보가 표시됩니다.

| 목표 정보 | 설명 |
|---|---|
| 목표 | 연관된 프로젝트가 있는 모든 목표 목록입니다. |
| 목표 계층 | 목표가 속한 계층입니다. 이 필드에는 목표와 목표의 부모만 표시됩니다. 하위 목표는 표시되지 않습니다. |
| 연결된 목표 수 | 한 프로젝트에 연결된 목표 수입니다. |
