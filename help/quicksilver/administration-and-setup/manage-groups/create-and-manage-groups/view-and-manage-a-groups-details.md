---
title: 그룹 세부 정보 보기 및 관리
description: 관리하는 그룹 또는 하위 그룹에 대한 그룹 세부 정보 페이지를 보고 편집할 수 있습니다.
author: Becky
feature: System Setup and Administration, People Teams and Groups
role: Admin
exl-id: edd2c58a-f912-4638-b6a3-ff3b1b622f48
source-git-commit: c711541f3e166f9700195420711d95ce782a44b2
workflow-type: tm+mt
source-wordcount: '604'
ht-degree: 1%

---

# 그룹 세부 정보 보기 및 관리

관리하는 그룹 또는 하위 그룹에 대한 그룹 세부 정보 페이지를 보고 편집할 수 있습니다. 이 페이지에는 다음이 포함되어 있습니다.

* 그룹에 대한 설명
* 비즈니스 리더 및 그룹 관리자의 이름
* 그룹 및 해당 하위 그룹을 공개 또는 비공개로 설정할 수 있는 옵션

그룹을 관리할 수 있는 다른 방법에 대한 자세한 내용은 [그룹 만들기](../../../administration-and-setup/manage-groups/create-and-manage-groups/create-a-group.md)를 참조하세요.

그룹을 비활성화하거나 다시 활성화하는 방법에 대한 자세한 내용은 [그룹 비활성화 또는 다시 활성화](../../../administration-and-setup/manage-groups/create-and-manage-groups/deactivate-or-reactivate-a-group.md)를 참조하십시오.

## 액세스 요구 사항

+++ 을 확장하여 이 문서의 기능에 대한 액세스 요구 사항을 봅니다.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>Adobe Workfront 패키지</td> 
   <td><p>임의</p></td> 
  </tr> 
  <tr> 
   <td>Adobe Workfront 라이선스</td> 
   <td><p>표준</p>
       <p>플랜</p></td>
  </tr>
  <tr> 
   <td>액세스 수준 구성</td> 
   <td>그룹의 그룹 관리자 또는 시스템 관리자여야 합니다.</td>
  </tr>
 </tbody> 
</table>

자세한 내용은 [Workfront 설명서의 액세스 요구 사항](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)을 참조하십시오.

+++

## 그룹 세부 정보 보기 및 관리

{{step-1-to-setup}}

1. **그룹**&#x200B;을 클릭합니다.

   표시되는 목록에서 관리하는 그룹과 포함된 하위 그룹을 볼 수 있습니다. Adobe Workfront 관리자는 모든 그룹을 볼 수 있습니다.

1. 편집할 최상위 그룹의 이름을 클릭합니다.
1. 그룹을 비활성화하거나 다시 활성화하려면
1. 왼쪽 메뉴에서 **그룹 세부 정보**&#x200B;를 클릭한 후 다음 중 하나를 수행합니다.

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">설명</td> 
      <td> <p>최대 512자를 입력할 수 있습니다.</p> <p>필드가 비어 있으면 <strong>추가</strong>를 클릭하여 설명을 입력하십시오.</p> </td> 
     </tr> 
     <tr data-mc-conditions=""> 
      <td role="rowheader">활성화됨</td> 
      <td> <p>(기본적으로 활성화됨) Workfront 인스턴스에서 그룹을 활성화합니다.</p> <p>아래 표시된 것처럼 자동 완성 필드에서는 일반 사용자가 그룹에 연결하거나 해당 그룹과 공유할 그룹을 검색할 때 활성 그룹만 목록에 표시됩니다.</p> <p> <img src="assets/group-type-aheads.jpg"> </p> <p>사용자를 위해 이를 간소화하려면 현재 사용 중이 아닌 그룹에 대해 [활성] 옵션을 비활성화하면 됩니다.</p> <p>이 필드를 사용하면 활성 또는 비활성 상태에 따라 그룹 목록을 쉽게 보고, 필터링하고, 그룹화할 수 있습니다. 목록에서 보기, 필터 및 그룹화를 사용하는 방법에 대한 자세한 내용은 <a href="../../../reports-and-dashboards/reports/reporting-elements/reporting-elements-filters-views-groupings.md" class="MCXref xref">보고 요소: 필터, 보기 및 그룹화</a>를 참조하십시오.</p> <p>비활성 그룹에 대한 자세한 내용은 문서 <a href="../../../administration-and-setup/manage-groups/create-and-manage-groups/deactivate-or-reactivate-a-group.md#inactive" class="MCXref xref">사용자 정의 양식 삭제 또는 비활성화</a>의 섹션 <a href="../../../administration-and-setup/customize-workfront/create-manage-custom-forms/delete-or-deactivate-a-custom-form.md" class="MCXref xref">비활성 그룹에 대한 고려 사항</a>을 참조하십시오.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">그룹 접근성</td> 
      <td> <p>(하위 그룹이 아니라 그룹의 세부 정보를 보는 경우에만 사용할 수 있습니다.) <strong>이 그룹과 하위 그룹을 비공개로 설정</strong> 옵션을 활성화하거나 비활성화합니다.</p> <p>공개 그룹의 경우, 편집 사용자 액세스 권한이 있는 모든 사용자(그룹 내 또는 그룹 외부)가 다른 사용자의 프로필에 그룹을 추가할 수 있습니다. 비공개 그룹에 대해서는 이 작업을 수행할 수 없습니다.</p> <p>수준이 둘 이상인 그룹 계층의 최상위 그룹에서만 이 옵션을 편집할 수 있습니다. 상위 그룹의 모든 하위 그룹은 해당 설정을 상속합니다.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">그룹 이해 당사자</td> 
      <td> 
       <ul> 
        <li><strong>그룹 관리자</strong>: 그룹의 그룹 관리자로 Planner 라이선스가 있는 사용자를 추가하거나 제거합니다. 사용자 이름을 입력한 다음 드롭다운 메뉴에 표시될 때 이름을 클릭합니다.</li> 
        <li><strong>비즈니스 리더</strong>: 다음 중 하나를 수행하십시오.
         <ul>
          <li>그룹에 비즈니스 리더를 아직 할당하지 않은 경우 <strong>추가</strong>를 클릭하고 할당할 사용자의 이름을 입력한 다음 해당 사용자의 이름이 나타나면 해당 이름을 클릭합니다.</li>
          <li>그룹에 이미 비즈니스 리더가 있는 경우 이를 변경하려면 기존 비즈니스 리더의 이름을 두 번 클릭합니다. 이름을 삭제하고 할당할 사용자의 이름을 입력한 다음 해당 사용자의 이름이 나타날 때 해당 이름을 클릭합니다.</li>
         </ul></li> 
       </ul> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">사용자 정의 양식 추가</td> 
      <td>액세스 수준에서 사용자 정의 양식을 관리할 수 있는 경우 사용자 정의 양식을 그룹에 추가하십시오. 자세한 내용은 <a href="../../../administration-and-setup/customize-workfront/create-manage-custom-forms/create-and-manage-custom-forms.md" class="MCXref xref">사용자 정의 양식</a>을 참조하세요.</td> 
     </tr> 
    </tbody> 
   </table>
