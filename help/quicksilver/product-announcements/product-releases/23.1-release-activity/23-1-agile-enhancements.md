---
title: 23.1 Agile 개선 사항
description: 23.1 Agile 개선 사항
author: Courtney
draft: Probably
feature: Product Announcements
exl-id: 4bd041a5-a6e3-4fe3-ae23-45980701e904
source-git-commit: f0e21f9b2846c5665474903a2910ce9f41cdf810
workflow-type: tm+mt
source-wordcount: '882'
ht-degree: 0%

---

# 23.1 Agile 개선 사항

이 페이지에서는 미리 보기 환경에 대한 23.1 릴리스로 인한 모든 Agile 개선 사항에 대해 설명합니다. 이러한 개선 사항은 2023년 1월 16일이 있는 주의 프로덕션 환경에서 사용할 수 있습니다.

23.1 릴리스에서 사용할 수 있는 모든 변경 사항 목록에 대해서는 다음을 참조하십시오 [23.1 릴리스 개요](/help/quicksilver/product-announcements/product-releases/23.1-release-activity/23-1-release-overview.md).

## Workfront 보드에 대한 스크럼 계획

Adobe Workfront 보드의 새로운 스크럼 계획 기능은 민첩한 프로세스를 관리할 수 있는 유연한 옵션을 제공합니다. 이러한 도구를 사용하여 다음을 수행할 수 있습니다.

* 반복 또는 스프린트에서 작업 추적
* Velocity를 사용하여 팀 약정 가이드
* 번다운 및 완료율 추적

스크럼 계획 기능은 23.1 릴리스 이후 &quot;빠른 후속&quot;입니다.

## 카드의 만기 날짜가 Workfront 개체의 계획된 완료 날짜에 매핑됩니다

>[!NOTE]
>
>이 기능은 Workfront 보드의 초기 기능 옵트인을 통해서만 사용할 수 있습니다.

이제 Workfront 보드의 연결된 카드에 대한 만기 날짜가 연결된 Workfront 개체에서 계획된 완료 날짜에 매핑됩니다. 카드의 만기 일자를 갱신하면, 작업 또는 발행에서 계획된 완료 일자가 갱신됩니다. 계획된 완료 일자를 변경하면 카드의 만기 일자도 변경됩니다. 이전에는 카드 기한 날짜가 수동 입력이었으며 작업 또는 문제에 대한 날짜에 매핑되지 않았습니다.

날짜 매핑은 하위 작업에 동기화된 연결된 체크리스트 항목에도 적용됩니다.

이제 연결된 카드와 애드혹 카드 모두에 대한 기한 필드에 시간 필드가 포함되어 있습니다.

자세한 내용은 [보드에서 연결된 카드 사용](/help/quicksilver/agile/get-started-with-boards/connected-cards.md).

[이 기능에 대한 비디오 데모 보기](https://video.tv.adobe.com/v/3411952/){target=_blank}

## 이제 보드 체크리스트 항목 및 Workfront 하위 작업이 연결됩니다

>[!NOTE]
>
>이 기능은 Workfront 보드의 초기 기능 옵트인을 통해서만 사용할 수 있습니다.

Workfront 작업을 위해 보드에 연결된 카드를 추가하면 모든 하위 작업을 카드의 체크리스트 항목으로 가져옵니다. 또한 연결된 카드에 체크리스트 항목을 만들면 Workfront 작업에 하위 작업이 추가됩니다. 문제에 대한 검사 목록 항목은 Workfront 개체에 연결되어 있지 않습니다.

이전에는 검사 목록 항목 및 하위 작업이 연결되지 않았습니다. 보드에 하위 작업을 포함하려면 별도의 연결된 카드로 가져오거나 체크리스트 항목을 카드에 수동으로 추가할 수 있습니다.

자세한 내용은 [보드에서 연결된 카드 사용](/help/quicksilver/agile/get-started-with-boards/connected-cards.md) 및 [카드의 검사 목록 항목 관리](/help/quicksilver/agile/get-started-with-boards/manage-checklist-items.md).

[이 기능에 대한 비디오 데모 보기](https://video.tv.adobe.com/v/3411951/){target=_blank}

## 보드 열의 카드 카운터

>[!NOTE]
>
>이 기능은 Workfront 보드의 초기 기능 옵트인을 통해서만 사용할 수 있습니다.

보드에 있는 모든 열에 대해 카드 카운터를 켜는 새로운 구성 설정을 사용할 수 있습니다. 열에서 WIP 제한을 사용하는 경우 별도의 카드 카운터는 추가되지 않습니다.

자세한 내용은 [보드 열 관리](/help/quicksilver/agile/get-started-with-boards/manage-board-columns.md).

## 보드 대시보드에서 검색 및 정렬

>[!NOTE]
>
>이 기능은 Workfront 보드의 초기 기능 옵트인을 통해서만 사용할 수 있습니다.

이제 보드 이름 또는 날짜별로 보드 대시보드를 정렬하고 목록에서 특정 보드를 검색할 수 있습니다.

자세한 내용은 [보드 대시보드 사용](/help/quicksilver/agile/get-started-with-boards/use-boards-page.md).

## 카드에 상태 표시

>[!NOTE]
>
>이 기능은 Workfront 보드의 초기 기능 옵트인을 통해서만 사용할 수 있습니다.

보드에 있는 카드에 상태가 지정된 경우 상태를 확인하기 위해 카드를 열 필요가 없도록 카드에 상태가 표시됩니다. 이 개선 사항은 애드혹 및 연결된 카드 모두에 적용됩니다.

자세한 내용은 [보드에서 연결된 카드 사용](/help/quicksilver/agile/get-started-with-boards/connected-cards.md) 및 [보드에 임시 카드 추가](/help/quicksilver/agile/get-started-with-boards/add-card-to-board.md).

![카드의 상태](/help/quicksilver/product-announcements/product-releases/assets/boards-connected-card-details-110922.png)

## 이제 보드에서 연결 가능한 카드를 사용할 수 있습니다

>[!NOTE]
>
>이 기능은 Workfront 보드의 초기 기능 옵트인을 통해서만 사용할 수 있습니다.

이제 특정 카드에 대한 링크를 다른 보드 사용자에게 보낼 수 있습니다. 사용자는 링크를 열기 전에 보드를 볼 수 있는 액세스 권한이 있어야 합니다.

보드에서 카드를 열면 브라우저 URL은 다음과 같습니다.

```
https://<Workfront-URL>/boards/<board-id>/card/<card-id>. 
```

전체 URL을 복사하여 다른 사람에게 보낼 수 있습니다. 해당 사용자는 링크에 액세스할 때 열린 카드로 바로 이동합니다.

이전에는 링크가 보드에서 사용할 수 있었지만 특정 카드는 사용할 수 없었습니다.

카드에 대한 자세한 내용은 [보드에 임시 카드 추가](/help/quicksilver/agile/get-started-with-boards/add-card-to-board.md) 및 [보드에서 연결된 카드 사용](/help/quicksilver/agile/get-started-with-boards/connected-cards.md).

## 보드에서 연결로 필터링

>[!NOTE]
>
>이 기능은 Workfront 보드의 초기 기능 옵트인을 통해서만 사용할 수 있습니다.

이제 보드의 필터 목록에 연결별로 필터링하는 옵션이 포함되어 있으며, 이는 특정 프로젝트에 연결된 모든 카드를 표시합니다. 연결되지 않은 카드로 필터링할 수도 있습니다.

자세한 내용은 [보드에서 필터링 및 검색](/help/quicksilver/agile/get-started-with-boards/filter-search-in-board.md).

[이 기능에 대한 비디오 데모 보기](https://video.tv.adobe.com/v/3412381/){target=_blank}

## 일정에 따라 보드에서 카드를 보관

>[!NOTE]
>
>이 기능은 Workfront 보드의 초기 기능 옵트인을 통해서만 사용할 수 있습니다.

카드를 일정에 따라 보관하거나 보드를 &quot;꺼짐&quot;하도록 보드를 구성할 수 있습니다. 특정 열에 카드를 설정하여 특정 일 또는 주 단위로 보관할 수 있는 옵션을 사용할 수 있습니다. 예를 들어 전체 열의 카드가 2주 동안 열에 있는 후 보관되도록 폴아웃을 정의할 수 있습니다.

카드가 보드에서 떨어진 후에 다시 표시하려면 보드 필터를 설정하여 보관된 카드를 표시할 수 있습니다.

자세한 내용은 [카드 폴아웃 구성](/help/quicksilver/agile/use-boards-agile-planning-tools/configure-card-falloff.md).

[이 기능에 대한 비디오 데모 보기](https://video.tv.adobe.com/v/3412323/){target=_blank}
