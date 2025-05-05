---
user-type: administrator
content-type: reference;overview
product-area: system-administration;user-management
navigation-topic: groups-overview
title: 하위 그룹 개요
description: 하나의 그룹 아래에 최대 14개의 하위 그룹 수준을 만들 수 있습니다. 이러한 수준 중 하나에서 병렬 하위 그룹을 무제한으로 만들 수 있습니다.
author: Lisa
feature: System Setup and Administration, People Teams and Groups
role: Admin
exl-id: a4280498-6719-4911-a69a-b715a5438eed
source-git-commit: 01487bb9cb195d6fa89bbe0fbdb7678254642714
workflow-type: tm+mt
source-wordcount: '639'
ht-degree: 0%

---

# 하위 그룹 개요

하나의 그룹 아래에 최대 14개의 하위 그룹 수준을 만들 수 있습니다. 이러한 수준 중 하나에서 병렬 하위 그룹을 무제한으로 만들 수 있습니다. 지침은 [하위 그룹 만들기](../../../administration-and-setup/manage-groups/create-and-manage-subgroups/create-a-subgroup.md)를 참조하십시오.

그룹에 대한 자세한 내용은 [그룹 개요](../../../administration-and-setup/manage-groups/groups-overview/groups.md)를 참조하세요.

## 하위 그룹은 무엇을 상속합니까?

하위 그룹은 상위 그룹의 멤버십을 상속합니다. 따라서 하위 그룹의 사용자와 그룹은 공유하는 상위 그룹에 속하는 사용자와 그룹과 모든 객체에 대해 동일한 가시성, 권한 및 액세스 권한을 갖습니다.

또한 하위 그룹은 최상위 그룹의 그룹 관리자를 자동으로 상속하지만, 하위 그룹의 멤버를 그룹 관리자로 지정할 수도 있습니다.

>[!TIP]
>
>필요한 객체에 대한 액세스 권한을 부여하기 위해 하위 그룹을 사용하여 여러 사용자를 기존 그룹에 추가할 수도 있습니다.
>
>예를 들어 헬프 데스크 기술자 그룹과 별도의 IT 책임자 그룹이 있다고 가정합니다. 헬프 데스크 그룹은 특정 요청 대기열에 대한 권한을 가집니다. 요청 대기열에 대한 사용 권한도 갖도록 헬프 데스크 그룹에 IT 디렉터를 추가하려는 경우 하위 그룹 기능이 없으면 헬프 데스크 그룹에 IT 디렉터를 수동으로 추가해야 하므로 비효율적이고 관리가 어려울 수 있습니다. 헬프 데스크 그룹에 IT 디렉터 그룹을 하위 그룹으로 추가하면 단 한 번의 변경으로 이 작업을 더 빨리 완료할 수 있습니다.

>[!NOTE]
>
>사용자가 하위 그룹과 상위 그룹 모두에 별도로 추가된 경우 한 그룹에서 사용자를 제거해도 다른 그룹에서 사용자가 제거되지 않습니다. 사용자에게 상위 그룹에 대한 액세스 권한이 허용되지 않게 하려면 하위 그룹과 상위 그룹 모두에서 사용자를 제거해야 합니다.

## 공개 및 비공개 하위 그룹

공개 그룹의 경우, 편집 사용자 액세스 권한이 있는 모든 사용자(그룹 내 또는 그룹 외부)가 다른 사용자의 프로필에 그룹을 추가할 수 있습니다. 비공개 그룹에 대해서는 이 작업을 수행할 수 없습니다.

수준이 둘 이상인 그룹 계층의 최상위 그룹에서만 이 옵션을 편집할 수 있습니다. 상위 그룹의 모든 하위 그룹은 해당 설정을 상속합니다.

공개 그룹 아래에 하위 그룹을 만들면, 기본적으로 하위 그룹도 공개입니다. 그룹을 만들고 공개하는 방법에 대한 자세한 내용은 [그룹 만들기](../../../administration-and-setup/manage-groups/create-and-manage-groups/create-a-group.md)를 참조하세요. 사용자 편집에 필요한 액세스 권한에 대한 자세한 내용은 [사용자에게 액세스 권한 부여](../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-other-users.md)를 참조하십시오.

기존 그룹에 추가하는 모든 그룹은 자동으로 하위 그룹이 되며 더 이상 주 그룹이 아닙니다. 그러나 하위 그룹은 새 상위 그룹에 속하는 모든 프로젝트, 작업 및 문제 상태 외에도 프로젝트, 문제 및 작업과의 관계를 비롯하여 기존 사용자를 유지합니다.

## 하위 그룹의 그룹 관리자

<!--
Group Admins of a subgroup can't manage statuses or project preferences of the subgroup YET (Sprint 22/Oct 28, 2020)</p>
-->

하위 그룹을 만들거나 편집할 때 하위 그룹 구성원을 그룹 관리자로 하위 그룹에 할당할 수 있습니다. 자세한 내용은 문서 [그룹 만들기](../../../administration-and-setup/manage-groups/create-and-manage-groups/create-a-group.md)의 [&#128279;](../../../administration-and-setup/manage-groups/create-and-manage-groups/create-a-group.md#create)을(를) 참조하십시오.

또는 하위 그룹의 관리를 상위 그룹에 할당된 그룹 관리자에게 위임할 수 있습니다. 하위 그룹을 만들면 상위 그룹의 그룹 관리자가 하위 그룹을 관리할 수 있는 자동 액세스 권한을 갖게 됩니다.

>[!NOTE]
>
>하위 그룹에 사용자를 추가하고 해당 사용자가 하위 그룹 위의 그룹에 대한 그룹 관리자인 경우, 해당 사용자는 하위 그룹에 대한 그룹 관리자로 지정되지 않아도 해당 하위 그룹을 관리할 수 있는 관리 권한을 갖습니다.

Workfront 시스템을 관리하는 Adobe Workfront 관리자, 최상위 그룹을 관리하는 그룹 관리자 및 하위 그룹을 관리하는 그룹 관리자가 사용할 수 있는 작업을 알아보려면 [다른 유형의 관리자에게 허용된 작업](../../../administration-and-setup/manage-groups/group-roles/group-actions-allowed-different-types-admins.md)을 참조하십시오.
