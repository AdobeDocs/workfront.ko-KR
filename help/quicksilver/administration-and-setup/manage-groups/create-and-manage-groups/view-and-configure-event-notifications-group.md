---
user-type: administrator
product-area: system-administration;user-management
keywords: 보기,그룹,이벤트,알림,구성,활성화,비활성화
navigation-topic: create-and-manage-groups
title: 그룹에 대한 이벤트 알림 보기 및 구성
description: 그룹 관리자는 관리하는 그룹에 대해 활성화된 이벤트 알림을 볼 수 있습니다. 또한 Adobe Workfront 관리자가 이벤트 알림의 잠금을 해제하는 경우 관리하는 최상위 그룹에 대해 이벤트 알림을 구성할 수 있습니다. 이벤트 알림의 구성은 활성화 또는 비활성화로 구성됩니다.
author: Lisa
feature: System Setup and Administration, People Teams and Groups
role: Admin
exl-id: a815aeb1-3403-4491-a8ad-7e47c519905c
source-git-commit: afbf2e2fbfcc2c527223da008518bc7632872c23
workflow-type: tm+mt
source-wordcount: '558'
ht-degree: 0%

---

# 그룹에 대한 이벤트 알림 보기 및 구성

그룹 관리자는 관리하는 그룹에 대해 활성화된 이벤트 알림을 볼 수 있습니다.

또한 Adobe Workfront 관리자가 이벤트 알림의 잠금을 해제하는 경우 관리하는 최상위 그룹에 대해 이벤트 알림을 구성할 수 있습니다. 이벤트 알림의 구성은 활성화 또는 비활성화로 구성됩니다.

Workfront 관리자는 모든 그룹에 대해 이 작업을 수행할 수도 있습니다.

그룹에 대한 이벤트 알림 구성은 해당 그룹 또는 하위 그룹 중 하나가 홈 그룹인 사용자에게 영향을 줍니다. 이러한 사용자는 사용자 프로필에서 시스템 전체에서 활성화된 이벤트 알림 대신 홈 그룹에 대해 활성화된 이벤트 알림을 보게 됩니다.

Workfront 관리자가 이벤트 알림을 잠금 해제하는 방법에 대한 자세한 내용은 [모든 그룹에 대한 이벤트 알림 구성 잠금 해제 또는 잠금](../../../administration-and-setup/manage-workfront/emails/unlock-configuration-of-event-notifications-for-groups.md)을 참조하십시오.

이벤트의 기본 알림 설정에 대한 자세한 내용은 [이벤트 알림 유형](../../../administration-and-setup/manage-workfront/emails/event-notifications-available-in-wf.md)을 참조하세요.

## 액세스 요구 사항

이 문서의 단계를 수행하려면 다음이 있어야 합니다.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Workfront 플랜*</td> 
   <td> <p>임의</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront 라이센스*</td> 
   <td> <p>플랜 </p> <p>그룹의 그룹 관리자 또는 Workfront 관리자여야 합니다. 자세한 내용은 <a href="../../../administration-and-setup/manage-groups/group-roles/group-administrators.md" class="MCXref xref">그룹 관리자</a> 및 <a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-a-user-full-administrative-access.md" class="MCXref xref">사용자에게 전체 관리 액세스 권한 부여</a>를 참조하십시오.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;보유 중인 플랜 또는 라이선스 유형을 확인해야 하는 경우 Workfront 관리자에게 문의하십시오.

## 그룹의 이벤트 알림 보기 및 구성

1. (조건부 및 선택 사항) Workfront 관리자이고 이미 이메일 알림 페이지(설정 > 이메일 > 알림)에 있는 경우 다음을 수행한 다음 6단계로 건너뛸 수 있습니다. 목록 위의 상자에서 **시스템 이벤트 알림**&#x200B;을 삭제하고 상자에 그룹 이름을 입력한 다음 표시될 때 클릭합니다.
1. Adobe Workfront 오른쪽 상단의 **기본 메뉴** 아이콘 ![](assets/main-menu-icon.png)을(를) 클릭한 다음 **설정** ![](assets/gear-icon-settings.png)을(를) 클릭합니다.

1. 왼쪽 패널에서 **그룹** ![](assets/groups-icon.png)을(를) 클릭합니다.

1. 최상위 그룹의 이름을 클릭합니다.
1. 왼쪽 메뉴에서 **이벤트 알림**&#x200B;을 클릭합니다.

   표시되는 목록에서 왼쪽의 **활성** 열은 그룹에 대해 활성(파란색) 및 비활성(회색)인 알림을 표시합니다.

1. 잠금 해제된 이벤트 알림을 활성화하거나 비활성화하려면 <strong>활성</strong> 열의 버튼을 클릭하여 활성화하십시오 <img src="assets/email-notification-enabled-unlocked.png"> 또는 비활성화 <img src="assets/email-notification-disabled-unlocked.png">.

   >[!INFO]
   >
   >**예:** 그룹에 대해 잠금 해제된 아래 표시된 상위 2개의 마케팅 그룹 이벤트 알림을 구성할 수 있습니다.</p> <p> <img src="assets/configure-group-event-notifications.png">
   >* <strong>활성</strong> 열의 단추가 회색으로 흐리게 표시되어 있는 경우 <img src="assets/email-notification-disabled-locked.png">, 모든 사용자에 대해 이벤트 알림이 비활성화되어 있으며 그룹 관리자가 이를 활성화하거나 이메일 제목을 편집할 수 없습니다.
   >* <strong>활성</strong> 열의 단추가 회색으로 흐리게 표시되지 않는 경우 <img src="assets/email-notification-disabled-unlocked.png">, 이벤트 알림이 모든 사용자에 대해 <strong>비활성화되어 있으며</strong> 그룹 관리자가 해당 그룹에 대해 활성화할 수 있습니다.
   >* <strong>활성</strong> 열의 단추가 파란색으로 흐리게 표시되어 있는 경우 <img src="assets/email-notification-enabled-locked.png">, 모든 사용자에 대해 이벤트 알림이 활성화되었으며 그룹 관리자는 이를 비활성화하거나 그룹의 이메일 제목 줄을 편집할 수 없습니다.
   >* <strong>활성</strong> 열의 단추가 파란색이고 흐리게 표시되지 않는 경우 <img src="assets/email-notification-enabled-unlocked.png">, 이벤트 알림이 모든 사용자에 대해 <strong>활성화되었으며</strong> 그룹 관리자는 해당 그룹에 대해 비활성화할 수 있습니다.

<!--
This step (with substeps) is for functionality from a Sprint 3 2021 story that got put on hold. Also see the PDF on the story for some text earlier in the article that needs to be added. 

1. To customize the email subject line of an event notification,
  1. Click the name of the event notification.
  1. In the <strong>Event Notification</strong> box that displays, in the <strong>Email Subject Line</strong> box, change the text and fields, including custom fields, then click <strong>Update</strong> to save the new subject lines for your emails.
  IMPORTANT: The names of the fields added must match the camel case syntax of our database structure. For more information about how our objects and their fields are named in the Workfront database, see the <a href="../../../wf-api/workfront-api.md" class="MCXref xref">Adobe Workfront API</a>.
  For more information about customizing the email subject line of an event notification, see <a href="../../../administration-and-setup/manage-workfront/emails/custom-email-subjects-event-notification.md" class="MCXref xref">Customize email subjects for event notifications</a>. 
-->

