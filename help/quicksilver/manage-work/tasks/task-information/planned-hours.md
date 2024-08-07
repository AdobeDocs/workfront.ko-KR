---
content-type: overview
product-area: projects
navigation-topic: task-information
title: 계획된 시간 개요
description: 작업, 문제 또는 프로젝트와 관련된 계획된 시간은 할당된 사용자가 작업, 문제 또는 프로젝트를 완료하는 데 필요한 시간을 나타냅니다.
author: Alina
feature: Work Management
exl-id: 0b86c760-691a-436e-9beb-31e9ac36440a
source-git-commit: 48efc796923079622ce4bc1c2bddb2429915c9a1
workflow-type: tm+mt
source-wordcount: '2815'
ht-degree: 0%

---

# 계획된 시간 개요

<!-- Audited: 01/2024 -->

작업, 문제 또는 프로젝트와 관련된 계획된 시간은 할당된 사용자가 작업, 문제 또는 프로젝트를 완료하는 데 필요한 시간을 나타냅니다.

## Adobe Workfront의 계획된 시간에 대한 고려 사항

* 계획된 시간은 주로 Adobe Workfront의 작업 항목(작업 및 문제)과 관련되어 있습니다. 작업 항목의 계획된 시간은 프로젝트의 계획된 시간으로 적상됩니다.
* 기본적으로 Workfront은 작업 및 문제 계획 시간을 작업 또는 문제 기간 의 모든 일에 균등하게 분배합니다.
* 작업 및 문제에 사용자 및 역할이 할당되면 작업 및 문제의 계획된 시간이 사용자 또는 역할 할당과 연결됩니다.
* Workfront에서 리소스 관리 도구를 사용하려면 작업 및 문제에 대한 계획된 시간 값을 정의해야 합니다.
* 일부 기간 유형에 대해서만 작업의 계획된 시간 값을 수정할 수 있습니다.

  작업의 기간 유형과 관련하여 작업의 계획된 시간을 수정하는 방법에 대한 자세한 내용은 이 문서의 [기간 유형에 따른 작업 계획된 시간 업데이트](#update-task-planned-hours-based-on-duration-type) 섹션을 참조하십시오.

* 언제든지 문제에 대한 계획된 시간 값을 수정할 수 있습니다.
* 프로젝트 또는 상위 작업의 계획된 시간 값은 모든 작업 및 하위 작업의 모든 계획된 시간의 계산된 합계이므로 수정할 수 없습니다.
* 리소스 관리 도구를 사용하여 사용자 할당을 관리하면 작업, 문제 및 프로젝트의 계획된 시간과 작업 항목과 연결된 할당의 시간이 변경될 수 있습니다.

## 작업의 계획된 시간과 프로젝트의 계획된 시간 비교 {#planned-hours-on-tasks-vs-planned-hours-on-projects}

작업의 계획된 시간은 프로젝트의 계획된 시간으로 롤업됩니다. 문제의 계획된 시간이 항상 프로젝트의 계획된 시간으로 롤업되는 것은 아닙니다.

이 섹션에서는 작업과 프로젝트 계획 시간의 차이점에 대해 설명합니다. 프로젝트에 롤업되는 문제 계획된 시간을 볼 수 있는 위치도 설명합니다.

### 작업에 대한 계획된 시간 {#planned-hours-on-tasks}

작업의 계획된 시간은 작업에 대한 실제 작업에 걸릴 것으로 예상되는 시간을 나타냅니다. 기본적으로 Workfront은 각 작업의 기간 내에 각 날에 대한 총 계획된 시간을 균등하게 분배합니다. 일별 계획된 시간이 작업에 대한 일별 할당이 됩니다. 작업이 여러 리소스에 할당되면 기본적으로 각 리소스에는 동일한 양의 일별 시간이 할당됩니다.

업무 균형자 를 사용하여 작업에 할당된 사용자의 일별 할당을 수정할 수 있습니다. 작업 기간 유형이 간단한 경우 작업의 계획된 시간을 업데이트할 수도 있습니다. 자세한 내용은 [업무 균형자에서 사용자 할당 관리](../../../resource-mgmt/workload-balancer/manage-user-allocations-workload-balancer.md) 문서의 &quot;사용자 할당 관리 시 작업 계획 시간 업데이트&quot; 섹션을 참조하십시오.

작업에 하위 작업이 포함된 경우 상위 작업의 계획된 시간은 하위 작업에 대한 모든 계획된 시간의 합계입니다. 상위 작업의 계획된 시간을 업데이트할 수 없습니다.

>[!NOTE]
>
>계획된 시간과 달리 상위 작업의 실제 시간은 상위 작업에 직접 기록된 시간입니다. 하위 작업의 실제 근로시간 합계를 나타내지 않습니다.\
>실제 사용 시간에 대한 자세한 내용은 [실제 사용 시간 보기](../../../manage-work/tasks/task-information/actual-hours.md)를 참조하십시오.

### 프로젝트의 계획된 시간 {#planned-hours-on-projects}

프로젝트의 계획된 시간 크기를 편집할 수 없습니다. 프로젝트의 계획된 시간은 프로젝트의 모든 작업에서 모든 계획된 시간의 계산된 합계입니다.

계획된 시간 계산에 문제가 포함되는지 여부는 계획된 시간을 보고 있는 프로젝트 내의 위치에 따라 다릅니다. 프로젝트 계획 시간은 프로젝트 내의 다음 위치에서 볼 수 있습니다.

* **프로젝트 세부 정보 섹션 및 프로젝트 편집 상자**: 프로젝트의 작업에 대한 계획된 시간만 고려됩니다. 프로젝트 세부 정보 섹션 또는 프로젝트 편집 상자에서 프로젝트에 대한 총 계획된 시간을 볼 때 프로젝트의 문제에 대한 계획된 시간은 고려되지 않습니다.

* **업무 균형자**: 업무 균형자에 표시되는 작업과 관련된 계획된 시간만 프로젝트의 업무 균형자에 표시됩니다. 사용자 일별 할당은 업무 균형자에서 프로젝트 일별 계획된 시간을 변경할 수 있습니다.
* **사용률 섹션**: 사용률 섹션에서 프로젝트에 대한 총 계획된 시간을 볼 때 작업에 할당된 사용자와 관련된 계획된 시간 및 프로젝트의 문제를 고려합니다.
* 작업 목록의 **역할 할당 패널**: 작업 역할 또는 작업 역할과 연결된 사용자에게 할당된 프로젝트의 작업 및 문제에 대한 계획된 시간이 이 영역에 표시됩니다. 팀에 할당되지 않거나 할당된 작업 및 문제와 관련된 계획된 시간은 이 영역에 표시되지 않습니다. 자세한 내용은 [역할 할당 패널에서 프로젝트 계획 시간 보기](../../../manage-work/projects/planning-a-project/view-planed-hours-in-role-allocation-panel.md)를 참조하십시오.

## 작업 기간 전체에 대한 계획된 시간 분포

기본적으로 Workfront은 작업 기간 동안 계획된 시간을 균등하게 분배하며 프로젝트 일정의 가용성에 따라 작업의 각 날에 대해 동일한 수의 계획된 시간을 할당합니다.

예를 들어, 작업이 오후 4시에 시작되도록 설정되고 예약에 작업의 첫 날에 1시간이 남은 경우 Workfront은 작업 기간의 첫 날에 1개의 계획된 시간을 배치한 다음 작업 기간의 나머지 일 간에 계획된 시간의 나머지를 균등하게 나눕니다.

>[!NOTE]
>
>일별 계획된 시간 또는 일별 할당은 작업 기간 동안 일별 계획된 시간을 할당하는 것입니다. 작업에 할당이 한 개 있는 경우 이 숫자는 할당당 하루 계획된 시간을 나타냅니다. 작업에 여러 개의 할당이 있는 경우 할당당 일별 계획된 시간이 작업에 대한 일별 계획된 시간과 다릅니다. 할당당 일별 계획된 시간 (일 기준), 여러 할당이 있는 작업에 대해서는 Workfront에 시각적으로 표시되지 않습니다.

## 계획된 시간 값 찾기 및 이해

Workfront의 다양한 영역에서 계획된 시간 값을 찾을 수 있습니다.

프로젝트의 작업 항목에서 시작되거나 표시되는 계획된 시간 수는 보고 있는 영역과 오브젝트에 따라 다르게 계산됩니다.

Workfront의 다음 영역에서 계획된 시간을 찾을 수 있습니다.

* [프로젝트, 작업 또는 문제의 세부 정보 섹션](#the-details-section-of-a-project-task-or-issue)
* [작업 편집 또는 문제 편집 상자](#the-edit-task-or-edit-issue-box)
* [보고서](#reports)
* [업무 균형자](#the-workload-balancer)
* [리소스 플래너](#the-resource-planner)
* [사용률 보고서](#the-utilization-report)
* [역할 할당 패널](#the-role-allocation-panel)

### 프로젝트, 작업 또는 문제의 세부 정보 섹션 {#the-details-section-of-a-project-task-or-issue}

세부 정보 섹션의 ![계획된 시간](assets/planned-hours-on-details-for-project.png)

작업, 문제 또는 프로젝트의 세부 정보 섹션에 있는 계획된 시간은 항목과 연결된 총 계획된 시간입니다.

프로젝트 계획된 시간에 대한 자세한 내용은 이 문서의 [작업에 대한 계획된 시간과 프로젝트에 대한 계획된 시간 비교](#planned-hours-on-tasks-vs-planned-hours-on-projects) 섹션을 참조하십시오.

### 작업 편집 또는 문제 편집 상자 {#the-edit-task-or-edit-issue-box}

![작업 상자 편집](assets/planned-hours-on-edit-task-box-nwe.png)

작업 또는 문제의 편집 상자에 있는 계획된 시간은 각 항목의 총 계획된 시간입니다.

프로젝트 계획된 시간에 대한 자세한 내용은 이 문서의 [작업에 대한 계획된 시간과 프로젝트에 대한 계획된 시간 비교](#planned-hours-on-tasks-vs-planned-hours-on-projects) 섹션을 참조하십시오.

작업의 경우 특정 기간 유형에 대해서만 계획된 시간을 편집할 수 있습니다. 자세한 내용은 이 문서에서 [기간 유형에 따라 작업 계획 시간 업데이트](#update-task-planned-hours-based-on-duration-type) 섹션을 참조하십시오.

할당 영역에서 작업 또는 문제에 할당된 각 사용자 또는 작업 역할에 대한 개별 계획된 시간 할당을 볼 수 있습니다.

### 보고서 {#reports}

보고서에 대한 ![계획된 시간](assets/planned-hours-on-task-report.png)

프로젝트, 작업 및 문제 보고서에 계획된 시간 필드를 추가할 수 있습니다.

계획된 시간 열은 기본적으로 작업 목록의 표준 보기에 포함됩니다.

작업, 문제 또는 프로젝트 보고서의 계획된 시간은 항목의 세부 정보 섹션 또는 편집 상자에 표시되는 각 항목의 총 계획된 시간입니다.

보고서 만들기에 대한 자세한 내용은 [사용자 지정 보고서 만들기](../../../reports-and-dashboards/reports/creating-and-managing-reports/create-custom-report.md)를 참조하세요.

>[!NOTE]
>
>프로젝트(재무 데이터) 보고서를 생성하여 날짜별로 그룹화할 경우 계획된 시간에는 프로젝트의 작업 타임라인에 따라 프로젝트의 계획된 시간의 일부가 표시될 수 있습니다. 기본적으로 Workfront은 작업 기간의 각 날에 대해 작업의 계획된 시간을 균등하게 분배합니다. 특정 시간대의 계획된 시간은 프로젝트(재무 데이터) 보고서에서 해당 시간대에 대해 Workfront이 설정한 균등 분포와 일치합니다.

<!--
### The Scheduling areas  {#the-scheduling-areas}

![](assets/task-detail-expanded-in-scheduler-with-planned-hours-and-adjusted-daily-allocations-nwe-350x323.png)

The Planned Hours for tasks and issues display in the Scheduling areas in the Planned Hours field.

You can view the daily allocation of Planned Hours for each user assigned to a task or an issue in the Scheduling areas.

The daily hour amount represents one of the following:

* the default amount equally distributed by Workfront for each day of the Duration of the tasks or issues
* the adjusted daily allocation managed by resource managers.

  For information about adjusting daily allocations in the Scheduling tools, see [Manage user allocations in the Scheduling areas](../../../resource-mgmt/resource-scheduling/manage-allocations-scheduling-areas.md).
-->

### 업무 균형자 {#the-workload-balancer}

![업무 균형자에서 계획된 시간](assets/planned-hours-on-wb-expanded-with-pti-info.png)

작업, 문제 및 프로젝트에 대한 다음 계획된 시간이 작업, 문제 또는 프로젝트 이름의 오른쪽에 있는 업무 균형자에 표시됩니다.

* 작업 및 문제의 경우 작업과 연결된 계획된 시간이 표시됩니다.
* 프로젝트의 경우 화면에 표시되는 작업 및 문제의 총 계획된 시간이 표시됩니다.

  >[!TIP]
  >
  >업무 균형자에 프로젝트의 계획된 모든 시간이 프로젝트 세부 정보 영역에 표시되는 것으로 표시되지 않습니다.

업무 균형자에서 작업 또는 문제에 할당된 각 사용자에 대한 일별 계획된 시간 할당을 볼 수 있습니다.

계획된 시간의 일일 시간 양은 다음 중 하나를 나타냅니다. 

* 작업, 문제 또는 프로젝트 기간 중 각 날에 Workfront에서 균등하게 분배하는 기본 금액
* 리소스 관리자가 관리하는 조정된 일일 할당

  업무 균형자에서 일별 할당을 조정하는 방법에 대한 자세한 내용은 [업무 균형자에서 사용자 할당 관리](../../../resource-mgmt/workload-balancer/manage-user-allocations-workload-balancer.md)를 참조하십시오.

### 리소스 플래너 {#the-resource-planner}

![리소스 플래너의 계획된 시간](assets/planned-hours-on-all-objects-in-resource-planned-expanded.png)

리소스 플래너에는 프로젝트, 작업 및 문제에 대한 계획된 시간이 표시됩니다.

리소스 플래너의 PLN 열에서 작업 항목과 연관된 사용자 및 작업 역할에 대한 주간 계획 시간 할당을 볼 수 있습니다.

>[!TIP]
>
>업무 균형자의 일일 할당 조정은 리소스 플래너의 작업 및 문제에 대한 주간 할당에 영향을 줍니다.

각 객체의 계획된 시간 수는 리소스 플래너에 적용하는 보기에 따라 다릅니다. 자세한 내용은 리소스 플래너의 프로젝트 및 역할 보기에서 [시간, FTE 및 비용 정보 개요](../../../resource-mgmt/resource-planning/overview-of-planner-hour-fte-cost-information-in-role-project-views.md)를 참조하십시오.

작업 및 문제에 대한 계획된 시간의 주별 시간 양은 다음 중 하나를 나타냅니다.

* 작업 또는 문제 기간 중 각 날에 대해 Workfront에서 균등하게 분배하는 기본 주별 금액
* 업무 균형자에서 리소스 관리자가 관리하는 조정된 주간 할당

  업무 균형자에서 일별 할당을 조정하는 방법에 대한 자세한 내용은 [업무 균형자에서 사용자 할당 관리](../../../resource-mgmt/workload-balancer/manage-user-allocations-workload-balancer.md)를 참조하십시오.

프로젝트, 사용자 및 역할의 주간 양은 프로젝트, 사용자 및 역할과 관련된 작업 및 문제에 대한 주간 계획된 시간의 영향을 받습니다.

### 활용성 보고서 {#the-utilization-report}

프로젝트 계획 시간은 각 작업 및 문제의 할당과 연결된 시간입니다.

>[!IMPORTANT]
>
>활용률 보고서의 계획된 시간은 작업과 문제 자체가 아니라 할당과 연관되어 있습니다. 활용성 보고서의 계획된 시간이 프로젝트의 작업 및 문제에 대한 계획된 시간과 항상 일치하는 것은 아닙니다. 그러나 계획된 시간은 작업 및 문제에 대한 할당과 연관된 시간과 일치합니다.

활용성 보고서에서 다음 유형의 계획된 시간을 조회할 수 있습니다.

* 포함된 프로젝트의 전체 수명 동안 프로젝트에 대한 모든 할당의 총 계획된 시간
* 지정된 날짜 범위에 대해서만 모든 할당의 총 계획된 시간(개별 주 또는 월을 지정할 수 있음).

  업무 균형자 를 사용하여 시간에 대한 사용자 일일 할당을 조정한 경우 활용성 보고서에서 선택한 날짜에 작업 또는 문제 기간의 일부만 포함된 경우 특정 날짜 범위에 대한 계획된 시간이 영향을 받을 수 있습니다. 사용자의 일일 할당 조정에 대한 자세한 내용은 [업무 균형자에서 사용자 할당 관리](../../../resource-mgmt/workload-balancer/manage-user-allocations-workload-balancer.md)를 참조하십시오.

자세한 내용은 [리소스 사용률 정보 보기](../../../resource-mgmt/resource-utilization/view-utilization-information.md)를 참조하십시오.

### 역할 할당 패널

역할 할당 패널의 계획된 시간은 프로젝트의 총 기간 동안 프로젝트의 작업 또는 문제에 할당된 각 작업 역할과 연관된 계획된 시간 수를 나타냅니다. 이 숫자는 리소스 플래너의 계획된 시간 역할과 일치합니다.

>[!TIP]
>
>사용자와 연결된 계획된 시간은 역할 할당 패널에 표시되지 않습니다.

자세한 내용은 [업무 균형자에서 프로젝트 및 이니셔티브에 대한 역할 할당 표시](../../../scenario-planner/show-role-allocation-workload-balancer.md)를 참조하십시오.

## 기간 유형에 따라 작업 계획 시간 업데이트 {#update-task-planned-hours-based-on-duration-type}

작업에 특정 기간 유형이 있는 경우에만 작업을 편집할 때 작업에 대한 총 계획된 시간을 업데이트할 수 있습니다.

다음과 같은 시나리오가 있습니다.

* 작업을 편집할 때 [계산된 할당] 또는 [단순 기간 유형]을 사용하는 경우에만 작업의 계획된 시간을 수정할 수 있습니다.

  계산된 할당 기간 유형에 대한 자세한 내용은 [기간 유형 개요: 계산된 할당](../../../manage-work/tasks/taskdurtn/calculated-assignment.md)을 참조하십시오.

  단순 기간 유형에 대한 자세한 내용은 [기간 유형 개요: 단순](../../../manage-work/tasks/taskdurtn/simple-duration-type.md)을 참조하십시오.

* 작업에 대한 사용자의 할당을 관리할 때 업무 균형자에서 단순 기간 유형 작업에 대해서만 작업 계획 시간을 업데이트할 수 있습니다. 업무 균형자에서 사용자 할당 관리에 대한 자세한 내용은 [업무 균형자에서 사용자 할당 관리](../../../resource-mgmt/workload-balancer/manage-user-allocations-workload-balancer.md)를 참조하십시오.
* 기간 유형이 작업량 고정 또는 계산된 작업인 작업의 계획된 시간은 수정할 수 없습니다. 이러한 경우 Workfront은 작업의 기간을 기반으로 계획된 시간을 결정합니다. 그러나 이 경우 계획된 시간은 항상 기간(시간)과 같으며 할당된 리소스의 퍼센트 할당의 영향을 받지 않습니다.

  작업량 고정 기간 유형에 대한 자세한 내용은 [작업량 유형 개요: 작업량 고정](../../../manage-work/tasks/taskdurtn/effort-driven.md)을 참조하십시오.

  계산된 작업 기간 유형에 대한 자세한 내용은 [기간 유형 개요: 계산된 작업](../../../manage-work/tasks/taskdurtn/calculated-work.md)을 참조하십시오.

## 사용자 할당 관리 시 작업 계획 시간 업데이트

작업에 대한 사용자 또는 작업 역할 할당을 수동으로 업데이트할 때 작업에 대한 계획된 시간을 업데이트할 수 있습니다. 작업의 기간 유형이 단순인 경우에만 가능합니다.

자세한 내용은 [기간 유형 개요: 단순](../../../manage-work/tasks/taskdurtn/simple-duration-type.md)을 참조하십시오.

작업에 할당된 사용자 및 역할의 전체 할당 또는 업무 균형자 사용 시 일일 사용자 할당을 업데이트할 수 있습니다.

작업에 대한 전체 사용자 및 작업 역할 할당 관리에 대한 자세한 내용은 [작업에 대한 사용자 및 역할 할당 시간 관리](../../../manage-work/tasks/assign-tasks/manage-allocation-hours-on-tasks.md)를 참조하십시오.

작업의 일일 할당 관리에 대한 자세한 내용은 [업무 균형자에서 사용자 할당 관리](../../../resource-mgmt/workload-balancer/manage-user-allocations-workload-balancer.md)를 참조하십시오.

작업에 대한 사용자 또는 작업 역할 할당을 수동으로 업데이트할 때 다음과 같은 시나리오가 있습니다.

* 작업 계획 시간에 대한 변경을 트리거하기 위해 개별 사용자 또는 역할 할당을 수동으로 업데이트하지 않은 경우 작업에 대한 할당을 추가, 제거 또는 대체할 때 계획된 시간은 변경되지 않습니다. 작업에 새 할당을 추가하면 개별 할당이 모든 할당자 간에 재배포됩니다.
* 작업 계획 시간에 대한 변경을 트리거하도록 할당을 수동으로 업데이트한 경우 작업에서 할당을 제거하면 계획 시간이 줄어듭니다. 할당을 대체할 때 변경되지 않습니다.
* 태스크 계획 시간에 대한 변경을 트리거하기 위해 할당을 수동으로 갱신하고 태스크에 지정을 추가하면 신규 지정은 기본적으로 0시간으로 할당됩니다. 계획된 시간에 영향을 미칠 수 있는 작업에 대한 할당을 수동으로 업데이트해야 합니다.
* 작업 계획 시간에 대한 변경을 트리거하기 위해 할당을 수동으로 갱신하지 않았으며 작업에 대한 모든 할당을 제거해도 계획 시간은 변경되지 않습니다.
* 작업 계획 시간에 대한 변경을 트리거하기 위해 할당을 수동으로 업데이트하고 작업에 대한 모든 할당을 제거하면 계획된 시간도 제거되고 작업의 계획된 시간은 0이 됩니다.

>[!NOTE]
>
>예를 들어 작업에 계획된 시간이 10시간이고 할당자가 2명인 경우 기본적으로 각각 5시간이 할당됩니다.
>
>* 업무 균형자 를 사용하여 개별 사용자 할당 또는 일별 할당을 업데이트하지 않고 할당자를 작업에서 모두 또는 모두 제거한 경우 작업 계획 시간은 10시간으로 유지됩니다.
>* 할당의 할당을 각각 4시간 및 6시간으로 수동으로 변경하고 6시간에 할당된 사용자와 해당 작업 역할을 제거하면 작업 계획 시간이 4시간으로 업데이트됩니다. 4시간에 할당된 사용자도 제거하지만 제거된 사용자와 연결된 작업 역할을 유지하는 경우, 작업의 계획된 시간은 4시간으로 유지됩니다. 작업 역할과 4시간에 할당된 마지막 사용자를 제거하고 작업이 할당 해제된 상태로 있으면 작업 계획 시간이 0이 됩니다.

## 작업 노력을 사용하여 작업 계획 시간을 자동으로 업데이트

작업 노력을 사용하여 작업을 완료하는 데 필요한 노력을 예상하면 작업의 계획된 시간이 자동으로 업데이트됩니다. 단순 기간 유형의 작업에만 가능합니다.

작업 노력을 사용하여 작업 노력을 예측하는 방법에 대한 자세한 내용은 [작업 노력 개요](../../../manage-work/tasks/task-information/work-effort.md)를 참조하십시오.

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: this issue has the explanation of how Planned Hours should work - from Vazgen and Anna: https://hub.workfront.com/issue/6217dced00730b7034c4b808339a35ce/</p>
-->

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">Details of their comments: </p>
-->

<!--
<div data-mc-conditions="QuicksilverOrClassic.Draft mode">
<p>Anna Asatryan</p>
<p>3/22/2022 At 3:16 PM</p>
<p>&nbsp;</p>
<p>to Mark Paul, Corrie Butler, Arman Simonyan, Gagik Khalatyan, Alina Wilson, Artur Sargsyan, Vazgen Babayan, Anna Asatryan</p>
<p>I have done some rough calculations on what the planned hours/revenues should look like Book.xlsx . And if we look, for example at the 2 users highlighted in one of the screenshots their planned hours look way off from what the calculation looks like in the spreadsheet (i.e. equally distributed allocation). When looking at the Workload balancer (the second screenshot), as an example for the user Yashas Mitta, I can see that the allocation has been modified. Obviously the utilization report calculates the allocations based on the modified contouring using the new work per day calculation. The project financial report uses the old, equal distribution of allocation along the full duration of the task. Hence. there is a difference when grouping per periods.</p>
<p>Vazgen Babayan</p>
<p>I believe we will need to prioritise syncing the project financial data report with the new work per day.</p>
<p>Alina Wilson</p>
<p>@Anna Asatryan , do you have a definition of what we should say in documentation (glossary, for example) for how the Planned Hours (or Planned Revenue) is calculated, keeping in mind that we don't document the concept of "workPerDay". We call them "daily allocations", for example, but let me know if that's accurate, too.</p>
<p>Vazgen Babayan</p>
<p>Last Thursday at 3:13 PM</p>
<p>I think an important note here is that regardless the calculation, even if the both views used the same formula, they will not display the same data, because the underlying data sources are different. The Financial Data report does not respect user-entered allocations in Workload Balancer at this moment. So there will be a clear discrepancy, as Anna showed in her message. My recommendation for communication will be to explain that the data sources are different so there can be a mismatch in data and that we will look into addressing that on our roadmap.</p>
<p>Alina Wilson</p>
<p>So far, I hear you guys say this (with my questions for confirmation/ comments in bold):</p>
<p>- the utilization report calculates the allocations based on the modified contouring using the new work per day calculation (so this is what we see in the Workload Balancer, right?)</p>
<p>- the project financial report uses the old, equal distribution of allocation along the full duration of the task (this is before the daily allocations for example were modified in the WB, right?)</p>
<p>I have these additional questions:</p>
<p>- what does the Project Details show? Which Planned Hours, for instance - because earlier, we had a question about this also. - which numbers?</p>
<p>- what does any Planned Hours/ Planned Revenue field that can be pulled in any other report (outside of Financial Data and Utilization reports) show? - which numbers?</p>
<p>- are there any other areas I am not thinking of that we need to document, @Corrie Butler</p>
<p>I will try to document all the possible areas where these display but please help. Thanks!</p>
<p>Vazgen Babayan</p>
<p>Last Saturday at 3:41 PM</p>
<ul>
<li> <p>Confirming the first two points </p> </li>
</ul>
<p>For the following questions</p>
<ul>
<li> <p>Project details show an aggregated sum of task planned hours. It doesn't have anything to do with the work per day because it always deals with total numbers for the whole duration of the Project/Task.</p> </li>
<li> <p>Same thing applies to the Planned Hours and Planned Revenue fields in reports - they show totals for the whole Project/Task duration and thus have no use of work per day.</p> </li>
<li> <p>Can't think of any other fields related to this right now.</p> </li>
<li> <p>In general, if I were to summarize the system behavior, it's as follows:</p> </li>
<li> <p>Every area that only deals with total numbers of Planned Hours / Planned Revenue, uses the numbers entered on the tasks. Those are Task / Project Details, reports exposing those fields.</p> </li>
<li> <p>Areas that deal with time-sensitive portions of Planned Hours / Planned Revenue, use work per day. Those are all Resource Management tools - Workload Balancer, Resource Planner, Utilization Report, importing projects via Scenario Planner.</p> </li>
<li> <p>All the areas in the second point support user-edited allocations made in Workload Balancer.</p> </li>
<li> <p>Scheduling area and Project Financial Data reports use the old version of the work per day, which doesn't respect user-edited allocations from Workload Balancer.</p> </li>
<li> <p>Scheduling will be removed this year, and we need to do work to move the Project Financial Data reports to the new work per day sometime after Q3.</p> </li>
</ul>
<p>Alina Wilson</p>
<p>@Vazgen Babayan , one clarifying question: when you say "Scheduling and Project Financial Data reports use the old version of the work per day, which doesn't respect user-edited allocations from WB" - you mean that those use the system default which spreads the allocations evenly, correct? Because you can edit (daily) allocations in Scheduling tools, but it doesn't use that, correct? It uses the default of the daily allocation that the system figures out when dividing the Planned Hours by the number of days in the Duration. Please let me know. And thanks!</p>
<p>Anna Asatryan</p>
<p>Yesterday at 11:42 AM</p>
<p>@Alina Wilson , that's correct, when saying "Scheduling and Project Financial Data reports use the old version of the work per day, which doesn't respect user-edited allocations from WB" Vazgen meant that it spreads the allocation evenly.</p>
<p>As for the scheduling, the allocation modification that's being done there isn't reflected anywhere else in the application other than in the Scheduling itself. That's probably one of the reasons it's being deprecated.</p>
</div>
-->

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode"> <br> </p>
-->

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: everything below is drafted because I replaced it with the table above)</p>
-->

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">You can find the Planned Hours information on tasks, issues, or projects in the following locations:</p>
-->

<!--
<div data-mc-conditions="QuicksilverOrClassic.Draft mode">
<p>The Planned Hours in the Details  section  of a task, issue, or project are the total Planned Hours of the respective item. </p>
<p>Finding the Planned Hours in the Details  section  is identical for tasks, issues, and projects. </p> <note type="tip">
You cannot edit the Planned Hours of projects manually, as they are a calculation of all Planned Hours of all the tasks on the project.
</note>
<p>To locate the Planned Hours value on the Details  section  of a task: </p>
<ol>
<li value="1">Go to a task for which you want to review the Planned Hours.</li>
<li value="2"> <p data-mc-conditions="QuicksilverOrClassic.Quicksilver">Click <strong>Task Details</strong> in the left panel. </p> </li>
<li value="3"> <p data-mc-conditions="QuicksilverOrClassic.Quicksilver">Click the <strong>Overview</strong> area and notice the Planned Hours value.</p> <p>This value represents the time it would take the user assigned to the task to complete it. </p> </li>
</ol>
</div>
-->

<!--
<div data-mc-conditions="QuicksilverOrClassic.Draft mode">
<h3> </h3>
<p>The Planned Hours in the Edit box of a task, issue, or project are the total Planned Hours of the respective item. </p>
<p>Finding the Planned Hours while editing a task or an issue is identical. </p> <note type="tip">
You cannot edit the Planned Hours of projects manually, as they are a calculation of all Planned Hours of all the tasks on the project.
</note>
<p>To locate the value of Planned Hours while editing a task:</p>
<ol>
<li value="1">Go to the task or issue you want to view Planned Hours for.</li>
<li value="2"> <p data-mc-conditions="QuicksilverOrClassic.Quicksilver">Click the <strong>More</strong> icon <img src="assets/qs-more-icon-on-an-object.png"> next to the task name, then click <strong>Edit</strong>.</p> <p>The Planned Hours are located in the <strong>Overview</strong> section. </p> </li>
</ol>
</div>
-->

<!--
<div data-mc-conditions="QuicksilverOrClassic.Draft mode">
<p>The Planned Hours column is included in the Standard view of a task list, by default. For issues and projects, you can add it to the view, when you are editing the view or when you build a report. </p>
<p>The Planned Hours in a task, issue, or project report are the total Planned Hours of the respective item as they display in the Details  section  or the Edit box of the items. </p>
<p>Adding the Planned Hours column to a project view is similar to building a view in a project report. </p>
<p>To show Planned Hours in a project report:</p>
<ol>
<li value="1"> <p data-mc-conditions="QuicksilverOrClassic.Quicksilver">Click the <strong>Main Menu</strong> icon <img src="assets/main-menu-icon.png"> in the upper-right corner of Workfront, then click <strong>Reports</strong>. </p> </li>
<li value="2">Click <strong>New Report</strong>, then choose <strong>Project</strong> as your object.</li>
<li value="3">Click <strong>Add Column</strong>, and start typing <strong>Planned Hours</strong> when the <strong>Show in this column</strong> drop-down field is displayed. Select the field when it appears in the list.</li>
<li value="4"> <p>Click <strong>Save + Close</strong> to save the report. </p> <p>The Planned Hours column shows the total number of Planned Hours on each project. </p> </li>
</ol>
</div>
-->

<!--
<div data-mc-conditions="QuicksilverOrClassic.Draft mode">
<p>Planned Hours in Resource Management tools</p> <note type="important">
When viewing Planned Hours in the Resource Management tools by a specific time frame, the daily allocations for each work item and the daily allocations for the resources assigned to the work items during that time frame can influence the daily Planned Hours of projects or work items.
</note>
<p>You can see the value of Planned Hours for your tasks, issues, or projects when using the following Resource Management tools:</p>
<ul>
<li> <p>Resource Planner</p> <p>For information about using the Resource Planner, see <a href="../../../resource-mgmt/resource-planning/get-started-resource-planner.md" class="MCXref xref">Resource Planner overview</a>.</p> </li>
<li> <p>Utilization Report.</p> <p>For information about the utilization report, see <a href="../../../reports-and-dashboards/reports/using-built-in-reports/resource-utilization-report.md" class="MCXref xref">Overview of the Resource Utilization report</a>.</p> </li>
<li>
<div data-mc-conditions="QuicksilverOrClassic.Quicksilver">
<p>Workload Balancer or Scheduling areas in the following sections:</p>
<ul>
<li>Scheduling or Workload Balancer sections in the Resourcing area</li>
<li>Scheduling or Workload Balancer section at the project level</li>
<li>Schedule or Workload Balancer section at the team level</li>
</ul>
</div> <p>For information about scheduling resources, see <a href="../../../resource-mgmt/resource-scheduling/get-started-resource-scheduling.md" class="MCXref xref">Get started with Resource Scheduling</a>.</p> <p>For information about the Workload Balancer, see <a href="../../../resource-mgmt/workload-balancer/overview-workload-balancer.md" class="MCXref xref">Workload Balancer overview</a>. </p> </li>
<li> <p><b>Role Allocation panel</b> in the project  task list or  Workload Balancer: The Planned Hours for the tasks and the issues on the project that are assigned to a job role or a user associated with a job role are taken into account in this area. For more information, see <a href="../../../manage-work/projects/planning-a-project/view-planed-hours-in-role-allocation-panel.md" class="MCXref xref">View project Planned Hours in the Role Allocation panel</a>. </p> </li>
</ul>
</div>
-->
