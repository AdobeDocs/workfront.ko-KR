---
product-area: portfolios;projects
navigation-topic: portfolio-optimizer
title: Portfolio 최적화 도구에서 프로젝트 최적화
description: '[!UICONTROL Portfolio 최적화 도구]를 사용하여 점수 및 기타 값을 기반으로 프로젝트의 우선 순위를 지정할 수 있습니다. Optimizer는 비용, 조정, 위험 및 ROI와 같은 중요한 프로젝트 정보를 고려하여 고객에게 더 중요한 사항에 따라 프로젝트의 우선 순위를 지정합니다.'
author: Alina
feature: Work Management, Strategic Planning
exl-id: 25debc5b-5d7d-453f-ab0a-9bf3fba05693
source-git-commit: b07b4926ab1b1eee9b7698a445644e1cd312fa09
workflow-type: tm+mt
source-wordcount: '488'
ht-degree: 0%

---

# [!UICONTROL Portfolio 최적화 도구]에서 프로젝트 최적화

[!UICONTROL Portfolio 최적화 도구]를 사용하여 점수 및 기타 값을 기반으로 프로젝트의 우선 순위를 지정할 수 있습니다. [!UICONTROL 최적화 도구]은(는) 비용, 정렬, 위험 및 ROI와 같은 중요한 프로젝트 정보를 고려하여 사용자에게 더 중요한 사항에 따라 프로젝트의 우선 순위를 지정합니다.

## 액세스 요구 사항

+++ 을 확장하여 이 문서의 기능에 대한 액세스 요구 사항을 봅니다.

이 문서의 단계를 수행하려면 다음 액세스 권한이 있어야 합니다.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] 플랜</td> 
   <td> 임의</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront 라이센스*</td> 
   <td> <p>새로운 기능: [!UICONTROL Standard] </p>
   <p>현재: [!UICONTROL Plan] </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">액세스 수준 구성*</td> 
   <td> <p>프로젝트 및 Portfolio에 대한 [!UICONTROL 편집] 액세스</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">개체 권한</td> 
   <td> <p>포트폴리오에 대한 [!UICONTROL 관리] 권한</p> <p>프로젝트에 대한 Contribute 이상 권한</p> 
   <p><b>프로젝트 우선 순위 설정</b>을 사용하려면 목록에 있는 모든 프로젝트에 대한 관리 권한이 있어야 합니다.</p>
    </td> 
  </tr> 
 </tbody> 
</table>

*자세한 내용은 [Workfront 설명서에 대한 액세스 요구 사항](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)을 참조하십시오.

+++

## Portfolio 최적화 도구에서 프로젝트 최적화

1. Portfolio을 열고 왼쪽 패널에서 **[!UICONTROL Portfolio 최적화]**&#x200B;를 클릭합니다.

   [!UICONTROL Portfolio 최적화 도구]가 표시됩니다.

1. **[!UICONTROL 최적화]** 아이콘 을 클릭합니다.

   ![](assets/optimize-icon-portfolio-optimizer.png)

   프로젝트에 점수를 매길 수 있는 범주가 [!UICONTROL 최적화] 아이콘 왼쪽에 표시됩니다.

1. 슬라이딩 원을 사용하여 다음 카테고리 중 하나의 최적화를 수정합니다.

   * **[!UICONTROL 낮은 비용]**: 슬라이더를 오른쪽으로 이동하여 [!UICONTROL 계획된 비용]이 가장 낮은 프로젝트를 봅니다.
   * **[!UICONTROL 높은 정렬]**: 슬라이더를 오른쪽으로 이동하여 [!UICONTROL 스코어카드]에 따라 가장 높은 정렬로 프로젝트를 봅니다.
   * **[!UICONTROL 높은 값]**: 슬라이더를 오른쪽으로 이동하여 [!UICONTROL 순 값] 점수가 높은 프로젝트를 봅니다.
   * **[!UICONTROL 낮은 위험 대 이익]**: 슬라이더를 오른쪽으로 이동하여 위험 대 이익 비율이 가장 낮은 프로젝트를 봅니다.
   * **[!UICONTROL 높은 ROI]**: 슬라이더를 오른쪽으로 이동하여 투자 수익률(ROI)이 더 높은 프로젝트를 볼 수 있습니다.

1. 최적화 범주를 닫으려면 **x 아이콘**&#x200B;을 클릭하십시오.

   **[!UICONTROL 점수]** 열의 각 프로젝트에 대한 [!UICONTROL 점수] 값을 업데이트합니다.

   [!UICONTROL Portfolio 최적화 프로그램] 점수에 대한 자세한 내용은 [Portfolio 최적화 프로그램 개요[!UICONTROL 4} 점수](../../../manage-work/portfolios/portfolio-optimizer/portfolio-optimizer-score.md)를 참조하십시오.]

1. **[!UICONTROL Score]** 열에 올바른 가중치를 설정한 후 **[!UICONTROL Score]** 열의 헤더를 클릭하여 이 열을 기준으로 정렬합니다. 점수가 가장 높은 프로젝트가 목록 맨 위에 표시됩니다.

1. (선택 사항) 우선 순위 순서대로 프로젝트를 드래그하여 놓습니다.
[!UICONTROL Portfolio 최적화 도구]에서 프로젝트의 순서를 변경합니다.
1. (선택 사항) 프로젝트의 새 우선 순위를 저장하려면 **[!UICONTROL 우선 순위 설정]**&#x200B;을 클릭합니다.

   >[!NOTE]
   >
   >   **프로젝트 우선 순위 설정**&#x200B;을 사용하려면 목록에 있는 모든 프로젝트에 대한 관리 권한이 있어야 합니다.

   [!UICONTROL Portfolio 최적화 도구]에서 프로젝트 우선 순위를 지정하는 방법에 대한 자세한 내용은 문서 [Portfolio 최적화 도구[!UICONTROL 에서 프로젝트 우선 순위 지정]](../../../manage-work/portfolios/portfolio-optimizer/prioritize-projects-in-portfolio-optimizer.md)을 참조하십시오.

1. **[!UICONTROL 저장]**&#x200B;을 클릭하여 [!UICONTROL Portfolio 최적화 도구]를 저장합니다.
