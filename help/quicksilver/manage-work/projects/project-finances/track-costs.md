---
content-type: reference;how-to-procedural
product-area: projects
navigation-topic: financials
title: 비용 추적
description: Adobe Workfront에서 프로젝트, 작업 및 문제에 대한 비용을 추적할 수 있습니다.
author: Alina, Lisa
feature: Work Management
exl-id: df3090ae-9721-4e9b-84b4-315890619801
source-git-commit: d2b62f2ec2f52c54129b342d68c336c782601242
workflow-type: tm+mt
source-wordcount: '2472'
ht-degree: 1%

---

# 비용 추적

{{highlighted-preview}}

Adobe Workfront에서 프로젝트, 작업 및 문제에 대한 비용을 추적할 수 있습니다.

## Workfront의 비용 계산 방법

비용을 추적하려면 사용자 및 작업 역할을 시간당 비용 요율과 연결해야 합니다.

시간당 비용 비율은 작업 역할 또는 사용자와 연결된 작업 단위당 비용 금액입니다. 요금에 작업 시간을 곱하면 프로젝트, 작업 또는 문제에 대한 비용이 발생합니다.

다음과 같은 시나리오가 있습니다.

* 작업의 비용 유형이 시간별 사용자인 경우 사용자 시간당 비율은 작업 및 프로젝트 비용을 계산합니다.

  사용자를 원가율과 연관시키는 방법에 대한 자세한 내용은 다음을 참조하십시오. [사용자 프로필 편집](../../../administration-and-setup/add-users/create-and-manage-users/edit-a-users-profile.md).

* 작업의 비용 유형이 시간별 역할인 경우 작업 역할 시간당 비율은 작업 및 프로젝트 비용을 계산합니다.

  작업 역할과 원가율 연관에 대한 자세한 내용은 다음을 참조하십시오. [작업 역할 만들기 및 관리](../../../administration-and-setup/set-up-workfront/organizational-setup/create-manage-job-roles.md).

* Workfront은 문제에 대해 실제 비용만 계산하며, 비용 유형이 없는 문제입니다. 자세한 내용은 섹션을 참조하십시오 [Workfront에서 문제 비용을 추적하는 방법](#how-workfront-tracks-costs-for-issues) 이 문서에서.

>[!TIP]
>
>프로젝트의 원가율을 재정의할 수 없습니다. 사용자 또는 작업 역할에 대해 시간당 비용 비율을 설정하면 해당 비율이 시스템의 모든 비용을 계산합니다.

## Workfront 비용 성과 지표

Workfront은 비용 효율성을 위해 프로젝트를 추적할 수 있도록 프로젝트에 대한 여러 비용 성과 지수를 계산합니다.\
비용 성과 지표 계산에 대한 자세한 내용은 다음을 참조하십시오.

* [원가 성과 지수(CPI) 계산](../../../manage-work/projects/project-finances/calculate-cpi.md)
* [CSI(원가 일정 성과 지표) 계산](../../../manage-work/projects/project-finances/calculate-csi.md)
* [SPI(일정 성과 지수) 계산](../../../manage-work/projects/project-finances/calculate-spi.md)

## Workfront에서 작업 및 프로젝트 비용을 추적하는 방법

* [Workfront의 비용 추적 방법](#how-workfront-tracks-costs)
* [Workfront에서 계획, 예산 및 실제 비용을 계산하는 방법](#how-workfront-calculates-planned-budgeted-and-actual-costs)
* [Workfront에서 작업에 대한 비용 유형을 계산하는 방법](#how-workfront-calculates-cost-types-for-tasks)

### Workfront의 비용 추적 방법  {#how-workfront-tracks-costs}

Workfront에서 작업 및 프로젝트에 대한 여러 유형의 비용을 추적할 수 있습니다. 전체 원가는 다음 공식에 의해 계산됩니다.

`Costs = Labor Costs + Expense Costs`

* **인건비** 은 작업 및 프로젝트의 시간 및 작업과 연결된 리소스의 시간당 비용 비율과 연결됩니다. 일반적으로 Workfront은 다음과 같은 인건비를 계산합니다.

  <table style="table-layout:auto"> 
   <col> 
   <col> 
   <tbody> 
    <tr> 
     <td>계획된 인건비</td> 
     <td> <p>다음 공식을 사용하여 계산됩니다.</p><code>Planned Labor Costs = Planned Hours * Cost per Hour rate</code> </td> 
    </tr> 
    <tr> 
     <td>예산 인건비</td> 
     <td> <p>다음 공식을 사용하여 계산됩니다.</p><code>Budgeted Labor Costs = Budgeted Hours * Cost per Hour rate</code> </td> 
    </tr> 
    <tr> 
     <td>실제 인건비</td> 
     <td> <p>다음 공식을 사용하여 계산됩니다.</p><code>Actual Labor Costs = Actual Hours * Cost per Hour rate</code> </td> 
    </tr> 
   </tbody> 
  </table>

  자세한 내용은 [Workfront에서 계획, 예산 및 실제 비용을 계산하는 방법](#how-workfront-calculates-planned-budgeted-and-actual-costs) 이 문서의 섹션.

* **경비** 프로젝트 및 작업의 경비와 연결됩니다.\
  프로젝트를 만들 때 전체 프로젝트에 대해 계획된 비용을 설정할 수 있습니다. 또한 경비를 새 작업이나 기존 작업과 연결할 수 있습니다. 자세한 내용은 [프로젝트 경비 관리](../../../manage-work/projects/project-finances/manage-project-expenses.md).

* **고정 비용** 는 프로젝트에 대한 고정 비용으로 정의됩니다. 이는 프로젝트를 완료하는 데 필요한 금액을 나타내는 프로젝트 계획된 비용의 일부입니다.

  >[!TIP]
  >
  >템플릿을 프로젝트에 첨부할 때 템플릿의 고정 비용이 프로젝트의 고정 비용에 추가됩니다. 자세한 내용은 [프로젝트에 템플릿 첨부 개요](../../../manage-work/projects/create-and-manage-templates/attach-template-to-project-overview.md).

### Workfront에서 계획, 예산 및 실제 비용을 계산하는 방법 {#how-workfront-calculates-planned-budgeted-and-actual-costs}

Workfront은 프로젝트의 각 개별 작업에 대한 계획된 비용과 실제 비용을 계산합니다. Workfront은 개별 작업에 대해 이러한 계산을 사용하여 프로젝트의 계획된 비용 및 실제 비용을 계산합니다.

* [계획된 비용](#planned-cost)
* [예산 비용](#budgeted-cost)
* [실제 비용](#actual-cost)

#### 계획된 비용 {#planned-cost}

프로젝트의 계획된 비용은 프로젝트의 계획된 작업(계획된 시간)과 관련된 비용입니다.

프로젝트의 계획된 비용은 다음 공식에 의해 계산됩니다.

`Planned Project Cost = Planned Labor Cost of all tasks + Planned Expense cost of all tasks + Planned Expense Cost of the project + Fixed Cost of the project`

예를 들어, 작업의 경비 탭에 $100 마케팅 비용과 $50 관리 비용이 있습니다. 재무 탭에서 사용자 시간당 비용 유형을 선택합니다. 사용자가 작업에 할당되며 사용자의 시간당 요금은 $15입니다. 사용자가 이 작업에 대한 5시간 작업에 할당되었습니다. 프로젝트의 경비 탭에서 컨설팅 비용이라는 경비에 대해 $100의 계획된 비용이 있습니다. 또한 프로젝트에 200달러의 고정 비용이 있습니다.

프로젝트의 계획된 비용은 다음과 같이 계산됩니다.

`$100 (Consulting Expense) + $100 (Marketing Expense) + $50 (Administrative Expense) + $15(Hourly Rate)*5(Planned Hours Logged) + $200 (Fixed Cost) = $525`

<span class="preview">공식의 시간당 환율은 환율의 모든 일자 유효 변경 사항을 고려합니다.</span>

#### 예산 비용 {#budgeted-cost}

프로젝트의 예산 비용은 프로젝트의 예산 작업(예산 시간)과 관련된 비용입니다.

다음 두 가지 조건이 충족되는 경우 프로젝트의 예산 원가는 프로젝트의 계획된 원가와 동일합니다.

* 프로젝트에 대한 작업의 계획된 시간이 예산 시간(리소스 플래너)과 일치합니다.
* 작업 청구 유형은 시간별 역할입니다.

다음 조건이 충족되는 경우 프로젝트의 예산 비용은 아래 공식을 사용하여 계산됩니다.

* 프로젝트에 대한 작업의 계획된 시간이 (리소스 플래너에서) 예산 시간과 일치하지 않습니다.
* 작업의 청구 유형은 시간별 역할입니다.

위의 조건이 충족되면 Workfront은 다음 공식을 사용하여 프로젝트의 예산 비용을 계산합니다.

`Budgeted Project Cost = Budgeted Labor Cost + Budgeted Expense Cost of all tasks + Budgeted Expense Cost of the project`

#### 실제 비용 {#actual-cost}

프로젝트의 실제 비용은 프로젝트의 실제 작업(기록된 시간)과 관련된 비용입니다.

실제 원가는 다음 공식을 사용하여 계산됩니다.

`Actual Project Cost = Actual Labor Cost of all tasks + Actual Expense Cost of all tasks + Actual Labor Cost of the project + Actual Expense Cost of the project + Fixed Cost of the project`

예를 들어, 작업의 비용 탭에 실제 비용이 $110인 마케팅 비용과 실제 비용이 $40인 관리 비용이 있습니다. 역할 시간당 비용 유형을 선택하고 컨설턴트의 작업 역할을 작업에 할당합니다. 컨설턴트 작업 역할의 비율은 시간당 15달러이며, 컨설턴트 작업 역할에 대한 작업에 6시간이 기록됩니다. 경비 탭에 프로젝트와 관련된 컨설팅 비용이 있습니다. 실제 비용은 $100이고 시간당 비용 비율은 $20인 사용자가 사용자 프로필 로그에 프로젝트의 10시간을 기록합니다. 또한 프로젝트에 200달러의 고정 비용이 있습니다.

프로젝트의 실제 비용은 다음과 같이 계산됩니다.

`$100 (Consulting Expense) + $110 (Marketing Expense) + $40 (Administrative Expense) +$15 (Hourly Rate)*6 (Actual Hours Logged) + $20 (Cost per Hour rate for the user logging time on the project)*10 (hours the user logs on the project) + $200 (Fixed Cost) = $740`

<span class="preview">공식의 시간당 환율은 환율의 모든 일자 유효 변경 사항을 고려합니다.</span>

>[!NOTE]
>
>프로젝트의 실제 비용은 다음과 같이 계산됩니다.
>`SUM (All Project Actual Expense Costs) + SUM (All Tasks Actual Expense Costs) + Project Fixed Cost`
>
>이러한 비용은 실제 비용 계산에서 중복되지 않습니다. 예를 들어 고정 비용이 프로젝트의 실제 비용 비용의 일부인 경우 실제 비용에 별도로 추가되지 않습니다.

>[!NOTE]
>
>프로젝트에 대한 시간을 기록할 때 프로젝트의 실제 인건비를 계산할 때 다음과 같은 시나리오가 존재합니다.
>
>* 기본적으로 Workfront은 사용자의 시간당 비용 비율을 사용하여 실제 인건비를 계산합니다.
>* 시간을 기록하는 사용자가 비용과 관련이 없는 경우 Workfront은 사용자의 기본 역할의 시간당 비용 비율을 사용합니다.
>* Workfront 관리자가 **시간 항목에 수동으로 작업 역할 할당** 타임시트 및 시간 환경 설정 영역에서 을 설정하고 프로젝트의 사용자 로깅 시간이 이 시간과 연결할 다른 역할을 선택하면 시간이 기록되었을 때 지정된 역할을 기반으로 프로젝트의 실제 비용이 계산됩니다. 특정 작업 역할에 대한 로깅 시간 활성화에 대한 자세한 내용은 문서 를 참조하십시오 [타임시트 및 시간 환경 설정 구성](../../../administration-and-setup/set-up-workfront/configure-timesheets-schedules/timesheet-and-hour-preferences.md).

### Workfront에서 작업에 대한 비용 유형을 계산하는 방법 {#how-workfront-calculates-cost-types-for-tasks}

태스크의 계획 및 실제 비용과 해당 노무비는 각 태스크의 원가 유형에 따라 결정됩니다.

프로젝트 내의 개별 작업에 대한 비용 유형을 구성할 수 있습니다. 각 원가 유형은 계획된 원가 및 실제 원가 값에 영향을 줍니다.

작업의 비용 유형을 수정하는 방법에 대한 자세한 내용은 [작업 비용 유형 업데이트](../../../manage-work/tasks/task-information/update-task-cost-type.md).

다음 표에서는 Workfront에서 사용 가능한 작업 비용 유형을 설명합니다.

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
   <td> <p>작업을 생성할 때 기본 원가 유형이 됩니다.</p> <p><strong>계획된 비용</strong> 는 다음 공식으로 계산됩니다. </p> <p><code style="font-style: normal;">Task Planned Cost = Task Planned Labor Cost + Task Planned Expense Cost</code> </p> <p>계획된 인건비 계산 방법:<br><code>Planned Labor Cost = Planned Hours * Cost per Hour Rate of the User assigned to the task</code></p> <p>참고: <p>사용자 시간당 비용 유형 사용 및 계획된 비용 계산의 영향을 고려하십시오.</p> 
     <ul> 
      <li>작업에 여러 리소스를 할당하면 Workfront은 각 리소스에 할당된 작업의 백분율을 기준으로 계획된 비용에 대한 계산을 조정합니다.</li>
      <li><span class="preview">일자 유효 원가율의 경우, 계획된 인건비는 태스크에 포함된 각 기간의 계획된 원가의 합계입니다.</span></li>
      <li>계획된 비용 필드의 값은 계획된 비용을 태스크 자체에서 조회하는지 아니면 활용률 보고서에서 조회하는지에 따라 다를 수 있습니다.<br><strong>작업 자체에서 계획된 비용을 볼 때:</strong> 계획된 비용 필드는 작업 역할 레벨에서 설정된 비용/Hr 필드를 고려합니다(비용/Hr 필드가 사용자 레벨에서 설정되지 않은 경우).<br><strong>프로젝트에 대한 활용성 보고서에서 계획된 원가를 조회할 때</strong> 계획된 비용 필드는 작업 역할 레벨에서 설정된 비용/시간 필드를 고려하지 않습니다. 대신 활용성 보고서에서 작업 역할 레벨에 설정된 비용/시간 필드를 고려하려면 태스크에 대한 비용 유형을 시간별 역할로 설정해야 합니다. </li> 
     </ul> </p> <p><strong>실제 비용</strong> 는 다음 공식으로 계산됩니다. </p> <p><code style="font-style: normal;">Task Actual Cost = Actual Labor Cost + Task Actual Expense Cost</code> </p> <p>실제 인건비를 계산하는 방법:</p> <p><code>Actual Labor Cost = Actual Hours * Cost per Hour Rate of the User logging the hours</code> </p> <p>예를 들어 사용자의 프로필에서 시간당 비용 비율이 $20입니다. 작업에 대해 5시간을 기록할 때 실제 인건비는 해당 작업에 대해 $100입니다. 사용자에게 시간당 비용 비율이 연결되어 있지 않으면 실제 비용은 기본 작업 역할의 시간당 비용 비율을 기반으로 계산됩니다. 작업 역할이 없거나 작업 역할의 시간당 비용 비율이 정의되지 않은 경우 작업의 실제 비용은 0입니다. </p> <p>주: 실제 비용은 작업에 할당된 사용자에 관계없이 시간을 기록하는 사용자의 시간당 비용을 기준으로 계산됩니다. <span class="preview">또한 공식의 청구 시간당 요금은 요금의 모든 일자 유효 변경 사항을 고려합니다.</span></p> </td> 
  </tr> 
  <tr> 
   <td> <p>시간별 역할</p> </td>
   <td> <p><strong>계획된 비용</strong> 는 다음 공식으로 계산됩니다. </p> <p><code style="font-style: normal;">Task Planned Cost = Task Planned Labor Cost+ Task Planned Expense Cost</code> </p> <p>태스크 계획 노무비 계산 방법:</p> <p><code>Task Planned Labor Cost = Planned Hours * Cost per Hour Rate of the Job Role assigned to the task</code> </p> <p>참고: 작업에 여러 리소스를 할당하면 Workfront은 각 리소스에 할당된 작업의 백분율을 기준으로 계획된 시간에 대한 계산을 조정합니다. <span class="preview">또한 공식의 시간별 비율은 비율의 모든 날짜 유효 변경 사항을 고려합니다.</span></p> <p><strong>실제 비용</strong> 는 다음 공식으로 계산됩니다. </p> <p><code style="font-style: normal;">Task Actual Cost = Task Actual Labor Cost + Task Actual Expense Cost</code> </p> <p>태스크 실제 노무비 계산 기준:</p> <p><code>Task Actual Labor Cost = Actual Hours * Cost per Hour Rate of the Job Role assigned to the task</code> </p> <p>예를 들어 작업 역할이나 시간당 비용 비율이 $20인 작업 역할이 있는 사용자에게 작업이 할당됩니다. 사용자가 작업에 대해 5시간을 기록할 때 실제 인건비는 해당 작업에 대해 $100입니다. 작업에 할당된 사용자에게 작업에 연결된 작업 역할이 없는 경우 실제 비용은 기본 작업 역할의 시간당 비용을 기반으로 계산됩니다. 작업 역할이 없거나 작업 역할의 시간당 비용 비율이 정의되지 않은 경우 작업의 실제 비용은 0입니다. </p> <p>참고:   <p> 시간별 역할 작업의 실제 시간은 시간을 기록하는 사용자와 연결된 역할이 아니라 작업과 연결된 사용자의 작업 역할을 기준으로 계산됩니다. <span class="preview">또한 공식의 청구 시간당 요금은 요금의 모든 일자 유효 변경 사항을 고려합니다.</span></p> <p>Workfront 관리자가 <strong>시간 항목에 수동으로 작업 역할 할당</strong> 타임시트 및 시간 환경 설정 영역에서 을 설정하고 작업에 대한 사용자 로깅 시간을 설정하면 이 시간과 연결할 다른 역할이 선택됩니다. 시간별 작업의 실제 비용은 시간이 기록되었을 때 지정된 역할을 기반으로 계산됩니다. 특정 작업 역할에 대한 로깅 시간 활성화에 대한 자세한 내용은 문서 를 참조하십시오 <a href="../../../administration-and-setup/set-up-workfront/configure-timesheets-schedules/timesheet-and-hour-preferences.md" class="MCXref xref">타임시트 및 시간 환경 설정 구성</a>.</p> </p> </td> 
  </tr> 
  <tr> 
   <td> <p>고정 시간별</p> </td> 
   <td> <p><strong>계획된 비용</strong> 는 다음 공식으로 계산됩니다.</p> <p><code style="font-style: normal;">Task Planned Cost = Task Planned Labor Cost + Task Planned Expense Cost</code> </p> <p>태스크 노무비 계산 방법:</p> <p><code>Task Planned Labor Cost = Planned Hours * Fixed Hourly Cost of the Task</code> </p> <p><strong>실제 비용</strong> 는 다음 공식으로 계산됩니다. </p> <p><code style="font-style: normal;">Task Actual Cost = Actual Task Labor Cost + Task Planned Expense Cost</code> </p> <p>실제 태스크 노무비를 계산하는 방법:</p> <p><code>Task Actual Labor Cost = Actual Hours * Fixed Hourly Cost of the Task</code> </p> <p>이 비용 유형은 개별 사용자 또는 작업 역할을 고려하지 않습니다.</p> </td> 
  </tr> 
  <tr> 
   <td> <p>비용 없음</p> </td> 
   <td> <p>이 원가 유형은 원가에 영향을 주지 않습니다. 상위 태스크에 이 원가 유형이 있는 경우 다른 원가 유형이 있는 하위 태스크는 개별 원가 유형에 따라 계산되며 상위 태스크의 원가가 그에 따라 영향을 받습니다. </p> <p>재무 데이터에 대한 액세스 권한이 없는 사용자 또는 템플릿에 대한 재무 권한이 없는 사용자가 해당 템플릿에서 프로젝트를 만들 때 프로젝트의 작업에 대한 기본 비용 유형이 됩니다.</p> <p>재무 데이터 액세스에 대한 자세한 내용은 문서 를 참조하십시오 <a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-financial.md" class="MCXref xref">재무 데이터에 대한 액세스 권한 부여</a>.</p> <p>개체에 대한 재무 권한에 대한 자세한 내용은 문서 를 참조하십시오 <a href="../../../workfront-basics/grant-and-request-access-to-objects/share-financial-permissions-object.md" class="MCXref xref">개체에 대한 재무 권한 공유</a>.</p> <p>템플릿으로 프로젝트를 만드는 방법에 대한 자세한 내용은 문서 를 참조하십시오 <a href="../../../manage-work/projects/create-projects/create-project-from-template.md" class="MCXref xref">템플릿을 사용하여 프로젝트 만들기</a>.</p> </td> 
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

## Workfront에서 문제 비용을 추적하는 방법 {#how-workfront-tracks-costs-for-issues}

프로젝트에는 다음 유형의 비용이 없으며 영향을 주지 않습니다.

* 계획된 비용
* 예산 비용

그러나 문제에는 **실제 비용** 이는 프로젝트의 실제 비용에도 영향을 미칩니다.

다음 표에서는 문제에 대한 할당 유형에 따라 문제에 대한 실제 비용이 계산되는 방식을 설명합니다.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th colspan="4">문제 실제 비용</th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td> <p>사용자 할당</p> <p> </p> </td> 
   <td colspan="3"> <p><strong>실제 비용</strong> 는 다음 공식으로 계산됩니다.</p> <p><code style="font-style: normal;">Issue Actual Cost = Actual Hours * Cost per Hour rate of the user logging the hours</code> </p> <p>문제에 할당된 사용자와 관계없이 시간을 기록하는 사용자의 시간당 비용 요금 이 여기에서 고려됩니다. </p> <p>시간을 기록하는 사용자가 프로필에 시간당 비용 비율이 없는 경우 기본 작업 역할의 시간당 비용 비율은 문제의 실제 비용을 계산합니다. 시간을 기록 중인 사용자가 프로필에 역할이 없거나 연결된 요금이 없는 경우 문제에 대한 기본 피할당자의 기본 작업 역할의 시간당 비용 요금을 사용하여 실제 시간이 계산됩니다. 해당 역할에 정의된 비율이 없으면 문제의 실제 비용은 0입니다. </p> </td> 
  </tr> 
  <tr> 
   <td> <p>역할 할당</p> <p> </p> </td> 
   <td colspan="3"> <p><strong>실제 비용</strong> 는 다음 공식으로 계산됩니다.</p><code>Issue Actual Cost = Actual Hours * Cost per Hour Rate of user logging the hours</code> <p>문제에 할당된 역할에 관계없이 문제에 시간을 기록하는 사용자의 시간당 비용 비율이 여기에서 고려됩니다. </p> <p>시간을 기록하는 사용자에게 시간당 비용 비율이 연결되어 있지 않으면 기본 역할의 시간당 비용 비율은 문제의 실제 비용을 계산합니다.<br>시간을 기록하는 사용자가 프로필에 역할이 없거나 연결된 요금이 없는 경우 문제의 실제 비용은 0입니다. </p> </td> 
  </tr> 
  <tr> 
   <td> <p>할당 없음</p> <p> </p> </td> 
   <td colspan="3"> <p><strong>실제 비용</strong> 는 다음 공식으로 계산됩니다.</p> <p><code>Issue Actual Cost = Actual Hours * Cost per Hour rate of the user logging the hours</code> </p> <p>시간을 기록하는 사용자에게 프로필과 연계된 시간당 비용 비율이 없는 경우 기본 작업 역할의 시간당 비용 비율은 문제의 실제 비용을 계산합니다. </p> <p>시간을 기록하는 사용자에게 프로필과 연결된 작업 역할이 없거나 기본 작업 역할에 시간당 비용이 정의되어 있지 않으면 문제의 실제 비용은 0입니다. </p> </td> 
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
