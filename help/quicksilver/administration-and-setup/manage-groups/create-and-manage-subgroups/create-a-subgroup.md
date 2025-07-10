---
user-type: administrator
product-area: system-administration;user-management
navigation-topic: create-and-manage-subgroups
title: 하위 그룹 만들기
description: 관리하는 그룹 아래에 하위 그룹을 만들어 사용자와 프로젝트를 구성하고 Adobe Workfront 내에 액세스 권한을 할당할 수 있습니다. 일반적으로 그룹 관리자는 그룹 및 하위 그룹을 관리합니다. 그룹 페이지를 사용하여 그룹과 하위 그룹을 한 곳에서 관리할 수 있습니다.
author: Lisa
feature: System Setup and Administration, People Teams and Groups
role: Admin
exl-id: b59b1491-9a78-49c0-89c9-ab1ce0099e0b
source-git-commit: 008f96d52632f5f05554d63ae1c38cc37d21544b
workflow-type: tm+mt
source-wordcount: '659'
ht-degree: 0%

---

# 하위 그룹 만들기

관리하는 그룹 아래에 하위 그룹을 만들어 사용자와 프로젝트를 구성하고 Adobe Workfront 내에 액세스 권한을 할당할 수 있습니다.

관리하는 그룹 위에 그룹이 있는 경우 해당 관리자는 해당 그룹에 대해 이 작업을 수행할 수도 있습니다. Workfront 관리자(모든 그룹)의 경우도 마찬가지입니다.

하지만 일반적으로 그룹 관리자는 그룹 및 하위 그룹을 관리합니다. 그룹 페이지를 사용하여 그룹과 하위 그룹을 한 곳에서 관리할 수 있습니다. Workfront 내에서 그룹과 하위 그룹이 작동하는 방식에 대한 자세한 내용은 [그룹 개요](../../../administration-and-setup/manage-groups/groups-overview/groups.md) 및 [하위 그룹 개요](../../../administration-and-setup/manage-groups/groups-overview/subgroups.md)를 참조하십시오.

## 액세스 요구 사항

+++ 을 확장하여 이 문서의 기능에 대한 액세스 요구 사항을 봅니다.

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
  <tr> 
   <td role="rowheader">Adobe Workfront 라이선스</td> 
   <td><p>새로운 기능: 표준</p>
       <p>또는</p>
       <p>현재: 플랜</p></td>
  </tr> 
  </tr> 
  <tr> 
   <td role="rowheader">액세스 수준 구성</td> 
   <td>그룹의 그룹 관리자 또는 시스템 관리자여야 합니다.</td>
  </tr> 
 </tbody> 
</table>

이 표의 정보에 대한 자세한 내용은 [Workfront 설명서의 액세스 요구 사항](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)을 참조하십시오.

+++

## 하위 그룹 추가

{{step-1-to-setup}}

1. **그룹**&#x200B;을 클릭합니다.

   표시되는 목록에서 관리하는 그룹과 포함된 하위 그룹을 볼 수 있습니다. Adobe Workfront 관리자는 모든 그룹을 볼 수 있습니다.

1. 새 하위 그룹을 추가하려는 기존 그룹 또는 하위 그룹을 선택합니다.
1. **새 하위 그룹**&#x200B;을 클릭합니다.
1. 표시되는 **새 하위 그룹** 상자에 하위 그룹의 **그룹 이름**&#x200B;을(를) 입력하십시오.
1. (선택 사항) 다음 정보를 입력합니다.

   * **설명**: 하위 그룹에 대한 설명을 입력하십시오. 최대 512자를 입력할 수 있습니다.
   * **활성 상태입니다**: 이 옵션은 기본적으로 활성화되어 있으며 Workfront 인스턴스에서 그룹을 활성화합니다.

     아래 표시된 것과 같은 자동 완성 필드에서는 일반 사용자가 그룹에 연결하거나 해당 그룹과 공유할 그룹을 검색할 때 활성 그룹만 목록에 표시됩니다.

     ![그룹에 대한 자동 완성 필드](assets/typeahead-for-group.png)

     사용자를 위해 이 작업을 간소화하려면 현재 사용 중이 아닌 그룹에 대해 **활성 상태임** 옵션을 비활성화하면 됩니다.

     이 필드를 사용하면 활성 또는 비활성 상태에 따라 그룹 목록을 쉽게 보고, 필터링하고, 그룹화할 수 있습니다. 목록에서 보기, 필터 및 그룹화를 사용하는 방법에 대한 자세한 내용은 [보고 요소: 필터, 보기 및 그룹화](/help/quicksilver/reports-and-dashboards/reports/reporting-elements/reporting-elements-filters-views-groupings.md)를 참조하십시오.

   * **비즈니스 리더**: 관리하는 하위 그룹의 비즈니스 리더로 한 명의 사용자를 할당할 수 있습니다. 비즈니스 리더는 하위 그룹에 대해 비즈니스 결정을 내리는 사람입니다. 자세한 내용은 [비즈니스 리더 개요](/help/quicksilver/administration-and-setup/manage-groups/group-roles/business-leader-overview.md)를 참조하십시오.

     아직 하위 그룹의 멤버가 아닌 경우 이 필드에 이름을 추가하면 그룹에도 추가됩니다.

     >[!NOTE]
     >
     >* 하위 그룹에서 비즈니스 리더를 제거하려면 먼저 비즈니스 리더 필드에서 해당 이름을 제거해야 합니다.
     >* 비즈니스 리더 필드에서 이름을 제거하면 해당 사용자는 그룹에서 제거하지 않는 한 하위 그룹의 멤버로 유지됩니다. 그룹에서 다른 사용자를 제거하는 방법에 대한 지침은 [그룹의 멤버십 보기 및 관리](/help/quicksilver/administration-and-setup/manage-groups/create-and-manage-groups/view-and-manage-a-groups-memberships.md)를 참조하세요.

   * **그룹 구성원 및 그룹 관리자**: 사용자 및 그룹을 하위 그룹의 구성원으로 추가하려면 추가할 기존 사용자 또는 그룹의 이름을 입력한 다음 표시될 때 이름을 선택하십시오.

     추가한 사용자 및 그룹은 그룹과 공유되는 모든 객체에 액세스할 수 있습니다.

     하위 그룹은 상위 그룹의 그룹 관리자를 상속하므로 사용자를 하위 그룹에 대한 그룹 관리자로 지정하는 것은 선택 사항입니다. 사용자 이름 오른쪽에 있는 드롭다운 메뉴를 사용하여 그룹 구성원을 그룹의 관리자로 지정할 수 있습니다.

   * **목록에서 사람 및 그룹 검색**: 이 하위 그룹에 이미 할당된 사용자 또는 그룹을 찾아야 하는 경우 여기에 이름을 입력하고 표시될 때 선택할 수 있습니다.

1. **저장**&#x200B;을 클릭합니다.
