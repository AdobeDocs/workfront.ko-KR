---
title: 23.2 Agile 개선
description: 23.2 Agile 개선
author: Courtney
draft: Probably
feature: Product Announcements
source-git-commit: 8a209bbe64b7b69b41cd9e4d2f603ff58491ba30
workflow-type: tm+mt
source-wordcount: '739'
ht-degree: 0%

---

# 23.2 Agile 개선

이 페이지에서는 미리 보기 환경에 대한 23.2 릴리스로 인한 모든 애자일 개선 사항에 대해 설명합니다. 이러한 개선 사항은 23.2 릴리스와 함께 프로덕션 환경에서 사용할 수 있습니다.

23.2 릴리스 주기에 있는 이 시점에서 사용할 수 있는 모든 변경 사항 목록은 [23.2 릴리스 개요](/help/quicksilver/product-announcements/product-releases/23.2-release-activity/23-2-release-overview.md).

<!--

## Iteration functionality available in Adobe Workfront Boards

Several new features available in Workfront Boards make it possible to use agile Scrum functionality. These features include:

* Workstreams for grouping boards related to the same team, and collaborating on work
* A list of cards, or backlog of work, with the option to use sources to connect cards to Workfront tasks and issues
* Iteration planning and iteration process boards

Note that collections have been renamed to workstreams. Workstreams help you visualize data in different ways. You can display items on cards in a list, on a board, or on an iteration. Cards in a workstream can also be shared among multiple boards. You can easily facilitate workflows using cards and boards in a workstream.

For more information, see [Manage workstreams](/help/quicksilver/agile/use-boards-agile-planning-tools/manage-collections.md), [Create an iteration](/help/quicksilver/agile/use-boards-agile-planning-tools/create-an-iteration.md), and [Use the card list](/help/quicksilver/agile/use-boards-agile-planning-tools/use-card-list.md). Second two articles will not be available in Main until I publish my branch.

## Add tasks and issues to Boards workstreams from lists and reports

You can now add existing tasks or issues to a workstream in Workfront Boards directly from a list or report view. Any items you add to the workstream are added to the card list as unplanned cards.

For more information, see [Add existing tasks or issues to a board](/help/quicksilver/agile/get-started-with-boards/add-card-from-list-to-board.md).

-->

## 보드에 연결된 카드에 대한 로그 시간

>[!NOTE]
>
>이 기능은 Workfront 보드의 초기 기능 옵트인을 통해서만 사용할 수 있습니다.

이제 작업이나 문제를 일으킬 때와 같은 방법으로 연결된 카드에 시간을 기록할 수 있습니다. 시간을 기록하려면 작업 또는 문제에 대한 올바른 권한이 있어야 합니다.

기본적으로 연결된 카드에 시간 로깅 필드가 표시되지 않습니다. 활성화 **시간** 를 입력합니다.

자세한 내용은 [보드에서 연결된 카드 사용](/help/quicksilver/agile/get-started-with-boards/connected-cards.md).

## 카드의 필드 표시 사용자 지정

>[!NOTE]
>
>이 기능은 Workfront 보드의 초기 기능 옵트인을 통해서만 사용할 수 있습니다.


이제 사용자 지정을 사용하여 카드가 열릴 때 전체 보기에서, 보드의 압축된 카드 보기에서 카드에 표시되는 필드를 구성할 수 있습니다. 필드를 비활성화하면 두 보기 모두에 표시되지 않습니다. 전체 보기에서 필드를 활성화하고 압축된 보기에서 숨길 수도 있습니다.

자세한 내용은 [카드에 표시되는 필드를 사용자 정의합니다](/help/quicksilver/agile/get-started-with-boards/customize-fields-on-card.md).

[이 기능에 대한 비디오 데모 보기](https://video.tv.adobe.com/v/3415710/){target=_blank}

## 보드 열로 이동한 카드에 대한 기본 상태를 정의합니다

>[!NOTE]
>
>이 기능은 Workfront 보드의 초기 기능 옵트인을 통해서만 사용할 수 있습니다.

이제 열 정책에서 사용자 지정 상태와 시스템 상태를 선택하여 특정 열로 이동한 카드에 적용할 기본 상태를 설정할 수 있습니다. 카드를 열로 이동하면 Workfront은 먼저 사용자 지정 상태(예: 피드백 대기)를 적용하려고 합니다. 해당 카드에 사용자 지정 상태를 사용할 수 없는 경우에는 Workfront이 대신 시스템 상태(예: 보류 중)를 적용합니다. 또한 연결된 작업 또는 문제의 상태가 열 정책에 설정된 사용자 지정 또는 시스템 상태로 변경되면 카드가 자동으로 열로 이동합니다.

이전에는 여러 상태를 사용할 수 있는 경우 열로 이동한 모든 카드의 상태를 선택하라는 메시지가 표시되었습니다.

자세한 내용은 [열 관리](/help/quicksilver/agile/get-started-with-boards/manage-board-columns.md).

[이 기능에 대한 비디오 데모 보기](https://video.tv.adobe.com/v/3415711/){target=_blank}

## 이제 Adobe Workfront 보드에서 컬렉션을 사용할 수 있습니다

>[!NOTE]
>
>이 기능은 Workfront 보드의 초기 기능 옵트인을 통해서만 사용할 수 있습니다.

이제 보드 대시보드에서 컬렉션을 만들 수 있습니다. 컬렉션은 공동 작업을 수행하는 보드 그룹입니다. 컬렉션 이름을 지정한 후에는 열 이름과 같이 사전 정의된 설정을 제공하는 템플릿 집합을 사용하여 보드에 보드를 추가할 수 있습니다. 독립형 보드를 컬렉션으로 이동할 수도 있습니다. 일단 보드에 컬렉션이 있으면 다른 컬렉션으로 이동할 수 있지만 독립형 보드가 될 수는 없습니다.

컬렉션에 구성원을 추가하는 것은 보드에 구성원을 추가하는 것과 같은 방식으로 작동합니다. 개인 또는 팀이 컬렉션에서 보드에서 구성원으로 추가될 수 있으려면 먼저 컬렉션의 구성원이어야 합니다.

자세한 내용은 [컬렉션 관리](/help/quicksilver/agile/use-boards-agile-planning-tools/manage-collections.md).

[이 기능에 대한 비디오 데모 보기](https://video.tv.adobe.com/v/3415609/){target=_blank}

## 연결된 카드의 예측 필드는 Workfront 개체의 스토리 포인트 필드에 매핑됩니다

>[!NOTE]
>
>이 기능은 Workfront 보드의 초기 기능 옵트인을 통해서만 사용할 수 있습니다.

이제 Workfront 보드의 연결된 카드에 있는 예측 필드가 연결된 Workfront 개체의 스토리 포인트 필드에 매핑됩니다.

새 스토리 포인트 필드는 작업 또는 문제에 대한 목록 또는 보고서의 보기에 추가할 수 있는 편집 가능한 자유 형식 필드입니다. 계획 시간이나 팀 발령과 연결되지 않습니다.

이전에는 카드 추정이 수동 입력이었으며 작업 또는 문제의 필드에 매핑되지 않았습니다.

또한, 애드혹 및 연결된 카드 모두에 있는 예측 필드에는 더 이상 문자 제한이 없습니다. 이전에는 최대 문자 수가 99자입니다.

자세한 내용은 [보드에서 연결된 카드 사용](/help/quicksilver/agile/get-started-with-boards/connected-cards.md).

## 흡입 열에서 카드 미리 보기

>[!NOTE]
>
>이 기능은 Workfront 보드의 초기 기능 옵트인을 통해서만 사용할 수 있습니다.

이제 가져오기 열에서 연결된 카드를 클릭하여 해당 콘텐츠의 보기 전용 버전을 볼 수 있습니다. 카드를 흡기 열에서 보드의 다른 열로 이동할 때까지 카드 콘텐츠를 편집할 수 없습니다.
