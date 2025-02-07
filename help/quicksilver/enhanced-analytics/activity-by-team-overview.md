---
title: 향상된 분석에서 팀별 활동 시각화 보기
content-type: overview
product-area: enhanced-analytics
navigation-topic: enhanced-analytics-navigation-topic
description: 팀 시각화별 활동 은 홈 팀의 특정 시간대 동안 발생하는 활동을 표시하므로 다양한 홈 팀이 Adobe Workfront에서 어떻게 시간을 보냈는지 이해할 수 있습니다. Workfront에서 홈 팀을 설정하는 방법에 따라 이 시각화를 통해 다양한 통찰력을 제공하고 다양한 질문에 답변할 수 있습니다.
author: Nolan
feature: Reports and Dashboards
exl-id: c4f9886c-ce76-43a8-bd43-cb64fff27e79
source-git-commit: 325334010d5f1206931cc9ace67f9511d614ffca
workflow-type: tm+mt
source-wordcount: '727'
ht-degree: 7%

---

# 향상된 분석에서 팀별 활동 시각화 보기

<!-- Audited: 12/2023 -->

팀 시각화별 활동 은 홈 팀의 특정 시간대 동안 발생하는 활동을 표시하므로 다양한 홈 팀이 Adobe Workfront에서 어떻게 시간을 보냈는지 이해할 수 있습니다. Workfront에서 홈 팀을 설정하는 방법에 따라 이 시각화를 통해 다양한 통찰력을 제공하고 다양한 질문에 답변할 수 있습니다.

>[!NOTE]
>
>프로젝트 활동 시각화는 이 시각화와 유사하지만, 홈 팀에 할당된 사람이 아닌 프로젝트에 할당된 사람을 기반으로 하는 활동을 표시합니다.\
>프로젝트 활동 시각화에 대한 자세한 내용은 [향상된 분석에서 프로젝트 활동 시각화 보기](../enhanced-analytics/project-activity-overview.md)를 참조하십시오.

팀별 ![활동](assets/activity-by-team-350x113.png){width="700"}

## 액세스 요구 사항

+++ 를 확장하여 액세스 요구 사항을 확인합니다.

이 문서의 단계를 수행하려면 다음 액세스 권한이 있어야 합니다.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"><a href="https://www.workfront.com/plans" target="_blank">Workfront 플랜</a></td> 
   <td> <p>비즈니스 이상</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><a href="../administration-and-setup/add-users/access-levels-and-object-permissions/wf-licenses.md" class="MCXref xref">Adobe Workfront 라이선스 개요</a></td> 
   <td>
      <p>신규:</p> 
         <ul><li>밝은 색 이상</li></ul>
      <p>현재:</p>
         <ul><li>검토 이상</li></ul>
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader">액세스 수준 구성</td> 
   <td> <p>프로젝트에 대한 액세스 보기</p> <!--<p>Note: If you still don't have access, ask your Workfront administrator if they set additional restrictions in your access level.<br>For information on how a Workfront administrator can change your access level, see <a href="../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Create or modify custom access levels</a>.</p>--> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">개체 권한</td> 
   <td> <p>보기</p> <!--<p>For information on requesting additional access, see <a href="../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Request access to objects </a>.</p>--> </td> 
  </tr> 
 </tbody> 
</table>

이 표의 정보에 대한 자세한 내용은 [Workfront 설명서의 액세스 요구 사항](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)을 참조하십시오.

+++

## 전제 조건

향상된 Analytics를 사용하기 위한 전제 조건은 [향상된 Analytics 개요](../enhanced-analytics/enhanced-analytics-overview.md)의 &quot;전제 조건&quot; 섹션을 참조하십시오.

## 팀 시각화별 활동 이해

서로 다른 활동이 서로 다른 색상으로 표시되어 필터링된 기간 동안의 특정 이벤트를 요약합니다.

* **로그인한 사용자**: 자주색 상자에 홈 팀의 사용자가 해당 날짜에 로그인했음을 표시됩니다. 어두운 음영은 더 많은 수의 로그인 사용자를 나타냅니다.

  ![로그인한 사용자](assets/project-activity-users-logged-in.png)

* **작업 상태 변경**: 분홍색 상자로 표시된 경우 홈 팀의 직원들이 해당 날짜의 작업 상태를 변경했습니다. 어두운 음영은 더 많은 수의 작업 상태가 변경됨을 나타냅니다.

  ![작업 상태 변경](assets/project-activity-task-status-changes.png)

* **작업 완료됨**: 홈 팀의 직원들이 해당 날짜에 작업을 완료했음을 파란색 상자로 표시합니다. 어두운 음영은 더 많은 수의 작업이 완료되었음을 나타냅니다.

  ![작업 완료됨](assets/project-activity-tasks-completed.png)

상자 위로 마우스를 가져가면 지정된 날짜에 작업이 완료된 정확한 횟수를 볼 수 있습니다. 팀을 선택하여 홈 팀의 각 사용자별로 이러한 활동의 분류를 확인할 수 있습니다.

이 정보를 보면 다음과 같은 사항을 확인할 수 있습니다.

* 홈 팀 내에서 발생하는 활동 및 속도.
* 어떤 홈팀이 과로를 하고 있거나 시스템을 더 많이 사용하고 있는가?
* 업무 배분이 홈 팀에 적합한지 여부.

이 시각화에 가장 적합한 데이터를 얻는 방법에 대해 알아보려면 [향상된 분석 개요](../enhanced-analytics/enhanced-analytics-overview.md)를 참조하십시오.

## 팀별 활동 시각화 보기

1. 주 메뉴 아이콘 ![주 메뉴 아이콘](assets/main-menu-icon-16x12.png)을 클릭한 다음 **분석**&#x200B;을 선택합니다.
1. 왼쪽 패널에서 **직원**&#x200B;을 선택합니다.

   ![사람 영역](assets/people-area-cropped-qs-350x276.png)

1. (선택 사항) 다른 날짜 범위를 사용하려면 날짜 범위 필터에서 새 시작 날짜와 종료 날짜를 선택합니다.

   ![날짜 범위 선택](assets/filters-select-date-range-350x344.png)

   날짜 범위 필터 사용에 대한 자세한 내용은 [향상된 분석에서 필터 적용](../enhanced-analytics/use-enhanced-analytics-filters.md)을 참조하십시오.

1. (조건부) 팀 필터를 설정하지 않은 경우 팀 필터를 추가하고 데이터를 보려는 각 팀을 선택합니다.

   향상된 분석에서 필터를 추가하는 방법에 대한 자세한 내용은 [향상된 분석에서 필터 적용](../enhanced-analytics/use-enhanced-analytics-filters.md)을 참조하십시오.

   필터를 추가하면 최대 50개의 프로젝트에 대한 데이터가 표시되고 페이지를 떠나거나 Workfront에서 로그아웃한 후에도 필터가 활성 상태로 유지됩니다.

1. (선택 사항) 날짜 범위를 확대하려면 날짜 범위 시작에 대한 시각화의 한 지점을 선택하고 날짜 범위의 끝으로 드래그합니다.

   다른 모든 시각화는 동일한 날짜 범위로 업데이트되며 일정 필터가 만들어집니다.

   ![일정 필터](assets/timeframe-filter-350x220.png)

1. 팀 이름 클릭

   <!--
   <MadCap:conditionalText data-mc-conditions="QuicksilverOrClassic.Draft mode">
   or role
   </MadCap:conditionalText>
   -->

   홈 팀이 완료한 활동에 대한 자세한 내용을 봅니다.

   목록이 확장되어 홈 팀에 할당된 각 사용자의 활동이 표시됩니다.

   <!--
   <span style="color: #ff1493;" data-mc-conditions="QuicksilverOrClassic.Draft mode"> Role not available</span>
   -->

1. 색 상자 위로 마우스를 가져가면 사용자가 작업을 완료한 날짜와 해당 날짜에 작업이 완료된 횟수를 볼 수 있습니다.

   어두운 색상은 더 높은 활동성을 나타냅니다.

   팀별 ![활동](assets/activity-by-team-activity-pop-up-350x155.png)

1. (선택 사항) 시각화 데이터를 내보내려면 시각화의 오른쪽 상단 모서리에 있는 내보내기 아이콘 ![내보내기 아이콘](assets/export.png)을 클릭한 다음 내보내기 형식을 선택합니다.

   * **차트(PNG)**
   * **데이터 테이블(XSLX)**

