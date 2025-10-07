---
content-type: release-notes
navigation-topic: product-releases-archive
title: 2017.3 Beta 최종 릴리스 활동
description: 이 페이지에서는 2017.3 Beta 최종 릴리스의 미리보기 환경에서 가장 최근에 사용할 수 있는 모든 변경 사항에 대해 설명합니다. 이 페이지의 기능은 2017년 9월 12일에 미리보기 환경에서 사용할 수 있습니다. 프로덕션 환경에서는 2017년 11월 초에 제공될 예정입니다.
author: Luke
feature: Product Announcements
recommendations: noDisplay, noCatalog
exl-id: 880828f4-3908-4ef0-ab1f-774f8dee72b6
source-git-commit: f5044d457ebf203269e8007075e98ba4c136660f
workflow-type: tm+mt
source-wordcount: '3791'
ht-degree: 0%

---

# 2017.3 Beta 최종 릴리스 활동

이 페이지에서는 2017.3 Beta 최종 릴리스의 미리보기 환경에서 가장 최근에 사용할 수 있는 모든 변경 사항에 대해 설명합니다. 이 페이지의 기능은 2017년 9월 12일에 미리보기 환경에서 사용할 수 있습니다. 프로덕션 환경에서는 2017년 11월 초에 제공될 예정입니다.

>[!IMPORTANT]
>
> 이 페이지에 설명된 기능은 프로덕션 환경에서 사용하기 전에 변경될 수 있습니다.

2017.3의 모든 변경 사항 목록은 다음을 참조하십시오.  [2017.3 릴리스 활동 개요](../../../../product-announcements/product-releases/quarterly-release-archive/2017.3-release-activity/2017-3-release-activity-overview.md).

2017.3 Beta 최종 릴리스에는 Workfront 관리자와 기타 사용자 모두를 위한 개선 사항이 포함되어 있습니다.

관리자용 **1&rbrace;**

* [승인 설정 영역에서 요청 회수를 위한 새 구성](#new-configuration-for-recalling-requests-in-the-approval-settings-area)
* [기본 증명 역할 구성](#configure-default-proof-roles)

**모든 사용자용**

* [홈 영역(내 작업 영역 업데이트됨)](#home-area-updated-my-work-area)

* [홈 영역을 지원하도록 레이아웃 템플릿을 업데이트했습니다](#updated-layout-template-to-support-the-home-area)

* 애자일용 [Kanban](#kanban-for-agile)
* [애자일 팀의 스크럼 백로그에 문제를 포함합니다](#include-issues-on-the-scrum-backlog-for-an-agile-team)
* [스크럼 애자일 스토리 보드에 문제 포함](#include-issues-on-the-scrum-agile-story-board)
* [애자일 팀의 백로그에 그룹화 및 필터 적용](#apply-groupings-and-filters-to-the-backlog-for-an-agile-team)
* [향상된 @Tagging 기능이 미리 보기 환경에서 반환됩니다](#enhanced-tagging-functionality-returns-in-the-preview-environment)
* [업데이트 스트림의 필터 시스템 업데이트가 이제 개체 간에 지속됩니다](#filter-system-updates-in-the-update-stream-is-now-persistent-across-objects)
* [사용률 보고서에서 데이터 시각화](#visualize-data-in-the-utilization-report)
* [사용률 보고서 성능 개선](#utilization-report-performance-improvement)
* [문서 개선 사항: 간소화된 인터페이스](#document-enhancements-streamlined-interface)
* [Workfront의 증명 개선 사항](#proofing-enhancements-within-workfront)
* [Workfront Proof 및 Workfront 모두에서 향상된 증명 기능](#proofing-enhancements-within-both-workfront-proof-and-workfront)
* [업데이트 및 전자 메일에 대한 서식 있는 텍스트 서식](#rich-text-formatting-for-updates-and-emails)
* [새 간트 차트 다시 디자인](#new-gantt-chart-redesign)
* [기본 제공 보고서에 업데이트된 설명이 포함되어 있음](#built-in-reports-contain-updated-descriptions)
* [내보낸 보고서, 목록 및 대시보드의 브랜딩](#branding-in-exported-reports-lists-and-dashboards)
* [작업 복사 및 작업 또는 문제 이동 시 개선 사항](#improvements-when-copying-tasks-and-moving-tasks-or-issues)
* [리소스 예산 시간 보고서에 대한 새 그룹화: 할당 날짜](#new-grouping-for-resource-budgeted-hour-reports-allocation-date)
* [리소스 플래너 개선 사항](#resource-planner-improvements)
* [모바일 개선 사항](#mobile-improvements)
* [Slack과 Workfront 통합](#workfront-integration-with-slack)
* [Outlook 365 개선 사항](#outlook-365-improvements)
* [API 변경 사항](#api-changes)

## 홈 영역(내 작업 영역 업데이트됨) {#home-area-updated-my-work-area}

>[!NOTE]
>
>이 기능은 17.3 릴리스와 함께 프로덕션 환경에 릴리스되지 않습니다. 2018년 초까지 미리보기에 유지됩니다.

새 홈 영역에서는 현재 내 작업 영역에서 사용할 수 있는 것과 동일한 데이터에 대해 개선된 대체 보기를 제공합니다. 홈 영역은 내 작업 영역에 비해 다음과 같은 이점을 제공합니다.

* 보다 능률적이고 직관적인 인터페이스
* 향상된 성능

다음 기능은 내 작업 영역에서 사용할 수 있지만 홈 영역에서는 아직 구현되지 않았습니다.

* 개인 캘린더 보기
* 서식 있는 텍스트 서식 관련 작업 및 문제 업데이트
* 증명 승인
* 승인을 위해 제출한 작업 목록 보기
* 프로젝트에 대한 임시 문제 만들기
* 귀하에게 위임된 승인만 보기

새 홈 영역 사용에 대한 자세한 내용은 [홈 영역 사용](../../../../workfront-basics/using-home/using-the-home-area/use-the-home-area.md)을 참조하세요.

## 홈 영역을 지원하도록 레이아웃 템플릿을 업데이트했습니다. {#updated-layout-template-to-support-the-home-area}

>[!NOTE]
>
>이 기능은 17.3 릴리스와 함께 프로덕션 환경에 릴리스되지 않습니다. 2018년 초까지 미리보기에 유지됩니다.

Workfront 관리자는 할당된 레이아웃 템플릿을 구성하여 조직의 사용자가 홈 영역에 액세스할 수 있는지 여부를 결정할 수 있습니다. 레이아웃 템플릿이 할당되지 않은 사용자는 항상 홈 영역에 액세스할 수 있습니다.

자세한 내용은 &quot;레이아웃 템플릿 만들기 및 관리&quot;에서 &quot;홈 맞춤화&quot;를 참조하십시오.

## 애자일용 칸반  {#kanban-for-agile}

이제 애자일 팀은 이미 지원되는 스크럼 애자일 방법론에 더하여 Workfront 내에서 Kanban 방법론을 사용할 수 있습니다.

Workfront의 스크럼 및 칸반 애자일 방법론은 다음과 같은 점에서 다릅니다.

**Workfront에서 Kanban을 사용할 때의 이점**

* Kanban 애자일 스토리 보드에 백로그를 표시합니다.

  자세한 내용은에서 를 참조하십시오.

* 다른 항목이 완료와 동일한 상태로 이동될 때 백로그에 있는 항목이 자동으로 Kanban 애자일 스토리 보드에 추가되도록 구성합니다.

  자세한 내용은 [Kanban 구성](../../../../agile/get-started-with-agile-in-workfront/configure-kanban.md#configur5)의 [백로그에서 자동으로 추가할 스토리 구성](../../../../agile/get-started-with-agile-in-workfront/configure-kanban.md)을 참조하십시오.

* Kanban 애자일 스토리 보드에 표시할 WIP(Work In Progress) 한도를 구성합니다.

  자세한 내용은 [Kanban 구성](../../../../agile/get-started-with-agile-in-workfront/configure-kanban.md#configur4)에서 [WIP(작업 진행 중) 제한 구성](../../../../agile/get-started-with-agile-in-workfront/configure-kanban.md)을 참조하십시오.

**Workfront에서 스크럼 사용의 이점**

* 애자일 반복에 스토리 세트를 추가하고 해당 반복에 대한 스토리 보드를 만듭니다.
* 스크럼 스토리 보드에 문제를 포함합니다.
* 애자일 팀의 백로그에 문제를 포함합니다.

  자세한 내용은 [스크럼 구성](../../../../agile/get-started-with-agile-in-workfront/configure-scrum.md#configur5)에서 [반복에 작업 항목을 추가할 때 날짜가 적용되는 방법 구성](../../../../agile/get-started-with-agile-in-workfront/configure-scrum.md)을 참조하십시오.

* 하위 작업은 스크럼 스토리 보드에 표시될 수 있습니다.
* 번다운 차트를 보고 반복 중 스토리에 대한 진행률을 확인합니다.

  자세한 내용은 [애자일 번다운 차트 개요](../../../../agile/use-scrum-in-an-agile-team/burndown/burndown-chart-overview.md)를 참조하세요.

애자일 팀을 위해 Kanban을 사용 및 구성하는 방법에 대한 자세한 내용은 [애자일 팀 만들기](../../../../agile/get-started-with-agile-in-workfront/create-an-agile-team.md#deciding)에서 [애자일 방식 결정](../../../../agile/get-started-with-agile-in-workfront/create-an-agile-team.md)을 참조하십시오.

## 애자일 팀의 스크럼 백로그에 문제를 포함합니다. {#include-issues-on-the-scrum-backlog-for-an-agile-team}

>[!NOTE]
>
>이 기능은 2017년 11월 14일에 프로덕션 환경에서 제거되었습니다. 향상된 디자인과 향상된 안정성으로 2018년 초에 미리보기 환경에 다시 도입될 예정입니다. 프로덕션 환경에서는 2018.1 릴리스에서 사용할 수 있습니다.

이제 스크럼 애자일 방법론을 사용할 때 애자일 팀의 백로그에 문제를 포함할 수 있습니다(Kanban 방법론을 사용할 때 애자일 팀의 백로그에 문제가 표시되지 않음). 문제를 포함하려면 기존 스크럼 애자일 팀이 이 기능을 활성화해야 합니다. 문제는 2017.3 릴리스 이후 생성된 스크럼 애자일 팀의 백로그에 자동으로 포함됩니다.

이 변경 이전에는 작업만 백로그에 추가할 수 있었습니다. 문제를 추가하려면 먼저 문제를 작업으로 변환해야 합니다.

이제 백로그에 있는 작업 외에 다른 작업에 액세스할 수 있으므로, 이전에 백로그에서 사용할 수 있었던 모든 사용자 지정 작업 보기가 복사되어 사용자 지정 백로그 작업 항목 보기로 백로그에 추가됩니다.

백로그에서 문제를 사용하는 방법에 대한 자세한 내용은  [애자일 백로그를 관리합니다](../../../../agile/work-in-an-agile-environment/manage-the-agile-backlog.md).

애자일 스크럼 팀의 백로그에서 사용할 수 있는 문제를 활성화하는 방법에 대한 자세한 내용은  [스크럼 구성](../../../../agile/get-started-with-agile-in-workfront/configure-scrum.md#configur5)에서 [작업 항목을 반복에 추가할 때 날짜가 적용되는 방식을 구성합니다](../../../../agile/get-started-with-agile-in-workfront/configure-scrum.md).

## 스크럼 애자일 스토리 보드에 문제 포함 {#include-issues-on-the-scrum-agile-story-board}

>[!NOTE]
>
>이 기능은 2017년 11월 14일에 프로덕션 환경에서 제거되었습니다. 향상된 디자인과 향상된 안정성으로 2018년 초에 미리보기 환경에 다시 도입될 예정입니다. 프로덕션 환경에서는 2018.1 릴리스에서 사용할 수 있습니다.

이제 스크럼 애자일 방법론을 사용할 때 스토리 보드에 문제를 포함할 수 있습니다.

자세한 내용은 [스크럼 구성](../../../../agile/get-started-with-agile-in-workfront/configure-scrum.md#configur2)에서 [애자일 스토리 보드에서 상태 열 구성](../../../../agile/get-started-with-agile-in-workfront/configure-scrum.md)을(를) 참조하십시오.

## 애자일 팀의 백로그에 그룹화 및 필터 적용 {#apply-groupings-and-filters-to-the-backlog-for-an-agile-team}

>[!NOTE]
>
>이 기능은 2017년 11월 14일에 프로덕션 환경에서 제거되었습니다. 향상된 디자인과 향상된 안정성으로 2018년 초에 미리보기 환경에 다시 도입될 예정입니다. 프로덕션 환경에서는 2018.1 릴리스에서 사용할 수 있습니다.

이제 애자일 백로그에서 그룹화 및 필터 옵션을 사용할 수 있으므로 그룹화별로 백로그를 구성하고 특정 작업 및 문제를 필터링할 수 있습니다.

이 변경 전에 보기에서 애자일 백로그에 적용할 수 있었습니다.

자세한 내용은  [애자일 백로그 관리](../../../../agile/work-in-an-agile-environment/manage-the-agile-backlog.md)  [애자일 백로그를 관리합니다](../../../../agile/work-in-an-agile-environment/manage-the-agile-backlog.md).

## 업데이트 및 전자 메일에 대한 서식 있는 텍스트 서식 {#rich-text-formatting-for-updates-and-emails}

>[!NOTE]
>
>미리 보기 환경 내에서 변경한 서식은 다시 서식이 지정되지 않은 상태로 되돌릴 수 있습니다.

이제 Workfront 개체에 대한 주석 및 업데이트의 서식을 지정하여 중요한 정보를 강조할 수 있습니다. 

서식 있는 텍스트 도구를 사용하여 텍스트에 서식 특성을 적용하고, 글머리 기호 및 번호 매기기 목록을 만들고, 추가 리소스에 하이퍼링크를 추가할 수 있습니다.

업데이트 스트림의 댓글에 적용된 서식은 업데이트 이메일 알림에도 표시됩니다. 댓글 서식 지정에 대한 자세한 내용은 [작업 업데이트](../../../../workfront-basics/updating-work-items-and-viewing-updates/update-work.md)를 참조하세요.

## 향상된 @Tagging 기능이 미리보기 환경에서 반환됨 {#enhanced-tagging-functionality-returns-in-the-preview-environment}

다시 한 번 @ 기호를 사용하여 미리보기 환경에 있는 모든 개체의 업데이트 스트림에서 다른 사용자를 태그 지정할 수 있습니다. 이전에는 태그@tagging 지정된 사용자의 이름과 성을 업데이트 스트림에 배치했습니다. 이제 향상된 @tagging 기능은 사용자의 이름만 표시합니다. 업데이트에 사용자를 태그 지정하는 방법에 대한 자세한 내용은 [업데이트에 다른 사용자 태그 지정](../../../../workfront-basics/updating-work-items-and-viewing-updates/tag-others-on-updates.md)을 참조하세요.

## 업데이트 스트림의 필터 시스템 업데이트가 이제 모든 오브젝트에서 지속됨 {#filter-system-updates-in-the-update-stream-is-now-persistent-across-objects}

이제 시스템 업데이트 필터링 옵션이 Workfront 사이트 전체의 오브젝트에서 지속됩니다. 이렇게 하면 시스템 업데이트를 숨기고 한 개체의 업데이트 스트림에서 사용자 주석만 볼 수 있으며 다른 개체를 탐색할 때 해당 설정을 유지할 수 있습니다.

이 변경 이전에는 Workfront 사이트를 탐색할 때 각 개체에 대한 시스템 업데이트를 필터링하도록 선택해야 했습니다.

자세한 내용은 [작업 업데이트](../../../../workfront-basics/updating-work-items-and-viewing-updates/update-work.md)를 참조하세요.

## 활용성 보고서에서 데이터 시각화 {#visualize-data-in-the-utilization-report}

 이제 차트 보기에서 사용률 정보를 볼 수 있습니다. 

자세한 내용은 [리소스 사용률 보고서 개요](../../../../reports-and-dashboards/reports/using-built-in-reports/resource-utilization-report.md)의 [리소스 사용률 보고서 개요](../../../../reports-and-dashboards/reports/using-built-in-reports/resource-utilization-report.md)를 참조하십시오.

## 활용성 보고서 성능 개선 {#utilization-report-performance-improvement}

>[!NOTE]
>
>이 기능은 Beta Final 릴리스 이후 패치로 릴리스되었습니다.

이제 활용성 보고서를 실행할 때 보고서를 실행하기 전에 필터를 적용하라는 메시지가 표시됩니다. 이 변경 사항은 가장 관련 있는 정보가 최대한 빨리 활용률 보고서에 생성되도록 합니다.

사용률 보고서 실행에 대한 자세한 내용은 [리소스 사용률 보고서 개요](../../../../reports-and-dashboards/reports/using-built-in-reports/resource-utilization-report.md)의 [리소스 사용률 보고서 개요](../../../../reports-and-dashboards/reports/using-built-in-reports/resource-utilization-report.md)를 참조하십시오.

## 문서 개선 사항: 간소화된 인터페이스 {#document-enhancements-streamlined-interface}

이제 Workfront에 문서를 추가하는 사용자 환경이 보다 간소화되고 직관적입니다. 이제 간단한 드롭다운 메뉴에서 파일 시스템에서 문서를 업로드하거나, 문서를 요청하거나, 서드파티 애플리케이션(예: Google 또는 Dropbox)에서 파일을 연결할 수 있습니다. 

이전에는 문서 추가 대화 상자를 시작하여 이러한 옵션을 사용할 수 있었습니다. 

자세한 내용은 다음 정보를 참조하십시오.

* [파일 시스템에서 Adobe Workfront에 문서 추가](../../../../documents/adding-documents-to-workfront/add-documents-from-file-system.md)
* [문서 요청](../../../../documents/adding-documents-to-workfront/request-a-document.md)
* [외부 응용 프로그램에서 문서 연결](../../../../documents/adding-documents-to-workfront/link-documents-from-external-apps.md) 

>[!NOTE]
>
>이 변경 사항으로 인해 클립보드에서 이미지 또는 문서를 붙여넣는 옵션을 더 이상 사용할 수 없습니다.

## Workfront의 증명 개선 사항 {#proofing-enhancements-within-workfront}

* [향상된 사용자 환경 및 추가 기능](#improved-user-experience-and-additional-functionality)
* [증명 뷰어에서 직접 공유](#share-directly-from-the-proofing-viewer)
* [기본 증명 역할 구성](#configure-default-proof-roles)

### 향상된 사용자 경험 및 추가 기능 {#improved-user-experience-and-additional-functionality}

이제 Workfront에서 증명을 만들 때 개선된 사용자 경험 외에도 다음과 같은 추가 기능을 사용할 수 있습니다.

* 여러 이미지를 하나의 증명으로 병합합니다.
* 여러 해상도의 증명 웹 사이트(여러 해상도가 개별 증명으로 생성되거나 단일 증명으로 결합될 수 있음)
* 업로드 프로세스 중에 파일 이름을 편집합니다.
* 증명 생성 양식에 사용자 정의 필드를 포함합니다.
* 증명 이메일 알림에 사용자 정의 메시지를 추가합니다.
* 추가 증명 설정 
* URL을 증명 할 때 실시간 오류 유효성 검사(이전에는 오류가 표시되기 전에 몇 분을 기다려야 함)

자세한 내용은 를 참조하십시오.

>[!NOTE]
>
> 자동화된 워크플로를 사용하여 새 증명을 만들 때 사용자를 한 단계에서 다른 단계로 이동하는 데 드래그 앤 드롭이 지원되지 않습니다. 대신 한 단계에서 사용자를 제거하고 다른 단계에 추가합니다.

*드래그 앤 드롭을 사용하여 사용자를 한 단계에서 다른 단계로 이동하는 옵션은 2018.1 릴리스와 함께 다시 도입됩니다.*

### 증명 뷰어에서 직접 공유 {#share-directly-from-the-proofing-viewer}

이제 증명 뷰어에서 특정 Workfront 사용자와 직접 공유할 수 있습니다.

>[!NOTE]
>
>이 기능은 새 증명(2017.3 릴리스 이후에 생성된 증명)과 Workfront Proof Premium 계정과 통합된 Workfront 인스턴스에만 사용할 수 있습니다.

이 변경 이전에는 링크를 만든 다음 해당 링크를 사용자와 공유하는 방법으로만 공유할 수 있었습니다. 

자세한 내용은 [Adobe Workfront 내에서 증명 공유](../../../../review-and-approve-work/proofing/managing-proofs-within-workfront/share-a-proof-in-workfront.md)에서 [Adobe Workfront 내에서 증명 공유](../../../../review-and-approve-work/proofing/managing-proofs-within-workfront/share-a-proof-in-workfront.md)를 참조하십시오.

### 기본 증명 역할 구성 {#configure-default-proof-roles}

이제 Workfront 시스템 내에서 새 사용자 및 게스트 사용자가 새 증명에 가져야 하는 기본 증명 역할을 구성할 수 있습니다. 

증명이 사용자와 공유될 때 증명에서 사용자가 할당 받는 기본 역할입니다. 

## Workfront Proof 및 Workfront 모두에서 향상된 증명 기능 {#proofing-enhancements-within-both-workfront-proof-and-workfront}

* [HTML5 비디오 증명 뷰어에서 다시 시작 및 건너뛰기(키보드 단축키)](#restart-and-skip-in-html5-video-proofing-viewer-keyboard-shortcuts)
* [HTML5 증명 뷰어 업데이트](#html5-proofing-viewer-updates)

### HTML5 비디오 증명 뷰어에서 다시 시작 및 건너뛰기(키보드 단축키) {#restart-and-skip-in-html5-video-proofing-viewer-keyboard-shortcuts}

이제 비디오용 HTML5 증명 뷰어 내에 비디오를 처음부터 다시 시작하고 비디오 끝으로 건너뛸 수 있는 키보드 단축키가 있습니다.

사용 가능한 키보드 단축키에 대한 자세한 내용은 [Workfront Proof 증명 뷰어의 키보드 단축키](../../../../workfront-proof/wp-work-proofsfiles/review-proofs-wpv/keyboard-shortcuts.md)를 참조하십시오.

### HTML5 증명 뷰어 업데이트 {#html5-proofing-viewer-updates}

이제 HTML5 뷰어가 정적 증명을 지원합니다.

이 변경 이전에는 HTML5 뷰어에서 비디오 증명만 지원했습니다. 

HTML 뷰어에는 정적 콘텐츠의 교정을 수행할 때 다음과 같은 새로운 기능이 포함됩니다.

* 단일 보기에서 여러 페이지의 마크업을 사용하여 단일 주석 작성

  이전에는 연속 보기 또는 매거진 보기에서만 가능했습니다

* 증명 썸네일을 통해 증명 탐색

   * 검토 중인 증명 부분을 쉽게 식별합니다. 이는 특히 사용자가 더 큰 형식 증명 및 긴 웹 페이지로 작업할 때 또는  세부 정보를 보려면 더 큰 확대/축소 레벨이 필요합니다.
   * 확대/축소 수준 변경
   * 콘텐츠 패닝

* 측정 도구에서 사용자 정의 값 지정
* Workfront Proof의 증명 뷰어에서 증명 내의 텍스트에 주석을 달 때 텍스트를 굵게, 기울임꼴 및 밑줄로 표시해야 함을 나타내는 옵션을 포함할 수 있습니다.

HTML5 뷰어는 현재 기존 Flash 뷰어에서 사용 가능한 모든 기능을 지원하지는 않습니다. 다음 기능은 현재 사용할 수 없지만 향후 릴리스에 포함될 예정입니다.

* 리치 미디어 파일 지원
* 비교 모드(비디오 및 정적)
* 댓글 필터링(비디오 및 정적)
* 문서의 하이퍼링크 검토(정적)
* 번역(비디오 및 정적)
* 현재 증명에서 작업 중인 사용자를 표시하는 현재 상태 표시기
* 증명 공유

HTML5 뷰어의 증명 정적 증명에 대한 자세한 내용은 를 참조하십시오.

Workfront Proof의 Workfront 관리자는 조직의 사용자가 비디오 증명에 대한 새 HTML5 증명 뷰어에 액세스할 수 있는지 여부를 결정할 수 있습니다.

## 새 간트 차트 재디자인 {#new-gantt-chart-redesign}

새 간트 차트에는 다음과 같은 개선 사항이 포함됩니다.

* 새 아이콘 및 마커
* 특정 시간대를 확대/축소하는 새로운 옵션
* 차트의 목록 부분에서 더 작은 작업 셀
* 설정, 인쇄 및 예상 날짜로 전환에 대한 옵션이 다시 디자인되었습니다.

간트 차트에서 옵션을 구성하는 방법에 대한 자세한 내용은 [간트 차트에 정보가 표시되는 방법 구성](../../../../manage-work/gantt-chart/use-the-gantt-chart/configure-info-on-gantt-chart.md)을 참조하십시오. 

## 기본 제공 보고서에는 업데이트된 설명이 포함되어 있습니다 {#built-in-reports-contain-updated-descriptions}

보고서 유형에 대한 정보와 포함된 필드를 포함하도록 Workfront에 있는 시스템 보고서에 대한 설명을 업데이트했습니다.  

이 변경 이전에는 대부분의 기본 제공 보고서에 설명이 없거나 매우 제한된 보고서가 있었습니다.

기본 제공 보고서에 대한 자세한 내용은 [Adobe Workfront 기본 제공 보고서 사용](../../../../reports-and-dashboards/reports/using-built-in-reports/use-workfront-built-in-reports.md)을 참조하세요.

## 내보낸 보고서, 목록 및 대시보드의 브랜딩 {#branding-in-exported-reports-lists-and-dashboards}

>[!NOTE]
>
>이 기능은 현재 미리보기 환경의 모든 클러스터에서 사용할 수 없습니다.

Workfront에서 브랜딩을 활용하는 경우 이제 전역 탐색 막대에서 사용 중인 로고가 Workfront에서 내보내는 .pdf 파일에 포함됩니다.

다음 .pdf 파일에는 내보낸 문서에 조직의 로고가 포함됩니다.

* 내보낸 목록
* 내보내고 게재된 보고서
* 인쇄된 대시보드

Workfront에서 데이터를 내보내는 방법에 대한 자세한 내용은 [데이터 내보내기](../../../../reports-and-dashboards/reports/creating-and-managing-reports/export-data.md)를 참조하십시오.

## 작업 복사 및 작업 또는 문제 이동 시 개선 사항 {#improvements-when-copying-tasks-and-moving-tasks-or-issues}

복사되거나 이동된 작업 또는 문제에 대한 상위 항목을 더 쉽게 선택할 수 있도록 작업을 복사하거나 작업 또는 문제를 이동하는 방법이 개선되었습니다. 예를 들어 작업을 복사하는 동안 상위 항목을 선택할 때 이제 상위-하위 관계가 있는 작업 계층을 볼 수 있을 뿐만 아니라 작업이 많은 프로젝트에서 상위 항목을 검색할 수 있습니다.

이 변경 전에 **상위 항목 선택** 단계에 검색 필드가 없었고 작업 목록에 작업 계층 구조가 표시되지 않았습니다.

작업 복사에 대한 자세한 내용은 [작업 복사 및 복제](../../../../manage-work/tasks/manage-tasks/copy-and-duplicate-tasks.md)를 참조하십시오.

문제 이동에 대한 자세한 내용은 [문제 이동](../../../../manage-work/issues/manage-issues/move-issues.md)을 참조하십시오.

## 승인 설정 영역에서 요청 회수를 위한 새 구성 {#new-configuration-for-recalling-requests-in-the-approval-settings-area}

Workfront 관리자가 사용자가 첫 번째 상태가 승인 보류 중인 문제 또는 요청을 상기할 수 있도록 허용할지 여부를 결정할 수 있도록 시스템 수준의 승인 설정 영역에 새 설정을 도입했습니다. 리콜이 허용되면 문제가 삭제됩니다. 리콜이 허용되지 않으면 문제의 첫 번째 상태가 승인 보류 중일 때 사용자에게 리콜 버튼이 표시되지 않습니다.

이 변경 이전에는 항상 이 문제에 대한 회수가 허용되었습니다. 승인이 회수되자 승인을 완전히 우회하여 사안을 아무런 승인이 첨부되지 않은 채 제1의 상태에 두었다.

승인 설정에 대한 자세한 내용은 [전역 승인 설정 구성](../../../../administration-and-setup/customize-workfront/configure-approval-milestone-processes/establish-approval-settings.md)을 참조하세요. 

>[!NOTE]
>
>이 기능이 릴리스되면 기본적으로 이 옵션이 비활성화됩니다. 현재 리콜 문제는 모든 조직에 대해 기본적으로 활성화되어 있습니다. 이 기능이 릴리스될 때 Workfront 관리자는 이 설정을 수동으로 활성화해야 Workfront의 기능을 그대로 유지할 수 있습니다.

## 자원 예산 시간 보고서의 신규 그룹화: 할당 일자 {#new-grouping-for-resource-budgeted-hour-reports-allocation-date}

리소스 예산 시간 보고서를 작성할 때 할당 날짜별로 결과를 그룹화하는 기능이 추가되었습니다.

이 변경 이전에는 보고서 보기에 할당 날짜를 표시하고 필터에서 사용할 수 있었지만 그룹화에서는 이 필드를 사용할 수 없었습니다.

할당 날짜에 대한 자세한 내용은 [Adobe Workfront 용어](../../../../workfront-basics/navigate-workfront/workfront-navigation/workfront-terminology-glossary.md)를 참조하십시오.

보고서 작성에 대한 자세한 내용은 [사용자 지정 보고서 만들기](../../../../reports-and-dashboards/reports/creating-and-managing-reports/create-custom-report.md)를 참조하십시오.

## 리소스 플래너 개선 사항 {#resource-planner-improvements}

* [리소스 플래너: FTE별로 데이터 표시](#resource-planner-show-data-by-fte)
* [리소스 플래너: 주 및 분기별 데이터 표시](#resource-planner-show-data-by-week-and-quarter)
* [리소스 플래너: 사용자별 보기](#resource-planner-view-by-user)
* [리소스 플래너: 프로젝트를 끌어다 놓아 우선 순위를 설정합니다](#resource-planner-drag-and-drop-projects-to-establish-priority)
* [리소스 플래너: 리소스 플래너의 데이터를 Excel로 내보내기](#resource-planner-export-the-data-in-the-resource-planner-to-excel)

### 리소스 플래너: FTE로 데이터 표시 {#resource-planner-show-data-by-fte}

이제 리소스 플래너에 FTE별로 리소스 할당 및 가용성을 표시할 수 있습니다. 이 변경 이전에는 값을 시간 단위로만 표시할 수 있었습니다.

리소스 플래너 사용에 대한 자세한 내용은 [리소스 플래너 개요](../../../../resource-mgmt/resource-planning/get-started-resource-planner.md)를 참조하십시오.

### 리소스 플래너: 주 및 분기별 데이터 표시 {#resource-planner-show-data-by-week-and-quarter}

이제 리소스 플래너의 시간대 간격을 변경하여 주 또는 분기별로 볼 수 있습니다. 이 변경 이전에는 리소스의 할당 및 가용성을 보고 월별 기준으로만 예산을 책정할 수 있었습니다.

리소스 플래너 사용에 대한 자세한 내용은 [리소스 플래너 개요](../../../../resource-mgmt/resource-planning/get-started-resource-planner.md)를 참조하십시오.

### 리소스 플래너: 사용자별 보기 {#resource-planner-view-by-user}

이제 리소스 플래너에 있는 정보를 사용자별로 먼저 표시한 다음 프로젝트, 역할 및 작업별로 표시할 수 있습니다. 사용자의 계획된 시간과 가용 시간 또는 FTE 간의 차이를 표시할 수도 있습니다. 이 변경 전에 리소스 플래너에 프로젝트 및 역할별로 정보를 표시할 수 있습니다.

리소스 플래너 사용에 대한 자세한 내용은 [리소스 플래너 개요](../../../../resource-mgmt/resource-planning/get-started-resource-planner.md)를 참조하십시오.

### 리소스 플래너: 프로젝트를 드래그하여 놓아 우선 순위 설정 {#resource-planner-drag-and-drop-projects-to-establish-priority}

이제 원하는 우선 순위 순서로 프로젝트를 드래그하여 놓을 수 있습니다. 이 변경 이전에는 수동으로 번호를 할당해야만 프로젝트의 우선 순위를 설정할 수 있었습니다.

리소스 플래너 사용에 대한 자세한 내용은 [리소스 플래너 개요](../../../../resource-mgmt/resource-planning/get-started-resource-planner.md)를 참조하십시오.

### 리소스 플래너: 리소스 플래너의 데이터를 Excel로 내보내기 {#resource-planner-export-the-data-in-the-resource-planner-to-excel}

이제 리소스 플래너의 정보를 Excel 파일로 내보낼 수 있습니다.

리소스 플래너 사용에 대한 자세한 내용은 [리소스 플래너 개요](../../../../resource-mgmt/resource-planning/get-started-resource-planner.md)를 참조하십시오.

## 모바일 개선 사항 {#mobile-improvements}

Workfront 모바일 앱에서 프로젝트에 액세스하고 프로젝트를 관리하는 기능이 추가되었습니다. 이제 Workfront 모바일 앱을 사용하여 다음을 수행할 수 있습니다.

* 프로젝트 목록 액세스
* 프로젝트의 작업 및 하위 작업 목록에 액세스
* 프로젝트의 문제 목록 액세스
* 프로젝트에 새 문제 기록

Workfront 모바일 앱을 업데이트할 때 이 기능을 설치할 수 있습니다. 업데이트는 2017년 11월에 Apple 및 Android 모바일 스토어 모두에서 사용할 수 있습니다.

## Slack과 Workfront 통합 {#workfront-integration-with-slack}

>[!NOTE]
>
>Slack 통합은 현재 사용할 수 없습니다. 프로덕션 환경에서는 2017년 11월에 사용할 수 있습니다.

Workfront과 Slack 간의 새로운 통합을 시작합니다. 조직에서 커뮤니케이션에 Slack을 이미 사용하고 있는 경우, 이제 Workfront과 통합하고 Slack의 커뮤니케이션 채널을 종료하지 않고 일반적인 Workfront 작업을 수행할 수 있습니다. 이제 Slack 계정에서 다음 작업을 수행할 수 있습니다.

* Workfront에서 항목 검색
* 작업 및 승인 목록 액세스
* 작업 만들기
* 문제 만들기
* 사용자와 공유되는 링크에서 해당 항목에 가입합니다
* 나와 공유된 링크의 작업 및 문제를 해당 사용자에게 할당
* 작업 승인
* 즐겨찾기 및 최근 항목 목록 액세스

Slack에서 Workfront에 액세스하는 방법에 대한 자세한 내용은 [Slack에서 Workfront 사용](https://support.workfront.com/hc/en-us/sections/115000458033)을 참조하십시오.

## Outlook 365 개선 사항 {#outlook-365-improvements}

용으로 Workfront 추가 기능이 다음과 같이 개선되었습니다.  Outlook 365:

* Workfront의 프로젝트에 작업 또는 문제 추가: 이제 Outlook 365 추가 기능을 사용하여 Workfront에서 이메일을 작업 또는 문제로 변환할 수 있습니다. 이 프로세스에서는 작업 또는 문제를 추가할 프로젝트, 할당자 및 기한을 지정할 수 있습니다. 이 개선 전에는 요청 대기열에만 요청을 제출하거나 Outlook 365에서 작업 중 목록에 개인 작업을 추가할 수 있었습니다. 
* 작업, 문제 또는 요청으로 전환된 원본 전자 메일에서 Workfront 개체에 대한 링크 유지: Outlook 365에서 작업, 문제 또는 요청으로 전자 메일을 변환할 때 Outlook 365에서는 원본 전자 메일 내에서 해당 전자 메일에서 전환된 작업 또는 문제에 대한 링크를 유지합니다. 이 변경 이전에는 Outlook에서 이메일이 작업으로 변환되었는지 또는 요청으로 제출되었는지 여부가 표시되지 않았습니다. 

## API 변경 사항 {#api-changes}

* [API 8을 사용할 수 있음](#api-8-now-available)
* [API의 제거된 버전 및 사용되지 않는 버전](#removed-and-deprecated-versions-of-the-api)
* [2017.3 Beta 최종 릴리스 활동](#updated-message-format-for-event-subscriptions)
* [전달할 수 없는 메시지에 대한 이벤트 구독 다시 시도](#event-subscription-retries-for-undeliverable-messages)

### 이제 API 8 사용 가능 {#api-8-now-available}

이제 Workfront API 버전 8을 사용할 수 있으며 Workfront 통합을 위한 새로운 리소스 및 업데이트된 리소스를 제공합니다.

Workfront API에 대한 변경 사항 목록은 [API 버전 업데이트](../../../../wf-api/api/new-api-version-8-updates.md)를 참조하십시오.

### API의 제거된 버전 및 사용되지 않는 버전 {#removed-and-deprecated-versions-of-the-api}

### 이벤트 구독에 대한 메시지 포맷 업데이트됨

Workfront 이벤트 구독 API를 포함하는 통합에 더 유용한 정보를 제공하기 위해 해당 리소스와 연결된 이전 값 및 새 값을 포함하여 지원되는 리소스에 대한 아웃바운드 메시지 형식을 변경했습니다. 실패를 방지하기 위해 Workfront 이벤트 구독 API를 사용하는 모든 통합은 [이벤트 구독 API](../../../../wf-api/general/event-subs-api.md)에 설명된 대로 새 형식을 업데이트해야 합니다.

### 전달할 수 없는 메시지에 대한 이벤트 구독 다시 시도 {#event-subscription-retries-for-undeliverable-messages}

이제 Workfront 이벤트 구독 프레임워크는 고객 엔드포인트에 전달되지 않는 이벤트 트리거 아웃바운드 메시지를 처리하기 위한 메커니즘을 제공합니다. 지속적인 메시지 전달을 위해 고객은 이벤트 구독의 아웃바운드 메시지를 사용하는 모든 엔드포인트가 올바르게 설정되었는지 확인해야 합니다. 자세한 내용은 [이벤트 구독 다시 시도](../../../../wf-api/api/event-sub-retries.md)를 참조하십시오.
