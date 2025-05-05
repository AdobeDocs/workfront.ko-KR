---
content-type: release-notes
navigation-topic: product-releases-archive
title: 2017.3 Beta 4 릴리스 활동
description: 이 페이지에서는 2017.3 Beta 4 릴리스의 미리보기 환경에서 가장 최근에 사용할 수 있는 모든 변경 사항에 대해 설명합니다. 이 페이지의 기능은 2017년 9월 25일이 있는 주에 미리보기 환경에서 사용할 수 있습니다. 프로덕션 환경에서는 2017년 11월 초에 제공될 예정입니다.
author: Luke
feature: Product Announcements
recommendations: noDisplay, noCatalog
exl-id: d6bb889c-a057-453f-8f80-761cfb1ad4a1
source-git-commit: 6405c01c8b1d842a4175f9caa18a7ed31316a3a1
workflow-type: tm+mt
source-wordcount: '1676'
ht-degree: 0%

---

# 2017.3 Beta 4 릴리스 활동

이 페이지에서는 2017.3 Beta 4 릴리스의 미리보기 환경에서 가장 최근에 사용할 수 있는 모든 변경 사항에 대해 설명합니다. 이 페이지의 기능은 2017년 9월 25일이 있는 주에 미리보기 환경에서 사용할 수 있습니다. 프로덕션 환경에서는 2017년 11월 초에 제공될 예정입니다.

>[!IMPORTANT]
>
> 이 페이지에 설명된 기능은 프로덕션 환경에서 사용하기 전에 변경될 수 있습니다.

2017.3의 모든 변경 사항 목록은 다음을 참조하십시오.  [2017.3 릴리스 활동 개요](../../../../product-announcements/product-releases/quarterly-release-archive/2017.3-release-activity/2017-3-release-activity-overview.md).

2017.3 Beta 4 릴리스에는 Workfront 관리자와 기타 사용자 모두를 위한 개선 사항이 포함되어 있습니다.

관리자용 **1&rbrace;**

* [설정 영역의 새 리소스 관리 기본 설정 영역](#new-resource-management-preferences-area-in-the-setup-area)

**모든 사용자용**

* [중복 작업](#duplicate-tasks)
* [리소스를 예약할 때 할당 자동화](#automate-assignments-when-scheduling-resources)
* [리소스를 예약할 때 여러 작업에 대한 할당 수정](#modify-assignments-for-multiple-tasks-when-scheduling-resources)
* [리소스 플래너에 FTE 배포 적용](#apply-fte-distribution-to-the-resource-planner)
* [사용자 설정에 대한 작업 역할 섹션에 FTE 사용 가능 비율이 포함됨](#job-role-section-for-user-settings-includes-percentage-of-fte-availability)
* [프로젝트의 사용률 보고서에 필터 저장 및 관리](#save-and-manage-filters-in-the-utilization-report-on-a-project)
* [사용률 보고서의 추가 필터링 옵션](#additional-filtering-options-in-the-utilization-report)
* [프로그램 또는 Portfolio의 사용률 보고서 보기](#view-the-utilization-report-by-program-or-portfolio)
* [프로젝트 및 작업 보고서에 원본 문제 정보 표시](#show-original-issue-information-in-project-and-task-reports)
* [업데이트 스트림의 필터 시스템 업데이트가 이제 개체 간에 지속됩니다](#filter-system-updates-in-the-update-stream-is-now-persistent-across-objects)
* [Workfront 내의 활성 증명 단계에 대해 보고](#report-on-active-proof-stages-within-workfront)
* [Workfront 내의 사용자에게 사용자 지정 Workfront Proof 권한 프로필 할당](#assign-custom-workfront-proof-permission-profiles-to-users-within-workfront)
* [이벤트 구독에 시간 리소스 추가됨](#hour-resource-added-to-event-subscriptions)

## 작업 복제 {#duplicate-tasks}

이제 프로젝트 내에서 작업 또는 작업 세트를 빠르게 복제할 수 있습니다. 이 작업은 원래 작업과 동일한 작업을 만듭니다. 복제 프로세스 중에는 새로 만든 작업을 변경할 수 있는 추가 옵션이 없습니다.  

이 변경 전에 작업을 새 프로젝트 또는 기존 프로젝트에 복사하고 복사할 때 일부 정보를 수정할 수 있습니다.

대상  작업 복제에 대한 자세한 내용은 [작업 복사 및 복제](../../../../manage-work/tasks/manage-tasks/copy-and-duplicate-tasks.md)를 참조하세요.

## 자원 스케줄링 시 할당 자동화 {#automate-assignments-when-scheduling-resources}

>[!NOTE]
>
>리소스 예약 도구는 23.1 릴리스에서 더 이상 사용되지 않으며 Workfront에서 제거되었습니다. 업무 균형자를 사용하여 리소스를 예약하는 방법에 대한 자세한 내용은 [업무 균형자 개요](../../../../resource-mgmt/workload-balancer/overview-workload-balancer.md)를 참조하십시오.

이제 Workfront에서 여러 프로젝트에 대한 자원을 스케줄링할 때(스케줄링 탭에서) 또는 단일 프로젝트에 대한 자원을 스케줄링할 때(스태핑 탭에서) 미할당 작업 및 문제에 대한 할당을 자동으로 제안하도록 허용할 수 있습니다.

Workfront은 사용 가능한 사용자 간 현재 작업 할당을 분석하고 아직 할당되지 않은 작업 또는 문제에 대한 지능적이고 논리적인 할당을 제안합니다. 발령을 완료하기 전에 제안된 발령 또는 기존 발령을 수정할 수 있습니다.

자세한 내용은 &quot;예약 영역에서 미할당 작업 및 문제 수동 할당&quot;을 참조하십시오.

## 자원을 예약할 때 여러 작업에 대한 할당 수정 {#modify-assignments-for-multiple-tasks-when-scheduling-resources}

이제 예약 탭 또는 직원 탭에서 리소스를 예약할 때 사용자를 일괄 할당, 대체 또는 할당 해제할 때 하나 이상의 프로젝트에서 지정한 특정 작업(모든 하위 작업 및 관련 문제 포함)에 대한 할당을 수정할 수 있습니다.

이 변경 이전에는 전체 프로젝트에 대해서만 작업 및 문제에 대한 할당을 수정할 수 있었습니다(프로젝트 내에서 특정 작업을 지정할 수 없음).

자세한 내용은 &quot;예약 영역에서 미할당 작업 및 문제 수동 할당&quot;을 참조하십시오.

## 리소스 플래너에 FTE 배포 적용 {#apply-fte-distribution-to-the-resource-planner}

>[!NOTE]
>
>이 기능은 현재 모든 클러스터의 미리보기에서 사용할 수 없습니다.

이제 사용자가 둘 이상의 역할을 가지고 있는 경우 각 역할에 대한 FTE 가용성 백분율을 기준으로 사용자의 각 역할에 대한 올바른 사용 가능 시간을 표시할 수 있습니다.

예를 들어, 사용자의 일정에 따라 한 달에 100시간 동안 작업할 수 있다고 표시되고 기본 역할에 대한 FTE 가용성 비율이 75%이고 다른 역할에 대한 FTE 가용성 비율이 25%인 경우 리소스 플래너는 사용자를 기본 역할에 75시간 사용 가능하고 다른 역할에 25시간 사용 가능으로 나열합니다.

이 변경 이전에는 기본 역할에 대해서만 리소스 플래너에 표시되는 사용자의 이름과 일정(100시간)에 따른 사용자의 전체 가용성이 기본 역할에만 연결되었습니다. 사용자가 해당 역할의 작업에 할당되고 다른 역할의 사용자에 대한 사용 가능한 시간이 0인 경우에만 리소스 플래너에 표시되는 사용자의 다른 역할.

리소스 플래너의 사용자 및 역할에 대해 사용 가능한 시간 및 사용 가능한 FTE를 계산하는 방법에 대한 자세한 내용은 [리소스 플래너의 사용자 및 역할에 대한 시간 및 FTE 계산 개요](../../../../resource-mgmt/resource-planning/calculate-hours-fte-for-users-roles-resource-planner.md)를 참조하십시오.

## 사용자 설정에 대한 작업 역할 섹션에는 FTE 가용성 백분율이 포함됩니다. {#job-role-section-for-user-settings-includes-percentage-of-fte-availability}

>[!NOTE]
>
>이 기능은 현재 모든 클러스터의 미리보기에서 사용할 수 없습니다.

이제 사용자 프로필을 업데이트할 때 사용자에게 추가 작업 역할을 추가하고 각 작업 역할에 할당된 FTE의 비율을 정의할 수 있습니다.

이 변경 이전에는 사용자가 연결된 작업 역할에 특정 양의 FTE를 할당할 수 없었습니다.

사용자의 작업 역할에 대한 FTE 사용 가능 비율을 업데이트하는 방법에 대한 자세한 내용은 [사용자 프로필 편집](../../../../administration-and-setup/add-users/create-and-manage-users/edit-a-users-profile.md) 또는 [내 설정 구성](../../../../workfront-basics/manage-your-account-and-profile/configuring-your-user-profile/configure-my-settings.md)을 참조하십시오.

## 설정 영역의 새 리소스 관리 기본 설정 영역 {#new-resource-management-preferences-area-in-the-setup-area}

이제 설정에서 리소스 관리라는 새 영역을 찾을 수 있습니다. 이 영역에는 리소스 플래너에서 사용자 가용성을 계산하는 방법을 지정할 수 있는 설정이 도입되었습니다. 다음 방법을 사용하여 계산할 수 있습니다.

* 수동: 사용자의 개별 FTE 외에 시스템의 기본 스케줄을 사용하여 리소스 플래너에서 사용자의 시간 가용성을 결정합니다. 사용자의 일정이 무시됩니다.
* 자동: 사용자 스케줄은 리소스 플래너에서 사용자의 시간 가용성을 결정하는 데 사용됩니다. FTE 가용성은 사용자의 일정과 기본 일정을 기반으로 계산됩니다. 사용자 FTE의 값은 무시됩니다. 

시스템의 리소스 관리 환경 설정을 구성하는 방법에 대한 자세한 내용은 [리소스 관리 환경 설정 구성](../../../../administration-and-setup/set-up-workfront/configure-system-defaults/configure-resource-mgmt-preferences.md)을 참조하십시오.

## 프로젝트의 사용률 보고서에서 필터 저장 및 관리 {#save-and-manage-filters-in-the-utilization-report-on-a-project}

이제 사용률 보고서에서 생성한 필터를 저장할 수 있습니다. 또한 저장된 필터의 이름을 바꾸거나, 저장된 필터를 복제하거나, 저장된 필터를 삭제하거나, 저장된 필터를 수정할 수 있습니다.

이전에는 활용성 보고서를 필터링할 때마다 개별 필터 옵션을 지정해야 했습니다.

사용률 보고서에서 필터를 저장하고 관리하는 방법에 대한 자세한 내용은 [리소스 사용률 보고서 개요](../../../../reports-and-dashboards/reports/using-built-in-reports/resource-utilization-report.md)의 [리소스 사용률 보고서 개요](../../../../reports-and-dashboards/reports/using-built-in-reports/resource-utilization-report.md)를 참조하십시오.

## 활용성 보고서의 추가 필터링 옵션 {#additional-filtering-options-in-the-utilization-report}

이제 활용성 보고서를 실행할 때 이전에 사용 가능했던 작업, 문제 및 역할 필드 외에 필터를 생성할 때 Portfolio, 프로그램 및 프로젝트에 대한 새 필터링 필드를 사용할 수 있습니다.

이 변경 이전에는 새 필터 규칙을 추가하여 포트폴리오, 프로그램 및 프로젝트별로 필터링할 수 있었습니다.

자세한 내용은 [리소스 사용률 보고서 개요](../../../../reports-and-dashboards/reports/using-built-in-reports/resource-utilization-report.md)의 [리소스 사용률 보고서 개요](../../../../reports-and-dashboards/reports/using-built-in-reports/resource-utilization-report.md)를 참조하십시오.

## 프로그램 또는 Portfolio으로 활용성 보고서 보기 {#view-the-utilization-report-by-program-or-portfolio}

이제 프로그램 또는 포트폴리오별로 활용률 보고서를 볼 수 있습니다. 이렇게 하면 단일 활용성 보고서 내에서 여러 프로젝트의 정보를 볼 수 있습니다.

이러한 변경을 용이하게 하기 위해 이제 개별 프로젝트 내뿐만 아니라 Workfront 내의 보고 영역에서도 활용성 탭을 사용할 수 있습니다.

이 변경 이전에는 프로젝트 내에서만 활용성 보고서에 액세스할 수 있었습니다.

자세한 내용은  [리소스 사용률 보고서의 개요](../../../../reports-and-dashboards/reports/using-built-in-reports/resource-utilization-report.md). 

## 프로젝트 및 작업 보고서에 원래 문제 정보 표시 {#show-original-issue-information-in-project-and-task-reports}

>[!NOTE]
>
>이 기능은 현재 모든 클러스터의 미리보기에서 사용할 수 없습니다.

이제 프로젝트 또는 작업 보고서에서 문제를 전환하여 생성된 프로젝트 및 작업에 대한 원래 문제에 대한 다음 정보를 찾을 수 있습니다.

* 원래 문제 입력 일자
* 원래 문제 이름
* 원래 문제 작성자 ID

이 정보는 텍스트 모드에서 사용자 지정 보기를 작성하여 작업 또는 프로젝트 보고서나 목록에 표시할 수 있습니다.

이 변경 이전에는 이 정보에 대해 보고할 수 없었습니다.

원래 문제의 정보를 캡처하는 사용자 지정 텍스트 모드 보기를 만드는 방법에 대한 자세한 내용은 [보기: 작업 또는 프로젝트 목록에 원래 문제 정보 표시](../../../../reports-and-dashboards/reports/custom-view-filter-grouping-samples/view-display-original-issue-info-task-project-list.md)를 참조하십시오.

## 업데이트 스트림의 필터 시스템 업데이트가 이제 모든 오브젝트에서 지속됨 {#filter-system-updates-in-the-update-stream-is-now-persistent-across-objects}

>[!NOTE]
>
>이 기능은 Beta 4를 사용하는 미리보기 환경에 릴리스되지 않았습니다. 이 기능은 10월 상반기 미리보기에서 사용할 수 있습니다.

이제 시스템 업데이트 필터링 옵션이 Workfront 사이트 전체의 오브젝트에서 지속됩니다. 이렇게 하면 시스템 업데이트를 숨기고 한 개체의 업데이트 스트림에서 사용자 주석만 볼 수 있으며 다른 개체를 탐색할 때 해당 설정을 유지할 수 있습니다.

이 변경 이전에는 Workfront 사이트를 탐색할 때 각 개체에 대한 시스템 업데이트를 필터링하도록 선택해야 했습니다.

자세한 내용은 [작업 업데이트](../../../../workfront-basics/updating-work-items-and-viewing-updates/update-work.md)를 참조하세요.

## Workfront 내의 활성 증명 단계에 대한 보고서 {#report-on-active-proof-stages-within-workfront}

이제 Workfront 내에 문서 버전 보고서를 만들 때 &quot;활성 증명 단계&quot;라는 열이 있습니다. 이 열에서 보고서의 각 문서 버전에서 현재 활성 상태인 증명 단계를 볼 수 있습니다. 단계 이름이 &quot;활성 증명 단계&quot; 열에 표시됩니다. 문서 버전에서 현재 활성화된 단계가 없으면 열이 비어 있습니다.

보기 및 보고서에서 사용 가능한 필드에 대한 자세한 내용은 [Adobe Workfront 용어](../../../../workfront-basics/navigate-workfront/workfront-navigation/workfront-terminology-glossary.md)를 참조하십시오.

## Workfront 내의 사용자에게 사용자 지정 Workfront Proof 권한 프로필 할당 {#assign-custom-workfront-proof-permission-profiles-to-users-within-workfront}

이제 Workfront에서 사용자에 대한 증명 기능을 활성화할 때 사용자 지정 Workfront Proof 권한 프로필을 할당할 수 있습니다. 

이 변경 이전에는 감독자, 관리자, 관리자 권한 프로필만 사용할 수 있었습니다.

## 이벤트 구독에 시간 리소스 추가됨 {#hour-resource-added-to-event-subscriptions}

이제 새 시간 리소스를 사용하여 청구 애플리케이션을 Workfront과 계속 동기화할 수 있는 이벤트 구독을 만들 수 있습니다.

이벤트 구독에 대한 자세한 내용은 [이벤트 구독 API](../../../../wf-api/general/event-subs-api.md)를 참조하세요.
