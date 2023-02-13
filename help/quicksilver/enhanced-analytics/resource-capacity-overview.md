---
title: Enhanced Analytics에서 리소스 용량 시각화 보기
content-type: overview
product-area: enhanced-analytics
navigation-topic: enhanced-analytics-navigation-topic
description: 자원 능력 시각화는 팀이 끝났는지, 아래에 있는지, 아니면 능력인지 보여줍니다. 이 계산은 - EDIT ME를 기반으로 합니다.
author: Nolan
feature: Reports and Dashboards
exl-id: 5bb45ef6-9e49-4063-8e53-c9f3bc994870
source-git-commit: 1b1f3c22b8112cfde5b10bef39076eed11630d0f
workflow-type: tm+mt
source-wordcount: '833'
ht-degree: 0%

---

# Enhanced Analytics에서 리소스 용량 시각화 보기

자원 능력 시각화는 팀이 끝났는지, 아래에 있는지, 아니면 능력인지 보여줍니다.

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
   <td> <p>프로젝트에 대한 액세스 보기</p> <p>참고: 여전히 액세스 권한이 없는 경우 Workfront 관리자에게 액세스 수준에서 추가 제한 사항을 설정하는지 문의하십시오.<br>Workfront 관리자가 액세스 수준을 변경하는 방법에 대한 자세한 내용은 <a href="../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">사용자 정의 액세스 수준 만들기 또는 수정</a>.</p> </td> 
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

## 자원 능력 시각화 이해

자원 능력 시각화는 팀이 끝났는지, 아래에 있는지, 아니면 능력인지 보여줍니다. 이 계산은 다음을 기반으로 합니다.

* **가용 용량**: 홈 팀이 필터링된 기간 동안 작업할 수 있는 총 시간

   >[!NOTE]
   >
   >미래 기간을 보고 있는 경우 가용 용량은 지난 7일 동안의 팀 능력에 따라 계산됩니다. 이러한 이유로 예정된 PTO는 고려되지 않습니다.

* **계획 용량**: 필터링된 기간 동안 홈 팀에서 예상되는 총 계획된 작업 시간

홈 팀의 계획된 시간과 실제 예약된 시간을 비교한 결과, 홈 팀에 충분한 작업을 할당하지 않고 있거나 과중한 작업 로드로 인해 과로로 인한 과열로 인한 과열로 인한 문제가 발생할 수 있는지 확인할 수 있습니다.

![](assets/resource-capacity-350x110.png)

자원 능력 시각화에서 다음 세부 정보를 볼 수 있습니다.

* **계획 용량**: 홈 팀 이름이 있는 인라인으로 파란색 원은 홈 팀에 할당된 계획 시간 수를 나타냅니다.

   ![](assets/resource-capacity-blue-circle.png)

* **실제 용량**: 홈 팀 이름이 있는 인라인으로, 수직 줄은 홈 팀이 사용할 수 있는 시간 수를 나타냅니다.

   ![](assets/resource-capacity-vertical-line.png)

* **용량 초과**: 수직 라인 오른쪽에 수평선과 파란색 원이 표시되면 홈 팀은 사용 가능한 시간 수에 비해 더 많은 작업을 할당받았습니다. 즉, 팀이 필터링된 기간 동안 용량을 초과할 수 있습니다. 팀이 완료해야 하는 나머지 시간(시간)은 파란색 원의 오른쪽에 표시됩니다.

   ![](assets/resource-capacity-over-capacity.png)

* **용량 부족**: 수직 라인 왼쪽에 수평선과 파란색 원이 표시되면 홈 팀은 할당된 작업 시간 수보다 사용 가능한 시간이 많습니다. 즉, 필터링된 기간 동안 팀의 용량이 부족할 수 있습니다. 홈 팀이 작업을 완료하는 데 사용할 수 있는 추가 시간 수가 파란색 원의 왼쪽에 표시됩니다.

   ![](assets/resource-capacity-under-capacity.png)

행 위로 마우스를 가져가면 계획 용량 및 가용 능력에 대한 정확한 시간과 홈 팀이 초과 또는 미완료 시간에 대한 수가 표시됩니다.

다음 정보를 확인하면 다음을 결정하는 데 도움이 됩니다.

* 홈 팀이 초과 할당되었거나 덜 할당된 경우.
* 가장 큰 프로젝트는 홈팀이 집중했던 것이었습니다.
* 어떤 홈팀이 일할 수 있나요?

이 시각화에 대한 최상의 데이터를 가져오는 방법에 대해 알아보려면 [향상된 분석 개요](../enhanced-analytics/enhanced-analytics-overview.md).

## 리소스 용량 시각화 보기

1. Main Menu 아이콘을 클릭합니다. ![](assets/main-menu-icon-16x12.png)를 선택하고 을 선택합니다. **Analytics**.
1. 왼쪽 패널에서 을 선택합니다 **사람**.

   ![](assets/people-area-cropped-qs-350x276.png)

1. (선택 사항) 다른 날짜 범위를 사용하려면 날짜 범위 필터에서 새 시작 날짜와 종료 날짜를 선택합니다.

   ![](assets/filters-select-date-range-350x344.png)

   날짜 범위 필터 사용에 대한 자세한 내용은 [고급 분석에서 필터 적용](../enhanced-analytics/use-enhanced-analytics-filters.md).

1. (조건부) 팀 필터를 설정하지 않은 경우 팀 필터를 추가하고 데이터를 볼 각 팀을 선택합니다.

   Enhanced Analytics에서 필터 추가에 대한 자세한 내용은 [고급 분석에서 필터 적용](../enhanced-analytics/use-enhanced-analytics-filters.md).

   필터를 추가하면 페이지를 나가거나 Workfront에서 로그아웃한 후에도 최대 50개의 프로젝트에 대한 데이터가 표시되고 필터가 활성 상태로 유지됩니다.

1. (선택 사항) 날짜 범위를 확대하려면 날짜 범위 시작에 대한 시각화에서 점을 선택하고 날짜 범위의 끝으로 드래그합니다.

   다른 모든 시각화는 동일한 날짜 범위 및 시간대 필터로 업데이트됩니다.

   ![](assets/timeframe-filter-350x220.png)

1. 홈 팀 라인 위로 마우스를 가져가면 계속 예약할 수 있는 시간, 홈 팀이 완료할 수 있도록 계획된 시간, 완료된 것으로 표시된 총 작업 시간(작업 시간)을 확인할 수 있습니다.

   ![](assets/resource-capacity-capacity-pop-up-350x213.png)

1. (선택 사항) 시각화 데이터를 내보내려면 **내보내기 아이콘** ![](assets/export.png) 시각화의 오른쪽 상단 모서리에서 내보내기 형식을 선택합니다.

   * **차트(PNG)**
   * **데이터 테이블(XSLX)**

1. 팀 용량 시각화에서 자세한 내용을 보려면 홈 팀 이름을 클릭합니다.

   팀 용량 시각화에 대한 자세한 내용은 [Enhanced Analytics에서 팀 용량 시각화 보기](../enhanced-analytics/team-capacity-overview.md).


