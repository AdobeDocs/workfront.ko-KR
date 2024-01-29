---
title: 향상된 분석에서 리소스 용량 시각화 보기
content-type: overview
product-area: enhanced-analytics
navigation-topic: enhanced-analytics-navigation-topic
description: Adobe Workfront에서 향상된 분석 리소스 용량 시각화 차트를 볼 때 팀이 용량 초과, 부족 또는 부족 상태인지를 평가할 수 있습니다.
author: Nolan
feature: Reports and Dashboards
exl-id: 5bb45ef6-9e49-4063-8e53-c9f3bc994870
source-git-commit: d9a8af627c8d3da4a7625cd5180bfca69da43b3d
workflow-type: tm+mt
source-wordcount: '844'
ht-degree: 1%

---

# 향상된 분석에서 리소스 용량 시각화 보기

<!--Audited: 01/2024-->

Adobe Workfront에서 향상된 분석 리소스 용량 시각화 차트를 볼 때 팀이 용량 초과, 부족 또는 부족 상태인지를 평가할 수 있습니다.

리소스 시각화에 표시된 팀은 지정된 기간 동안 작업에 할당된 사용자의 홈 팀을 나타냅니다.

## 액세스 요구 사항

다음 항목이 있어야 합니다.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>Adobe Workfront 플랜</a>*</td> 
   <td> <p>현재: 비즈니스 이상</p>
   또는
   <p>새로 만들기: 모두</p>
    </td> 
  </tr> 
  <tr> 
   <td>Adobe Workfront 라이센스*</td> 
   <td> <p>현재: 검토 이상</p>
   또는
   <p>새로운 기능: 표준</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">액세스 수준 구성</td> 
   <td> <p>프로젝트에 대한 액세스 보기</p></td> 
  </tr> 
  <tr> 
   <td role="rowheader">개체 권한</td> 
   <td> <p>프로젝트에 대한 권한 보기</p>  </td> 
  </tr> 
 </tbody> 
</table>

*보유 중인 플랜, 라이선스 유형 또는 액세스 권한을 확인하려면 Workfront 관리자에게 문의하십시오. 자세한 내용은 [Workfront 설명서의 액세스 요구 사항](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

## 전제 조건

Enhanced Analytics를 사용하기 위한 사전 요구 사항은 의 &quot;사전 요구 사항&quot; 섹션을 참조하십시오. [향상된 분석 개요](../enhanced-analytics/enhanced-analytics-overview.md).

## 리소스 용량 시각화 이해

리소스 수용작업량 시각화는 팀이 수용작업량 초과, 미만 또는 초과인지 여부를 보여 줍니다. 이 계산은 다음을 기반으로 합니다.

* **가용 용량**: 필터링된 기간 동안 홈 팀이 작업할 수 있는 총 시간입니다.

  >[!NOTE]
  >
  >향후 기간을 고려하는 경우 가용 용량은 지난 7일 동안의 팀 용량을 기준으로 계산됩니다. 이러한 이유로 스케줄링된 유급휴가는 고려되지 않습니다.

* **계획된 수용작업량**: 필터링된 기간 내에 홈 팀에서 예상되는 총 작업 시간

홈 팀의 계획된 시간과 실제 계획된 시간을 비교하면 홈 팀에 충분한 작업을 할당하지 않고 있는지 또는 과중한 업무로 인한 소진이 있는지 여부를 확인하는 데 도움이 될 수 있습니다.

![](assets/resource-capacity-350x110.png)

자원 능력 시각화에서 다음 상세내역을 볼 수 있습니다.

* **계획된 수용작업량**: 홈 팀 이름과 인라인으로, 파란색 원은 홈 팀에 할당된 계획 시간을 나타냅니다.

  ![](assets/resource-capacity-blue-circle.png)

* **실제 수용작업량**: 홈 팀 이름과 인라인인 수직선은 홈 팀이 사용할 수 있는 시간을 나타냅니다.

  ![](assets/resource-capacity-vertical-line.png)

* **수용작업량 초과**: 수평선과 파란색 원이 수직선 오른쪽에 표시되면 홈 팀에는 사용 가능한 시간 수에 완료할 수 있는 작업보다 더 많은 작업이 할당되었습니다. 이는 팀이 필터링된 기간 동안 수용작업량을 초과할 수 있음을 의미합니다. 팀이 완료하는 데 필요한 나머지 시간이 파란색 원 오른쪽에 표시됩니다.

  ![](assets/resource-capacity-over-capacity.png)

* **수용작업량 이하**: 수직선 왼쪽에 수평선과 파란색 원이 표시되면 홈 팀은 할당된 계획된 작업 시간보다 사용 가능한 시간이 더 많습니다. 이는 팀이 필터링된 기간 동안 능력이 부족할 수 있음을 의미합니다. 홈 팀이 작업을 완료하는 데 사용할 수 있는 추가 시간이 파란색 원 왼쪽에 표시됩니다.

  ![](assets/resource-capacity-under-capacity.png)

팀의 행 위로 마우스를 가져가면 홈 팀이 용량을 초과하거나 미만인 시간 수뿐만 아니라 계획된 용량 및 사용 가능한 용량에 대한 정확한 시간 수를 볼 수 있습니다.

이 정보를 보면 다음을 확인할 수 있습니다.

* 팀이 초과 할당되거나 과소 할당된 경우.
* 가장 큰 프로젝트는 홈팀이 집중하는 프로젝트다.
* 일할 수 있는 팀은 어디입니까?

이 시각화에 대한 최상의 데이터를 얻는 방법에 대해 알아보려면 다음을 참조하십시오. [향상된 분석 개요](../enhanced-analytics/enhanced-analytics-overview.md).

## 리소스 수용작업량 시각화 보기

{{step1-to-analytics}}

1. 왼쪽 패널에서 을 선택합니다 **사람**.

   ![](assets/people-area-cropped-qs-350x276.png)

1. (선택 사항) 다른 날짜 범위를 사용하려면 차트의 오른쪽 위 모서리에 있는 날짜 범위 필터에서 새 시작 날짜와 종료 날짜를 선택합니다.

   ![](assets/filters-select-date-range-350x344.png)

   날짜 범위 필터 사용에 대한 자세한 내용은 [향상된 분석에서 필터 적용](../enhanced-analytics/use-enhanced-analytics-filters.md).

1. (조건부) 팀 필터를 설정하지 않은 경우 팀 필터를 추가하고 데이터를 보려는 각 팀을 선택합니다.

   향상된 분석에서 필터를 추가하는 방법에 대한 자세한 내용은 [향상된 분석에서 필터 적용](../enhanced-analytics/use-enhanced-analytics-filters.md).

   필터를 추가하면 최대 50개의 프로젝트에 대한 데이터가 표시되고 페이지를 떠나거나 Workfront에서 로그아웃한 후에도 필터가 활성 상태로 유지됩니다.

1. (선택 사항) 날짜 범위를 확대하려면 날짜 범위 시작에 대한 시각화의 한 지점을 선택하고 날짜 범위의 끝으로 드래그합니다.

   다른 모든 시각화는 동일한 날짜 범위로 업데이트되며 일정 필터가 만들어집니다.

   ![](assets/timeframe-filter-350x220.png)

1. 홈 팀 라인 위로 마우스를 가져가면 다음을 볼 수 있습니다.

   * 몇 시간 동안 예약할 수 있습니까
   * 홈 팀이 완료하기 위해 계획된 시간입니다.
   * 작업한 총 시간 수. 총 작업 시간 수에 다음 레이블이 있을 수 있습니다.

      * 초과
      * 아래
      * 최대 수용작업입니다.

   ![](assets/resource-capacity-capacity-pop-up-350x213.png)

1. (선택 사항) 시각화 데이터를 내보내려면 **내보내기 아이콘** ![](assets/export.png) 시각화의 오른쪽 상단 모서리에서 내보내기 형식을 선택합니다.

   * **차트(PNG)**
   * **데이터 테이블(XSLX)**

1. 팀 수용작업량 시각화에서 자세한 정보를 보려면 홈 팀 이름을 클릭하십시오.

   팀 수용작업량 시각화에 대한 자세한 내용은 [향상된 분석에서 팀 용량 시각화 보기](../enhanced-analytics/team-capacity-overview.md).


