---
content-type: release-notes
keywords: 메모,분기별,업데이트,릴리스
navigation-topic: 2021-2-release-activity
title: 21.2 리소스 관리 개선 사항
description: 이 페이지에서는 미리 보기 환경에 대한 21.2 릴리스로 향상된 리소스 관리 기능에 대해 설명합니다. 이러한 개선 사항은 2021년 5월 10일이 있는 프로덕션 환경에서 사용할 수 있습니다. 21.2 릴리스에서 사용할 수 있는 모든 변경 사항 목록은 21.2 릴리스 개요를 참조하십시오.
author: Luke
feature: Product Announcements
exl-id: 00133efe-f779-4217-87af-a223dcf043ee
source-git-commit: 665732453b33b49421108791a560ab84d51280b9
workflow-type: tm+mt
source-wordcount: '556'
ht-degree: 0%

---

# 21.2 리소스 관리 개선 사항

이 페이지에서는 미리 보기 환경에 대한 21.2 릴리스로 향상된 리소스 관리 기능에 대해 설명합니다. 이러한 개선 사항은 2021년 5월 10일이 있는 프로덕션 환경에서 사용할 수 있습니다. 21.2 릴리스에서 사용할 수 있는 모든 변경 사항 목록에 대해서는 다음을 참조하십시오 [21.2 릴리스 개요](../../../product-announcements/product-releases/21.2-release-activity/21-2-release-overview.md).

## 작업 로드 밸런서의 월 수준 보기

더 많은 시간 동안 리소스 할당을 관리하는 데 도움이 되도록, 이제 Workload Balancer에 대한 월 레벨 뷰를 구현했습니다. 한 번에 최대 3개월을 보고 월별 리소스 할당을 업데이트할 수 있습니다. 이 변경 전에 작업 로드 밸런서를 일 또는 주로만 볼 수 있습니다.

자세한 내용은 [작업 로드 밸런서 탐색](../../../resource-mgmt/workload-balancer/navigate-the-workload-balancer.md).

## 시나리오 플래너, 작업 로드 밸런서 및 작업 목록 간 연결

>[!NOTE]
>
>새 Adobe Workfront 경험에서만 사용할 수 있습니다.

프로젝트의 전략적 계획을 지원하고 시나리오 플래너의 대규모 이니셔티브에 맞게 프로젝트를 계획할 수 있도록 하기 위해 Adobe에서는 프로젝트의 작업 항목에 대한 예상 작업 시간과 이니셔티브 작업 역할 요구 사항을 표시하는 프로젝트에 새 영역을 만들었습니다. 이 영역은 프로젝트 수준 작업 로드 밸런서와 새 Workfront 환경의 작업 목록에 사용할 수 있습니다. 클래식 환경에서는 프로젝트 작업 로드 밸런서에만 사용할 수 있습니다.

자세한 내용은 다음 문서를 참조하십시오.

* [프로젝트 및 이니셔티브 간 리소스 할당 조정 개요](../../../scenario-planner/overview-reconcile-allocations-between-projects-initiatives.md).
* [작업 로드 밸런서 탐색](../../../resource-mgmt/workload-balancer/navigate-the-workload-balancer.md)

>[!IMPORTANT]
>
>이 새 기능은 새 사용자와 클래식 Workfront 경험 모두에서 모든 사용자가 볼 수 있습니다. Workfront Scenario Planner 라이센스를 구입하지 않은 고객에게도 표시됩니다.

## 자원 계획자에서 순 값을 계산할 때 계획 시간 사용

자원 계획자의 새 설정을 사용하면 순 값을 계산할 때 계획 시간을 사용할 수 있습니다.

이 개선 사항 전에 Workfront은 예산책정된 시간만 사용하여 순 값을 계산했습니다. 순 값에는 사용 가능 및 예산책정됨 또는 계획됨 시간, FTE 또는 원가 간의 차이가 표시됩니다. 예산책정된 시간은 순 값을 계산할 때 여전히 기본 설정입니다.

자세한 내용은 [리소스 계획자의 프로젝트 및 역할 뷰의 시간, FTE 및 비용 정보 개요](../../../resource-mgmt/resource-planning/overview-of-planner-hour-fte-cost-information-in-role-project-views.md).

## 작업 로드 밸런서에서 12주 보기

이제 작업 로드 밸런서에서 최대 12주의 정보를 볼 수 있습니다. 이 개선 사항 전에 2, 4 및 6주의 정보를 볼 수 있습니다.

작업 로드 밸런서 보기에 대한 자세한 내용은 [작업 로드 밸런서 탐색](../../../resource-mgmt/workload-balancer/navigate-the-workload-balancer.md)작업 로드 밸런서를 탐색합니다.

## 작업 부하 분산 장치의 [지정되지 않음] 영역에서 작업 역할 필터가 작동하는 방식을 변경합니다.

작업 로드 밸런서에서 작업 역할 필터가 작동하는 방식을 개선하고 사용자의 기대에 부응하기 위해 미지정 영역에서 필터 기능을 수정했습니다. 이제 필터에 지정하는 작업 역할에 할당된 시간만 볼 수 있습니다.

이 개선 사항 전에 [작업 역할] 필터를 [지정되지 않음] 영역에 적용할 때 [작업 밸런서]는 작업 역할에 할당된 작업 항목과 관련된 모든 시간을 표시합니다.

작업 로드 밸런서의 필터링 정보에 대한 자세한 내용은 [작업 로드 밸런서에서 필터 관리](../../../resource-mgmt/workload-balancer/filter-information-workload-balancer.md).
