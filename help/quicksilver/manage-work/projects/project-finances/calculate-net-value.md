---
content-type: overview;how-to-procedural
product-area: projects
navigation-topic: financials
title: 순 가치 계산
description: 프로젝트의 순 가치(Net Value)는 프로젝트의 편익을 계산하고 비용을 제거한 후 프로젝트의 총 예상 가치입니다.
author: Lisa
feature: Work Management
exl-id: 44e3f211-c816-4ee1-aafc-c40fc8732f1a
source-git-commit: dbc4404501e20b3f1905a5eebd13734a65db27ae
workflow-type: tm+mt
source-wordcount: '402'
ht-degree: 1%

---

# 순 가치 계산

프로젝트의 순 가치(Net Value)는 프로젝트의 편익을 계산하고 비용을 제거한 후 프로젝트의 총 예상 가치입니다.

## 프로젝트 순 가치 개요

Adobe Workfront은 다음 공식을 사용하여 프로젝트의 순 가치를 계산합니다.

```
Project Net Value = Planned Benefit - Budgeted Cost - Potential Risk Cost
```

다음 필드는 프로젝트의 순 가치에 영향을 줄 수 있습니다.

* **계획된 이익**: 비즈니스 사례의 **프로젝트 정보** 영역을 완료할 때 프로젝트 소유자가 지정한 수동 항목입니다.\
  프로젝트의 계획된 혜택에 대한 자세한 내용은 문서 [비즈니스 사례 영역 개요](../../../manage-work/projects/define-a-business-case/areas-of-business-case.md#project-info)의 [프로젝트 정보](../../../manage-work/projects/define-a-business-case/areas-of-business-case.md) 섹션을 참조하십시오.

* **예산 비용**: 프로젝트를 처음 시작할 때 예상한 프로젝트와 관련된 총 비용입니다.

  **예산 비용**&#x200B;은(는) 비즈니스 사례의 리소스 예산 책정에서 계산되는 **예산 인건비** 값을 사용하며 리소스 플래너에서 작업 역할에 대해 예산 책정된 시간과 각 작업 역할의 시간당 비용을 고려합니다.\
  예산 비용은 프로젝트의 **순 가치**&#x200B;에 영향을 줍니다. 예산 비용 계산 방법에 대한 자세한 내용은 [예산 비용 계산](../../../manage-work/projects/project-finances/budgeted-cost.md)을 참조하세요.

* **잠재적 위험 비용**: 비즈니스 사례 또는 프로젝트의 위험 탭에 정의된 대로 프로젝트의 위험과 관련된 비용입니다.\
  프로젝트의 잠재적 위험 비용 계산에 대한 자세한 내용은 [잠재적 위험 비용 계산](../../../manage-work/projects/project-finances/potential-risk-cost.md) 문서를 참조하십시오.



## 프로젝트 순 가치 찾기

Workfront의 다음 영역에서 프로젝트에 대한 순 가치 를 찾을 수 있습니다.

* 비즈니스 사례의 비즈니스 사례 요약 영역\
  비즈니스 사례 요약 영역에 대한 자세한 내용은 문서 [프로젝트에 대한 비즈니스 사례 만들기](../../../manage-work/projects/define-a-business-case/create-business-case.md) [프로젝트에 대한 비즈니스 사례 만들기](../../../manage-work/projects/define-a-business-case/create-business-case.md)의 &quot;비즈니스 사례 요약 이해&quot; 섹션을 참조하십시오.

  ![비즈니스 사례의 순 가치](assets/net-value-on-business-case-summary-highlighted-350x444.png)

* 프로젝트가 포트폴리오와 연결된 경우 Portfolio Optimizer에서

  >[!TIP]
  >
  >모든 프로젝트 순 가치 합계는 포트폴리오의 순 가치입니다.

  Portfolio Optimizer에 대한 자세한 내용은 [Portfolio Optimizer 개요](../../../manage-work/portfolios/portfolio-optimizer/portfolio-optimizer-overview.md)를 참조하세요.

* 다음 목록 및 보고서의 프로젝트 순 값 필드에서 다음을 수행합니다.

   * 프로젝트
   * 작업
   * 문제
   * 프로젝트(재무 데이터)

  보고서 만들기에 대한 자세한 내용은 문서 [사용자 지정 보고서 만들기](../../../reports-and-dashboards/reports/creating-and-managing-reports/create-custom-report.md)를 참조하십시오.
