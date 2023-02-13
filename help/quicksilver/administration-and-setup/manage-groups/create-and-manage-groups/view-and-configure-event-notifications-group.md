---
user-type: administrator
product-area: system-administration;user-management
keywords: 보기,그룹,이벤트,알림,구성,활성화,비활성화
navigation-topic: create-and-manage-groups
title: 그룹에 대한 이벤트 알림 보기 및 구성
description: 그룹 관리자는 관리하는 그룹에 대해 활성화된 이벤트 알림을 볼 수 있습니다. 또한 Adobe Workfront 관리자가 이벤트 알림을 잠금 해제하는 경우 관리하는 최상위 그룹에 대해 구성할 수 있습니다. 이벤트 알림의 구성은 이벤트 알림을 활성화하거나 비활성화하는 것으로 구성됩니다.
author: Caroline
feature: System Setup and Administration, People Teams and Groups
role: Admin
exl-id: a815aeb1-3403-4491-a8ad-7e47c519905c
source-git-commit: 306d6493ff0413d5814f4aed8ab44fb897f3568d
workflow-type: tm+mt
source-wordcount: '592'
ht-degree: 0%

---

# 그룹에 대한 이벤트 알림 보기 및 구성

그룹 관리자는 관리하는 그룹에 대해 활성화된 이벤트 알림을 볼 수 있습니다.

또한 Adobe Workfront 관리자가 이벤트 알림을 잠금 해제하는 경우 관리하는 최상위 그룹에 대해 구성할 수 있습니다. 이벤트 알림의 구성은 이벤트 알림을 활성화하거나 비활성화하는 것으로 구성됩니다.

Workfront 관리자는 모든 그룹에 대해서도 이 작업을 수행할 수 있습니다.

그룹에 대한 이벤트 알림을 구성하는 것은 해당 그룹 또는 해당 하위 그룹 중 하나가 홈 그룹인 사용자에게 영향을 줍니다. 사용자 프로필에서는 시스템 전체에 활성화된 이벤트 알림 대신 홈 그룹에 대해 활성화된 이벤트 알림이 표시됩니다.

Workfront 관리자가 이벤트 알림 잠금을 해제하는 방법에 대한 자세한 내용은 [모든 그룹에 대한 이벤트 알림 구성 잠금 해제 또는 잠금](../../../administration-and-setup/manage-workfront/emails/unlock-configuration-of-event-notifications-for-groups.md).

이벤트의 기본 알림 설정에 대한 자세한 내용은 [Adobe Workfront에서 사용할 수 있는 이벤트 알림](../../../administration-and-setup/manage-workfront/emails/event-notifications-available-in-wf.md).

## 액세스 요구 사항

이 문서의 절차를 수행하려면 다음 사항이 있어야 합니다.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"><a href="https://www.workfront.com/plans" target="_blank">Workfront 플랜</a>*</td> 
   <td> <p>Pro 이상</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><a href="https://one.workfront.com/s/document-item?bundleId=the-new-workfront-experience&amp;topicId=Content%2FAdministration_and_Setup%2FAdd_users%2FAccess_levels_and_object_permissions%2Fwf-licenses.html&amp;_LANG=en" target="_blank">Adobe Workfront 라이선스</a>*</td> 
   <td> <p>플랜 </p> <p>그룹의 그룹 관리자 또는 Workfront 관리자여야 합니다. 자세한 내용은 <a href="../../../administration-and-setup/manage-groups/group-roles/group-administrators.md" class="MCXref xref">그룹 관리자</a> 및 <a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-a-user-full-administrative-access.md" class="MCXref xref">사용자에게 전체 관리자 액세스 권한 부여</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;보유하고 있는 플랜 또는 라이선스 유형을 찾아야 하는 경우 Workfront 관리자에게 문의하십시오.

## 그룹의 이벤트 알림 보기 및 구성

1. (조건부 및 선택 사항) Workfront 관리자이며 이미 이메일 알림 페이지(설정 > 이메일 > 알림)에 있는 경우 다음을 수행한 다음 6단계로 건너뛸 수 있습니다. 삭제 **시스템 이벤트 알림** 목록 위의 상자에서 상자에 그룹 이름을 입력한 다음 그룹 이름이 나타나면 클릭합니다.
1. 을(를) 클릭합니다. **기본 메뉴** 아이콘 ![](assets/main-menu-icon.png) Adobe Workfront의 오른쪽 위 모서리에서 을(를) 클릭하고 **설정** ![](assets/gear-icon-settings.png).

1. 왼쪽 패널에서 **그룹** ![](assets/groups-icon.png).

1. 최상위 수준 그룹의 이름을 클릭합니다.
1. 왼쪽 메뉴에서 **이벤트 알림**.

   표시되는 목록에서 **활성** 왼쪽의 열에는 그룹에 대해 활성(파란색) 및 비활성(회색)이 표시됩니다.

1. 잠금 해제된 이벤트 알림을 활성화하거나 비활성화하려면: 에서 버튼을 클릭합니다. <strong>활성</strong> 활성화할 열 <img src="assets/email-notification-enabled-unlocked.png"> 또는 비활성화 <img src="assets/email-notification-disabled-unlocked.png"> 그래

   >[!INFO]
   >
   >**예:** 아래에 표시된 그룹 잠금이 해제된 두 개의 마케팅 그룹 이벤트 알림을 구성할 수 있습니다.</p> <p> <img src="assets/configure-group-event-notifications.png">
   >* 버튼은 <strong>활성</strong> 열은 회색으로 표시되며 흐리게 표시됩니다 <img src="assets/email-notification-disabled-locked.png">, 모든 사용자 및 그룹 관리자가 이벤트 알림을 활성화하거나 이메일 제목 줄을 편집할 수 없는 경우 이벤트 알림이 비활성화됩니다
   >* 버튼은 <strong>활성</strong> 열은 회색으로 표시되며 흐리게 표시되지 않습니다 <img src="assets/email-notification-disabled-unlocked.png">로 설정되면 이벤트 알림이 <strong>모든 사용자에 대해 비활성화되고</strong> 그룹 관리자는 그룹에 대해 활성화할 수 있습니다.
   >* 버튼은 <strong>활성</strong> 열은 파란색으로 표시되며 흐리게 표시됩니다 <img src="assets/email-notification-enabled-locked.png">이벤트 알림이 모든 사용자 및 그룹 관리자에 대해 활성화되면 이벤트 알림을 비활성화하거나 해당 그룹의 이메일 제목 줄을 편집할 수 없습니다.
   >* 버튼은 <strong>활성</strong> 열은 파란색이며 흐리게 표시되지 않습니다 <img src="assets/email-notification-enabled-unlocked.png">로 설정되면 이벤트 알림이 <strong>모든 사용자에 대해 활성화됨</strong> 그룹 관리자는 그룹에 대해 비활성화할 수 있습니다.


<!--
This step (with substeps) is for functionality from a Sprint 3 2021 story that got put on hold. Also see the PDF on the story for some text earlier in the article that needs to be added. 

1. To customize the email subject line of an event notification,
  1. Click the name of the event notification.
  1. In the <strong>Event Notification</strong> box that displays, in the <strong>Email Subject Line</strong> box, change the text and fields, including custom fields, then click <strong>Update</strong> to save the new subject lines for your emails.
  IMPORTANT: The names of the fields added must match the camel case syntax of our database structure. For more information about how our objects and their fields are named in the Workfront database, see the <a href="../../../wf-api/workfront-api.md" class="MCXref xref">Adobe Workfront API</a>.
  For more information about customizing the email subject line of an event notification, see <a href="../../../administration-and-setup/manage-workfront/emails/custom-email-subjects-event-notification.md" class="MCXref xref">Customize email subjects for event notifications</a>. 
-->

