---
content-type: overview;how-to-procedural
product-area: projects
navigation-topic: financials
title: 순 값 계산
description: 프로젝트의 순 값은 혜택을 계산하고 비용을 제거한 후 프로젝트의 총 예상 값입니다.
author: Alina
feature: Work Management
exl-id: 44e3f211-c816-4ee1-aafc-c40fc8732f1a
source-git-commit: f2f825280204b56d2dc85efc7a315a4377e551c7
workflow-type: tm+mt
source-wordcount: '397'
ht-degree: 1%

---

# 순 값 계산

프로젝트의 순 값은 혜택을 계산하고 비용을 제거한 후 프로젝트의 총 예상 값입니다. 

## 프로젝트 순 값 개요

Adobe Workfront은 다음 공식을 사용하여 프로젝트의 순 값을 계산합니다. 

```
Project Net Value = Planned Benefit - Budgeted Cost - Potential Risk Cost
```

다음 필드는 프로젝트의 순 값에 영향을 줄 수 있습니다.

* **계획된 혜택**: 프로젝트 소유자가 다음을 완료할 때 지정한 수동 입력입니다 **프로젝트 정보** 비즈니스 케이스의 영역.\
   프로젝트의 계획된 이익에 대한 자세한 내용은 [프로젝트 정보](../../../manage-work/projects/define-a-business-case/areas-of-business-case.md#project-info) 섹션 [비즈니스 사례 영역 개요](../../../manage-work/projects/define-a-business-case/areas-of-business-case.md).

* **예산책정된 비용**: 프로젝트를 처음 시작할 때 예상되는 프로젝트 관련 총 비용입니다.

   다음 **예산책정된 비용** 사용 **예산책정된 인건비** 비즈니스 사례의 자원 예산 영역에서 계산되며, 자원 계획자에서 작업 역할에 대해 책정된 시간과 각 작업 역할의 시간당 비용 비율을 고려합니다.\
   예산책정된 비용은 **순 값** 프로젝트 구성 예산책정된 원가 계산 방법에 대한 자세한 내용은 [예산책정된 비용 계산](../../../manage-work/projects/project-finances/budgeted-cost.md).

* **잠재적 위험 비용**: 이는 프로젝트의 비즈니스 사례 또는 위험 탭에 정의된 대로 프로젝트의 위험 요소와 연관된 비용입니다.\
   프로젝트의 잠재적 위험 비용 계산에 대한 자세한 내용은 문서를 참조하십시오 [잠재적 위험 비용 계산](../../../manage-work/projects/project-finances/potential-risk-cost.md).

    

## 프로젝트 순 값 찾기

Workfront의 다음 영역에서 프로젝트에 대한 순 값을 찾을 수 있습니다.

* 비즈니스 사례의 비즈니스 사례 요약 영역 \
   비즈니스 사례 요약 영역에 대한 자세한 내용은 문서의 &quot;비즈니스 사례 요약 이해&quot; 섹션을 참조하십시오 [프로젝트에 대한 비즈니스 사례 생성](../../../manage-work/projects/define-a-business-case/create-business-case.md) [프로젝트에 대한 비즈니스 사례 생성](../../../manage-work/projects/define-a-business-case/create-business-case.md).

   ![](assets/net-value-on-business-case-summary-highlighted-350x444.png)

* 프로젝트가 포트폴리오와 연결된 경우 Portfolio 최적기에서

   >[!TIP]
   >
   >모든 프로젝트 순 값의 합계는 포트폴리오의 순 값입니다.

   Portfolio 최적기에 대한 자세한 내용은 [Portfolio 최적화 프로그램 개요](../../../manage-work/portfolios/portfolio-optimizer/portfolio-optimizer-overview.md).

* 다음 목록 및 보고서의 프로젝트 순 값 필드에서 다음을 수행합니다.

   * 프로젝트
   * 작업
   * 문제
   * 프로젝트(재무 데이터)
   보고서 만들기에 대한 자세한 내용은 문서를 참조하십시오 [사용자 지정 보고서 만들기](../../../reports-and-dashboards/reports/creating-and-managing-reports/create-custom-report.md).
