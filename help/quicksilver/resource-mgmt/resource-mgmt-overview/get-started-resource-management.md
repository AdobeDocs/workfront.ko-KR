---
content-type: overview
product-area: resource-management
navigation-topic: resource-management-overview
title: 리소스 관리 시작
description: 자원 관리를 사용하면 자원 가용성에 따라 자원의 사용을 정확하게 예측하도록 시스템을 구성할 수 있으므로 수행해야 하는 작업이 시간 및 예산에 맞춰 완료됩니다.
author: Alina
feature: Resource Management
exl-id: b10ef503-60ea-4450-b63e-b2918e9bcc11
source-git-commit: 59c3a57e334d1660e3e59da480a90060b1ba81b7
workflow-type: tm+mt
source-wordcount: '1169'
ht-degree: 0%

---

# 리소스 관리 시작

<!-- Audited: 12/2023 -->

<!--
<p>(NOTE: DO NOT DELETE THIS ARTICLE. MANY ARTICLES MENTIONING RES MANAGEMENT ARE AND STILL SHOULD / WILL BE LINKED TO IT.) </p>
<p>(NOTE: Alina: ***As functionality is removed from Legacy and added to Res Planning - this will be continually updated: remove the Legacy Res Planning when that functionality is removed from the system.) </p>
</div>
-->

자원 관리를 사용하면 자원 가용성에 따라 자원의 사용을 정확하게 예측하도록 시스템을 구성할 수 있으므로 수행해야 하는 작업이 시간 및 예산에 맞춰 완료됩니다.

## Adobe Workfront의 리소스 관리 개요

자원 관리는 Adobe Workfront 관리자, 자원 관리자 및 프로젝트 소유자가 조직의 자원을 계획(자원 또는 시나리오 계획)하고 일정(업무 균형자)을 수립하고 가용성을 고려하여 수행해야 하는 작업에 할당하는 모든 활동을 의미합니다. 또한 자원 관리는 보고서 보기(활용률 보고서)에서 계획 및 실제 자원 배부에 대한 정보를 보는 것을 의미합니다.

Workfront에는 리소스를 관리하는 데 사용되는 몇 가지 도구 세트가 있습니다. 각 도구에는 개별 범위가 있습니다. 현재, 사용 중인 리소스 관리 단계에 따라 Workfront에서 다음 리소스 관리 도구를 사용할 수 있습니다.

* 프로젝트에 대한 실제 작업이 시작되기 전에 리소스가 더 높은 수준에서 할당되는 방법을 계획하려면 다음 도구를 사용하십시오.

   * **리소스 플래너**: 리소스 관리의 첫 번째 단계에서 리소스 플래너를 사용하여 예약된 가용성에 따라 리소스에 대한 프로젝트 시간을 예약할 수 있습니다. 리소스 계획 단계에서 리소스 풀의 사용자를 구성하고 프로젝트에 여러 리소스 풀을 할당할 수 있습니다.

     리소스 계획에 대한 자세한 내용은 [Adobe Workfront의 리소스 계획](../../resource-mgmt/resource-planning/resource-planning-overview.md).

   * **시나리오 플래너**: 1년, 3년 또는 5년 계획에 걸쳐 여러 개의 이니셔티브를 관리하고 여러 프로젝트를 포함할 수 있는 상위 수준의 리소스 계획입니다. 가용성과 예산을 최대한 활용하기 위해 최상의 시나리오를 사용할 수 있습니다.

     시나리오 플래너에는 Workfront 라이센스 외에 별도의 라이센스가 필요합니다. Workfront 시나리오 플래너에 대한 자세한 내용은 다음을 참조하십시오. [시나리오 플래너 개요](../../scenario-planner/scenario-planner-overview.md).

     <!--   
     <p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: when more functionality is added, maybe we add that we recommend to start here if this is available for them?!) </p>   
     -->

* 실제 작업(작업 및 문제)에 리소스를 예약하거나 할당하려면 다음 도구를 사용합니다.

   * **업무 균형자**: 완료하는 데 필요한 시간 및 가용성을 기반으로 실제 작업(작업 및 문제)을 완료해야 하는 데 리소스를 할당할 수 있는 리소스 관리의 하위 수준 단계에 속합니다. 업무 균형자 를 사용하여 현재 할당 해제되거나 작업 역할에 할당된 실제 작업에 사용자를 할당할 수 있습니다.

     Workfront 밸런서에 대한 자세한 내용은 [업무 균형자: 문서 색인](../../resource-mgmt/workload-balancer/workload-balancer.md).

<!--

  * **Scheduling** (deprecated <span class="preview">and removed from the Preview environment</span>): Refers to assigning actual work to users by matching the job roles assigned to the tasks and issues with the job roles they can fulfill, or assigning actual work to users on tasks and issues which are currently unassigned. This happens at a lower-level in the process of managing resources, where you can assign your resources to the actual work (tasks and issues) that they must fulfill, according to the hours needed in the project plan to fulfill them.  

     For more information about resource scheduling, see the section [Resource Scheduling](../../resource-mgmt/resource-scheduling/resource-scheduling-overview.md).

    >[!CAUTION]
    >
    >
    >We are no longer supporting the Resource Scheduling tools and they will be removed from Workfront in **January 2023**. We recommend that you use the Workload Balancer for scheduling your resources. 
    >
    >
    >* For information about scheduling resources using the Workload Balancer, see the section [The Workload Balancer](../../resource-mgmt/workload-balancer/workload-balancer.md).
    >
    >
    >* For more information about the timeline for removing the Resource Scheduling tools and replacing them with the Workload Balancer, see [Deprecation of Resource Scheduling tools in Adobe Workfront](../../resource-mgmt/resource-mgmt-overview/deprecate-resource-scheduling.md).

-->
* 여러 프로젝트에서 예산, 계획 및 실제 할당을 분석하려면 다음 도구를 사용합니다.

   * **활용성 보고서**: 이 보고서를 사용하여 프로젝트에 대한 리소스 사용률을 볼 수 있습니다. 프로젝트에 대한 예산, 계획 및 실제 할당과 프로젝트의 비용 및 매출에 미치는 영향을 비교할 수 있습니다.

     활용성 보고서에 대한 자세한 내용은 다음을 참조하십시오. [자원 가동률 정보 보기](../../resource-mgmt/resource-utilization/view-utilization-information.md).

## 리소스 관리 프로세스의 구성 요소

>[!NOTE]
>
>Workfront에서 리소스 관리는 정체된 프로세스가 아닙니다. 프로젝트 일정, 사용자 가용성 또는 역할 변경에 따라 리소스, 할당 및 프로젝트, 작업 및 문제에 대한 할당에 대한 정보를 지속적으로 조정해야 합니다.

Workfront에서 리소스를 관리하는 프로세스에는 다음 단계가 포함됩니다.

* **구성**: 시스템 관리자, 리소스 관리자 또는 프로젝트 소유자는 리소스를 관리하기 전에 Workfront 인스턴스에서 특정 필드 및 개체를 구성해야 합니다. Workfront에서 리소스 관리를 시작하는 데 필요한 사전 요구 사항에 대한 자세한 내용은 [정확한 리소스 관리를 위한 사전 요구 사항](#prerequisites-for-accurate-resource-management) 이 문서의 섹션.\
  작업 항목이 있는 프로젝트가 있을 뿐만 아니라 Workfront에서 다음 항목을 구성해야 합니다.

   * 사용자\
     사용자 만들기에 대한 자세한 내용은 문서 를 참조하십시오 [사용자 추가](../../administration-and-setup/add-users/create-and-manage-users/add-users.md).

   * 작업 역할\
     작업 역할 생성에 대한 자세한 내용은 문서 를 참조하십시오 [작업 역할 만들기 및 관리](../../administration-and-setup/set-up-workfront/organizational-setup/create-manage-job-roles.md).

   * 일정\
     일정 만들기에 대한 자세한 내용은 문서 를 참조하십시오 [일정 만들기](../../administration-and-setup/set-up-workfront/configure-timesheets-schedules/create-schedules.md).

   * 프로젝트 환경 설정

     >[!TIP]
     >
     >시스템 또는 그룹 관리자만 시스템 또는 그룹의 프로젝트 환경 설정을 수정할 수 있습니다.

     프로젝트 환경 설정 정의에 대한 자세한 내용은 문서 를 참조하십시오 [시스템 전체 프로젝트 환경 설정 구성](../../administration-and-setup/set-up-workfront/configure-system-defaults/set-project-preferences.md).

   * 리소스 풀

     리소스 풀 만들기에 대한 자세한 내용은 [리소스 풀 만들기](../../resource-mgmt/resource-planning/resource-pools/create-resource-pools.md).

   * 리소스 관리 환경 설정

     시스템의 경우, 사용자의 일정이나 시스템의 기본 일정을 사용하든 간에 Workfront이 시스템 수준에서 사용자 가용성을 계산하는 방법을 결정해야 합니다.

     자세한 내용은 [리소스 관리 환경 설정 구성](../../administration-and-setup/set-up-workfront/configure-system-defaults/configure-resource-mgmt-preferences.md).

* **리소스 할당**: 리소스 관리자 또는 프로젝트 소유자는 프로젝트에 대한 리소스 할당을 정의하고 작업을 할당할 수 있습니다. 이 단계에서는 리소스 플래너 또는 시나리오 플래너를 사용하여 리소스 할당 예측을 관리하고 업무 균형자에서 사용자에게 실제 작업을 할당할 수 있습니다.

  리소스 계획 및 할당 작업에 대한 자세한 내용은 다음 섹션을 참조하십시오.

   * [Adobe Workfront의 리소스 계획](../../resource-mgmt/resource-planning/resource-planning-overview.md)
   * [Adobe Workfront 시나리오 플래너](../../scenario-planner/scenario-planning.md)
   * [업무 균형자: 문서 색인](../../resource-mgmt/workload-balancer/workload-balancer.md)

<!--
* **Resource scheduling**: After generally planning for resources to use on your projects at a high level, you can start assigning work items (tasks and issues) to users based on their job roles using the Workload Balancer.

  For more information, see [Workload Balancer overview](../workload-balancer/overview-workload-balancer.md). 
-->

* **Analysis**: 리소스 관리자, 프로젝트 소유자 또는 사람 관리자의 경우, 활용성 보고서를 검토하여 리소스의 예산 및 계획 할당이 실제 할당과 어떻게 비교되는지 파악합니다. 시간, 비용 또는 매출로 정보를 검토합니다. 활용률 보고서에 대한 자세한 내용은 다음을 참조하십시오. [자원 가동률 정보 보기](../../resource-mgmt/resource-utilization/view-utilization-information.md).

## Workfront의 리소스 관리 도구를 사용하여 리소스를 보고 관리하는 데 필요한 액세스 권한

다음 사용자는 Workfront의 리소스 관리 도구에 액세스할 수 있습니다.

다음 사용자 중 하나여야 하며 리소스 관리 도구에 액세스하려면 다음 액세스 및 권한이 있어야 합니다.

* 시스템 관리자.
* 플랜 라이선스가 있는 사용자.

  작업 라이선스가 있는 사용자는 프로젝트의 업무 균형자 를 사용하고 할당 및 할당을 관리할 수 있습니다.

  특정 리소스 관리 도구를 사용하려면 Work 또는 Higher 라이센스가 있을 뿐만 아니라 다음을 수행해야 합니다.

   * 리소스 관리에 대한 액세스 편집(업무 균형자에서 할당할 필요가 없음)
   * 재무 데이터에 대한 액세스 권한을 편집하여 리소스 플래너에 비용 정보 표시
   * 재무 데이터에 대한 액세스를 조회하여 활용성 보고서에서 비용 및 수익 정보를 조회합니다(계획 라이센스가 있는 사용자만).

* 리소스를 관리할 프로젝트에 대한 할당 만들기를 포함하는 기여 또는 상위 권한

<!--
* Designated as a Resource Manager for projects to use the Scheduling tool (the Scheduling tool is deprecated).

  >[!TIP]
  >
  >You do not have to be a Resource Manager to use the Resource Planner, Scenario Planner, or the Workload Balancer. 
-->

리소스 예산을 책정하는 데 필요한 액세스에 대한 자세한 내용은 문서 를 참조하십시오 [리소스 예산에 필요한 액세스 권한](../../resource-mgmt/resource-planning/access-needed-to-budget-resources.md).

업무 균형자에서 리소스를 관리하는 데 필요한 액세스에 대한 자세한 내용은 [업무 균형자에서 리소스를 관리하는 데 필요한 액세스](../../resource-mgmt/workload-balancer/access-needed-manage-resources-balancer.md).

## 정확한 리소스 관리를 위한 사전 요구 사항  {#prerequisites-for-accurate-resource-management}

Workfront에서 리소스 관리 도구를 효율적으로 사용하려면 먼저 요구 사항 세트를 충족해야 합니다.

Workfront의 각 리소스 관리 도구에 대한 요구 사항 정보는 다음을 참조하십시오.

* 섹션 [리소스 플래너에서 작업하기 위한 사전 요구 사항](../../resource-mgmt/resource-planning/get-started-resource-planner.md#prerequisites-for-working-in-the-resource-planner) 이 문서에서 [리소스 플래너 개요](../../resource-mgmt/resource-planning/get-started-resource-planner.md).
  <!--remove this at production: * The section "Prerequisites" in the article [Get started with Resource Scheduling](../../resource-mgmt/resource-scheduling/get-started-resource-scheduling.md).-->
* 섹션 [업무 균형자 사용에 대한 우수 사례](../../resource-mgmt/workload-balancer/overview-workload-balancer.md#best-practices-for-using-the-workload-balancer) 이 문서에서 [업무 균형자 개요](../../resource-mgmt/workload-balancer/overview-workload-balancer.md).
* [Adobe Workfront에서 리소스 예산을 책정하는 데 필요한 액세스 권한](../../resource-mgmt/resource-planning/access-needed-to-budget-resources.md).
* [업무 균형자에서 리소스를 관리하는 데 필요한 액세스](../../resource-mgmt/workload-balancer/access-needed-manage-resources-balancer.md).

<!--
<div data-mc-conditions="QuicksilverOrClassic.Draft mode">
<p>(NOTE: drafted and replaced with the links to each prerequisites instead) </p>
<p> We recommend that the following settings exist before starting to manage resources for your organization: </p>
<ul>
<li> You must have users in the system who have active accounts. </li>
<li> You must assign a Plan or a Worker license to the users whose work allocation you want to manage. <note type="note">
Although you can assign work to a Reviewer or a Requestor, they cannot complete it.
<br>We recommend against assigning work to Reviewers or Requestors. For information about access levels in Workfront, see
<a href="../../administration-and-setup/add-users/access-levels-and-object-permissions/access-levels-overview.md" class="MCXref xref" xrefformat="{para}">Access levels overview</a>.
</note></li>
<li> You must have job roles configured in the system.<br>For information about adding job roles to Workfront, see the article <a href="../../administration-and-setup/set-up-workfront/organizational-setup/create-manage-job-roles.md" class="MCXref xref" xrefformat="{para}">Create and manage job roles</a>.</li>
<li> (Optional) If you want to budget cost for your work, your job roles and your users must also have rates associated with them.<br></li>
<li> You must associate at least one job role with your users. </li>
<li> You must specify a valid value for the FTE field of all users when you use the User's Schedule instead of The Default Schedule in your Resource Management system preferences. <br>For information about editing users to ensure they have a job role, FTE, or cost associated with them, see the article <a href="../../administration-and-setup/add-users/create-and-manage-users/edit-a-users-profile.md" class="MCXref xref" xrefformat="{para}">Edit a user's profile</a>. For information about editing the Resource Management preferences in your system, see <a href="../../administration-and-setup/set-up-workfront/configure-system-defaults/configure-resource-mgmt-preferences.md" class="MCXref xref" xrefformat="{para}">Configure Resource Management preferences</a>.</li>
<li>You must associate accurate schedules with your users and they should include schedule exceptions.<br>For information about creating and editing schedules, see the article <a href="../../administration-and-setup/set-up-workfront/configure-timesheets-schedules/create-schedules.md" class="MCXref xref" xrefformat="{para}">Create a schedule</a>.</li>
<li>The Time Off calendar of the users must be up to date. </li>
<li> <p>The following is recommended for the Resource Planner when applying the Project and Role views: </p>
<ul>
<li> <p>You must associate projects with Resource Pools.<br>For information about associating projects with Resource Pools, see <a href="../../resource-mgmt/resource-planning/resource-pools/associate-resource-pools-with-projects-and-templates.md" class="MCXref xref" xrefformat="{para}">Associate resource pools with projects and templates</a>.</p> </li>
</ul> </li>
<li> <p>Your must designate a Resource Manager on your projects and they must have the correct access to budget resources when using the Scheduling tools. </p> <p>For information about the access needed to budget resources, see the article <a href="../../resource-mgmt/resource-planning/access-needed-to-budget-resources.md" class="MCXref xref" xrefformat="{para}">Access needed to budget resources in&nbsp;Adobe Workfront</a>.</p> </li>
<li> <p>You must assign the tasks and issues in your system to job roles, teams, or users.</p> </li>
<li>You must specify a valid value for Planned Hours and Duration for all tasks in your system.<br>For information about Planned Hours, see the article <a href="../../manage-work/tasks/task-information/planned-hours.md" class="MCXref xref" xrefformat="{para}">Planned Hours overview</a>.<br>For information about Duration, see the article <a href="../../manage-work/tasks/taskdurtn/task-duration-and-duration-type.md" class="MCXref xref" xrefformat="{para}">Overview of Task Duration and Duration Type</a>.</li>
</ul>
</div>
-->
