---
product-area: resource-management
navigation-topic: resource-pools
title: 사용자와 리소스 풀 연결
description: 리소스 풀을 사용자와 연결하려면 먼저 리소스 풀을 만들어야 합니다. 리소스 풀을 만들 때 사용자를 리소스 풀과 연결할 수 있습니다.
author: Lisa
feature: Resource Management
exl-id: 0816a2d6-2a45-4e01-8ca2-6d0d190b2568
source-git-commit: 36599722aafadcbbc630650a94005fd73b3e517e
workflow-type: tm+mt
source-wordcount: '512'
ht-degree: 1%

---

# 사용자와 리소스 풀 연결

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: The info about how to add resource pools to users, are duplicated from the articles listed in those sections (Creating Users, etc). I decided to keep the steps here because those articles are too long to rummage through for updating just this one field.)</p>
-->

리소스 풀은 Adobe Workfront에서 리소스를 관리하는 데 도움이 되는 사용자의 컬렉션입니다.

리소스 풀을 사용자와 연결하려면 먼저 리소스 풀을 만들어야 합니다.

리소스 풀을 만들 때 사용자를 리소스 풀과 연결할 수 있습니다.

사용자로 채우지 않고 리소스 풀을 만드는 경우 나중에 사용자를 편집하거나 새 사용자를 만들 때 리소스 풀을 사용자와 연결할 수 있습니다.

리소스 풀에 대한 자세한 내용은 [리소스 풀 개요](../../../resource-mgmt/resource-planning/resource-pools/work-with-resource-pools.md)를 참조하십시오.

리소스 풀 만들기에 대한 자세한 내용은 [리소스 풀 만들기](../../../resource-mgmt/resource-planning/resource-pools/create-resource-pools.md)를 참조하십시오.

## 액세스 요구 사항

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
   <td role="rowheader">Adobe Workfront 라이센스*</td> 
   <td> <p>플랜 </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">액세스 수준 구성*</td> 
   <td> <p>리소스 풀 관리에 대한 액세스 권한을 포함하는 리소스 관리에 대한 액세스 편집</p> <p>프로젝트, 템플릿 및 사용자에 대한 액세스 편집</p> <p>참고: 여전히 액세스 권한이 없는 경우 Workfront 관리자에게 액세스 수준에서 추가 제한을 설정하는지 문의하십시오. Workfront 관리자가 액세스 수준을 변경하는 방법에 대한 자세한 내용은 <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">사용자 지정 액세스 수준 만들기 또는 수정</a>을 참조하십시오.</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader">개체 권한</td> 
   <td> <p>리소스 풀을 연결할 프로젝트, 템플릿 및 사용자에 대한 권한을 관리합니다.</p> <p>추가 액세스 요청에 대한 자세한 내용은 <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">개체 </a>에 대한 액세스 요청 을 참조하십시오.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;보유 중인 플랜, 라이선스 유형 또는 액세스 권한을 확인하려면 Workfront 관리자에게 문의하십시오.

## 한 명의 사용자와 리소스 풀 연결

1. Adobe Workfront 오른쪽 상단의 **주 메뉴** 아이콘 ![](assets/main-menu-icon.png)을(를) 클릭합니다.

1. **사용자**&#x200B;를 클릭합니다.
1. 목록에서 사용자 이름 옆에 있는 상자를 선택한 다음 **편집**&#x200B;을 클릭합니다.
1. **리소스 계획**&#x200B;을 클릭합니다.
1. **리소스 풀** 필드에 사용자와 연결할 리소스 풀의 이름을 입력한 다음 목록이 나타나면 목록에서 선택하십시오.\
   여러 리소스 풀을 한 명의 사용자와 연결할 수 있습니다.\
   ![add_resource_pool_to_user.png](assets/add-resource-pool-to-user-350x307.png)

1. **변경 내용 저장**&#x200B;을 클릭합니다.

사용자 편집에 대한 자세한 내용은 [사용자 프로필 편집](../../../administration-and-setup/add-users/create-and-manage-users/edit-a-users-profile.md)을 참조하세요.

새 사용자를 만드는 방법에 대한 자세한 내용은 [사용자 추가](../../../administration-and-setup/add-users/create-and-manage-users/add-users.md)를 참조하십시오.

## 리소스 풀을 사용자와 일괄 연결

여러 사용자를 일괄적으로 편집하고 동일한 리소스 풀을 모든 사용자와 동시에 연결할 수 있습니다.

리소스 풀을 여러 사용자와 일괄 연결하려면 다음을 수행하십시오.

1. Adobe Workfront 오른쪽 상단의 **주 메뉴** 아이콘 ![](assets/main-menu-icon.png)을(를) 클릭합니다.

1. **사용자**&#x200B;를 클릭합니다.
1. 목록에서 여러 사용자를 선택하고 **편집**&#x200B;을 클릭합니다.
1. **리소스 계획**&#x200B;을 클릭합니다.
1. **리소스 풀** 필드에 사용자와 연결할 리소스 풀의 이름을 입력한 다음 목록이 나타나면 해당 이름을 선택하십시오.\
   여러 리소스 풀을 여러 사용자와 연결할 수 있습니다.

   >[!NOTE]
   >
   >이 필드에는 선택한 모든 사용자에게 공통되는 리소스 풀만 표시됩니다. 선택한 사용자에게 공유 리소스 풀이 없는 경우 이 필드는 비어 있습니다. 이 필드가 비어 있으면 여기에서 지정한 리소스 풀이 해당 개별 리소스 풀을 덮어씁니다.

1. **변경 내용 저장**&#x200B;을 클릭합니다.

사용자를 일괄 편집하는 방법에 대한 자세한 내용은 [사용자 프로필 일괄 편집](../../../administration-and-setup/add-users/create-and-manage-users/edit-user-profiles-in-bulk.md)을 참조하십시오.
