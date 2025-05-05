---
content-type: release-notes
navigation-topic: product-releases-archive
title: 2018.1 Beta 1 릴리스 활동
description: 이 페이지에서는 2018.1 Beta 1 릴리스의 미리보기 환경에서 가장 최근에 사용할 수 있는 모든 변경 사항에 대해 설명합니다. 이 페이지의 기능은 2017년 12월 1일에 미리보기 환경에서 사용할 수 있습니다. 프로덕션 환경에서는 2018년 3월에 사용할 수 있습니다.
author: Luke
feature: Product Announcements
recommendations: noDisplay, noCatalog
exl-id: efcc2217-ab69-4ac4-8e9a-f811eba77d49
source-git-commit: f1e463c90641f9221228e335b583cab72762b3bd
workflow-type: tm+mt
source-wordcount: '1065'
ht-degree: 0%

---

# 2018.1 Beta 1 릴리스 활동

이 페이지에서는 2018.1 Beta 1 릴리스의 미리보기 환경에서 가장 최근에 사용할 수 있는 모든 변경 사항에 대해 설명합니다. 이 페이지의 기능은 2017년 12월 1일에 미리보기 환경에서 사용할 수 있습니다. 프로덕션 환경에서는 2018년 3월에 사용할 수 있습니다.

>[!IMPORTANT]
>
> 이 페이지에 설명된 기능은 프로덕션 환경에서 사용하기 전에 변경될 수 있습니다.

2018.1의 모든 변경 사항 목록은 다음을 참조하십시오.  [2018.1 릴리스 활동 개요](../../../../product-announcements/product-releases/quarterly-release-archive/2018.1-release-activity/2018-1-release-activity-overview.md).

2018.1 Beta 1 릴리스에는 Workfront 관리자와 기타 사용자 모두를 위한 개선 사항이 포함되어 있습니다.

관리자용 **1&rbrace;**

* [홈 영역을 지원하도록 레이아웃 템플릿을 업데이트했습니다](#updated-layout-template-to-support-the-home-area)
* [Workfront에서 보낸 증명 전자 메일 알림 사용 안 함](#disable-proofing-email-notifications-sent-from-workfront)
* [이벤트 구독에 추가된 새 리소스](#new-resources-added-to-event-subscriptions)

**모든 사용자용**

* [홈 영역(내 작업 영역 업데이트됨)](#home-area-updated-my-work-area)
* [비즈니스 사례 및 업데이트된 비즈니스 사례 요약에 리소스 플래너 데이터 표시](#display-resource-planner-data-under-the-business-case-and-updated-business-case-summary)
* [리소스 플래너의 계획된 시간 할당 비율을 표시합니다](#display-the-percentage-of-planned-hour-allocation-in-the-resource-planner)
* [자동 및 변경 시 및 변경 전용 업데이트 유형은 작업이 업데이트되는 동시에 상위 개체에 대한 업데이트를 트리거합니다](#the-automatic-and-on-change-and-change-only-update-types-trigger-updates-to-the-parent-objects-at-the-same-time-as-tasks-are-updated)
* [간트 차트에서 사용할 수 있는 타임라인 스냅샷](#timeline-snapshot-available-in-the-gantt-chart)

## 홈 영역(내 작업 영역 업데이트됨) {#home-area-updated-my-work-area}

새 홈 영역에서는 현재 내 작업 영역에서 사용할 수 있는 것과 동일한 데이터에 대해 개선된 대체 보기를 제공합니다. 홈 영역은 내 작업 영역에 비해 다음과 같은 이점을 제공합니다.

* 보다 능률적이고 직관적인 인터페이스
* 향상된 성능
* 서식 있는 텍스트 서식 관련 작업 및 문제 업데이트

## 홈 영역을 지원하도록 레이아웃 템플릿을 업데이트했습니다. {#updated-layout-template-to-support-the-home-area}

Workfront 관리자는 할당된 레이아웃 템플릿을 구성하여 조직의 사용자가 홈 영역에 액세스할 수 있는지 여부를 결정할 수 있습니다. 레이아웃 템플릿이 할당되지 않은 사용자는 항상 홈 영역에 액세스할 수 있습니다.

자세한 내용은 &quot;레이아웃 템플릿 만들기 및 관리&quot;를 참조하십시오.

## Workfront에서 보낸 증명 이메일 알림 비활성화 {#disable-proofing-email-notifications-sent-from-workfront}

이제 증명에 대한 댓글이 있을 때 Workfront 인스턴스의 사용자가 Workfront에서 이메일 알림을 수신하는지 여부를 구성할 수 있습니다.

이전에는 증명에 댓글이 달리면 항상 Workfront에서 증명 이메일이 전송되었습니다. Workfront Proof에서도 알림을 활성화한 경우 이로 인해 사용자가 중복 알림을 받게 되었습니다. 

기존 Workfront 고객의 경우 Workfront은 증명에 댓글이 있을 때 이메일을 보내도록 기본적으로 구성됩니다.

Workfront에서 증명에 대한 이메일 알림을 비활성화하여 Workfront Proof에서만 증명 이메일을 전송하는 방법에 대한 자세한 내용은 을 참조하십시오.  

## 비즈니스 사례 및 업데이트된 비즈니스 사례 요약 아래에 리소스 플래너 데이터 표시 {#display-resource-planner-data-under-the-business-case-and-updated-business-case-summary}

이제 프로젝트의 비즈니스 사례에서 리소스 예산 영역을 사용할 수 있습니다. 이 영역에서는 리소스 플래너의 리소스에 대해 예상되는 예산 시간 및 이와 연관된 예산 인건비를 검토할 수 있습니다.

비즈니스 사례의 리소스 견적 영역 이름이 기존 리소스 견적서로 변경되었습니다.

이 변경 사항의 일부로서, 이제 비즈니스 사례 요약에 리소스 추정과 리소스 예산 편성을 모두 기반으로 하는 재무 정보가 포함됩니다.

이 변경 이전에는 프로젝트의 비즈니스 사례에 대한 리소스 플래너 정보를 볼 수 없었습니다. 레거시 리소스 풀의 용량 플래너에 지정된 리소스 견적 정보만 볼 수 있습니다.

비즈니스 사례 만들기에 대한 자세한 내용은 [프로젝트에 대한 비즈니스 사례 만들기](../../../../manage-work/projects/define-a-business-case/create-business-case.md)를 참조하세요.

## 리소스 플래너에 계획된 시간 할당의 백분율 표시 {#display-the-percentage-of-planned-hour-allocation-in-the-resource-planner}

이제 리소스 플래너의 사용자 보기에는 사용자와 작업 역할에 대한 총 가용 시간의 백분율로 계획된 시간 할당을 볼 수 있는 새 열이 포함됩니다.

이 변경 이전에는 사용자 및 작업 역할에 대한 계획된 시간과 가용 시간의 합계를 별도의 열에서만 볼 수 있었습니다.

계획된 시간 할당 백분율 열에 대한 자세한 내용은 [리소스 플래너 개요](../../../../resource-mgmt/resource-planning/get-started-resource-planner.md)의 &quot;리소스 플래너에서 사용 가능한 시간과 계획된 시간 또는 FTE 사이의 차이 보기&quot; 섹션을 참조하십시오.

## &quot;자동 및 변경 시에만&quot; 및 &quot;변경 전용&quot; 업데이트 유형은 작업 업데이트와 동시에 상위 오브젝트에 대한 업데이트를 트리거합니다 {#the-automatic-and-on-change-and-change-only-update-types-trigger-updates-to-the-parent-objects-at-the-same-time-as-tasks-are-updated}

프로젝트에서 하위 수준 개체가 업데이트될 때 상위 작업 및 프로젝트가 업데이트되는 방식을 변경했습니다. 상위 객체가 업데이트되는 시간은 프로젝트의 업데이트 유형 필드에 의해 결정됩니다. 다음 업데이트 유형 중에서 선택할 수 있습니다.

* 자동 및 변경 시
* 변경만
* 자동만
* 수동만

이제 &quot;자동 및 변경 시에만&quot; 또는 &quot;변경만&quot; 업데이트 유형을 선택하면 개별 작업에 적용되는 변경 사항이 상위 작업 및 프로젝트에도 즉시 적용됩니다.

이 변경 이전에는 페이지를 새로 고쳐 상위 개체와 프로젝트의 타임라인도 업데이트되었는지 확인해야 했습니다.

프로젝트의 업데이트 형식에 대한 자세한 내용은 [프로젝트 업데이트 형식 선택](../../../../manage-work/projects/manage-projects/select-project-update-type.md)을 참조하세요.

## 간트 차트에서 사용할 수 있는 타임라인 스냅샷 {#timeline-snapshot-available-in-the-gantt-chart}

이제 간트 차트에서 새 타임라인 스냅샷을 사용하여 프로젝트 수명의 특정 지점으로 빠르게 스크롤할 수 있습니다.

작업 또는 프로젝트 목록을 보는 동안 간트 차트에 대해 보다 세분화된 기간을 선택하면 간트 차트 하단에 가로 스크롤 막대가 표시됩니다. 스크롤 막대를 클릭하면 프로젝트의 전체 타임라인을 스냅샷으로 볼 수 있습니다. 간트 차트 스냅샷 내부의 아무 곳이나 클릭하여 프로젝트 수명의 특정 지점으로 이동할 수 있습니다.

이 변경 이전에는 전체 간트 차트에서 가로로 스크롤하여 특정 시점을 찾거나 세부 보기에서 축소해야 했습니다.

간트 차트에 정보가 표시되는 방법에 대한 자세한 내용은 [간트 차트에 정보가 표시되는 방법 구성](../../../../manage-work/gantt-chart/use-the-gantt-chart/configure-info-on-gantt-chart.md)을 참조하십시오.

## 이벤트 구독에 추가된 새 리소스 {#new-resources-added-to-event-subscriptions}

이제 다음 리소스에 대한 이벤트 구독을 만들 수 있습니다.

* **경비:** 경비를 추가하거나 수정하면 알려줍니다.
* **할당:** 사용자, 작업 역할 또는 팀의 작업 또는 문제에 대한 할당이 추가되거나 수정되면 알림을 보냅니다.
* **타임시트:** 타임시트가 제출, 거부 또는 승인되면 알려줍니다.

이벤트 구독에 대한 자세한 내용은 [이벤트 구독 API](../../../../wf-api/general/event-subs-api.md)를 참조하세요.
