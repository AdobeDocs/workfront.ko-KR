---
product-area: workfront-integrations
navigation-topic: workfront-for-slack
title: ' [!DNL Adobe Workfront] 에서  [!DNL Slack]알림 수신'
description: ' [!DNL Adobe Workfront] 에서  [!DNL Slack]알림 수신'
author: Becky
feature: Workfront Integrations and Apps
exl-id: bc1ce4ea-58be-4cd7-ab59-7dddb82949b9
source-git-commit: 6178cabbf021fbf92bd8795c5c2bd0346801d64d
workflow-type: tm+mt
source-wordcount: '584'
ht-degree: 1%

---

# [!DNL Adobe Workfront]에서 [!DNL Slack]개의 알림 수신

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: Alina: *** Linked to Accessing Workfront from Slack.***Some of this information is duplicating in Accessing Workfront from Slack (also screen shots))</p>
-->

[!DNL Adobe Workfront for Slack]을(를) 설치한 후에는 [!DNL Workfront]에서 [!DNL Slack]개의 알림을 받을 수 있습니다.\
[!DNL Workfront for Slack] 설치에 대한 자세한 내용은 [구성 [!DNL Adobe Workfront for Slack]](../../workfront-integrations-and-apps/using-workfront-with-slack/configure-workfront-for-slack.md)을 참조하십시오.

[!UICONTROL &#x200B; 인터페이스의 알림 버블에 표시되는 &#x200B;]알림[!DNL Workfront]의 선택 개수를 [!DNL Slack]에서도 전달할 수 있습니다.

전자 메일 알림은 [!DNL Workfront] 인터페이스 알림과 독립적으로 작동합니다. 사용자 또는 [!DNL Workfront] 관리자는 전자 메일 알림을 비활성화할 수 있지만 [!DNL Workfront]에서는 인터페이스 알림을 비활성화할 수 없습니다.\
그러나 [!DNL Workfront] 인터페이스 내에서만 해당 알림에 집중하려면 [!DNL Slack]에서 받을 수 있는 [!DNL Workfront] 알림을 비활성화할 수 있습니다.

## 액세스 요구 사항

+++ 을 확장하여 이 문서의 기능에 대한 액세스 요구 사항을 봅니다.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront 패키지</td> 
   <td> <p>임의</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront 라이선스</td> 
   <td> <p>임의</p>
  </tr> 
 </tbody> 
</table>

자세한 내용은 [Workfront 설명서의 액세스 요구 사항](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)을 참조하십시오.

+++

## 전제 조건

[!DNL Workfront]에서 [!DNL Slack]개의 알림을 받으려면 먼저 다음을 수행해야 합니다.

* [!DNL Workfront for Slack] 구성\
   [!DNL Workfront for Slack] 구성에 대한 지침은 [구성 [!DNL Adobe Workfront for Slack]](../../workfront-integrations-and-apps/using-workfront-with-slack/configure-workfront-for-slack.md)을 참조하십시오.

## [!DNL Workfront]에 대한 [!DNL Slack] 알림 구성 {#configure-workfront-notifications-for-slack}

1. (조건부) [!DNL Workfront]이(가) [!DNL Slack] 인스턴스에 추가되면 [!DNL Workfront]에서 [!DNL Slack]에 로그인합니다.\
   [!DNL Workfront]에서 [!DNL Slack]에 로그인하는 방법에 대한 자세한 내용은 [액세스 [!DNL Adobe Workfront] 출처 [!DNL Slack]](../../workfront-integrations-and-apps/using-workfront-with-slack/access-workfront-from-slack.md)를 참조하십시오.

1. 모든 채널에서 메시지 필드에 다음 명령 중 하나를 입력하십시오.

   `/workfront settings`

   또는

   `/wf settings`

1. 모든 알림은 기본적으로 활성화되어 있습니다.\
   다음 알림을 비활성화합니다.

   * [!UICONTROL 새 작업 또는 문제에 할당됨]
   * [!UICONTROL 내 팀이 새 작업 또는 문제에 할당되었습니다]
   * [!UICONTROL 새 승인 또는 액세스 요청을 받습니다]
   * [!UICONTROL 누군가가 지시된 업데이트에 나를 포함시킵니다.]
   * [!UICONTROL 내가 있는 스레드에 누군가 댓글을 남겼습니다]
   * [!UICONTROL 내가 구독 중인 작업, 문제 또는 프로젝트에 업데이트가 이루어짐]
   * [!UICONTROL 누군가 내 작업 항목 중 하나에 댓글을 남겼습니다]
   * [!UICONTROL 누군가 내 도움말 요청에 댓글을 남겼습니다]

   [!UICONTROL 알림] 옵션에 대한 변경 사항이 즉시 적용됩니다.\
   활성화한 알림은 [!DNL Workfront] [!DNL Slack] 채널에서 전달됩니다. 여기에서 알림을 사용하지 않도록 설정하면 [!DNL Slack] 인터페이스가 아닌 [!DNL Workfront]에 대해서만 사용할 수 없습니다. 인터페이스 오른쪽 상단의 [!DNL Workfront] 알림 버블에서 계속 수신합니다.

## [!DNL Workfront]의 [!DNL Slack] 알림 관리

[!DNL Workfront]에서 [!DNL Slack]개의 알림을 받고 응답할 수 있습니다.

[!DNL Slack]에서 사용하도록 설정한 알림에 대해 이메일 알림을 사용하지 않도록 설정하여 중복 알림을 받지 않도록 할 수 있습니다.\
전자 메일 알림 구성에 대한 자세한 내용은 [전자 메일 알림 수정](../../workfront-basics/using-notifications/activate-or-deactivate-your-own-event-notifications.md)을 참조하세요.

[!DNL Workfront]에서 [!DNL Slack] 알림을 사용하거나 사용하지 않도록 설정해도 [!DNL Workfront] 인터페이스 내에서 받는 알림에는 영향을 주지 않습니다.\
[!DNL Workfront] 인터페이스 내의 알림을 사용하지 않도록 설정할 수 없습니다.

[!DNL Workfront]에 대한 [!DNL Slack] 알림을 관리하려면:

1. [!UICONTROL Slack]에 로그인합니다.
1. [!DNL Workfront]에서 [!DNL Slack]에 로그인합니다.\
   [!DNL Workfront]에서 [!DNL Slack]에 로그인하는 방법에 대한 자세한 내용은 [!DNL Workfront]Access[!DNL Slack]from[의 &quot; [!DNL Adobe Workfront] 에서  [!DNL Slack]](../../workfront-integrations-and-apps/using-workfront-with-slack/access-workfront-from-slack.md)에 로그인&quot; 섹션을 참조하십시오.

1. [!DNL Workfront]에 대한 [!DNL Slack] 알림이 활성화되어 있는지 확인하십시오.\
   [!DNL Workfront]에도 전송할 수 있도록 구성할 수 있는 [!DNL Slack] 알림에 대한 자세한 내용은 [구성 [!DNL Workfront] 알림 [!DNL Slack]](#configure-workfront-notifications-for-slack-configure-workfront-notifications-for-slack)을 참조하십시오.

1. **[!DNL Workfront]** 채널로 이동하여 [!DNL Workfront] 알림을 찾으십시오.
1. (조건부 및 선택 사항) 다음 중 하나를 수행합니다.

   * 작업을 수락하려면 **[!UICONTROL 작업]**&#x200B;을 클릭하세요.

   * (조건부 및 선택 사항) 댓글에 회신하려면 **[!UICONTROL [!DNL Workfront]]**&#x200B;에서 회신을 클릭하고 회신을 입력한 다음 **[!UICONTROL 회신]**&#x200B;을 클릭합니다.

   * (조건부 및 선택 사항) 승인을 보류 중인 작업, 문제 또는 프로젝트를 승인하거나 거부하려면 **[!UICONTROL 승인]** 또는 **[!UICONTROL 거부]**&#x200B;를 클릭합니다.

   * (조건부 및 선택 사항) 문서를 승인하거나, 변경 내용을 적용하거나, 거부하려면 **[!UICONTROL 승인]**, **[!UICONTROL 변경 내용]** 또는 **[!UICONTROL 거부]**&#x200B;를 클릭합니다.

     문서를 승인하기 전에 문서의 축소판 위로 마우스를 가져간 후 돋보기 아이콘을 클릭하여 더 큰 미리 보기를 볼 수도 있습니다.\
      승인된 Slack [파일 형식](https://api.slack.com/types/file)만 미리 볼 수 있습니다.

   * (조건부 및 선택 사항) 다른 사용자의 추가 액세스 요청에 대한 권한을 부여하거나 무시하려면 **[!UICONTROL 부여]** 또는 **[!UICONTROL 무시]**&#x200B;를 클릭합니다.\

     알림 내에서 결정하는 모든 결정에 대해 [!DNL Workfront]에 작업이 완료되었다는 확인 메시지가 표시됩니다.
