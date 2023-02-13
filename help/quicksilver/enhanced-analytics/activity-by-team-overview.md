---
title: Enhanced Analytics에서 팀 시각화별 활동 보기
content-type: overview
product-area: enhanced-analytics
navigation-topic: enhanced-analytics-navigation-topic
description: 팀별 활동 시각화는 홈 팀의 특정 기간 동안 발생하는 활동을 보여주므로 여러 홈 팀이 Adobe Workfront에서 보낸 시간을 파악할 수 있습니다. 홈 팀이 Workfront에서 설정되는 방식에 따라 이 시각화는 다양한 통찰력을 제공하고 다양한 질문에 답변할 수 있습니다.
author: Nolan
feature: Reports and Dashboards
exl-id: c4f9886c-ce76-43a8-bd43-cb64fff27e79
source-git-commit: 1b1f3c22b8112cfde5b10bef39076eed11630d0f
workflow-type: tm+mt
source-wordcount: '734'
ht-degree: 0%

---

# Enhanced Analytics에서 팀 시각화별 활동 보기

팀별 활동 시각화는 홈 팀의 특정 기간 동안 발생하는 활동을 보여주므로 여러 홈 팀이 Adobe Workfront에서 보낸 시간을 파악할 수 있습니다. 홈 팀이 Workfront에서 설정되는 방식에 따라 이 시각화는 다양한 통찰력을 제공하고 다양한 질문에 답변할 수 있습니다.

>[!NOTE]
>
>프로젝트 활동 시각화는 이 시각화와 유사하지만, 홈 팀에 지정된 사람이 아니라 프로젝트에 할당된 사람을 기반으로 활동을 표시합니다.\
>프로젝트 활동 시각화에 대한 자세한 내용은 [Enhanced Analytics에서 프로젝트 활동 시각화 보기](../enhanced-analytics/project-activity-overview.md).

![](assets/activity-by-team-350x113.png)

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

## 팀 시각화별 활동 이해

필터링된 기간 동안의 특정 이벤트를 요약하기 위해 다양한 활동이 서로 다른 색상으로 표시됩니다.

* **로그인한 사용자**: 보라색 상자는 그 날 홈팀 사람들이 로그인했다는 것을 보여줍니다. 어두운 색조는 들어오는 사람이 더 많음을 나타냅니다.

   ![](assets/project-activity-users-logged-in.png)

* **작업 상태 변경**: 분홍 박스들은 홈 팀의 사람들이 그 날 작업의 상태를 변경했다는 것을 보여줍니다. 어두운 색조는 작업 상태가 변경되는 작업이 더 많음을 나타냅니다.

   ![](assets/project-activity-task-status-changes.png)

* **작업이 완료됨**: 파란 상자는 홈 팀의 사람들이 그 날 작업을 완료했다는 것을 보여줍니다. 어두운 음영은 완료되는 작업의 수가 더 많음을 나타냅니다.

   ![](assets/project-activity-tasks-completed.png)

마우스로 상자를 가리키면 지정된 날짜에 작업이 완료된 정확한 횟수가 표시됩니다. 팀을 선택하여 홈팀의 각 개인이 이러한 활동에 대한 분류를 볼 수 있습니다.

다음 정보를 확인하면 다음을 결정하는 데 도움이 됩니다.

* 홈 팀 내에서 발생하는 활동과 그 비율
* 어떤 홈 팀이 과로 중이거나 더 많이 사용하고 있는가.
* 홈 팀에 적합한 작업 배포라면

이 시각화에 대한 최상의 데이터를 가져오는 방법에 대해 알아보려면 [향상된 분석 개요](../enhanced-analytics/enhanced-analytics-overview.md).

## 팀 시각화별 활동 보기

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

1. 팀 이름 클릭

   <!--
   <MadCap:conditionalText data-mc-conditions="QuicksilverOrClassic.Draft mode">
   or role
   </MadCap:conditionalText>
   -->

   홈 팀에서 완료한 활동에 대한 자세한 내용을 보려면

   목록이 확장되어 홈 팀에 지정된 각 개인의 활동이 표시됩니다.

   <!--
   <span style="color: #ff1493;" data-mc-conditions="QuicksilverOrClassic.Draft mode"> Role not available</span>
   -->

1. 색상 상자 위로 마우스를 가져가면 사용자가 작업을 완료한 날짜와 해당 작업을 완료한 횟수를 볼 수 있습니다.

   어두운 색상은 더 높은 활동을 나타냅니다.

   ![](assets/activity-by-team-activity-pop-up-350x155.png)

1. (선택 사항) 시각화 데이터를 내보내려면 내보내기 아이콘을 클릭합니다 ![](assets/export.png) 시각화의 오른쪽 상단 모서리에서 내보내기 형식을 선택합니다.

   * **차트(PNG)**
   * **데이터 테이블(XSLX)**

