---
title: Enhanced Analytics에서 팀 용량 시각화 보기
content-type: overview
product-area: enhanced-analytics
navigation-topic: enhanced-analytics-navigation-topic
description: 팀 용량 시각화는 홈 팀이 보유한 총 용량, 초과 할당 또는 미할당 여부 및 시간이 지남에 따라 용량이 얼마나 동적이는지를 보여줍니다.
author: Nolan
feature: Reports and Dashboards
exl-id: cfeb1a87-01be-4088-9e33-53a97e3871ad
source-git-commit: 1b1f3c22b8112cfde5b10bef39076eed11630d0f
workflow-type: tm+mt
source-wordcount: '735'
ht-degree: 0%

---

# Enhanced Analytics에서 팀 용량 시각화 보기

팀 용량 시각화는 홈 팀이 보유한 총 용량, 초과 할당 또는 미할당 여부 및 시간이 지남에 따라 용량이 얼마나 동적이는지를 보여줍니다.

![](assets/team-capacity-350x110.png)

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

## 팀 용량 시각화 이해

팀 용량 시각화는 주어진 날에 홈 팀에 할당된 작업의 양을 표시합니다.

* **번아웃**: 짙은 파란색 채우기 색상이 점선 위에 있으면 홈 팀이 작업할 수 있는 시간 내에 완료할 수 있는 시간보다 더 많은 작업 시간이 지정됩니다. 이는 팀이 너무 많이 할당되어 있고 완전히 소모될 수 있음을 나타냅니다.

   ![](assets/team-capacity-over-capacity.png)

* **Uncertified**: 어두운 파란색 채우기 색상이 점선 아래에 있으면 홈 팀이 할당된 작업량보다 더 많은 시간을 사용할 수 있습니다. 이것은 그 팀이 할당량이 부족하고 문제될 수 있음을 나타낸다.

   ![](assets/team-capacity-under-capacity.png)

* **잔액**: 보다 가볍거나 투명한 파란색 채우기 색상이 점선 바로 위, 바로 아래 또는 점선 바로 위에 있으면 홈 팀은 근무 시간이 지정되므로 사용 가능한 근무 시간 내에 완료할 수 있습니다. 이것은 팀의 업무량이 더 균형 잡힌 상태임을 나타냅니다.

   ![](assets/team-capacity-at-capacity.png)

시각화의 특정 지점을 마우스로 가리키면 지정된 날짜에 대해 다음 세부 정보가 표시됩니다.

* **예약된 시간**: 팀이 완료해야 하는 계획된 작업 시간입니다.
* **사용 가능한 시간**: 팀이 일할 수 있는 근무 시간 수입니다.
* **용량**: 용량 퍼센트 외에도 용량, 미달 용량 또는 초과 용량의 지정도 표시됩니다.

다음 정보를 확인하면 다음을 결정하는 데 도움이 됩니다.

* 홈 팀이 초과 할당 또는 덜 할당된 경우
* 홈 팀이 매일 초과 할당되거나 덜 할당된 경우.
* 홈 팀의 작업 로드가 얼마나 일관됩니까?
* 새 작업에 용량 문제를 만드는 경우

이 시각화에 대한 최상의 데이터를 가져오는 방법에 대해 알아보려면 [향상된 분석 개요](../enhanced-analytics/enhanced-analytics-overview.md).

## 팀 용량 시각화 보기

1. Main Menu 아이콘을 클릭합니다. ![](assets/main-menu-icon-16x12.png)를 선택하고 을 선택합니다. **Analytics**.
1. 왼쪽 패널에서 을 선택합니다 **사람**.

   ![](assets/people-area-cropped-qs-350x276.png)

1. (선택 사항) 다른 날짜 범위를 사용하려면 날짜 범위 필터에서 새 시작 날짜와 종료 날짜를 선택합니다.

   ![](assets/filters-select-date-range-350x344.png)

   날짜 범위 필터 사용에 대한 자세한 내용은 [고급 분석에서 필터 적용](../enhanced-analytics/use-enhanced-analytics-filters.md).

1. (조건부) 팀 필터를 설정하지 않은 경우 팀 필터를 추가하고 데이터를 볼 각 팀을 선택합니다.

   Enhanced Analytics에서 필터 추가에 대한 자세한 내용은 [고급 분석에서 필터 적용](../enhanced-analytics/use-enhanced-analytics-filters.md).

   필터를 추가하면 페이지를 나가거나 Workfront에서 로그아웃한 후에도 최대 50개의 프로젝트에 대한 데이터가 표시되고 필터가 활성 상태로 유지됩니다.

1. 리소스 용량 시각화에서 팀을 클릭하여 자세한 내용을 확인합니다.

   팀 용량 시각화가 표시됩니다.

   자원 능력 시각화에 대한 자세한 내용은 다음을 참조하십시오 [Enhanced Analytics에서 리소스 용량 시각화 보기](../enhanced-analytics/resource-capacity-overview.md).

1. (선택 사항) 날짜 범위를 확대하려면 날짜 범위 시작에 대한 시각화에서 점을 선택하고 날짜 범위의 끝으로 드래그합니다.

   다른 모든 시각화는 동일한 날짜 범위 및 시간대 필터로 업데이트됩니다.

   ![](assets/timeframe-filter-350x220.png)

1. 그래프 라인의 한 지점을 마우스로 가리키면 지정된 날짜에 대한 예약된 시간 및 계획 시간, 용량 비율 및 홈 팀이 해당 시점에 종료되었는지, 하인지 또는 용량인지 확인할 수 있습니다.

   ![](assets/team-capacity-capacity-pop-up-350x351.png)

1. (선택 사항) 시각화 데이터를 내보내려면 **내보내기 아이콘** ![](assets/export.png) 시각화의 오른쪽 상단 모서리에서 내보내기 형식을 선택합니다.

   * **차트(PNG)**
   * **데이터 테이블(XSLX)**

