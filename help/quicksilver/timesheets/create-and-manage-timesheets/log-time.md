---
product-area: timesheets
navigation-topic: create-and-manage-timesheets
title: 로그 시간
description: 작업 항목에 대한 시간을 Adobe Workfront(&n)에 기록하여 작업에 소비한 시간을 나타낼 수 있습니다. 휴가, 병가, 회의 등 업무와 관련 없는 시간도 기록할 수 있다. 기록한 시간이 타임시트에 표시됩니다.
author: Alina
feature: Timesheets
exl-id: 120173a8-95f1-4233-ab40-d3bcfe38c977
source-git-commit: 38a7329ebac4051439601ddd8ad2a89ee24c7971
workflow-type: tm+mt
source-wordcount: '3337'
ht-degree: 0%

---

# 로그 시간

<!--remove all preview and production references from this article with 23.3 release-->

<!--<span class="preview">The highlighted information on this page refers to functionality not yet generally available. It is available only in the Preview environment.</span>-->

Adobe Workfront에서 작업 항목에 대한 시간을 기록하여 작업에 소비한 시간을 나타낼 수 있습니다. 휴가, 병가, 회의 등 업무와 관련 없는 시간도 기록할 수 있다. 기록한 시간이 타임시트에 표시됩니다.

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

이 문서의 단계를 수행하고 프로젝트별 시간을 기록하려면 다음 액세스 권한이 있어야 합니다.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront 플랜*</td> 
   <td> <p>모든</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront 라이센스*</td> 
   <td> <ul><li>타임시트에 일반 시간을 기록하려면 이상을 검토하십시오.</li>
   <li> 프로젝트, 작업 또는 문제에 시간을 기록하려면 이상 작업</li></ul>
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader">액세스 수준 구성*</td> 
   <td> <p>시간을 기록한 작업 항목 유형에 대한 액세스 편집 </p> <p>예를 들어 문제에 대한 시간을 기록하려면 문제에 대한 편집 액세스 권한이 필요합니다</p> <p>여전히 액세스 권한이 없는 경우 Workfront 관리자에게 액세스 수준에 추가 제한을 설정하는지 문의하십시오. Workfront 관리자가 액세스 수준을 수정하는 방법에 대한 자세한 내용은 <a href="../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">사용자 정의 액세스 수준 만들기 또는 수정</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">개체 권한</td> 
   <td> <p>시간을 기록하는 작업 항목에 대한 기여 또는 더 높은 권한에는 시간 기록 권한이 포함됩니다.</p> <p>추가 액세스 요청에 대한 자세한 내용은 <a href="../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">오브젝트에 대한 액세스 요청 </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

*보유 중인 플랜, 라이선스 유형 또는 액세스 권한을 확인하려면 Workfront 관리자에게 문의하십시오.

## Workfront에서 시간 로깅 시 고려 사항

* 프로젝트, 작업 또는 문제에 시간을 기록하거나 타임시트에 직접 시간을 기록할 수 있습니다.

  타임시트 만들기에 대한 자세한 내용은 [일회용 타임시트 만들기](../../timesheets/create-and-manage-timesheets/create-tmshts.md).

* 타임시트 이외의 도구를 통해 기록된 모든 시간이 해당 기간의 타임시트에 표시됩니다.
* 현재 상태가 아닌 프로젝트의 작업 및 문제는 타임시트에 미리 채워지지 않습니다.
* 타임시트에 기록된 시간은 작업, 문제 또는 프로젝트에 즉시 적용됩니다.
* 타임시트에는 기록된 모든 날짜에 대한 총 시간이 포함됩니다. 에 설명된 대로 타임라인 계산이 주말을 제외하도록 구성된 경우에도 주말은 항상 포함됩니다 [시스템 전체 프로젝트 환경 설정 구성](../../administration-and-setup/set-up-workfront/configure-system-defaults/set-project-preferences.md)).
* 타임시트에 표시되는 최대 항목 수는 45개입니다. 일자가 타임시트 시간대와 일치하는 항목이 45개를 초과하는 경우 가장 최근에 업데이트된 항목만 표시됩니다.
* 청구된 청구 기록에 포함된 시간 항목은 흐리게 표시되어 타임시트에서 편집할 수 없습니다. 자세한 내용은 [청구 기록 만들기](../../manage-work/projects/project-finances/create-billing-records.md).

## 로그 시간

Workfront의 다음 영역에서 시간을 기록할 수 있습니다.

* [타임시트](#timesheet)
* [홈](#home)
* [프로젝트, 작업 또는 문제](#project-task-or-issue)
* [요약 패널](#summary-panel)
* [보드](#boards)
* [모바일 앱](#mobile-app)

### 타임시트 {#timesheet}


#### 타임시트에 시간 기록 {#log-time-on-a-timesheet}

타임시트에 일반 시간 또는 프로젝트별 시간을 기록할 수 있습니다.

>[!NOTE]
>
>타임시트 프로필에 할당된 검토 사용자에게 타임시트 영역이 표시되고 일반 시간이 기록됩니다. 하지만 타임시트에 표시되는 할당된 작업 또는 문제에 대해서는 시간을 기록할 수 없습니다.

1. 다음을 클릭합니다. [!UICONTROL **메인 메뉴**] 아이콘 ![](assets/main-menu-icon.png) Adobe Workfront 오른쪽 상단에 있습니다.

1. 클릭 [!UICONTROL **타임시트**]. 현재 타임시트가 기본적으로 표시됩니다.
   ![타임시트](assets/timesheet-redesigned-nwe.png)

   타임시트는 타임시트의 시간대 동안 사용자에게 할당된 항목으로 미리 채워집니다. 타임시트를 미리 채우는 방법에 대한 자세한 내용은 [타임시트 및 시간 환경 설정 구성](../../administration-and-setup/set-up-workfront/configure-timesheets-schedules/timesheet-and-hour-preferences.md). 타임시트에 항목이 표시되지 않으면 추가할 수 있습니다.

   >[!NOTE]
   >
   >타임시트는 사용자에게 할당된 항목으로만 미리 채워집니다. 팀이나 작업 역할에 할당된 항목으로 미리 채우지 않습니다.
   >
   >팀에 할당된 항목에 대한 처리 작업을 클릭하면 항목이 사용자에게 할당되고 해당 항목이 타임시트에 표시됩니다.


1. (선택 사항) **전체 화면** 아이콘 ![](assets/full-screen.png) 타임시트를 전체 화면 모드로 표시하려면 다음 아이콘을 클릭합니다. **전체 화면 종료** ![](assets/exit-full-screen.png) ( 타임시트로 돌아가는 아이콘)

   <!-- drafted for the resize columns in timesheet story: 1. (optional) Click on the separator lines between weeks or between the time frame area and the work item area to resize the columns of the timesheet.-->

1. (선택 사항) 타임시트에 프로젝트, 작업 또는 문제를 추가하려면 **항목 추가** 타임시트의 왼쪽 위 모서리에 있는 드롭다운 메뉴를 클릭한 다음 을(를) 클릭합니다. **프로젝트 추가**, **작업 추가**, 또는 **문제 추가**.

   프로젝트, 작업 또는 문제 목록이 표시됩니다.

   <!--drafted for full screen mode for add projects story - align it with the rest of the steps when you enable this:: 1. (Optional) Click the **full-screen** icon ![](assets/full-screen.png) to display the list of objects in full-screen mode.-->

1. (선택 사항) 검색 아이콘을 클릭합니다 ![항목 검색](assets/search-icon.png) 타임시트에 추가할 키워드를 사용하여 특정 항목을 검색합니다.

1. (선택 사항) 필터, 보기 또는 그룹화 드롭다운 메뉴를 확장하여 드롭다운 메뉴를 적용하거나 사용자 지정하고 원하는 항목 정보를 봅니다.

1. 목록에서 항목을 하나 이상 선택한 다음 **추가**.

   >[!NOTE]
   >
   >타임시트에 작업 또는 문제를 추가하면 프로젝트도 추가됩니다.


1. (조건부) 한 번에 50개 이상의 항목을 추가하는 경우 타임시트에 추가된 항목 수를 표시하는 확인 메시지가 표시됩니다.

   클릭 **모두 추가** 모든 항목을 추가하거나 **취소** 선택한 항목의 추가를 중지하려면 다음을 수행합니다 **취소** 을 클릭하여 항목 목록을 닫습니다.

   작업 및 문제는 프로젝트 이름 아래에 나열됩니다.

   >[!NOTE]
   >
   >타임시트에 수동으로 추가하는 항목은 고정되며 수동으로 고정 해제하여 제거할 때까지 현재 및 향후 타임시트에 유지됩니다. 항목을 고정 해제하여 타임시트에서 제거하는 방법에 대한 자세한 내용은 10단계를 계속하십시오.

   <!--(ensure this stays accurate)-->

1. (선택 사항) **접기** ![](assets/collapse-icon.png) 또는 **확장** ![](assets/expand-icon.png) 프로젝트의 작업 및 문제 목록을 표시하거나 숨길 수 있는 프로젝트 이름 옆에 있는 아이콘


   >[!TIP]
   >
   >   표준 QWERTY 키보드를 사용할 때 타임시트에서 프로젝트 이름을 클릭한 후 다음 키 세트를 눌러 프로젝트를 축소하거나 확장합니다.
   >   * 프로젝트를 확장하고 작업 항목을 표시하려면 다음을 수행합니다.
   >     * Windows 컴퓨터의 경우 Shift + Alt + 위쪽 화살표
   >     * Mac 컴퓨터의 Shift + Option + 위쪽 화살표
   >   * 프로젝트를 축소하고 작업 항목을 숨기려면 다음을 수행합니다.
   >     * Windows 컴퓨터의 경우 Shift + Alt + 아래쪽 화살표
   >     * Mac 컴퓨터의 Shift + Option + 아래쪽 화살표


1. (선택 사항) 타임시트에 표시되는 항목을 수동으로 고정하려면 항목의 이름을 마우스로 가리킨 다음, **핀** 아이콘 ![](assets/empty-pin-icon.png).

   >[!TIP]
   >
   >   타임시트에서 항목을 클릭한 후 표준 QWERTY 키보드를 사용할 때 다음 키 세트를 눌러 항목을 고정합니다.
   >   * Windows 및 Mac 컴퓨터 모두에 대해 Option + P입니다.


1. (선택 사항) 검색 아이콘을 클릭합니다 ![](assets/search-icon.png) 타임시트에서 프로젝트, 작업 또는 문제를 찾으려면 키워드를 입력하십시오.

1. (조건부) Workfront 또는 그룹 관리자가 **시간 항목에 수동으로 작업 역할 할당** 을 설정하고 드롭다운 메뉴에서 작업 역할을 선택합니다. 작업 항목에 할당할 때 지정된 역할이 기본적으로 표시됩니다. 오브젝트에 역할이 할당되지 않은 경우 기본 역할이 기본값으로 표시됩니다. 이 설정에 대한 자세한 내용은 문서를 참조하십시오 [타임시트 및 시간 환경 설정 구성](../../administration-and-setup/set-up-workfront/configure-timesheets-schedules/timesheet-and-hour-preferences.md).

   ![타임시트의 여러 역할에 대한 시간 기록](assets/job-role-plus-sign-and-boxes-in-redesigned-timesheet.png)


1. (선택 사항) **+** 아이콘 을 클릭하여 다른 행을 추가한 다음 의 드롭다운 메뉴에서 새 시간 유형을 선택합니다. [!UICONTROL 시간 유형] 열을 사용하여 다른 시간 유형에 시간을 기록합니다.

   ![시간 유형 드롭다운 메뉴](assets/hour-type-drop-down-expanded-redesigned-timesheet.png)

   >[!TIP]
   >
   >   운영 체제나 브라우저에 따라 표준 QWERTY 키보드를 사용할 때는 다음 키 세트를 눌러 다른 행을 추가합니다.
   >   * Windows 컴퓨터의 경우 Ctrl + Option + +
   >   * Mac 컴퓨터의 Cmd + Option + +

   에 설명된 대로 시스템, 프로젝트 및 사용자 수준에서 정의된 내용에 따라 시간 유형을 사용할 수 있습니다. [타임시트의 시간 유형 및 가용성 정의](define-hour-types-and-availability.md).

   타임시트가 종료된 후에는 시간 유형을 변경할 수 없습니다.

   >[!TIP]
   >
   >이전에 시간을 기록했으며 선택한 시간 유형이 현재 비활성화된 경우 기록된 시간에 대한 전체 행이 흐리게 표시됩니다. 다른 시간 유형을 선택하고 페이지를 새로 고치면 드롭다운 목록에서 비활성화된 시간 유형 옵션이 제거되므로 해당 시간 유형에 시간을 추가할 수 없습니다.
   >
   >에 대해 추가 시간을 기록할 작업 항목에 대해 새 라인을 추가하고, 비활성화된 시간 유형을 이전 기록된 시간과 연관시켜 유지하려면 새 시간 유형을 선택하는 것이 좋습니다.

1. 다음을 클릭합니다. **삭제** 아이콘  ![](assets/delete.png) 작업 역할 옆에 배치하여 제거합니다. 역할에 대해 기록된 시간도 모두 제거됩니다.

   >[!TIP]
   >
   >   운영 체제나 브라우저에 따라 표준 QWERTY 키보드를 사용할 때는 다음 키 세트를 눌러 행을 삭제합니다.
   >   * Windows 컴퓨터의 경우 Ctrl + Option + -
   >   * Cmd + Option + - Mac 컴퓨터


1. 타임시트의 타임라인 섹션에서 특정 날짜에 로그인할 시간을 지정한 다음 시간 상자 외부를 클릭하여 시간 항목을 저장합니다. 시간이 자동으로 저장됩니다. 시간을 기록하는 행은 연한 파란색으로 강조 표시되고 시간 항목 상자는 진한 파란색으로 윤곽이 표시됩니다.

   ![타임시트에 시간 상자 기록](assets/log-time-with-blue-hightlight-redesigned-timesheet.png)

   시간을 시간 또는 일 단위로 기록합니다. 이 설정은 다음에 설명된 대로 플랜 라이선스가 있는 사용자 또는 시스템 관리자가 구성합니다. [시간이 시간 단위로 기록되는지 또는 일 단위로 기록되는지 구성](../../timesheets/config-timesheet-prefs/config-time-logged-hrs-days.md).

   >[!IMPORTANT]
   >
   >다음 시나리오 중 하나가 발생하는 경우 타임시트를 수동으로 저장해야 합니다.
   >
   >* 이전에 기록한 시간과 연관된 작업 역할이 변경되었으며 **시간 항목에 수동으로 작업 역할 할당** 설정이 비활성화되었습니다. 새 날짜에 대한 로깅 시간은 다른 작업 역할과 연결됩니다.
   >   
   >   역할이 변경되고 **시간 항목에 수동으로 작업 역할 할당** 설정이 활성화되면 시간을 기록하거나 역할을 업데이트할 수 있으며 변경 사항이 자동으로 저장됩니다.
   >
   >* 작업 또는 문제에 할당된 작업 역할이 타임시트 소유자가 시간을 기록하는 작업 역할과 다릅니다. <!--or assigned to them_ this last  piece came from a Support note but but sure what role it's referring to. Leaving it out for now.-->.
   >
   >두 역할 간에 충돌하는 항목이 더 이상 없을 때 타임시트가 다시 시간을 자동으로 절약합니다.
   >

1. (선택 사항) 타임시트 헤더의 초과 근무 필드에 초과 근무 금액을 지정합니다.

   >[!TIP]
   >
   >타임시트에 현재 총 시간보다 많은 수의 초과 근무 시간을 기록할 수 없습니다. 예를 들어 지금까지 타임시트에 7시간을 기록한 경우 8시간의 초과 근무를 기록할 수 없습니다.

1. (선택 사항) **댓글** 시간 항목에 대한 댓글을 추가합니다.

   ![](assets/commment-button-on-hour-log-redesigned-timesheet.png)

   >[!TIP]
   >
   >   시간 입력 상자를 클릭한 후 표준 QWERTY 키보드를 사용할 때 다음 키 세트를 눌러 주석 상자를 엽니다.
   >   * Windows 및 Mac 컴퓨터 모두에 대해 Shift + F2를 누릅니다.

1. 클릭 **완료** 주석을 저장합니다.

   >[!TIP]
   >
   >   표준 QWERTY 키보드를 사용할 때 주석 상자 내에서 다음 키 세트를 눌러 주석을 저장합니다.
   >   * Windows 컴퓨터의 경우 Ctrl + Enter를 누릅니다.
   >   * Cmd + Mac 컴퓨터용 Return


1. (선택 사항) **댓글 표시** 을 클릭하여 작업 항목 아래에 시간 입력 설명을 표시합니다.

   ![타임시트의 항목 아래에 나열된 주석](assets/comments-expanded-under-tasks-redesigned-timesheet.png)

   >[!TIP]
   >
   >   타임시트에 대한 모든 변경 내용은 자동으로 저장됩니다.

1. (선택 사항) 작업 또는 문제의 행을 클릭한 다음 **요약 열기** 타임시트의 오른쪽 상단 모서리에서 업데이트를 추가하거나 작업 또는 문제에 대한 정보를 업데이트합니다. 오른쪽에 요약 패널이 열립니다.

   ![task-opened-in-timesheet에 대한 요약 패널](assets/summary-panel-for-task-opened-in-timesheet-redesigned-timesheet.png)

   기록된 시간과 연관된 작업 항목의 업데이트 영역에 업데이트가 표시됩니다.

   >[!TIP]
   >
   >프로젝트 또는 일반 시간 항목에 대해 댓글을 달 수 없습니다.

1. 클릭 [!UICONTROL **요약 닫기**] 요약 패널을 닫고 타임시트로 돌아갑니다.

1. (선택 사항) [!UICONTROL **업데이트**] 왼쪽 패널에서 업데이트를 타임시트에 추가합니다. Workfront 업데이트에 대한 자세한 내용은 [작업 업데이트](../../workfront-basics/updating-work-items-and-viewing-updates/update-work.md).

   ![재설계된 타임시트 왼쪽 패널 업데이트](assets/enter-an-update-in-redesigned-timesheet-left-panel.png)

   * **닫기**: 타임시트 업데이트를 마치면 타임시트를 닫습니다. 이 옵션은 타임시트가 승인자와 연결되어 있지 않은 경우에만 사용할 수 있습니다.

   * **승인을 위한 제출:** 이 옵션은 타임시트에 승인자가 있는 경우에만 사용할 수 있습니다. 변경 사항을 저장하고 승인을 위해 제출합니다. 타임시트를 닫은 후 다음을 클릭하여 열 수 있습니다. **회수**, 승인이 아직 부여되지 않은 경우. 자세한 내용은 [승인을 위해 타임시트 제출](../../timesheets/create-and-manage-timesheets/submit-timesheet-for-approval.md).

   * **거부**: 이 옵션은 타임시트 승인자이고 타임시트가 승인을 위해 제출되었을 때 표시됩니다. 타임시트의 상태가 거부됨으로 변경되고 타임시트는 열린 상태로 유지됩니다.

   * **승인**: 이 옵션은 타임시트 승인자이고 타임시트가 승인을 위해 제출되었을 때 표시됩니다. 타임시트의 상태를 승인됨으로 변경하고 타임시트를 닫습니다.

   >[!TIP]
   >
   >시스템 관리자이고 타임시트가 승인자와 연결된 경우 거부 및 승인 옵션도 타임시트에 표시됩니다.

1. (조건부) 승인을 위해 타임시트를 닫거나 제출한 경우 다음 옵션 중 하나를 클릭합니다.

   * **다시 열기**: 이 옵션은 이미 닫았으며 승인자가 없는 타임시트 또는 이미 승인된 타임시트에 사용할 수 있습니다. 시간 항목을 수정하려면 타임시트를 다시 엽니다.
   * **회수**: 이 옵션은 승인을 위해 제출되었지만 아직 승인 또는 거부되지 않은 타임시트에 사용할 수 있습니다. 클릭 **회수** 타임시트를 다시 열고 시간 항목을 수정합니다.

#### 타임시트에서 항목 제거

타임시트에서 시간 항목 또는 항목(프로젝트, 작업 또는 문제)을 제거할 수 있습니다.

타임시트에서 시간 항목을 제거하려면 다음 작업을 수행하십시오.

1. 타임시트로 이동하여 제거할 시간 항목을 찾습니다.
1. 입력한 시간을 0으로 바꾸거나 시간을 제거하고 0으로 바꾼 다음 Enter 키를 누릅니다.

   시간이 제거되고 타임시트가 자동으로 저장됩니다.

아직 시간 기록이 없고 의 4-8단계에 설명된 대로 항목을 수동으로 추가한 경우 타임시트를 고정 해제하여 항목(프로젝트, 작업 또는 문제)을 타임시트에서 제거할 수 있습니다. [타임시트에 시간 기록](#log-time-on-a-timesheet) 섹션 참조). <!--ensure this stays accurate-->

타임시트를 미리 채우도록 구성된(에 설명된 대로) Workfront 시스템 또는 그룹의 타임시트 환경 설정에 따라 타임시트에 포함된 항목을 자동으로 제거할 수 없습니다 [타임시트 및 시간 환경 설정 구성](../../administration-and-setup/set-up-workfront/configure-timesheets-schedules/timesheet-and-hour-preferences.md)). 항목의 날짜가 타임시트의 시간 범위를 벗어나는 경우 항목 미리 채우기가 중지됩니다.

수동으로 추가된 타임시트에서 항목을 제거하려면 다음 작업을 수행하십시오.

1. 항목에 대해 기록된 시간이 없는지 확인합니다.
1. 다음을 클릭합니다. **고정 해제** 아이콘 ![항목 고정](assets/pin-icon.png) 타임시트에서 항목을 고정 해제할 항목 옆에 있습니다.

   >[!TIP]
   >
   >   타임시트에서 항목을 클릭한 후 표준 QWERTY 키보드를 사용할 때 다음 키 세트를 눌러 항목을 고정 해제합니다.
   > * Windows 및 Mac 컴퓨터 모두에 대해 Option + P입니다.

   이 항목은 페이지를 새로 고친 후 타임시트에서 제거됩니다.

### 홈 {#home}

홈에서 프로젝트별 시간을 기록할 수 있습니다.

홈 영역 사용에 대한 일반 정보는 다음을 참조하십시오. [홈 영역 사용](../../workfront-basics/using-home/using-the-home-area/use-the-home-area.md).

홈 영역에서 작업 항목에 시간을 기록하려면 다음을 수행합니다.

1. 다음에서 **작업 목록** 영역에서 시간을 기록할 항목을 선택합니다.
1. 오른쪽 패널에서 를 클릭합니다. **로그 시간**.

   ![](assets/log-time-home-350x181.png)

1. 다음에서 **시간 입력** 드롭다운 메뉴에서 적절한 시간 유형을 선택합니다.\
   에 설명된 대로 시스템, 프로젝트 및 사용자 수준에서 정의된 내용에 따라 시간 유형을 사용할 수 있습니다. [타임시트의 시간 유형 및 가용성 정의](../../timesheets/create-and-manage-timesheets/define-hour-types-and-availability.md).
1. (조건부) Workfront 또는 그룹 관리자가 **시간 항목에 수동으로 작업 역할 할당** 을 설정하고 드롭다운 메뉴에서 작업 역할을 선택합니다. 작업 항목에 할당할 때 지정된 역할이 기본적으로 표시됩니다. 오브젝트에 역할이 할당되지 않은 경우 기본 역할이 기본값으로 표시됩니다. 이 설정에 대한 자세한 내용은 문서를 참조하십시오 [타임시트 및 시간 환경 설정 구성](../../administration-and-setup/set-up-workfront/configure-timesheets-schedules/timesheet-and-hour-preferences.md).
1. 기록할 시간을 지정한 다음 **로그 시간**.

### 프로젝트, 작업 또는 문제 {#project-task-or-issue}

다음 섹션에서 프로젝트, 작업 또는 문제에 대한 프로젝트별 시간을 기록할 수 있습니다.

* [업데이트 섹션](#updates-section)
* [시간 섹션](#hours-section)

#### 업데이트 섹션{#updates-section}

<!--remove the note below when the -->

>[!NOTE]
>
> 현재 업데이트 섹션과 새 업데이트 섹션 사이에는 사용자 인터페이스의 모양과 느낌에 약간의 차이가 있습니다. 이 섹션의 정보는 새 댓글 달기 경험에 표시되는 기능을 참조합니다.
>
>새 업데이트 섹션에 대한 자세한 내용은 [새 댓글 달기 환경](../../product-announcements/betas/new-commenting-experience-beta/unified-commenting-experience.md).

프로젝트, 작업 또는 문제의 업데이트 섹션에 시간을 기록하려면 다음 항목이 있어야 합니다.

* 작업 또는 플랜 라이선스.
* 로그 시간에 대한 액세스 권한으로 프로젝트, 작업 또는 문제에 기여하거나 더 높은 권한을 부여합니다.\
  프로젝트에 대한 권한 부여에 대한 자세한 내용은 [Adobe Workfront에서 프로젝트 공유](../../workfront-basics/grant-and-request-access-to-objects/share-a-project.md).

* Workfront 관리자는 다음에서 프로젝트에 직접 시간 기록 설정을 활성화해야 합니다. [!UICONTROL **타임시트 및 시간**]> [!UICONTROL **환경 설정**]&#x200B;프로젝트에 직접 시간을 기록하려는 경우.

  사용자가 시간을 프로젝트에 직접 기록할 수 있도록 허용하는 방법에 대한 자세한 내용은 [타임시트 및 시간 환경 설정 구성](../../administration-and-setup/set-up-workfront/configure-timesheets-schedules/timesheet-and-hour-preferences.md).

프로젝트, 작업 또는 문제의 업데이트 섹션에 시간을 기록하려면 다음 작업을 수행하십시오.

1. 프로젝트, 작업 또는 문제로 이동합니다.
1. 왼쪽 패널에서 을 선택합니다 **업데이트**.
1. 클릭 **로그 시간**. <!-- did Anna B change the casing for this button? If yes and if she changed it for the other areas, update screen shot too-->

   로그 시간 대화 상자가 표시됩니다.

   >[!TIP]
   >
   >   프로필의 기본 설정을 일 단위로 기록하도록 설정하면 일 입력 상자가 표시됩니다.
   >   
   >   일 입력 상자의 오른쪽 상단 모서리에는 하루에 몇 시간이 포함되는지 표시됩니다.

   ![](assets/log-time-box-in-updates-stream.png)

1. 다음 정보를 지정합니다.

   * **시간 유형**: 기본적으로 표시되는 시간 유형과 다른 경우 드롭다운 메뉴에서 시간 유형을 선택합니다.

     시스템에 구성된 시간 유형에 따라 여기 옵션이 다를 수 있습니다. 시간 유형 구성에 대한 자세한 내용은 [타임시트의 시간 유형 및 가용성 정의](../../timesheets/create-and-manage-timesheets/define-hour-types-and-availability.md).

   * **작업 역할**: (조건부) Workfront 또는 그룹 관리자가 **시간 항목에 수동으로 작업 역할 할당** 설정, 선택 **작업 역할** 드롭다운 메뉴에서 을(를) 선택합니다. 객체에 지정될 때 지정된 역할이 기본적으로 표시됩니다. 오브젝트에 역할이 할당되지 않은 경우 기본 역할이 기본값으로 표시됩니다. 이 설정에 대한 자세한 내용은 문서를 참조하십시오 [타임시트 및 시간 환경 설정 구성](../../administration-and-setup/set-up-workfront/configure-timesheets-schedules/timesheet-and-hour-preferences.md).

   * **시간**: 프로젝트, 작업 또는 문제의 시간 수를 입력합니다.

1. 클릭 **로그 시간**.

#### 시간 섹션{#hours-section}

시간 섹션에 프로젝트, 작업 및 문제에 대한 시간을 기록하려면 Workfront 관리자여야 합니다.

또는

다음 항목이 모두 있어야 합니다.

* 타임시트 및 시간에 대한 관리 액세스 권한이 있는 플랜 라이선스. 타임시트 및 시간에 대한 관리 액세스 권한을 부여하는 방법에 대한 자세한 내용은 다음을 참조하십시오. [사용자에게 특정 영역에 대한 관리 액세스 권한 부여](../../administration-and-setup/add-users/configure-and-grant-access/grant-users-admin-access-certain-areas.md).
* 로그 시간에 액세스할 수 있는 프로젝트에 대한 또는 더 높은 권한을 제공하십시오. 프로젝트에 대한 권한 부여에 대한 자세한 내용은 [Adobe Workfront에서 프로젝트 공유](../../workfront-basics/grant-and-request-access-to-objects/share-a-project.md).
* 프로젝트에 직접 시간을 기록하려면 Workfront 관리자가 타임시트 및 시간 > 환경 설정에서 프로젝트에 직접 시간 기록 설정을 활성화해야 합니다. 사용자가 시간을 프로젝트에 직접 기록할 수 있도록 허용하는 방법에 대한 자세한 내용은 [타임시트 및 시간 환경 설정 구성](../../administration-and-setup/set-up-workfront/configure-timesheets-schedules/timesheet-and-hour-preferences.md).

프로젝트, 작업 또는 문제의 시간 섹션에 시간을 기록하려면 다음을 수행하십시오.

1. 프로젝트, 작업 또는 문제로 이동합니다.
1. 왼쪽 패널에서 **시간**.
1. 클릭 **로그 시간**.

   로그 시간 대화 상자가 표시됩니다.

1. 다음 정보를 지정합니다.

   * **소유자:** 기본적으로 이름이 이 필드에 표시됩니다.\
     다른 사용자의 시간을 기록하는 경우 해당 이름을 지정합니다.

   * **시간**: 프로젝트, 작업 또는 문제의 시간 수를 입력합니다.
   * **시간 유형**: 기본적으로 표시되는 시간 유형과 다른 경우 드롭다운 메뉴에서 시간 유형을 선택합니다.

     시스템에 구성된 시간 유형에 따라 여기 옵션이 다를 수 있습니다. 시간 유형 구성에 대한 자세한 내용은 [타임시트의 시간 유형 및 가용성 정의](../../timesheets/create-and-manage-timesheets/define-hour-types-and-availability.md).

   * **작업 역할**: (조건부) Workfront 또는 그룹 관리자가 **시간 항목에 수동으로 작업 역할 할당** 설정, 선택 **작업 역할** 드롭다운 메뉴에서 을(를) 선택합니다. 객체에 지정될 때 지정된 역할이 기본적으로 표시됩니다. 오브젝트에 역할이 할당되지 않은 경우 기본 역할이 기본값으로 표시됩니다. 이 설정에 대한 자세한 내용은 문서를 참조하십시오 [타임시트 및 시간 환경 설정 구성](../../administration-and-setup/set-up-workfront/configure-timesheets-schedules/timesheet-and-hour-preferences.md).

     ![Screen_Shot_2017-05-03_at_10.16.52_AM.png](assets/screen-shot-2017-05-03-at-10.16.52-am-350x346.png)

1. 클릭 **시간 기록**.

### 요약 패널

요약 패널에서 작업 및 문제에 대한 시간을 기록할 수 있습니다.
자세한 내용은 [요약 개요](../../workfront-basics/the-new-workfront-experience/summary-overview.md).

![](assets/summary-hour-log.png)

### 보드 {#boards}

Workfront 보드의 연결된 카드에 시간을 기록할 수 있습니다. 이 프로세스는 작업 또는 문제에 시간을 기록하는 프로세스와 동일하며, 카드에 기록된 시간은 연결된 작업 또는 문제에 저장됩니다.
자세한 내용은 [보드에서 연결된 카드 사용](/help/quicksilver/agile/get-started-with-boards/connected-cards.md).

### 모바일 앱 {#mobile-app}

Workfront 모바일 앱에서 시간을 기록할 수 있습니다.
자세한 내용은 [Android용 Adobe Workfront](/help/quicksilver/workfront-basics/mobile-apps/using-the-workfront-mobile-app/workfront-for-android.md) 또는 [iOS용 Adobe Workfront](/help/quicksilver/workfront-basics/mobile-apps/using-the-workfront-mobile-app/workfront-for-ios.md).
