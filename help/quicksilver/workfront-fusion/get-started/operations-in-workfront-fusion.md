---
content-type: reference
product-previous: workfront-fusion
product-area: workfront-integrations
navigation-topic: get-started-with-workfront-fusion-2-0
title: Adobe Workfront Fusion의 작업
description: Adobe Workfront Fusion의 작업은 모듈에서 수행하는 작업입니다. 추적 목적으로 모듈에서 수행된 모든 성공적인 작업은 작업입니다.
author: Becky
feature: Workfront Fusion
source-git-commit: 8d82fd10a6742f13f62b5479fafa5b42e567700f
workflow-type: tm+mt
source-wordcount: '331'
ht-degree: 0%

---

# 의 작업 [!DNL Adobe Workfront Fusion]

의 작업 [!DNL Adobe Workfront Fusion] 는 모듈에서 수행하는 작업입니다. 추적 목적으로 모듈에서 수행된 모든 성공적인 작업은 작업입니다.

## 작업 수 계산 시 고려 사항

* 일반적으로 성공적인 작업 단계 실행은 작업으로 간주됩니다.

* 시나리오의 첫 번째 모듈은 한 번만 실행되며 번들을 반환하지 않는 경우에도 항상 하나의 작업으로 계산됩니다.

* 나머지 모듈 실행 횟수는 처리해야 하는 번들 수에 따라 다릅니다.  한 번들에 대한 모듈의 한 실행은 한 번의 작업입니다. 처리 중인 번들 세트당 하나의 작업으로 계산되는 집계 모듈은 예외입니다.

* 작업은 다음에서 계산됩니다. [!UICONTROL 완료] 시나리오 실행 단계입니다.

* 다음은 **아님** 작업으로 계산:

   * 모든 필터 단계

   * 오류 또는 중지되는 모든 작업입니다.

   * 대체 경로 또는 비활성화된 경로와 같이 경로의 규칙이 충족되지 않아 실행되지 않는 모든 경로.

   * 필터에서 데이터 통과를 허용하지 않았거나 오류로 인해 시나리오가 중지되었기 때문에 실행되지 않는 모든 작업입니다.

## 작업 제한

조직에 월별 작업 제한이 있을 수 있습니다. 다음을 기반으로 합니다. [!DNL Workfront] 조직이 구입한 계획을 수립합니다. 다음 [!UICONTROL 최적] [!DNL Workfront] 플랜 은 무제한 운영을 제공합니다.

조직에 월별 제한이 있는 경우 제한에 근접하면 알림이 표시됩니다. 한도를 넘으면, [!DNL Workfront] 은(는) 플랜이 요구 사항을 충족하는지 확인하기 위해 조직에 연락합니다.

## 지난 30일 동안 수행된 작업 수 보기

수행된 작업의 수를 보여주는 그래프를 볼 수 있습니다. 이러한 그래프는 다음 위치에서 사용할 수 있습니다.

* **조직 대시보드**: 전체 조직에서 사용하는 작업
* **팀 대시보드**: 이 팀이 소유한 시나리오에서 사용하는 작업([!DNL Adobe Experience Cloud] 만)
* **시나리오 세부 정보 페이지**: 이 시나리오에서 사용하는 작업([!DNL Adobe Experience Cloud] 만)

