---
content-type: overview;how-to-procedural
product-area: projects
navigation-topic: financials
title: SPI(일정 성과 인덱스) 계산
description: 스케줄 성과 색인(SPI)은 계획 스케줄과 실제 스케줄 간의 관계를 설명합니다.
author: Alina
feature: Work Management
exl-id: 38259774-f22b-4b69-9e22-5b541118a7de
source-git-commit: a55041ad5a6cd41cd11ec3ade27bf5227ae0ac47
workflow-type: tm+mt
source-wordcount: '439'
ht-degree: 1%

---

# SPI(일정 성과 인덱스) 계산

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: Linked to the product. Do not change link.)</p>
-->

스케줄 성과 색인(SPI)은 계획 스케줄과 실제 스케줄 간의 관계를 설명합니다. Adobe Workfront은 프로젝트 및 작업 수준에서 SPI를 계산합니다. 프로젝트 관리자는 이 지표를 검토하여 현재 작업 또는 프로젝트가 예정보다 앞당겨 추적되는지 아니면 뒤에서 추적되는지를 확인합니다.

## 액세스 요구 사항

이 문서의 절차를 수행하려면 다음 액세스 권한이 있어야 합니다.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront 플랜*</td> 
   <td> <p>모든</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront 라이선스*</td> 
   <td> <p>검토 이상</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">액세스 수준 구성*</td> 
   <td> <p>프로젝트 및 재무 데이터에 대한 액세스 보기</p> <p>참고: 여전히 액세스 권한이 없는 경우 Workfront 관리자에게 액세스 수준에서 추가 제한 사항을 설정하는지 문의하십시오. Workfront 관리자가 액세스 수준을 수정하는 방법에 대한 자세한 내용은 <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">사용자 정의 액세스 수준 만들기 또는 수정</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">개체 권한</td> 
   <td> <p>재무 보기에 대한 권한이 있는 프로젝트에 대한 더 높은 권한 보기</p> <p>추가 액세스 요청에 대한 자세한 내용은 <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">개체에 대한 액세스 요청 </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;어떤 계획, 라이선스 유형 또는 액세스 권한을 보유하고 있는지 알아보려면 Workfront 관리자에게 문의하십시오.

## SPI(성능 인덱스 예약) 개요

* [SPI 값에 표시되는 내용](#what-the-spi-value-shows)
* [Workfront이 SPI를 계산하는 방법](#how-workfront-calculates-spi)

### SPI 값에 표시되는 내용 {#what-the-spi-value-shows}

프로젝트 관리자는 SPI 값이 1이면 프로젝트가 계획 중이거나 일정에 따라 실행되고 있음을 의미합니다.  값이 1보다 큰 값은 프로젝트가 예약보다 앞서있음을 나타내며, 값이 1보다 작은 값은 프로젝트가 예약보다 뒤쳐짐을 의미합니다.  1에서 더 나아가, 그 계획으로부터 더 큰 편차.

| **SPI 값** | **&quot;일정에 따라&quot; 표시** |
|---|---|
| 1 | 계획 또는 일정에 따라 |
| > 1(1보다 큼) | 예정보다 빨리 |
| &lt; 1(1 미만) | 비일정 |

{style=&quot;table-layout:auto&quot;}

### Workfront이 SPI를 계산하는 방법  {#how-workfront-calculates-spi}

Workfront은 다음 수식으로 SPI를 계산합니다.

```
SPI = (Total Planned Hours x % Complete) / Planned Hours Scheduled to Date*
```

*&#42;계획된 시간(일자 기준) = 0인 경우, SPI = 1*.

계획된 시간 스케줄-일자 값은 계산을 수행할 때 분 단위로 계산됩니다. 현재 일자까지 계획된 계획 시간 수를 표시합니다. 재무 데이터를 정확하게 변경할 때 자동으로 다시 계산될 수 있습니다. Workfront에는 이 값을 나타내는 필드가 없습니다.

예를 들어, 하나의 태스크가 있는 프로젝트가 있고 10개의 계획 시간과 10일 기간이 있는 경우, 5일의 계획 시간 스케줄은 5일입니다. 

## 프로젝트 또는 작업에서 SPI 찾기

1. SPI를 보려는 프로젝트 또는 작업으로 이동합니다.
1. 프로젝트에서 SPI를 볼지 또는 작업에 따라 다음 중 하나를 수행하십시오.

   1. 클릭 **프로젝트 세부 사항** 왼쪽 패널에서 **재무** 영역.

   1. 클릭 **작업 세부 사항** 왼쪽 패널에서 **재무** 영역.

      ![](assets/spi-on-project-nwe.png)

1. 를 찾습니다. **CPI/SPI/CSI** 필드.
