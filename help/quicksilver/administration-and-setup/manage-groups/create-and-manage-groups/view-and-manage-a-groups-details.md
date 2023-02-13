---
title: 그룹 세부 정보 보기 및 관리
description: 관리하는 그룹 또는 하위 그룹에 대한 그룹 세부 정보 페이지를 보고 편집할 수 있습니다.
author: Caroline
feature: System Setup and Administration, People Teams and Groups
role: Admin
exl-id: edd2c58a-f912-4638-b6a3-ff3b1b622f48
source-git-commit: fe399743ee495334face9d4d632686d9472bc8ef
workflow-type: tm+mt
source-wordcount: '636'
ht-degree: 1%

---

# 그룹 세부 정보 보기 및 관리

관리하는 그룹 또는 하위 그룹에 대한 그룹 세부 정보 페이지를 보고 편집할 수 있습니다. 이 페이지에는 다음이 포함되어 있습니다.

* 그룹에 대한 설명입니다
* 비즈니스 책임자 및 그룹 관리자의 이름
* 그룹 및 해당 하위 그룹을 공개 또는 비공개로 만들 수 있는 옵션입니다

   <!--
  <li>An option that allows you to deactivate or reactivate a group and its subgroups.
  DRAFTED IN FLARE:
  Make this change when Callisto adds the
  <b>Is active</b>
   option to the Details pag
  </li>
  -->

그룹을 관리할 수 있는 다른 방법에 대한 자세한 내용은 [그룹 만들기](../../../administration-and-setup/manage-groups/create-and-manage-groups/create-a-group.md).

그룹을 비활성화하거나 다시 활성화하는 방법에 대한 자세한 내용은 [그룹 비활성화 또는 다시 활성화](../../../administration-and-setup/manage-groups/create-and-manage-groups/deactivate-or-reactivate-a-group.md).

<!--
DRAFTED IN FLARE:
Delete this paragraph when Callisto adds the
<b>Is active</b>
 option to the Details pag
-->

## 액세스 요구 사항

이 문서의 절차를 수행하려면 다음 사항이 있어야 합니다.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Workfront 플랜*</td> 
   <td>모든</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront 라이선스*</td> 
   <td> <p>플랜 </p> <p>그룹의 그룹 관리자 또는 Workfront 관리자여야 합니다. 자세한 내용은 <a href="../../../administration-and-setup/manage-groups/group-roles/group-administrators.md" class="MCXref xref">그룹 관리자</a> 및 <a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-a-user-full-administrative-access.md" class="MCXref xref">사용자에게 전체 관리자 액세스 권한 부여</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;보유하고 있는 플랜 또는 라이선스 유형을 찾아야 하는 경우 Workfront 관리자에게 문의하십시오.

## 그룹 세부 정보 보기 및 관리

1. 을(를) 클릭합니다. **기본 메뉴** 아이콘 ![](assets/main-menu-icon.png) Adobe Workfront의 오른쪽 위 모서리에서 을(를) 클릭하고 **설정** ![](assets/gear-icon-settings.png).

1. 클릭 **그룹**.

   표시되는 목록에서 관리하는 그룹과 해당 그룹의 하위 그룹을 볼 수 있습니다. Adobe Workfront 관리자는 모든 그룹을 볼 수 있습니다.

1. 편집할 최상위 그룹의 이름을 클릭합니다.
1. 그룹을 비활성화하거나 다시 활성화하려면,
1. 왼쪽 메뉴에서 **그룹 세부 정보**&#x200B;를 입력한 후 다음 중 하나를 수행합니다.

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">설명</td> 
      <td> <p>최대 512자를 입력할 수 있습니다.</p> <p>필드가 비어 있는 경우 <strong>추가</strong> 설명을 입력합니다.</p> </td> 
     </tr> 
     <tr data-mc-conditions=""> 
      <td role="rowheader">활성화됨</td> 
      <td> <p>(기본적으로 활성화됨) Workfront 인스턴스에서 그룹을 활성화합니다.</p> <p>아래 표시된 것과 같은 자동 완성 필드에서는 일반 사용자가 객체에 첨부하거나 객체를 공유하기 위해 그룹을 검색할 때 활성 그룹만 목록에 표시됩니다.</p> <p> <img src="assets/group-type-aheads.jpg"> </p> <p>사용자를 위해 이 작업을 간소화하려면 현재 사용 중이 아닌 그룹에 대해 활성 상태임 옵션을 비활성화할 수 있습니다.</p> <p>이 필드를 사용하여 활성 또는 비활성 상태에 따라 그룹 목록을 쉽게 보고, 필터링하고, 그룹화할 수 있습니다. 보기, 필터 및 목록 그룹화를 사용하는 방법에 대한 자세한 내용은 <a href="../../../reports-and-dashboards/reports/reporting-elements/reporting-elements-filters-views-groupings.md" class="MCXref xref">보고 요소: 필터, 보기 및 그룹화</a>.</p> <p>비활성 그룹에 대한 자세한 내용은 섹션을 참조하십시오 <a href="../../../administration-and-setup/manage-groups/create-and-manage-groups/deactivate-or-reactivate-a-group.md#inactive" class="MCXref xref">비활성 그룹에 대한 고려 사항</a> 기사 <a href="../../../administration-and-setup/customize-workfront/create-manage-custom-forms/delete-or-deactivate-a-custom-form.md" class="MCXref xref">사용자 지정 양식 삭제 또는 비활성화</a>.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">그룹 접근성</td> 
      <td> <p>(하위 그룹이 아닌 그룹의 세부 정보를 보고 있는 경우에만 사용할 수 있습니다.) 옵션을 활성화 또는 비활성화합니다 <strong>이 그룹 및 하위 그룹을 비공개로 지정</strong>.</p> <p>공개 그룹의 경우 편집 사용자 액세스 권한이 있는 사용자(그룹 내 또는 그룹 외부)가 다른 사용자의 프로필에 그룹을 추가할 수 있습니다. 개인 그룹에 대해서는 이 작업을 수행할 수 없습니다.</p> <p>이 옵션은 둘 이상의 수준이 있는 그룹 계층 구조의 맨 위 상위 그룹에서만 편집할 수 있습니다. 상위 그룹의 모든 하위 그룹은 해당 설정을 상속합니다.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">그룹 이해 당사자</td> 
      <td> 
       <ul> 
        <li><strong>그룹 관리자</strong>: 계획자 라이센스가 있는 사용자를 그룹의 그룹 관리자로 추가하거나 제거합니다. 사용자 이름을 입력하기 시작한 다음 드롭다운 메뉴에 표시되는 이름을 클릭합니다.</li> 
        <li><strong>비즈니스 리더</strong>: 다음 중 하나를 수행합니다.
         <ul>
          <li>그룹에 대한 비즈니스 리더를 아직 할당하지 않은 경우 <strong>추가</strong>을(를) 클릭하고 할당할 사용자의 이름을 입력한 다음 해당 사용자의 이름이 나타나면 해당 이름을 클릭합니다.</li>
          <li>그룹에 이미 비즈니스 리더가 있고 이를 변경하려면 기존 비즈니스 리더의 이름을 두 번 누릅니다. 이름을 삭제하고 할당할 사용자의 이름을 입력한 다음 해당 사용자의 이름이 나타나면 이름을 클릭합니다.</li>
         </ul></li> 
       </ul> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">사용자 정의 양식 추가</td> 
      <td>액세스 수준에서 사용자 지정 양식을 관리할 수 있는 경우 사용자 지정 양식을 그룹에 추가합니다. 자세한 내용은 <a href="../../../administration-and-setup/customize-workfront/create-manage-custom-forms/create-and-manage-custom-forms.md" class="MCXref xref">사용자 지정 양식</a>.</td> 
     </tr> 
    </tbody> 
   </table>
