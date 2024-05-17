---
title: 향상된 분석 개요
content-type: overview
product-area: enhanced-analytics
navigation-topic: enhanced-analytics-navigation-topic
description: 향상된 Analytics는 계획 및 완료로 프로젝트 데이터를 보고 트렌드를 식별할 수 있도록 해주는 미리 작성된 시각화가 있는 Adobe Workfront의 강력한 도구입니다. 프로젝트에 대한 이러한 통찰력을 통해 현재 작업을 관리하고 향후 작업을 보다 정확하게 계획할 수 있습니다.
author: Nolan
feature: Reports and Dashboards
exl-id: a14ad57c-859b-43df-84c0-575ccda86e50
source-git-commit: 530c4451f4720a1710350f8e822e343794b63e87
workflow-type: tm+mt
source-wordcount: '1203'
ht-degree: 3%

---

# 향상된 분석 개요

향상된 Analytics는 계획 및 완료로 프로젝트 데이터를 보고 트렌드를 식별할 수 있도록 해주는 미리 작성된 시각화가 있는 Adobe Workfront의 강력한 도구입니다. 프로젝트에 대한 이러한 통찰력을 통해 현재 작업을 관리하고 향후 작업을 보다 정확하게 계획할 수 있습니다.

향상된 분석을 통해 다음을 식별할 수 있습니다.

* 프로젝트를 계획하는 방법
* 작업이 프로젝트에 추가될 때
* 다른 프로젝트에 대해 완료되는 작업량
* 홈 팀이 예정된 시간 또는 일수와 비교하여 프로젝트를 완료하는 데 필요한 시간 또는 일수입니다.
* 프로젝트 진행 중 사용자가 특정 작업을 완료하는 빈도
* 프로젝트 진행 상황 및 프로젝트 내 개별 작업

![](assets/nwe-full-screen-analytics-350x222.png)

사용 사례를 확인하거나 Enhanced Analytics를 사용하여 현재 작업 관리 및 향후 작업 계획에 대해 자세히 알아보려면 다음을 참조하십시오. [향상된 분석 학습 경로](https://one.workfront.com/s/enhanced-analytics-program).

## 전제 조건

고급 분석 영역에 액세스하려면 다음을 수행해야 합니다.

* 비즈니스 또는 엔터프라이즈 플랜이 있습니다.

  자세한 내용은 [Workfront 플랜](https://www.workfront.com/plans).

* Workfront 관리자가 레이아웃 템플릿에 향상된 분석을 추가하도록 합니다.

  자세한 내용은 [향상된 Analytics: 레이아웃 템플릿에 분석 추가](https://one.workfront.com/s/managed-content-videos/enhanced-analytics-adding-analytics-to-layout-templates-MCH7URDSIXRREHHHF7TRTYYP2LTE).

프로젝트 및 작업에 대한 정보를 보려면 다음을 수행해야 합니다.

* 액세스 수준의 프로젝트 및 작업 영역에 대한 보기 권한이 있습니다.

  Workfront 관리자가 액세스 수준을 수정하는 방법에 대한 자세한 내용은 [사용자 정의 액세스 수준 만들기 또는 수정](../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md).

* 특정 작업 및/또는 프로젝트에 대한 보기 권한이 있습니다.

  추가 액세스 요청에 대한 자세한 내용은 [오브젝트에 대한 액세스 요청](../workfront-basics/grant-and-request-access-to-objects/request-access.md).

## 향상된 분석을 위한 우수 사례

프로젝트에 가장 적합한 데이터를 가져오려면 정확한 계획된 시간 및 기간(일)이 있는 템플릿을 사용하십시오. 또한 사용자가 가능한 한 정확하게 아래 필드를 입력하고 업데이트하는지 확인해야 합니다.

>[!NOTE]
>
>다음 필드 중 일부는 사용자가 입력하는 정보를 기반으로 Workfront이 수행하는 계산입니다. 이러한 필드는 수동으로 업데이트할 수 없습니다.

* 계획된 시간

  이것은 작성해야 할 가장 중요한 필드입니다.

  >[!NOTE]
  >
  >팀에서 계획된 시간을 사용하지 않는 경우에도 프로젝트 기간을 기준으로 일부 데이터를 볼 수 있습니다.\
  >자세한 내용은 섹션을 참조하십시오 [기간 보기](#duration-view) 이 문서에서.

* 프로젝트 이름

  이름은 프로젝트를 설명하는 이름이어야 합니다.

* 프로젝트 상태
* 프로젝트 상태
* 프로젝트 계획 시작 일자
* 계획된 완료 일자 기준
* 프로젝트 실제 시작 일자
* 프로젝트 실제 종료 일자
* 프로젝트 기간(시간)
* 프로젝트 실제 근로시간
* 작업 상태(완료 표시 작업이 포함됩니다.)
* 작업 이름
* 작업 완료율
* 작업 계획 시작 일자
* 작업 계획된 완료 일자

>[!IMPORTANT]
>
>작업 및 프로젝트에 수행된 변경 사항이 향상된 분석에 반영되기까지 최대 24시간이 걸릴 수 있습니다.

## 기간 보기 {#duration-view}

번다운 및 프로젝트 트리맵 시각화는 기본적으로 계획된 시간을 기반으로 합니다. 팀이 계획된 시간을 사용하지 않는 경우 프로젝트 기간을 기반으로 이러한 시각화를 볼 수 있습니다.

향상된 분석에서 프로젝트 기간은 다음 공식으로 계산됩니다.

* 계획된 일정:

  ```
  Planned Completion Date of the project - Start Date of the project
  ```

* 근무일:

  ```
  Planned Duration for tasks completed in the selected date range / Typical hours per work day
  ```

  >[!NOTE]
  >
  >8시간은 의 기본 번호입니다. **근무일당 일반 근로시간**. Adobe Workfront 관리자는 다음을 업데이트할 수 있습니다. **근무일당 일반 근로시간** 아래에 설정 **설정** > **프로젝트 환경 설정** > **프로젝트** > **타임라인**.\
  >자세한 내용은 다음을 참조하십시오. [시스템 전체 프로젝트 환경 설정 구성](../administration-and-setup/set-up-workfront/configure-system-defaults/set-project-preferences.md).

계획된 기간에 대한 자세한 내용은 [프로젝트 기간 개요](../manage-work/projects/planning-a-project/project-duration.md).

## 키보드 단축키

키보드의 다음 키를 사용하여 고급 분석 영역에서 특정 작업을 탐색하거나 완료할 수 있습니다.

| 키 | 개 액션 |
|---|---|
| **탭** | 페이지에 표시되지 않는 각 시각화에 대한 정보가 있는 테이블뿐만 아니라 페이지의 각 요소로 이동합니다 |
| **입력** | 달력 위젯 열기, 기존 필터 삭제, 필터 옵션 추가 열기, 필터 값 선택/선택 해제, 만든 필터 적용, 각 시각화에서 내보내기 옵션 열기, 번다운, 진행 중인 작업 및 프로젝트 트리맵 시각화에서 드롭다운 메뉴 열기 |
| **화살표 키** | 달력 위젯의 날짜로 이동하거나, 필터를 추가할 때 필터 옵션을 통해 이동하거나, 시각화의 모든 드롭다운 메뉴에서 옵션을 통해 이동합니다. |
| **스페이스바** | 달력 위젯에서 날짜를 선택하고 필터를 추가할 때 필터 유형을 선택한 다음 각 시각화의 드롭다운 메뉴에서 내보내기 옵션을 선택하고 번다운, 진행 중인 작업 및 프로젝트 트리맵 시각화의 드롭다운 메뉴에서 옵션을 선택합니다 |

{style="table-layout:auto"}

화면 읽기 소프트웨어나 플러그인을 사용하는 경우 화면 판독기는 화면의 정보를 큰 소리로 읽고 위에 나열된 키를 사용할 때 완료하는 작업을 설명합니다.

## 향상된 Analytics 보기 및 기능

Enhanced Analytics의 특정 기능에 대한 세부 정보, 추가 통찰력을 얻기 위해 완료할 수 있는 작업 및 이 데이터에서 배울 수 있는 사항에 대해서는 다음 문서를 참조하십시오.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th>기사</th> 
   <th>설명</th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td><a href="../enhanced-analytics/use-enhanced-analytics-filters.md" class="MCXref xref">향상된 분석에서 필터 적용</a> </td> 
   <td> <p>사용자 지정 필터, 프로젝트 필드 필터 또는 팀 필터를 적용하여 특정 기준에 맞는 프로젝트만 볼 수 있습니다. 필터를 추가하면 그에 따라 프로젝트 수가 업데이트됩니다.</p> </td> 
  </tr> 
  <tr> 
   <td><a href="../enhanced-analytics/understand-enhanced-analytics-kpis.md" class="MCXref xref">향상된 분석 KPI 이해</a> </td> 
   <td> <p>특정 시간대 내의 모든 프로젝트에 대한 주요 성과 지표(KPI)는 화면 상단에 있습니다.</p> </td> 
  </tr> 
  <tr> 
   <td> <p><a href="../enhanced-analytics/flight-plan-overview.md" class="MCXref xref">향상된 분석에서 플라이트 플랜 시각화 보기</a> </p> </td> 
   <td> <p>다음 <b>플라이트 플랜</b> 시각화는 프로젝트 기간 동안 상태가 변경되었음을 보여 줍니다. 시각화와 상호 작용하면 특정 날짜에 대한 세부 정보를 얻을 수 있습니다. 프로젝트를 선택하면 번다운 및 진행 중인 작업 시각화가 열립니다.</p> </td> 
  </tr> 
  <tr> 
   <td><a href="../enhanced-analytics/burndown-overview.md" class="MCXref xref">향상된 분석에서 번다운 시각화 보기</a> </td> 
   <td> <p>다음 <b>번다운</b> 시각화는 프로젝트에 소요된 실제 시간과 비교하여 프로젝트의 계획된 속도를 보여 줍니다. 시각화와 상호 작용하면 특정 날짜의 프로젝트 상태에 대한 자세한 내용을 볼 수 있습니다.</p> </td> 
  </tr> 
  <tr> 
   <td><a href="../enhanced-analytics/tasks-in-flight-overview.md" class="MCXref xref">향상된 분석에서 진행 중인 작업 시각화 보기</a> </td> 
   <td> <p>다음 <b>진행 중인 작업</b> 시각화는 프로젝트 내의 각 작업의 상태를 보여 줍니다. 시각화와 상호 작용하면 작업을 빠르고 쉽게 변경할 수 있습니다.</p> </td> 
  </tr> 
  <tr> 
   <td><a href="../enhanced-analytics/project-activity-overview.md" class="MCXref xref">향상된 분석에서 프로젝트 활동 시각화 보기</a> </td> 
   <td> <p>다음 <b>프로젝트 활동</b> 시각화는 프로젝트에 할당된 사용자가 Workfront에 로그인하고, 해당 프로젝트의 작업 상태를 변경하고, 해당 프로젝트에서 작업을 완료한 시점의 히트맵을 보여 줍니다. 시각화와 상호 작용하면 각 사용자에 대한 이러한 세부 사항을 볼 수 있습니다. 각 작업이 완료된 횟수와 이러한 작업에 대한 특정 날짜도 볼 수 있습니다.</p> </td> 
  </tr> 
  <tr> 
   <td><a href="../enhanced-analytics/project-treemap-overview.md" class="MCXref xref">향상된 분석에서 프로젝트 트리맵 시각화 보기</a> </td> 
   <td> <p>다음 <b>프로젝트 트리맵</b> 시각화는 다른 프로젝트에 비해 일부 프로젝트에서 얼마나 많은 시간이 소요되었는지를 보여 줍니다. 시각화와 상호 작용하면 프로젝트의 상태, 계획된 프로젝트 완료 및 실제 프로젝트 완료에 대한 세부 정보를 확인할 수 있습니다.</p> </td> 
  </tr> 
  <tr> 
   <td><a href="../enhanced-analytics/activity-by-team-overview.md" class="MCXref xref">향상된 분석에서 팀별 활동 시각화 보기</a> </td> 
   <td> <p>다음 <b>팀별 활동</b> 시각화는 홈 팀의 사용자가 Workfront에 로그인하여 작업 상태를 변경하고 작업을 완료한 시점의 히트맵을 보여 줍니다. 시각화와 상호 작용하면 각 개별 사용자에 대한 이러한 세부 사항을 볼 수 있습니다. 각 작업이 완료된 횟수와 이러한 작업에 대한 특정 날짜도 볼 수 있습니다.</p> </td> 
  </tr> 
  <!-- Features permanently removed from Workfront
  <tr> 
   <td><a href="../enhanced-analytics/resource-capacity-overview.md" class="MCXref xref">View the Resource capacity visualization in Enhanced analytics</a> </td> 
   <td> <p>The <b>Resource capacity</b> visualization shows you which home teams have the capacity to take on more work and which home teams have more work assigned to them than they can complete. Interacting with the visualization allows you to see more details about work completed and available hours for more work.&nbsp;Selecting a team opens the Team capacity visualization.</p> </td> 
  </tr> 
  <tr> 
   <td><a href="../enhanced-analytics/team-capacity-overview.md" class="MCXref xref">View the Team capacity visualization in Enhanced analytics</a> </td> 
   <td> <p>The <b>Team capacity</b> visualization shows you a percentage of the amount of work a home team has completed out of the amount of work assigned to them. Interacting with the visualization allows you to see scheduled hours and planned hours for a specific date, as well as the capacity percentage and whether the home team was over, under, or at capacity on that day.</p> </td> 
  </tr>--> 
 </tbody> 
</table>
