---
title: Enhanced Analytics에서 프로젝트 활동 시각화 보기
content-type: overview
product-area: enhanced-analytics
navigation-topic: enhanced-analytics-navigation-topic
description: 프로젝트 활동 시각화는 특정 기간 동안 발생한 프로젝트 수준의 활동(프로젝트에 지정된 각 사람의 활동)에 대한 집계 보기를 보여줍니다. 포커스 범위를 좁혀 프로젝트 내의 활동을 이해하거나 프로젝트 활동을 Adobe Workfront의 다른 프로젝트와 비교할 수 있습니다.
author: Nolan
feature: Reports and Dashboards
exl-id: 9ef52be8-48d0-4f83-a214-dd32e794c73e
source-git-commit: 1b1f3c22b8112cfde5b10bef39076eed11630d0f
workflow-type: tm+mt
source-wordcount: '800'
ht-degree: 1%

---

# Enhanced Analytics에서 프로젝트 활동 시각화 보기

프로젝트 활동 시각화는 특정 기간 동안 발생한 프로젝트 수준의 활동(프로젝트에 지정된 각 사람의 활동)에 대한 집계 보기를 보여줍니다. 포커스 범위를 좁혀 프로젝트 내의 활동을 이해하거나 프로젝트 활동을 Adobe Workfront의 다른 프로젝트와 비교할 수 있습니다.

>[!NOTE]
>
>팀별 활동 시각화는 이 시각화와 유사하게 동작하지만 팀별 활동 시각화는 모든 프로젝트에 대한 홈 팀 활동을 보여줍니다.\
>팀 시각화별 활동에 대한 자세한 내용은 [Enhanced Analytics에서 팀 시각화별 활동 보기](../enhanced-analytics/activity-by-team-overview.md).

<!--WRITER bad link; there is no Activity by Team.png
[![](assets/project-activity-350x114.png)](../Resources/Images/Analytics/Activity by Team.png)
-->

## 액세스 요구 사항

다음 항목이 있어야 합니다.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"><a href="https://www.workfront.com/plans" target="_blank">Workfront 플랜</a>*</td> 
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

## 프로젝트 활동 시각화 이해

일정 기간 동안 프로젝트의 특정 이벤트를 요약하기 위해 프로젝트 활동이 서로 다른 색상으로 표시됩니다.

* **로그인한 사용자**: 자주색 상자는 프로젝트에 지정된 사람들이 그 날 로그인한 것을 보여줍니다. 어두운 색조는 들어오는 사람이 더 많음을 나타냅니다.

   ![](assets/project-activity-users-logged-in.png)

* **작업 상태 변경**: 분홍색 상자는 사람들이 그 날 프로젝트의 작업 상태를 변경했다는 것을 보여 줍니다. 어두운 색조는 작업 상태가 변경되는 작업이 더 많음을 나타냅니다.

   ![](assets/project-activity-task-status-changes.png)

* **작업이 완료됨**: 파란색 상자는 사람들이 프로젝트에 대한 작업을 완료했음을 보여 줍니다. 어두운 음영은 완료되는 작업의 수가 더 많음을 나타냅니다.

   ![](assets/project-activity-tasks-completed.png)

마우스로 상자를 가리키면 지정된 날짜에 작업이 완료된 정확한 횟수가 표시됩니다. 프로젝트를 선택하여 프로젝트의 각 개별 기여자별로 이러한 활동의 분류를 볼 수 있습니다.

다음 정보를 확인하면 다음을 결정하는 데 도움이 됩니다.

* 특정 프로젝트의 활동입니다.
* 한 프로젝트의 활동이 다른 프로젝트와 비교됩니다.
* 프로젝트에서 작업 중인 사용자 및 빈도를 지정합니다.

이 시각화에 대한 최상의 데이터를 가져오는 방법에 대해 알아보려면 [향상된 분석 개요](../enhanced-analytics/enhanced-analytics-overview.md).

## 프로젝트 활동 시각화 보기

1. Main Menu 아이콘을 클릭합니다. ![](assets/main-menu-icon-16x12.png)를 선택하고 을 선택합니다. **Analytics**.
1. (선택 사항) 다른 날짜 범위를 사용하려면 날짜 범위 필터에서 새 시작 날짜와 종료 날짜를 선택합니다.

   ![](assets/filters-select-date-range-350x344.png)

   날짜 범위 필터 사용에 대한 자세한 내용은 [고급 분석에서 필터 적용](../enhanced-analytics/use-enhanced-analytics-filters.md).

   >[!NOTE]
   >
   >3개월 이상의 기간에 대해 날짜 범위를 선택하는 경우 프로젝트 활동 시각화에 데이터가 표시되지 않습니다.

1. (조건부) 프로젝트 데이터 세트를 제한해야 하는 경우 사용할 필터를 선택하고 적용합니다.

   Enhanced Analytics에서 필터 추가에 대한 자세한 내용은 [고급 분석에서 필터 적용](../enhanced-analytics/use-enhanced-analytics-filters.md).

   필터를 추가하면 페이지를 나가거나 Workfront에서 로그아웃한 후에도 최대 50개의 프로젝트에 대한 데이터가 표시되고 필터가 활성 상태로 유지됩니다.

1. (선택 사항) 날짜 범위를 확대하려면 날짜 범위 시작에 대한 시각화에서 점을 선택하고 날짜 범위의 끝으로 드래그합니다.

   다른 모든 시각화는 동일한 날짜 범위 및 시간대 필터로 업데이트됩니다.

   ![](assets/timeframe-filter-350x220.png)

1. (선택 사항) 프로젝트의 정렬 방법을 변경하려면 **정렬 기준** 메뉴를 클릭한 다음 새 정렬 옵션을 선택합니다.

   * **A - Z**
   * **Z - A**
   * **계획된 완료 일자**
   * **계획된 시작 일자**

   페이지의 다른 모든 시각화는 정렬 선택과 일치하도록 업데이트됩니다.

1. (조건부) 데이터 세트에 50개가 넘는 프로젝트가 있는 경우 시각화의 왼쪽 하단 모서리에 있는 화살표를 사용하여 50개의 프로젝트 그룹에서 다음 그룹으로 이동합니다.

   페이지의 다른 모든 시각화는 페이지 선택 내용과 일치하도록 업데이트됩니다.

   ![](assets/pagination-350x118.png)

1. 프로젝트에 대한 자세한 내용을 보려면 시각화에서 프로젝트를 클릭하십시오.

   목록이 확장되어 프로젝트에 있는 각 개별 기여자의 활동이 표시됩니다.

1. 상자 위에 마우스를 올려 놓아 사용자가 작업을 완료한 날짜와 해당 날짜에 대한 작업을 완료한 횟수를 확인합니다.

   ![](assets/project-activity-activity-pop-up-350x137.png)

1. (선택 사항) 시각화 데이터를 내보내려면 **내보내기 아이콘** ![](assets/export.png) 시각화의 오른쪽 상단 모서리에서 내보내기 형식을 선택합니다.

   * **차트(PNG)**
   * **데이터 테이블(XSLX)**

