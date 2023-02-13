---
product-area: resource-management
navigation-topic: resource-pools
title: 사용자와 리소스 풀 연결
description: 사용자와 리소스 풀 연결
author: Alina
feature: Resource Management
exl-id: 0816a2d6-2a45-4e01-8ca2-6d0d190b2568
source-git-commit: f2f825280204b56d2dc85efc7a315a4377e551c7
workflow-type: tm+mt
source-wordcount: '494'
ht-degree: 0%

---

# 사용자와 리소스 풀 연결

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: The info about how to add resource pools to users, are duplicated from the articles listed in those sections (Creating Users, etc). I decided to keep the steps here because those articles are too long to rummage through for updating just this one field.)</p>
-->

리소스 풀은 Adobe Workfront에서 리소스를 관리하는 데 도움이 되는 사용자의 컬렉션입니다.

사용자와 연결하려면 먼저 리소스 풀을 만들어야 합니다.

리소스 풀을 만들 때 사용자를 리소스 풀에 연결할 수 있습니다.

사용자로 채우지 않고 리소스 풀을 생성하는 경우 나중에 새 사용자를 편집하거나 만들 때 사용자와 리소스 풀을 연결할 수 있습니다.

리소스 풀에 대한 자세한 내용은 [리소스 풀 개요](../../../resource-mgmt/resource-planning/resource-pools/work-with-resource-pools.md).

리소스 풀 만들기에 대한 내용은 [리소스 풀 만들기](../../../resource-mgmt/resource-planning/resource-pools/create-resource-pools.md).

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
   <td role="rowheader">Adobe Workfront 라이선스*</td> 
   <td> <p>플랜 </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">액세스 수준 구성*</td> 
   <td> <p>리소스 풀 관리에 대한 액세스를 포함하는 리소스 관리에 대한 액세스 편집</p> <p>프로젝트, 템플릿 및 사용자에 대한 액세스 편집</p> <p>참고: 여전히 액세스 권한이 없는 경우 Workfront 관리자에게 액세스 수준에서 추가 제한 사항을 설정하는지 문의하십시오. Workfront 관리자가 액세스 수준을 변경하는 방법에 대한 자세한 내용은 <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">사용자 정의 액세스 수준 만들기 또는 수정</a>.</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader">개체 권한</td> 
   <td> <p>프로젝트, 템플릿 및 리소스 풀을</p> <p>추가 액세스 요청에 대한 자세한 내용은 <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">개체에 대한 액세스 요청 </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;어떤 계획, 라이선스 유형 또는 액세스 권한을 보유하고 있는지 알아보려면 Workfront 관리자에게 문의하십시오.

## 리소스 풀을 한 명의 사용자와 연결

1. 을(를) 클릭합니다. **기본 메뉴** 아이콘 ![](assets/main-menu-icon.png) Adobe Workfront의 오른쪽 상단 모서리에서

1. 클릭 **사용자**.
1. 목록에서 사용자 이름 옆에 있는 상자를 선택한 다음 를 클릭합니다 **편집**.
1. 클릭 **리소스 계획**.
1. 사용자에게 연결할 리소스 풀의 이름을 **리소스 풀** 필드를 선택한 다음 목록이 표시되면 목록에서 선택합니다.\
   여러 리소스 풀을 하나의 사용자와 연결할 수 있습니다.\
   ![add_resource_pool_to_user.png](assets/add-resource-pool-to-user-350x307.png)

1. 클릭 **변경 내용 저장**.

사용자 편집에 대한 자세한 내용은 [사용자 프로필 편집](../../../administration-and-setup/add-users/create-and-manage-users/edit-a-users-profile.md).

새 사용자 만들기에 대한 자세한 내용은 [사용자 추가](../../../administration-and-setup/add-users/create-and-manage-users/add-users.md).

## 리소스 풀을 사용자와 일괄 연결

여러 사용자를 일괄적으로 편집하고 동일한 리소스 풀을 모든 사용자와 동시에 연결할 수 있습니다.

여러 사용자와 자원 풀을 일괄적으로 연결하려면

1. 을(를) 클릭합니다. **기본 메뉴** 아이콘 ![](assets/main-menu-icon.png) Adobe Workfront의 오른쪽 상단 모서리에서

1. 클릭 **사용자**.
1. 목록에서 여러 사용자를 선택하고 **편집**.
1. 클릭 **리소스 계획**.
1. 에서 사용자와 연결할 리소스 풀의 이름을 입력하십시오. **리소스 풀** 필드를 선택한 다음 목록이 표시되면 목록에서 선택합니다.\
   여러 리소스 풀을 여러 사용자와 연결할 수 있습니다.

   >[!NOTE]
   >
   >선택한 모든 사용자에게 공통인 리소스 풀만 이 필드에 나타납니다. 선택한 사용자에게 공유 리소스 풀이 없는 경우 이 필드는 비어 있습니다. 이 필드가 비어 있으면 여기에서 지정하는 리소스 풀이 개별 리소스 풀을 덮어씁니다.

1. 클릭 **변경 내용 저장**.

사용자를 일괄적으로 편집하는 방법에 대한 자세한 내용은 [사용자 프로필 일괄 편집](../../../administration-and-setup/add-users/create-and-manage-users/edit-user-profiles-in-bulk.md).
