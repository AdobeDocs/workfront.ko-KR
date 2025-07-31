---
product-area: projects;agile-and-teams
navigation-topic: plan-a-project
title: 프로젝트 팀 관리
description: 프로젝트 팀은 프로젝트와 연계된 사용자로 구성됩니다. 프로젝트 팀의 멤버는 프로젝트의 사람 섹션 또는 프로젝트를 만드는 데 사용할 수 있는 템플릿의 사람 섹션에 표시됩니다.
author: Alina
feature: Work Management, Projects
role: User
exl-id: 6e8036fc-feda-4277-9502-0b973028fccb
source-git-commit: fe51ded26c57e3b7137e42ad2218d79adf032b85
workflow-type: tm+mt
source-wordcount: '1280'
ht-degree: 1%

---

# 프로젝트 팀 관리

<!--take preview and production references out at production - August 7-->

<div class="preview">

이 페이지에서 강조 표시된 정보는 아직 일반적으로 사용할 수 없는 기능을 참조합니다. 모든 고객을 위한 미리보기 환경에서만 사용할 수 있습니다. 미리보기 릴리스부터 1주일 후에 모든 고객의 프로덕션 환경에서도 동일한 기능을 사용할 수 있습니다.

자세한 내용은 [인터페이스 현대화](/help/quicksilver/product-announcements/product-releases/interface-modernization/interface-modernization.md)를 참조하십시오.

</div>

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

+++ 를 확장하여 액세스 요구 사항을 확인합니다.

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
   <td> <p>새로운 기능: 표준 </p>
    <p>현재: 플랜 </p>
    </td> 
  </tr> 
  <tr> 
   <td role="rowheader">액세스 수준</td> 
   <td> <p>프로젝트 및 템플릿에 대한 액세스 편집</p> <p>사용자에 대한 보기 또는 상위 액세스 권한</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">개체 권한</td> 
   <td> <p>프로젝트 또는 템플릿에 대한 보기 이상의 권한</p> </td> 
  </tr> 
 </tbody> 
</table>

*자세한 내용은 [Workfront 설명서의 액세스 요구 사항](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)을 참조하십시오.

+++

<!--Old access: 

You must have the following access to perform the steps in this article:

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
   <td> <p>Plan </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Access level configurations*</td> 
   <td> <p>Edit access to Projects</p> <p>View or higher access to Users</p> <p><b>NOTE</b> 
   
   If you still don't have access, ask your Workfront administrator if they set additional restrictions in your access level. For information on how a Workfront administrator can modify your access level, see <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Create or modify custom access levels</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Object permissions</td> 
   <td> <p>View or higher permissions to the project</p> <p>For information on requesting additional access, see <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Request access to objects </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

*To find out what plan, license type, or access you have, contact your Workfront administrator.

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

-->

## 프로젝트에서 사람 관리

1. 프로젝트 팀을 관리할 프로젝트로 이동합니다.

   >[!TIP]
   >
   >작업, 문제에 할당되거나 프로젝트의 관련자로 할당된 사용자가 있어야 사람 섹션에 표시할 수 있습니다.

1. 왼쪽 패널에서 **사람**&#x200B;을 클릭합니다.

1. **사용자 추가**&#x200B;를 클릭합니다.

   **프로젝트 팀에 사용자 추가** 상자가 표시됩니다.

   ![add_users_dialog.png](assets/add-users-dialog-350x217.png)

1. **사용자 추가** 상자에서 프로젝트 팀에 추가할 활성 Workfront 사용자의 이름을 입력한 다음 목록에 표시될 때 이름을 클릭합니다.

   이 단계를 반복하여 프로젝트 팀에 여러 사용자를 추가합니다. 사용자는 프로젝트와 연계된 그룹에 속해야 합니다.

   >[!TIP]
   >
   >* 팀, 그룹, 회사 또는 작업 역할을 추가하여 사용자를 추가할 수 없습니다.
   >* 사용자를 추가할 때 아바타, 사용자의 기본 역할 및 이메일 주소에 따라 동일한 이름을 가진 사용자가 구별됩니다. 사용자를 추가할 때 이를 보려면 사용자를 하나 이상의 작업 역할과 연결해야 합니다.
   >
   >  사용자의 이메일을 보려면 사용자의 액세스 수준에서 연락처 정보 보기 설정을 활성화해야 합니다. 자세한 내용은 [사용자에게 액세스 권한 부여](../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-other-users.md)를 참조하십시오.

1. **추가**&#x200B;를 클릭합니다.

   사용자는 프로젝트에 대한 보기 권한을 얻고 프로젝트 팀의 일부로 프로젝트에 대한 알림을 받게 됩니다.

1. (선택 사항) 작업 역할이 작업, 문제 또는 프로젝트 승인에 추가될 때 사용자에게 알림을 보내려면 사용자의 **작업 역할** 열 내부를 클릭하고 승인과 연결할 작업 역할을 선택하십시오.

   사용자는 선택한 작업 역할에 할당된 승인과 관련된 알림을 받게 됩니다.

   자세한 내용은 문서 [프로젝트 팀 개요](/help/quicksilver/manage-work/projects/planning-a-project/project-team-overview.md)의 &quot;역할 기반 승인&quot; 섹션을 참조하십시오.

1. 목록에서 사용자를 한 명 이상 선택한 다음 **제거** 아이콘 ![제거 아이콘](assets/remove-icon.png)을 클릭하여 팀에서 제거합니다.

1. **예, 선택한 사용자 제거**&#x200B;를 클릭하여 사용자를 확인하고 제거합니다.

   사용자가 미완료 작업 항목에서 제거되고 할당 해제됩니다.

   자세한 내용은 이 문서의 [프로젝트 팀에서 사용자를 제거할 때 고려할 사항](#considerations-for-removing-users-from-a-project-team) 섹션을 참조하십시오.
1. (선택 사항) 이 프로젝트에 대한 업데이트를 사용자에게 보내려면 모두 업데이트 를 클릭하여 팀의 모든 사용자에게 업데이트를 보냅니다

   또는

   목록에서 사용자를 한 명 이상 선택한 다음 **사용자에게 업데이트 보내기**&#x200B;를 클릭합니다.

   ![프로젝트의 사용자에게 업데이트 보내기](assets/send-update-to-user-on-project-box.png)

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

1. 목록에서 사용자를 한 명 또는 여러 명 선택한 다음 **제거**&#x200B;를 클릭하여 팀에서 제거합니다.

1. **예, 선택한 사용자 제거**&#x200B;를 클릭하여 사용자를 확인하고 제거합니다.

   템플릿 작업에서 사용자가 제거되며 할당이 해제됩니다.

   자세한 내용은 이 문서의 [프로젝트 팀에서 사용자를 제거할 때 고려할 사항](#considerations-for-removing-users-from-a-project-team) 섹션을 참조하십시오.

1. (선택 사항) 사용자에게 업데이트를 보내려면 모두 업데이트를 클릭하여 목록의 모든 사용자에게 업데이트를 보냅니다

   또는

   목록에서 사용자를 한 명 이상 선택한 다음 **업데이트**&#x200B;를 클릭합니다.

   <!--update screen shot for unshim production, notice the text above the box - it needs to say "Post an update to each person's profile"-->

   ![템플릿의 사용자 상자로 업데이트 보내기](assets/send-update-to-user-on-template-box.png)

   **사용자에게 업데이트 보내기** 상자가 열립니다.

1. 다음을 수행합니다.

   * 프로덕션 환경에서:

      * 선택한 사용자에 대한 업데이트를 추가합니다.
      * 인물 아이콘을 클릭하여 동일한 업데이트를 수신할 추가 사용자에 태그를 지정합니다.
      * 잠금 아이콘을 클릭하여 회사 내 사용자에 대한 업데이트를 비공개로 만듭니다.
      * **보내기**&#x200B;를 클릭합니다.

   * <span class="preview">미리 보기 환경에서: </span>

   <div class="preview">

   * 선택한 사용자에 대한 업데이트를 추가합니다.
   * 동일한 업데이트를 받을 추가 사용자를 태그 지정하려면 **사람 태그 지정**&#x200B;을 클릭하세요.
   * 업데이트를 회사 사용자에게 비공개로 설정하려면 **내 회사에 비공개** 옵션을 선택하십시오.
   * **보내기**&#x200B;를 클릭합니다.

   </div>

   태그가 지정된 각 사용자 프로필의 **업데이트** 섹션에 업데이트가 추가됩니다.

   사용자는 이메일 알림이 활성화되어 있을 경우 받을 수 있으며 새 업데이트에 대한 인앱 알림을 받게 됩니다.

1. (선택 사항) 사용자 목록을 파일로 내보내려면 **내보내기**&#x200B;를 클릭합니다

   또는

   사용자를 선택한 다음 **내보내기**&#x200B;를 클릭하여 특정 사용자만 내보냅니다.

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

