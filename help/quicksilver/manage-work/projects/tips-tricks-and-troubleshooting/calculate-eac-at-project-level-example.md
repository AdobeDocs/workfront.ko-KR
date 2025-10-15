---
content-type: tips-tricks-troubleshooting
product-area: projects
navigation-topic: tips-tricks-and-troubleshooting-projects
title: 계산 예 - 프로젝트 수준에서 EAC 계산
description: 이 문서에서는 Adobe Workfront의 프로젝트 수준에서 프로젝트의 EAC(완료 시 추정 비용)를 계산하는 예를 제공합니다.
author: Lisa
feature: Work Management
exl-id: ff88b7e3-2a5b-464f-bed1-6848067840b8
source-git-commit: 5bc7a1c00b72cfc07270cafee5bf753989b48d33
workflow-type: tm+mt
source-wordcount: '2214'
ht-degree: 1%

---

# 계산 예 - 프로젝트 수준에서 EAC 계산

## EAC 메서드: 프로젝트 수준에서 계산

* [PIM = 시간 기반](#pim-hour-based)
* [PIM= 비용 기반](#pim-cost-based)

### PIM = 시간 기반 {#pim-hour-based}

* [간단한 예: 프로젝트에 하위 작업이 없습니다](#simple-example-project-has-no-children-tasks)
* [복잡한 예: 프로젝트에 하위 작업이 있음](#complicated-example-project-has-children-tasks)

#### 간단한 예: 프로젝트에 하위 작업이 없음 {#simple-example-project-has-no-children-tasks}

PIM = 시간 기반

EAC 방법 = 프로젝트 수준에서 계산 ****

1. 비용/시간이 $100.00인 사용자 1에게 모두 할당된 세 개의 태스크(하위 태스크 없음)로 프로젝트 A를 생성합니다.
1. 아래 표에 따라 각 작업에 계획된 시간 및 실제 시간을 추가하고 완료율(%)을 지정합니다.

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

1. 프로젝트에 대한 재무를 다시 계산합니다.
1. 작업 1에 대한 **CPI** = .04 다음과 같이 계산됨:\
   작업 1에 대한 **CPI** = *IF* 실제 시간 > 0 *THEN* CPI = TotalBudgetedCostWorkPerformed/실제 시간\
      *ELSE* CPI = 1\
   작업 1에 대한 **CPI** = 1 / 25\
   작업 1에 대한 **CPI** = .04

1. 작업 1에 대한 **EAC** = 125시간 다음과 같이 계산됨:\
   **작업 1 EAC** = *IF* CPI &lt;> 0 *THEN* EAC = 계획된 시간/CPI\
       *ELSE* EAC = 계획된  시간 + 실제  시간\
   **작업 EAC** = 5 / .04\
   작업 1에 대한 **EAC** = 125시간****

1. 작업 2와 3에 대한 CPI/EAC는 다음과 같습니다.\
   작업  2 = .12 / 83.33  시간\
   작업 3 = 0.24 / 62.5시간

1. **프로젝트에 대한 CPI** = .13 다음과 같이 계산됨:\
   **프로젝트에 대한 CPI** = *IF* 실제 시간 > 0 *THEN* CPI = TotalBudgetedCostWorkPerformed/실제 시간\
       *ELSE* CPI = 1\
   **프로젝트에 대한 CPI** = 10 / 75\
   프로젝트에 대한 **CPI** = .13

1. **프로젝트에 대한 EAC** = 225시간 계산됨:\
   **프로젝트 EAC** = *IF* CPI &lt;> 0 *THEN* EAC = 계획된 시간/CPI\
       *ELSE* EAC = 계획된  시간 + 실제  시간\
   **프로젝트에 대한 EAC** = 30 / .13333\
   프로젝트에 대한 **EAC** = 225시간

#### 복잡한 예: 프로젝트에 하위 작업이 있음 {#complicated-example-project-has-children-tasks}

PIM = 시간 기반

EAC 방법 = 프로젝트 수준에서 계산

1. 아래와 같이 작업 3이 작업 4 및 5의 상위 항목이고 작업 1이 작업 2 및 3의 상위 항목인 6개의 작업으로 프로젝트 A를 만듭니다.\
   작업 1\
      작업 2\
      작업 3\
         작업 4\
         작업 5\
   작업 6

1. 비용/시간 비율이 $100.00인 사용자 1에게 태스크 2, 4, 5 및 6을 지정합니다.
1. 아래 표에 따라 각 작업의 계획/실제 시간 및 완료율(%)을 추가하십시오.

   >[!NOTE]
   >
   >작업 1과 3의 경우 실제 시간만 추가합니다.

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

1. 프로젝트에 50시간을 직접 추가합니다(더 보기>시간>로그 시간).
1. 작업 2에 대한 **CPI** = .1은 다음과 같이 계산됩니다.\
   **작업 2에 대한 CPI** = *IF* 실제 시간 > 0 *THEN* CPI = TotalBudgetedCostWorkPersed/실제 시간\
       *ELSE* CPI = 1\
   작업 2에 대한 **CPI** = 1 / 10\
   작업 2에 대한 **CPI** = .1

1. 작업 2에 대한 **EAC** = 50시간 계산됨:\
   **작업 2 EAC** = *IF* CPI &lt;> 0 *THEN* EAC = 계획된 시간/CPI\
       *ELSE* EAC = 계획된  시간 + 실제  시간\
   작업 2 **= 5 / .1에 대한** EAC\
   작업 2에 대한 **EAC** = 50시간

1. 작업 4, 5 및 6에 대한 CPI/EAC는 다음과 같습니다.\
   작업 4: .4 / 25시간\
   작업 5: .75 / 20시간\
   작업 6: 1.2 / 16.67시간

1. 작업 3에 대한 **CPI** = .38  다음과 같이 계산됩니다.\
   작업 3에 대한 **CPI** = *IF* 실제 시간 > 0 *THEN* CPI = TotalBudgetedCostWorkPersed/실제 시간\
       *ELSE* CPI = 1\
   작업 3에 대한 **CPI** = 11.5 / 30\
   작업 3에 대한 **CPI** = .38

1. 작업 3에 대한 **EAC** = 65.22시간은 다음과 같이 계산됩니다.\
   작업 3에 대한 **EAC** = *IF* CPI &lt;> 0 *THEN* EAC = 계획된 시간/CPI\
       *ELSE* EAC = 계획된  시간 + 실제  시간\
   작업 3에 대한 **EAC** =  25 / .383333\
   작업 3에 대한 **EAC** = 65.22시간

1. 작업 1에 대한 **CPI** = .25 다음과 같이 계산됨:\
   작업 1에 대한 **CPI** = *IF* 실제 시간 > 0 *THEN* CPI = TotalBudgetedCostWorkPerformed/실제 시간\
       *ELSE* CPI = 1\
   작업 1에 대한 **CPI** = 12.5 / 50\
   작업 1에 대한 **CPI** = .25

1. 작업 1에 대한 **EAC** = 120시간 계산됨:\
   **작업 1 EAC** = *IF* CPI &lt;> 0 *THEN* EAC = 계획된 시간 / CPI\
       *ELSE* EAC = 계획된  시간 + 실제  시간\
   **작업 1** =  30/.25\
   작업 1에 대한 **EAC** = 120시간

1. **프로젝트에 대한 CPI** = .22 다음과 같이 계산됨:\
   **프로젝트에 대한 CPI** = *IF* 실제 시간 > 0 *THEN* CPI = TotalBudgetedCostWorkPerformed/실제 시간\
       *ELSE* CPI = 1\
   **프로젝트에 대한 CPI** = 24.5 / 110\
   프로젝트에 대한 **CPI** = .22272\
   프로젝트에 대한 **CPI** = .22

1. **프로젝트에 대한 EAC** = 224.49  다음과 같이 계산된 시간:\
   **프로젝트 EAC** = *IF* CPI &lt;> 0 *THEN* EAC = 계획된 시간/CPI\
       *ELSE* EAC = 계획된  시간 + 실제  시간\
   **프로젝트에 대한 EAC** =  50 / .22272\
   프로젝트의 **EAC** = 224.49시간

### PIM= 비용 기반 {#pim-cost-based}

* [간단한 예: 프로젝트에 하위 작업이 없습니다](#simple-example-project-has-no-children-tasks)
* [복잡한 예: 프로젝트에 하위 작업이 있음](#complicated-example-project-has-children-tasks)

#### 간단한 예: 프로젝트에 하위 작업이 없음 {#simple-example-project-has-no-children-tasks-1}

PIM = 비용 기반

EAC 방법 = 프로젝트 수준에서 계산

1. 비용/시간이 $100.00인 사용자 1에게 모두 할당된 세 개의 태스크(하위 태스크 없음)로 프로젝트 A를 생성합니다.
1. 아래 표에 따라 각 작업에 계획된/실제 시간 및 완료율(%)을 추가합니다.

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
   <th> <br> <p><strong>계획된 인건비</strong> </p> </th> 
   <th> <br> <p><strong>실제 근로시간</strong> </p> </th> 
   <th> <br> <p><strong>실제 인건비</strong> </p> </th> 
   <th> <p><strong>% 완료</strong> </p> </th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td> <p>작업 1</p> </td> 
   <td> <p>5시간</p> </td> 
   <td> <p>500달러</p> </td> 
   <td> <p>25시간</p> </td> 
   <td> <p>US$2,500.00</p> </td> 
   <td> <p>20%</p> </td> 
  </tr> 
  <tr> 
   <td> <p>작업 2</p> </td> 
   <td> <p>10시간</p> </td> 
   <td> <p>US$1,000.00</p> </td> 
   <td> <p>25시간</p> </td> 
   <td> <p>US$2,500.00</p> </td> 
   <td> <p>30%</p> </td> 
  </tr> 
  <tr> 
   <td> <p>작업 3</p> </td> 
   <td> <p>15시간</p> </td> 
   <td> <p>US$1,500.00</p> </td> 
   <td> <p>25시간</p> </td> 
   <td> <p>US$2,500.00</p> </td> 
   <td> <p>40%</p> </td> 
  </tr> 
 </tbody> 
</table>

1. 아래 표에 따라 각 작업에 경비를 추가하십시오.

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
   <td> <p>작업 1 만료 1</p> </td> 
   <td> <p>300달러</p> </td> 
   <td> <p>400달러</p> </td> 
  </tr> 
  <tr> 
   <td> <p>작업 1</p> </td> 
   <td> <p>작업 1 만료 2</p> </td> 
   <td> <p>500달러</p> </td> 
   <td> <p>US$0.00</p> </td> 
  </tr> 
  <tr> 
   <td> <p>작업 2</p> </td> 
   <td> <p>작업 2 경비</p> </td> 
   <td> <p>200달러</p> </td> 
   <td> <p>100달러</p> </td> 
  </tr> 
  <tr> 
   <td> <p>작업 3</p> </td> 
   <td> <p>작업 3 경비</p> </td> 
   <td> <p>US$800.00</p> </td> 
   <td> <p>700달러</p> </td> 
  </tr> 
 </tbody> 
</table>

1. 다음과 같이 프로젝트에 경비 두 개(즉, 작업에 연결되지 않음)를 추가합니다.

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
   <td> <p>프로젝트 만료 1</p> </td> 
   <td> <p>US$1,000.00</p> </td> 
   <td> <p>US$1,500.00</p> </td> 
  </tr> 
  <tr> 
   <td> <p>작업 1 만료 2</p> </td> 
   <td> <p>US$2,500.00</p> </td> 
   <td> <p>US$0.00</p> </td> 
  </tr> 
 </tbody> 
</table>

1. 위의 값을 기준으로 발생/미발생 원가는 다음과 같이 결정됩니다.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th> <p><strong>작업</strong> </p> </th> 
   <th> <p><strong>계획된 경비가 발생하지 않음</strong> </p> </th> 
   <th> <p><strong>계획된 경비 발생</strong> </p> </th> 
   <th> <p><strong>실제 경비 발생</strong> </p> </th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td> <p>작업 1</p> </td> 
   <td> <p>500달러</p> </td> 
   <td> <p>300달러</p> </td> 
   <td> <p>400달러</p> </td> 
  </tr> 
  <tr> 
   <td> <p>작업 2</p> </td> 
   <td> <p>US$0.00</p> </td> 
   <td> <p>200달러</p> </td> 
   <td> <p>100달러</p> </td> 
  </tr> 
  <tr> 
   <td> <p>작업 3</p> </td> 
   <td> <p>US$0.00</p> </td> 
   <td> <p>US$800.00</p> </td> 
   <td> <p>700달러</p> </td> 
  </tr> 
  <tr> 
   <td> <p>프로젝트</p> </td> 
   <td> <p>US$3,000.00</p> </td> 
   <td> <p>US$2,300.00</p> </td> 
   <td> <p> US$2,700.00 <strong></strong></p> </td> 
  </tr> 
 </tbody> 
</table>

1. 프로젝트 작업에서 재무 재계산을 실행합니다.
1. 작업 1에 대한 **CPI** = .14
1. 작업 1에 대한 **CPI****1} = .14 다음과 같이 계산됨:**\
   **CPI**  **작업 1** = *IF* 실제 인건비 + UsedActualExpenseCost  &lt;> 0 *THEN*

   ```
   CPI = (TotalBudgetedCostWorkPerformed + IncurredPlannedExpenseCost) / (ActualLaborCost + IncurredActualExpenseCost)
   ```

   *    ELSE* CPI = CPI_Labor\
   **CPI****작업 1}에 대한** = (100+300) / (2500+400)\
   **CPI**  **작업 1** = 400 / 2900\
   **CPI**  **작업 1**&#x200B;용  = .14****

1. **작업 1****1에 대한 EAC** = $13,400.00\
   **CPI Labor**  **작업 1** = 실제 인건비 &lt;> 0인 경우

   ```
   CPI_Labor = TotalBudgetedCostWorkPerformed/Actual Labor Cost
   ```

      ELSE CPI_Labor = 1\
   **CPI Labor**  **작업 1** = 100/2500\
   **CPI Labor**  **작업 1의 경우** = .04 ****** EAC 인건비&#x200B;****작업 1의 경우&#x200B;**=*IF *CPI_Labor &lt;> 0*THEN *EAC 인건비 = 계획된 인건비/CPI_Labor\
   *    ELSE* EAC  노무 = 계획 노무비 + 실제 노무비\
   **EAC Labor ****작업 1** = 500.00/.04\
   **작업 ****에 대한 EAC 인건비** = $12,500.00\
   **EAC 경비****작업 1} = UsedActualExpenseCost + NotUsedPlannedExpense**\
   **작업 ****에 대한 EAC 경비** = $400.00 + $500.00\
   **작업 ****에 대한 EAC 경비** = $900.00\
   **EAC****for Task 1** = EAC 인건비 + EAC 경비\
   **작업 ****에 대한 EAC**  = $12,500.00 + $900.00\
   **작업 ****에 대한 EAC**  = $13,400.00

1. 다음은 작업 2 및 작업 3에 대한 CPI/EAC 값입니다.\
   작업 2 = .19 / $8,433.33\
   작업 3 = .44 / $6,950.00

1. **프로젝트에 대한 CPI** = .32 다음과 같이 계산됨:\
   **프로젝트의 CPI****1} =** IF *실제 인건비 + UsedActualExpenseCost  &lt;> 0* THEN **

   ```
   CPI = (TotalBudgetedCostWorkPerformed + IncurredPlannedExpenseCost)/ActualLaborCost + IncurredActualExpenseCost)
   ```

   *   ELSE* CPI = CPI_Labor\
   **프로젝트용 CPI****1} = (1000 + 2300) / (7500 + 2700)**\
   **프로젝트용 CPI****1} = 3300 / 10200**\
   **프로젝트용 CPI****1} = .32**

1. **프로젝트에 대한 EAC** = $28,200.00은 다음과 같이 계산됩니다.\
   **프로젝트에 대한 CPI 인건비****1} = 실제 인건비 &lt;> 0인 경우**

   ```
   CPI_Labor = TotalBudgetedCostWorkPerformed/Actual Labor Cost
   ```

      ELSE CPI_Labor = 1\
   **프로젝트용 CPI 인건비****1} = 1000 / 7500**\
   **프로젝트용 CPI ****** = .13333\
   **프로젝트에 대한 CPI ****** = .13

   **EAC Labor****for Project** = *IF* CPI_Labor &lt;> 0 *THEN*

   ```
   EAC Labor = Planned Labor Cost/CPI_Labor
   ```

   *   ELSE* EAC  노무 = 계획 노무비 + 실제 노무비\
   **프로젝트에 대한 EAC ****** = 3000/ .13333\
   **프로젝트용 EAC 인건비****1} = $22,500.00**

   **EAC 경비****프로젝트** =

   ```
   IncurredActualExpenseCost + NotIncurredPlannedExpense
   ```

   **EAC 경비****프로젝트** = $3,000.00 + 2,700.00\
   **EAC 경비****프로젝트** = $5,700.00

   **EAC****Project** = EAC 인건비 + EAC 경비\
   **EAC****프로젝트**  = $22,500.00 + $5,700.00\
   **EAC****프로젝트**  = $28,200.00

#### 복잡한 예: 프로젝트에 하위 작업이 있음 {#complicated-example-project-has-children-tasks-1}

PIM = 비용 기반

EAC 방법 = 프로젝트 수준에서 계산

1. 아래와 같이 작업 3이 작업 4 및 5의 상위 항목이고 작업 1이 작업 2 및 3의 상위 항목인 6개의 작업으로 프로젝트 A를 만듭니다.\
   작업 1\
      작업 2\
      작업 3\
         작업 4\
         작업 5\
   작업 6

1. 비용/시간 비율이 $100.00인 사용자 1에게 태스크 2, 4, 5 및 6을 지정합니다.
1. 아래 표에 따라 각 작업의 계획/실제 시간 및 완료율(%)을 추가하십시오.

   >[!NOTE]
   >
   >작업 1과 3의 경우 실제 시간만 추가합니다.

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
   <th> <br> <p><strong>계획된 인건비</strong> </p> </th> 
   <th> <br> <p><strong>실제 근로시간</strong> </p> </th> 
   <th> <br> <p><strong>실제 인건비</strong> </p> </th> 
   <th> <p><strong>% 완료</strong> </p> </th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td> <p>작업 1</p> </td> 
   <td> </td> 
   <td> </td> 
   <td> <p>10시간</p> </td> 
   <td> <p>US$1,000.00</p> </td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td> <p>작업 2</p> </td> 
   <td> <p>5시간</p> </td> 
   <td> <p>500달러</p> </td> 
   <td> <p>10시간</p> </td> 
   <td> <p>US$1,000.00</p> </td> 
   <td> <p>20%</p> </td> 
  </tr> 
  <tr> 
   <td> <p>작업 3</p> </td> 
   <td> </td> 
   <td> </td> 
   <td> <p>10시간</p> </td> 
   <td> <p>US$1,000.00</p> </td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td> <p>작업 4</p> </td> 
   <td> <p>10시간</p> </td> 
   <td> <p>US$1,000.00</p> </td> 
   <td> <p>10시간</p> </td> 
   <td> <p>US$1,000.00</p> </td> 
   <td> <p>40%</p> </td> 
  </tr> 
  <tr> 
   <td> <p>작업 5</p> </td> 
   <td> <p>15시간</p> </td> 
   <td> <p>US$1,500.00</p> </td> 
   <td> <p>10시간</p> </td> 
   <td> <p>US$1,000.00</p> </td> 
   <td> <p>50%</p> </td> 
  </tr> 
  <tr> 
   <td> <p>작업 6</p> </td> 
   <td> <p>20시간</p> </td> 
   <td> <p>US$2,000.00</p> </td> 
   <td> <p>10시간</p> </td> 
   <td> <p>US$1,000.00</p> </td> 
   <td> <p>60%</p> </td> 
  </tr> 
 </tbody> 
</table>

1. 프로젝트에 직접 50시간을 추가(추가>시간>로그 시간)하여 프로젝트에 직접 기록된 실제 인건비 5,000.00달러가 되도록 합니다. ****
1. 아래 표에 따라 각 작업에 비용을 추가합니다(읽기 쉽도록 각 작업 사이에 빈 행을 추가했습니다).

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
   <td> <p>작업 1 만료 1</p> </td> 
   <td> <p>300달러</p> </td> 
   <td> <p>-$400.00</p> </td> 
  </tr> 
  <tr> 
   <td> <p>작업 1</p> </td> 
   <td> <p>작업 1 만료 2</p> </td> 
   <td> <p>-$500.00</p> </td> 
   <td> <p>US$800.00</p> </td> 
  </tr> 
  <tr> 
   <td> <p>작업 1</p> </td> 
   <td> <p>작업 1 만료 3</p> </td> 
   <td> <p>400달러</p> </td> 
   <td> <p>US$0.00</p> </td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td> </td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td> <p>작업 2</p> </td> 
   <td> <p>작업 2 만료 1</p> </td> 
   <td> <p>500달러</p> </td> 
   <td> <p>700달러</p> </td> 
  </tr> 
  <tr> 
   <td> <p>작업 2</p> </td> 
   <td> <p>작업 2 경비 2</p> </td> 
   <td> <p>-$400.00</p> </td> 
   <td> <p>US$0.00</p> </td> 
  </tr> 
  <tr> 
   <td> <p>작업 2</p> </td> 
   <td> <p>작업 2 만료 3</p> </td> 
   <td> <p>-$200.00</p> </td> 
   <td> <p>600달러</p> </td> 
  </tr> 
  <tr> 
   <td> <p>작업 2</p> </td> 
   <td> <p>작업 2 경비 4</p> </td> 
   <td> <p>700달러</p> </td> 
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
   <td> <p>작업 3 경비</p> </td> 
   <td> <p>US$0.00</p> </td> 
   <td> <p>US$1,000.00</p> </td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td> </td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td> <p>작업 4</p> </td> 
   <td> <p>작업 4 만료 1</p> </td> 
   <td> <p>US$800.00</p> </td> 
   <td> <p>US$0.00</p> </td> 
  </tr> 
  <tr> 
   <td> <p>작업 4</p> </td> 
   <td> <p>작업 4 만료 2</p> </td> 
   <td> <p>-$100.00</p> </td> 
   <td> <p>300달러</p> </td> 
  </tr> 
  <tr> 
   <td> <p>작업 4 </p> </td> 
   <td> <p>작업 4 만료 3</p> </td> 
   <td> <p>-200.00</p> </td> 
   <td> <p>US$0.00</p> </td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td> </td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td> <p>작업 5</p> </td> 
   <td> <p>작업 5 만료 1</p> </td> 
   <td> <p>700달러</p> </td> 
   <td> <p>US$800.00</p> </td> 
  </tr> 
  <tr> 
   <td> <p>작업 5</p> </td> 
   <td> <p>작업 5 만료 2</p> </td> 
   <td> <p>-$100.00</p> </td> 
   <td> <p>300달러</p> </td> 
  </tr> 
  <tr> 
   <td> <p>작업 5</p> </td> 
   <td> <p>작업 5 만료 3</p> </td> 
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
   <td> <p>작업 6 만료 1</p> </td> 
   <td> <p>600달러</p> </td> 
   <td> <p>700달러</p> </td> 
  </tr> 
  <tr> 
   <td> <p>작업 6</p> </td> 
   <td> <p>작업 6 만료 2</p> </td> 
   <td> <p>500달러</p> </td> 
   <td> <p>-$300.0</p> </td> 
  </tr> 
 </tbody> 
</table>

1. 다음과 같이 프로젝트에 경비 두 개(즉, 작업에 연결되지 않음)를 추가합니다.

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
   <td> <p>프로젝트 만료 1</p> </td> 
   <td> <p>US$1,000.00</p> </td> 
   <td> <p>US$1,500.00</p> </td> 
  </tr> 
  <tr> 
   <td> <p>작업 1 만료 2</p> </td> 
   <td> <p>US$2,500.00</p> </td> 
   <td> <p> US$0.00 <strong></strong></p> </td> 
  </tr> 
 </tbody> 
</table>

1. 위의 값을 기준으로 발생/미발생 원가는 다음과 같이 결정됩니다.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th> <p><strong>작업</strong> </p> </th> 
   <th> <p><strong>계획된 경비가 발생하지 않음</strong> </p> </th> 
   <th> <p><strong>계획된 경비 발생</strong> </p> </th> 
   <th> <p><strong>실제 경비 발생</strong> </p> </th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td> <p>작업 1</p> </td> 
   <td> <p>400달러</p> </td> 
   <td> <p>-$500.00</p> </td> 
   <td> <p>US$800.00</p> </td> 
  </tr> 
  <tr> 
   <td> <p>작업 2</p> </td> 
   <td> <p>-$400.00</p> </td> 
   <td> <p>300달러</p> </td> 
   <td> <p>US$1,300.00</p> </td> 
  </tr> 
  <tr> 
   <td> <p>작업 3</p> </td> 
   <td> <p>US$0.00</p> </td> 
   <td> <p>US$0.00</p> </td> 
   <td> <p>US$1,000.00</p> </td> 
  </tr> 
  <tr> 
   <td> <p>작업 4</p> </td> 
   <td> <p>600달러</p> </td> 
   <td> <p>-$100.00</p> </td> 
   <td> <p>300달러</p> </td> 
  </tr> 
  <tr> 
   <td> <p>작업 5</p> </td> 
   <td> <p>US$0.00</p> </td> 
   <td> <p>600달러</p> </td> 
   <td> <p>US$1,100.00</p> </td> 
  </tr> 
  <tr> 
   <td> <p>작업 6</p> </td> 
   <td> <p>US$0.00</p> </td> 
   <td> <p>600달러</p> </td> 
   <td> <p>700달러</p> </td> 
  </tr> 
  <tr> 
   <td> <p>프로젝트</p> </td> 
   <td> <p>US$2,500.00</p> </td> 
   <td> <p>1000달러</p> </td> 
   <td> <p>US$1,500.00</p> </td> 
  </tr> 
 </tbody> 
</table>

1. 프로젝트 작업에서 재무 재계산을 실행합니다.
1. 작업 2 = .17에 대한 **CPI**&#x200B;은(는) 다음과 같이 계산됩니다.\
   **CPI 작업 2** = *IF* 실제 인건비 + UsedActualExpenseCost  &lt;> 0 *THEN* CPI = (TotalBudgetedCostWorkPerformed + UsedPlannedExpenseCost) / (ActualLaborCost + UsedActualExpenseCost)\
   *   ELSE* CPI = CPI_Labor\
   **CPI****작업 2** = (100+300) / (1000+1300)\
   **CPI****작업 2**  = 400 / 2300\
   **CPI****작업 2**  = .17

1. 작업 2에 대한 **EAC** = $5,900.00\
   **CPI 인건비****태스크 2** = 실제 인건비 &lt;> 0인 경우 CPI_Labor = TotalBudgetedCostWorkPerformed / 실제 인건비\
      ELSE CPI_Labor = 1\
   **CPI Labor****Task 2** = 100/1000\
   **CPI Labor****Task 2** = .1

   **EAC Labor****Task 2** = *IF* CPI_Labor &lt;> 0 *THEN*

   ```
   EAC Labor = Planned Labor Cost/CPI_Labor
   ```

   *   ELSE* EAC  노무 = 계획 노무비 + 실제 노무비\
   **EAC Labor****Task 2** = 500.00/.1\
   **EAC Labor****Task 2** = $5,000.00 ****** EAC 경비&#x200B;****Task 2 **= UsedActualExpenseCost + NotUsedPlannedExpense\
   **EAC 경비&#x200B;****작업 2** = $1,300.00 + -$400.00\
   **EAC 경비****작업 2** = $900.00

   **EAC****Task 2** = EAC 인건비 + EAC 경비\
   **EAC****작업 2**  = $5,000.00 + $900.00\
   **EAC****작업 2**  = $5,900.00

1. 작업 4, 5 및 6에 대한 CPI/EAC는 동일한 방식으로 결정되므로 아래에 해당 값을 제공하겠습니다.\
   작업 4: .23 / $3,400.00\
   작업 5: .64 / $3,100.00\
   작업 6: 1.06 / $2,366.67

1. 작업 3의 CPI = .31 다음과 같이 계산됩니다.\
   **CPI****작업 3** = *IF* 실제 인건비 + UsedActualExpenseCost  &lt;> 0 *THEN*

   ```
   CPI = (TotalBudgetedCostWorkPerformed + IncurredPlannedExpenseCost)/(ActualLaborCost + IncurredActualExpenseCost)
   ```

   *   ELSE* CPI = CPI_Labor\
   **CPI****작업 3**  = (1,150 + 500) / (3000 + 2400)\
   **CPI****작업 3**  =  1650 / 5400\
   **CPI****작업 3**  = 작업 3 ****** = $9,521.74에 대한 .31 **EAC는 다음과 같이 계산됩니다.\
   **CPI 인건비&#x200B;****태스크 3** = 실제 인건비가 &lt;> 0인 경우

   ```
   CPI_Labor = TotalBudgetedCostWorkPerformed / Actual Labor Cost
   ```

      ELSE CPI_Labor = 1\
   **CPI Labor****Task 3** = 1150/3000\
   **CPI Labor****Task 3** = .383333\
   **CPI Labor****Task 3** = .38

   **EAC Labor****Task 3** = *IF* CPI_Labor &lt;> 0 *THEN*

   ```
   EAC Labor = Planned Labor Cost / CPI_Labor
   ```

   *   ELSE* EAC  노무 = 계획 노무비 + 실제 노무비\
   **EAC Labor****Task 3** = $2,500.00 / .383333\
   **EAC Labor****Task 3** = $6,521.74

   **EAC 경비****작업 3** = UsedActualExpenseCost + NotUsedPlannedExpense\
   **EAC 경비****작업 3** = $2,400.00 + $600.00\
   **EAC 경비****작업 3** = $3,000.00

   **EAC****작업 3** = EAC 인건비 + EAC 경비\
   **EAC****작업 3**  = $6,521.74 + $3,000.00\
   **EAC****작업 3**  = $9,521.74

1. 작업 1의 CPI = .16 다음과 같이 계산됩니다.\
   **CPI****작업 1** = *IF* 실제 인건비 + UsedActualExpenseCost  &lt;> 0 *THEN*

   ```
   CPI = (TotalBudgetedCostWorkPerformed + IncurredPlannedExpenseCost) / (ActualLaborCost + IncurredActualExpenseCost)
   ```

   *   ELSE* CPI = CPI_Labor\
   **CPI****작업 1**  = (1250 + 300) / (5000 + 4500)\
   **CPI****작업 1**  =  1550 / 9500=\
   **CPI****작업 1**  = .16

1. 작업 1의 EAC는 다음과 같이 계산된 $17,100.00입니다.\
   **CPI 인건비****작업 1** = 실제 인건비가 &lt;> 0인 경우

   ```
   CPI_Labor = TotalBudgetedCostWorkPerformed / Actual Labor Cost
   ```

      ELSE CPI_Labor = 1\
   **CPI Labor****Task 1** = 1250 / 5000\
   **CPI Labor****Task 1** = .25

   **EAC Labor****Task 1** = *IF* CPI_Labor &lt;> 0 *THEN* EAC Labor = 계획된 인건비 / CPI_Labor\
   *   ELSE* EAC  노무 = 계획 노무비 + 실제 노무비\
   **EAC Labor****Task 1** = $3,000.00 / .25\
   **EAC Labor****Task 1** = $12,000.00

   **EAC 경비****작업 1** = UsedActualExpenseCost + NotUsedPlannedExpense\
   **EAC 경비****작업 1** = $4500 + 600\
   **EAC 경비****작업 1** = $5,100.00

   **EAC****작업 1** = EAC 인건비 + EAC 경비\
   **EAC****작업 1**  = $12,000.00 + 5,100.00\
   **EAC****작업 1**  = $17,100.00

1. 프로젝트에 대한 CPI는 .25입니다.\
   **프로젝트의 CPI****1} =** IF *실제 인건비 + UsedActualExpenseCost  &lt;> 0* THEN **

   ```
   CPI = (TotalBudgetedCostWorkPerformed + IncurredPlannedExpenseCost)/(ActualLaborCost + IncurredActualExpenseCost)
   ```

   *   ELSE* CPI = CPI_Labor

   **프로젝트용 CPI****1} = (2450 + 1900) / (11000 + 6700)**\
   **프로젝트용 CPI****1} =   4350 / 17700**\
   **프로젝트용 CPI****1} = .25**

1. **프로젝트에 대한 EAC** = $32,248.98 다음과 같이 계산됨:\
   **프로젝트에 대한 CPI 인건비****1} = 실제 인건비 &lt;> 0인 경우**

   ```
   CPI_Labor = TotalBudgetedCostWorkPerformed / Actual Labor Cost
   ```

      ELSE CPI_Labor = 1\
   **프로젝트용 CPI 인건비****1} = 2450 / 11000**\
   **프로젝트용 CPI ****** = .22272\
   **프로젝트용 CPI ****** = .22

   **EAC Labor****for Project** = *IF* CPI_Labor &lt;> 0 *THEN*

   ```
   EAC Labor = Planned Labor Cost / CPI_Labor
   ```

   *   ELSE* EAC  노무 = 계획 노무비 + 실제 노무비\
   **프로젝트용 EAC 인건비****1} = $5,000.00 / .22272**\
   **프로젝트에 대한 EAC 인건비****1} = $22,448.97959**\
   **프로젝트용 EAC 인건비****1} = $22,448.98**

   **EAC 경비****프로젝트** = UsedActualExpenseCost + NotUsedPlannedExpense\
   **EAC 경비****프로젝트** = $3,100.00 + $6,700.00\
   **EAC 경비****프로젝트** = $9,800.00

   **EAC****Project** = EAC 인건비 + EAC 경비\
   **EAC****프로젝트**  = $22,448.98 + 9,800.00\
   **EAC****프로젝트**  = US$32,248.98
