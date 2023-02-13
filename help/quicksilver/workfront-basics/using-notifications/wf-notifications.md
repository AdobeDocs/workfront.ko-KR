---
content-type: overview;reference
navigation-topic: notifications
title: Adobe Workfront 알림
description: Adobe Workfront이 모바일 장치에서 이메일 알림, 인앱 알림 및 알림을 보냅니다.
author: Lisa
feature: Get Started with Workfront
exl-id: 118677e9-a13f-47e6-96a3-6f5e93b005e9
source-git-commit: 073e6c7d4e830dfd2b8920a20e1490c5524d71bd
workflow-type: tm+mt
source-wordcount: '1255'
ht-degree: 1%

---

# [!DNL Adobe Workfront] 알림

[!DNL Adobe Workfront] 모바일 장치에서 이메일 알림, 인앱 알림 및 알림을 보냅니다.

## 이메일 알림

[!DNL Workfront] 에서는 Workfront의 활동에 대해 사용자에게 알리고 유용한 정보와 링크를 제공하는 많은 이메일 알림을 보냅니다.

>[!NOTE]
>
>샌드박스 환경에서 이메일 알림을 수신하려면 해당 환경의 사용자 프로필에서 이메일을 활성화해야 합니다.

다음 이메일 알림을 받을 수 있습니다. [!DNL Workfront]:

* [이벤트 알림](#event-notifications)
* [일별 다이제스트 알림](#daily-digest-notifications)
* [게시된 댓글 알림](#notification-of-posted-comments)
* [자동 미리 알림](#automatic-reminders)
* [미리 알림](#reminder-notifications)
* [기타 [!DNL Workfront] 이메일](#other-workfront-emails)

### 이벤트 알림

이벤트 알림은에서 미리 정의됩니다. [!DNL Workfront]. 일반적으로 특정 이벤트에 의해 트리거됩니다.

이벤트 알림이에 의해 활성화되면 [!DNL Workfront] 관리자 또는 그룹 관리자, [!UICONTROL 알림 을 참조하십시오] 사용자 프로필의 환경 설정. 이벤트가 발생하면 알림을 수신할지, 아니면 하나의 일별 다이제스트 이메일에 요약된 이벤트를 수신할지 여부를 선택할 수도 있습니다.

방법에 따라 [!DNL Workfront] 관리자가 이벤트 알림을 구성했습니다 [!DNL Workfront] 시스템(에 설명된 대로 [시스템의 모든 사용자에 대한 이벤트 알림을 구성합니다](../../administration-and-setup/manage-workfront/emails/configure-event-notifications-for-everyone-in-the-system.md)), 설정에 이러한 알림의 하위 세트만 표시될 수 있습니다.

기본 상태는 새 사용자를 만들 때 기본적으로 새 사용자에 대해 활성화된 알림(일별, 인스턴트 또는 둘 다)을 보여줍니다.

이벤트 알림의 전체 목록 및 시스템 수준, 그룹 수준 또는 사용자 수준에서 이벤트 알림의 활성화 및 구성 방법에 대한 자세한 내용은 [에서 사용할 수 있는 이벤트 알림 [!DNL Adobe Workfront]](../../administration-and-setup/manage-workfront/emails/event-notifications-available-in-wf.md).

받을 이벤트 알림을 선택하는 방법에 대한 자세한 내용은 [고유한 이벤트 알림 활성화 또는 비활성화](../../workfront-basics/using-notifications/activate-or-deactivate-your-own-event-notifications.md).

>[!NOTE]
>
>이벤트 알림은 일별 다이제스트 업데이트로 전달되도록 구성할 수 있는 유일한 알림입니다.

### 일별 다이제스트 알림

일별 다이제스트 이메일 게재에 대해 이메일 알림이 활성화되는 전체 목록과 이메일 알림의 모든 카테고리에 대한 정보는 를 참조하십시오 [이벤트 알림](../../workfront-basics/using-notifications/event-notifications.md#understanding-instant-and-daily-digest-notifications).

>[!NOTE]
>
>[!UICONTROL Workfront] 에 대한 일별 다이제스트 알림을 전송하지 않습니다. [!UICONTROL 기타] 및 [!DNL Goals] 이벤트 카테고리. 이러한 카테고리에 대해서는 일별 알림을 비활성화할 수 없습니다.

일별 다이제스트 알림을 받을 때 주의해야 할 몇 가지 사항이 있습니다.

* 각 [!UICONTROL 알림] 섹션 **[!UICONTROL 내 설정]** 패널은 자체 일별 다이제스트 이메일을 생성합니다. 일별 다이제스트 이메일에 사용할 수 있는 알림 설정만큼 매일 다이제스트 이메일을 많이 사용할 수 있습니다.\
   예를 들어, **[!UICONTROL 프로젝트 ID에 대한 정보] 소유,** 이 영역에 대해 충족된 모든 이벤트를 나열하는 전자 메일 알림을 한 개 받습니다.

* 일별 다이제스트 이메일의 알림은 다양한 기준으로 그룹화됩니다. 예를 들어 **[!UICONTROL 내 소유 프로젝트 정보]**&#x200B;를 채울 때는 이벤트를 프로젝트 이름으로 그룹화합니다.

   대상 **[!UICONTROL 통신]** 카테고리에서는 통신이 발생한 개체별로 알림이 그룹화됩니다.

* 일별 다이제스트 전자 메일에는 특정 영역(예: **소유한 프로젝트 정보**)을 클릭하여 제품에서 사용할 수 있습니다.
* 일별 다이제스트 전달을 위해 선택한 시간의 시간대는 브라우저에 구성된 시간대와 일치합니다.
* 일별 다이제스트 이메일에는 제목 줄에 있는 섹션의 이름과 배달되는 날짜가 있습니다.
* 하나 이상의 이벤트가 일별 다이제스트를 배달하려면 알림을 트리거해야 합니다. 일별 다이제스트 이메일에 대해 표시된 이벤트가 충족되지 않으면 일별 다이제스트가 전송되지 않습니다.

### 게시된 댓글 알림

의 알림 [!UICONTROL 통신] 카테고리에 게시된 댓글에 대한 경고 [!UICONTROL 업데이트] 특정 항목의 스트림.

에 대한 일별 다이제스트 이메일 [!UICONTROL 통신] 카테고리가 사용 가능한 모든 알림에 대해 선택됩니다.

이 정보는 통신이 발생한 객체에 대해 요약되며 각 객체에 대해 총 통신 메시지 수가 표시됩니다.

이메일 알림 구성에 대한 자세한 내용은 [고유한 이벤트 알림 활성화 또는 비활성화](../../workfront-basics/using-notifications/activate-or-deactivate-your-own-event-notifications.md).

에 대한 주석 달기에 대한 지침 [!UICONTROL 통신] 이메일, [작업 업데이트](../../workfront-basics/updating-work-items-and-viewing-updates/update-work.md).

에 대해 자세히 알아보려면 [!UICONTROL 통신] 이메일, [고유한 이벤트 알림 활성화 또는 비활성화](../../workfront-basics/using-notifications/activate-or-deactivate-your-own-event-notifications.md).

일별 다이제스트 알림 활성화에 대한 자세한 내용은 [고유한 이벤트 알림 활성화 또는 비활성화](../../workfront-basics/using-notifications/activate-or-deactivate-your-own-event-notifications.md).

### 자동 미리 알림

자동 미리 알림은 [!DNL Workfront] 관리자가 기한, 지연 또는 계획된 완료 일자 근처에 있는 작업 및 문제를 알려드립니다. 지연 알림의 경우 작업이나 문제가 완료될 때까지 매일 밤 이메일이 전송됩니다. 관리자가 이러한 구성 후 비활성화할 수 없습니다. 또한 자동 미리 알림으로 트리거되는 전자 메일의 콘텐츠 또는 제목 줄은 변경할 수 없습니다.

다음 중 하나 이상으로 보낼 수 있습니다.

* 작업 또는 문제에 지정된 사용자
* 사용자의 즉시 관리자
* 바로 아래 관리자의 관리자

자동 미리 알림 이메일은 사용자의 이메일 주소에서 전송됩니다 [!DNL Workfront] 보내는 전자 메일을 처리하도록 선택한 관리자

자동 미리 알림은 활성화되는 항목에 따라 자동 미리 알림 이메일에서 다음 종류의 정보를 사용할 수 있습니다.

* 작업 또는 문제가 만들어진 날짜입니다
* 작업 또는 문제 이름
* 작업 또는 문제가 있는 프로젝트의 이름
* 작업 또는 문제에 대한 설명
* 작업 또는 문제에 할당된 사용자 목록입니다
* 작업 또는 문제를 입력한 사용자의 이름입니다
* 작업 또는 문제의 우선 순위
* 작업 또는 문제가 지연된 날짜

자동 미리 알림 활성화에 대한 자세한 내용은 [자동 미리 알림 설정](../../administration-and-setup/manage-workfront/emails/setting-up-automatic-reminders.md).

### 미리 알림

A [!DNL Workfront] 관리자(또는 [!UICONTROL 계획자] 미리 알림 액세스 수준 및 관리자 액세스)를 통해 마감일이 도래하는 것에 대한 미리 알림 알림을 디자인하고 프로젝트, 작업, 문제 및 작업표에 연결할 수 있습니다. 필요한 관리 액세스를 얻는 방법에 대한 자세한 내용은 [특정 영역에 대한 관리자 액세스 권한 부여](../../administration-and-setup/add-users/configure-and-grant-access/grant-users-admin-access-certain-areas.md).

>[!IMPORTANT]
>
>사용자가 위에 언급된 객체에 대한 미리 알림 알림을 받은 후 기한이 변경되면 사용자는 다른 미리 알림 알림을 받지 않습니다.

미리 알림 은 [!DNL Workfront] 보내는 전자 메일을 처리하도록 선택한 관리자

미리 알림 설정 및 활성화에 대한 자세한 내용은 [미리 알림 설정](../../administration-and-setup/manage-workfront/emails/set-up-reminder-notifications.md).

### 기타 [!DNL Workfront] 이메일

받을 수 있는 다른 이메일이 있습니다 [!DNL Workfront] 구성할 수 없습니다. 다음 이메일은 자동으로 [!DNL Workfront] 이러한 조건이 충족되는 경우:

* 항목 복원: 이 [!DNL Workfront] 관리자는 [!UICONTROL 재활용] Bin에는 이메일이 전송됩니다 [!DNL Workfront] 관리자
* 복원하지 못했습니다. 이 [!DNL Workfront] 관리자가 휴지통에서 개체를 복원하려고 하면 복원이 실패하고 전자 메일이 [!DNL Workfront] 관리자

다음 이메일은 사용자 프로필 수준에서만 구성할 수 있습니다. 시스템 수준에서 활성화하거나 비활성화할 수 없습니다.

* 개인 작업 완료: 다른 사람에게 지정한 개인 작업이 완료되면 이메일을 받게 됩니다.
* 사용자에게 주석 추가: 누군가 사용자 프로필에 댓글을 달면 이메일이 전송됩니다.

## 인앱 알림

내에서 알림을 받을 수 있습니다 [!DNL Workfront] 웹 응용 프로그램, 특정 이벤트가 발생하는 경우

인앱 알림에 대한 자세한 내용은 [인앱 알림 보기 및 관리](../../workfront-basics/using-notifications/view-and-manage-in-app-notifications.md).

## 모바일 이메일 앱의 이메일 알림

받을 수 있습니다 [!DNL Workfront] 모바일 이메일 앱, 모바일 장치의 이메일 알림입니다.

만약 [!DNL Workfront] 휴대폰에 설치된 모바일 앱에서 이메일의 링크를 탭하면 [!DNL Workfront] 모바일 앱. 여기에는 다음 작업 단추를 탭하는 작업이 포함됩니다.

* [!UICONTROL 작업 수행]
* [!UICONTROL 댓글]
* [!UICONTROL 승인 결정]
* [!UICONTROL 모든 알림 보기]
* [!UICONTROL 추가]
* [!UICONTROL 시작하기]
* [!UICONTROL 자세한 내용 보기]

에 대한 자세한 정보 [!DNL Workfront] 모바일 앱의 경우 다음을 참조하십시오. [를 사용하십시오 [!DNL Adobe Workfront] 모바일 앱](../../workfront-basics/mobile-apps/using-the-workfront-mobile-app/use-the-mobile-app.md).
