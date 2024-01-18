---
content-type: release-notes
keywords: 메모,분기별,업데이트
navigation-topic: product-releases
title: 21.1 기타 개선 사항
description: 이 페이지에서는 미리보기 환경에 대한 21.1 릴리스의 기타 모든 개선 사항에 대해 설명합니다. 이러한 개선 사항은 2021년 2월 15일이 있는 주에 프로덕션 환경에서 사용할 수 있습니다.
author: Luke
feature: Product Announcements
recommendations: noDisplay, noCatalog
exl-id: aa6cfba2-d1df-4d7c-975b-2ae0e63b6d85
source-git-commit: 76deb76c66e8f8a7dea721378591ae035b8d42e7
workflow-type: tm+mt
source-wordcount: '742'
ht-degree: 0%

---

# 21.1 기타 개선 사항

이 페이지에서는 미리보기 환경에 대한 21.1 릴리스의 기타 모든 개선 사항에 대해 설명합니다. 이러한 개선 사항은 2021년 2월 15일이 있는 주에 프로덕션 환경에서 사용할 수 있습니다.

21.1 릴리스에서 사용할 수 있는 모든 변경 사항의 목록은 을 참조하십시오. [21.1 릴리스 개요](../../../product-announcements/product-releases/21.1-release-activity/21-1-release-overview.md).

## 이벤트 구독 실패 요구 사항에 대한 업데이트

이벤트 구독 실패의 소프트 비활성화 요구 사항을 업데이트하는 중입니다. 기존 요구 사항 외에도 이제 이벤트 구독이 2000회 시도 내에 성공적으로 배달되지 못할 경우 소프트 비활성화됩니다. 이는 어떤 조건하에서 과다 실패가 발생할 수 있는 기존의 70% 실패 규칙을 강화하기 위함이다.

또한 2021년 2월부터 하드 비활성화 요구 사항을 추가할 예정입니다.

새로운 소프트 비활성화 및 하드 비활성화 요구 사항에 대한 자세한 내용은 [FAQ - 이벤트 구독](../../../wf-api/general/event-subs-faq.md).

## 일별 다이제스트에서 사용할 수 있는 새 팀 필드

필요한 작업 일별 요약 이메일에 팀 승인 및 할당 필드를 추가했습니다.

자세한 내용은 [알림: 조치 필요](../../../workfront-basics/using-notifications/notifications-action-needed.md).

## 요청 대기열의 POP 이메일 옵션 바꾸기

요청 대기열에 대한 POP 이메일 옵션을 새로운 Workfront 관리 시스템으로 바꾸는 중입니다. 이메일을 통해 요청을 제출할 수는 있지만, 대신 요청 대기열 영역에서 새 Adobe Workfront 관리 이메일 주소를 설정해야 합니다.

이러한 변경 사항은 미리보기에서 테스트할 수 있습니다.

모든 미리보기 환경에서 이메일이 자동으로 비활성화됩니다. 테스트 목적으로 이메일을 활성화하려면 다음을 참조하십시오 [미리보기 샌드박스 환경에서 이메일 게재 활성화](../../../workfront-basics/using-notifications/enable-delivery-emails-from-preview-sandbox-environment.md).

자세한 내용은 [사용자가 문제를 요청 대기열 프로젝트에 이메일로 보낼 수 있도록 설정](/help/quicksilver/manage-work/requests/create-requests/enable-email-issues-into-projects.md).

이 변경 작업을 수행하는 이유에 대한 자세한 내용은 [요청 대기열에 대한 POP 이메일을 21.1로 대체하는 새로운 Adobe Workfront 관리 시스템](../../../product-announcements/announcements/announcement-archive/pop-removal-request-queue.md).

이 기능은 이제 [새로운 Workfront 환경의 대기열 관리](https://one.workfront.com/s/learningpath4/queue-management-MCYCJRWK36QZBP7PGMNDMSPRN3LE) Workfront One의 학습 경로.

## 타임시트의 시간 편집 제한

타임시트 및 시간 편집을 보다 세밀하게 제어하기 위해 타임시트 소유자 및 시스템 관리자로 시간 편집을 제한할 수 있는 설정을 추가했습니다.

이전에는 액세스 수준에서 타임시트 및 시간 옵션이 활성화된 사용자는 모든 타임시트의 시간을 편집할 수 있었습니다.

자세한 내용은 [타임시트 및 시간 환경 설정 구성](../../../administration-and-setup/set-up-workfront/configure-timesheets-schedules/timesheet-and-hour-preferences.md).

## 타임시트 영역의 필터 및 보기 개선

타임시트에 프로젝트, 작업 또는 문제를 추가할 때 다음과 같은 개선 사항이 추가되었습니다.

* 필터: 프로젝트 및 문제에 대한 필터를 추가했습니다. 이러한 필터를 보려면 기타 옵션을 클릭하십시오. 이전에는 작업만 필터링을 사용할 수 있었습니다.
* 보기: 검색 페이지에 보기 및 그룹화 옵션을 추가했습니다.

자세한 내용은 [로그 시간](../../../timesheets/create-and-manage-timesheets/log-time.md).

## 타임시트에서 초과 작업 시간 상자 숨기기

이제 Workfront에서 초과 근무를 추적하지 않는 경우 사용자 혼동을 완화하기 위해 초과 작업 시간 상자를 숨길 수 있습니다. 일회성 타임시트 또는 타임시트 프로필에 대한 초과 작업 시간 상자를 숨길 수 있습니다.

* 단일 사용 타임시트: 개별 타임시트에서 초과 작업 시간 상자를 숨기도록 선택하면 해당 타임시트에만 숨겨집니다. 자세한 내용은 [일회용 타임시트 만들기](../../../timesheets/create-and-manage-timesheets/create-tmshts.md).
* 타임시트 프로필: 타임시트 프로필에서 초과 작업 시간 상자를 숨기도록 선택하면 해당 프로필에 할당된 사용자에 대해 생성된 모든 향후 타임시트에 초과 작업 시간 상자가 표시되지 않습니다. 자세한 내용은 [타임시트 프로필 만들기, 편집 및 할당](../../../timesheets/create-and-manage-timesheets/create-timesheet-profiles.md).

이전에는 타임시트에서 초과 작업 시간 상자를 숨길 수 없었습니다.

## 이동 경로 탐색에서 항목 확장 또는 축소

전체 탐색 표시 경로를 더 쉽게 볼 수 있도록 확장 및 축소 기능이 추가되었습니다.

이제 잘린 모든 항목이 프로젝트 앞에 &quot;more&quot; 텍스트로 그룹화됩니다. 예를 들어 &quot;3개 더&quot;는 표시되지 않는 개체가 3개 있음을 나타냅니다.

이전에는 줄임표를 클릭하여 드롭다운 메뉴에 잘린 개체를 표시해야 했습니다.

이동 경로의 모든 항목을 보려면 이동 경로의 시작 부분에서 &quot;자세히&quot;를 클릭하여 항목을 확장합니다. 확장되면 &quot;간단히&quot;를 클릭하여 항목을 다시 축소할 수 있습니다.

## 이동 경로 탐색의 새로운 모양과 느낌

사용자가 Workfront에서 자신의 위치를 보다 잘 식별하고 개체 간을 보다 쉽게 탐색할 수 있도록 탐색 표시를 다음과 같이 개선했습니다.

* 이제 이동 경로의 각 항목에 개체 레이블이 포함됩니다.
* 이제 현재 페이지가 탐색 표시에 포함되어 있으며 기울임꼴로 표시됩니다.
* 이제 이동 경로에서 키보드 탐색과 화면 판독기 탐색을 사용할 수 있습니다.
* 추가 부수적 스타일 변경

