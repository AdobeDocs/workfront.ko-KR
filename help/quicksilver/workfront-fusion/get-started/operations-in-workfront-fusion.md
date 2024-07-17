---
content-type: reference
product-previous: workfront-fusion
product-area: workfront-integrations
navigation-topic: get-started-with-workfront-fusion-2-0
title: Adobe Workfront Fusion의 작업
description: Adobe Workfront Fusion의 작업은 모듈에서 수행하는 작업입니다. 추적 목적으로 모듈에서 수행된 모든 성공적인 작업은 작업입니다.
author: Becky
feature: Workfront Fusion
exl-id: 34268fb6-e485-42be-b751-3ee79bbf5797
source-git-commit: abb021a6857f8016d4f8b6bcf99fe818e47faea6
workflow-type: tm+mt
source-wordcount: '332'
ht-degree: 0%

---

# [!DNL Adobe Workfront Fusion]의 작업

[!DNL Adobe Workfront Fusion]의 작업은 모듈에서 수행하는 작업입니다. 추적 목적으로 모듈에서 수행된 모든 성공적인 작업은 작업입니다.

## 작업 수 계산 시 고려 사항

* 일반적으로 성공적인 작업 단계 실행은 작업으로 간주됩니다.

* 시나리오의 첫 번째 모듈은 한 번만 실행되며 번들을 반환하지 않는 경우에도 항상 하나의 작업으로 계산됩니다.

* 나머지 모듈 실행 횟수는 처리해야 하는 번들 수에 따라 다릅니다.  한 번들에 대한 모듈의 한 실행은 한 번의 작업입니다. 처리 중인 번들 세트당 하나의 작업으로 계산되는 집계 모듈은 예외입니다.

* 작업은 시나리오 실행의 [!UICONTROL 완료] 단계에서 계산됩니다.

* 다음은 작업으로 계산되는 **not**&#x200B;입니다.

   * 모든 필터 단계

   * 오류 또는 중지되는 모든 작업입니다.

   * 대체 경로 또는 비활성화된 경로와 같이 경로의 규칙이 충족되지 않아 실행되지 않는 모든 경로.

   * 필터에서 데이터 통과를 허용하지 않았거나 오류로 인해 시나리오가 중지되었기 때문에 실행되지 않는 모든 작업입니다.

## 작업 제한

조직에 월별 작업 제한이 있을 수 있습니다. 조직에서 구입한 [!DNL Workfront] 플랜을 기반으로 합니다. [!UICONTROL Ultimate] [!DNL Workfront] 요금제에서는 무제한 작업을 제공합니다.

조직에 월별 제한이 있는 경우 제한에 근접하면 알림이 표시됩니다. 한도를 초과하면 [!DNL Workfront]에서 사용자의 계획을 충족하도록 조직에 연락합니다.

## 지난 30일 동안 수행된 작업 수 보기

수행된 작업의 수를 보여주는 그래프를 볼 수 있습니다. 이러한 그래프는 다음 위치에서 사용할 수 있습니다.

* **조직 대시보드**: 전체 조직에서 사용하는 작업
* **팀 대시보드**: 이 팀이 소유한 시나리오에서 사용하는 작업([!DNL Adobe Experience Cloud]만 해당)
* **시나리오 세부 정보 페이지**: 이 시나리오에서 사용되는 작업([!DNL Adobe Experience Cloud]만 해당)
