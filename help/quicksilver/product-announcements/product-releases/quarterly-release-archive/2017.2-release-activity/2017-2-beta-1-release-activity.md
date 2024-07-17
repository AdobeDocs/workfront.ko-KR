---
content-type: release-notes
navigation-topic: product-releases-archive
title: 2017.2 Beta 1 릴리스 활동
description: 이 페이지에서는 2017.2 Beta 1 릴리스의 미리보기 환경에서 사용할 수 있는 모든 변경 사항에 대해 설명합니다. 이 페이지의 기능은 2017년 5월 10일에 미리보기 환경에서 사용할 수 있습니다.
author: Luke
feature: Product Announcements
recommendations: noDisplay, noCatalog
exl-id: 99812ed3-a300-478e-973f-b957382d934b
source-git-commit: f1e463c90641f9221228e335b583cab72762b3bd
workflow-type: tm+mt
source-wordcount: '1380'
ht-degree: 0%

---

# 2017.2 Beta 1 릴리스 활동

이 페이지에서는 2017.2 Beta 1 릴리스의 미리보기 환경에서 사용할 수 있는 모든 변경 사항에 대해 설명합니다. 이 페이지의 기능은 2017년 5월 10일에 미리보기 환경에서 사용할 수 있습니다.

>[!IMPORTANT]
>
>이 페이지에 설명된 기능은 프로덕션 환경에서 사용하기 전에 변경될 수 있습니다.

2017.2 Beta 1 릴리스에는 Workfront 관리자와 기타 사용자를 위한 개선 사항이 포함되어 있습니다.

**관리자용:**

* [문서 복원](#restore-documents)
* [릴리스 정보가 포함된 새 미리 보기 배너](#new-preview-banner-with-release-information) 
* [API 7 가용성](#api-7-availability)

**모든 사용자의 경우:**

* [작업 및 문제 구독](#subscribe-to-tasks-and-issues)
* [리소스 예약 개선](#resource-scheduling-improvements)
* [증명 비교](#compare-proofs)
* [사용자 및 프로젝트에 대한 리소스 풀의 새 필드](#new-field-for-resource-pools-for-users-and-projects)
* [대시보드 목록에서 모양과 느낌을 업데이트했습니다](#updated-look-and-feel-in-the-dashboard-list)
* [Workfront에서 보증 기능 제거](#removing-the-endorsements-functionality-in-workfront)
* [드래그하여 놓기로 목록의 열 순서 바꾸기(기능은 제거 중)](#reorder-columns-in-any-list-with-drag-and-drop-functionality-is-being-removed)

## 문서 복원 {#restore-documents}

이제 Workfront 관리자는 지난 30일 이내에 삭제된 개별 문서를 복원할 수 있습니다. 

이 변경 이전에는 Workfront 관리자가 프로젝트, 작업 및 문제(삭제된 프로젝트, 작업 또는 문제와 함께 삭제된 문서 포함)만 복원할 수 있었습니다.

자세한 내용은 [삭제된 항목 복원](../../../../administration-and-setup/manage-workfront/manage-deleted-items/restore-deleted-items.md)을 참조하세요.

## 릴리스 정보가 포함된 새 미리 보기 배너 {#new-preview-banner-with-release-information}

이제 미리보기 샌드박스 환경 상단에 있는 파란색 배너에 미리보기 환경의 릴리스 이름과 버전 번호가 표시됩니다. 릴리스 이름을 클릭하면 현재 미리보기 릴리스에 대한 자세한 정보를 찾을 수 있는 도움말 사이트 문서로 이동합니다. 미리 보기 샌드박스 환경에 대한 자세한 내용은 [Adobe Workfront 미리 보기 샌드박스 환경](../../../../administration-and-setup/set-up-workfront/workfront-testing-environments/wf-preview-sandbox-environment.md)을 참조하십시오. 

## API 7 가용성 {#api-7-availability}

이제 API 7을 사용할 수 있으며 새 오브젝트와 업데이트된 오브젝트를 포함합니다.

자세한 내용은 [API 버전 7의 새로운 기능](../../../../wf-api/api/new-api-version-7.md)을 참조하세요.

## 작업 및 문제 구독 {#subscribe-to-tasks-and-issues}

Workfront은 귀하에게 할당되거나 귀하가 소유한 항목에 대한 알림을 보냅니다.

현재 릴리스부터 자신에게 할당되지 않았지만 작업에 영향을 줄 수 있는 항목을 팔로우하려는 경우 해당 항목에 가입할 수 있습니다.

보기 이상의 권한이 있는 문제 및 작업을 구독할 수 있습니다. 구독하는 문제 또는 작업에 새 댓글이 추가되면 해당 댓글에 대한 알림을 이메일로 받게 됩니다.

문제 및 작업 구독에 대한 자세한 내용은 [Adobe Workfront에서 항목 구독](../../../../workfront-basics/using-notifications/subscribe-to-items-in-workfront.md)을 참조하세요.

## 리소스 예약 개선 사항 {#resource-scheduling-improvements}

>[!NOTE]
>
>리소스 예약 도구는 23.1 릴리스에서 더 이상 사용되지 않으며 Workfront에서 제거되었습니다. 업무 균형자를 사용하여 리소스를 예약하는 방법에 대한 자세한 내용은 [업무 균형자 개요](../../../../resource-mgmt/workload-balancer/overview-workload-balancer.md)를 참조하십시오.

리소스를 예약할 때 다음과 같은 개선 사항을 사용할 수 있습니다.

* [단일 보기에서 리소스 예약 타임라인에서 더 많은 항목 보기](#view-more-items-on-the-resource-scheduling-timeline-in-a-single-view)
* [일정 타임라인에서 작업 및 문제에 표시할 프로젝트 이름을 구성하십시오](#configure-the-project-name-to-display-on-tasks-and-issues-on-the-scheduling-timeline)
* [일정 타임라인에 상위 작업이 표시되는지 여부를 구성합니다](#configure-whether-parent-tasks-are-displayed-on-the-scheduling-timeline)
* [예약 타임라인에서 모든 작업 및 문제를 쉽게 확장하거나 축소할 수 있습니다](#more-easily-expand-or-collapse-all-tasks-and-issues-on-the-scheduling-timeline)
* [역할 및 사용자 정보는 스크롤할 때 예약 타임라인의 맨 위에 유지됩니다.](#role-and-user-information-remains-at-the-top-of-the-scheduling-timeline-when-scrolling)

### 단일 보기에서 리소스 예약 타임라인에 더 많은 항목 보기 {#view-more-items-on-the-resource-scheduling-timeline-in-a-single-view}

이제 리소스 관리자인 팀 또는 프로젝트에 대한 리소스를 예약할 때 작업 및 문제는 예약 타임라인에서 더 적은 수직 공간을 사용합니다. 이를 통해 하나의 보기에서 더 많은 작업 및 문제를 볼 수 있습니다.

예약 타임라인에서 각 작업 및 문제에 프로젝트 이름을 표시하기로 결정한 경우 각 작업 및 문제의 수직 공간이 확장되어 단일 보기에서 표시되는 작업 및 문제가 줄어듭니다.

리소스 예약에 대한 자세한 내용은  &quot;리소스 일정 조정 시작&quot;

### 예약 타임라인의 작업 및 문제에 표시할 프로젝트 이름 구성 {#configure-the-project-name-to-display-on-tasks-and-issues-on-the-scheduling-timeline}

이제 팀 또는 리소스 관리자인 프로젝트에 대한 리소스를 예약할 때 각 작업 및 문제에 일정 타임라인에 표시할 프로젝트 이름을 구성할 수 있습니다. 이렇게 하면 일정 조정 타임라인을 보는 사용자가 작업 또는 문제가 있는 프로젝트의 이름을 빠르게 볼 수 있습니다.

자세한 내용은 &quot;리소스 예약 시작&quot;을 참조하십시오.

### 일정 예약 타임라인에 상위 작업을 표시할지 여부를 구성합니다. {#configure-whether-parent-tasks-are-displayed-on-the-scheduling-timeline}

이제 리소스 관리자인 프로젝트에 대한 리소스를 예약할 때 프로젝트의 요약 완료 모드 옵션이 수동으로 설정된 경우 상위 작업이 일정 타임라인에 표시되는지 여부를 구성할 수 있습니다.

이 변경 이전에는 프로젝트에 대한 요약 완료 모드가 수동으로 설정되어 있으면 항상 일정 타임라인에 상위 작업이 표시됩니다. 

프로젝트의 요약 완료 모드가 자동으로 설정되어 있으면 상위 작업을 일정 타임라인에 표시할 수 없습니다. 이 경험은 변경되지 않았습니다.

자세한 내용은 &quot;리소스 예약 시작&quot;을 참조하십시오.

### 예약 타임라인에서 모든 작업 및 문제를 보다 쉽게 확장 또는 축소할 수 있습니다. {#more-easily-expand-or-collapse-all-tasks-and-issues-on-the-scheduling-timeline}

예약 타임라인에서 모든 작업 및 문제를 보다 쉽게 축소할 수 있는 새 링크를 사용할 수 있습니다.

자세한 내용은 &quot;리소스 예약 시작&quot;을 참조하십시오.

### 역할 및 사용자 정보는 스크롤할 때 예약 타임라인의 맨 위에 유지됩니다. {#role-and-user-information-remains-at-the-top-of-the-scheduling-timeline-when-scrolling}

이제 예약 타임라인에서 아래로 스크롤하여 추가 정보를 볼 때 역할 이름 및 사용자 이름은 예약 타임라인의 사용자 및 역할 영역 맨 위에 유지되므로 작업 및 문제와 관련된 사용자 및 역할을 보다 쉽게 확인할 수 있습니다.

이 변경 전에 역할 이름과 사용자 이름이 현재 보기에서 스크롤됩니다.

리소스 예약에 대한 자세한 내용은  &quot;리소스 일정 조정 시작&quot;

## 증명 비교 {#compare-proofs}

이제 프로젝트, 작업, 문제, 포트폴리오의 문서 탭 내 또는 전역 탐색 막대의 기본 문서 영역 내처럼 단일 문서 목록 내에서 두 문서 증명을 비교할 수 있습니다. 

두 개의 증명은 검토 및 승인 도구에 표시되며, 나란히 보기에서 각 문서를 비교하면서 증명을 만들 수 있습니다.

자세한 내용은 [증명 비교](../../../../review-and-approve-work/proofing/reviewing-proofs-within-workfront/review-a-proof/compare-proofs.md)를 참조하십시오.

## 사용자 및 프로젝트를 위한 리소스 풀의 새 필드 {#new-field-for-resource-pools-for-users-and-projects}

R1.5 릴리스에는 미리보기 환경에 대한 리소스 계획에 대한 새로운 기능이 도입되었습니다. 이 기능을 사용하면 사용자 컬렉션인 새 리소스 풀을 만들 수 있습니다.

이제 이러한 리소스 풀을 프로젝트 및 사용자와 연결할 수 있습니다. 이제 프로젝트 및 사용자 오브젝트에 &quot;리소스 풀&quot;이라는 새 필드가 표시됩니다.

새 리소스 풀 및 이를 프로젝트 및 사용자와 연결하는 방법에 대한 자세한 내용은 [리소스 풀 개요](../../../../resource-mgmt/resource-planning/resource-pools/work-with-resource-pools.md)를 참조하세요.

## 대시보드 목록에서 모양과 느낌이 업데이트됨 {#updated-look-and-feel-in-the-dashboard-list}

이제 대시보드 목록을 볼 때 모양과 느낌이 보다 현대적이고 확장 가능합니다.

이 기능은 이전에는 조기 액세스에 등록된 사용자만 사용할 수 있었습니다. 이제 미리보기 환경의 모든 사용자가 사용할 수 있습니다. 2017.2 릴리스를 통해 프로덕션 환경의 모든 사용자가 사용할 수 있게 됩니다. 

대시보드에 대한 자세한 내용은 [대시보드 만들기](../../../../reports-and-dashboards/dashboards/creating-and-managing-dashboards/create-dashboard.md)를 참조하십시오.

## Workfront에서 보증 기능 제거 {#removing-the-endorsements-functionality-in-workfront}

업데이트 스트림에 포함된 기능을 평가하는 동안 낮은 채택률과 낮은 사용 기능으로 보증 을 식별했습니다. 2017.2년에, 2017.2 릴리스부터 Workfront에서 보증에 대한 다음 기능이 제거됩니다(이 기능은 더 이상 미리보기에서 사용할 수 없음).

* 사용자 프로필 영역의 보증 탭
* 보증 오브젝트는 API 탐색기에서 제거됩니다. 현재 오브젝트 &quot;보증&quot; 또는 &quot;보증 공유&quot;에 대한 API 보고서를 가져오는 경우 이 오브젝트를 제거하면 호출이 유효하지 않게 됩니다.

다음 기능은 웹 응용 프로그램에서 계속 유지됩니다.

* 이 기능이 제거되기 전에 다른 사용자가 사용자를 보증하면 보증인의 업데이트 스트림에 남아 있게 됩니다. 

보증이 보고 가능한 오브젝트가 아니어서 이 오브젝트에 대한 보고에 변경 사항이 없습니다.

## 드래그하여 놓기로 목록의 열 순서 바꾸기(기능은 제거 중) {#reorder-columns-in-any-list-with-drag-and-drop-functionality-is-being-removed}

한 위치에서 열을 끌어 다른 위치에 놓아 목록의 열 순서를 변경하는 기능은 2017.2 릴리스의 프로덕션 환경에서 조기 액세스에서 제거되며 더 이상 사용자가 사용할 수 없습니다. 

이 기능에 대한 자세한 내용은 [열 너비 및 순서 수정](../../../../reports-and-dashboards/reports/reporting-elements/modify-column-width-order.md)을 참조하십시오.
