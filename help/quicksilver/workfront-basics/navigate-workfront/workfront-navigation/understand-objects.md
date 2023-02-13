---
content-type: overview;reference
navigation-topic: workfront-navigation
title: 의 개체 이해 [!DNL Adobe Workfront]
description: 의 개체 이해 [!DNL Adobe Workfront]
feature: Get Started with Workfront
exl-id: f324f198-5472-4cf2-a46e-7fc24605ca90
source-git-commit: 9c78d8e08e62c86a4e1340644ed76c61ce7f2674
workflow-type: tm+mt
source-wordcount: '2308'
ht-degree: 6%

---

# 의 개체 이해 [!DNL Adobe Workfront]

<!--
<***Linked to several articles, do not remove/ change. 
-->

표시되는 정보 [!DNL Adobe Workfront] 는 [!DNL Workfront] 데이터베이스. 개체는 정보를 유도하는 것입니다 [!DNL Workfront].

객체정의방법 이해 [!DNL Workfront] 는 조직에서 필요한 요구 사항에 올바른 개체를 사용할 수 있도록 중요한 것입니다.

예를 들어 많은 양의 작업을 계획할 때 [!UICONTROL 프로젝트] 작업을 정의하는 개체입니다. 이 작업을 작은 계획된 증분으로 분할하려면 [!UICONTROL 작업] 개체. 계획되지 않은 작업량이 적고 예기치 않게 발생할 수 있는 경우 Issue 개체를 사용할 수 있습니다. 프로젝트 그룹의 진행 상황과 예산 및 타임라인 준수를 추적하려는 경우,에서 이를 구성할 수 있습니다 [!UICONTROL Portfolio] 및 [!UICONTROL 프로그램]. 작업을 해결하는 데 도움이 되는 다른 요소를 정의하려면 아래에 저장된 다른 객체를 사용합니다 [!UICONTROL 프로젝트], [!UICONTROL 작업], [!UICONTROL 문제], 또는 [!UICONTROL Portfolio]과 비슷함 [!UICONTROL 문서], [!UICONTROL 참고], [!UICONTROL 시간], [!UICONTROL 사용자], 또는 [!UICONTROL 작업 역할].

[!UICONTROL 보고서] 및 [!UICONTROL 대시보드] 에 있는 데이터의 양을 구성하는 데 도움이 되는 개체의 또 다른 예입니다 [!DNL Workfront] 시각적으로, 모든 사용자가 쉽게 액세스할 수 있도록 합니다.

의 전체 개체 목록 [!DNL Workfront]를 참조하고 [API 탐색기](../../../wf-api/general/api-explorer.md).

## 개체의 상호 종속성 및 계층

개체는에서 서로 연결되어 있습니다 [!UICONTROL Workfront]. 예를 들어 작업이나 문제는 프로젝트 외부에서 독립적으로 존재할 수 없습니다. [!UICONTROL 작업] 및 [!UICONTROL 문제] 는 [!UICONTROL 프로젝트] 개체. [!UICONTROL 작업] 및 [!UICONTROL 문제] 는 프로젝트에 하위 개체로 간주됩니다.

다음은 에서 가장 일반적으로 사용되는 객체 중 일부입니다 [!DNL Workfront] 및 각각의 부모 및 자식 객체

| **오브젝트** | **상위 개체** | **하위 개체** |
|---|---|---|
| [!UICONTROL 포트폴리오] |  | [!UICONTROL 프로그램], [!UICONTROL 프로젝트], [!UICONTROL 문서], [!DNL Notes], [!UICONTROL 사용자] |
| [!UICONTROL 프로그램] | [!UICONTROL 포트폴리오] | [!UICONTROL 프로젝트], [!UICONTROL 문서], [!UICONTROL 참고], [!UICONTROL 사용자] |
| [!UICONTROL 프로젝트] | [!UICONTROL Portfolio], [!UICONTROL 프로그램] | [!UICONTROL 작업], [!UICONTROL 문제], [!UICONTROL 문서], [!UICONTROL 참고], [!UICONTROL 시간], [!UICONTROL 사용자] |
| [!UICONTROL 작업] | [!UICONTROL 프로젝트] | [!UICONTROL 문제], [!UICONTROL 하위 작업], [!UICONTROL 문서], [!UICONTROL 참고], [!UICONTROL 시간], [!UICONTROL 사용자] |
| [!UICONTROL 문제] | [!UICONTROL 작업], [!UICONTROL 프로젝트] | [!UICONTROL 문서], [!UICONTROL 참고], [!UICONTROL 시간], [!UICONTROL 사용자] |
| [!UICONTROL 대시보드] |  | [!UICONTROL 보고서], 외부 페이지 |
| [!UICONTROL 보고서] | [!UICONTROL 대시보드] |  |
| [!UICONTROL 그룹] |  | [!UICONTROL 사용자] |
| [!UICONTROL 팀] |  | [!UICONTROL 사용자] |
| [!UICONTROL 사용자] | [!UICONTROL 그룹], [!UICONTROL 팀], [!UICONTROL 회사] | [!UICONTROL 작업 역할] |
| [!UICONTROL 회사] |  | [!UICONTROL 사용자] |
| [!UICONTROL 문서] | [!UICONTROL 작업], [!UICONTROL 문제], [!UICONTROL 프로젝트], [!UICONTROL Portfolio], [!UICONTROL 프로그램], [!UICONTROL 사용자] |  |
| [!UICONTROL 플랜]* |  | [!UICONTROL 이니셔티브] |
| [!DNL Goals]* |  | [!UICONTROL 결과], [!UICONTROL 활동] |

의 전체 개체 목록 [!DNL Workfront]를 참조하고 [API 탐색기](../../../wf-api/general/api-explorer.md).

*계획은 [!DNL Workfront Scenario Planner]. 에 대한 정보 [!DNL Scenario Planner]를 참조하십시오. [다음 [!UICONTROL 시나리오 플래너] 개요](../../../scenario-planner/scenario-planner-overview.md).

*[!UICONTROL 목표] 의 개체입니다 [!DNL Workfront Goals]. 에 대한 자세한 정보 [!DNL Workfront Goals]를 참조하십시오. [[!DNL Adobe Workfront Goals] 개요](../../../workfront-goals/goal-management/wf-goals-overview.md).


## 개체 이름 사용자 지정

로서의 [!DNL Workfront] 관리자는 [!DNL Workfront] 사용  [!UICONTROL 레이아웃 템플릿].

를 사용하여 개체 이름을 사용자 지정하는 방법에 대한 자세한 정보  [!UICONTROL 레이아웃 템플릿]를 참조하십시오. [레이아웃 템플릿 만들기 및 관리](../../../administration-and-setup/customize-workfront/use-layout-templates/create-and-manage-layout-templates.md).

레이아웃 템플릿을 사용자 지정하고 사용자에게 할당하면 해당 사용자는 객체에 대해 사용자 지정된 이름을 볼 수 있습니다. 레이아웃 템플릿에 할당된 사용자는 더 이상 웹 응용 프로그램의 모든 위치에 개체의 기본 이름을 볼 수 없습니다.

>[!NOTE]
>
>사용자가 볼 수 있는 객체의 새 이름을 보려면 로그아웃한 다음 다시 로그인해야 합니다 [!DNL Workfront] 저장한 후  [!UICONTROL 레이아웃 템플릿].

>[!IMPORTANT]
>
>다음 [!DNL Workfront] 설명서는 항상 객체의 기본 이름을 참조합니다. 로서의 [!DNL Workfront] 관리자는 사용자에게 개체 이름의 변경 내용을 알리고 사용자가 [!DNL Workfront] 객체 이름의 변경 사항을 반영하지 않는 응용 프로그램의 영역뿐 아니라 설명서입니다.

* [를 사용하여 사용자 지정할 수 있는 개체 이름  [!UICONTROL 레이아웃 템플릿]](#object-names-that-can-be-customized-using-a-layout-template)
* [영역 [!DNL Workfront] 사용자 지정된 개체 이름을 반영합니다](#areas-of-workfront-that-reflect-the-customized-object-names)
* [영역 [!DNL Workfront] 사용자 지정된 개체 이름을 반영하지 않습니다](#areas-of-workfront-that-do-not-reflect-the-customized-object-names)

### 를 사용하여 사용자 지정할 수 있는 개체 이름 [!UICONTROL 레이아웃 템플릿]

로서의 [!DNL Workfront] 관리자는 조직의 용어와 일치하도록 다음 객체의 이름을 사용자 정의할 수 있습니다.

* [!UICONTROL 포트폴리오]
* [!UICONTROL 프로그램]
* [!UICONTROL 프로젝트]
* [!UICONTROL 작업]
* [!UICONTROL 문제]
* [!UICONTROL 목표]*
* [!UICONTROL 결과]*
* [!UICONTROL 활동]*

   *[!UICONTROL 목표], [!UICONTROL 결과], 및 [!UICONTROL 활동] 은 회사가 구입한 경우에만 사용할 수 있습니다 [!DNL Workfront Goals]. 에 대한 자세한 정보 [!DNL Workfront Goals]를 참조하십시오. [[!DNL Adobe Workfront Goals] 개요](../../../workfront-goals/goal-management/wf-goals-overview.md).

* [!UICONTROL 이니셔티브]**
* [!UICONTROL 시나리오]**
* [!UICONTROL 플랜]**

   **[!UICONTROL 이니셔티브], [!UICONTROL 시나리오], 및 [!UICONTROL 플랜] 는 회사가 구입한 경우에만 사용할 수 있습니다 [!DNL Workfront Scenario Planner]. 에 대한 정보 [!DNL Scenario Planner]를 참조하십시오. [시작하기 [!DNL Scenario Planner]](../../../scenario-planner/get-started-with-scenario-planning.md).


예를 들어 조직에서 많은 양의 작업을 &#39;참여&#39;라고 하는 경우 이름을 &#39;[!UICONTROL 프로젝트]&#39; &#39;Engagement&#39;가 포함된 경우 사용자 [!DNL Workfront] 인터페이스에 &#39; 대신 &#39;Engagement&#39;가 표시됩니다.[!UICONTROL 프로젝트]&#39; 이름이 &#39; 인 모든 위치[!UICONTROL 프로젝트]&#39; 이(가) 나타납니다.

를 사용하여 개체 이름을 사용자 지정하는 방법에 대한 자세한 정보  [!UICONTROL 레이아웃 템플릿]를 참조하십시오. [레이아웃 템플릿 만들기 및 관리](../../../administration-and-setup/customize-workfront/use-layout-templates/create-and-manage-layout-templates.md).

Workfront에 있는 다른 개체의 이름을 사용자 지정할 수 없습니다. 의 전체 개체 목록 [!DNL Workfront]를 참조하고 [API 탐색기](../../../wf-api/general/api-explorer.md).

객체 이름을 사용자 지정하면 해당 객체의 새 이름이 [!DNL Workfront] 객체 이름이 표시되는 응용 프로그램입니다.

### 영역 [!DNL Workfront] 사용자 지정된 개체 이름을 반영합니다

다음 영역은 객체의 업데이트된 이름을 보여 줍니다.

* 상위 탐색
* 왼쪽 패널 탐색의 모든 섹션
* 모든 메뉴
* 인앱 알림
* Report Builder 및 보고 요소(보기, 필터 및 그룹화)
* [!UICONTROL 저장] 버튼
* 내보낸 파일
* 이메일
* 모바일 앱

### 영역 [!DNL Workfront] 사용자 지정된 개체 이름을 반영하지 않습니다

다음 영역에는 객체의 업데이트된 이름이 표시되지 않습니다.

<!--
  <li data-mc-conditions="QuicksilverOrClassic.Draft mode"> <p>Referenced Object Type selection for a Typeahead field in a Custom Form </p> <p>(NOTE: drafting this because I don't think this is true)</p> </li>
  -->

* [!DNL Outlook] 추가 기능

## 개체 이름 사용자 지정에 대한 의미

에서 개체 이름을 사용자 지정할 때는 다음 사항을 알고 있어야 합니다 [!DNL Workfront]:

* 시스템 디스플레이에서 문법 또는 문법 오류가 발생할 수 있습니다. 예를 들어 &#39;[!UICONTROL 문제]&#39;Request&#39;를 &#39;Request&#39;로 변경하여 &#39;An request&#39;라는 구문을 시스템의 어느 곳에서든 볼 수 있게 되면 이는 의도한 대로 작동하므로 버그로 간주해서는 안 됩니다.
* 개체의 사용자 지정 이름이 번역 가능하지 않습니다. 전용 [!DNL Workfront] 기본 이름은 지원되는 언어로 번역될 수 있습니다. 에서 지원되는 언어에 대한 자세한 내용은 [!DNL Workfront]를 참조하십시오. [의 지원되는 언어 [!DNL Adobe Workfront]](../../../workfront-basics/supported-languages-in-workfront.md). 사용자 지정 개체 이름 필드는 모든 언어로 용어를 입력할 수 있도록 외부 문자를 지원합니다.
* 를 사용하여 개체 이름을 사용자 정의할 때  [!UICONTROL 레이아웃 템플릿]를 지정하는 것이 좋습니다  [!UICONTROL 레이아웃 템플릿] 비즈니스 단위(팀 또는 그룹)에 대한 정보.\
   혼동을 방지하기 위해 이러한 사업부 사용자가 명확하게 이해할 수 있는 이름을 사용하는 것이 좋습니다.
* 전자 메일 알림 및 게재된 보고서에는 항상  [!UICONTROL 레이아웃 템플릿] 이메일을 생성하는 사용자의 이름입니다. 사용자는 다른 팀 및 그룹의 사용자로부터 이메일 알림을 받는 경우 해당 그룹 또는 팀과 관련이 없는 이메일에 개체 이름을 볼 준비가 되어 있어야 합니다.\
   로서의 [!DNL Workfront] 관리자는 사용자에게 각 객체와 연관된 아이콘을 알 수 있도록 합니다. 아이콘은 데이터베이스에 나타나는 것처럼 다양한 객체 이름 간에 일관되며 기본 객체와 일치합니다. 모든 [!DNL Workfront] 객체와 연관된 아이콘은 [개체 아이콘](#object-icons).

   >[!TIP]
   >
   >조직의 일반적인 작업에 대해서는 용어를 반영하도록 사용자 지정 설명서를 만드는 것이 좋습니다.

## 개체 아이콘

다음 [!DNL Workfront] 설명서는 항상 객체의 기본 이름을 참조합니다. 객체의 이름이 사용자 지정된 경우 해당 객체와 연관된 아이콘을 사용하여 해당 객체에 대응하는 사용자 정의 객체를 파악할 수 있습니다 [!DNL Workfront] 기본 개체입니다.

에서 사용자 지정할 수 있는 객체에 대한 자세한 내용은 [!DNL Workfront]를 참조하십시오. [를 사용하여 사용자 지정할 수 있는 개체 이름  [!UICONTROL 레이아웃 템플릿]](#object-names-that-can-be-customized-using-a-layout-template).

다음은 Workfront의 개체 및 해당 아이콘 목록입니다.

| **오브젝트** | **아이콘** | **사용자 지정 가능한 개체 이름** |
|---|---|---|
| [!UICONTROL 회사] | ![](assets/company-icon-nwe.png)  , ![](assets/nwe-company-icon-54x54.png) |  |
| [!UICONTROL 대시보드] | ![](assets/dashboard-icon-nwe.png)  , ![](assets/nwe-dashboards-icon.png) |  |
| [!UICONTROL 목표] | ![](assets/nwe-goal-icon.png) | ✔ |
| [!UICONTROL 그룹] | ![](assets/groups-icon-nwe.png)  , ![](assets/nwe-group-icon.png) |  |
| [!UICONTROL 문제] | ![](assets/issue-icon-nwe.png)  , ![](assets/nwe-issues-icon.png) | ✔ |
| [!UICONTROL 작업 역할] | ![job_role_icon.png](assets/job-role-icon-52x50.png), ![job_role_icon__1_.png](assets/job-role-icon--1--53x44.png), ![](assets/job-role-nwe-no-color.png), ![](assets/job-role-icon-nwe-color.png) |  |
| [!UICONTROL 플랜] | ![](assets/plan-icon.png), ![](assets/nwe-plan-icon-60x57.png) |  |
| [!UICONTROL 포트폴리오] | ![](assets/portfolio-icon-nwe.png)  , ![](assets/nwe-portfolios-icon.png) | ✔ |
| [!UICONTROL 프로그램] | ![](assets/program-icon-nwe.png)  , ![](assets/nwe-programs-icon.png) | ✔ |
| [!UICONTROL 프로젝트] | ![](assets/project-icon-nwe.png)  , ![](assets/nwe-projects-icon.png) | ✔ |
| [!UICONTROL 보고서] | ![](assets/report-icon-nwe.png) , ![](assets/nwe-reports-icon.png) |  |
| [!UICONTROL 작업] | ![](assets/task-icon-new.png)  , ![](assets/nwe-tasks-icon.png) | ✔ |
| [!UICONTROL 팀] | ![](assets/team-icon-nwe.png), ![](assets/team-icon-nwe-color.png) , ![](assets/nwe-teams-icon.png) |  |
| [!UICONTROL 템플릿] | ![](assets/template-icon-nwe.png)  , ![](assets/nwe-templates-icon.png) |  |

## 개체 참조 번호

에서 만들어진 각 개체 [!DNL Workfront] 에는 고유한 참조 번호가 지정됩니다. 참조 번호는 같은 이름의 작업과 같이 서로 유사한 두 개체를 구별할 때 유용합니다. 참조 번호를 사용하여 객체를 검색할 수 있으며 보고서에 참조 번호를 포함할 수 있습니다.

참조 번호별로 객체를 검색하는 방법에 대한 자세한 내용은 [개체 참조 번호 사용](../../../workfront-basics/navigate-workfront/search/reference-number-of-objects.md).

## 개체별 검색

에서 검색할 수 있는 모든 개체를 검색할 수 있습니다 [!DNL Workfront]또는 기본 및 고급 검색에서 검색할 특정 개체를 선택할 수 있습니다.

일부 개체는에서 검색할 수 없습니다 [!DNL Workfront]. 에서 다음 개체에 대해 기본 및 고급 검색을 실행할 수 있습니다 [!DNL Workfront]:

| **오브젝트** | **기본 검색** | **고급 검색** |
|---|---|---|
| [!UICONTROL 프로젝트] | ✓ | ✓ |
| [!UICONTROL 작업] | ✓ | ✓ |
| [!UICONTROL 문제] | ✓ | ✓ |
| [!UICONTROL 보고서] | ✓ | ✓ |
| [!UICONTROL 사용자] | ✓ | ✓ |
| [!UICONTROL 템플릿] | ✓ | ✓ |
| [!UICONTROL 문서] | ✓ | ✓ |
| [!UICONTROL 포트폴리오] | ✓ | ✓ |
| [!UICONTROL 프로그램] | ✓ | ✓ |
| [!UICONTROL 대시보드] | ✓ | ✓ |
| [!UICONTROL 회사] | ✓ | ✓ |
| [!UICONTROL 메모] | ✓ |  |

기본 및 고급 검색 실행에 대한 자세한 내용은 [!DNL Workfront]를 참조하십시오. [검색 [!DNL Adobe Workfront]](../../../workfront-basics/navigate-workfront/search/search-workfront.md).

## 객체에 대한 보고서

에서 보고서 작성을 시작하기 전에 개체의 계층 구조 및 상호 종속성을 이해하는 것이 매우 중요합니다 [!DNL Workfront]. 보고서는 개체별로 다릅니다. 원하는 데이터를 표시하려면 먼저 보고서에 대한 올바른 개체를 선택해야 합니다.

보고서에 대해 선택한 객체에 따라 보고서의 객체에 직접 연결된 객체만 액세스할 수 있습니다.

>[!IMPORTANT]
>
>선택한 객체와 동일한 보고서의 상위 객체만 보고할 수 있습니다. 상위 객체 보고서의 하위 객체에 대한 정보를 가질 수 없습니다. 예를 들어, 프로젝트 정보는 작업 보고서에 표시할 수 있지만 프로젝트 보고서에는 작업 정보가 표시되지 않습니다.

열린 API를 사용하여 데이터베이스의 모든 개체에 대해 보고할 수 있습니다. 데이터베이스의 모든 개체 전체 목록을 보려면 [API 탐색기](../../../wf-api/general/api-explorer.md).

>[!NOTE]
>
>레이아웃 템플릿을 사용하여 개체의 이름을 사용자 지정한 경우 Report Builder의 개체 이름도 사용자 지정되었습니다. 사용자 지정된 개체를 파악하고 Report Builder에서 사용자 지정된 이름을 찾습니다. 에서 사용자 지정할 수 있는 객체에 대한 자세한 내용은 [!DNL Workfront]를 참조하십시오. *[를 사용하여 사용자 지정할 수 있는 개체 이름  [!UICONTROL 레이아웃 템플릿]](#object-names-that-can-be-customized-using-a-layout-template).*
>보고서에서 텍스트 모드를 사용할 때 텍스트 모드 표현식의 개체 이름은 [!DNL Workfront]및 사용자 지정된 개체 이름이 아닙니다. 보고서에서 텍스트 모드를 사용하는 방법에 대한 자세한 내용은 [텍스트 모드 개요](../../../reports-and-dashboards/reports/text-mode/understand-text-mode.md).

보고서 작성에 대한 자세한 내용은 [사용자 지정 보고서 만들기](../../../reports-and-dashboards/reports/creating-and-managing-reports/create-custom-report.md).\
API에 대한 자세한 내용은 [API 탐색기](../../../wf-api/general/api-explorer.md).

에서 Report Builder를 사용할 때 다음 개체에 대해 보고할 수 있습니다 [!DNL Workfront] 웹 애플리케이션:

* [!UICONTROL 프로젝트]
* [!UICONTROL 작업]
* [!UICONTROL 시간]
* [!UICONTROL 문제]
* [!UICONTROL 사용자]
* [!UICONTROL 액세스 수준]
* [!UICONTROL 승인]
* [!UICONTROL 승인 진행]
* [!UICONTROL 할당]
* [!UICONTROL 백로그 작업 항목]\
   빠른 백로그에 작업 또는 문제를 표시합니다. 애자일 백로그에 대한 자세한 내용은 [애자일 백로그 관리](../../../agile/work-in-an-agile-environment/manage-the-agile-backlog.md).

* [!UICONTROL 기준선]
* [!UICONTROL 기준선 작업]
* [!UICONTROL 청구 기록]
* [!UICONTROL 예산 시간]

   이것은 [!UICONTROL 예산책정된 시간]이전의 사용되지 않는 리소스 관리 도구에서 표시된에 표시됩니다.

   &quot;버드&quot; 시간(시)&quot; 필드 [!UICONTROL 예산책정 시간] 보고서는 [!UICONTROL 리소스 플래너]. 자세한 내용은 [이해 [!UICONTROL 예산책정된 인건비] 및 [!UICONTROL 예산책정된 시간] 프로젝트](../../../manage-work/projects/project-finances/budgeted-labor-cost.md).

* [!UICONTROL 캘린더 이벤트]
* [!UICONTROL 카테고리] 또는 [!UICONTROL 사용자 지정 양식])
* [!UICONTROL 회사]
* [!UICONTROL 대시보드]
* [!UICONTROL 문서]
* [!UICONTROL 문서 승인]
* [!UICONTROL 문서 버전]\
   문서 버전, 버전이 연결된 문서, 버전을 만든 사용자, 문서 버전 증명을 만든 사용자(증명 생성자)에 대한 다양한 정보를 볼 수 있습니다.
* [!UICONTROL 이메일 템플릿]
* [!UICONTROL 경비]
* [!UICONTROL 경비 유형]
* [!UICONTROL 외부 페이지]
* [!UICONTROL 즐겨찾기]
* [!UICONTROL 필터]
* [!UICONTROL 목표]

   전략적 목표에 대한 보고서를 작성하거나, 프로젝트가 목표 활동과 연결되어 있을 때 프로젝트 보고서에 목표 관련 정보를 표시할 수 있습니다. 조직에서 전략적 목표를 구입한 경우에만 전략적 목표를 만들고 프로젝트를 연결할 수 있습니다 [!DNL Workfront Goals] 라이센스. 에 대한 자세한 정보 [!DNL Workfront Goals]를 참조하십시오. [[!DNL Workfront Goals] 개요](https://one.workfront.com/s/document-item?bundleId=the-new-workfront-experience&amp;topicId=Content%2FWorkfront_Goals%2FGoal_management%2Fwf-goals-overview.htm&amp;_LANG=en). 프로젝트를 전략적 목표에 연결하는 방법에 대한 자세한 내용은 [Adobe Workfront 목표의 목표에 프로젝트 추가](https://one.workfront.com/s/document-item?bundleId=the-new-workfront-experience&amp;topicId=Content%2FWorkfront_Goals%2FResults_and_activities%2Fconnect-projects-to-goals-overview.htm&amp;_LANG=en).

   <!--
  <MadCap:conditionalText data-mc-conditions="QuicksilverOrClassic.Draft mode">
  (NOTE: hardcoded links in this paragraph)
  </MadCap:conditionalText>
  -->

   >[!TIP]
   >
   >와 연결된 프로젝트 목표에 대해서는 보고할 수 없습니다 [!UICONTROL 비즈니스 사례]. 프로젝트 목표와 전략적 목표에 대한 자세한 내용은 [용어 설명 [!DNL Adobe Workfront] 용어](../../../workfront-basics/navigate-workfront/workfront-navigation/workfront-terminology-glossary.md).

* [!UICONTROL 그룹]
* [!UICONTROL 그룹화]
* [!UICONTROL 시간 유형]
* [!UICONTROL 이니셔티브]

   회사가 다음을 구입한 경우에만 계획의 하위 객체인 이니셔티브 보고서를 작성할 수 있습니다 [!DNL Workfront Scenario Planner] 라이센스. 이니셔티브에 대한 자세한 내용은 [의 이니셔티브 개요 [!DNL Workfront Scenario Planner]](https://one.workfront.com/s/csh?context=2066&amp;pubname=the-new-workfront-experience).

   <!--
  <MadCap:conditionalText data-mc-conditions="QuicksilverOrClassic.Draft mode">
  (NOTE: this link is hardcoded)
  </MadCap:conditionalText>
  -->

* 이니셔티브 작업 역할

   회사가 A를 구매한 경우에만 계획에서 이니셔티브와 연관된 Job 역할에 대한 보고서를 작성할 수 있습니다 [!DNL Workfront Scenario Planner] 라이센스. 이니셔티브 생성 및 Job 역할과 연관에 대한 자세한 내용은 [에서 이니셔티브 만들기 및 편집 [!DNL Workfront Scenario Planner]](https://one.workfront.com/s/csh?context=2061&amp;pubname=the-new-workfront-experience).

   <!--
  <MadCap:conditionalText data-mc-conditions="QuicksilverOrClassic.Draft mode">
  (NOTE: this link is hardcoded)
  </MadCap:conditionalText>
  -->

* [!UICONTROL 반복]
* [!UICONTROL 작업 역할]
* [!UICONTROL 저널 항목]

   에서 추적된 시스템 업데이트를 보고할 수 있습니다 [!UICONTROL 업데이트] 작업, 프로젝트, 문제 등과 같은 객체 영역 자세한 내용은 [보고서 [!UICONTROL 업데이트] 영역](../../../reports-and-dashboards/reports/creating-and-managing-reports/create-journal-entry-report.md).

* [!UICONTROL 레이아웃 템플릿]
* [!UICONTROL 마일스톤]
* [!UICONTROL 마일스톤 경로]
* [!UICONTROL 참고]

   >[!NOTE]
   >
   >개별 사용자가 추가한 주석에 대해 보고할 수 있습니다.

* [!UICONTROL 매개 변수] 또는 [!UICONTROL 사용자 지정 필드])
* [!UICONTROL 매개 변수 그룹] 또는 [!UICONTROL 섹션 나누기])
* [!UICONTROL 포털 프로필] (더 이상 사용되지 않는 정보가 표시됩니다.)
* [!UICONTROL 포트폴리오]
* [!UICONTROL 프로그램]
* [!UICONTROL 프로젝트] ([!UICONTROL 재무 데이터])

   >[!NOTE]
   >
   >재무 정보는에 채워집니다 [!UICONTROL 프로젝트] ([!UICONTROL 재무 데이터])은 연결된 데이터가 5년 미만인 경우에만 보고합니다. 예를 들어, 2015년 1월에 Job 역할이 Task에 할당되었고 오늘이 2021년 9월인 경우 다음과 같은 재무 요청이 [!UICONTROL 할당 날짜] 의 경우 작업 역할이 [!UICONTROL 프로젝트(재무 데이터)] 보고서 세트에 대해 설명합니다.

* [!UICONTROL 증명 승인]\
   다음을 포함하여 증명 승인에 대한 다양한 정보를 볼 수 있습니다. 승인을 위해 제출된 증명, [!UICONTROL 승인자], 요청자에 대한 정보(요청자가 라이센스가 있는 경우) [!DNL Workfront] 사용자), 버전 정보, 증명 ID 및 증명 작성 날짜\
   [!UICONTROL 증명 승인] 보고서에는 아직 결정을 내리지 않은 사용자의 내 작업 영역에서 사용할 수 있는 증명만 포함됩니다.\
   증명 승인는에서 지정됩니다. [!DNL Workfront] 설명 [증명에 사용자 추가](../../../review-and-approve-work/proofing/managing-proofs-within-workfront/share-a-proof-in-workfront.md#add) in [내에서 증명 공유 [!DNL Adobe Workfront]](../../../review-and-approve-work/proofing/managing-proofs-within-workfront/share-a-proof-in-workfront.md).

* [!UICONTROL 대기열]
* [!UICONTROL 대기열 주제]
* [!UICONTROL 비율] (작업 역할을 표시합니다.) [!UICONTROL 청구 비율] information)
* [!UICONTROL 미리 알림]
* [!UICONTROL 보고서]
* [!UICONTROL 리소스 풀]
* [!UICONTROL 위험]
* [!UICONTROL 위험 유형]
* [!UICONTROL 일정]
* [!UICONTROL 스코어카드]
* [!UICONTROL 팀]
* [!UICONTROL 템플릿]
* [!UICONTROL 템플릿 작업]
* [!UICONTROL 휴무]

   사용자의 프로필에서 사용자가 지정한 대로 사용자의 휴가에 대해 보고할 수 있습니다.

* [!UICONTROL 타임시트]
* [!UICONTROL 타임시트 프로필]
* [!UICONTROL 주제 그룹]
* [!UICONTROL 사용자 위임]

   부재 중 다른 사람의 작업 및 문제를 수행하도록 위임된 사용자에 대해 보고할 수 있습니다. 이 보고서에는 부재 중인 사용자와 부재 중 직무 수행을 수행하는 사용자가 표시됩니다.

*  보기
* [!UICONTROL 작업 항목] (작업 및 문제를 나타냅니다.)
