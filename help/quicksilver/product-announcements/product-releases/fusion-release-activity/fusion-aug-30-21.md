---
title: Workfront Fusion 릴리스 활동:&Nbsp;2021년 8월 30일 주
description: Workfront Fusion 릴리스 활동:&Nbsp;2021년 8월 30일 주
author: Luke
draft: Probably
feature: Product Announcements, Workfront Fusion
exl-id: 988349f9-aa12-4017-9032-be4d0078959e
hidefromtoc: true
source-git-commit: e6995cd57c4210725d49379df5bcd7e93ce4b02a
workflow-type: tm+mt
source-wordcount: '423'
ht-degree: 0%

---

# Workfront Fusion 릴리스 활동: 2021년 8월 30일 주

이 페이지에서는 2021년 8월 30일이 있는 주의 Adobe Workfront Fusion에서 향상된 기능에 대해 설명합니다.

최근 변경 사항 목록을 보려면 [Adobe Workfront Fusion 릴리스 활동](../../../product-announcements/product-releases/fusion-release-activity/fusion-release-activity.md).

Workfront Fusion의 최근 버그 수정 목록에 대해서는 다음을 참조하십시오. [Workfront 유지 관리 업데이트](https://experienceleague.adobe.com/docs/workfront-known-issues/releases/current-updates.html) 페이지를 방문하여 Workfront Fusion Maintenance Update라는 업데이트를 확인하십시오.

## Workfront > Watch 이벤트 모듈을 트리거하는 이벤트 필터링

1. Workfront > Watch 이벤트 모듈을 트리거하는 이벤트에 대한 사용자 지정 필터를 설정합니다

   불필요한 시나리오 실행 수를 줄이기 위해 이벤트 필터링을 사용하도록 Workfront > Watch 레코드 모듈을 업데이트했습니다. 이제 웹 후크를 만들 때 필터를 설정할 수 있습니다. 이렇게 하면 이벤트가 특정 기준을 충족하는 경우에만 시나리오를 트리거할 수 있습니다.

   이벤트 필터는 현재 다음 작업을 제공합니다.

   * 같음: 이벤트가 필터 조건과 일치하는 경우에만 시나리오를 트리거합니다. 예를 들어 특정 프로젝트에서 이벤트가 발생하는 경우에만 시나리오를 트리거하는 필터를 설정할 수 있습니다.
   * 같지 않음: 이벤트가 필터 조건과 일치하지 않는 경우에만 시나리오를 트리거합니다. 예를 들어에서 이벤트가 발생하는 문제에 상태가 닫히지 않은 경우에만 시나리오를 트리거하는 필터를 만들 수 있습니다.

   이전에는 시계 레코드 모듈이 모든 레코드를 검색했습니다. 사용자는 시나리오에서 나중에 필터를 설정하여 필터링할 수 있습니다.

   이벤트 필터링을 활용하려면 Watch 이벤트 모듈에서 새 웹 후크를 만듭니다. 현재 이 기능을 포함하도록 기존 웹 후크를 편집할 수 없습니다. 기존 시나리오에 대한 이벤트 필터를 사용하여 새 웹 후크를 만드는 것이 좋습니다.

1. 현재 연결에 의해 트리거된 이벤트를 필터링합니다.

   Workfront > Watch 이벤트 모듈에 대한 웹 후크를 보다 쉽게 설정할 수 있도록 가장 일반적인 이벤트 필터를 포함했습니다. 이제 웹 후크에는 Watch 이벤트 모듈에 대해 지정된 연결을 사용하여 모듈에서 수행한 변경 사항을 필터링하는 옵션이 있습니다. 즉, 이 필터가 활성화되면 해당 연결과 연결된 Workfront 사용자가 변경한 모든 사항은 시나리오를 트리거할 수 없습니다.

   이전에는 이 필터를 사용할 수 없었습니다. 따라서 Workfront 모듈에서 변경된 사항이 해당 모듈이 포함된 시나리오를 트리거하면 더 쉽게 변경되므로 시나리오가 무한 루프에서 자신을 트리거할 수 있습니다.

Workfront > Watch 이벤트 모듈의 이벤트 필터에 대한 자세한 내용은 다음을 참조하십시오 [Adobe Workfront 모듈](../../../workfront-fusion/apps-and-their-modules/workfront-modules.md).

