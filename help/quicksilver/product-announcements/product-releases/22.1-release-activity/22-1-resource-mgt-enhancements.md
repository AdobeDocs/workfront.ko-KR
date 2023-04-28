---
title: 22.1 리소스 관리 개선 사항
description: 22.1 리소스 관리 개선 사항
author: Luke
draft: Probably
feature: Product Announcements
exl-id: 513e0831-5571-4432-ade3-4f11b7e97266
source-git-commit: e0a8093be33773a8b801567cfbe90f67701f9ff3
workflow-type: tm+mt
source-wordcount: '367'
ht-degree: 0%

---

# 22.1 리소스 관리 개선 사항

이 페이지에서는 미리 보기 환경에 대한 22.1 릴리스로 향상된 리소스 관리 기능에 대해 설명합니다. 이러한 개선 사항은 프로덕션 환경에서 사용할 수 있습니다

<!--
<MadCap:conditionalText data-mc-conditions="QuicksilverOrClassic.Draft mode">
in January 2022
</MadCap:conditionalText>
-->

2022년 1월 17일이 있는 주.

22.1 릴리스에서 사용할 수 있는 모든 변경 사항 목록에 대해서는 다음을 참조하십시오 [22.1 릴리스 개요](../../../product-announcements/product-releases/22.1-release-activity/22-1-release-overview.md).

## 설정 패널 및 작업 로드 밸런서에서 프로젝트 및 해당 작업의 색상 코드 조정 기능이 개선되었습니다

작업 로드 밸런서를 사용할 때 경험을 향상시키기 위해 다음과 같은 개선 사항이 도입되었습니다.

* 이전에 도구 모음에 있었던 옵션을 포함하도록 설정 패널을 다시 디자인했습니다. 이렇게 하면 도구 모음의 공간 사용이 개선됩니다.
* 프로젝트별로 색상 테마를 사용자 지정하는 기능을 추가했습니다. [프로젝트]로 색상 코드 지정을 선택하면 각 프로젝트 및 해당 작업 항목이 동일한 색상으로 표시됩니다. 각 프로젝트마다 색상이 고유합니다. 이 개선 사항 전에는 프로젝트 상태로만 색상 코드를 만들 수 있습니다.

자세한 내용은 [작업 로드 밸런서 탐색](../../../resource-mgmt/workload-balancer/navigate-the-workload-balancer.md).

## 작업 로드 밸런서를 사용하여 일괄 작업 할당

스케줄링 도구를 사용하지 않고 작업 로드 밸런서로 대체하기 위한 노력을 계속 수행하면서, Adobe는 일괄 관리를 위한 기능을 추가했습니다. 이제 여러 사용자에게 한 번에 여러 작업 항목을 할당하고, 여러 작업 항목의 사용자를 다른 사용자로 대체하고, 여러 항목에서 사용자 할당을 한 번에 취소할 수 있습니다. 작업 로드 밸런서에서 새 일괄 지정 기능을 사용하여 이러한 작업을 하나의 작업으로 수행할 수 있습니다.

이 개선 사항 전에 수동으로 또는 드래그 앤 드롭으로 한 명의 사용자만 작업 항목에 할당할 수 있습니다.

새 벌크 지정에는 이름 외에 프로젝트 및 태스크 상태별 새 필터링 기능도 포함됩니다.

자세한 내용은 [작업 로드 밸런서에서 작업 할당 개요](../../../resource-mgmt/workload-balancer/assign-work-in-workload-balancer.md).

## 작업 역할을 관리할 때 통화 대체

글로벌 조직 전체의 비용 및 청구 비율을 쉽게 관리할 수 있도록 Adobe에서는 Job 역할의 통화를 재정의하는 것을 구현했습니다. 이제 이 기능을 사용하여 작업 역할의 위치와 일치하는 통화로 작업 역할에 대한 비용 및 청구 비율을 설정할 수 있습니다. 이 경우 작업 역할에 대한 모든 재무 계산에서 시스템 통화가 대체됩니다.

자세한 내용은 [작업 역할 만들기 및 관리](../../../administration-and-setup/set-up-workfront/organizational-setup/create-manage-job-roles.md).

