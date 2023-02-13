---
title: 22.4 리소스 관리 개선 사항
description: 22.4 리소스 관리 개선 사항
author: Luke
draft: Probably
feature: Product Announcements
exl-id: cd026fc9-e3be-4cff-8d85-4f50fae9dd77
source-git-commit: 87d0b668185c4185646bfa1622eb37337844bcbc
workflow-type: tm+mt
source-wordcount: '415'
ht-degree: 0%

---

# 22.4 리소스 관리 개선 사항

이 페이지에서는 미리 보기 환경에 대한 22.4 릴리스로 향상된 리소스 관리 기능에 대해 설명합니다. 이러한 개선 사항은 2022년 10월 3일이 있는 주에 제공될 예정입니다.

22.4 릴리스에서 사용할 수 있는 모든 변경 사항 목록에 대해서는 다음을 참조하십시오 [22.4 릴리스 개요](/help/quicksilver/product-announcements/product-releases/22.4-release-activity/22-4-release-overview.md).

## 프로젝트의 작업 로드 밸런서에 대한 모든 사용자 표시

프로젝트의 작업 로드 밸런서를 종료하지 않고 시스템의 모든 사용자 및 해당 용량을 표시할 수 있도록 &quot;모든 사용자 표시&quot; 옵션을 추가했습니다. 이 옵션이 활성화되면 프로젝트의 작업 로드 밸런서에는 지정된 작업 영역에 시스템의 모든 사용자가 표시됩니다. 이러한 개선 사항을 통해 미지정 작업 영역에 나열된 작업에 할당해야 하는 사용자를 쉽게 식별할 수 있습니다.

자세한 내용은 [드래그 앤 드롭으로 작업 로드 밸런서에서 작업 할당](/help/quicksilver/resource-mgmt/workload-balancer/assign-work-in-workload-balancer-by-drag-and-drop.md).

[이 기능에 대한 비디오 데모 보기](https://video.tv.adobe.com/v/3412873/){target=_blank}

## 작업을 일괄 할당할 때 작업 부하 분산 장치에 선택된 작업 역할이 있는 모든 사용자 표시

작업 역할을 일괄 작업 밸런서의 사용자로 대체할 때 적합한 사용자를 보다 쉽게 찾을 수 있도록 사용 가능한 사용자 목록이 채워지는 방식을 개선했습니다. 이제 동일한 사용자 목록에서 두 개의 개별 영역에서 선택한 역할을 수행할 수 있는 시스템의 모든 사용자를 볼 수 있습니다.

* 첫 번째 영역(제안된 지정)에는 Smart Assignments 논리로 식별된 사용자가 표시됩니다. 자세한 내용은 [스마트 할당 개요](/help/quicksilver/manage-work/tasks/assign-tasks/smart-assignments.md).

* 두 번째 영역(기타 지정)에는 선택한 역할을 이행할 수 있는 모든 사용자가 표시됩니다.

이 개선 사항 전에 Smart Assignments 로직에 따라 할당할 수 있는 사용자 목록만 볼 수 있습니다.

작업 로드 밸런서를 사용하여 작업을 일괄 지정하는 방법에 대한 자세한 내용은 [작업 로드 밸런서를 사용하여 일괄 작업 할당](/help/quicksilver/resource-mgmt/workload-balancer/assign-work-in-workload-balancer-in-bulk.md).

[이 기능에 대한 비디오 데모 보기](https://video.tv.adobe.com/v/3412874/){target=_blank}

## 작업 라이선스 사용자 및 문제 설정을 위한 작업 로드 밸런서 개선 사항

예약 도구의 사용 중단을 준비하기 위해 다음 개선 사항이 작업 로드 밸런서에 추가되었습니다.

* 이제 작업 라이선스 사용자는 프로젝트의 작업 로드 밸런서를 사용할 때 할당을 조정할 수 있습니다

* &quot;문제 발생 시간 포함&quot; 설정을 활성화하면 미지정 작업 영역에 문제가 표시됩니다

이러한 개선 사항 전에 Plan-license 사용자만 지정된 작업 영역에만 표시되는 사용자 할당 및 문제를 조정할 수 있습니다.

자세한 내용은 다음 문서를 참조하십시오.

* [작업 로드 밸런서 탐색](/help/quicksilver/resource-mgmt/workload-balancer/navigate-the-workload-balancer.md).

* [작업 로드 밸런서에서 사용자 할당 관리](/help/quicksilver/resource-mgmt/workload-balancer/manage-user-allocations-workload-balancer.md).

예약의 사용 중단에 대한 자세한 내용은 [Adobe Workfront의 리소스 예약 도구 사용 중단](/help/quicksilver/resource-mgmt/resource-mgmt-overview/deprecate-resource-scheduling.md).
