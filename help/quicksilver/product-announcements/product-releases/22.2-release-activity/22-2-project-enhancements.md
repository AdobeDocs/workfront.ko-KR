---
title: 22.2&nbsp;프로젝트 개선 사항
description: 22.2&nbsp;프로젝트 개선 사항
author: Luke
draft: Probably
feature: Product Announcements
exl-id: 43ea91db-d6f2-4218-9261-580a7e5b31d0
source-git-commit: be4904f0b37870c1bfc8ec345e468d5fc283aa36
workflow-type: tm+mt
source-wordcount: '1087'
ht-degree: 1%

---

# 22.2 프로젝트 개선 사항

이 페이지에서는 미리 보기 환경에 대한 22.2 릴리스로 수행된 모든 프로젝트 개선 사항에 대해 설명합니다. 이러한 개선 사항은 프로덕션 환경에서 사용할 수 있습니다

<!--
<MadCap:conditionalText data-mc-conditions="QuicksilverOrClassic.Draft mode">
in January 2022
</MadCap:conditionalText>
-->

2022년 4월 4일이 있는 주. 22.2 릴리스에서 사용할 수 있는 모든 변경 사항 목록에 대해서는 다음을 참조하십시오 [22.2 릴리스 개요](../../../product-announcements/product-releases/22.2-release-activity/22-2-release-overview.md).

## 이제 Adobe Workfront 보드를 사용할 수 있습니다!

보드는 열과 카드가 포함된 공유 보드에 대한 액세스를 제공하여 팀 공동 작업이 가능한 유연한 도구입니다.

보드를 사용하면 다음 작업을 수행할 수 있습니다.

* 여러 열이 있는 작업 보드를 신속하게 설정
* 상태 또는 카테고리를 표시하도록 열 구성
* 보드에 다른 사용자를 추가하고 카드에 할당합니다
* 열린 종료 카드 및 확인 목록을 신속하게 추가

보드의 카드는 Adobe Workfront의 개체 및 작업 항목에 연결되어 있지 않습니다.

시스템 관리자는 레이아웃 템플릿의 보드를 활성화하여 기본 메뉴에서 모든 사용자가 이 옵션을 사용할 수 있도록 해야 합니다.

자세한 내용은 [보드 개요](../../../agile/boards-overview.md).

## Workfront 보드에 대한 추가 개선 사항

이제 Workfront 보드에 다음과 같은 추가 개선 사항을 사용할 수 있습니다.

* 보드에 카드에 태그 지정

   이제 보드에 있는 카드를 색상 코드로 분류할 수 있습니다. 태그를 사용하면 카드를 신속하게 식별할 수 있습니다. 적용된 태그를 기준으로 보드를 정렬할 수도 있습니다.

* 보드에서 카드 관리

   보드에서 카드를 관리하는 데 도움이 되는 다음 기능을 추가했습니다.

   * 카드 복사: 보드에 기존 카드의 사본을 만듭니다.
   * 카드 이동: 새로운 열 상단 및 열 메뉴 하단 옵션을 사용하여 보드의 맨 위 또는 맨 아래로 카드를 빠르게 이동합니다.

* 보드에서 검색

   보드의 모든 카드를 검색할 수 있도록 검색 막대를 추가했습니다.

* 보드에 카드의 기한 설정

   이제 보드에 있는 개별 카드에 대한 기한을 설정할 수 있습니다.

자세한 내용은 [Adobe Workfront에서 보드 시작](../../../agile/get-started-with-boards/get-started-with-boards.md).

## 게시물 업데이트 실행 취소 옵션

이제 업데이트를 게시할 때 실수를 잡는 것이 더 쉽습니다. 이제 개체의 업데이트 탭에서 주석을 완료하면 7초 동안 팝업 창이 생성되어 포스트를 취소하고 편집을 다시 시작할 수 있습니다. 시스템 타임스탬프가 전송되거나 전자 메일 및 인앱 알림을 보내기 전에 말이죠. 팝업 창을 닫거나 페이지를 비워 두거나 창이 시간 초과될 때까지 7초를 대기하면 게시물이 정상적으로 수행됩니다.

자세한 내용은 [작업 업데이트](../../../workfront-basics/updating-work-items-and-viewing-updates/update-work.md).

## 문제를 복사 및 이동할 때 경험이 업데이트되었습니다

Workfront을 새로운 Adobe Workfront 환경과 일관되게 사용하기 위해 Adobe에서는 문제를 복사 및 이동하기 위한 인터페이스를 다시 디자인했습니다. 현재 단일 문제를 복사 또는 이동하거나, 목록 또는 보고서에서 문제를 일괄적으로 복사 또는 이동할 때 사용할 수 있습니다.

새로 디자인된 인터페이스의 일부 개선 사항은 다음과 같습니다.

* 한 개의 연속 페이지에 이동되기 전에 업데이트해야 하는 모든 정보입니다.
* Workfront은 프로젝트를 선택한 후 즉시 대상 프로젝트에 액세스할 수 있는지 여부를 확인합니다. 이 개선 사항 전에 Workfront에서 추가 단계가 발생하고 이동이 허용되지 않는 동작을 확인한 후에는 올바른 액세스 권한이 없음을 경고했습니다.
* 작업 이동 상자를 벗어나지 않고 문제를 이동하려는 프로젝트에 대한 액세스를 요청할 수 있습니다.
* 다른 위치로 이동할 때 문제에 있는 항목(할당, 진행, 문서, 권한, 업데이트)을 제거할 수 있습니다. 이 기능은 이전에 복사 문제에만 사용할 수 있었습니다.
* 문제를 복사할 때 대상 프로젝트를 선택하는 것 외에 대상 작업을 선택하는 기능.

문제 이동 또는 복사에 대한 자세한 내용은 다음 문서를 참조하십시오.

* [문제 복사](../../../manage-work/issues/manage-issues/copy-issues.md)
* [문제 이동](../../../manage-work/issues/manage-issues/move-issues.md)

## 프로젝트 복사 시 새로운 경험

Workfront을 새로운 Adobe Workfront 환경과 일관되게 사용하기 위해 프로젝트 복사 인터페이스를 다시 디자인했습니다. 현재 프로젝트 페이지에서 프로젝트를 복사하거나 목록 또는 보고서에서 프로젝트를 복사할 때 사용할 수 있습니다. 이 업데이트 전에는 프로젝트 페이지에서만 프로젝트를 복사할 수 있습니다.

자세한 내용은 [프로젝트 복사](../../../manage-work/projects/manage-projects/copy-project.md).

## 새로운 추가 메뉴의 목록 및 보고서에서 프로젝트를 관리하는 기능

프로젝트 목록 및 보고서에 다음 작업을 수행할 수 있도록 새 추가 메뉴를 추가했습니다.

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
* [프로젝트 재무 재계산](../../../manage-work/projects/project-finances/recalculate-project-finances.md)
* [사용자 지정 양식 필드에서 정보 편집](../../../workfront-basics/work-with-custom-forms/edit-custom-forms.md)
* [프로젝트에 템플릿 첨부](../../../manage-work/projects/create-and-manage-templates/attach-template-to-project.md)
* [Microsoft 프로젝트로 프로젝트 내보내기](../../../manage-work/projects/manage-projects/export-project-to-ms-project.md)
* [Adobe Workfront의 항목 구독](../../../workfront-basics/using-notifications/subscribe-to-items-in-workfront.md)

## 문제를 프로젝트로 전환한 후 대시보드, 목록 또는 보고서에 사용자를 유지합니다

효율성을 높이고 클릭 수를 줄이기 위해 목록, 보고서 또는 대시보드에서 문제를 프로젝트로 변환할 때 개선 사항을 발표했습니다.

문제를 프로젝트의 페이지로 리디렉션되지 않고 프로젝트로 전환한 후에도 사용자가 목록, 보고서 또는 대시보드에 남아 있습니다. 전환이 완료되면 프로젝트 링크가 포함된 성공 알림이 표시되므로 필요한 경우 프로젝트를 쉽게 탐색할 수 있습니다.

자세한 내용은 [Adobe Workfront에서 문제를 프로젝트로 변환](../../../manage-work/issues/convert-issues/convert-issue-to-project.md).

## 할당을 변경할 때 할당 시간은 더 이상 제거되지 않습니다

>[!NOTE]
>
>이 기능은 원래 22.2 릴리스와 함께 릴리스될 예정이었습니다. 2022년 4월 21일에 프로덕션에 릴리스됩니다.

데이터의 정확성을 보장하기 위해, Adobe에서는 작업의 할당을 변경할 때 할당 시간을 유지하고 계획 시간을 변경하지 않도록 변경할 수 있습니다.

단순 기간 유형이 있는 작업에 대해 다음과 같은 변경 사항이 있습니다.

* 계획된 시간은 모든 지정자를 제거할 때 유지됩니다.
* 개별 할당 할당은 사용자와 역할을 바꿀 때 유지됩니다.
* 개별 할당 할당은 사용자를 제거할 때 역할에 유지됩니다. (릴리스에서 제거되었습니다. 이제 모든 지정자를 제거한 후 계획 시간이 0으로 설정됩니다.)

계획된 시간에 대한 자세한 내용은 [계획 시간 개요](../../../manage-work/tasks/task-information/planned-hours.md).

## 폴더 계층 구조의 상위 5개 수준에서만 폴더 공유

>[!NOTE]
>
>이 기능은 일시적으로 사용할 수 없습니다. 이 기능은 프로덕션에서 사용할 수 있으면 이 릴리스 노트를 업데이트할 예정입니다.

폴더를 공유하는 사용자에게 최상의 성능을 보장하기 위해 현재 Adobe에서는 개체의 폴더 계층 구조에서 상위 5개 수준으로 공유를 제한하고 있습니다.

여섯 번째 수준 또는 그 아래의 각 폴더는 폴더 바로 위의 공유 구성을 상속합니다.

폴더 공유에 대한 자세한 내용은 [문서 폴더 공유](../../../workfront-basics/grant-and-request-access-to-objects/share-a-document-folder.md).

