---
content-type: overview
product-area: enhanced-analytics
navigation-topic: enhanced-analytics-navigation-topic
title: Enhanced Analytics에서 프로젝트 트리맵 시각화 보기
description: 프로젝트 트리맵 시각화는 크기가 다른 작업 노력과 비교하여 특정 시간 창에서 작업된 시간 또는 일 보기입니다. 이렇게 하면 사람들이 프로젝트에 얼마나 많은 시간을 할애했는지 이해할 수 있습니다.
author: Nolan
feature: Reports and Dashboards
exl-id: 6216465e-c3bb-4f2f-b71c-766ad0c2ed40
source-git-commit: 1b1f3c22b8112cfde5b10bef39076eed11630d0f
workflow-type: tm+mt
source-wordcount: '858'
ht-degree: 1%

---

# Enhanced Analytics에서 프로젝트 트리맵 시각화 보기

프로젝트 트리맵 시각화는 크기가 다른 작업 노력과 비교하여 특정 시간 창에서 작업된 시간 또는 일 보기입니다. 이렇게 하면 사람들이 프로젝트에 얼마나 많은 시간을 할애했는지 이해할 수 있습니다.

![](assets/project-treemap-350x126.png)

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

## 프로젝트 트리맵 시각화 이해

프로젝트 트리맵 시각화의 상자는 프로젝트를 나타내고 상자 크기는 다른 프로젝트에서 사용한 시간을 비교한 것을 보여줍니다. 상자가 클수록 프로젝트에 더 많은 시간이 소요됩니다.

프로젝트 트리맵 시각화는 다음과 같이 구성됩니다.

* **작은 파란색 상자**: 시간(일)이 적은 프로젝트는 연한 파란색의 작은 상자로 표시됩니다.

   ![](assets/project-treemap-smaller-box.png)

* **크고 진한 파란색 상자**: 시간이 더 많은 프로젝트(또는 일)가 어두운 파란색의 큰 상자로 표시됩니다.

   ![](assets/project-treemap-larger-box-350x205.png)

* **중간 크기의 파란색 상자**: 두 범주 사이에 속하는 프로젝트는 짙은 파란색과 밝은 파란색의 명암 사이의 중간 크기의 상자로 표시됩니다. 중간 크기의 상자들에 대해 가능한 파란색 음영이 3가지 있다.

오른쪽의 범례는 파란색 음영의 각 시간 동안의 완료된 시간을 보여줍니다. 이 범례는 동적이며 데이터에 따라 업데이트됩니다.

![](assets/project-treemap-hours-completed.png)

>[!NOTE]
>
>프로젝트 트리맵 시각화를 계획된 시간 대신 기간별로 보는 경우 이 범례는 각 파란색 음영으로 작업한 날짜 분류를 표시합니다.\
>![](assets/project-treemap-days-worked.png)>

다음 정보를 확인하면 다음을 결정하는 데 도움이 됩니다.

* 선택한 날짜 범위 동안 작업되는 항목의 우선 순위입니다.
* 어느 팀이 시간을 보내고 있습니까?
* 만약 팀이 옳은 것에 집중한다면.
* 특정 프로젝트를 클릭하면 해당 기간 동안 변경된 프로젝트 범위의 양입니다.

이 시각화에 대한 최상의 데이터를 가져오는 방법에 대해 알아보려면 [향상된 분석 개요](../enhanced-analytics/enhanced-analytics-overview.md).

## 프로젝트 트리맵 시각화 보기

1. Main Menu 아이콘을 클릭합니다. ![](assets/main-menu-icon-16x12.png)를 선택하고 을 선택합니다. **Analytics**.
1. (선택 사항) 다른 날짜 범위를 사용하려면 날짜 범위 필터에서 새 시작 날짜와 종료 날짜를 선택합니다.

   ![](assets/filters-select-date-range-350x344.png)

   날짜 범위 필터 사용에 대한 자세한 내용은 [고급 분석에서 필터 적용](../enhanced-analytics/use-enhanced-analytics-filters.md).

1. (조건부) 프로젝트 데이터 세트를 제한해야 하는 경우 사용할 필터를 선택하고 적용합니다.

   Enhanced Analytics에서 필터 추가에 대한 자세한 내용은 [고급 분석에서 필터 적용](../enhanced-analytics/use-enhanced-analytics-filters.md).

   필터를 추가하면 페이지를 나가거나 Workfront에서 로그아웃한 후에도 최대 50개의 프로젝트에 대한 데이터가 표시되고 필터가 활성 상태로 유지됩니다.

1. (선택 사항) 프로젝트의 정렬 방법을 변경하려면 **정렬 기준** 프로젝트 트리맵 시각화의 오른쪽 상단 모서리에 있는 메뉴를 선택한 다음 새 정렬 옵션을 선택합니다.

   * **A - Z**
   * **Z - A**
   * **계획된 완료 일자**
   * **계획된 시작 일자**

   페이지의 다른 모든 시각화는 정렬 선택과 일치하도록 업데이트됩니다.

1. (조건부) 데이터 세트에 50개가 넘는 프로젝트가 있는 경우 시각화의 왼쪽 하단 모서리에 있는 화살표를 사용하여 50개의 프로젝트 그룹에서 다음 그룹으로 이동합니다.

   페이지의 다른 모든 시각화는 페이지 선택 내용과 일치하도록 업데이트됩니다.

   ![](assets/pagination-350x118.png)

1. (선택 사항) 보기를 **계획 시간** to **기간**.

   기본적으로 계획 시간이 선택됩니다.

1. 마우스를 프로젝트 위로 가져가면 프로젝트 조건과 함께 총 계획된 시간, 총 완료된 시간, 일별 평균 프로젝트 체류 시간 수를 볼 수 있습니다.

   ![](assets/project-treemap-project-details-350x404.png)

   >[!NOTE]
   >
   >을(를) 선택한 경우 **기간** 다음과 같은 기간 세부 사항이 표시됩니다.
   >
   >* **계획 일정**: 프로젝트를 완료하기 위해 계획된 일 수입니다.
   >* **작업 시간**: 맨 위에서 선택한 날짜 범위 내에서 완료된 각 작업의 계획된 기간을 일별 시간 수로 나눈 기간입니다.

   >   
   >![](assets/duration-treemap-350x159.png)
   >
   >지속 시간에 대한 자세한 내용은 [향상된 분석 개요](../enhanced-analytics/enhanced-analytics-overview.md).

1. (선택 사항) 시각화 데이터를 내보내려면 **내보내기 아이콘** ![](assets/export.png) 시각화의 오른쪽 상단 모서리에서 내보내기 형식을 선택합니다.

   * **차트(PNG)**
   * **데이터 테이블(XSLX)**

1. 프로젝트를 클릭하여 비행 시각화에서 번다운 및 작업을 열어 프로젝트 크기에 대한 작업 및 시간(일)의 통찰력을 얻을 수 있습니다.

Burndown 시각화에 대한 자세한 내용은 [Enhanced Analytics에서 Burndown 시각화 보기](../enhanced-analytics/burndown-overview.md). 플라이트 시각화의 작업에 대한 자세한 내용은 [Enhanced Analytics에서 플라이트 시각화의 작업 보기](../enhanced-analytics/tasks-in-flight-overview.md).

