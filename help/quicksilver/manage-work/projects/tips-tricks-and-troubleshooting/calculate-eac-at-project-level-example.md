---
content-type: tips-tricks-troubleshooting
product-area: projects
navigation-topic: tips-tricks-and-troubleshooting-projects
title: 계산 예 - 프로젝트 수준에서 EAC 계산
description: PIM = 시간 기반
author: Alina
feature: Work Management
exl-id: ff88b7e3-2a5b-464f-bed1-6848067840b8
source-git-commit: a849ecaf6097dcdc924aaab2867f37bf57d5bc09
workflow-type: tm+mt
source-wordcount: '1768'
ht-degree: 9%

---

# 계산 예 - 프로젝트 수준에서 EAC 계산

## EAC 메서드: 프로젝트 수준에서 계산

* [PIM = 시간 기반](#pim-hour-based)
* [PIM= 비용 기반](#pim-cost-based)

### PIM = 시간 기반 {#pim-hour-based}

* [단순 예: 프로젝트에 하위 작업이 없습니다.](#simple-example-project-has-no-children-tasks)
* [복잡한 예: 프로젝트에 하위 작업이 있습니다.](#complicated-example-project-has-children-tasks)

#### 단순 예: 프로젝트에 하위 작업이 없습니다. {#simple-example-project-has-no-children-tasks}

PIM = 시간 기반

EAC 방법 = 프로젝트 수준에서 계산 ****

1. 비용/hr이 $100.00인 사용자 1에 세 개의 태스크(하위 태스크 없음)가 지정된 프로젝트 A를 생성합니다.
1. 아래 테이블에 따라 각 작업에 계획 및 실제 시간을 추가하고 % 완료 를 추가합니다.

   <table style="table-layout:auto">
    <col>
    <col>
    <col>
    <col>
    <thead>
     <tr>
      <th><br><p><strong>작업</strong></p></th>
      <th><br><p><strong>계획된 시간</strong></p></th>
      <th><br><p><strong>실제 근로시간</strong></p></th>
      <th><p><strong>% 완료</strong></p></th>
     </tr>
    </thead>
    <tbody>
     <tr>
      <td><p>작업 1</p></td>
      <td><p>5시간</p></td>
      <td><p>25시간</p></td>
      <td><p>20%</p></td>
     </tr>
     <tr>
      <td><p>작업 2</p></td>
      <td><p>10시간</p></td>
      <td><p>25시간</p></td>
      <td><p>30%</p></td>
     </tr>
     <tr>
      <td><p>작업 3</p></td>
      <td><p>15시간</p></td>
      <td><p>25시간</p></td>
      <td><p>40%</p></td>
     </tr>
    </tbody>
   </table>

1. 프로젝트에서 재무 재계산
1. **작업 1용 CPI** = .04 다음과 같이 계산됩니다.\
   **작업 1용 CPI** = *IF* 실제 시간 > 0 *THEN* CPI = TotalBudgetCostWorkPerformed/실제 시간\
      *ELSE* CPI = 1\
   **작업 1용 CPI** = 1 / 25\
   **작업 1용 CPI** = .04

1. **작업 1용 EAC** = 다음과 같이 계산되는 125시간\
   **작업 1용 EAC** = *IF* CPI &lt;> 0 *THEN* EAC = 계획된 시간/CPI\
       *ELSE* EAC = 계획 시간 + 실제 시간\
   **작업 1용 EAC** = 5 / 0.04\
   **작업 1용 EAC** = 125시간****

1. 작업 2 및 3의 CPI / EAC:\
   작업 2 = 0.12 / 83.33시간\
   작업 3 = 0.24 / 62.5시간

1. **프로젝트용 CPI** = .13 다음과 같이 계산됩니다.\
   **프로젝트용 CPI** = *IF* 실제 시간 > 0 *THEN* CPI = TotalBudgetCostWorkPerformed/실제 시간\
       *ELSE* CPI = 1\
   **프로젝트용 CPI** = 10 / 75\
   **프로젝트용 CPI** = .13

1. **프로젝트용 EAC** = 다음과 같이 계산되는 225시간\
   **프로젝트용 EAC** = *IF* CPI &lt;> 0 *THEN* EAC = 계획된 시간/CPI\
       *ELSE* EAC = 계획 시간 + 실제 시간\
   **프로젝트용 EAC** = 30 / .13333\
   **프로젝트용 EAC** = 225시간

#### 복잡한 예: 프로젝트에 하위 작업이 있습니다. {#complicated-example-project-has-children-tasks}

PIM = 시간 기반

EAC 메서드 = 프로젝트 수준에서 계산

1. 작업 3이 태스크 4 및 5의 상위이고 태스크 1이 태스크 2 및 3의 상위인 6개의 태스크로 프로젝트 A를 생성합니다.\
   작업 1\
      작업 2\
      작업 3\
         작업 4\
         작업 5\
   작업 6

1. 비용/시간당 비율이 $100.00인 사용자 1에 태스크 2, 4, 5 및 6을 지정합니다.
1. 아래 테이블에 따라 각 작업에 대해 계획된/실제 시간 및 % 완료 를 추가합니다.

   >[!NOTE]
   >
   >작업 1 및 3의 경우 실제 시간만 추가합니다.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th> <br> <p><strong>작업</strong> </p> </th> 
   <th> <br> <p><strong>계획된 시간</strong> </p> </th> 
   <th> <br> <p><strong>실제 근로시간</strong> </p> </th> 
   <th> <p><strong>% 완료</strong> </p> </th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td> <p>작업 1</p> </td> 
   <td> </td> 
   <td> <p>10시간</p> </td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td> <p>작업 2</p> </td> 
   <td> <p>5시간</p> </td> 
   <td> <p>10시간</p> </td> 
   <td> <p>20%</p> </td> 
  </tr> 
  <tr> 
   <td> <p>작업 3</p> </td> 
   <td> </td> 
   <td> <p>10시간</p> </td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td> <p>작업 4</p> </td> 
   <td> <p>10시간</p> </td> 
   <td> <p>10시간</p> </td> 
   <td> <p>40%</p> </td> 
  </tr> 
  <tr> 
   <td> <p>작업 5</p> </td> 
   <td> <p>15시간</p> </td> 
   <td> <p>10시간</p> </td> 
   <td> <p>50%</p> </td> 
  </tr> 
  <tr> 
   <td> <p>작업 6</p> </td> 
   <td> <p>20시간</p> </td> 
   <td> <p>10시간</p> </td> 
   <td> <p>60%</p> </td> 
  </tr> 
 </tbody> 
</table>

1. 프로젝트에 바로 50시간을 추가합니다(자세히>시간>로그 시간).
1. **작업 2용 CPI** = 다음과 같이 계산된 .1.\
   **작업 2용 CPI** = *IF* 실제 시간 > 0 *THEN* CPI = TotalBudgetCostWorkPerformed/실제 시간\
       *ELSE* CPI = 1\
   **작업 2용 CPI** = 1 / 10\
   **작업 2용 CPI** =.1

1. **작업 2용 EAC** = 다음과 같이 계산되는 50시간\
   **작업 2용 EAC** = *IF* CPI &lt;> 0 *THEN* EAC = 계획된 시간/CPI\
       *ELSE* EAC = 계획 시간 + 실제 시간\
   **작업 2용 EAC** = 5 / .1\
   **작업 2용 EAC** = 50시간

1. 작업 4, 5 및 6에 대한 CPI/EAC는 다음과 같습니다.\
   작업 4: 25시간\
   작업 5: 20시간\
   작업 6: 1.2 / 16.67시간

1. **작업 3용 CPI** = .38 다음과 같이 계산됩니다.\
   **작업 3용 CPI** = *IF* 실제 시간 > 0 *THEN* CPI = TotalBudgetCostWorkPerformed/실제 시간\
       *ELSE* CPI = 1\
   **작업 3용 CPI** = 11.5 / 30\
   **작업 3용 CPI** =.38

1. **작업 3용 EAC** = 다음과 같이 계산되는 65.22시간\
   **작업 3용 EAC** = *IF* CPI &lt;> 0 *THEN* EAC = 계획된 시간/CPI\
       *ELSE* EAC = 계획 시간 + 실제 시간\
   **작업 3용 EAC** = 25 / .383333\
   **작업 3용 EAC** = 65.22시간

1. **작업 1용 CPI** = .25 다음과 같이 계산됩니다.\
   **작업 1용 CPI** = *IF* 실제 시간 > 0 *THEN* CPI = TotalBudgetCostWorkPerformed/실제 시간\
       *ELSE* CPI = 1\
   **작업 1용 CPI** = 12.5 / 50\
   **작업 1용 CPI** =.25

1. **작업 1용 EAC** = 다음과 같이 계산되는 120시간\
   **작업 1용 EAC** = *IF* CPI &lt;> 0 *THEN* EAC = 계획된 시간 / CPI\
       *ELSE* EAC = 계획 시간 + 실제 시간\
   **작업 1용 EAC** = 30/.25\
   **작업 1용 EAC** = 120시간

1. **프로젝트용 CPI** = .22 다음과 같이 계산됩니다.\
   **프로젝트용 CPI** = *IF* 실제 시간 > 0 *THEN* CPI = TotalBudgetCostWorkPerformed/실제 시간\
       *ELSE* CPI = 1\
   **프로젝트용 CPI** = 24.5 / 110\
   **프로젝트용 CPI** = .22272\
   **프로젝트용 CPI** = .22

1. **프로젝트용 EAC** = 다음과 같이 계산되는 224.49시간\
   **프로젝트용 EAC** = *IF* CPI &lt;> 0 *THEN* EAC = 계획된 시간/CPI\
       *ELSE* EAC = 계획 시간 + 실제 시간\
   **프로젝트용 EAC** = 50 / .22272\
   **프로젝트용 EAC** = 224.49시간

### PIM= 비용 기반 {#pim-cost-based}

* [단순 예: 프로젝트에 하위 작업이 없습니다.](#simple-example-project-has-no-children-tasks)
* [복잡한 예: 프로젝트에 하위 작업이 있습니다.](#complicated-example-project-has-children-tasks)

#### 단순 예: 프로젝트에 하위 작업이 없습니다. {#simple-example-project-has-no-children-tasks-1}

PIM = 비용 기반

EAC 메서드 = 프로젝트 수준에서 계산

1. 비용/hr이 $100.00인 사용자 1에 세 개의 태스크(하위 태스크 없음)가 지정된 프로젝트 A를 생성합니다.
1. 각 작업에 계획 / 실제 시간을 추가하고 아래 테이블에 따라 % 완료 를 추가합니다.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <col> 
 <col> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th> <br> <p><strong>작업</strong> </p> </th> 
   <th> <br> <p><strong>계획된 시간</strong> </p> </th> 
   <th> <br> <p><strong>Pln Lbr 비용</strong> </p> </th> 
   <th> <br> <p><strong>실제 근로시간</strong> </p> </th> 
   <th> <br> <p><strong>법률 비용</strong> </p> </th> 
   <th> <p><strong>% 완료</strong> </p> </th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td> <p>작업 1</p> </td> 
   <td> <p>5시간</p> </td> 
   <td> <p>$500.00</p> </td> 
   <td> <p>25시간</p> </td> 
   <td> <p>$2,500.00</p> </td> 
   <td> <p>20%</p> </td> 
  </tr> 
  <tr> 
   <td> <p>작업 2</p> </td> 
   <td> <p>10시간</p> </td> 
   <td> <p>$1,000.00</p> </td> 
   <td> <p>25시간</p> </td> 
   <td> <p>$2,500.00</p> </td> 
   <td> <p>30%</p> </td> 
  </tr> 
  <tr> 
   <td> <p>작업 3</p> </td> 
   <td> <p>15시간</p> </td> 
   <td> <p>$1,500.00</p> </td> 
   <td> <p>25시간</p> </td> 
   <td> <p>$2,500.00</p> </td> 
   <td> <p>40%</p> </td> 
  </tr> 
 </tbody> 
</table>

1. 아래 표에 따라 각 작업에 비용을 추가합니다.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th> <p><strong>작업</strong> </p> </th> 
   <th> <p><strong>경비</strong> </p> </th> 
   <th> <p><strong>계획된 금액</strong> </p> </th> 
   <th> <p><strong>실제 금액</strong> </p> </th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td> <p>작업 1</p> </td> 
   <td> <p>작업 1 확장 1</p> </td> 
   <td> <p>$300.00</p> </td> 
   <td> <p>$400.00</p> </td> 
  </tr> 
  <tr> 
   <td> <p>작업 1</p> </td> 
   <td> <p>작업 1 확장 2</p> </td> 
   <td> <p>$500.00</p> </td> 
   <td> <p>$0.00</p> </td> 
  </tr> 
  <tr> 
   <td> <p>작업 2</p> </td> 
   <td> <p>작업 2 확장</p> </td> 
   <td> <p>$200.00</p> </td> 
   <td> <p>$100.00</p> </td> 
  </tr> 
  <tr> 
   <td> <p>작업 3</p> </td> 
   <td> <p>작업 3 확장</p> </td> 
   <td> <p>$800.00</p> </td> 
   <td> <p>$700.00</p> </td> 
  </tr> 
 </tbody> 
</table>

1. 다음과 같이 프로젝트에 두 개의 비용(즉, 작업에 연결되지 않음)을 추가합니다.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th> <p><strong>경비</strong> </p> </th> 
   <th> <p><strong>계획된 금액</strong> </p> </th> 
   <th> <p><strong>실제 금액</strong> </p> </th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td> <p>프로젝트 확장 1</p> </td> 
   <td> <p>$1,000.00</p> </td> 
   <td> <p>$1,500.00</p> </td> 
  </tr> 
  <tr> 
   <td> <p>작업 1 확장 2</p> </td> 
   <td> <p>$2,500.00</p> </td> 
   <td> <p>$0.00</p> </td> 
  </tr> 
 </tbody> 
</table>

1. 위의 값을 기준으로 발생됨/발생되지 않은 비용은 다음과 같이 결정됩니다.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th> <p><strong>작업</strong> </p> </th> 
   <th> <p><strong>발생되지 않은 계획 비용</strong> </p> </th> 
   <th> <p><strong>예상 비용 발생</strong> </p> </th> 
   <th> <p><strong>실제 비용 발생</strong> </p> </th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td> <p>작업 1</p> </td> 
   <td> <p>$500.00</p> </td> 
   <td> <p>$300.00</p> </td> 
   <td> <p>$400.00</p> </td> 
  </tr> 
  <tr> 
   <td> <p>작업 2</p> </td> 
   <td> <p>$0.00</p> </td> 
   <td> <p>$200.00</p> </td> 
   <td> <p>$100.00</p> </td> 
  </tr> 
  <tr> 
   <td> <p>작업 3</p> </td> 
   <td> <p>$0.00</p> </td> 
   <td> <p>$800.00</p> </td> 
   <td> <p>$700.00</p> </td> 
  </tr> 
  <tr> 
   <td> <p>프로젝트</p> </td> 
   <td> <p>$3,000.00</p> </td> 
   <td> <p>$2,300.00</p> </td> 
   <td> <p> $2,700.00 <strong></strong></p> </td> 
  </tr> 
 </tbody> 
</table>

1. 프로젝트 작업에서 재무 재계산을 실행합니다
1. **작업 1용 CPI** = .14
1. **작업 1용 CPI****** = .14 다음과 같이 계산됩니다.\
   **CPI**  **작업 1** = *IF* 실제 노무비 + ExtualExpenseCost &lt;> 0 *THEN*

   ```
   CPI = (TotalBudgetedCostWorkPerformed + IncurredPlannedExpenseCost) / (ActualLaborCost + IncurredActualExpenseCost)
   ```

   *    ELSE* CPI = CPI_Labor\
   **작업 1용 CPI****** = (100+300) / (2500+400)\
   **CPI**  **작업 1** = 400 / 2900\
   **CPI**  **작업 1**  = .14****

1. **작업 1용 EAC****** = $13,400.00\
   **CPI 노동력**  **작업 1** = 실제 노무비 &lt;> 0인 경우

   ```
   CPI_Labor = TotalBudgetedCostWorkPerformed/Actual Labor Cost
   ```

      ELSE CPI_Labor = 1\
   **CPI 노동력**  **작업 1** = 100/2500\
   **CPI 노동력**  **작업 1** = .04 ****** EAC 노동력&#x200B;****작업 1 **=*IF *CPI_Labor &lt;> 0*THEN *EAC 노무 = 계획된 노무 비용/CPI_Labor\
   *    ELSE* EAC 노무 = 계획된 노무비 + 실제 노무비\
   **EAC 노무&#x200B;****작업 1** = 500.00/.04용\
   **태스크 1용 EAC 노무****** = $12,500.00\
   **작업 1에 대한 EAC 비용****** = ProredActualExpenseCost + NotProredPlanningExpense\
   **작업 1에 대한 EAC 비용****** = $400.00 + $500.00\
   **작업 1에 대한 EAC 비용****** = $900.00\
   **작업 1용 EAC****** = EAC 노무 + EAC 비용\
   **작업 1용 EAC******  = $12,500.00 + $900.00\
   **작업 1용 EAC******  = $13,400.00

1. 작업 2 및 작업 3의 CPI / EAC 값은 다음과 같습니다.\
   작업 2 = .19 / $8,433.33\
   작업 3 = .44 / $6,950.00

1. **프로젝트용 CPI** = .32 다음과 같이 계산됩니다.\
   **프로젝트용 CPI****** = *IF* 실제 노무비 + ExtualExpenseCost &lt;> 0 *THEN*

   ```
   CPI = (TotalBudgetedCostWorkPerformed + IncurredPlannedExpenseCost)/ActualLaborCost + IncurredActualExpenseCost)
   ```

   *   ELSE* CPI = CPI_Labor\
   **프로젝트용 CPI****** = (1000 + 2300) / (7500 + 2700)\
   **프로젝트용 CPI****** = 3300 / 10200\
   **프로젝트용 CPI****** = .32

1. **프로젝트용 EAC** = 다음과 같이 계산되는 $28,200.00:\
   **CPI Labor****for Project** = 실제 노무비 &lt;> 0인 경우

   ```
   CPI_Labor = TotalBudgetedCostWorkPerformed/Actual Labor Cost
   ```

      ELSE CPI_Labor = 1\
   **CPI Labor****for Project** = 1000 / 7500\
   **CPI Labor****for Project** = .13333\
   **CPI Labor****for Project** = .13

   **프로젝트용 EAC Labor****** = *IF* CPI_Labor &lt;> 0 *THEN*

   ```
   EAC Labor = Planned Labor Cost/CPI_Labor
   ```

   *   ELSE* EAC 노무 = 계획된 노무비 + 실제 노무비\
   **프로젝트용 EAC Labor****** = 3000/ .13333\
   **프로젝트용 EAC Labor****** = $22,500.00

   **EAC 비용****프로젝트** =

   ```
   IncurredActualExpenseCost + NotIncurredPlannedExpense
   ```

   **EAC 비용****프로젝트** = $3000.00 + 2,700.00\
   **EAC 비용****프로젝트** = $5,700.00

   **EAC****Project** = EAC 노무 + EAC 비용\
   **EAC****Project**  = $22,500.00 + $5,700.00\
   **EAC****Project**  = $28,200.00

#### 복잡한 예: 프로젝트에 하위 작업이 있습니다. {#complicated-example-project-has-children-tasks-1}

PIM = 비용 기반

EAC 메서드 = 프로젝트 수준에서 계산

1. 작업 3이 태스크 4 및 5의 상위이고 태스크 1이 태스크 2 및 3의 상위인 6개의 태스크로 프로젝트 A를 생성합니다.\
   작업 1\
      작업 2\
      작업 3\
         작업 4\
         작업 5\
   작업 6

1. 비용/시간당 비율이 $100.00인 사용자 1에 태스크 2, 4, 5 및 6을 지정합니다.
1. 아래 테이블에 따라 각 작업에 대한 계획/실제 시간 및 % 완료 를 추가합니다.

   >[!NOTE]
   >
   >작업 1 및 3의 경우 실제 시간만 추가합니다.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <col> 
 <col> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th> <br> <p><strong>작업</strong> </p> </th> 
   <th> <br> <p><strong>계획된 시간</strong> </p> </th> 
   <th> <br> <p><strong>Pln Lbr 비용</strong> </p> </th> 
   <th> <br> <p><strong>실제 근로시간</strong> </p> </th> 
   <th> <br> <p><strong>법률 비용</strong> </p> </th> 
   <th> <p><strong>% 완료</strong> </p> </th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td> <p>작업 1</p> </td> 
   <td> </td> 
   <td> </td> 
   <td> <p>10시간</p> </td> 
   <td> <p>$1,000.00</p> </td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td> <p>작업 2</p> </td> 
   <td> <p>5시간</p> </td> 
   <td> <p>$500.00</p> </td> 
   <td> <p>10시간</p> </td> 
   <td> <p>$1,000.00</p> </td> 
   <td> <p>20%</p> </td> 
  </tr> 
  <tr> 
   <td> <p>작업 3</p> </td> 
   <td> </td> 
   <td> </td> 
   <td> <p>10시간</p> </td> 
   <td> <p>$1,000.00</p> </td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td> <p>작업 4</p> </td> 
   <td> <p>10시간</p> </td> 
   <td> <p>$1,000.00</p> </td> 
   <td> <p>10시간</p> </td> 
   <td> <p>$1,000.00</p> </td> 
   <td> <p>40%</p> </td> 
  </tr> 
  <tr> 
   <td> <p>작업 5</p> </td> 
   <td> <p>15시간</p> </td> 
   <td> <p>$1,500.00</p> </td> 
   <td> <p>10시간</p> </td> 
   <td> <p>$1,000.00</p> </td> 
   <td> <p>50%</p> </td> 
  </tr> 
  <tr> 
   <td> <p>작업 6</p> </td> 
   <td> <p>20시간</p> </td> 
   <td> <p>$2,000.00</p> </td> 
   <td> <p>10시간</p> </td> 
   <td> <p>$1,000.00</p> </td> 
   <td> <p>60%</p> </td> 
  </tr> 
 </tbody> 
</table>

1. 프로젝트에 직접 기록되는 실제 인건비 비용이 5,000.00달러가 되도록 50시간을 프로젝트에 직접 추가합니다(자세히>시간>로그 시간). ****
1. 아래 표에 따라 각 작업에 비용을 추가합니다(읽기 쉽게 만들기 위해 각 작업 사이에 빈 행을 추가했습니다.).

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th> <p><strong>작업</strong> </p> </th> 
   <th> <p><strong>경비</strong> </p> </th> 
   <th> <p><strong>계획된 금액</strong> </p> </th> 
   <th> <p><strong>실제 금액</strong> </p> </th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td> <p>작업 1</p> </td> 
   <td> <p>작업 1 확장 1</p> </td> 
   <td> <p>$300.00</p> </td> 
   <td> <p>-$400.00</p> </td> 
  </tr> 
  <tr> 
   <td> <p>작업 1</p> </td> 
   <td> <p>작업 1 확장 2</p> </td> 
   <td> <p>-$500.00</p> </td> 
   <td> <p>$800.00</p> </td> 
  </tr> 
  <tr> 
   <td> <p>작업 1</p> </td> 
   <td> <p>작업 1 확장 3</p> </td> 
   <td> <p>$400.00</p> </td> 
   <td> <p>$0.00</p> </td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td> </td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td> <p>작업 2</p> </td> 
   <td> <p>작업 2 확장 1</p> </td> 
   <td> <p>$500.00</p> </td> 
   <td> <p>$700.00</p> </td> 
  </tr> 
  <tr> 
   <td> <p>작업 2</p> </td> 
   <td> <p>작업 2 확장 2</p> </td> 
   <td> <p>-$400.00</p> </td> 
   <td> <p>$0.00</p> </td> 
  </tr> 
  <tr> 
   <td> <p>작업 2</p> </td> 
   <td> <p>작업 2 Exp 3</p> </td> 
   <td> <p>-$200.00</p> </td> 
   <td> <p>$600.00</p> </td> 
  </tr> 
  <tr> 
   <td> <p>작업 2</p> </td> 
   <td> <p>작업 2 확장 4</p> </td> 
   <td> <p>$700.00</p> </td> 
   <td> <p>-$200.00</p> </td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td> </td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td> <p>작업 3</p> </td> 
   <td> <p>작업 3 확장</p> </td> 
   <td> <p>$0.00</p> </td> 
   <td> <p>$1,000.00</p> </td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td> </td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td> <p>작업 4</p> </td> 
   <td> <p>작업 4 확장 1</p> </td> 
   <td> <p>$800.00</p> </td> 
   <td> <p>$0.00</p> </td> 
  </tr> 
  <tr> 
   <td> <p>작업 4</p> </td> 
   <td> <p>작업 4 확장 2</p> </td> 
   <td> <p>-$100.00</p> </td> 
   <td> <p>$300.00</p> </td> 
  </tr> 
  <tr> 
   <td> <p>작업 4 </p> </td> 
   <td> <p>작업 4 확장 3</p> </td> 
   <td> <p>-200.00</p> </td> 
   <td> <p>$0.00</p> </td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td> </td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td> <p>작업 5</p> </td> 
   <td> <p>작업 5 확장 1</p> </td> 
   <td> <p>$700.00</p> </td> 
   <td> <p>$800.00</p> </td> 
  </tr> 
  <tr> 
   <td> <p>작업 5</p> </td> 
   <td> <p>작업 5 확장 2</p> </td> 
   <td> <p>-$100.00</p> </td> 
   <td> <p>$300.00</p> </td> 
  </tr> 
  <tr> 
   <td> <p>작업 5</p> </td> 
   <td> <p>작업 5 Exp 3</p> </td> 
   <td> <p>-$400.00</p> </td> 
   <td> <p>-$200.00</p> </td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td> </td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td> <p>작업 6</p> </td> 
   <td> <p>작업 6 확장 1</p> </td> 
   <td> <p>$600.00</p> </td> 
   <td> <p>$700.00</p> </td> 
  </tr> 
  <tr> 
   <td> <p>작업 6</p> </td> 
   <td> <p>작업 6 확장 2</p> </td> 
   <td> <p>$500.00</p> </td> 
   <td> <p>-$300.0</p> </td> 
  </tr> 
 </tbody> 
</table>

1. 다음과 같이 프로젝트에 두 개의 비용(즉, 작업에 연결되지 않음)을 추가합니다.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th> <p><strong>경비</strong> </p> </th> 
   <th> <p><strong>계획된 금액</strong> </p> </th> 
   <th> <p><strong>실제 금액</strong> </p> </th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td> <p>프로젝트 확장 1</p> </td> 
   <td> <p>$1,000.00</p> </td> 
   <td> <p>$1,500.00</p> </td> 
  </tr> 
  <tr> 
   <td> <p>작업 1 확장 2</p> </td> 
   <td> <p>$2,500.00</p> </td> 
   <td> <p> $0.00 <strong></strong></p> </td> 
  </tr> 
 </tbody> 
</table>

1. 위의 값을 기준으로 발생됨/발생되지 않은 비용은 다음과 같이 결정됩니다.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th> <p><strong>작업</strong> </p> </th> 
   <th> <p><strong>발생되지 않은 계획 비용</strong> </p> </th> 
   <th> <p><strong>예상 비용 발생</strong> </p> </th> 
   <th> <p><strong>실제 비용 발생</strong> </p> </th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td> <p>작업 1</p> </td> 
   <td> <p>$400.00</p> </td> 
   <td> <p>-$500.00</p> </td> 
   <td> <p>$800.00</p> </td> 
  </tr> 
  <tr> 
   <td> <p>작업 2</p> </td> 
   <td> <p>-$400.00</p> </td> 
   <td> <p>$300.00</p> </td> 
   <td> <p>$1,300.00</p> </td> 
  </tr> 
  <tr> 
   <td> <p>작업 3</p> </td> 
   <td> <p>$0.00</p> </td> 
   <td> <p>$0.00</p> </td> 
   <td> <p>$1,000.00</p> </td> 
  </tr> 
  <tr> 
   <td> <p>작업 4</p> </td> 
   <td> <p>$600.00</p> </td> 
   <td> <p>-$100.00</p> </td> 
   <td> <p>$300.00</p> </td> 
  </tr> 
  <tr> 
   <td> <p>작업 5</p> </td> 
   <td> <p>$0.00</p> </td> 
   <td> <p>$600.00</p> </td> 
   <td> <p>$1,100.00</p> </td> 
  </tr> 
  <tr> 
   <td> <p>작업 6</p> </td> 
   <td> <p>$0.00</p> </td> 
   <td> <p>$600.00</p> </td> 
   <td> <p>$700.00</p> </td> 
  </tr> 
  <tr> 
   <td> <p>프로젝트</p> </td> 
   <td> <p>$2,500.00</p> </td> 
   <td> <p>$1000.00</p> </td> 
   <td> <p>$1,500.00</p> </td> 
  </tr> 
 </tbody> 
</table>

1. 프로젝트 작업에서 재무 재계산을 실행합니다
1. **CPI** 작업 2 = .17의 경우 다음과 같이 계산됩니다.\
   **CPI 작업 2** = *IF* 실제 노무비 + ExtualExpenseCost &lt;> 0 *THEN* CPI = (TotalBudgetCostWorkPerformed + ProredPlanningExpenseCost) / (ActualLaborCost + ProredActualExpenseCost)\
   *   ELSE* CPI = CPI_Labor\
   **CPI****작업 2** = (100+300) / (1000+1300)\
   **CPI****작업 2**  = 400 / 2300\
   **CPI****작업 2**  = .17

1. **EAC** 작업 2의 경우 = $5,900.00\
   **CPI Labor****작업 2** = IF 실제 노무비 &lt;> 0 CPI_Labor = TotalBudgetCostWorkPerformed / 실제 노무비\
      ELSE CPI_Labor = 1\
   **CPI Labor****작업 2** = 100/1000\
   **CPI Labor****작업 2** =.1

   **EAC Labor****작업 2** = *IF* CPI_Labor &lt;> 0 *THEN*

   ```
   EAC Labor = Planned Labor Cost/CPI_Labor
   ```

   *   ELSE* EAC 노무 = 계획된 노무비 + 실제 노무비\
   **EAC Labor****작업 2** = 500.00/.1\
   **EAC Labor****작업 2** = $5,000.00 ****** EAC 비용&#x200B;****작업 2 **= ProredActualExpenseCost + NotProredPlanningExpense\
   **EAC 비용&#x200B;****작업 2** = $1,300.00 + -$400.00\
   **EAC 비용****작업 2** = $900.00

   **EAC****작업 2** = EAC 노무 + EAC 비용\
   **EAC****작업 2**  = $5,000.00 + $900.00\
   **EAC****작업 2**  = $5,900.00

1. 작업 4, 5 및 6에 대한 CPI/EAC는 같은 방식으로 결정되므로 아래에 해당 값을 제공하겠습니다.\
   작업 4: 3,400.00 / 23\
   작업 5: 3,100.00 / US$64\
   작업 6: 1.06 / $2,366.67

1. 작업 3에 대한 CPI = .31은 다음과 같이 계산됩니다.\
   **CPI****작업 3** = *IF* 실제 노무비 + ExtualExpenseCost &lt;> 0 *THEN*

   ```
   CPI = (TotalBudgetedCostWorkPerformed + IncurredPlannedExpenseCost)/(ActualLaborCost + IncurredActualExpenseCost)
   ```

   *   ELSE* CPI = CPI_Labor\
   **CPI****작업 3**  = (1,150 + 500) / (3000 + 2400)\
   **CPI****작업 3**  = 1650 / 5400\
   **CPI****작업 3**  =.31 ******&#x200B;작업 3용 EAC **= 다음과 같이 계산된 $9,521.74:\
   **CPI 노동력&#x200B;****작업 3** = IF 실제 노무비 &lt;> 0

   ```
   CPI_Labor = TotalBudgetedCostWorkPerformed / Actual Labor Cost
   ```

      ELSE CPI_Labor = 1\
   **CPI Labor****작업 3** = 1150/3000\
   **CPI Labor****작업 3** = .383333\
   **CPI Labor****작업 3** =.38

   **EAC Labor****작업 3** = *IF* CPI_Labor &lt;> 0 *THEN*

   ```
   EAC Labor = Planned Labor Cost / CPI_Labor
   ```

   *   ELSE* EAC 노무 = 계획된 노무비 + 실제 노무비\
   **EAC Labor****작업 3** = $2,500.00 / .383333\
   **EAC Labor****작업 3** = $6,521.74

   **EAC 비용****작업 3** = ProredActualExpenseCost + NotProredPlanningExpense\
   **EAC 비용****작업 3** = $2,400.00 + $600.00\
   **EAC 비용****작업 3** = $3,000.00

   **EAC****작업 3** = EAC 노무 + EAC 비용\
   **EAC****작업 3**  = $6,521.74 + $3,000.00\
   **EAC****작업 3**  = $9,521.74

1. 작업 1에 대한 CPI = .16은 다음과 같이 계산됩니다.\
   **CPI****작업 1** = *IF* 실제 노무비 + ExtualExpenseCost &lt;> 0 *THEN*

   ```
   CPI = (TotalBudgetedCostWorkPerformed + IncurredPlannedExpenseCost) / (ActualLaborCost + IncurredActualExpenseCost)
   ```

   *   ELSE* CPI = CPI_Labor\
   **CPI****작업 1**  = (1250 + 300) / (5000 + 4500)\
   **CPI****작업 1**  = 1550 / 9500=\
   **CPI****작업 1**  =.16

1. 작업 1의 EAC는 다음과 같이 계산되는 $17,100.00입니다.\
   **CPI Labor****작업 1** = 실제 노무비 &lt;> 0인 경우

   ```
   CPI_Labor = TotalBudgetedCostWorkPerformed / Actual Labor Cost
   ```

      ELSE CPI_Labor = 1\
   **CPI Labor****작업 1** = 1250 / 5000\
   **CPI Labor****작업 1** =.25

   **EAC Labor****작업 1** = *IF* CPI_Labor &lt;> 0 *THEN* EAC 노무 = 계획된 노무 비용 / CPI_Labor\
   *   ELSE* EAC 노무 = 계획된 노무비 + 실제 노무비\
   **EAC Labor****작업 1** = $3,000.00 / .25\
   **EAC Labor****작업 1** = $12,000.00

   **EAC 비용****작업 1** = ProredActualExpenseCost + NotProredPlanningExpense\
   **EAC 비용****작업 1** = $4500 + 600\
   **EAC 비용****작업 1** = $5,100.00

   **EAC****작업 1** = EAC 노무 + EAC 비용\
   **EAC****작업 1**  = $12,000.00 + 5,100.00\
   **EAC****작업 1**  = $17,100.00

1. 프로젝트용 CPI는 .25입니다.\
   **프로젝트용 CPI****** = *IF* 실제 노무비 + ExtualExpenseCost &lt;> 0 *THEN*

   ```
   CPI = (TotalBudgetedCostWorkPerformed + IncurredPlannedExpenseCost)/(ActualLaborCost + IncurredActualExpenseCost)
   ```

   *   ELSE* CPI = CPI_Labor

   **프로젝트용 CPI****** = (2450 + 1900) / (11000 + 6700)\
   **프로젝트용 CPI****** = 4350 / 17700\
   **프로젝트용 CPI****** =.25

1. **프로젝트용 EAC** = 다음과 같이 계산되는 $32,248.98:\
   **CPI Labor****for Project** = 실제 노무비 &lt;> 0인 경우

   ```
   CPI_Labor = TotalBudgetedCostWorkPerformed / Actual Labor Cost
   ```

      ELSE CPI_Labor = 1\
   **CPI Labor****for Project** = 2450 / 11000\
   **CPI Labor****for Project** = .22272\
   **CPI Labor****for Project** = .22

   **프로젝트용 EAC Labor****** = *IF* CPI_Labor &lt;> 0 *THEN*

   ```
   EAC Labor = Planned Labor Cost / CPI_Labor
   ```

   *   ELSE* EAC 노무 = 계획된 노무비 + 실제 노무비\
   **프로젝트용 EAC Labor****** = $5,000.00 / .22272\
   **프로젝트용 EAC Labor****** = $22,448.97959\
   **프로젝트용 EAC Labor****** = $22,448.98

   **EAC 비용****프로젝트** = ProredActualExpenseCost + NotProredPlanningExpense\
   **EAC 비용****프로젝트** = $3,100.00 + $6,700.00\
   **EAC 비용****프로젝트** = $9,800.00

   **EAC****Project** = EAC 노무 + EAC 비용\
   **EAC****Project**  = $22,448.98 + 9,800.00\
   **EAC****Project**  = $32,248.98
