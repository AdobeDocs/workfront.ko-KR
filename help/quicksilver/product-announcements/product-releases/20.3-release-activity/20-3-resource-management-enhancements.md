---
content-type: release-notes
navigation-topic: 2020-3-release-activity
title: 20.3 리소스 관리 개선 사항
description: 이 페이지에서는 프로덕션 환경에 대한 20.3 릴리스에서 향상된 리소스 관리 기능에 대해 설명합니다. 이러한 개선 사항은 2020년 8월 10일이 있는 주의 프로덕션 환경에서 사용할 수 있었습니다.
author: Luke
feature: Product Announcements
exl-id: a2c34117-e03c-4394-9b81-7c18433531d1
source-git-commit: 665732453b33b49421108791a560ab84d51280b9
workflow-type: tm+mt
source-wordcount: '829'
ht-degree: 0%

---

# 20.3 리소스 관리 개선 사항

이 페이지에서는 프로덕션 환경에 대한 20.3 릴리스에서 향상된 리소스 관리 기능에 대해 설명합니다. 이러한 개선 사항은 2020년 8월 10일이 있는 주의 프로덕션 환경에서 사용할 수 있었습니다.

20.3 릴리스에서 사용할 수 있는 모든 변경 사항 목록에 대해서는 다음을 참조하십시오 [20.3 릴리스 개요](../../../product-announcements/product-releases/20.3-release-activity/20.3-release-overview.md).

## 작업 로드 밸런서의 지정된 작업 영역 문제 발생 시간 포함

모든 사용자 작업 로드의 전체 그림을 볼 수 있도록, 작업 로드 밸런서의 할당된 작업 영역에 있는 문제의 시간을 포함할 수 있는 설정을 도입했습니다.

작업 로드 밸런서에서 작업에 대한 자세한 내용은 [작업 로드 밸런서 탐색](../../../resource-mgmt/workload-balancer/navigate-the-workload-balancer.md).

## 작업 로드 밸런서에서 비작업 날짜에 대한 할당 조정

작업 로드 밸런서를 사용하여 비근무일 자원에 대한 할당을 조정할 수 있습니다.

작업 로드 밸런서에서 할당 관리에 대한 자세한 내용은 [작업 로드 밸런서에서 사용자 할당 관리](../../../resource-mgmt/workload-balancer/manage-user-allocations-workload-balancer.md).

## 작업 로드 밸런서에서 사용할 수 있는 변수 필터

경험을 향상하고 정보를 공유할 때 보다 유연하게 활용할 수 있도록 작업 로드 밸런서에 대한 변수 필터를 구현했습니다. 다음 필터가 작업 로드 밸런서에 추가되었습니다.

* &quot;Me&quot;(사용자별로 필터링할 때)
* &quot;내 기본 역할&quot;(역할별로 필터링할 때)
* &quot;내 홈 팀&quot; 또는 &quot;모든 내 팀&quot;(팀별로 필터링할 때)

이 필터는 $$USER.ID, $$USER.roleID, $$USER.homeTeamID 및 $$USER.teamIDs의 와일드카드 필터 변수를 대체합니다

이러한 필터 중 하나를 적용한 다음 작업 로드 밸런서를 공유하거나 대시보드에 배치하면 다른 모든 사용자는 자신의 정보를 볼 수 있습니다.

작업 로드 밸런서에 필터를 적용하는 방법은 다음을 참조하십시오 [작업 로드 밸런서에서 정보 필터링](../../../resource-mgmt/workload-balancer/filter-information-workload-balancer.md).

## 작업 로드 밸런서에서 프로젝트에 대한 새 정렬

이제 작업 로드 밸런서는 사용자가 화면에 표시하는 시간대에 발생하는 프로젝트의 가장 이른 계획 시작 날짜와 두 번째 계획 완료 날짜에 따라 프로젝트를 정렬합니다. 이를 통해 하루 동안의 작업을 보다 쉽게 식별할 수 있도록 트리 형태의 계층 구조로 작업을 구성할 수 있습니다.

작업 로드 밸런서에서 프로젝트 및 작업 항목 보기에 대한 자세한 내용은 [작업 로드 밸런서 탐색](../../../resource-mgmt/workload-balancer/navigate-the-workload-balancer.md).

## 작업 로드 밸런서에서 실제 작업 진행 상태 표시

작업 로드 진행 상황을 정확하게 파악할 수 있도록 작업 로드 밸런서에 작업 및 문제의 타임라인을 예상 날짜에 따라 표시하는 새로운 설정을 도입했습니다. 예상 날짜 표시 설정을 활성화하여 계획된 타임라인과 함께 작업 항목의 예상 타임라인을 볼 수 있습니다.

또한 이 개선 사항을 통해, 작업 또는 문제가 계획 완료 일자보다 먼저 완료된 경우 남은 일수의 할당된 시간이 사용자의 전체 할당에 포함되지 않음을 나타냅니다.

작업 로드 밸런서 탐색 및 설정 활성화에 대한 자세한 내용은 [작업 로드 밸런서 탐색](../../../resource-mgmt/workload-balancer/navigate-the-workload-balancer.md).

## 20.2 릴리즈와 함께 릴리스된 작업 로드 밸런서 기능

* [작업 로드 밸런서에서 일별 및 주별 할당 조정](#adjust-daily-and-weekly-allocation-in-the-workload-balancer)
* [작업 로드 밸런서에서 작업 계획 시간 업데이트](#update-task-planned-hours-in-the-workload-balancer)
* [작업 로드 밸런서에서 할당을 보다 간편하게 업데이트하는 방법](#a-more-convenient-way-to-update-allocations-in-the-workload-balancer)

### 작업 로드 밸런서에서 일별 및 주별 할당 조정 {#adjust-daily-and-weekly-allocation-in-the-workload-balancer}

이제 리소스가 소모되지 않도록 작업 로드 밸런서를 사용하여 작동하도록 사용자의 일별 및 주별 할당을 조정할 수 있습니다.

이 개선 사항 이전에는 리소스 예약 도구를 사용해야만 이 작업이 가능했습니다.

작업 로드 밸런서에서 할당 관리에 대한 자세한 내용은 [작업 로드 밸런서에서 사용자 할당 관리](../../../resource-mgmt/workload-balancer/manage-user-allocations-workload-balancer.md).

**다음 환경에서 사용 가능:**

* Adobe Workfront Classic
* 새로운 Adobe Workfront 경험

### 작업 로드 밸런서에서 작업 계획 시간 업데이트 {#update-task-planned-hours-in-the-workload-balancer}

>[!NOTE]
>
>이 개선 사항은 2020.2 릴리스 직후 프로덕션에서 사용할 수 있습니다.

이제 액세스 수준의 리소스 관리 영역에 있는 새 옵션을 통해 이 액세스 권한이 있는 사용자가 작업 로드 밸런서에서 계획 시간을 편집할 수 있습니다. 작업 로드 밸런서에서 할당을 조정할 때 일일 할당 총계는 작업의 계획 시간 수와 일치하지 않아도 됩니다. 할당을 저장하면 총 할당 시간이 작업의 계획 시간이 됩니다. 단순 기간 유형이 있는 작업에만 가능합니다.

작업 로드 밸런서에서 할당 관리에 대한 자세한 내용은 [작업 로드 밸런서에서 사용자 할당 관리](../../../resource-mgmt/workload-balancer/manage-user-allocations-workload-balancer.md).

리소스 관리에 대한 액세스 권한 부여에 대한 자세한 내용은 [리소스 관리에 대한 액세스 권한 부여](../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-resource-management.md).

### 작업 로드 밸런서에서 할당을 보다 간편하게 업데이트하는 방법 {#a-more-convenient-way-to-update-allocations-in-the-workload-balancer}

이제 작업 로드 밸런서에서 작업 항목에 대한 사용자의 할당을 보다 간편하게 관리할 수 있도록 작업 항목을 두 번 클릭할 수 있습니다. 기존 할당 편집 메뉴 옵션을 사용할 수도 있습니다. 또한 더 이상 할당을 업데이트하기 위해 할당을 표시할 필요가 없습니다.

작업 로드 밸런서에서 할당 관리에 대한 자세한 내용은 [작업 로드 밸런서에서 사용자 할당 관리](../../../resource-mgmt/workload-balancer/manage-user-allocations-workload-balancer.md).
