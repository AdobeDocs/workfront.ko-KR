---
title: Enhanced Analytics에서 플라이트 계획 시각화 보기
content-type: overview
product-area: enhanced-analytics
navigation-topic: enhanced-analytics-navigation-topic
description: 비행 계획 시각화는 얼마나 많은 프로젝트(적용된 필터 기준 내)가 비행 중이었는지, 이러한 프로젝트의 수명 동안 어떤 조건이 변경되었는지, 그리고 이러한 프로젝트가 계획된 완료 기한에 얼마나 가깝게 부착되었는지를 보여줍니다.
author: Nolan
feature: Reports and Dashboards
exl-id: c64ed752-151a-40f7-ab18-684e2cd032bc
source-git-commit: 1b1f3c22b8112cfde5b10bef39076eed11630d0f
workflow-type: tm+mt
source-wordcount: '862'
ht-degree: 2%

---

# Enhanced Analytics에서 플라이트 계획 시각화 보기

비행 계획 시각화는 얼마나 많은 프로젝트(적용된 필터 기준 내)가 비행 중이었는지, 이러한 프로젝트의 수명 동안 어떤 조건이 변경되었는지, 그리고 이러한 프로젝트가 계획된 완료 기한에 얼마나 가깝게 부착되었는지를 보여줍니다.

![](assets/flight-plan-350x132.png)

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
   <td> <p>프로젝트에 대한 액세스 권한 보기</p> <p>추가 액세스 요청에 대한 자세한 내용은 <a href="../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">개체에 대한 액세스 요청 </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;어떤 계획, 라이선스 유형 또는 액세스 권한을 보유하고 있는지 알아보려면 Workfront 관리자에게 문의하십시오.

## 전제 조건

Enhanced Analytics를 사용하기 위한 사전 요구 사항에 대해서는 [향상된 분석 개요](../enhanced-analytics/enhanced-analytics-overview.md).

## 플라이트 계획 시각화 이해

프로젝트의 실제 지속 기간에서는 다음 프로젝트 조건만 볼 수 있습니다.

* 대상
* 위험 상태
* 문제 발생

프로젝트 조건에 대해 알아보려면 [프로젝트 조건 및 조건 유형 개요](../manage-work/projects/manage-projects/project-condition-and-condition-type.md).

플라이트 계획 시각화는 다음 프로젝트 세부 사항을 보여줍니다.

* **계획된 기간**: 수평 파란색 선은 프로젝트의 계획된 길이를 나타내고, 선 끝에는 시작 날짜와 종료 날짜를 나타내는 삼각형이 있습니다.

   ![](assets/planned-duration-line-350x37.png)

* **실제 기간**: 계획된 기간 아래의 굵은 색상 선은 프로젝트의 실제 길이를 나타냅니다. 프로젝트 수명 중 해당 특정 시간에 프로젝트의 조건에 따라 라인 색상이 변경됩니다.

   ![](assets/actual-duration-line.png)

* **실제 조건**: 굵고 색상이 지정된 선은 서로 다른 시점에 프로젝트의 상태를 표시합니다. 프로젝트의 조건에 따라 라인 색상이 변경됩니다.

   * **녹색**: Target 시
   * **주황**: 위험
   * **빨간색**: 문제 발생

   ![](assets/actual-condition-color.png)

플라이트 계획 시각화의 프로젝트 행을 마우스로 가리키면 프로젝트의 계획 일정, 현재 프로젝트 조건, 사용자 정의 조건에 대한 정보가 표시됩니다(해당되는 경우). 기간 또는 조건에 영향을 줄 수 있는 사항을 보다 심층적으로 보려면 Enhanced Analytics 영역에서 다른 시각화를 볼 수 있습니다.

다음 정보를 확인하면 다음을 결정하는 데 도움이 됩니다.

* 최초 계획 완료 일자까지 프로젝트를 확장하는 이벤트는 무엇입니까?
* 프로젝트에 문제가 발생하기 시작하면
* 동일한 기간 동안 열려 있는 프로젝트 수입니다.
* 활성 상태인 프로젝트 수입니다.
* 추가 관심이나 지원이 필요한 프로젝트

이 시각화에 가장 적합한 데이터를 가져오는 방법에 대한 자세한 내용은 [향상된 분석 개요](../enhanced-analytics/enhanced-analytics-overview.md).

## 플라이트 계획 시각화 보기

1. 을(를) 클릭합니다. **기본 메뉴** 아이콘 ![](assets/main-menu-icon-16x12.png)를 선택하고 을 선택합니다. **Analytics**.
1. (선택 사항) 다른 날짜 범위를 사용하려면 날짜 범위 필터에서 새 시작 날짜와 종료 날짜를 선택합니다.

   ![](assets/filters-select-date-range-350x344.png)

   날짜 범위 필터 사용에 대한 자세한 내용은 [고급 분석에서 필터 적용](../enhanced-analytics/use-enhanced-analytics-filters.md).

1. (조건부) 프로젝트 데이터 세트를 제한해야 하는 경우 사용할 필터를 선택하고 적용합니다.

   Enhanced Analytics에서 필터 추가에 대한 자세한 내용은 [고급 분석에서 필터 적용](../enhanced-analytics/use-enhanced-analytics-filters.md).

   필터를 추가하면 페이지를 나가거나 Workfront에서 로그아웃한 후에도 최대 50개의 프로젝트에 대한 데이터가 표시되고 필터가 활성 상태로 유지됩니다.

1. (선택 사항) 날짜 범위를 확대하려면 날짜 범위 시작에 대한 시각화에서 점을 선택하고 날짜 범위의 끝으로 드래그합니다.

   다른 모든 시각화는 동일한 날짜 범위 및 시간대 필터로 업데이트됩니다.

   ![](assets/timeframe-filter-350x220.png)

1. (선택 사항) 프로젝트의 정렬 방법을 변경하려면 **정렬 기준** 플라이트 계획 시각화의 오른쪽 위 모서리에 있는 메뉴를 선택한 다음, 새 정렬 옵션을 선택합니다.

   * **A - Z**
   * **Z - A**
   * **계획된 완료 일자**
   * **계획된 시작 일자**

   페이지의 다른 모든 시각화는 정렬 선택과 일치하도록 업데이트됩니다.

1. (조건부) 데이터 세트에 50개가 넘는 프로젝트가 있는 경우 시각화의 왼쪽 하단 모서리에 있는 화살표를 사용하여 50개의 프로젝트 그룹에서 다음 그룹으로 이동합니다.

   페이지의 다른 모든 시각화는 페이지 선택 내용과 일치하도록 업데이트됩니다.

   ![](assets/pagination-350x118.png)

1. 프로젝트 막대 그래프 위로 마우스를 가져가면 파란색 날짜 라인과 다음 세부 사항을 볼 수 있습니다.

   * 계획된 타임라인
   * 현재 조건
   * 사용자 지정 조건(해당하는 경우)

   ![](assets/project-bar-graph-350x143.png)

1. (선택 사항) 시각화 데이터를 내보내려면 **내보내기** 아이콘 ![](assets/export.png) 시각화의 오른쪽 상단 모서리에서 내보내기 형식을 선택합니다.

   * **차트(PNG)**
   * **데이터 테이블(XSLX)**

1. 프로젝트 정보를 더 보려면 시각화에서 프로젝트를 클릭하여 비행 시각화의 번다운 및 작업을 엽니다.

   이러한 시각화는 프로젝트가 제대로 작동하지 않게 된 원인에 대한 심층적인 통찰력을 얻을 수 있도록 해줍니다. 또한 진행 중인 프로젝트에 쉽게 체크 인할 수 있습니다.\
   Burndown 시각화에 대한 자세한 내용은 [Enhanced Analytics에서 Burndown 시각화 보기](../enhanced-analytics/burndown-overview.md). 플라이트 시각화의 작업에 대한 자세한 내용은 [Enhanced Analytics에서 플라이트 시각화의 작업 보기](../enhanced-analytics/tasks-in-flight-overview.md).

