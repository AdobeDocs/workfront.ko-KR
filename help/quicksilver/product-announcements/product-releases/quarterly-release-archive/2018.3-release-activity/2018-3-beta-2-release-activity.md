---
content-type: release-notes
navigation-topic: product-releases-archive
title: 2018.3 Beta 2 릴리스 활동
description: 이 페이지에서는 2018.3 Beta 2 릴리스의 미리보기 환경에서 가장 최근에 사용할 수 있는 모든 변경 사항에 대해 설명합니다. 이 기능은 2018년 8월 1일에 미리보기 환경에서 사용할 수 있습니다. Beta 2와 함께 향상된 증명 기능은 7월 18일 수요일에 미리보기 환경에서 사용할 수 있습니다. 프로덕션 환경에서는 2018년 11월에 사용할 수 있습니다.
author: Luke
feature: Product Announcements
recommendations: noDisplay, noCatalog
exl-id: 97945661-e97d-43c8-b564-624c4388de2f
source-git-commit: f1e463c90641f9221228e335b583cab72762b3bd
workflow-type: tm+mt
source-wordcount: '908'
ht-degree: 0%

---

# 2018.3 Beta 2 릴리스 활동

이 페이지에서는 2018.3 Beta 2 릴리스의 미리보기 환경에서 가장 최근에 사용할 수 있는 모든 변경 사항에 대해 설명합니다. 이 기능은 2018년 8월 1일에 미리보기 환경에서 사용할 수 있습니다. Beta 2와 함께 향상된 증명 기능은 7월 18일 수요일에 미리보기 환경에서 사용할 수 있습니다. 프로덕션 환경에서는 2018년 11월에 사용할 수 있습니다.

>[!NOTE]
>
> 이 페이지에 설명된 기능은 프로덕션 환경에서 사용하기 전에 변경될 수 있습니다.

2018.3의 모든 변경 사항 목록은 다음을 참조하십시오.  [2018.3 릴리스 활동 개요](../../../../product-announcements/product-releases/quarterly-release-archive/2018.3-release-activity/2018-3-release-activity-overview.md).

2018.3 Beta 2 릴리스에는 Workfront 관리자와 기타 사용자를 위한 개선 사항이 포함되어 있습니다.

관리자용 **1&rbrace;**

* [그룹 관리자로서 사용자 프로필의 이메일 주소 업데이트](#update-the-email-address-in-the-user-profile-as-a-group-administrator)

**모든 사용자용**

* [홈 영역에서 내게 위임된 승인 보기](#view-approvals-delegated-to-me-in-the-home-area)
* [리소스 플래너에서 지정된 기간의 데이터를 내보냅니다](#export-data-for-a-given-period-in-the-resource-planner)
* 사용자가 초과 할당되면 [일별 합계가 빨간색으로 표시됩니다](#daily-totals-now-display-in-red-when-the-user-is-overallocated)
* [최소화된 경우 작업 및 문제가 일정 타임라인에서 숨겨짐](#tasks-and-issues-are-hidden-on-the-scheduling-timeline-when-minimized)
* [증명 뷰어에서 사용자별 댓글 및 답글 필터링](#filter-comments-and-replies-by-user-in-the-proofing-viewer)
* [비디오 증명의 푸티지 범위에 주석 달기](#comment-on-a-range-of-footage-in-a-video-proof)
* [증명 뷰어의 주석 마크업에 대한 새 폴리라인 도구](#new-polyline-tool-for-comment-markup-in-the-proofing-viewer)
* [보고서, 캘린더 및 문서 공유에 대한 Flash 제거](#flash-removal-for-report-calendar-and-document-sharing)

## 그룹 관리자로서 사용자 프로필의 이메일 주소 업데이트 {#update-the-email-address-in-the-user-profile-as-a-group-administrator}

이제 관리하는 그룹에 속한 사용자의 이메일 주소를 업데이트할 수 있습니다. 

이전에는 Workfront 관리자만 다른 사용자의 이메일 주소를 업데이트할 수 있었습니다. 

자세한 내용은 [그룹 관리자](../../../../administration-and-setup/manage-groups/group-roles/group-administrators.md)를 참조하세요.

## 홈 영역에서 내게 위임된 승인 보기 {#view-approvals-delegated-to-me-in-the-home-area}

이제 홈 영역에서 귀하에게 위임된 프로젝트, 작업 및 문제 승인을 볼 수 있습니다.

이 변경 이전에는 내 작업 영역에서만 위임된 승인을 볼 수 있었습니다.

자세한 내용은 [승인 요청 위임](../../../../review-and-approve-work/manage-approvals/delegate-approval-requests.md)을 참조하십시오.

## 리소스 플래너에서 지정된 기간에 대한 데이터 내보내기 {#export-data-for-a-given-period-in-the-resource-planner}

이제 리소스 플래너에서 정보를 내보낼 때 내보낸 파일의 특정 기간을 선택할 수 있는 새 창이 표시됩니다.

이 기능이 향상되기 전에는 화면에 표시된 정보만 내보낼 수 있었습니다.

리소스 플래너에서 데이터를 내보내는 방법에 대한 자세한 내용은 [리소스 플래너 탐색 개요](../../../../resource-mgmt/resource-planning/resource-planner-navigation.md) 문서의 [리소스 플래너 탐색 개요](../../../../resource-mgmt/resource-planning/resource-planner-navigation.md)를 참조하십시오.

## 이제 사용자가 초과 할당되면 일별 합계가 빨간색으로 표시됩니다. {#daily-totals-now-display-in-red-when-the-user-is-overallocated}

>[!NOTE]
>
>리소스 예약 도구는 23.1 릴리스에서 더 이상 사용되지 않으며 Workfront에서 제거되었습니다. 업무 균형자를 사용하여 리소스를 예약하는 방법에 대한 자세한 내용은 [업무 균형자 개요](../../../../resource-mgmt/workload-balancer/overview-workload-balancer.md)를 참조하십시오.

사용자가 초과 할당되면 이제 사용자가 초과 할당된 일수의 일일 합계가 빨간색으로 표시됩니다. 이 옵션은 일정 예약 타임라인 설정에서 일별 계획된 시간의 합계 표시 옵션이 활성화된 경우에만 표시됩니다. 이 개선 이전에는 사용자가 초과 할당된 날짜에 대한 빨간색 막대 표시기가 있었지만 일별 합계는 빨간색 강조 표시 없이 표시되었습니다.

사용자 할당에 대한 자세한 내용은 &quot;예약 영역에서 사용자 할당 관리&quot;를 참조하십시오.

## 작업 및 문제는 최소화되면 예약 타임라인에서 숨겨집니다. {#tasks-and-issues-are-hidden-on-the-scheduling-timeline-when-minimized}

이제 예약 타임라인에서 작업 및 문제를 최소화할 때 설정에 [일별 계획된 시간의 합계 표시] 옵션이 활성화된 경우 사용자 및 역할에 대해 이 작업이 숨겨집니다. 미할당 영역의 작업 및 문제는 압축된 보기로 표시됩니다.

이전에는 작업 및 문제를 최소화할 때 작업 및 문제가 사용자 및 역할에 대한 예약 타임라인에 남아 있지만 압축된 보기에 표시됩니다.

예약 타임라인에서 작업 및 문제를 최소화하는 방법에 대한 자세한 내용은 다음을 참조하십시오.  &quot;리소스 일정 조정 시작&quot;

## 증명 뷰어에서 사용자별 댓글 및 답글 필터링 {#filter-comments-and-replies-by-user-in-the-proofing-viewer}

이제 지정한 사용자가 작성한 댓글을 필터링할 때 답글을 포함할 수 있습니다. 이 기능은 클라이언트나 프로젝트 관리자와 같은 중요한 검토자가 작성한 모든 피드백에 집중하려는 경우에 유용합니다.

이전에는 사용자별 필터링이 지정한 검토자가 작성(시작)한 주석으로만 제한되었습니다.

## 비디오 증명의 푸티지 범위에 주석 달기 {#comment-on-a-range-of-footage-in-a-video-proof}

비디오 증명에서 푸티지 범위에 대한 주석을 만들 수 있습니다. 이 기능은 푸티지 세그먼트를 다시 촬영하거나 제거해야 함을 나타내야 하는 경우 유용합니다.

이전에는 비디오 타임라인에서 단일 포인트에 대해서만 주석을 만들 수 있었습니다.

## 증명 뷰어의 주석 마크업에 대한 새 폴리라인 도구 {#new-polyline-tool-for-comment-markup-in-the-proofing-viewer}

이제 증명에 주석을 추가할 때 폴리라인 마크업을 사용하여 분할된 선과 모양을 그릴 수 있습니다. 열린 세그먼트 선 또는 닫힌 모양을 만들 수 있습니다. 이 도구는 기술 이미지 또는 아키텍처 이미지와 같은 복잡한 이미지로 작업할 때 특히 유용합니다.

이전에는 증명을 표시하여 주석을 추가할 때 사각형, 직선, 자유 곡선, 모양 또는 화살표를 그릴 수 있었습니다.

## 보고서, 캘린더 및 문서 공유에 대한 Flash 제거 {#flash-removal-for-report-calendar-and-document-sharing}

Workfront의 다음 공유 대화 상자에서 Flash을 제거했습니다.

* 보고서
* 캘린더
* 문서

이전과 마찬가지로 이러한 개체를 공유할 수 있지만, 이제 더 이상 경험이 Flash에 의존하지 않습니다.
