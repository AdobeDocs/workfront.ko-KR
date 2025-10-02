---
product-area: timesheets;system-administration
navigation-topic: create-and-manage-timesheets
title: 타임시트 프로필 만들기, 편집 및 할당
description: 사용자의 추가 개입 없이 사용자에 대해 반복 타임시트를 생성하는 타임시트 프로필을 만들고, 편집하고, 할당할 수 있습니다. 이렇게 하면 시간이 절약되고 사용자 간의 일관성이 보장됩니다.
author: Lisa
feature: Timesheets
exl-id: 8f4826bd-82b4-4157-a7d4-a7c94b8fc879
source-git-commit: 611c3c947855610cf86cdcbf96d1e9d847e34f38
workflow-type: tm+mt
source-wordcount: '1668'
ht-degree: 2%

---

# 타임시트 프로필 만들기, 편집 및 할당

<!--Audited: 06/2025-->

<span class="preview">이 페이지에서 강조 표시된 정보는 아직 일반적으로 사용할 수 없는 기능을 참조합니다. 미리 보기 샌드박스 환경에서만 사용할 수 있으며 프로덕션에 단계적으로 롤아웃할 때 릴리스됩니다.</span>

사용자의 추가 개입 없이 사용자에 대해 반복 타임시트를 생성하는 타임시트 프로필을 만들고, 편집하고, 할당할 수 있습니다. 이렇게 하면 시간이 절약되고 사용자 간에 다음 사항이 일관되도록 할 수 있습니다.

* 타임시트 시간대
* 승인자
* 일반 시간 유형

타임시트를 수동으로 만드는 방법에 대한 자세한 내용은 [일회용 타임시트 만들기](../../timesheets/create-and-manage-timesheets/create-tmshts.md)를 참조하십시오.

## 액세스 요구 사항

+++ 을 확장하여 이 문서의 기능에 대한 액세스 요구 사항을 봅니다.

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
   <td> <p>새로운 기능: 표준 </p>
 <p>또는</p> 
<p>현재: 플랜 </p> 
</td> 
  </tr> 
  <tr> 
   <td role="rowheader">액세스 수준 구성</td> 
   <td> <p>타임시트에 대한 관리 액세스 권한이 있어야 합니다. </p> </td> 
  </tr> 
 </tbody> 
</table>

*이 표의 정보에 대한 자세한 내용은 [Workfront 설명서의 액세스 요구 사항](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)을 참조하십시오.

+++

## 타임시트 프로필 만들기 또는 편집

<!--Old info: 
<div style="color: #ff1493;" data-mc-conditions="QuicksilverOrClassic.Draft mode">
<p style="color: #ff1493;">Alina drafted an Important note under this heading because Tracy/WorkEx said this is not working as designed - the changes WILL take effect the minute to make them for existing timesheets - see this issue - https://hub.workfront.com/issue/5dba59f600c401cca536567c368aa299/overview</p>
<p style="color: #ff1493;">Important: The changes you make to an existing timesheet profile are not automatically applied to timesheets that have already been generated. The changes you make to a timesheet prile are applied only to the timesheets that are&nbsp;generated after the timesheet profiles changes are made. To&nbsp;apply your&nbsp;changes to the timesheet profile for the timesheets that are already generated, you must delete the existing timesheets and manually generate&nbsp;them.For more information about deleting and manually generating timesheets, see&nbsp;Delete and manually generating Timesheets.</p>
</div>
-->

>[!IMPORTANT]
>
>현재 타임시트에서 타임시트 프로필 변경 사항을 활성화하려면 타임시트 프로필을 변경하기 전에 기존 타임시트를 삭제한 다음 새 타임시트를 생성해야 합니다. 지침은 [Adobe Workfront에서 타임시트 삭제](../../timesheets/create-and-manage-timesheets/delete-timesheets.md) 및 [타임시트 수동으로 생성](../../timesheets/create-and-manage-timesheets/manually-generate-timesheets.md)을 참조하십시오.

{{step-1-to-setup}}

1. 시스템 전체에서 사용할 타임시트 프로필을 만들거나 편집하는 경우 **타임시트 및 시간**&#x200B;을 클릭합니다.

   또는

   그룹에 대한 타임시트 프로필을 만들거나 편집하는 경우 **그룹**&#x200B;을 클릭한 다음 그룹 이름을 클릭합니다.

1. **타임시트 프로필**&#x200B;을 클릭합니다.
1. 타임시트 프로필을 만들려면 **새 프로필**&#x200B;을 클릭하세요.

   또는

   기존 타임시트 프로필을 편집하려면 편집할 타임시트 프로필을 선택한 다음 **편집**&#x200B;을 클릭합니다.

   새 또는 기존 타임시트 프로필 페이지가 표시됩니다.

1. 다음 정보를 업데이트합니다.

   * **이름**: 타임시트 프로필의 이름을 추가합니다. 직원들이 타임시트에 대해 동일한 시간대를 공유하는 팀 또는 그룹의 이름일 수 있습니다. 필수 필드입니다.
   * **설명**: 타임시트 프로필에 대한 정보를 더 추가합니다.
   * **관리 액세스 권한이 있는 그룹**: 시스템 수준 타임시트 프로필을 만드는 경우 이 필드를 비워 두십시오.

     사용자 계정을 편집할 수 있는 모든 사용자는 시스템 수준 타임시트를 다른 사용자에게 첨부할 수 있습니다.

     Workfront 관리자만 시스템 수준 타임시트 프로필을 편집할 수 있습니다.

     관리하는 그룹에 대한 타임시트 프로필을 만드는 경우 여기에서 그룹을 식별하십시오.

     이렇게 하면 그룹의 사용자에게 타임시트 프로필이 할당되지 않고 그룹의 관리자만 타임시트 프로필을 수정할 수 있습니다. 6단계에서 사용자에게 프로필을 할당합니다.

     >[!NOTE]
     >
     >그룹 외부의 사용자가 다른 사용자에게 타임시트 프로필을 첨부할 때 이 타임시트 프로필을 보거나 첨부할 수 없습니다.

   * **타임시트 만들기**: 타임시트 프로필에서 타임시트를 생성할 시기를 지정합니다. 타임시트는 주별, 격주, 반월별 또는 월별 기준으로 자동 생성되도록 설정할 수 있습니다. 타임시트를 만들려는 요일을 선택합니다.

     주별 타임시트는 생성된 날짜부터 시작됩니다. 예를 들어 매주 목요일에 주간 타임시트를 만드는 경우 타임시트의 첫 번째 날은 목요일입니다.

     >[!NOTE]
     >
     >Workfront은 항상 한 번에 두 개의 타임시트를 만듭니다. 첫 번째 타임시트에는 항상 현재 날짜가 포함되며, 두 번째 타임시트는 첫 번째 타임시트의 일정이 끝날 때 시작됩니다.

   * **승인자**: 승인자는 타임시트에 연결된 사용자의 타임시트를 승인하는 사용자입니다. 타임시트에서 승인자로 최대 7명의 사용자를 식별할 수 있습니다. 여러 사용자를 식별하면 누군가가 부재 중일 때 승인자가 사용 가능한지 확인하는 데 유용합니다. 사용자가 승인을 위해 타임시트를 제출하면 모든 승인자에게 알림이 전송됩니다. 타임시트를 승인하려면 한 명의 사용자만 타임시트를 승인해야 합니다.

     타임시트 관리 권한이 있는 사용자만 승인자로 설정할 수 있습니다. 타임시트 관리 권한에 대한 자세한 내용은 [특정 영역에 대한 관리자 액세스 권한 부여](/help/quicksilver/administration-and-setup/add-users/configure-and-grant-access/grant-users-admin-access-certain-areas.md)를 참조하십시오.

     드롭다운 메뉴를 사용하여 타임시트에 대한 승인자를 선택합니다(승인자가 필요한 경우). 다음 옵션 중에서 선택할 수 있습니다.

      * **없음**: 타임시트를 승인할 필요가 없습니다.
      * **관리자**: 시스템이 설정한 기본 승인자입니다. 이 경우 관리자로 지정된 사용자가 승인을 위해 제출한 타임시트를 승인합니다.
      * **특정 직원**: 이름으로 특정 사용자를 타임시트 승인자로 지정할 수 있습니다. 타임시트에 여러 승인자가 있을 수 있습니다. 이 경우 승인자 중 한 명이 타임시트를 승인하면 타임시트가 **마감됨**(으)로 표시되고 나머지 모든 승인자의 타임시트 승인 목록에서 사라집니다.

   * **시간을 편집할 수 있음**: 승인자가 타임시트의 시간을 편집할 수 있도록 하려면 이 옵션을 선택하십시오.

     이 옵션은 설정 > 타임시트 및 시간 > 환경 설정 영역에서 **타임시트 편집을 소유자 및 관리자로 제한** 설정과 함께 작동합니다. 자세한 내용은 [타임시트 및 시간 환경 설정 구성](/help/quicksilver/administration-and-setup/set-up-workfront/configure-timesheets-schedules/timesheet-and-hour-preferences.md)을 참조하십시오.

     다음과 같은 시나리오가 있습니다.

     **타임시트 편집을 소유자 및 관리자로 제한** 옵션이 활성화된 경우:

      * 승인자는 시간 편집 가능 의 활성화 여부에 관계없이 타임시트만 승인하고 거부할 수 있습니다.
      * 타임시트 소유자의 관리자는 부하 직원의 타임시트만 볼 수 있습니다.

     **타임시트 편집을 소유자 및 관리자로 제한** 옵션이 비활성화된 경우:

      * **시간을 편집할 수 있음**&#x200B;이 활성화되면 승인자는 타임시트를 제출하거나 다시 열거나 닫을 수 있고 시간을 편집할 수 있습니다.
      * **시간을 편집할 수 있음**&#x200B;이 비활성화되면 승인자는 타임시트를 제출하거나 다시 열거나 닫을 수 없으며 시간을 편집할 수 없습니다. 승인자는 타임시트만 승인하거나 거부할 수 있습니다.
      * 타임시트 소유자의 관리자는 부하 직원의 타임시트를 제출, 회수, 다시 열고 편집할 수 있습니다.

     >[!NOTE]
     >
     >승인을 위해 타임시트를 제출하면 더 이상 시간을 편집할 수 없습니다. 제출된 타임시트를 편집 가능한 상태로 되돌리려면 타임시트를 불러오거나 승인자가 타임시트를 거부하도록 하십시오. 자세한 내용은 [승인을 위한 타임시트 제출](/help/quicksilver/timesheets/create-and-manage-timesheets/submit-timesheet-for-approval.md) 및 [타임시트 승인](/help/quicksilver/timesheets/create-and-manage-timesheets/timesheet-approvals.md)을 참조하세요.

   * **초과 작업 시간**: 타임시트에서 초과 작업 시간 상자를 숨기도록 선택할 수 있습니다. 이 옵션은 기본적으로 비활성화되어 있습니다.
   * **사용 가능한 시간 유형**: 이 설정은 일반 시간 유형만 참조하며 프로젝트별 시간 유형은 참조하지 않습니다.

     기본적으로 사용자는 타임시트에 모든 일반 시간을 볼 수 있습니다. 그러나 조직에서 특정 사용자 집합에 대해 특정 일반 시간만 표시하기를 원하는 경우 이 필드의 타임시트 프로필에서 일반 시간을 선택하여 타임시트에 표시해야 하는 일반 시간을 선택할 수 있습니다. 모든 일반 시간을 비활성화하려면 모든 시간 유형을 선택 해제하여 일반 시간에 대한 섹션 없이 타임시트를 생성합니다.

   * **미리 알림**: 미리 알림을 추가합니다. Workfront은 사용자에게 타임시트를 완료하거나 승인하도록 요청하는 미리 알림을 보냅니다. 미리 알림을 타임시트 프로필과 연결하려면 먼저 미리 알림을 만들어야 합니다.

1. 프로덕션에서 그룹 수준 타임시트 프로필을 만들 때 **사람 할당** 탭을 클릭하여 타임시트 프로필을 특정 사용자, 그룹 또는 (Workfront 관리자인 경우) 팀과 연결합니다. <!--To associate the timesheet profile with specific users, groups, or (if you are a Workfront administrator) teams, scroll towards the bottom of the page and find the **Assign People** section.-->

   <span class="preview">미리 보기에서 그룹 수준 타임시트 프로필을 만들 때 페이지 아래쪽으로 스크롤하여 **사람 할당** 섹션을 찾습니다.</span>

   시스템에 대한 타임시트 프로필을 만들 때 페이지 아래쪽으로 스크롤하여 **사람 할당** 섹션을 찾습니다.

   사용자, 그룹 또는 팀의 이름을 입력한 다음 드롭다운 목록에 나타나면 클릭합니다.

   그룹 관리자인 경우 관리하는 그룹에 타임시트 프로필을 할당할 수 있지만 팀에는 할당할 수 없습니다. 자세한 내용은 이 문서에서 [그룹 관리자가 타임시트 프로필을 할당하는 제한](#limitations-for-a-group-administrator-assigning-a-timesheet-profile)을 참조하십시오.

   >[!NOTE]
   >
   >* 사용자 프로필을 편집하여 사용자를 타임시트 프로필과 연결할 수도 있습니다. 자세한 내용은 [사용자 프로필 편집](../../administration-and-setup/add-users/create-and-manage-users/edit-a-users-profile.md)을 참조하세요.
   >* 그룹을 추가하면 사용자 할당 탭에 그룹 이름만 표시되고 그룹 구성원 목록은 표시되지 않습니다. 여기에 나열된 그룹 구성원을 보려면 변경 사항 저장을 클릭한 다음 방금 만든 타임시트 프로필의 이름을 클릭합니다.
   >* 이 단계를 완료하면 타임시트 프로필은 현재 기간에 대한 타임시트가 없는 할당된 사용자 또는 그룹 멤버에 대해서만 타임시트를 생성합니다.

1. **저장**&#x200B;을 클릭합니다.

1. 타임시트 프로필 목록의 맨 위에서 **자세히** 아이콘 ![자세히 아이콘](assets/more-icon.png)을 클릭한 다음 **타임시트 생성**&#x200B;을 클릭합니다.

   타임시트가 성공적으로 생성되었다는 확인 메시지가 화면 맨 아래에 표시됩니다. 새 타임시트는 사용자가 만든 새 프로필을 기반으로 생성됩니다.

   자세한 내용은 [수동으로 타임시트 생성](/help/quicksilver/timesheets/create-and-manage-timesheets/manually-generate-timesheets.md)을 참조하십시오.

   타임시트 프로필에서 타임시트를 처음 생성할 때 현재 시간을 포함하는 시간대와 다음 시간대에 대해 각 사용자에 대해 두 개의 타임시트가 만들어집니다.

   이후 새 타임시트를 생성할 때마다 사용자당 하나의 타임시트가 생성됩니다.

   <!--the content in the table above will need to match the content in the Create timesheets article-->

## 타임시트 프로필을 할당하는 그룹 관리자에 대한 제한 사항 {#limitations-for-a-group-administrator-assigning-a-timesheet-profile}

그룹 관리자이고 액세스 수준에서 관리 액세스 옵션 타임시트 및 시간이 비활성화된 경우 타임시트 프로필을 만들 수 있지만 이를 다음에만 할당할 수 있습니다.

* 관리하는 그룹
* 관리할 그룹에 속한 사용자를 편집할 수 있는 액세스 권한이 있는 개별 사용자

이러한 그룹 및 사용자의 경우 타임시트 프로필에서 생성하는 타임시트에 액세스할 수 없습니다.

또한 액세스 수준에서도 사용자 관리자(그룹 사용자) 옵션이 비활성화되어 있으면 관리하는 그룹에 타임시트 프로필을 할당할 수 있지만, 이 작업은 편집할 수 있는 액세스 권한이 있는 그룹의 사용자만 영향을 받습니다. 그룹에 편집 액세스 권한이 없는 사용자가 포함되어 있으면 그룹의 나머지 사용자와 함께 타임시트 프로필이 할당되지 않습니다.

액세스 수준의 타임시트 및 시간 옵션에 대한 자세한 내용은 [특정 영역에 대한 관리자 액세스 권한 부여](../../administration-and-setup/add-users/configure-and-grant-access/grant-users-admin-access-certain-areas.md)를 참조하십시오.

액세스 수준의 사용자 관리자(그룹 사용자) 옵션에 대한 자세한 내용은 [사용자에게 액세스 권한 부여](../../administration-and-setup/add-users/configure-and-grant-access/grant-access-other-users.md)를 참조하십시오.

## 여러 반복 타임시트 프로필

다음과 같은 경우 조직에 대한 타임시트 프로필을 두 개 이상 보유할 수 있습니다.

* 다양한 사용자 집합에 대한 고유 지급 기간
* 다양한 사용자 집합에 대한 고유 승인자
* 다양한 사용자 집합에 대한 고유한 일반 시간 요구 사항

한 번에 한 명의 사용자를 두 개 이상의 타임시트 프로필과 연결할 수 없습니다.

<!--
<table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader"><strong>Name</strong> </td> 
      <td> <p> Add a name for the timesheet profile. It could be the name of a team or a group whose people share the same timeframe for their timesheets. </p> <p>This ia a required field.</p> </td> 
     </tr> 

   <tr> 
      <td role="rowheader"><strong>Description</strong> </td> 
      <td> <p> Add more information about the timesheet profile.     
      </p> </td> 
     </tr>

   <tr> 
   <td role="rowheader"><strong>Group with Administration Access</strong> </td> 
      <td> <p> 
      <ul> 
      <li> <p>If you are creating a system-level timesheet profile, leave this field blank.</p> <p>Any user who can edit user accounts can attach a system-level timesheet to other users.</p> <p>Only a Workfront administrator can edit a system-level timesheet profile.</p> </li> 
      </ul> 
     <ul> 
      <li> <p>If you are creating a timesheet profile for a group you administer, identify the group here.</p> <p>This does not assign the timesheet profile to the users in the group; it only allows the group's administrators to modify the timesheet profile. You will assign the profile to users in Step 6.</p>

   <p><b>NOTE</b>: When users outside the group are attaching timesheet profiles to other users, they won't be able to see or attach this timesheet profile.</p> </li> 
      </ul> </p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>Create timesheets</strong> </td> 
      <td> <p> <p>Specify when the timesheet profile should generate the timesheets. A timesheet can be set to automatically generate on a weekly, bi-weekly, semi-monthly, or monthly basis. Select the day of the week when you want the timesheet to be produced.</p>
      <p>A weekly timesheet begins on the date it is generated. For example, if you create weekly timesheets every Thursday, the first day of the week on the timesheet is Thursday.</p>
    
      
   <p><b>NOTE</b>: Workfront always creates two timesheets at a time: the first timesheet always includes the current date, and the second timesheet starts when the time frame of the first one ends.</p> </p> </td> 
   </tr> 
     <tr> 
      <td role="rowheader"><p><strong>Approvers</strong></p> </td> 
      <td> <p> <p>Approvers are users who approve the timesheet for the users associated with the timesheet. You can identify up to 7 users as approvers on a timesheet. Identifying multiple users is useful to ensure an approver is available when someone is out of the office. All approvers are notified when a user submits the timesheet for approval. Only one user is required to approve the timesheet in order for it to be approved.</p> <p>Only users with timesheet administrative rights can be set as approvers. For more information about timesheet administrative rights, see <a href="../../administration-and-setup/add-users/configure-and-grant-access/grant-users-admin-access-certain-areas.md" class="MCXref xref">Grant users administrative access to certain areas</a>.</p> <p>Use the drop-down menu&nbsp;to select&nbsp;the approver&nbsp;for the timesheet (if an approver is required). You can select from the following options:</p> 
      <ul> 
      <li><strong>None</strong>: The timesheet does not need to&nbsp;be approved.</li> 
      <li><strong>Their Manager</strong>: This is the default approver, set by the system. In this case, the user designated as their manager approves the timesheet when it is submitted for approval.</li> 
      <li><strong>Specific People:</strong>&nbsp;You can designate specific users, by name, as timesheet approvers. You can have multiple approvers on a timesheet. In this case, after&nbsp;one of the approvers approves the timesheet, the timesheet is marked as <strong>Closed</strong> and it disappears from the timesheet approvals list of all the remaining approvers.</li> 
       </ul> </p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>Can edit time </strong> </td> 
      <td> <p> <p>Select this option to allow the approvers to edit hours on the timesheet. 

   <p>This option works together with the **Restrict timesheet editing to owners and admins** setting in the Setup > Timesheet & Hours > Preferences area. For more information, see <a href="../../administration-and-setup/set-up-workfront/configure-timesheets-schedules/timesheet-and-hour-preferences.md">Configure timesheet and hour preferences</a>.</p>

   <p>The following scenarios exist: </p>

   <ul>
      <li>When the <b>Restrict timesheet editing to owners and admins</b> option is enabled:</li>
      <ul><li>Approvers can only approve and reject timesheet, regardless of whether the <b>Can edit time</b> is enabled or not. </li>
      <li>Timesheet owners' managers can only view their direct reports' timesheets.</li></ul>
      <li>When the <b>Restrict timesheet editing to owners and admins</b> option is disabled:</li>
    <ul><li>When the <b>Can edit time</b> is enabled, approvers can submit, reopen, or close the timesheet and can edit the time.</li>
      <li>When the <b>Can edit time</b> is disabled, approvers cannot submit, reopen, or close the timesheet and cannot edit the time. Approvers can only approve or reject the timesheet. </li>
      <li>Timesheet owners' managers can submit, recall, reopen, and edit their direct reports' timesheets.</li></ul>
      </ul>

   <p>

   <b>NOTE</b>: Once you submit a timesheet for approval, you can no longer edit the hours. To return a submitted timesheet to an editable state, recall the timesheet or have the approver reject the timesheet. For more information, see <a href="../../timesheets/create-and-manage-timesheets/submit-timesheet-for-approval.md">Submit a timesheet for approval</a> and <a href="../../timesheets/create-and-manage-timesheets/timesheet-approvals.md">Approve a timesheet</a>.</p> </p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>Overtime</strong> </td> 
      <td>You can choose to hide the Overtime box in timesheets. This option is disabled by default.</td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>Available Hour Types</strong> </td> 
      <td><p>This setting refers only to General Hour Types, and not to project-specific hour types. </p>
      <p>By default, users see all general hours on a timesheet. However, if your organization wants only specific general hours to be shown for a particular set of users, you can select the general hours that they need to see in their timesheets by selecting them in their timesheet profile in this field. If you want to disable all general hours, deselect all hour types to generate the timesheet without a section for general hours.</p></td> 
     </tr> 

   <tr> 
      <td role="rowheader"><strong>Reminder notifications</strong> </td> 
      <td> <p> Add a reminder notification. Workfront will send reminders to users to ask them to complete or approve their timesheets. You must create reminder notifications before you can associate them with a timesheet profile.  </p> </td> 
     </tr>
    </tbody> 
   </table>
-->