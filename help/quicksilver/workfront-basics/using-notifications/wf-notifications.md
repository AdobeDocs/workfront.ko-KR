---
content-type: overview;reference
navigation-topic: notifications
title: 알림 개요
description: Adobe Workfront은 모바일 디바이스에서 이메일 알림, 인앱 알림 및 알림을 보냅니다.
author: Courtney
feature: Get Started with Workfront
exl-id: 118677e9-a13f-47e6-96a3-6f5e93b005e9
source-git-commit: 64b8a835a57be8995c82a0ab15c40f46170c7067
workflow-type: tm+mt
source-wordcount: '1395'
ht-degree: 1%

---

# 알림 개요

<!--Audited: 12/2023-->

[!DNL Adobe Workfront]이(가) 모바일 장치에서 이메일 알림, 인앱 알림 및 알림을 보냅니다.

## 이메일 알림

[!DNL Workfront]이(가) 사용자에게 Workfront의 활동에 대해 경고하는 전자 메일 알림을 보내고 유용한 정보와 링크를 제공합니다.

전자 메일 알림의 기본 설정을 변경하려면 [전자 메일 알림 수정](../../workfront-basics/using-notifications/activate-or-deactivate-your-own-event-notifications.md)을 참조하세요.

>[!NOTE]
>
>샌드박스 환경에서 이메일 알림을 수신하려면 해당 환경의 사용자 프로필에서 이메일을 활성화해야 합니다.

[!DNL Workfront]에서 다음 전자 메일 알림을 받을 수 있습니다.

* [이벤트 알림](#event-notifications)
* [일별 다이제스트 알림](#daily-digest-notifications)
* [게시된 의견 알림](#notification-of-posted-comments)
* [자동 미리 알림](#automatic-reminders)
* [미리 알림](#reminder-notifications)
* [게시판 알림](#boards-notifications)
* [기타 [!DNL Workfront] 개의 전자 메일](#other-workfront-emails)

### 이벤트 알림

이벤트 알림은 일반적으로 사용자에게 작업을 할당하거나 작성한 댓글에 대한 답변을 받는 것과 같이 사전 정의된 특정 이벤트에 의해 트리거됩니다.

[!DNL Workfront] 관리자 또는 그룹 관리자가 [!DNL Workfront] 시스템에서 이벤트 알림을 활성화한 후 사용자 프로필에서 [!UICONTROL 알림] 기본 설정을 편집하여 수신하려는 알림을 선택할 수 있습니다. 이벤트 발생 시 알림을 수신할지 또는 일일 요약 이메일 하나로 요약된 이벤트를 수신할지 여부를 선택할 수도 있습니다.

[!DNL Workfront] 관리자가 [!DNL Workfront] 시스템에 대해 이벤트 알림을 구성한 방법에 따라 설정에 이러한 알림의 하위 집합만 표시될 수 있습니다. 자세한 내용은 [시스템의 모든 사용자를 위한 이벤트 알림 구성](../../administration-and-setup/manage-workfront/emails/configure-event-notifications-for-everyone-in-the-system.md)을 참조하십시오.

새 사용자를 만들 때 새 사용자에 대해 기본적으로 활성화되어 있는 알림(매일, 인스턴트 또는 둘 다)이 기본 상태에 표시됩니다.

이벤트 알림의 전체 목록과 시스템 수준, 그룹 수준 또는 사용자 수준에서 이벤트 알림을 활성화하고 구성하는 방법에 대한 자세한 내용은 [사용 가능한 이벤트 알림 [!DNL Adobe Workfront]](../../administration-and-setup/manage-workfront/emails/event-notifications-available-in-wf.md)을 참조하십시오.

받을 이벤트 알림을 선택하는 방법에 대한 자세한 내용은 [전자 메일 알림 수정](../../workfront-basics/using-notifications/activate-or-deactivate-your-own-event-notifications.md)을 참조하세요.

>[!NOTE]
>
>이벤트 알림은 일별 다이제스트 업데이트에서 전달하도록 구성할 수 있는 유일한 알림입니다.

### 일별 다이제스트 알림

일별 요약 알림은 이메일 24시간 전에 받은 특정 유형의 알림이 모두 포함된 이메일입니다.

매일 요약 전자 메일 배달에 사용할 수 있는 전자 메일 알림과 전자 메일 알림의 모든 범주에 대한 전체 목록이 필요하면 [이벤트 알림](../../workfront-basics/using-notifications/event-notifications.md#understanding-instant-and-daily-digest-notifications)을 참조하세요.

>[!NOTE]
>
>[!UICONTROL Workfront]은(는) 이벤트의 [!UICONTROL 기타] 및 [!DNL Goals] 범주에 대한 일별 요약 알림을 보내지 않습니다. 이러한 범주에 대해 일별 알림을 비활성화할 수 없습니다.

일별 요약 알림을 받을 때 알아야 할 몇 가지 사항이 있습니다.

* [!UICONTROL 내 설정] 패널의 각 **[!UICONTROL 알림]** 섹션에서 매일 다이제스트 전자 메일을 만듭니다. 일별 다이제스트 전자 메일에 대해 활성화된 알림 설정만큼 일별 다이제스트 전자 메일을 매일 가질 수 있습니다.\
   예를 들어, **[!UICONTROL 내가 소유한 프로젝트에 대한 정보]에서 여러 작업에 대한 일일 요약 이메일을 수신하도록 선택한 경우** 이 영역에 대해 충족된 모든 이벤트를 나열하는 하나의 이메일 알림을 받게 됩니다.

* 일별 다이제스트 이메일의 알림은 다양한 기준으로 그룹화됩니다. 예를 들어 **[!UICONTROL 내가 소유한 프로젝트에 대한 정보]**&#x200B;의 경우 이벤트는 프로젝트 이름별로 그룹화됩니다.

  **[!UICONTROL Communication]** 범주의 경우 알림은 통신이 발생한 개체별로 그룹화됩니다.

  >[!NOTE]
  >
  >통신 범주의 경우 즉시 게재에 대해서만 개별 알림을 선택할 수 있습니다. 일별 요약으로 알림을 전달하려면 알림을 모두 선택해야 합니다.

* 일별 요약 전자 메일에는 배달을 위해 선택한 시간 전 24시간 내에 특정 영역(**내가 소유한 프로젝트에 대한 정보** 등)의 작업에 대해 발생한 이벤트가 나열됩니다.
* 일별 다이제스트 배달을 위해 선택한 시간의 시간대는 브라우저에 구성되어 있으므로 해당 시간대와 일치합니다.
* 일별 요약 이메일에는 제목란에 있는 섹션의 이름과 게재된 날짜가 있습니다.
* 일별 다이제스트를 게재하려면 적어도 하나의 이벤트가 알림을 트리거해야 합니다. 일별 요약 이메일로 표시된 이벤트가 충족되지 않으면 일별 요약이 전송되지 않습니다.

### 게시된 의견 알림

[!UICONTROL Communication] 범주의 알림은 특정 항목의 [!UICONTROL 업데이트] 스트림에 게시된 댓글에 대해 경고합니다.

사용 가능한 모든 알림에 대해 [!UICONTROL 통신] 범주의 일별 요약 전자 메일이 선택됩니다.

통신이 발생한 객체에 대한 정보가 요약되고, 각 객체에 대한 총 통신 메시지 수가 표시됩니다.

Workfront에서 댓글에 답글을 달거나 댓글을 보려면 다음 작업을 수행하십시오.

1. 전자 메일의 **[!UICONTROL 댓글]** 단추를 클릭합니다.

   개체의 [!UICONTROL 업데이트] 영역이 열리고 구체적인 설명은 파란색으로 표시됩니다.

   댓글에 회신하는 데 사용할 수 있는 회신 상자가 열려 있습니다.

일별 요약 알림을 포함하여 전자 메일 알림을 구성하는 방법에 대한 자세한 내용은 [전자 메일 알림 설정 수정](../../workfront-basics/using-notifications/activate-or-deactivate-your-own-event-notifications.md#view-and-modify-your-email-notification-settings)에서 [전자 메일 알림 설정 보기 및 수정](../../workfront-basics/using-notifications/activate-or-deactivate-your-own-event-notifications.md)을 참조하세요.

### 자동 미리 알림

[!DNL Workfront] 관리자가 기한이 지났거나, 늦었거나, 계획된 완료 날짜에 근접한 작업 및 문제에 대해 경고하기 위해 자동 미리 알림을 사용하도록 설정했습니다. 지연 알림의 경우 작업 또는 문제가 완료될 때까지 이메일이 매일 밤 전송됩니다. 관리자가 이를 구성한 후에는 비활성화할 수 없습니다. 또한 자동 미리 알림으로 트리거된 이메일의 콘텐츠나 제목 줄은 변경할 수 없습니다.

자동 알림은 다음 중 하나 이상으로 보낼 수 있습니다.

* 작업 또는 문제에 할당된 사용자
* 사용자의 직속 관리자
* 직속 관리자의 관리자

[!DNL Workfront] 관리자가 발신 전자 메일을 처리하기 위해 선택한 전자 메일 주소에서 자동 미리 알림 전자 메일이 전송됩니다.

활성화된 자동 미리 알림에 따라 자동 미리 알림 이메일에서 다음 유형의 정보를 사용할 수 있습니다.

* 작업 또는 문제가 생성된 날짜
* 작업 또는 문제 이름
* 작업 또는 문제가 있는 프로젝트의 이름
* 작업 또는 문제에 대한 설명
* 작업 또는 문제에 할당된 사용자 목록
* 작업 또는 문제를 입력한 사용자의 이름
* 작업 또는 문제의 우선 순위
* 작업 또는 문제가 기한이 지난 날짜

자동 미리 알림 사용에 대한 자세한 내용은 [자동 미리 알림 설정](../../administration-and-setup/manage-workfront/emails/setting-up-automatic-reminders.md)을 참조하세요.

### 미리 알림

[!DNL Workfront] 관리자(또는 미리 알림에 대한 [!UICONTROL 플래너] 액세스 수준과 관리 액세스 권한이 있는 사용자)는 기한이 다가오는 것에 대한 미리 알림을 디자인하고 프로젝트, 작업, 문제 및 타임시트와 수동으로 연결할 수 있습니다.

>[!IMPORTANT]
>
>사용자가 위에서 언급한 객체에 대한 미리 알림을 받은 후 기한이 변경되면 사용자는 다른 미리 알림을 받지 않습니다.

미리 알림은 [!DNL Workfront] 관리자가 발신 전자 메일을 처리하기 위해 선택한 전자 메일 주소에서 전송됩니다.

미리 알림 설정 및 활성화에 대한 자세한 내용은 [미리 알림 설정](../../administration-and-setup/manage-workfront/emails/set-up-reminder-notifications.md)을 참조하세요.

필요한 관리 액세스 권한을 받는 방법에 대한 자세한 내용은 [특정 영역에 대한 관리 액세스 권한 부여](../../administration-and-setup/add-users/configure-and-grant-access/grant-users-admin-access-certain-areas.md)를 참조하십시오.

### 게시판 알림

[!DNL Adobe Workfront] [!UICONTROL 게시판]에서 사용자가 게시판에 추가되고 사용자에게 카드가 할당되면 전자 메일을 보냅니다. 보드 환경 설정에서 수신할 이메일을 선택할 수 있습니다.

자세한 내용은 [게시판 전자 메일 알림 및 환경 설정](/help/quicksilver/agile/get-started-with-boards/boards-emails.md)을 참조하세요.

### 기타 [!DNL Workfront]개의 전자 메일

구성할 수 없는 [!DNL Workfront]에서 받을 수 있는 다른 전자 메일이 있습니다.

다음 조건이 충족되면 [!DNL Workfront]이(가) 자동으로 다음 이메일을 보냅니다.

* 항목 복원: [!DNL Workfront] 관리자가 [!UICONTROL 휴지통] 저장소에서 개체를 복원하면 [!DNL Workfront] 관리자에게 전자 메일이 전송됩니다.
* 복원되지 않음: [!DNL Workfront] 관리자가 휴지통에서 개체를 복원하려고 할 때 복원이 실패하면 [!DNL Workfront] 관리자에게 전자 메일이 전송됩니다.

다음 이메일은 사용자 프로필 수준에서만 구성할 수 있습니다. 시스템 수준에서 활성화하거나 비활성화할 수 없습니다.

* 개인 작업 완료: 다른 사람에게 할당한 개인 작업이 완료되면 이메일을 받게 됩니다.
* 사용자에 추가된 댓글: 누군가 사용자 프로필에 댓글을 달면 이메일을 받게 됩니다.

## 인앱 알림

특정 이벤트가 발생하면 [!DNL Workfront] 웹 응용 프로그램 내에서 알림을 받을 수 있습니다.

인앱 알림에 대한 자세한 내용은 [인앱 알림 보기 및 관리](../../workfront-basics/using-notifications/view-and-manage-in-app-notifications.md)를 참조하십시오.

## 모바일 이메일 앱의 이메일 알림

모바일 장치에서 모바일 이메일 앱에서 [!DNL Workfront]개의 이메일 알림을 받을 수 있습니다.

휴대폰에 [!DNL Workfront] 모바일 앱이 설치되어 있는 경우 전자 메일의 링크를 탭하면 [!DNL Workfront] 모바일 앱에서 링크가 열립니다. 여기에는 다음 작업 버튼 탭하기 등이 포함됩니다.

* [!UICONTROL 작업]
* [!UICONTROL 댓글]
* [!UICONTROL 승인 결정]
* [!UICONTROL 모든 알림 보기]
* [!UICONTROL 추가]
* [!UICONTROL 시작]
* [!UICONTROL 자세히 보기]

[!DNL Workfront] 모바일 앱에 대한 자세한 내용은 [모바일 앱 사용 [!DNL Adobe Workfront] 을 참조하십시오](../../workfront-basics/mobile-apps/using-the-workfront-mobile-app/use-the-mobile-app.md).
