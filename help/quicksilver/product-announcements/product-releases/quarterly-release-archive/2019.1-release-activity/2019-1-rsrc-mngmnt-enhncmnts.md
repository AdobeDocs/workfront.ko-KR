---
content-type: release-notes
navigation-topic: 2019-1-release-activity
title: 2019.1 리소스 관리 개선 사항
description: 이 페이지에서는 2019.1 릴리스에 포함된 모든 리소스 관리 개선 사항에 대해 설명합니다. 이제 프로덕션 환경에서 기능을 사용할 수 있습니다.
author: Luke
feature: Product Announcements
recommendations: noDisplay, noCatalog
exl-id: 6eed6023-96cc-45d7-8dae-a36d45e92068
source-git-commit: f1e463c90641f9221228e335b583cab72762b3bd
workflow-type: tm+mt
source-wordcount: '953'
ht-degree: 0%

---

# 2019.1 리소스 관리 개선 사항

이 페이지에서는 2019.1 릴리스에 포함된 모든 리소스 관리 개선 사항에 대해 설명합니다. 이제 프로덕션 환경에서 기능을 사용할 수 있습니다.

2019.1의 모든 변경 사항 목록은 을 참조하십시오. [2019.1 릴리스 활동 개요](../../../../product-announcements/product-releases/quarterly-release-archive/2019.1-release-activity/2019-1-release-activity-overview.md).

## 리소스 플래너의 기본 필터가 업데이트되었습니다.

리소스 플래너의 기본 필터가 더 이상 프로젝트 그룹별로 필터링되지 않습니다.

이제 리소스 플래너를 볼 때 기본적으로 현재 및 날짜에 민감한 프로젝트만 표시됩니다. 기본적으로 다음 프로젝트의 정보가 포함됩니다.

* 오늘 달의 첫 번째 날짜 이후에 발생하는 계획된 완료 일자와 함께.
* 오늘부터 4번째 달의 마지막 날짜 이전에 발생하는 계획된 시작 일자입니다.
* 현재 또는 계획 상태

이전에는 기본 필터가 다음 추가 프로젝트에서 정보를 검색했습니다.

* 오늘 달의 첫 번째 날짜 이후에 발생하는 계획된 완료 일자와 함께.
* 오늘부터 4번째 달의 마지막 날짜 이전에 발생하는 계획된 시작 일자입니다.
* 현재 또는 계획 상태
* 로그인한 사용자의 홈 그룹과 일치하는 그룹 포함.

리소스 플래너에 필터를 적용하는 방법에 대한 자세한 내용은 [리소스 플래너에서 정보 필터링](../../../../resource-mgmt/resource-planning/filter-resource-planner.md).

## 리소스 플래너 필터에 와일드카드 사용

이제 리소스 플래너에서 필터를 작성할 때 와일드카드를 사용할 수 있습니다. 예를 들어 $$USER.ID를 사용하여 로그인한 사용자에 대한 정보를 필터링하거나 $$USER.companyID를 사용하여 로그인한 사용자와 동일한 회사에 속하는 모든 사용자에 대한 정보를 필터링할 수 있습니다. 사용자 기반 변수의 전체 목록을 보려면 [사용자 기반 와일드카드 필터 변수](../../../../reports-and-dashboards/reports/reporting-elements/understand-wildcard-filter-variables.md#user-based-variables) 의 섹션 [와일드카드 필터 변수](../../../../reports-and-dashboards/reports/reporting-elements/understand-wildcard-filter-variables.md).

이전에는 리소스 플래너 필터에 와일드카드를 사용할 수 없었습니다.

리소스 플래너에서의 필터링에 대한 자세한 내용은 [리소스 플래너에서 정보 필터링](../../../../resource-mgmt/resource-planning/filter-resource-planner.md).

<!--
<iframe class="mt-media" src="assets/290697527?title=0&byline=0&portrait=0" width="640px" height="360px" frameborder="0" allowfullscreen></iframe>
-->

## 리소스 플래너에서 날짜 기반 와일드카드 필터 변수 지원

이제 리소스 플래너에서 필터를 작성할 때 $$TODAY 와일드카드 필터 변수의 모든 버전을 사용할 수 있습니다.

이 개선 이전에는 사용자 기반 와일드카드 필터 변수만 사용할 수 있었습니다.

리소스 플래너에서의 필터링에 대한 자세한 내용은 [리소스 플래너에서 정보 필터링](../../../../resource-mgmt/resource-planning/filter-resource-planner.md).

와일드카드 필터 변수에 대한 자세한 내용은 [와일드카드 필터 변수](../../../../reports-and-dashboards/reports/reporting-elements/understand-wildcard-filter-variables.md).

## 리소스 플래너의 역할 보기에 대한 내보내기 옵션

이제 역할 보기의 리소스 플래너에서 내보낼 정보 수준을 선택할 수 있습니다. 다음 중 하나를 내보낼 수 있습니다.

* 역할만
* 역할 및 프로젝트
* 역할, 프로젝트 및 사용자

이 개선 이전에는 역할 보기에서 모든 수준의 정보를 내보냈습니다. 이러한 옵션은 이전 릴리스의 프로젝트 및 사용자 보기에 도입되었습니다.

리소스 플래너에서 정보를 내보내는 방법에 대한 자세한 내용은 [리소스 플래너에서 정보 내보내기](../../../../resource-mgmt/resource-planning/export-resource-planner.md).

## 리소스 플래너 내보내기를 위한 데이터 서식 옵션

이제 리소스 플래너에서 내보낼 때 Excel 파일에 정보를 표시하는 방법을 선택할 수 있습니다.

리소스 플래너에서 내보낸 정보의 가용성과 할당을 다음과 같은 방법으로 표시할 수 있습니다.

* 해당 개체가 속한 개체의 이름으로 그룹화되지 않았습니다. 이 경우 각 데이터 행에 해당 객체가 속한 객체 이름이 표시됩니다. (기본 옵션입니다)
* 해당 개체가 속한 개체의 이름으로 그룹화됩니다. 이 경우 내보낸 파일의 정보는 Workfront에 표시된 대로 나타납니다.

이 기능이 향상되기 전에는 내보낸 파일의 정보가 Workfront에 나타나는 것처럼 표시되었습니다.

리소스 플래너에서 정보를 내보내는 방법에 대한 자세한 내용은 [리소스 플래너에서 정보 내보내기](../../../../resource-mgmt/resource-planning/export-resource-planner.md).

## 지속 예약 타임라인

>[!NOTE]
>
>리소스 예약 도구는 23.1 릴리스에서 더 이상 사용되지 않으며 Workfront에서 제거되었습니다. 업무 균형자 를 사용하여 리소스를 예약하는 방법에 대한 자세한 내용은 [업무 균형자 개요](../../../../resource-mgmt/workload-balancer/overview-workload-balancer.md).

이제 타임라인을 예약하면 타임라인을 새로 고치거나 페이지에서 멀리 이동할 때 선택한 타임프레임이 유지됩니다.

이 개선 이전에는 페이지를 새로 고치거나 페이지에서 멀리 탐색할 때 예약 타임라인이 기본 시간대로 반환되었습니다.

이 개선 사항은 다음 영역에서 사용할 수 있습니다.

* 사람 영역의 예약 탭
* 탭에서 작업 중인 팀
* 프로젝트의 스태핑 탭에 있는 스케줄링 하위 탭

리소스 예약 영역에서 타임라인 작업에 대한 자세한 내용은 &quot;리소스 예약 시작&quot;을 참조하십시오.

## 리소스 플래너의 새 내보내기 옵션

이제 리소스 플래너에서 내보낼 정보 수준을 선택할 수 있습니다. 프로젝트 보기에서 다음 중 하나를 내보낼 수 있습니다.

* 프로젝트만
* 프로젝트 및 역할
* 프로젝트, 역할 및 사용자

사용자 보기에서 다음 중 하나를 내보낼 수 있습니다.

* 사용자만
* 사용자 및 프로젝트
* 사용자, 프로젝트, 역할, 작업 및 문제

이 개선 이전에는 기본적으로 리소스 플래너의 모든 보기에서 모든 수준의 정보를 내보냈습니다.

리소스 플래너에서 정보를 내보내는 방법에 대한 자세한 내용은 [리소스 플래너에서 정보 내보내기](../../../../resource-mgmt/resource-planning/export-resource-planner.md).

## 리소스 플래너에서 사용자 보기 업데이트

이제 시스템의 모든 사용자가 리소스 플래너의 사용자 보기에 표시되지만, 필터링된 프로젝트와 연결된 사용자만 시간 정보를 표시합니다.

이 업데이트 이전에는 필터링하는 프로젝트의 작업 항목에 할당된 사용자만 리소스 플래너의 사용자 보기에 표시됩니다.

사용자 기반 필터를 사용하여 사용자 보기에 표시되는 사용자 수를 표시하려는 프로젝트에 할당된 사용자만 줄일 수 있습니다.

리소스 플래너의 필터에 대한 자세한 내용은 [리소스 플래너에서 정보 필터링](../../../../resource-mgmt/resource-planning/filter-resource-planner.md).
