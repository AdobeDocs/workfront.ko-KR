---
product-area: timesheets
navigation-topic: create-and-manage-timesheets
title: 로그 시간
description: Adobe Workfront에서 작업 항목의 시간을 로그하여 작업 시간을 표시할 수 있습니다(&N). 휴가, 병가 시간, 모임 시간 등 업무와 관련이 없는 로그 타임도 가능합니다. 기록표에 표시하는 시간입니다.
author: Alina
feature: Timesheets
exl-id: 120173a8-95f1-4233-ab40-d3bcfe38c977
source-git-commit: b2859f3d268bd947fba5bb0280677465b3039d93
workflow-type: tm+mt
source-wordcount: '2992'
ht-degree: 0%

---

# 로그 시간

Adobe Workfront에서 작업 항목에 대한 시간을 로그하여 작업 시간을 지정할 수 있습니다. 휴가, 병가 시간, 모임 시간 등 업무와 관련이 없는 로그 타임도 가능합니다. 기록표에 표시하는 시간입니다.

Workfront에 로그인할 수 있는 시간 유형에 대한 자세한 내용은 [시간 유형 관리](../../administration-and-setup/set-up-workfront/configure-timesheets-schedules/hour-types.md).

## 액세스 요구 사항

<!--drafted for P&P - replace the table:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront plan*</td> 
   <td> <p>Any</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront license*</td> 
   <td> <p>Current license: Light or higher</p>
   <p>Legacy license: 
   <ul><li>Review or higher to log General Hours in a timesheet</li>
   <li>Work or higher to log hours on a project, task, or issue</li></ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Access level configurations*</td> 
   <td> <p>Edit access to the type of work item you log time for </p> <p>For example, you need Edit access to Issues, to log time for issues</p> <p>If you still don't have access, ask your Workfront administrator if they set additional restrictions in your access level. For information on how a Workfront administrator can modify your access level, see <a href="../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Create or modify custom access levels</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Object permissions</td> 
   <td> <p>Contribute or higher permissions on the work item you log time for that includes permissions to Log Hours</p> <p>For information on requesting additional access, see <a href="../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Request access to objects </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>
-->

이 문서의 단계를 수행하고 프로젝트 특정 시간을 기록하려면 다음 액세스 권한이 있어야 합니다.

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
   <td> <ul><li>작업표에 일반 시간을 기록하려면 검토 또는 그 이상</li>
   <li> 프로젝트, 작업 또는 문제에 대해 몇 시간 이상 로그온하는 작업</li></ul>
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader">액세스 수준 구성*</td> 
   <td> <p>작업 항목 유형에 대한 액세스 편집 </p> <p>예를 들어 문제에 대한 편집 액세스 권한이 있어야 문제를 기록할 수 있습니다</p> <p>여전히 액세스 권한이 없는 경우 Workfront 관리자에게 액세스 수준에서 추가 제한 사항을 설정하는지 문의하십시오. Workfront 관리자가 액세스 수준을 수정하는 방법에 대한 자세한 내용은 <a href="../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">사용자 정의 액세스 수준 만들기 또는 수정</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">개체 권한</td> 
   <td> <p>로그 시간에 대해 기록하는 작업 항목에 대한 Contribute 또는 더 높은 사용 권한에 로그 시간에 대한 사용 권한이 포함됩니다.</p> <p>추가 액세스 요청에 대한 자세한 내용은 <a href="../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">개체에 대한 액세스 요청 </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

*보유하고 있는 플랜, 라이선스 유형 또는 액세스를 알아보려면 Workfront 관리자에게 문의하십시오.

## Workfront에서 시간 로깅 시 고려 사항

* 프로젝트, 작업 또는 문제에 대한 시간을 기록하거나 작업표에 직접 시간을 기록할 수 있습니다.

   작업표 작성에 대한 자세한 내용은 [단일 사용 작업표 만들기](../../timesheets/create-and-manage-timesheets/create-tmshts.md).

* 작업표 이외의 다른 도구를 통해 기록되는 모든 시간은 해당 기간의 작업표에 나타납니다.
* 현재 상태가 아닌 프로젝트의 작업 및 문제는 작업표에 미리 채워지지 않습니다.
* 작업표에 기록된 시간은 작업, 문제 또는 프로젝트에 즉시 적용됩니다.
* 작업표에는 모든 로그된 날짜에 대한 총 시간이 포함됩니다. 에 설명된 대로 타임라인 계산이 제외되도록 구성된 경우에도 주말은 항상 포함됩니다 [시스템 전체 프로젝트 환경 설정 구성](../../administration-and-setup/set-up-workfront/configure-system-defaults/set-project-preferences.md)).
* 작업표에 표시되는 최대 항목 수는 45개입니다. 작업표 시간대와 일치하는 날짜가 45개 이상인 항목이 있는 경우 가장 최근에 업데이트된 항목만 표시됩니다.
* 청구된 청구 레코드에 포함된 시간 항목은 흐리게 표시되어 작업표에서 편집할 수 없습니다. 자세한 내용은 [청구 레코드 만들기](../../manage-work/projects/project-finances/create-billing-records.md).

## 로그 시간

Workfront의 다음 영역에서 시간을 로그인할 수 있습니다.

* [타임시트](#timesheet)
* [홈](#home)
* [프로젝트, 작업 또는 문제](#project-task-or-issue)
* [요약 패널](#summary-panel)
* [보드](#boards)
* [모바일 앱](#mobile-app)

### 타임시트 {#timesheet}

작업표에 일반 시간이나 프로젝트 특정 시간을 기록할 수 있습니다.

>[!NOTE]
>
>작업표 프로필에 할당된 사용자를 검토하면 작업표 탭과 로그 일반 시간을 볼 수 있습니다. 그러나 작업표에 나타나는 작업이나 문제에 대해 시간을 기록하지 못합니다.

1. 을(를) 클릭합니다. [!UICONTROL **기본 메뉴**] 아이콘 ![](assets/main-menu-icon.png) Adobe Workfront의 오른쪽 상단 모서리에서

1. 클릭 [!UICONTROL **작업표**]. 현재 작업표가 기본적으로 표시됩니다.
   ![타임시트](assets/timesheet-redesigned-nwe.png)

   작업표의 기간 동안 작업표에 할당된 항목으로 미리 채워집니다. 작업표의 미리 채우기 방법에 대한 자세한 내용은 [작업표 및 시간 환경 설정 구성](../../administration-and-setup/set-up-workfront/configure-timesheets-schedules/timesheet-and-hour-preferences.md). 작업표에 항목이 표시되지 않으면 추가할 수 있습니다.

   >[!NOTE]
   >
   >작업표는 사용자에게 할당된 항목만 미리 채웁니다. 팀 또는 작업 역할에 할당된 항목으로 미리 채우지 않습니다.
   >
   >팀에 할당된 항목에 있는 작업에 대한 작업 을 클릭하면 해당 항목이 사용자에게 할당되고 해당 항목이 작업표에 표시됩니다.


1. (선택 사항) **전체 화면** 아이콘 ![](assets/full-screen.png) 작업표를 전체 화면 모드로 표시하려면 **exit-full-screen** ![](assets/exit-full-screen.png) 작업표로 돌아갈 아이콘입니다.

   <!-- drafted for the resize columns in timesheet story: 1. (optional) Click on the separator lines between weeks or between the time frame area and the work item area to resize the columns of the timesheet.-->

1. (선택 사항) 작업표에 프로젝트, 작업 또는 문제를 추가하려면 **항목 추가** 작업표의 왼쪽 위 모서리에 있는 드롭다운 메뉴를 클릭한 다음 **프로젝트 추가**, **작업 추가**, 또는 **문제 추가**.

   프로젝트, 작업 또는 문제 목록이 표시됩니다.

   <!--drafted for full screen mode for add projects story - align it with the rest of the steps when you enable this:: 1. (Optional) Click the **full-screen** icon ![](assets/full-screen.png) to display the list of objects in full-screen mode.-->

1. (선택 사항) 검색 아이콘을 클릭합니다 ![항목 검색](assets/search-icon.png) 작업표에 추가할 키워드를 사용하여 특정 항목을 검색하려면

1. (선택 사항) 필터, 보기 또는 그룹화 드롭다운 메뉴를 확장하여 메뉴를 적용하거나 사용자 정의하여 원하는 항목 정보를 봅니다.

1. 목록에서 하나 또는 여러 항목을 선택한 다음 를 클릭합니다 **추가**.

   >[!NOTE]
   >
   >작업표에 작업이나 문제를 추가하면 프로젝트가 추가됩니다.


1. (조건부) 한 번에 50개 이상의 항목을 추가하면 작업표에 추가된 항목 수가 표시되는 확인 메시지가 표시됩니다.

   클릭 **모두 추가** 모든 항목을 추가하려면 를 클릭하고, **취소** 선택한 항목의 추가를 중지하려면 **취소** 를 클릭하여 항목 목록을 닫습니다.

   작업 및 문제는 프로젝트 이름 아래에 나열됩니다.

   >[!NOTE]
   >
   >작업표에 수동으로 추가하는 항목은 고정되어 있으며, 사용자가 수동으로 작업표를 제거하여 제거할 때까지 현재 작업표와 향후 작업표에 유지됩니다. 작업표에서 제거할 항목을 고정하지 않는 방법에 대한 자세한 내용은 10단계를 계속 진행하십시오.

   <!--(ensure this stays accurate)-->

1. (선택 사항) **축소** ![](assets/collapse-icon.png) 또는 **확장** ![](assets/expand-icon.png) 프로젝트 이름 옆에 있는 아이콘을 사용하여 프로젝트의 작업 및 문제 목록을 표시하거나 숨깁니다.


   >[!TIP]
   >
   >   표준 QWERTY 키보드를 사용할 때 작업표에서 프로젝트 이름을 클릭한 후 다음 키 집합을 눌러 프로젝트를 축소하거나 확장합니다.
   >   * 프로젝트를 확장하고 해당 작업 항목을 표시하려면 다음을 수행하십시오.
      >     * Shift + Alt + Windows 컴퓨터의 위쪽 화살표
      >     * Shift + Option + Mac 컴퓨터의 위쪽 화살표
   >   * 프로젝트를 축소하고 작업 항목을 숨기려면
      >     * Shift + Alt + Windows 컴퓨터의 아래쪽 화살표
      >     * Shift + Option + Mac 컴퓨터의 아래쪽 화살표.



1. (선택 사항) 작업표에 자동으로 표시되는 항목을 수동으로 고정하려면 항목 이름을 마우스로 가리킨 다음 **핀** 아이콘 ![](assets/empty-pin-icon.png).

   >[!TIP]
   >
   >   작업표에서 항목을 클릭한 후 표준 QWERTY 키보드를 사용하는 경우 다음 키 집합을 눌러 항목을 고정할 수 있습니다.
   >   * Windows 및 Mac 컴퓨터 모두에 대한 옵션 + P.



1. (선택 사항) 검색 아이콘을 클릭합니다 ![](assets/search-icon.png) 그리고 작업표에서 프로젝트, 작업 또는 문제를 찾기 위한 키워드 입력을 시작합니다.

1. (선택 사항) 항목을 수동으로 추가한 경우(단계 3-6에서 설명한 대로), 항목을 고정 해제하여 기록하지 않은 경우 작업표에서 항목(프로젝트, 작업 또는 문제)을 제거할 수 있습니다. <!--ensure this stays accurate-->

   작업표를 미리 채우도록 구성된 Workfront 시스템이나 그룹의 작업표 환경 설정에 따라 작업표에 포함된 항목을 자동으로 제거할 수 없습니다. [작업표 및 시간 환경 설정 구성](../../administration-and-setup/set-up-workfront/configure-timesheets-schedules/timesheet-and-hour-preferences.md).

   수동으로 추가한 작업표에서 항목을 제거하려면 다음을 수행하십시오.

   1. 항목에 대해 기록된 시간이 없는지 확인합니다.
   1. 을(를) 클릭합니다. **고정** 아이콘 ![항목 고정](assets/pin-icon.png) 작업표에서 항목을 고정 해제할 항목 옆에 있습니다.

   >[!TIP]
   >
   >   작업표에서 항목을 클릭한 후 표준 QWERTY 키보드를 사용하는 경우 다음 키 집합을 눌러 항목을 고정 해제합니다.
   >   * Windows 및 Mac 컴퓨터 모두에 대한 옵션 + P.



   페이지를 새로 고친 후 작업표에서 항목이 제거됩니다.

1. (조건부) Workfront 또는 그룹 관리자가 **작업 역할을 시간 항목에 수동으로 할당** 을 설정하고 드롭다운 메뉴에서 작업 역할을 선택합니다. 작업 항목에 지정될 때 지정된 역할이 기본적으로 표시됩니다. 객체에 역할이 할당되지 않은 경우 기본 역할이 기본값으로 표시됩니다. 이 설정에 대한 자세한 내용은 문서를 참조하십시오 [작업표 및 시간 환경 설정 구성](../../administration-and-setup/set-up-workfront/configure-timesheets-schedules/timesheet-and-hour-preferences.md).

   ![작업표의 여러 역할에 대한 로그 시간](assets/job-role-plus-sign-and-boxes-in-redesigned-timesheet.png)


1. (선택 사항) **+** 아이콘을 사용하여 다른 행을 추가한 다음 [!UICONTROL 시간 유형] 열을 사용하여 다른 시간 유형에 대한 시간을 기록합니다.

   ![시간 유형 드롭다운 메뉴](assets/hour-type-drop-down-expanded-redesigned-timesheet.png)

   >[!TIP]
   >
   >   운영 체제나 브라우저에 따라 표준 QWERTY 키보드를 사용할 때 다음 키 세트를 눌러 다른 행을 추가합니다.
   >   * Windows 컴퓨터용 Ctrl + Option + +
   >   * Mac 컴퓨터용 Cmd + Option + + +


   시간 유형은 다음에 설명된 대로 시스템, 프로젝트 및 사용자 수준에서 정의된 내용에 따라 사용할 수 있습니다. [작업표의 시간 유형 및 가용성을 정의합니다.](define-hour-types-and-availability.md).

   작업표를 닫은 후에는 시간 형식을 변경할 수 없습니다.

   >[!TIP]
   >
   >이전에 기록된 시간과 선택한 시간 유형이 이제 비활성화된 경우, 로그된 시간 동안의 전체 행이 흐리게 표시됩니다. 다른 시간 유형을 선택하고 페이지를 새로 고치면 드롭다운 목록에서 비활성화된 시간 유형 옵션이 제거되므로 해당 시간 유형에 추가 시간을 추가할 수 없습니다.
   >
   >추가 시간을 기록하려는 작업 항목에 대해 새 라인을 추가하고, 비활성화 시간 유형을 과거 로그된 시간과 연관되게 유지하려면 새 시간 유형을 선택합니다.

1. 을(를) 클릭합니다. **delete** 아이콘  ![](assets/delete.png) 작업 역할 옆에 있는 작업을 제거합니다. 역할에 대해 기록된 모든 시간도 제거됩니다.

   >[!TIP]
   >
   >   운영 체제나 브라우저에 따라 표준 QWERTY 키보드를 사용할 때 다음 키 세트를 눌러 행을 삭제합니다.
   >   * Ctrl + Option + - Windows 컴퓨터용
   >   * Cmd + Option + - Mac 컴퓨터용



1. 작업표의 타임라인 섹션에 지정된 날짜에 로그온할 시간을 지정한 다음 시간 상자 외부를 클릭하여 시간 항목을 저장합니다. 시간이 자동으로 저장됩니다. 로그 시간이 기록되는 행은 연한 파란색으로 강조 표시되고 시간 입력 상자는 진한 파란색으로 윤곽이 표시됩니다.

   ![작업표의 로그 시간 상자](assets/log-time-with-blue-hightlight-redesigned-timesheet.png)

   몇 시간 또는 며칠 안에 로그인할 수 있습니다. 이 설정은 다음에 설명된 대로 Plan 라이센스를 가진 사용자 또는 시스템 관리자가 구성합니다 [시간 또는 일 단위로 로그인 여부 구성](../../timesheets/config-timesheet-prefs/config-time-logged-hrs-days.md).

   >[!IMPORTANT]
   >
   >로그된 시간에 대한 작업 역할이 변경된 경우 **작업 역할을 시간 항목에 수동으로 할당** 설정이 비활성화되었습니다. 시간 항목을 수동으로 저장해야 합니다. 작업표가 변경된 작업 역할에 대해 기록된 시간이 더 이상 없는 경우에만 시간이 자동으로 다시 저장됩니다.
   >
   >역할이 변경된 경우 **작업 역할을 시간 항목에 수동으로 할당** 설정이 활성화되면 시간을 기록하거나 역할을 업데이트할 수 있으며 변경 사항이 자동으로 저장됩니다.

1. (선택 사항) 작업표 헤더의 시간별 필드에서 초과 작업 시간을 지정합니다.

   >[!TIP]
   >
   >작업표의 현재 총 시간보다 더 많은 초과 근무 시간을 기록할 수 없습니다. 예를 들어 작업표에 7시간을 기록하면 8시간의 초과 근무를 기록할 수 없습니다.

1. (선택 사항) **댓글** 을 클릭하여 시간 항목에 대한 설명을 추가합니다.

   ![](assets/commment-button-on-hour-log-redesigned-timesheet.png)

   >[!TIP]
   >
   >   시간 입력 상자를 클릭한 후 표준 QWERTY 키보드를 사용할 때 다음 키 세트를 눌러 주석 상자를 엽니다.
   >   * Shift + F2(Windows 및 Mac 컴퓨터 모두).


1. 클릭 **완료** 을 눌러 설명을 저장합니다.

   >[!TIP]
   >
   >   표준 QWERTY 키보드를 사용할 때 주석 상자 내에서 다음 키 세트를 눌러 설명을 저장합니다.
   >   * Windows 컴퓨터의 경우 Ctrl + Enter를 누릅니다.
   >   * Mac 컴퓨터의 Cmd + 반환



1. (선택 사항) **댓글 표시** 도구 모음에서 작업 항목 아래에 시간 항목 설명을 표시할 수 있습니다.

   ![작업표의 항목 아래에 나열된 주석](assets/comments-expanded-under-tasks-redesigned-timesheet.png)

   >[!TIP]
   >
   >   작업표에 대한 모든 변경 내용은 자동으로 저장됩니다.

1. (선택 사항) 작업이나 문제의 행을 클릭한 다음 **요약 열기** 작업표 오른쪽 위 모서리에서 업데이트를 추가하거나 작업이나 문제에 대한 정보를 업데이트하는 데 사용됩니다. 요약 패널이 오른쪽에 열립니다.

   ![summary-panel-for-task-opened-in-timeset](assets/summary-panel-for-task-opened-in-timesheet-redesigned-timesheet.png)

   로그된 시간과 연관된 작업 항목의 업데이트 영역에 업데이트가 표시됩니다.

   >[!TIP]
   >
   >프로젝트 또는 일반 시간 시간 항목에 대해서는 주석을 달 수 없습니다.

1. 클릭 [!UICONTROL **요약 닫기**] 요약 패널을 닫고 작업표로 돌아가려면

1. (선택 사항) [!UICONTROL **업데이트**] 왼쪽 패널에서 작업표에 업데이트를 추가합니다. Workfront 업데이트에 대한 자세한 내용은 [작업 업데이트](../../workfront-basics/updating-work-items-and-viewing-updates/update-work.md).

   ![update-in-redesigned-timesheet-left-panel 입력](assets/enter-an-update-in-redesigned-timesheet-left-panel.png)

   * **닫기**: 업데이트 작업을 완료하면 작업표를 닫습니다. 이 옵션은 작업표가 승인자와 연결되어 있지 않은 경우에만 사용할 수 있습니다.

   * **승인을 위해 제출:** 이 옵션은 작업표에 승인자가 있는 경우에만 사용할 수 있습니다. 변경 사항을 저장하고 승인을 위해 제출합니다. 작업표를 닫은 후 **회수**: 승인이 아직 안 된 경우. 자세한 내용은 [승인을 위한 작업표 제출](../../timesheets/create-and-manage-timesheets/submit-timesheet-for-approval.md).

   * **거부**: 작업표 승인자이고 승인을 위해 작업표를 제출했을 때 이 옵션이 표시됩니다. 작업표의 상태가 거부됨으로 변경되고 작업표가 열려 있습니다.

   * **승인**: 작업표 승인자이고 승인을 위해 작업표를 제출했을 때 이 옵션이 표시됩니다. 작업표의 상태를 승인됨으로 변경하고 작업표를 닫습니다.
   >[!TIP]
   >
   >시스템 관리자이고 작업표가 승인자와 연결되어 있을 때 거부와 승인 옵션도 작업표에 표시됩니다.

1. (조건부) 승인을 위해 작업표를 닫거나 제출한 경우 다음 옵션 중 하나를 클릭합니다.

   * **다시 열기**: 이 옵션은 이미 닫혀 있고 승인자가 없는 작업시트나 이미 승인된 작업표에 사용할 수 있습니다. 시간 항목을 수정하려면 작업표를 다시 엽니다.
   * **회수**: 이 옵션은 승인을 위해 제출되었지만 아직 승인 또는 거부되지 않은 작업표에 사용할 수 있습니다. 클릭 **회수** 작업표를 다시 열고 시간 항목을 수정하려면 다음을 수행합니다.

### 홈 {#home}

홈에서 프로젝트별 시간을 기록할 수 있습니다.

홈 영역 사용에 대한 일반적인 정보는 [홈 영역 사용](../../workfront-basics/using-home/using-the-home-area/use-the-home-area.md).

홈 영역에서 작업 항목에 대한 시간을 기록하려면

1. 에서 **작업 목록** 영역에서 시간을 기록할 항목을 선택합니다.
1. 오른쪽 패널에서 **로그 시간**.

   ![](assets/log-time-home-350x181.png)

1. 에서 **시간 입력** 드롭다운 메뉴에서 해당 시간 유형을 선택합니다.\
   시간 유형은 다음에 설명된 대로 시스템, 프로젝트 및 사용자 수준에서 정의된 내용에 따라 사용할 수 있습니다. [작업표의 시간 유형 및 가용성을 정의합니다.](../../timesheets/create-and-manage-timesheets/define-hour-types-and-availability.md).
1. (조건부) Workfront 또는 그룹 관리자가 **작업 역할을 시간 항목에 수동으로 할당** 을 설정하고 드롭다운 메뉴에서 작업 역할을 선택합니다. 작업 항목에 지정될 때 지정된 역할이 기본적으로 표시됩니다. 객체에 역할이 할당되지 않은 경우 기본 역할이 기본값으로 표시됩니다. 이 설정에 대한 자세한 내용은 문서를 참조하십시오 [작업표 및 시간 환경 설정 구성](../../administration-and-setup/set-up-workfront/configure-timesheets-schedules/timesheet-and-hour-preferences.md).
1. 기록할 시간을 지정한 다음 **로그 시간**.

### 프로젝트, 작업 또는 문제 {#project-task-or-issue}

프로젝트, 작업 또는 문제에 프로젝트 특정 시간을 기록할 수 있습니다.

#### 로깅 시간에 필요한 권한

프로젝트, 작업 또는 문제에 대한 시간을 기록하려면 특정 권한이 있어야 합니다. 프로젝트, 작업 또는 문제에 대해 두 위치에서 시간을 로그인할 수 있습니다.

* [업데이트 탭](#updates-tab)
* [시간 탭](#hours-tab)

##### 업데이트 탭{#updates-tab}

프로젝트, 작업 또는 문제의 업데이트 탭에서 시간을 기록하려면 먼저 다음을 수행해야 합니다.

* 작업 또는 계획 라이센스가 있어야 합니다.
* 프로젝트, 작업 또는 로그 시간에 대한 액세스 권한에 대해 최소한 Contribute 권한이 있어야 합니다.\
   프로젝트에 대한 권한 부여에 대한 자세한 내용은 [Adobe Workfront에서 프로젝트 공유](../../workfront-basics/grant-and-request-access-to-objects/share-a-project.md).

* 프로젝트에 직접 시간을 기록하려는 경우 Workfront 관리자가 아래에 있는 프로젝트에서 직접 로그 시간 설정을 활성화해야 합니다 [!UICONTROL **작업표 및 시간** ]> [!UICONTROL **기본 설정**].\
   사용자가 프로젝트에 직접 시간을 로그할 수 있도록 하는 방법에 대한 자세한 내용은 [작업표 및 시간 환경 설정 구성](../../administration-and-setup/set-up-workfront/configure-timesheets-schedules/timesheet-and-hour-preferences.md).

##### 시간 탭{#hours-tab}

프로젝트, 작업 또는 문제의 시간 탭에서 시간을 기록하려면 먼저 다음을 수행해야 합니다.

* 시스템 관리자여야 합니다.

또는 다음을 모두 포함해야 합니다.

* 작업표 및 시간에 대한 관리 액세스 권한이 있는 계획 라이센스가 있어야 합니다. 작업표 및 시간에 대한 관리자 액세스 권한 부여에 대한 자세한 내용은 [특정 영역에 대한 관리자 액세스 권한 부여](../../administration-and-setup/add-users/configure-and-grant-access/grant-users-admin-access-certain-areas.md).
* 로그 시간에 액세스할 수 있는 프로젝트에 대한 Contribute 권한 이상이 있어야 합니다. 프로젝트에 대한 권한 부여에 대한 자세한 내용은 [Adobe Workfront에서 프로젝트 공유](../../workfront-basics/grant-and-request-access-to-objects/share-a-project.md).
* 프로젝트에 직접 시간을 기록하려면, Workfront 관리자가 작업표 및 시간 > 환경 설정에서 프로젝트 로그온 시간을 직접 활성화해야 합니다. 사용자가 프로젝트에 직접 시간을 로그할 수 있도록 하는 방법에 대한 자세한 내용은 [작업표 및 시간 환경 설정 구성](../../administration-and-setup/set-up-workfront/configure-timesheets-schedules/timesheet-and-hour-preferences.md).

프로젝트, 작업 또는 문제에 대한 시간을 기록하려면

1. 프로젝트, 작업 또는 문제로 이동합니다.
1. 왼쪽 패널에서 을 선택합니다 **시간**.
1. 클릭 **로그 시간**.

   로그 시간 대화 상자가 표시됩니다.

1. 다음 정보를 지정합니다.

   * **소유자:** 기본적으로 이 필드에 이름이 표시됩니다.\
      다른 사용자에 대해 시간을 기록하는 경우 해당 이름을 지정합니다.

   * **시간**: 프로젝트, 작업 또는 문제에 대한 시간(시)을 입력합니다.
   * **시간 유형**: 기본적으로 표시되는 시간과 다른 경우 드롭다운 메뉴에서 시간 유형을 선택합니다.

      시스템에서 구성된 시간 유형에 따라 여기에서 선택할 수 있는 옵션이 달라질 수 있습니다. 시간 유형 구성에 대한 자세한 내용은 [작업표의 시간 유형 및 가용성을 정의합니다.](../../timesheets/create-and-manage-timesheets/define-hour-types-and-availability.md).

   * **작업 역할**: (조건부) Workfront 또는 그룹 관리자가 **작업 역할을 시간 항목에 수동으로 할당** 설정, 선택 **작업 역할** 를 클릭합니다. 객체에 지정될 때 지정된 역할이 기본적으로 표시됩니다. 객체에 역할을 지정하지 않으면 기본 역할이 기본값으로 표시됩니다. 이 설정에 대한 자세한 내용은 문서를 참조하십시오 [작업표 및 시간 환경 설정 구성](../../administration-and-setup/set-up-workfront/configure-timesheets-schedules/timesheet-and-hour-preferences.md).

      ![Screen_Shot_2017-05-03_at_10.16.52_AM.png](assets/screen-shot-2017-05-03-at-10.16.52-am-350x346.png)

1. 클릭 **로그 시간**.

### 요약 패널

요약 패널에서 작업 및 문제에 대한 시간을 기록할 수 있습니다.
자세한 내용은 [요약 개요](../../workfront-basics/the-new-workfront-experience/summary-overview.md).

![](assets/summary-hour-log.png)

### 보드 {#boards}

>[!NOTE]
>
>이 기능은 Workfront 보드의 초기 기능 옵트인을 통해서만 사용할 수 있습니다.

Workfront 보드에 연결된 카드에 대해 로그인할 수 있습니다. 이는 작업 또는 문제에 대한 로깅 시간과 동일한 프로세스이며, 카드에 기록된 시간은 연결된 작업 또는 문제에 저장됩니다.
자세한 내용은 [보드에서 연결된 카드 사용](/help/quicksilver/agile/get-started-with-boards/connected-cards.md).

### 모바일 앱 {#mobile-app}

Workfront 모바일 앱에서 시간을 기록할 수 있습니다.
자세한 내용은 [Android용 Adobe Workfront](/help/quicksilver/workfront-basics/mobile-apps/using-the-workfront-mobile-app/workfront-for-android.md) 또는 [Adobe Workfront for iOS](/help/quicksilver/workfront-basics/mobile-apps/using-the-workfront-mobile-app/workfront-for-ios.md).
