---
content-type: overview;how-to-procedural
product-area: projects
navigation-topic: financials
title: 원가 스케줄 성과 인덱스 계산(CSI)
description: 원가 스케줄 성과 지수(CSI)는 원가 성과 지수(CPI)와 스케줄 성과 지수(SPI)를 원가 및 스케줄을 조정하는 하나의 일반 지표에 결합하는 자동 계산입니다.
author: Alina
feature: Work Management
exl-id: 38a8c5e0-b812-499d-8fe7-a71ddccb3aad
source-git-commit: a55041ad5a6cd41cd11ec3ade27bf5227ae0ac47
workflow-type: tm+mt
source-wordcount: '337'
ht-degree: 0%

---

# 원가 스케줄 성과 인덱스 계산(CSI)

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: Linked to the product. Do not change link.) </p>
-->

## 원가 스케줄 성능 인덱스(CSI) 개요

원가 스케줄 성과 지수(CSI)는 원가 성과 지수(CPI)와 스케줄 성과 지수(SPI)를 원가 및 스케줄을 조정하는 하나의 일반 지표에 결합하는 자동 계산입니다. 이 값들을 함께 곱함으로써, 단일 지표는 더 낮은 예산에서 또는 그 반대로 오래 된 일정을 계산할 수 있습니다. 프로젝트 관리자는 이를 사용하여 프로젝트 중간에 일정을 계획하기 위해 비용이 소모될 때 일반적인 프로젝트 또는 작업 상태를 결정할 수 있습니다.

>[!TIP]
>
>Adobe Workfront은 작업과 프로젝트 모두에 대한 CSI를 계산합니다. Workfront에서 문제에 대한 CSI 값을 계산하지 않습니다.

다음 정보가 조직에 있는 경우에만 이 지표로 제공된 정보를 활용할 수 있습니다.

* 사용자가 완료하는 작업에 대해 시간을 기록하고 있습니다.\
   시간이 지남에 따라 CSI가 계산됩니다.
* 사용자 또는 작업 역할에는 시간 당 비용이 연결되어 있습니다. 

   이를 통해 비용을 기준으로 CSI가 계산됩니다.

## Workfront이 CSI(원가 스케줄 성과 인덱스)를 계산하는 방법

Workfront은 다음 공식을 사용하여 프로젝트 또는 작업의 비용 성과 색인(CSI)을 계산합니다.

```
CSI = CPI x SPI
```

CPI에 대한 자세한 내용은 문서를 참조하십시오 [원가 성과 지수 계산(CPI)](../../../manage-work/projects/project-finances/calculate-cpi.md).

SPI에 대한 자세한 내용은 문서를 참조하십시오 [SPI(일정 성과 인덱스) 계산](../../../manage-work/projects/project-finances/calculate-spi.md).

CSI에는 다음 세 가지 가능한 값이 있습니다.

* 1 = 전체 계획을 따릅니다.   
* 
   >1 = 예산 스케줄 조합 아래
* &lt;1 = 초과 예산 스케줄 조합

![](assets/csi-highlighted.png)

## 원가 스케줄 성능 인덱스(CSI)를 찾습니다.

>[!CAUTION]
>
>프로젝트나 작업의 CSI 값을 보려면 액세스 수준에서 재무 데이터 보기에 액세스할 수 있어야 하며 프로젝트 또는 작업을 볼 수 있는 권한도 있어야 합니다.

Workfront의 다음 영역에서 CSI를 찾을 수 있습니다.

* 프로젝트 상세내역 섹션의 재무 영역.
* 작업 세부 사항 섹션의 재무 영역입니다.
* 프로젝트 또는 작업 보기
* 프로젝트 또는 작업 보고서
