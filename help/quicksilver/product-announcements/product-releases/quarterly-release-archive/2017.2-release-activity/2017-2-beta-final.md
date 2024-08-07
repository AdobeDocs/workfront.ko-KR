---
content-type: release-notes
navigation-topic: product-releases-archive
title: 2017.2 Beta 결승전
description: 이 페이지에서는 2017.2 릴리스의 미리보기 환경에서 가장 최근에 사용할 수 있는 모든 변경 사항에 대해 설명합니다. 이 페이지의 기능은 2017년 6월 28일에 미리보기 환경에서 사용할 수 있습니다. 프로덕션 환경에서는 2017년 7월 26일에 사용할 수 있습니다.
author: Luke
feature: Product Announcements
recommendations: noDisplay, noCatalog
exl-id: 768e9aad-d7e7-4a3c-9f93-926cf588ddc7
source-git-commit: f1e463c90641f9221228e335b583cab72762b3bd
workflow-type: tm+mt
source-wordcount: '2314'
ht-degree: 0%

---

# 2017.2 Beta 결승전

이 페이지에서는 2017.2 릴리스의 미리보기 환경에서 가장 최근에 사용할 수 있는 모든 변경 사항에 대해 설명합니다. 이 페이지의 기능은 2017년 6월 28일에 미리보기 환경에서 사용할 수 있습니다. 프로덕션 환경에서는 2017년 7월 26일에 사용할 수 있습니다.

>[!IMPORTANT]
>
>이 페이지에 설명된 기능은 프로덕션 환경에서 사용하기 전에 변경될 수 있습니다.

2017.2의 모든 변경 사항 목록은 [2017.2 릴리스 활동 개요](../../../../product-announcements/product-releases/quarterly-release-archive/2017.2-release-activity/2017-2-release-activity-overview.md)를 참조하십시오.

2017.2 Beta 최종 릴리스에는 Workfront 관리자와 기타 사용자를 위한 개선 사항이 포함되어 있습니다.

**관리자용:**

* [HTML5 비디오 증명 뷰어(ProofHQ 및 Workfront)의 사용 가능 여부 확인](#determine-the-availability-of-the-html5-video-proofing-viewer-proofhq-and-workfront)
* [SAML 2.0에 대한 SHA-256 인증서 지원](#support-sha-256-certificates-for-saml-2-0)
* [특성 매핑에 대해 미리 입력](#type-ahead-for-mapping-attributes)
* [API 개선 사항: 사용자 할당에 액세스](#api-enhancement-access-user-allocations)

**모든 사용자의 경우:**

* [리소스 플래너](#resource-planner)
* [프로젝트의 새 일정 영역(팀 빌더)](#new-scheduling-area-in-a-project-team-builder)
* [리소스 예약: 기본적으로 더 적은 항목 표시](#resource-scheduling-show-fewer-items-by-default)
* [리소스 예약: 작업 및 문제를 드래그할 때 드롭 표시기 및 초과 할당 표시](#resource-scheduling-display-drop-indicator-and-over-allocation-when-dragging-tasks-and-issues)
* [리소스 예약: 사용자 할당이 더 이상 가장 가까운 30분으로 반올림되지 않습니다](#resource-scheduling-user-allocations-are-no-longer-rounded-to-the-nearest-half-hour)
* [TSV 및 PDF 형식으로 사용률 보고서 내보내기](#export-the-utilization-report-in-tsv-and-pdf-formats)
* [2017.2 Beta Final](#user-calendar-enhancements-in-the-my-work-area%22)
* [2017.2 Beta Final](#layout-template-determines-whether-the-new-or-legacy-calendar-displays-in-the-my-work-area)
* [증명 결정이 내 작업 영역(Workfront)에 표시됨](#proof-decision-displays-in-the-my-work-area-workfront)
* [사전 설정 해상도(ProofHQ 및 Workfront)에서 리치 미디어 증명 보기](#view-rich-media-proofs-in-preset-resolutions-proofhq-and-workfront)
* [리치 미디어 증명(ProofHQ 및 Workfront)에 대한 댓글에서 하위 페이지에 대한 URL 보기](#view-url-to-sub-pages-in-comments-on-rich-media-proofs-proofhq-and-workfront)
* [기존 표준 보기(ProofHQ)를 기반으로 사용자 지정 보기 만들기](#create-custom-views-based-on-existing-standard-views-proofhq)
* [보고 영역(ProofHQ) 필터링](#filter-the-reporting-area-proofhq)
* [보고서에 최소값 및 최대값 표시(ProofHQ)](#display-minimum-and-maximum-values-in-reports-proofhq)
* [증명 승인을 위한 인앱 알림](#in-app-notification-for-proof-approval)
* [모바일 개선 사항](#mobile-improvements)
* 쉼표를 포함하는 필드 값의 필터 문에 [슬래시가 추가됨](#slash-added-to-filter-statements-for-field-values-that-contain-commas)
* [여러 청구 요금](#multiple-billing-rates)
* [새 리소스 예산 시간 필드](#new-resource-budgeted-hour-field)
* [작업 및 문제에 대한 세부 정보 페이지의 &#39;할당 대상&#39; 영역에 사용자 작업 역할 표시](#show-user-job-role-in-assigned-to-area-on-the-details-page-for-tasks-and-issues)

>[!NOTE]
>
>리소스 예약 도구는 23.1 릴리스에서 더 이상 사용되지 않으며 Workfront에서 제거되었습니다. 업무 균형자를 사용하여 리소스를 예약하는 방법에 대한 자세한 내용은 [업무 균형자 개요](../../../../resource-mgmt/workload-balancer/overview-workload-balancer.md)를 참조하십시오.

## 프로젝트의 새 일정 영역(팀 빌더) {#new-scheduling-area-in-a-project-team-builder}

프로젝트의 예약 영역(이전의 팀 빌더)이 업데이트되고 보다 직관적인 사용자 인터페이스로 다시 디자인되었습니다. 이제 새로운 예약 기능이 Workfront의 다른 영역에서 현재 사용할 수 있는 리소스 예약 기능과 더 가깝게 일치합니다.

향상된 기능은 다음과 같습니다.

* 프로젝트 팀원의 현재 리소스 할당을 보고 할당시 보다 현명한 결정을 내릴 수 있습니다.
* 예약 타임라인에서 작업 기간을 시각적으로 표시
* 예약 타임라인에 표시된 정보 필터링
* 예약 타임라인에서 바로 프로젝트 팀에 사용자를 쉽게 추가하고 제거할 수 있습니다.

다음 기능은 리소스를 예약할 때 도구의 다른 영역에서 사용할 수 있지만 팀 예약 영역에서 리소스를 예약할 때는 사용할 수 없습니다.

* 일정 타임라인에 표시할 상위 작업 구성
* 예약 타임라인에 표시할 프로젝트 이름 구성
* 교체 도구를 사용하여 사용자 지정 수정
* 포트폴리오, 프로그램 및 프로젝트로 필터링

팀 예약 영역에서 사용할 수 있는 기능에 대한 자세한 내용은 &quot;리소스 예약 시작&quot;을 참조하십시오.

## 리소스 예약: 기본적으로 더 적은 항목 표시 {#resource-scheduling-show-fewer-items-by-default}

기본적으로 이제 지정된 사용자의 예약 타임라인에 하루에 최대 10개의 작업 항목이 표시됩니다. 목록을 확장하여 해당 사용자에게 현재 할당된 모든 작업 및 문제를 볼 수 있습니다.

이를 통해 사용자에게 많은 작업과 문제가 할당되었을 때 예약 타임라인을 보다 쉽게 찾아볼 수 있습니다.

이 변경 이전에는 모든 작업 및 문제가 항상 모든 사용자에 대해 표시되었습니다.

예약 타임라인에서 사용자에게 작업 및 문제를 할당하는 방법에 대한 자세한 내용은 &quot;예약 영역에서 할당 해제된 작업 및 문제 수동으로 할당&quot;을 참조하십시오.

## 리소스 예약: 작업 및 문제를 드래그할 때 드롭 표시기 및 초과 할당 표시 {#resource-scheduling-display-drop-indicator-and-over-allocation-when-dragging-tasks-and-issues}

드래그 앤 드롭을 통해 예약 타임라인의 사용자에게 작업 또는 문제를 할당할 때 이제 작업 또는 문제를 릴리스하고 할당을 완료하기 전에 다음 정보가 표시됩니다.

* 사용자의 행에 드롭 표시기가 표시됩니다. 이렇게 하면 할당하기 전에 항목이 지정되는 위치를 확인할 수 있습니다.
* 사용자 할당이 스케줄링 타임라인에서 활성화된 경우 할당을 완료하면 사용자가 초과 할당되면 빨간색 초과 할당 표시기가 표시됩니다.

이러한 변경 이전에는 작업 또는 문제를 릴리스하기 전에 정보가 표시되지 않았습니다.

예약 타임라인에서 사용자에게 작업 및 문제를 할당하는 방법에 대한 자세한 내용은 &quot;예약 영역에서 할당 해제된 작업 및 문제 수동으로 할당&quot;을 참조하십시오.

## 리소스 예약: 사용자 할당이 더 이상 가장 가까운 30분으로 반올림되지 않음 {#resource-scheduling-user-allocations-are-no-longer-rounded-to-the-nearest-half-hour}

여러 사용자가 작업 또는 문제에 할당되거나 작업 또는 문제가 여러 날에 걸쳐 수행되는 경우 Workfront은 할당된 사용자와 일 간에 계획된 시간을 균등하게 분배하려고 합니다. 시간은 기본적으로 가장 가까운 100분의 1로 반올림됩니다(예: 1.33).

이전에는 분산 시간을 수동으로 수정하면 시간이 조정되고 가장 가까운 30분으로 반올림되었습니다(예: 1.33은 1.5로 반올림됨).

이제 시간이 더 이상 조정되지 않고 가장 가까운 30분으로 반올림됩니다(예: 1.33은 1.33으로 남음).

## API 개선 사항: 사용자 할당에 액세스 {#api-enhancement-access-user-allocations}

이제 Workfront API를 통해 사용자 할당 음영에 액세스할 수 있습니다.

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">For more information, see <a href="../../../../wf-api/api/access-proj-allocation-info-api.md" class="MCXref xref" xrefformat="{para}">Access Project Allocation Information via the API</a>.</p>
-->

## TSV 및 PDF 형식으로 활용성 보고서 내보내기 {#export-the-utilization-report-in-tsv-and-pdf-formats}

이제 XLSX 형식 외에도 TSV 및 PDF 형식으로 프로젝트에 대한 사용률 보고서를 내보낼 수 있습니다.

이 변경 이전에는 활용성 보고서를 XLSX 형식으로만 내보낼 수 있었습니다.

사용률 보고서 내보내기에 대한 자세한 내용은 [리소스 사용률 보고서 개요](../../../../reports-and-dashboards/reports/using-built-in-reports/resource-utilization-report.md)의 [리소스 사용률 보고서 개요](../../../../reports-and-dashboards/reports/using-built-in-reports/resource-utilization-report.md)를 참조하십시오.

## 증명 결정이 내 작업 영역(Workfront)에 표시됨 {#proof-decision-displays-in-the-my-work-area-workfront}

이제 [내 작업] 영역의 [내 승인] 탭에서 증명 승인을 볼 때 증명 결정이 [내 작업] 영역에 표시되고 Workfront 내의 새 새로 고침 단추를 클릭할 때까지 또는 다음 번에 브라우저 페이지를 새로 고칠 때까지 유지됩니다.

이 변경 이전에는 증명에 대한 결정이 이미 결정되었음을 나타내는 표시가 없었고, 증명이 브라우저를 새로 고칠 때까지 내 승인 탭에 남아 있었습니다.

자세한 내용은 [작업 승인](../../../../review-and-approve-work/manage-approvals/approving-work.md)에서 [작업 승인](../../../../review-and-approve-work/manage-approvals/approving-work.md)을 참조하세요.

## 사전 설정 해상도로 리치 미디어 증명 보기(ProofHQ 및 Workfront) {#view-rich-media-proofs-in-preset-resolutions-proofhq-and-workfront}

미리보기 환경에 대한 이전 릴리스에서는 사용자 지정 해상도를 지정하거나 이미지를 원하는 해상도로 드래그하여 리치 미디어 증명의 해상도를 조정하는 기능이 도입되었습니다.

이제 다양한 휴대폰, 태블릿, 노트북 및 데스크탑의 사전 설정된 해상도 옵션 중에서 선택할 수 있습니다.

자세한 내용은 [증명 뷰어에서 대화형 증명 해상도 변경](../../../../review-and-approve-work/proofing/reviewing-proofs-within-workfront/review-a-proof/view-interactive-content-as-it-appears-in-device.md)의 &quot;사전 설정 해상도 보기&quot;를 참조하십시오.

## 리치 미디어 증명(ProofHQ 및 Workfront)에 대한 댓글에서 하위 페이지에 대한 URL 보기 {#view-url-to-sub-pages-in-comments-on-rich-media-proofs-proofhq-and-workfront}

>[!NOTE]
>
>이 기능은 현재 프로덕션 환경에서 사용할 수 있습니다.

이제 Rich Media 증명에서 하위 페이지에 댓글을 달면 해당 하위 페이지의 URL이 댓글에 표시됩니다.

이 변경 이전에는 댓글이 어느 하위 페이지를 지칭하는지 명확하지 않았습니다.

자세한 내용은

## HTML5 비디오 증명 뷰어(ProofHQ 및 Workfront)의 가용성 확인 {#determine-the-availability-of-the-html5-video-proofing-viewer-proofhq-and-workfront}

ProofHQ의 Workfront 관리자는 조직의 사용자가 비디오 증명에 대한 새 HTML5 증명 뷰어에 액세스할 수 있는지 여부를 결정할 수 있습니다.

Workfront에서 이 옵션을 구성하는 방법에 대한 자세한 내용은에서 를 참조하십시오.

## 기존 표준 보기(ProofHQ)를 기반으로 맞춤형 보기 생성 {#create-custom-views-based-on-existing-standard-views-proofhq}

이제 표준 보기를 기반으로 하여 사용자 지정 보기를 만들 수 있습니다. 표준 보기의 열, 정렬 및 필터 옵션은 기본적으로 새 보기에 포함됩니다.

이 변경 전에 사용자 지정 보기를 만들려면 처음부터 보기를 만들어야 했습니다. 

자세한 내용은 [Workfront Proof Proof에서 사용자 지정 보기 만들기 및 관리](../../../../workfront-proof/wp-work-proofsfiles/manage-your-work/create-and-manage-custom-views.md)에서 [사용자 지정 보기 만들기](../../../../workfront-proof/wp-work-proofsfiles/manage-your-work/create-and-manage-custom-views.md#creating)를 참조하십시오.

## 보고 영역 필터링(ProofHQ) {#filter-the-reporting-area-proofhq}

기본적으로 보고서 탭에 표시되는 데이터에는 ProofHQ 시스템의 모든 정보가 포함됩니다. 이제 필터를 사용하여 요구 사항과 관련된 정보만 표시할 수 있습니다. 

자세한 내용은 [보고서 필터링](../../../../workfront-proof/wp-work-proofsfiles/manage-your-work/run-reports.md#filtering-reports)을 참조하세요.  [Workfront Proof에서 보고서 실행](../../../../workfront-proof/wp-work-proofsfiles/manage-your-work/run-reports.md).

## 보고서에 최소값 및 최대값 표시(ProofHQ) {#display-minimum-and-maximum-values-in-reports-proofhq}

이제 보고서를 볼 때 그래프에 최소값과 최대값을 표시할지 여부를 구성할 수 있습니다.

자세한 내용은 [보고서 보기](../../../../workfront-proof/wp-work-proofsfiles/manage-your-work/run-reports.md#viewing-reports)를 참조하세요.  [Workfront Proof에서 보고서 실행](../../../../workfront-proof/wp-work-proofsfiles/manage-your-work/run-reports.md).

## SAML 2.0용 SHA-256 인증서 지원 {#support-sha-256-certificates-for-saml-2-0}

이제 SAML 2.0으로 SSO용 Workfront을 구성할 때 보안 해시 알고리즘 256(SHA-256)을 지원합니다. 이 릴리스 이전에는 SHA-1(Secure Hash Algorithm 1)만 지원했습니다.

SAML 2.0을 사용하여 Workfront을 구성하는 방법에 대한 자세한 내용은 [SAML 2.0을 사용하여 Adobe Workfront 구성](../../../../administration-and-setup/add-users/single-sign-on/configure-workfront-saml-2.md)을 참조하십시오.

## 속성 매핑을 위해 미리 입력 {#type-ahead-for-mapping-attributes}

속성 매핑(Attribute Mapping) 대화상자의 기본값(Default Value) 필드 유형이 자동 완성(type-ahead) 필드로 업데이트되었습니다. 이 변경 이전에는 기본값 필드의 유형이 드롭다운이었습니다.

이 변경 사항은 다음 SSO 프로토콜에 적용됩니다.

* Active Directory
* LDAP
* SAML 2.0

SAML 1.1은 속성 매핑을 지원하지 않습니다.

## 모바일 개선 사항 {#mobile-improvements}

>[!NOTE]
>
> 모바일 애플리케이션은 기본 Workfront 애플리케이션과 별도로 릴리스됩니다. 이 섹션에 설명된 기능은 8월 초에 릴리스됩니다.

모바일 앱에서 Android 및 iOS 플랫폼 모두에 대해 다음과 같은 추가 기능이 표시됩니다.

* 모바일 앱에서 요청 제출
* 모바일 앱의 타임시트 새 항목
* 모바일 앱에서 사용자 정의 양식 편집
* 모바일 앱의 증명 승인 요청

Android 플랫폼용 이러한 기능 중 일부에 대한 공개 베타 프로그램이 있을 예정입니다.

모바일용 베타 프로그램에 대한 자세한 내용은  [&quot;베타&quot;](https://support.workfront.com/hc/en-us/sections/115000743248) 페이지입니다.

Workfront 모바일 앱 사용에 대한 자세한 내용은 을 참조하십시오.  

## 쉼표를 포함하는 필드 값의 필터 문에 슬래시가 추가됨 {#slash-added-to-filter-statements-for-field-values-that-contain-commas}

텍스트 모드에서 필터를 작성하고 쉼표를 포함하는 필드 값을 필터링할 때 값을 구분하는 쉼표 앞에 슬래시(&quot;/&quot;)를 추가하여 값을 하나의 필터 옵션으로 읽도록 해야 합니다. 이는 다음 필드 유형에만 적용됩니다.

* 드롭다운
* 라디오 버튼
* 확인란

이 변경 이전에는 쉼표가 포함된 옵션이 있는 필드를 필터링할 수 없었습니다.

이 변경 내용에 대한 자세한 내용은 [필터 개요](../../../../reports-and-dashboards/reports/reporting-elements/filters-overview.md)를 참조하십시오.

## 여러 청구 요금 {#multiple-billing-rates}

이제 프로젝트 수준의 동일한 작업 역할에 대해 여러 청구 요금 재정의를 추가할 수 있습니다. 이 새로운 기능을 사용하면 각 청구 요금 재정의에 대한 날짜 범위를 정의할 수 있습니다. 지정된 날짜 범위 동안 프로젝트의 작업에 할당된 작업 역할에는 다른 청구 요금이 적용됩니다. 청구 요금에 프로젝트의 시간을 곱하여 수익을 계산합니다. 청구 요금의 날짜 범위 내에서 계산된 매출은 해당 요금에 잠긴 상태를 유지하며 프로젝트 업데이트에 대한 작업 역할의 요율로 업데이트되지 않습니다. 실제 매출의 경우 청구 요금을 재정의하기 전에 기록된 시간이 현재 청구 요금을 반영하도록 다시 계산되지 않습니다. 청구 요금 재정의가 프로젝트에 추가되기 전에 기록된 시간은 해당 시점의 작업 역할 청구 요율과 연결됩니다.

이 변경 이전에는 작업 역할의 청구 요금을 한 번만 재정의할 수 있었으며, 청구 요금이 변경되기 전에 기록된 모든 시간에 대한 현재 청구 요금을 반영하도록 실제 수익 이 다시 계산됩니다.

청구 요금 및 매출에 대한 자세한 내용은 [청구 및 매출 개요](../../../../manage-work/projects/project-finances/billing-and-revenue-overview.md)를 참조하십시오.

프로젝트 수준의 작업 역할에 대한 청구 요율 재정의에 대한 자세한 내용은 [작업 역할 청구 요율 재정의 개요 및 프로젝트의 수익 계산](../../../../manage-work/projects/project-finances/override-role-billing-rates-and-calculate-project-revenue.md)을 참조하십시오.

## 리소스 플래너 {#resource-planner}

이번 릴리스에서는 사람 영역의 새 계획 탭 재설계의 일부인 리소스 플래너의 첫 번째 단계를 소개합니다. 리소스 플래너를 사용하면 리소스 풀의 사용자가 리소스 관리자인 현재 모든 프로젝트에 할당되는 시간을 예산으로 책정할 수 있습니다. 리소스 플래너에서 프로젝트, 작업 역할 및 사용자별로 다음 할당 번호를 볼 수 있습니다.

* 사용 가능한 시간
* 계획된 시간
* 예산 시간
* 시간 차이(예산 시간과 계획 시간 사이)
* 순 시간 차이(가용 시간과 예산 시간 간)

리소스 플래너 사용에 대한 자세한 내용은 [리소스 플래너 개요](../../../../resource-mgmt/resource-planning/get-started-resource-planner.md)를 참조하십시오.

## 새 리소스 예산 시간 필드 {#new-resource-budgeted-hour-field}

새 계획 기능 및 리소스 플래너를 지원하기 위해 리소스 예산 시간에 대해 보고할 수 있는 새 필드가 Report Builder에 추가되었습니다. 이 필드는 프로젝트의 리소스 예산 시간을 캡처합니다. 레거시 리소스 계획 기능을 사용하여 리소스 예산을 책정하는 경우에는 이 필드를 사용할 수 없습니다.

리소스 플래너에서 예산 시간을 사용하는 방법에 대한 자세한 내용은 [리소스 플래너 개요](../../../../resource-mgmt/resource-planning/get-started-resource-planner.md)를 참조하십시오.

## 증명 승인을 위한 인앱 알림 {#in-app-notification-for-proof-approval}

증명에 대한 승인자로 지정되면 결정을 기다리는 증명 승인에 대한 인앱 알림을 받게 됩니다. 알림에 다음과 같은 텍스트가 표시됩니다. `<User name>`님이 이 증명을 승인하기를 원합니다.&quot; 사용자 정보를 사용할 수 없는 경우 알림이 &quot;이 증명은 귀하의 승인이 필요합니다.&quot;로 변경됩니다.

이 개선 이전에는 증명에서 승인자로 지정되었음을 시각적으로 표시한 것은 내 작업 영역에서 새 증명 요청뿐입니다.

인앱 알림에 대한 자세한 내용은 [인앱 알림 보기 및 관리](../../../../workfront-basics/using-notifications/view-and-manage-in-app-notifications.md)를 참조하십시오.

## 작업 및 문제에 대한 세부 정보 페이지의 &#39;할당 대상&#39; 영역에 사용자 작업 역할 표시 {#show-user-job-role-in-assigned-to-area-on-the-details-page-for-tasks-and-issues}

이제 작업 또는 문제의 세부 정보 페이지를 볼 때 할당 대상 영역에서 할당자 이름 아래에 작업 역할이 표시됩니다. 이 작업 역할은 작업 또는 문제의 작업 역할 할당과 일치하는 사용자의 작업 역할을 나타냅니다. 작업 또는 문제가 작업 역할에 할당되지 않은 경우 할당된 사용자의 기본 작업 역할이 표시됩니다.

이 변경 이전에는 할당 대상 영역에서 사용자 이름 아래에 사용자의 제목만 표시되었습니다. 
