---
content-type: overview;how-to-procedural
product-area: projects
navigation-topic: financials
title: 투자 수익률 계산(ROI)
description: ROI(Return On Investment)는 포트폴리오 관리자가 프로젝트의 최초 계획 혜택 및 예산 비용에 대해 프로젝트가 어떻게 수행되고 있는지를 신속하게 확인할 수 있도록 하는 Adobe Workfront 지표입니다.
author: Alina
feature: Work Management
exl-id: 1a3d16cb-8cb1-472e-8102-0ea8e0bc0edd
source-git-commit: f2f825280204b56d2dc85efc7a315a4377e551c7
workflow-type: tm+mt
source-wordcount: '348'
ht-degree: 0%

---

# 투자 수익률 계산(ROI)

ROI(Return On Investment)는 포트폴리오 관리자가 프로젝트의 최초 계획 혜택 및 예산 비용에 대해 프로젝트가 어떻게 수행되고 있는지를 신속하게 확인할 수 있도록 하는 Adobe Workfront 지표입니다.

## 프로젝트 ROI(투자 수익률) 개요

Workfront은 다음 공식을 사용하여 ROI를 계산합니다.

```
Project ROI = [(Project Planned Benefit - Project Budgeted Cost) / Project Budgeted Cost] x 100
```

다음 필드는 프로젝트의 ROI에 영향을 줍니다.

* **프로젝트 계획 혜택**: 비즈니스 케이스의 프로젝트 정보 영역을 완료할 때 프로젝트 소유자가 지정한 수동 입력입니다. 이는 프로젝트 소유자로서 프로젝트를 완료하면 프로젝트의 이점이 있을 것이라고 판단되는 사항에 대한 예측입니다. 이는 특정 통화 금액이며 양수 값이어야 합니다.\
   프로젝트의 계획된 혜택에 대한 자세한 내용은 문서의 &quot;프로젝트 정보&quot; 섹션을 참조하십시오 [프로젝트에 대한 비즈니스 사례 생성](../../../manage-work/projects/define-a-business-case/create-business-case.md).

* **프로젝트 예산책정된 비용**: 프로젝트를 처음 시작할 때 예상되는 프로젝트 관련 총 비용입니다.

   다음 **예산책정된 비용** 사용 **예산책정된 인건비** 비즈니스 사례의 자원 예산 영역에서 계산되며, 자원 계획자에서 작업 역할에 대해 책정된 시간과 각 작업 역할의 시간당 비용 비율을 고려합니다.\
   자세한 내용은 [예산책정된 비용 계산](../../../manage-work/projects/project-finances/budgeted-cost.md).

## 프로젝트 ROI(투자 수익률)를 찾습니다.

Workfront의 다음 영역에서 프로젝트에 대한 ROI 값을 볼 수 있습니다.

* 프로젝트가 포트폴리오와 연결된 경우 Portfolio 최적기에서

   >[!NOTE]
   >
   >모든 프로젝트 ROI 값의 합계는 포트폴리오의 ROI입니다.

   Portfolio 최적기에 대한 자세한 내용은 문서를 참조하십시오 [Portfolio 최적화 프로그램 개요](../../../manage-work/portfolios/portfolio-optimizer/portfolio-optimizer-overview.md).

* 다음 목록 및 보고서의 프로젝트 ROI 필드에서 다음을 수행합니다. 

   * 프로젝트
   * 작업
   * 문제
   * 프로젝트(재무 데이터)
   Workfront에서 보고서 작성에 대한 자세한 내용은 문서를 참조하십시오 [사용자 지정 보고서 만들기](../../../reports-and-dashboards/reports/creating-and-managing-reports/create-custom-report.md).
