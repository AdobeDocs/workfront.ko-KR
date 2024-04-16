---
product-area: projects
navigation-topic: update-work-items-and-view-updates
title: 업데이트에 다른 사용자 태그 지정
description: Adobe Workfront 개체에 업데이트 설명을 제공하면 프로젝트의 모든 사용자가 제출된 정보를 볼 수 있습니다. 그러나 프로젝트에 없는 사용자가 이 정보를 볼 때 혜택을 받을 때가 있을 수 있습니다. 프로젝트에 해당 사용자를 포함시키는 대신 업데이트에 태그를 지정하여 사용자와 공유할 수 있습니다. 태그 지정된 사용자가 이벤트 알림을 받습니다.
author: Alina
feature: Get Started with Workfront
exl-id: c4c0d74f-ac50-4fc5-89d6-28f004c25b29
source-git-commit: a9cfeaadad136f503797794050e8bc23f1392f22
workflow-type: tm+mt
source-wordcount: '997'
ht-degree: 0%

---

# 업데이트에 다른 사용자 태그 지정

<!--Audited: April, 2024-->

<!--
>[!IMPORTANT]
>
>We are currently redesigning the commenting experience in Adobe Workfront.
>
>Depending on what objects you access the commenting experience for, you might see the following functionality for the Updates section:
>* The new experience
>* The legacy experience
>* The new and the legacy experience
>
>For more information about the new commenting experience and its availability, see [New commenting experience](../../product-announcements/betas/new-commenting-experience-beta/unified-commenting-experience.md). 
>
><Span class="preview"> The legacy commenting experience has been removed from projects, tasks, issues, and documents in the Preview environment. </span>
>
>The new commenting experience is available only for the Updates section of Workfront objects, and it is not available when you access updates from the following areas:
>
> * Home
> * Summary panel in lists
> * Summary panel in timesheets 
> * Summary panel in the Workload Balancer
>
><span class="preview">The new commenting experience is available in the Summary panel in lists, timesheets, and the Workload Balancer in the Preview environment and in the Production environment for customers who have opted for the fast release process. </span> 
-->

오브젝트를 업데이트할 때 사용자가 따르지 않을 수 있는 오브젝트에 주의를 집중시키려면 사용자를 태그 지정할 수 있습니다.

이러한 사용자를 객체에 할당하거나 구독하도록 하여 해당 사용자를 객체에 포함시키는 대신, 업데이트에서 태그를 지정하여 사용자와 공유할 수 있습니다. 태그가 지정된 사용자는 입력한 업데이트에 대한 Workfront 알림을 받습니다. 알림 설정에 따라 입력한 업데이트에 대한 이메일을 받게 됩니다.

## 업데이트의 사용자 태그 지정에 대한 고려 사항

* 업데이트를 태그 지정한 사용자가 이메일 알림을 받으려면 프로필에서 개인 알림을 활성화해야 합니다. 자세한 내용은 [이메일 알림 수정](../../workfront-basics/using-notifications/activate-or-deactivate-your-own-event-notifications.md).

  Workfront 개체에 업데이트를 추가하는 방법에 대한 자세한 내용은 [작업 업데이트](../../workfront-basics/updating-work-items-and-viewing-updates/update-work.md).

* 문제가 프로젝트 또는 작업으로 전환되면 업데이트가 새 프로젝트 또는 작업에 복사되지만 태그가 지정된 사용자는 복사되지 않습니다. 대화를 계속하려면 참가자를 다시 태그 지정해야 합니다.

## 액세스 요구 사항

이 문서의 단계를 수행하려면 다음 액세스 권한이 있어야 합니다.

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"><strong>Adobe Workfront 플랜</strong></td> 
   <td> <p>임의</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>Adobe Workfront 라이센스*</strong></td> 
   <td> <p>새로운 기능: 문제 및 문서에 대한 기여자 이상, 기타 모든 오브젝트에 대한 라이트 이상</p>
   <p>현재: 문제 및 문서에 대해 요청 이상, 다른 모든 객체에 대해 검토 이상</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>액세스 수준 구성</strong></td> 
   <td> <p>답글을 게시하려는 오브젝트에 대한 보기 이상의 액세스 권한</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>개체 권한</strong></td> 
   <td> <p>답글을 게시하려는 오브젝트에 대한 이상의 권한 보기</p> </td> 
  </tr> 
 </tbody> 
</table>

*보유 중인 플랜, 라이선스 유형 또는 액세스 권한을 확인하려면 Workfront 관리자에게 문의하십시오. 자세한 내용은 [Workfront 설명서에 대한 액세스 요구 사항](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

## 업데이트에 다른 사용자 태그 지정

다음과 같은 방법으로 업데이트에 다른 사용자를 태그 지정할 수 있습니다.

* **자동**: 사용자가 스레드를 시작하거나, 댓글을 추가하거나, 답글을 추가하면 자동으로 태그가 지정되고 댓글 달기 상자의 사람 또는 팀 태그 영역에 추가됩니다.
* **수동**: 댓글 달기 상자의 인물 태그 영역에 사용자를 수동으로 추가하는 경우.

댓글을 편집하거나 답글을 달 때 실수로 태그가 지정된 사용자를 제거할 수도 있습니다.

1. 에 설명된 대로 작업 항목 업데이트를 시작합니다. [작업 업데이트](../../workfront-basics/updating-work-items-and-viewing-updates/update-work.md). 댓글 소유자는 자동으로 태그를 지정하고 댓글 달기 상자의 사람 또는 팀 태그 영역에 추가됩니다.

   >[!TIP]
   >
   >댓글 소유자는 댓글 상자의 태그 사용자 또는 팀 영역에서 자신의 이름을 볼 수 없습니다.

1. 다음에서 **사람 또는 팀에 태그 지정** 필드에 포함할 사용자 또는 팀의 이름을 입력한 다음 드롭다운 목록에 나타나면 이름을 클릭합니다.

   또는

   다음에 @ 기호를 입력합니다. **댓글 작성** 영역에 업데이트에 포함할 사용자 또는 팀의 이름을 입력한 다음 드롭다운 목록에 나타나면 이름을 클릭합니다.

   >[!TIP]
   > 
   >이름이 유사하거나 동일한 사용자가 있을 때 올바른 사용자를 식별하려면 아바타, 사용자의 기본 역할 또는 이메일 주소를 확인합니다.
   > 
   >업데이트에서 태그 지정할 때 사용자를 보려면 최소 하나 이상의 작업 역할과 연결되어 있어야 합니다.
   > 
   >사용자의 이메일을 보려면 사용자의 액세스 수준에서 연락처 정보 보기 설정을 활성화해야 합니다. 자세한 내용은 [사용자에게 액세스 권한 부여](../../administration-and-setup/add-users/configure-and-grant-access/grant-access-other-users.md).

   ![사용자 태그 지정](assets/tag-others-unified-commenting-with-all-tab.png)

1. (선택 사항) 업데이트를 비공개로 설정하려면 을 활성화합니다 **내 회사에 비공개** 업데이트 상자의 오른쪽 아래 모서리에 있습니다. 이렇게 하면 회사의 사용자에게만 업데이트가 표시됩니다. 다음 **내 회사에 비공개** 옵션은 회사가 Workfront 프로필에 지정된 경우에만 사용할 수 있습니다.

   >[!NOTE]
   >
   >* 이 옵션은 사용자가 회사와 연결되어 있을 때만 표시됩니다.
   >* 회사 외부의 태그 지정된 사용자는 업데이트 탭에 개인 댓글이 표시되지 않더라도 인앱 알림이나 이메일을 계속 받을 수 있습니다. 외부 사용자와 정보를 공유하지 않으려면 업데이트에 외부 사용자에게 태그를 지정하지 않는 것이 좋습니다.

1. (선택 사항) 여러 사용자와 팀을 추가하려면 2단계를 반복합니다. <!--insure this stays accurate-->

   >[!NOTE]
   >
   >&quot;직원 또는 팀 태그&quot; 필드에 나열된 모든 사용자 및 팀 구성원은 업데이트에 대한 인앱 알림을 받으며 이메일 알림 설정의 구성에 따라 이메일을 받을 수 있습니다. 댓글 또는 회신에 태그를 지정한 사용자는 해당 댓글 또는 회신에 대한 알림을 받고, 나머지 스레드 동안 스레드 멤버로 이름이 나열된 상태로 볼 수 있지만 자신을 다시 태그 지정하지 않는 한 다른 알림을 받지 않습니다. 자세한 내용은 [이메일 알림 수정](../../workfront-basics/using-notifications/activate-or-deactivate-your-own-event-notifications.md) 및 [시스템의 모든 사용자를 위한 이벤트 알림 구성](../../administration-and-setup/manage-workfront/emails/configure-event-notifications-for-everyone-in-the-system.md).

1. 클릭 **제출**.\
   업데이트에 포함된 사용자에게는 객체에 대한 보기 권한이 자동으로 부여되고 객체에 대한 업데이트를 보고 응답할 수 있습니다.

   태그가 지정된 엔티티의 이름이 해당 아바타 옆에 최대 2개의 엔티티로 표시됩니다. 두 개 이상의 엔티티에 태그가 지정되어 있으면 태그가 지정된 추가 엔티티 수와 함께 첫 번째 엔티티의 이름이 표시됩니다.

   ![](assets/members-icons-expanded-unshimmed.png)

   주석 텍스트에서 태그가 지정되면 해당 주석에서 이름이 강조 표시됩니다.

   작업 항목을 업데이트할 때 사용할 수 있는 추가 기능에 대한 자세한 내용은 [작업 업데이트](../../workfront-basics/updating-work-items-and-viewing-updates/update-work.md).

1. (선택 사항) **자세히** 메뉴 ![](assets/more-menu.png) 주석의 오른쪽 상단 모서리에서 을(를) 클릭한 다음 을(를) 클릭합니다 **편집**. 태그된 사용자를 제거한 다음 **제출**.

   >[!IMPORTANT]
   >
   >댓글을 입력한 후 15분 이내에만 편집할 수 있습니다. 추가한 의견만 편집할 수 있습니다.


<!--
   >[!TIP]
   >
   >When using the legacy commenting experience to add comments and replies, comment owners that were not specifically tagged cannot be manually removed by people who use the new commenting experience.
-->

<!--
### Tag others on updates in the legacy Updates section

You can manually tag users in the legacy Updates section. 

1. Begin updating a work item, as described in [Update work](../../workfront-basics/updating-work-items-and-viewing-updates/update-work.md).
1. In the **Notify** field, begin typing the name of the user or team you want to include, then click the name when it appears in the drop-down list.

   Or

   Type the @ symbol in the **Start a new update** area, begin typing the name of the user or team you want to include on the update, then click the name when it appears in the drop-down list.

   >[!TIP]
   >
   >To identify the correct user when there are users with similar or identical names, notice the avatar, the user's Primary Role, or their email address. 
   >
   >Users must be associated with at least one job role to view it as you tag them in an update. 
   >
   >You must have the View Contact Info setting enabled in your access level for Users to view users' emails. For information, see [Grant access to users](../../administration-and-setup/add-users/configure-and-grant-access/grant-access-other-users.md).

   ![](assets/tag-users-in-update.png)

1. (Optional) To make the update private, enable **Private to my company** in the lower-right corner of the update box. This makes the update visible just to users in your company. The **Private to my company** option is available only when a Company is specified in your Workfront profile. 

   >[!NOTE]
   >
   >Tagged users outside the company could still receive an in-app notification or email, even though they will not see the private comments on the Updates tab. We recommend not to tag external users on an update if you do not want to share the information with them.  

1. (Optional) To add multiple users and teams, repeat step 2.

   >[!NOTE]
   >
   >All users and team members listed in the Notify field receive an in-app notification for the update and might receive an email, depending on the configuration of their email notification settings. Users who tag themselves in a comment or reply receive a notification for that comment or reply and can see their name in the Notify field for the remainder of the thread, but they do not receive another notification unless they tag themselves again. For more information, see [Modify your own email notifications](../../workfront-basics/using-notifications/activate-or-deactivate-your-own-event-notifications.md) and [Configure event notifications for everyone in the system](../../administration-and-setup/manage-workfront/emails/configure-event-notifications-for-everyone-in-the-system.md).

1. Click **Update**.  
   Users included in the update are automatically granted View permission to the object and can view and respond to updates made to the object.

   You can see who has been tagged in each reply at the top of the update thread. These users, along with any users subscribed to the object, receive a notification whenever an update or reply is made on the object.

   ![](assets/tagging-transparency-350x192.png)
-->

작업 항목을 업데이트할 때 사용할 수 있는 추가 기능에 대한 자세한 내용은 [작업 업데이트](../../workfront-basics/updating-work-items-and-viewing-updates/update-work.md).



