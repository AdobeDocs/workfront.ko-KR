---
title: 시스템의 모든 사용자에 대한 이벤트 알림을 구성합니다
description: 이벤트 알림은 특정 이벤트가 발생할 때 사용자에게 이메일을 트리거합니다. 계획자 액세스 레벨을 가진 Adobe Workfront 관리자나 사용자는 시스템의 모든 사용자에 대한 이벤트 통지를 구성할 수 있습니다. 이벤트 알림의 구성은 이벤트 알림을 활성화하거나 비활성화하는 것으로 구성됩니다.
author: Caroline, Lisa
feature: System Setup and Administration
role: Admin
exl-id: 027ecebd-d9de-4cdd-b15a-88de18367591
source-git-commit: 730932f6c8d4658273dd943e464a038828d288e9
workflow-type: tm+mt
source-wordcount: '604'
ht-degree: 0%

---

# 시스템의 모든 사용자에 대한 이벤트 알림을 구성합니다

<!--DON'T DELETE, DRAFT OR HIDE THIS ARTICLE. IT IS LINKED TO THE PRODUCT, THROUGH THE CONTEXT SENSITIVE HELP LINKS-->

이벤트 알림은 특정 이벤트가 발생할 때 사용자에게 이메일을 트리거합니다. 계획자 액세스 레벨을 가진 Adobe Workfront 관리자나 사용자는 시스템의 모든 사용자에 대한 이벤트 통지를 구성할 수 있습니다. 이벤트 알림의 구성은 이벤트 알림을 활성화하거나 비활성화하는 것으로 구성됩니다.

<!--Alina annotation on the word "all" in 2nd sentence: abive, drafted and remains QS only-->

활성화한 이벤트와 사용자가 자신의 프로필에 대해 계속 활성화하면 이벤트가 발생할 때 인스턴트, 일별 또는 인스턴트 및 일별 이메일 알림을 받게 됩니다.

먼저 Workfront 인스턴스의 설정 영역에서 모든 사용자가 받을 알림을 지정해야 합니다. 설정 영역에서 알림을 활성화하면 프로필 페이지에서 각 사용자에 대해 활성화됨으로 표시됩니다.

알림이 설정 영역에서 활성화되고 사용자의 프로필 페이지에 표시되면 개별 사용자 또는 계획 라이센스가 있는 다른 사용자가 사용자 프로필에서 활성화된 알림을 구성하여 특정 사용자가 받는 알림과 빈도를 제어할 수도 있습니다. 자세한 내용은 [고유한 이벤트 알림 활성화 또는 비활성화](../../../workfront-basics/using-notifications/activate-or-deactivate-your-own-event-notifications.md).

활성화 및 비활성화할 수 있는 모든 이벤트 알림 목록은 다음을 참조하십시오 [Adobe Workfront에서 사용할 수 있는 이벤트 알림](../../../administration-and-setup/manage-workfront/emails/event-notifications-available-in-wf.md).

그룹 관리자가 그룹에 대해 구성할 수 있도록 이벤트 알림 잠금을 해제하는 방법에 대한 내용은 [모든 그룹에 대한 이벤트 알림 구성 잠금 해제 또는 잠금](../../../administration-and-setup/manage-workfront/emails/unlock-configuration-of-event-notifications-for-groups.md) 및 [그룹에 대한 이벤트 알림 보기 및 구성](../../../administration-and-setup/manage-groups/create-and-manage-groups/view-and-configure-event-notifications-group.md).

## 액세스 요구 사항

이 문서의 절차를 수행하려면 다음 액세스 권한이 있어야 합니다.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront 플랜*</td> 
   <td>모든</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront 라이선스*</td> 
   <td>플랜</td> 
  </tr> 
  <tr> 
   <td role="rowheader">액세스 수준 구성*</td> 
   <td> <p>미리 알림 알림에 대한 관리자 액세스 권한이 있는 계획자 이상</p> <p>계획 사용자 관리 액세스 권한을 제공하는 방법에 대한 자세한 내용은 <a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-users-admin-access-certain-areas.md" class="MCXref xref">특정 영역에 대한 관리자 액세스 권한 부여</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;어떤 계획, 라이선스 유형 또는 액세스 권한을 보유하고 있는지 알아보려면 Workfront 관리자에게 문의하십시오.

## 모든 사용자에 대한 이벤트 알림 구성

사용자가 프로필에서 알림을 활성화하거나 비활성화하려면 먼저 Workfront의 설정 영역에서 알림을 활성화해야 합니다.

>[!TIP]
>
>설정 영역에서 Workfront 목표에 대한 알림을 활성화할 수 없습니다. 사용자는 프로필에서만 이러한 알림을 활성화할 수 있습니다. 계획 라이센스가 있는 사용자는 다른 사용자에 대해 활성화할 수 있습니다. 사용자를 위한 Workfront 목표 알림 활성화에 대한 자세한 내용은 [알림: 목표](../../../workfront-basics/using-notifications/notifications-goals.md).

1. 을(를) 클릭합니다. **기본 메뉴** 아이콘 ![](assets/main-menu-icon.png) Adobe Workfront의 오른쪽 위 모서리에서 을(를) 클릭하고 **설정** ![](assets/gear-icon-settings.png).

1. 클릭 **이메일** > **알림 을 참조하십시오**.

1. 다음을 확인합니다. **이벤트 알림** 탭이 열려 있습니다.
1. 이벤트 이름의 왼쪽에 있는 스위치를 클릭하여 켜거나 끕니다.

   이벤트에 대한 기본 알림 상태를 보려면 [이벤트 알림](../../../workfront-basics/using-notifications/event-notifications.md).

1. (선택 사항) 이벤트 알림의 이름을 클릭하여 이메일 알림의 제목란을 사용자 지정합니다.

   이메일 알림의 제목란 사용자 지정에 대한 자세한 내용은 다음을 참조하십시오 [이벤트 알림에 대한 이메일 주체 사용자 정의](../../../administration-and-setup/manage-workfront/emails/custom-email-subjects-event-notification.md).

1. (선택 사항) 그룹 관리자가 그룹에 대해 별도로 구성할 수 있도록 전자 메일 알림에 대한 구성을 잠금 해제하려면 버튼을 클릭합니다 ![](assets/lock-toggle-button.png) 알림 오른쪽으로 전환하여 잠금 해제된 위치로 전환합니다. ![](assets/unlock-toggle-button.png).

   >[!NOTE]
   >
   >이 기능은 처음에 단계적 롤아웃의 일부로 클러스터 4의 고객에게만 제공됩니다. 곧 다른 클러스터에 사용할 수 있게 됩니다. 이 경우 이 문서가 업데이트됩니다.

   자세한 내용은 [모든 그룹에 대한 이벤트 알림 구성 잠금 해제 또는 잠금](../../../administration-and-setup/manage-workfront/emails/unlock-configuration-of-event-notifications-for-groups.md).
