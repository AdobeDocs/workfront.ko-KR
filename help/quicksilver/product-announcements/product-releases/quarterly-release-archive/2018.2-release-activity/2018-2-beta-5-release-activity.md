---
content-type: release-notes
navigation-topic: product-releases-archive
title: 2018.2 Beta 5 릴리스 활동
description: 이 페이지에서는 2018.2 Beta 5 릴리스의 미리보기 환경에서 가장 최근에 사용할 수 있는 모든 변경 사항에 대해 설명합니다. 이 기능은 2018년 6월 1일에 미리보기 환경에서 사용할 수 있습니다. Beta 5와 함께 향상된 증명 기능은 6월 4일 월요일에 미리보기 환경에서 사용할 수 있습니다. 프로덕션 환경에서는 2018년 7월에 사용할 수 있습니다.
author: Luke
feature: Product Announcements
recommendations: noDisplay, noCatalog
exl-id: 0a8602aa-34c8-44d0-a102-9497d106f806
source-git-commit: b18a7835c6de131c125b77c6688057638c62fa4a
workflow-type: tm+mt
source-wordcount: '3158'
ht-degree: 1%

---

# 2018.2 Beta 5 릴리스 활동

이 페이지에서는 2018.2 Beta 5 릴리스의 미리보기 환경에서 가장 최근에 사용할 수 있는 모든 변경 사항에 대해 설명합니다. 이 기능은 2018년 6월 1일에 미리보기 환경에서 사용할 수 있습니다. Beta 5와 함께 향상된 증명 기능은 6월 4일 월요일에 미리보기 환경에서 사용할 수 있습니다. 프로덕션 환경에서는 2018년 7월에 사용할 수 있습니다.

>[!IMPORTANT]
>
> 이 페이지에 설명된 기능은 프로덕션 환경에서 사용하기 전에 변경될 수 있습니다.

2018.2의 모든 변경 사항 목록은 다음을 참조하십시오.  [2018.2 릴리스 활동 개요](../../../../product-announcements/product-releases/quarterly-release-archive/2018.2-release-activity/2018-2-release-activity-overview.md).

2018.2 Beta 5 릴리스에는 Workfront 관리자 및 기타 사용자를 위한 개선 사항이 포함되어 있습니다.

관리자용 **1&rbrace;**

* [감사 로그로 사용자가 트리거한 변경 내용 보기](#view-user-triggered-changes-with-audit-logs)
* [그룹 관리자로 라이선스 정보 보기](#view-license-information-as-a-group-administrator)

**모든 사용자용**

* [홈 영역의 달력 보기](#calendar-view-in-the-home-area)
* [홈의 작업 목록(왼쪽 패널)에 대한 추가 업데이트](#additional-updates-to-the-work-list-left-panel-in-home)
* [자동화된 리소스 예약에 대한 작업 역할 제한 구성](#configure-job-role-limits-for-automated-resource-scheduling)
* [리소스 플래너의 프로젝트 및 역할 보기 개선 사항](#project-and-role-view-improvements-in-the-resource-planner)
* [프로젝트 목록의 열 너비 조정](#resize-column-widths-for-project-lists)
* [새 프로젝트 목록에 대한 아이콘 지원](#icon-support-for-the-new-project-lists)
* [문서 보기에서 &quot;큰 축소판 그림&quot; 필드 추가](#add-large-thumbnail-field-in-document-views)
* [Excel 내보내기 제한 늘리기](#increase-excel-export-limit)
* [프로젝트 목록에 대한 빠른 필터](#quick-filters-for-project-lists)
* [프로젝트 및 작업 보고서에서 문제 컬렉션 참조](#reference-issue-collections-in-project-and-task-reports)
* [Workfront에서 새 문서 버전을 추가할 때 더 강력한 새 버전 메뉴](#new-more-robust-version-menu-when-adding-new-document-versions-in-workfront)
* [Android Beta 모바일 앱의 모바일 개선 사항](#mobile-improvements-in-the-android-beta-mobile-app)
* [증명 뷰어 개선 사항(Workfront 및 Workfront Proof)](#proofing-viewer-enhancements-workfront-and-workfront-proof)
* [Workfront의 증명 개선 사항](#proofing-enhancements-in-workfront)
* [Workfront Proof의 증명 개선 사항](#proofing-enhancements-in-workfront-proof)

## 홈 영역의 달력 보기 {#calendar-view-in-the-home-area}

이제 Workfront 홈 캘린더 보기를 사용하여 개인 작업 작업 및 일정을 관리할 수 있습니다. 홈 캘린더 보기에서 다음 작업을 수행할 수 있습니다.

* 자신에게 할당된 Workfront 작업 달성을 위한 나만의 일정 설정
* 기한이 지나거나 기한이 지난 작업을 빠르게 확인
* 1주일에 할당된 총 시간 보기
* 할당된 작업 업데이트

Outlook에서 일정을 사용하는 경우 일정을 통합하여 홈 일정 보기에서 Outlook 이벤트를 표시할 수 있습니다.

## 홈의 작업 목록(왼쪽 패널)에 대한 추가 업데이트 {#additional-updates-to-the-work-list-left-panel-in-home}

이제 홈 영역의 작업 목록에서 다음과 같은 향상된 기능을 사용할 수 있습니다.

* 이제 완료된 항목의 수가 필터 드롭다운 메뉴의 완료됨 옵션 옆에 괄호로 표시됩니다.

  이전에는 완료된 항목 수가 필터 메뉴에 표시되지 않았습니다. 

* 완료된 항목이 이전 2주 동안 표시됩니다.

  이전에는 완료된 항목이 이전 3개월 동안 표시되었습니다.

  홈 영역에서 완료된 작업을 보는 방법에 대한 자세한 내용은 문서 [홈 영역에서 작업 목록에 항목 표시](../../../../workfront-basics/using-home/using-the-home-area/display-items-in-home-work-list.md)에서 [홈 영역에서 작업 목록에 항목 표시](../../../../workfront-basics/using-home/using-the-home-area/display-items-in-home-work-list.md)를 참조하십시오.

* 홈 영역에서 항목을 선택할 때 표시할 기간 필드와 할당 필드를 추가합니다.

  이전에는 할당 필드를 기본적으로 사용할 수 있었지만 삭제했다면 다시 추가할 수 없었습니다. 이전에는 기간 필드를 추가할 수 없었습니다.

  홈 영역에 필드를 추가하는 방법에 대한 자세한 내용은 &quot;레이아웃 템플릿 만들기 및 관리&quot;를 참조하십시오.

홈 영역 사용에 대한 자세한 내용은 [홈 영역 사용](../../../../workfront-basics/using-home/using-the-home-area/use-the-home-area.md)을 참조하세요.

## 감사 로그를 사용하여 사용자가 트리거한 변경 사항 보기 {#view-user-triggered-changes-with-audit-logs}

사용자가 트리거한 변경 사항을 추적하기 위해 Workfront 관리자를 위한 다음과 같은 감사 로그를 만들었습니다.

* 사용자 감사 로그
* 액세스 수준 감사 로그
* 그룹 감사 로그
* 로그인 시도 감사 로그

이전에는 시스템 내에서 변경 사항을 추적할 방법이 없었습니다.

자세한 내용은 [감사 로그 보기 및 내보내기](../../../../administration-and-setup/add-users/create-and-manage-users/view-and-export-audit-logs.md)를 참조하십시오.

## 그룹 관리자로 라이선스 정보 보기 {#view-license-information-as-a-group-administrator}

그룹 관리자가 관리하는 그룹의 라이선스 수를 볼 수 있는 읽기 전용 라이선스 페이지를 만들었습니다.

이 변경 이전에는 그룹 관리자가 라이선스 정보를 볼 수 없었습니다.

자세한 내용은 [그룹 관리자](../../../../administration-and-setup/manage-groups/group-roles/group-administrators.md)를 참조하세요.

## 리소스 일정 자동 조정을 위한 작업 역할 제한 구성 {#configure-job-role-limits-for-automated-resource-scheduling}

>[!NOTE]
>
>리소스 예약 도구는 23.1 릴리스에서 더 이상 사용되지 않으며 Workfront에서 제거되었습니다. 업무 균형자를 사용하여 리소스를 예약하는 방법에 대한 자세한 내용은 [업무 균형자 개요](../../../../resource-mgmt/workload-balancer/overview-workload-balancer.md)를 참조하십시오.

이제 Automated Resource Scheduling 설정에서 작업 역할에 대한 제한을 할당할 수 있습니다. 이를 통해 작업 할당 시 동일한 역할을 가진 리소스의 수를 제어할 수 있습니다.

이전에는 특정 작업 역할 내에 작업을 할당할 수 있는 사용자 수를 지정할 수 없었습니다.

자세한 내용은 &quot;예약 영역에서 미할당 작업 및 문제 수동 할당&quot;을 참조하십시오.

## 리소스 플래너의 프로젝트 및 역할 보기 개선 사항 {#project-and-role-view-improvements-in-the-resource-planner}

이제 리소스 플래너의 프로젝트 및 역할 보기에 다음과 같은 개선 사항이 포함됩니다.

* 화면의 정보뿐만 아니라 전체 데이터베이스에서 정보를 가져오는 필터가 개선되었습니다.
* 전체 화면 모드.
* 이제 성능이 더 빠르고 효율적입니다.

   * 표시할 수 있는 프로젝트, 역할 및 사용자 수에 대한 새로운 제한.
   * 소극적 로드, 프로젝트 및 역할 로드 속도 향상.

* 리소스 플래너에서 바로 프로젝트 및 사용자에 대한 빠른 액세스.
* 프로젝트 보기에서 더 빠른 드래그 앤 드롭 기능으로 프로젝트의 우선 순위를 지정할 수 있습니다.

이러한 개선 사항에 앞서 리소스 플래너의 로드 속도가 느리고 표시된 데이터에서 부조화를 발견했다고 보고했습니다. 이러한 개선 사항을 통해 이제 이러한 문제를 제거해야 합니다.

리소스 플래너의 새로운 제한에 대한 자세한 내용과 이해는 [리소스 플래너 표시 제한](../../../../resource-mgmt/resource-planning/resource-planner-display-limitations.md)을 참조하십시오.

<!--
<p dir="ltr" data-mc-conditions="QuicksilverOrClassic.Draft mode">To participate in our current beta program and give us feedback on the functionality of the Resource Planner, see <a href="../../../../product-announcements/betas/resource-planner-performance-beta.md" class="MCXref xref" xrefformat="{para}">Resource Planner performance beta </a></p>
-->

## 프로젝트 목록의 열 너비 조정 {#resize-column-widths-for-project-lists}

목록의 기능을 개선하기 위해 노력하면서 다음 프로젝트 목록의 열 너비를 조정할 수 있는 기능을 일시적으로 비활성화했습니다.

* 내가 소유한 프로젝트
* 내가 진행 중인 프로젝트
* 모든 프로젝트

이번 릴리스에서는 모든 프로젝트 목록의 열 크기를 다시 조정할 수 있습니다.

이 기능에 대한 추가 개선 사항이 추가되었습니다.

이제 열의 크기를 조정하기 위해 열의 오른쪽 테두리를 드래그하면 오른쪽에 인접한 열의 크기가 그대로 유지되므로 목록도 수정되지 않고 더 넓게 표시됩니다. 또한 인접한 열의 테두리를 지나 오른쪽으로 열의 테두리를 끌 수도 있습니다.

이 개선 전에 크기가 조정된 열의 오른쪽에 있는 인접한 열의 크기가 화면에 맞게 비례적으로 조정되며 열 테두리를 인접한 열의 오른쪽 테두리를 지나 드래그할 수 없습니다.  

목록의 열 순서 조정 방법에 대한 자세한 내용은 [열 너비 및 순서 수정](../../../../reports-and-dashboards/reports/reporting-elements/modify-column-width-order.md)을 참조하십시오.

현재 목록 개선 사항에 대한 베타 테스트 프로그램에 참여하려면 [새 목록 연구를 참조하십시오.](https://experienceleaguecommunities.adobe.com/t5/workfront/ct-p/workfront?profile.language=ko)&#x200B;(로그인 필요)

## 새 프로젝트 목록에 대한 아이콘 지원 {#icon-support-for-the-new-project-lists}

목록의 기능을 개선하기 위해 노력하면서 다음 프로젝트 목록에서 상태 아이콘 표시를 일시적으로 비활성화했습니다.

* 내가 소유한 프로젝트
* 내가 진행 중인 프로젝트
* 모든 프로젝트

이번 릴리스를 통해 프로젝트의 프로젝트 목록 또는 프로젝트 목록의 다른 오브젝트에 상태 아이콘이 다시 표시될 수 있습니다.

목록에서 작업하는 방법에 대한 자세한 내용은 [Adobe Workfront에서 목록 시작](../../../../workfront-basics/navigate-workfront/use-lists/view-items-in-a-list.md)을 참조하세요.

## 문서 보기에서 &quot;큰 썸네일&quot; 필드 추가 {#add-large-thumbnail-field-in-document-views}

목록 또는 보고서의 문서 보기에 큰 축소판이라는 새 필드를 추가하고 있습니다. 문서 보기에서 선택한 경우 이 필드에는 목록 또는 보고서에 있는 문서의 400픽셀 전체 썸네일이 표시됩니다.

이 변경 이전에는 문서의 33-66픽셀 폭의 축소판을 표시하는 문서 보기에만 축소판 필드를 추가할 수 있었습니다.

목록 및 보고서의 필드에 대한 자세한 내용은 [Adobe Workfront 용어 설명](../../../../workfront-basics/navigate-workfront/workfront-navigation/workfront-terminology-glossary.md)을 참조하세요.

## Excel 내보내기 제한 늘리기 {#increase-excel-export-limit}

Excel 파일로 내보낼 수 있는 행 수에 대한 제한을 늘렸습니다. 이제 다음을 내보낼 수 있습니다.

* Excel .xls 파일의 65,000개 행
* Excel .xlsx 파일의 100,000개 행

새 제한은 Workfront에서 다음을 내보낼 때 적용됩니다.

* 웹 인터페이스의 목록 또는 보고서
* API를 사용하는 목록 또는 보고서
* 예약 및 게재된 보고서

이 개선 이전에는 모든 Excel 파일에서 50,000개의 행만 내보낼 수 있었습니다.

Workfront에서 데이터를 내보내는 방법에 대한 자세한 내용은 [데이터 내보내기](../../../../reports-and-dashboards/reports/creating-and-managing-reports/export-data.md)를 참조하십시오.

## 프로젝트 목록에 대한 빠른 필터 {#quick-filters-for-project-lists}

이제 목록에 빠른 필터를 적용할 수 있습니다.

빠른 필터의 목적은 중요한 큰 목록의 항목을 직접 탐색할 수 있도록 돕기 위한 것입니다. 이를 통해 빠른 검토, 업데이트 또는 다른 사람과 공유할 수 있습니다.

현재 빠른 필터는 다음 하위 탭의 프로젝트 목록에만 사용할 수 있습니다.

* 내가 진행 중인 프로젝트
* 내가 소유한 프로젝트
* 모든 프로젝트

빠른 필터에 대한 자세한 내용은 [Adobe Workfront 목록 시작](../../../../workfront-basics/navigate-workfront/use-lists/view-items-in-a-list.md)의 &quot;목록에 빠른 필터 적용&quot; 섹션을 참조하십시오.

## 프로젝트 및 작업 보고서에서 문제 컬렉션 참조 {#reference-issue-collections-in-project-and-task-reports}

이제 프로젝트 또는 작업 보기 및 필터에서 문제 컬렉션을 참조할 수 있습니다. 보고서를 작성하는 동안에는 텍스트 모드 를 사용해야만 할 수 있습니다.

이 개선 이전에는 프로젝트 보기 또는 필터에서 작업 컬렉션만 참조할 수 있었습니다.

보고서에서 컬렉션을 참조하는 방법에 대한 자세한 내용은 [보고서에서 컬렉션 참조](../../../../reports-and-dashboards/reports/text-mode/reference-collections-report.md)를 참조하십시오.

텍스트 모드 사용에 대한 자세한 내용은  [텍스트 모드의 일반적인 사용 개요](../../../../reports-and-dashboards/reports/text-mode/understand-common-uses-text-mode.md).

>[!NOTE]
>
>다음 비디오에서는 문제 컬렉션에 대한 샘플 텍스트 모드가 올바르지 않습니다. 보고서의 [참조 컬렉션](../../../../reports-and-dashboards/reports/text-mode/reference-collections-report.md)에서 올바른 샘플 텍스트 모드를 사용할 수 있습니다.

## Workfront에서 새 문서 버전을 추가할 때 더욱 강력한 새 버전 메뉴 {#new-more-robust-version-menu-when-adding-new-document-versions-in-workfront}

이제 Workfront의 문서에 새 버전을 추가할 때 새 버전 메뉴에는 추가 옵션이 포함되어 있으며 이제 Workfront 영역에서 새 버전을 추가할 수 있습니다.

Workfront의 다음 영역에서 새 문서 버전을 추가할 수 있습니다.

* 문서 탭의 기타 드롭다운 메뉴에서
* 문서 세부 정보 페이지의 문서 작업 메뉴에서
* 문서 세부 정보 페이지의 모든 버전 탭에서

이 변경 이전에는 문서 탭의 기타 드롭다운 메뉴에만 새 버전을 추가하기 위한 모든 옵션이 포함되어 있었습니다.

이제 새 버전을 추가할 수 있는 모든 영역에 대해 새 버전 메뉴에서 다음 옵션을 사용할 수 있습니다.

* 교정쇄
* 문서 전용
* 연결된 옵션(Dropbox, Google 드라이브 등)
* 클립보드에서 붙여넣기(버전을 추가할 때 새로운 옵션 사용)

자세한 내용은 문서 [파일 시스템에서 Adobe Workfront에 문서 추가](../../../../documents/adding-documents-to-workfront/add-documents-from-file-system.md)에서 [파일 시스템에서 Adobe Workfront에 문서 추가](../../../../documents/adding-documents-to-workfront/add-documents-from-file-system.md)를 참조하십시오.

## Android Beta 모바일 앱의 모바일 개선 사항 {#mobile-improvements-in-the-android-beta-mobile-app}

이 릴리스 당일 직후 모바일 앱의 Android Beta 버전에서 다음과 같은 개선 사항을 사용할 수 있습니다.

* 스와이프 동작

  Workfront 모바일 앱에서 다양한 오브젝트를 살짝 밀어 작업을 자원하거나, 작업을 완료하거나, 알림을 확인됨 또는 신규로 표시하거나, 텍스트를 입력하거나, 연락처를 호출하는 등의 활동을 수행할 수 있습니다.

  이 기능을 사용하여 다음 영역이 개선되었습니다.

   * 내 작업 및 홈
   * 알림
   * 연락처
   * 승인

* 항목의 세부 정보 탭을 볼 때의 새로운 모양과 느낌

  모바일 앱의 Android Beta 버전에서 항목을 보고, 편집하거나, 완료하거나, 문서를 첨부할 때 인터페이스가 변경되었습니다.

* 시간을 기록할 때의 새로운 경험

  로그 시간 버튼에 쉽게 액세스하고 시간을 로깅할 수 있도록 보다 간소화된 인터페이스를 통해 이전보다 로깅 시간이 빨라지고 간편해졌습니다.

이번 릴리스에서는 Workfront 모바일 앱의 Android Beta 버전에서만 이러한 개선 사항을 사용할 수 있습니다. 현재 iOS에서 사용할 수 없습니다.

베타 테스터에 등록하고 Android Beta 버전의 Workfront 모바일 앱을 다운로드하는 방법에 대한 자세한 내용은 을 참조하십시오.

## 증명 뷰어 개선 사항(Workfront 및 Workfront Proof) {#proofing-viewer-enhancements-workfront-and-workfront-proof}

* [인쇄 요약 페이지를 업데이트했습니다](#updated-print-summary-page)
* [증명 뷰어에서 직접 증명에 사용자 추가](#add-users-to-a-proof-directly-from-the-proofing-viewer)
* [증명 뷰어에 모든 마크업 도구 표시](#display-all-markup-tools-in-the-proofing-viewer)
* [증명 뷰어에서 기본 정렬 옵션 구성](#configure-default-sorting-options-in-the-proofing-viewer)
* [데스크톱 증명 뷰어에서 Workfront 문서 승인 보기](#view-workfront-document-approvals-in-the-desktop-proofing-viewer)
* [Desktop Proofing Viewer 내에서 새 탭과 창을 여는 링크 구성](#configure-links-that-open-new-tabs-and-windows-to-open-within-the-desktop-proofing-viewer)
* 증명 뷰어의 [현재 상태 표시기](#presence-indicator-in-the-proofing-viewer)
* [데스크톱 증명 뷰어에서 대화형 URL 증명에 대한 단일 페이지를 표시하도록 주석을 필터링](#filter-comments-to-display-a-single-page-for-interactive-url-proofs-in-the-desktop-proofing-viewer)
* 정적 및 비디오 콘텐츠에 대한 [데스크톱 증명 뷰어](#desktop-proofing-viewer-for-static-and-video-content)
* [시스템에 사용자 정의 장치 추가](#add-custom-devices-to-your-system)

### 인쇄 요약 페이지를 업데이트했습니다. {#updated-print-summary-page}

인쇄 요약 페이지가 새로운 모양과 느낌과 향상된 기능으로 업데이트되었습니다.

자세한 내용은 [Adobe Workfront 내에서 증명 요약 인쇄](../../../../review-and-approve-work/proofing/managing-proofs-within-workfront/print-proof-summary-in-wf.md)를 참조하십시오.

### 증명 뷰어에서 직접 증명에 사용자 추가 {#add-users-to-a-proof-directly-from-the-proofing-viewer}

이제 웹 증명 뷰어와 데스크탑 증명 뷰어에서 직접 증명에 사용자를 추가할 수 있습니다. 

이전에는 증명에 개별 사용자를 추가할 수 없었습니다. 대신 공개 URL 또는 포함 코드만 복사할 수 있습니다.

자세한 내용은 문서에서 [사용자를 추가하여 증명 공유](../../../../review-and-approve-work/proofing/reviewing-proofs-within-workfront/review-a-proof/share-a-proof-in-proofing-viewer.md#sharing-with-individual-users)를 참조하십시오.  [증명 뷰어에서 증명 공유](../../../../review-and-approve-work/proofing/reviewing-proofs-within-workfront/review-a-proof/share-a-proof-in-proofing-viewer.md).

### 증명 뷰어에 모든 마크업 도구 표시 {#display-all-markup-tools-in-the-proofing-viewer}

이제 열어야 하는 메뉴가 아니라 항상 표시하도록 마크업 도구를 구성할 수 있습니다. 이렇게 하면 도구 간 전환이 더 빨라집니다. 이러한 방식으로 구성된 경우 웹 증명 뷰어와 데스크탑 증명 뷰어의 맨 위에 마크업 도구가 가로로 표시됩니다.

이전에는 마크업 도구를 드롭다운 메뉴 내에서만 사용할 수 있었습니다.

이 마크업 설정 구성에 대한 자세한 내용은 [증명 뷰어 설정 구성](../../../../review-and-approve-work/proofing/reviewing-proofs-within-workfront/configure-proofing-viewer-settings.md)을 참조하십시오.

증명을 검토할 때 마크업 옵션을 사용하는 방법에 대한 자세한 내용은 문서 를 참조하십시오.

### 증명 뷰어에서 기본 정렬 옵션 구성 {#configure-default-sorting-options-in-the-proofing-viewer}

이제 증명의 주석 목록 내에서 정렬 옵션을 변경하면 다음에 웹 증명 뷰어 또는 데스크탑 증명 뷰어 내에서 증명을 열 때 이 옵션이 기본 정렬 옵션이 됩니다. 

자세한 내용은 이 문서에서 를 참조하십시오.

### Desktop Proofing Viewer에서 Workfront 문서 승인 보기 {#view-workfront-document-approvals-in-the-desktop-proofing-viewer}

이제 Desktop Proofing Viewer에서 Workfront 문서 승인 결정을 내릴 수 있습니다.

이전에는 웹 증명 뷰어에서만 Workfront 문서 승인 결정을 내릴 수 있었습니다. 

자세한 내용은  문서의 [증명 뷰어에서 증명에 대한 결정](../../../../review-and-approve-work/proofing/reviewing-proofs-within-workfront/make-a-decision-on-a-proof/make-decisions-on-proof.md)  [증명 뷰어에서 증명에 대한 결정을 내립니다](../../../../review-and-approve-work/proofing/reviewing-proofs-within-workfront/make-a-decision-on-a-proof/make-decisions-on-proof.md).

### Desktop Proofing Viewer에서 새 탭과 창을 여는 링크 구성 {#configure-links-that-open-new-tabs-and-windows-to-open-within-the-desktop-proofing-viewer}

이제 Desktop Proofing Viewer에서 대화형 내용을 교정할 때 Desktop Proofing Viewer 내에서 새 탭이나 새 창에서 열리는 링크를 구성하여 교정을 계속할 수 있습니다.

기존 증명 뷰어에서는 새 탭이나 새 창에서 연 링크를 증명 뷰어에서 검토할 수 없었습니다.

자세한 내용은 [증명 뷰어 설정 구성](../../../../review-and-approve-work/proofing/reviewing-proofs-within-workfront/configure-proofing-viewer-settings.md)을 참조하십시오.

### 증명 뷰어의 현재 상태 표시기 {#presence-indicator-in-the-proofing-viewer}

이제 웹 증명 뷰어 또는 데스크탑 증명 뷰어에서 증명을 검토할 때 현재 증명을 보고 있는 각 사용자의 아바타가 증명 뷰어의 오른쪽 상단 모서리에 표시되는 것을 볼 수 있습니다.

자세한 내용은 [여러 검토자와 동시에 증명 검토](../../../../workfront-proof/wp-work-proofsfiles/review-proofs-wpv/review-proof-with-multiple-reviewers.md)를 참조하십시오.

### 주석을 필터링하여 데스크탑 증명 뷰어에서 대화형 URL 증명에 대한 단일 페이지를 표시 {#filter-comments-to-display-a-single-page-for-interactive-url-proofs-in-the-desktop-proofing-viewer}

이제 Desktop Proofing Viewer에서 대화형 증명의 URL을 검토할 때 주석을 필터링하여 현재 페이지에서만 작성된 주석을 표시할 수 있습니다. 

이 변경 이전에는 정적 증명에만 이 옵션을 사용할 수 있었습니다.

자세한 내용은 이 문서에서 를 참조하십시오.

### 정적 및 비디오 콘텐츠에 대한 데스크톱 증명 뷰어 {#desktop-proofing-viewer-for-static-and-video-content}

이제 Desktop Proofing Viewer에서 정적 및 비디오 콘텐츠를 지원합니다.

이전에는 대화형 컨텐츠만 지원했습니다.

데스크톱 증명 뷰어에서 열도록 정적 증명 및 비디오 증명을 구성하는 방법에 대한 자세한 내용은 [증명 뷰어 설정 구성](../../../../review-and-approve-work/proofing/reviewing-proofs-within-workfront/configure-proofing-viewer-settings.md)을 참조하십시오.

Desktop Proofing Viewer에 대한 자세한 내용은 [Desktop Proofing Viewer에서 증명 검토](https://support.workfront.com/hc/en-us/sections/360000686434)를 참조하십시오.

### 시스템에 사용자 정의 장치 추가 {#add-custom-devices-to-your-system}

이제 사용자 정의 장치를 시스템에 추가하여 사용자가 Desktop Proofing Viewer에서 증명을 검토할 때 대화형 콘텐츠를 검토하고 특정 장치에 표시되는 방식을 시뮬레이션할 수 있습니다.

이 변경 이전에는 사용자가 사전 구성된 표준 디바이스 목록에서만 선택할 수 있었습니다.

사용자 지정 장치 추가에 대한 자세한 내용은

사용자가 대화형 콘텐츠를 검토할 때 장치를 선택할 수 있는 방법에 대한 자세한 내용은 [증명 뷰어에서 대화형 증명 해상도 변경](../../../../review-and-approve-work/proofing/reviewing-proofs-within-workfront/review-a-proof/view-interactive-content-as-it-appears-in-device.md)을 참조하십시오.

## Workfront의 증명 개선 사항 {#proofing-enhancements-in-workfront}

* [Workfront에서 직접 증명 링크 공유](#share-the-proof-link-directly-from-workfront)
* [Workfront의 추가 증명 데이터에 대해 보고](#report-on-additional-proofing-data-in-workfront)
* [Workfront에서 증명 승인을 위한 내역 데이터 보기](#view-historical-data-for-proof-approvals-in-workfront)

### Workfront에서 바로 증명 링크 공유 {#share-the-proof-link-directly-from-workfront}

이제 Workfront 내에서 증명에 대한 링크를 생성하고 Workfront에서 직접 공유할 수 있습니다. 또는 URL을 복사하여 대체 방법을 사용하여 배포할 수 있습니다.

이 변경 이전에는 Workfront 내에서만 증명 링크를 복사하고 대체 방법을 사용하여 배포할 수 있었습니다.

자세한 내용은 문서 [Adobe Workfront 내에서 증명 공유](../../../../review-and-approve-work/proofing/managing-proofs-within-workfront/share-a-proof-in-workfront.md)에서 [Adobe Workfront 내에서 증명 공유](../../../../review-and-approve-work/proofing/managing-proofs-within-workfront/share-a-proof-in-workfront.md)를 참조하십시오.

>[!NOTE]
>
>현재 사용할 수 있는 포함 링크는 향후 릴리스에서 제거됩니다. 포함 링크는 Workfront API를 통해 계속 액세스할 수 있습니다.

### Workfront의 추가 증명 데이터에 대한 보고서 {#report-on-additional-proofing-data-in-workfront}

문서 버전 보고서 및 증명 승인 보고서와 같이 문서 버전 개체가 포함된 보고서에서 추가 증명 정보를 볼 수 있는 여러 필드를 사용할 수 있습니다.

* 교정 기한

  증명 기한의 요일, 날짜, 시간 및 연도를 표시합니다.

* 교정 결정

  증명의 결정 상태(보류 중, 변경 필수 또는 승인됨)를 표시합니다.

* 교정쇄 이름

  증명 이름을 표시합니다.

* 교정쇄 페이지

  증명에 포함된 페이지 수를 표시합니다.

* 교정 진행 상황

  증명의 진행 상태(전송됨, 열림, 설명됨, 결정됨)를 표시합니다.

이러한 각 필드에 대한 자세한 내용은  [Adobe Workfront 용어](../../../../workfront-basics/navigate-workfront/workfront-navigation/workfront-terminology-glossary.md).

### Workfront에서 증명 승인을 위한 내역 데이터 보기 {#view-historical-data-for-proof-approvals-in-workfront}

증명 승인 보고서에서 더 이상 활성화되지 않은 증명에 대한 증명 승인 결정을 볼 수 있는 필드를 추가할 수 있습니다. 승인자 결정 필드를 보고서에 추가하여 이 작업을 수행할 수 있습니다.

이 변경 이전에는 증명에 대한 결정이 내려진 후 해당 결정을 더 이상 Workfront 보고서에 표시할 수 없었습니다.

자세한 내용은  [Adobe Workfront 용어](../../../../workfront-basics/navigate-workfront/workfront-navigation/workfront-terminology-glossary.md).

## Workfront Proof의 증명 개선 사항 {#proofing-enhancements-in-workfront-proof}

* [증명 뷰어(Workfront Proof)에서 직접 새 증명 버전을 만듭니다](#create-a-new-version-of-a-proof-directly-from-the-proofing-viewer-workfront-proof)
* [증명 뷰어 및 데스크탑 증명 뷰어의 새 증명 세부 정보 링크(Workfront Proof)](#new-proof-details-link-in-the-proofing-viewer-and-desktop-proofing-viewer-workfront-proof)

### 증명 뷰어에서 직접 증명의 새 버전 만들기(Workfront Proof) {#create-a-new-version-of-a-proof-directly-from-the-proofing-viewer-workfront-proof}

이제 Workfront Proof 내에서 증명을 수행할 때 새 증명 뷰어와 데스크탑 증명 뷰어에서 직접 새 증명 버전을 생성할 수 있습니다.

이전에는 이 옵션을 레거시 Flash 뷰어 내에서만 사용할 수 있었습니다.

자세한 내용은 문서에서 [Workfront Proof에서 증명 복사](../../../../workfront-proof/wp-work-proofsfiles/create-proofs-and-files/copy-proofs.md)를 참조하십시오.  [Workfront Proof에서 증명 복사](../../../../workfront-proof/wp-work-proofsfiles/create-proofs-and-files/copy-proofs.md).

### 증명 뷰어 및 데스크탑 증명 뷰어의 새 증명 세부 정보 링크(Workfront Proof) {#new-proof-details-link-in-the-proofing-viewer-and-desktop-proofing-viewer-workfront-proof}

이제 Workfront Proof 사용자가 증명 뷰어에서 증명을 볼 때 Workfront Proof 내의 증명 세부 정보 페이지로 빠르게 이동할 수 있습니다.

자세한 내용은 &quot;증명 세부 정보 보기&quot;를 참조하십시오.
