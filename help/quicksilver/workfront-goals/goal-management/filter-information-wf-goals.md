---
product-previous: workfront-goals
navigation-topic: goal-management
title: Adobe Workfront 목표에서 정보 필터링
description: 사용자 또는 Adobe Workfront 목표에 추가된 다른 사용자가 볼 수 있습니다. 목표 만들기에 대한 자세한 내용은 Adobe Workfront 목표에서 목표 만들기 를 참조하십시오. 목표를 볼 때 Workfront 목표의 정보를 필터링하여 자신에게 중요한 목표만 볼 수 있습니다.
author: Alina
feature: Workfront Goals
exl-id: ec9b6789-fffe-425c-8316-eefe670ad0d6
source-git-commit: 1d221d10e5845e477dff825f853330b9b4df0adf
workflow-type: tm+mt
source-wordcount: '1342'
ht-degree: 2%

---

# Adobe Workfront 목표에서 정보 필터링

사용자 또는 Adobe Workfront 목표에 추가된 다른 사용자가 볼 수 있습니다. 목표 만들기에 대한 내용은 [Adobe Workfront 목표에서 목표 만들기](../../workfront-goals/goal-management/create-goals.md). 목표를 볼 때 Workfront 목표의 정보를 필터링하여 자신에게 중요한 목표만 볼 수 있습니다.

## 액세스 요구 사항

<!--drafted - replace the table below with this one when P&P releases: 

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

이 문서에 설명된 작업을 수행하려면 다음 액세스 권한이 있어야 합니다.

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
   <td role="rowheader">액세스 수준*</td> 
   <td> <p>목표에 대한 액세스 권한 보기 이상</p> <p><b>메모</b>

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
     <p>목표에 대한 권한 보기 이상</p> 
     <p>목표 공유에 대한 자세한 내용은 <a href="../../workfront-goals/workfront-goals-settings/share-a-goal.md" class="MCXref xref">Workfront 목표에서 목표 공유</a>. </p> 
    </div> </td> 
  </tr> 
 </tbody> 
</table>

*보유하고 있는 플랜, 라이선스 유형 또는 액세스를 알아보려면 Workfront 관리자에게 문의하십시오.

## 전제 조건

시작하려면 먼저 다음을 수행해야 합니다.

* 기본 메뉴의 목표 영역을 포함하는 레이아웃 템플릿.

## Workfront 목표의 필터 개요

>[!NOTE]
>
>올바른 목표를 효율적으로 찾고 집중하기 위해 Workfront 목표에 필터를 사용하는 것이 좋습니다. 이를 통해 중요한 목표 관리를 시작하기 전에 올바른 정보를 표시할 수 있습니다. 기본적으로 Workfront 목표는 시스템의 모든 목표를 표시합니다.

Workfront의 다음 목표 영역에서 목표를 찾아 필터링할 수 있습니다.

* 목표 목록
* 그래프
* 목표 정렬

목표 영역의 섹션에 대한 자세한 내용은 [Adobe Workfront 목표 섹션 개요](../../workfront-goals/goal-review-and-workfront-goals-sections/overview-of-wf-goals-sections.md).

>[!IMPORTANT]
>
>한 섹션에 대한 필터를 구성할 수 있으며 Workfront 목표의 다른 섹션으로 이동할 때 계속 유지됩니다.

Workfront 목표에서 필터를 사용할 때는 다음 사항을 고려하십시오.

* 필터를 저장하지 않고 만들고 적용할 수 있고, 필터를 저장하여 나중에 다시 사용할 수 있습니다.

   다음 시나리오가 있습니다.

   * 필터를 저장하면 Workfront 목표에 로그인할 때마다 필터가 기본 필터로 사용됩니다.
   * 필터를 저장하지 않고 적용할 때 페이지를 새로 고쳐 원래 목록으로 되돌릴 수 있습니다.

* 만든 필터만 보고 적용할 수 있습니다. 다른 사용자가 만든 필터는 해당 사용자에 대해서만 표시됩니다.
* 만든 필터는 다른 사용자와 공유할 수 없습니다.

## Workfront 목표에 빠른 필터 적용

목표 목록에서 빠른 필터를 사용하여 중요한 항목만 찾는 데 도움이 될 수 있습니다. 빠른 필터를 저장할 수 없으며 지속적이지 않습니다. Workfront은 페이지를 새로 고칠 때 빠른 필터 결과를 지웁니다.

자세한 내용은 [목록에 빠른 필터 적용](../../workfront-basics/navigate-workfront/use-lists/apply-quick-filter-list.md).

## Workfront 목표에서 필터 만들기 및 적용

필터를 만드는 프로세스는 Workfront 목표 섹션에 대해 동일합니다.

필터를 처음부터 만들거나 내장된 필터 중 하나를 편집할 수 있습니다.

1. Workfront 목표 으로 이동합니다.

   Workfront 목표 액세스에 대한 자세한 내용은 [Adobe Workfront 목표의 액세스 및 공개 목표](../../workfront-goals/goal-management/access-goals-in-wf-goals.md)

   기본적으로 목표 목록 섹션이 표시됩니다.

1. 클릭 **필터** 목록의 오른쪽 상단에서.

   ![](assets/filter-icon-and-label.png)

   기본적으로 Workfront은 **모두** 시스템에 모든 목표를 표시하는 필터입니다.

   >[!TIP]
   >
   >모두 필터를 편집하거나 삭제할 수 없습니다.

1. 다음 중 하나를 수행하십시오.

   * 다음 소유자에 대해서만 목표를 표시하려면 사전 정의된 다음 필터 중 하나를 클릭합니다.

      <table style="table-layout:auto"> 
      <col> 
      <col> 
      <tbody> 
       <tr> 
        <td>모두</td> 
        <td> <p>시스템의 모든 목표는 목표를 생성한 사람, 기간을 지정하거나 소유자가 누구인지에 상관없이 모두 사용할 수 있습니다. 기본 필터이므로 편집할 수 없습니다. </p> <!--
          <p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: what the ALL filter displays might change; right now, it displays all, regardless of status, period, owner, etc)</p>
         --> </td> 
       </tr> 
       <tr> 
        <td>개인</td> 
        <td>소유자에 대한 목표</td> 
       </tr> 
       <tr> 
        <td>내 팀</td> 
        <td> <p>모든 팀이 소유자로 선택되는 목표. </p> <p><b>팁</b>

      팀에 할당되지 않은 경우에는 목표가 표시되지 않습니다. </p> </td>
      </tr> 
       <tr> 
        <td>내 그룹</td> 
        <td>그룹 중 소유자로 선택되는 목표. </td> 
       </tr> 
       <tr> 
        <td>회사</td> 
        <td> <p>조직과 연관된 목표. </p> <p><b>팁</b>
        <p>Adobe Workfront 목표에서 회사 필터는 조직이 소유자로 선택되는 목표를 표시합니다. </p> <p>이 필드를 사용하여 회사를 검색할 수 없습니다. 기본적으로 Workfront 인스턴스의 소유자인 조직만 선택됩니다. </p> </p> </td> 
       </tr> 
      </tbody> 
     </table>

   * 필터 이름을 마우스로 가리킨 다음 **편집** 아이콘 ![](assets/edit-icon.png) 이름 옆에 사용자 지정하고 사용자, 팀, 그룹 또는 조직의 특정 이름을 추가한 다음 목록에 표시될 때 선택합니다.

   * 클릭 **새 필터** 새 필터를 만들려면 다음 옵션 중에서 선택하여 새 필터를 사용자 지정합니다.

      <table style="table-layout:auto"> 
      <col> 
      <col> 
      <tbody> 
       <tr> 
        <td role="rowheader">기간</td> 
        <td>드롭다운 메뉴에서 기간을 선택합니다. 여러 기간을 선택할 수 있습니다. </td> 
       </tr> 
       <tr> 
        <td role="rowheader">상태</td> 
        <td> <p>다음 옵션 중에서 드롭다운 메뉴에서 상태를 선택합니다.</p> 
         <ul> 
          <li> <p>활성</p> </li> 
          <li> <p>초안</p> </li> 
          <li> <p>비활성</p> </li> 
          <li> <p>마감됨</p> </li> 
         </ul> </td> 
       </tr> 
       <tr> 
        <td role="rowheader">진행</td> 
        <td> <p>다음 옵션 중에서 드롭다운 메뉴에서 진행률을 선택합니다. </p> 
         <ul> 
          <li> <p>문제 발생</p> </li> 
          <li> <p>위험 상태</p> </li> 
          <li> <p>대상</p> </li> 
         </ul> </td> 
       </tr> 
       <tr> 
        <td role="rowheader">소유자</td> 
        <td> <p>소유자 이름을 입력하기 시작한 다음 목록에 표시될 때 선택합니다. </p> <p>사용자, 팀, 그룹 또는 조직 이름을 입력하거나 사전 정의된 옵션 중에서 선택할 수 있습니다. </p> <p>다음 사전 정의된 필터 옵션은 항상 현재 로그인되어 있는 사용자를 참조합니다. </p> 
         <ul> 
          <li> <p><strong>Me</strong>: 소유자인 위치에 목표를 표시합니다.</p> </li> 
          <li> <p><strong>내 홈 팀</strong> 및 <strong>모든 내 팀</strong>: 홈 팀이나 팀이 소유자로 지정된 목표를 표시합니다. </p> <p>팁: 팀에 할당되지 않은 경우에는 목표가 표시되지 않습니다. </p> </li> 
          <li> <p><strong>내 홈 그룹</strong> 및 <strong>모든 내 그룹</strong>: 홈 그룹 또는 그룹이 소유자로 지정된 목표를 표시합니다.</p> </li> 
         </ul> </td> 
       </tr> 
      </tbody> 
     </table>

1. (선택 사항) **재설정** 필터 상자의 오른쪽 아래 모서리에서 선택한 모든 필드를 지우고 처음부터 필터 작성을 시작합니다.
1. (선택 사항) **적용** 을 눌러 필터를 저장하지 않고 적용합니다.

   필터가 **저장하지 않음** 필터 빌더의 영역 **새 필터**.

   저장하지 않은 필터의 이름은 변경할 수 없습니다.

   다음에 Workfront에서 로그아웃한 다음 다시 로그인하면 저장하지 않은 필터가 목표 영역에서 제거됩니다.

   >[!TIP]
   >
   >저장하지 않은 새 필터를 한 번에 하나만 보유할 수 있습니다.

1. 클릭 **저장** 나중에 사용할 수 있도록 필터를 저장하려면 **필터 이름 추가** 필드를 입력하고 **완료**.

   이렇게 하면 필터가 **저장됨** 세그먼트 빌더의 섹션을 참조하십시오. 나중에 이 필터를 사용할 수 있습니다.

   다음에 Workfront에 다시 로그인할 때 기본적으로 마지막으로 저장한 필터가 표시됩니다

1. (선택 사항) **왼쪽 방향 화살표** 다음 **새 필터** 필터 빌더를 종료하고 필터 목록으로 돌아갑니다.
1. (선택 사항) 사용자 지정 필터의 이름을 마우스로 가리킨 다음, **자세히** 메뉴를 클릭한 다음 **삭제**, 그런 다음 **삭제**. 필터를 삭제하므로 복구할 수 없습니다.

   >[!TIP]
   >
   >사전 정의된 필터는 삭제할 수 없습니다.

1. 을(를) 클릭합니다. **X 아이콘** 필터 빌더의 오른쪽 위 모서리에서 을(를) 클릭하여 필터 빌더를 닫습니다.

   현재 적용된 필터 이름은 목표 목록의 오른쪽 위 모서리에 필터 아이콘 오른쪽에 표시됩니다.

   목표 목록은 필터 기준으로 필터링됩니다.

1. (선택 사항 및 조건부) 목표 정렬 섹션에서 목표를 볼 때 **표시** 필터링된 종료 목표를 보려면

   ![](assets/show-them-link-on-filtered-items-goal-list-350x109.png)

   필터 이름은 무시되고 있음을 나타내도록 노란색으로 윤곽선이 표시됩니다.

   ![](assets/filter-yellow-outline-next-to-reapply-filter-link-350x118.png)


1. (선택 사항 및 조건부) **필터 다시 적용** 필터를 적용하고 이전 단계에 표시된 항목을 생략하려면 다음을 수행하십시오.


