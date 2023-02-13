---
title: 그룹
user-type: administrator
content-type: reference;overview
product-area: system-administration;user-management
navigation-topic: groups-overview
description: Workfront 관리자는 부서 구조와 일치하는 사용자 그룹을 생성할 수 있습니다. 그룹은 팀 및 회사와 유사하지만 구별됩니다. Workfront 관리자는 그룹에게 작업 및 커뮤니케이션이 필요한 Workfront 영역에 대한 액세스 권한을 부여합니다. 그런 다음 각 그룹은 사용자, 템플릿, 사용자 지정 양식 등의 Workfront 정보 및 프로젝트를 다른 부서의 정보와 별도로 유지할 수 있습니다. 각 그룹에 대해 하나 이상의 그룹 관리자가 필요합니다. 그룹 관리자는 그룹 페이지를 사용하여 그룹 그룹을 한 곳에서 관리할 수 있습니다. 하나의 그룹에 최대 14개의 하위 그룹 수준을 만들 수 있습니다.
author: Caroline
feature: System Setup and Administration, People Teams and Groups
role: Admin
exl-id: 1353ab04-7de7-4d30-a092-27807c950777
source-git-commit: f2f825280204b56d2dc85efc7a315a4377e551c7
workflow-type: tm+mt
source-wordcount: '999'
ht-degree: 0%

---

# 그룹 개요

Workfront 관리자는 부서 구조와 일치하는 사용자 그룹을 생성할 수 있습니다. 그룹은 팀 및 회사와 유사하지만 구별됩니다.

Workfront 관리자는 그룹에게 작업 및 커뮤니케이션이 필요한 Workfront 영역에 대한 액세스 권한을 부여합니다. 그런 다음 각 그룹은 사용자, 템플릿, 사용자 지정 양식 등의 Workfront 정보 및 프로젝트를 다른 부서의 정보와 별도로 유지할 수 있습니다.

각 그룹에 대해 하나 이상의 그룹 관리자가 필요합니다. 그룹 관리자는 그룹 페이지를 사용하여 그룹 그룹을 한 곳에서 관리할 수 있습니다. 자세한 내용은 [그룹 관리자](../../../administration-and-setup/manage-groups/group-roles/group-administrators.md).

하나의 그룹에 최대 14개의 하위 그룹 수준을 만들 수 있습니다. 자세한 내용은 [하위 그룹 개요](../../../administration-and-setup/manage-groups/groups-overview/subgroups.md) 및 [하위 그룹 만들기](../../../administration-and-setup/manage-groups/create-and-manage-subgroups/create-a-subgroup.md).

## 그룹을 사용하여 사용자 구성

Workfront 관리자 또는 그룹 관리자는 사용자를 그룹 및 하위 그룹에 연결할 수 있습니다. 그룹을 공개하면 계획자 라이센스를 가진 사용자가 그룹과 연결할 수 있습니다. 그룹 관리자 및 공용 그룹에 대한 자세한 내용은 [그룹 만들기](../../../administration-and-setup/manage-groups/create-and-manage-groups/create-a-group.md).

사용자를 생성할 때 해당 사용자를 적절한 홈 그룹 및 사용자가 작업해야 하는 기타 그룹에 추가하는 것이 좋습니다. 사용자는 하나의 홈 그룹만 가질 수 있지만 다른 여러 그룹에 있을 수 있습니다.

그룹의 일부가 되면 사용자는 그룹 및 하위 그룹과 공유되는 객체에 액세스할 수 있습니다. 예를 들어, 프로젝트를 그룹과 공유하는 경우 그룹 및 그룹의 하위 그룹의 사용자가 프로젝트에 액세스할 수 있습니다.

>[!TIP]
>
>조직의 부서가 프로젝트 및 해당 프로젝트의 리소스를 관리하기 위해 함께 작업하는 경우가 많다면 부서를 여러 작은 그룹으로 분할하지 않아도 됩니다. 몇몇 높은 수준의 그룹이 가장 잘 될지도 모릅니다.

그룹에는 무제한 사용자가 있을 수 있습니다.

새 사용자 만들기에 대한 자세한 내용은 [사용자 추가](../../../administration-and-setup/add-users/add-users.md).

## 객체에 대한 그룹 액세스 권한 부여

그룹과 객체를 공유하면 해당 그룹의 모든 멤버(하위 그룹의 멤버 포함)가 객체에 액세스할 수 있습니다. Workfront에서의 공유에 대한 자세한 내용은 [개체에 대한 권한 공유 개요](../../../workfront-basics/grant-and-request-access-to-objects/sharing-permissions-on-objects-overview.md).

## 그룹과 객체 연결

다음 Workfront 개체 중 하나를 만들거나 편집할 때 그룹과 연결할 수 있습니다.

* **프로젝트**: 프로젝트의 소유권을 나타내기 위해 단일 그룹을 프로젝트와 연결할 수 있습니다.

   이렇게 해도 그룹의 각 구성원이 프로젝트에 대한 권한을 암시적으로 부여하지는 않습니다. 프로젝트 사용자에게 권한을 부여하려면 프로젝트 사용자와 프로젝트를 공유하여 권한을 받아야 합니다.

   사용자는 여러 그룹의 구성원이 될 수 있지만, 프로젝트와 관련된 단일 그룹이 있을 수 있습니다. 프로젝트가 다른 그룹 또는 해당 그룹과 공유된 경우 다른 그룹의 사용자가 여전히 동일한 프로젝트에서 작업할 수 있습니다. 프로젝트와 연결된 그룹은 일반적으로 프로젝트를 완료할 책임이 있는 그룹 또는 프로젝트를 전달할 그룹입니다.

   프로젝트를 그룹과 연결하는 방법에 대한 지침은 [프로젝트 개요 영역의 정보 관리](../../../manage-work/projects/manage-projects/understand-project-overview-area.md).

* **Portfolio, 프로그램 또는 회사**: 포트폴리오, 프로그램 또는 회사를 만들거나 편집할 때 해당 그룹에 단일 그룹을 할당하여 해당 그룹이 이 그룹을 소유하거나 이에 대한 책임이 있음을 나타낼 수 있습니다. 이러한 연관성을 통해 관리자와 사용자는 자신의 그룹이 어떤 포트폴리오, 프로그램 및 회사를 쉽게 식별할 수 있습니다.

   예를 들어, 그룹 관리자는 목록이나 보고서, 그룹 열에서 포트폴리오 그룹에 할당된 메모를 사용하여 조직의 모든 포트폴리오를 나열할 수 있습니다.

   >[!NOTE]
   >
   >그룹을 포트폴리오, 프로그램 또는 그룹에 할당한다는 것은 해당 그룹의 정보가 해당 데이터에 액세스할 수 있다는 것을 자동으로 의미하지는 않습니다. 해당 사용자가 데이터를 볼 수 있으려면 먼저 그룹과 데이터에 대한 액세스 권한을 수동으로 공유해야 합니다.

   자세한 내용은 [포트폴리오 만들기](../../../manage-work/portfolios/create-and-manage-portfolios/create-portfolios.md), [프로그램 만들기](../../../manage-work/portfolios/create-and-manage-programs/create-program.md), 및 [회사 만들기 및 편집](../../../administration-and-setup/set-up-workfront/organizational-setup/create-and-edit-companies.md).

* **승인 프로세스**: 특정 그룹에 속하는 프로젝트, 작업 및 문제에 대해 승인 프로세스를 사용할 수 있도록 만들 수 있습니다. 자세한 내용은 [작업 항목에 대한 승인 프로세스 생성](../../../administration-and-setup/customize-workfront/configure-approval-milestone-processes/create-approval-processes.md).
* **이정표 경로**: 특정 그룹의 사용자가 해당 프로젝트에서 이정표 경로를 사용하도록 허용할 수 있습니다. 자세한 내용은 [이정표 경로 만들기](../../../administration-and-setup/customize-workfront/configure-approval-milestone-processes/create-milestone-path.md).
* **레이아웃 템플릿**: 그룹의 관리자에게 레이아웃 템플릿을 수정할 수 있는 권한을 부여할 수 있습니다. 자세한 내용은 [레이아웃 템플릿에 대한 관리자 액세스 권한 부여](../../../administration-and-setup/customize-workfront/use-layout-templates/grant-admin-access-layout-template.md).

* **작업표 프로필**: 작업표 프로필을 수정할 그룹의 관리자 권한을 부여할 수 있습니다. 자세한 내용은 [작업표 프로필 만들기, 편집 및 할당](../../../timesheets/create-and-manage-timesheets/create-timesheet-profiles.md).

* **예약**: 그룹의 관리자에게 예약을 수정할 수 있는 권한을 부여할 수 있습니다. 자세한 내용은 [예약 만들기](../../../administration-and-setup/set-up-workfront/configure-timesheets-schedules/create-schedules.md).
* **팀**: 그룹 및 해당 하위 그룹의 관리자가 그룹 영역에서 해당 팀을 보고 작업할 수 있도록 그룹과 그룹을 연관시킬 수 있습니다. 자세한 내용은 [팀 만들기](../../../people-teams-and-groups/create-and-manage-teams/create-a-team.md) 또는 [팀 설정 편집](../../../people-teams-and-groups/create-and-manage-teams/edit-team-settings.md).
* **템플릿**: 프로젝트 템플릿에 그룹을 할당할 수 있습니다. 이를 통해 프로젝트 생성 프로세스를 간소화할 수 있고, 프로젝트 템플릿을 소유하는 그룹을 보다 쉽게 식별하고 보고할 수 있습니다. 자세한 내용은 섹션을 참조하십시오 [개요](../../../manage-work/projects/create-and-manage-templates/edit-templates.md#overview) 기사 [프로젝트 템플릿 편집](../../../manage-work/projects/create-and-manage-templates/edit-templates.md).

* **최근에 삭제 및 복원된 항목**: 최근에 삭제한 그룹을 보고 관리할 수 있습니다. 자세한 내용은 [그룹의 최근 삭제된 항목 보기 및 관리](../../../administration-and-setup/manage-groups/work-with-group-objects/view-manage-groups-recently-deleted-objects.md) 및 [그룹의 최근 복원된 항목 보기 및 관리](../../../administration-and-setup/manage-groups/work-with-group-objects/view-manage-groups-recently-restored-objects.md).
