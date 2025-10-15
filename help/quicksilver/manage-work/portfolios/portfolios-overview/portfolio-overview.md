---
content-type: overview
product-area: portfolios
navigation-topic: portfolios-overview
title: Portfolio 방법론 이해
description: Portfolio은 통합 특성이 있는 프로젝트 모음입니다. 이러한 프로젝트는 일반적으로 동일한 리소스, 예산 또는 시간대에 대해 경쟁합니다. 포트폴리오를 프로그램으로 나누고 Portfolio에 추가하기 전에 프로젝트를 프로그램과 연결할 수 있습니다.
author: Alina
feature: Work Management, Strategic Planning
exl-id: b340501e-1190-415e-aa96-5aad177c4b7b
source-git-commit: d7600a55b3dffb242957234de9d85a0deb1ad2e3
workflow-type: tm+mt
source-wordcount: '587'
ht-degree: 0%

---

# 포트폴리오 방법론 이해

<!-- Audited: 1/2024 -->

Portfolio 또는 Project PPM(Portfolio Management)은 특정 비즈니스 목표를 달성하기 위해 프로젝트 목록을 우선 순위 지정하고 관리하는 프로세스입니다.

PPM에 대한 일반적인 정보는 [Portfolio 관리 개요](/help/quicksilver/manage-work/portfolios/portfolios-overview/portfolio-managament-overview.md)를 참조하십시오.

Adobe Workfront에서 포트폴리오는 통합 특성이 있는 프로젝트 모음입니다. 이러한 프로젝트는 일반적으로 동일한 리소스, 예산 또는 시간대에 대해 경쟁합니다. 포트폴리오를 프로그램으로 나누고 Portfolio에 추가하기 전에 프로젝트를 프로그램과 연결할 수 있습니다.

포트폴리오 및 프로그램 을 사용하여 프로젝트를 구성할 수 있습니다. 프로젝트 구성을 통해 유사한 프로젝트를 비교하고 자원이 가장 잘 사용될 위치를 결정할 수 있습니다.

프로그램 사용에 대한 자세한 내용은 [프로그램 만들기](../../../manage-work/portfolios/create-and-manage-programs/create-program.md)를 참조하십시오.

이 문서에는 Workfront의 포트폴리오에 대한 일반적인 정보가 포함되어 있습니다.

## 포트폴리오를 만드는 데 필요한 액세스

<!--leave the table uncollapsed as this article is about access-->

+++ 을 확장하여 이 문서의 기능에 대한 액세스 요구 사항을 봅니다. 

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] 패키지</td> 
   <td> <p>Workfront Prime 이상</p>
   <p>워크플로우 Prime 이상</p>
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] 라이센스</td> 
   <td> <p>[!UICONTROL Standard]</p>
   <p>[!UICONTROL 계획]</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">액세스 수준 구성</td> 
   <td> <p>포트폴리오에 대한 [!UICONTROL 편집] 액세스</p>  </td> 
  </tr> 
  <tr> 
   <td role="rowheader">개체 권한</td> 
   <td> <p>포트폴리오를 만들면 기본적으로 이에 대한 관리 권한이 있습니다</p> 
   <p>포트폴리오를 편집하거나 포트폴리오에 프로젝트를 추가할 수 있는 권한 관리</p>
   <p>포트폴리오에 대한 권한을 보고 Workfront에서 확인</p>
    </td> 
  </tr> 
 </tbody> 
</table>

*자세한 내용은 [Workfront 설명서의 액세스 요구 사항](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)을 참조하십시오.

+++

<!--Old:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] plan*</td> 
   <td> <p>New: Any</p>
   <p>Current:[!UICONTROL Business] or higher</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] license*</td> 
   <td> <p>New: [!UICONTROL Standard]</p>
   <p>Current:[!UICONTROL Plan] </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Access level configurations</td> 
   <td> <p>[!UICONTROL Edit] access to Portfolios</p>  </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Object permissions</td> 
   <td> <p>After you create a portfolio, you have Manage permissions to it, by default</p> 
   <p>Manage permissions to edit a portfolio or add projects to it</p>
   <p>View permissions to a portfolio to view it in Workfront</p>
    </td> 
  </tr> 
 </tbody> 
</table>-->

## [!DNL Adobe Workfront] 포트폴리오 방법론 이해

[!DNL Workfront]에서 포트폴리오에 프로젝트를 추가하여 포트폴리오를 만들고 구성할 수 있습니다.

포트폴리오를 효율적으로 구성하려면 다음 단계를 수행하는 것이 좋습니다.

1. 프로젝트에 대한 비즈니스 사례를 만들고 프로젝트를 Portfolio과 연결합니다.

   조직에 가치를 가져다 주는 효율적인 포트폴리오를 만들려면 프로젝트 요청으로 시작하여 나중에 포트폴리오에 추가되는 각 프로젝트에 대한 비즈니스 사례를 정의해야 합니다.

   [!UICONTROL 비즈니스 사례]에 다음 정보가 포함되어 있습니다.

   * 프로젝트에 대한 일반 정보(설명, Portfolio 및 프로그램 할당, 프로젝트 소유자 및 스폰서)
   * 프로젝트의 목표 또는 목표
   * 예상 경비
   * 인건비에 대한 리소스 예산
   * 정렬 점수
   * 위험 평가

   [!UICONTROL 비즈니스 사례]에 대한 자세한 내용은 [프로젝트에 대한 비즈니스 사례 만들기](../../../manage-work/projects/define-a-business-case/create-business-case.md)를 참조하세요.

   비즈니스 사례를 빌드하는 동안 프로젝트를 포트폴리오와 연결할 수 있습니다. 포트폴리오를 프로젝트와 연결하려면 먼저 만들어야 합니다. 자세한 내용은 [포트폴리오 만들기](/help/quicksilver/manage-work/portfolios/create-and-manage-portfolios/create-portfolios.md)를 참조하세요.

   비즈니스 사례를 만드는 동안 수집한 세부 정보는 [!UICONTROL 포트폴리오 최적화 도구] 및 [!UICONTROL 리소스 플래너]에서 프로젝트 선택 관리에 도움이 됩니다.
1. 비즈니스 사례를 빌드할 때 리소스 풀을 프로젝트와 연결합니다.

   포트폴리오는 일반적으로 리소스 풀과 일치하도록 구성됩니다. Portfolio의 프로그램도 리소스 풀과 일치합니다. 일반적으로 동일한 Portfolio 내의 프로젝트가 동일한 리소스에 대해 경쟁하기 때문에 이러한 상관 관계를 통해 모든 리소스 계획이 Portfolio의 목적에 부합하도록 할 수 있습니다.

   자세한 내용은 [리소스 풀 만들기](/help/quicksilver/resource-mgmt/resource-planning/resource-pools/create-resource-pools.md)를 참조하세요.

1. Portfolio 관리자가 승인한 [!UICONTROL 비즈니스 사례]를 가져옵니다.

   자세한 내용은 [비즈니스 사례 승인](/help/quicksilver/manage-work/projects/define-a-business-case/approve-business-case.md)을 참조하세요.
1. [!UICONTROL Portfolio Optimizer]의 포트폴리오 내에서 프로젝트의 성과를 관리합니다.

   Portfolio 관리자는 Portfolio 대시보드를 사용하여 포트폴리오 내에서 재무 성과를 추적할 수 있습니다. 이 대시보드는 Portfolio의 헤더에 표시됩니다.

   Portfolio의 재무 필드에 대한 자세한 내용은 [Portfolio Optimizer 개요](../../../manage-work/portfolios/portfolio-optimizer/portfolio-optimizer-overview.md#financial-fieds-subsection)의 [Portfolio Optimizer에서 재무 필드 이해](../../../manage-work/portfolios/portfolio-optimizer/portfolio-optimizer-overview.md) 섹션을 참조하십시오.
