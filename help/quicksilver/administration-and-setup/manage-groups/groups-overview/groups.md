---
title: 그룹 개요
user-type: administrator
content-type: reference;overview
product-area: system-administration;user-management
navigation-topic: groups-overview
description: Workfront 관리자는 부서 구조와 일치하는 사용자 그룹을 만들 수 있습니다. 그룹은 팀 및 회사와 유사하지만 다릅니다.
author: Becky
feature: System Setup and Administration, People Teams and Groups
role: Admin
exl-id: 1353ab04-7de7-4d30-a092-27807c950777
source-git-commit: c711541f3e166f9700195420711d95ce782a44b2
workflow-type: tm+mt
source-wordcount: '927'
ht-degree: 0%

---

# 그룹 개요

<!-- Audited: 01/2024 -->

Workfront 관리자는 부서 구조와 일치하는 사용자 그룹을 만들 수 있습니다. 그룹은 팀 및 회사와 유사하지만 다릅니다.

Workfront 관리자는 그룹에게 작업과 통신이 필요한 Workfront 영역에 대한 액세스 권한을 부여합니다. 그런 다음 각 그룹은 사용자, 템플릿 및 사용자 정의 양식과 같은 Workfront 정보와 다른 부서의 프로젝트와 분리하여 보관할 수 있습니다.

모든 그룹에 최소 한 명 이상의 그룹 관리자가 필요합니다. 그룹 관리자는 그룹 페이지를 사용하여 한 곳에서 그룹을 관리할 수 있습니다. 자세한 내용은 [그룹 관리자](../../../administration-and-setup/manage-groups/group-roles/group-administrators.md)를 참조하세요.

하나의 그룹 아래에 최대 14개의 하위 그룹 수준을 만들 수 있습니다. 자세한 내용은 [하위 그룹 개요](../../../administration-and-setup/manage-groups/groups-overview/subgroups.md) 및 [하위 그룹 만들기](../../../administration-and-setup/manage-groups/create-and-manage-subgroups/create-a-subgroup.md)를 참조하십시오.

## 그룹을 사용하여 사용자 구성

Workfront 관리자 또는 그룹 관리자는 사용자를 그룹 및 하위 그룹과 연결할 수 있습니다. 그룹을 공개로 설정하는 경우 Standard(신규) 또는 Plan(현재) 라이선스를 가진 사용자가 사용자와 그룹을 연결할 수 있습니다. 그룹 관리자 및 공용 그룹에 대한 자세한 내용은 [그룹 만들기](../../../administration-and-setup/manage-groups/create-and-manage-groups/create-a-group.md)를 참조하십시오.

사용자를 만들 때 해당 사용자를 적절한 홈 그룹 과 사용자가 작업해야 하는 다른 그룹에 추가하는 것이 좋습니다. 사용자는 홈 그룹을 하나만 가질 수 있지만 여러 다른 그룹에 있을 수 있습니다.

그룹의 일부가 되면 사용자는 그룹 및 하위 그룹과 공유되는 오브젝트에 액세스할 수 있습니다. 예를 들어 프로젝트를 그룹과 공유하는 경우 그룹 및 그룹의 하위 그룹의 사용자는 프로젝트에 액세스할 수 있습니다.

>[!TIP]
>
>조직의 부서가 프로젝트 및 해당 프로젝트에 대한 리소스를 관리하기 위해 함께 작업하는 경우가 많은 경우 부서를 여러 개의 작은 그룹으로 나눌 필요가 없을 수 있습니다. 몇 개의 높은 수준의 그룹이 가장 잘 작동할 수 있습니다.

그룹에는 무제한의 사용자가 있을 수 있습니다.

새 사용자를 만드는 방법에 대한 자세한 내용은 [사용자 추가](../../../administration-and-setup/add-users/add-users.md)를 참조하십시오.

## 객체에 대한 그룹 액세스 권한 부여

객체를 그룹과 공유할 때 해당 그룹의 모든 구성원(하위 그룹의 구성원 포함)은 해당 객체에 액세스할 수 있습니다. Workfront에서의 공유에 대한 자세한 내용은 [개체에 대한 공유 권한 개요](../../../workfront-basics/grant-and-request-access-to-objects/sharing-permissions-on-objects-overview.md)를 참조하십시오.

## 그룹과 객체 연결

다음 Workfront 개체 중 하나를 만들거나 편집할 때 그룹과 연결할 수 있습니다.

* **프로젝트**: 프로젝트의 소유권을 표시하기 위해 단일 그룹을 프로젝트와 연결할 수 있습니다.

  이는 그룹의 각 구성원에게 프로젝트에 대한 권한을 암시적으로 부여하지 않습니다. 프로젝트에 대한 권한을 가지려면 사용자가 프로젝트를 공유해야 합니다.

  사용자는 여러 그룹의 구성원이 될 수 있지만 프로젝트에는 단일 그룹이 연결될 수 있습니다. 프로젝트가 다른 그룹 또는 그룹과 공유된 경우 다른 그룹의 사용자는 여전히 동일한 프로젝트에서 작업할 수 있습니다. 일반적으로 프로젝트와 연관된 그룹은 프로젝트 완료를 담당하는 그룹 또는 프로젝트가 전달된 그룹입니다.

  프로젝트를 그룹과 연결하는 방법에 대한 지침은 [프로젝트 개요 영역의 정보 관리](../../../manage-work/projects/manage-projects/understand-project-overview-area.md)를 참조하십시오.

* **Portfolio, 프로그램 또는 회사**: 포트폴리오, 프로그램 또는 회사를 만들거나 편집할 때 그룹에 하나의 그룹을 할당하여 그룹이 소유하거나 해당 그룹에 대한 책임이 있음을 나타낼 수 있습니다. 이러한 연결을 통해 관리자와 사용자는 그룹이 작업 중인 포트폴리오, 프로그램 및 회사를 쉽게 식별할 수 있습니다.

  예를 들어 그룹 관리자는 목록이나 보고서를 사용하여 조직의 모든 포트폴리오를 나열할 수 있고 그룹 열에 자신의 그룹에 할당된 포트폴리오를 메모할 수 있습니다.

  >[!NOTE]
  >
  >그룹이 있는 포트폴리오, 프로그램 또는 회사에 그룹을 할당한다고 해서 해당 그룹의 데이터에 액세스할 수 있는 정보가 자동으로 지정되는 것은 아닙니다. 데이터를 보려면 그룹과 데이터에 대한 액세스 권한을 수동으로 공유해야 합니다.

  지침은 [포트폴리오 만들기](../../../manage-work/portfolios/create-and-manage-portfolios/create-portfolios.md), [프로그램 만들기](../../../manage-work/portfolios/create-and-manage-programs/create-program.md) 및 [회사 만들기 및 편집](../../../administration-and-setup/set-up-workfront/organizational-setup/create-and-edit-companies.md)을 참조하세요.

* **승인 프로세스**: 특정 그룹에 속한 프로젝트, 작업 및 문제에 승인 프로세스를 사용할 수 있도록 설정할 수 있습니다. 자세한 내용은 [작업 항목에 대한 승인 프로세스 만들기](../../../administration-and-setup/customize-workfront/configure-approval-milestone-processes/create-approval-processes.md)를 참조하십시오.
* **마일스톤 경로**: 특정 그룹의 사용자가 프로젝트에 마일스톤 경로를 사용하도록 허용할 수 있습니다. 자세한 내용은 [마일스톤 경로 만들기](../../../administration-and-setup/customize-workfront/configure-approval-milestone-processes/create-milestone-path.md)를 참조하세요.
* **레이아웃 템플릿**: 그룹의 관리자에게 레이아웃 템플릿을 수정할 수 있는 권한을 부여할 수 있습니다. 자세한 지침은 [레이아웃 템플릿에 대한 관리 액세스 권한 부여](../../../administration-and-setup/customize-workfront/use-layout-templates/grant-admin-access-layout-template.md)를 참조하십시오.

* **타임시트 프로필**: 그룹의 관리자에게 타임시트 프로필을 수정할 수 있는 권한을 부여할 수 있습니다. 자세한 내용은 [타임시트 프로필 만들기, 편집 및 할당](../../../timesheets/create-and-manage-timesheets/create-timesheet-profiles.md)을 참조하세요.

* **일정**: 그룹의 관리자에게 일정을 수정할 수 있는 권한을 부여할 수 있습니다. 자세한 내용은 [일정 만들기](../../../administration-and-setup/set-up-workfront/configure-timesheets-schedules/create-schedules.md)를 참조하세요.
* **팀**: 그룹 및 해당 하위 그룹의 관리자가 그룹 영역에서 해당 팀을 보고 작업할 수 있도록 그룹을 팀과 연결할 수 있습니다. 자세한 내용은 [팀 만들기](../../../people-teams-and-groups/create-and-manage-teams/create-a-team.md) 또는 [팀 설정 편집](../../../people-teams-and-groups/create-and-manage-teams/edit-team-settings.md)을 참조하세요.
* **템플릿**: 그룹을 프로젝트 템플릿에 할당할 수 있습니다. 이를 통해 프로젝트 생성 프로세스를 간소화하고 어떤 그룹이 어떤 프로젝트 템플릿을 소유하는지 보다 쉽게 식별하고 보고할 수 있습니다. 자세한 내용은 [프로젝트 템플릿 편집](../../../manage-work/projects/create-and-manage-templates/edit-templates.md#overview) 문서의 [개요](../../../manage-work/projects/create-and-manage-templates/edit-templates.md) 섹션을 참조하십시오.

* **최근에 삭제되고 복원된 항목**: 최근에 삭제된 항목 그룹을 보고 관리할 수 있습니다. 자세한 내용은 [최근 삭제된 그룹 항목 보기 및 관리](../../../administration-and-setup/manage-groups/work-with-group-objects/view-manage-groups-recently-deleted-objects.md) 및 [최근 복원된 그룹 항목 보기 및 관리](../../../administration-and-setup/manage-groups/work-with-group-objects/view-manage-groups-recently-restored-objects.md)를 참조하십시오.
