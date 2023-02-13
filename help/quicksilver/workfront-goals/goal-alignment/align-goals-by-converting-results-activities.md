---
product-previous: workfront-goals
navigation-topic: goal-alignment
title: 결과 및 활동을 목표로 변환하여 목표 정렬
description: 두 개의 목표를 수동으로 맞추거나 기존 목표의 결과와 활동을 다른 목표로 전환할 수 있습니다. 변환된 결과 또는 활동이 원래 목표의 하위 목표가 됩니다. 두 목표를 수동으로 정렬하는 방법에 대한 자세한 내용은 Adobe Workfront 목표에 연결하여 목표 맞춤 을 참조하십시오.
author: Alina
feature: Workfront Goals
exl-id: 48371389-952c-4732-b519-9774cd4d1b93
source-git-commit: 1d221d10e5845e477dff825f853330b9b4df0adf
workflow-type: tm+mt
source-wordcount: '643'
ht-degree: 0%

---

# 결과 및 활동을 목표로 변환하여 목표 정렬

두 개의 목표를 수동으로 맞추거나 기존 목표의 결과와 활동을 다른 목표로 전환할 수 있습니다. 변환된 결과 또는 활동이 원래 목표의 하위 목표가 됩니다.
두 목표를 수동으로 정렬하는 방법에 대한 자세한 내용은 [Adobe Workfront 목표에 연결하여 목표 정렬](../../workfront-goals/goal-alignment/align-goals-by-connecting-them.md).

## 액세스 요구 사항


<!--drafted for P&P release: 

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
   <td> <p>목표 이상에 대한 액세스 편집</p> <p><b>메모</b> 
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

## 전제 조건

시작하려면 먼저 다음을 수행해야 합니다.

* 기본 메뉴의 목표 영역을 포함하는 레이아웃 템플릿.
* 기존 결과 및 활동이 있는 기존 목표.

   목표 만들기에 대한 내용은 [Adobe Workfront 목표에서 목표 만들기](../../workfront-goals/goal-management/create-goals.md).

>[!IMPORTANT]
>
>목표에는 최대 1000개의 진행 상태 표시기가 있을 수 있습니다.

<!--drafted for goal redesign: At PRODUCTION: update the sentence above to remove Production/ Preview references-->

## 결과 및 활동을 목표로 변환할 때의 고려 사항

경우에 따라 결과나 활동은 예상보다 더 큰 범위를 가질 수 있으며 목표가 되는 것이 더 적절할 수 있습니다. 기존 목표의 결과 및 활동을 새 목표로 변환할 수 있습니다. 이는 목표 조정을 위한 상향식 접근 방식입니다.

결과 및 활동을 목표로 변환할 때는 다음 사항을 고려하십시오.

* 변환된 결과나 활동이 원래 목표의 하위 목표가 되고 두 목표가 일치합니다.
* 원래 목표에 추가 결과나 활동이 없는 경우 새로 생성된 목표가 원래 목표에 대한 단일 진행률 표시기가 됩니다. 진행 상황을 추적할 수 있으려면 결과 및 활동을 하위 목표에 추가해야 합니다.
* 결과나 활동을 목표로 전환하는 것은 되돌릴 수 없습니다. 변환된 새 하위 목표는 상위 목표에 대한 결과나 활동이 될 수 없습니다.

## 결과나 활동을 목표로 변환

<!--
<span class="preview">Converting results and activities differs depending on what environment you use. </span>

### Convert a result or activity to a goal in the Production environment

1. Go to a goal that has a result or an activity that you want to convert to a goal.
1. Click the name of the goal to open the **Goal Details** panel.
1. Expand the **Results** or **Activities** right-pointing arrows to see a list of results or activities for the goal. 

1. Click the **gear icon** ![](assets/settings-gear-icon.png) to the right of the result or activity name that you want to convert, then click **Convert into a Goal**.

   ![](assets/convert-to-goal-link-highlighted-350x191.png)

1. (Optional) Remove the name of the original activity or result owner from the **Goal Owner** field and replace it with another user, team, group, or your organization's name. By default, Workfront selects the owner of the result or the activity as the goal owner. 
1. Click **Convert**. The activity or result displays as an aligned goal in the Goal Details panel of the original goal and the original activity or result is removed from the original goal and transferred to the second goal. By default, the new goal has the same name as the original converted result or activity. 
1. (Optional) Click the name of the new goal to open the **Goal Details** panel and edit the name of the goal. For information about editing any information for an existing goal, see [Edit goals in Adobe Workfront Goals](../../workfront-goals/goal-management/edit-goals.md).
-->

1. 목표로 변환할 결과나 활동이 있는 목표로 이동합니다.
1. 목표 페이지에서 **진행률 표시기** 왼쪽 패널에 표시됩니다.
1. 진행 상태 표시기 목록에서 결과나 활동을 선택한 다음 **목표로 변환** 아이콘 ![](assets/convert-to-goal-icon-unshimmed.png) 진행률 표시기 목록의 맨 위에 표시됩니다. 목표로 변환 상자가 열립니다.

   ![](assets/convert-to-goal-box-unshimmed.png)
1. 다음 정보를 업데이트합니다.
   * **목표 이름**: 기본적으로 새 목표의 이름은 원래 결과나 활동과 동일합니다.
   * **기간**: 기본적으로 새 목표의 기간은 현재 분기입니다. 을(를) 선택할 수 있습니다 **사용자 지정 날짜 활성화** 새 목표에 대한 사용자 지정 기간 을 정의하기 위한 설정.
   * **목표 소유자**: 기본적으로 새 목표 소유자는 원래 결과나 활동의 소유자입니다.
   * **설명**: 새 목표에 대한 추가 정보를 추가합니다.
1. **저장**&#x200B;을 클릭합니다

   이제 결과 또는 활동이 원래 목표의 하위 목표로 변환됩니다. 원래 목표의 진행률 지표 목록에 목표로 나열됩니다.



