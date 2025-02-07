---
content-type: release-notes
keywords: 메모,분기별,업데이트,릴리스
navigation-topic: 2021-2-release-activity
title: 21. 2 보고 개선 사항
description: 이 페이지에서는 미리보기 환경에 대한 21.2 릴리스의 모든 보고 개선 사항에 대해 설명합니다. 이러한 개선 사항은 2021년 5월 10일이 있는 주에 프로덕션 환경에서 사용할 수 있습니다. 21.2 릴리스에서 사용할 수 있는 모든 변경 사항 목록은 21.2 릴리스 개요 를 참조하십시오.
author: Luke
feature: Product Announcements
recommendations: noDisplay, noCatalog
exl-id: 1d5f76ef-bea7-4630-8051-454b0d109341
source-git-commit: 494c7bf8aaf3570d4a01b5e88b85410ee3f52f18
workflow-type: tm+mt
source-wordcount: '551'
ht-degree: 0%

---

# 21. 2 보고 개선 사항

이 페이지에서는 미리보기 환경에 대한 21.2 릴리스의 모든 보고 개선 사항에 대해 설명합니다. 이러한 개선 사항은 2021년 5월 10일이 있는 주에 프로덕션 환경에서 사용할 수 있습니다. 21.2 릴리스에서 사용할 수 있는 모든 변경 사항 목록을 보려면 [21.2 릴리스 개요](../../../product-announcements/product-releases/21.2-release-activity/21-2-release-overview.md)를 참조하십시오.

## 프로젝트 및 보고서에서 시간 편집 제한

프로젝트 및 시간 보고서의 시간 탭에서 시간 편집을 더 세밀하게 제어할 수 있도록 Workfront 관리자가 시간 편집을 시간 소유자 및 시스템 관리자로 제한할 수 있는 설정을 추가했습니다.

이전에는 타임시트 및 시간이 액세스 수준에서 활성화된 사용자가 시간을 편집할 수 있었습니다.

자세한 내용은 [타임시트 및 시간 환경 설정 구성](../../../administration-and-setup/set-up-workfront/configure-timesheets-schedules/timesheet-and-hour-preferences.md)을 참조하십시오.

## 업데이트된 목록 및 보고서의 할당 필드에 대한 새로운 모양과 느낌

>[!NOTE]
>
>이 기능은 새로운 Adobe Workfront 환경에서만 사용할 수 있습니다.

새 Workfront 경험에 있는 다른 영역의 현대적인 모양과 일치하도록 업데이트된 목록 및 보고서의 할당 필드에 대한 스타일이 변경되었습니다. 이 재설계에는 다음이 포함됩니다.

* 사용자 프로필 사진, 작업 역할 및 팀에 대한 둥근 아바타
* 프로필 사진이 없는 사용자의 이니셜 표시
* 새 작업 역할 아이콘
* 고급 할당에 대한 새 사람 아이콘
* 새로운 제한된 액세스 아이콘
* 기타 사소한 디자인 변경 사항

목록의 할당에 대한 자세한 내용은 [작업 할당](../../../manage-work/tasks/assign-tasks/assign-tasks.md) 또는 [문제 할당](../../../manage-work/issues/manage-issues/assign-issues.md)을 참조하세요.

![할당 업데이트](assets/assignments-updates-350x193.png)

## 업데이트된 목록 및 보고서에서 자동 완성 필드의 새로운 모양과 느낌

>[!NOTE]
>
>2021년 5월 20일에 프로덕션 환경에서 임시로 제거되었습니다.

>[!NOTE]
>
>이 기능은 새로운 Adobe Workfront 환경에서만 사용할 수 있습니다.

새 Workfront 경험에 있는 다른 영역의 현대적인 모양과 일치하도록 업데이트된 목록 및 보고서의 자동 완성 필드에 대한 스타일이 변경되었습니다. 이러한 변경 사항은 다음과 같습니다.

* 자동 완성 아이콘이 필드에서 제거되었습니다.
* 자동 완성 필드를 클릭하면 이제 텍스트를 입력하기 전에 제안 메뉴가 표시됩니다.
* 제안 메뉴는 값의 길이에 더 잘 반응하며 이러한 값은 값의 중간이 아닌 문자 제한이 충족되는 경우 끝에서 잘립니다.

업데이트된 목록에 대한 자세한 내용은 문서 [Adobe Workfront 목록 시작](../../../workfront-basics/navigate-workfront/use-lists/view-items-in-a-list.md)에서 [업데이트된 목록과 기존 목록의 차이점](../../../workfront-basics/navigate-workfront/use-lists/view-items-in-a-list.md#updated) 섹션을 참조하십시오.

![자동 완성 필드](assets/typeahead-updates-350x336.png)

## 시스템 업데이트 보고서

새 분개 입력 보고서를 사용하면 다음을 포함하여 시스템 갱신으로 드릴인할 수 있으므로 감사 기능이 향상됩니다.

* 프로젝트, 작업 또는 문제의 상태 변경
* 작업 또는 문제 삭제됨
* 사용자 정의 필드의 값
* 계획된 완료 일자
* 프로젝트 소유자 변경 사항

예를 들어, 값을 처음 입력할 때 사용자 정의 필드에 대한 프로젝트, 해당 값의 내용, 필드를 업데이트할 때 이전 값의 내용, 새로 입력한 값의 내용, 사용자가 이러한 작업을 완료한 내용 등을 포함하여 특정 사용자 정의 필드에 대한 활동을 표시하도록 이 보고서를 설정할 수 있습니다.

이전에는 Workfront API를 통해서만 시스템 업데이트에 대해 보고할 수 있었습니다.

이 보고서와 이 보고서를 사용할 수 있는 용도에 대한 자세한 내용은 [저널 게시물 보고서를 사용하여 업데이트 영역에 대한 보고](../../../reports-and-dashboards/reports/creating-and-managing-reports/create-journal-entry-report.md)를 참조하세요.

