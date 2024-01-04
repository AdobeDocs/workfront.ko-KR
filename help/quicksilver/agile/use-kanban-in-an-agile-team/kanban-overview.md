---
content-type: overview
product-area: agile-and-teams
navigation-topic: use-kanban-in-an-agile-team
title: Kanban 개요
description: 칸반 보드의 작동 방식을 더 잘 이해하려면 이 문서를 검토하십시오.
author: Lisa
feature: Agile
exl-id: d7daa6c1-dae2-4e5c-a765-6a6ebdfaa331
source-git-commit: fa499d74df891441e729c32188e9b2f74e4ef5c0
workflow-type: tm+mt
source-wordcount: '486'
ht-degree: 0%

---

# Kanban 개요

<!-- Audited: 01/2024 -->

다음 섹션에서는 다음의 방법을 더 잘 이해할 수 있습니다. [!UICONTROL 칸반] 보드 기능.

K에 대한 설명[!UICONTROL 안반] 방법론, 참조 [애자일 팀 만들기](/help/quicksilver/agile/get-started-with-agile-in-workfront/create-an-agile-team.md).

애자일 팀에서 마이그레이션하려는 경우 [!UICONTROL 칸반] 게시판 [!DNL Workfront] [!UICONTROL 게시판], 참조 [애자일 팀 마이그레이션 [!UICONTROL 칸반] 카드 대상 [!DNL Workfront] 게시판](/help/quicksilver/agile/use-boards-agile-planning-tools/migrate-kanban-cards-to-boards.md).

## [!UICONTROL 칸반] 보드 레이아웃 및 기능

다음 [!UICONTROL 칸반] 보드는 다음 요소로 구성됩니다.

**백로그 열**: 현재 백로그에 있는 모든 작업을 표시합니다. 이 열은 기본적으로 표시되지 않습니다. 백로그에 표시하는 방법을 포함하여 백로그에 대한 자세한 정보를 보려면 [!UICONTROL 칸반] 게시판, 참조 [애자일 백로그 관리](../../agile/work-in-an-agile-environment/manage-the-agile-backlog.md).

**스토리 상태**: 스토리가 속한 상태 열에 따라 스토리가 진행되는 방식을 나타냅니다.

자세한 내용은 [에서 스토리 상태 업데이트 [!UICONTROL 칸반] 보드](../../agile/use-kanban-in-an-agile-team/update-the-status-of-stories.md).

섹션에 설명된 대로 애자일 보기를 수정하여 프로젝트에 대해 스토리 상태를 사용자 정의할 수 있습니다 [[!UICONTROL 애자일 보기 만들기 또는 사용자 지정]](/help/quicksilver/reports-and-dashboards/reports/reporting-elements/create-edit-views.md#create-or-customize-an-agile-view) 위치: [다음 위치에서 보기 만들기 또는 편집 [!DNL Adobe Workfront]](/help/quicksilver/reports-and-dashboards/reports/reporting-elements/create-edit-views.md).

>[!NOTE]
>
>기본적으로 Kanban 보드에 최대 50개의 카드가 표시되지만 **[!UICONTROL 더 보기]** 추가 카드를 표시합니다.

## 하위 작업과 스토리 간의 관계

스토리에 하위 작업이 포함된 경우 상위 스토리 자체에 대한 정보(예: 포인트/시간 또는 완료율)는 업데이트할 수 없습니다. 또한 스토리를 이동할 수 없습니다 [!UICONTROL 칸반] 게시판을 통해 상태를 업데이트할 수 있습니다. 오히려 스토리의 하위 작업에 대해 변경한 내용이 스토리에 반영됩니다. 모든 하위 작업에 대해 결합된 스토리 포인트 또는 시간이 상위 스토리의 포인트 또는 시간을 결정합니다.

예를 들어, 한 스토리에 4점으로 평가되는 하위 작업이 하나만 있다면, 스토리 자체도 4점으로 평가된다. 하위 작업 점 값을 3으로 변경하면 상위 스토리의 점 값이 3으로 변경됩니다. 동일한 스토리에 다른 하위 작업을 만들고 해당 하위 작업의 점 값을 4로 설정하면 스토리의 점 값이 7로 변경되어 두 하위 작업의 결합된 점 값을 반영합니다.

이와 동일한 논리가 두 번째 수준 하위 작업(하위 작업의 하위 작업)에 적용됩니다. 하위 작업에 하나 이상의 두 번째 수준 하위 작업이 있으면 두 번째 수준 하위 작업을 기반으로 하위 작업이 계산됩니다.

## 지원되는 기능

Kanban 보드를 사용할 때 다음 작업을 수행할 수 있습니다.

* [의 기존 스토리에 하위 작업 추가 [!UICONTROL 칸반] 보드](../../agile/use-kanban-in-an-agile-team/add-a-subtask-to-an-existing-story.md)
* [에 기존 작업 또는 문제 추가 [!UICONTROL 칸반] 보드](../../agile/use-kanban-in-an-agile-team/add-existing-tasks-or-issues-to-the-kanban-board.md)
* [의 스토리에 사용자 할당 [!UICONTROL 칸반] 보드](../../agile/use-kanban-in-an-agile-team/assign-users-to-a-story.md)
* [에서 스토리 및 문제 추가 [!UICONTROL 칸반] 보드](../../agile/use-kanban-in-an-agile-team/add-story-from-kanban-board.md)
* [에서 스토리 또는 문제 삭제 [!UICONTROL 칸반] 보드](../../agile/use-kanban-in-an-agile-team/delete-story-from-kanban-board.md)
* [스토리 정보 편집](../../agile/use-kanban-in-an-agile-team/edit-story-information.md)
* [사용자별로 필터링 [!UICONTROL 칸반] 보드](../../agile/use-kanban-in-an-agile-team/filter-by-user.md)
* [에 대한 WIP(Work In Progress) 한도 관리 [!UICONTROL 칸반] 보드](../../agile/use-kanban-in-an-agile-team/work-in-progress-limit-on-the-kanban-board.md)
* [에서 스토리 재정렬 [!UICONTROL 칸반] 보드](../../agile/use-kanban-in-an-agile-team/reorder-stories-on-the-kanban-board.md)
* [에서 스토리 상태 업데이트 [!UICONTROL 칸반] 보드](../../agile/use-kanban-in-an-agile-team/update-the-status-of-stories.md)
* [의 스토리에 플래그 사용 [!UICONTROL 칸반] 보드](../../agile/use-kanban-in-an-agile-team/use-flags-on-stories.md)
* [백로그를 다음에 추가합니다. [!UICONTROL 칸반] 보드](../../agile/use-kanban-in-an-agile-team/view-the-backlog-on-the-kanban-board.md)
