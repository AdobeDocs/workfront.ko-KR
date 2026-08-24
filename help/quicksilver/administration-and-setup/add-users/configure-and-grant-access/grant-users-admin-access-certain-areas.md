---
title: 사용자에게 특정 영역에 대한 관리 액세스 권한 부여
description: Adobe Workfront 관리자는 액세스 수준을 사용하여 플랜 라이선스 사용자에게 시스템의 특정 영역에 대한 관리 액세스 권한을 부여할 수 있습니다.
author: Becky
feature: System Setup and Administration
role: Admin
exl-id: 9d12895d-cf7f-41c6-a2ac-bb731770c187
TQID: https://experienceleague.adobe.com/1nXA0NxLQW3tiIrhCKAd5EMfqBjQW68GHNN42dQmptQ
product_v2:
  - id: c4a86a5d-6562-4fc6-aa00-bfa25833aed9
feature_v2:
  - id: d968a1bc-9a90-4926-a531-bcf272c32aad
subfeature_v2:
  - id: ce22a157-dd2c-405f-b740-c2f204bb4c1a
  - id: d87de1f9-8e24-4c4d-aa4c-a403075091a1
role_v2:
  - id: c66ffd68-0f65-42bb-aa23-b4020f12e0bd
topic_v2:
  - id: bce87dde-a4ab-44c9-8a18-ad66e4ddb377
  - id: eddd9b14-83bd-4ff4-9072-54a4a484abb7
source-git-commit: 9041e7a1c1bf6f7909039fe238b4564ab204752c
workflow-type: tm+mt
source-wordcount: 714
ht-degree: 5%

---

# 사용자에게 특정 영역에 대한 관리 액세스 권한 부여

{{preview-fast-release-general}}

<!--Linked in several places, do not rename or change URL.-->

Adobe Workfront 관리자는 액세스 수준을 사용하여 표준 또는 플랜 라이선스 사용자에게 시스템의 특정 영역에 대한 관리 액세스 권한을 부여할 수 있습니다.

>[!NOTE]
>
>사용자에게 Workfront에 대한 전체 관리 액세스 권한을 부여하는 것과 다릅니다. 자세한 내용은 [사용자에게 전체 관리 액세스 권한 부여](../../../administration-and-setup/add-users/configure-and-grant-access/grant-a-user-full-administrative-access.md)를 참조하십시오&#x200B;.

## 액세스 요구 사항

+++ 이 문서의 기능에 대한 액세스 요구 사항을 보려면 확장하십시오.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront 패키지</td> 
   <td>Any</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront 라이선스</td> 
   <td>   <p>표준</p>
   <p>플랜</p></td> 
  </tr> 
  <tr> 
   <td role="rowheader">액세스 수준 구성</td> 
   <td> <p>Workfront 관리자여야 합니다.</p> </td> 
  </tr> 
 </tbody> 
</table>

이 표의 정보에 대한 자세한 내용은 [Workfront 설명서의 액세스 요구 사항](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)을 참조하십시오.

+++

## Workfront의 특정 영역에 대한 Standard 또는 Plan 사용자에게 관리 액세스 권한 부여

>[!IMPORTANT]
>
>사용자를 설정한 후에 참조할 수 있도록 기본 제공 액세스 수준을 변경하지 않는 것이 좋습니다. 액세스 수준을 사용자 지정하려면 기본 액세스 수준을 복사하고 복사본을 수정합니다. (시스템 관리자 및 외부 사용자를 제외한 모든 액세스 수준에 대해 이 작업을 수행할 수 있습니다.)

{{step-1-to-setup}}

1. 왼쪽 패널에서 **액세스 수준**&#x200B;을 클릭합니다.
1. 사용자에게 Workfront의 특정 영역에 대한 관리 액세스 권한을 부여하는 데 사용할 액세스 수준의 이름을 클릭합니다.
1. **관리 액세스 허용** 섹션에서 필요한 관리 액세스 권한을 부여하는 확인란을 선택하십시오.

   이러한 옵션을 사용하면 다음 기능을 부여할 수 있습니다.

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">승인 프로세스</td> 
      <td><p>시스템 전체에서 그리고 특정 그룹에 사용할 승인 프로세스를 만들고 관리합니다.</p><p>이 액세스 권한이 없으면 사용자는 관리 액세스 권한이 있는 항목에 대해 임시 승인 프로세스만 만들 수 있습니다.</p></td> 
     </tr> 
     <tr> 
      <td role="rowheader"><span class="preview">변경 기록</span></td> 
      <td><p><span class="preview">설정 &gt; 변경 내용 추적 &gt; 변경 내용 목록에서 Workfront 변경 내용 로그를 봅니다.</span></p>
      <p><span class="preview">이 액세스 권한이 없으면 사용자는 설정 영역에서 이 옵션을 사용할 수 없습니다.</span></p></td> 
     </tr> 
     <tr> 
      <td role="rowheader">회사</td> 
      <td><p>Workfront에서 새 회사 추가 및 기존 회사 편집</p>
      <p>이 액세스 권한이 없으면 사용자는 기존 회사만 볼 수 있습니다.</p></td> 
     </tr> 
     <tr> 
      <td role="rowheader">사용자 정의 양식</td> 
      <td><p>그룹 내에서 사용자 정의 양식을 만들고 편집(필드 추가, 편집 및 삭제)합니다.</p><p>이 액세스 권한이 없으면 사용자는 기여 또는 관리에 대한 액세스 권한이 있는 개체에만 기존 양식을 첨부할 수 있습니다.</p></td> 
     </tr> 
     <tr> 
      <td role="rowheader">환율</td> 
      <td> <p>Workfront에서 새 통화를 추가합니다.</p> <p>이 액세스 권한이 없으면 사용자는 자신이 만드는 프로젝트에 기존 통화만 추가할 수 있습니다.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">경비</td> 
      <td><p>Workfront의 개체에 대한 모든 비용을 봅니다.</p><p>사용자가 새 경비 유형을 만들 수 없습니다.</p><p>이 액세스 권한이 없으면 사용자는 다음만 볼 수 있습니다.</p>
       <ul>
        <li>관리하는 프로젝트, 작업 또는 문제의 경비</li>
        <li>자신의 경비</li>
        <li>부하 직원의 비용</li>
       </ul></td> 
     </tr>
     <tr> 
      <td role="rowheader">내 그룹의 마일스톤</td> 
      <td>설정 의 마일스톤 경로 메뉴에서 시스템의 모든 마일스톤 경로를 봅니다. 사용자는 자신의 그룹에 속한 모든 마일스톤 경로를 편집하거나 삭제할 수도 있습니다. 사용자는 그룹 중 어느 것에도 할당되지 않은 마일스톤 경로를 관리(편집 또는 삭제)할 수 없습니다.<br><p>이 액세스 권한이 없으면 사용자는 기존 마일스톤 경로를 보고 관리할 수 있는 액세스 권한이 있는 프로젝트에만 적용할 수 있습니다.</p></td> 
     </tr> 
     <tr> 
      <td role="rowheader">미리 알림</td> 
      <td>Workfront에서 미리 알림을 만들고 관리하십시오.<br>이 액세스 권한이 없는 사용자는 알림을 받고 볼 수 있습니다.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">타임시트 및 시간</td> 
      <td> <p>사용자가 Workfront의 모든 시간과 타임시트를 볼 수 있도록 허용합니다.</p> <p>이 옵션이 비활성화되면 사용자는 다음에 대한 시간만 볼 수 있습니다.</p> 
       <ul> 
        <li>프로젝트, 작업 또는 문제</li> 
        <li>자신의 타임시트</li> 
        <li>사용자에게 보고하는 사람의 타임시트</li> 
        <li>해당 사용자가 승인한 타임시트</li> 
       </ul> <p><b>참고</b>:  <p>이 옵션의 활성화 여부에 관계없이 그룹 관리자는 자신이 관리하는 그룹 및 하위 그룹에 대한 타임시트 프로필을 만들고 편집할 수 있는 액세스 권한이 있는 그룹 구성원에게 할당할 수 있습니다.</p> <p>이 옵션을 활성화하면 관리하는 그룹의 사용자뿐만 아니라 시스템의 모든 사용자에 대해 타임시트 프로필에서 생성된 타임시트(및 시간)를 볼 수 있으므로 일부 그룹 관리자에게 너무 많은 액세스 권한을 제공할 수 있습니다. 액세스 권한이 필요하지 않은 그룹 관리자에 대해 이 옵션을 비활성화할 수 있습니다.</p> </p> </td> 
     </tr> 
    </tbody> 
   </table>

1. 완료되면 **저장**&#x200B;을 클릭하세요.
1. [사용자 추가](../../../administration-and-setup/add-users/create-and-manage-users/add-users.md)에 설명된 대로 사용자에게 새 액세스 수준을 할당합니다.

   >[!NOTE]
   >
   >사용자가 사용자에게 관리 액세스 권한을 부여할 수 있습니다. 사용자가 사용자 계정을 관리할 수 있도록 사용자에게 관리 액세스 권한을 부여하는 방법에 대한 자세한 내용은 [사용자에게 액세스 권한 부여](../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-other-users.md)를 참조하십시오.


<!--     
     <tr> 
      <td role="rowheader">Job roles</td> 
      <td> <p><b>NOTE</b>: In the Preview environment, access to job roles is controlled as an object type in the access level. See <a href="/help/quicksilver/administration-and-setup/add-users/configure-and-grant-access/grant-access-job-roles.md">Grant access to job roles</a>.</p>
      <p>With this access, the user is allowed to do the following:</p> 
       <ul> 
        <li>View and edit existing job roles</li> 
        <li>Add new job roles</li> 
        <li>Edit role billing and cost rates</li> 
       </ul> <p><b>IMPORTANT</b>: If you grant a Standard or Plan user administrative access to job roles, the Financial Data access setting Edit Role Billing &amp; Cost Rates is enabled for the user automatically. Later, if you disable administrative access to job roles for the Standard or Plan user, job roles are still visible to the user because the Edit Role Billing &amp; Cost Rates setting is still enabled. If this happens and you need to remove the user's access to view job roles, you need to disable the user's Edit Role Billing &amp; Cost Rates permission setting. For instructions, see <a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-financial.md" class="MCXref xref">Grant access to financial data</a>.</p> </td> 
     </tr>
-->

<!--
## Access of a Workfront administrator vs. access of a Standard or Plan user with administrative rights  {#access-of-a-workfront-administrator-vs-access-of-a-plan-user-with-administrative-rights}

The two tables below show the difference between the access rights of a user with a Workfront System Administrator access level versus those of a user with a Standard or Plan license with some administrative rights.

Workfront administrators can view all the objects in the system (regardless of who created them), create new ones, and modify or delete existing ones. They have full access to all objects in the system.

Users with a Standard or Plan license who can edit functionality in one area have full access to the functionality in that area.

>[!NOTE]
>
>Users with a Standard or Plan license who are designated as group administrators can perform some of the actions allowed for Workfront administrators. They are allowed to perform these actions only for the groups they administer, their subgroups, and the users in these groups and subgroups. For more information, see [Group administrators](../../../administration-and-setup/manage-groups/group-roles/group-administrators.md).

* [Access to the Setup area](#access-to-the-setup-area)
* [Access to objects](#access-to-objects)

### Access to the Setup area {#access-to-the-setup-area}

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th>Area/object</th> 
   <th>Workfront administrator </th> 
   <th>User with a Standard or Plan license and some administrative rights</th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td>Project Preferences: Projects</td> 
   <td>Full access</td> 
   <td>No access</td> 
  </tr> 
  <tr> 
   <td>Project Preferences: Tasks &amp; Issues</td> 
   <td>Full access</td> 
   <td>No access</td> 
  </tr> 
  <tr> 
   <td>Project Preferences: Statuses</td> 
   <td>Full access</td> 
   <td> <p>No access</p> </td> 
  </tr> 
  <tr> 
   <td>Project Preferences: Priorities</td> 
   <td>Full access</td> 
   <td>No access</td> 
  </tr> 
  <tr> 
   <td>Project Preferences: Severities</td> 
   <td>Full access</td> 
   <td>No access</td> 
  </tr> 
  <tr> 
   <td>Project Preferences: Exchange Rates</td> 
   <td>Full access</td> 
   <td>Full access</td> 
  </tr> 
  <tr> 
   <td>Processes: Approvals</td> 
   <td> <p>Full access</p> </td> 
   <td>Full access</td> 
  </tr> 
  <tr> 
   <td>Processes: Milestone Paths</td> 
   <td>Full access</td> 
   <td>Full access</td> 
  </tr> 
  <tr> 
   <td>Custom Forms</td> 
   <td>Full access</td> 
   <td> <p>Manage custom forms they created or custom forms shared with them.</p> <p>Attach custom forms they created or custom forms shared with them to objects they have manage or contribute permissions to.</p> </td> 
  </tr> 
  <tr> 
   <td>Recycle Bin: Recently Deleted</td> 
   <td>Full access</td> 
   <td> <p>Users who are group administrators can restore projects assigned to Groups they manage, and tasks, issues, or documents associated with those projects.</p> </td> 
  </tr> 
  <tr> 
   <td>Recycle Bin: Recently Restored</td> 
   <td>Full access</td> 
   <td>Users who are group administrators can see the items they have recently restored.</td> 
  </tr> 
  <tr> 
   <td>Job Roles</td> 
   <td>Full access</td> 
   <td> <p>Modify but not delete existing job roles.</p> <p>Add new job roles.</p> </td> 
  </tr> 
  <tr> 
   <td>Teams</td> 
   <td>Full access</td> 
   <td> <p>No access to create Teams.</p> <p>Add existing teams to users when creating or editing users.</p> </td> 
  </tr> 
  <tr> 
   <td>Groups</td> 
   <td>Full access</td> 
   <td> <p>No access to create Groups.</p> <p>Only group administrators can manage group membership, subgroups, and group-level statuses for the groups they manage. </p> </td> 
  </tr> 
  <tr> 
   <td>Companies</td> 
   <td>Full access</td> 
   <td>Full access</td> 
  </tr> 
  <tr> 
   <td>Log in As</td> 
   <td>Full access </td> 
   <td> <p>If their group administrative access is enabled on their access level and they are designated as a group administrator, they can log in as the users in the group they administer and their subgroups. They cannot log in as a System Administrator.<br>For more information about enabling group administrative access for users, see <a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-other-users.md" class="MCXref xref">Grant access to users</a>.</p> </td> 
  </tr> 
  <tr> 
   <td>Schedules</td> 
   <td>Full access</td> 
   <td> <p>No access to edit Schedules.</p> <p>Access to add existing schedules to other users, at the user level. </p> </td> 
  </tr> 
  <tr> 
   <td>Timesheet &amp; Hours: Timesheet Profiles</td> 
   <td>Full access</td> 
   <td> <p>Access to assign existing Timesheet Profiles to users, at the user level.</p> <p>Users who are group administrators can create Timesheet Profiles for the groups they administer and their subgroups. </p> </td> 
  </tr> 
  <tr> 
   <td>Timesheet &amp; Hours: Hour Types</td> 
   <td>Full access</td> 
   <td> <p>Access to assign Hour Types to users, at the user level.</p> </td> 
  </tr> 
  <tr> 
   <td>Timesheet &amp; Hours: Preferences</td> 
   <td>Full access</td> 
   <td>No access</td> 
  </tr> 
  <tr> 
   <td>Email: Notifications: Event Notifications</td> 
   <td>Activate/ Deactivate all</td> 
   <td>No access</td> 
  </tr> 
  <tr> 
   <td>Email: Notifications: Reminder Notifications</td> 
   <td>Full access</td> 
   <td>Full access</td> 
  </tr> 
  <tr> 
   <td>Email: Notifications: Email Templates</td> 
   <td>Full access</td> 
   <td> <p>No access to edit Email Templates.</p> <p>Access to add existing Email Templates to Reminder Notifications.</p> </td> 
  </tr> 
  <tr> 
   <td>Email: Automatic Reminders</td> 
   <td>Full access</td> 
   <td>No access</td> 
  </tr> 
  <tr> 
   <td>Email: Invitations</td> 
   <td>Full access</td> 
   <td> <p>No access to edit Email Invitations.</p> <p>Access to resend email invitations to unregistered users only from the People tab.</p> </td> 
  </tr> 
  <tr> 
   <td>Email: Setup</td> 
   <td>Full access</td> 
   <td> <p>No access</p> </td> 
  </tr> 
  <tr> 
   <td>Scorecards</td> 
   <td>Full access</td> 
   <td> <p>Full access</p> </td> 
  </tr> 
  <tr> 
   <td>Expense Types</td> 
   <td>Full access</td> 
   <td> <p>No access</p> </td> 
  </tr> 
  <tr> 
   <td>Risk Types</td> 
   <td>Full access</td> 
   <td>No access</td> 
  </tr> 
  <tr> 
   <td>Access Levels</td> 
   <td> <p>Full access to modify all access levels.</p> <p>The System Administrator and External User access levels cannot be modified, by default.</p> </td> 
   <td> <p>No access to edit Access Levels.</p> <p>Assign an access level to other users which is lower or equal to theirs at the user level.</p> </td> 
  </tr> 
  <tr> 
   <td>Interface: Layout Templates</td> 
   <td>Full access</td> 
   <td> <p>Access to assign existing Layout Templates to other users, at the user level. </p> <p>Users designated as group administrators can create Layout Templates for groups and subgroups they manage.</p> </td> 
  </tr> 
  <tr> 
   <td>Interface: Update Feeds</td> 
   <td>Full access</td> 
   <td> <p>No access to modify Update Feeds.</p> <p>Access to add fields to be tracked in the Update Feeds when editing Custom Forms.</p> </td> 
  </tr> 
  <tr> 
   <td>Interface: Filters</td> 
   <td>Full access</td> 
   <td> <p>No access to create Filters in the Setup area.</p> <p>Access to create new filters in a list of objects.</p> </td> 
  </tr> 
  <tr> 
   <td>Interface: Views</td> 
   <td>Full access</td> 
   <td> <p>No access to create Views in the Setup area.</p> <p>Access to create new views in a list of objects.</p> </td> 
  </tr> 
  <tr> 
   <td>Interface: Groupings</td> 
   <td>Full access</td> 
   <td> <p>No access to create Groupings in the Setup area.</p> <p>Access to create new groupings in a list of objects.</p> </td> 
  </tr> 
  <tr> 
   <td>Interface: List Controls</td> 
   <td>Full access</td> 
   <td> <p>No access</p> </td> 
  </tr> 
  <tr> 
   <td>Documents: Cloud Providers</td> 
   <td>Full access</td> 
   <td> <p>No access to configure Cloud Providers.</p> <p>Access to link documents to and from Cloud Providers from the Documents tab, after the Cloud Providers have been integrated with Workfront.</p> </td> 
  </tr> 
  <tr> 
   <td>Documents: Metadata Mapping</td> 
   <td>Full access</td> 
   <td>No access</td> 
  </tr> 
  <tr> 
   <td>Documents: SharePoint Integration</td> 
   <td>Full access</td> 
   <td> <p>No access to configure a SharePoint integration.</p> <p>Access to link documents to and from SharePoint from the Documents tab, after the SharePoint integration with Workfront has been configured.</p> </td> 
  </tr> 
  <tr> 
   <td>Documents: Custom Integration</td> 
   <td>Full access</td> 
   <td> <p>No access to configure a Custom Integration.</p> <p>Access to link documents to and from third-party providers from the Documents tab, after the third-party providers have been integrated with Workfront.</p> </td> 
  </tr> 
  <tr> 
   <td>System: Branding</td> 
   <td>Full access</td> 
   <td>No access</td> 
  </tr> 
  <tr> 
   <td>System: Customer Info</td> 
   <td>Full access</td> 
   <td>No access</td> 
  </tr> 
  <tr> 
   <td>System: Single Sign-On (SSO)</td> 
   <td>Full access</td> 
   <td>No access</td> 
  </tr> 
  <tr> 
   <td>System: Update Users for SSO</td> 
   <td>Full access</td> 
   <td>No access</td> 
  </tr> 
  <tr> 
   <td>System: Kick-Starts</td> 
   <td>Full access</td> 
   <td>No access</td> 
  </tr> 
  <tr> 
   <td>System: Diagnostics</td> 
   <td>Full access</td> 
   <td>No access</td> 
  </tr> 
  <tr> 
   <td>System: Preferences</td> 
   <td>Full access</td> 
   <td>No access</td> 
  <tr> 
   <td>Change Tracking: Configuration</td> 
   <td>Full access</td> 
   <td>No access</td> 
  <tr> 
   <td>Change Tracking: Change History List</td> 
   <td>Full access</td> 
   <td>Full access</td> 
  </tr> 
 </tbody> 
</table>

### Access to objects {#access-to-objects}

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th>Area/object</th> 
   <th>Workfront administrator </th> 
   <th>User with a Standard or Plan license and some administrative rights</th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td>Calendars</td> 
   <td>Full access</td> 
   <td>Manage calendars they create and calendars shared with them.</td> 
  </tr> 
  <tr> 
   <td>Dashboards</td> 
   <td>Full access</td> 
   <td>Manage dashboards they create and dashboards shared with them.</td> 
  </tr> 
  <tr> 
   <td>Documents</td> 
   <td>Full access</td> 
   <td>Manage documents they upload or documents shared with them.</td> 
  </tr> 
  <tr> 
   <td>Issues</td> 
   <td>Full access</td> 
   <td>Manage issues they create or issues shared with them.</td> 
  </tr> 
  <tr> 
   <td>Portfolios</td> 
   <td>Full access</td> 
   <td>Manage portfolios they create or portfolios shared with them. </td> 
  </tr> 
  <tr> 
   <td>Programs</td> 
   <td>Full access</td> 
   <td>Manage programs they create or programs shared with them.</td> 
  </tr> 
  <tr> 
   <td>Project</td> 
   <td>Full access</td> 
   <td>Manage projects they create or projects shared with them.</td> 
  </tr> 
  <tr> 
   <td>Reports</td> 
   <td>Full access</td> 
   <td>Manage reports they create or reports shared with them. View, copy and edit system reports.</td> 
  </tr> 
  <tr> 
   <td>Tasks</td> 
   <td>Full access</td> 
   <td>Manage tasks they create or tasks shared with the</td> 
  </tr> 
  <tr> 
   <td>Templates</td> 
   <td>Full access</td> 
   <td>Manage templates they create or templates shared with them</td> 
  </tr> 
  <tr> 
   <td>Timesheets</td> 
   <td>Full access</td> 
   <td>Full access</td> 
  </tr> 
  <tr> 
   <td>Users</td> 
   <td>Full access</td> 
   <td> <p>Limited access</p> <p>They cannot assign groups to users for which they are not a group administrator or groups that are not public.</p> <p>They cannot assign an access level to users which is higher then their own access level.</p> <p>If their group administrative access is enabled on their access level and they are designated as a group administrator on a group, they can reset the password of and log in as the users in the group they administer and their subgroups. They cannot reset the password of or log in as a System Administrator.<br>For more information about enabling group administrative access for users, see <a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-other-users.md" class="MCXref xref">Grant access to users</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

-->


