---
user-type: administrator
product-area: system-administration;user-management
keywords: 관리,그룹,편집,
navigation-topic: create-and-manage-groups
title: 그룹 관리
description: 그룹 관리자는 설정의 그룹 영역에서 관리하는 그룹을 관리할 수 있습니다. 관리하는 그룹 위에 그룹이 있으면 해당 관리자가 사용자 그룹을 위해 이 작업을 수행할 수도 있습니다. Workfront 관리자(모든 그룹의 경우)도 마찬가지입니다.
author: Caroline
feature: System Setup and Administration, People Teams and Groups
role: Admin
exl-id: 86c120de-16b8-4ca8-a7a1-76ece70c0505
source-git-commit: 02191d80ea58f80de2e7be2ff55f43663e415e31
workflow-type: tm+mt
source-wordcount: '1321'
ht-degree: 0%

---

# 그룹 관리

<!--
Though this might not seem that helpful because it is more of a catalog/TOC, it's the only article to link to for editing a group. Don't remove it.
-->

그룹 관리자는 설정의 그룹 영역에서 관리하는 그룹을 관리할 수 있습니다. 관리하는 그룹 위에 그룹이 있으면 해당 관리자가 사용자 그룹을 위해 이 작업을 수행할 수도 있습니다. Workfront 관리자(모든 그룹의 경우)도 마찬가지입니다.

>[!NOTE]
>
>그룹의 관리자로 지정되면 그 아래에 있는 하위 그룹에 대해 그룹 관리자 역할을 상속합니다. 하위 그룹을 관리할 수 있는 사용자는 하위 그룹 위의 상위 그룹에 대한 그룹 관리자와 하위 그룹에 지정된 그룹 관리자만 됩니다.

## 액세스 요구 사항

이 문서의 절차를 수행하려면 다음 사항이 있어야 합니다.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Workfront 플랜*</td> 
   <td>모든</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront 라이선스*</td> 
   <td> <p>플랜 </p> <p>그룹의 그룹 관리자 또는 Workfront 관리자여야 합니다. 자세한 내용은 <a href="../../../administration-and-setup/manage-groups/group-roles/group-administrators.md" class="MCXref xref">그룹 관리자</a> 및 <a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-a-user-full-administrative-access.md" class="MCXref xref">사용자에게 전체 관리자 액세스 권한 부여</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;보유하고 있는 플랜 또는 라이선스 유형을 찾아야 하는 경우 Workfront 관리자에게 문의하십시오.

## 그룹 구성원 관리

관리하는 그룹에서 사용자 및 기타 그룹에 사용자를 추가하고 제거할 수 있습니다. 그룹 구성원을 그룹에 대한 관리자로 지정하고 그룹 구성원의 사용자 프로필 정보를 관리할 수도 있습니다.

자세한 내용은 [그룹 멤버십 보기 및 관리](../../../administration-and-setup/manage-groups/create-and-manage-groups/view-and-manage-a-groups-memberships.md).

## 그룹 세부 정보 관리

관리하는 그룹 또는 하위 그룹에 대한 그룹 세부 정보 페이지를 보고 편집할 수 있습니다. 이 페이지에는 그룹에 대한 설명, 비즈니스 리더 및 그룹 관리자의 이름, 그룹 및 모든 하위 그룹을 공개 또는 비공개로 만들 수 있는 옵션이 포함되어 있습니다. 또한 액세스 수준에서 사용자 지정 양식을 관리할 수 있는 경우 사용자 지정 양식을 그룹에 첨부할 수 있습니다.

<!--
"and an option that allows you to deactivate or reactivate the group"

Add this at end of 2nd-to-last sentence in this^ paragraph when they add the **Is active** option to the Details page!
-->

자세한 내용은 [그룹 세부 정보 보기 및 관리](../../../administration-and-setup/manage-groups/create-and-manage-groups/view-and-manage-a-groups-details.md).

## 그룹 편집, 복사 또는 삭제

보고 있는 그룹의 기본 페이지를 종료하지 않고 빠르게 편집, 복사 또는 삭제할 수 있습니다

<!--
DRAFTED IN FLARE:
or deactivate

-->

그룹도 포함되어 있습니다.

<!--
DRAFTED IN FLARE:
Make this change when they add the </span>
<b>Is active</b>
 option to the Details page!</span>

-->

1. 을(를) 클릭합니다. **기본 메뉴** 아이콘 ![](assets/main-menu-icon.png) Adobe Workfront의 오른쪽 위 모서리에서 을(를) 클릭하고 **설정** ![](assets/gear-icon-settings.png).

1. 클릭 **그룹**.

   표시되는 목록에서 관리하는 그룹과 해당 그룹의 하위 그룹을 볼 수 있습니다. Adobe Workfront 관리자는 모든 그룹을 볼 수 있습니다.

1. 그룹을 선택한 다음 편집을 클릭합니다 ![](assets/edit-icon.png), 복사 ![](assets/copy-icon.png), 또는 삭제 ![](assets/delete.png) 아이콘.

   표시되는 상자를 사용하는 방법에 대한 정보가 필요한 경우 다음 중 하나를 참조하십시오.

   * **편집**: [그룹 세부 정보 보기 및 관리](../../../administration-and-setup/manage-groups/create-and-manage-groups/view-and-manage-a-groups-details.md)

   * **복사**: [기존 그룹 또는 하위 그룹을 복사하여 최상위 그룹을 만듭니다](../../../administration-and-setup/manage-groups/create-and-manage-groups/create-a-group.md#copying-an-existing-group-and-sub-group) 기사 [그룹 만들기](../../../administration-and-setup/manage-groups/create-and-manage-groups/create-a-group.md)

   * **삭제**: [그룹 삭제](../../../administration-and-setup/manage-groups/create-and-manage-groups/delete-a-group.md)

## 그룹에 대한 프로젝트, 작업 및 문제 환경 설정 구성

그룹 관리자이고 그룹에 시스템 수준에서 설정된 다른 프로젝트, 작업 및 문제 환경 설정이 필요한 경우 Workfront 관리자에게 조직 내 모든 그룹에 대한 환경 설정을 잠금 해제하도록 요청할 수 있습니다. 잠금이 해제된 후 관리자(및 다른 모든 그룹의 그룹 관리자)가 관리하는 그룹에 대해 그룹 관리자를 구성할 수 있습니다.

자세한 내용은 [그룹에 대한 프로젝트 환경 설정 구성](../../../administration-and-setup/manage-groups/create-and-manage-groups/configure-project-preferences-group.md) 및  [그룹에 대한 작업 및 문제 환경 설정 구성](../../../administration-and-setup/manage-groups/create-and-manage-groups/configure-task-issue-preferences-group.md).

## 하위 그룹 목록, 추가 및 구성

관리하는 그룹 아래에 하위 그룹을 생성, 보기, 편집, 복사, 이름 변경, 내보내기 및 삭제할 수 있습니다.

## 그룹에 대한 이벤트 알림 구성

Workfront 관리자가 조직의 그룹에 대한 이벤트 알림을 구성하는 기능을 잠금 해제하는 경우, 관리하는 그룹에 대해 구성할 수 있습니다. 자세한 내용은 [그룹에 대한 이벤트 알림 보기 및 구성](../../../administration-and-setup/manage-groups/create-and-manage-groups/view-and-configure-event-notifications-group.md).

## 그룹에 대한 상태 만들기 및 사용자 지정

그룹 관리자는 관리하는 최상위 그룹에 대한 사용자 지정 상태를 만들 수 있습니다. 이를 통해 조직의 자율성이 보장되며 수십 개의 회사 전체 사용자 지정 상태가 필요하지 않습니다. (Workfront 관리자는 모든 그룹에 대해 이 작업을 수행할 수도 있습니다.)

Workfront 관리자가 사용자 지정을 허용하도록 구성한 경우 최상위 그룹에 대한 시스템 상태를 사용자 지정할 수도 있습니다.

자세한 내용은 [그룹 상태 만들기 또는 편집](../../../administration-and-setup/manage-groups/manage-group-statuses/create-or-edit-a-group-status.md).

## 그룹의 프로젝트를 사용한 작업

[설정]의 [그룹] 영역에서 관리하는 그룹의 주 페이지를 볼 때 프로젝트를 사용하여 다음을 수행할 수 있습니다.

* 그룹 및 해당 하위 그룹과 연결되어 있고 사용자와 공유된 프로젝트를 나열하고 작업(편집, 복사, 삭제 및 내보내기)합니다
* 그룹에 대한 새 프로젝트 만들기

자세한 내용은 [그룹의 프로젝트 만들기 및 수정](../../../administration-and-setup/manage-groups/work-with-group-objects/create-and-modify-a-groups-projects.md).

## 그룹의 승인 프로세스 보기 및 관리

그룹 영역에서 관리하는 그룹을 보는 경우, 그룹의 관리자 또는 해당 하위 그룹 중 한 명이 관리자 액세스 권한이 있는 승인 프로세스를 보고 작업할 수 있습니다.

자세한 내용은 [그룹 수준 승인 프로세스](../../../administration-and-setup/manage-groups/work-with-group-objects/create-and-modify-groups-approval-processes.md).

## 그룹의 레이아웃 템플릿 보기 및 관리

[그룹] 영역에서 관리하는 그룹을 볼 때 그룹의 관리자 또는 해당 하위 그룹 중 하나가 관리자 액세스 권한을 가진 레이아웃 템플릿을 보고 작업할 수 있습니다.

자세한 내용은 [그룹의 레이아웃 템플릿 만들기 및 수정](../../../administration-and-setup/manage-groups/work-with-group-objects/create-and-modify-a-groups-layout-templates.md).

## 그룹 구성원의 일정 보기 및 관리

그룹에 대한 일정을 만드는 그룹 관리자는 관리자가 일정을 관리할 그룹을 지정해야 합니다. 일반적으로 이 그룹은 일정을 만드는 그룹이지만 그룹 관리자가 여러 그룹을 관리하고 다른 그룹 중 하나를 대신 지정하는 경우 다른 그룹일 수 있습니다.

관리하는 그룹의 기본 페이지를 볼 때, 관리자가 예약을 편집할 수 있는 그룹으로 지정된 경우 해당 그룹의 페이지에서 일정을 보고 관리할 수 있습니다.

자세한 내용은 [그룹의 일정 만들기 및 수정](../../../administration-and-setup/manage-groups/work-with-group-objects/create-and-modify-a-groups-schedules.md).

## 그룹 구성원의 작업표 프로필을 보고 관리합니다

관리하는 그룹의 주 페이지를 볼 때 사용자와 다른 그룹 관리 또는 하위 그룹 중 하나에서 편집할 수 있는 작업표 프로필을 관리할 수 있습니다. 자세한 내용은 [그룹의 작업표 프로필 만들기 및 관리](../../../administration-and-setup/manage-groups/work-with-group-objects/create-and-modify-a-groups-timesheet-profiles.md).

## 그룹의 하위 그룹 구성원 보기 및 관리

관리하는 그룹의 기본 페이지를 볼 때 그룹의 하위 그룹에서 모든 사용자를 보고 관리할 수 있습니다. 자세한 내용은 [하위 그룹 구성원 보기 및 관리](../../../administration-and-setup/manage-groups/create-and-manage-subgroups/view-and-manage-subgroup-members.md).

## 그룹 팀 보기 및 관리

그룹 영역에서 관리하는 그룹을 볼 때 그룹 또는 해당 하위 그룹과 연관된 팀을 보고 작업할 수 있습니다.

자세한 내용은 [그룹 팀 만들기 및 수정](../../../administration-and-setup/manage-groups/work-with-group-objects/create-and-modify-a-groups-teams.md).

## 그룹의 회사 보기 및 관리

그룹 영역에서 관리하는 그룹을 볼 때 그룹 또는 해당 하위 그룹과 연관된 회사를 보고 작업할 수 있습니다. 자세한 내용은 [그룹의 회사 만들기 및 수정](../../../administration-and-setup/manage-groups/work-with-group-objects/create-and-modify-a-groups-companies.md).

## 그룹의 포트폴리오 및 프로그램 보기 및 관리

[그룹] 영역에서 관리하는 그룹을 볼 때 다음 내용이 모두 해당되면 포트폴리오와 프로그램을 보고 작업할 수 있습니다.

* 표시된 그룹이나 하위 그룹과 연결됩니다
* 사용자가 만들었거나 사용자와 공유했기 때문에 볼 수 있는 권한이 있습니다

자세한 내용은 [그룹의 프로젝트 만들기 및 수정](../../../administration-and-setup/manage-groups/work-with-group-objects/create-and-modify-a-groups-portfolios.md) 및 [그룹의 프로그램 만들기, 수정 및 보기](../../../administration-and-setup/manage-groups/work-with-group-objects/create-and-modify-a-groups-programs.md).

## 그룹 비활성화 또는 다시 활성화

<!--
DRAFTED IN FLARE:
Delete this section when they add the </span>
<b>Is active</b>
 option to the Details page!</span>

-->

그룹을 기본 활성 상태로 유지하거나 비활성화할 수 있습니다.

그룹 비활성화는 사용자가 다른 개체와 연결하려는 그룹을 검색할 때 미리 보기 필드에서 해당 그룹을 더 이상 볼 수 없으므로 현재 사용하지 않는 경우에 유용합니다.

그룹을 비활성 또는 활성 상태로 만드는 방법에 대한 지침은 [그룹 비활성화 또는 다시 활성화](../../../administration-and-setup/manage-groups/create-and-manage-groups/deactivate-or-reactivate-a-group.md).
