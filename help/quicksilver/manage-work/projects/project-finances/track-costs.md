---
content-type: reference;how-to-procedural
product-area: projects
navigation-topic: financials
title: 비용 추적
description: Adobe Workfront에서 프로젝트, 작업 및 문제에 대한 비용을 추적할 수 있습니다.
author: Alina
feature: Work Management
exl-id: df3090ae-9721-4e9b-84b4-315890619801
source-git-commit: d8c274d2153836647367c263cad8d786402cbe7f
workflow-type: tm+mt
source-wordcount: '2372'
ht-degree: 1%

---

# 비용 추적

Adobe Workfront에서 프로젝트, 작업 및 문제에 대한 비용을 추적할 수 있습니다.

## Workfront이 비용을 계산하는 방법

비용을 추적하려면 사용자 및 작업 역할을 시간별 비용 요금과 연결해야 합니다.

시간별 비용 비율은 작업 역할이나 사용자와 연관된 작업 단위당 비용 금액입니다. 작업에 사용한 시간을 곱하면 프로젝트, 작업 또는 문제에 대한 비용이 생성됩니다.

다음 시나리오가 있습니다.

* 작업의 원가 유형이 시간별 사용자인 경우 사용자 시간별 비율은 작업 및 프로젝트 원가를 계산합니다.

   사용자와 원가율 연결에 대한 자세한 내용은 [사용자 프로필 편집](../../../administration-and-setup/add-users/create-and-manage-users/edit-a-users-profile.md).

* 작업의 비용 유형이 시간별 역할이면 작업 역할 시간별 비율은 작업 및 프로젝트 비용을 계산합니다.

   작업 역할과 원가율 연결에 대한 자세한 내용은 [작업 역할 만들기 및 관리](../../../administration-and-setup/set-up-workfront/organizational-setup/create-manage-job-roles.md).

* Workfront은 문제에 대한 실제 비용만 계산하며 비용 유형이 없는 문제에 대해 계산됩니다. 자세한 내용은 섹션을 참조하십시오 [Workfront이 문제에 대한 비용을 추적하는 방법](#how-workfront-tracks-costs-for-issues) 참조하십시오.

>[!TIP]
>
>프로젝트에 대한 원가율은 대체할 수 없습니다. 사용자 또는 작업 역할에 대한 시간당 비용을 설정하면 그 비율은 시스템의 모든 비용을 계산합니다.

## Workfront 비용 성능 인덱스

Workfront은 프로젝트에 대한 많은 비용 성능 인덱스를 계산하여 비용 효율성을 위해 프로젝트를 추적할 수 있습니다.\
원가 성능 인덱스 계산에 대한 자세한 내용은 다음을 참조하십시오.

* [원가 성과 지수 계산(CPI)](../../../manage-work/projects/project-finances/calculate-cpi.md)
* [원가 스케줄 성과 인덱스 계산(CSI)](../../../manage-work/projects/project-finances/calculate-csi.md)
* [SPI(일정 성과 인덱스) 계산](../../../manage-work/projects/project-finances/calculate-spi.md)

## Workfront이 작업 및 프로젝트에 대한 비용을 추적하는 방법

* [Workfront이 비용을 추적하는 방법](#how-workfront-tracks-costs)
* [Workfront이 계획, 예산책정 및 실제 원가를 계산하는 방법](#how-workfront-calculates-planned-budgeted-and-actual-costs)
* [Workfront이 작업의 비용 유형을 계산하는 방법](#how-workfront-calculates-cost-types-for-tasks)

### Workfront이 비용을 추적하는 방법  {#how-workfront-tracks-costs}

Workfront에서 작업 및 프로젝트에 대한 몇 가지 유형의 비용을 추적할 수 있습니다. 전체 원가는 다음 공식으로 계산됩니다.

```
Costs = Labor Costs + Expense Costs
```

* **인건비** 작업 및 프로젝트 시간 및 작업과 관련된 리소스의 시간당 비용 비율과 연결됩니다. 일반적으로 Workfront은 다음과 같은 인건비 비용을 계산합니다.

   <table style="table-layout:auto"> 
   <col> 
   <col> 
   <tbody> 
    <tr> 
     <td>계획된 인건비</td> 
     <td> <p>다음 공식을 사용하여 계산됩니다.</p><pre>계획 노무비 = 계획 시간 * 시간당 비용</pre> </td> 
    </tr> 
    <tr> 
     <td>예산책정된 인건비</td> 
     <td> <p>다음 공식을 사용하여 계산됩니다.</p><pre>예산책정된 노무비 = 예산책정된 시간 * 시간당 비용</pre> </td> 
    </tr> 
    <tr> 
     <td>실제 인건비</td> 
     <td> <p>다음 공식을 사용하여 계산됩니다.</p><pre>실제 노무비 = 실제 시간 * 시간당 비용</pre> </td> 
    </tr> 
   </tbody> 
  </table>

   자세한 내용은 [Workfront이 계획, 예산책정 및 실제 원가를 계산하는 방법](#how-workfront-calculates-planned-budgeted-and-actual-costs) 섹션에 자세히 설명되어 있습니다.

* **비용 비용** 프로젝트 및 작업의 비용과 연관됩니다.\
   프로젝트를 생성할 때 전체 프로젝트에 대한 계획 비용을 설정할 수 있습니다. 또한 비용을 신규 또는 기존 작업과 연관시킬 수 있습니다. 자세한 내용은 [프로젝트 비용 관리](../../../manage-work/projects/project-finances/manage-project-expenses.md).

* **고정 비용** 는 프로젝트에 대한 고정 비용으로 정의됩니다. 프로젝트를 완료하는 데 필요한 금액을 나타내는 프로젝트의 계획 비용의 일부입니다.

   >[!TIP]
   >
   >템플릿을 프로젝트에 첨부할 때 템플릿의 고정 비용이 프로젝트의 고정 비용에 추가됩니다. 자세한 내용은 [프로젝트에 템플릿 첨부 개요](../../../manage-work/projects/create-and-manage-templates/attach-template-to-project-overview.md).

### Workfront이 계획, 예산책정 및 실제 원가를 계산하는 방법 {#how-workfront-calculates-planned-budgeted-and-actual-costs}

Workfront은 프로젝트의 각 개별 태스크에 대한 계획 원가 및 실제 원가를 계산합니다. Workfront은 개별 작업에 이러한 계산을 사용하여 프로젝트에 대한 계획 원가와 실제 비용을 계산합니다.

* [계획된 비용](#planned-cost)
* [예산 비용](#budgeted-cost)
* [실제 비용](#actual-cost)

#### 계획된 비용 {#planned-cost}

프로젝트의 계획 원가는 프로젝트의 계획 작업 시간(계획 시간)과 연관된 원가입니다.

프로젝트의 계획 원가는 다음 공식으로 계산됩니다.

```
Planned Project Cost = Planned Labor Cost of all tasks + Planned Expense cost of all tasks + Planned Expense Cost of the project + Fixed Cost of the project
```

예를 들어, 작업의 비용 탭에 다음과 같은 비용이 있습니다. 100달러의 마케팅 비용과 50달러의 관리 비용. 재무 탭에서 사용자 시간별 원가 유형을 선택합니다. 사용자에게 작업이 할당되고 사용자의 시간당 비율은 $15입니다. 사용자는 이 작업에서 5시간 작업에 할당됩니다. 프로젝트의 비용 탭에는 컨설팅이라는 비용에 대해 100달러의 계획 비용이 있습니다. 프로젝트에 대해 200달러의 고정 비용이 있습니다.

프로젝트의 계획 비용은 다음과 같이 계산됩니다.

```
$100 (Consulting Expense) + $100 (Marketing Expense) + $50 (Administrative Expense) + $15(Hourly Rate)*5(Planned Hours Logged) + $200 (Fixed Cost) = $525
```

#### 예산 비용 {#budgeted-cost}

프로젝트의 예산책정된 원가는 프로젝트에 대한 예산책정된 작업(예산책정된 시간)과 연관된 원가입니다.

다음 두 가지 조건이 충족되는 경우 프로젝트의 예산 원가와 프로젝트 계획 원가가 동일합니다.

* 프로젝트의 계획 시간(자원 계획자)이 예산책정된 시간과 일치합니다
* 태스크 청구 유형은 시간별 역할입니다.

다음 조건이 충족되는 경우 아래 공식을 사용하여 프로젝트의 예산 원가를 계산합니다.

* 프로젝트의 계획 시간(Resource Planner)이 예산책정된 시간과 일치하지 않습니다.
* 작업의 청구 유형은 시간별 역할입니다.

위의 조건이 충족되면 Workfront은 다음 공식을 사용하여 프로젝트의 예산책정된 원가를 계산합니다.
<pre>예산책정된 프로젝트 원가 = 예산책정된 노무비 + 모든 태스크의 예산책정된 비용 + 프로젝트의 예산책정된 비용</pre>

#### 실제 비용 {#actual-cost}

프로젝트의 실제 원가는 프로젝트의 실제 작업 시간(로그된 시간)과 연관된 원가입니다.

실제 원가는 다음 공식을 사용하여 계산됩니다.

```
Actual Project Cost = Actual Labor Cost of all tasks + Actual Expense Cost of all tasks + Actual Labor Cost of the project + Actual Expense Cost of the project + Fixed Cost of the project
```

예를 들어, 작업의 비용 탭에 다음과 같은 비용이 있습니다. 실제 원가가 110달러이고 실제 원가가 40달러인 관리 비용이 있는 마케팅 비용. 역할 시간별 원가 유형을 선택하고 작업에 컨설턴트 작업 역할을 지정합니다. 컨설턴트 작업 역할의 비율은 시간당 15달러이고 컨설턴트 작업 역할에 대해 작업에 로그온하는 6시간이 있습니다. 프로젝트(비용 탭)와 연관된 컨설팅 비용이 있으며 실제 비용은 $100이며 사용자 프로필에서 시간당 비용이 $20인 사용자가 프로젝트에서 10시간 동안 기록됩니다. 프로젝트에 대해 200달러의 고정 비용이 있습니다.

프로젝트의 실제 비용은 다음과 같이 계산됩니다.

```
$100 (Consulting Expense) + $110 (Marketing Expense) + $40 (Administrative Expense) +$15 (Hourly Rate)*6 (Actual Hours Logged) + $20 (Cost per Hour rate for the user logging time on the project)*10 (hours the user logs on the project) + $200 (Fixed Cost) = $740
```

>[!NOTE]
>
>프로젝트에 대한 시간을 기록할 때 프로젝트에 대한 실제 노무비를 계산할 때 다음 시나리오가 존재합니다.
>
>* 기본적으로 Workfront은 사용자의 시간당 비용 비율을 사용하여 실제 노무비를 계산합니다.
>* 시간을 기록하는 사용자가 비용과 연관되지 않은 경우 Workfront은 사용자의 기본 역할에 대한 시간당 비용 비율을 사용합니다.
>* Workfront 관리자가 **작업 역할을 시간 항목에 수동으로 할당** 작업표 및 시간 기본 설정 영역에서 를 설정하고, 프로젝트의 사용자 로깅 시간이 이 시간과 연결할 다른 역할을 선택하면 프로젝트의 실제 비용은 시간이 기록될 때 지정된 역할에 따라 계산됩니다. 특정 작업 역할에 대한 로깅 시간을 활성화하는 방법에 대한 내용은 문서를 참조하십시오 [작업표 및 시간 환경 설정 구성](../../../administration-and-setup/set-up-workfront/configure-timesheets-schedules/timesheet-and-hour-preferences.md).
>


### Workfront이 작업의 비용 유형을 계산하는 방법 {#how-workfront-calculates-cost-types-for-tasks}

태스크 및 노무비의 계획 및 실제 원가는 각 태스크의 원가 유형에 의해 결정됩니다.

프로젝트 내의 개별 작업에 대한 원가 유형을 구성할 수 있습니다. 각 원가 유형은 계획 원가 및 실제 원가 값에 영향을 줍니다.

작업의 비용 유형을 수정하는 방법에 대한 자세한 내용은 [태스크 원가 유형 갱신](../../../manage-work/tasks/task-information/update-task-cost-type.md).

다음 표에서는 Workfront에서 사용 가능한 작업 비용 유형에 대해 설명합니다.

<table border="1" cellspacing="15"> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th> <p><strong>작업 비용 유형</strong> </p> </th> 
   <th> <p><strong>설명</strong> </p> </th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td> <p>시간별 사용자</p> </td> 
   <td> <p>작업을 생성할 때 기본 원가 유형입니다.</p> <p><strong>계획 비용</strong> 는 다음 수식으로 계산됩니다. </p> <p><code style="font-style: normal;">Task Planned Cost = Task Planned Labor Cost + Task Planned Expense Cost</code> </p> <p>계획 노무비를 계산되는 경우<br><code>Planned Labor Cost = Planned Hours * Cost per Hour Rate of the User assigned to the task</code></p> <p>참고:   <p>사용자 시간별 원가 유형을 사용하고 계획 원가를 계산할 때 다음과 같은 영향을 고려하십시오.</p> 
     <ul> 
      <li>작업에 여러 리소스를 지정하는 경우 Workfront은 각 리소스에 할당된 작업의 백분율에 따라 계획 비용에 대한 계산을 조정합니다.</li> 
      <li>계획 원가 필드의 값은 작업 자체에서 계획 원가를 볼지 또는 활용률 보고서와 비교하여 다를 수 있습니다.<br><strong>작업 자체에서 계획 원가를 조회할 때:</strong> 계획 원가 필드는 작업 역할 레벨에서 설정된 원가/Hr 필드를 고려합니다(사용자 레벨에서 원가/Hr 필드가 설정되지 않은 경우).<br><strong>프로젝트의 가동률 보고서에서 계획 원가를 조회할 때</strong> 계획 원가 필드는 작업 역할 레벨에서 설정된 비용/시간 필드를 고려하지 않습니다. 대신, 작업 역할 레벨에서 설정된 비용/시간 필드를 고려하여 활용률 보고서를 고려할 경우 작업의 비용 유형을 시간별 역할로 설정해야 합니다. </li> 
     </ul> </p> <p><strong>실제 비용</strong> 는 다음 수식으로 계산됩니다. </p> <p><code style="font-style: normal;">Task Actual Cost = Actual Labor Cost + Task Actual Expense Cost</code> </p> <p>실제 노무비가 계산되는 경우</p> <p><code>Actual Labor Cost = Actual Hours * Cost per Hour Rate of the User logging the hours</code> </p> <p>예를 들어, 사용자의 프로필에는 시간당 비용 $20가 있습니다. 작업에 대해 5시간을 기록하면 실제 인건비 비용은 해당 작업에 대해 100달러입니다. 사용자에게 시간당 비용이 연관된 경우, 실제 원가는 1차 작업 역할의 시간당 비용 비율을 기준으로 계산됩니다. Job 역할이 없거나 Job 역할의 시간당 비용 비율이 정의되지 않은 경우 작업의 실제 비용은 0입니다. </p> <p>참고: 실제 원가는 작업에 지정된 사람에 관계없이 시간을 기록하고 있는 사용자의 시간당 비용을 기준으로 계산됩니다. </p> </td> 
  </tr> 
  <tr> 
   <td> <p>시간별 역할</p> </td> 
   <td> <p><strong>계획 비용</strong> 는 다음 수식으로 계산됩니다. </p> <p><code style="font-style: normal;">Task Planned Cost = Task Planned Labor Cost+ Task Planned Expense Cost</code> </p> <p>태스크 계획 노무비 계산 위치:</p> <p><code>Task Planned Labor Cost = Planned Hours * Cost per Hour Rate of the Job Role assigned to the task</code> </p> <p>참고: 작업에 여러 리소스를 할당하는 경우 Workfront은 각 리소스에 할당된 작업의 백분율에 따라 계획 시간에 대한 계산을 조정합니다.</p> <p><strong>실제 비용</strong> 는 다음 수식으로 계산됩니다. </p> <p><code style="font-style: normal;">Task Actual Cost = Task Actual Labor Cost + Task Actual Expense Cost</code> </p> <p>태스크 실제 노무비 계산 위치:</p> <p><code>Task Actual Labor Cost = Actual Hours * Cost per Hour Rate of the Job Role assigned to the task</code> </p> <p>예를 들어, 작업은 Job 역할이나 Job 역할이 있는 사용자에게 할당되며, Cost per Hour 비율이 $20입니다. 사용자가 작업에 대해 5시간을 기록하면 실제 인건비 비용은 해당 작업에 대해 100달러입니다. 작업에 지정된 사용자에게 태스크에 연관된 작업 역할이 없는 경우 실제 원가는 1차 작업 역할의 시간당 원가에 따라 계산됩니다. Job 역할이 없거나 Job 역할의 시간당 비용 비율이 정의되지 않은 경우 작업의 실제 비용은 0입니다. </p> <p>참고:   <p> 시간별 역할의 실제 시간 작업은 시간을 기록하는 사용자와 연관된 역할이 아니라 작업과 연결된 사용자의 작업 역할에 따라 계산됩니다.</p> <p>Workfront 관리자가 <strong>작업 역할을 시간 항목에 수동으로 할당</strong> 작업표 및 시간 기본 설정 영역에서 설정하고, 작업에 대한 사용자 로깅 시간이 이 시간과 연결할 다른 역할을 선택하면 시간별 역할 실제 비용 작업은 시간이 기록될 때 지정된 역할에 따라 계산됩니다. 특정 작업 역할에 대한 로깅 시간을 활성화하는 방법에 대한 내용은 문서를 참조하십시오 <a href="../../../administration-and-setup/set-up-workfront/configure-timesheets-schedules/timesheet-and-hour-preferences.md" class="MCXref xref">작업표 및 시간 환경 설정 구성</a>.</p> </p> </td> 
  </tr> 
  <tr> 
   <td> <p>고정 시간별</p> </td> 
   <td> <p><strong>계획 비용</strong> 는 다음 수식으로 계산됩니다.</p> <p><code style="font-style: normal;">Task Planned Cost = Task Planned Labor Cost + Task Planned Expense Cost</code> </p> <p>태스크 노무 원가가 계산되는 위치:</p> <p><code>Task Planned Labor Cost = Planned Hours * Fixed Hourly Cost of the Task</code> </p> <p><strong>실제 비용</strong> 는 다음 수식으로 계산됩니다. </p> <p><code style="font-style: normal;">Task Actual Cost = Actual Task Labor Cost + Task Planned Expense Cost</code> </p> <p>실제 태스크 노무 원가가 계산되는 경우:</p> <p><code>Task Actual Labor Cost = Actual Hours * Fixed Hourly Cost of the Task</code> </p> <p>이 비용 유형은 개별 사용자 또는 작업 역할을 고려하지 않습니다.</p> </td> 
  </tr> 
  <tr> 
   <td> <p>비용 없음</p> </td> 
   <td> <p>이 원가 유형은 비용에 영향을 주지 않습니다. 상위 태스크에 이 원가 유형이 있는 경우, 다른 원가 유형을 사용하는 하위 태스크는 개별 원가 유형에 따라 계산되며, 상위 태스크의 원가가 그에 따라 영향을 받습니다. </p> <p>재무 데이터에 대한 액세스 권한이 없는 사용자 또는 템플릿에 대한 재무 권한이 없는 사용자가 해당 템플릿에서 프로젝트를 생성하는 경우, 이는 프로젝트의 작업에 대한 기본 비용 유형입니다.</p> <p>재무 데이터 액세스에 대한 자세한 내용은 문서를 참조하십시오 <a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-financial.md" class="MCXref xref">재무 데이터에 대한 액세스 권한 부여</a>.</p> <p>객체에 대한 재무 권한에 대한 자세한 내용은 문서를 참조하십시오 <a href="../../../workfront-basics/grant-and-request-access-to-objects/share-financial-permissions-object.md" class="MCXref xref">개체에 대한 재무 권한 공유</a>.</p> <p>템플릿에서 프로젝트 만들기에 대한 자세한 내용은 문서를 참조하십시오 <a href="../../../manage-work/projects/create-projects/create-project-from-template.md" class="MCXref xref">템플릿을 사용하여 프로젝트 만들기</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

<!--
<div data-mc-conditions="QuicksilverOrClassic.Draft mode">
<p>(NOTE: drafted because this was moved to its own how-to article linked above. Could be removed after some time.) </p>
<p>To configure the Cost Type of an individual task:</p>
<ol>
<li value="1">Go to the task where you want to configure the Cost Type. </li>
<li value="2"> <p data-mc-conditions="QuicksilverOrClassic.Quicksilver">Click <strong>Task Details</strong> in the left panel, then expand the <strong>Finance</strong> area. </p> </li>
<li value="3"> <p data-mc-conditions="QuicksilverOrClassic.Quicksilver">Double click <strong>Cost Type</strong> and select the cost type that you want to apply to the task. </p> </li>
<li value="4">Click <strong>Save.</strong></li>
</ol>
</div>
-->

## Workfront이 문제에 대한 비용을 추적하는 방법 {#how-workfront-tracks-costs-for-issues}

문제는 프로젝트에 대한 다음 유형의 비용이 없고 영향을 주지 않습니다.

* 계획된 비용
* 예산 비용

그러나 문제는 **실제 비용** 프로젝트의 실제 비용에도 영향을 줍니다.

다음 표에서는 문제에 대한 지정 유형에 따라 문제에 대해 실제 비용을 계산하는 방법을 설명합니다.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th colspan="4">발행 실제 비용</th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td> <p>사용자 지정</p> <p> </p> </td> 
   <td colspan="3"> <p><strong>실제 비용</strong> 는 다음 수식으로 계산됩니다.</p> <p><code style="font-style: normal;">Issue Actual Cost = Actual Hours * Cost per Hour rate of the user logging the hours</code> </p> <p>시간을 기록하고 있는 사용자의 시간당 비용 비율은 문제에 지정된 사람에 관계없이 여기에서 고려됩니다. </p> <p>시간을 기록하는 사용자가 프로필에 시간당 비용이 없는 경우, 1차 작업 역할의 시간당 비용 비율은 문제의 실제 비용을 계산합니다. 시간을 기록하고 있는 사용자가 프로파일에 역할이 없거나 해당 시간과 연관된 비율이 없는 경우, 실제 시간은 해당 문제에 대한 기본 담당자의 주요 작업 역할의 시간당 비용 비율을 사용하여 계산됩니다. 해당 역할에 정의된 비율이 없는 경우 문제의 실제 비용은 0입니다. </p> </td> 
  </tr> 
  <tr> 
   <td> <p>역할 할당</p> <p> </p> </td> 
   <td colspan="3"> <p><strong>실제 비용</strong> 는 다음 수식으로 계산됩니다.</p><code>Issue Actual Cost = Actual Hours * Cost per Hour Rate of user logging the hours</code> <p>문제에 지정된 역할과 관계없이 문제 발생 시간을 기록하는 사용자의 시간당 비용 비율은 여기에서 고려됩니다. </p> <p>시간을 기록하는 사용자에게 시간 당 비용이 연결되어 있지 않은 경우, 주 역할의 시간당 비용 비율은 문제의 실제 비용을 계산합니다.<br>시간을 기록하는 사용자가 프로필에 역할이 없거나 해당 시간과 연관된 비율이 없는 경우 문제의 실제 비용은 0입니다. </p> </td> 
  </tr> 
  <tr> 
   <td> <p>할당 없음</p> <p> </p> </td> 
   <td colspan="3"> <p><strong>실제 비용</strong> 는 다음 수식으로 계산됩니다.</p> <p><code>Issue Actual Cost = Actual Hours * Cost per Hour rate of the user logging the hours</code> </p> <p>시간을 기록하는 사용자에게 해당 프로필과 연관된 시간당 비용이 없는 경우, 1차 작업 역할의 시간당 비용 비율은 문제의 실제 비용을 계산합니다. </p> <p>시간을 기록하는 사용자에게 프로필과 연관된 작업 역할이 없거나 기본 작업 역할에 시간당 비용이 정의되어 있지 않으면 문제의 실제 비용은 0입니다. </p> </td> 
  </tr> 
  <!--<tr data-mc-conditions=""> 
   <td colspan="4"> 
    <div> <MadCap:conditionalText data-mc-conditions="">
       If your Workfront administrator enabled the 
      <strong>Assign Job Roles to hour entries manually</strong> setting in the Timesheets &amp; Hours Preferences area, and the user logging time on the issue selects a different role to associate with this time, the Actual Cost of the issue calculates based on the role specified when the hours were logged. For information about enabling logging time for a specific job role, see the article 
      <a href="../../../administration-and-setup/set-up-workfront/configure-timesheets-schedules/timesheet-and-hour-preferences.md" class="MCXref xref">Configure timesheet and hour preferences</a>. 
     </MadCap:conditionalText> 
    </div> </td> 
  </tr> 
  -->
 </tbody> 
</table>
