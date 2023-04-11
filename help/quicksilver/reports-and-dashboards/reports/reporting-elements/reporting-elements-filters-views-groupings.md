---
product-area: reporting
navigation-topic: reporting-elements
title: '''보고 요소: 필터, 보기 및 그룹화'
description: 모든 목록 및 보고서에 포함해야 하는 기본 요소는 필터, 보기 및 그룹입니다. 각 요소는 보고서 내에서 다른 정보를 제공합니다.
author: Nolan
feature: Reports and Dashboards
exl-id: 5697905e-42c0-403b-85d4-798a1a3a2e7f
source-git-commit: 302771f4d64b386149623f87a3436d0c40f421d5
workflow-type: tm+mt
source-wordcount: '843'
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

Adobe Workfront에서 가능한 목록 또는 보고서를 만드는 몇 가지 요소가 있습니다. 모든 목록 및 보고서에 포함해야 하는 기본 요소는 필터, 보기 및 그룹입니다. 각 요소는 보고서 내에서 다른 정보를 제공합니다.

## 보고 요소에 대한 고려 사항

필터, 보기 및 그룹화를 사용할 때는 다음 사항을 고려하십시오.

* 보고 요소는 보고의 기본 요소로 작동합니다. 보고서 또는 목록의 모양과 느낌, 보고서 또는 목록에 포함된 정보를 정의합니다.
* Workfront의 보고서는 한 개체에만 적용됩니다. 보고서를 만들려면 먼저 보고서에 대한 기본 개체를 정의해야 합니다. 따라서 모든 보고 요소는 개체별로 다릅니다.
* 목록 및 보고서에서 보거나 편집하려면 액세스 수준의 필터, 보기 및 그룹화에 대한 액세스 권한을 Workfront 관리자가 부여해야 합니다.

   필터, 보기 및 그룹화에 대한 액세스 권한 부여에 대한 자세한 내용은 [필터, 보기 및 그룹화에 대한 액세스 권한 부여](../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-fvg.md).

* 보고서를 보거나 편집하려면 Workfront 관리자가 액세스 수준의 보고서, 대시보드 및 달력에 대한 액세스 권한을 부여해야 합니다.

   보고서, 대시보드 및 달력에 대한 액세스 권한 부여에 대한 자세한 내용은 [보고서, 대시보드 및 달력에 대한 액세스 권한 부여](../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-reports-dashboards-calendars.md).

* 보고서나 목록에서 필터, 보기 또는 그룹을 선택하는 경우 브라우저를 로그아웃하거나 닫아도 Workfront에서 해당 개체 목록에 대해 이 선택 항목을 유지합니다. 예를 들어, 작업 보고서에 대한 특정 보기를 선택하면 프로젝트의 작업 목록과 같은 다른 작업 목록에 대한 선택 항목이 나타납니다.

## 필터

이 필터는 보고서에 나타나는 결과를 제어하며, 일반적으로 결과를 일반에서 특성으로 좁힙니다. 필요한 정보를 가져와서 보고서에 다시 가져오는 것처럼 작동합니다.

예를 들어, 로그인한 사용자에게 할당된 작업만 보려는 경우 &quot;내 작업&quot;이라는 필터를 만들고 필터에 대해 충족해야 하는 기준을 정의하고, 로그인한 사용자에게 할당된 작업만 보려면 보고서를 실행할 수 있습니다.

필터의 일부 특성은 다음과 같습니다.

* Workfront에서는 기본적으로 다양한 개체에 대해 많은 필터를 제공합니다.
* 소유하거나 관리하는 필터를 사용자 지정할 수 있습니다.

   필터에 대한 자세한 내용은 문서를 참조하십시오 [Adobe Workfront의 필터 개요](../../../reports-and-dashboards/reports/reporting-elements/filters-overview.md).

![필터 아이콘](assets/projects-list-with-filter-drop-down-highlighted-nwe.png)

## 조회수

보고서 보기를 정의하면 보고서에 포함할 정보를 정의합니다. 모든 보고 요소와 마찬가지로 보기는 하나의 개체 유형을 기반으로 합니다.\
예를 들어, 태스크 보고서의 뷰는 기한 일자를 표시하거나, 비용과 같은 주요 재무 상세내역을 포함하거나, 지정 및 납품 일자 상세내역을 표시하는 데 사용될 수 있습니다. 보기는 보고서의 데이터에 대한 다양한 세부 사항을 전달하는 데 사용할 수 있습니다.

보기의 일부 속성은 다음과 같습니다.

* 기본 Workfront 보기를 사용하거나 직접 만들 수 있습니다.
* 보고서를 실행한 후 보기 드롭다운 필드에서 추가 보기를 적용할 수 있습니다.
* 보고서를 만들 때 정의된 보기를 일시적으로 추가 보기로 바꿉니다. 하지만 다음에 보고서로 돌아가면 기본 보기가 표시됩니다.

   보기에 대한 자세한 내용은 문서를 참조하십시오 [Adobe Workfront의 보기 개요](../../../reports-and-dashboards/reports/reporting-elements/views-overview.md).

## 그룹화

그룹화는 데이터를 구성하는 방법을 제어하므로 보다 쉽게 읽고 이해할 수 있습니다. 그룹화는 일반적인 속성으로 함께 나열된 결과를 표시하는 보고서 전체에서 가로 막대를 만듭니다. 그룹을 만들 때 보고서 결과를 그룹화하는 방법에 대한 기준을 정의합니다.

예를 들어, 여러 프로젝트에 걸쳐 있는 작업 목록을 프로젝트 이름으로 그룹화하면 해당 이름으로 단일 프로젝트에 속하는 모든 작업이 구성됩니다.

그룹화 속성은 다음과 같습니다.

* 그룹화는 나중에 보고서에 차트를 추가하려면 필수 보고 요소입니다.
* 그룹화 결과는 집계 값을 &#x200B; 표시합니다.
* 그룹화는 차트에서 축을 결정합니다.
* 그룹화는 매트릭스 보고서에서 헤더 식별을 결정합니다.\
   매트릭스 보고서에 대한 자세한 내용은 문서를 참조하십시오 [매트릭스 보고서 만들기](../../../reports-and-dashboards/reports/creating-and-managing-reports/create-matrix-report.md).

* 그룹화는 보고서의 요약 탭을 빌드하여 보고서의 집계된 값을 제공하는 데 도움이 됩니다.
* Workfront에서는 기본적으로 서로 다른 개체를 위한 여러 그룹을 제공합니다.
* 소유 또는 관리하는 그룹을 사용자 지정할 수 있습니다.

   그룹화에 대한 자세한 내용은 [Adobe Workfront의 그룹화 개요](../../../reports-and-dashboards/reports/reporting-elements/groupings-overview.md).

## 기타 보고 요소

필터, 보기 및 그룹화 외에도 보고서에 다음 요소를 추가할 수 있습니다.

* **프롬프트**: 보고서를 실행할 때마다 사용자 지정하고 다르게 적용할 수 있는 열린 필터입니다.\
   프롬프트에 대한 자세한 내용은 문서를 참조하십시오 [보고서에 프롬프트 추가](../../../reports-and-dashboards/reports/creating-and-managing-reports/add-prompt-report.md).

* **차트**: 차트를 추가하고 정보를 시각적으로 표시하여 보고서를 향상시킬 수 있습니다.\
   보고서의 차트에 대한 자세한 내용은 문서를 참조하십시오 [보고서에 차트 추가](../../../reports-and-dashboards/reports/creating-and-managing-reports/add-chart-report.md).
