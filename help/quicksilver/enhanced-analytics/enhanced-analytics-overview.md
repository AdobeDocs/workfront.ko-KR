---
title: 향상된 분석 개요
content-type: overview
product-area: enhanced-analytics
navigation-topic: enhanced-analytics-navigation-topic
description: Enhanced Analytics는 Adobe Workfront에 사전 설치된 시각화를 사용하여 프로젝트 데이터를 보고 계획 및 완료로 트렌드를 식별할 수 있는 강력한 도구입니다. 프로젝트에 대한 이러한 통찰력은 현재 작업을 관리하는 데 도움이 되며 향후 작업에 보다 정확하게 계획을 수립할 수 있도록 해줍니다.
author: Nolan
feature: Reports and Dashboards
exl-id: a14ad57c-859b-43df-84c0-575ccda86e50
source-git-commit: 1b1f3c22b8112cfde5b10bef39076eed11630d0f
workflow-type: tm+mt
source-wordcount: '1354'
ht-degree: 2%

---

# 향상된 분석 개요

Enhanced Analytics는 Adobe Workfront에 사전 설치된 시각화를 사용하여 프로젝트 데이터를 보고 계획 및 완료로 트렌드를 식별할 수 있는 강력한 도구입니다. 프로젝트에 대한 이러한 통찰력은 현재 작업을 관리하는 데 도움이 되며 향후 작업에 보다 정확하게 계획을 수립할 수 있도록 해줍니다.

향상된 분석 기능은 다음을 식별하는 데 도움이 될 수 있습니다.

* 프로젝트를 계획하는 방법
* 프로젝트에 작업이 추가되는 시기
* 다른 프로젝트에 대해 완료되는 작업 양
* 홈 팀이 예약한 시간 또는 일과 비교하여 프로젝트를 완료하는 데 필요한 시간 또는 일수입니다.
* 사용자가 프로젝트 중에 특정 작업을 완료하는 빈도
* 프로젝트 진행 및 프로젝트 내의 개별 작업

![](assets/nwe-full-screen-analytics-350x222.png)

사용 사례를 확인하거나 Enhanced Analytics에서 향후 작업을 위한 현재 작업 및 계획에 대한 자세한 내용은 [향상된 분석 학습 경로](https://one.workfront.com/s/enhanced-analytics-program).

## 전제 조건

Enhanced Analytics 영역에 액세스하려면 다음을 수행해야 합니다.

* 비즈니스 또는 엔터프라이즈 플랜이 있습니다.

   자세한 내용은 [Workfront 플랜](https://www.workfront.com/plans).

* Workfront 관리자가 레이아웃 템플릿에 Enhanced Analytics를 추가하도록 합니다.

   자세한 내용은 [향상된 분석: 레이아웃 템플릿에 분석 추가](https://one.workfront.com/s/managed-content-videos/enhanced-analytics-adding-analytics-to-layout-templates-MCH7URDSIXRREHHHF7TRTYYP2LTE).

프로젝트 및 작업에 대한 정보를 보려면 다음을 수행해야 합니다.

* 액세스 수준에서 프로젝트 및 작업 영역에 대한 보기 권한이 있습니다.

   Workfront 관리자가 액세스 수준을 수정하는 방법에 대한 자세한 내용은 [사용자 정의 액세스 수준 만들기 또는 수정](../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md).

* 특정 작업 및/또는 프로젝트에 대한 보기 권한이 있습니다.

   추가 액세스 요청에 대한 자세한 내용은 [개체에 대한 액세스 요청](../workfront-basics/grant-and-request-access-to-objects/request-access.md).

## Enhanced Analytics 우수 사례

프로젝트에 가장 적합한 데이터를 가져오려면 정확한 계획 시간 및 기간 일수를 갖는 템플릿을 사용하십시오. 또한 사용자가 아래 필드를 최대한 정확하게 입력하고 업데이트하는지 확인해야 합니다.

>[!NOTE]
>
>다음 필드 중 일부는 사용자가 입력하는 정보를 기반으로 Workfront에서 수행하는 계산입니다. 이러한 필드는 수동으로 업데이트할 수 없습니다.

* 계획된 시간

   이것은 작성하기에 가장 중요한 분야이다.

   >[!NOTE]
   >
   >팀에서 계획 시간을 사용하지 않는 경우에도 프로젝트 지속 시간에 따라 일부 데이터를 볼 수 있습니다.\
   >자세한 내용은 섹션을 참조하십시오 [기간 보기](#duration-view) 참조하십시오.

* 프로젝트 이름

   이름은 프로젝트를 설명해야 합니다.

* 프로젝트 상태
* 프로젝트 상태
* 프로젝트 계획 시작 일자
* 계획된 완료 일자
* 프로젝트 실제 시작 날짜
* 프로젝트 실제 종료 날짜
* 프로젝트 기간 시간
* 프로젝트 실제 시간
* 작업 상태(완료된 표시 작업 포함)
* 작업 이름
* 작업 완료율
* 작업 계획 시작 날짜
* 작업 계획된 완료 일자

>[!IMPORTANT]
>
>작업 및 프로젝트를 변경한 사항이 Enhanced Analytics에 반영되는 데 최대 24시간이 걸릴 수 있습니다.

## 기간 보기 {#duration-view}

기본적으로 Burndown 및 프로젝트 트리맵 시각화는 계획된 시간을 기반으로 합니다. 팀이 계획된 시간을 사용하지 않는 경우 프로젝트 지속 시간을 기반으로 하여 이러한 시각화를 볼 수 있습니다.

Enhanced Analytics에서 프로젝트 기간은 다음 수식으로 계산됩니다.

* 계획 일정:

   ```
   Planned Completion Date of the project - Start Date of the project
   ```

* 근무일수:

   ```
   Planned Duration for tasks completed in the selected date range / Typical hours per work day
   ```

   >[!NOTE]
   >
   >8시간은 **업무일 기준 시간**. Adobe Workfront 관리자는 **업무일 기준 시간** 설정 **설정** > **프로젝트 환경 설정** > **프로젝트** > **타임라인**.\
   >자세한 내용은 [시스템 전체 프로젝트 환경 설정 구성](../administration-and-setup/set-up-workfront/configure-system-defaults/set-project-preferences.md).

계획 기간에 대한 자세한 내용은 [프로젝트 기간 개요](../manage-work/projects/planning-a-project/project-duration.md).

## 키보드 단축키

키보드에서 다음 키를 사용하여 Enhanced Analytics 영역에서 특정 작업을 탐색하거나 완료할 수 있습니다.

| 키 | 개 액션 |
|---|---|
| **탭** | 페이지의 각 요소와 페이지에 표시되지 않는 각 시각화에 대한 정보가 있는 테이블로 이동합니다 |
| **입력** | 달력 위젯을 열고, 기존 필터를 삭제하고, 필터 추가 옵션을 열고, 필터 값을 선택/선택 취소하고, 만든 필터를 적용하고, 각 시각화에서 내보내기 옵션을 열고, 번다운, 비행 중인 작업 및 프로젝트 트리맵 시각화에서 드롭다운 메뉴를 엽니다 |
| **화살표 키** | 필터를 추가할 때 필터 옵션을 통해 달력 위젯의 날짜로 이동하고 시각화의 모든 드롭다운 메뉴에서 옵션을 통해 날짜로 이동합니다 |
| **스페이스바** | 달력 위젯에서 날짜를 선택하고, 필터를 추가할 때 필터 유형을 선택하고, 각 시각화의 드롭다운 메뉴에서 내보내기 옵션을 선택하고, 번다운, 비행 중인 작업 및 프로젝트 트리맵 시각화의 드롭다운 메뉴에서 옵션을 선택합니다 |

{style=&quot;table-layout:auto&quot;}

화면 읽기 소프트웨어 또는 플러그인을 사용하는 경우 화면 판독기는 화면 상의 정보를 소리 내어 읽고 위에 나열된 키를 사용할 때 완료하는 작업에 대해 설명합니다.

## 향상된 분석 보기 및 기능

Enhanced Analytics 내의 특정 기능에 대한 세부 사항, 더 자세한 통찰력을 얻기 위해 완료할 수 있는 작업 및 이 데이터에서 배울 수 있는 작업에 대해 자세히 알아보려면 다음 문서를 참조하십시오.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th>문서</th> 
   <th>설명</th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td><a href="../enhanced-analytics/use-enhanced-analytics-filters.md" class="MCXref xref">고급 분석에서 필터 적용</a> </td> 
   <td> <p>사용자 지정 필터, 프로젝트 필드 필터 또는 팀 필터를 적용하여 특정 기준에 맞는 프로젝트만 볼 수 있습니다. 필터를 추가하면 프로젝트 수가 그에 따라 업데이트됩니다.</p> </td> 
  </tr> 
  <tr> 
   <td><a href="../enhanced-analytics/understand-enhanced-analytics-kpis.md" class="MCXref xref">향상된 분석 KPI 이해</a> </td> 
   <td> <p>특정 기간 내의 모든 프로젝트에 대한 KPI(주요 성능 지표)는 화면 맨 위에 있습니다.</p> </td> 
  </tr> 
  <tr> 
   <td> <p><a href="../enhanced-analytics/flight-plan-overview.md" class="MCXref xref">Enhanced Analytics에서 플라이트 계획 시각화 보기</a> </p> </td> 
   <td> <p>다음 <b>플라이트 플랜</b> 시각화는 프로젝트 수명 동안 조건이 변경되었음을 보여줍니다. 시각화와 상호 작용하면 특정 날짜에 대한 자세한 내용을 알 수 있습니다. 프로젝트를 선택하면 플라이트 시각화의 번다운 및 작업이 열립니다.</p> </td> 
  </tr> 
  <tr> 
   <td><a href="../enhanced-analytics/burndown-overview.md" class="MCXref xref">Enhanced Analytics에서 Burndown 시각화 보기</a> </td> 
   <td> <p>다음 <b>번다운</b> 시각화는 프로젝트에서 체류한 실제 시간과 비교하여 프로젝트의 계획된 속도를 보여줍니다. 시각화와 상호 작용하면 특정 날짜에 프로젝트의 조건에 대한 자세한 내용을 알 수 있습니다.</p> </td> 
  </tr> 
  <tr> 
   <td><a href="../enhanced-analytics/tasks-in-flight-overview.md" class="MCXref xref">Enhanced Analytics에서 플라이트 시각화의 작업 보기</a> </td> 
   <td> <p>다음 <b>비행 중인 작업</b> 시각화는 프로젝트 내의 각 작업의 상태를 표시합니다. 시각화와 상호 작용하여 작업을 빠르고 쉽게 변경할 수 있습니다.</p> </td> 
  </tr> 
  <tr> 
   <td><a href="../enhanced-analytics/project-activity-overview.md" class="MCXref xref">Enhanced Analytics에서 프로젝트 활동 시각화 보기</a> </td> 
   <td> <p>다음 <b>프로젝트 활동</b> 시각화는 프로젝트에 지정된 사용자가 Workfront에 로그인하고, 해당 프로젝트에서 작업 상태를 변경하고, 해당 프로젝트에서 작업을 완료했을 때의 히트맵을 보여 줍니다. 시각화와 상호 작용하여 각 사용자에 대해 이러한 세부 사항을 볼 수 있습니다. 이러한 작업에 대한 특정 날짜와 각 작업이 완료된 횟수를 볼 수도 있습니다.</p> </td> 
  </tr> 
  <tr> 
   <td><a href="../enhanced-analytics/project-treemap-overview.md" class="MCXref xref">Enhanced Analytics에서 프로젝트 트리맵 시각화 보기</a> </td> 
   <td> <p>다음 <b>프로젝트 트리맵</b> 시각화는 일부 프로젝트에서 다른 프로젝트에 걸린 시간을 보여줍니다. 시각화와 상호 작용하여 프로젝트의 조건, 계획된 프로젝트 완료 및 실제 프로젝트 완료에 대한 세부 정보를 제공합니다.</p> </td> 
  </tr> 
  <tr> 
   <td><a href="../enhanced-analytics/activity-by-team-overview.md" class="MCXref xref">Enhanced Analytics에서 팀 시각화별 활동 보기</a> </td> 
   <td> <p>다음 <b>팀별 활동</b> 시각화는 홈 팀의 사용자가 Workfront에 로그인하여 작업 상태를 변경하고 작업을 완료한 시간에 대한 히트맵을 보여 줍니다. 시각화와 상호 작용하여 각 개별 사용자에 대해 이러한 세부 사항을 볼 수 있습니다. 이러한 작업에 대한 특정 날짜와 각 작업이 완료된 횟수를 볼 수도 있습니다.</p> </td> 
  </tr> 
  <tr> 
   <td><a href="../enhanced-analytics/resource-capacity-overview.md" class="MCXref xref">Enhanced Analytics에서 리소스 용량 시각화 보기</a> </td> 
   <td> <p>다음 <b>자원 능력</b> 시각화는 더 많은 작업을 수행할 수 있는 능력이 있는 홈 팀과 더 많은 작업을 수행할 수 있는 홈 팀을 표시합니다. 시각화와 상호 작용하여 더 많은 작업을 위해 완료된 작업과 사용 가능한 시간에 대한 자세한 내용을 볼 수 있습니다. 팀을 선택하면 팀 용량 시각화가 열립니다.</p> </td> 
  </tr> 
  <tr> 
   <td><a href="../enhanced-analytics/team-capacity-overview.md" class="MCXref xref">Enhanced Analytics에서 팀 용량 시각화 보기</a> </td> 
   <td> <p>다음 <b>팀 용량</b> 시각화는 홈 팀이 자신에게 할당된 작업 중 완료한 작업 금액의 백분율을 보여줍니다. 시각화와 상호 작용하여 특정 날짜에 대한 예약된 시간 및 계획된 시간과 용량 백분율과 해당 날의 홈 팀이 완료되었는지, 부족했는지 또는 용량인지 볼 수 있습니다.</p> </td> 
  </tr> 
 </tbody> 
</table>
