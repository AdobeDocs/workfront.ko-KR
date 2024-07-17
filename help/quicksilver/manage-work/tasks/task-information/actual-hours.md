---
content-type: overview
product-area: projects
navigation-topic: task-information
title: 실제 근로시간 보기
description: Adobe Workfront에서 작업 항목에 로그온하는 시간은 실제 시간으로 간주됩니다.
author: Alina
feature: Work Management
exl-id: c4b0e431-1765-416d-89f5-6ac663ac1d4f
source-git-commit: f2f825280204b56d2dc85efc7a315a4377e551c7
workflow-type: tm+mt
source-wordcount: '796'
ht-degree: 0%

---

# 실제 근로시간 보기

Adobe Workfront에서 작업 항목에 로그온하는 시간은 실제 시간으로 간주됩니다.

실제 근로시간은 작업, 문제 또는 프로젝트를 완료하는 데 걸린 실제 시간을 나타냅니다.

작업과 문제인 작업 항목에 시간을 기록하는 것이 좋습니다.

하지만 Workfront 관리자는 조직의 워크플로우에 따라 사용자가 프로젝트에 시간을 기록하도록 허용할 수 있습니다.

사용자가 프로젝트에 시간을 기록할 수 있도록 시스템을 설정하는 방법에 대한 자세한 내용은 [타임시트 및 시간 환경 설정 구성](../../../administration-and-setup/set-up-workfront/configure-timesheets-schedules/timesheet-and-hour-preferences.md)을 참조하십시오.

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
   <td> <p>작업, 프로젝트 또는 문제에 대한 보기 이상의 액세스 권한</p> <p>참고: 여전히 액세스 권한이 없는 경우 Workfront 관리자에게 액세스 수준에서 추가 제한을 설정하는지 문의하십시오. Workfront 관리자가 액세스 수준을 수정하는 방법에 대한 자세한 내용은 <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">사용자 지정 액세스 수준 만들기 또는 수정</a>을 참조하십시오.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">개체 권한</td> 
   <td> <p>작업, 프로젝트 또는 문제에 대한 이상의 권한 보기</p> <p>추가 액세스 요청에 대한 자세한 내용은 <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">개체 </a>에 대한 액세스 요청 을 참조하십시오.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;보유 중인 플랜, 라이선스 유형 또는 액세스 권한을 확인하려면 Workfront 관리자에게 문의하십시오.

## 작업 및 문제의 실제 시간과 프로젝트의 실제 시간 비교

작업 및 문제의 실제 시간은 작업 및 문제에 직접 기록된 시간을 나타냅니다.

>[!NOTE]
>
>하위 작업의 실제 시간은 상위 작업의 실제 시간으로 롤업됩니다. 다음 공식은 상위 작업의 실제 시간에 적용됩니다.

```
Parent Task Actual Hours = All Tasks Actual Hours + Parent Task Actual Hours
```

프로젝트의 실제 시간은 프로젝트에 대한 모든 작업(상위 작업에 직접 기록된 시간 포함), 프로젝트에 대한 모든 문제 및 프로젝트에 기록된 실제 시간의 총 실제 시간을 나타냅니다.

다음 공식은 프로젝트의 실제 시간에 적용됩니다.

```
Project Actual Hours = All Tasks Actual Hours + All Issues Actual Hours + All Project Actual Hours
```

## 실제 근로시간 찾기

항목에 대한 실제 시간 값을 찾는 것은 작업, 프로젝트 및 문제에 대해 동일합니다.

작업에 대한 실제 근로시간 정보는 다음 위치에서 찾을 수 있습니다.

* [세부 정보 섹션의 실제 근로시간](#actual-hours-in-the-details-section)
* [시간 섹션의 실제 근로시간](#actual-hours-in-the-hours-section)
* [보고서의 실제 근로시간](#actual-hours-in-reports)
* [리소스 관리 도구의 실제 근로시간](#actual-hours-in-resource-management-tools)

### 세부 정보 섹션의 실제 시간 {#actual-hours-in-the-details-section}

세부 정보 섹션의 실제 시간 찾기는 프로젝트, 작업 및 문제에 대해 동일합니다.

작업 세부 정보에서 실제 시간을 찾으려면 다음을 수행합니다.

1. 실제 시간을 검토할 작업으로 이동합니다.
1. 왼쪽 패널에서 **작업 세부 정보**&#x200B;를 클릭합니다.
1. **개요**&#x200B;를 클릭하고 **실제 근로시간** 값을 확인합니다.

   이 작업에 기록된 총 시간입니다.

### 시간 섹션의 실제 시간 {#actual-hours-in-the-hours-section}

시간 섹션의 실제 시간 찾기는 프로젝트, 작업 및 문제에 대해 동일합니다.

시간 섹션에서 실제 시간을 찾으려면 다음을 수행하십시오.

1. 실제 시간을 검토할 작업으로 이동합니다.
1. 왼쪽 패널에서 **시간**&#x200B;을 클릭합니다.

   구성에 따라 시간 섹션이 **자세히 표시** 아래에 나열될 수 있습니다.

   작업에 기록된 시간 항목 목록이 표시됩니다.

1. **표준** 보기 및 **프로젝트** 그룹화가 이 목록에 적용되었는지 확인하십시오.

   **Hours** 열의 그룹화 줄에 표시된 숫자는 작업의 총 실제 시간 수입니다.

### 보고서의 실제 근로시간 {#actual-hours-in-reports}

작업, 문제 또는 프로젝트 보고서를 작성할 때 보고서에서 각 작업, 문제 또는 프로젝트에 대한 실제 시간 값을 표시할 수 있습니다.

작업 보기에 실제 시간 열을 추가하는 것은 보고서에서 보기를 작성하는 것과 비슷합니다.

작업 보고서에 실제 근로시간을 표시하려면

1. Workfront 오른쪽 상단의 **기본 메뉴** 아이콘 ![](assets/main-menu-icon.png)을(를) 클릭한 다음 **보고서**&#x200B;를 클릭합니다.
1. **새 보고서**&#x200B;를 클릭한 다음 **작업**&#x200B;을(를) 개체로 선택하십시오.

1. **열 추가**&#x200B;를 클릭하고 **이 열에 표시** 드롭다운 필드가 표시되면 **실제 시간**&#x200B;을 입력하세요. 목록에 표시될 때 필드를 선택합니다.

1. 보고서를 저장하려면 **저장 + 닫기**&#x200B;를 클릭하십시오.

   실제 작업 시간 열에는 각 작업에 기록된 시간이 표시됩니다.

### 리소스 관리 도구의 실제 근로시간 {#actual-hours-in-resource-management-tools}

사용자가 할당된 작업 및 문제에 대해 수행하는 작업의 진행 상황을 보려면 다음 리소스 관리 도구에서 볼 수 있습니다.

* 활용성 보고서.\
  사용률 보고서에 대한 자세한 내용은 [리소스 사용률 보고서 개요](../../../reports-and-dashboards/reports/using-built-in-reports/resource-utilization-report.md)를 참조하십시오.

* 리소스 플래너.

  리소스 플래너에서 실제 시간을 보는 방법에 대한 자세한 내용은 [사용자 보기를 사용할 때 리소스 플래너에서 사용 가능한 시간, 계획된 시간 및 실제 시간 또는 FTE 보기](../../../resource-mgmt/resource-planning/view-hours-fte-user-view-resource-planner.md)를 참조하십시오.

## 로그 시간

작업, 문제 및 프로젝트에 여러 가지 방법으로 시간을 기록할 수 있습니다.

Workfront의 로깅 시간에 대한 자세한 내용은 [로그 시간](../../../timesheets/create-and-manage-timesheets/log-time.md)을 참조하십시오.
