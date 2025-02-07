---
title: 향상된 분석에서 플라이트 플랜 시각화 보기
content-type: overview
product-area: enhanced-analytics
navigation-topic: enhanced-analytics-navigation-topic
description: 플라이트 계획 시각화는 적용된 필터 기준 내에서 얼마나 많은 프로젝트가 작동 중인지, 이러한 프로젝트의 라이프타임 동안 어떤 상태 변화가 발생했는지, 그리고 이러한 프로젝트가 계획된 완료 기한을 얼마나 준수했는지 보여 줍니다.
author: Nolan
feature: Reports and Dashboards
exl-id: c64ed752-151a-40f7-ab18-684e2cd032bc
source-git-commit: 325334010d5f1206931cc9ace67f9511d614ffca
workflow-type: tm+mt
source-wordcount: '885'
ht-degree: 4%

---

# 향상된 분석에서 플라이트 플랜 시각화 보기

플라이트 계획 시각화는 적용된 필터 기준 내에서 얼마나 많은 프로젝트가 작동 중인지, 이러한 프로젝트의 라이프타임 동안 어떤 상태 변화가 발생했는지, 그리고 이러한 프로젝트가 계획된 완료 기한을 얼마나 준수했는지 보여 줍니다.

![플라이트 플랜](assets/flight-plan-350x132.png)

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
   <td> <p>프로젝트에 대한 액세스 보기</p> <p>참고: 여전히 액세스 권한이 없는 경우 Workfront 관리자에게 액세스 수준에서 추가 제한을 설정하는지 문의하십시오.<br>Workfront 관리자가 액세스 수준을 변경하는 방법에 대한 자세한 내용은 <a href="../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">사용자 지정 액세스 수준 만들기 또는 수정</a>을 참조하십시오.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">개체 권한</td> 
   <td> <p>프로젝트에 대한 액세스 보기</p> <p>추가 액세스 요청에 대한 자세한 내용은 <a href="../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">개체 </a>에 대한 액세스 요청 을 참조하십시오.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;보유 중인 플랜, 라이선스 유형 또는 액세스 권한을 확인하려면 Workfront 관리자에게 문의하십시오.

## 전제 조건

향상된 Analytics를 사용하기 위한 전제 조건은 [향상된 Analytics 개요](../enhanced-analytics/enhanced-analytics-overview.md)의 &quot;전제 조건&quot; 섹션을 참조하십시오.

## 플라이트 계획 시각화 이해

프로젝트의 실제 기간에서는 다음 프로젝트 조건만 볼 수 있습니다.

* 대상
* 위험 상태
* 문제 발생

프로젝트 조건에 대해 알아보려면 [프로젝트 조건 및 조건 형식 개요](../manage-work/projects/manage-projects/project-condition-and-condition-type.md)를 참조하세요.

플라이트 계획 시각화에는 다음 프로젝트 세부 사항이 표시됩니다.

* **계획된 기간**: 파란색 가로 선은 프로젝트의 계획된 길이를 나타내며, 선 끝에 있는 삼각형은 시작 날짜와 종료 날짜를 나타냅니다.

  ![계획된 기간](assets/planned-duration-line-350x37.png)

* **실제 기간**: 계획된 기간 아래의 굵고 색상이 지정된 선은 프로젝트의 실제 길이를 나타냅니다. 프로젝트의 수명 중 해당 특정 시점에 프로젝트의 상태에 따라 선의 색상이 변경됩니다.

  ![실제 기간](assets/actual-duration-line.png)

* **실제 상태**: 굵고 색상이 지정된 선은 시간대별로 프로젝트의 상태를 표시합니다. 선 색상은 프로젝트의 상태에 따라 달라집니다.

   * **녹색**: 대상에 있음
   * **주황**: 위험 상태
   * **빨강**: 문제 발생

  ![실제 상태](assets/actual-condition-color.png)

플라이트 플랜 시각화의 프로젝트 행 위로 마우스를 가져가면 프로젝트의 계획된 일정, 현재 프로젝트 상태 및(해당하는 경우) 사용자 지정 상태에 대한 정보를 볼 수 있습니다. 지속 시간이나 조건에 영향을 미칠 수 있는 사항을 보다 깊이 있게 보려면 고급 분석 영역에서 다른 시각화를 살펴볼 수 있습니다.

이 정보를 보면 다음과 같은 사항을 확인할 수 있습니다.

* 프로젝트가 원래 계획된 완료 일자를 지나 확장되는 이벤트는 무엇입니까?
* 프로젝트에 문제가 발생하기 시작하는 시점.
* 동일한 기간 동안 진행되는 프로젝트의 수.
* 활성 프로젝트의 수.
* 특별한 관심이나 지원이 필요한 프로젝트.

이 시각화에 가장 적합한 데이터를 얻는 방법에 대한 자세한 내용은 [향상된 분석 개요](../enhanced-analytics/enhanced-analytics-overview.md)를 참조하십시오.

## 플라이트 계획 시각화 보기

1. **주 메뉴** 아이콘 ![주 메뉴 아이콘](assets/main-menu-icon-16x12.png)을 클릭한 다음 **Analytics**&#x200B;를 선택합니다.
1. (선택 사항) 다른 날짜 범위를 사용하려면 날짜 범위 필터에서 새 시작 날짜와 종료 날짜를 선택합니다.

   ![날짜 범위 선택](assets/filters-select-date-range-350x344.png)

   날짜 범위 필터 사용에 대한 자세한 내용은 [향상된 분석에서 필터 적용](../enhanced-analytics/use-enhanced-analytics-filters.md)을 참조하십시오.

1. (조건부) 프로젝트 데이터 세트를 제한해야 하는 경우 사용할 필터를 선택하고 적용합니다.

   향상된 분석에서 필터를 추가하는 방법에 대한 자세한 내용은 [향상된 분석에서 필터 적용](../enhanced-analytics/use-enhanced-analytics-filters.md)을 참조하십시오.

   필터를 추가하면 최대 50개의 프로젝트에 대한 데이터가 표시되고 페이지를 떠나거나 Workfront에서 로그아웃한 후에도 필터가 활성 상태로 유지됩니다.

1. (선택 사항) 날짜 범위를 확대하려면 날짜 범위 시작에 대한 시각화의 한 지점을 선택하고 날짜 범위의 끝으로 드래그합니다.

   다른 모든 시각화는 동일한 날짜 범위로 업데이트되며 일정 필터가 만들어집니다.

   ![일정 필터](assets/timeframe-filter-350x220.png)

1. (선택 사항) 프로젝트 정렬 방법을 변경하려면 플라이트 계획 시각화의 오른쪽 상단에 있는 **정렬 기준** 메뉴를 클릭한 다음, 새 정렬 옵션을 선택하십시오.

   * **A - Z**
   * **Z - A**
   * **계획된 완료 일자**
   * **계획된 시작 일자**

   페이지의 다른 모든 시각화는 정렬 선택 사항과 일치하도록 업데이트됩니다.

1. (조건부) 데이터 세트에 50개가 넘는 프로젝트가 있는 경우 시각화의 왼쪽 하단 모서리에 있는 화살표를 사용하여 50개의 프로젝트 그룹 중 하나에서 다음 그룹으로 이동합니다.

   페이지의 다른 모든 시각화는 페이지 선택 사항과 일치하도록 업데이트됩니다.

   ![페이지 매김](assets/pagination-350x118.png)

1. 프로젝트 막대 그래프 위로 마우스를 가져가면 파란색 날짜 줄과 다음 세부 정보를 볼 수 있습니다.

   * 계획된 타임라인
   * 현재 상태
   * 사용자 지정 조건(해당되는 경우)

   ![프로젝트 막대 그래프](assets/project-bar-graph-350x143.png)

1. (선택 사항) 시각화 데이터를 내보내려면 시각화의 오른쪽 상단에 있는 **내보내기** 아이콘 ![내보내기 아이콘](assets/export.png)을 클릭한 다음 내보내기 형식을 선택합니다.

   * **차트(PNG)**
   * **데이터 테이블(XSLX)**

1. 자세한 프로젝트 정보를 보려면 시각화에서 프로젝트를 클릭하여 번다운 및 진행 중인 작업 시각화를 엽니다.

   이러한 시각화는 프로젝트가 궤도를 이탈하게 한 원인에 대한 심층적인 통찰력을 얻는 데 도움이 될 수 있습니다. 또한 진행 중인 프로젝트에 쉽게 체크 인할 수 있습니다.\
   번다운 시각화에 대한 자세한 내용은 [향상된 분석에서 번다운 시각화 보기](../enhanced-analytics/burndown-overview.md)를 참조하십시오. 진행 중인 작업 시각화에 대한 자세한 내용은 [향상된 분석에서 진행 중인 작업 시각화 보기](../enhanced-analytics/tasks-in-flight-overview.md)를 참조하십시오.

