---
title: 22.2 향상된 리소스 관리 기능
description: 22.2 향상된 리소스 관리 기능
author: Luke
draft: Probably
feature: Product Announcements
recommendations: noDisplay, noCatalog
exl-id: 5f11c43c-3aa8-4135-b6bf-07b9993e63d9
source-git-commit: 76deb76c66e8f8a7dea721378591ae035b8d42e7
workflow-type: tm+mt
source-wordcount: '373'
ht-degree: 0%

---

# 22.2 향상된 리소스 관리 기능

이 페이지에서는 미리보기 환경에 대한 22.2 릴리스의 모든 리소스 관리 개선 사항에 대해 설명합니다. 이러한 개선 사항은 프로덕션 환경에서 사용할 수 있습니다

<!--
<MadCap:conditionalText data-mc-conditions="QuicksilverOrClassic.Draft mode">
in January 2022
</MadCap:conditionalText>
-->

2022년 4월 4일이 있는 주

22.2 릴리스에서 사용할 수 있는 모든 변경 사항 목록을 보려면 [22.2 릴리스 개요](../../../product-announcements/product-releases/22.2-release-activity/22-2-release-overview.md)를 참조하십시오.

## 업무 균형자 탐색 개선

업무 균형자 를 사용할 때의 경험을 개선하기 위해 다음과 같은 개선 사항이 도입되었습니다.

* 할당을 조정할 때 취소 및 저장 단추는 작업이 화면에 포함된 시간보다 길거나 요약 패널이 표시되는 경우에도 이제 고정됩니다.
* 이제 사용자 및 작업 항목의 이름을 표시하는 왼쪽 패널이 고정되므로 더 긴 기간 동안 가로로 스크롤하고 패널에 나열된 항목 이름을 계속 읽을 수 있습니다.
* 사용자 또는 프로젝트 수준이 아닌 한 번의 클릭으로 왼쪽 패널에 나열된 모든 항목을 축소하고 확장할 수 있습니다.
* 이제 왼쪽 패널의 크기도 조정할 수 있습니다.
* 이제 업무 균형자에 대한 전체 화면 모드가 있습니다.

업무 균형자 탐색에 대한 자세한 내용은 [업무 균형자 탐색](../../../resource-mgmt/workload-balancer/navigate-the-workload-balancer.md)을 참조하십시오.

## 업무 균형자에서 고급 할당에 액세스

이제 작업 항목을 보다 쉽고 정확하게 할당할 수 있도록 업무 균형자에서 작업 항목을 수동으로 할당할 때 고급 할당을 수행할 수 있습니다. 이 개선 전에는 항목 헤더 또는 목록에서 항목을 편집할 때 고급 할당에 액세스할 수 있었습니다.

자세한 내용은 [업무 균형자를 사용하여 수동으로 작업 할당](../../../resource-mgmt/workload-balancer/assign-work-in-workload-balancer-manually.md)을 참조하십시오.

## 기본 일정 기본 설정을 선택한 경우 사용자 가용성을 계산하는 새 공식

리소스 관리 도구에 대한 보다 정확한 정보를 제공하기 위해 Workfront 관리자가 리소스 관리 환경 설정에서 기본 일정을 선택할 때 Workfront이 사용자 가용성을 계산하는 데 사용하는 공식을 변경했습니다. 새 업데이트를 통해 Workfront은 다음 공식을 사용하여 사용자 가용성을 계산합니다.

사용자 사용 가능 시간 = (기본 예약 시간 - 예외) &#42; FTE - 휴무 시간

이 업데이트 이전에는 기본 일정이 선택되었을 때 Workfront에서 다음 공식을 사용하여 사용자 가용성을 계산했습니다.

사용자 사용 가능 시간 = (기본 일정 시간 - (일정 예외 + 휴무 시간)) &#42; 사용자 FTE 값

자세한 내용은 [리소스 관리 환경 설정 구성](../../../administration-and-setup/set-up-workfront/configure-system-defaults/configure-resource-mgmt-preferences.md)을 참조하십시오.

