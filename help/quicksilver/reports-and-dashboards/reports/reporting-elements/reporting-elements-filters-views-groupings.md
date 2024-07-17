---
product-area: reporting
navigation-topic: reporting-elements
title: '보고 요소: 필터, 보기 및 그룹화'
description: Workfront에서 모든 목록과 보고서에 포함해야 하는 주요 요소는 필터, 보기 및 그룹입니다. 각 요소는 모든 보고서 내에 서로 다른 정보를 제공합니다.
author: Nolan
feature: Reports and Dashboards
exl-id: 5697905e-42c0-403b-85d4-798a1a3a2e7f
source-git-commit: 548e713700fda79070f59f3dc3457410d2c50133
workflow-type: tm+mt
source-wordcount: '840'
ht-degree: 0%

---

# 보고 요소: 필터, 보기 및 그룹화

<!--
<div style="color: #ff1493;" data-mc-conditions="QuicksilverOrClassic.Draft mode">
<p>AL: Add information here about all the different kinds of FVGs: in reports, in lists, beta, etc // OR: this article should be a high-level overview of reporting elements. Then, each type of element should have:</p>
<p>- overview for Filters</p>
<p>- create a filter</p>
<p>- share a filter</p>
<p>ALL in Reporting elements but the Shared ones should be linked to Basics> Sharing; some of the articles in the Basics> Navigation> Use lists might beed to link here as well</p>
</div>
-->

Adobe Workfront에서 목록 또는 보고서를 가능하게 하는 몇 가지 요소가 있습니다. 모든 목록과 보고서에 포함해야 하는 주요 요소는 필터, 보기 및 그룹입니다. 각 요소는 모든 보고서 내에 서로 다른 정보를 제공합니다.

## 보고 요소에 대한 고려 사항

필터, 보기 및 그룹화 작업 시 다음 사항을 고려하십시오.

* 보고 요소는 보고의 기본 요소로 작동합니다. 보고서나 목록의 모양과 느낌은 물론 보고서나 목록에 포함된 정보를 정의합니다.
* Workfront의 보고서는 한 개의 오브젝트에 한정됩니다. 보고서를 작성하려면 먼저 보고서에 대한 주 개체를 정의해야 합니다. 따라서 모든 보고 요소는 개체별로 다릅니다.
* Workfront 관리자는 목록 및 보고서에서 보거나 편집할 수 있도록 액세스 수준의 필터, 보기 및 그룹화에 대한 액세스 권한을 부여해야 합니다.

  필터, 보기 및 그룹화에 대한 액세스 권한을 부여하는 방법에 대한 자세한 내용은 [필터, 보기 및 그룹화에 대한 액세스 권한 부여](../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-fvg.md)를 참조하십시오.

* 보고서를 보거나 편집할 수 있으려면 Workfront 관리자가 액세스 수준에서 보고서, 대시보드 및 달력에 대한 액세스 권한을 부여해야 합니다.

  보고서, 대시보드 및 캘린더에 대한 액세스 권한을 부여하는 방법에 대한 자세한 내용은 [보고서, 대시보드 및 캘린더에 대한 액세스 권한 부여](../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-reports-dashboards-calendars.md)를 참조하십시오.

* 보고서나 목록에서 필터, 보기 또는 그룹화를 선택하면 Workfront은 사용자가 브라우저를 로그아웃하거나 닫은 후에도 해당 오브젝트의 목록에 대해 이 선택 내용을 유지합니다. 예를 들어 작업 보고서에 대해 특정 보기를 선택하면 프로젝트의 작업 목록과 같은 다른 작업 목록에 대해 해당 선택 사항이 표시됩니다.

## 필터

이 필터는 보고서에 나타나는 결과를 제어합니다. 일반적으로 결과를 일반에서 특정 항목으로 좁힙니다. 이는 필요한 정보만 체득하여 해당 정보를 보고서에 다시 가져오는 것처럼 작동합니다.

예를 들어 로그인한 사용자에게 할당된 작업만 보려면 &quot;내 작업&quot;이라는 필터를 만들고, 필터에 대해 충족해야 하는 기준을 정의하고, 보고서를 실행하여 로그인한 사용자에게 할당된 작업만 볼 수 있습니다.

필터의 일부 속성은 다음과 같습니다.

* Workfront은 기본적으로 다양한 오브젝트에 대한 여러 필터를 제공합니다.
* 소유하거나 관리하는 필터를 사용자 지정할 수 있습니다.

  필터에 대한 자세한 내용은 문서 [필터 개요](../../../reports-and-dashboards/reports/reporting-elements/filters-overview.md)를 참조하십시오.

![필터 아이콘](assets/projects-list-with-filter-drop-down-highlighted-nwe.png)

## 보기

보고서 보기를 정의하여 보고서에 포함할 정보를 정의합니다. 모든 보고 요소와 마찬가지로 보기는 하나의 객체 유형을 기반으로 합니다.\
예를 들어 작업 보고서 보기에는 기한을 표시하거나 비용 등 주요 재무 세부 정보를 포함하거나 할당 및 납품 일자 세부 정보를 표시하는 데 사용할 수 있습니다. 보기는 보고서의 데이터에 대한 다양한 세부 사항을 전달하는 데 사용할 수 있습니다.

보기의 일부 속성은 다음과 같습니다.

* 기본 Workfront 보기를 사용하거나 직접 만들 수 있습니다.
* 보고서를 실행한 후 보기 드롭다운 필드에서 추가 보기를 적용할 수 있습니다.
* 추가 보기는 보고서를 만들 때 정의된 보기를 임시로 대체합니다. 그러나 다음 번에 보고서로 돌아가면 기본 보기가 표시됩니다.

  보기에 대한 자세한 내용은 문서 [Adobe Workfront의 보기 개요](../../../reports-and-dashboards/reports/reporting-elements/views-overview.md)를 참조하십시오.

## 그룹화

그룹화는 데이터를 구성하는 방법을 제어하여 읽고 이해하는 데 도움이 됩니다. 그룹화하면 보고서 전체에서 일반 특성별로 함께 나열된 결과를 표시하는 가로 막대가 만들어집니다. 그룹화를 생성할 때 보고서 결과를 그룹화하는 방법에 대한 기준을 정의합니다.

예를 들어, 여러 프로젝트에 걸쳐 있는 작업 목록을 해당 프로젝트 이름으로 그룹화하면 단일 프로젝트에 속하는 모든 각 작업이 해당 이름으로 구성됩니다.

그룹화의 일부 속성은 다음과 같습니다.

* 그룹화는 나중에 보고서에 차트를 추가하려는 경우 필수 보고 요소입니다.
* 그룹화는 결과에 집계 값을 표시합니다&#x200B;.
* 그룹화는 차트에서 축을 결정합니다.
* 그룹화는 매트릭스 보고서에서 헤더 ID를 결정합니다.\
  매트릭스 보고서에 대한 자세한 내용은 문서 [매트릭스 보고서 만들기](../../../reports-and-dashboards/reports/creating-and-managing-reports/create-matrix-report.md)를 참조하십시오.

* 그룹화는 보고서의 요약 탭을 만들고 보고서의 집계된 값을 제공하는 데 도움이 됩니다.
* Workfront은 기본적으로 서로 다른 개체에 대해 여러 가지 그룹화를 제공합니다.
* 소유하거나 관리하는 그룹화를 사용자 지정할 수 있습니다.

  그룹화에 대한 자세한 내용은 Adobe Workfront의 [그룹화 개요](../../../reports-and-dashboards/reports/reporting-elements/groupings-overview.md)를 참조하십시오.

## 기타 보고 요소

필터, 보기 및 그룹화 외에 다음 요소를 보고서에 추가할 수도 있습니다.

* **프롬프트**: 보고서를 실행할 때마다 다르게 사용자 지정 및 적용할 수 있는 열린 필터입니다.\
  프롬프트에 대한 자세한 내용은 문서 [보고서에 프롬프트 추가](../../../reports-and-dashboards/reports/creating-and-managing-reports/add-prompt-report.md)를 참조하십시오.

* **차트**: 차트를 추가하고 정보를 시각적으로 표시하여 보고서를 향상시킬 수 있습니다.\
  보고서의 차트에 대한 자세한 내용은 [보고서에 차트 추가](../../../reports-and-dashboards/reports/creating-and-managing-reports/add-chart-report.md) 문서를 참조하십시오.
