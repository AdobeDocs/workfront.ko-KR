---
product-area: workfront-integrations
navigation-topic: workfront-for-slack
title: 수신 [!DNL Adobe Workfront] 의 알림 [!DNL Slack]
description: 수신 [!DNL Adobe Workfront] 의 알림 [!DNL Slack]
author: Becky
feature: Workfront Integrations and Apps
exl-id: bc1ce4ea-58be-4cd7-ab59-7dddb82949b9
source-git-commit: f6335f4e94d286681adfb50165562b2c41b5acac
workflow-type: tm+mt
source-wordcount: '587'
ht-degree: 6%

---

# 수신 [!DNL Adobe Workfront] 의 알림 [!DNL Slack]

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: Alina: *** Linked to Accessing Workfront from Slack.***Some of this information is duplicating in Accessing Workfront from Slack (also screen shots))</p>
-->

를 설치한 후 [!DNL Adobe Workfront for Slack], 다음을 받을 수 있습니다. [!DNL Workfront] 의 알림 [!DNL Slack].\
설치에 대한 자세한 내용 [!DNL Workfront for Slack], 참조 [구성 [!DNL Adobe Workfront for Slack]](../../workfront-integrations-and-apps/using-workfront-with-slack/configure-workfront-for-slack.md).

다음의 선택 숫자를 활성화할 수 있습니다. [!UICONTROL 알림] 의 알림 버블에 표시되는 [!DNL Workfront] 인터페이스(게재할 위치) [!DNL Slack].

이메일 알림은 과 독립적으로 작동합니다. [!DNL Workfront] 인터페이스 알림입니다. 본인 또는 본인 [!DNL Workfront] 관리자는에서 이메일 알림을 비활성화할 수 있지만 인터페이스 알림은 비활성화할 수 없습니다. [!DNL Workfront].\
그러나 을 비활성화할 수 있습니다 [!DNL Workfront] 에서 수신할 수 있는 알림 [!DNL Slack]을 사용하여 내부 알림에만 집중할 수 있습니다. [!DNL Workfront] 인터페이스.

## 액세스 요구 사항

다음 항목이 있어야 합니다.

<table style="table-layout:auto"> 
 <col> 
 </col> 
 <col> 
 </col> 
 <tbody> 
  <tr> 
   <td role="rowheader"><a href="https://www.workfront.com/plans" target="_blank">[!DNL [!DNL Adobe Workfront] 플랜]</a>*</td> 
   <td> <p>[!UICONTROL Pro] 이상</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;보유 중인 플랜, 라이선스 유형 또는 액세스 권한을 알아보려면 [!DNL Workfront] 관리자\

## 전제 조건

받기 전 [!DNL Workfront] 의 알림 [!DNL Slack], 다음을 수행해야 합니다.

* Configure [!DNL Workfront for Slack]\
   구성에 대한 지침 [!DNL Workfront for Slack], 참조 [구성 [!DNL Adobe Workfront for Slack]](../../workfront-integrations-and-apps/using-workfront-with-slack/configure-workfront-for-slack.md).

## 구성 [!DNL Workfront] 다음에 대한 알림: [!DNL Slack] {#configure-workfront-notifications-for-slack}

1. (조건부) 이후 [!DNL Workfront] 이(가) 다음에 추가되었습니다. [!DNL Slack] 인스턴스, 로그인 [!DNL Workfront] 출처: [!DNL Slack].\
   에 로그인하는 방법에 대한 자세한 정보 [!DNL Workfront] 출처: [!DNL Slack], 참조 [액세스 [!DNL Adobe Workfront] 출처: [!DNL Slack]](../../workfront-integrations-and-apps/using-workfront-with-slack/access-workfront-from-slack.md).

1. 모든 채널에서 메시지 필드에 다음 명령 중 하나를 입력하십시오.

   `/workfront settings`

   또는

   `/wf settings`

1. 모든 알림은 기본적으로 활성화되어 있습니다.\
   다음 알림을 비활성화합니다.

   * [!UICONTROL 새로운 작업 또는 문제에 할당됨]
   * [!UICONTROL 내 팀이 새 작업 또는 문제에 할당되었습니다.]
   * [!UICONTROL 새로운 승인 또는 액세스 요청을 받습니다.]
   * [!UICONTROL 누군가가 지시된 업데이트에 나를 포함시킵니다.]
   * [!UICONTROL 누군가 내가 속한 스레드에 주석을 남김]
   * [!UICONTROL 내가 구독 중인 작업, 문제 또는 프로젝트에 업데이트가 이루어짐]
   * [!UICONTROL 누군가 내 작업 항목 중 하나에 댓글을 남겼습니다.]
   * [!UICONTROL 누군가 내 도움말 요청에 주석을 남김]

   다음에 대한 변경 사항 [!UICONTROL 알림] 옵션은 즉시 적용됩니다.\
   활성화한 알림은 [!DNL Workfront] [!DNL Slack] 채널. 여기에서 알림을 비활성화하면 다음에 대한 알림만 비활성화됩니다. [!DNL Slack], 및 를 위한 것이 아님 [!DNL Workfront] 인터페이스. 에서 계속 수신합니다. [!DNL Workfront] 인터페이스 오른쪽 상단의 알림 버블입니다.

## 관리 [!DNL Workfront] 다음에서 알림: [!DNL Slack]

을 받고 응답할 수 있습니다. [!DNL Workfront] 다음에서 알림: [!DNL Slack].

에서 활성화하는 알림에 대해 이메일 알림을 비활성화할 수 있습니다. [!DNL Slack]중복 알림을 받지 않도록 하기 위해 입니다.\
이메일 알림 구성에 대한 자세한 내용은 [이메일 알림 수정](../../workfront-basics/using-notifications/activate-or-deactivate-your-own-event-notifications.md).

활성화 또는 비활성화 [!DNL Workfront] 의 알림 [!DNL Slack] 에서 수신하는 알림에 영향을 주지 않음 [!DNL Workfront] 인터페이스.\
내부 알림 [!DNL Workfront] 인터페이스를 비활성화할 수 없습니다.

을(를) 관리하려면 [!DNL Workfront] 다음에 대한 알림: [!DNL Slack]:

1. 에 로그인 [!UICONTROL Slack].
1. 에 로그인 [!DNL Workfront] 출처: [!DNL Slack].\
   에 로그인하는 방법에 대한 자세한 내용 [!DNL Workfront] 출처: [!DNL Slack]에 로그인하는 방법을 참조하십시오. [!DNL Workfront] 출처: [!DNL Slack]의 &quot; 섹션 [액세스 [!DNL Adobe Workfront] 출처: [!DNL Slack]](../../workfront-integrations-and-apps/using-workfront-with-slack/access-workfront-from-slack.md).

1. 다음을 확인합니다. [!DNL Workfront] 다음에 대한 알림: [!DNL Slack] 활성화되었습니다.\
   에 대한 자세한 내용은 [!DNL Workfront] 알림도 (으)로 보내도록 구성할 수 있습니다. [!DNL Slack], 참조 [구성 [!DNL Workfront] 다음에 대한 알림: [!DNL Slack]](#configure-workfront-notifications-for-slack-configure-workfront-notifications-for-slack).

1. 로 이동 **[!DNL Workfront]** 채널을 통해 [!DNL Workfront] 알림입니다.
1. (조건부 및 선택 사항) 다음 중 하나를 수행합니다.

   * 클릭 **[!UICONTROL 처리 중]** 을(를) 수락하여 작업에 대한 작업을 수행합니다.

   * (조건부 및 선택 사항) 클릭 **[!UICONTROL 회신[!DNL Workfront]]** 댓글에 회신하려면 회신을 입력하고 **[!UICONTROL 답변]**.

   * (조건부 및 선택 사항) 클릭 **[!UICONTROL 승인]** 또는 **[!UICONTROL 거부]** 승인 보류 중인 작업, 문제 또는 프로젝트를 승인하거나 거부합니다.

   * (조건부 및 선택 사항) 클릭 **[!UICONTROL 승인]**, **[!UICONTROL 변경 사항]**, 또는 **[!UICONTROL 거부]**&#x200B;를 입력하여 문서를 승인하거나, 변경 내용을 적용하거나, 거부합니다.

     문서를 승인하기 전에 문서의 축소판 위로 마우스를 가져간 후 돋보기 아이콘을 클릭하여 더 큰 미리 보기를 볼 수도 있습니다.\
      승인된 Slack [파일 유형](https://api.slack.com/types/file) 미리보기 가능.

   * (조건부 및 선택 사항) 클릭 **[!UICONTROL 부여]** 또는 **[!UICONTROL 무시]** 다른 사용자의 추가 액세스 요청에 대한 권한을 부여하거나 무시합니다.\

     다음 항목에서 작업이 완료되었다는 확인 메시지가 표시됩니다 [!DNL Workfront]을 추가하여 알림에서 결정하는 모든 것을 선택할 수 있습니다.
