---
product-area: portfolios
navigation-topic: portfolio-optimizer
title: 포트폴리오에서 순 가치에 대한 위험 계산
description: Portfolio Optimizer에서 [!UICONTROL 순 가치에 대한 위험] 표시기는 Portfolio Optimizer에 표시된 모든 프로젝트에서 제공하는 순 가치를 고려하여 잠재적 위험을 측정합니다.
author: Alina
feature: Work Management, Strategic Planning
exl-id: 9e86f6eb-dd82-4731-aebb-ce8da1df5614
TQID: https://experienceleague.adobe.com/mClkaUv0y-Y9wiqg4oJivWYtmJDuKG701nOr5TU5rCA
product_v2:
  - id: c4a86a5d-6562-4fc6-aa00-bfa25833aed9
feature_v2:
  - id: a0dacc9f-0e23-495b-8e9f-a77c2e60b40c
subfeature_v2:
  - id: c10f2e93-7a58-4212-aa24-684c265ebe76
  - id: f0dd7b45-76b5-49d4-afe3-39f436b6fbd3
role_v2:
  - id: b69b2659-1057-424e-8fc5-ed9e016dc554
source-git-commit: 55a9d9feae8cc1128e3427a8874414ba734dd467
workflow-type: tm+mt
source-wordcount: 178
ht-degree: 0%

---

# 포트폴리오의 [!UICONTROL 순 가치 대비 위험] 계산

[!UICONTROL Portfolio Optimizer]에서 [!UICONTROL 순 가치에 대한 위험] 표시기는 [!UICONTROL Portfolio Optimizer]에 표시된 모든 프로젝트에서 제공하는 [!UICONTROL 순 가치]을(를) 고려하여 잠재적 위험을 측정합니다.

포트폴리오 내에서 가장 효율성을 높이기 위해 [!UICONTROL 위험] 지표는 낮고 [!UICONTROL 순 가치] 지표는 높음을 확인하려고 합니다.

[!UICONTROL 위험] 및 [!UICONTROL 순 가치] 지표는 서로 어떻게 관련되는지를 보여 줍니다.

[!DNL Adobe Workfront]은(는) 다음 수식을 사용하여 [!UICONTROL 위험] 및 [!UICONTROL 순 값] 지표를 계산합니다.

* [!UICONTROL 위험] 표시기는 다음 수식으로 계산됩니다.

  ```
  Risk indicator = Risk / (Risk + Net Value)
  ```

* [!DNL Net Value] 표시기는 다음 수식으로 계산됩니다.

  ```
  Net Value indicator = 1 - Risk / (Risk + Net Value)
  ```

  또는

  ```
  Net Value indicator = Net Value / (Risk + Net Value)
  ```

>[!NOTE]
>
>[!UICONTROL 순 가치 대비 위험] 지표는 [!UICONTROL Portfolio 최적화 도구]에 표시되는 프로젝트를 기반으로 계산되며 포트폴리오와 연결된 모든 프로젝트에서는 계산되지 않습니다.
