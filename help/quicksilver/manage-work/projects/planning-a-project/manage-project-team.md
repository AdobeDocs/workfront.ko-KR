---
product-area: projects;agile-and-teams
navigation-topic: plan-a-project
title: 프로젝트 팀 관리
description: 프로젝트 팀은 프로젝트와 연계된 사용자로 구성됩니다. 프로젝트 팀의 멤버는 프로젝트의 사람 섹션 또는 프로젝트를 만드는 데 사용할 수 있는 템플릿의 사람 섹션에 표시됩니다.
author: Alina
feature: Work Management, Projects
role: User
exl-id: 6e8036fc-feda-4277-9502-0b973028fccb
source-git-commit: 00e693fc8b35a59f6ed212bc30da7f85cc78c845
workflow-type: tm+mt
source-wordcount: '838'
ht-degree: 2%

---

# 프로젝트 팀 관리

<!--take preview and production references out at production - August 7-->

<!--<div class="preview"> 

The highlighted information on this page refers to functionality not yet generally available. It is available only in the Preview environment for all customers. The same features will also be available in the Production environment for all customers after a week from the Preview release.      

For more information, see [Interface modernization](/help/quicksilver/product-announcements/product-releases/interface-modernization/interface-modernization.md).  

</div>

-->

프로젝트 팀은 프로젝트와 연계된 사용자로 구성됩니다. 자세한 내용은 [프로젝트 팀 개요](/help/quicksilver/manage-work/projects/planning-a-project/project-team-overview.md)를 참조하십시오.

프로젝트 팀의 멤버가 프로젝트의 사람 섹션에 표시됩니다.

템플릿에서 프로젝트를 만든 후 프로젝트 템플릿의 사람 섹션에 표시되는 사용자는 프로젝트 팀이 됩니다.

프로젝트와 템플릿 모두에 대해 다음 사용자가 프로젝트 팀에 자동으로 추가됩니다.

* 소유자
* 스폰서
* 작업에 할당된 사용자
* 문제에 할당된 사용자(프로젝트에만 해당)

프로젝트 팀의 사용자는 프로젝트에 대한 알림을 받습니다. 자세한 내용은 [이벤트 알림 유형](/help/quicksilver/administration-and-setup/manage-workfront/emails/event-notifications-available-in-wf.md)을 참조하세요.

프로젝트 및 템플릿의 팀에 사용자를 추가(프로젝트만 해당)하거나 제거하거나 업데이트를 전송하여 관리할 수 있습니다.

## 액세스 요구 사항

+++ 을 확장하여 이 문서의 기능에 대한 액세스 요구 사항을 봅니다. 

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront 패키지</td> 
   <td> <p>임의</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront 라이선스</td> 
   <td> <p>표준</p>
    <p>플랜</p>
    </td> 
  </tr> 
  <tr> 
   <td role="rowheader">액세스 수준 구성</td> 
   <td> <p>프로젝트 및 템플릿에 대한 액세스 편집</p> <p>사용자에 대한 보기 또는 상위 액세스 권한</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">개체 권한</td> 
   <td> <p>프로젝트 또는 템플릿에 대한 보기 이상의 권한</p> </td> 
  </tr> 
 </tbody> 
</table>

자세한 내용은 [Workfront 설명서의 액세스 요구 사항](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)을 참조하십시오.

+++

<!--Old access: 

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
   <td> <p>Standard </p>
    <p>Plan </p>
    </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Access level</td> 
   <td> <p>Edit access to Projects and Templates</p> <p>View or higher access to Users</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Object permissions</td> 
   <td> <p>View or higher permissions to a project or to a template</p> </td> 
  </tr> 
 </tbody> 
</table>

*For information, see [Access requirements in Workfront documentation](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).



## Add users to a Project Team

When you add users to the project team, they gain View permissions on the project and the tasks, issues, and documents of the project. For more information, see the article [Project Team overview](../../../manage-work/projects/planning-a-project/project-team-overview.md).

>[!TIP]
>
>Users on the Project Team are not automatically added to the resource management tools for the project.

You can add users to the project team in the following ways:

* [Automatically add users to a Project Team](#automatically-add-users-to-a-project-team) 
* [Manually add users to a Project Team](#manually-add-users-to-a-project-team)

### Automatically add users to a Project Team {#automatically-add-users-to-a-project-team}

The users that fulfill the following roles on the project are automatically added to the project team and appear  in the People section when the project is created:

* The creator of the project
* The project owner
* The project sponsor

Users are also automatically added to the project team when they are assigned to the following:

* Tasks
* Issues

### Manually add users to a Project Team {#manually-add-users-to-a-project-team}

If users that don't fulfill any role on the project want to be notified about certain updates or changes during the life of the project, you can manually add them to the project team. 

 For more information about what notifications can be enabled for users on the project team, see [Event notification types](../../../administration-and-setup/manage-workfront/emails/event-notifications-available-in-wf.md). 

 <!--drafted - this used to be the case, in the note below but this limitation was removed on Jan 5, 2023 - as a patch, not a release feature:

>[!IMPORTANT]
>
>You can add to the Project Team only users that belong to the Group associated with the project. You cannot add users that belong to the Subgroups of the project's group. 



## Manage people on a project

1. Go to the project you want to manage the project team for.

   >[!TIP]
   >
   >You must have users assigned to tasks, issues or as stakeholders on the project to have them display in the People section.

1. Click **People** in the left panel. 

1. Click **Add users**. 

   The **Add users to Project Team** box displays.

   ![add_users_dialog.png](assets/add-users-dialog-350x217.png)

1. In the **Add users** box, begin typing the name of an active Workfront user that you want to add to the project team, then click the name when it appears in the list.

   Repeat this step to add multiple users to the project team. The users must belong to the group associated with the project. 

   >[!TIP]
   >
   >* You cannot add users by adding their teams, groups, companies, or job roles.
   >* As you add the users, notice the avatar, the user's Primary Role, and their email address to distinguish between users with identical names. Users must be associated with at least one job role to view it as you add them.
   >
   >  You must have the View Contact Info setting enabled in your access level for Users to view users' emails. For information, see [Grant access to users](../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-other-users.md).

1. Click **Add**.

   The users gain View permissions to the project and receive notifications about the project as part of the project team.

1. (Optional) If you want a user to receive a  notification when their job role is added to a task, issue, or project approval, click inside the **Job Role** column for the user, and select a job role that will be associated with the approval. 

   The users will receive notifications related to the approvals assigned to the selected job role. 

   For more information see the "Role-based approvals" section in the article [Project Team overview](/help/quicksilver/manage-work/projects/planning-a-project/project-team-overview.md).

1. Select one or several users in the list, then click the **Remove** icon ![Remove icon](assets/remove-icon.png) to remove them from the team. 
 
1. Click **Yes, Remove Selected Users** to confirm and remove the users.

   Users are removed and unassigned from incomplete work items.

   For more information, see the [Considerations for removing users from a project team](#considerations-for-removing-users-from-a-project-team) section in this article.
1. (Optional) To send an update for this project to users, click **Update All** to send the update to everyone on the team

   Or 

   Select one or multiple users in the list, then click **Send Update to User**.

   <!--update screen shot when they fix the bug - the text above the box needs to match the OLD box, below-->

![프로젝트의 사용자 상자로 업데이트 보내기](assets/send-update-to-user-on-project-box-2025.png)

<!--Old UI for projects but the text above the comment box is right and matches the functionality):
   ![OLD Send update to user on a project](assets/send-update-to-user-on-project-box.png)-->

**사용자에게 업데이트 보내기** 상자가 열립니다.

1. 다음 중 하나를 수행하십시오.

   * 선택한 사용자에 대한 업데이트를 추가합니다.
   * 잠금 아이콘을 클릭하여 회사 내 사용자에 대한 업데이트를 비공개로 만듭니다.
   * 추가 사용자에 태그를 지정하여 동일한 업데이트를 받습니다.
   * **보내기**&#x200B;를 클릭합니다.

   업데이트가 프로젝트의 **업데이트** 섹션에 추가되고 선택한 모든 사용자가 태그 지정된 사용자로 표시됩니다.

   사용자는 이메일 알림이 활성화되어 있을 경우 받을 수 있으며 새 업데이트에 대한 인앱 알림을 받게 됩니다.

1. (선택 사항) 사용자 목록을 파일로 내보내려면 **내보내기** 아이콘 ![내보내기 아이콘](assets/export-icon.png)을 클릭합니다

   또는

   사용자를 선택한 다음 **내보내기** 아이콘을 클릭하여 특정 사용자만 내보냅니다.

## 템플릿에서 직원 관리

1. 프로젝트 팀을 관리할 템플릿으로 이동합니다.

   >[!TIP]
   >
   >작업에 할당되거나 템플릿에 대한 이해 당사자로 할당된 사용자가 인력 섹션에 표시되도록 해야 합니다.

1. 왼쪽 패널에서 **사람**&#x200B;을 클릭합니다.

1. 목록에서 사용자를 한 명 또는 여러 명 선택한 다음 **제거** 아이콘을 클릭하여 팀에서 제거합니다.

1. **예, 선택한 사용자 제거**&#x200B;를 클릭하여 사용자를 확인하고 제거합니다.

   템플릿 작업에서 사용자가 제거되며 할당이 해제됩니다.

   자세한 내용은 이 문서의 [프로젝트 팀에서 사용자를 제거할 때 고려할 사항](#considerations-for-removing-users-from-a-project-team) 섹션을 참조하십시오.

1. (선택 사항) 업데이트를 사용자에게 보내려면 **모두 업데이트**&#x200B;를 클릭하여 목록의 모든 사용자에게 업데이트를 보냅니다

   또는

   목록에서 사용자를 한 명 이상 선택한 다음 **사용자에게 업데이트 보내기**&#x200B;를 클릭합니다.

   <!--update screen shot for unshim production, notice the text above the box - it needs to say "Post an update to each person's profile"-->

   ![템플릿의 사용자 상자로 업데이트 보내기](assets/send-update-to-user-on-template-box.png)

   **사용자에게 업데이트 보내기** 상자가 열립니다.

1. 다음을 수행합니다.

   * 선택한 사용자에 대한 업데이트를 추가합니다.
   * 동일한 업데이트를 받을 추가 사용자를 태그 지정하려면 **사람 태그 지정**&#x200B;을 클릭하세요.
   * 업데이트를 회사 사용자에게 비공개로 설정하려면 **내 회사에 비공개** 옵션을 선택하십시오.
   * **보내기**&#x200B;를 클릭합니다.

     >[!TIP]
     >
     >**회사에 비공개** 설정은 Workfront 프로필이 회사와 연결되어 있을 때만 사용할 수 있습니다.

   태그가 지정된 각 사용자 프로필의 **업데이트** 섹션에 업데이트가 추가됩니다.

   사용자는 이메일 알림이 활성화되어 있을 경우 받을 수 있으며 새 업데이트에 대한 인앱 알림을 받게 됩니다.

1. 사용자 목록을 파일로 내보내려면 **내보내기** 아이콘 ![내보내기 아이콘](assets/export-icon.png)을 클릭하십시오.

   또는

   사용자를 선택한 다음 **내보내기** 아이콘을 클릭하여 특정 사용자만 내보냅니다.

## 프로젝트 팀에서 사용자 제거 시 고려 사항

프로젝트에서 사용자를 역할에서 제거하면 해당 사용자는 프로젝트 팀의 일부로 유지됩니다.

프로젝트 팀에 전송된 알림의 수신을 중단하려면 프로젝트의 사람 섹션에서 프로젝트 팀을 제거해야 합니다.

프로젝트 팀에서 사용자를 제거하고 사용자가 프로젝트의 작업 또는 문제에 할당되면 완료되지 않은 작업 및 문제에서 사용자가 할당 해제됩니다. 이 경우 작업과 문제는 업무 균형자의 미할당 작업 영역으로 돌아갑니다.

완료된 작업 및 문제에 할당된 사용자는 프로젝트 팀에서 제거한 후에도 작업 및 문제에 할당된 상태로 유지됩니다.

프로젝트 또는 템플릿의 사람 섹션에서 다음 사용자를 제거하면 해당 사용자가 프로젝트에 대한 역할에서 제거됩니다.

* 미완료 작업에 할당된 사용자
* 미완료 문제에 할당된 사용자

다음 사용자는 프로젝트 또는 템플릿의 인물 섹션에서 제거할 때 프로젝트에 대한 역할에서 제거되지 않습니다.

* 소유자
* 스폰서

프로젝트 팀에서 사용자를 제거하는 방법에 대한 자세한 내용은 [프로젝트에서 사용자 제거](../../../manage-work/projects/manage-projects/remove-users-from-projects.md)를 참조하십시오.

