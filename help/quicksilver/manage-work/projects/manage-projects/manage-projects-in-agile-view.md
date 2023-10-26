---
product-area: projects;agile-and-teams
navigation-topic: manage-projects
title: 애자일 보기에서 프로젝트 관리
description: 필요한 계획, 라이선스 유형 및 액세스 Adobe Workfront 계획 팀, Pro, 비즈니스 또는 엔터프라이즈 Workfront 라이선스 유형 액세스 모델에서 검토, 작업 또는 계획 권한 편집 액세스 및 보고서, 대시보드 및 캘린더 생성 기능
author: Alina
feature: Work Management
exl-id: fc633fd6-35b4-4949-8045-22c775002436
source-git-commit: 72511f98e05c160e2ca69def8aa3a929ed62bb40
workflow-type: tm+mt
source-wordcount: '1393'
ht-degree: 0%

---

# 애자일 보기에서 프로젝트 관리

<!--
Required plans, license types, and access

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td> <p><a href="https://www.workfront.com/plans" target="_blank">Adobe Workfront Plan</a> </p> </td> 
   <td> <p>Team, Pro, Business, or Enterprise </p> </td> 
  </tr> 
  <tr> 
   <td> <p>Workfront License Type</p> </td> 
   <td> <p>Review, Work, or Plan </p> </td> 
  </tr> 
   <tr data-mc-conditions="QuicksilverOrClassic.Draft mode"> 
    <td> <p>Permissions in the access model</p> </td> 
    <td> <li>Edit access and ability to create reports, dashboards, and calendars</li> </td> 
   </tr>
 </tbody> 
</table>
-->

일반적으로 애자일 사례(팀 백로그 관리 또는 반복 생성 등)와 관련된 관리 문제 없이 프로젝트에 대한 애자일 기능을 활용할 수 있습니다.

팀 백로그를 사용하고 백로그의 작업에서 반복을 생성할 수 있는 애자일 환경에서 작업하려면 의 지침을 따르십시오 [애자일 환경에서 작업](../../../agile/work-in-an-agile-environment/work-in-an-agile-environment.md).

## 액세스 요구 사항

이 문서의 단계를 수행하려면 다음 액세스 권한이 있어야 합니다.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront 플랜*</td> 
   <td> <p>모든</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront 라이센스*</td> 
   <td> <p>검토 이상</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">액세스 수준 구성*</td> 
   <td> <p>다음 영역에 대한 액세스 편집:</p> 
    <ul> 
     <li> <p>프로젝트</p> </li> 
     <li> <p>보고서, 대시보드, 캘린더</p> </li> 
     <li> <p>필터, 보기, 그룹화</p> </li> 
    </ul> <p>참고: 여전히 액세스 권한이 없는 경우 Workfront 관리자에게 액세스 수준에서 추가 제한을 설정하는지 문의하십시오. Workfront 관리자가 액세스 수준을 수정하는 방법에 대한 자세한 내용은 <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">사용자 정의 액세스 수준 만들기 또는 수정</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">개체 권한</td> 
   <td> <p>프로젝트에 대한 권한 보기</p> <p>추가 액세스 요청에 대한 자세한 내용은 <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">오브젝트에 대한 액세스 요청 </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;보유 중인 플랜, 라이선스 유형 또는 액세스 권한을 확인하려면 Workfront 관리자에게 문의하십시오.

## 애자일 프로젝트 이해

>[!NOTE]
>
>이 섹션은 프로젝트의 보드 보기가 아닌 레거시 애자일 보기에만 적용됩니다.

* [프로젝트의 애자일 기능](#agile-functionality-in-a-project)
* [프로젝트에서 애자일 보기를 사용할 때와 반복에서 사용할 때의 차이점](#differences-when-using-the-agile-view-on-a-project-versus-on-an-iteration)

### 프로젝트의 애자일 기능 {#agile-functionality-in-a-project}

애자일 보기에서 프로젝트를 관리할 때 다음 애자일 기능을 사용할 수 있습니다.

* 완료 상태\
  완료 상태에 대한 자세한 내용은 [반복 완료 상태 개요](../../../agile/use-scrum-in-an-agile-team/burndown/iteration-completion-status-overview.md).

* 스토리보드\
  스토리 보드에 대한 자세한 내용은 [스크럼 보드](../../../agile/use-scrum-in-an-agile-team/scrum-board/scrum-board.md) 섹션.

프로젝트에서 애자일 보기를 사용할 때와 순수 애자일 환경(백로그 및 반복 사용)에서 작업할 때의 몇 가지 차이점이 있습니다. 자세한 내용은 [프로젝트에서 애자일 보기를 사용할 때와 반복에서 사용할 때의 차이점](#differences-when-using-the-agile-view-on-a-project-versus-on-an-iteration) 이 문서에서.

### 프로젝트에서 애자일 보기를 사용할 때와 반복에서 사용할 때의 차이점 {#differences-when-using-the-agile-view-on-a-project-versus-on-an-iteration}

* [작업 및 하위 작업은 스토리 보드에서 다양한 표시 규칙을 따릅니다.](#tasks-and-subtasks-follow-different-display-rules-on-the-story-board)
* [백로그 및 반복은 사용되지 않습니다](#backlogs-and-iterations-are-not-used)
* [작업 순서는 애자일 보기에서 유지되며 순서를 변경할 수 없습니다.](#task-order-is-maintained-in-the-agile-view-and-cannot-be-reordered)
* [작업은 계획된 시간으로만 측정됩니다.](#tasks-are-measured-only-in-planned-hours)
* [애자일 팀이 사용되지 않음](#the-agile-team-is-not-used)
* [프로젝트의 각 사용자는 다른 애자일 보기에서 프로젝트를 볼 수 있습니다](#each-user-on-the-project-can-view-the-project-in-a-different-agile-view)

#### 작업 및 하위 작업은 스토리 보드에서 다양한 표시 규칙을 따릅니다. {#tasks-and-subtasks-follow-different-display-rules-on-the-story-board}

* 상위 작업이나 하위 작업이 없는 작업은 항상 스토리 보드에 단일 스토리 카드로 표시됩니다.\
  예를 들어 이러한 작업은 프로젝트 목록 보기에서 다음과 같이 표시됩니다.

  ![애자일 프로젝트 목록 - 상위 또는 하위 작업이 없는 작업](assets/agile-project-single-list-nwe.png) 이러한 작업은 프로젝트 애자일 보기에 다음과 같이 표시됩니다.

  ![프로젝트 애자일 보기 - 상위 또는 하위 작업이 없는 작업](assets/agile-project-singlecard-nwe.png)

* 하위 작업이 있는 상위 작업은 항상 **스토리** 스토리 보드의 열입니다. 하위 작업이 상위 작업의 스윔레인에 표시됩니다.\
  예를 들어 이러한 작업은 프로젝트 목록 보기에서 다음과 같이 표시됩니다.

  ![애자일 프로젝트 목록 - 상위 및 하위 작업이 있는 작업](assets/agile-project-parent-list-nwe.png)\
  이러한 작업은 프로젝트 애자일 보기에 다음과 같이 표시됩니다.

  ![애자일 프로젝트 보기 - 상위 및 하위 작업이 있는 작업](assets/agile-project-parent-nwe.png)

* 두 번째 수준 하위 작업(하위 작업의 하위 작업)은 바로 위 상위 작업에서 정지된 회색 카드로 표시됩니다.
* 세 번째 수준 하위 작업(하위 작업의 하위 작업)은 스토리 보드에 표시되지 않습니다.

#### 백로그 및 반복은 사용되지 않습니다 {#backlogs-and-iterations-are-not-used}

애자일 보기에서 프로젝트를 볼 때 다음 애자일 구성 요소가 사용되지 않습니다.

* **백로그:** 프로젝트의 작업이 자동으로 스토리로 표시되므로 백로그가 사용되지 않습니다.
* **반복:** 작업이 완료되는 날짜를 정의하기 위해 반복을 생성하는 대신 프로젝트 타임라인에서 현재 지정된 날짜가 작업 날짜가 됩니다.

#### 작업 순서는 애자일 보기에서 유지되며 순서를 변경할 수 없습니다. {#task-order-is-maintained-in-the-agile-view-and-cannot-be-reordered}

애자일 스토리 보드에서 프로젝트를 볼 때 프로젝트에 작업이 표시되는 순서가 유지됩니다.

애자일 보기에서 프로젝트를 볼 때 프로젝트의 작업을 재정렬할 수 없습니다. 작업 순서를 수정하면 종속성이 있을 수 있는 다른 작업에 영향을 줄 수 있으므로 작업 순서를 수정하려면 표준 보기에서 프로젝트를 확인해야 합니다.

#### 작업은 계획된 시간으로만 측정됩니다. {#tasks-are-measured-only-in-planned-hours}

프로젝트의 작업은 항상 계획된 시간 단위로 측정됩니다.

반복에서는 작업(스토리)을 시간 또는 포인트 단위로 측정할 수 있습니다.

#### 애자일 팀이 사용되지 않음 {#the-agile-team-is-not-used}

애자일 팀은 할당된 반복에 대한 작업을 완료하므로 애자일 보기에서 프로젝트를 볼 때 애자일 팀이 사용되지 않습니다.

대신 프로젝트의 모든 사용자는 기본적으로 해당 프로젝트의 애자일 팀이 됩니다.

#### 프로젝트의 각 사용자는 다른 애자일 보기에서 프로젝트를 볼 수 있습니다 {#each-user-on-the-project-can-view-the-project-in-a-different-agile-view}

애자일 반복과 달리 프로젝트의 사용자는 애자일 보기를 직접 사용자 정의할 수 있으며 다른 사용자는 다른 애자일 보기를 사용합니다.

애자일 반복에서는 애자일 스토리 보드에서 사용할 수 있는 정보(예: 사용 가능한 상태 열)가 팀 수준에서 결정됩니다.

애자일 보기를 사용자 지정하는 방법에 대한 자세한 내용은 [애자일 보기 만들기 또는 사용자 지정](../../../reports-and-dashboards/reports/reporting-elements/views-overview.md#customizing-an-agile-view) 위치: [Adobe Workfront의 보기 개요](../../../reports-and-dashboards/reports/reporting-elements/views-overview.md).

## 애자일 보기에서 프로젝트 보기

1. 작업 목록 또는 문제 목록에서 애자일 보기로 보려는 프로젝트로 이동합니다.
1. 다음을 클릭합니다. **보드** 아이콘 ![보드 아이콘](assets/board-icon-for-agile-view.png).

   기본적으로 프로젝트의 보드 보기가 표시됩니다.

   ![프로젝트 게시판 보기](assets/project-agile-board-view.png)

   <!--(Legacy agile view only) If you previously viewed the project in a custom agile view, the project is displayed in that view rather than in the default agile view.-->

1. (선택 사항) **구성** 을 클릭하여 열 및 카드에 대한 옵션을 설정합니다.

   자세한 내용은 [보드 열 관리](/help/quicksilver/agile/get-started-with-boards/manage-board-columns.md) 및 [카드에 표시할 필드 사용자 지정](/help/quicksilver/agile/get-started-with-boards/customize-fields-on-card.md). 프로젝트의 보드 보기에서 열 정책을 정의할 수 없습니다.

1. (선택 사항) **기존 애자일 사용** 보드 보기 대신 레거시 애자일 보기를 사용합니다.

1. (선택 사항 - 이전 애자일 보기 전용) 사용자 정의 애자일 보기를 만들었거나, 다른 사용자가 사용자 정의 애자일 보기를 만들어 공유한 경우, 기본 애자일 보기 대신 볼 수 있습니다.

   다음을 클릭합니다. **보기** 드롭다운 메뉴를 클릭한 다음 보려는 사용자 지정 애자일 보기를 클릭합니다.

   사용자 지정 애자일 보기는 다음에 를 클릭할 때 사용됩니다. **애자일** 아이콘.

   새 애자일 보기를 만드는 방법에 대한 자세한 내용은 [애자일 보기 만들기 및 사용자 지정](#create-and-customize-agile-views).

   프로젝트가 사용자 지정 애자일 보기에 표시됩니다.

1. (조건부 - 이전 애자일 보기만 해당) 프로젝트의 작업이 &quot;신규&quot;, &quot;진행 중&quot; 또는 &quot;완료&quot; 이외의 상태(애자일 보기의 기본 상태)를 사용하는 경우 해당 상태의 작업이 표시되도록 애자일 보기에 추가 상태를 추가해야 합니다.

   작업이 애자일 스토리 보드에 표시되지 않는 상태일 경우 작업 자체가 애자일 스토리 보드에 표시되지 않습니다(하지만 이러한 작업의 완료율은 여전히 상위 작업의 완료율 및 전체 프로젝트의 완료율에 기여함).

   애자일 보기에 상태를 추가하려면 문서의 &quot;애자일 보기 만들기 또는 사용자 지정&quot; 섹션에 설명된 대로 새 애자일 보기를 만들거나 기존 애자일 보기를 사용자 지정합니다 [Adobe Workfront의 보기 개요](../../../reports-and-dashboards/reports/reporting-elements/views-overview.md).

1. (선택 사항) 목록 보기로 돌아가려면 **목록** 아이콘.

## 애자일 보기 만들기 및 사용자 지정 {#create-and-customize-agile-views}

>[!NOTE]
>
>이 섹션은 프로젝트의 보드 보기가 아닌 레거시 애자일 보기에만 적용됩니다.

Workfront의 표준 보기와 마찬가지로 기존 애자일 보기를 사용자 정의하거나 새 애자일 보기를 처음부터 만들 수 있습니다. 표준 보기와 달리 기존 애자일 보기를 기반으로 새 애자일 보기를 만들 수 없습니다.

애자일 보기 만들기 및 사용자 지정에 대한 자세한 내용은 문서의 &quot;애자일 보기 만들기 또는 사용자 지정&quot; 섹션을 참조하십시오 [Adobe Workfront의 보기 개요](../../../reports-and-dashboards/reports/reporting-elements/views-overview.md).

## 기존 애자일 보기 공유

>[!NOTE]
>
>이 섹션은 프로젝트의 보드 보기가 아닌 레거시 애자일 보기에만 적용됩니다.

애자일 보기를 공유하는 방법에 대한 자세한 내용은 [필터, 보기 또는 그룹화 공유](../../../reports-and-dashboards/reports/reporting-elements/share-filter-view-grouping.md).

## 기존 애자일 보기 제거

>[!NOTE]
>
>이 섹션은 프로젝트의 보드 보기가 아닌 레거시 애자일 보기에만 적용됩니다.

보기를 삭제하는 방법에 대한 자세한 내용은 문서의 &quot;보기 제거&quot; 섹션을 참조하십시오 [Adobe Workfront의 보기 개요](../../../reports-and-dashboards/reports/reporting-elements/views-overview.md).
