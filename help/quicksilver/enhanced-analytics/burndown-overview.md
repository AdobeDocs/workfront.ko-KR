---
title: Enhanced Analytics에서 Burndown 시각화 보기
content-type: overview
product-area: enhanced-analytics
navigation-topic: enhanced-analytics-navigation-topic
description: Burndown 시각화는 시간에 따른 특정 프로젝트의 번다운을 보여주며 프로젝트 조건, 속도 및 남은 시간(일) 간의 관계를 이해하는 데 도움이 됩니다.
author: Nolan
feature: Reports and Dashboards
exl-id: e67c92d5-b309-406b-b6f0-4d414d0e7dcc
source-git-commit: d337008d4fca8c41b98b10f9059ec1cc379811e1
workflow-type: tm+mt
source-wordcount: '797'
ht-degree: 0%

---

# Enhanced Analytics에서 Burndown 시각화 보기

Burndown 시각화는 시간에 따른 특정 프로젝트의 번다운을 보여주며 프로젝트 조건, 속도 및 남은 시간(일) 간의 관계를 이해하는 데 도움이 됩니다.

![](assets/burndown-350x112.png)

## 액세스 요구 사항

다음 항목이 있어야 합니다.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"><a href="https://www.workfront.com/plans" target="_blank">Adobe Workfront 플랜</a>*</td> 
   <td> <p>비즈니스 이상</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><a href="../administration-and-setup/add-users/access-levels-and-object-permissions/wf-licenses.md" class="MCXref xref">Adobe Workfront 라이선스 개요</a>*</td> 
   <td> <p>검토 이상</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">액세스 수준 구성*</td> 
   <td> <p>프로젝트에 대한 액세스 보기</p> <p>참고: 여전히 액세스 권한이 없는 경우 Workfront 관리자에게 액세스 수준에서 추가 제한 사항을 설정하는지 문의하십시오.<br>Workfront 관리자가 액세스 수준을 수정하는 방법에 대한 자세한 내용은 <a href="../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">사용자 정의 액세스 수준 만들기 또는 수정</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">개체 권한</td> 
   <td> <p>보기</p> <p>추가 액세스 요청에 대한 자세한 내용은 <a href="../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">개체에 대한 액세스 요청 </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;어떤 계획, 라이선스 유형 또는 액세스 권한을 보유하고 있는지 알아보려면 Workfront 관리자에게 문의하십시오.

## 전제 조건

Enhanced Analytics를 사용하기 위한 사전 요구 사항에 대해서는 [향상된 분석 개요](../enhanced-analytics/enhanced-analytics-overview.md).

## Burndown 시각화 이해

솔리드 파란색 선은 시작 날짜부터 계획된 완료 일자까지의 계획 속도를 보여줍니다. 이 선은 작업이 추가, 제거 또는 업데이트될 때 조정되며 프로젝트가 계획된 완료 날짜에 도달하면 파선 수직 라인으로 변경됩니다.

![](assets/burndown-planned-line.png)

실제 줄은 시간에 따라 프로젝트에서 보낸 시간(또는 일)을 보여줍니다. 이 선의 색상은 매일 프로젝트의 조건을 나타냅니다.

* **녹색**: 프로젝트가 타겟에 있습니다.

   ![](assets/burndown-green.png)

* **주황**: 그 프로젝트는 위험에 처해 있다.

   ![](assets/burndown-orange.png)

* **빨간색**: 그 프로젝트는 곤경에 처해 있다.

   ![](assets/burndown-red.png)

이러한 프로젝트 조건에 대한 자세한 내용은 [프로젝트 조건 및 조건 유형 개요](../manage-work/projects/manage-projects/project-condition-and-condition-type.md).

실제 줄이 상하로 이동하면 프로젝트에 작업이 추가되었습니다. 줄이 세로로 이동되면 프로젝트에 대한 작업이 제거되거나 완료되었습니다.

시각화의 x축 아래에서 지정된 날(추가된 금액, 완료된 금액 및 두 시간 사이의 차이점)에서 작업 및 시간(또는 일)이 변경되는 방법에 대한 자세한 정보를 볼 수 있습니다.

Burndown 시각화에서 이 모든 정보를 보면 다음을 결정하는 데 도움이 됩니다.

* 시간에 따른 개별 프로젝트의 상태
* 문제 발생(또는 계획되지 않은 작업)이 계획된 작업에 어떻게 영향을 주는지 설명합니다.
* 원래 완료 날짜 이후에 프로젝트를 확장한 이벤트입니다.

이 시각화에 대한 최상의 데이터를 가져오는 방법에 대해 알아보려면 [향상된 분석 개요](../enhanced-analytics/enhanced-analytics-overview.md).

## Burndown 시각화 보기

1. Main Menu 아이콘을 클릭합니다. ![](assets/main-menu-icon-16x12.png)를 선택하고 을 선택합니다. **Analytics**.
1. (선택 사항) 다른 날짜 범위를 사용하려면 날짜 범위 필터에서 새 시작 날짜와 종료 날짜를 선택합니다.

   ![](assets/filters-select-date-range-350x344.png)

   날짜 범위 필터 사용에 대한 자세한 내용은 [고급 분석에서 필터 적용](../enhanced-analytics/use-enhanced-analytics-filters.md).

1. (조건부) 프로젝트 데이터 세트를 제한해야 하는 경우 사용할 필터를 선택하고 적용합니다.

   Enhanced Analytics에서 필터 추가에 대한 자세한 내용은 [고급 분석에서 필터 적용](../enhanced-analytics/use-enhanced-analytics-filters.md).

   필터를 추가하면 페이지를 나가거나 Workfront에서 로그아웃한 후에도 최대 50개의 프로젝트에 대한 데이터가 표시되고 필터가 활성 상태로 유지됩니다.

1. (선택 사항) 날짜 범위를 확대하려면 날짜 범위 시작에 대한 시각화에서 점을 선택하고 날짜 범위의 끝으로 드래그합니다.

   다른 모든 시각화는 동일한 날짜 범위 및 시간대 필터로 업데이트됩니다.

   ![](assets/timeframe-filter-350x220.png)

1. 플라이트 계획 또는 프로젝트 트리맵 시각화에서 프로젝트를 클릭하여 자세한 정보를 확인합니다.

   플라이트 시각화의 번다운 및 작업이 표시됩니다.

   >[!NOTE]
   >
   >이러한 다른 시각화에 대해 자세히 알려면 다음을 참조하십시오.
   >
   >   
   >   
   >   * [Enhanced Analytics에서 플라이트 계획 시각화 보기](../enhanced-analytics/flight-plan-overview.md)
   >   * [Enhanced Analytics에서 프로젝트 트리맵 시각화 보기](../enhanced-analytics/project-treemap-overview.md)
   >   * [Enhanced Analytics에서 플라이트 시각화의 작업 보기](../enhanced-analytics/tasks-in-flight-overview.md)


1. (선택 사항) 보기를 계획 시간에서 로 변경합니다. **기간**.

   기본적으로 계획 시간이 선택됩니다.

   >[!NOTE]
   >
   >선택 **기간** 모든 시간 정보를 일로 변경합니다.\
   >![](assets/duration-burndown-350x112.png)\
   >Enhanced Analytics 영역의 지속 시간에 대한 자세한 내용은 [향상된 분석 개요](../enhanced-analytics/enhanced-analytics-overview.md).

1. 선 그래프에서 임의의 점을 클릭합니다.

   선택한 날짜에 대한 정확한 날짜가 표시되고 작업 및 시간(또는 일)에 대한 추가 정보가 아래에 표시됩니다.

   ![](assets/burndown-task-and-hour-changes-350x121.png)

   >[!NOTE]
   >
   >실제 속도가 시각화의 x축(0시간 또는 0일이 있는 인라인)을 따라 실행되는 플랫 라인인 경우 계획된 시간(또는 일)이 프로젝트에 추가되지 않았음을 의미합니다.\
   >실제 속도가 작동 중지되지 않는 x축(시간 또는 일 수가 있는 인라인)의 위 플랫 라인인 경우 필터링된 기간 내에 작업이 완료되지 않았음을 의미합니다.

1. (선택 사항) 시각화 데이터를 내보내려면 **내보내기** 아이콘 ![](assets/export.png)시각화의 오른쪽 상단 모서리에서 내보내기 형식을 선택합니다.

   * **차트(PNG)**
   * **데이터 테이블(XSLX)**

1. (선택 사항) 선택한 프로젝트에서 작업 진행 상황에 대한 세부 사항을 보려면 Burndown 시각화 아래에 나타나는 비행 중 작업 시각화를 보십시오.
