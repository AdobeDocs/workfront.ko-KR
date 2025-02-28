---
content-type: overview;how-to-procedural
product-area: projects
navigation-topic: financials
title: 원가 성과 지수(CPI) 계산
description: 원가 성과 지수(CPI)는 프로젝트 또는 태스크 레벨에서 계획된 원가와 실제 원가 사이의 관계를 설명합니다. 프로젝트 관리자는 이 지표를 검토하여 특정 시점에 비용 이하로 또는 비용 이상으로 현재 추적 중인 작업 또는 프로젝트를 식별합니다.
author: Lisa
feature: Work Management
exl-id: 7f2efe26-7292-482d-986c-2d2077a7ca52
source-git-commit: b983a780198743a2b87b4b48cf4d6afdf1cee437
workflow-type: tm+mt
source-wordcount: '615'
ht-degree: 0%

---

# 원가 성과 지수(CPI) 계산

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: Linked to the product. Do not change link.)</p>
-->

원가 성과 지수(CPI)는 프로젝트 또는 태스크 레벨에서 계획된 원가와 실제 원가 사이의 관계를 설명합니다. 프로젝트 관리자는 이 지표를 검토하여 특정 시점에 비용 이하로 또는 비용 이상으로 현재 추적 중인 작업 또는 프로젝트를 식별합니다. 비용은 PIM(Performance Index Method)에 따라 몇 시간 또는 몇 달러 단위로 측정할 수 있습니다. 성능 인덱스 메서드 설정에 대한 자세한 내용은 [PIM(성능 인덱스 메서드) 설정](../../../manage-work/projects/project-finances/set-pim.md)을 참조하십시오.

시간 입력이 필요한 조직만 CPI를 사용할 수 있습니다. 또한 비용 기반 PIM 값은 작업 담당자(작업 역할 또는 사용자)에 대한 비용 비율을 정의한 조직에서만 정확합니다.

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

## 원가 성과 지수(CPI) 개요

* [CPI 값](#the-cpi-value)
* [CPI 계산 방법](#how-cpi-is-calculated)

### CPI 값 {#the-cpi-value}

프로젝트 관리자는 CPI 값이 1이면 프로젝트가 정확히 예산대로 진행되고 있음을 이해합니다. 값이 1보다 크면 프로젝트가 예산 미만임을 나타내고(원래 계획보다 적은 시간 또는 비용이 기록됨) 값이 1보다 작으면 프로젝트가 예산 초과임을 나타냅니다(원래 계획보다 많은 시간 또는 비용이 기록됨). 1에서 더 멀수록 계획과의 편차가 더 크다.

| **CPI 값** | **예산에 표시** |
|---|---|
| 1 | 계획 또는 예산 |
| > 1(1보다 큼) | 예산 미만 |
| &lt; 1(1 미만) | 예산 초과 |


### CPI 계산 방법 {#how-cpi-is-calculated}

Adobe Workfront에서 CPI의 계산은 프로젝트에 대해 선택한 성과 지수 방법에 따라 다릅니다. 성능 인덱스 메서드 설정에 대한 자세한 내용은 [PIM(성능 인덱스 메서드) 설정](../../../manage-work/projects/project-finances/set-pim.md)을 참조하십시오.

* [시간 기반 PIM을 사용할 때의 CPI 계산](#cpi-calculations-when-using-hour-based-pim)
* [비용 기반 PIM 사용 시 CPI 계산](#cpi-calculations-when-using-cost-based-pim)

#### 시간 기반 PIM 사용 시 CPI 계산 {#cpi-calculations-when-using-hour-based-pim}

조건

```
Actual Hours > 0 THEN CPI = Total Budgeted Cost Work Performed / Actual Hours
```

그렇지 않은 경우

```
CPI = 1
```

* **부모가 아닌 작업의 경우:**

  ```
  Total Budgeted Cost Work Performed = Planned Hours * (Percent Complete / 100)
  ```

* **상위 작업의 경우:**
수행된 총 예산 비용 작업 수 = 모든 직접 하위 작업에 대해 수행된 총 예산 비용 작업 수 필드의 합계.

* **프로젝트의 경우:**
수행된 총 예산 비용 작업 수 = 모든 최상위 레벨 태스크(상위 및 독립형 태스크)에 대한 수행된 총 예산 비용 작업 수 필드의 합계

BCWP(수행된 총 예산 비용 작업)에 대한 자세한 내용은 [BCWP(수행된 예산 비용 작업) 계산](../../../manage-work/projects/project-finances/calculate-bcwp.md)을 참조하십시오.

#### 비용 기반 PIM 사용 시 CPI 계산 {#cpi-calculations-when-using-cost-based-pim}

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode"><code>CPI = (Planned Cost of Work Performed + Planned Cost of Incurred Expenses) / (Total Actual Cost + Actual Cost of Incurred Expenses) </code> </p>
-->

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode"><code>NOTE: this used to be here before - above - but Anna sent me the one below. I kept the other one, although she is still researching its validity - see this issue: https://hub.workfront.com/issue/5fc7b1cf00012aeebf9e822db8ea2513/overview)</code> </p>
-->

조건

```
Actual Labor Cost + Incurred Actual Expense Cost <> 0 THEN CPI = (Total Budgeted Cost Work Performed + Incurred Planned Expense Cost) / (Actual Labor Cost + Incurred Actual Expense Cost)
```



그렇지 않은 경우

```
CPI = 1
```

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode"><code>(NOTE: above: this used to say: CPI = CPI Labor, but Anna had me fix it on July 21, 2021)</code> </p>
-->

이 계산의 필드는 아래에 설명되어 있습니다.

```
Total Actual Cost = Actual (logged) Hours * Hourly Rate of assignees
```

```
Incurred Actual Expense Cost = Actual Cost
```

발생 경비는 실제 비용이 0보다 큰 경비입니다.

```
Planned Cost of Incurred Expenses = Total of Planned Cost of all incurred expenses
```



<!--
  <p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: Old calculation - taken out by Lilit and replaced below: Planned Cost of Work Performed= (planned labor cost) * (percent complete) / 100 where planned labor cost is the planned hours allocated to assignees * their rates.)</p>
  -->

* 수행된 작업의 계획된 비용은 다음 공식에 의해 계산됩니다.

  ```
  Planned Cost of Work Performed = Planned cost * Percent Complete / 100
  ```

수행된 총 예산 비용 작업은 다음에 대해 계산됩니다.

* **부모가 아닌 작업의 경우:**

  ```
  Total Budgeted Cost Work Performed = Planned Labor Cost * Percent Complete / 100
  ```

* **상위 작업의 경우:**

  ```
  Total Budgeted Cost Work Performed = SUM(Total Budgeted Cost Work Performed field from all direct child tasks)
  ```

* **프로젝트의 경우:**

  ```
  Total Budgeted Cost Work Performed = SUM(Total Budgeted Cost Work Performed field for all top level tasks)
  ```



## 프로젝트 또는 작업에서 CPI 찾기

프로젝트나 작업 목록 또는 보고서에 프로젝트나 작업의 CPI를 표시할 수 있습니다. 또한 프로젝트 또는 작업 수준에서 볼 수 있습니다.

1. CPI를 보려는 프로젝트 또는 작업으로 이동합니다.
1. 프로젝트에 대한 CPI를 보고 있는지 아니면 작업에 대한 CPI를 보고 있는지에 따라 왼쪽 패널에서 **프로젝트 세부 정보** 또는 **작업 세부 정보**&#x200B;을 확장합니다.

1. **재무**&#x200B;을 클릭합니다.

   CPI가 **CPI/ SPI/ CSI** 필드에 표시됩니다.

   프로젝트의 ![CPI](assets/cpi-on-project-nwe.png)
