---
product-area: projects;agile-and-teams
navigation-topic: manage-projects
title: Agile 보기에서 프로젝트 관리
description: 필요한 계획, 라이센스 유형 및 액세스 Adobe Workfront 계획 팀, Pro, Business 또는 Enterprise Workfront 라이선스 유형 액세스 모델의 검토, 작업 또는 계획 권한 편집 액세스 및 보고서, 대시보드 및 달력을 만드는 기능
author: Alina
feature: Work Management
exl-id: fc633fd6-35b4-4949-8045-22c775002436
source-git-commit: a849ecaf6097dcdc924aaab2867f37bf57d5bc09
workflow-type: tm+mt
source-wordcount: '1311'
ht-degree: 0%

---

# Agile 보기에서 프로젝트 관리

필요한 계획, 라이센스 유형 및 액세스

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td> <p><a href="https://www.workfront.com/plans" target="_blank">Adobe Workfront 플랜</a> </p> </td> 
   <td> <p>Team, Pro, Business 또는 Enterprise </p> </td> 
  </tr> 
  <tr> 
   <td> <p><a href="https://one.workfront.com/s/article/Understanding-License-Types-906212506?language=en_US&amp;r=16&amp;ui-comm-runtime-components-aura-components-siteforce-qb.Quarterback.validateRoute=1&amp;ui-communities-components-aura-components-forceCommunity-breadcrumbs.Breadcrumbs.getAncestors=1&amp;ui-communities-components-aura-components-forceCommunity-seoAssistant.SeoAssistant.getSeoData=1&amp;ui-force-components-controllers-recordGlobalValueProvider.RecordGvp.getRecord=1&amp;ui-self-service-components-controller.ArticleTopicList.getTopics=1&amp;ui-self-service-components-controller.ArticleView.getArticleHeaderDetail=1" target="_blank">Workfront 라이선스 유형</a> </p> </td> 
   <td> <p>검토, 작업 또는 계획 </p> </td> 
  </tr> <!--
   <tr data-mc-conditions="QuicksilverOrClassic.Draft mode"> 
    <td> <p>Permissions in the access model</p> </td> 
    <td> <li>Edit access and ability to create reports, dashboards, and calendars</li> </td> 
   </tr>
  --> 
 </tbody> 
</table>

프로젝트에 대해 민첩한 기능을 활용할 수 있습니다

<!--
<MadCap:conditionalText data-mc-conditions="QuicksilverOrClassic.Draft mode">
(such as story boards and burndown charts)
</MadCap:conditionalText>
-->

 팀 백로그 관리 또는 반복 생성과 같이 일반적으로 민첩한 관행이 따르는 관리 문제 없이

팀 백로그를 사용하고 백로그의 작업에서 반복을 만들 수 있는 민첩한 환경에서 작업하려면 다음 지침을 따르십시오. [민첩한 환경에서 작업](../../../agile/work-in-an-agile-environment/work-in-an-agile-environment.md).

## 액세스 요구 사항

이 문서의 절차를 수행하려면 다음 액세스 권한이 있어야 합니다.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront 플랜*</td> 
   <td> <p>모든</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront 라이선스*</td> 
   <td> <p>검토 이상</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">액세스 수준 구성*</td> 
   <td> <p>다음 영역에 대한 액세스 편집:</p> 
    <ul> 
     <li> <p>프로젝트</p> </li> 
     <li> <p>보고서, 대시보드, 달력</p> </li> 
     <li> <p>필터, 보기, 그룹화</p> </li> 
    </ul> <p>참고: 여전히 액세스 권한이 없는 경우 Workfront 관리자에게 액세스 수준에서 추가 제한 사항을 설정하는지 문의하십시오. Workfront 관리자가 액세스 수준을 수정하는 방법에 대한 자세한 내용은 <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">사용자 정의 액세스 수준 만들기 또는 수정</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">개체 권한</td> 
   <td> <p>프로젝트에 대한 권한 보기</p> <p>추가 액세스 요청에 대한 자세한 내용은 <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">개체에 대한 액세스 요청 </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;어떤 계획, 라이선스 유형 또는 액세스 권한을 보유하고 있는지 알아보려면 Workfront 관리자에게 문의하십시오.

## 애자일 프로젝트 이해

* [프로젝트의 민첩한 기능](#agile-functionality-in-a-project)
* [프로젝트에서 Agile 보기를 사용할 때와 반복 시 차이점](#differences-when-using-the-agile-view-on-a-project-versus-on-an-iteration)

### 프로젝트의 민첩한 기능 {#agile-functionality-in-a-project}

애자일 보기에서 프로젝트를 관리할 때에는 다음 애자일 기능을 사용할 수 있습니다.

* 완료 상태\
   완료 상태에 대한 자세한 내용은 [반복 완료 상태 개요](../../../agile/use-scrum-in-an-agile-team/burndown/iteration-completion-status-overview.md).

* 스토리 보드\
   스토리 보드에 대한 자세한 내용은 [스크럼 보드](../../../agile/use-scrum-in-an-agile-team/scrum-board/scrum-board.md) 섹션을 참조하십시오.

프로젝트에서 애자일 보기를 사용할 때와 순수 애자일 환경에서 작업할 때(백로그 및 반복 사용) 몇 가지 차이점이 있습니다. 자세한 내용은 [프로젝트에서 Agile 보기를 사용할 때와 반복 시 차이점](#differences-when-using-the-agile-view-on-a-project-versus-on-an-iteration) 참조하십시오.

### 프로젝트에서 Agile 보기를 사용할 때와 반복 시 차이점 {#differences-when-using-the-agile-view-on-a-project-versus-on-an-iteration}

* [작업 및 하위 작업은 스토리 보드의 다른 표시 규칙을 따릅니다](#tasks-and-subtasks-follow-different-display-rules-on-the-story-board)
* [백로그 및 반복은 사용되지 않습니다](#backlogs-and-iterations-are-not-used)
* [작업 순서는 Agile 보기에서 유지되며 순서를 변경할 수 없습니다](#task-order-is-maintained-in-the-agile-view-and-cannot-be-reordered)
* [작업은 계획 시간으로만 측정됩니다](#tasks-are-measured-only-in-planned-hours)
* [Agile Team이 사용되지 않습니다](#the-agile-team-is-not-used)
* [프로젝트의 각 사용자는 다른 Agile 보기에서 프로젝트를 볼 수 있습니다](#each-user-on-the-project-can-view-the-project-in-a-different-agile-view)

#### 작업 및 하위 작업은 스토리 보드의 다른 표시 규칙을 따릅니다 {#tasks-and-subtasks-follow-different-display-rules-on-the-story-board}

* 상위 작업이나 하위 작업이 없는 작업은 항상 스토리 보드에 단일 스토리 카드로 표시됩니다.\
   예를 들어 이러한 작업은 프로젝트 목록 보기에서 다음과 같이 나타납니다.

   ![Agile 프로젝트 목록 - 상위 또는 하위 작업이 없는 작업](assets/agile-project-single-list-nwe.png) 이러한 작업은 프로젝트 애자일 보기에서 다음과 같이 나타납니다.

   ![프로젝트 애자일 보기 - 상위 또는 하위 작업이 없는 작업](assets/agile-project-singlecard-nwe.png)

* 하위 작업이 있는 상위 작업은 항상 **스토리** 스토리 보드의 열. 하위 작업은 상위 작업의 수영선에 표시됩니다.\
   예를 들어 이러한 작업은 프로젝트 목록 보기에서 다음과 같이 나타납니다.

   ![애자일 프로젝트 목록 - 상위 및 하위 작업이 있는 작업](assets/agile-project-parent-list-nwe.png)\
   이러한 작업은 프로젝트 애자일 보기에서 다음과 같이 나타납니다.

   ![애자일 프로젝트 보기 - 상위 및 하위 작업이 있는 작업](assets/agile-project-parent-nwe.png)

* 두 번째 수준 하위 작업(하위 작업의 하위 작업)은 즉시 상위 작업의 회색 카드로 표시됩니다.
* 하위 작업의 하위 작업 하위 작업 하위 작업은 스토리 보드에 표시되지 않습니다.

#### 백로그 및 반복은 사용되지 않습니다 {#backlogs-and-iterations-are-not-used}

애자일 보기에서 프로젝트를 볼 때 다음과 같은 애자일 구성 요소가 사용되지 않습니다.

* **백로그:** 프로젝트의 모든 작업이 자동으로 스토리로 표시되므로 백로그가 사용되지 않습니다.
* **반복:** 작업이 완료되는 날짜를 정의하기 위해 반복을 만드는 대신 프로젝트 타임라인에서 현재 지정된 일수는 작업 일수가 됩니다.

#### 작업 순서는 Agile 보기에서 유지되며 순서를 변경할 수 없습니다 {#task-order-is-maintained-in-the-agile-view-and-cannot-be-reordered}

프로젝트를 애자일 스토리 보드에서 볼 때 프로젝트에 작업이 나타나는 순서는 유지됩니다.

민첩한 보기에서 프로젝트를 볼 때는 프로젝트의 작업을 재정렬할 수 없습니다. 작업 순서를 수정하면 종속성이 있을 수 있는 다른 작업에 영향을 줄 수 있으므로 작업 순서를 수정하려면 표준 보기에서 프로젝트를 봐야 합니다.

#### 작업은 계획 시간으로만 측정됩니다 {#tasks-are-measured-only-in-planned-hours}

프로젝트의 작업은 항상 계획 시간으로 측정됩니다.

반복에서 작업(스토리)은 시간 또는 지점 단위로 측정할 수 있습니다.

#### Agile Team이 사용되지 않습니다 {#the-agile-team-is-not-used}

애자일 팀은 지정된 반복 작업을 완료하므로 애자일 보기에서 프로젝트를 볼 때는 애자일 팀이 사용되지 않습니다.

대신 프로젝트의 모든 사용자는 기본적으로 해당 프로젝트에 대한 민첩한 팀이 됩니다.

#### 프로젝트의 각 사용자는 다른 Agile 보기에서 프로젝트를 볼 수 있습니다 {#each-user-on-the-project-can-view-the-project-in-a-different-agile-view}

민첩한 반복과 달리, 프로젝트의 사용자는 자신에 대해 애자일 보기를 사용자 지정할 수 있고, 다른 사용자는 다른 애자일 보기를 사용합니다.

민첩한 반복에서, 애자일 스토리 보드에서 사용할 수 있는 정보(예: 사용 가능한 상태 열)는 팀 수준에서 결정됩니다.

애자일 보기를 사용자 지정하는 방법에 대한 자세한 내용은  [애자일 뷰 만들기 또는 사용자 정의](../../../reports-and-dashboards/reports/reporting-elements/views-overview.md#customizing-an-agile-view) in  [Adobe Workfront의 보기 개요](../../../reports-and-dashboards/reports/reporting-elements/views-overview.md). 

## 애자일 보기에서 프로젝트 보기

1. 기민한 보기에서 보려는 프로젝트로 이동합니다.
1. 을(를) 클릭합니다. **애자일** 아이콘.\
   ![애자일 아이콘](assets/agile-icon-nwe.png)\
   프로젝트가 기본 애자일 보기에 표시됩니다.\
   이전에 사용자 지정 애자일 보기에서 프로젝트를 본 경우에는 기본 애자일 보기가 아닌 해당 보기에 프로젝트가 표시됩니다.

1. (선택 사항) 사용자 지정 애자일 보기를 만들었거나 다른 사용자가 사용자 지정 애자일 보기를 만들어 사용자와 공유한 경우, 기본 애자일 보기 대신 볼 수 있습니다.\
   을(를) 클릭합니다. **보기** 드롭다운 메뉴를 클릭한 다음 보려는 사용자 지정 애자일 보기를 클릭합니다.

   사용자 지정 애자일 보기는 다음에 **애자일** 아이콘.\
   새로운 애자일 뷰를 만드는 방법에 대한 자세한 내용은 [애자일 뷰 만들기 및 사용자 정의](#create-and-customize-agile-views).\
   프로젝트가 사용자 지정 애자일 보기에 표시됩니다.

1. (조건부) 프로젝트의 작업이 &quot;신규&quot;, &quot;진행 중&quot; 또는 &quot;완료&quot; 이외의 상태(애자일 보기의 기본 상태)를 사용하는 경우 해당 상태의 작업에 대해 추가 상태를 애자일 보기에 추가해야 합니다.\
   작업이 애자일 스토리 보드에 표시되지 않는 상태에 있는 경우 작업 자체가 애자일 스토리 보드에 표시되지 않습니다(하지만 이러한 작업의 완료율은 상위 작업의 완료율 및 전체 프로젝트의 완료율에 여전히 기여함).\
   애자일 보기에 상태를 추가하려면 문서의 &quot;애자일 보기 만들기 또는 사용자 지정&quot; 섹션에 설명된 대로 새 애자일 보기를 만들거나 기존 애자일 보기를 사용자 지정합니다 [Adobe Workfront의 보기 개요](../../../reports-and-dashboards/reports/reporting-elements/views-overview.md).

1. (선택 사항) 목록 보기로 돌아가려면 **목록** 아이콘.\
   ![](assets/list-icon.png)

## 애자일 뷰 만들기 및 사용자 정의 {#create-and-customize-agile-views}

Workfront의 표준 보기처럼 기존의 애자일 보기를 사용자 지정하거나 처음부터 새로운 애자일 보기를 만들 수 있습니다. 표준 뷰와 달리 기존 애자일 보기를 기반으로 새로운 애자일 뷰를 생성할 수 없습니다.

애자일 보기를 만들고 사용자 지정하는 방법에 대한 자세한 내용은 문서의 &quot;애자일 보기 만들기 또는 사용자 지정&quot; 섹션을 참조하십시오 [Adobe Workfront의 보기 개요](../../../reports-and-dashboards/reports/reporting-elements/views-overview.md). 

## 기존 Agile 보기 공유

기민한 보기를 공유하는 방법에 대한 자세한 내용은 [필터, 보기 또는 그룹화 공유](../../../reports-and-dashboards/reports/reporting-elements/share-filter-view-grouping.md).

## 기존 Agile 보기 제거

보기를 삭제하는 방법에 대한 자세한 내용은 문서의 &quot;보기 제거&quot; 섹션을 참조하십시오 [Adobe Workfront의 보기 개요](../../../reports-and-dashboards/reports/reporting-elements/views-overview.md). 
