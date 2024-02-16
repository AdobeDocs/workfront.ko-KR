---
content-type: release-notes
navigation-topic: product-releases-archive
title: 2018.2 베타 2 릴리스 활동
description: 이 페이지에서는 2018.2 베타 2 릴리스의 미리보기 환경에서 가장 최근에 사용할 수 있는 모든 변경 사항에 대해 설명합니다. 이 기능은 2018년 4월 5일에 미리보기 환경에서 사용할 수 있습니다. 프로덕션 환경에서는 2018년 6월에 사용할 수 있습니다.
author: Luke
feature: Product Announcements
recommendations: noDisplay, noCatalog
exl-id: c8ef68f5-53db-4c3c-af0f-e1c98521ec27
source-git-commit: f1e463c90641f9221228e335b583cab72762b3bd
workflow-type: tm+mt
source-wordcount: '901'
ht-degree: 0%

---

# 2018.2 베타 2 릴리스 활동

이 페이지에서는 2018.2 베타 2 릴리스의 미리보기 환경에서 가장 최근에 사용할 수 있는 모든 변경 사항에 대해 설명합니다. 이 기능은 2018년 4월 5일에 미리보기 환경에서 사용할 수 있습니다. 프로덕션 환경에서는 2018년 6월에 사용할 수 있습니다.

>[!IMPORTANT]
>
> 이 페이지에 설명된 기능은 프로덕션 환경에서 사용하기 전에 변경될 수 있습니다.

2018.2의 모든 변경 사항 목록은 다음을 참조하십시오.  [2018.2 릴리스 활동 개요](../../../../product-announcements/product-releases/quarterly-release-archive/2018.2-release-activity/2018-2-release-activity-overview.md).

2018.2 베타 2 릴리스에는 다음과 같은 개선 사항이 포함됩니다.

* [홈 영역에서 직접 필드 편집](#edit-fields-directly-from-the-home-area)
* [기간 내 시간 기록](#log-time-in-days)
* [프로젝트 목록의 간트 차트에서 프로젝트 간 전임 작업 관계 보기](#view-cross-project-predecessor-relationships-on-the-gantt-chart-in-a-list-of-projects)
* [Portfolio 최적화 도구에서 예산 비용을 사용하여 Portfolio 재무 계산](#use-budgeted-cost-in-the-portfolio-optimizer-to-calculate-portfolio-finances)
* [활용성 보고서: 신규 자원 예산 책정에서 예산 시간을 채웁니다.](#utilization-report-populates-budgeted-hours-from-new-resource-budgeting-area) (미리 보기 전용)

* [활용성 보고서: 프로젝트에 대한 사용자별 예산 시간 보기](#utilization-report-view-budgeted-hours-by-user-on-a-project) (미리 보기 전용)

* [비증명 사용자가 사용할 수 있는 문서 목록의 증명 진행률](#proof-progress-from-the-document-list-available-to-non-proofing-users)
* [모바일 개선 사항](#mobile-improvements)

## 홈 영역에서 직접 필드 편집 {#edit-fields-directly-from-the-home-area}

이제 홈 영역에서 오브젝트를 선택하면 홈 영역의 오른쪽 패널에서 해당 오브젝트와 연관된 필드를 직접 편집할 수 있습니다. 

이 변경 이전에는 정보를 편집하지 않고 홈 영역에서만 볼 수 있었습니다.

자세한 내용은 [홈 영역에서 작업 항목 업데이트 또는 편집](../../../../workfront-basics/using-home/using-the-home-area/update-and-edit-work-item-home.md) 이 문서에서  [홈 영역에서 작업 항목 업데이트 또는 편집](../../../../workfront-basics/using-home/using-the-home-area/update-and-edit-work-item-home.md).

## 기간 내 시간 기록 {#log-time-in-days}

이제 Workfront 관리자는 조직의 사용자가 시간을 일 단위로 기록할지 또는 시간 단위로 기록할지 구성할 수 있습니다. 플래너 라이선스가 있는 사용자는 자신을 위해 이 설정을 구성할 수 있습니다.

이 변경 이전에는 사용자가 시간을 시간 단위로만 기록할 수 있었습니다.

사용자 프로필을 편집하여 이 설정을 구성할 수 있습니다. 자세한 내용은 [시간이 시간 단위로 기록되는지 또는 일 단위로 기록되는지 구성](../../../../timesheets/config-timesheet-prefs/config-time-logged-hrs-days.md).

이 설정이 업데이트된 후 사용자가 일 단위로 시간을 기록할 수 있는 방법에 대한 자세한 내용은 [로그 시간](../../../../timesheets/create-and-manage-timesheets/log-time.md).

## 프로젝트 목록의 간트 차트에서 프로젝트 간 전임 작업 관계 보기 {#view-cross-project-predecessor-relationships-on-the-gantt-chart-in-a-list-of-projects}

이제 다음 프로젝트 목록의 간트 차트에서 프로젝트 간 전임 작업 관계를 볼 수 있습니다.

* 포트폴리오 또는 프로그램 내의 프로젝트 탭
* 프로젝트 보고서에서

이 변경 이전에는 프로젝트 수준의 개별 작업에 대해서만 프로젝트 간 전임 작업 관계를 볼 수 있었습니다.

자세한 내용은 [간트 차트에 정보가 표시되는 방식 구성](../../../../manage-work/gantt-chart/use-the-gantt-chart/configure-info-on-gantt-chart.md). 

## Portfolio 최적화 도구에서 예산 비용을 사용하여 Portfolio 재무 계산 {#use-budgeted-cost-in-the-portfolio-optimizer-to-calculate-portfolio-finances}

이제 새 Portfolio 최적기는 비즈니스 사례의 새 리소스 예산 책정 영역 또는 리소스 플래너에서 예산 책정된 원가를 사용하여 다음 필드를 계산합니다.

* 순 가치
* 투자 수익률(ROI)
* 비용

이전에는 신규 및 기존 Portfolio 최적화 도구에서 모두 기존 예산 비용을 사용했습니다. 기존 Portfolio 최적기는 여전히 기존 예산 비용을 사용하여 순 가치, 투자 수익률 및 비용을 계산합니다.

또한 Portfolio 재무 필드에 레거시 ROI 및 레거시 순 가치라는 두 가지 새로운 필드를 추가하여 새로운 리소스 관리 도구에서 새로운 가치를 포착했습니다.

자세한 내용은 [Portfolio 최적화 프로그램 개요](../../../../manage-work/portfolios/portfolio-optimizer/portfolio-optimizer-overview.md) 이 문서에서  [Portfolio 최적화 프로그램 개요](../../../../manage-work/portfolios/portfolio-optimizer/portfolio-optimizer-overview.md).

## 활용성 보고서: 신규 자원 예산 책정에서 예산 시간을 채웁니다. {#utilization-report-populates-budgeted-hours-from-new-resource-budgeting-area}

>[!NOTE]
>
>이 기능은 2018.2 릴리스의 미리보기 환경에 대한 공식 릴리스에 포함되지 않습니다. 2018.3 릴리스의 베타 기간 동안 다시 도입되며, 2018.3 릴리스와 함께 프로덕션 환경에 릴리스될 예정입니다. 

활용성 보고서의 예산 시간은 이제 비즈니스 사례의 새 리소스 예산 책정에서 사용할 수 있는 정보로 채워집니다.

이 변경 이전에는 기존 리소스 견적 영역의 정보가 사용되었습니다.

자세한 내용은 [자원 가동률 보고서 개요](../../../../reports-and-dashboards/reports/using-built-in-reports/resource-utilization-report.md) 이 문서에서  [자원 가동률 보고서 개요](../../../../reports-and-dashboards/reports/using-built-in-reports/resource-utilization-report.md).

## 활용성 보고서: 프로젝트에 대한 사용자별 예산 시간 보기 {#utilization-report-view-budgeted-hours-by-user-on-a-project}

>[!NOTE]
>
>이 기능은 2018.2 릴리스의 미리보기 환경에 대한 공식 릴리스에 포함되지 않습니다. 2018.3 릴리스의 베타 기간 동안 다시 도입되며, 2018.3 릴리스와 함께 프로덕션 환경에 릴리스될 예정입니다. 

이제 프로젝트의 활용성 보고서에 사용자별 예산 시간이 표시됩니다.

이 변경 이전의 활용성 보고서에는 작업 역할별 예산 시간만 표시됩니다. 

자세한 내용은 [자원 가동률 보고서 개요](../../../../reports-and-dashboards/reports/using-built-in-reports/resource-utilization-report.md) 이 문서에서 [자원 가동률 보고서 개요](../../../../reports-and-dashboards/reports/using-built-in-reports/resource-utilization-report.md).

## 비증명 사용자가 사용할 수 있는 문서 목록의 증명 진행률 {#proof-progress-from-the-document-list-available-to-non-proofing-users}

이제 문서 목록을 볼 때 모든 사용자에 대해 증명 진행 표시기(보냄, 열림, 설명 및 결정)가 표시됩니다. 여기에는 증명을 생성할 수 없는 사용자가 포함됩니다(사용자가 증명을 생성하는 방법에 대한 자세한 내용은 섹션 참조).

이 변경 이전에는 증명을 생성할 수 있는 사용자에 대해서만 증명 진행 상태 표시기를 사용할 수 있었습니다.

자세한 내용은 [증명 진행 상황 및 상태 개요](../../../../review-and-approve-work/proofing/proofing-overview/view-progress-status-proof.md).

## 모바일 개선 사항 {#mobile-improvements}

모바일 앱에는 다음과 같은 개선 사항이 포함되어 있습니다.

* 다른 모바일 애플리케이션에서 사용자와 공유되는 링크가 이제 Workfront 모바일 앱에서 열립니다.

  링크 공유에 대한 자세한 내용은 를 참조하십시오.

  이제 iOS 및 Android에서 이 업데이트를 사용할 수 있습니다.

* iPhone X를 지원하도록 iOS 플랫폼에 대한 지원 요구 사항이 업데이트되었습니다.

  지원되는 모바일 장치 및 운영 체제에 대한 자세한 내용은 를 참조하십시오. 
