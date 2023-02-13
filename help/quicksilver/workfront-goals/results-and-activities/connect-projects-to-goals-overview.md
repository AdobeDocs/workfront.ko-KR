---
content-type: overview
product-previous: workfront-goals
product-area: projects
navigation-topic: results-and-activities
title: Adobe Workfront 목표의 목표에 프로젝트 추가
description: 프로젝트를 목표에 연결하여 프로젝트의 실제 진행 상황을 기반으로 목표가 어떻게 진행되는지를 나타낼 수 있습니다. 프로젝트는 목표에 대한 진행 지표가 됩니다.
author: Alina
feature: Workfront Goals
exl-id: 683c9cd9-6c7b-4d50-b326-b4000c9863e8
source-git-commit: dc3461803e23f61877c31efa2c52fffdc7bd79bf
workflow-type: tm+mt
source-wordcount: '888'
ht-degree: 1%

---

# Adobe Workfront 목표의 목표에 프로젝트 추가

<!--
THIS MIGHT NEED TO BE RENAMED BECAUSE THERE WILL BE OTHER OBJECTS CONNECTED TO GOALS IN THE FUTURE
-->

프로젝트를 목표에 연결하여 프로젝트의 실제 진행 상황을 기반으로 목표가 어떻게 진행되는지를 나타낼 수 있습니다. 프로젝트는 목표에 대한 진행 지표가 됩니다.

프로젝트를 목표에 연결하여 조직의 전략적 계획(목표)을 사람들이 매일 수행하고 완료하는 실제 작업에 연결할 수 있습니다(프로젝트).

>[!IMPORTANT]
>
>프로젝트의 비즈니스 사례 영역에서 만들어진 프로젝트 수준 목표는 Workfront 목표에 연결되어 있지 않습니다. 비즈니스 사례 프로젝트 목표에 대한 자세한 내용은 [비즈니스 사례 목표 생성](../../manage-work/projects/define-a-business-case/create-business-case-goals.md).


## 액세스 요구 사항

<!--drafted for P&P release: replace the table below with this: 

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
   <td> <p>목표에 대한 액세스 편집</p> <p><b>메모</b>

<p>여전히 액세스 권한이 없는 경우 Workfront 관리자에게 액세스 수준에서 추가 제한 사항을 설정하는지 문의하십시오. Workfront 관리자가 액세스 수준을 변경하는 방법에 대한 자세한 내용은 다음을 참조하십시오.</p> 
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

*보유하고 있는 플랜, 라이선스 유형 또는 액세스를 알아보려면 Workfront 관리자에게 문의하십시오.

Workfront 목표 액세스에 대한 자세한 내용은 [Workfront 목표 사용 요구 사항](../goal-management/access-needed-for-wf-goals.md).

## 프로젝트에 목표 연결 고려 사항

* 다음 기준을 충족하는 프로젝트를 목표에 추가할 수 있습니다.

   * 볼 수 있는 권한이 있어야 합니다.

      >[!NOTE]
      >
      >프로젝트에 목표를 추가한 후 프로젝트를 볼 수 있는 권한이 손실된 경우 목표에 대한 프로젝트 정보를 볼 수 있지만 더 이상 프로젝트에 액세스할 수 없습니다.

   * 프로젝트가 중단 상태이면 안 됩니다.

* 여러 프로젝트를 목표와 연결할 수 있습니다.
* 동일한 프로젝트를 여러 목표와 연결할 수 있습니다.
* 프로젝트가 첨부된 목표에서는 프로젝트의 진행 상태를 수동으로 업데이트할 수 없습니다. 대신 Workfront은 프로젝트 완료율을 계산하고 Workfront 목표는 이 완료율을 사용하여 목표 진행 상황을 계산합니다. 프로젝트 비율 업데이트 후 실시간으로 목표를 업데이트합니다.
* 프로젝트 기간은 목표 기간을 초과할 수 있습니다. 프로젝트가 목표 최종 기한 보다 오래 지속되는 경우, 목표를 닫고 완료된 것으로 간주할 수 있지만 목표 완료율은 100%가 되지 않습니다. 프로젝트의 완료율이 목표에 대해 더 이상 업데이트되지 않습니다.

<!--this is no longer visible in the new redesigned interface for goals: logged a bug for this: https://experience.adobe.com/#/@adobeinternalworkfront/so:hub-Hub/workfront/issue/63ceb049000080d30022aab9a359f6f1/updates - but confirmed that this will not be brought back at least for now - Jan 2023. 

There is an indication on the goal list that the project no longer updates progress for the goal.

  ![](assets/goal-closed-project-active-warning-goal-list-350x94.png)
-->

* 목표에 첨부된 프로젝트를 삭제하면 목표에서도 프로젝트가 삭제됩니다.

   >[!CAUTION]
   >
   >프로젝트를 삭제하기 전에 목표가 활성 상태이고 목표에 다른 진행률 표시기가 없는 경우 목표가 비활성 상태가 됩니다.


## 목표에 프로젝트 추가

1. 을(를) 클릭합니다. **기본 메뉴** ![](assets/main-menu-icon.png) (셸에 대해 이 초안 작성: 또는 **기본 메뉴** ![](assets/three-line-main-menu-icon.png) 왼쪽 위 모서리에서 사용 가능한 경우) 을 클릭합니다. **목표**.
1. 목표 목록에서 목표 페이지를 열 목표 이름을 클릭합니다.
1. 클릭 **진행률 표시기** 왼쪽 패널에 표시됩니다.
1. 에서 **새 진행률 표시기** 드롭다운 메뉴에서 **기존 프로젝트 추가**.

   목표에 프로젝트 추가 상자가 표시됩니다.
1. (선택 사항) **보기**, **필터**, 또는 **그룹화** 목록 오른쪽 위의 각 아이콘을 클릭하여 프로젝트 목록이 표시되는 방식을 수정합니다.
1. (선택 사항) **검색** 아이콘 ![](assets/search-icon.png) 프로젝트 이름을 입력하여 목록에서 신속하게 찾을 수 있습니다.
1. 목표에 추가할 프로젝트를 선택한 다음 **추가**.

   선택한 프로젝트가 목표에 추가되고, 목표 페이지의 아래 진행 상태 표시기 섹션에 표시됩니다. **프로젝트** 그룹화.

   목표를 활성화하면 프로젝트 진행 상태가 업데이트되면 목표 진행 상태가 자동으로 업데이트됩니다. 목표 활성화에 대한 자세한 내용은 [Adobe Workfront 목표에서 목표 활성화](../goal-management/activate-goals.md).

## 목표에 대한 프로젝트 정보 찾기

<p>
다음 프로젝트 정보는 목표 페이지의 진행 지표 섹션에 있는 목표 수준에서 표시됩니다.

</p>

<table>
  <tr>
   <td>프로젝트 이름
   </td>
   <td>프로젝트 이름의 변경 사항도 연결된 프로젝트에 반영됩니다.
   </td>
  </tr>
  <tr>
   <td>프로젝트 소유자
   </td>
   <td>프로젝트 소유자의 모든 변경 사항은 연결된 프로젝트도 반영합니다.
   </td>
  </tr>
    <tr>
   <td>실제 진행 상황
   </td>
   <td> <p>프로젝트 완료율. 목표에서 완료된 프로젝트 비율은 수동으로 업데이트할 수 없습니다. Workfront은 작업 완료율을 기반으로 자동으로 계산합니다. </p>
   </td>
  </tr>
  <tr>
   <td>진행
   </td>
   <td>막대로 표시된 프로젝트의 완료율. 프로젝트가 완료되는 백분율을 변경하면, 목표가 닫히지 않는 한 목표 진행 상태가 자동으로 업데이트됩니다.
   </td>
  </tr>

</table>

## 프로젝트에서 목표 정보 찾기

다음 목표 정보는 프로젝트 목록 또는 보고서에 표시됩니다.

| 목표 정보 | 설명 |
|---|---|
| 목표 | 프로젝트가 연결된 모든 목표 목록입니다. |
| 목표 계층 | 목표가 속한 계층. 이 필드에는 목표 및 목표에 대한 부모만 표시됩니다. 하위 목표는 표시되지 않습니다. |
| 연결된 목표 수 | 하나의 프로젝트에 연결된 목표 수. |
