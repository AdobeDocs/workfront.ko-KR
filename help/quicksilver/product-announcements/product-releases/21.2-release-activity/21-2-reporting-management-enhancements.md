---
content-type: release-notes
keywords: 메모,분기별,업데이트,릴리스
navigation-topic: 2021-2-release-activity
title: 21. 2가지 보고 개선 사항
description: 이 페이지에서는 미리 보기 환경에 대한 21.2 릴리스로 수행된 모든 보고 개선 사항에 대해 설명합니다. 이러한 개선 사항은 2021년 5월 10일이 있는 프로덕션 환경에서 사용할 수 있습니다. 21.2 릴리스에서 사용할 수 있는 모든 변경 사항 목록은 21.2 릴리스 개요를 참조하십시오.
author: Luke
feature: Product Announcements
exl-id: 1d5f76ef-bea7-4630-8051-454b0d109341
source-git-commit: 665732453b33b49421108791a560ab84d51280b9
workflow-type: tm+mt
source-wordcount: '537'
ht-degree: 0%

---

# 21. 2가지 보고 개선 사항

이 페이지에서는 미리 보기 환경에 대한 21.2 릴리스로 수행된 모든 보고 개선 사항에 대해 설명합니다. 이러한 개선 사항은 2021년 5월 10일이 있는 프로덕션 환경에서 사용할 수 있습니다. 21.2 릴리스에서 사용할 수 있는 모든 변경 사항 목록에 대해서는 다음을 참조하십시오 [21.2 릴리스 개요](../../../product-announcements/product-releases/21.2-release-activity/21-2-release-overview.md).

## 프로젝트 및 보고서에서 시간 편집 제한

프로젝트 및 시간 보고서의 시간 탭에서 시간 편집을 보다 세밀하게 제어하기 위해 Workfront 관리자가 시간 소유자 및 시스템 관리자로 시간 편집을 제한할 수 있는 설정을 추가했습니다.

이전에는 액세스 수준에서 작업표와 시간이 활성화된 사용자가 시간을 편집할 수 있었습니다.

자세한 내용은 [작업표 및 시간 환경 설정 구성](../../../administration-and-setup/set-up-workfront/configure-timesheets-schedules/timesheet-and-hour-preferences.md).

## 업데이트된 목록 및 보고서의 지정 필드에 대한 새로운 모양과 느낌

>[!NOTE]
>
>이 기능은 새 Adobe Workfront 경험에서만 사용할 수 있습니다.

새 Workfront 경험에서 다른 영역의 최신 모양과 일치하도록 업데이트된 목록 및 보고서의 지정 필드에 대한 스타일이 변경되었습니다. 이 재설계에는 다음이 포함됩니다.

* 사용자 프로필 사진, 작업 역할 및 팀에 대한 반올림된 아바타
* 프로필 사진이 없는 사용자를 위해 이니셜이 표시됩니다
* 새 작업 역할 아이콘
* 고급 지정에 대한 새 사람 아이콘
* 새 제한된 액세스 아이콘
* 기타 사소한 디자인 변경

목록의 할당에 대한 자세한 내용은 [작업 할당](../../../manage-work/tasks/assign-tasks/assign-tasks.md) 또는 [문제 할당](../../../manage-work/issues/manage-issues/assign-issues.md).

![](assets/assignments-updates-350x193.png)

## 업데이트된 목록 및 보고서에서 새로운 서체 필드 모양 및 느낌

>[!NOTE]
>
>2021년 5월 20일에 프로덕션 환경에서 일시적으로 제거되었습니다.

>[!NOTE]
>
>이 기능은 새 Adobe Workfront 경험에서만 사용할 수 있습니다.

새 Workfront 경험에서 다른 영역의 최신 모양과 일치하도록 업데이트된 목록 및 보고서에서 서체 진행 필드에 대한 스타일이 변경되었습니다. 이러한 변경 사항은 다음과 같습니다.

* Typeahead 아이콘이 필드에서 제거되었습니다.
* 이제 서체 필드를 클릭하면 텍스트를 입력하기 전에 제안 메뉴가 표시됩니다.
* 제안 메뉴는 값 길이에 더 응답하며, 이제 값 중간에 가 아닌 문자 제한을 충족할 때 끝에서 잘립니다.

업데이트된 목록에 대한 자세한 내용은 [업데이트된 목록과 기존 목록 간의 차이점](../../../workfront-basics/navigate-workfront/use-lists/view-items-in-a-list.md#updated) 문서의 섹션 [Adobe Workfront에서 목록 시작](../../../workfront-basics/navigate-workfront/use-lists/view-items-in-a-list.md).

![](assets/typeahead-updates-350x336.png)

## 시스템 업데이트 보고서

새 분개 입력 보고서는 다음을 포함하여 시스템 갱신으로 드릴다운할 수 있도록 함으로써 더 큰 감사 가능성을 제공합니다.

* 프로젝트, 작업 또는 문제에 대한 상태 변경
* 삭제된 작업 또는 문제
* 사용자 지정 필드의 값
* 계획 완료 일자
* 프로젝트 소유자 변경

예를 들어 이 보고서를 설정하여 사용자 지정 필드에 대한 프로젝트, 사용자 지정 필드의 프로젝트, 값이 처음 입력되었을 때, 해당 값이 무엇인지, 필드가 업데이트되었을 때, 이전 값이 무엇이었는지, 새로 입력한 값이 무엇인지, 사용자가 이러한 작업을 완료했는지 등을 포함하여 특정 사용자 지정 필드 주위에 활동을 표시할 수 있습니다.

이전에는 Workfront API를 통해서만 시스템 업데이트를 보고할 수 있었습니다.

이 보고서와 이 보고서를 사용할 수 있는 작업에 대한 자세한 내용은 [업데이트 영역에 대한 보고서](../../../reports-and-dashboards/reports/creating-and-managing-reports/create-journal-entry-report.md).

