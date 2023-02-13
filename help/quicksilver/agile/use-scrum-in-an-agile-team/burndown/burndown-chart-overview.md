---
content-type: overview
product-area: agile-and-teams
navigation-topic: burndown
title: Agile Burndown 차트 개요
description: 번다운 차트는 반복이나 프로젝트를 통해 이야기가 어떻게 진행되는지에 대한 시각적 표현을 제공합니다. 실제 번다운 비율은 반복 또는 프로젝트 타임라인에 대한 이상적인 번다운 비율에 따라 측정됩니다.
author: Lisa
feature: Agile
exl-id: 414e3315-35ed-4aa4-a2d8-be42ec585f29
source-git-commit: 373f2522b85196d6395f189ae6cfe03449cac61a
workflow-type: tm+mt
source-wordcount: '936'
ht-degree: 0%

---

# Agile Burndown 차트 개요

번다운 차트는 반복을 통해 이야기가 어떻게 진행되는지에 대한 시각적 표현을 제공합니다. 실제 번다운 비율은 이터레이션 타임라인에 대한 이상적인 번다운 비율에 따라 측정됩니다.

번다운 차트는 선택한 날짜에 따라 조정됩니다. 기본값은 현재 날짜입니다. 이전 날짜를 선택하면 번다운 차트의 모든 데이터와 의 모든 값이 [!UICONTROL 완료 상태] 번다운 차트 위의 섹션은 선택한 날의 끝에 있는 데이터를 나타내도록 다시 계산됩니다. 지난 일 또는 현재 일을 선택할 수 있습니다. 미래에는 일을 선택할 수 없습니다.)

![](assets/agile-iteration-burndown-350x88.png)

## 시각적 표시기

번다운 차트에는 다음과 같은 시각적 표시기가 포함되어 있습니다.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <img src="assets/agile-iteration-burndown-dottedblue.png" alt=""> </td> 
   <td> <p>반복 시작 시점을 기준으로 하는 최적의 번다운 속도입니다.</p> <p>반복의 범위가 변경되지 않고(시간 또는 점이 추가 또는 제거되지 않음) 이 선은 표시되지 않습니다.</p> <p>이 선은 쉬는 날 작업이 완료되면 평탄하게 표시됩니다. 자세한 내용은 <a title="Agile Burndown 차트 사용" href="#how-days-off-affect-the-burndown-chart" class="MCXref xref">휴가 일수가 번다운 차트에 미치는 영향</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <img src="assets/agile-iteration-burndown-solidblue.png" alt=""> </td> 
   <td> <p>현재 스토리나 작업에 따라 최적의 번다운 속도</p> <p>현재 이상적인 번다운 속도(단색 파란색 선)는 반복이 시작된 후 반복에서 시간 또는 점을 추가하거나 제거할 때 원래의 이상적인 번다운 속도(점선 파란색 선)와 다릅니다.</p> <p>이 선은 쉬는 날 작업이 완료되면 평탄하게 표시됩니다.</p> <p>자세한 내용은 <a title="Agile Burndown 차트 사용" href="#how-days-off-affect-the-burndown-chart" class="MCXref xref">휴가 일수가 번다운 차트에 미치는 영향</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <img src="assets/agile-iteration-burndown-red.png" alt=""> </td> 
   <td> <p>실제 번다운 비율은 번다운 비율이 이상적인 값보다 작으면 빨간색으로 표시됩니다(이상적인 번다운 계산보다 일당 남아 있는 포인트 또는 시간 초과).</p> <p>다음 공식은 실제 번다운 비율을 계산하는 데 사용됩니다.</p> <p>[SUM(진행 중인 작업의 지점 또는 시간 값 * 완료율) + 완료된 작업의 지점 또는 시간 값]</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <img src="assets/agile-iteration-burndown-green.png" alt=""> </td> 
   <td> <p>실제 번다운 비율은 번다운 비율이 이상보다 크거나 같으면 녹색으로 표시됩니다(이상적인 번다운 계산보다 1일 잔존 포인트 또는 더 적음).</p> <p>다음 공식은 실제 번다운 비율을 계산하는 데 사용됩니다.</p> <p>[SUM(진행 중인 작업의 지점 또는 시간 값 * 완료율) + 완료된 작업의 지점 또는 시간 값]</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <img src="assets/agile-iteration-burndown-scope.png" alt=""> </td> 
   <td> <p>범위 변경(시간 또는 지점이 반복에서 추가 또는 제거됨).</p> <p>범위 변경 사항은 항상 중간 부분에 세로 라인으로 표시됩니다. 또한 범위 변경이 발생한 하루 중 중간에 파란색 점이 표시됩니다.</p> <p>번다운 차트의 세로 축은 스토리 포인트 또는 시간을 보여줍니다.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <img src="assets/agile-iteration-burndown-scope.png" alt=""> </td> 
   <td> <p>날짜 범위 변경(반복 기간이 증가 또는 감소).</p> <p>반복 기간이 변경된 날짜 중간에 파란색 점이 표시됩니다.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <img src="assets/agile-iteration-burndown-scope.png" alt=""> </td> 
   <td> <p>작업이 중단되는 시간 동안 실제 번망률에 녹색 또는 빨간색 점이 표시됩니다. (그 날 실제 번다운률이 빨간색이면 점은 빨간색이다. 그 날 실제 번다운 속도가 녹색이면 점은 녹색입니다.)</p> <p>다음 중 하나가 발생하면 작업이 중단됩니다.</p> 
    <ul> 
     <li> [!UICONTROL Percent Complete]가 스토리에 대해 증가합니다.<br>다음과 같은 경우 [!UICONTROL 완료 비율]이 증가합니다. 
      <ul> 
       <li> <p>수동으로 변경됨</p> </li> 
       <li> <p>스토리에 대한 점수나 시간 수가 업데이트됩니다</p> </li> 
      </ul></li>  
     <li>스토리의 상태가 [!UICONTROL 완료]로 변경되었습니다.</li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

## 휴가 일수가 번다운 차트에 미치는 영향 {#how-days-off-affect-the-burndown-chart}

에 정의된 기본 일정 [!DNL Workfront] 번다운에서 휴가(주말 및 휴일)를 제외하여 번다운 차트에 영향을 줍니다. 번다운 차트는 기본 스케줄을 사용하여 작업 일수를 정의합니다(에 설명된 대로).  [예약 만들기](../../../administration-and-setup/set-up-workfront/configure-timesheets-schedules/create-schedules.md)).

기사에서 설명한 대로 대체 일정을 정의하여 팀별 비근무 일수를 통합할 수 있습니다 [번다운 차트에 대체 팀 스케줄 사용](../../../agile/use-scrum-in-an-agile-team/burndown/use-alt--team-schedule-burndown-charts.md)). 그런 다음 이 대체 스케줄은 팀에 할당된 모든 반복의 번다운 차트에 반영됩니다. 대체 스케줄은 번다운 차트에만 영향을 줍니다.

휴가 일수는 다음의 경우에만 번다운 차트에 반영됩니다.

* 이전에 쉬는 날에 작업이 기록되었습니다. (작업이 기록된 날이 표시됩니다.)

   휴일에 작업이 기록되는 경우:

   * 팀이 작업을 하도록 예약되어 있지 않으므로 이상적인 번다운을 계산할 때 로그된 작업이 포함되지 않습니다.
   * 작업이 수행된 하루 또는 번다운 차트를 보고 있는 날(휴일에 보고 있는 경우), 번다운 차트에 평탄한 상태로 표시되는 이상적인 번다운 선(단색 파란색 선 및 파선 파란색 선)이 표시됩니다.
   * 예상 완료 및 일별 평균 포인트 또는 시간과 같은 기타 번다운 통계를 계산할 때 기록된 작업이 포함됩니다.

* 휴일에 번다운 차트를 보고 계십니다. 보고 있는 날이 번다운 차트에 표시됩니다.
* 휴일에 반복에 대한 나머지 작업의 전체 작업을 완료합니다.

   사용자가 하루 쉬는 시간에 반복에 대해 남은 전체 작업을 완료하면 [!UICONTROL 예상 완료] 필드는 이터레이션이 완료된 날짜를 표시합니다.

   이터레이션을 계획할 때 비작업일에 대한 반복 종료 날짜를 설정하고 이터레이션이 시간에 따라 완료되도록 추적되는 경우 [!UICONTROL 예상 완료] 사용자가 설정한 반복 종료 날짜 이전의 마지막 작업 날짜에 대해 날짜가 설정됩니다(작업 시간이 비근무 일에 대해 연소되도록 예약되지 않기 때문).

   문서에 설명된 대로 반복을 계획할 때 이터레이션의 종료 날짜가 지정됩니다 [반복 만들기](../../../agile/use-scrum-in-an-agile-team/iterations/create-an-iteration.md).
