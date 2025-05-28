---
title: 향상된 분석에서 번다운 시각화 보기
content-type: overview
product-area: enhanced-analytics
navigation-topic: enhanced-analytics-navigation-topic
description: 번다운 시각화는 시간 경과에 따른 특정 프로젝트의 번다운을 보여주며 프로젝트 상태, 속도 및 남은 시간(또는 일) 간의 관계를 이해하는 데 도움이 됩니다.
author: Nolan
feature: Reports and Dashboards
exl-id: e67c92d5-b309-406b-b6f0-4d414d0e7dcc
source-git-commit: 2a6e767036ae702f6c19dc71cdb11dae8e9e37ea
workflow-type: tm+mt
source-wordcount: '834'
ht-degree: 0%

---

# 향상된 분석에서 번다운 시각화 보기

>[!IMPORTANT]
>
>향상된 Analytics가 5월 27일에 Workfront에서 제거되었습니다. Workfront Data Connect는 새로운 대체 솔루션이며 현재 사용하는 향상된 Analytics 시각화를 복제하는 데 사용할 수 있습니다. <br>자세한 내용은 [향상된 Analytics 사용 중단](/help/quicksilver/product-announcements/announcements/enhanced-analytics-deprecation.md) 안내서를 참조하십시오.


<!-- Audited: 12/2023 -->

번다운 시각화는 시간 경과에 따른 특정 프로젝트의 번다운을 보여주며 프로젝트 상태, 속도 및 남은 시간(또는 일) 간의 관계를 이해하는 데 도움이 됩니다.

![향상된 분석 번다운 예](assets/burndown120623.png)

## 액세스 요구 사항

이 문서의 단계를 수행하려면 다음 액세스 권한이 있어야 합니다.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront 플랜</td> 
   <td>
      <p>새로 만들기: 모두</p>
      <p>또는</p>
      <p>현재: 비즈니스 이상</p></td>
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront 라이선스</td> 
   <td>
      <p>새로운 기능: 밝게 또는 높음</p>
      <p>또는</p>
      <p>현재: 검토 이상</p>
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader">액세스 수준 구성</td> 
   <td> <p>프로젝트에 대한 액세스 보기</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">개체 권한</td> 
   <td> <p>보기</p> </td>
  </tr> 
 </tbody> 
</table>

이 표의 정보에 대한 자세한 내용은 [Workfront 설명서의 액세스 요구 사항](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)을 참조하십시오.

## 전제 조건

향상된 Analytics를 사용하기 위한 전제 조건은 [향상된 Analytics 개요](../enhanced-analytics/enhanced-analytics-overview.md)의 &quot;전제 조건&quot; 섹션을 참조하십시오.

## 번다운 시각화 이해

파란색 실선은 시작 일자부터 계획된 완료 일자까지의 계획된 속도를 보여줍니다. 이 선은 작업이 추가, 제거 또는 업데이트될 때 조정되며 프로젝트가 계획된 완료 날짜에 도달하면 파선 세로선으로 변경됩니다.

![계획된 속도](assets/burndown-planned-line.png)

실제 행에는 프로젝트에 소요된 시간(일)이 시간 경과에 따라 표시됩니다. 이 선의 색상은 매일 프로젝트의 상태를 나타냅니다.

* **녹색**: 프로젝트가 대상에 있습니다.

  ![대상](assets/burndown-green.png)

* **주황**: 프로젝트가 위험합니다.

  ![위험 상태](assets/burndown-orange.png)

* **빨강**: 프로젝트에 문제가 있습니다.

  ![문제 발생](assets/burndown-red.png)

이러한 프로젝트 상태에 대한 자세한 내용은 [프로젝트 상태 및 상태 형식 개요](../manage-work/projects/manage-projects/project-condition-and-condition-type.md)를 참조하십시오.

실제 선이 수직으로 위로 이동하면 프로젝트에 작업이 추가되었습니다. 선이 수직으로 아래로 이동하면 프로젝트에 대한 작업이 제거되거나 완료된 것입니다.

시각화의 x축 아래에서는 주어진 일에 작업 및 시간(또는 일)이 변경되는 방법(추가된 금액, 완료된 금액 및 두 기간의 차이)에 대한 자세한 정보를 볼 수 있습니다.

번다운 시각화에서 이러한 모든 정보를 확인하면 다음을 결정하는 데 도움이 됩니다.

* 시간 경과에 따른 개별 프로젝트의 상태
* 문제 발생(또는 계획되지 않은 작업)이 계획된 작업에 미치는 영향
* 원래 완료 일자 이후에 프로젝트를 연장한 이벤트는 무엇입니까?

이 시각화에 가장 적합한 데이터를 얻는 방법에 대해 알아보려면 [향상된 분석 개요](../enhanced-analytics/enhanced-analytics-overview.md)를 참조하십시오.

## 번다운 시각화 보기

{{step1-to-analytics}}

1. (선택 사항) 다른 날짜 범위를 사용하려면 날짜 범위 필터에서 새 시작 날짜와 종료 날짜를 선택합니다.

   ![날짜 선택](assets/filters-select-date-range-350x344.png)

   날짜 범위 필터 사용에 대한 자세한 내용은 [향상된 분석에서 필터 적용](../enhanced-analytics/use-enhanced-analytics-filters.md)을 참조하십시오.

1. (조건부) 프로젝트 데이터 세트를 제한해야 하는 경우 사용할 필터를 선택하고 적용합니다.

   향상된 분석에서 필터를 추가하는 방법에 대한 자세한 내용은 [향상된 분석에서 필터 적용](../enhanced-analytics/use-enhanced-analytics-filters.md)을 참조하십시오.

   필터를 추가하면 최대 50개의 프로젝트에 대한 데이터가 표시되고 페이지를 떠나거나 Workfront에서 로그아웃한 후에도 필터가 활성 상태로 유지됩니다.

1. (선택 사항) 날짜 범위를 확대하려면 날짜 범위의 시작에 대한 시각화의 한 지점을 선택하고 날짜 범위의 끝으로 드래그합니다.

   다른 모든 시각화는 동일한 날짜 범위로 업데이트되고, 일정 필터가 자동으로 만들어집니다.

   ![일정 필터](assets/timeframe-filter-350x220.png)

1. 플라이트 계획 또는 프로젝트 트리맵 시각화에서 프로젝트를 클릭하여 자세한 정보를 봅니다.

   번다운 및 진행 중인 작업 시각화가 표시됩니다.

   >[!NOTE]
   >
   >이러한 다른 시각화에 대한 자세한 내용은 다음을 참조하십시오.
   >
   >   * [향상된 분석에서 플라이트 플랜 시각화 보기](../enhanced-analytics/flight-plan-overview.md)
   >   * [향상된 분석에서 프로젝트 트리맵 시각화 보기](../enhanced-analytics/project-treemap-overview.md)
   >   * [향상된 분석에서 진행 중인 작업 시각화 보기](../enhanced-analytics/tasks-in-flight-overview.md)
   >

1. (선택 사항) 보기를 계획된 시간에서 **지속 시간**(으)로 변경합니다.

   계획된 시간이 기본적으로 선택됩니다.

   >[!NOTE]
   >
   >**지속 시간**&#x200B;을 선택하면 모든 시간 정보가 일로 변경됩니다.\
   >![기간 번다운](assets/duration-burndown-350x112.png)\
   >향상된 분석 영역의 기간에 대한 자세한 내용은 [향상된 분석 개요](../enhanced-analytics/enhanced-analytics-overview.md#duration-view)의 &quot;기간 보기&quot; 섹션을 참조하십시오.

1. 선 그래프의 임의의 점을 클릭합니다.

   정확한 날짜가 표시되고 선택한 날의 작업 및 시간(또는 일)에 대한 추가 정보가 그래프 아래에 표시됩니다.

   ![번다운 세부 정보](assets/burndown-task-and-hour-changes-350x121.png)

   >[!NOTE]
   >
   >실제 속도가 시각화의 x축(0시간 또는 0일로 인라인)을 따라 실행되는 플랫 라인인 경우 프로젝트에 계획된 시간(또는 일)이 추가되지 않았음을 의미합니다.\
   >실제 속도가 x축(시간 또는 일 수로 인라인됨) 위에 절대 내려가지 않는 플랫 라인인 경우 이는 필터링된 기간 내에 작업이 완료되지 않았음을 의미합니다.

1. (선택 사항) 시각화 데이터를 내보내려면 시각화의 오른쪽 상단에 있는 **내보내기** 아이콘 ![내보내기 아이콘](assets/export.png)을 클릭하고 내보내기 형식을 선택합니다.

   * 차트(PNG)
   * 데이터 테이블(XSLX)

1. (선택 사항) 선택한 프로젝트에서 작업의 진행 상황에 대한 세부 정보를 보려면 번다운 시각화 아래에 표시되는 진행 중인 작업 시각화를 참조하십시오. 자세한 내용은 [향상된 분석에서 진행 중인 작업 시각화 보기](/help/quicksilver/enhanced-analytics/tasks-in-flight-overview.md)를 참조하십시오.
