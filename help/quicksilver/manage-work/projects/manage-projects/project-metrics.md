---
content-type: overview;how-to-procedural
product-area: projects
keywords: analytics,지표,프로젝트,향상,작업,할당자,완료,상태,지연됨,예정
navigation-topic: manage-projects
title: 프로젝트 지표 개요
description: 프로젝트 지표는 프로젝트에서 발생하는 내용을 시각화하므로 프로젝트의 요구 사항과 상태를 신속하게 평가할 수 있습니다. 프로젝트 왼쪽 패널에서 지표 영역을 해석하는 방법을 알아봅니다.
author: Alina
feature: Work Management
exl-id: 54c2a59d-9f6b-4126-9526-5169aeda8517
source-git-commit: 24cc3ece515fd778a9bc9e8afbcd534f48b24230
workflow-type: tm+mt
source-wordcount: '1275'
ht-degree: 0%

---

# 프로젝트 지표 개요

프로젝트 지표는 프로젝트 수행 방식에 대한 일반적인 보기를 차트 형식으로 제공합니다.

## 액세스 요구 사항

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Workfront 플랜*</td> 
   <td> <p>모든</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Workfront 라이선스*</td> 
   <td> <p>검토 이상 </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">액세스 수준*</td> 
   <td> <p>프로젝트에 대한 액세스 보기</p> <p><b>메모</b>

여전히 액세스 권한이 없는 경우 Workfront 관리자에게 액세스 수준에서 추가 제한 사항을 설정하는지 문의하십시오. 프로젝트 액세스에 대한 자세한 내용은 <a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-projects.md" class="MCXref xref">프로젝트에 대한 액세스 권한 부여</a>. Workfront 관리자가 액세스 수준을 변경하는 방법에 대한 자세한 내용은 <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">사용자 정의 액세스 수준 만들기 또는 수정</a>. </p> </td>
</tr> 
  <tr> 
   <td role="rowheader">개체 권한</td> 
   <td> <p>프로젝트에 대한 권한 보기</p> <p> 프로젝트 권한에 대한 자세한 내용은 <a href="../../../workfront-basics/grant-and-request-access-to-objects/share-a-project.md" class="MCXref xref">Adobe Workfront에서 프로젝트 공유</a>.</p> <p>추가 액세스 요청에 대한 자세한 내용은 <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">개체에 대한 액세스 요청 </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

*보유하고 있는 플랜, 라이선스 유형 또는 액세스를 알아보려면 Workfront 관리자에게 문의하십시오.

## 전제 조건

프로젝트의 왼쪽 패널에서 지표 영역에 액세스하려면 다음을 수행해야 합니다.

* 레이아웃 템플릿의 프로젝트 영역에서 왼쪽 패널 옵션 지표 를 활성화한 상태로 두십시오.

   Workfront 관리자 또는 그룹 관리자가 레이아웃 템플릿으로 왼쪽 패널을 사용자 지정하는 방법에 대한 자세한 내용은 [레이아웃 템플릿을 사용하여 왼쪽 패널 사용자 정의](../../../administration-and-setup/customize-workfront/use-layout-templates/customize-left-panel.md).

## 프로젝트 지표 영역 개요

프로젝트 지표는 프로젝트에서 발생하는 내용을 시각화하므로 프로젝트의 요구 사항과 상태를 신속하게 평가할 수 있습니다.

![](assets/project-metrics-full-screen-350x238.png)

지표 영역에서는 프로젝트의 전체 상태와 다음을 볼 수 있습니다.

* 작업이 활성 또는 정지된 경우
* 열려 있는 작업 항목이 지정된 사용자
* 계획 완료 일자에 미착되거나 마감되는 태스크 또는 문제에 대한 상세내역

각 차트로 드릴다운하여 특정 범주의 작업 또는 문제를 보다 자세히 확인할 수도 있습니다.

이러한 작업 또는 문제를 보는 방법에 대한 자세한 내용은 [지표 세부 사항 보기](#view-metrics-details).

>[!TIP]
>
>프로그램, 포트폴리오 등 내에서 프로젝트 그룹에 대한 상위 수준에서 지표를 보려면 Enhanced Analytics 영역으로 이동합니다.\
>Enhanced Analytics에 대한 자세한 내용은 [향상된 분석 개요](../../../enhanced-analytics/enhanced-analytics-overview.md).

## 프로젝트 KPI

지표 영역 맨 위에 주요 성과 지표(KPI)가 표시됩니다.

![](assets/project-metrics-kpis-350x52.png)

이 KPI는 다음 카테고리로 분류됩니다.

| 완료된 작업 | **완료된 작업** 완료 상태의 작업 수를 표시합니다. 이 번호에는 완료와 일치하는 사용자 지정 상태가 있는 작업도 포함됩니다. |
|---|---|
| 완료되지 않은 작업 | **완료되지 않은 작업** 완료 또는 닫힌 상태가 아닌 작업의 수나 완료와 같은 상태를 표시합니다. |
| 지연된 작업 | **지연된 작업** 완료 또는 마감 상태가 아닌 계획 완료 일자 이후의 태스크 수 또는 완료 또는 마감과 연관된 상태를 표시합니다. |
| 총 작업 수 | **총 작업 수** 프로젝트의 총 작업 수를 표시합니다. |

>[!TIP]
>
>특정 KPI에 대한 작업 항목 목록을 표시하려면 해당 KPI를 클릭합니다. 해당 목록에서 특정 작업 항목을 클릭하여 새 탭에서 자세한 내용을 볼 수 있습니다.\
>![](assets/completed-tasks-dialog-350x75.png)\
>자세한 내용은 [지표 세부 사항 보기](#view-metrics-details).

## 작업 또는 문제 표시줄 차트

프로젝트 KPI 아래에 표시되는 막대 차트에서는 프로젝트에 있는 작업 항목의 상태 또는 우선 순위를 확인할 수 있습니다. 기본적으로 작업 보기가 선택됩니다.

이 차트에서 상태를 선택하면 프로젝트의 모든 작업 또는 문제 상태를 볼 수 있습니다. 각 상태는 차트의 막대로 그룹화됩니다. 모든 기본 시스템 상태와 사용자 정의 상태가 이 차트에 표시됩니다.

![](assets/project-metrics-task-issue-by-status-350x120.png)

이 차트에서 우선 순위를 선택하면 프로젝트의 모든 작업 또는 문제에 대한 우선 순위를 볼 수 있습니다.

![](assets/project-metrics-task-issue-by-priority-350x121.png)

>[!TIP]
>
>특정 상태 또는 우선 순위를 갖는 작업 항목 목록을 표시하려면 차트의 막대를 클릭합니다. 해당 목록에서 특정 작업 항목을 클릭하여 새 탭에서 자세한 내용을 볼 수 있습니다.\
>![](assets/completed-tasks-dialog-350x75.png)\
>자세한 내용은 [지표 세부 사항 보기](#view-metrics-details).

## 도넛 차트

프로젝트 KPI 아래에 있는 도넛 차트를 통해 완료된 작업 항목과 프로젝트의 불완전한 작업 항목의 비율을 확인할 수 있습니다.

![](assets/tasks-issues-by-complete-status-350x250.png)

차트 위의 드롭다운 메뉴에서 다음을 선택할 수 있습니다.

| 모든 작업 | 선택 **작업** 프로젝트의 총 작업 수와 완료된 작업과 완료되지 않은 작업 사이의 비율을 표시합니다. |
|---|---|
| 모든 문제 | 선택 **문제** 프로젝트의 총 문제 수와 완료된 문제와 불완전한 문제 사이의 비율을 표시합니다. |

>[!TIP]
>
>완료되었거나 완료되지 않은 작업 항목 목록을 표시하려면 도넛 차트에서 해당 섹션을 클릭합니다. 해당 목록에서 특정 작업 항목을 클릭하여 새 탭에서 자세한 내용을 볼 수 있습니다.\
>![](assets/completed-tasks-dialog-350x75.png)\
>자세한 내용은 [지표 세부 사항 보기](#view-metrics-details).

## 할당자 막대 차트

할당자 막대 차트는 프로젝트의 각 사람에게 할당된 작업의 수를 보여 줍니다. 이 숫자는 드롭다운 메뉴에서 선택한 카테고리에 따라 달라집니다.

![](assets/tasks-issues-by-assignee-350x104.png)

다음 범주에서 프로젝트에 대한 태스크 지정을 확인하도록 선택할 수 있습니다.

| 완료 | 선택 **완료** 완료된 각 사용자에게 할당된 작업 수를 표시합니다. |
|---|---|
| 완료 안 됨 | 선택 **완료되지 않음** 아직 완료되지 않은 각 사용자에게 할당된 작업 수를 표시합니다. |
| 예정 | 선택 **예정된 날짜** 계획된 시작 날짜에 아직 도달하지 않은 각 사용자에게 할당된 작업의 수를 표시합니다. |
| 기한 초과 | 선택 **기한 초과** 계획된 완료 일자를 지났으며 아직 완료되지 않은 각 사용자에게 할당된 작업의 수를 표시합니다. |

>[!TIP]
>
>특정 사용자에게 할당된 선택된 범주에 있는 작업 항목 목록을 표시하려면 차트에서 사용자 이름 옆에 있는 막대를 누릅니다. 해당 목록에서 특정 작업 항목을 클릭하여 새 탭에서 자세한 내용을 볼 수 있습니다.\
>![](assets/completed-tasks-dialog-350x75.png)\
>자세한 내용은 [지표 세부 사항 보기](#view-metrics-details).

## 지표 세부 사항 보기 {#view-metrics-details}

지표 영역의 차트와 상호 작용하여 차트의 다른 측면을 보거나 차트 내의 작업 및 문제를 보다 자세히 볼 수 있습니다.

1. 지표를 볼 프로젝트로 이동합니다.
1. 왼쪽 패널에서 **자세히 표시** 섹션을 더 표시하려면 을(를) 클릭합니다. **지표**.\
   지표 영역의 차트는 기본적으로 작업에 대한 정보를 표시합니다.\
   ![](assets/metrics-section-350x298.png)

1. (조건부) 드롭다운 화살표가 차트에 표시되면 **드롭다운 화살표** 아이콘 ![](assets/dropdown-arrow.png) 차트에서 메뉴에서 원하는 옵션을 선택합니다.\
   각 차트의 메뉴에 나타나는 옵션에 대한 자세한 내용은 위의 관련 섹션을 참조하십시오.

1. (선택 사항) 페이지에서 지표에 대한 작업 또는 문제를 자세히 살펴보려면 다음을 수행하십시오.

   1. 세부 정보를 보려는 특정 사용자에게 할당된 작업, 우선 순위가 높은 문제 또는 모든 지연 작업과 같은 요소를 클릭합니다.

      작업 또는 문제 목록이 표시됩니다.

      ![](assets/completed-tasks-dialog-350x75.png)

   1. 목록 맨 아래의 화살표를 사용하여 확인할 작업 또는 문제를 찾습니다.

      또는

      특정 페이지에서 작업이나 문제를 표시하려면 특정 숫자를 선택합니다.

      ![](assets/pagination-300x152.png)

   1. 자세한 내용을 보려면 작업 또는 문제를 선택하십시오.

      작업이나 문제가 새 탭에서 열립니다.

1. (선택 사항) 프로젝트 지표 대시보드를 .png 파일로 내보내려면 **내보내기** 아이콘 ![](assets/export.png)를 선택하고 을 선택합니다. **PNG로 내보내기** 를 클릭합니다.

   >[!TIP]
   >
   >대시보드를 내보낼 때 내보낸 파일에는 현재 뷰포트에 표시되는 파일만 포함됩니다. 내보낸 파일에 특정 항목을 포함하려면 페이지에서 위나 아래로 스크롤하거나 브라우저의 확대/축소 설정을 조정해야 할 수 있습니다.
