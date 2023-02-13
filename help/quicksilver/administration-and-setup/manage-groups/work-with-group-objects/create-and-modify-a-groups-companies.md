---
user-type: administrator
product-area: system-administration;user-management
navigation-topic: work-with-a-groups-objects
title: 그룹의 회사 만들기 및 수정
description: 그룹 영역에서 관리하는 그룹을 볼 때 그룹 및 해당 하위 그룹과 연관된 회사를 보고 작업할 수 있습니다.
author: Caroline
feature: System Setup and Administration, People Teams and Groups
role: Admin
exl-id: 407f6631-ecc1-4ed8-bfec-6d726ae87a3d
source-git-commit: e20934501c2117455ca7950834d868f78576dee7
workflow-type: tm+mt
source-wordcount: '811'
ht-degree: 0%

---

# 그룹의 회사 만들기 및 수정

그룹 영역에서 관리하는 그룹을 볼 때 그룹 및 해당 하위 그룹과 연관된 회사를 보고 작업할 수 있습니다.

그룹 위에 그룹이 있으면 해당 관리자가 사용자 그룹을 위해 이러한 작업을 수행할 수도 있습니다. Workfront 관리자(모든 그룹의 경우)도 마찬가지입니다.

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
   <td> <p>플랜 </p> <p>그룹의 그룹 관리자 또는 Workfront 관리자여야 합니다. 자세한 내용은 <a href="../../../administration-and-setup/manage-groups/group-roles/group-administrators.md" class="MCXref xref" data-mc-variable-override="">그룹 관리자</a> 및 <a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-a-user-full-administrative-access.md" class="MCXref xref" data-mc-variable-override="">사용자에게 전체 관리자 액세스 권한 부여</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;보유하고 있는 플랜 또는 라이선스 유형을 찾아야 하는 경우 Workfront 관리자에게 문의하십시오.

## 그룹 영역에서 그룹에 대한 회사 보기, 작업 및 생성

1. 을(를) 클릭합니다. **기본 메뉴** 아이콘 ![](assets/main-menu-icon.png) Adobe Workfront의 오른쪽 위 모서리에서 을(를) 클릭하고 **설정** ![](assets/gear-icon-settings.png).

1. 왼쪽 패널에서 **그룹** ![](assets/groups-icon.png).

1. 회사를 만들거나 수정할 그룹의 이름을 클릭합니다.
1. 왼쪽 패널에서 **회사** 그룹과 연관된 회사 및 그룹과 연관된 하위 그룹을 나열하려면 다음을 수행합니다.
1. (선택 사항) 회사를 추가하려면 **회사 추가**&#x200B;그런 다음 아래 나열된 옵션을 사용하여 회사를 구성합니다. 완료되면 를 클릭합니다 **회사 만들기**.

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">기본 정보 섹션</td> 
      <td> 
       <ul> 
        <li> <p><b>회사 이름</b>: 회사 이름을 입력합니다.</p> </li> 
        <li> <p><b>활성 상태</b>: 이 옵션이 활성화되면 사용자가 회사를 찾아 만들어 편집하는 프로젝트에 첨부할 수 있습니다. 비활성 회사는 프로젝트에 연결할 수 없습니다. 이 옵션은 기본적으로 활성화되어 있습니다.</p> </li> 
        <li> <p><b>주 회사입니다</b>: 회사를 조직의 기본 회사로 지정합니다. 기본 회사는 일반적으로 대부분의 사용자가 일하는 Workfront 계정을 나타냅니다.</p> <p>액세스 수준을 수정하여 사용자가 다른 사용자를 보도록 제한할 수 있습니다.</p> 
         <ul> 
          <li>기본 회사에서만</li> 
          <li> <p>관련 회사 및 기본 회사에서</p> <p>사용자의 액세스 수준 내 기본 회사 기능에 대한 자세한 내용은 <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref" data-mc-variable-override="">사용자 정의 액세스 수준 만들기 또는 수정</a>.</p> <p>1차 회사로 지정되는 회사는 한 개 또는 한 개만 가질 수 있지만, 1차 회사로 지정된 여러 회사를 가질 수는 없습니다. 자세한 내용은 <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref" data-mc-variable-override="">사용자 정의 액세스 수준 만들기 또는 수정</a>.</p> </li> 
         </ul> </li> 
        <li> <p><b>그룹</b>: 회사와 비즈니스를 수행하는 그룹이 있으면 여기에 그룹 이름을 추가할 수 있습니다. 이 기능은 그룹 그룹이 비즈니스 업무를 수행하는 모든 회사를 보고 관리해야 하는 그룹 관리자에게 유용합니다.</p> <p data-mc-conditions="SnippetConditions-wf-groups.groups">시스템이 <strong>그룹</strong> 보고 있는 그룹이 있는 새 회사의 필드입니다.</p> <p data-mc-conditions="SnippetConditions-wf-groups.groups">액세스 수준의 회사에 대한 관리자 액세스 권한이 있는 경우 회사에서 그룹을 제거하고 다른 그룹을 할당하거나 그룹 없이 회사를 나갈 수 있습니다.</p> <p data-mc-conditions="SnippetConditions-wf-groups.groups">회사에 대한 관리자 액세스 권한이 없는 경우 <strong>그룹</strong> 필수 필드이며 관리하는 그룹만 선택하거나 해당 그룹 아래에서 하위 그룹을 선택할 수 있습니다.</p> <p data-mc-conditions="SnippetConditions-wf-groups.groups">회사에 대한 관리 액세스에 대한 자세한 내용은 <a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-users-admin-access-certain-areas.md" class="MCXref xref" data-mc-variable-override="">특정 영역에 대한 관리자 액세스 권한 부여</a>.</p> </li> 
        <li> <p><b>회사 구성원</b>: 회사에 기존 사용자를 추가합니다. 이렇게 하면 이러한 사용자를 이 회사와 연결하게 됩니다.</p> <p>한 회사에 연결하는 사용자 수에는 제한이 없지만, 사용자는 두 개 이상의 회사와 연결할 수 없습니다.</p> </li> 
       </ul> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">청구 비율 섹션</td> 
      <td> <p>회사 레벨에서 직무 역할과 연관된 청구 비율을 대체할 수 있습니다. Job 역할 생성 및 청구 단가 연관에 대한 자세한 내용은 <a href="../../../administration-and-setup/set-up-workfront/organizational-setup/create-manage-job-roles.md" class="MCXref xref" data-mc-variable-override="">작업 역할 만들기 및 관리</a>.</p> <p>회사 레벨에서 청구 비율 재지정에 대한 자세한 내용은 <a href="../../../administration-and-setup/set-up-workfront/organizational-setup/override-job-role-billing-rates-company-level.md" class="MCXref xref" data-mc-variable-override="">회사 레벨에서 직무 역할 청구 비율 대체</a>.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">사용자 지정 Forms 섹션</td> 
      <td> <p>Workfront에서 사용할 수 없는 필드를 회사에 추가하려는 경우 사용자 지정 양식을 작성하여 회사와 연결할 수 있습니다. 이 양식은 드롭다운 메뉴에서 선택하여 회사에 첨부할 수 있습니다. 드롭다운 메뉴에는 활성 회사만 나열됩니다. 사용자 지정 Forms 만들기에 대한 내용은 <a href="../../../administration-and-setup/customize-workfront/create-manage-custom-forms/create-or-edit-a-custom-form.md" class="MCXref xref" data-mc-variable-override="">사용자 지정 양식 만들기 또는 편집</a>. </p> </td> 
     </tr> 
    </tbody> 
   </table>

   >[!TIP]
   >
   >액세스 수준의 회사에 대한 관리자 액세스 권한이 있는 경우 목록 맨 아래에 있는 추가 회사 를 클릭할 수도 있습니다. 이렇게 하면 새 회사를 빠르게 구성할 수 있는 행이 추가됩니다.

1. (선택 사항) 회사를 편집하거나 삭제하려면 하나 이상의 회사를 선택한 다음 도구 모음 단추를 사용하여 편집합니다 ![](assets/edit-icon.png) 또는 삭제 ![](assets/delete.png) 그래

   회사 편집에 대한 자세한 내용은 섹션을 참조하십시오 [Workfront에서 회사 만들기 또는 편집](../../../administration-and-setup/set-up-workfront/organizational-setup/create-and-edit-companies.md#adding-a-company-to-workfront) 기사 [회사 만들기 및 편집](../../../administration-and-setup/set-up-workfront/organizational-setup/create-and-edit-companies.md).

1. (선택 사항) 회사 목록을 내보내려면 내보내기 아이콘을 클릭합니다 ![](assets/export.png)를 선택한 다음 내보낸 목록에 사용할 파일 형식을 선택합니다.
