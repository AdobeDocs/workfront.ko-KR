---
product-area: workfront-integrations;setup
navigation-topic: workfront-for-slack
title: Slack에 대해  [!DNL Adobe Workfront] 구성
description: ' [!DNL Adobe Workfront] Slack과 통합하여 Slack에서  [!DNL Workfront] 작업 항목, 승인, 즐겨찾기, 최근 항목에 액세스하고 만들 수 있습니다.'
author: Becky
feature: Workfront Integrations and Apps
exl-id: cac75a81-26e8-4713-a6be-453943b431ab
source-git-commit: 6178cabbf021fbf92bd8795c5c2bd0346801d64d
workflow-type: tm+mt
source-wordcount: '406'
ht-degree: 0%

---

# [!DNL Adobe Workfront for Slack] 구성

[!DNL Adobe Workfront]을(를) [!DNL Slack]과(와) 통합하여 다음 작업을 수행할 수 있습니다.

* [!DNL Workfront]에서 [!DNL Slack] 작업 항목, 승인, 즐겨찾기, 최근 항목에 액세스합니다.
* [!DNL Slack]에서 작업 구독, 승인, 할당
* [!DNL Slack]에서 작업 및 문제를 만듭니다.
* [!DNL Workfront]에서 [!DNL Slack]개의 알림을 받습니다.

[!DNL Slack] 환경을 구성하는 방법에 따라 [!DNL Workfront for Slack]을(를) 직접 설치하고 구성할 수 있습니다. 또는 직접 구성하기 전에 [!DNL Workfront] 관리자가 먼저 설치하고 구성해야 합니다.

[!DNL Slack] 인스턴스를 [!DNL Workfront] 사용자와 통합하면 사용자가 [!DNL Workfront] 채널 내에서 공동 작업하는 동안 [!DNL Slack]을(를) 사용할 수 있습니다. [!DNL Slack] 모바일 앱을 포함한 모든 [!DNL Slack] 환경에서 통합을 사용할 수 있습니다. ## 액세스 요구 사항

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

## [!DNL Workfront]에서 [!DNL Slack]을(를) 사용하기 위한 필수 구성 요소

* [!DNL Slack] 인스턴스가 있어야 합니다.
* [!DNL Slack] 시스템 관리자는 모든 [!DNL Slack] 사용자가 [!DNL Workfront for Slack]을(를) 설치하도록 허용해야 합니다.
* [!DNL Workfront]의 통합 기능을 사용하려면 [!DNL Workfront] 라이선스가 있어야 합니다.

  >[!NOTE]
  >
  >[!DNL Workfront] 라이선스 유형의 사용자는 [!DNL Workfront]에서 [!DNL Slack]에 액세스할 수 있습니다. [!DNL Slack]에서 수행할 수 있는 작업은 [!DNL Workfront] 라이선스 및 권한 수준으로 제한됩니다.

[!DNL Slack]에서 앱을 관리하는 방법에 대한 자세한 내용은 [Workspace용 앱 관리](https://get.slack.help/hc/en-us/articles/222386767-Manage-apps-for-your-workspace)를 참조하십시오.

## [!DNL Workfront for Slack] 설치

[!DNL Slack]에서 [!DNL Workfront]을(를) 사용하려면 각 [!DNL Workfront] 사용자는 [!DNL Slack] 앱 자체를 설치해야 합니다.

다음과 같은 방법으로 앱을 설치할 수 있습니다.

* [ [!DNL Workfront] 외부 앱 설치 [!DNL Slack]](#install-the-workfront-app-outside-slack-install-the-workfront-app-outside-slack)
* [ [!DNL Workfront]  내에  [!DNL Slack]앱 설치](#install-the-workfront-app-within-slack-install-the-workfront-app-within-slack)

### [!DNL Workfront] 외부에 [!DNL Slack] 앱 설치 {#install-the-workfront-app-outside-slack}

설치 프로세스를 실행하고 [!DNL Workfront for Slack] 인스턴스에서 [!DNL Slack]을(를) 승인하려면 아래 단계를 따르십시오.

>[!IMPORTANT]
>
>Slack용 [!DNL Workfront]의 새 버전이 출시되면 앱을 계속 사용하려면 앱을 다시 승인해야 합니다.

1. [!DNL Adobe Workfront]스토어[[!DNL Slack] 에서 ](https://workfront.slack.com/apps/A7CLAMVNW-adobe-workfront?tab=more_info) 추가 기능을 찾습니다.

1. **[!UICONTROL 에서[!DNL Slack]]**&#x200B;열기를 클릭합니다.

1. [!DNL Slack] URL을 지정하고 **[!UICONTROL 계속]**&#x200B;을 클릭하여 작업 영역에 로그인합니다.\

1. [!DNL Slack]이(가) 요청하는 액세스를 검사합니다. 이 액세스에 동의하면 **[!UICONTROL 액세스 허용]**&#x200B;을 클릭하여 [!DNL Workfront] 앱을 인증하세요.

이제 [!DNL Workfront]액세스[!DNL Slack]출처[출처 [!DNL Workfront] 에 설명된 대로  [!DNL Slack]](../../workfront-integrations-and-apps/using-workfront-with-slack/access-workfront-from-slack.md#viewing-all-available-commands) section in [Access [!DNL Adobe Workfront] 에서  [!DNL Slack]](../../workfront-integrations-and-apps/using-workfront-with-slack/access-workfront-from-slack.md)에 액세스할 수 있습니다.

### [!DNL Workfront] 내에 [!DNL Slack] 앱 설치 {#install-the-workfront-app-within-slack}

[!DNL Workfront] 응용 프로그램에서 직접 [!DNL Slack] 앱을 설치할 수 있습니다.

1. [!DNL Slack] URL로 이동합니다.

   예: *`<YourTeamName>`.slack.com/apps*.

   또는

   **[!UICONTROL 인스턴스에서]**&#x200B;앱 추가[!DNL Slack] 아이콘을 클릭합니다.

1. 검색 필드에 *[!DNL Workfront]*&#x200B;을(를) 입력하십시오.
1. Enter 키를 누릅니다.
1. **[!DNL Workfront]** 앱을 선택하십시오.
1. **[!UICONTROL 설정]**&#x200B;을 클릭합니다.

   [앱 디렉토리] 페이지가 표시됩니다.

1. **[!UICONTROL 앱 사이트 방문]**&#x200B;을 클릭합니다.
1. **[!UICONTROL [!DNL Slack]]**&#x200B;에 추가를 클릭합니다.
1. 다음 단계에 따라 설치를 완료합니다.
1. 설치가 완료되면 [!DNL Workfront][!UICONTROL 액세스[!DNL Slack]from[from [!DNL Workfront] 에 설명된 대로  [!DNL Slack]]](../../workfront-integrations-and-apps/using-workfront-with-slack/access-workfront-from-slack.md#viewing-all-available-commands) section in [Access [!DNL Adobe Workfront] 에서  [!DNL Slack]](../../workfront-integrations-and-apps/using-workfront-with-slack/access-workfront-from-slack.md)에 액세스할 수 있습니다.
