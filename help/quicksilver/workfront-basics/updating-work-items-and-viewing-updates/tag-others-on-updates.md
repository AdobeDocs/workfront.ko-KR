---
product-area: projects
navigation-topic: update-work-items-and-view-updates
title: 업데이트에 다른 사용자에게 태그 지정
description: Adobe Workfront 객체에 대한 업데이트 주석을 제공할 때 프로젝트의 모든 사용자는 제출된 정보를 볼 수 있습니다. 그러나 프로젝트에 없는 사용자가 이 정보를 볼 수 있는 이점이 있을 수 있습니다. 프로젝트에 해당 사용자를 포함시키지 않고 업데이트에서 해당 사용자에게 태그를 지정하여 사용자와 공유할 수 있습니다. 태그가 지정된 사용자는 이벤트 알림을 받습니다.
author: Lisa and Alina
feature: Get Started with Workfront
exl-id: c4c0d74f-ac50-4fc5-89d6-28f004c25b29
source-git-commit: ba1d8d5a23da7e252e8c182a6bdb1cdd1e304eab
workflow-type: tm+mt
source-wordcount: '773'
ht-degree: 0%

---

# 업데이트에 다른 사용자에게 태그 지정

<!--take "Beta" references out when we remove the beta-->

<!-- Drafted for commenting experience: 

<!--
<span class="preview">The highlighted information on this page refers to functionality not yet generally available. It is available only in the Preview environment.</span> 

>[!NOTE]
>
>We are currently redesigning the commenting experience in Adobe Workfront.
>For more information about the new updating experience, see [New commenting experience](../updating-work-items-and-viewing-updates/unified-commenting-experience.md). 
>
>You can access the new design for the following objects:
> * <span class="preview">Issues, when enabling the commenting Beta. </span>
> * Goals
>   The new commenting experience is the default for goals. You must have an additional license to access Workfront Goals. For more information, see [Requirements to uses Workfront Goals](../../workfront-goals/goal-management/access-needed-for-wf-goals.md). 

-->
객체에 주의를 기울이려면 객체를 업데이트할 때 사용자에게 태그를 지정할 수 있습니다. 그렇지 않으면 사용자가 따르지 않을 수 있습니다.
객체에 해당 사용자를 할당하거나 가입하도록 하여 해당 사용자를 객체에 포함시키지 않고 업데이트 시 해당 사용자에 태그를 지정하여 해당 사용자와 공유할 수 있습니다. 태그가 지정된 사용자는 입력하는 업데이트에 대한 알림을 받습니다.

>[!NOTE]
>
>사용자가 이메일 알림을 받으려면 이벤트 알림을 활성화해야 합니다. 관리자는 전체 시스템 또는 최상위 그룹에 대한 알림을 활성화할 수 있습니다. 사용자는 자신의 사용자 프로필에서 개별 이벤트 알림을 활성화하고 비활성화할 수도 있습니다. 자세한 내용은 다음을 참조하십시오.
>
>* [시스템의 모든 사용자에 대한 이벤트 알림을 구성합니다](../../administration-and-setup/manage-workfront/emails/configure-event-notifications-for-everyone-in-the-system.md).
>* [그룹에 대한 이벤트 알림 보기 및 구성](../../administration-and-setup/manage-groups/create-and-manage-groups/view-and-configure-event-notifications-group.md)
>* [고유한 이벤트 알림 활성화 또는 비활성화](../../workfront-basics/using-notifications/activate-or-deactivate-your-own-event-notifications.md).
>


Workfront 객체에 업데이트 추가에 대한 내용은 [작업 업데이트](../../workfront-basics/updating-work-items-and-viewing-updates/update-work.md).

>[!NOTE]
>
>문제가 프로젝트 또는 작업으로 변환되면 업데이트가 새 프로젝트 또는 작업에 복사되지만 태그가 지정된 사용자는 복사되지 않습니다. 대화를 계속하려면 참가자에게 태그를 다시 지정해야 합니다.

## 액세스 요구 사항

이 문서의 절차를 수행하려면 다음 액세스 권한이 있어야 합니다.

<table style="table-layout:auto"> 
 <col> 
 </col> 
 <col> 
 </col> 
 <tbody> 
  <tr> 
   <td role="rowheader"><strong>Adobe Workfront 플랜*</strong></td> 
   <td> <p>모든</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>Adobe Workfront 라이선스*</strong></td> 
   <td> <p>문제 및 문서에 대한 요청 이상 다른 모든 객체에 대해 검토 또는 이상</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>액세스 수준 구성*</strong></td> 
   <td> <p>문제 및 문서에 대한 요청자 이상 다른 모든 개체의 검토자 이상</p> <p>참고: 여전히 액세스 권한이 없는 경우 Workfront 관리자에게 액세스 수준에서 추가 제한 사항을 설정하는지 문의하십시오. Workfront 관리자가 액세스 수준을 수정하는 방법에 대한 자세한 내용은 <a href="../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">사용자 정의 액세스 수준 만들기 또는 수정</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>개체 권한</strong></td> 
   <td> <p>객체에 대한 액세스 보기</p> <p>추가 액세스 요청에 대한 자세한 내용은 <a href="../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">개체에 대한 액세스 요청 </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

*보유하고 있는 플랜, 라이선스 유형 또는 액세스를 알아보려면 Workfront 관리자에게 문의하십시오.

## 업데이트에 다른 사용자에게 태그 지정

<!--
Tagging others in an update differs depending on which experience and which object you select.

### Tag others on updates in the current Updates section
-->

1. 에 설명된 대로 작업 항목 업데이트를 시작합니다. [작업 업데이트](../../workfront-basics/updating-work-items-and-viewing-updates/update-work.md).
1. 에서 **알림** 필드에서는 포함할 사용자 또는 팀의 이름을 입력하고 드롭다운 목록에 표시될 때 이름을 클릭합니다.

   또는

   에 @ 기호를 입력합니다. **새 업데이트 시작** 영역에서 업데이트에 포함할 사용자 또는 팀의 이름을 입력하고 드롭다운 목록에 나타나면 이름을 클릭합니다.

   >[!TIP]
   >
   >이름이 유사하거나 동일한 사용자가 있을 때 올바른 사용자를 식별하려면 아바타, 사용자의 기본 역할 또는 이메일 주소를 참조하십시오. 업데이트에서 사용자를 태깅할 때 해당 역할을 보려면 사용자를 하나 이상의 작업 역할과 연결해야 합니다.

   ![](assets/tag-users-in-update.png)

1. (선택 사항) 업데이트를 비공개로 설정하려면 다음을 활성화합니다 **회사 개인** 업데이트 상자의 오른쪽 아래 모서리에 있습니다. 이렇게 하면 회사 사용자만 업데이트를 볼 수 있습니다.

   >[!NOTE]
   >
   >회사 외부에서 태그가 지정된 사용자는 업데이트 탭에 비공개 주석이 표시되지 않더라도 인앱 알림 또는 이메일을 받을 수 있습니다. 외부 사용자와 정보를 공유하지 않으려는 경우 업데이트에서 외부 사용자에게 태그를 지정하지 않는 것이 좋습니다.

1. (선택 사항) 여러 사용자와 팀을 추가하려면 2단계를 반복합니다.

   >[!NOTE]
   >
   >알림 필드에 나열된 모든 사용자 및 팀 구성원은 업데이트에 대한 인앱 알림을 받게 되며, 전자 메일 알림 설정의 구성에 따라 이메일을 받을 수 있습니다. 댓글 또는 답글에 태그 지정 또는 응답한 사용자는 해당 댓글 또는 회신에 대한 알림을 받고 나머지 스레드 동안 알림 필드에서 해당 이름을 볼 수 있지만, 다시 태그 지정 없이 다른 알림을 받지 않습니다. 자세한 내용은 [고유한 이벤트 알림 활성화 또는 비활성화](../../workfront-basics/using-notifications/activate-or-deactivate-your-own-event-notifications.md) 및 [시스템의 모든 사용자에 대한 이벤트 알림을 구성합니다](../../administration-and-setup/manage-workfront/emails/configure-event-notifications-for-everyone-in-the-system.md).

1. 클릭 **업데이트**.\
   업데이트에 포함된 사용자는 객체에 대한 보기 권한을 자동으로 부여받고 객체에 대한 업데이트를 보고 응답할 수 있습니다.

   업데이트 스레드 맨 위에서 각 응답에서 태그가 지정된 사용자를 확인할 수 있습니다. 이러한 사용자는 개체를 구독한 사용자와 함께 개체에 대해 업데이트나 응답이 있을 때마다 알림을 받습니다.

   ![](assets/tagging-transparency-350x192.png)

   작업 항목을 업데이트할 때 사용할 수 있는 추가 기능에 대한 자세한 내용은 [작업 업데이트](../../workfront-basics/updating-work-items-and-viewing-updates/update-work.md).

<!--
<div class="preview">

### Tag others on updates in the commenting Beta experience

1. Begin updating a work item, as described in [Update work](../../workfront-basics/updating-work-items-and-viewing-updates/update-work.md).
1. In the **Tag people or teams** field, begin typing the name of the user or team you want to include, then click the name when it appears in the drop-down list.

   <!- ********************* this doesn't seem to work in Beta - keep drafted for now: 
   Or

   Type the @ symbol in the **Start a new update** area, begin typing the name of the user or team you want to include on the update, then click the name when it appears in the drop-down list. ************close draft

   >[!TIP]
   >
   >To identify the correct user when there are users with similar or identical names, notice the avatar, the user's Primary Role, or their email address. Users must be associated with at least one job role to view it as you tag them in an update.

   ![](assets/tag-others-unified-commenting.png)

      <!-******************* this might not be there for issues yet - keep drafted if not: 
      1. (Optional) To make the update private, enable **Private to my company** in the lower-right corner of the update box. This makes the update visible just to users in your company.

         >[!NOTE]
         >
         >* This option displays only when the user is associated with a Company.
         >* Tagged users outside the company could still receive an in-app notification or email, even though they will not see the private comments on the Updates tab. We recommend not to tag external users on an update if you do not want to share the information with them. - ************close draft 
      
1. (Optional) To add multiple users and teams, repeat step 2.

   >[!NOTE]
   >
   >All users and team members listed in the "Tag people or teams" field receive an in-app notification for the update and might receive an email, depending on the configuration of their email notification settings. Users who tag themselves in a comment or reply receive a notification for that comment or reply and can see their name in listed as a member of the thread for the remainder of the thread, but they do not receive another notification unless they tag themselves again. For more information, see [Activate or deactivate your own event notifications](../../workfront-basics/using-notifications/activate-or-deactivate-your-own-event-notifications.md) and [Configure event notifications for everyone in the system](../../administration-and-setup/manage-workfront/emails/configure-event-notifications-for-everyone-in-the-system.md).

1. Click **Submit**.  
   Users included in the update are automatically granted View permission to the object and can view and respond to updates made to the object.

   You can see who has been tagged in each reply under the text of the update, in the Members area. These users, along with any users subscribed to the object, receive a notification whenever an update or reply is made on the object.
1. (Optional) Cick the number of members included in the update to display a list of entities that the update you entered is shared with. 

   ![](assets/members-icons-expanded-unshimmed.png)

   For information about the additional functionality that is available when updating a work item, see [Update work](../../workfront-basics/updating-work-items-and-viewing-updates/update-work.md).

-->