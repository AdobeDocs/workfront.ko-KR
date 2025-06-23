---
content-type: overview;how-to-procedural
product-area: projects
navigation-topic: financials
title: CSI(원가 일정 성과 지표) 계산
description: CSI(Cost Schedule Performance Index)는 CPI(Cost Performance Index)와 SPI(Schedule Performance Index)를 비용과 일정의 균형을 맞추는 하나의 일반 지표로 결합하는 자동 계산입니다.
author: Lisa
feature: Work Management
exl-id: 38a8c5e0-b812-499d-8fe7-a71ddccb3aad
source-git-commit: abf5f21281b05dedfecbe71c6ffbf54ee69e2460
workflow-type: tm+mt
source-wordcount: '331'
ht-degree: 0%

---

# CSI(원가 일정 성과 지표) 계산

<!-- Audited: 6/2025 -->

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: Linked to the product. Do not change link.) </p>
-->

## CSI(Cost Schedule Performance Index) 개요

CSI(Cost Schedule Performance Index)는 CPI(Cost Performance Index)와 SPI(Schedule Performance Index)를 비용과 일정의 균형을 맞추는 하나의 일반 지표로 결합하는 자동 계산입니다. 이러한 값을 함께 곱하면 단일 지표가 더 낮은 예산에서 오래 걸리는 일정을 설명할 수 있으며 그 반대의 경우도 가능합니다. 프로젝트 관리자는 이를 사용하여 프로젝트 중간 일정을 추진하기 위해 비용이 투입될 때 일반 프로젝트 또는 작업 상태를 확인할 수 있습니다.

>[!TIP]
>
>Adobe Workfront은 작업과 프로젝트 모두에 대한 CSI를 계산하지만 문제는 계산하지 않습니다.

조직에 다음 시나리오가 있는 경우에만 이 지표가 제공하는 정보를 활용할 수 있습니다.

* 사용자가 완료하는 작업의 시간을 기록하고 있습니다. 이는 시간을 기반으로 CSI를 계산합니다.
* 사용자 또는 작업 역할에는 시간당 비용이 연관되어 있습니다. 이것은 비용을 기반으로 CSI를 계산합니다.

## Workfront에서 CSI(Cost Schedule Performance Index)를 계산하는 방법

Workfront은 다음 공식을 사용하여 프로젝트 또는 작업의 비용 성과 지수(CSI)를 계산합니다.

`CSI = CPI x SPI`

CPI에 대한 자세한 내용은 [CPI(비용 성과 지표) 계산](../../../manage-work/projects/project-finances/calculate-cpi.md) 문서를 참조하십시오.

SPI에 대한 자세한 내용은 [SPI(일정 성과 지수) 계산](../../../manage-work/projects/project-finances/calculate-spi.md) 문서를 참조하십시오.

CSI에는 다음과 같은 세 가지 가능한 값이 있습니다.

* 1 = 전체 계획 준수
* \>1 = 예산 일정 조합 미만
* &lt;1 = 예산 초과 스케줄 조합

![CSI](assets/csi-highlighted.png)

## CSI(Cost Schedule Performance Index) 찾기

>[!CAUTION]
>
>프로젝트 또는 작업의 CSI 값을 보려면 액세스 수준에서 재무 데이터 보기에 대한 액세스 권한과 프로젝트 또는 작업을 볼 수 있는 권한이 있어야 합니다.

Workfront의 다음 영역에서 CSI를 찾을 수 있습니다.

* 프로젝트 세부 정보 섹션의 재무 영역.
* 작업 세부 정보 섹션의 재무 영역.
* 프로젝트 또는 작업 보기.
* 프로젝트 또는 작업 보고서.
