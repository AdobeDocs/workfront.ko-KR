---
title: 레이아웃 템플릿에 대한 관리 액세스 권한 부여
user-type: administrator
product-area: system-administration;templates;user-management
navigation-topic: layout-templates
description: Adobe Workfront 관리자는 특정 그룹의 그룹 관리자가 템플릿을 편집할 수 있도록 레이아웃 템플릿에 대한 관리 액세스 권한을 부여할 수 있습니다. 이렇게 해도 그룹의 사용자에게는 템플릿이 할당되지 않습니다.
author: Alina
feature: System Setup and Administration
role: Admin
exl-id: 066a55ef-1904-4678-8866-c59428f78bc1
source-git-commit: 7ee96045e5673c51c3ce348f395226857686a923
workflow-type: tm+mt
source-wordcount: '429'
ht-degree: 0%

---

# 레이아웃 템플릿에 대한 관리 액세스 권한 부여

Adobe Workfront 관리자는 특정 그룹의 그룹 관리자가 템플릿을 편집할 수 있도록 레이아웃 템플릿에 대한 관리 액세스 권한을 부여할 수 있습니다. 이렇게 해도 그룹의 사용자에게는 템플릿이 할당되지 않습니다.

레이아웃 템플릿에 사용자를 할당하는 방법에 대한 자세한 내용은 [레이아웃 템플릿에 사용자 할당](../../../administration-and-setup/customize-workfront/use-layout-templates/assign-users-to-layout-template.md)을 참조하십시오.

레이아웃 템플릿에 대한 자세한 내용은 [레이아웃 템플릿 만들기 및 관리](../../../administration-and-setup/customize-workfront/use-layout-templates/create-and-manage-layout-templates.md)를 참조하십시오.

그룹의 레이아웃 템플릿에 대한 자세한 내용은 [그룹의 레이아웃 템플릿 만들기 및 수정](../../../administration-and-setup/manage-groups/work-with-group-objects/create-and-modify-a-groups-layout-templates.md)을 참조하십시오.

## 액세스 요구 사항

이 문서의 단계를 수행하려면 다음 액세스 권한이 있어야 합니다.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront 플랜</td> 
   <td>임의</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront 라이선스</td> 
   <td>플랜</td> 
  </tr> 
  <tr> 
   <td role="rowheader">액세스 수준 구성</td> 
   <td><p>시스템 관리자 액세스 수준</p><p><b>참고</b>: 아직 액세스 권한이 없는 경우 Workfront 관리자에게 액세스 수준에 추가 제한을 설정했는지 문의하세요. Workfront 관리자가 액세스 수준을 수정하는 방법에 대한 자세한 내용은 <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">사용자 지정 액세스 수준 만들기 또는 수정</a>을 참조하십시오.</p> </td> 
  </tr> 
 </tbody> 
</table>

## 레이아웃 템플릿에 대한 관리 액세스 권한 부여

1. [레이아웃 템플릿 만들기 및 관리](../../../administration-and-setup/customize-workfront/use-layout-templates/create-and-manage-layout-templates.md)에 설명된 대로 레이아웃 템플릿 작업을 시작합니다.
1. 페이지 상단 섹션에서 **액세스 권한 부여**&#x200B;를 클릭합니다.
1. 표시되는 상자에서 **그룹 추가**&#x200B;를 클릭하고 그룹 이름을 입력한 다음 표시될 때 이름을 클릭한 다음 **완료**&#x200B;를 클릭합니다.

   지정한 그룹의 그룹 관리자로 지정된 모든 사용자는 레이아웃 템플릿을 관리할 수 있습니다. 그러나 그룹 구성원에게는 사용할 수 있는 템플릿이 할당되지 않습니다. 그룹에 레이아웃 템플릿을 할당하는 방법에 대한 자세한 내용은 이 문서에서 [사용자에게 레이아웃 템플릿 할당](../../../administration-and-setup/customize-workfront/use-layout-templates/assign-users-to-layout-template.md#assign)을 참조하십시오.

   >[!NOTE]
   >
   >* 그룹 관리자가 레이아웃 템플릿을 만들 때 관리 액세스 권한을 지정해야 합니다. 레이아웃 템플릿은에 지정되며 지정된 그룹에만 표시됩니다. 자세한 내용은 [사용자 프로필 편집](../../../administration-and-setup/add-users/create-and-manage-users/edit-a-users-profile.md)을 참조하세요. 그룹 관리자에 대한 자세한 내용은 [그룹 관리자](../../../administration-and-setup/manage-groups/group-roles/group-administrators.md)를 참조하십시오.
   >   
   >* 특정 그룹의 그룹 관리자에 대한 관리 액세스 권한을 부여하지 않는 경우 사용자 계정을 편집할 수 있는 모든 사용자는 레이아웃 템플릿에 대한 관리 액세스 권한을 갖게 됩니다. 일부 Workfront 관리자는 의도적으로 레이아웃 템플릿을 시스템 수준 레이아웃 템플릿으로 만들기 위해 해당 템플릿에 대한 관리 액세스 권한을 부여하지 않습니다.

1. 언제든지 저장 을 클릭하여 진행 상황을 저장한 다음 나중에 템플릿을 계속 수정할 수 있습니다.
