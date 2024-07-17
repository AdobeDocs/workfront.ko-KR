---
content-type: release-notes
keywords: 메모,분기별,업데이트,릴리스
navigation-topic: 2021-2-release-activity
title: 21.2 향상된 리소스 관리 기능
description: 이 페이지에서는 미리보기 환경에 대한 21.2 릴리스의 모든 리소스 관리 개선 사항에 대해 설명합니다. 이러한 개선 사항은 2021년 5월 10일이 있는 주에 프로덕션 환경에서 사용할 수 있습니다. 21.2 릴리스에서 사용할 수 있는 모든 변경 사항 목록은 21.2 릴리스 개요 를 참조하십시오.
author: Luke
feature: Product Announcements
recommendations: noDisplay, noCatalog
exl-id: 00133efe-f779-4217-87af-a223dcf043ee
source-git-commit: 76deb76c66e8f8a7dea721378591ae035b8d42e7
workflow-type: tm+mt
source-wordcount: '564'
ht-degree: 0%

---

# 21.2 향상된 리소스 관리 기능

이 페이지에서는 미리보기 환경에 대한 21.2 릴리스의 모든 리소스 관리 개선 사항에 대해 설명합니다. 이러한 개선 사항은 2021년 5월 10일이 있는 주에 프로덕션 환경에서 사용할 수 있습니다. 21.2 릴리스에서 사용할 수 있는 모든 변경 사항 목록을 보려면 [21.2 릴리스 개요](../../../product-announcements/product-releases/21.2-release-activity/21-2-release-overview.md)를 참조하십시오.

## 업무 균형자의 월별 수준 보기

더 많은 기간 동안 리소스 할당을 관리할 수 있도록 이제 업무 균형자에 대한 월 단위 보기를 구현했습니다. 한 번에 최대 3개월을 보고 월별 리소스 할당을 업데이트할 수 있습니다. 이 변경 이전에는 일별 또는 주별로만 업무 균형자를 볼 수 있었습니다.

자세한 내용은 [업무 균형자 탐색](../../../resource-mgmt/workload-balancer/navigate-the-workload-balancer.md)을 참조하십시오.

## 시나리오 플래너, 업무 균형자 및 작업 목록 간의 연결

>[!NOTE]
>
>새로운 Adobe Workfront 경험에서만 사용할 수 있습니다.

프로젝트의 전략적 계획을 수립하고 시나리오 플래너의 전체적인 이니셔티브에 맞게 조정할 수 있도록 이니셔티브의 작업 역할 요구 사항과 프로젝트의 작업 항목에 대한 계획된 시간을 표시하는 새로운 영역을 프로젝트에 만들었습니다. 이 영역은 프로젝트 수준의 업무 균형자 와 새 Workfront 환경의 작업 목록에서 사용할 수 있습니다. 클래식 경험에서는 업무 균형자 프로젝트에서만 사용할 수 있습니다.

자세한 내용은 다음 문서를 참조하십시오.

* [프로젝트와 이니셔티브 간의 리소스 할당 조정에 대한 개요](../../../scenario-planner/overview-reconcile-allocations-between-projects-initiatives.md).
* [업무 균형자 탐색](../../../resource-mgmt/workload-balancer/navigate-the-workload-balancer.md)

>[!IMPORTANT]
>
>이 새 기능은 새 Workfront 환경과 클래식 환경 모두에서 모든 사용자에게 표시됩니다. Workfront Scenario Planner 라이선스를 구입하지 않은 고객에게도 표시됩니다.

## 리소스 플래너에서 순 값을 계산할 때 계획된 시간 사용

리소스 플래너의 새 설정을 사용하면 순 값을 계산할 때 계획된 시간을 사용할 수 있습니다.

이 개선 이전에는 Workfront에서 예산 시간만 사용하여 순 값을 계산했습니다. 순 값에는 가용 시간과 예산 또는 계획 시간, FTE 또는 비용의 차이가 표시됩니다. 순 값을 계산할 때 예산 시간은 여전히 기본 설정입니다.

자세한 내용은 리소스 플래너의 프로젝트 및 역할 보기에서 [시간, FTE 및 비용 정보 개요](../../../resource-mgmt/resource-planning/overview-of-planner-hour-fte-cost-information-in-role-project-views.md)를 참조하십시오.

## 업무 균형자에서 12주 보기

이제 업무 균형자에서 최대 12주의 정보를 볼 수 있습니다. 이 기능이 향상되기 전에는 2, 4, 6주 동안의 정보를 볼 수 있었습니다.

업무 균형자 보기에 대한 자세한 내용은 [업무 균형자 탐색](../../../resource-mgmt/workload-balancer/navigate-the-workload-balancer.md)업무 균형자 탐색을 참조하십시오.

## 업무 균형자의 미할당 영역에서 작업 역할 필터 작동 방식 변경

업무 균형자에서 작업 역할 필터 의 작동 방식을 개선하고 사용자의 기대에 맞게 할당되지 않음 영역에서 필터 기능을 수정했습니다. 이제 필터에서 지정한 작업 역할에 할당된 시간만 볼 수 있습니다.

이 개선 사항 이전에는 작업 역할 필터를 미할당 영역에 적용할 때 업무 균형자에 작업 역할에 할당된 작업 항목과 연결된 모든 시간이 표시되었습니다.

업무 균형자에서 정보를 필터링하는 방법에 대한 자세한 내용은 [업무 균형자에서 필터 관리](../../../resource-mgmt/workload-balancer/filter-information-workload-balancer.md)를 참조하십시오.
