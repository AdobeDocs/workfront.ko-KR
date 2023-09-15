---
content-type: overview
navigation-topic: notifications
title: 이벤트 알림
description: 이벤트 알림은 프로젝트, 작업 또는 문제와 같은 개체에 대한 다양한 유형의 이벤트에 의해 트리거되는 이메일입니다. 프로젝트에서 다른 사용자가 알아야 하는 사항이 발생하면 전송됩니다. 이벤트에 따라 사용자는 인스턴트, 매일 또는 인스턴트 및 일별 이메일 알림을 모두 받습니다.
author: Lisa
feature: Get Started with Workfront
exl-id: 09b70427-691d-437a-b9d2-86f78bd4d6a2
source-git-commit: f6335f4e94d286681adfb50165562b2c41b5acac
workflow-type: tm+mt
source-wordcount: '553'
ht-degree: 0%

---

# 이벤트 알림

이벤트 알림은 프로젝트, 작업 또는 문제와 같은 개체에 대한 다양한 유형의 이벤트에 의해 트리거되는 이메일입니다. 프로젝트에서 다른 사용자가 알아야 하는 사항이 발생하면 전송됩니다. 이벤트에 따라 사용자는 인스턴트, 매일 또는 인스턴트 및 일별 이메일 알림을 모두 받습니다.

>[!NOTE]
>
>이벤트 알림은 다음과 같은 여러 유형 중 하나입니다. [!DNL Adobe Workfront] 알림입니다. 모든 항목에 대한 정보 [!DNL Workfront] 알림 유형, 참조 [[!DNL Adobe Workfront] 알림](../../workfront-basics/using-notifications/wf-notifications.md).

## 이벤트 알림 구성

이벤트 알림 이메일은 아래 나열된 다음 수준에서 구성할 수 있습니다. 이벤트 알림의 구성은 활성화 또는 비활성화로 구성됩니다.

* **시스템 수준**: A [!DNL Workfront] 에 설명된 대로 관리자는 시스템 수준에서 이벤트 알림을 활성화하고 비활성화할 수 있습니다. [시스템의 모든 사용자를 위한 이벤트 알림 구성](../../administration-and-setup/manage-workfront/emails/configure-event-notifications-for-everyone-in-the-system.md).

  모든 그룹은 기본적으로 시스템 알림을 상속하지만, 그룹 관리자가 허용한 경우 그룹 수준에서 일부 구성을 변경할 수 있습니다. [!DNL Workfront] 관리자: 아래 다음 글머리 기호 항목에 설명되어 있습니다.

* **그룹 수준**: 그룹 관리자는 다음 작업 후에 자신이 관리하는 그룹에 대한 이벤트 알림을 구성할 수 있습니다. [!DNL Workfront] 관리자가 그룹에 대해 이 기능의 잠금을 해제합니다. 관리하는 그룹 위에 그룹이 있는 경우 해당 관리자는 해당 그룹에 대해 이 작업을 수행할 수도 있습니다. 에 대해서도 마찬가지입니다 [!DNL Workfront] 관리자(모든 그룹의 경우). 자세한 내용은 [그룹에 대한 이벤트 알림 보기 및 구성](../../administration-and-setup/manage-groups/create-and-manage-groups/view-and-configure-event-notifications-group.md).

  >[!NOTE]
  >
  >이 기능은 처음에는 단계적 롤아웃의 일부로 클러스터 4의 고객만 사용할 수 있습니다. 곧 다른 클러스터에서 사용할 수 있게 됩니다. 이 문서는 이에 따라 업데이트됩니다.

* **사용자 수준**: 시스템 전체에서 활성화된 모든 이벤트 알림이 각 사용자의 [!UICONTROL 알림] 섹션에 있는 섹션을 참조하십시오. 사용자는 여기에서 개별 이벤트 알림을 활성화 및 비활성화할 수 있습니다.

  [!DNL Workfront] 관리자 및 다른 사용자를 편집할 수 있는 액세스 권한이 있는 사용자는 개별 사용자의 프로필에서 알림을 활성화 및 비활성화할 수도 있습니다.

  자세한 내용은 [이메일 알림 수정](../../workfront-basics/using-notifications/activate-or-deactivate-your-own-event-notifications.md).

  >[!NOTE]
  >
  >사용자 수준 알림에는 다음도 포함됩니다 [!DNL Workfront Goals] 알림입니다. 그러나 [!DNL Workfront] 관리자 또는 그룹 관리자가 다음에 대한 알림을 구성할 수 없음: [!DNL Workfront Goals]. 각 사용은 자체 를 구성해야 합니다. [!DNL Workfront Goals] 알림이 표시됩니다. 사용자 편집 액세스 권한이 있는 경우 다른 사용자에 대해 이러한 알림을 수정할 수도 있습니다. 활성화용 [!DNL Workfront Goals] 프로필 또는 편집할 수 있는 액세스 권한이 있는 다른 사용자에 대한 알림은 [알림: 목표](../../workfront-basics/using-notifications/notifications-goals.md).

  알림에 대한 자세한 내용은 [!DNL Workfront] 관리자가 구성할 수 있습니다. 다음을 참조하십시오. [시스템의 모든 사용자를 위한 이벤트 알림 구성](../../administration-and-setup/manage-workfront/emails/configure-event-notifications-for-everyone-in-the-system.md). [!DNL Workfront Goals] 은(는) 새 [!DNL Adobe Workfront] 경험.

## 이벤트 알림 콘텐츠

이벤트 알림 이메일에는 발생한 이벤트에 대한 정보와 다음에 대한 링크가 포함되어 있습니다. [!DNL Workfront] 시스템에서 이벤트를 볼 수 있는 위치입니다. 이메일 알림 수신에 대한 자세한 내용은 [[!DNL Adobe Workfront] 알림](../../workfront-basics/using-notifications/wf-notifications.md).

A [!DNL Workfront] 전자 메일 알림은 다음으로 구성되므로 관리자가 콘텐츠를 변경할 수 없습니다. [!DNL Workfront]. 하지만 이벤트 알림 이메일의 제목 줄을 변경할 수 있습니다. 자세한 내용은 [이벤트 알림에 대한 이메일 제목 사용자 지정](../../administration-and-setup/manage-workfront/emails/custom-email-subjects-event-notification.md).

모든 목록의 경우 [!DNL Workfront] 이벤트 알림, 각 이벤트에 대한 간략한 설명 및 기본적으로 활성 또는 비활성인지 여부를 참조하십시오. [에서 사용할 수 있는 이벤트 알림 [!DNL Adobe Workfront]](../../administration-and-setup/manage-workfront/emails/event-notifications-available-in-wf.md).
