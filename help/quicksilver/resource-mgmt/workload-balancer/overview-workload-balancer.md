---
content-type: overview
product-area: resource-management
navigation-topic: the-workload-balancer
title: 작업 로드 밸런서 개요
description: 프로젝트 관리자가 프로젝트에 대한 작업을 계획하고 작업을 만든 후 작업 로드 밸런서를 사용하여 이 작업을 팀의 사용자에게 할당할 수 있습니다.
author: Alina
feature: Resource Management
exl-id: 9398bd04-9df7-4b77-8361-fdb5bdce6829
source-git-commit: 11c87d8a97261c24d063fbc824f2e907d07f8217
workflow-type: tm+mt
source-wordcount: '1122'
ht-degree: 0%

---

# 작업 로드 밸런서 개요

<!--
<p>(NOTE: this is linked from the UI for the Workload Balancer page. DO NOT CHANGE TITLE OR LINK) </p>
-->

프로젝트 관리자가 프로젝트에 대한 작업을 계획하고 작업을 생성한 후 작업 로드 밸런서를 사용하여 이 작업을 사용자에게 할당할 수 있습니다.

>[!IMPORTANT]
>
>작업 로드 밸런서를 사용하여 사용자에게 실제 작업(작업 및 문제)을 지정할 수 있습니다.
>
>높은 수준에서 프로젝트에 대한 작업 역할 할당을 추정하려면 작업 로드 밸런서가 아닌 리소스 플래너를 사용해야 합니다. 리소스 계획자에 대한 자세한 내용은 [리소스 플래너 개요](../../resource-mgmt/resource-planning/get-started-resource-planner.md).

이 문서에서는 작업 로드 밸런서의 일반적인 목적과 프로젝트 및 리소스를 성공적으로 사용할 수 있도록 설정하는 방법에 대한 몇 가지 모범 사례에 대해 설명합니다.

## 작업 로드 밸런서를 찾습니다.

<!--
<p>(NOTE: This will be taken out when all we will have is one tool - should be replaced by a blurb that says you can add this tool anywhere, in any custom tab, etc (long term dev promise)) </p>
-->

자원 스케줄링에 대해 다음 영역에서 작업 로드 밸런서를 사용하는 것이 좋습니다.

* 시스템 수준에서 리소스 영역에서
* 프로젝트 수준에서 프로젝트의 작업 로드 밸런서 섹션에서
* 팀 레벨의 팀 작업 로드 밸런서 섹션에서

작업 로드 밸런서를 찾는 방법에 대한 자세한 내용은 [작업 로드 밸런서를 찾습니다.](../../resource-mgmt/workload-balancer/locate-workload-balancer.md).

## 작업 로드 밸런서의 이점

작업 로드 밸런서를 사용할 때 다음과 같은 이점을 고려하십시오.

<!--
<p> Add about the what-if scenarios as a benefit when they become available </p>
-->

* 모든 이해 당사자에게 투명한 리소스 오버할당 및 저활용도의 명확한 시각적 매핑에 액세스합니다.
* 사람 관리자로서, 여러분은 여러분의 사람들을 지치지 않도록 보호하고 그들이 더 나은 초점, 품질 및 참여로 최고의 일을 할 수 있도록 할 수 있습니다. 전체 활용률을 보장하고 사일로를 분리하며 팀 간의 작업 정렬을 수행할 수 있습니다.
* 작업 또는 문제 수준에서 작업을 할당하면 사용자의 사용 가능 여부를 알 수 없습니다. 작업 로드 밸런서를 사용할 때 작업 로드에서 사용 가능한 사용자를 확인하여 작업 또는 문제를 제시간에 완료할 수 있습니다. 여기에는 시간 초과 및 예약 예외 세부 사항이 포함됩니다.

   자세한 내용은 [작업 로드 밸런서에서 작업 할당 개요](../../resource-mgmt/workload-balancer/assign-work-in-workload-balancer.md).

   또한 여러 프로젝트에서 여러 작업 항목을 한 번에 쉽게 배포할 수 있도록 작업 항목을 일괄적으로 할당할 수도 있습니다. 자세한 내용은 [작업 로드 밸런서를 사용하여 일괄 작업 할당](../../resource-mgmt/workload-balancer/assign-work-in-workload-balancer-in-bulk.md).

* 경영진은 조직 내의 사람들이 어떻게 활용되는지에 대한 투명성을 통해 적시에 직원을 채용할 수 있다.
* 팀원은 동료들의 작업 내용을 언제든지 볼 수 있으므로 더 나은 협업을 통해 이익을 얻는다. 작업 로드 밸런서에서 리소스를 보거나 관리하는 데 필요한 액세스에 대한 자세한 내용은 [작업 로드 밸런서에서 리소스를 관리하는 데 필요한 액세스](../../resource-mgmt/workload-balancer/access-needed-manage-resources-balancer.md).
* 사용자 지정 탭에 링크를 포함하여 리소스 영역에 대한 액세스 권한이 없는 사용자와 공유합니다. 자세한 내용은 [링크와 작업 로드 밸런서 공유](../../resource-mgmt/workload-balancer/share-link-for-workload-balancer.md)
* 역할에 따라 글로벌, 프로젝트 또는 팀 레벨에서 하나의 보기에서 사용자의 워크로드 및 수요를 시각화하고 관리합니다. 프로젝트를 관리할 때 프로젝트에 대한 리소스 할당은 물론 Adobe Workfront 시나리오 플래너에서 리소스 할당을 시각화하기도 포함됩니다. 인력 관리자는 Workfront 시나리오 플래너를 사용하여 조직 전체에서 Job 기술을 관리합니다. 시나리오 플래너는 새 Adobe Workfront 경험에서만 사용할 수 있습니다.

   >[!NOTE]
   >
   >  시나리오 플래너는 추가 라이센스가 필요합니다. Workfront 시나리오 플래너에 대한 자세한 내용은 [시나리오 계획자 개요](../../scenario-planner/scenario-planner-overview.md).


## 작업 로드 밸런서 사용 우수 사례

작업 로드 밸런서를 사용하여 리소스를 예약하기 전에 프로젝트 계획, 사용자 구성 및 필터 사용에 대한 다음의 모범 사례를 권장합니다.

* [작업 로드 밸런서에 정보를 표시하는 우수 사례](#best-practices-for-displaying-information-in-the-workload-balancer)
* [사용자 설정 우수 사례](#best-practices-for-setting-up-users)
* [작업 및 문제 설정에 대한 우수 사례](#best-practices-for-setting-up-tasks-and-issues)

### 작업 로드 밸런서에 정보를 표시하는 우수 사례 {#best-practices-for-displaying-information-in-the-workload-balancer}

할당되지 않은 작업 항목과 할당된 작업 항목 모두에 대해 관련된 정보만 표시할 수 있도록 필터를 사용하는 것이 좋습니다.

작업 로드 밸런서에서 필터 생성 및 사용에 대한 자세한 내용은 [작업 로드 밸런서에서 정보 필터링](../../resource-mgmt/workload-balancer/filter-information-workload-balancer.md).

### 사용자 설정 우수 사례

* 일정을 예약하는 사용자가 다른 사용자에 대해 작동하므로 작업을 위한 리소스를 예약하려면 올바른 액세스 및 권한이 있어야 합니다.

   작업 로드 밸런서에서 리소스의 작업 로드를 관리하는 데 필요한 액세스에 대한 자세한 내용은 [작업 로드 밸런서에서 리소스를 관리하는 데 필요한 액세스](../../resource-mgmt/workload-balancer/access-needed-manage-resources-balancer.md).

* 관리할 작업 로드가 있는 사용자는 가용성 및 기술에 대한 정보가 정확하도록 다음 기준을 충족해야 합니다.

   * 해당 프로필과 연관된 일정 및 작업 역할이 있습니다.
   * 일정 및 작업 역할을 사용자와 연관시키는 방법에 대한 자세한 내용은 [사용자 추가](../../administration-and-setup/add-users/create-and-manage-users/add-users.md)
   * 사용자가 예약과 연결되지 않은 경우 리소스 관리를 위해 Workfront 시스템의 기본 예약 이 사용자와 기본적으로 연결됩니다.
   * 예약 예외가 해당 스케줄에 갱신되었습니다.\
      예약 작성에 대한 자세한 내용은 [예약 만들기](../../administration-and-setup/set-up-workfront/configure-timesheets-schedules/create-schedules.md)

   * 해당 프로필에서 휴가 일정 을 업데이트하세요.\
      사용자의 시간 초과 달력 업데이트에 대한 자세한 내용은 [Adobe Workfront에서 개인 시간 설정](../../workfront-basics/manage-your-account-and-profile/configuring-your-user-profile/personal-time-overview.md).

      <!--   
     <div data-mc-conditions="QuicksilverOrClassic.Draft mode">   
     <p>(NOTE: Add another bullet for Costs, when this becomes available:</p>   
     <p>If you want to budget your resources by Cost, you must associate Job Roles with Cost/ Hr. rates. The cost associated with Job Roles assigned to users in your Resource Pools is used to calculate the Budgeted Labor Cost and the Budgeted Cost of the project.For more information about associating job roles with rates, see the article Creating and Managing Job Roles in the new Adobe Workfront experience.For more information about calculating Budgeted Labor Cost, see the article Calculating Budgeted Labor Cost in the new Adobe Workfront experience.For more information about calculating Budgeted Cost, see the article Calculating Budgeted Cost in .) </p>   
     </div>   
     -->

* Workfront 관리자는 Workfront이 사용자 가용성을 계산하는 방법을 결정해야 합니다. Workfront에서 시스템 기본 예약 또는 사용자의 일정을 사용하여 사용자가 작업할 수 있는 시간을 계산할지 여부를 결정할 수 있습니다. 자세한 내용은 [리소스 관리 환경 설정 구성](../../administration-and-setup/set-up-workfront/configure-system-defaults/configure-resource-mgmt-preferences.md).

### 작업 및 문제 설정에 대한 우수 사례 {#best-practices-for-setting-up-tasks-and-issues}

작업 로드 밸런서에서 사용자에게 작업 할당을 시작하기 전에 다음 작업 및 문제 설정이 있는지 확인합니다.

* 상위 작업은 사용자 또는 역할에 할당되지 않습니다. 작업 로드 밸런서에 표시되지 않습니다.
* 태스크 및 문제에는 0보다 큰 계획 시간 값이 있습니다.

* 작업 및 문제는 지속 시간 값이 0보다 큰 값을 갖습니다.
* 문제의 계획 날짜는 프로젝트의 타임라인 내에 있습니다.

## 작업 로드 밸런서를 사용하기 전에

* 작업 로드 밸런서를 사용하여 작업을 할당하고 조직의 사용자에 대한 일별 할당을 관리할 수 있습니다.

   이 문서에서는 작업 로드 밸런서를 탐색하여 다음 작업을 수행하는 방법을 안내합니다. [작업 로드 밸런서 탐색](../workload-balancer/navigate-the-workload-balancer.md).

   다음 문서에서는 작업을 할당하고 사용자 할당을 관리하는 방법을 설명합니다.

   * [작업 로드 밸런서에서 작업 할당 개요](../workload-balancer/assign-work-in-workload-balancer.md).
   * [작업 로드 밸런서에서 사용자 할당 관리](../workload-balancer/manage-user-allocations-workload-balancer.md).

* 작업 로드 밸런서는 Workfront의 여러 영역에 있을 수 있습니다. 작업 로드 밸런서를 찾을 수 있는 위치에 대한 자세한 내용은 [작업 로드 밸런서를 찾습니다.](../../resource-mgmt/workload-balancer/locate-workload-balancer.md).

## 작업 로드 밸런서를 사용하는 데 필요한 액세스

Workfront에서 작업 로드 밸런서를 보고 사용하려면 특정 프로젝트에 대한 올바른 Workfront 액세스 및 권한이 있어야 합니다. 작업 로드 밸런서를 사용하는 데 필요한 액세스에 대한 자세한 내용은 문서를 참조하십시오 [작업 로드 밸런서에서 리소스를 관리하는 데 필요한 액세스](../../resource-mgmt/workload-balancer/access-needed-manage-resources-balancer.md).
