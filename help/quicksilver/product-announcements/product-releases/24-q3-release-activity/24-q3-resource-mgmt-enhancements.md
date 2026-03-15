---
title: 2024년 3분기 리소스 관리 개선 사항
description: 2024년 3분기 리소스 관리 개선 사항
author: Courtney
feature: Product Announcements
recommendations: noDisplay, noCatalog
exl-id: 40ca0460-5a01-4df9-b3dc-72055a272072
source-git-commit: 6a6d3d47ed5741e3202c44b7240a2e67b687ea95
workflow-type: tm+mt
source-wordcount: '181'
ht-degree: 0%

---

# 2024년 3분기 리소스 관리 개선 사항

이 페이지에서는 미리보기 환경에 대한 2024년 3분기 릴리스의 모든 리소스 관리 개선 사항에 대해 설명합니다. 이러한 개선 사항은 2024년 3분기 릴리스를 통해 프로덕션 환경에서 사용할 수 있습니다.

2024년 3분기 릴리스 주기에 있는 이 시점에서 사용 가능한 모든 변경 내용의 목록은 [2024년 3분기 릴리스 개요](/help/quicksilver/product-announcements/product-releases/24-q3-release-activity/24-q3-release-overview.md)를 참조하십시오.

## 이제 작업 로드 밸런서에 시간이 반영됨

>[!NOTE]
>
>미리 보기 릴리스: 2024년 6월 6일, 모든 고객을 위한 프로덕션 릴리스: 24.7 릴리스 포함(2024년 7월 18일)

작업 로드 밸런서는 작업의 1차 피할당자가 휴식 시간을 예약한 경우 작업을 원활하게 조정하기 위해 이제 프로젝트 타임라인이 다시 계산될 때 1차 사용자와 2차 사용자 모두에게 시간을 재할당합니다. (이 기능은 Workfront 관리자가 사용자의 사용 중지 시간을 고려하여 설정 영역에서 사용 중지 설정을 활성화한 경우에만 사용할 수 있습니다.)

이전에는 타임라인이 다시 계산될 때 시간이 다시 할당되지 않았습니다.

자세한 내용은 [작업 부하 분산 장치에서 사용자 할당 관리](/help/quicksilver/resource-mgmt/workload-balancer/manage-user-allocations-workload-balancer.md)를 참조하십시오.
