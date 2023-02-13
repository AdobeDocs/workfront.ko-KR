---
content-type: overview
product-area: agile-and-teams
navigation-topic: use-kanban-in-an-agile-team
title: 간판 개요
description: 간판 보드가 작동하는 방식을 더 잘 이해하려면 이 문서를 검토하십시오.
author: Lisa
feature: Agile
exl-id: d7daa6c1-dae2-4e5c-a765-6a6ebdfaa331
source-git-commit: a478e5355db33e076b321a6219442198901f3252
workflow-type: tm+mt
source-wordcount: '444'
ht-degree: 0%

---

# 간판 개요

다음 섹션에서는 [!UICONTROL 간판] 보드 함수:

## [!UICONTROL 간판] 보드 레이아웃 및 함수

다음 [!UICONTROL 간판] 보드는 다음 요소로 구성됩니다.

**백로그 열**: 현재 백로그에 있는 모든 작업을 표시합니다. 이 열은 기본적으로 표시되지 않습니다. 백로그에 표시하는 방법을 비롯하여 백로그에 대한 자세한 정보 [!UICONTROL 간판] 보드 [애자일 백로그 관리](../../agile/work-in-an-agile-environment/manage-the-agile-backlog.md).

**스토리 상태**: 스토리가 속한 상태 열을 기반으로 스토리가 진행 중인 방식을 나타냅니다.

자세한 내용은 [에서 스토리 상태 업데이트 [!UICONTROL 간판] 보드](../../agile/use-kanban-in-an-agile-team/update-the-status-of-stories.md).

섹션에 설명된 대로 민첩한 보기를 수정하여 프로젝트에 대해 스토리 상태를 사용자 지정할 수 있습니다 [[!UICONTROL 애자일 뷰 만들기 또는 사용자 정의]](../../reports-and-dashboards/reports/reporting-elements/views-overview.md#customizing-an-agile-view) in [의 보기 개요 [!DNL Adobe Workfront]](../../reports-and-dashboards/reports/reporting-elements/views-overview.md).

>[!NOTE]
>
>기본적으로 간판 보드에 최대 50개의 카드가 표시되지만, **[!UICONTROL 자세히 표시]** 추가 카드를 표시합니다.

## 하위 작업과 스토리 간의 관계

스토리에 하위 작업이 포함되어 있으면 상위 스토리 자체에 대한 정보(예: 포인트/시간 또는 완료율)는 업데이트할 수 없습니다. 또한 스토리를 [!UICONTROL 간판] 보드를 사용하여 상태를 업데이트합니다. 오히려, 스토리의 하위 작업에 대한 변경 사항이 스토리에 반영됩니다. 모든 하위 작업에 대해 결합된 스토리 포인트 또는 시간은 상위 스토리의 포인트 또는 시간을 결정합니다.

예를 들어, 하나의 스토리에는 4점으로 평가되는 하나의 하위 작업만 있다면, 스토리 자체에도 4점이 있습니다. 하위 작업 포인트 값을 3으로 변경하면 상위 스토리의 포인트 값이 3으로 변경됩니다. 동일한 스토리에 다른 하위 작업을 만들고 해당 하위 작업의 포인트 값을 4로 설정하면 스토리의 포인트 값이 7로 변경되어 두 하위 작업의 결합 포인트 값을 반영합니다.

이러한 논리가 두 번째 수준 하위 작업(하위 작업의 하위 작업)에 적용됩니다. 하위 작업에 하나 이상의 두 번째 수준 하위 작업이 있는 경우, 하위 작업은 두 번째 수준 하위 작업을 기반으로 계산됩니다.

## 지원되는 기능

간판 보드를 사용할 때 다음 작업을 수행할 수 있습니다.

* [의 기존 스토리에 하위 작업 추가 [!UICONTROL 간판] 보드](../../agile/use-kanban-in-an-agile-team/add-a-subtask-to-an-existing-story.md)
* [기존 작업 또는 문제를 [!UICONTROL 간판] 보드](../../agile/use-kanban-in-an-agile-team/add-existing-tasks-or-issues-to-the-kanban-board.md)
* [사용자를 [!UICONTROL 간판] 보드](../../agile/use-kanban-in-an-agile-team/assign-users-to-a-story.md)
* [에서 스토리 및 문제 추가 [!UICONTROL 간판] 보드](../../agile/use-kanban-in-an-agile-team/add-story-from-kanban-board.md)
* [에서 스토리 또는 문제 삭제 [!UICONTROL 간판] 보드](../../agile/use-kanban-in-an-agile-team/delete-story-from-kanban-board.md)
* [스토리 정보 편집](../../agile/use-kanban-in-an-agile-team/edit-story-information.md)
* [사용자별로 필터링 [!UICONTROL 간판] 보드](../../agile/use-kanban-in-an-agile-team/filter-by-user.md)
* [WIP(진행 중인 작업) 제한을 [!UICONTROL 간판] 보드](../../agile/use-kanban-in-an-agile-team/work-in-progress-limit-on-the-kanban-board.md)
* [에서 스토리 순서 조정 [!UICONTROL 간판] 보드](../../agile/use-kanban-in-an-agile-team/reorder-stories-on-the-kanban-board.md)
* [에서 스토리 상태 업데이트 [!UICONTROL 간판] 보드](../../agile/use-kanban-in-an-agile-team/update-the-status-of-stories.md)
* [스토리에 플래그 사용 [!UICONTROL 간판] 보드](../../agile/use-kanban-in-an-agile-team/use-flags-on-stories.md)
* [백로그를 [!UICONTROL 간판] 보드](../../agile/use-kanban-in-an-agile-team/view-the-backlog-on-the-kanban-board.md)
