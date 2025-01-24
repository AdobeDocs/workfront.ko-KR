---
content-type: overview;reference
navigation-topic: workfront-navigation
title: '[!DNL Adobe Workfront]개 개체 개요'
description: ' [!DNL Adobe Workfront] 에 표시하는 정보는  [!DNL Workfront] 데이터베이스에 저장된 개체로 표시됩니다. 개체는  [!DNL Workfront]의 정보를 유도하는 요소입니다. 이 문서에서 이러한 개체에 대해 자세히 알아보십시오.'
feature: Get Started with Workfront
author: Alina
exl-id: f324f198-5472-4cf2-a46e-7fc24605ca90
source-git-commit: 158af1f48fba264b98108b5f0a573b7904eb875e
workflow-type: tm+mt
source-wordcount: '2424'
ht-degree: 1%

---

# [!DNL Adobe Workfront]개 개체 개요

<!--Audited: 12/2023-->

<!--
<***Linked to several articles, do not remove/ change. 
-->

[!DNL Adobe Workfront]에 표시하는 정보는 [!DNL Workfront] 데이터베이스에 저장된 개체로 표시됩니다. 개체가 [!DNL Workfront]의 정보를 유도하는 요소입니다.

[!DNL Workfront]에서 개체가 정의되는 방식을 이해하는 것이 중요하므로 조직에서 필요한 요구 사항에 적합한 개체를 사용할 수 있습니다.

예를 들어 많은 양의 작업을 계획하는 경우 [!UICONTROL Project] 개체를 사용하여 해당 작업을 정의해야 합니다. 이 작업을 더 작은 계획된 증분으로 나누려면 [!UICONTROL Task] 개체를 사용할 수 있습니다. 계획되지 않고 예기치 않게 발생할 수 있는 적은 양의 작업의 경우 Issue 개체를 사용할 수 있습니다. 프로젝트 그룹의 진행 상황과 예산 및 타임라인 준수를 추적하려면 [!UICONTROL Portfolio] 및 [!UICONTROL 프로그램]에서 구성할 수 있습니다. 작업을 확인하는 데 도움이 되는 다른 요소를 정의하려면 [!UICONTROL 프로젝트], [!UICONTROL 작업], [!UICONTROL 문제] 또는 [!UICONTROL Portfolio]에 저장된 다른 개체(예: [!UICONTROL 문서], [!UICONTROL 업데이트], [!UICONTROL 시간], [!UICONTROL 사용자] 또는 [!UICONTROL 작업 역할])를 사용합니다.

[!UICONTROL 보고서] 및 [!UICONTROL 대시보드]는 모든 사용자가 쉽게 액세스할 수 있도록 시각적으로 [!DNL Workfront]에 있는 데이터의 양을 구성하는 데 도움이 되는 개체의 또 다른 예입니다.

[!DNL Workfront]의 전체 개체 목록은 [API 탐색기](../../../wf-api/general/api-explorer.md)를 참조하십시오.

## 객체의 상호 의존성 및 계층

개체가 [!UICONTROL Workfront]에서 서로 연결되어 있습니다. 예를 들어 작업 또는 문제는 프로젝트 외부에 독립적으로 존재할 수 없습니다. [!UICONTROL 작업] 및 [!UICONTROL 문제]은(는) [!UICONTROL 프로젝트] 개체에 저장된 개체의 예입니다. [!UICONTROL 작업] 및 [!UICONTROL 문제]은(는) 프로젝트에 대한 하위 개체로 간주됩니다.

다음은 [!DNL Workfront]에서 가장 일반적으로 사용되는 개체 중 일부와 해당 부모 및 자식 개체입니다.

| **개체** | **상위 개체** | **자식 개체** |
|---|---|---|
| [!UICONTROL 포트폴리오] |  | [!UICONTROL 프로그램], [!UICONTROL 프로젝트], [!UICONTROL 문서], [!DNL Notes], [!UICONTROL 사용자] |
| [!UICONTROL 프로그램] | [!UICONTROL 포트폴리오] | [!UICONTROL 프로젝트], [!UICONTROL 문서], [!UICONTROL 메모], [!UICONTROL 사용자] |
| [!UICONTROL 프로젝트] | [!UICONTROL Portfolio], [!UICONTROL 프로그램] | [!UICONTROL 작업], [!UICONTROL 문제], [!UICONTROL 문서], [!UICONTROL 메모], [!UICONTROL 시간], [!UICONTROL 사용자] |
| [!UICONTROL 작업] | [!UICONTROL 프로젝트] | [!UICONTROL 문제], [!UICONTROL 하위 작업], [!UICONTROL 문서], [!UICONTROL 메모], [!UICONTROL 시간], [!UICONTROL 사용자] |
| [!UICONTROL 문제] | [!UICONTROL 작업], [!UICONTROL 프로젝트] | [!UICONTROL 문서], [!UICONTROL 메모], [!UICONTROL 시간], [!UICONTROL 사용자] |
| [!UICONTROL 대시보드] |  | [!UICONTROL 보고서], 외부 페이지 |
| [!UICONTROL 보고서] | [!UICONTROL 대시보드] |  |
| [!UICONTROL 그룹] |  | [!UICONTROL 사용자] |
| [!UICONTROL 팀] |  | [!UICONTROL 사용자] |
| [!UICONTROL 사용자] | [!UICONTROL 그룹], [!UICONTROL 팀], [!UICONTROL 회사] | [!UICONTROL 작업 역할] |
| [!UICONTROL 회사] |  | [!UICONTROL 사용자] |
| [!UICONTROL 문서] | [!UICONTROL 작업], [!UICONTROL 문제], [!UICONTROL 프로젝트], [!UICONTROL Portfolio], [!UICONTROL 프로그램], [!UICONTROL 사용자] |  |
| [!UICONTROL 계획]* |  | [!UICONTROL 이니셔티브] |
| [!DNL Goals]* |  | [!UICONTROL 결과], [!UICONTROL 활동] |

[!DNL Workfront]의 전체 개체 목록은 [API 탐색기](../../../wf-api/general/api-explorer.md)를 참조하십시오.

*플랜은 [!DNL Adobe Workfront Scenario Planner]의 개체입니다. [!DNL Scenario Planner]에 대한 자세한 내용은 [시나리오 플래너 [!UICONTROL 개요]](../../../scenario-planner/scenario-planner-overview.md)를 참조하십시오.

*[!UICONTROL 목표]는 [!DNL Adobe Workfront Goals]의 개체입니다. [!DNL Workfront Goals]에 대한 자세한 내용은 [[!DNL Adobe Workfront Goals] 개요](../../../workfront-goals/goal-management/wf-goals-overview.md)를 참조하십시오.


## 개체 이름 사용자 지정

[!DNL Workfront] 관리자는 [!UICONTROL 레이아웃 템플릿]을(를) 사용하여 [!DNL Workfront]에서 개체 이름을 사용자 지정할 수 있습니다.

[!UICONTROL 레이아웃 템플릿]을 사용하여 개체 이름을 사용자 지정하는 방법에 대한 자세한 내용은 [레이아웃 템플릿 만들기 및 관리](../../../administration-and-setup/customize-workfront/use-layout-templates/create-and-manage-layout-templates.md)를 참조하십시오.

레이아웃 템플릿을 사용자 정의하고 사용자에게 할당하면 해당 사용자에게 객체에 대해 사용자 정의된 이름이 표시됩니다. 레이아웃 템플릿에 할당된 사용자에게 웹 애플리케이션의 어디에서든 오브젝트의 기본 이름이 더 이상 표시되지 않습니다.

예를 들어 조직에서 더 많은 양의 작업을 &#39;참여&#39;라고 하는 경우 이름 &#39;[!UICONTROL 프로젝트]&#39;을(를) &#39;참여&#39;로 바꿀 수 있습니다. [!DNL Workfront] 인터페이스에 이름 &#39;[!UICONTROL Project]&#39;이(가) 나타나는 모든 곳에서 &#39;[!UICONTROL Project]&#39; 대신 &#39;Engagement&#39;가 표시됩니다.

>[!NOTE]
>
>[!UICONTROL 레이아웃 템플릿]을(를) 저장한 후 사용자의 새 개체 이름을 표시하려면 해당 사용자가 로그아웃한 후 [!DNL Workfront]에 다시 로그인해야 합니다.

>[!IMPORTANT]
>
>[!DNL Workfront] 설명서는 항상 개체의 기본 이름을 참조합니다. [!DNL Workfront] 관리자는 사용자가 개체 이름의 변경 내용을 반영하지 않는 응용 프로그램의 영역뿐만 아니라 [!DNL Workfront] 설명서를 사용하는 방법을 이해할 수 있도록 개체 이름의 변경 내용을 사용자에게 알리는지 확인합니다.

* [[!UICONTROL 레이아웃 템플릿]을(를) 사용하여 사용자 지정할 수 있는 개체 이름](#object-names-that-can-be-customized-using-a-layout-template)
* [사용자 지정된 개체 이름을 반영하는  [!DNL Workfront] 의 영역](#areas-of-workfront-that-reflect-the-customized-object-names)
* [사용자 지정된 개체 이름을 반영하지 않는  [!DNL Workfront] 의 영역](#areas-of-workfront-that-do-not-reflect-the-customized-object-names)

### [!UICONTROL 레이아웃 템플릿]을(를) 사용하여 사용자 지정할 수 있는 개체 이름

[!DNL Workfront] 관리자는 조직의 용어와 일치하도록 다음 개체의 이름을 사용자 지정할 수 있습니다.

* [!UICONTROL Portfolio]
* [!UICONTROL 프로그램]
* [!UICONTROL 프로젝트]
* [!UICONTROL 작업]
* [!UICONTROL 문제]
* [!UICONTROL 목표]*
* [!UICONTROL 결과]*
* [!UICONTROL 활동]*

  *[!UICONTROL 목표], [!UICONTROL 결과] 및 [!UICONTROL 활동]은(는) 회사에서 [!DNL Workfront Goals]을(를) 구입한 경우에만 사용할 수 있습니다. [!DNL Workfront Goals]에 대한 자세한 내용은 [[!DNL Adobe Workfront Goals] 개요](../../../workfront-goals/goal-management/wf-goals-overview.md)를 참조하십시오.

* [!UICONTROL 이니셔티브]**
* [!UICONTROL 시나리오]**
* [!UICONTROL 계획]**

  **[!UICONTROL 이니셔티브], [!UICONTROL 시나리오] 및 [!UICONTROL 계획]은(는) 회사에서 [!DNL Workfront Scenario Planner]을(를) 구입한 경우에만 사용할 수 있습니다. [!DNL Scenario Planner]에 대한 자세한 내용은 [시작하기 [!DNL Scenario Planner]](../../../scenario-planner/get-started-with-scenario-planning.md)를 참조하십시오.



[!UICONTROL 레이아웃 템플릿]을 사용하여 개체 이름을 사용자 지정하는 방법에 대한 자세한 내용은 [레이아웃 템플릿 만들기 및 관리](../../../administration-and-setup/customize-workfront/use-layout-templates/create-and-manage-layout-templates.md)를 참조하십시오.

Workfront에서 다른 개체의 이름은 사용자 지정할 수 없습니다. [!DNL Workfront]의 전체 개체 목록은 [API 탐색기](../../../wf-api/general/api-explorer.md)를 참조하십시오.

개체 이름을 사용자 지정하면 해당 개체 이름이 표시되는 [!DNL Workfront] 응용 프로그램의 대부분의 영역에 해당 개체의 새 이름이 나타납니다.

### 사용자 지정된 개체 이름을 반영하는 [!DNL Workfront] 영역

다음 영역에는 업데이트된 개체 이름이 표시됩니다.

* 상위 탐색
* 왼쪽 패널 탐색의 모든 섹션
* 모든 메뉴
* 인앱 알림
* Report Builder 및 보고 요소 (보기, 필터 및 그룹화)
* [!UICONTROL 저장] 단추
* 내보낸 파일
* 이메일
* 모바일 앱

### 사용자 지정된 개체 이름을 반영하지 않는 [!DNL Workfront]의 영역

다음 영역에는 업데이트된 개체 이름이 표시되지 않습니다.

<!--
  <li data-mc-conditions="QuicksilverOrClassic.Draft mode"> <p>Referenced Object Type selection for a Typeahead field in a Custom Form </p> <p>(NOTE: drafting this because I don't think this is true)</p> </li>
  -->

* [!DNL Outlook] 추가 기능

### 개체 이름 사용자 지정의 의미

[!DNL Workfront]에서 개체 이름을 사용자 지정할 때는 다음 사항에 유의해야 합니다.

* 시스템 디스플레이에서 양식적 또는 문법적 오류가 발생할 수 있습니다. 예를 들어 &#39;[!UICONTROL 문제]&#39;의 이름을 &#39;요청&#39;으로 바꾸고 시스템의 어느 곳에서든 &#39;요청&#39;이라는 구문이 표시되면 이 구문은 의도한 대로 작동하는 것이므로 버그로 간주해서는 안 됩니다.
* 개체에 대한 사용자 정의 이름을 번역할 수 없습니다. [!DNL Workfront] 기본 이름만 지원되는 언어로 번역할 수 있습니다. [!DNL Workfront]에서 지원되는 언어에 대한 자세한 내용은 [지원되는 언어 [!DNL Adobe Workfront]](../../../workfront-basics/supported-languages-in-workfront.md)를 참조하십시오. 사용자 정의 개체 이름 필드는 모든 언어로 용어를 입력할 수 있도록 외래 문자를 지원합니다.
* [!UICONTROL 레이아웃 템플릿]을(를) 사용하여 개체 이름을 사용자 지정하는 경우 비즈니스 단위(팀 또는 그룹)에 따라 [!UICONTROL 레이아웃 템플릿]을(를) 할당하는 것이 좋습니다.\
   혼동을 피하기 위해 이러한 비즈니스 단위의 사용자가 명확히 이해할 수 있는 이름을 사용하는 것이 좋습니다.
* 전자 메일 알림 및 배달된 보고서에는 항상 전자 메일을 생성하는 사용자의 [!UICONTROL 레이아웃 템플릿]에서 정의한 개체 이름이 포함됩니다. 사용자는 다른 팀 및 그룹의 사용자로부터 이메일 알림을 받는 경우 그룹 또는 팀과 관련되지 않은 이메일의 개체 이름을 볼 수 있도록 준비해야 합니다.\
   [!DNL Workfront] 관리자는 사용자에게 각 개체와 관련된 아이콘을 확인할 것을 권장합니다. 아이콘은 데이터베이스에 나타나는 것처럼 다양한 객체 이름 간에 일관되고 기본 객체와 일관됩니다. 개체와 관련된 모든 [!DNL Workfront] 아이콘 목록은 [개체 아이콘](#object-icons)을 참조하십시오.

  >[!TIP]
  >
  >조직의 일반적인 작업의 경우 용어를 반영하도록 사용자 지정 설명서를 만드는 것이 좋습니다.

## 개체 아이콘

[!DNL Workfront] 설명서는 항상 개체의 기본 이름을 참조합니다. 개체의 이름이 사용자 지정된 경우 해당 개체와 관련된 아이콘을 사용하여 사용자 지정된 개체가 기본 개체 [!DNL Workfront]에 해당하는지 파악할 수 있습니다.

[!DNL Workfront]에서 사용자 지정할 수 있는 개체에 대한 자세한 내용은 [레이아웃 템플릿]](#object-names-that-can-be-customized-using-a-layout-template)을 사용하여 사용자 지정할 수 있는 개체 이름을 참조하십시오.[!UICONTROL 

다음은 Workfront에 있는 개체 및 해당 아이콘 목록입니다.

| **개체** | **아이콘** | **사용자 지정 가능한 개체 이름** |
|---|---|---|
| [!UICONTROL 회사] | ![](assets/company-icon-nwe.png) , ![](assets/nwe-company-icon-54x54.png) |  |
| [!UICONTROL 대시보드] | ![](assets/dashboard-icon-nwe.png) , ![](assets/nwe-dashboards-icon.png) |  |
| [!UICONTROL 목표] | ![](assets/nwe-goal-icon.png) | ✔ |
| [!UICONTROL 그룹] | ![](assets/groups-icon-nwe.png) , ![](assets/nwe-group-icon.png) |  |
| [!UICONTROL 문제] | ![](assets/issue-icon-nwe.png) , ![](assets/nwe-issues-icon.png) | ✔ |
| [!UICONTROL 작업 역할] | ![job_role_icon.png](assets/job-role-icon-52x50.png), ![job_role_icon__1_.png](assets/job-role-icon--1--53x44.png), ![](assets/job-role-nwe-no-color.png), ![](assets/job-role-icon-nwe-color.png) |  |
| [!UICONTROL 계획] | ![](assets/plan-icon.png), ![](assets/nwe-plan-icon-60x57.png) |  |
| [!UICONTROL Portfolio] | ![](assets/portfolio-icon-nwe.png) , ![](assets/nwe-portfolios-icon.png) | ✔ |
| [!UICONTROL 프로그램] | ![](assets/program-icon-nwe.png) , ![](assets/nwe-programs-icon.png) | ✔ |
| [!UICONTROL 프로젝트] | ![](assets/project-icon-nwe.png) , ![](assets/nwe-projects-icon.png) | ✔ |
| [!UICONTROL 보고서] | ![](assets/report-icon-nwe.png) , ![](assets/nwe-reports-icon.png) |  |
| [!UICONTROL 작업] | ![](assets/task-icon-new.png) , ![](assets/nwe-tasks-icon.png) | ✔ |
| [!UICONTROL 팀] | ![](assets/team-icon-nwe.png), ![](assets/team-icon-nwe-color.png), ![](assets/nwe-teams-icon.png) |  |
| [!UICONTROL 템플릿] | ![](assets/template-icon-nwe.png) , ![](assets/nwe-templates-icon.png) |  |
| [!UICONTROL 사용자] | ![](assets/users-icon-gray.png) , ![](assets/user-icon-blue.png) , ![](assets/user-icon-initials.png) , ![](assets/user-avatar.png) , ![](assets/user-main-menu-area.png) |  |

## 개체 참조 번호

[!DNL Workfront]에서 만들어진 각 개체에는 고유한 참조 번호가 할당됩니다. 참조 번호는 다른 유사한 두 객체(예: 동일한 이름을 가진 작업)를 구별하는 데 유용합니다. 참조 번호를 사용하여 객체를 검색할 수 있으며, 보고서에 참조 번호를 포함할 수 있습니다.

참조 번호로 개체를 검색하는 방법에 대한 자세한 내용은 [개체 참조 번호 사용](../../../workfront-basics/navigate-workfront/search/reference-number-of-objects.md)을 참조하십시오.

## 오브젝트별 검색

[!DNL Workfront]에서 검색 가능한 모든 개체를 검색하거나 기본 및 고급 검색에서 검색할 특정 개체를 선택할 수 있습니다.

[!DNL Workfront]에서 모든 개체를 검색할 수 있는 것은 아닙니다. [!DNL Workfront]에서 다음 개체에 대해 기본 및 고급 검색을 실행할 수 있습니다.

| **개체** | **기본 검색** | **고급 검색** |
|---|---|---|
| [!UICONTROL 프로젝트] | ✓ 덧신 | ✓ 덧신 |
| [!UICONTROL 작업] | ✓ 덧신 | ✓ 덧신 |
| [!UICONTROL 문제] | ✓ 덧신 | ✓ 덧신 |
| [!UICONTROL 보고서] | ✓ 덧신 | ✓ 덧신 |
| [!UICONTROL 사용자] | ✓ 덧신 | ✓ 덧신 |
| [!UICONTROL 템플릿] | ✓ 덧신 | ✓ 덧신 |
| [!UICONTROL 문서] | ✓ 덧신 | ✓ 덧신 |
| [!UICONTROL 포트폴리오] | ✓ 덧신 | ✓ 덧신 |
| [!UICONTROL 프로그램] | ✓ 덧신 | ✓ 덧신 |
| [!UICONTROL 대시보드] | ✓ 덧신 | ✓ 덧신 |
| [!UICONTROL 회사] | ✓ 덧신 | ✓ 덧신 |
| [!UICONTROL 메모](또는 [!UICONTROL 업데이트]) | ✓ 덧신 |  |

[!DNL Workfront]에서 기본 및 고급 검색을 실행하는 방법에 대한 자세한 내용은 [검색 [!DNL Adobe Workfront]](../../../workfront-basics/navigate-workfront/search/search-workfront.md)을 참조하십시오.


## 오브젝트에 대한 제한된 액세스

사용자에게 오브젝트에 대한 액세스 권한이 없는 경우 Workfront에 해당 오브젝트 이름이 표시되는 모든 위치에 &quot;액세스 권한 없음&quot;이 표시됩니다.

객체에 대한 액세스는 액세스 수준 또는 특정 객체의 권한으로 제한될 수 있습니다.

이 문서는 이 문서의 [개체의 상호 종속성 및 계층 구조](#interdependency-and-hierarchy-of-objects) 섹션에 나열된 모든 개체 및 자식 개체에 적용됩니다. 팀 및 사용자 개체에는 적용되지 않습니다.

## 오브젝트에 대한 보고서

[!DNL Workfront]에서 보고서를 작성하기 전에 개체의 계층 구조 및 상호 종속성을 이해하는 것이 매우 중요합니다. 보고서는 개체별로 다릅니다. 원하는 데이터를 표시하려면 먼저 보고서에 대한 올바른 개체를 선택해야 합니다.

>[!IMPORTANT]
>
>선택한 객체와 동일한 보고서의 상위 객체에만 보고할 수 있습니다. 상위 객체 보고서에는 하위 객체에 대한 정보가 포함될 수 없습니다. 예를 들어 작업 보고서에는 프로젝트 정보가 표시되지만 프로젝트 보고서에는 작업 정보가 표시되지 않습니다.

Open API를 사용하여 데이터베이스의 모든 개체에 대해 보고할 수 있습니다. 데이터베이스에 있는 모든 개체의 전체 목록을 보려면 [API 탐색기](../../../wf-api/general/api-explorer.md)를 참조하십시오.

>[!NOTE]
>
> * 레이아웃 템플릿을 사용하여 오브젝트의 이름을 사용자 정의한 경우 Report Builder의 오브젝트 이름도 사용자 정의되었습니다. 사용자 정의된 개체를 알고 Report Builder에서 사용자 정의된 이름을 찾습니다. [!DNL Workfront]에서 사용자 지정할 수 있는 개체에 대한 자세한 내용은 이 문서에서 [!UICONTROL 레이아웃 템플릿]](#object-names-that-can-be-customized-using-a-layout-template)을 사용하여 사용자 지정할 수 있는 [개체 이름을 참조하십시오.
> * 보고서에서 텍스트 모드를 사용할 때 텍스트 모드 표현식의 개체 이름은 사용자 지정된 개체 이름이 아니라 [!DNL Workfront]의 표준 이름입니다. 보고서에서 텍스트 모드를 사용하는 방법에 대한 자세한 내용은 [텍스트 모드 개요](../../../reports-and-dashboards/reports/text-mode/understand-text-mode.md)를 참조하십시오.

보고서 작성에 대한 자세한 내용은 [사용자 지정 보고서 만들기](../../../reports-and-dashboards/reports/creating-and-managing-reports/create-custom-report.md)를 참조하십시오.\
API에 대한 자세한 내용은 [API 탐색기](../../../wf-api/general/api-explorer.md)를 참조하십시오.

### 보고서에 사용할 수 있는 객체

[!DNL Workfront] 웹 응용 프로그램에서 Report Builder를 사용할 때 다음 개체에 대해 보고할 수 있습니다. 들여쓴 글머리 기호는 개체에 대한 자세한 정보를 제공하며 추가 개체를 나타내지 않습니다.

* [!UICONTROL 프로젝트]
* [!UICONTROL 작업]
* [!UICONTROL 시간]
* [!UICONTROL 문제]
* [!UICONTROL 사용자]
* [!UICONTROL 액세스] 수준
* [!UICONTROL 승인]
* [!UICONTROL 승인 프로세스]
* [!UICONTROL 할당]
* [!UICONTROL 기준선]
* [!UICONTROL 기준선 작업]
* [!UICONTROL 청구 기록]
* [!UICONTROL 예산 시간]
   * 더 이상 사용되지 않는 이전 리소스 관리 도구에 표시되는 [!UICONTROL 예산 시간]입니다.
   * &quot;싹&quot;이요 [!UICONTROL 예산 시간] 보고서의 &quot;시간&quot; 필드는 [!UICONTROL 리소스 플래너]에서 작업 역할에 대해 예산 책정된 시간을 나타냅니다. 자세한 내용은 [프로젝트 예산 인건비 이해[!UICONTROL 이해] 및 [!UICONTROL 예산 시간]](../../../manage-work/projects/project-finances/budgeted-labor-cost.md)을 참조하세요.

* [!UICONTROL 일정 이벤트]
* [!UICONTROL 회사]
* [!UICONTROL 사용자 정의 양식]
* [!UICONTROL 대시보드]
* [!UICONTROL 문서]
* [!UICONTROL 문서 승인]
* [!UICONTROL 문서 버전]
   * 문서 버전, 버전과 연관된 문서, 버전을 생성한 사람, 문서 버전에서 증명을 생성한 사용자(있는 경우)에 대한 정보를 볼 수 있습니다(증명 생성자).
* [!UICONTROL 전자 메일 템플릿]
* [!UICONTROL 경비]
* [!UICONTROL 경비 유형]
* [!UICONTROL 외부 페이지]
* [!UICONTROL 즐겨찾기]
* [!UICONTROL 필터]
* [!UICONTROL 목표]
   * 전략적 목표에 대한 보고서를 작성하거나 프로젝트가 목표 활동과 연결되어 있을 때 프로젝트 보고서에 목표 관련 정보를 표시할 수 있습니다. 조직에서 [!DNL Workfront Goals] 라이선스를 구입한 경우에만 전략적 목표를 만들고 프로젝트를 연결할 수 있습니다. [!DNL Workfront Goals]에 대한 자세한 내용은 [[!DNL Workfront Goals] 개요](../../../workfront-goals/goal-management/wf-goals-overview.md)를 참조하십시오. 프로젝트를 전략적 목표에 연결하는 방법에 대한 자세한 내용은 [Adobe Workfront 목표의 목표에 프로젝트 추가](../../../workfront-goals/results-and-activities/connect-projects-to-goals-overview.md)를 참조하십시오.
*[!UICONTROL 비즈니스 사례]와(과) 관련된 프로젝트 목표에 대해 보고할 수 없습니다. 프로젝트 목표와 전략 목표에 대한 자세한 내용은 [용어집 [!DNL Adobe Workfront] 용어](../../../workfront-basics/navigate-workfront/workfront-navigation/workfront-terminology-glossary.md)를 참조하십시오.

* [!UICONTROL 그룹]
* [!UICONTROL 그룹화]
* [!UICONTROL 시간 유형]
* [!UICONTROL 이니셔티브]
   * 회사에서 [!DNL Workfront Scenario Planner] 라이선스를 구입한 경우에만 플랜의 하위 개체인 이니셔티브에 대한 보고서를 만들 수 있습니다. 이니셔티브에 대한 자세한 내용은  [!DNL Workfront Scenario Planner]](../../../scenario-planner/initiatives-overview.md)에서 [이니셔티브 개요 를 참조하십시오.

* 이니셔티브 작업 역할
   * 회사에서 [!DNL Workfront Scenario Planner] 라이선스를 구입한 경우에만 플랜의 이니셔티브와 연결된 작업 역할에 대한 보고서를 만들 수 있습니다. 이니셔티브를 만들고 작업 역할과 연결하는 방법에 대한 자세한 내용은 [이니셔티브 만들기 및 편집 [!DNL Workfront Scenario Planner]](../../../scenario-planner/create-and-edit-initiatives.md)을 참조하십시오.

* [!UICONTROL 반복]
* [!UICONTROL 작업 역할]
* [!UICONTROL 저널 게시물]
   * 작업, 프로젝트, 문제 등과 같은 개체의 [!UICONTROL 업데이트] 영역에서 추적된 시스템 업데이트를 보고할 수 있습니다. 자세한 내용은 [저널 게시물 보고서로 업데이트 영역 보고](../../../reports-and-dashboards/reports/creating-and-managing-reports/create-journal-entry-report.md)를 참조하세요.

* [!UICONTROL 레이아웃 템플릿]
* [!UICONTROL 마일스톤]
* [!UICONTROL 마일스톤 경로]
* [!UICONTROL 참고] 또는 [!UICONTROL 업데이트]
   * 개별 사용자가 추가한 댓글에 대해 보고할 수 있습니다.

* [!UICONTROL 매개 변수](또는 [!UICONTROL 사용자 지정 필드])
* [!UICONTROL 매개 변수 그룹](또는 [!UICONTROL 섹션 구분])
* [!UICONTROL Portfolio]
* [!UICONTROL 프로그램]
* [!UICONTROL 프로젝트(재무 데이터)]
   * 재무 정보는 [!UICONTROL 프로젝트(재무 데이터)]에서 채우며, 이 데이터와 관련된 데이터가 5년 미만인 경우에만 보고됩니다. 예를 들어 작업 역할이 2015년 1월에 작업에 할당되었고 오늘이 2021년 9월인 경우 작업 역할에 대한 [!UICONTROL 할당 일자]와 같은 재무 필드가 [!UICONTROL 프로젝트(재무 데이터)] 보고서에 채워지지 않습니다.

  >[!CAUTION]
  >
  >프로젝트(재무 데이터) 보고서를 실행하면 재무 데이터가 다시 계산되어 이전 재무 데이터를 덮어쓸 수 있으며 상당한 시간이 소요될 수 있습니다. 재무 데이터 다시 계산 결과에 대한 자세한 내용은 [프로젝트 재무 다시 계산](/help/quicksilver/manage-work/projects/project-finances/recalculate-project-finances.md)을 참조하십시오.

* [!UICONTROL 교정쇄 승인]
   * 승인을 위해 제출된 증명, [!UICONTROL 승인자]에 대한 정보, 요청자에 대한 정보(요청자가 라이선스가 있는 [!DNL Workfront] 사용자인 경우), 버전 정보, 증명 ID 및 증명 생성 날짜를 포함하여 증명 승인에 대한 다양한 정보를 볼 수 있습니다.\
      [!UICONTROL 증명 승인] 보고서에는 아직 결정이 내려지지 않은 사용자의 내 작업 영역에서 사용할 수 있는 증명만 포함됩니다.\
   * [내에서 증명 공유 [!DNL Adobe Workfront]](../../../review-and-approve-work/proofing/managing-proofs-within-workfront/share-a-proof-in-workfront.md)의 [증명에 사용자 추가](../../../review-and-approve-work/proofing/managing-proofs-within-workfront/share-a-proof-in-workfront.md#add)에 설명된 대로 [!DNL Workfront]에서 증명 승인이 할당됩니다.

* [!UICONTROL 큐]
* [!UICONTROL 대기열 주제]
* [!UICONTROL 요금](작업 역할 [!UICONTROL 청구 요금] 정보를 표시함)
* [!UICONTROL 미리 알림]
* [!UICONTROL 보고서]
* [!UICONTROL 리소스 풀]
* [!UICONTROL 위험]
* [!UICONTROL 위험 유형]
* [!UICONTROL 예약]
* [!UICONTROL 스코어카드]
* [!UICONTROL 팀]
* [!UICONTROL 템플릿]
* [!UICONTROL 템플릿 작업]
* [!UICONTROL 휴무]
   * 프로필에서 사용자가 지정한 대로 사용자의 휴무를 보고할 수 있습니다.

* [!UICONTROL 타임시트]
* [!UICONTROL 타임시트 프로필]
* [!UICONTROL 주제 그룹]
* [!UICONTROL 사용자 승인]
* [!UICONTROL 사용자 위임]

   * 부재 중 다른 사람의 작업 및 문제를 수행하도록 위임된 사용자에 대해 보고할 수 있습니다. 이 보고서에는 부재 중인 사용자와 부재 중 직무를 수행하는 사용자가 표시됩니다.

* [!UICONTROL 사용자 결정]

   * 이번 달에 사용자가 증명 및 문서에 대해 내린 결정 횟수를 보고할 수 있습니다.

* [!UICONTROL 보기]
* [!UICONTROL 작업 항목](작업 및 문제에 대한 보고서 생성)
