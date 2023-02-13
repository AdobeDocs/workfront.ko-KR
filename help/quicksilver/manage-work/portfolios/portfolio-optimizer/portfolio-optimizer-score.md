---
content-type: overview
product-area: portfolios
navigation-topic: portfolio-optimizer
title: Portfolio 최적기 점수 개요
description: Portfolio 최적기에서 Portfolio 최적기 점수를 찾을 수 있습니다. 이 보고서 세트는 [!UICONTROL 점수] 모든 프로젝트에 대한 열입니다. 이는 포트폴리오의 모든 프로젝트에 대한 점수를 나타냅니다.
author: Alina
feature: Work Management, Strategic Planning
exl-id: 4451b1a3-57ae-4c66-a6a1-a85bd51a1648
source-git-commit: b6defd7dba91a06feb365ead74bd9c48f5165c77
workflow-type: tm+mt
source-wordcount: '727'
ht-degree: 1%

---

# 개요 [!UICONTROL Portfolio 최적화 프로그램] 점수

다음 항목이 있습니다. [!UICONTROL Portfolio 최적화 프로그램] 의 점수 [!UICONTROL Portfolio 최적화 프로그램]. 이 보고서 세트는 **[!UICONTROL 점수]** 모든 프로젝트에 대한 열입니다. 이는 포트폴리오의 모든 프로젝트에 대한 점수를 나타냅니다.

찾기 관련 정보 [!UICONTROL Portfolio 최적화 프로그램], 문서를 참조하십시오 [[!UICONTROL Portfolio 최적화 프로그램] 개요](../../../manage-work/portfolios/portfolio-optimizer/portfolio-optimizer-overview.md).

방법 [!DNL Adobe Workfront] 에서는 프로젝트 점수 및 기타 프로젝트 정보를 사용하여 [!UICONTROL Portfolio 최적화 프로그램]를 참조하십시오. [Portfolio 최적기에서 프로젝트 최적화](../../../manage-work/portfolios/portfolio-optimizer/optimize-projects-in-portfolio-optimizer.md).

## 의 차이점 [!UICONTROL 정렬 점수] 그리고 [!UICONTROL Portfolio 최적화 프로그램 점수]

프로젝트의 정렬 점수와 포트폴리오 최적기 점수 간에 차이가 있습니다.

프로젝트의 정렬 점수는 스코어카드를 완료한 후 얻은 점수를 기반으로 계산됩니다. 그런 다음 이 점수를 사용하여 포트폴리오 정렬 점수를 결정합니다. 정렬 점수가 백분율로 표시됩니다.\
프로젝트의 정렬 점수가 **[!UICONTROL 정렬]** 열 [!UICONTROL Portfolio 최적화 프로그램] 또는 [!UICONTROL 정렬] 필드 [!UICONTROL 비즈니스 사례 요약].

![](assets/business-case-summary-aligned-field-highlighted.png)

![](assets/project-alignment-score-portfolio-optimizer-highlighted-350x174.png)

프로젝트의 정렬 점수 생성에 대한 자세한 내용은 문서를 참조하십시오 [프로젝트에 스코어카드를 적용하고 정렬 점수를 생성합니다](../../../manage-work/projects/define-a-business-case/apply-scorecard-to-project-to-generate-alignment-score.md).

다음 [!UICONTROL 포트폴리오 최적화 프로그램] 점수는 [!UICONTROL Portfolio 최적화 프로그램] 우선 순위를 지정할 수 있습니다. portfolio optimizer 점수가 숫자와 함께 표시기 아이콘으로 표시되고 **[!UICONTROL 점수]** 열 [!UICONTROL Portfolio 최적화 프로그램].

>[!NOTE]
>
>프로젝트 점수가 [!UICONTROL Portfolio 최적화 프로그램] 비즈니스 케이스가 완료된 경우에만 해당됩니다. 비즈니스 사례 완료에 대한 자세한 내용은 문서를 참조하십시오 [[!UICONTROL 비즈니스 사례 만들기] 프로젝트](../../../manage-work/projects/define-a-business-case/create-business-case.md).

![](assets/portfolio-optimizer-project-score-highlighted-350x132.png)

각 프로젝트의 점수는 다음 카테고리의 중요도에 따라 계산됩니다.

* [!UICONTROL 비용]
* [!UICONTROL 정렬]
* [!UICONTROL 순 가치]
* [!UICONTROL 위험 요소]
* [!UICONTROL ROI]

## 계산 [!UICONTROL Portfolio 최적화 프로그램] 점수

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: This was edited based on this issue, per Anna: https://hub.workfront.com/issue/603d0c58000095ea0bc00ce5e2110693/overview)</p>
-->

[!DNL Workfront] 를 사용하여 점수를 생성합니다. [!UICONTROL Portfolio 최적화 프로그램] 프로젝트의 우선 순위를 지원하기 위한 순위입니다. 포트폴리오의 값은 프로젝트의 비즈니스 사례에 입력된 값을 기반으로 하며 프로젝트의 점수를 계산하는 데 사용됩니다. 점수가 높은 프로젝트는 더 중요한 것으로 간주될 수 있으며 먼저 완료되도록 우선 순위를 지정할 수 있습니다.

프로젝트의 등급을 확인하려면 다음을 수행하십시오.

1. 로 이동합니다. [!UICONTROL Portfolio 최적화 프로그램].
1. 순위 아이콘 위로 마우스를 가져가면 프로젝트에 대한 portfolio optimizer 점수를 볼 수 있습니다.

![ranking_icon_in_portfolio_optimizer_new.png](assets/ranking-icon-in-portfolio-optimizer-new-350x160.png)

점수 계산 알고리즘은 프로젝트의 비즈니스 사례에 요약된 값과 프로젝트가 수행하는 가중치를 고려합니다. 최적기의 모든 프로젝트에 점수를 부여하고 해당 점수를 정규화하므로 점수가 100인 프로젝트가 항상 있습니다. 이것은 가장 좋은 프로젝트에 높은 점수를 준다.

**예:** 예를 들어 [!UICONTROL 높은 정렬] 고려해야 할 유일한 요소는 정렬이 가장 높은 프로젝트가 100점을 받는 것입니다.

다음은 프로젝트에 대해 점수를 매길 수 있는 기준입니다.

* [!UICONTROL 비용]
* [!UICONTROL 정렬]
* [!UICONTROL 값]
* [!UICONTROL 위험 요소]
* [!UICONTROL ROI]

![](assets/optimizer-sliding-value-options-350x77.png)

포트폴리오에서 프로젝트를 최적화하는 방법에 대한 자세한 내용은 [에서 프로젝트 최적화 [!UICONTROL Portfolio 최적화 프로그램]](../../../manage-work/portfolios/portfolio-optimizer/optimize-projects-in-portfolio-optimizer.md).

구성 패널의 각 기준([!UICONTROL 비용], [!UICONTROL 정렬], [!UICONTROL ROI], [!UICONTROL 순 값], [!UICONTROL 위험 요소])은 선택한 내용에 따라 0-100 범위에서 가중치가 제공됩니다.

전체 비즈니스 사례가 있는 각 프로젝트에 대해 다음 공식을 사용하여 기준당 점수가 생성됩니다.

```
Score Per Criteria = (Project Value For The Criteria - AVG(all the project values for this criteria)) / Standard Deviation of that value for that project
```

**예:** 대상 [!UICONTROL 정렬 점수] 프로젝트 A의 경우 다음을 수행합니다.

```
Alignment Score = (Project A Alignment Score - AVG (of all the project Alignments)) / Standard Deviation of alignment score for that project
```

일단 모든 [!UICONTROL 기준당 점수] 계산되면 가중치를 고려하여 프로젝트에 대한 전체 점수를 얻기 위해 추가할 수 있습니다. 프로젝트의 점수는 다음 공식을 사용하여 계산됩니다.

```
Score = Cost Score * Cost Weight + Alignment Score * Alignment Weight + ROI Score * ROI Weight + Net Value Score * Net Value Weight + Risk Score * Risk Weight
```

프로젝트 비용 및 [!UICONTROL 위험] 논리는 다른 기준이 작동하는 방식과 반대로 작동합니다. 원한다면 [!UICONTROL 저렴한 비용] 중요한 것은, 그것은 증가하지 않고 프로젝트의 전체 점수를 감소시키는 것입니다. `Cost Score * Cost Weight`.

각 프로젝트에 대해 점수를 계산했으면 [!UICONTROL 최적화 점수] 는 프로젝트에 대해 다음과 같은 방법으로 정의됩니다.

1. [!UICONTROL 최소] 및 [!UICONTROL 최대] 점수가 정의됩니다.
1. 해당 값 사이의 범위가 계산됩니다.
1. 각 프로젝트에 대해 [!UICONTROL 최적화 점수] 는 다음 공식을 사용하여 계산됩니다.

   ```
   Optimization Score = Rounded ((Score - Minimum / Range)*100)
   ```
