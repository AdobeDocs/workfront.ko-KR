---
title: 22.2&nbsp;프로젝트 개선 사항
description: 22.2&nbsp;프로젝트 개선 사항
author: Luke
draft: Probably
feature: Product Announcements
recommendations: noDisplay, noCatalog
exl-id: 43ea91db-d6f2-4218-9261-580a7e5b31d0
source-git-commit: 76deb76c66e8f8a7dea721378591ae035b8d42e7
workflow-type: tm+mt
source-wordcount: '1095'
ht-degree: 1%

---

# 22.2 프로젝트 개선 사항

이 페이지에서는 미리보기 환경에 대한 22.2 릴리스의 모든 프로젝트 개선 사항에 대해 설명합니다. 이러한 개선 사항은 프로덕션 환경에서 사용할 수 있습니다

<!--
<MadCap:conditionalText data-mc-conditions="QuicksilverOrClassic.Draft mode">
in January 2022
</MadCap:conditionalText>
-->

2022년 4월 4일이 있는 주 22.2 릴리스에서 사용할 수 있는 모든 변경 사항의 목록은 을 참조하십시오. [22.2 릴리스 개요](../../../product-announcements/product-releases/22.2-release-activity/22-2-release-overview.md).

## 이제 Adobe Workfront 보드를 사용할 수 있습니다!

보드는 열과 카드가 포함된 공유 보드에 대한 액세스를 제공하여 팀 공동 작업을 허용하는 유연한 도구입니다.

보드를 사용하여 다음을 수행할 수 있습니다.

* 여러 열이 있는 작업 보드를 빠르게 설정
* 상태 또는 범주를 표시하도록 열 구성
* 다른 사용자를 보드에 추가하고 카드에 할당
* 열린 끝 카드 및 체크리스트를 빠르게 추가

보드의 카드는 Adobe Workfront의 오브젝트 및 작업 항목에 연결되어 있지 않습니다.

시스템 관리자는 레이아웃 템플릿에서 보드를 활성화하여 메인 메뉴의 모든 사용자가 옵션을 사용할 수 있도록 해야 합니다.

자세한 내용은 [보드 개요](../../../agile/boards-overview.md).

## Workfront 보드에 대한 추가 개선 사항

이제 Workfront 보드에 대해 다음과 같은 추가 개선 사항을 사용할 수 있습니다.

* 보드에서 카드에 태그 지정

  이제 보드에 있는 카드를 색상으로 구분된 태그로 분류할 수 있습니다. 태그를 사용하면 카드를 빠르게 식별할 수 있습니다. 적용된 태그를 기반으로 보드를 정렬할 수도 있습니다.

* 보드에서 카드 관리

  보드에서 카드를 관리하는 데 도움이 되는 다음 기능이 추가되었습니다.

   * 카드 복사: 보드에 기존 카드의 복사본을 만듭니다.
   * 카드 이동: 새로운 열 상단 및 열 하단 메뉴 옵션이 있는 보드 상단 또는 하단으로 카드를 빠르게 이동합니다.

* 보드에서 검색

  보드에 있는 모든 카드를 검색하는 데 도움이 되는 검색 창을 추가했습니다.

* 보드에서 카드 기한 설정

  이제 보드에서 개별 카드에 대한 기한을 설정할 수 있습니다.

자세한 내용은 [Adobe Workfront에서 보드 시작](../../../agile/get-started-with-boards/get-started-with-boards.md).

## 업데이트 게시물에 대한 실행 취소 옵션

이제 업데이트를 게시할 때 실수를 더 쉽게 발견할 수 있습니다. 이제 오브젝트의 업데이트 탭에서 댓글을 확정하면 시스템에서 타임스탬프를 부여하거나 이메일 및 인앱 알림을 보내기 전에 게시물을 취소하고 편집으로 돌아갈 수 있는 팝업 창이 7초 동안 만들어집니다. 팝업 창을 닫거나 페이지를 떠나거나 창이 시간 초과될 때까지 7초 동안 대기하면 게시물이 정상적으로 만들어집니다.

자세한 내용은 [작업 업데이트](../../../workfront-basics/updating-work-items-and-viewing-updates/update-work.md).

## 문제 복사 및 이동 시 경험 업데이트됨

Workfront을 새로운 Adobe Workfront 환경과 일관되게 사용하기 위해 문제 복사 및 이동 인터페이스를 다시 설계했습니다. 현재 하나의 문제를 복사하거나 이동할 때 또는 목록이나 보고서에서 문제를 일괄적으로 복사하거나 이동할 때 사용할 수 있습니다.

새로 디자인된 이 인터페이스의 몇 가지 개선 사항은 다음과 같습니다.

* 이동 전에 업데이트해야 하는 모든 정보가 하나의 연속 페이지에 표시됩니다.
* Workfront은 프로젝트를 선택한 후 즉시 대상 프로젝트에 액세스할 수 있는지 확인합니다. 이 개선 이전에 Workfront은 추가 단계를 수행하고 이동이 허용되지 않는 이동을 확인한 후 올바른 액세스 권한이 없다고 경고했습니다.
* 작업 이동 상자를 종료하지 않고 문제를 이동할 프로젝트에 대한 액세스 권한을 요청할 수 있습니다.
* 문제를 다른 위치로 이동할 때 해당 문제에서 항목(할당, 진행 상황, 문서, 권한, 업데이트)을 제거하는 기능. 이 기능은 이전에는 문제를 복사할 때만 사용할 수 있었습니다.
* 문제를 복사할 때 대상 프로젝트를 선택하는 것 외에 대상 작업을 선택하는 기능.

문제 이동 또는 복사에 대한 자세한 내용은 다음 문서를 참조하십시오.

* [문제 복사](../../../manage-work/issues/manage-issues/copy-issues.md)
* [문제 이동](../../../manage-work/issues/manage-issues/move-issues.md)

## 프로젝트를 복사할 때의 새로운 경험

Workfront을 새로운 Adobe Workfront 환경과 일관되게 사용하기 위해 프로젝트 복사 인터페이스를 다시 설계했습니다. 현재 프로젝트 페이지에서 프로젝트를 복사하거나 목록 또는 보고서에서 프로젝트를 복사할 때 사용할 수 있습니다. 이 업데이트 이전에는 프로젝트 페이지에서만 프로젝트를 복사할 수 있었습니다.

자세한 내용은 [프로젝트 복사](../../../manage-work/projects/manage-projects/copy-project.md).

## 새 기타 메뉴에서 목록 및 보고서에서 프로젝트를 관리하는 기능

프로젝트 목록 및 보고서에 이러한 영역에서 다음 작업을 수행할 수 있는 새로운 추가 메뉴를 추가했습니다.

* 한 번에 여러 프로젝트의 경우:
* 타임라인 다시 계산
* 재무 다시 계산
* 사용자 정의 표현식 다시 계산
* 단일 프로젝트의 경우:
* 템플릿 첨부
* MS 프로젝트로 내보내기
* 구독

자세한 내용은 다음 문서를 참조하십시오.

* [프로젝트 타임라인 다시 계산](../../../manage-work/projects/manage-projects/recalculate-project-timeline.md)
* [프로젝트 재무 다시 계산](../../../manage-work/projects/project-finances/recalculate-project-finances.md)
* [사용자 정의 양식 필드의 정보 편집](../../../workfront-basics/work-with-custom-forms/edit-custom-forms.md)
* [프로젝트에 템플릿 첨부](../../../manage-work/projects/create-and-manage-templates/attach-template-to-project.md)
* [Microsoft 프로젝트로 프로젝트 내보내기](../../../manage-work/projects/manage-projects/export-project-to-ms-project.md)
* [Adobe Workfront에서 항목 구독](../../../workfront-basics/using-notifications/subscribe-to-items-in-workfront.md)

## 문제를 프로젝트로 전환한 후 대시보드, 목록 또는 보고서에 사용자 유지

효율성을 높이고 클릭 수를 줄이기 위해 문제를 목록, 보고서 또는 대시보드에서 프로젝트로 전환할 때 개선 사항이 릴리스되었습니다.

사용자는 문제를 프로젝트의 페이지로 리디렉션되지 않고 프로젝트로 전환한 후 목록, 보고서 또는 대시보드에 남아 있습니다. 필요한 경우 프로젝트로 쉽게 이동할 수 있도록 전환이 완료된 후 프로젝트에 대한 링크가 있는 성공 알림이 표시됩니다.

자세한 내용은 [Adobe Workfront에서 문제를 프로젝트로 전환](../../../manage-work/issues/convert-issues/convert-issue-to-project.md).

## 할당을 변경할 때 할당 시간이 더 이상 제거되지 않음

>[!NOTE]
>
>이 기능은 원래 22.2 릴리스와 함께 릴리스될 예정입니다. 2022년 4월 21일 프로덕션에 출시될 예정입니다.

데이터의 정확성을 보장하기 위해 할당 시간을 보존하고 작업 할당을 변경할 때 작업 계획 시간을 변경하지 않도록 변경했습니다.

단순 기간 유형의 작업이 다음과 같이 변경되었습니다.

* 모든 할당자를 제거하면 계획된 시간이 유지됩니다.
* 사용자 및 역할을 대체할 때 개별 할당 할당은 유지됩니다.
* 개별 할당 할당은 사용자를 제거할 때 역할에 유지됩니다. (릴리스에서 제거됨. 이제 모든 할당자를 제거한 후 계획된 시간이 0으로 설정됩니다.)

계획된 시간에 대한 자세한 내용은 다음을 참조하십시오. [계획된 시간 개요](../../../manage-work/tasks/task-information/planned-hours.md).

## 폴더 계층의 상위 5개 수준에서만 폴더 공유

>[!NOTE]
>
>이 기능은 일시적으로 사용할 수 없습니다. 프로덕션 환경에서 이 기능을 사용할 수 있게 되면 이 릴리스 정보를 업데이트하겠습니다.

폴더를 공유하는 사용자에게 최상의 성능을 보장하기 위해 현재 오브젝트의 폴더 계층 구조에서 상위 5개 수준으로 공유를 제한하고 있습니다.

여섯 번째 수준 또는 그 이하의 각 폴더는 바로 위의 폴더에서 공유 구성을 상속합니다.

폴더 공유에 대한 자세한 내용은 [문서 폴더 공유](../../../workfront-basics/grant-and-request-access-to-objects/share-a-document-folder.md).

