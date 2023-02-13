---
user-type: administrator
content-type: reference;overview
product-area: system-administration;user-management
navigation-topic: groups-overview
title: 하위 그룹 개요
description: 하나의 그룹에 최대 14개의 하위 그룹 수준을 만들 수 있습니다. 이러한 수준 중 하나에서 병렬 하위 그룹을 무제한으로 만들 수 있습니다.
author: Caroline
feature: System Setup and Administration, People Teams and Groups
role: Admin
exl-id: a4280498-6719-4911-a69a-b715a5438eed
source-git-commit: f2f825280204b56d2dc85efc7a315a4377e551c7
workflow-type: tm+mt
source-wordcount: '637'
ht-degree: 0%

---

# 하위 그룹 개요

하나의 그룹에 최대 14개의 하위 그룹 수준을 만들 수 있습니다. 이러한 수준 중 하나에서 병렬 하위 그룹을 무제한으로 만들 수 있습니다. 자세한 내용은 [하위 그룹 만들기](../../../administration-and-setup/manage-groups/create-and-manage-subgroups/create-a-subgroup.md).

그룹에 대한 자세한 내용은 [그룹 개요](../../../administration-and-setup/manage-groups/groups-overview/groups.md).

## 하위 그룹은 어떤 것을 상속합니까?

하위 그룹은 상위 그룹의 구성원을 상속합니다. 따라서 하위 그룹의 사용자 및 그룹은 공유되는 상위 그룹에 속하는 사용자와 그룹과 동일한 가시성, 권한 및 모든 객체에 대한 액세스 권한을 갖습니다.

또한 하위 그룹은 최상위 그룹의 그룹 관리자를 자동으로 상속하지만 하위 그룹의 구성원을 그룹 관리자로 지정할 수도 있습니다.

>[!TIP]
>
>경우에 따라 하위 그룹을 사용하여 기존 그룹에 여러 사용자를 추가하여 필요한 객체에 액세스할 수 있도록 할 수 있습니다.
>
>예를 들어, 헬프데스크 기술자 그룹과 별도의 IT 책임자 그룹이 있다고 가정합니다. 도움말 데스크 그룹에 특정 요청 큐에 대한 권한이 있습니다. IT 디렉터는 Request Queue에 대한 권한도 갖도록 Help Desk 그룹에 추가하려고 합니다. 하위 그룹 기능이 없으면 수동으로 IT 디렉터를 헬프데스크 그룹에 추가해야 하므로 비효율적이고 관리가 어렵습니다. IT 디렉터 그룹을 Help Desk 그룹에 하위 그룹으로 추가하는 경우 한 번의 변경 작업으로 이 작업을 보다 빠르게 수행할 수 있습니다.

>[!NOTE]
>
>사용자가 하위 그룹과 상위 그룹 모두에 개별적으로 추가된 경우 해당 사용자를 한 그룹에서 제거해도 다른 그룹에서 사용자가 제거되지 않습니다. 사용자에게 상위 그룹에 대한 액세스 권한이 허용되지 않게 하려면 하위 그룹과 상위 그룹에서 사용자를 모두 제거해야 합니다.

## 공용 및 개인 하위 그룹

공개 그룹의 경우 편집 사용자 액세스 권한이 있는 사용자(그룹 내 또는 그룹 외부)가 다른 사용자의 프로필에 그룹을 추가할 수 있습니다. 개인 그룹에 대해서는 이 작업을 수행할 수 없습니다.

이 옵션은 둘 이상의 수준이 있는 그룹 계층 구조의 맨 위 상위 그룹에서만 편집할 수 있습니다. 상위 그룹의 모든 하위 그룹은 해당 설정을 상속합니다.

공개되는 그룹 아래에 하위 그룹을 만들면 기본적으로 하위 그룹도 공개됩니다. 그룹 만들기 및 공개에 대한 자세한 내용은 [그룹 만들기](../../../administration-and-setup/manage-groups/create-and-manage-groups/create-a-group.md). 사용자 편집에 필요한 액세스에 대한 자세한 내용은 [사용자에게 액세스 권한 부여](../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-other-users.md).

기존 그룹에 추가하는 모든 그룹은 자동으로 하위 그룹이 되며 더 이상 주 그룹이 아닙니다. 그러나 하위 그룹에는 기존 사용자와 프로젝트, 문제 및 작업과 관련된 모든 연결, 새 상위 그룹에 속하는 모든 프로젝트, 작업 및 문제 상태가 유지됩니다.

## 하위 그룹의 그룹 관리자

<!--
Group Admins of a subgroup can't manage statuses or project preferences of the subgroup YET (Sprint 22/Oct 28, 2020)</p>
-->

하위 그룹을 만들거나 편집할 때 하위 그룹 구성원을 그룹 관리자로 지정할 수 있습니다. 자세한 내용은 [](../../../administration-and-setup/manage-groups/create-and-manage-groups/create-a-group.md#create) 기사 [그룹 만들기](../../../administration-and-setup/manage-groups/create-and-manage-groups/create-a-group.md).

또는 하위 그룹 관리를 위 그룹에 지정된 그룹 관리자에게 남겨 둘 수 있습니다. 하위 그룹을 생성할 때 하위 그룹 위에 있는 그룹의 그룹 관리자는 하위 그룹을 관리할 수 있는 자동 액세스 권한이 있습니다.

>[!NOTE]
>
>사용자를 하위 그룹에 추가하고 해당 사용자가 하위 그룹 위의 임의의 그룹에 대한 그룹 관리자인 경우, 해당 사용자는 하위 그룹에 대한 그룹 관리자로 할당되지 않고 하위 그룹을 관리할 관리 권한이 있습니다.

Workfront 시스템을 관리하는 Adobe Workfront 관리자, 최상위 그룹을 관리하는 그룹 관리자, 하위 그룹을 관리하는 그룹 관리자가 사용할 수 있는 작업을 알아보려면 [다양한 유형의 관리자에 대해 허용되는 작업](../../../administration-and-setup/manage-groups/group-roles/group-actions-allowed-different-types-admins.md).
