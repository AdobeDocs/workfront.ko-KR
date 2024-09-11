---
title: Portfolio 최적화 도구에서 프로젝트 우선 순위 지정
product-area: portfolios;projects
navigation-topic: portfolio-optimizer
description: Portfolio 최적화 도구에서 프로젝트의 우선 순위를 지정하여 프로젝트를 완료해야 하는 순서를 설정할 수 있습니다.
author: Alina
feature: Work Management, Strategic Planning
exl-id: 54e33746-5995-49de-8e21-bf973f0694a6
source-git-commit: 2bfb6d03f3d0f792180a67ade8a704e4c899a671
workflow-type: tm+mt
source-wordcount: '514'
ht-degree: 0%

---

# [!UICONTROL Portfolio 최적화 도구]에서 프로젝트 우선 순위 지정

[!UICONTROL Portfolio 최적화 도구]에서 프로젝트의 우선 순위를 지정하여 프로젝트를 완료해야 하는 순서를 설정할 수 있습니다.

[!UICONTROL Portfolio 최적화 도구]를 사용할 때는 다음 사항을 고려하십시오.

* [!UICONTROL Portfolio 최적화 도구]의 맨 위에 있는 프로젝트가 맨 아래에 나열된 프로젝트보다 더 중요한 것으로 간주됩니다. Portfolio을 최적화하려면 [!UICONTROL Portfolio 최적화 도구]에서 우선 순위 순서대로 프로젝트를 완료해야 합니다.
* [!UICONTROL Portfolio 최적화 도구]의 프로젝트 우선 순위는 프로젝트의 [!UICONTROL 프로젝트 세부 정보] 탭에 있는 [!UICONTROL 우선 순위] 필드와 관련이 없습니다.

  [!UICONTROL 프로젝트 세부 정보] 탭의 [!UICONTROL 우선 순위] 필드는 프로젝트의 중요성을 이해하기 위해 수동으로 지정하는 시각적 플래그입니다.

* Portfolio 최적화 도구에서 프로젝트의 우선 순위가 [!DNL Resource Planner]에 표시됩니다(활성화된 경우). [!DNL Resource Planner]에서 프로젝트는 [!UICONTROL Portfolio 우선 순위]가 아닌 [!UICONTROL 리소스 플래너] 우선 순위 순서로 리소스를 받습니다.

  [!UICONTROL 리소스 플래너]에서 프로젝트 우선 순위를 지정하는 방법에 대한 자세한 내용은 문서 [리소스 플래너에서 프로젝트 우선 순위 지정[!UICONTROL 을 참조하십시오.]](../../../resource-mgmt/resource-planning/prioritize-projects-resource-planner.md)

* [!UICONTROL Portfolio 최적화 도구]의 **[!UICONTROL 프로젝트 우선 순위]** 영역에는 기본적으로 [!UICONTROL 계획된 시작 일자] 및 [!UICONTROL 순 값] 순서로 프로젝트가 표시됩니다.

## 액세스 요구 사항

+++ 을 확장하여 이 문서의 기능에 대한 액세스 요구 사항을 봅니다.

이 문서의 단계를 수행하려면 다음 액세스 권한이 있어야 합니다.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] 플랜</td> 
   <td> <p>임의 </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront 라이센스*</td> 
   <td> <p>새로운 기능: 표준</p>
   <p>현재: 플랜</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">액세스 수준 구성*</td> 
   <td> <p>프로젝트 및 Portfolio에 대한 [!UICONTROL 편집] 액세스</p></td> 
  </tr> 
  <tr> 
   <td role="rowheader">개체 권한</td> 
   <td> <p>포트폴리오에 대한 [!UICONTROL 관리] 권한</p> <p>프로젝트에 대한 Contribute 이상 권한</p>  </td> 
  </tr> 
 </tbody> 
</table>

*자세한 내용은 [Workfront 설명서에 대한 액세스 요구 사항](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)을 참조하십시오.

+++

## [!UICONTROL Portfolio 최적화 도구]에서 프로젝트의 우선 순위 변경

1. Adobe Workfront 오른쪽 상단의 **[!UICONTROL 주 메뉴]** 아이콘 ![](assets/main-menu-icon.png)을(를) 클릭합니다.

1. **[!UICONTROL Portfolio]**&#x200B;을 클릭합니다.
1. (선택 사항) **[!UICONTROL 필터]** 드롭다운 메뉴에서 올바른 필터를 선택하여 올바른 포트폴리오 목록을 확인합니다.
1. 포트폴리오의 이름을 클릭하여 엽니다.
1. 왼쪽 패널에서 **[!UICONTROL Portfolio 최적화]**&#x200B;를 클릭합니다.
1. [!UICONTROL 프로젝트 최적화] 영역에서 프로젝트를 우선 순위 순서로 드래그한 다음 원하는 표시 위치로 드롭하여 프로젝트의 우선 순위를 변경합니다.

   ![](assets/portfolio-optimizer-with-projects-nwe-350x89.png)

   프로젝트 다시 정렬을 마치면 프로젝트 최적화 영역에서 **[!UICONTROL 우선 순위 설정]**&#x200B;을 클릭합니다. 프로젝트는 새로운 주문에 따라 새로운 번호를 받게 됩니다.

1. **[!UICONTROL 저장]**&#x200B;을 클릭하여 [!UICONTROL Portfolio 최적화 도구]에 새 프로젝트 우선 순위를 저장합니다. 우선 순위는 **#** 숫자 열에 숫자로 나열됩니다.

   >[!TIP]
   >
   >프로젝트 목록이 **#** 열 이외의 열을 기준으로 정렬할 수 있으므로 [!UICONTROL Portfolio 최적화 도구]의 프로젝트 순서를 변경할 필요는 없습니다. 프로젝트 우선 순위별로 목록을 정렬하려면 **#** 열 헤더를 클릭하십시오.

   리소스 플래너에서 **[!UICONTROL Portfolio 우선 순위 표시]** 설정을 활성화하면 리소스 플래너의 [!UICONTROL Portfolio 최적화 도구]에 표시되는 프로젝트의 우선 순위를 볼 수 있습니다.

   [!UICONTROL 리소스 플래너]에서 프로젝트 우선 순위를 지정하는 방법에 대한 자세한 내용은 문서 [리소스 플래너에서 프로젝트 우선 순위 지정[!UICONTROL 을 참조하십시오.]](../../../resource-mgmt/resource-planning/prioritize-projects-resource-planner.md)
