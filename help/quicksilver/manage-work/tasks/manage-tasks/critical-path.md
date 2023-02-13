---
content-type: overview
product-area: projects
navigation-topic: manage-tasks
title: 프로젝트 중요 경로 개요
description: 프로젝트의 중요 경로 결정은 Adobe Workfront이 프로젝트 타임라인에 영향을 줄 가능성이 있는 프로젝트의 작업 시퀀스를 플래그를 지정하는 자동 방법입니다. 프로젝트의 타임라인에 영향을 줄 수 있는 작업은 중요 경로 작업으로 플래그가 지정됩니다.
author: Alina
feature: Work Management
exl-id: 9cbc84bf-d02b-4bb7-8d5d-922554d1262e
source-git-commit: f2f825280204b56d2dc85efc7a315a4377e551c7
workflow-type: tm+mt
source-wordcount: '771'
ht-degree: 0%

---

# 프로젝트 중요 경로 개요

프로젝트의 중요 경로 결정은 Adobe Workfront이 프로젝트 타임라인에 영향을 줄 가능성이 있는 프로젝트의 작업 시퀀스를 플래그를 지정하는 자동 방법입니다. 프로젝트의 타임라인에 영향을 줄 수 있는 작업은 중요 경로 작업으로 플래그가 지정됩니다.

다음 기능은 프로젝트의 중요 경로에 영향을 줄 수 있습니다.

* 프로젝트의 작업 분류 구조입니다.

   작업 분류 구조에 대한 자세한 내용은 [프로젝트에서 작업 분류 구조 결정](../../../manage-work/projects/planning-a-project/determine-project-work-breakdown-structure.md)

* 각 작업을 완료하는 데 걸리는 시간(기간)입니다.
* 작업 간의 종속성.

   다음 사항을 고려하십시오.

   * Critical Path에 대한 작업에 선행 관계가 있는 경우, 선행 작업 또는 후임자의 날짜 변경 사항이 해당 종속 항목에 직접 영향을 주는 경우, 선행 작업 및 후속 작업 역시 Critical Path에 있습니다.

      >[!TIP]
      >
      >작업 후속 작업의 날짜가 종속 작업의 날짜에 직접적으로 영향을 주지 않고 프로젝트 날짜에 영향을 주지 않는 경우 후속 작업은 중요한 경로에 있지 않습니다.
      >
      >
      >![](assets/successor-not-on-critical-path-350x150.png)     >

   * 하위 태스크가 위기 경로 태스크로 식별되면 상위의 예상 시작 날짜 및 시간이 하위 태스크와 동일한 경우 상위 태스크도 위기 경로 태스크로 식별됩니다.

이러한 기능을 고려하여, 시스템은 가장 이른 작업과 프로젝트 종료를 결정하는 작업 사이의 가장 긴 경로를 사용하여 임계 경로를 계산합니다. 중요 경로 계산에서는 프로젝트를 더 길게 하지 않고도 각 작업이 시작되고 완료될 수 있는 가장 이른 시간과 최신 시간을 고려합니다. 이 프로세스는 &quot;위험&quot;(그리고 가장 긴 경로에 속함) 및 &quot;총 부동&quot;(프로젝트를 더 길게 하지 않고 지연할 수 있음)을 가진 작업을 결정합니다.

위기 경로 작업 지연이 프로젝트의 예상 완료 날짜에 직접적으로 영향을 줍니다(중요한 경로에 플로트가 없음).

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
   <td> <p>작업 이상</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">액세스 수준 구성*</td> 
   <td> <p>작업에 대한 액세스 권한 보기 이상</p> <p>참고: 여전히 액세스 권한이 없는 경우 Workfront 관리자에게 액세스 수준에서 추가 제한 사항을 설정하는지 문의하십시오. Workfront 관리자가 액세스 수준을 수정하는 방법에 대한 자세한 내용은 <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">사용자 정의 액세스 수준 만들기 또는 수정</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">개체 권한</td> 
   <td> <p>작업에 대한 권한 보기 이상 </p> <p>추가 액세스 요청에 대한 자세한 내용은 <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">개체에 대한 액세스 요청 </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;어떤 계획, 라이선스 유형 또는 액세스 권한을 보유하고 있는지 알아보려면 Workfront 관리자에게 문의하십시오.

## 중요 경로 보기

Workfront 애플리케이션의 다음 영역에서 중요 경로에 속하는 작업을 볼 수 있습니다.

* [간트 차트에서 중요 경로 보기](#view-the-critical-path-in-the-gantt-chart)
* [작업 목록 또는 보고서에서 중요한 경로 보기](#view-the-critical-path-in-a-task-list-or-report)

### 간트 차트에서 중요 경로 보기 {#view-the-critical-path-in-the-gantt-chart}

Gantt 차트의 중요 경로에 있는 작업을 보려면

1. 중요한 경로를 볼 프로젝트로 이동합니다.
1. 클릭 **작업** 왼쪽 패널에 표시됩니다.
1. 을(를) 클릭합니다. **간트 차트** 작업 목록의 오른쪽 위 모서리에 있는 아이콘.

   ![gantt_chart_icon__1_.png](assets/gantt-chart-icon--1-.png)

1. 를 확장합니다. **옵션** 메뉴를 클릭한 다음 **중요 경로** 선택 사항입니다.

   중요 경로에 있는 작업은 간트 차트의 타임라인 위에 빨간색 선이 있습니다.

   ![metric_path_on_gantt__1_.png](assets/crtitical-path-on-gantt--1--350x137.png)

### 작업 목록 또는 보고서에서 중요한 경로 보기 {#view-the-critical-path-in-a-task-list-or-report}

작업 목록에서 중요한 경로에 있는 작업을 보려면

1. 중요한 경로를 볼 프로젝트로 이동합니다.
1. 클릭 **작업** 왼쪽 패널에 표시됩니다.
1. 에서 **보기** 드롭다운 메뉴에서 **상태**.

   중요 경로에 있는 작업은 다음과 같습니다 **중요 경로** 의 플래그 **플래그** 열의 을 포함합니다.

   작업 보고서에 동일한 보기를 적용할 수 있습니다.

   보고서 만들기에 대한 자세한 내용은 문서를 참조하십시오 [사용자 지정 보고서 만들기](../../../reports-and-dashboards/reports/creating-and-managing-reports/create-custom-report.md).

   또는

   에서 **필터** 드롭다운 메뉴에서 **새 필터**.

1. 클릭 **필터 규칙 추가** 입력을 시작합니다. **중요** 에서 **작업 표시...** 필드.

1. 목록에 있으면 선택합니다.
1. 클릭 **필터 저장**.

   목록에는 위기 경로에 있는 작업만 표시됩니다.
