---
content-type: reference
product-area: resource-management
navigation-topic: resource-planning
title: 리소스 플래너에서 사용자 및 역할에 대한 시간 및 FTE 계산 개요
description: 리소스 플래너에서 사용자 및 역할에 대한 시간 및 FTE 계산 개요.
author: Lisa
feature: Resource Management
exl-id: 10b0e507-658e-4d12-994a-e38da6111f5d
source-git-commit: 7f0aac7c8519b1e570e29fedf1492918e8120ad2
workflow-type: tm+mt
source-wordcount: '1323'
ht-degree: 0%

---

# 리소스 플래너에서 사용자 및 역할에 대한 시간 및 FTE 계산 개요

<!-- Audited: 5/2025 -->

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: Alina:KEEP THIS:***Linked to: Configuring My Settings, Editing User Accounts, Planning in the Resource Planner -- *** Some of this documentation is also duplicated in this article (Scheduling): https://support.workfront.com/hc/en-us/articles/360000557174)</p>
-->

시간, FTE 또는 비용별로 리소스 플래너에 리소스의 할당 및 가용성을 표시할 수 있습니다.\
리소스 플래너에서 비용을 계산하는 방법에 대한 자세한 내용은 [리소스 플래너에서 비용 계산](../../resource-mgmt/resource-planning/calculate-costs-resource-planner.md)을 참조하십시오.

FTE(Full Time Equivalent)는 사용자 또는 작업 역할에 대한 일별 또는 주별 실제 작업 시간을 나타내는 시간 측정값입니다.

다음 리소스 정보 세트는 리소스 플래너에서 다르게 계산됩니다.

* 사용 가능한 시간 또는 FTE 값은 시스템 관리자가 시스템에서 리소스 관리 환경 설정을 구성하는 방식을 기반으로 계산됩니다.\
  사용 가능한 시간 및 FTE 값을 계산하는 방법에 대한 자세한 내용은 [리소스 플래너의 사용자 및 작업 역할에 대한 사용 가능한 시간 또는 FTE 계산](#calculate-available-hours-or-fte-for-users-and-job-roles-in-the-resource-planner)을 참조하십시오.\
  Adobe Workfront 시스템의 리소스 관리 환경 설정을 정의하는 방법에 대한 자세한 내용은 [리소스 관리 환경 설정 구성](../../administration-and-setup/set-up-workfront/configure-system-defaults/configure-resource-mgmt-preferences.md)을 참조하십시오.

* 다른 모든 FTE 값은 시스템 기본 일정을 기준으로 계산됩니다.\
  FTE를 사용할 때 리소스 플래너에 다른 모든 값이 표시되는 방법에 대한 자세한 내용은 이 문서의 [리소스 플래너의 사용자 및 작업 역할에 대한 다른 모든 시간 및 FTE 값 계산](#calculate-all-other-hour-and-fte-values-for-users-and-job-roles-in-the-resource-planner) 섹션을 참조하십시오.

각 사용자 및 해당 작업 역할에 대한 FTE가 무엇인지 파악하여 작업에 리소스를 할당할 때 정확하게 관리하는 것이 중요합니다.

## 리소스 플래너에서 사용자 및 작업 역할에 대한 가용 시간 또는 FTE 계산 {#calculate-available-hours-or-fte-for-users-and-job-roles-in-the-resource-planner}

### 리소스 플래너에서 사용자의 사용 가능한 시간 및 FTE 계산 {#calculate-the-available-hours-and-fte-for-a-user-in-the-resource-planner}

Workfront 관리자는 설정의 리소스 관리 영역에서 다음 중 하나를 선택하여 사용자의 사용 가능 시간을 계산하는 방법을 결정합니다.

* 시스템 및 사용자 FTE의 기본 일정입니다.
* 사용자의 일정입니다.

![사용자 일정에 대한 시스템 설정](assets/setup-resource-mgmt.png)

>[!NOTE]
>
>시스템 수준에서 리소스 가용성을 계산하는 방법을 결정합니다. 시스템의 리소스 관리 환경 설정을 정의하는 방법에 대한 자세한 내용은 [리소스 관리 환경 설정 구성](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/configure-resource-mgmt-preferences.md)을 참조하십시오.

이 설정을 구성하는 방법에 따라 리소스 플래너의 사용자 가용성(시간과 FTE 가용성)은 다음 방법을 사용하여 계산됩니다.

* **기본 일정**: 시스템의 기본 일정과 사용자 FTE를 사용하여 리소스 플래너에서 사용자의 사용 가능한 시간과 FTE 값을 결정합니다. 사용자의 일정이 무시됩니다. 이 경우:

   * 리소스 플래너의 사용 가능 시간은 다음 공식을 사용하여 계산됩니다.

     `User Available Hours = Default Schedule Hours * User FTE value`

     예를 들어 기본 일정에 일주일에 40시간을 사용할 수 있고 사용자 FTE가 0.5인 경우 리소스 플래너에서 일주일에 20시간 동안 작업할 수 있습니다.

     기본 일정을 포함하여 일정에 대한 자세한 내용은 [일정 만들기](/help/quicksilver/administration-and-setup/set-up-workfront/configure-timesheets-schedules/create-schedules.md)를 참조하십시오.

   * 리소스 플래너의 사용자에 대해 사용 가능한 FTE는 사용자 설정에 지정된 사용자 FTE와 동일합니다.

     예를 들어 사용자 설정에서 사용자 FTE가 0.5이면 리소스 플래너에서 사용자의 사용 가능한 FTE는 0.5입니다. 사용자 설정에 표시되는 사용자 FTE의 값에 대한 자세한 내용은 [사용자 프로필 편집](/help/quicksilver/administration-and-setup/add-users/create-and-manage-users/edit-a-users-profile.md)을 참조하십시오.

* **사용자 일정**: 사용자 일정은 리소스 플래너에서 사용자의 사용 가능 여부를 확인하는 데 사용됩니다. 사용자 FTE의 값은 무시됩니다. 이 경우:

   * 리소스 플래너의 사용 가능한 시간은 사용자 일정의 시간과 동일합니다.

     예를 들어 사용자의 일정에 일주일에 40시간을 작업할 수 있는 경우 리소스 플래너에서 일주일에 40시간 동안 작업할 수 있습니다.

   * 리소스 플래너의 사용 가능한 FTE는 다음 수식으로 계산됩니다.

     `User Available FTE = Hours from the Schedule of the User/ Default Schedule Hours`

     예를 들어 사용자의 일정에 20시간을 사용할 수 있고 Workfront의 기본 일정에 40시간을 사용할 수 있는 경우 사용자의 FTE는 0.5입니다.

     기본 일정을 포함하여 일정에 대한 자세한 내용은 [일정 만들기](/help/quicksilver/administration-and-setup/set-up-workfront/configure-timesheets-schedules/create-schedules.md)를 참조하십시오.

>[!NOTE]
>
>사용자가 일정과 연결되어 있지 않은 경우 기본 일정을 사용하여 사용자의 사용 가능한 시간이 계산됩니다.

### 리소스 플래너에서 작업 역할에 대한 사용 가능한 시간 및 FTE 계산 {#calculate-the-available-hours-and-fte-for-a-job-role-in-the-resource-planner}

먼저 사용자 가용성을 계산한 다음 각 작업 역할의 가용성을 계산할 수 있습니다.

리소스 플래너에서 작업 역할의 가용성은 사용자의 총 가용성과 사용자의 각 역할과 연관된 FTE 가용성의 백분율을 고려합니다.\
![percent_of_fte_availability_at_the_user_level.png](assets/percent-of-fte-availability-at-the-user-level-350x144.png)

사용자의 작업 역할과 FTE 가용성 비율 값을 연결하는 방법에 대한 자세한 내용은 [사용자 프로필 편집](../../administration-and-setup/add-users/create-and-manage-users/edit-a-users-profile.md)을 참조하십시오.

예를 들어, 사용자의 사용 가능 시간 값이 40이고 해당 시간의 75%에 대한 1차 역할 및 해당 시간의 25%에 대한 1개의 다른 역할을 수행할 수 있는 경우 리소스 플래너는 1주 동안 1차 역할에 대한 사용 가능 시간 값이 30시간이고 다른 역할에 대한 사용 가능 시간 값이 10시간임을 보여 줍니다. 이 경우 기본 역할에 대한 FTE는 0.75이고 다른 역할에 대한 FTE는 0.25입니다.

>[!NOTE]
>
>사용자의 총 사용 가능 시간은 이 문서의 [리소스 플래너 섹션에서 사용자의 사용 가능한 시간 및 FTE 계산](#calculate-the-available-hours-and-fte-for-a-user-in-the-resource-planner)에 설명된 두 가지 방법 중 하나를 사용하여 계산됩니다.

역할 보기에서 리소스 플래너를 볼 때 한 작업 역할의 가용성은 해당 작업 역할을 수행할 수 있는 모든 사용자의 가용성의 합계입니다.

리소스 플래너의 리소스 가용성에 대한 자세한 내용은 [리소스 플래너 개요](../../resource-mgmt/resource-planning/get-started-resource-planner.md)를 참조하십시오.

### 리소스 플래너에서 사용자의 가용 시간 및 FTE 계산(예) {#calculate-the-available-hours-and-fte-for-a-user-in-the-resource-planner-example}

다음 표는 시스템 관리자가 리소스 관리 환경설정에서 FTE 계산을 위해 사용하는 방법에 따라 리소스 플래너에서 사용자에 대해 사용 가능한 시간 및 사용 가능한 FTE가 계산되는 방법을 보여 줍니다.

이 예에서는 다음 숫자를 사용합니다.

* 40시간의 시스템 기본 일정
* 20시간의 사용자 일정
* 사용자 FTE 0.8

| FTE 계산 방법(시스템 설정) | 사용자의 일정에서 **시간** | 기본 일정에서 **시간** | **사용자 FTE 필드** | 리소스 플래너의 **사용 가능한 시간** | **리소스 플래너에서 사용 가능한 FTE** |
|---|---|---|---|---|---|
| **기본 일정** | 무시됨 | 40 | 0.8 | **32**(계산됨) | **0.8** |
| **사용자의 일정** | 20 | 40 | 무시됨 | **20** | **0.5**(계산됨) |

일정 예외 및 휴무는 계획된 시간 또는 FTE의 양에 영향을 줄 수 있습니다. 자세한 내용은 [리소스 관리 환경 설정 구성](../../administration-and-setup/set-up-workfront/configure-system-defaults/configure-resource-mgmt-preferences.md)을 참조하십시오.

사용자 및 시간별 리소스 플래너 보기 예:

![사용자 및 시간별 리소스 플래너 보기](assets/resource-planner-by-user-by-hours.png)

사용자 및 FTE별 리소스 플래너 보기 예:

![사용자 및 FTE별 리소스 플래너 보기](assets/resource-planner-by-user-by-fte.png)

## 리소스 플래너에서 사용자 및 작업 역할에 대한 다른 모든 시간 및 FTE 값 계산 {#calculate-all-other-hour-and-fte-values-for-users-and-job-roles-in-the-resource-planner}

사용 가능한 시간 또는 FTE 외에도 다음 시간 정보가 리소스 플래너에 표시됩니다.

* 계획된 시간
* 예산 시간
* 시간 차이
* 순 시간\
  자세한 내용은 리소스 플래너의 프로젝트 및 역할 보기에서 [시간, FTE 및 비용 정보 개요](../../resource-mgmt/resource-planning/overview-of-planner-hour-fte-cost-information-in-role-project-views.md)를 참조하십시오.

* 시간 차이\
  자세한 내용은 리소스 플래너의 프로젝트 및 역할 보기에서 [시간, FTE 및 비용 정보 개요](../../resource-mgmt/resource-planning/overview-of-planner-hour-fte-cost-information-in-role-project-views.md)를 참조하십시오.

리소스 플래너에 FTE 또는 시간과 동일한 정보를 표시할 수 있습니다.

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
