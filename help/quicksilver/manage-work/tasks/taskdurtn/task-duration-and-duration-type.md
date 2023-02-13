---
content-type: overview
product-area: projects
navigation-topic: task-duration
title: 작업 기간 및 기간 유형 개요
description: 작업 기간은 작업의 계획 완료 일자와 계획 시작 일자 간의 차이입니다. 기간 은 작업이 완료되는 데 사용할 수 있는 기간을 나타냅니다.
author: Alina
feature: Work Management
exl-id: c81e485a-7e8c-4907-8e6c-9991681c3541
source-git-commit: f2f825280204b56d2dc85efc7a315a4377e551c7
workflow-type: tm+mt
source-wordcount: '1383'
ht-degree: 2%

---

# 작업 기간 및 기간 유형 개요

작업 기간은 작업의 계획 완료 일자와 계획 시작 일자 간의 차이입니다. 기간 은 작업이 완료되는 데 사용할 수 있는 기간을 나타냅니다.

작업의 기간 유형은 작업에 할당된 리소스 수, 총 투입 및 총 작업 기간 간의 관계를 식별합니다.

## 작업 기간 개요

>[!NOTE]
>
>프로젝트에서 기본 담당자의 휴가 시간을 고려할 때, 작업의 계획 날짜는 조정될 수 있지만, 작업 기간은 동일하게 유지됩니다. 프로젝트를 계획할 때 기본 할당자의 시간을 고려하는 방법에 대한 자세한 내용은  [시스템 전체 프로젝트 환경 설정 구성](../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-project-preferences.md).

작업의 실제 시작 및 실제 완료 날짜가 프로젝트 일정, 기본 담당자 또는 기본 일정 범위를 벗어나는 경우 작업 기간은 0입니다.

**예:** 오전 9시에 시작하여 오후 12시에 끝나는 스케줄과 오후 2시에 시작하여 오후 4시에 종료되도록 예약된 작업이 있는 경우 작업의 기간은 0입니다.

다음은 Adobe Workfront에서 기간을 계산할 때 존재하는 두 가지 시나리오입니다.

* 작업이 사용자 Workfront에 할당된 경우 다음 예약 중 하나를 사용하여 기간을 정확히 계산합니다.

   1. Workfront은 사용자의 일정을 고려합니다.
   1. 사용자가 예약과 연결되어 있지 않으면 Workfront에서 프로젝트 일정을 고려합니다.
   1. 프로젝트가 일정과 연결되어 있지 않으면 Workfront에서 시스템의 기본 일정을 고려합니다. 예약에 대한 자세한 내용은 [예약 만들기](../../../administration-and-setup/set-up-workfront/configure-timesheets-schedules/create-schedules.md).

* 작업이 여러 사용자에게 할당된 경우:

   Workfront은 프로젝트의 일정이나 기본 할당자의 일정을 고려합니다.

   Workfront 관리자는 작업이 여러 사용자에게 할당될 때 Workfront에서 사용하는 일정을 결정합니다. 자세한 내용은 [시스템 전체 프로젝트 환경 설정 구성](../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-project-preferences.md).

   이 단계는 Workfront에서 지속 시간을 계산하기 위해 사용하는 일정을 이해한 후 첫 번째 시나리오와 유사합니다.

## 작업 기간 시간 단위

계획 시작 및 계획 완료 일자 사이의 경과 시간 및 정규 시간 모두에 작업 기간을 표시할 수 있습니다.

목록에서 작업 기간을 업데이트할 때 Workfront의 시간 단위를 나타내는 다음 약어를 사용할 수 있습니다.

| 시간 단위 | 약어 |
|---|---|
| 분 | M |
| 시간 | H |
| 일. 기본값입니다. | D |
| 주 | W |
| 개월 | T |
| 경과 시간 (분) | EM |
| 경과 시간 | 에 |
| 경과 일수 | ED |
| 경과 주 수 | EW |
| 경과 기간 (월) | ET |

{style=&quot;table-layout:auto&quot;}

**예:** 작업의 기간이 3경과 일임을 나타내려면 작업 목록의 기간 필드에 &quot;3ED&quot;를 입력합니다.  작업을 편집할 때 사용 가능한 드롭다운 메뉴 또는 작업 세부 정보 섹션에서 기간 단위의 기본 설정 옵션을 선택할 수도 있습니다. 작업 편집에 대한 자세한 내용은 [작업 편집](../../../manage-work/tasks/manage-tasks/edit-tasks.md).

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: stays QS only forever; for the pictures below: make the first one classic at preview time and the second one stays QS always. The second one is yellow >> take out at 21.2 production!!)</p>
-->

![](assets/duration-elapsed-days-tasks-nwe-350x282.png)

작업 기간을 표시할 때 다음 사항을 고려하십시오.

* 경과 시간은 작업의 지속 시간에 대한 시간 단위입니다. 휴일, 주말 및 휴일이 포함된 작업의 계획 시작 일자와 계획 완료 일자 사이의 시간입니다. 즉, 경과 시간은 달력 일수의 경과입니다.
* 일반 시간은 휴일, 주말 및 휴가를 고려하여 작업 지속 시간에서 제외합니다.

* 작업 기간(주)을 지정하면, Workfront은 설정의 프로젝트 환경 설정 영역에서 Workfront 관리자가 설정한 일반 주당 근무 시간 및 일당 평균 시간 설정을 기준으로 기간(일 및 시간)을 계산합니다.
* Workfront에서는 기간(개월)을 계산할 때 1개월 동안 기본 기간인 4주를 사용합니다.

## 작업 기간 유형 개요

작업의 기간 유형 관리를 통해 작업의 필요에 따라 일관된 자원 지정을 설정할 수 있습니다.

기간 유형은 다음 질문에 답변하는 데 도움이 됩니다.

* 얼마나 바쁘죠?
* 그 일은 얼마나 큰가요?
* 얼마나 걸리나요?

![duration_type_triangle.png](assets/duration-type-triangle-350x245.png)

## 기간 유형 정의

<table border="1" cellspacing="15" cellpadding="1"> 
 <col> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th scope="row">기간 유형 </th> 
   <th scope="col"> <p><strong>함수</strong> </p> </th> 
   <th scope="col"> <p><strong>리소스 영향</strong> </p> </th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <th scope="col"> <p><strong>계산된 할당</strong> </p> </th> 
   <td scope="col"> <p>작업의 각 할당자에 대한 할당 비율을 계산합니다. </p> <p>이 기간 유형을 선택하면 작업에 대해 개별 기간 및 계획 시간을 입력할 수 있습니다. Workfront은 계획 시간을 작업 기간 내의 시간 수로 나눈 다음 작업에 할당된 리소스 수로 나누어 각 할당자에 대한 할당을 계산합니다.</p> <p>자세한 내용은 <a href="../../../manage-work/tasks/taskdurtn/calculated-assignment.md" class="MCXref xref">기간 유형 개요: 계산된 할당</a>.</p> </td> 
   <td scope="col">태스크에 지정자를 추가하거나 제거할 때 기간 및 계획 시간은 변경되지 않습니다. </td> 
  </tr> 
  <tr> 
   <th scope="col"> <p><strong>계산된 작업</strong> </p> </th> 
   <td scope="col"> <p>작업을 완료하는 데 필요한 계획 시간(작업량)을 결정합니다.</p> <p>일반적으로 작업에 할당된 리소스가 전체 작업 기간 동안 할당될 때 사용됩니다.</p> <p>이 기간 유형을 선택하면 작업에 대한 개별 기간 을 입력할 수 있습니다. Workfront은 작업 기간(일) 수에 예약의 작업 시간 수 및 작업에 대한 담당자 수를 곱하여 작업 계획 시간을 계산합니다. </p> <p>각 할당자의 할당 비율을 태스크로 수동으로 변경할 수 있으므로 계획 시간의 양이 단축됩니다.</p> <p>자세한 내용은 <a href="../../../manage-work/tasks/taskdurtn/calculated-work.md" class="MCXref xref">기간 유형 개요: 계산된 작업 시간</a>.</p> </td> 
   <td scope="col"> <p>작업이 작업에 추가되면 계획 시간이 증가합니다. </p> <p>작업 시 지정된 작업이 제거되면 계획 시간이 줄어듭니다.</p> </td> 
  </tr> 
  <tr> 
   <th scope="col"> <p>작업량 고정</p> </th> 
   <td scope="col"> <p>자원 수를 기준으로 계획 시간을 결정합니다.</p> <p>이 기간 유형을 선택하면 작업에 대한 개별 기간 을 입력할 수 있습니다. Workfront은 기간(일) 수에 예약의 작업 시간 수를 곱하고 작업에 할당된 시간 수로 나누어 작업에 대한 계획 시간을 계산합니다. </p> <p>각 할당자의 할당 비율을 수동으로 태스크로 변경할 수 있지만 계획 시간 수는 동일하게 유지됩니다.</p> <p>자세한 내용은 <a href="../../../manage-work/tasks/taskdurtn/effort-driven.md" class="MCXref xref">기간 유형 개요: 작업 기반</a>.</p> </td> 
   <td scope="col"> <p>작업에서 지정된 사람이 제거되면 계획된 시간이 증가합니다.</p> <p>작업 시 지정된 사항이 추가되면 계획된 시간이 줄어듭니다. </p> <p>기간 은 담당자 수나 일정 변경에 관계없이 변경되지 않습니다. </p> <p>기간은 계획 시간과 같습니다. 계획 기간은 계획 시간 을 지정자 수로 나눈 시간과 같습니다.</p> </td> 
  </tr> 
  <tr> 
   <th scope="col"> <p><strong>단순</strong> </p> </th> 
   <td scope="col"> <p>각 할당자가 할당된 시간을 기준으로 계획 시간 및 기간(이 기간 유형에 대해 동일함)을 결정합니다. </p> <p>Workfront은 각 할당자에 대해 계획된 할당 시간을 추가하여 계획 시간을 계산합니다. </p> <p>각 할당자가 할당되는 시간, 계획 시간 수 및 지속 시간 양이 그에 따라 변경되는 시간을 수동으로 변경할 수 있습니다. 모든 할당자에 대해 할당된 총 시간 수를 선택하는 경우 해당 수는 각 할당자 간에 균등하게 분할됩니다.</p> <p>자세한 내용은 <a href="../../../manage-work/tasks/taskdurtn/simple-duration-type.md" class="MCXref xref">기간 유형 개요: 단순</a>.</p> </td> 
   <td scope="col"> <p>할당된 총 시간 수를 선택하면 할당자 간에 시간이 균등하게 분배됩니다. 그러나 프로젝트 관리자는 각 할당자에 대한 시간을 수동으로 조정할 수 있습니다. </p> <p>단순 기간 유형 인라인 또는 작업 레벨에서 태스크의 계획 시간 및 기간을 편집할 수 있습니다. </p> <p>애자일 팀이 작업에 지정된 경우 기간 유형은 자동으로 단순 로 설정되며 변경할 수 없습니다. 애자일 팀의 작업 기간은 0분보다 커야 합니다.</p> </td> 
  </tr> 
 </tbody> 
</table>

## 새 작업의 기간 유형

새 작업의 기간 유형은 시스템에 설정된 기간 유형과 일치합니다. 기본 기간 유형은 계산된 할당입니다. Workfront 관리자나 그룹 관리자는 시스템 또는 프로젝트와 관련된 그룹의 기본 기간 유형을 업데이트할 수 있습니다. 자세한 내용은 [시스템 전체 작업 및 문제 환경 설정 구성](../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-task-issue-preferences.md).

## 작업의 기간 유형 변경

작업의 기간 유형 변경에 대한 자세한 내용은 [작업의 기간 유형 업데이트](../../../manage-work/tasks/taskdurtn/update-duration-type-of-task.md).
