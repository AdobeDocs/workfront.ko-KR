---
user-type: administrator
product-area: system-administration;user-management
navigation-topic: create-and-manage-users
title: 사용자 프로필 일괄 편집
description: Adobe Workfront 관리자는 사용자 계정을 대량으로 편집할 수 있습니다.
author: Lisa
feature: System Setup and Administration
role: Admin
exl-id: cb709b2f-659e-4110-81ac-a1ef967d534c
source-git-commit: 72d0b8e0e190f774c7e3f14a78904fb1dd3f2b14
workflow-type: tm+mt
source-wordcount: '2587'
ht-degree: 0%

---

# 사용자 프로필 일괄 편집

<!--

>[!IMPORTANT]
>
>The procedure described on this page applies only to organizations that have not yet been onboarded to the Admin Console. If your organization has been onboarded to the Adobe Admin Console, you must perform this action through the Adobe Admin Console.
>
>For instructions on editing a user's profile in the Adobe Admin Console, see the section "Edit user details" in the article [Bulk Upload Users](https://helpx.adobe.com/enterprise/using/bulk-upload-users.html) or contact your Adobe Admin Console Administrator.
>
>For a list of procedures that differ based on whether your organization has been onboarded to the Adobe Admin Console, see [Platform-based administration differences (Adobe Workfront/Adobe Business Platform)](../../../administration-and-setup/get-started-wf-administration/actions-in-admin-console.md).
-->

사용자 계정을 일괄적으로 편집할 수 있습니다. 사용자를 일괄 편집할 때 특별히 선택한 필드만 선택한 모든 사용자에 대해 동일한 정보로 업데이트됩니다. 선택하지 않은 다른 모든 필드는 각 사용자에 대해 다르더라도 각 개별 사용자에 대해 동일하게 유지됩니다.

>[!NOTE]
>
>* 사용자 프로필의 개인 정보 섹션은 모든 사용자에 대해 고유해야 하므로 벌크 편집할 수 없습니다.
>* 데이터의 정확성과 최적의 성능을 보장하려면 일괄 편집을 위해 한 번에 2000명 이하의 사용자를 선택하는 것이 좋습니다.
>

## 액세스 요구 사항

+++ 을 확장하여 이 문서의 기능에 대한 액세스 요구 사항을 봅니다.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>Adobe Workfront 패키지</td> 
   <td><p>임의</p></td> 
  </tr> 
  <tr> 
   <td>Adobe Workfront 라이선스</td> 
   <td><p>표준</p><p>플랜</p></td> 
  </tr> 
  <tr> 
   <td>액세스 수준 구성</td> 
   <td> <p>다음 중 하나가 있어야 합니다.</p> 
    <ul> 
     <li> <p>시스템 관리자 액세스 수준입니다. </li> 
     <li> <p>액세스 수준의 <b>사용자</b> 설정이 <b>편집</b> 액세스로 구성되었으며, <b>만들기</b>와 <b>설정을 미세 조정</b> <b>에서 두 개의 </b>사용자 관리<img src="assets/gear-icon-in-access-levels.png"> 옵션 중 하나 이상을 사용할 수 있습니다. </p> <p>이 두 옵션 중 <b>사용자 관리자(그룹 사용자)</b>를 사용하도록 설정한 경우 사용자가 구성원인 그룹의 그룹 관리자여야 합니다.</p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

자세한 내용은 [Workfront 설명서의 액세스 요구 사항](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)을 참조하십시오.

+++

## 사용자 계정 일괄 편집

{{step-1-to-users}}

1. 사용자를 두 명 이상 선택한 다음 **편집** 아이콘 ![편집 아이콘](assets/edit-icon.png)을 클릭합니다.

1. **사용자 편집** 상자에서 모든 섹션의 정보를 변경하고 언제든지 **저장**&#x200B;을 클릭합니다.

### 환경 설정

* **시간대**: 사용자의 시간대입니다.

  사용자가 Workfront에서 시간대 간에 공동 작업하는 데 대한 자세한 내용은 [시간대 간에 작업](/help/quicksilver/workfront-basics/tips-tricks-and-troubleshooting/working-across-timezones.md)을 참조하세요.

* **전자 메일 로케일**: 사용자의 기본 전자 메일 로케일입니다. 이는 Workfront에서 이 사용자에게 제공되는 이메일의 숫자 및 날짜 형식에 영향을 줍니다.

  >[!NOTE]
  >
  >조직이 Adobe 통합 환경을 사용하는 경우 사용자의 언어 환경 설정은 Adobe 프로필에 저장되고 이메일 로케일은 사용되지 않습니다. 이러한 환경 설정에 액세스하는 방법에 대한 자세한 내용은 [Workfront용 Adobe 통합 환경](/help/quicksilver/workfront-basics/navigate-workfront/workfront-navigation/adobe-unified-experience.md)을 참조하십시오.

### 알림

사용자에 대해 활성화해야 하는 이메일 알림을 선택합니다.

인스턴트 및 일별 다이제스트 알림을 선택할 수 있습니다. 일별 다이제스트 알림은 선택한 모든 사용자에 대해 같은 시간 이후에 모두 전달됩니다.

자세한 내용은 [시스템의 모든 사용자를 위한 이벤트 알림 구성](/help/quicksilver/administration-and-setup/manage-workfront/emails/configure-event-notifications-for-everyone-in-the-system.md)을 참조하십시오.

### 액세스

* **사용자가 활성 상태입니다**: 사용자가 활성 상태임을 나타내려면 이 옵션을 활성화하십시오. 활성 사용자는 Workfront 라이선스를 사용합니다. 필드를 비활성화하면 사용자가 Workfront에 로그인할 수 없습니다.

* **액세스 수준**: 이 사용자에게 할당할 액세스 수준을 선택하십시오. 선택한 모든 사용자의 액세스 수준은 동일합니다.

  사용자에게 액세스 수준을 할당할 때 자신의 액세스 수준과 같거나 낮은 수준을 할당할 수 있습니다. (예를 들어 액세스 수준이 표준인 경우 관리자 액세스 수준을 할당할 수 없습니다.)

  하지만 Workfront 관리자가 자신의 액세스 수준에서도 활성화되지 않은 액세스 수준에 대해 기본이 아닌 권한을 활성화한 경우에는 기본적으로 자신의 액세스 수준보다 낮은 액세스 수준을 할당할 수 없습니다.

  예를 들어 작업을 삭제할 수 있는 액세스 권한이 없는 Standard 라이센스가 있는 경우 Light 라이센스가 Standard 라이센스보다 낮지만 작업을 삭제할 수 있는 액세스 권한이 있는 Light 라이센스를 다른 사용자에게 할당할 수 없습니다. 자세한 내용은 [사용자 지정 액세스 수준 만들기 또는 수정](/help/quicksilver/administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md)을 참조하세요.

  액세스 수준에 대한 자세한 내용은 [Adobe Workfront 액세스 구성](/help/quicksilver/administration-and-setup/add-users/configure-and-grant-access/configure-access.md)을 참조하십시오.

  >[!NOTE]
  >
  >조직에서 새 액세스 모델(표준/라이트/기여자)을 사용하는 경우 해당 사용자가 해당 월에 대한 결정 한도에 이미 도달한 경우 표준 또는 라이트 사용자를 기여자 액세스 수준에 재할당할 수 없습니다.
  >
  >새 액세스 모델에 대한 자세한 내용은 [새 액세스 수준 개요](/help/quicksilver/administration-and-setup/add-users/how-access-levels-work/access-level-overview.md)를 참조하십시오.
  >
  >결정 한도에 대한 자세한 내용은 [비유료 사용자에 대한 제한된 문서 및 증명 결정 개요](/help/quicksilver/review-and-approve-work/proof-doc-decision-limits.md)를 참조하십시오.

* **레이아웃 템플릿**: 사용자에 대한 레이아웃 템플릿을 선택하십시오. 이 레이아웃 템플릿은 홈 그룹, 홈 팀 또는 기본 역할에 할당된 모든 레이아웃 템플릿보다 우선합니다. 레이아웃 템플릿의 할당 우선 순위에 대한 자세한 내용은 [레이아웃 템플릿 만들기 및 관리](/help/quicksilver/administration-and-setup/customize-workfront/use-layout-templates/create-and-manage-layout-templates.md)를 참조하십시오.

  다음 목록은 이 필드에서 사용할 수 있는 템플릿 목록이 액세스 권한에 따라 어떻게 달라지는지 설명합니다.

   * Workfront 관리자는 모든 시스템 수준 및 그룹 수준 레이아웃 템플릿을 볼 수 있습니다.
   * 그룹 관리자는 시스템 수준 레이아웃 템플릿과 관리하는 그룹과 관련된 템플릿을 볼 수 있습니다.
   * Standard 또는 Plan 라이선스가 있고 사용자 편집 액세스 권한이 있는 사용자는 시스템 수준 레이아웃 템플릿만 볼 수 있습니다.

     그룹 수준 레이아웃 템플릿에 대한 자세한 내용은 [그룹의 레이아웃 템플릿 만들기 및 수정](/help/quicksilver/administration-and-setup/manage-groups/work-with-group-objects/create-and-modify-a-groups-layout-templates.md)을 참조하십시오.

### 조직

* **회사**: 사용자의 회사입니다. 사용자는 한 회사에만 연결할 수 있습니다. 회사를 사용자와 연결하려면 먼저 회사를 만들어야 합니다. 활성 회사만 목록에 표시됩니다. 회사 만들기에 대한 자세한 내용은 [회사 만들기 및 편집](/help/quicksilver/administration-and-setup/set-up-workfront/organizational-setup/create-and-edit-companies.md)을 참조하세요.
* **홈 팀**: 사용자의 홈 팀을 지정합니다. 사용자는 홈 팀을 하나만 보유할 수 있습니다.
* **다른 팀**: 사용자가 여러 팀에 속할 수 있습니다.
* **현재 홈 그룹**: 사용자를 할당할 적절한 그룹을 선택하십시오. 이를 통해 사용자는 그룹과 공유되는 오브젝트에 액세스할 수 있습니다. 홈 그룹과 레이아웃 템플릿을 공유할 수도 있습니다.

  필수 필드입니다. 모든 사용자는 홈 그룹과 연결되어 있어야 합니다. 홈 그룹을 선택하지 않으면 홈 그룹이 홈 그룹으로 할당됩니다.

  다음 중 하나가 참인 경우에만 사용자에게 그룹을 할당할 수 있습니다.

   * Workfront 관리자입니다
   * 그룹의 관리자입니다.
   * 그룹이 공개 그룹임

* **기타 그룹**: 사용자가 여러 그룹에 속할 수 있습니다. Workfront 관리자이거나 그룹의 관리자이거나 그룹이 공개인 경우에만 그룹을 사용자에게 할당할 수 있습니다.

  >[!IMPORTANT]
  >
  >100개가 넘는 그룹에 사용자를 추가하면 그룹 목록을 로드하는 Workfront 영역에서 성능 문제가 발생할 수 있습니다.

  공용 그룹에 대한 자세한 내용은 [그룹 만들기](/help/quicksilver/administration-and-setup/manage-groups/create-and-manage-groups/create-a-group.md)를 참조하십시오.

  그룹에 대한 자세한 내용은 [그룹 개요](/help/quicksilver/administration-and-setup/manage-groups/groups-overview/groups.md)를 참조하세요.

### 리소스 계획 수립

* **작업 시간**: 사용자가 오버헤드를 포함하지 않고 실제 작업에 사용할 수 있는 FTE(Full Time Equivalent) 시간의 비율을 나타냅니다. 작업 시간은 최대 1의 10진수여야 하며 0일 수 없습니다. 예를 들어, 실제 작업에 대한 20% 가용성은 0.2입니다.

  필드의 기본값은 1이며, 사용자가 전체 FTE를 실제 프로젝트 관련 작업에 사용함을 나타냅니다.

  시스템은 이 숫자를 사용하여 실제 프로젝트 관련 작업에 대한 사용자의 가용성을 계산합니다.

  Workfront에서 일정을 만드는 방법에 대한 자세한 내용은 [일정 만들기](/help/quicksilver/administration-and-setup/set-up-workfront/configure-timesheets-schedules/create-schedules.md)를 참조하십시오.

  일정 예외 및 휴무는 사용자의 용량에 영향을 줄 수도 있습니다.

  Workfront은 설정 영역의 리소스 관리 기본 설정에 따라 사용자의 가용성을 계산합니다. 자세한 내용은 [리소스 관리 환경 설정 구성](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/configure-resource-mgmt-preferences.md)을 참조하십시오.

  >[!TIP]
  >
  >작업 시간 값을 1로 설정하면 사용자가 프로젝트 관련 작업에 전체 시간에 해당하는 전체 시간을 사용할 수 있음을 나타냅니다.

* **비활성화 날짜 설정**: 이러한 사용자를 특정 날짜와 특정 시간에 비활성화하도록 예약하려면 이 단추를 클릭하십시오.
* **비활성화 날짜**: 사용자가 비활성화되는 날짜와 시간입니다. 비활성화에 대한 사용자 예약에 대한 자세한 내용은 [사용자 비활성화 또는 다시 활성화](/help/quicksilver/administration-and-setup/add-users/create-and-manage-users/deactivate-a-user.md#schedule-users-for-deactivation)에서 [비활성화에 대한 사용자 예약](/help/quicksilver/administration-and-setup/add-users/create-and-manage-users/deactivate-a-user.md)을 참조하십시오.
* **기본 역할**: 사용자가 Workfront에서 수행할 수 있는 기본 작업 역할입니다. 사용자가 할당된 모든 작업 및 문제도 이 작업 역할에 할당됩니다. 작업 역할은 리소스 관리에서 필수적입니다. 관리자 액세스 권한이 있는 Standard 또는 Plan 라이선스가 있거나 Workfront 관리자인 경우에만 이 필드를 업데이트할 수 있습니다. 관리자 액세스 권한을 가진 사용자 설정에 대한 자세한 내용은 [사용자에게 액세스 권한 부여](/help/quicksilver/administration-and-setup/add-users/configure-and-grant-access/grant-access-other-users.md)를 참조하십시오.

  활성 작업 역할만 목록에 표시됩니다.

* (조건부) **기본 역할**&#x200B;을(를) 선택한 경우 **FTE 가용성의 백분율** 필드가 표시됩니다. 사용자의 일정 중 이 작업 역할에 할당되는 시간의 백분율을 지정합니다. 기본 역할에 대한 FTE 가용성 백분율의 기본값은 100%입니다.
* **다른 역할**: 사용자는 Workfront에서 여러 작업 역할을 가질 수 있습니다. 작업 역할은 리소스 관리에서 필수적입니다. 사용자가 이행할 수 있는 작업 역할 수에는 제한이 없습니다. 그러나 너무 많은 수의 작업 역할에 한 명의 사용자를 할당하지 않는 것이 좋습니다. 리소스 관리가 너무 복잡해질 수 있기 때문입니다.

  활성 작업 역할만 목록에 표시됩니다. 작업 역할에 대한 자세한 내용은 [작업 역할 만들기 및 관리](/help/quicksilver/administration-and-setup/set-up-workfront/organizational-setup/create-manage-job-roles.md)를 참조하십시오.

  관리자 액세스 권한이 있는 Standard 또는 Plan 라이선스가 있거나 Workfront 관리자인 경우에만 이 필드를 업데이트할 수 있습니다.

  관리자 액세스 권한을 가진 사용자 설정에 대한 자세한 내용은 [사용자에게 액세스 권한 부여](/help/quicksilver/administration-and-setup/add-users/configure-and-grant-access/grant-access-other-users.md)를 참조하십시오.

* (조건부) 하나 이상의 **다른 역할**&#x200B;을(를) 선택한 경우 각 역할에 대해 **FTE 가용성의 백분율** 필드가 표시됩니다. 사용자의 일정 중 각 작업 역할에 할당되는 시간의 백분율을 지정합니다. 다른 역할에 대한 FTE 가용성 백분율의 기본값은 0%입니다.

  다른 역할에 0% FTE 가용성이 있는 경우 사용자가 이러한 역할의 작업에 할당되지 않는 한 리소스 플래너에 표시되지 않습니다.

  모든 역할에 대한 모든 **FTE 가용성의 백분율**&#x200B;의 합은 100%여야 합니다. FTE 가용성의 각 비율은 리소스 플래너의 사용자당 각 역할에 대한 가용 시간을 계산합니다. 사용자당 각 역할에 대한 사용 가능한 시간은 사용자의 사용 가능한 시간에 따라 다릅니다.

  Workfront 관리자가 리소스 관리 환경 설정에서 FTE를 계산하기 위해 선택한 방법에 따라 사용자의 사용 가능한 시간이 Workfront에서 계산됩니다.

  사용자 가용성의 계산에 대한 자세한 내용은 [리소스 플래너에서 사용자 및 역할에 대한 시간 및 FTE 계산 개요](/help/quicksilver/resource-mgmt/resource-planning/calculate-hours-fte-for-users-roles-resource-planner.md)를 참조하십시오.

  리소스 관리 환경 설정 구성에 대한 자세한 내용은 [리소스 관리 환경 설정 구성](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/configure-resource-mgmt-preferences.md)을 참조하십시오.

* **일정**: 일정을 사용자와 연결합니다. 사용자 일정은 사용자가 할당된 작업의 타임라인을 계산합니다.

  일정을 사용자와 연결하려면 먼저 일정을 만들어야 합니다. 일정 만들기에 대한 자세한 내용은 [일정 만들기](/help/quicksilver/administration-and-setup/set-up-workfront/configure-timesheets-schedules/create-schedules.md)를 참조하세요.

  >[!IMPORTANT]
  >
  >Workfront은 **리소스 가용성 계산** 설정이 **사용자의 일정**(으)로 설정된 경우에만 사용자의 일정을 사용합니다. 이 설정이 리소스 관리에 사용되는 일정에 영향을 주는 방법에 대한 자세한 내용은 [리소스 관리 환경 설정 구성](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/configure-resource-mgmt-preferences.md)을 참조하십시오.

* **타임시트 프로필**: 타임시트가 자동으로 생성되도록 타임시트 프로필을 사용자와 연결합니다.

  이 필드에서 사용할 수 있는 프로필 목록은 액세스 권한에 따라 다릅니다.

   * Workfront 관리자는 모든 시스템 수준 및 모든 그룹 수준의 타임시트 프로필을 볼 수 있습니다.
   * 그룹 관리자는 시스템 수준의 타임시트 프로필과 관리하는 그룹과 관련된 프로필을 볼 수 있습니다.
   * 표준 또는 플랜 라이선스가 있고 사용자 편집 액세스 권한이 있는 사용자는 시스템 수준의 타임시트 프로필만 볼 수 있습니다. 그룹 수준 타임시트 프로필에 대한 자세한 내용은 [타임시트 프로필 만들기, 편집 및 할당](/help/quicksilver/timesheets/create-and-manage-timesheets/create-timesheet-profiles.md)을 참조하세요.

* **기본 시간 유형**: 사용자의 기본 시간 유형을 선택합니다. 사용자가 시간을 기록할 때 기본적으로 사용되는 시간 유형입니다.
* **사용 가능한 시간 유형**: 사용자가 사용할 수 있는 시간 유형을 선택합니다. 이러한 시간 유형은 사용자가 시간을 기록할 수 있는 Workfront의 모든 곳에서 볼 수 있습니다. 사용자는 프로젝트 수준과 사용자 수준에서 활성화된 시간 유형만 볼 수 있습니다. 사용자가 사용할 수 있는 시간 유형에 대한 자세한 내용은 [시간 유형 및 가용성 정의](/help/quicksilver/timesheets/create-and-manage-timesheets/define-hour-types-and-availability.md)를 참조하십시오.
* **FTE**: 사용자에 해당하는 Full Time입니다. Workfront은 시스템 수준의 리소스 관리 기본 설정이 기본 일정으로 설정된 경우에만 이 숫자를 사용하여 기본 일정을 기준으로 사용자의 가용성을 계산합니다.

  FTE는 사용자가 직장에서 보낼 수 있는 시간을 나타냅니다. 여기에는 간접비와 프로젝트 작업에 소비된 시간이 포함됩니다. 예를 들어, 회의나 교육에서 보내는 시간도 FTE에 포함됩니다.

  FTE는 최대 1까지의 십진수여야 하며 0일 수 없습니다. 예를 들어 FTE 값이 0.5이고 Workfront의 기본 일정이 40시간인 경우 사용자는 일주일에 20시간 동안 사용할 수 있습니다.

  필드의 기본값은 1입니다.

  일정 예외, 휴무 및 작업 시간 값은 사용자의 가용성에 영향을 줄 수 있습니다.

  Workfront은 설정 영역의 리소스 관리 기본 설정에 따라 사용자의 가용성을 계산합니다.

  시스템 수준의 리소스 관리 기본 설정이 사용자 일정으로 설정된 경우 여기에서 지정한 값이 무시되며 사용자는 일정에 지정된 내용에 따라 사용할 수 있는 것으로 간주됩니다.

  자세한 내용은 [리소스 관리 환경 설정 구성](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/configure-resource-mgmt-preferences.md)을 참조하십시오.

  Workfront에서 일정을 만드는 방법에 대한 자세한 내용은 [일정 만들기](/help/quicksilver/administration-and-setup/set-up-workfront/configure-timesheets-schedules/create-schedules.md)를 참조하십시오.

* **리소스 풀**: 사용자를 리소스 풀과 연결합니다.

  >[!NOTE]
  >
  >이 필드에는 선택한 모든 사용자에게 공통되는 리소스 풀만 표시됩니다. 선택한 사용자에게 공유 리소스 풀이 없는 경우 이 필드는 비어 있습니다. 이 필드가 비어 있으면 여기에서 지정한 리소스 풀이 해당 개별 리소스 풀을 덮어씁니다.

  리소스 풀에 대한 자세한 내용은 [사용자와 리소스 풀 연결](/help/quicksilver/resource-mgmt/resource-planning/resource-pools/associate-resource-pools-with-users.md)을 참조하십시오.

* **비용 비율**: 사용자의 시간당 비용입니다.

  날짜 유효 비용 요율을 보려면 **요율 추가**&#x200B;를 클릭하십시오. 기간에 대한 원가율 값을 입력하고 필요에 따라 시작 일자와 종료 일자를 지정합니다. 원가율 1에는 시작 일자가 없고 최종 원가율에는 종료 일자가 없습니다.

  일부 날짜는 자동으로 추가됩니다. 예를 들어, 원가 환율 1에 종료 일자가 없고 시작 일자가 2023년 5월 1일인 원가 환율 2를 추가하면, 종료 일자가 2023년 4월 30일로 원가 환율 1에 추가되므로 간격이 없습니다.

* **청구 요금**: 사용자의 시간당 청구 금액입니다.

  날짜 유효 청구 요금을 보려면 **요금 추가**&#x200B;를 클릭하십시오. 기간에 대한 청구 요금의 값을 입력하고 필요에 따라 시작 일자와 종료 일자를 지정합니다. 청구 요금 1에는 시작 일자가 없으며 마지막 청구 요금에 종료 일자가 없습니다.

  일부 날짜는 자동으로 추가됩니다. 예를 들어 청구 요금 1에 종료 일자가 없고 시작 일자가 2023년 5월 1일인 초를 추가하는 경우, 2023년 4월 30일인 종료 일자가 청구 요금 1에 추가되므로 간격이 없습니다.

### 사용자 정의 양식

기존 사용자 정의 양식을 사용자와 연결합니다. 사용자 정의 양식을 사용자와 연결하려면 먼저 사용자 정의 양식을 만들어야 합니다. 활성 사용자 정의 양식만 목록에 표시됩니다. 편집 액세스 권한이 없는 필드는 개별 사용자 정의 양식에 표시되지 않습니다.

>[!NOTE]
>
>외부 조회 필드 및 Workfront 기본 필드와 같은 고급 사용자 정의 양식 기능은 사용자 편집 대화 상자가 아닌 세부 정보 페이지에서 사용자 레코드를 열 때만 사용할 수 있습니다. (사용자 목록에서 사용자 이름을 클릭하여 세부 정보를 엽니다.)

선택적으로 **사용자 정의 표현식 다시 계산** 옵션을 선택하여 선택한 사용자에게 첨부된 사용자 정의 양식의 모든 계산된 사용자 정의 필드가 최신 상태인지 확인할 수 있습니다.

사용자 정의 양식 만들기에 대한 자세한 내용은 [사용자 정의 양식 만들기](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/form-designer/design-a-form/design-a-form.md)를 참조하십시오.

### 댓글

사용자 및 해당 사용자 프로필의 업데이트 영역에 보낼 주석을 입력합니다.

<!--
   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">Preferences</td> 
      <td> 
       <ul> 
        <li><b>Time Zone:</b> The users' time zone.</li> 
        <li><b>Locale</b>: The users' preferred locale. This affects the format of numbers and dates in the emails that come from Workfront.</li> 
        <li><b>Send work I assign to myself to my Working On tab</b>: This setting refers to a deprecated feature that has been removed from Workfront.</li> 
       </ul> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Notifications</td> 
      <td>Select the email notifications which should be enabled for the new user.<p>You can select instant as well as daily digest notifications. All the daily digest notifications are delivered sometime after the same time for all the users selected. For more information, see <a href="../../../administration-and-setup/manage-workfront/emails/configure-event-notifications-for-everyone-in-the-system.md" class="MCXref xref">Configure event notifications for everyone in the system</a>.</p></td> 
     </tr> 
     <tr> 
      <td role="rowheader">Access</td> 
      <td> 
       <ul> 
        <li><b>Is Active:</b> Select this field to indicate whether the users are active. Active users use a Workfront license. Deselecting the field deactivates the users.</li> 
        <li> 
        <p><b>Access Level:</b> Select the access level to assign to these users. All users selected will have the same access level.
        </p> 
        <p>When you assign an access level to users, you can assign a level equal to or less than your own access level. (For example, if your access level is Planner, you cannot assign the Administrator access level.) </p>
        <p>However, you cannot assign an access level that is lower than your own if the Workfront administrator has enabled permissions on the access level that are not also enabled in your own (via the Fine-Tune settings, as described in <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Create or modify custom access levels</a>).</p> 
        <p>For more information about access levels, see <a href="../../../administration-and-setup/add-users/configure-and-grant-access/configure-access.md" class="MCXref xref">Configure access to Adobe Workfront</a>.</p> 
         </li> 
        <li> 
        <p><b>Layout Template</b>: Choose a layout template for the users. The layout template assigned to the users will take precedence over any layout template assigned to their Home Group, Home Team or primary job role. For more information about the assignment priority of layout template, see <a href="../../../administration-and-setup/customize-workfront/use-layout-templates/create-and-manage-layout-templates.md" class="MCXref xref">Create and manage layout templates</a>.</p> 
        <p><b>NOTE</b>:  The list of layout templates you have available in this field depends on your access:
          <ul>
           <li>As a Workfront administrator, you can see all system-level and group-level layout templates.</li>
           <li>As a group administrator, you can see system-level layout templates, as well as those associated with the groups that you manage.</li>
           <li><p>As a user with a Planner license and access to edit users, you can see only system-level layout templates. </p>
           <p>For information about group-level layout templates, see <a href="../../../administration-and-setup/customize-workfront/use-layout-templates/create-and-manage-layout-templates.md" class="MCXref xref">Create and manage layout templates</a>.</p>
           </li>
          </ul></p> 
          </li> 
       </ul> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Organization</td> 
      <td> 
       <ul> 
        <li><b>Company</b>: The company of the users. Users can be associated only with one company. You must create a company before you can associate it with a user. Only active companies display in the list. For information about creating companies, see Understanding and Managing Companies.</li> 
        <li><b>Home Team</b>: Specify the home team for the users. Users can only have one home team. </li> 
        <li><b>Other Teams</b>: Users can belong to multiple teams. </li> 
        <li> <p><b>Home Group:</b> Select an appropriate group to assign the users as their Home Group. This gives the user the ability to access objects that are shared with the group.</p> <p><b>NOTE</b>:  This is a required field. You cannot have users not associated with a Home Group.</p> <p>You can assign a group to users only in the following situations:</p> 
         <ul> 
          <li>You are a Workfront administrator.</li> 
          <li>You are the administrator of that group.</li> 
          <li>The group is public.</li> 
         </ul> </li> 
        <li> <p><b>Other Groups</b>: Users can belong to multiple groups. You can assign a group to a user only  in the following situations:</p> 
         <ul> 
          <li>You are a Workfront administrator.</li> 
          <li>You are the administrator of that group.</li> 
          <li> <p>The group is public. </p> 
          <p>For more information about public groups, see <a href="../../../administration-and-setup/manage-groups/create-and-manage-groups/create-a-group.md" class="MCXref xref">Create a group</a>.</p> 
          <p>For more information about groups, see <a href="../../../administration-and-setup/manage-groups/groups-overview/groups.md" class="MCXref xref">Groups overview</a>.</p> 
          </li> 
         </ul> 
         </li> 
       </ul> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Resource Planning</td> 
      <td> 
       <ul> 
      
      <li>
       <b>Work Time</b>: Represents the percentage of the Full Time Equivalent (FTE) time that the user is available for actual work, not including overhead. Work Time must be a decimal number up to 1, and it cannot be 0. For example, a 20% availability for actual work would be 0.2.

      The field's default is 1, indicating that a user spends their entire FTE on actual, project-related work. 

      The system uses this number to calculate the availability of the user for actual, project-related work. 

      For more information about creating schedules in Workfront, see <a href="../../set-up-workfront/configure-timesheets-schedules/create-schedules.md">Create a schedule</a>.

      Schedule exceptions and time off might also affect the user capacity. 

      Workfront calculates a user's availability depending on the Resource Management preferences in your Setup area. For more information, see <a href="../../set-up-workfront/configure-system-defaults/configure-resource-mgmt-preferences.md">Configure Resource Management preferences</a>. 

      <b>TIP</b>

      Set the Work Time value to  1 to indicate that the user is available for project-related work their entire full-time equivalent.
      </li> 

      <li><b>Schedule Deactivation</b>: Check this box if you want to schedule users to be deactivated after a period of time.</li> 
       <li><b>Scheduled Deactivation Date</b>: The date after which the users become deactivated. For more information about scheduling users for deactivation, see the section <a href="../../../administration-and-setup/add-users/create-and-manage-users/deactivate-a-user.md#scheduling-users-for-deactivation" class="MCXref xref">Schedule users for deactivation</a> in <a href="../../../administration-and-setup/add-users/create-and-manage-users/deactivate-a-user.md" class="MCXref xref">Deactivate or reactivate a user</a>.</li> 
       <li> <p><b>Primary Role</b>: This is the primary job role that a user has in Workfront. Every task and issue that the users are assigned to is also assigned to this job role, by default. Job roles are essential in resource management. For more information about job roles, see <a href="../../../administration-and-setup/set-up-workfront/organizational-setup/create-manage-job-roles.md" class="MCXref xref">Create and manage job roles</a></p> <p>You can update this field only if you have a Plan license with administrative user access, or if you are a Workfront administrator. For more information about setting up users with administrative user access, see <a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-other-users.md" class="MCXref xref">Grant access to users</a>.</p> </li> 
       <li>(Conditional) If you selected a <b>Primary Role</b>, the <b>Percentage of FTE Availability</b> field displays. Specify what percentage of time of the users' schedules is allocated to this job role. The default value for the Percentage of FTE Availability for the Primary Role is 100%.</li> 
       <li> <p><b>Other Roles</b>: Users can have multiple job roles in Workfront. Job roles are essential in resource management. There is no limit for how many job roles a user can fulfill. However, we recommend to not assign one user to an excessively large number of job roles, because resource management might become too complex for these users.</p> <p>For more information about job roles, see <a href="../../../administration-and-setup/set-up-workfront/organizational-setup/create-manage-job-roles.md" class="MCXref xref">Create and manage job roles</a>.</p> <p>You can update this field only if you have a Plan license with administrative user access, or if you are a Workfront administrator. For more information about setting up users with administrative user access, see <a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-other-users.md" class="MCXref xref">Grant access to users</a>.</p> </li> 
       <li> <p>(Conditional) If you selected one or multiple <b>Other Roles</b>, the <b>Percentage of FTE Availability</b> field displays for each role. Specify what percentage of time of the users' schedules is allocated to each job role. The default value for the Percentage of FTE Availability for the Other Roles is 0%.</p> <p><b>NOTE</b>:  
       <ul> 
       <li>If Other Roles have a 0% FTE Availability, they do not display in the Resource Planner, unless the users are assigned to tasks in these roles.</li> 
       <li> <p>The sum of all Percentages of FTE Availability for all roles must equal 100%. Each Percentage of FTE Availability calculates the Available Hours for each role per user in the Resource Planner. The Available Hours for each role per user depends on the available time for the user.</p> <p>The available time for the user is calculated by Workfront depending on the method that has been selected by the Workfront administrator to calculate the FTE in the Resource Management Preferences.</p> <p>For more information about calculating availability for the user, see <a href="../../../resource-mgmt/resource-planning/calculate-hours-fte-for-users-roles-resource-planner.md" class="MCXref xref">Overview of calculating hours and FTE for users and roles in the Resource Planner</a>.</p> <p>For more information about configuring Resource Management preferences, see <a href="../../../administration-and-setup/set-up-workfront/configure-system-defaults/configure-resource-mgmt-preferences.md" class="MCXref xref">Configure Resource Management preferences</a>.</p> </li> 
       </ul> </p> </li> 
       <li> <p><b>Schedule</b>: Associate a schedule with the users. The schedule of the users calculates the timeline of the tasks the users are assigned to.</p> <p>A Workfront administrator or a group administrator must create a schedule before it can be associated with users.</p> <p>Select a system-level or a group schedule to assign it to the selected users.</p> <p>For more information about system-level and group schedules, see <a href="../../../administration-and-setup/set-up-workfront/configure-timesheets-schedules/create-schedules.md" class="MCXref xref">Create a schedule</a>.</p> <p><b>IMPORTANT</b>: Workfront uses the schedule of a user only when the Calculate Resource Availability Using setting is set to The User's Schedule. For information about how the Calculate Resource Availability Using setting affects which schedule is used for Resource Management, see <a href="../../../administration-and-setup/set-up-workfront/configure-system-defaults/configure-resource-mgmt-preferences.md" class="MCXref xref">Configure Resource Management preferences</a>.</p> </li> 
       <li> <p><b>Timesheet Profile</b>: Associate a Timesheet Profile with the users. This ensures that timesheets generate automatically for the users.</p> 
       <p><b>NOTE</b>:  
       <ul> 
       <li>The list of timesheet profiles you have available in this field depends on your access:
       <ul>
       <li>As a Workfront administrator, you can see all system-level and group-level timesheet profiles.</li>
       <li><p>As a group administrator, you can see system-level timesheet profiles, as well as those associated with the groups that you manage.</p></li>
       <li><p>As a user with a Planner license and access to edit users, you can see only system-level timesheet profiles.</p></li>
       </ul></li> 
       <li>If you are a group administrator, all of the users you are editing must be members of a group that you administer.</li> 
       </ul> </p> </li> 
       <li><b>Default Hour Type</b>: Select the default hour type for the users. This is the hour type that is used by default when the users log time.</li> 
       <li> <p><b>Available Hour Types</b>: Select the hour types that should be available to the user. These hour types are visible everywhere in Workfront where the users can log time. A user can only see the hour types that are enabled at the project level as well as the user level.</p> 
       <p>For more information about what hour types are available to users, see <a href="../../../timesheets/create-and-manage-timesheets/define-hour-types-and-availability.md" class="MCXref xref">Define hour types and availability</a>.</p> 
       </li> 
       <li> <b>FTE</b>: This is the Full Time Equivalent of the user. Workfront uses this number to calculate the availability of the user based on the Default Schedule only when the Resource Management Preferences at the system level are set to The Default Schedule. 

      <p>The FTE indicates the amount of time that the user can spend at work. This includes overhead, as well as time spent on project work. For example, time that is spent in meetings, or training is also included in the FTE.</p> 

      The FTE must be a decimal number up to 1, and it cannot be 0. For example, if the FTE value is 0.5 and the Default Schedule in Workfront is 40 hours, the user is available for 20 hours a week. 

      The field's default is 1.

      Schedule exceptions, time off might, and the value of Work Time may affect the availability of the user. 

      Workfront calculates a user's availability depending on the Resource Management preferences in your Setup area.

      If the Resource Management Preferences at the system level are set to The User's Schedule, the value you specify here is ignored and the user is considered to be available according to what is specified in their schedule. 

      For more information, see <a href="../../set-up-workfront/configure-system-defaults/configure-resource-mgmt-preferences.md">Configure Resource Management preferences</a>. 

      For more information about creating schedules in Workfront, see <a href="../../set-up-workfront/configure-timesheets-schedules/create-schedules.md">Create a schedule</a>.
      </li> 
       <li> <p><b>Resource Pools</b>: Associate the users with resource pools.</p> <p><b>NOTE</b>:  Only the resource pools that are common to all the users selected appear in this field. If the users selected have no shared resource pools, this field is empty. If this field is empty, the resource pools you specify here will overwrite their individual resource pools.</p> 
       <p>For more information about resource pools, see <a href="../../../resource-mgmt/resource-planning/resource-pools/work-with-resource-pools.md" class="MCXref xref"> Resource pools overview </a>.</p> </li> 
       <li><b>Cost Per Hour</b>: The amount of cost per hour for the user. </li> 
       <li><b>Billing Per Hour</b>: The amount of billing per hour for the user.</li> 
       <li><b>Custom Forms</b>: Associate an existing user custom form with the users. You must create a custom form before you can associate it with a user. Only active custom forms display in the list. For information about creating custom forms, see <a href="/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/form-designer/design-a-form/design-a-form.md">Create a custom form</a>.</li> 
       <li><b>Comment</b>: Enter a comment in the field provided. All users selected will receive an in-app notification as well as an email notification with your comment. The comment shows in the Updates tab of the users' profile.</li> 
       </ul> </td> 
     </tr> 
    </tbody> 
   </table>
-->

