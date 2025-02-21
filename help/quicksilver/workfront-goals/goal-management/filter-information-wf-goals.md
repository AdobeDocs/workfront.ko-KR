---
product-previous: workfront-goals
navigation-topic: goal-management
title: Adobe Workfront 목표의 정보 필터링
description: 본인 또는 다른 사람이 Adobe Workfront 목표에 추가한 목표를 볼 수 있습니다. 목표 만들기에 대한 자세한 내용은 Adobe Workfront 목표에서 목표 만들기 를 참조하십시오. 목표를 볼 때 Workfront 목표에서 정보를 필터링하여 자신에게 중요한 목표만 볼 수 있습니다.
author: Alina
feature: Workfront Goals
exl-id: ec9b6789-fffe-425c-8316-eefe670ad0d6
source-git-commit: 45c71a8106bdb8eeaa38f2fb83ff0312e48183d0
workflow-type: tm+mt
source-wordcount: '1379'
ht-degree: 2%

---

# Adobe Workfront 목표의 정보 필터링

본인 또는 다른 사람이 Adobe Workfront 목표에 추가한 목표를 볼 수 있습니다. 목표 만들기에 대한 자세한 내용은 [Adobe Workfront 목표에서 목표 만들기](../../workfront-goals/goal-management/create-goals.md)를 참조하십시오. 목표를 볼 때 Workfront 목표에서 정보를 필터링하여 자신에게 중요한 목표만 볼 수 있습니다.

## 액세스 요구 사항

이 문서에 설명된 작업을 수행하려면 다음 액세스 권한이 있어야 합니다.

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
  <ul><li>Ultimate 플랜 </li> </ul>

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
<li>기본적으로 Workfront 목표를 포함하는 Ultimate Workfront 플랜입니다. </li></ul>
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

## Workfront 목표의 필터 개요

>[!NOTE]
>
>올바른 목표를 효율적으로 찾고 집중하려면 Workfront 목표에서 필터를 사용하는 것이 좋습니다. 따라서 중요한 목표 관리를 시작하기 전에 올바른 정보를 표시할 수 있습니다. 기본적으로 Workfront 목표에는 시스템의 모든 목표가 표시됩니다.

Workfront의 목표 영역의 다음 섹션에서 목표를 찾고 필터링할 수 있습니다.

* 목표 목록
* 그래프
* 목표 정렬

목표 영역의 섹션에 대한 자세한 내용은 [Adobe Workfront 목표 섹션 개요](../../workfront-goals/goal-review-and-workfront-goals-sections/overview-of-wf-goals-sections.md)를 참조하십시오.

>[!IMPORTANT]
>
>한 섹션에 대한 필터를 구성할 수 있으며, Workfront 목표의 다른 섹션으로 이동할 때 계속 유지됩니다.

Workfront 목표에서 필터를 사용할 때는 다음 사항을 고려하십시오.

* 필터를 저장하지 않고 만들어 적용하거나, 나중에 다시 사용하도록 필터를 저장할 수 있습니다.

  다음과 같은 시나리오가 있습니다.

   * 필터를 저장하면 Workfront 목표에 로그인할 때마다 이 필터가 기본 필터가 됩니다.
   * 필터를 저장하지 않고 적용하면 페이지를 새로 고쳐 원래 목록으로 되돌릴 수 있습니다.

* 생성한 필터만 보고 적용할 수 있습니다. 다른 사용자가 만든 필터는 해당 사용자에 대해서만 표시됩니다.
* 생성한 필터는 다른 사용자와 공유할 수 없습니다.

## Workfront 목표에서 빠른 필터 적용

목표 목록에서 빠른 필터를 사용하여 자신에게 중요한 항목만 찾을 수 있습니다. 빠른 필터는 저장할 수 없으며 영구적이지 않습니다. Workfront은 페이지를 새로 고칠 때 빠른 필터의 결과를 지웁니다.

자세한 내용은 [목록에 빠른 필터 적용](../../workfront-basics/navigate-workfront/use-lists/apply-quick-filter-list.md)을 참조하십시오.

## Workfront 목표에서 필터 만들기 및 적용

필터를 만드는 프로세스는 Workfront 목표의 모든 섹션에 대해 동일합니다.

필터를 처음부터 만들거나 기본 제공 필터 중 하나를 편집할 수 있습니다.

1. Workfront 목표로 이동합니다.

   Workfront 목표에 액세스하는 방법에 대한 자세한 내용은 [Adobe Workfront 목표에서 목표 액세스 및 열기](../../workfront-goals/goal-management/access-goals-in-wf-goals.md)를 참조하십시오.

   기본적으로 목표 목록 섹션이 표시됩니다.

1. 목록의 오른쪽 상단 모서리에서 **필터**&#x200B;를 클릭합니다.

   ![필터 아이콘](assets/filter-icon-and-label.png)

   기본적으로 Workfront은 시스템의 모든 목표를 표시하는 **모두** 필터를 적용합니다.

   >[!TIP]
   >
   >모두 필터는 편집하거나 삭제할 수 없습니다.

1. 다음 중 하나를 수행하십시오.

   * 미리 정의된 다음 필터 중 하나를 클릭하여 다음 소유자에 대한 목표만 표시합니다.

     <table style="table-layout:auto"> 
      <col> 
      <col> 
      <tbody> 
       <tr> 
        <td>모두</td> 
        <td> <p>시스템의 모든 목표 작성자, 기간, 소유자 등에 상관없이 모든 목표를 지정할 수 있습니다. 기본 필터이므로 편집할 수 없습니다. </p> <!--
          <p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: what the ALL filter displays might change; right now, it displays all, regardless of status, period, owner, etc)</p>
         --> </td> 
       </tr> 
       <tr> 
        <td>개인</td> 
        <td>사용자가 소유하는 목표입니다.</td> 
       </tr> 
       <tr> 
        <td>내 팀</td> 
        <td> <p>팀이 소유자로 선택된 목표. </p> <p><b>팁</b>

     팀에 할당되지 않은 경우 목표가 표시되지 않습니다. </p> </td>
     </tr> 
       <tr> 
        <td>내 그룹</td> 
        <td>그룹 중 하나를 소유자로 선택하는 목표입니다. </td> 
       </tr> 
       <tr> 
        <td>회사</td> 
        <td> <p>조직과 연관된 목표입니다. </p> <p><b>팁</b>
        <p>Adobe Workfront 목표에서 회사 필터는 조직이 소유자로 선택된 목표를 표시합니다. </p> <p>이 필드를 사용하여 회사를 검색할 수 없습니다. Workfront 인스턴스의 소유자인 조직만 기본적으로 선택됩니다. </p> </p> </td> 
       </tr> 
      </tbody> 
     </table>

   * 필터 이름을 마우스로 가리킨 다음, 필터 이름 옆에 있는 **편집** 아이콘 ![편집 아이콘](assets/edit-icon.png)을 클릭하여 사용자 지정하고 사용자, 팀, 그룹 또는 조직의 이름을 추가한 다음 목록에 표시될 때 선택합니다.

   * **새 필터**&#x200B;를 클릭하여 새 필터를 만든 다음 다음 다음 옵션 중에서 선택하여 새 필터를 사용자 지정합니다.

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
        <td> <p>다음 옵션에서 드롭다운 메뉴의 상태를 선택합니다.</p> 
         <ul> 
          <li> <p>활성</p> </li> 
          <li> <p>초안</p> </li> 
          <li> <p>비활성</p> </li> 
          <li> <p>마감됨</p> </li> 
         </ul> </td> 
       </tr> 
       <tr> 
        <td role="rowheader">진행</td> 
        <td> <p>다음 옵션 중 드롭다운 메뉴에서 진행률을 선택합니다. </p> 
         <ul> 
          <li> <p>문제 발생</p> </li> 
          <li> <p>위험 상태</p> </li> 
          <li> <p>대상</p> </li> 
         </ul> </td> 
       </tr> 
       <tr> 
        <td role="rowheader">소유자</td> 
        <td> <p>소유자 이름을 입력한 다음 목록에 나타나면 이름을 선택합니다. </p> <p>사용자, 팀, 그룹 또는 조직 이름을 입력하거나 미리 정의된 선택 사항에서 선택할 수 있습니다. </p> <p>다음과 같이 사전 정의된 필터 옵션은 항상 현재 로그인한 사용자를 참조합니다. </p> 
         <ul> 
          <li> <p><strong>내</strong>: 사용자가 소유자인 목표를 표시합니다.</p> </li> 
          <li> <p><strong>내 홈 팀</strong> 및 <strong>모든 내 팀</strong>: 홈 팀이나 팀이 소유자로 지정된 목표를 표시합니다. </p> <p>팁: 팀에 할당되지 않은 경우 목표가 표시되지 않습니다. </p> </li> 
          <li> <p><strong>내 홈 그룹</strong> 및 <strong>모든 내 그룹</strong>: 홈 그룹 또는 그룹이 소유자로 지정된 목표를 표시합니다.</p> </li> 
         </ul> </td> 
       </tr> 
      </tbody> 
     </table>

1. (선택 사항) 필터 상자의 오른쪽 아래 모서리에 있는 **재설정**&#x200B;을 클릭하여 선택한 모든 필드를 지우고 처음부터 필터 빌드를 시작합니다.
1. (선택 사항) 저장하지 않고 필터를 적용하려면 **적용**&#x200B;을 클릭하십시오.

   필터가 필터 빌더의 **저장되지 않음** 영역에 **새 필터**(으)로 표시됩니다.

   저장하지 않은 필터의 이름은 변경할 수 없습니다.

   다음에 Workfront에서 로그아웃했다가 다시 로그인하면 저장되지 않은 필터가 목표 영역에서 제거됩니다.

   >[!TIP]
   >
   >한 번에 하나의 저장되지 않은 새 필터만 가질 수 있습니다.

1. 나중에 사용하기 위해 필터를 저장하려면 **저장**&#x200B;을 클릭한 다음 **필터 이름 추가** 필드에 필터 이름을 추가하고 **완료**&#x200B;를 클릭합니다.

   필터 빌더의 **저장됨** 섹션에 필터가 저장됩니다. 나중에 이 필터를 사용할 수 있습니다.

   다음에 Workfront에 다시 로그인할 때 마지막으로 저장되고 적용된 필터가 기본적으로 표시됩니다

1. (선택 사항) **새 필터** 옆에 있는 **왼쪽 방향 화살표**&#x200B;를 클릭하여 필터 빌더를 종료하고 필터 목록으로 돌아갑니다.
1. (선택 사항) 사용자 지정 필터의 이름 위로 마우스를 가져간 후 **자세히** 메뉴를 클릭한 다음 **삭제**, **삭제**&#x200B;를 클릭합니다. 이렇게 하면 필터가 삭제되며 복구할 수 없습니다.

   >[!TIP]
   >
   >사전 정의된 필터는 삭제할 수 없습니다.

1. 필터 빌더의 오른쪽 위 모서리에 있는 **X 아이콘**&#x200B;을 클릭하여 필터 빌더를 닫습니다.

   현재 적용된 필터의 이름은 목표 목록의 오른쪽 상단 모서리에 있는 필터 아이콘 오른쪽에 표시됩니다.

   목표 목록은 필터 기준으로 필터링됩니다.

1. (선택 사항 및 조건부) 목표 정렬 섹션에서 목표를 볼 때 필터링된 목표를 보려면 **목표 표시**&#x200B;를 클릭합니다.

   ![필터링된 항목에 대한 링크 표시](assets/show-them-link-on-filtered-items-goal-list-350x109.png)

   필터 이름의 윤곽선이 노란색으로 표시되어 무시되고 있음을 나타냅니다.

   ![노란색 윤곽선 필터링](assets/filter-yellow-outline-next-to-reapply-filter-link-350x118.png)


1. (선택 사항 및 조건부) **필터 다시 적용**&#x200B;을 클릭하여 필터를 적용하고 이전 단계에서 표시한 항목을 생략합니다.


