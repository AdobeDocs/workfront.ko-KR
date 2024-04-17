---
user-type: administrator
product-area: system-administration;user-management
keywords: 만들기,그룹,하위 그룹,새로 만들기
navigation-topic: create-and-manage-groups
title: 그룹 만들기
description: Adobe Workfront 관리자는 사용자 및 프로젝트를 구성하고 Workfront 내에 액세스 권한을 할당하기 위한 그룹을 만들 수 있습니다.
author: Lisa
feature: System Setup and Administration, People Teams and Groups
role: Admin
exl-id: 4a039619-0943-4b5b-ba7a-1ad9b5c11df0
source-git-commit: 0afd578ebaa55d911c04a1d08fbcadddc1d05bbc
workflow-type: tm+mt
source-wordcount: '1677'
ht-degree: 3%

---

# 그룹 만들기

<!--
DON'T DELETE, DRAFT, OR HIDE THIS ARTICLE. IT IS LINKED TO THE PRODUCT THROUGH CONTEXT-SENSITIVE HELP LINKS.
-->

Adobe Workfront 관리자는 사용자 및 프로젝트를 구성하고 Workfront 내에 액세스 권한을 할당하기 위한 그룹을 만들 수 있습니다. 자세한 내용은 [그룹 개요](../../../administration-and-setup/manage-groups/groups-overview/groups.md).

모든 하위 그룹에는 최소 한 명 이상의 그룹 관리자가 필요합니다. 그룹 관리자는 그룹 페이지를 사용하여 한 곳에서 그룹을 관리할 수 있습니다.

그룹 관리자나 Workfront 관리자는 그룹 아래에 하위 그룹을 만들 수도 있습니다. 자세한 내용은 [하위 그룹 만들기](../../../administration-and-setup/manage-groups/create-and-manage-subgroups/create-a-subgroup.md).

## 액세스 요구 사항

이 문서의 단계를 수행하려면 다음이 있어야 합니다.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Workfront 플랜*</td> 
   <td>임의</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront 라이센스*</td> 
   <td> <p>플랜 </p> <p>그룹의 그룹 관리자 또는 Workfront 관리자여야 합니다. 자세한 내용은 <a href="../../../administration-and-setup/manage-groups/group-roles/group-administrators.md" class="MCXref xref">그룹 관리자</a> 및 <a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-a-user-full-administrative-access.md" class="MCXref xref">사용자에게 전체 관리 액세스 권한 부여</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;보유 중인 플랜 또는 라이선스 유형을 확인해야 하는 경우 Workfront 관리자에게 문의하십시오.

## 처음부터 최상위 그룹 만들기

이 단계에서는 처음부터 새 그룹을 만드는 방법을 설명합니다. 기존 그룹을 복사하여 그룹이나 하위 그룹을 생성하는 방법에 대한 자세한 내용은 [기존 그룹 또는 하위 그룹을 복사하여 최상위 그룹 생성](#create-a-top-level-group-by-copying-an-existing-group-or-subgroup) 이 문서에서.

최상위 그룹을 생성하려면 Workfront 관리자여야 합니다.

1. 다음을 클릭합니다. **메인 메뉴** 아이콘 ![](assets/main-menu-icon.png) Adobe Workfront의 오른쪽 상단에서 을(를) 클릭한 다음 **설정** ![](assets/gear-icon-settings.png).

1. 왼쪽 패널에서 **그룹** ![](assets/groups-icon.png).

1. 그룹 목록 위에서 **새 그룹**.

   >[!TIP]
   >
   >그룹 목록의 맨 아래에서 **더 많은 그룹 추가** 인라인으로 그룹을 추가하려면 **입력** 그룹 정보를 추가했으면

1. 다음에서 **새 그룹** 표시되는 상자에서 그룹의 이름을 입력합니다.
1. 다음 정보를 지정합니다.

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">그룹 이름</td> 
      <td>그룹 이름을 변경합니다.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">설명</td> 
      <td>그룹에 대한 설명을 입력합니다. 최대 512자를 입력할 수 있습니다.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">활성화됨</td> 
      <td> <p>(기본적으로 활성화됨) Workfront 인스턴스에서 그룹을 활성화합니다.</p> <p>아래 표시된 것처럼 자동 완성 필드에서는 일반 사용자가 그룹에 연결하거나 해당 그룹과 공유할 그룹을 검색할 때 활성 그룹만 목록에 표시됩니다.</p> <p> <img src="assets/group-type-aheads.jpg"> </p> <p>사용자를 위해 이를 간소화하려면 현재 사용 중이 아닌 그룹에 대해 [활성] 옵션을 비활성화하면 됩니다.</p> <p>이 필드를 사용하면 활성 또는 비활성 상태에 따라 그룹 목록을 쉽게 보고, 필터링하고, 그룹화할 수 있습니다. 목록에서 보기, 필터 및 그룹화를 사용하는 방법에 대한 자세한 내용은 <a href="../../../reports-and-dashboards/reports/reporting-elements/reporting-elements-filters-views-groupings.md" class="MCXref xref">보고 요소: 필터, 보기 및 그룹화</a>.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">이 그룹 및 해당 하위 그룹을 공개로 설정</td> 
      <td> <p>(하위 그룹이 아닌 최상위 그룹에 대한 세부 정보를 보는 경우에만 사용할 수 있습니다.) 그룹의 관리자가 아닌 그룹 내 사용자 편집 액세스 권한이 있는 사용자가 다른 사용자의 사용자 프로필에 이 그룹 및 해당 하위 그룹을 추가할 수 있도록 하려면 이 옵션을 활성화합니다.</p> <p>공개 그룹의 경우, 편집 사용자 액세스 권한이 있는 모든 사용자(그룹 내 또는 그룹 외부)가 다른 사용자의 프로필에 그룹을 추가할 수 있습니다. 비공개 그룹에 대해서는 이 작업을 수행할 수 없습니다.</p> <p>수준이 둘 이상인 그룹 계층의 최상위 그룹에서만 이 옵션을 편집할 수 있습니다. 상위 그룹의 모든 하위 그룹은 해당 설정을 상속합니다.</p> <p><b>참고</b>:  
        <ul> 
         <li>하위 그룹을 단독으로 공개로 설정할 수 없지만 최상위 수준의 상위 그룹을 공개로 설정할 수 있습니다. 이렇게 하면 상위 그룹의 모든 하위 그룹도 공개됩니다.</li> 
         <li>공개 그룹에 속한 하위 그룹은 기본적으로 공용이므로 사용자 편집 권한이 있는 모든 사용자는 다른 사용자에게도 하위 그룹을 추가할 수 있습니다.</li> 
        </ul> </p> <p>사용자를 편집하는 데 필요한 액세스 권한에 대한 정보가 필요한 경우 <a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-other-users.md" class="MCXref xref">사용자에게 액세스 권한 부여</a>. 사용자 편집에 대한 자세한 내용은 <a href="../../../administration-and-setup/add-users/create-and-manage-users/edit-a-users-profile.md" class="MCXref xref">사용자 프로필 편집</a>.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">비즈니스 리더 </td> 
      <td> <p>관리하는 그룹에 대해 한 명의 사용자를 비즈니스 리더로 할당할 수 있습니다. 비즈니스 리더는 그룹을 위해 비즈니스 결정을 내리는 사람입니다. 자세한 내용은 <a href="../../../administration-and-setup/manage-groups/group-roles/business-leader-overview.md" class="MCXref xref">비즈니스 리더 개요</a><span>.</span></p> <p>아직 그룹의 구성원이 아닌 경우 이 필드에 이름을 추가하면 그룹에도 추가됩니다.</p> <p><b>참고</b>:  
        <ul> 
         <li>그룹에서 비즈니스 리더를 제거하려면 먼저 비즈니스 리더 필드에서 비즈니스 리더의 이름을 제거해야 합니다.</li> 
         <li>비즈니스 리더 필드에서 이름을 제거할 경우, 해당 사용자에서 이름을 제거하지 않는 한 해당 사용자는 그룹의 멤버로 유지됩니다. 그룹에서 사용자를 제거하는 방법에 대한 지침은 섹션을 참조하십시오 <a href="../../../administration-and-setup/manage-groups/create-and-manage-groups/manage-a-group.md#manage" class="MCXref xref">그룹의 멤버십 관리</a> 이 문서에서 <a href="../../../administration-and-setup/manage-groups/create-and-manage-groups/manage-a-group.md" class="MCXref xref">그룹 관리</a>.</li> 
        </ul> </p> <p>자세한 내용은 <a href="../../../administration-and-setup/manage-groups/group-roles/business-leader-overview.md" class="MCXref xref">비즈니스 리더 개요</a>.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">그룹 멤버 및 그룹 관리자</td> 
      <td>
        <p>그룹 구성원을 추가하려면 추가하려는 기존 사용자 또는 그룹의 이름을 입력한 다음 표시될 때 이름을 선택합니다.</p> 
        <p>추가한 사용자 및 그룹은 그룹과 공유되는 모든 객체에 액세스할 수 있습니다.</p>
        <p>최상위 그룹에는 최소 한 명 이상의 그룹 관리자가 있어야 합니다. </p>
     </tr> 
     <tr> 
      <td role="rowheader">목록에서 직원 및 그룹 검색</td> 
      <td> 이 그룹에 이미 할당된 사용자 또는 그룹을 찾아야 하는 경우 여기에 해당 이름을 입력하고 표시될 때 선택할 수 있습니다.</td> 
     </tr> 
    </tbody> 
   </table>

1. 클릭 **그룹 만들기**.

## 기존 그룹 또는 하위 그룹을 복사하여 최상위 그룹 생성 {#create-a-top-level-group-by-copying-an-existing-group-or-subgroup}

Workfront 관리자는 기존 그룹 또는 하위 그룹을 복사하여 새 최상위 그룹을 생성할 수 있습니다.

이 작업을 수행하려면 다음 사항을 염두에 두십시오.

* 기존 그룹에 속한 모든 멤버 및 하위 그룹이 새 최상위 그룹에 복사됩니다.
* 복사된 그룹의 멤버는 원래 그룹에 있던 임무를 유지합니다. 따라서 원래 그룹의 그룹 관리자도 복사된 그룹의 그룹 관리자로 지정됩니다.

그룹 또는 하위 그룹을 복사하여 신규 최상위 레벨 그룹을 생성하려면

1. 다음을 클릭합니다. **메인 메뉴** 아이콘 ![](assets/main-menu-icon.png) Adobe Workfront의 오른쪽 상단에서 을(를) 클릭한 다음 **설정** ![](assets/gear-icon-settings.png).

1. 왼쪽 패널에서 **그룹** ![](assets/groups-icon.png).

   표시되는 목록에서 관리하는 그룹과 포함된 하위 그룹을 볼 수 있습니다. Adobe Workfront 관리자는 모든 그룹을 볼 수 있습니다.

1. 복사할 그룹을 선택한 다음 복사 아이콘을 클릭합니다 ![](assets/copy-icon.png).
1. 다음에서 **그룹 복사** 나타나는 상자에 a **그룹 이름** 복사한 그룹용입니다.

1. 다음 정보를 지정합니다.

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">그룹 이름</td> 
      <td>그룹 이름을 변경합니다.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">설명</td> 
      <td>그룹에 대한 설명을 입력합니다. 최대 512자를 입력할 수 있습니다.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">활성화됨</td> 
      <td> <p>(기본적으로 활성화됨) Workfront 인스턴스에서 그룹을 활성화합니다.</p> <p>아래 표시된 것처럼 자동 완성 필드에서는 일반 사용자가 그룹에 연결하거나 해당 그룹과 공유할 그룹을 검색할 때 활성 그룹만 목록에 표시됩니다.</p> <p> <img src="assets/group-type-aheads.jpg"> </p> <p>사용자를 위해 이를 간소화하려면 현재 사용 중이 아닌 그룹에 대해 [활성] 옵션을 비활성화하면 됩니다.</p> <p>이 필드를 사용하면 활성 또는 비활성 상태에 따라 그룹 목록을 쉽게 보고, 필터링하고, 그룹화할 수 있습니다. 목록에서 보기, 필터 및 그룹화를 사용하는 방법에 대한 자세한 내용은 <a href="../../../reports-and-dashboards/reports/reporting-elements/reporting-elements-filters-views-groupings.md" class="MCXref xref" data-mc-variable-override="">보고 요소: 필터, 보기 및 그룹화</a>.</p>  </td> 
     </tr> 
     <tr> 
      <td role="rowheader">이 그룹 및 해당 하위 그룹을 공개로 설정</td> 
      <td> <p>(하위 그룹이 아닌 최상위 그룹에 대한 세부 정보를 보는 경우에만 사용할 수 있습니다.) 그룹의 관리자가 아닌 그룹 내 사용자 편집 액세스 권한이 있는 사용자가 다른 사용자의 사용자 프로필에 이 그룹 및 해당 하위 그룹을 추가할 수 있도록 하려면 이 옵션을 활성화합니다.</p> <p>공개 그룹의 경우, 편집 사용자 액세스 권한이 있는 모든 사용자(그룹 내 또는 그룹 외부)가 다른 사용자의 프로필에 그룹을 추가할 수 있습니다. 비공개 그룹에 대해서는 이 작업을 수행할 수 없습니다.</p> <p>수준이 둘 이상인 그룹 계층의 최상위 그룹에서만 이 옵션을 편집할 수 있습니다. 상위 그룹의 모든 하위 그룹은 해당 설정을 상속합니다.</p> <p><b>참고</b>:  
        <ul> 
         <li>하위 그룹을 단독으로 공개로 설정할 수 없지만 최상위 수준의 상위 그룹을 공개로 설정할 수 있습니다. 이렇게 하면 상위 그룹의 모든 하위 그룹도 공개됩니다.</li> 
         <li>공개 그룹에 속한 하위 그룹은 기본적으로 공용이므로 사용자 편집 권한이 있는 모든 사용자는 다른 사용자에게도 하위 그룹을 추가할 수 있습니다.</li> 
        </ul> </p> <p>사용자를 편집하는 데 필요한 액세스 권한에 대한 정보가 필요한 경우 <a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-other-users.md" class="MCXref xref" data-mc-variable-override="">사용자에게 액세스 권한 부여</a>. 사용자 편집에 대한 자세한 내용은 <a href="../../../administration-and-setup/add-users/create-and-manage-users/edit-a-users-profile.md" class="MCXref xref" data-mc-variable-override="">사용자 프로필 편집</a>.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">비즈니스 리더 </td> 
      <td> <p>관리하는 그룹에 대해 한 명의 사용자를 비즈니스 리더로 할당할 수 있습니다. 비즈니스 리더는 그룹을 위해 비즈니스 결정을 내리는 사람입니다. 자세한 내용은 <a href="../../../administration-and-setup/manage-groups/group-roles/business-leader-overview.md" class="MCXref xref" data-mc-variable-override="">비즈니스 리더 개요</a><span>.</span></p> <p>아직 그룹의 구성원이 아닌 경우 이 필드에 이름을 추가하면 그룹에도 추가됩니다.</p> <p><b>참고</b>:  
        <ul> 
         <li>그룹에서 비즈니스 리더를 제거하려면 먼저 비즈니스 리더 필드에서 비즈니스 리더의 이름을 제거해야 합니다.</li> 
         <li>비즈니스 리더 필드에서 이름을 제거할 경우, 해당 사용자에서 이름을 제거하지 않는 한 해당 사용자는 그룹의 멤버로 유지됩니다. 그룹에서 사용자를 제거하는 방법에 대한 지침은 섹션을 참조하십시오 <a href="../../../administration-and-setup/manage-groups/create-and-manage-groups/manage-a-group.md#manage" class="MCXref xref" data-mc-variable-override="">그룹의 멤버십 관리</a> 이 문서에서 <a href="../../../administration-and-setup/manage-groups/create-and-manage-groups/manage-a-group.md" class="MCXref xref" data-mc-variable-override="">그룹 관리</a>.</li> 
        </ul> </p> <p>자세한 내용은 <a href="../../../administration-and-setup/manage-groups/group-roles/business-leader-overview.md" class="MCXref xref" data-mc-variable-override="">비즈니스 리더 개요</a>.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">그룹 멤버 및 그룹 관리자</td> 
      <td> 
       <ul> 
        <li> <p>그룹 구성원: 그룹에 사용자 및 그룹을 추가하려면 추가할 기존 사용자 또는 그룹의 이름을 입력한 다음 표시될 때 이름을 선택합니다.</p> <p>추가한 사용자 및 그룹은 그룹과 공유되는 모든 객체에 액세스할 수 있습니다.</p> </li> 
        <li> <p>그룹 관리자: 원래 그룹의 모든 그룹 관리자는 복사된 그룹에서 그룹 관리자로 지정됩니다. 사용자 이름 오른쪽에 있는 드롭다운 메뉴를 사용하여 그룹 구성원을 그룹의 관리자로 지정할 수 있습니다.</p> <p>최상위 그룹에는 최소 한 명 이상의 그룹 관리자가 있어야 합니다.</p> </li> 
       </ul> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">목록에서 직원 및 그룹 검색</td> 
      <td> 이 그룹에 이미 할당된 사용자 또는 그룹을 찾아야 하는 경우 여기에 해당 이름을 입력하고 표시될 때 선택할 수 있습니다.</td> 
     </tr> 
    </tbody> 
   </table>

   >[!NOTE]
   >
   >* 원래 그룹에 하위 그룹이 있는 경우, 하위 그룹은 새 그룹에 추가되며, 해당 이름은 기본적으로 &quot;원래 하위 그룹 이름(복사본)&quot;입니다.
   >* 사용자 또는 하위 그룹 이름의 오른쪽에 있는 X를 클릭하여 원래 그룹에서 사용자 또는 하위 그룹을 제거할 수 있습니다.

1. 클릭 **그룹 만들기**.
