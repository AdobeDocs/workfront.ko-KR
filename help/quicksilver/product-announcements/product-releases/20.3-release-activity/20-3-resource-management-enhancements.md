---
content-type: release-notes
navigation-topic: 2020-3-release-activity
title: 20.3 향상된 리소스 관리 기능
description: 이 페이지에서는 프로덕션 환경에 대한 20.3 릴리스의 모든 리소스 관리 개선 사항에 대해 설명합니다. 이러한 개선 사항은 2020년 8월 10일 주에 프로덕션 환경에서 사용할 수 있습니다.
author: Luke
feature: Product Announcements
recommendations: noDisplay, noCatalog
exl-id: a2c34117-e03c-4394-9b81-7c18433531d1
source-git-commit: f1e463c90641f9221228e335b583cab72762b3bd
workflow-type: tm+mt
source-wordcount: '837'
ht-degree: 0%

---

# 20.3 향상된 리소스 관리 기능

이 페이지에서는 프로덕션 환경에 대한 20.3 릴리스의 모든 리소스 관리 개선 사항에 대해 설명합니다. 이러한 개선 사항은 2020년 8월 10일 주에 프로덕션 환경에서 사용할 수 있습니다.

20.3 릴리스에서 사용할 수 있는 모든 변경 사항의 목록은 을 참조하십시오. [20.3 릴리스 개요](../../../product-announcements/product-releases/20.3-release-activity/20-3-release-overview.md).

## 업무 균형자의 할당된 작업 영역에 문제의 시간 포함

사용자의 모든 워크로드에 대한 전체 그림을 볼 수 있도록 업무 균형자의 할당된 작업 영역에 문제의 시간을 포함할 수 있는 설정을 도입했습니다.

업무 균형자 작업에 대한 자세한 내용은 [업무 균형자 탐색](../../../resource-mgmt/workload-balancer/navigate-the-workload-balancer.md).

## 업무 균형자에서 비근무일에 대한 할당 조정

업무 균형자 를 사용하여 휴무일에 대한 리소스 할당을 조정할 수 있습니다.

업무 균형자에서 할당을 관리하는 방법에 대한 자세한 내용은 [업무 균형자에서 사용자 할당 관리](../../../resource-mgmt/workload-balancer/manage-user-allocations-workload-balancer.md).

## 업무 균형자에서 사용할 수 있는 변수 필터

사용자 경험을 개선하고 정보를 공유할 때 더 많은 유연성을 제공하기 위해 이제 업무 균형자에 대한 변수 필터가 구현되었습니다. 다음 필터가 업무 균형자에 추가되었습니다.

* &quot;내&quot;(사용자별로 필터링할 때)
* &quot;내 기본 역할&quot;(역할별로 필터링할 때)
* &quot;내 홈 팀&quot; 또는 &quot;모든 내 팀&quot;(팀별로 필터링할 때).

이러한 필터는 $$USER.ID, $$USER.roleID, $$USER.homeTeamID 및 $$USER.teamIDs의 와일드카드 필터 변수를 대체합니다

이러한 필터 중 하나를 적용한 다음 업무 균형자 를 공유하거나 대시보드에 배치하면 다른 모든 사용자에게 자체 정보가 표시됩니다.

업무 균형자에 필터를 적용하는 방법에 대한 자세한 내용은 [업무 균형자에서 정보 필터링](../../../resource-mgmt/workload-balancer/filter-information-workload-balancer.md).

## 업무 균형자에서 프로젝트에 대한 새 정렬

이제 업무 균형자에서 사용자가 화면에 표시하는 시간 동안 발생하는 프로젝트의 작업 중 가장 빠른 계획된 시작 일자와 두 번째 가장 늦은 계획된 완료 일자를 기준으로 프로젝트를 정렬합니다. 이를 통해 하루 동안의 작업을 보다 쉽게 식별할 수 있도록 작업을 트리와 같은 계층으로 구성할 수 있습니다.

업무 균형자에서 프로젝트 및 작업 항목을 보는 방법에 대한 자세한 내용은 [업무 균형자 탐색](../../../resource-mgmt/workload-balancer/navigate-the-workload-balancer.md).

## 업무 균형자에 실제 작업 진행 상황 표시

작업 로드 진행 상황을 정확하게 파악할 수 있도록 업무 균형자에 예상 날짜에 따라 작업 및 문제의 타임라인을 표시하는 새로운 설정을 도입했습니다. 예상 일자 표시 설정을 사용하여 계획된 타임라인 외에 작업 항목의 예상 타임라인을 볼 수 있습니다.

또한 이 개선 작업으로 작업 또는 문제가 계획된 완료 일자보다 일찍 완료되면 남은 일수에서 할당된 시간이 취소되어 사용자의 전체 할당에 계산되지 않음을 나타냅니다.

업무 균형자 탐색 및 설정 활성화에 대한 자세한 내용은 다음을 참조하십시오. [업무 균형자 탐색](../../../resource-mgmt/workload-balancer/navigate-the-workload-balancer.md).

## 이전에 20.2 릴리스와 함께 릴리스될 때 통신한 업무 균형자 기능

* [업무 균형자에서 일별 및 주별 할당 조정](#adjust-daily-and-weekly-allocation-in-the-workload-balancer)
* [업무 균형자에서 작업 계획 시간 업데이트](#update-task-planned-hours-in-the-workload-balancer)
* [업무 균형자에서 할당을 보다 편리하게 업데이트할 수 있는 방법](#a-more-convenient-way-to-update-allocations-in-the-workload-balancer)

### 업무 균형자에서 일별 및 주별 할당 조정 {#adjust-daily-and-weekly-allocation-in-the-workload-balancer}

이제 리소스가 소진되지 않도록 업무 균형자를 사용하여 작업할 사용자의 일별 및 주별 할당을 조정할 수 있습니다.

이 기능이 향상되기 전에는 리소스 예약 도구를 사용해야 이 작업을 수행할 수 있었습니다.

업무 균형자에서 할당을 관리하는 방법에 대한 자세한 내용은 [업무 균형자에서 사용자 할당 관리](../../../resource-mgmt/workload-balancer/manage-user-allocations-workload-balancer.md).

**다음 환경에서 사용할 수 있습니다.**

* Adobe Workfront 클래식
* 새로운 Adobe Workfront 환경

### 업무 균형자에서 작업 계획 시간 업데이트 {#update-task-planned-hours-in-the-workload-balancer}

>[!NOTE]
>
>이 개선 사항은 2020.2 릴리스 직후 프로덕션에서 사용할 수 있습니다.

이제 액세스 수준의 리소스 관리 영역에 있는 새 옵션을 사용하여 이 액세스 권한이 있는 사용자가 업무 균형자에서 계획된 시간을 편집할 수 있습니다. 업무 균형자에서 할당을 조정할 때 일일 할당의 합계는 작업의 계획된 시간 수와 일치하지 않아도 됩니다. 할당을 저장하면 총 할당 시간이 작업의 계획된 시간이 됩니다. 단순 기간 유형이 있는 작업에만 가능합니다.

업무 균형자에서 할당을 관리하는 방법에 대한 자세한 내용은 [업무 균형자에서 사용자 할당 관리](../../../resource-mgmt/workload-balancer/manage-user-allocations-workload-balancer.md).

리소스 관리에 대한 액세스 권한 부여에 대한 자세한 내용은 [리소스 관리에 대한 액세스 권한 부여](../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-resource-management.md).

### 업무 균형자에서 할당을 보다 편리하게 업데이트할 수 있는 방법 {#a-more-convenient-way-to-update-allocations-in-the-workload-balancer}

업무 균형자에서 작업 항목에 대한 사용자의 할당을 보다 편리하게 관리하려면 이제 작업 항목을 두 번 클릭합니다. 기존 할당 편집 메뉴 옵션을 계속 사용할 수도 있습니다. 또한 할당을 업데이트하기 위해 더 이상 할당 표시를 활성화할 필요가 없습니다.

업무 균형자에서 할당을 관리하는 방법에 대한 자세한 내용은 [업무 균형자에서 사용자 할당 관리](../../../resource-mgmt/workload-balancer/manage-user-allocations-workload-balancer.md).
