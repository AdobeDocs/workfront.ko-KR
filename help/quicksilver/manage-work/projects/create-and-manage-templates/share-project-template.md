---
product-area: templates
navigation-topic: templates-navigation-topic
title: 프로젝트 템플릿 공유
description: 템플릿을 사용자와 공유하거나, 템플릿 수준에서 다음 공유 옵션을 사용하여 템플릿으로 만든 프로젝트를 사용자와 공유하는 방법을 정의할 수 있습니다.
author: Alina
feature: Work Management
exl-id: 99c6b241-a2c9-4b6c-b605-177bbbc3f21a
source-git-commit: f21fd0761d942916039f6364e62f489a07217bfe
workflow-type: tm+mt
source-wordcount: '787'
ht-degree: 2%

---

# 프로젝트 템플릿 공유

템플릿을 사용자와 공유하거나, 템플릿 수준에서 다음 공유 옵션을 사용하여 템플릿으로 만든 프로젝트를 사용자와 공유하는 방법을 정의할 수 있습니다.

Adobe Workfront에서 오브젝트를 공유할 때 다른 사용자가 해당 오브젝트를 보거나, 기여하거나, 편집할 수 있도록 허용합니다.

Workfront 권한에 대한 자세한 내용은 [개체에 대한 공유 권한 개요](../../../workfront-basics/grant-and-request-access-to-objects/sharing-permissions-on-objects-overview.md)를 참조하십시오.

템플릿을 공유할 때 사용자에게 부여할 수 있는 권한에 대한 자세한 내용은 [템플릿 공유](../../../workfront-basics/grant-and-request-access-to-objects/share-a-template.md)를 참조하십시오.

## 액세스 요구 사항

이 문서의 단계를 수행하려면 다음 액세스 권한이 있어야 합니다.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront 플랜*</td> 
   <td> <p>임의 </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront 라이센스*</td> 
   <td> <p>플랜 </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">액세스 수준 구성*</td> 
   <td> <p>템플릿에 대한 액세스 편집</p> <p>참고: 여전히 액세스 권한이 없는 경우 Workfront 관리자에게 액세스 수준에서 추가 제한을 설정하는지 문의하십시오. Workfront 관리자가 액세스 수준을 수정하는 방법에 대한 자세한 내용은 <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">사용자 지정 액세스 수준 만들기 또는 수정</a>을 참조하십시오.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">개체 권한</td> 
   <td> <p>템플릿에 대한 권한 관리</p> <p>추가 액세스 요청에 대한 자세한 내용은 <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">개체 </a>에 대한 액세스 요청 을 참조하십시오.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;보유 중인 플랜, 라이선스 유형 또는 액세스 권한을 확인하려면 Workfront 관리자에게 문의하십시오.

## 템플릿 공유 {#share-a-template}

템플릿 공유를 사용하여 템플릿을 다른 사용자와 공유할 수 있습니다. 이 작업은 템플릿에 대한 권한이 있는 사용자를 정의합니다.

>[!NOTE]
>
>활성 사용자를 템플릿 소유자로 지정하면 해당 사용자는 템플릿에 대한 관리 권한을 자동으로 받습니다. 사용자를 템플릿 소유자로 지정하는 방법에 대한 자세한 내용은 [프로젝트 템플릿 편집](../../../manage-work/projects/create-and-manage-templates/edit-templates.md)을 참조하십시오.

템플릿을 공유하려면 다음 작업을 수행하십시오.

1. **주 메뉴** 아이콘 ![주 메뉴 아이콘](assets/main-menu-icon.png)에서 **서식 파일**&#x200B;을 클릭합니다.

1. 다음 중 하나를 수행하십시오.\
   템플릿 이름을 클릭하여 연 다음 **자세히** 메뉴 ![추가 아이콘](assets/qs-more-icon-on-an-object.png), **템플릿 공유**&#x200B;를 클릭합니다.

   또는

   목록에서 템플릿을 선택하고 공유 아이콘 ![](assets/share-icon.png)을(를) 클릭한 다음 **템플릿**&#x200B;을(를) 클릭합니다.

   >[!TIP]
   >
   >활성 사용자, 팀, 역할 또는 회사와만 객체를 공유할 수 있습니다.

1. **템플릿 액세스** 상자에서 템플릿을 공유할 사람, 팀, 역할, 그룹 또는 회사를 선택합니다.

   **옵션** 아이콘을 클릭하여 템플릿을 시스템 전체에서 사용할 수 있도록 설정할 수도 있습니다.

1. 공유 중인 각 엔티티의 드롭다운 메뉴에서 다음 중 하나를 선택합니다.

   * **보기**: 이러한 권한이 있는 사용자는 템플릿을 보고 템플릿을 사용하여 프로젝트를 만들거나 기존 프로젝트에 첨부할 수 있습니다.

     >[!TIP]
     >
     >프로젝트를 생성하려면 Workfront 관리자가 프로젝트에 대한 편집 액세스 권한을 부여해야 합니다.

   * **관리**: 이러한 권한이 있는 사용자는 템플릿을 편집하거나 삭제할 수 있습니다.

     여기에서 사용할 수 있는 고급 설정 ![](assets/gear-icon-in-access-levels.png)에 대한 자세한 내용은 문서 [템플릿 공유](../../../workfront-basics/grant-and-request-access-to-objects/share-a-template.md)에서 [템플릿 공유에 대한 고급 설정](../../../workfront-basics/grant-and-request-access-to-objects/share-a-template.md#template-permissions) 섹션을 참조하십시오.

1. **저장**&#x200B;을 클릭합니다.

## 템플릿에서 프로젝트 공유 {#share-a-project-from-a-template}

템플릿 프로젝트 공유를 사용하면 템플릿 수준에서 템플릿으로 만든 프로젝트에 대해 권한이 있는 사용자를 정의할 수 있습니다.

템플릿에서 생성된 향후 프로젝트를 사용자와 공유하려면 다음 작업을 수행하십시오.

1. 다음 중 하나를 수행하십시오.\
   템플릿 이름을 클릭하여 연 다음 **자세히** 메뉴 ![추가 아이콘](assets/qs-more-icon-on-an-object.png), **템플릿 공유**&#x200B;를 클릭합니다.

   ![템플릿에서 프로젝트 공유](assets/project-sharing-on-template-nwe-2022-350x172.png)

   또는

   목록에서 템플릿을 선택하고 **공유**&#x200B;를 클릭한 다음 **프로젝트를 클릭합니다.**

1. **프로젝트 액세스** 상자에서 템플릿을 공유할 사람, 팀, 역할, 그룹 또는 회사를 선택합니다.

   >[!TIP]
   >
   >활성 사용자, 팀, 역할 또는 회사와만 객체를 공유할 수 있습니다.

1. 각 엔티티에 대한 드롭다운 메뉴에서 다음을 선택합니다.

   * **액세스 권한 없음**: 템플릿에 액세스할 수 없는 사용자를 지정할 수 있습니다.\
     이 옵션은 템플릿에서 프로젝트를 대량으로 공유하는 경우에만 사용할 수 있습니다. 
   * **보기**: 이러한 권한이 있는 사용자는 템플릿에서 만든 프로젝트를 볼 수 있습니다.
   * **참여**: 이러한 권한이 있는 사용자는 템플릿에서 만든 프로젝트에 참여할 수 있습니다. 
   * **관리**: 이러한 권한이 있는 사용자는 이 템플릿에서 만든 프로젝트를 관리하거나 삭제할 수 있습니다.

1. (선택 사항) **옵션** 아이콘을 클릭하여 프로젝트를 시스템 전체에서 사용할 수 있도록 합니다.
1. **저장**&#x200B;을 클릭합니다.

<!--
<div data-mc-conditions="QuicksilverOrClassic.Draft mode">
<h3>Overview of project sharing from other sources</h3>
<p>You may already have been assigned access to projects from other areas of Workfront. <br>You may have been assigned access to projects from the following areas: </p>
<ul>
<li>When a project is created<br>For more information about sharing projects when the project is created, see the "Access" section in <a href="../../../manage-work/projects/manage-projects/edit-projects.md" class="MCXref xref">Edit projects</a>.</li>
<li>When your Workfront administrator sets user access levels<br>For more information about setting access levels, see <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Create or modify custom access levels</a>.</li>
<li>When using the project access template</li>
</ul>
<p>When using the Template Project Sharing feature, if a user's access to a project is View, but you set the access permissions for Template Project Sharing to Manage, the user will have Manage permission for every project created using this specific template. The user will only have View permission for the other projects they are on.</p>
</div>
-->

## 템플릿의 템플릿과 프로젝트를 일괄적으로 공유

여러 템플릿과 여러 템플릿의 프로젝트를 동시에 공유할 수 있습니다.

>[!NOTE]
>
>여러 템플릿을 선택하면 개별 템플릿에 대한 권한이 이미 있는 사용자를 볼 수 없습니다.

1. 템플릿 목록으로 이동합니다.
1. 여러 템플릿을 선택한 다음 ![공유](assets/share-icon.png)를 클릭합니다.

   ![템플릿 또는 프로젝트를 일괄적으로 공유](assets/share-templates-projects-in-bulk-link-in-toolbar-nwe-2022.png)

   >[!TIP]
   >
   >활성 사용자, 팀, 역할 또는 회사와만 객체를 공유할 수 있습니다.

1. 선택한 템플릿을 공유하려면 **템플릿**&#x200B;을(를) 클릭하십시오.

   또는

   선택한 템플릿에서 만들 프로젝트를 공유하려면 **프로젝트**&#x200B;를 클릭하십시오.

1. 이 문서의 다음 섹션에 설명된 대로 템플릿 또는 프로젝트를 계속 공유합니다.

   * [템플릿 공유](#share-a-template)
   * [템플릿에서 프로젝트 공유](#share-a-project-from-a-template)
