---
content-type: overview
product-area: timesheets
navigation-topic: timesheets-navigation-topic
title: 타임시트 개요
description: 타임시트를 사용하여 작업에 소비하는 시간을 추적할 수 있습니다. Adobe Workfront의 타임시트 레이아웃에 대한 자세한 내용은 타임시트 레이아웃 이해를 참조하십시오.
author: Alina
feature: Timesheets
exl-id: 2174a879-4a19-4a0f-803a-f19a8909f227
source-git-commit: 48f46abab1958325aba6832b85247dc2c80f4e80
workflow-type: tm+mt
source-wordcount: '707'
ht-degree: 0%

---

# 타임시트 개요

타임시트를 사용하여 Adobe Workfront에서 작업에 소비하는 시간을 추적할 수 있습니다.

Workfront 또는 그룹 관리자는 타임시트를 만들고 사용자와 연결할 수 있습니다. 타임시트 만들기에 대한 자세한 내용은 [타임시트 만들기 및 관리](../create-and-manage-timesheets/create-and-manage-timesheets.md).

타임시트는 작업 항목과 달력 영역을 표시하는 그리드 형식 테이블입니다. 항목에 대한 시간을 기록하고 작업을 수행한 날짜와 연결할 수 있습니다. Workfront에서의 실제 작업 시간을 추적합니다. 타임시트에는 회의, 교육 또는 사무실 외 시간과 같은 업무 외 항목에 대한 시간을 기록할 수 있는 영역도 있습니다.

Adobe Workfront의 타임시트 레이아웃에 대한 자세한 내용은 [타임시트 레이아웃 이해](../../timesheets/timesheets/timesheet-layout.md).

![](assets/timesheet-example.png)

일반적으로 작업이 수행되는 프로젝트, 작업 또는 문제 수준에서 다양한 방법으로 Workfront에 시간을 기록할 수 있습니다. 작업, 문제 및 프로젝트에 대해 기록된 시간도 타임시트에 표시됩니다.

일반 시간 아래에서 프로젝트가 아닌 작업에 대한 시간을 기록할 수도 있습니다. 일반 시간 시간은 타임시트에만 기록할 수 있습니다.

Workfront에서 시간을 기록할 수 있는 위치에 대한 자세한 내용은 [로그 시간](../../timesheets/create-and-manage-timesheets/log-time.md).

>[!TIP]
>
>또한 Workfront 모바일 앱을 사용하여 업데이트를 게시하고, 기록된 시간을 변경하고, 댓글을 입력하고, 타임시트를 닫을 수 있습니다.

## 액세스 요구 사항

이 문서의 단계를 수행하려면 다음이 있어야 합니다.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront 플랜</td> 
   <td> <p>모든</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront 라이선스</td> 
   <td> <p>플랜 </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">액세스 수준 구성*</td> 
   <td> <p>타임시트에 대한 관리 액세스 권한이 있어야 합니다. </p> <p>자세한 내용은 <a href="../../administration-and-setup/add-users/configure-and-grant-access/grant-users-admin-access-certain-areas.md" class="MCXref xref">사용자에게 특정 영역에 대한 관리 액세스 권한 부여</a>.</p> <p><b>메모</b>

여전히 액세스 권한이 없는 경우 Workfront 관리자에게 액세스 수준에 추가 제한을 설정하는지 문의하십시오. Workfront 관리자가 액세스 수준을 수정하는 방법에 대한 자세한 내용은 <a href="../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">사용자 정의 액세스 수준 만들기 또는 수정</a>.</p> </td>
</tr> 
 </tbody> 
</table>

&#42;보유 중인 플랜, 라이선스 유형 또는 액세스 권한을 확인하려면 Workfront 관리자에게 문의하십시오.


## 프로젝트 시간과 비프로젝트 시간 이해

타임시트는 사용자가 프로젝트와 비프로젝트 작업 모두에 대한 시간을 추적할 수 있는 간단한 방법을 제공합니다.

* **프로젝트 시간:** 시간을 추적할 작업 또는 프로젝트에서 직접 가져옵니다.

  타임시트를 통해 작업, 문제 및 프로젝트에 기록된 시간은 프로젝트 및 작업에 소요된 노력을 정확하게 나타내기 위해 각 작업 항목과 연결됩니다. 정확한 시간 입력이 없으면 청구 목적으로 데이터가 정확하지 않을 수 있습니다.

  또한 리소스가 작업에 시간을 직접 기록할 때 사용자가 타임시트에 액세스할 때 문제 및 프로젝트가 자동으로 표시됩니다. 타임시트 날짜 범위가 시간이 기록된 날짜에 걸쳐 있다고 가정합니다.

* **프로젝트 외 시간:** 사용자 타임시트에서 바로 확인할 수 있습니다. Workfront에서 시간을 추적하는 방법에 대한 자세한 내용은 다음을 참조하십시오.   [로그 시간](../../timesheets/create-and-manage-timesheets/log-time.md).

  타임시트에서 자원은 휴가 시간, 병가 시간, 수송 시간, 장비 수리 또는 유지 관리 시간 또는 만들려는 일반 오버헤드 시간 유형을 기록할 수 있습니다.

## 타임시트 영역의 타임시트에 액세스

시간을 기록할 수 있는 Workfront의 모든 영역에 대한 자세한 내용은 [로그 시간](../../timesheets/create-and-manage-timesheets/log-time.md).

타임시트에 액세스하려면:

1. 다음을 클릭합니다. **메인 메뉴** 아이콘 ![](assets/dots-main-menu.png) 오른쪽 상단 또는 **메인 메뉴** 아이콘 ![](assets/lines-main-menu.png) Workfront의 왼쪽 상단 모서리에서 사용 가능한 경우 타임시트를 클릭합니다.

   타임시트 영역에는 기본적으로 사용자가 소유하거나 보기 액세스 권한이 있는 모든 타임시트가 표시됩니다.

   ![](assets/all-timesheets-list-nwe-350x68.png)

1. 오른쪽 상단에서 다음 옵션 중 하나를 클릭하여 제한된 수의 타임시트를 표시합니다.

   * **내 타임시트** 타임시트만 표시합니다.

   ![](assets/my-timesheets-list-various-statuses-nwe-350x60.png)

   * **내 타임시트 승인** 승인한 타임시트만 표시합니다.

     ![](assets/timesheets-i-approve-list-with0filters-new-nwe-350x61.png)

   필터링된 타임시트 목록이 표시됩니다.

1. (선택 사항) 타임시트 목록 맨 위에서 보기, 필터 및 그룹화를 업데이트합니다. 자세한 내용은 [보고 요소: 필터, 보기 및 그룹화](../../reports-and-dashboards/reports/reporting-elements/reporting-elements-overview.md).

1. 다음을 클릭합니다. **날짜 범위** 타임시트를 열어 보십시오.

   각 타임시트에는 시간을 기록한 모든 작업, 문제 및 프로젝트가 표시됩니다. 타임시트에는 타임시트의 시간대 내에 날짜가 있는 사용자에게 할당되었지만 아직 시간이 기록되지 않은 최대 45개의 작업, 문제 또는 프로젝트도 표시됩니다.

   자세한 내용은 [타임시트 및 시간 환경 설정 구성](../../administration-and-setup/set-up-workfront/configure-timesheets-schedules/timesheet-and-hour-preferences.md).



