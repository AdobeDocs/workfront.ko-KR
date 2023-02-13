---
product-area: portfolios
navigation-topic: portfolio-optimizer
title: 포트폴리오의 순 가치 평가
description: Portfolio 최적기에서 [!UICONTROL 순가치 위험] 지표 는 Portfolio 최적기에 표시된 모든 프로젝트에서 제공하는 순 값을 고려하여 잠재적 위험을 측정합니다.
author: Alina
feature: Work Management, Strategic Planning
exl-id: 9e86f6eb-dd82-4731-aebb-ce8da1df5614
source-git-commit: b6defd7dba91a06feb365ead74bd9c48f5165c77
workflow-type: tm+mt
source-wordcount: '178'
ht-degree: 0%

---

# 계산 [!UICONTROL 순가치 위험] 포트폴리오

에서 [!UICONTROL Portfolio 최적화 프로그램], [!UICONTROL 순가치 위험] 지표 는 잠재적 위험을 고려하여 측정합니다 [!UICONTROL 순 값] 에 표시되는 모든 프로젝트에서 제공 [!UICONTROL Portfolio 최적화 프로그램]. 

포트폴리오 내에서 가장 효율적인 성능을 얻으려면 [!UICONTROL 위험] 표시기가 낮고 [!UICONTROL 순 값] 표시기가 높습니다. 

다음 [!UICONTROL 위험] 및 [!UICONTROL 순 값] 지표는 서로 어떻게 관련되는지를 관점으로 표현됩니다.

[!DNL Adobe Workfront] 계산 [!UICONTROL 위험] 및 [!UICONTROL 순 값] 다음 공식을 사용하는 지표:

* 다음 [!UICONTROL 위험] 표시기는 다음 공식으로 계산됩니다.

   ```
   Risk indicator = Risk / (Risk + Net Value)
   ```

* 다음 [!DNL Net Value] 표시기는 다음 공식으로 계산됩니다.

   ```
   Net Value indicator = 1 - Risk / (Risk + Net Value)
   ```

   또는

   ```
   Net Value indicator = Net Value / (Risk + Net Value)
   ```

>[!NOTE]
>
>다음 [!UICONTROL 순가치 위험] 표시기에는 [!UICONTROL Portfolio 최적화 프로그램]로 설정되며 포트폴리오와 연관된 모든 프로젝트에는 적용되지 않습니다. 
