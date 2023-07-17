---
content-type: reference
product-area: resource-management
navigation-topic: resource-planning
title: 리소스 플래너에서 사용자 및 역할에 대한 시간 및 FTE 계산 개요
description: 리소스 플래너에서 사용자 및 역할에 대한 시간 및 FTE 계산 개요
author: Alina
feature: Resource Management
exl-id: 10b0e507-658e-4d12-994a-e38da6111f5d
source-git-commit: 4331917d133c52cf727f148b75a213853c1e5679
workflow-type: tm+mt
source-wordcount: '977'
ht-degree: 1%

---

# 리소스 플래너에서 사용자 및 역할에 대한 시간 및 FTE 계산 개요

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: Alina:KEEP THIS:***Linked to: Configuring My Settings, Editing User Accounts, Planning in the Resource Planner -- *** Some of this documentation is also duplicated in this article (Scheduling): https://support.workfront.com/hc/en-us/articles/360000557174)</p>
-->

시간, FTE 또는 비용별로 리소스 플래너에 리소스의 할당 및 가용성을 표시할 수 있습니다.\
리소스 플래너에서 비용 계산에 대한 자세한 내용은 다음을 참조하십시오. [리소스 플래너에서 비용 계산](../../resource-mgmt/resource-planning/calculate-costs-resource-planner.md).

&quot;FTE&quot;는 Full Time Equivalent를 의미합니다. 사용자 또는 직무 역할에 대해 하루 또는 일주일 동안 실제 업무에 할애된 시간을 나타내는 시간 측정치입니다.

다음 리소스 정보 세트는 리소스 플래너에서 다르게 계산됩니다.

* 사용 가능한 시간 또는 FTE 값은 시스템 관리자가 시스템에서 리소스 관리 환경 설정을 구성하는 방식을 기반으로 계산됩니다.\
  사용 가능한 시간 및 FTE 값을 계산하는 방법에 대한 자세한 내용은 [리소스 플래너에서 사용자 및 작업 역할에 대한 가용 시간 또는 FTE 계산](#calculate-available-hours-or-fte-for-users-and-job-roles-in-the-resource-planner).\
  Adobe Workfront 시스템의 리소스 관리 환경 설정 정의에 대한 자세한 내용은 [리소스 관리 환경 설정 구성](../../administration-and-setup/set-up-workfront/configure-system-defaults/configure-resource-mgmt-preferences.md).

* 다른 모든 FTE 값은 시스템 기본 일정을 기준으로 계산됩니다.\
  FTE를 사용할 때 리소스 플래너에 다른 모든 값이 표시되는 방법에 대한 자세한 내용은 섹션 을 참조하십시오 [리소스 플래너에서 사용자 및 작업 역할에 대한 다른 모든 시간 및 FTE 값 계산](#calculate-all-other-hour-and-fte-values-for-users-and-job-roles-in-the-resource-planner) 이 문서에서.

각 사용자 및 해당 작업 역할에 대한 FTE가 무엇인지 파악하여 작업에 리소스를 할당할 때 정확하게 관리하는 것이 중요합니다.

## 리소스 플래너에서 사용자 및 작업 역할에 대한 가용 시간 또는 FTE 계산 {#calculate-available-hours-or-fte-for-users-and-job-roles-in-the-resource-planner}

* [리소스 플래너에서 사용자의 사용 가능한 시간 및 FTE 계산](#calculate-the-available-hours-and-fte-for-a-user-in-the-resource-planner)
* [리소스 플래너에서 작업 역할에 대한 사용 가능한 시간 및 FTE 계산](#calculate-the-available-hours-and-fte-for-a-job-role-in-the-resource-planner)
* [리소스 플래너에서 사용자의 가용 시간 및 FTE 계산(예)](#calculate-the-available-hours-and-fte-for-a-user-in-the-resource-planner-example)

### 리소스 플래너에서 사용자의 사용 가능한 시간 및 FTE 계산 {#calculate-the-available-hours-and-fte-for-a-user-in-the-resource-planner}

Workfront 관리자는 설정의 리소스 관리 영역에서 다음 중 하나를 사용하도록 선택하여 사용자의 사용 가능 시간을 계산하는 방법을 결정합니다.

* 시스템 및 사용자 FTE의 기본 일정입니다.
* 사용자의 일정입니다.

자세한 내용은 [리소스 관리 환경 설정 구성](../../administration-and-setup/set-up-workfront/configure-system-defaults/configure-resource-mgmt-preferences.md).

<!--
<div data-mc-conditions="QuicksilverOrClassic.Draft mode">
<p><br></p>
<p> <img src="assets/nwe-resource-management-system-setting-user's-schedule-350x157.png" style="width: 350;height: 157;" data-mc-conditions="QuicksilverOrClassic.Quicksilver"> </p>
<p>(NOTE: The determines how to calculate resource availability at the system level.For more information about defining the Resource Management preferences for the system, see Configure Resource Management preferences.)</p>
<p>Based on how this setting is configured, the availability of the users in the Resource Planner (hours as well as FTE availability) is calculated by using the following methods: </p>
<ul>
<li><strong>The Default Schedule</strong>: The Default Schedule of the system and the user FTE are used to determine the Available Hours and FTE value for the user in the Resource Planner. The Schedule of the user is ignored. In this case:
<ul>
<li> The <strong>Available Hours</strong> in the<strong>Resource Planner</strong> are calculated using the following formula:<br><code>User Available Hours = Default Schedule Hours * User FTE value</code> <span style="color: #dc143c;">( NOTE: this is the correct value. If this shows as a division in other articles, that is wrong. It's a multiplication between these 2 values).</span><br>For example, if the Default Schedule has 40 hours a week available for work, and the user FTE is 0.5, the user is available to work for 20 hours a week in the Resource Planner.<br>For more information about schedules, including the Default Schedule, see <a href="../../administration-and-setup/set-up-workfront/configure-timesheets-schedules/create-schedules.md" class="MCXref xref">Create a schedule</a></li>
<li style="font-weight: normal;"> The <strong>Available FTE</strong> for the user in the<strong>Resource Planner</strong> is the same as the user FTE specified in the user settings. <br>For example, if the user FTE is 0.5 in the user settings, the available FTE of the user is 0.5 in the Resource Planner. For more information about the value of the user FTE as it displays in the user settings, see <a href="../../administration-and-setup/add-users/create-and-manage-users/edit-a-users-profile.md" class="MCXref xref">Edit a user's profile</a>.<br></li>
</ul></li>
<li><strong>The User's Schedule</strong>: The Schedule of the user is used to determine the availability of the user in the Resource Planner. The value of the user FTE is ignored. In this case:
<ul>
<li> The <strong>Available Hours</strong> in the<strong>Resource Planner</strong> are the same as the Hours from the Schedule of the user.<br>For example, if the Schedule of the user has 40 hours a week available for work, the user is available to work for 40 hours a week in the Resource Planner. </li>
<li> The <strong>Available FTE</strong> in the<strong>Resource Planner</strong> is calculated by the following formula:<br><em><code>User Available FTE = Hours from the Schedule of the User/ Default Schedule Hours</code><br></em>For example, if the Schedule of the user has 20 hours available to work, and the Default Schedule in Workfront has 40 hours available to work, the user's FTE is 0.5.<br>For more information about schedules, including the Default Schedule, see <a href="../../administration-and-setup/set-up-workfront/configure-timesheets-schedules/create-schedules.md" class="MCXref xref">Create a schedule</a>.</li>
</ul></li>
</ul> <note type="note">
If the user is not associated with a schedule, the Available Hours for the user are calculated using the Default Schedule.
</note>
</div>
-->

### 리소스 플래너에서 작업 역할에 대한 사용 가능한 시간 및 FTE 계산 {#calculate-the-available-hours-and-fte-for-a-job-role-in-the-resource-planner}

먼저 사용자 가용성을 계산한 다음 각 작업 역할의 가용성을 계산할 수 있습니다.

리소스 플래너에서 작업 역할의 가용성은 사용자의 총 가용성과 **FTE 가용성 백분율** 를 사용자의 각 역할과 연결합니다.\
![percent_of_fte_availability_at_the_user_level.png](assets/percent-of-fte-availability-at-the-user-level-350x144.png)

연결에 대한 자세한 내용 **FTE 가용성 백분율** 사용자의 작업 역할이 있는 값입니다. [사용자 프로필 편집](../../administration-and-setup/add-users/create-and-manage-users/edit-a-users-profile.md).

예를 들어, 사용자의 사용 가능 시간 값이 40이고 1차 역할이 해당 시간의 75%에 대해 1차 역할을 수행하고 1차 역할이 해당 시간의 25%에 대해 다른 역할을 수행할 수 있는 경우 리소스 플래너는 다음을 표시합니다. **사용 가능한 시간** 1주 동안 기본 역할의 값은 30시간이며 **사용 가능한 시간** 다른 역할의 값은 10시간입니다. 이 경우 기본 역할에 대한 FTE는 0.75이고 다른 역할에 대한 FTE는 0.25입니다.

>[!NOTE]
>
>사용자의 총 사용 가능 시간은 다음에 설명된 두 가지 방법 중 하나에 의해 계산됩니다. [리소스 플래너에서 사용자의 사용 가능한 시간 및 FTE 계산](#calculate-the-available-hours-and-fte-for-a-user-in-the-resource-planner) 이 문서의 섹션.

역할 보기에서 리소스 플래너를 볼 때 한 작업 역할의 가용성은 해당 작업 역할을 수행할 수 있는 모든 사용자의 가용성의 합계입니다.\
리소스 플래너의 리소스 가용성에 대한 자세한 내용은 [리소스 플래너 개요](../../resource-mgmt/resource-planning/get-started-resource-planner.md).

### 리소스 플래너에서 사용자의 가용 시간 및 FTE 계산(예) {#calculate-the-available-hours-and-fte-for-a-user-in-the-resource-planner-example}

다음 표는 시스템 관리자가 리소스 관리 환경설정에서 FTE 계산을 위해 사용하는 방법에 따라 리소스 플래너에서 사용자에 대해 사용 가능한 시간 및 사용 가능한 FTE가 계산되는 방법을 보여 줍니다.

이 예에서는 다음 숫자를 사용합니다.

* 40시간의 시스템 기본 일정
* 20시간의 사용자 일정
* 사용자 FTE 0.75

| FTE 계산 방법(시스템 설정) | **사용자 일정 후 경과 시간** | **기본 일정의 시간** | **사용자 FTE 필드** | **리소스 플래너의 사용 가능한 시간** | **리소스 플래너에서 사용 가능한 FTE** |
|---|---|---|---|---|---|
| **기본 일정** | 무시됨 | 40 | 0.75 | **30** (계산됨) | **0.75** |
| **사용자의 일정** | 20 | 40 | 무시됨 | **20** | **0.5** (계산됨) |

일정 예외 및 휴무는 계획된 시간 또는 FTE의 양에 영향을 줄 수 있습니다. 자세한 내용은 [리소스 관리 환경 설정 구성](../../administration-and-setup/set-up-workfront/configure-system-defaults/configure-resource-mgmt-preferences.md).

## 리소스 플래너에서 사용자 및 작업 역할에 대한 다른 모든 시간 및 FTE 값 계산 {#calculate-all-other-hour-and-fte-values-for-users-and-job-roles-in-the-resource-planner}

사용 가능한 시간 또는 FTE 외에도 다음 시간 정보가 리소스 플래너에 표시됩니다.

* 계획된 시간
* 예산 시간
* 시간 차이
* 순 시간\
  이러한 값에 대한 자세한 내용은 [리소스 플래너의 프로젝트 및 역할 보기에서 시간, FTE 및 비용 정보 개요](../../resource-mgmt/resource-planning/overview-of-planner-hour-fte-cost-information-in-role-project-views.md)

* 시간 차이\
  이 값이 나타내는 내용에 대한 자세한 내용은 [리소스 플래너의 프로젝트 및 역할 보기에서 시간, FTE 및 비용 정보 개요](../../resource-mgmt/resource-planning/overview-of-planner-hour-fte-cost-information-in-role-project-views.md).

리소스 플래너에 FTE 또는 시간으로 동일한 정보를 표시할 수 있습니다.

Workfront은 다음 공식을 사용하여 리소스 플래너에 다른 모든 값을 FTE로 표시합니다.

`FTE = Resource Planner Hours/ Default Schedule Hours`

>[!NOTE]
>
>리소스 플래너에서 사용 가능한(AVL) FTE 값을 제외한 모든 값에 대한 FTE를 계산할 때 사용자의 일정이 무시됩니다. 기본 스케줄만 계산에 고려됩니다.

이 계산은 다음 값에 적용됩니다.

* 계획된 FTE(PLN)
* 예산 FTE(BDG)
* FTE 분산(VAR)
* 순 FTE
* FTE 차이(DIF)
