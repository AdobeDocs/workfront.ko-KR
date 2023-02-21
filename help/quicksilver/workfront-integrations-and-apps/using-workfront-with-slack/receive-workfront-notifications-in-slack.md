---
product-area: workfront-integrations
navigation-topic: workfront-for-slack
title: 수신 [!DNL Adobe Workfront] 알림 [!DNL Slack]
description: 수신 [!DNL Adobe Workfront] 알림 [!DNL Slack]
author: Becky
feature: Workfront Integrations and Apps
exl-id: bc1ce4ea-58be-4cd7-ab59-7dddb82949b9
source-git-commit: 65bfeafe67a10c72e87a02e0ece285df619fcb81
workflow-type: tm+mt
source-wordcount: '589'
ht-degree: 6%

---

# 수신 [!DNL Adobe Workfront] 알림 [!DNL Slack]

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: Alina: *** Linked to Accessing Workfront from Slack.***Some of this information is duplicating in Accessing Workfront from Slack (also screen shots))</p>
-->

설치한 후 [!DNL Adobe Workfront for Slack]: [!DNL Workfront] 알림 [!DNL Slack].\
설치에 대한 자세한 정보 [!DNL Workfront for Slack]를 참조하십시오. [구성 [!DNL Adobe Workfront for Slack]](../../workfront-integrations-and-apps/using-workfront-with-slack/configure-workfront-for-slack.md).

선택한 수의 [!UICONTROL 알림] 알림 버블에 표시되는 [!DNL Workfront] 인터페이스, 전달 [!DNL Slack].

이메일 알림은 과 독립적으로 작동합니다 [!DNL Workfront] 인터페이스 알림을 참조하십시오. 사용자 또는 사용자 [!DNL Workfront] 관리자는 이메일 알림을 비활성화할 수 있지만 인터페이스 알림은 을 [!DNL Workfront].\
그러나 비활성화하거나 [!DNL Workfront] 수신할 수 있는 알림 [!DNL Slack]를 설정하는 것이 좋습니다 [!DNL Workfront] 인터페이스.

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

&#42;어떤 계획, 라이센스 유형 또는 액세스 권한을 보유하고 있는지 확인하려면 [!DNL Workfront] 관리자\

## 전제 조건

받기 전에 [!DNL Workfront] 알림 [!DNL Slack]:

* Configure [!DNL Workfront for Slack]\
   구성에 대한 지침 [!DNL Workfront for Slack]를 참조하십시오. [구성 [!DNL Adobe Workfront for Slack]](../../workfront-integrations-and-apps/using-workfront-with-slack/configure-workfront-for-slack.md).

## 구성 [!DNL Workfront] 알림 [!DNL Slack] {#configure-workfront-notifications-for-slack}

1. (조건부) 이후 [!DNL Workfront] 이(가) [!DNL Slack] 인스턴스, 로그인 [!DNL Workfront] 변환 전: [!DNL Slack].\
   로그인하는 방법에 대한 자세한 내용은 [!DNL Workfront] 변환 전: [!DNL Slack]를 참조하십시오. [액세스 [!DNL Adobe Workfront] 변환 전: [!DNL Slack]](../../workfront-integrations-and-apps/using-workfront-with-slack/access-workfront-from-slack.md).

1. 채널에서 메시지 필드에 다음 명령 중 하나를 입력합니다.

   `/workfront settings`

   또는

   `/wf settings`

1. 기본적으로 모든 알림이 활성화됩니다.\
   다음 알림 중 하나를 비활성화합니다.

   * [!UICONTROL 새 작업이나 문제에 할당되었습니다]
   * [!UICONTROL 내 팀이 새 작업 또는 문제에 할당되었습니다]
   * [!UICONTROL 새로운 승인 또는 액세스 요청을 받습니다]
   * [!UICONTROL 누군가가 지시된 업데이트에 나를 포함시킵니다.]
   * [!UICONTROL 누군가 내가 속한 스레드에 주석을 남김]
   * [!UICONTROL 내가 구독 중인 작업, 문제 또는 프로젝트에 업데이트가 이루어짐]
   * [!UICONTROL 누군가 내 작업 항목 중 하나에 댓글을 남겼습니다.]
   * [!UICONTROL 내 도움말 요청에 대한 댓글]

   사용자가 변경한 [!UICONTROL 알림] 옵션은 즉시 적용됩니다.\
   활성화한 알림은 [!DNL Workfront] [!DNL Slack] 채널. 여기에서 알림을 비활성화하면 [!DNL Slack], 및에 대해 아님 [!DNL Workfront] 인터페이스. 에서 계속 수신됩니다 [!DNL Workfront] 인터페이스 오른쪽 상단의 알림 버블입니다.

## 관리 [!DNL Workfront] 알림 [!DNL Slack]

수신하고 응답할 수 있습니다 [!DNL Workfront] 알림 [!DNL Slack].

에서 활성화한 알림에 대한 이메일 알림을 비활성화할 수 있습니다 [!DNL Slack]중복 알림을 받지 않도록 합니다.\
이메일 알림 구성에 대한 자세한 내용은 [고유한 이벤트 알림 활성화 또는 비활성화](../../workfront-basics/using-notifications/activate-or-deactivate-your-own-event-notifications.md).

활성화 또는 비활성화 [!DNL Workfront] 알림 [!DNL Slack] 는 내에서 받는 알림에 영향을 주지 않습니다 [!DNL Workfront] 인터페이스.\
내부 알림 [!DNL Workfront] 인터페이스를 사용하지 않도록 설정할 수 없습니다.

를 관리하려면 [!DNL Workfront] 알림 [!DNL Slack]:

1. 에 로그인합니다. [!UICONTROL Slack].
1. 에 로그인합니다. [!DNL Workfront] 변환 전: [!DNL Slack].\
   로그인하는 방법에 대한 자세한 내용 [!DNL Workfront] 변환 전: [!DNL Slack]에 로그인하는 것은 [!DNL Workfront] 변환 전: [!DNL Slack]&quot; 섹션 [액세스 [!DNL Adobe Workfront] 변환 전: [!DNL Slack]](../../workfront-integrations-and-apps/using-workfront-with-slack/access-workfront-from-slack.md).

1. 에서 [!DNL Workfront] 알림 [!DNL Slack] 이 활성화되어 있습니다.\
   자세한 내용 [!DNL Workfront] 알림도 전송하도록 구성할 수 있습니다 [!DNL Slack]를 참조하십시오. [구성 [!DNL Workfront] 알림 [!DNL Slack]](#configure-workfront-notifications-for-slack-configure-workfront-notifications-for-slack).

1. 로 이동합니다. **[!DNL Workfront]** 찾을 채널 [!DNL Workfront] 알림.
1. (조건부 및 선택 사항) 다음 중 하나를 수행합니다.

   * 클릭 **[!UICONTROL 작업]** 일을 맡도록 수락하다.

   * (조건부 및 선택 사항) **[!UICONTROL 회신[!DNL Workfront]]** 댓글에 응답하려면 응답을 입력한 다음 **[!UICONTROL 회신]**.

   * (조건부 및 선택 사항) **[!UICONTROL 승인]** 또는 **[!UICONTROL 거부]** 승인 보류 중인 작업, 문제 또는 프로젝트를 승인하거나 거부하려면 다음을 수행하십시오.

   * (조건부 및 선택 사항) **[!UICONTROL 승인]**, **[!UICONTROL 변경 사항]**, 또는 **[!UICONTROL 거부]**&#x200B;를 사용하여 문서를 승인하거나, 변경 사항으로 승인하거나, 거부할 수 있습니다.

      문서의 축소판 위로 마우스를 가져간 다음 확대경 아이콘을 클릭하여 문서를 승인하기 전에 더 큰 미리 보기를 볼 수도 있습니다.\
      승인된 Slack만 [파일 형식](https://api.slack.com/types/file) 미리 보기를 수행할 수 있습니다.

   * (조건부 및 선택 사항) **[!UICONTROL 승인]** 또는 **[!UICONTROL 무시]** 다른 사용자에 대한 추가 액세스 요청을 부여하거나 무시하려면\

      작업이 완료되었다는 확인 메시지가 나타납니다. [!DNL Workfront]를 설정하는 것이 좋습니다.
