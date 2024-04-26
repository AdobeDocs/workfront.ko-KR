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
source-git-commit: 948cd81908df3174eb985d1c65533077d3ef5d49
workflow-type: tm+mt
source-wordcount: '892'
ht-degree: 2%

---

# Adobe Workfront 목표의 목표에 프로젝트 추가

<!--
THIS MIGHT NEED TO BE RENAMED BECAUSE THERE WILL BE OTHER OBJECTS CONNECTED TO GOALS IN THE FUTURE
-->

프로젝트를 목표에 연결하여 프로젝트의 실제 진행 상황에 따라 목표가 어떻게 진행되는지 나타낼 수 있습니다. 프로젝트가 목표에 대한 진행 표시기가 됩니다.

프로젝트를 목표에 연결함으로써 조직의 전략 계획(목표)을 직원들이 매일 수행하고 완료하는 실제 작업(프로젝트)에 연결할 수 있습니다.

>[!IMPORTANT]
>
>프로젝트의 비즈니스 사례 영역에서 생성된 프로젝트 수준 목표는 Workfront 목표에서 생성된 전략적 목표와 연결되지 않습니다. 비즈니스 사례 프로젝트 목표에 대한 자세한 내용은 [비즈니스 사례 목표 만들기](../../manage-work/projects/define-a-business-case/create-business-case-goals.md).


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
 <p>현재 라이선스: 요청 이상</p> <p>자세한 내용은 <a href="../../administration-and-setup/add-users/access-levels-and-object-permissions/wf-licenses.md" class="MCXref xref">Adobe Workfront 라이선스 개요</a>.</p> </td>
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

  ![](assets/goal-closed-project-active-warning-goal-list-350x94.png)
-->

* 목표에 첨부된 프로젝트를 삭제하면 프로젝트도 목표에서 삭제됩니다.

  >[!CAUTION]
  >
  >프로젝트를 삭제하기 전에 목표가 활성 상태이고 목표에 다른 진행 표시기가 없는 경우 목표가 비활성 상태가 됩니다.


## 목표에 프로젝트 추가

1. 다음을 클릭합니다. **메인 메뉴** ![](assets/main-menu-icon.png) (셸에 대해 이 초안 작성: 또는 **메인 메뉴** ![](assets/three-line-main-menu-icon.png) 왼쪽 상단 모서리에서 을(를) 사용할 수 있는 경우) 다음을 수행합니다. **목표**.
1. 목표 목록에서 목표 이름을 클릭하여 목표 페이지를 엽니다.
1. 클릭 **진행 표시기** 왼쪽 패널에서
1. 다음에서 **새로운 진행 표시기** 드롭다운 메뉴, 클릭 **기존 프로젝트 추가**.

   목표에 프로젝트 추가 상자가 표시됩니다.
1. (선택 사항) **보기**, **필터**, 또는 **그룹화** 목록의 오른쪽 상단에 있는 각 아이콘을 클릭하여 프로젝트 목록이 표시되는 방식을 수정합니다.
1. (선택 사항) **검색** 아이콘 ![](assets/search-icon.png) 목록에서 빠르게 찾을 수 있도록 프로젝트 이름을 입력하십시오.
1. 목표에 추가할 프로젝트를 선택한 다음 **추가**.

   선택한 프로젝트가 목표에 추가되고 목표 페이지의 아래 진행 표시기 섹션에 표시됩니다. **프로젝트** 그룹화.

   목표를 활성화하면 프로젝트 진행 상황이 업데이트될 때 목표의 진행 상황이 자동으로 업데이트됩니다. 목표 활성화에 대한 자세한 내용은 [Adobe Workfront 목표에서 목표 활성화](../goal-management/activate-goals.md).

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
