---
user-type: administrator
product-area: system-administration;user-management
navigation-topic: work-with-a-groups-objects
title: 그룹의 회사 만들기 및 수정
description: 그룹 영역에서 관리하는 그룹을 볼 때 그룹과 관련된 회사 및 해당 하위 그룹을 보고 작업할 수 있습니다.
author: Lisa
feature: System Setup and Administration, People Teams and Groups
role: Admin
exl-id: 407f6631-ecc1-4ed8-bfec-6d726ae87a3d
source-git-commit: 1554c067afcc548c7f7abd03dbc3a49404e3c89c
workflow-type: tm+mt
source-wordcount: '727'
ht-degree: 0%

---

# 그룹의 회사 만들기 및 수정

그룹 영역에서 관리하는 그룹을 볼 때 그룹과 관련된 회사 및 해당 하위 그룹을 보고 작업할 수 있습니다.

그룹 위에 그룹이 있는 경우 해당 관리자는 그룹을 위해 이러한 작업을 수행할 수도 있습니다. Workfront 관리자(모든 그룹)의 경우도 마찬가지입니다.

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

## 그룹 영역에서 그룹을 위한 회사 보기, 작업 및 만들기

{{step-1-to-setup}}

1. 왼쪽 패널에서 **그룹** ![그룹](assets/groups-icon.png)을 클릭합니다.

1. 회사를 만들거나 수정할 그룹의 이름을 클릭합니다.
1. 왼쪽 패널에서 **회사**&#x200B;를 클릭하여 그룹과 관련된 회사 및 그룹에 포함될 수 있는 하위 그룹을 나열합니다.
1. (선택 사항) 회사를 추가하려면 **회사 추가**&#x200B;를 클릭한 다음 아래 나열된 옵션을 사용하여 회사를 구성하십시오. 완료되면 **회사 만들기**&#x200B;를 클릭하세요.

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">기본 정보 섹션</td> 
      <td> 
       <ul> 
        <li> <p><b>회사 이름</b>: 회사의 이름을 입력하십시오.</p> </li> 
        <li> <p><b>활성 상태임</b>: 이 옵션을 활성화하면 사용자가 회사를 찾아 만들고 편집한 프로젝트에 첨부할 수 있습니다. 비활성 회사는 프로젝트에 연결할 수 없습니다. 이 옵션은 기본적으로 활성화되어 있습니다.</p> </li> 
        <li> <p><b>기본 회사입니다</b>: 회사를 조직의 기본 회사로 할당합니다. 기본 회사는 일반적으로 대부분의 사용자가 근무하는 Workfront 계정을 나타냅니다.</p> <p>액세스 수준을 수정하여 사용자를 다른 사용자로 보도록 제한할 수 있습니다.</p> 
         <ul> 
          <li>기본 회사에서만</li> 
          <li> <p>관련 회사 및 기본 회사</p> <p>사용자의 액세스 수준 내에서 기본 회사 기능에 대한 자세한 내용은 <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref" data-mc-variable-override="">사용자 지정 액세스 수준 만들기 또는 수정</a>을 참조하세요.</p> <p>1차 회사로 지정된 회사가 하나이거나 하나도 없을 수 있지만, 여러 개의 회사를 1차 회사로 지정할 수는 없습니다. 자세한 내용은 <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref" data-mc-variable-override="">사용자 지정 액세스 수준 만들기 또는 수정</a>을 참조하세요.</p> </li> 
         </ul> </li> 
        <li> <p><b>그룹</b>: 회사와 거래하는 그룹이 있으면 여기에 그룹 이름을 추가할 수 있습니다. 이 기능은 그룹이 거래하는 모든 회사에 대해 보고하고 관리해야 하는 그룹 관리자에게 유용합니다.</p> <p data-mc-conditions="SnippetConditions-wf-groups.groups">새 회사의 <strong>그룹</strong> 필드에 사용자가 보고 있는 그룹이 입력됩니다.</p> <p data-mc-conditions="SnippetConditions-wf-groups.groups">액세스 수준에 있는 회사에 대한 관리 액세스 권한이 있는 경우 회사에서 그룹을 제거하고 다른 그룹을 할당하거나 그룹 없이 회사를 떠날 수 있습니다.</p> <p data-mc-conditions="SnippetConditions-wf-groups.groups">회사에 대한 관리 액세스 권한이 없는 경우 <strong>그룹</strong> 필드가 필요하며 관리하는 그룹이나 해당 그룹의 하위 그룹만 선택할 수 있습니다.</p> <p data-mc-conditions="SnippetConditions-wf-groups.groups">회사에 대한 관리 액세스 권한에 대한 자세한 내용은 <a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-users-admin-access-certain-areas.md" class="MCXref xref" data-mc-variable-override="">특정 영역에 대한 사용자 관리 액세스 권한 부여</a>를 참조하십시오.</p> </li> 
        <li> <p><b>회사 구성원</b>: 회사에 기존 사용자를 추가합니다. 이렇게 하면 이러한 사용자를 이 회사와 연결하게 됩니다.</p> <p>한 회사에 연결하는 사용자 수에는 제한이 없지만 사용자는 두 개 이상의 회사에 연결할 수 없습니다.</p> </li> 
       </ul> </td> 
     </tr>
     <tr> 
      <td role="rowheader">사용자 지정 Forms 섹션</td> 
      <td> <p>Workfront에서 사용할 수 없는 필드를 회사에 추가하려는 경우 사용자 정의 양식을 작성하여 회사에 연결할 수 있습니다. 드롭다운 메뉴에서 이 양식을 선택하여 회사에 첨부할 수 있습니다. 활성 회사만 드롭다운 메뉴에 나열됩니다. 사용자 정의 양식 만들기에 대한 자세한 내용은 <a href="/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/form-designer/design-a-form/design-a-form.md">사용자 정의 양식 만들기</a>를 참조하십시오. </p> </td> 
     </tr> 
    </tbody> 
   </table>

   >[!TIP]
   >
   >액세스 수준의 회사에 대한 관리 액세스 권한이 있는 경우 목록 하단의 더 많은 회사 추가를 클릭할 수도 있습니다. 이렇게 하면 새 회사를 빠르게 구성할 수 있는 행이 추가됩니다.

1. (선택 사항) 회사를 편집하거나 삭제하려면 하나 이상의 회사를 선택한 다음 도구 모음 단추를 사용하여 ![편집 아이콘](assets/edit-icon.png)을 편집하거나 ![삭제 아이콘](assets/delete.png)을(를) 삭제합니다.

   회사 편집에 대한 자세한 내용은 문서 [회사 만들기 및 편집](../../../administration-and-setup/set-up-workfront/organizational-setup/create-and-edit-companies.md#adding-a-company-to-workfront)에서 [Workfront에서 회사 만들기 또는 편집](../../../administration-and-setup/set-up-workfront/organizational-setup/create-and-edit-companies.md) 섹션을 참조하십시오.

1. (선택 사항) 회사 목록을 내보내려면 내보내기 아이콘 ![내보내기 아이콘](assets/export.png)을 클릭한 다음 내보낸 목록에 사용할 파일 형식을 선택합니다.
