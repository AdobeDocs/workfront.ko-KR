---
content-type: overview
product-area: projects
navigation-topic: task-information
title: 실제 시간 보기
description: Adobe Workfront에서 작업 항목에 로그온하는 시간은 실제 시간으로 간주됩니다.
author: Alina
feature: Work Management
exl-id: c4b0e431-1765-416d-89f5-6ac663ac1d4f
source-git-commit: f2f825280204b56d2dc85efc7a315a4377e551c7
workflow-type: tm+mt
source-wordcount: '796'
ht-degree: 0%

---

# 실제 시간 보기

Adobe Workfront에서 작업 항목에 로그온하는 시간은 실제 시간으로 간주됩니다.

실제 시간은 작업, 문제 또는 프로젝트를 완료하는 데 걸린 실제 시간을 나타냅니다.

작업 및 문제인 작업 항목에 시간을 로그온하는 것이 좋습니다.

그러나 Workfront 관리자는 사용자가 조직의 워크플로우에 따라 프로젝트에서 로그인하여 하도록 허용할 수 있습니다.

사용자가 프로젝트에 로그인할 수 있도록 시스템을 설정하는 방법에 대한 자세한 내용은 다음을 참조하십시오 [작업표 및 시간 환경 설정 구성](../../../administration-and-setup/set-up-workfront/configure-timesheets-schedules/timesheet-and-hour-preferences.md).

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
   <td> <p>작업, 프로젝트 또는 문제에 대한 보기 또는 더 높은 액세스 권한</p> <p>참고: 여전히 액세스 권한이 없는 경우 Workfront 관리자에게 액세스 수준에서 추가 제한 사항을 설정하는지 문의하십시오. Workfront 관리자가 액세스 수준을 수정하는 방법에 대한 자세한 내용은 <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">사용자 정의 액세스 수준 만들기 또는 수정</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">개체 권한</td> 
   <td> <p>작업, 프로젝트 또는 문제에 대한 권한 또는 그 이상의 권한 보기</p> <p>추가 액세스 요청에 대한 자세한 내용은 <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">개체에 대한 액세스 요청 </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;어떤 계획, 라이선스 유형 또는 액세스 권한을 보유하고 있는지 알아보려면 Workfront 관리자에게 문의하십시오.

## 작업 및 문제에 대한 실제 시간과 프로젝트의 실제 시간

작업 및 문제에 대한 실제 시간은 작업 및 문제에 직접 로그된 시간 수를 나타냅니다.

>[!NOTE]
>
>하위 작업의 실제 시간은 상위 작업의 실제 시간으로 롤업됩니다. 다음 공식은 상위 작업의 실제 시간(시)에 적용됩니다.

```
Parent Task Actual Hours = All Tasks Actual Hours + Parent Task Actual Hours
```

프로젝트에 대한 실제 시간은 프로젝트의 모든 작업(상위 작업에 직접 로그온한 시간 포함)에서 총 실제 시간을 나타내며 프로젝트 자체에 로그된 실제 시간은 물론 프로젝트의 모든 문제를 나타냅니다.

다음 공식은 프로젝트의 실제 시간에 적용됩니다.

```
Project Actual Hours = All Tasks Actual Hours + All Issues Actual Hours + All Project Actual Hours
```

## 실제 시간 찾기

항목에 대한 실제 시간 값을 찾는 것은 작업, 프로젝트 및 문제에 대해 동일합니다.

다음 위치에서 작업에 대한 실제 시간 정보를 찾을 수 있습니다.

* [세부 정보 섹션의 실제 시간](#actual-hours-in-the-details-section)
* [시간 섹션의 실제 시간](#actual-hours-in-the-hours-section)
* [보고서의 실제 시간](#actual-hours-in-reports)
* [리소스 관리 도구의 실제 시간](#actual-hours-in-resource-management-tools)

### 세부 정보 섹션의 실제 시간 {#actual-hours-in-the-details-section}

세부 정보 섹션의 실제 시간 검색은 프로젝트, 작업 및 문제에 대해 동일합니다.

작업 세부 정보에서 실제 시간을 찾으려면

1. 실제 시간을 검토할 작업으로 이동합니다.
1. 클릭 **작업 세부 사항** 왼쪽 패널에 표시됩니다.
1. 클릭 **개요** 그리고 **실제 시간** 값.

   이 작업에 로그온한 총 시간입니다.

### 시간 섹션의 실제 시간 {#actual-hours-in-the-hours-section}

시간 섹션에서 실제 시간을 찾는 것은 프로젝트, 작업 및 문제에 대해 동일합니다.

시간 섹션에서 실제 시간을 찾으려면

1. 실제 시간을 검토할 작업으로 이동합니다.
1. 클릭 **시간** 왼쪽 패널에 표시됩니다.

   구성에 따라 다음과 같은 시간 섹션이 표시될 수 있습니다 **자세히 표시**.

   작업에 기록된 시간 항목 목록이 표시됩니다.

1. 다음을 확인합니다. **표준** 보기 및 **프로젝트** 그룹화가 이 목록에 적용됩니다.

   그룹핑 라인에 표시된 번호 **시간** 열은 작업의 총 실제 시간 수입니다.

### 보고서의 실제 시간 {#actual-hours-in-reports}

작업, 문제 또는 프로젝트 보고서를 작성할 때 보고서에 각 작업, 문제 또는 프로젝트에 대한 실제 시간 값을 표시할 수 있습니다.

작업 보기에 실제 시간 열을 추가하는 것은 보고서에서 보기를 작성하는 것과 비슷합니다.

작업 보고서에 실제 시간을 표시하려면

1. 을(를) 클릭합니다. **기본 메뉴** 아이콘 ![](assets/main-menu-icon.png) Workfront의 오른쪽 위 모서리에서 을(를) 클릭하고 **보고서**.
1. 클릭 **새 보고서**, 그런 다음 **작업** 를 개체로 사용하십시오.

1. 클릭 **열 추가**, 입력 시작 **실제 시간** http 화이트보드 **이 열에 표시** 드롭다운 필드가 표시됩니다. 목록에 해당 필드가 나타나면 필드를 선택합니다.

1. 클릭 **저장 + 닫기** 보고서를 저장합니다.

   실제 시간 열에는 각 작업에 로그온한 시간이 표시됩니다.

### 리소스 관리 도구의 실제 시간 {#actual-hours-in-resource-management-tools}

사용자가 할당된 작업 및 문제에 대해 수행하는 작업의 진행 상황을 보려면 다음 리소스 관리 도구에서 볼 수 있습니다.

* 활용률 보고서.\
   활용률 보고서에 대한 자세한 내용은 [자원 가동률 보고서 개요](../../../reports-and-dashboards/reports/using-built-in-reports/resource-utilization-report.md).

* 리소스 플래너.

   리소스 계획자에서 실제 시간 보기에 대한 자세한 내용은 [사용자 뷰를 사용할 때 리소스 계획자에서 사용 가능한 시간, 계획 시간 또는 실제 시간 또는 FTE 보기](../../../resource-mgmt/resource-planning/view-hours-fte-user-view-resource-planner.md).

## 로그 시간

여러 가지 방법으로 작업, 문제 및 프로젝트에 대한 시간을 기록할 수 있습니다.

Workfront에서 로깅 시간에 대한 자세한 내용은 [로그 시간](../../../timesheets/create-and-manage-timesheets/log-time.md).
