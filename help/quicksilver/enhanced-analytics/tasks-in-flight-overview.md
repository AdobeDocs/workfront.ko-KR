---
title: Enhanced Analytics에서 플라이트 시각화의 작업 보기
content-type: overview
product-area: enhanced-analytics
navigation-topic: enhanced-analytics-navigation-topic
description: 비행 중인 작업 시각화는 프로젝트에 대해 진행 중인 작업(적용된 필터 기준 내)의 수, 각 작업에 대해 완료된 작업의 비율 및 작업 예약 방법을 보여줍니다.
author: Nolan
feature: Reports and Dashboards
exl-id: cc738450-362a-49e8-836f-611fa82057b5
source-git-commit: 1b1f3c22b8112cfde5b10bef39076eed11630d0f
workflow-type: tm+mt
source-wordcount: '717'
ht-degree: 0%

---

# Enhanced Analytics에서 플라이트 시각화의 작업 보기

비행 중인 작업 시각화는 프로젝트에 대해 진행 중인 작업(적용된 필터 기준 내)의 수, 각 작업에 대해 완료된 작업의 비율 및 작업 예약 방법을 보여줍니다.

![](assets/tasks-in-flight-possible-replacement-350x104.png)

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
   <td> <p>프로젝트에 대한 액세스 보기</p> <p>작업에 대한 액세스 보기(작업을 업데이트하려면 작업에 대한 편집 액세스 권한이 필요합니다.)</p> <p>참고: 여전히 액세스 권한이 없는 경우 Workfront 관리자에게 액세스 수준에서 추가 제한 사항을 설정하는지 문의하십시오.<br>Workfront 관리자가 액세스 수준을 수정하는 방법에 대한 자세한 내용은 <a href="../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">사용자 정의 액세스 수준 만들기 또는 수정</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">개체 권한</td> 
   <td> <p>프로젝트 및 작업 개체 모두에 대한 권한 보기</p> <p>추가 액세스 요청에 대한 자세한 내용은 <a href="../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">개체에 대한 액세스 요청 </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;어떤 계획, 라이선스 유형 또는 액세스 권한을 보유하고 있는지 알아보려면 Workfront 관리자에게 문의하십시오.

## 전제 조건

Enhanced Analytics를 사용하기 위한 사전 요구 사항에 대해서는 [향상된 분석 개요](../enhanced-analytics/enhanced-analytics-overview.md).

## 비행 시각화의 작업 이해

플라이트 계획 시각화의 작업 세부 사항은 다음과 같습니다.

* **계획된 작업 기간**: 작업 표시줄의 길이는 작업의 시작 날짜 및 완료 날짜를 기준으로 하는 계획된 기간을 나타냅니다.

   ![](assets/tasks-in-flight-duration-350x80.png)

* **작업 완료**: 작업 표시줄 내의 어두운 파란색 색상은 작업에 대해 완료된 작업의 양을 나타냅니다. 이 완료 백분율이 작업 표시줄의 오른쪽에 표시됩니다.

   ![](assets/tasks-in-flight-dark-blue-350x35.png)

* **남은 작업**: 작업 표시줄 내의 연한 파란색 색상은 작업에 대해 완료해야 하는 작업의 양을 나타냅니다.

   ![](assets/tasks-in-flight-light-blue-350x35.png)

이 정보는 다음을 결정하는 데 도움이 될 수 있습니다.

* 작업 노력이 집중되어 있는 곳.
* 어떤 작업이 프로젝트를 위험에 빠뜨릴 수 있습니다.
* 작업이 완료되는 시점
* 특정 작업에 대해 이야기할 필요가 있는 사람.

이 시각화에 대한 최상의 데이터를 가져오는 방법에 대해 알아보려면 [향상된 분석 개요](../enhanced-analytics/enhanced-analytics-overview.md).

## 플라이트 시각화의 작업 보기

1. Main Menu 아이콘을 클릭합니다. ![](assets/main-menu-icon-16x12.png)를 선택하고 을 선택합니다. **Analytics**.
1. (선택 사항) 다른 날짜 범위를 사용하려면 날짜 범위 필터에서 새 시작 날짜와 종료 날짜를 선택합니다.

   ![](assets/filters-select-date-range-350x344.png)

   날짜 범위 필터 사용에 대한 자세한 내용은 [고급 분석에서 필터 적용](../enhanced-analytics/use-enhanced-analytics-filters.md).

1. (조건부) 프로젝트 데이터 세트를 제한해야 하는 경우 사용할 필터를 선택하고 적용합니다.

   Enhanced Analytics에서 필터 추가에 대한 자세한 내용은 [고급 분석에서 필터 적용](../enhanced-analytics/use-enhanced-analytics-filters.md).

   필터를 추가하면 페이지를 나가거나 Workfront에서 로그아웃한 후에도 최대 50개의 프로젝트에 대한 데이터가 표시되고 필터가 활성 상태로 유지됩니다.

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
   >   * [Enhanced Analytics에서 Burndown 시각화 보기](../enhanced-analytics/burndown-overview.md)


1. (선택 사항) 날짜 범위를 확대하려면 날짜 범위 시작에 대한 시각화에서 점을 선택하고 날짜 범위의 끝으로 드래그합니다.

   다른 모든 시각화는 동일한 날짜 범위 및 시간대 필터로 업데이트됩니다.

   ![](assets/timeframe-filter-350x220.png)

1. (선택 사항) 작업이 정렬되는 방식을 변경하려면 **정렬 기준** 메뉴를 클릭한 다음 새 정렬 옵션을 선택합니다.

   * **완료 일자**
   * **알파벳순 A-Z**
   * **작업 분류 구조** (이 옵션은 작업이 프로젝트에 표시되는 순서와 일치합니다.)

   페이지의 다른 모든 시각화는 정렬 선택과 일치하도록 업데이트됩니다.

1. 선택한 프로젝트에서 작업 진행 상태를 검토한 다음 특정 작업을 마우스로 가리키면 계획 시간 수, 예정 기한 및 완료 비율이 표시됩니다.

   ![](assets/tasks-in-flight-task-details-350x242.png)

1. 작업을 클릭하여 화면 오른쪽에 있는 작업 세부 정보 를 엽니다. 이 화면에서 작업에 대한 자세한 정보를 보거나 업데이트를 입력하거나 작업을 변경할 수 있습니다.

   ![](assets/task-details-qs-350x675.png)

1. (선택 사항) 시각화 데이터를 내보내려면 **내보내기 아이콘** ![](assets/export.png) 시각화의 오른쪽 상단 모서리에서 내보내기 형식을 선택합니다.

   * **차트(PNG)**
   * **데이터 테이블(XSLX)**

