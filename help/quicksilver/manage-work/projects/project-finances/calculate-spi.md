---
content-type: overview;how-to-procedural
product-area: projects
navigation-topic: financials
title: SPI(일정 성과 지수) 계산
description: 일정 성과 지수(SPI)는 계획된 일정과 실제 일정 간의 관계를 설명합니다.
author: Lisa
feature: Work Management
exl-id: 38259774-f22b-4b69-9e22-5b541118a7de
source-git-commit: b983a780198743a2b87b4b48cf4d6afdf1cee437
workflow-type: tm+mt
source-wordcount: '419'
ht-degree: 0%

---

# SPI(일정 성과 지수) 계산

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: Linked to the product. Do not change link.)</p>
-->

일정 성과 지수(SPI)는 계획된 일정과 실제 일정 간의 관계를 설명합니다. Adobe Workfront은 프로젝트 및 작업 수준에서 SPI를 계산합니다. 프로젝트 관리자는 이 지표를 검토하여 작업 또는 프로젝트가 현재 예정보다 앞당겨지거나 지연되고 있는지 확인합니다.

## 액세스 요구 사항

+++ 을 확장하여 이 문서의 기능에 대한 액세스 요구 사항을 봅니다.

이 문서의 단계를 수행하려면 다음 액세스 권한이 있어야 합니다.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront 플랜</td> 
   <td>임의</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront 라이선스</td> 
   <td>
   <p>새로운 기능: 밝게 또는 높음</p>
   <p>또는</p>
   <p>현재: 검토 이상</p></td>  
  </tr> 
  <tr> 
   <td role="rowheader">액세스 수준 구성</td> 
   <td>프로젝트 및 재무 데이터에 대한 액세스 보기</td> 
  </tr> 
  <tr> 
   <td role="rowheader">개체 권한</td> 
   <td>재무 보기 권한이 있는 프로젝트에 대한 보기 이상의 권한</td> 
  </tr> 
 </tbody> 
</table>

이 표의 정보에 대한 자세한 내용은 [Workfront 설명서의 액세스 요구 사항](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)을 참조하십시오.

+++

## 일정 성과 지수(SPI) 개요

* [SPI 값이 표시하는 내용](#what-the-spi-value-shows)
* [Workfront에서 SPI를 계산하는 방법](#how-workfront-calculates-spi)

### SPI 값의 내용 {#what-the-spi-value-shows}

프로젝트 관리자는 SPI 값이 1이면 프로젝트가 계획 중이거나 일정에 있음을 의미합니다.  값이 1보다 크면 프로젝트가 예정보다 빨라짐을 나타내고 값이 1보다 작으면 프로젝트가 예정보다 늦어짐을 의미합니다.  1에서 더 멀수록 계획과의 편차가 더 크다.

| **SPI 값** | **일정에 따라 표시** |
|---|---|
| 1 | 계획 또는 일정에 따라 |
| > 1(1보다 큼) | 예정보다 빨리 |
| &lt; 1(1 미만) | 지연됨 |

{style="table-layout:auto"}

### Workfront에서 SPI를 계산하는 방법  {#how-workfront-calculates-spi}

Workfront은 다음 수식으로 SPI를 계산합니다.

```
SPI = (Total Planned Hours x % Complete) / Planned Hours Scheduled to Date*
```

*&#42;계획된 시간이 일자 = 0으로 예약된 경우 SPI = 1*.

계획된 시간 스케줄 누계는 계산을 수행할 때 분 단위로 계산됩니다. 현재 날짜까지 계획된 계획된 시간 수를 표시합니다. 재무 데이터를 정확하게 변경하면 자동으로 다시 계산할 수 있습니다. Workfront에는 이 값을 나타내는 필드가 없습니다.

예를 들어, 1개의 작업이 있는 프로젝트가 있고 작업에 10개의 계획된 시간과 10일의 기간이 있는 경우, 5일째의 일자에 대한 계획된 시간 스케줄은 5입니다. 

## 프로젝트 또는 작업에서 SPI 찾기

1. SPI를 보려는 프로젝트 또는 작업으로 이동합니다.
1. 프로젝트에서 SPI를 볼 것인지 아니면 작업에서 SPI를 볼 것인지에 따라 다음 중 하나를 수행합니다.

   1. 왼쪽 패널에서 **프로젝트 세부 정보**&#x200B;를 클릭한 다음 **재무** 영역을 봅니다.

   1. 왼쪽 패널에서 **작업 세부 정보**&#x200B;를 클릭한 다음 **재무** 영역을 봅니다.

      ![프로젝트의 SPI](assets/spi-on-project-nwe.png)

1. **CPI/ SPI/ CSI** 필드를 찾습니다.
