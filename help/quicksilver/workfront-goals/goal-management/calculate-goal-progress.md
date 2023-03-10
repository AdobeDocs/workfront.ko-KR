---
product-previous: workfront-goals
navigation-topic: goal-management
title: Adobe Workfront 목표의 목표 진행 및 조건 개요
description: 목표 진행은 활동, 결과 또는 하위 목표와 같은 진행 상태 지표에 의해 결정됩니다. 목표 조건은 현재 시점에서 목표의 진행 상태에 의해 결정됩니다.
author: Alina
feature: Workfront Goals
exl-id: 3050f7ff-a579-4fb8-82fd-bef850f27c20
source-git-commit: 1d221d10e5845e477dff825f853330b9b4df0adf
workflow-type: tm+mt
source-wordcount: '821'
ht-degree: 1%

---

# Adobe Workfront 목표의 목표 진행 및 조건 개요

<!--drafted for P&P release: the note at the top will need to be replaced with this:

Your organization must have the following to use the functionality described in this article:

* For the legacy plan and license structure: 

  * A Pro or higher [Adobe Workfront plan](https://www.workfront.com/plans). 
  * An Adobe Workfront Goals license in addition to a Workfront license.

* For the current plan and license structure:

  * An Ultimate plan 
    
    Or
    
    An additional license for Adobe Workfront Goals for the Prime or Select Adobe Workfront plans. <is there a link we can add here for the plans and what they contain?!>

Contact your Workfront account manager to learn about a Workfront Goals license.

For additional information about access to Workfront Goals, see [Requirements to use Workfront Goals](../../workfront-goals/goal-management/access-needed-for-wf-goals.md).
-->

>[!NOTE]
>
>이 문서에 설명된 기능을 사용하려면 조직에 다음 내용이 있어야 합니다.
>
>* Pro 이상 [Adobe Workfront 플랜](https://www.workfront.com/plans).
>* Workfront 라이선스 외에 Adobe Workfront 목표 라이선스.
>
>Workfront 목표 라이센스에 대한 자세한 내용은 Workfront 계정 관리자에게 문의하십시오.
>Workfront 목표 액세스에 대한 자세한 내용은 [Workfront 목표 사용 요구 사항](../../workfront-goals/goal-management/access-needed-for-wf-goals.md).

Adobe Workfront은 진행 상태 표시기의 진행 상황을 기반으로 자동으로 목표 진행 상태를 계산합니다.

## 전제 조건

시작하려면 먼저 다음을 수행해야 합니다.

* 기본 메뉴의 목표 영역을 포함하는 레이아웃 템플릿.

## 목표 진행률 및 임계값 개요

목표를 활성화한 후 Workfront 목표는 진행 상황과 조건 계산을 시작하고 진행 필드 위로 마우스를 가져가면 다음 표시기를 표시합니다.

| 표시기 | 지표 설명 |
|---|---|
| 실제 완료율 | 실제로 얼마나 많은 목표가 달성되었는가? Workfront 목표는 목표와 연결된 모든 진행 상태 표시기의 완료율을 평균하여 이 값을 계산합니다. |
| 예상 완료율 | 목표가 제 시간에 완성되기 위해서는 지금까지 얼마나 많은 목표를 달성해야 하는가. Workfront 목표는 목표의 지속 시간 및 현재 시간 순간을 보고 이 값을 계산합니다. 정시에 완료하려는 경우 목표가 현재 시간에 이 값을 표시해야 합니다. |
| 진행 | 목표가 제 시간에 완료되도록 타겟에 있는지, 또는 목표가 위험에 처해 있는지 또는 완료되지 않을 것인지 나타내는 레이블입니다. |

![](assets/in-trouble-goal-progress-expanded.png)

<!--drafted for the redesign: replace the screen shot above with the redesigned one which is white, not black-->

* [실제 완료율](#actual-percent-complete)
* [예상 완료율](#expected-percent-complete)
* [진행 및 조건](#progress)

### 실제 완료율 {#actual-percent-complete}

Workfront 목표는 목표 진행 상태 지표의 전체 평균 퍼센트를 기반으로 목표의 실제 완료율을 자동으로 계산합니다.

다음 항목은 목표에 대한 진행 상태 표시기로 간주됩니다.

* 결과

   목표에 결과 추가에 대한 자세한 내용은 [Adobe Workfront 목표에 결과 추가](../../workfront-goals/results-and-activities/add-results-to-goals.md).

* 활동

   목표에 프로젝트를 포함한 활동을 추가하는 방법에 대한 자세한 내용은 [Adobe Workfront 목표의 목표에 활동 추가](../../workfront-goals/results-and-activities/add-activities-to-goals.md).

* 연계된 하위 목표

   상위 및 하위 목표에 대한 자세한 내용은 [Adobe Workfront 목표에 연결하여 목표 정렬](../../workfront-goals/goal-alignment/align-goals-by-connecting-them.md).

   Workfront 목표는 다음 공식을 사용하여 실제 완료율을 계산합니다.

   ```
   Actual percent complete of goal = SUM(Percent complete of goal progress indicators)* 100 / Number of progress indicators
   ```

   예를 들어, 목표에 20% 완료된 결과, 30% 완료된 수동 진행률 표시줄, 10% 완료된 프로젝트 및 40% 완료된 하위 목표가 있는 경우 목표 완료율은 25%입니다.

### 예상 완료율 {#expected-percent-complete}

Workfront 목표는 목표 기간 동안 총 일 수와 목표 시작 날짜 이후 경과된 일 수를 기반으로 목표의 예상 완료 퍼센트를 자동으로 계산합니다.

Workfront 목표는 다음 공식을 사용하여 예상 완료 퍼센트를 계산합니다.

```
Expected percent complete of goal = Number of days since the goal start date * 100/ Number of days in the goal duration
```

예를 들어 목표가 90일 후에 완료되어야 하고 오늘이 해당 기간의 45일이면 예상 완료율이 50%입니다.

### 진행 및 조건 {#progress}

Workfront 목표는 진행 백분율을 계산하고 현재 시점에서 완료되는 예상 백분율에서 얻은 백분율에 따라 목표에 진행률 레이블을 지정합니다. 목표 퍼센트 완료 막대의 색상이 변경되어 목표의 진행 상황을 나타냅니다.

목표에 대한 조건도 업데이트되어 목표가 제 시간에 완료되는 목표인지, 뒤처지고 있는지를 나타냅니다.

Workfront 목표는 다음 공식을 사용하여 목표의 진행 비율을 계산합니다.

```
Goal progress percentage = Actual percent complete * 100 / Expected percent complete
```

예를 들어 예상 완료율이 현재 시간에 53%이고 실제 완료율이 30%인 경우 목표 진행 완료율은 56%입니다. Workfront 목표는 &quot;문제 발생&quot; 조건으로 이 목표에 레이블을 지정합니다.

다음 차트에서는 조건 레이블과 진행률 비율 간의 관계를 보여 줍니다.

![](assets/progress-status-labels-charted-after-match-with-project-condition-350x147.png)

아래 표에는 각 레이블과 연관된 목표 조건 레이블과 목표 진행 비율이 나와 있습니다.

>[!TIP]
>
>목표 조건 레이블은 Workfront 프로젝트 조건 이름 및 색상과 일치합니다.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td><b>목표 진행률 이름</b></td> 
   <td><b>목표 진행 정의</b></td> 
   <td><b>목표 진행 비율</b></td> 
   <td><b>전체 막대의 색상</b></td> 
   <td><b>조건 표시기 아이콘</b></td> 
  </tr> 
  <tr> 
   <td>신규</td> 
   <td> <p>목표가 새로 만들어지고 아직 진행 상태를 기록하지 않습니다. 목표 진행 상태는 처음 진행 상황을 업데이트할 때까지 새로 시작으로 표시됩니다. </p> <p>목표 진행 상태 업데이트에 대한 자세한 내용은 <a href="../../workfront-goals/goal-review-and-workfront-goals-sections/check-in-goals.md" class="MCXref xref">Adobe Workfront 목표에서 목표 진행 상태 업데이트</a>.</p> </td> 
   <td>백분율 없음</td> 
   <td>막대 없음</td> 
   <td><img src="assets/new-goal-icon-condition.png" alt="new_goal_icon_condition.png"></td>
  </tr> 
  <tr> 
   <td> <p><span>대상</span> </p> </td> 
   <td>목표가 예상대로 표시되고 있으며, 제 시간에 완료할 가능성이 높습니다. </td> 
   <td>90-100%</td> 
   <td>녹색</td> 
    <td><img src="assets/on-target-icon-condition.png" alt="on_target_icon_condition.png"></td>
  </tr> 
  <tr> 
   <td> <p><span>위험 상태</span> </p> </td> 
   <td>목표가 뒤떨어지고 있지만, 제 시간에 그것을 완성하는 것은 여전히 가능할 것이다. </td> 
   <td>70-89.99%</td> 
   <td>노란색</td>
   <td><img src="assets/at-risk-icon-condition.png" alt="at_risk_icon_condition.png"></td> 
  </tr> 
  <tr> 
   <td> <p><span>문제 발생</span> </p> </td> 
   <td> <p>목표가 제 시간에 끝나지 않을 것 같다. </p> </td> 
   <td>0-69.99%</td> 
   <td>빨간색</td> 
   <td><img src="assets/in-trouble-icon-condition.png" alt="in_troubleshoot_icon_condition.png"></td> 
  </tr> 
 </tbody> 
</table>