---
content-type: overview
product-area: projects
navigation-topic: manage-tasks
title: 프로젝트 중요 경로 개요
description: 프로젝트의 중요 경로를 결정하는 것은 Adobe Workfront이 프로젝트의 타임라인에 영향을 줄 수 있는 프로젝트 작업 시퀀스에 플래그를 지정하는 자동 방법입니다. 프로젝트의 타임라인에 영향을 줄 수 있는 작업은 중요 경로 작업으로 플래그가 지정됩니다.
author: Alina
feature: Work Management
exl-id: 9cbc84bf-d02b-4bb7-8d5d-922554d1262e
source-git-commit: f2f825280204b56d2dc85efc7a315a4377e551c7
workflow-type: tm+mt
source-wordcount: '764'
ht-degree: 0%

---

# 프로젝트 중요 경로 개요

프로젝트의 중요 경로를 결정하는 것은 Adobe Workfront이 프로젝트의 타임라인에 영향을 줄 수 있는 프로젝트 작업 시퀀스에 플래그를 지정하는 자동 방법입니다. 프로젝트의 타임라인에 영향을 줄 수 있는 작업은 중요 경로 작업으로 플래그가 지정됩니다.

다음 기능은 프로젝트의 중요 경로에 영향을 줄 수 있습니다.

* 프로젝트의 작업 분류 구조.

  작업 분류 구조에 대한 자세한 내용은 [프로젝트에서 작업 분류 구조 결정](../../../manage-work/projects/planning-a-project/determine-project-work-breakdown-structure.md)을 참조하십시오.

* 각 작업이 완료되는 데 소요되는 시간(기간)입니다.
* 작업 간의 종속성.

  다음 사항을 고려하십시오.

   * 중요 경로의 작업에 전임 작업 관계가 있는 경우 전임 작업 또는 후임 작업의 날짜 변경이 종속 항목에 직접 영향을 주는 경우 해당 전임 작업 및 후임 작업도 중요 경로에 포함됩니다.

     >[!TIP]
     >
     >후속 작업의 날짜가 종속 작업의 날짜에 직접 영향을 주지 않고 프로젝트 날짜에도 영향을 주지 않는 경우 후속 작업이 중요 경로에 없습니다.
     >
     >
     >![](assets/successor-not-on-critical-path-350x150.png)     >
     >

   * 하위 작업이 중요 경로 작업으로 식별되는 경우, 상위 작업의 예상 시작 일자와 시간이 하위 작업의 예상 시작 일자와 동일한 경우, 상위 작업도 중요 경로 작업으로 식별됩니다.

이러한 기능을 고려하여 가장 이른 작업과 프로젝트 종료를 결정하는 작업 사이의 가장 긴 경로를 사용하여 중요 경로 를 계산합니다. 중요 경로 계산에서는 프로젝트를 더 길게 하지 않고도 각 작업을 시작하고 완료할 수 있는 가장 이른 시간과 가장 늦은 시간을 고려합니다. 이 프로세스는 &quot;위험&quot;(및 가장 긴 경로에 속함)한 작업과 &quot;총 부동&quot;(프로젝트를 더 길게 하지 않고 지연시킬 수 있음)을 갖는 작업을 결정합니다.

중요 경로에서 작업 활동이 지연되면 프로젝트의 예상 완료 일자에 직접 영향을 미칩니다. 중요 경로에는 부동 소수점이 없습니다.

## 액세스 요구 사항

이 문서의 단계를 수행하려면 다음 액세스 권한이 있어야 합니다.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront 플랜*</td> 
   <td> <p>임의</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront 라이센스*</td> 
   <td> <p>작업 이상</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">액세스 수준 구성*</td> 
   <td> <p>작업에 대한 보기 또는 상위 액세스 권한</p> <p>참고: 여전히 액세스 권한이 없는 경우 Workfront 관리자에게 액세스 수준에서 추가 제한을 설정하는지 문의하십시오. Workfront 관리자가 액세스 수준을 수정하는 방법에 대한 자세한 내용은 <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">사용자 지정 액세스 수준 만들기 또는 수정</a>을 참조하십시오.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">개체 권한</td> 
   <td> <p>작업에 대한 이상의 권한 보기 </p> <p>추가 액세스 요청에 대한 자세한 내용은 <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">개체 </a>에 대한 액세스 요청 을 참조하십시오.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;보유 중인 플랜, 라이선스 유형 또는 액세스 권한을 확인하려면 Workfront 관리자에게 문의하십시오.

## 중요 경로 보기

Workfront 애플리케이션의 다음 영역에서 중요 경로에 속하는 작업을 볼 수 있습니다.

* [간트 차트에서 중요 경로 보기](#view-the-critical-path-in-the-gantt-chart)
* [작업 목록 또는 보고서에서 중요 경로 보기](#view-the-critical-path-in-a-task-list-or-report)

### 간트 차트에서 중요 경로 보기 {#view-the-critical-path-in-the-gantt-chart}

간트 차트의 중요 경로에서 작업을 보려면 다음과 같이 하십시오.

1. 중요 경로를 보려는 프로젝트로 이동합니다.
1. 왼쪽 패널에서 **작업**&#x200B;을 클릭합니다.
1. 작업 목록의 오른쪽 상단에 있는 **간트 차트** 아이콘을 클릭합니다.

   ![gantt_chart_icon__1_.png](assets/gantt-chart-icon--1-.png)

1. **옵션** 메뉴를 확장한 다음 **중요 경로** 옵션을 활성화합니다.

   중요 경로에 있는 작업은 간트 차트에서 타임라인 위에 빨간색 선이 표시됩니다.

   ![critical_path_on_gantt__1_.png](assets/crtitical-path-on-gantt--1--350x137.png)

### 작업 목록 또는 보고서에서 중요 경로 보기 {#view-the-critical-path-in-a-task-list-or-report}

작업 목록에서 중요 경로에 있는 작업을 보려면 다음과 같이 하십시오.

1. 중요 경로를 보려는 프로젝트로 이동합니다.
1. 왼쪽 패널에서 **작업**&#x200B;을 클릭합니다.
1. **보기** 드롭다운 메뉴에서 **상태**&#x200B;를 선택합니다.

   중요 경로에 있는 작업은 목록의 **플래그** 열에 **중요 경로** 플래그가 있습니다.

   작업 보고서에 동일한 보기를 적용할 수 있습니다.

   보고서 만들기에 대한 자세한 내용은 문서 [사용자 지정 보고서 만들기](../../../reports-and-dashboards/reports/creating-and-managing-reports/create-custom-report.md)를 참조하세요.

   또는

   **필터** 드롭다운 메뉴에서 **새 필터**&#x200B;을(를) 선택합니다.

1. **필터 규칙 추가**&#x200B;를 클릭하고 **다음 항목의 작업만 표시** 필드에 **중요**&#x200B;을(를) 입력하십시오.

1. 목록에 나타나면 선택합니다.
1. **필터 저장**&#x200B;을 클릭합니다.

   중요 경로에 있는 작업만 목록에 표시됩니다.
