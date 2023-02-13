---
title: 그룹 관리자
user-type: administrator
content-type: reference;overview
product-area: system-administration;user-management
navigation-topic: group-roles
description: 많은 부서가 있는 대규모 조직의 Adobe Workfront 관리자는 해당 부서 내의 조직의 모든 부서 및 그룹을 관리하지 않을 수 있습니다. 대신 그룹 관리자가 관리하는 해당 그룹 내의 각 부서 및 하위 그룹에 대한 그룹을 만들 수 있습니다.
author: Caroline
feature: System Setup and Administration, People Teams and Groups
role: Admin
exl-id: 589cf9fb-f195-4b69-a240-3f73e6ca623e
source-git-commit: 03667fbdd1b0d68b9ad2d2db4a1ed85b8136062b
workflow-type: tm+mt
source-wordcount: '987'
ht-degree: 0%

---

# 그룹 관리자

많은 부서가 있는 대규모 조직의 Adobe Workfront 관리자는 해당 부서 내의 조직의 모든 부서 및 그룹을 관리하지 않을 수 있습니다. 대신 그룹 관리자가 관리하는 해당 그룹 내의 각 부서 및 하위 그룹에 대한 그룹을 만들 수 있습니다.

그룹 관리자는 사용자 멤버십, 레이아웃 템플릿, 사용자 지정 데이터, 상태 및 환경 설정과 같은 그룹의 요구 사항을 관리할 수 있습니다.

하나의 그룹 아래에 최대 14개의 하위 그룹 수준이 있을 수 있습니다.

>[!NOTE]
>
>하위 그룹 위의 계층 구조의 모든 그룹 관리자는 해당 하위 그룹을 관리할 관리 권한이 있습니다.

그룹 만들기 및 관리에 대한 자세한 내용은 [그룹 만들기](../../../administration-and-setup/manage-groups/create-and-manage-groups/create-a-group.md) 및 [그룹 관리](../../../administration-and-setup/manage-groups/create-and-manage-groups/manage-a-group.md). 또한, [하위 그룹 개요](../../../administration-and-setup/manage-groups/groups-overview/subgroups.md).

## 그룹 관리자 지정

모든 최상위 수준 그룹에는 하나 이상의 그룹 관리자가 있어야 합니다. Workfront 관리자 또는 그룹 관리자는 그룹 관리자를 그룹의 하위 그룹에 할당할 수 있지만 필수는 아닙니다. 자세한 내용은 [그룹 만들기](../../../administration-and-setup/manage-groups/create-and-manage-groups/create-a-group.md).

Workfront 관리자의 경우 사용자를 그룹 관리자로 지정하기 전에 다음을 수행하는 것이 좋습니다.

* 시스템의 현재 Workfront 관리자 수를 확인합니다.
* 시스템에 있는 그룹 수를 확인합니다.
* 일부 Workfront 관리자의 액세스 수준을 변경하고 대신 그룹 관리자로 지정할 수 있는지 여부를 결정합니다.

   그룹 관리자의 기능에 대한 자세한 내용은 [그룹 관리자가 수행한 작업](#tasks-done-by-group-administrators).

* 그룹 관리자가 다른 사용자로 로그인할 수 있도록 할지 또는 관리하는 그룹의 사용자에 대한 암호를 재설정할지 여부를 결정합니다. 이러한 작업을 수행하려면 다음에 설명된 대로 추가 액세스 권한이 필요합니다. [그룹 관리자에 필요한 액세스](#access-needed-for-group-administrators).
* 사용자 관리를 개선하려면 다음 개체에 사용자 대신 그룹이나 하위 그룹을 지정하는 것이 좋습니다.

   * 레이아웃 템플릿
   * 일정
   * 타임시트 프로필

## 그룹 관리자에 필요한 액세스 {#access-needed-for-group-administrators}

모든 그룹 관리자는 계획 라이센스가 있어야 합니다.

다음 작업을 수행할 수 있도록 그룹 관리자가 사용자에 대한 편집 액세스 권한을 갖는 것이 좋습니다.

* 관리하는 그룹 및 하위 그룹에서 다른 사용자로 로그인합니다.
* 사용자가 관리하는 그룹에서 다른 사용자의 암호를 재설정합니다.

>[!IMPORTANT]
>
>그룹 관리자는 관리하는 관리자보다 액세스 권한이 더 높아야 합니다. 그렇지 않으면 낮은 액세스 수준을 보거나 수정할 수 없습니다.
>이 액세스 권한 부여에 대한 지침은 [사용자 정의 액세스 수준 만들기 또는 수정](../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md).

그룹 및 하위 그룹의 사용자에게 작업표 프로필을 할당해야 하는 그룹 관리자의 경우 작업표와 시간에 대한 관리 액세스를 권장합니다. 이 액세스 권한 부여에 대한 지침은 [특정 영역에 대한 관리자 액세스 권한 부여](../../../administration-and-setup/add-users/configure-and-grant-access/grant-users-admin-access-certain-areas.md).

## 그룹 관리자가 수행한 작업 {#tasks-done-by-group-administrators}

그룹 관리자는 아래 작업을 수행하여 감독한 그룹을 관리할 수 있습니다. 이러한 기능 중 일부는 Workfront 관리자에게 제공되는 기능과 동일합니다.

* [그룹 구성원 관리](#manage-group-members)
* [그룹 개체 관리](#manage-group-objects)
* [그룹 환경 설정 및 도구 관리](#manage-group-preferences-and-tools)

### 그룹 구성원 관리 {#manage-group-members}

* 관리하는 그룹 및 하위 그룹 내에서 하위 그룹을 생성, 편집 및 삭제합니다. 자세한 내용은 [하위 그룹 만들기](../../../administration-and-setup/manage-groups/create-and-manage-subgroups/create-a-subgroup.md).
* 그룹 및 하위 그룹에 대한 편집 액세스 권한이 있는 사용자를 모두 추가합니다. 또는 프로필을 편집하여 그룹 및 하위 그룹에 사용자를 추가합니다.

   액세스 수준에서 사용자 관리(그룹 사용자) 권한을 활성화한 경우 그룹 구성원의 프로필에 있는 필드를 업데이트할 수도 있습니다.

   자세한 내용은 [사용자 프로필 편집](../../../administration-and-setup/add-users/create-and-manage-users/edit-a-users-profile.md).

   >[!NOTE]
   >
   >Workfront 관리자는 그룹 관리자가 수행한 그룹 멤버십의 변경 사항을 무시할 수 있습니다.

* 관리하는 그룹의 구성원인 사용자의 암호를 재설정합니다. 자세한 내용은 [사용자 프로필 편집](../../../administration-and-setup/add-users/create-and-manage-users/edit-a-users-profile.md).
* 관리하는 그룹의 구성원인 사용자로 로그인합니다. 자세한 내용은 [다른 사용자로 로그인](../../../administration-and-setup/add-users/create-and-manage-users/log-in-as-another-user.md).
* 사용 가능한 사용 가능한 라이선스 수와 그 아래 하위 그룹을 확인합니다. 자세한 내용은 [시스템에서 사용 가능한 라이센스 관리](../../../administration-and-setup/get-started-wf-administration/manage-available-licenses-in-your-system.md).

### 그룹 개체 관리 {#manage-group-objects}

* 그룹 수준 레이아웃 템플릿을 만들고 관리하는 그룹 및 하위 그룹과 연결합니다. 자세한 내용은 [레이아웃 템플릿 만들기 및 관리](../../../administration-and-setup/customize-workfront/use-layout-templates/create-and-manage-layout-templates.md).
* 그룹 수준 작업표 프로필을 만들고, 관리하는 사용자 및 그룹과 연결하고, 작업표를 수동으로 생성합니다. 자세한 내용은 [작업표 프로필 만들기, 편집 및 할당](../../../timesheets/create-and-manage-timesheets/create-timesheet-profiles.md).
* 승인 프로세스에 대한 관리자 액세스 권한이 없으면 관리하는 그룹 및 하위 그룹에 대한 승인 프로세스를 만들고 편집합니다. 자세한 내용은 [작업 항목에 대한 승인 프로세스 생성](../../../administration-and-setup/customize-workfront/configure-approval-milestone-processes/create-approval-processes.md).

   승인 프로세스에 대한 관리 액세스에 대한 자세한 내용은 [특정 영역에 대한 관리자 액세스 권한 부여](../../../administration-and-setup/add-users/configure-and-grant-access/grant-users-admin-access-certain-areas.md).

* 일정을 만들고 관리하는 그룹과 연결합니다. 자세한 내용은 [예약 만들기](../../../administration-and-setup/set-up-workfront/configure-timesheets-schedules/create-schedules.md).
* 팀 구성원이 아닌 사용자가 관리하는 그룹에 할당된 팀을 관리합니다. 또한 그룹 필드를 기반으로 팀 보고서를 만들어 특정 팀이 지정된 그룹을 식별합니다. 자세한 내용은 [팀 만들기](../../../people-teams-and-groups/create-and-manage-teams/create-a-team.md).
* 관리하는 그룹과 연결된 프로젝트를 프로젝트와 관련된 작업, 문제 또는 문서와 함께 복원합니다. 자세한 내용은 [삭제된 항목 복원](../../../administration-and-setup/manage-workfront/manage-deleted-items/restore-deleted-items.md).

### 그룹 환경 설정 및 도구 관리 {#manage-group-preferences-and-tools}

* 시스템 전체에서 그룹에 대한 프로젝트 기본 설정, 작업 또는 문제 기본 설정 또는 작업표 및 시간 기본 설정이 잠금 해제된 경우 관리하는 그룹에 대한 해당 기본 설정을 편집합니다. 이러한 환경 설정은 프로젝트, 작업 및 문제 동작에 영향을 줍니다. 자세한 내용은 다음을 참조하십시오.

   * [그룹에 대한 프로젝트 환경 설정 구성](../../../administration-and-setup/manage-groups/create-and-manage-groups/configure-project-preferences-group.md)
   * [그룹에 대한 작업 및 문제 환경 설정 구성](../../../administration-and-setup/manage-groups/create-and-manage-groups/configure-task-issue-preferences-group.md)

* 관리하는 그룹의 그룹 상태를 만들고 편집합니다. 자세한 내용은 [그룹 상태 만들기 또는 편집](../../../administration-and-setup/manage-groups/manage-group-statuses/create-or-edit-a-group-status.md).
* 관리하는 그룹에 대한 이벤트 알림을 구성합니다. Workfront 관리자가 시스템을 통해 그룹에 대한 이벤트 알림을 구성하는 기능을 잠금 해제한 후에만 이 작업을 수행할 수 있습니다. 자세한 내용은 [그룹에 대한 이벤트 알림 보기 및 구성](../../../administration-and-setup/manage-groups/create-and-manage-groups/view-and-configure-event-notifications-group.md).
