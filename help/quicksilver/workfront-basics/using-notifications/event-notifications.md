---
content-type: overview
navigation-topic: notifications
title: 이벤트 알림
description: 이벤트 알림은 프로젝트, 작업 또는 문제와 같은 개체에 대한 다양한 유형의 이벤트에 의해 트리거되는 이메일입니다. 프로젝트에서 다른 사용자가 알아야 하는 사항이 발생하면 전송됩니다. 이벤트에 따라 사용자는 인스턴트, 매일 또는 인스턴트 및 일별 이메일 알림을 모두 받습니다.
author: Courtney
feature: Get Started with Workfront
exl-id: 09b70427-691d-437a-b9d2-86f78bd4d6a2
source-git-commit: c79d030ff2d05487e5f7e3457bf98df591822a80
workflow-type: tm+mt
source-wordcount: '486'
ht-degree: 0%

---

# 이벤트 알림

<!-- Audited: 4/2025 -->

이벤트 알림은 프로젝트, 작업 또는 문제와 같은 개체에 대한 다양한 유형의 이벤트에 의해 트리거되는 이메일입니다. 프로젝트에서 다른 사용자가 알아야 하는 사항이 발생하면 전송됩니다. 이벤트에 따라 사용자는 인스턴트, 매일 또는 인스턴트 및 일별 이메일 알림을 모두 받습니다.

>[!NOTE]
>
>이벤트 알림은 여러 유형의 [!DNL Adobe Workfront] 알림 중 하나입니다. 모든 [!DNL Workfront] 알림 유형에 대한 자세한 내용은 [알림 개요](../../workfront-basics/using-notifications/wf-notifications.md)를 참조하십시오.

## 이벤트 알림 구성

이벤트 알림 이메일은 다음 수준에서 구성할 수 있습니다.

* **시스템 수준**: [시스템의 모든 사용자를 위한 이벤트 알림 구성](../../administration-and-setup/manage-workfront/emails/configure-event-notifications-for-everyone-in-the-system.md)에 설명된 대로 [!DNL Workfront] 관리자는 시스템 수준에서 이벤트 알림을 활성화하거나 비활성화할 수 있습니다.

  모든 그룹은 기본적으로 시스템 알림을 상속하지만 [!DNL Workfront] 관리자가 허용한 경우 그룹 관리자가 그룹 수준에서 일부 구성을 변경할 수 있습니다.

* **그룹 수준**: [!DNL Workfront] 관리자가 그룹에 대한 이 기능을 잠금 해제한 후 그룹 관리자가 자신이 관리하는 그룹에 대한 이벤트 알림을 구성할 수 있습니다. 관리하는 그룹 위에 그룹이 있는 경우 해당 관리자는 해당 그룹에 대해 이 작업을 수행할 수도 있습니다. [!DNL Workfront] 관리자(모든 그룹)의 경우도 마찬가지입니다. 자세한 내용은 [그룹에 대한 이벤트 알림 보기 및 구성](../../administration-and-setup/manage-groups/create-and-manage-groups/view-and-configure-event-notifications-group.md)을 참조하세요.

* **사용자 수준**: 시스템 전체에서 활성화된 모든 이벤트 알림은 개별 프로필에서 각 사용자의 [!UICONTROL 알림] 섹션에 나열됩니다. 사용자는 여기에서 개별 이벤트 알림을 활성화 및 비활성화할 수 있습니다.

  [!DNL Workfront] 관리자와 다른 사용자를 편집할 수 있는 액세스 권한이 있는 사용자는 개별 사용자의 프로필에서 알림을 활성화하거나 비활성화할 수도 있습니다.

  자세한 내용은 [전자 메일 알림 수정](../../workfront-basics/using-notifications/activate-or-deactivate-your-own-event-notifications.md)을 참조하세요.

  >[!NOTE]
  >
  >사용자 수준 알림에는 [!DNL Workfront Goals]개의 알림도 포함됩니다. 그러나 [!DNL Workfront] 관리자 또는 그룹 관리자가 [!DNL Workfront Goals]에 대한 알림을 구성할 수 없습니다. 각 사용자는 프로필에서 자신의 [!DNL Workfront Goals] 알림을 구성해야 합니다. 사용자 편집 액세스 권한이 있는 경우 다른 사용자에 대해 이러한 알림을 수정할 수도 있습니다. 프로필 또는 편집할 수 있는 액세스 권한이 있는 다른 사용자에 대해 [!DNL Workfront Goals] 알림을 사용하려면 [알림: 목표](../../workfront-basics/using-notifications/notifications-goals.md)를 참조하세요.

  [!DNL Workfront] 관리자가 구성할 수 있는 알림에 대한 자세한 내용은 [시스템의 모든 사용자를 위한 이벤트 알림 구성](../../administration-and-setup/manage-workfront/emails/configure-event-notifications-for-everyone-in-the-system.md)을 참조하십시오.

## 이벤트 알림 콘텐츠

이벤트 알림 이메일에는 발생한 이벤트에 대한 정보가 포함되어 있으며 시스템에서 이벤트를 볼 수 있는 [!DNL Workfront]에 대한 링크가 포함되어 있습니다. 전자 메일 알림 수신에 대한 자세한 내용은 [알림 개요](../../workfront-basics/using-notifications/wf-notifications.md)를 참조하세요.

[!DNL Workfront] 관리자는 전자 메일 알림 콘텐츠를 [!DNL Workfront]에서 구성한 대로 변경할 수 없지만 이벤트 알림 전자 메일 제목 줄은 변경할 수 있습니다. 자세한 내용은 [이벤트 알림에 대한 전자 메일 제목 사용자 지정](../../administration-and-setup/manage-workfront/emails/custom-email-subjects-event-notification.md)을 참조하십시오.

모든 [!DNL Workfront] 이벤트 알림 목록과 각 이벤트에 대한 간략한 설명 및 기본적으로 활성 상태인지 비활성 상태인지에 대해서는 [이벤트 알림 유형](../../administration-and-setup/manage-workfront/emails/event-notifications-available-in-wf.md)을 참조하십시오.
