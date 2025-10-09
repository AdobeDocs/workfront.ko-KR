---
content-type: overview
product-area: projects
navigation-topic: task-information
title: 실제 근로시간 보기
description: Adobe Workfront에서 작업 항목에 로그온하는 시간은 실제 시간으로 간주됩니다. 실제 근로시간은 작업, 문제 또는 프로젝트를 완료하는 데 걸린 실제 시간을 나타냅니다.
author: Alina
feature: Work Management
exl-id: c4b0e431-1765-416d-89f5-6ac663ac1d4f
source-git-commit: d577fb1f84c2a91c7b4a37be271235ffa338c9fd
workflow-type: tm+mt
source-wordcount: '1253'
ht-degree: 0%

---

# 실제 근로시간 보기

<!-- Audited: 5/2025 -->

Adobe Workfront에서 작업 항목에 로그온하는 시간은 실제 시간으로 간주됩니다.

실제 근로시간은 작업, 문제 또는 프로젝트를 완료하는 데 걸린 실제 시간을 나타냅니다.

작업과 문제인 작업 항목에 시간을 기록하는 것이 좋습니다. 그러나 Workfront 관리자는 사용자가 조직의 워크플로에 따라 프로젝트에 시간을 기록하도록 허용할 수 있습니다.

사용자가 프로젝트에 시간을 기록할 수 있도록 시스템을 설정하는 방법에 대한 자세한 내용은 [타임시트 및 시간 환경 설정 구성](../../../administration-and-setup/set-up-workfront/configure-timesheets-schedules/timesheet-and-hour-preferences.md)을 참조하십시오.

## 액세스 요구 사항

+++ 을 확장하여 이 문서의 기능에 대한 액세스 요구 사항을 봅니다.

이 문서의 단계를 수행하려면 다음 액세스 권한이 있어야 합니다.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront 플랜</td> 
   <td> <p>임의</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront 라이센스*</td> 
   <td> 
   <p>새로운 기능: 표준<p>
   <p>또는</p>
   <p>현재: 작업 시간 이상</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">액세스 수준 구성</td> 
   <td> <p>작업, 프로젝트 또는 문제에 대한 보기 이상의 액세스 권한</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">개체 권한</td> 
   <td> <p>작업, 프로젝트 또는 문제에 대한 이상의 권한 보기</p> <p>추가 액세스 요청에 대한 자세한 내용은 <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">개체 </a>에 대한 액세스 요청 을 참조하십시오.</p> </td> 
  </tr> 
 </tbody> 
</table>

*이 표의 정보에 대한 자세한 내용은 [Workfront 설명서의 액세스 요구 사항](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)을 참조하십시오.

+++

## 실제 근로시간과 기존 실제 근로시간 비교

실제 시간을 액세스하는 Workfront의 영역에 따라 다음 로그 시간 중 하나를 참조할 수 있습니다.

* 프로젝트, 작업 및 문제 보고서와 목록:

   * **실제 시간**: 2021년 5월 이후 프로젝트, 작업 또는 문제에 기록된 시간입니다. 이 매개 변수는 몇 시간 후에 Workfront 데이터베이스에 저장되며 해당 value 필드는 `actualWorkRequiredDouble`입니다.
   * **기존 실제 시간**: 2021년 5월 이전을 포함하여 언제든지 프로젝트, 작업 또는 문제에 기록된 시간입니다. 분 단위로 Workfront 데이터베이스에 저장되며 해당 value 필드는 `actualWorkRequired`입니다.

     >[!IMPORTANT]
     >
     >프로젝트의 실제 비용은 기존 실제 시간을 사용하여 계산됩니다.

* 프로젝트, 작업 또는 문제 세부 정보 영역에서 실제 시간이 다음 필드에 표시될 수 있습니다.

   * **실제 시간**: 세부 정보 탭에서 2021년 5월 이후의 프로젝트, 작업 또는 문제에 대해 기록된 시간입니다. 이 매개 변수는 몇 시간 후에 Workfront 데이터베이스에 저장되며 해당 value 필드는 `actualWorkRequiredDouble`입니다.
   * **실제 시간**: 프로젝트, 작업 또는 문제 사용자 정의 양식에서 실제 시간 네이티브 필드를 참조하는 네이티브 필드 참조 사용자 정의 필드를 사용하여 액세스한 경우. 2021년 5월 이후 프로젝트, 작업 또는 문제에 대해 기록된 시간입니다. 이 매개 변수는 몇 시간 후에 Workfront 데이터베이스에 저장되며 해당 value 필드는 `actualWorkRequiredDouble`입니다.

>[!NOTE]
>
>기존의 실제 시간 필드는 증분이 반올림되는 방식으로 인해 부정확한 시간이 표시될 수 있으므로 가능할 때마다 실제 시간 필드를 사용하는 것이 좋습니다.

## 작업 및 문제의 실제 시간과 프로젝트의 실제 시간 비교

작업 및 문제의 실제 시간은 작업 및 문제에 직접 기록된 시간을 나타냅니다.

하위 작업의 실제 시간은 상위 작업의 실제 시간으로 롤업됩니다. 다음 공식은 상위 작업의 실제 시간에 적용됩니다.

```
Parent Task Actual Hours = All Tasks Actual Hours + Parent Task Actual Hours
```

프로젝트의 실제 시간은 모든 프로젝트 작업(상위 작업에 직접 기록된 시간 포함), 모든 프로젝트 문제 및 프로젝트에 기록된 실제 시간의 총 합계를 나타냅니다.

다음 공식은 프로젝트의 실제 시간에 적용됩니다.

```
Project Actual Hours = All Tasks Actual Hours + All Issues Actual Hours + All Project Actual Hours
```

## 실제 근로시간 찾기

항목에 대한 실제 시간 값을 찾는 것은 작업, 프로젝트 및 문제에 대해 동일합니다.

### 세부 정보 섹션의 실제 시간 {#actual-hours-in-the-details-section}

세부 정보 섹션의 실제 시간 찾기는 프로젝트, 작업 및 문제에 대해 동일합니다.

작업 세부 정보에서 실제 시간을 찾으려면 다음을 수행합니다.

1. 실제 근로시간을 검토할 작업으로 이동합니다.
1. 왼쪽 패널에서 **작업 세부 정보**&#x200B;를 클릭합니다. **개요** 섹션이 표시됩니다.
1. **작업 시간** 섹션에서 **실제 근로시간** 값을 찾습니다. 이 작업에 기록된 총 시간입니다.
1. (선택 사항 및 조건부) 실제 시간 기본 필드 참조가 프로젝트, 작업 또는 문제 사용자 정의 양식에 추가된 경우 사용자 정의 양식으로 이동하여 사용자 정의 필드에서 실제 시간을 찾습니다. 개체에 기록된 총 시간입니다.

### 시간 섹션의 실제 시간 {#actual-hours-in-the-hours-section}

시간 섹션의 실제 시간 찾기는 프로젝트, 작업 및 문제에 대해 동일합니다.

작업의 시간 섹션에서 실제 시간을 찾으려면 다음을 수행합니다.

1. 실제 근로시간을 검토할 작업으로 이동합니다.

1. 왼쪽 패널에서 **시간**&#x200B;을 클릭합니다. 작업에 기록된 시간 항목 목록이 표시되고 **시간** 열에 작업에 대한 총 실제 시간이 표시됩니다.

1. **표준** 보기 및 **프로젝트** 그룹화가 이 목록에 적용되었는지 확인하십시오.
1. 작업의 실제 시간이 **실제 시간** 열의 그룹화 줄에 표시됩니다.

### 보고서의 실제 근로시간 및 레거시 실제 근로시간

작업, 문제 또는 프로젝트 보고서를 작성할 때 보고서의 각 작업, 문제 또는 프로젝트에 대한 실제 근로시간 및 이전 실제 근로시간 값을 표시할 수 있습니다.

실제 시간과 기존 실제 시간의 차이에 대한 자세한 내용은 이 문서의 [실제 시간과 기존 실제 시간](#actual-hours-vs-legacy-actual-hours) 섹션을 참조하십시오.

작업 보고서에 실제 근로시간 및 기존 실제 근로시간을 표시하려면 다음을 수행합니다.

{{step1-to-reports}}

1. **보고서** 페이지에서 **새 보고서**&#x200B;를 클릭한 다음 **작업**&#x200B;을 개체로 선택하십시오.
1. 페이지의 오른쪽 아래 모서리에서 **열 추가**&#x200B;를 클릭합니다.
1. **이 열에 표시** 드롭다운 필드에서 **실제 시간**&#x200B;을 입력한 다음 목록에 표시될 때 필드를 선택합니다.
1. 위의 단계를 반복하여 **기존 실제 근로시간** 필드를 보고서에 추가합니다.

1. 페이지의 왼쪽 하단 모서리에서 **저장 + 닫기**&#x200B;를 클릭하여 보고서를 저장합니다.

1. **이 보고서의 이름을 지정하여 저장** 대화 상자에서 새 보고서 이름을 입력한 다음 **적용**&#x200B;을 클릭합니다.
1. 프로젝트 또는 문제 보고서에 대해 동일한 단계를 반복합니다.

### 리소스 관리 도구의 실제 근로시간 {#actual-hours-in-resource-management-tools}

사용자가 할당된 작업 및 문제에 대해 수행하는 작업의 진행 상황을 보려면 다음 리소스 관리 도구에서 볼 수 있습니다.

* 활용성 보고서.\
  자세한 내용은 [리소스 사용률 보고서 개요](../../../reports-and-dashboards/reports/using-built-in-reports/resource-utilization-report.md)를 참조하십시오.

* 리소스 플래너.

  자세한 내용은 사용자 보기를 사용할 때 리소스 플래너에서 [사용 가능 시간, 계획된 시간 및 실제 시간 또는 FTE 보기](../../../resource-mgmt/resource-planning/view-hours-fte-user-view-resource-planner.md)를 참조하십시오.


### Workfront API의 실제 시간

<!--this section was added as a result to this issue: https://experience.adobe.com/#/@adobeinternalworkfront/so:hub-Hub/workfront/task/6810910e0001b932e0948336208e76f2/overview-->

시간을 저장하는 대부분의 Workfront 필드는 Workfront 데이터베이스에 분 단위로 저장됩니다. 예를 들어 작업의 계획된 시간 필드 이름은 Workfront 데이터베이스에서 `workRequired`이고 분 단위로 저장됩니다.

API 호출이나 계산된 사용자 지정 필드 또는 열의 이러한 필드에 액세스할 때 분 단위에서 시간 단으로의 전환을 고려해야 합니다.

프로젝트, 작업 또는 문제에 대해 기록된 실제 시간이 현재 Workfront 데이터베이스에 분으로 저장되어 있으며 해당 valuefield는 `actualWorkRequired`입니다.

다음 버전의 Workfront API는 2025년 말에 릴리스될 예정이며, 실제 시간은 데이터베이스의 다음 필드 및 단위에 저장됩니다.

* **실제 시간**: 2021년 5월 이후 프로젝트, 작업 또는 문제에 기록된 시간입니다. 이 매개 변수는 몇 시간 후에 Workfront 데이터베이스에 저장되며 해당 value 필드는 `actualWorkRequiredDouble`입니다.
* **기존 실제 시간**: 2021년 5월 이전을 포함하여 언제든지 프로젝트, 작업 또는 문제에 기록된 시간입니다. 분 단위로 Workfront 데이터베이스에 저장되며 해당 value 필드는 `actualWorkRequired`입니다.

  >[!IMPORTANT]
  >
  >프로젝트의 실제 비용은 기존 실제 시간을 사용하여 계산됩니다.

  계산된 열 또는 필드에서 실제 시간을 사용하는 방법에 대한 자세한 내용은 [보고서 FAQ](/help/quicksilver/reports-and-dashboards/reports/tips-tricks-and-troubleshooting/reports-faq.md)를 참조하십시오.

## 로그 시간

작업, 문제 및 프로젝트에 여러 가지 방법으로 시간을 기록할 수 있습니다.

자세한 내용은 [로그 시간](../../../timesheets/create-and-manage-timesheets/log-time.md)을 참조하세요.
