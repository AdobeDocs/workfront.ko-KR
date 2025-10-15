---
product-area: workfront-integrations;agile-and-teams;user-management
navigation-topic: workfront-for-microsoft-teams
title: ' [!DNL Adobe Workfront] 팀에서  [!DNL Microsoft] 액세스'
description: Workfront 봇 채널 또는 다른 팀 채널에 명령을 입력하여 [!DNL Adobe Workfront] from [!DNL Microsoft Teams] 에 액세스하고 [!DNL Workfront] 에서 여러 작업을 수행할 수 있습니다.
author: Becky
feature: Workfront Integrations and Apps
exl-id: a12277e8-2c2e-4b53-990f-6ee9a6541492
source-git-commit: 4cf780aa1b1221cd6ff8e6ce58fbb7d3621f7fa9
workflow-type: tm+mt
source-wordcount: '516'
ht-degree: 1%

---

# [!DNL Adobe Workfront]에서 [!DNL Microsoft Teams] 액세스

<!--Audited: 01/2024-->

>[!IMPORTANT]
>
>[Microsoft이 새 팀 클라이언트로 전환](https://learn.microsoft.com/en-us/microsoftteams/teams-classic-client-end-of-availability)됨에 따라 클래식 팀 클라이언트는 2025년 7월 1일 이후에 더 이상 사용할 수 없습니다. Workfront과 같은 Microsoft Teams 및 통합 앱을 계속 사용하려면 이 날짜 이전에 고객이 New Teams 클라이언트로 전환해야 합니다.
>
>이제 업데이트된 Workfront 통합을 사용할 수 있으며 새 팀 경험과 완전히 호환됩니다. 대부분의 경우 사용자가 전환되면 Workfront이 자동으로 표시됩니다. 그렇지 않은 경우 Microsoft Teams App Store에서 수동으로 통합을 설치할 수 있습니다. 새 Teams 클라이언트에서 Workfront 통합을 설치하거나 확인하려면 [Microsoft Teams용 설치 [!DNL Adobe Workfront] 를 참조하십시오](/help/quicksilver/workfront-integrations-and-apps/using-workfront-with-microsoft-teams/install-workfront-ms-teams.md).


[!DNL Adobe Workfront] 봇 채널 또는 다른 팀 채널에 명령을 입력하여 [!DNL Microsoft Teams]에서 [!DNL Workfront]에 액세스하고 [!DNL Workfront]에서 여러 작업을 수행할 수 있습니다.

[!DNL Workfront]의 [!DNL Microsoft Teams]에서 다음을 수행할 수 있습니다.

* 프로젝트, 작업 또는 문제 검색
* 개인 작업 만들기
* 알림에 응답
* 문서 승인 관리

이러한 작업을 수행하기 위해 [!DNL Microsoft Teams]에서 사용하는 명령은 [!DNL Workfront]에 액세스하려는 채널에 따라 다릅니다.

>[!NOTE]
>
>[!DNL Microsoft Teams]은(는) 더 이상 [!DNL Internet Explorer]을(를) 지원하지 않습니다. [!DNL Adobe Workfront for Microsoft Teams integration]을(를) 사용하려면 [!DNL Internet Explorer] 이외의 웹 브라우저를 사용해야 합니다.

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
   <td> <p>표준</p>
   <p>작업 이상</p> </td> 
  </tr> 
 </tbody> 
</table>

자세한 내용은 [Workfront 설명서의 액세스 요구 사항](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)을 참조하십시오.

+++

## 전제 조건

다음 조건이 충족되는 경우 [!DNL Adobe Workfront]의 [!DNL Microsoft Teams]에서 개인 작업을 만들 수 있습니다.

* 팀 소유자가 귀하의 팀에 대해 [!DNL Workfront for Microsoft Teams]을(를) 설치하고 구성했습니다.
* [!DNL Workfront]에서 [!DNL Microsoft Teams]에 로그인했습니다.

## [!DNL Workfront] 봇 채팅 채널에서 [!DNL Workfront]에 액세스

Workfront에 로그인해야 합니다.

1. **[!DNL Workfront]** 봇 채팅 채널을 엽니다.
1. 텍스트 필드 아래의 **[!DNL Workfront]** 아이콘을 클릭하여 검색 상자를 표시합니다.

   ![teams_search_box_in_the_bot_channel.PNG](assets/teams-search-box-in-the-bot-channel-350x456.png)

1. 프로젝트, 작업 또는 문제의 이름을 입력하십시오.

   항목 검색에 대한 자세한 내용은 [항목 검색 및 공유 [!DNL Adobe Workfront] 항목 위치 [!DNL Microsoft Teams]](../../workfront-integrations-and-apps/using-workfront-with-microsoft-teams/search-for-and-share-wf-items-in-ms-teams.md) in the article [Search for and share [!DNL Adobe Workfront] 항목 위치 [!DNL Microsoft Teams]](../../workfront-integrations-and-apps/using-workfront-with-microsoft-teams/search-for-and-share-wf-items-in-ms-teams.md) 섹션을 참조하십시오.

1. **[!UICONTROL 여기에 질문을 입력하십시오]** 필드를 클릭합니다.

   ![ms_teams_type_your_questions_here_and_what_can_I_do_fields.png](assets/ms-teams-type-your-questions-here-and-what-can-i-do-fields-350x71.png)

1. 다음 중 하나를 수행하십시오.

   * **[!UICONTROL 을(를) 클릭합니다.]**&#x200B;을(를) 만든 다음 **[!UICONTROL 로그인]** 또는 **[!UICONTROL 의]**&#x200B;로그아웃[!DNL Workfront]을(를) 하거나 **[!UICONTROL 에서]**&#x200B;새 작업[!DNL Workfront]&#x200B;(개인 작업)을 만들거나 사용 가능한 명령을 나열하여 **[!UICONTROL 도움말]**&#x200B;을 받으세요.

   * [!DNL Workfront]여기에 질문을 입력하십시오&#x200B;**[!UICONTROL 필드에 명령을 입력하여]**&#x200B;에 직접 액세스할 수 있습니다.

     명령은 대/소문자를 구분하지 않습니다.

     [!DNL Workfront] 봇이 [!DNL Workfront] 봇 채팅 채널에서 요청에 응답합니다.

## 팀 채널에서 [!DNL Workfront]에 액세스

Workfront에 로그인해야 합니다.

1. 팀 채널을 열고 **@[!DNL Workfront]**&#x200B;을(를) 입력한 다음 **[!DNL Workfront].**&#x200B;을(를) 선택하십시오.

1. 프로젝트, 작업 또는 문제를 검색하려면 **[!UICONTROL 검색]**&#x200B;을 클릭하십시오.

   항목 검색에 대한 자세한 내용은 [항목 검색 및 공유 [!DNL Adobe Workfront] 항목 위치 [!DNL Microsoft Teams]](../../workfront-integrations-and-apps/using-workfront-with-microsoft-teams/search-for-and-share-wf-items-in-ms-teams.md) section in the [Search for and share [!DNL Adobe Workfront] 항목 위치 [!DNL Microsoft Teams]](../../workfront-integrations-and-apps/using-workfront-with-microsoft-teams/search-for-and-share-wf-items-in-ms-teams.md) 문서를 참조하십시오.

1. Workfront에서 이러한 작업을 수행하려면 다음 명령을 입력합니다.\
   명령은 대/소문자를 구분하지 않습니다.

   * **[!UICONTROL 에 로그인하려면]**&#x200B;로그인[!DNL Workfront]
   * Workfront에서 로그아웃할 **[!DNL Log out]**
   * 새 개인 작업을 만들려면 **[!DNL New task]**

     [!DNL Microsoft Teams]에서 작업을 만드는 방법에 대한 자세한 내용은 [만들기 [!DNL Adobe Workfront] 작업 [!DNL Microsoft Teams]](../../workfront-integrations-and-apps/using-workfront-with-microsoft-teams/create-workfront-tasks-from-ms-teams.md)을 참조하세요.

   * 사용 가능한 모든 명령 목록을 보려면 **[!UICONTROL 도움말]**&#x200B;을 보세요.

     [!DNL Workfront] 봇이 [!DNL Workfront] 봇 채팅 채널에서 요청에 응답합니다.

1. [!DNL Workfront] 봇 채팅 채널로 이동하여 [!DNL Workfront]에 액세스하고 요청을 완료합니다.
