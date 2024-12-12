---
content-type: overview;how-to-procedural
product-area: projects
navigation-topic: financials
title: 투자 수익률(ROI) 계산
description: 투자 수익률(ROI)은 포트폴리오 관리자가 프로젝트의 원래 계획된 이익 및 예산 비용에 대해 프로젝트의 성과를 빠르게 확인할 수 있는 Adobe Workfront 지표입니다.
author: Lisa
feature: Work Management
exl-id: 1a3d16cb-8cb1-472e-8102-0ea8e0bc0edd
source-git-commit: 6afa65f921864403c10541d283ef717dce81aed7
workflow-type: tm+mt
source-wordcount: '348'
ht-degree: 0%

---

# 투자 수익률(ROI) 계산

투자 수익률(ROI)은 포트폴리오 관리자가 프로젝트의 원래 계획된 이익 및 예산 비용에 대해 프로젝트의 성과를 빠르게 확인할 수 있는 Adobe Workfront 지표입니다.

## 프로젝트 ROI 개요

Workfront은 다음 공식을 사용하여 ROI를 계산합니다.

```
Project ROI = [(Project Planned Benefit - Project Budgeted Cost) / Project Budgeted Cost] x 100
```

다음 필드는 프로젝트의 ROI에 영향을 줍니다.

* **프로젝트 계획 이익**: 비즈니스 사례의 프로젝트 정보 영역을 완료할 때 프로젝트 소유자가 지정한 수동 항목입니다. 이는 프로젝트 소유자로서 프로젝트를 완료하면 프로젝트의 이점이 있을 것으로 간주하는 예상 값입니다. 이는 특정 통화 금액이며 양의 값이어야 합니다.\
  프로젝트의 계획된 혜택에 대한 자세한 내용은 문서 [프로젝트에 대한 비즈니스 사례 만들기](../../../manage-work/projects/define-a-business-case/create-business-case.md)의 &quot;프로젝트 정보&quot; 섹션을 참조하십시오.

* **프로젝트 예산 비용**: 프로젝트를 처음 시작할 때 예상한 대로 프로젝트와 관련된 총 비용입니다.

  **예산 비용**&#x200B;은(는) 비즈니스 사례의 리소스 예산 책정에서 계산되는 **예산 인건비** 값을 사용하며 리소스 플래너에서 작업 역할에 대해 예산 책정된 시간과 각 작업 역할의 시간당 비용을 고려합니다.\
  자세한 내용은 [예산 비용 계산](../../../manage-work/projects/project-finances/budgeted-cost.md)을 참조하세요.

## 프로젝트 ROI( 투자 수익률 ) 찾기

Workfront의 다음 영역에서 프로젝트에 대한 ROI 값을 볼 수 있습니다.

* 프로젝트가 포트폴리오와 연결된 경우 Portfolio 최적화 도구에서

  >[!NOTE]
  >
  >모든 프로젝트 ROI 값의 합계는 포트폴리오의 ROI입니다.

  Portfolio 최적화 프로그램에 대한 자세한 내용은 문서 [Portfolio 최적화 프로그램 개요](../../../manage-work/portfolios/portfolio-optimizer/portfolio-optimizer-overview.md)를 참조하십시오.

* 다음 목록 및 보고서의 프로젝트 ROI 필드: 

   * 프로젝트
   * 작업
   * 문제
   * 프로젝트(재무 데이터)

  Workfront에서 보고서를 작성하는 방법에 대한 자세한 내용은 문서 [사용자 지정 보고서 만들기](../../../reports-and-dashboards/reports/creating-and-managing-reports/create-custom-report.md)를 참조하십시오.
