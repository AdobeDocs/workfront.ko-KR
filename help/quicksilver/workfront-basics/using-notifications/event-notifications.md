---
content-type: overview
navigation-topic: notifications
title: 이벤트 알림
description: 이벤트 알림은 프로젝트, 작업 또는 문제와 같은 개체에서 다양한 유형의 이벤트에 의해 트리거되는 이메일입니다. 프로젝트에서 다른 사람이 알고 있어야 하는 상황이 발생하면 전송됩니다. 이벤트에 따라 사용자는 인스턴트, 일별 또는 인스턴트 및 일별 이메일 알림을 받을 수 있습니다.
author: Lisa
feature: Get Started with Workfront
exl-id: 09b70427-691d-437a-b9d2-86f78bd4d6a2
source-git-commit: f3ba39e02d690dd3a0d50ecdb22af0c12a3d4ffb
workflow-type: tm+mt
source-wordcount: '555'
ht-degree: 0%

---

# 이벤트 알림

이벤트 알림은 프로젝트, 작업 또는 문제와 같은 개체에서 다양한 유형의 이벤트에 의해 트리거되는 이메일입니다. 프로젝트에서 다른 사람이 알고 있어야 하는 상황이 발생하면 전송됩니다. 이벤트에 따라 사용자는 인스턴트, 일별 또는 인스턴트 및 일별 이메일 알림을 받을 수 있습니다.

>[!NOTE]
>
>이벤트 알림은 몇 가지 유형 중 하나입니다 [!DNL Adobe Workfront] 알림. 모든 항목에 대한 정보 [!DNL Workfront] 알림 유형, 자세한 내용은 [[!DNL Adobe Workfront] 알림](../../workfront-basics/using-notifications/wf-notifications.md).

## 이벤트 알림 구성

아래 나열된 다음 수준에서 이벤트 알림 이메일을 구성할 수 있습니다. 이벤트 알림의 구성은 이벤트 알림을 활성화하거나 비활성화하는 것으로 구성됩니다.

* **시스템 수준**: A [!DNL Workfront] 관리자는 다음에 설명된 대로 시스템 수준에서 이벤트 알림을 활성화하고 비활성화할 수 있습니다. [시스템의 모든 사용자에 대한 이벤트 알림을 구성합니다](../../administration-and-setup/manage-workfront/emails/configure-event-notifications-for-everyone-in-the-system.md).

   모든 그룹은 기본적으로 시스템 알림을 상속하지만 그룹 관리자는 그룹 수준에서 허용되는 경우 일부 구성을 변경할 수 있습니다 [!DNL Workfront] 아래의 다음 글머리 기호 항목에 설명된 대로 관리자.

* **그룹 수준**: 그룹 관리자는 그룹 이후에 관리하는 그룹에 대한 이벤트 알림을 구성할 수 있습니다 [!DNL Workfront] 관리자는 그룹에 대해 이 기능을 잠금 해제합니다. 관리하는 그룹 위에 그룹이 있으면 해당 관리자가 사용자 그룹을 위해 이 작업을 수행할 수도 있습니다. 같은 것이 [!DNL Workfront] 관리자(그룹에 대해) 자세한 내용은 [그룹에 대한 이벤트 알림 보기 및 구성](../../administration-and-setup/manage-groups/create-and-manage-groups/view-and-configure-event-notifications-group.md).

   >[!NOTE]
   >
   >이 기능은 처음에 단계적 롤아웃의 일부로 클러스터 4의 고객에게만 제공됩니다. 곧 다른 클러스터에 사용할 수 있게 됩니다. 이 경우 이 문서가 업데이트됩니다.

* **사용자 수준**: 시스템 전체에 활성화된 모든 이벤트 알림은 각 사용자의 [!UICONTROL 알림 을 참조하십시오] 개별 프로필에 대한 섹션을 참조하십시오. 사용자는 여기에서 개별 이벤트 알림을 활성화하고 비활성화할 수 있습니다.

   [!DNL Workfront] 다른 사용자를 편집할 수 있는 액세스 권한이 있는 관리자 및 사용자는 개별 사용자의 프로필에서 알림을 활성화하고 비활성화할 수도 있습니다.

   자세한 내용은 [고유한 이벤트 알림 활성화 또는 비활성화](../../workfront-basics/using-notifications/activate-or-deactivate-your-own-event-notifications.md).

   >[!NOTE]
   >
   >사용자 수준 알림에는 다음이 포함됩니다 [!DNL Workfront Goals] 알림. 하지만, [!DNL Workfront] 관리자 또는 그룹 관리자가 알림을 구성할 수 없습니다 [!DNL Workfront Goals]. 각 사용자는 자체 구성을 수행해야 합니다 [!DNL Workfront Goals] 프로필의 알림입니다. 사용자를 편집할 수 있는 액세스 권한이 있는 경우에는 다른 사용자에 대해 이러한 알림을 수정할 수도 있습니다. 활성화 [!DNL Workfront Goals] 프로필 또는 편집할 수 있는 액세스 권한이 있는 다른 사용자에 대한 알림은 [알림: 목표](../../workfront-basics/using-notifications/notifications-goals.md).

   다음 알림에 대한 자세한 정보 [!DNL Workfront] 관리자가 구성할 수 있습니다. 자세한 내용은 [시스템의 모든 사용자에 대한 이벤트 알림을 구성합니다](../../administration-and-setup/manage-workfront/emails/configure-event-notifications-for-everyone-in-the-system.md). [!DNL Workfront Goals] 새 버전에서만 사용 가능 [!DNL Adobe Workfront] 경험으로 제어됩니다.

## 이벤트 알림 콘텐츠

이벤트 알림 이메일에는 발생한 이벤트에 대한 정보가 포함되며 연결되는 링크가 포함되어 있습니다 [!DNL Workfront] 시스템에서 이벤트를 볼 수 있는 위치입니다. 이메일 알림 수신에 대한 자세한 내용은 [[!DNL Adobe Workfront] 알림](../../workfront-basics/using-notifications/wf-notifications.md).

A [!DNL Workfront] 관리자는 전자 메일 알림의 내용을 변경할 수 없습니다. 전자 메일 알림은 [!DNL Workfront]. 하지만 이벤트 알림 이메일의 제목란을 변경할 수 있습니다. 자세한 내용은 [이벤트 알림에 대한 이메일 주체 사용자 정의](../../administration-and-setup/manage-workfront/emails/custom-email-subjects-event-notification.md).

목록 [!DNL Workfront] 각 이벤트에 대한 간단한 설명과 함께 이벤트 알림이 기본적으로 활성 상태인지 아니면 비활성 상태인지를 참조하십시오. [에서 사용할 수 있는 이벤트 알림 [!DNL Adobe Workfront]](../../administration-and-setup/manage-workfront/emails/event-notifications-available-in-wf.md).
