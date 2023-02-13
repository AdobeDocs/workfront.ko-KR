---
content-type: release-notes
keywords: 메모,분기별,업데이트
navigation-topic: product-releases
title: 21.1 기타 개선 사항
description: 이 페이지에서는 미리 보기 환경에 대한 21.1 릴리스로 수행된 다른 모든 개선 사항에 대해 설명합니다. 이러한 개선 사항은 2021년 2월 15일이 있는 프로덕션 환경에서 사용할 수 있습니다.
author: Luke
feature: Product Announcements
exl-id: aa6cfba2-d1df-4d7c-975b-2ae0e63b6d85
source-git-commit: 1bc7334423c567ef5f7fd9bcbc28de267e035c0a
workflow-type: tm+mt
source-wordcount: '739'
ht-degree: 0%

---

# 21.1 기타 개선 사항

이 페이지에서는 미리 보기 환경에 대한 21.1 릴리스로 수행된 다른 모든 개선 사항에 대해 설명합니다. 이러한 개선 사항은 2021년 2월 15일이 있는 프로덕션 환경에서 사용할 수 있습니다.

21.1 릴리스에서 사용할 수 있는 모든 변경 사항 목록에 대해서는 다음을 참조하십시오 [21.1 릴리스 개요](../../../product-announcements/product-releases/21.1-release-activity/21-1-release-overview.md).

## 이벤트 구독 실패 요구 사항 업데이트

이벤트 구독 실패의 소프트 비활성화 요구 사항을 업데이트하고 있습니다. 기존 요구 사항 외에, 이제 이벤트 구독이 2000번 시도에서 성공적으로 게재되지 않으면 소프트 비활성화될 수 있습니다. 현행 70%의 실패 규칙을 보강해 일부 조건을 적용할 경우 과다 실패를 초래할 수 있다.

또한 2021년 2월부터 하드 비활성화 요구 사항을 추가할 예정입니다.

새로운 소프트 비활성화 및 하드 비활성화 요구 사항에 대한 자세한 내용은 [FAQ - 이벤트 구독](../../../wf-api/general/event-subs-faq.md).

## Daily Digest에서 사용할 수 있는 새 팀 필드

필요한 작업 일별 다이제스트 전자 메일에 팀 승인 및 할당 필드를 추가했습니다.

자세한 내용은 [알림: 필요한 작업](../../../workfront-basics/using-notifications/notifications-action-needed.md).

## 요청 큐에서 POP 전자 메일 옵션 바꾸기

요청 큐에 대한 POP 전자 메일 옵션을 새로운 Workfront 관리 시스템으로 바꾸고 있습니다. 여전히 이메일을 통해 요청을 제출할 수는 있지만, 대신 요청 큐 영역에서 새 Adobe Workfront 관리 이메일 주소를 설정해야 합니다.

이러한 변경 사항은 미리 보기에서 테스트하는 데 사용할 수 있습니다.

모든 미리 보기 환경에서 이메일이 자동으로 비활성화됩니다. 테스트 목적으로 이메일을 활성화하려면 [미리 보기 샌드박스 환경에서 전자 메일 게재 활성화](../../../workfront-basics/using-notifications/enable-delivery-emails-from-preview-sandbox-environment.md).

자세한 내용은 [사용자가 요청 큐 프로젝트에 문제를 이메일로 보낼 수 있도록 설정](/help/quicksilver/manage-work/requests/create-requests/enable-email-issues-into-projects.md).

이 변경 작업을 수행하는 이유에 대한 자세한 내용은 [요청 큐의 POP 이메일을 21.1로 대체하기 위한 새로운 Adobe Workfront 관리 시스템](../../../product-announcements/announcements/announcement-archive/pop-removal-request-queue.md).

이 기능은 이제 [새 Workfront 환경의 큐 관리](https://one.workfront.com/s/learningpath4/queue-management-MCYCJRWK36QZBP7PGMNDMSPRN3LE) Workfront One에서 학습 경로.

## 작업표에서 시간 편집 제한

작업표 및 시간 편집을 보다 효율적으로 제어하기 위해 작업표 소유자 및 시스템 관리자에게 시간 편집을 제한할 수 있는 설정을 추가했습니다.

이전에는 액세스 수준에서 작업표 및 시간 옵션이 활성화된 사용자가 작업표에서 시간을 편집할 수 있었습니다.

자세한 내용은 [작업표 및 시간 환경 설정 구성](../../../administration-and-setup/set-up-workfront/configure-timesheets-schedules/timesheet-and-hour-preferences.md).

## 작업표 영역의 필터 및 보기가 개선되었습니다

작업표에 프로젝트, 작업 또는 문제를 추가할 때 다음과 같은 개선 사항을 추가했습니다.

* 필터: 프로젝트 및 문제에 대한 필터를 추가했습니다. 이러한 필터를 보려면 추가 옵션 을 클릭합니다. 이전에는 작업만 필터링을 사용할 수 있었습니다.
* 보기: 검색 페이지에 보기 및 그룹화 옵션이 추가되었습니다.

자세한 내용은 [로그 시간](../../../timesheets/create-and-manage-timesheets/log-time.md).

## 작업표에서 초과 작업 상자를 숨깁니다.

이제 Workfront에서 시간외 근무를 추적하지 않으면 사용자 혼란을 완화하도록 시간외 근무 상자를 숨길 수 있습니다. 단일 사용 작업표 또는 작업표 프로필의 초과 작업 상자를 숨길 수 있습니다.

* 단일 사용 작업표: 개별 작업표에서 초과 작업 상자를 숨기도록 선택하면 해당 작업표에 대해서만 숨겨집니다. 자세한 내용은 [단일 사용 작업표 만들기](../../../timesheets/create-and-manage-timesheets/create-tmshts.md).
* 작업표 프로필: 작업표 프로필에서 초과 작업 상자를 숨기도록 선택하면 해당 프로필에 할당된 사용자에 대해 만든 이후의 모든 작업표에 초과 작업 상자가 표시되지 않습니다. 자세한 내용은 [작업표 프로필 만들기, 편집 및 할당](../../../timesheets/create-and-manage-timesheets/create-timesheet-profiles.md).

이전에는 작업표에서 초과 작업 상자를 숨길 수 없었습니다.

## 탐색 표시 탐색에서 항목을 확장하거나 축소합니다.

전체 탐색 표시 경로를 쉽게 볼 수 있도록 확장 및 축소 기능을 추가했습니다.

이제 잘린 항목은 프로젝트 앞에 &quot;자세히&quot;라는 텍스트를 사용하여 그룹화됩니다. 예를 들어 &quot;3개 이상&quot;은 표시되지 않는 3개의 개체가 있음을 나타냅니다.

이전에는 생략 부호를 클릭하여 드롭다운 메뉴에 잘린 개체를 표시해야 했습니다.

탐색 표시의 모든 항목을 보려면 탐색 표시의 시작 부분에서 &quot;자세히&quot;를 클릭하여 항목을 확장합니다. 확장되면 &quot;감소&quot;를 클릭하여 항목을 다시 축소할 수 있습니다.

## 탐색 표시 탐색의 새로운 모양 및 느낌

사용자가 Workfront에서 어디에 있는지 더 잘 식별하고 개체 간을 더 쉽게 탐색할 수 있도록 지원하기 위해 탐색 표시 탐색을 다음과 같이 개선했습니다.

* 이제 이동 경로에 있는 각 항목에 개체 레이블이 포함됩니다.
* 현재 페이지는 이제 이동 경로에 포함되며 기울임꼴로 표시됩니다.
* 이제 탐색 표시에 키보드 탐색 및 화면 판독기 탐색을 사용할 수 있습니다.
* 추가적인 부 스타일 변경 사항

