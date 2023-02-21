---
product-area: workfront-integrations;setup
navigation-topic: workfront-for-slack
title: 구성 [!DNL Adobe Workfront] Slack
description: 통합 [!DNL Adobe Workfront] 을(를) 통해 액세스 및 생성 가능 [!DNL Workfront] Slack의 작업 항목, 승인, 즐겨찾기, 최근 항목
author: Becky
feature: Workfront Integrations and Apps
exl-id: cac75a81-26e8-4713-a6be-453943b431ab
source-git-commit: 65bfeafe67a10c72e87a02e0ece285df619fcb81
workflow-type: tm+mt
source-wordcount: '418'
ht-degree: 0%

---

# Configure [!DNL Adobe Workfront for Slack]

통합 [!DNL Adobe Workfront] with [!DNL Slack] 다음을 수행할 수 있습니다.

* 액세스 권한 [!DNL Workfront] 작업 항목, 승인, 즐겨찾기, 최근 항목 [!DNL Slack].
* 가입, 승인, 작업 할당 대상 [!DNL Slack].
* 작업 및 문제 만들기 [!DNL Slack].
* 일부 수신 [!DNL Workfront] 알림 [!DNL Slack].

사용자의 [!DNL Slack] 환경은 구성되므로 설치 및 구성할 수 있습니다 [!DNL Workfront for Slack] 네 자신이나 [!DNL Workfront] 직접 구성하려면 먼저 관리자가 설치 및 구성해야 합니다.

를 통합할 때 [!DNL Slack] 인스턴스가 있는 인스턴스 [!DNL Workfront] 사용자는 [!DNL Workfront] 공유하면서 [!DNL Slack] 채널입니다. 통합은 모든 위치에서 사용할 수 있습니다 [!DNL Slack] 환경(다음을 포함) [!DNL Slack] 모바일 앱.

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

## 사용하기 위한 사전 요구 사항 [!DNL Workfront] with [!DNL Slack]

* 다음을 수행해야 합니다. [!DNL Slack] 인스턴스.
* 사용자 [!DNL Slack] 시스템 관리자는 모든 것을 허용해야 합니다. [!DNL Slack] 설치 사용자 [!DNL Workfront for Slack].
* 다음을 수행해야 합니다. [!DNL Workfront] 의 통합 기능을 사용할 수 있는 라이선스 [!DNL Workfront].

   >[!NOTE]
   >
   >임의의 [!DNL Workfront] 라이센스 유형이 액세스 가능 [!DNL Workfront] 변환 전: [!DNL Slack]. 수행할 수 있는 작업 [!DNL Slack] 는 [!DNL Workfront] 라이선스 및 권한 수준.

의 앱 관리에 대한 자세한 정보 [!DNL Slack]를 참조하십시오. [Analysis Workspace용 앱을 관리합니다.](https://get.slack.help/hc/en-us/articles/222386767-Manage-apps-for-your-workspace)

## 설치 [!DNL Workfront for Slack]

각 [!DNL Slack] 사용자가 설치 [!DNL Workfront] 사용하기 위해 앱 자체 [!DNL Workfront] 변환 전: [!DNL Slack].

다음과 같은 방법으로 앱을 설치할 수 있습니다.

* [설치 [!DNL Workfront] 앱 외부 [!DNL Slack]](#install-the-workfront-app-outside-slack-install-the-workfront-app-outside-slack)
* [설치 [!DNL Workfront] 앱 내 [!DNL Slack]](#install-the-workfront-app-within-slack-install-the-workfront-app-within-slack)

### 설치 [!DNL Workfront] 앱 외부 [!DNL Slack] {#install-the-workfront-app-outside-slack}

설치 프로세스를 실행하고 권한을 부여하려면 아래 단계를 따르십시오 [!DNL Workfront for Slack] 설정 [!DNL Slack] 인스턴스.

>[!IMPORTANT]
>
>새 버전의 [!DNL Workfront] Slack이 릴리스된 경우 앱을 계속 사용하려면 다시 인증해야 합니다.

1. 을(를) 찾습니다 [!DNL Adobe Workfront] 의 추가 기능 [[!DNL Slack] 스토어](https://workfront.slack.com/apps/A7CLAMVNW-adobe-workfront?tab=more_info).

1. 클릭 **[!UICONTROL 여는 위치[!DNL Slack]]**.

1. 을(를) 지정하여 작업 영역에 로그인합니다 [!DNL Slack] URL 및 클릭 **[!UICONTROL 계속]**.\

1. 다음 액세스 권한을 검사합니다. [!DNL Slack] 을 요청하는 중입니다. 이 액세스 권한에 동의하는 경우 **[!UICONTROL 액세스 허용]** 권한을 부여하려면 [!DNL Workfront] 앱.

이제 액세스할 수 있습니다 [!DNL Workfront] 변환 전: [!DNL Slack]에 설명된 대로 [액세스 [!DNL Workfront] 변환 전: [!DNL Slack]](../../workfront-integrations-and-apps/using-workfront-with-slack/access-workfront-from-slack.md#viewing-all-available-commands) section in [Access [!DNL Adobe Workfront] 변환 전: [!DNL Slack]](../../workfront-integrations-and-apps/using-workfront-with-slack/access-workfront-from-slack.md).

### 설치 [!DNL Workfront] 앱 내 [!DNL Slack] {#install-the-workfront-app-within-slack}

을(를) 설치할 수 있습니다 [!DNL Workfront] 앱에서 바로 사용 [!DNL Slack] 애플리케이션:

1. 로 이동합니다. [!DNL Slack] URL.

   예: *`<YourTeamName>`.slack.com/apps*.

   또는

   을(를) 클릭합니다. **[!UICONTROL 앱 추가]** 아이콘 사용 [!DNL Slack] 인스턴스.

1. 입력 시작 *[!DNL Workfront]* 검색 필드에서 을 클릭합니다.
1. Enter 키를 누릅니다.
1. 을(를) 선택합니다 **[!DNL Workfront]** 앱.
1. 클릭 **[!UICONTROL 설정]**.

   앱 디렉토리 페이지가 표시됩니다.

1. 클릭 **[!UICONTROL 앱 사이트 방문]**.
1. 클릭 **[!UICONTROL 추가 대상[!DNL Slack]]**.
1. 단계에 따라 설치를 완료합니다.
1. 설치가 완료되면 [!DNL Workfront] 변환 전: [!DNL Slack]에 설명된 대로 [[!UICONTROL Access [!DNL Workfront] 변환 전: [!DNL Slack]]](../../workfront-integrations-and-apps/using-workfront-with-slack/access-workfront-from-slack.md#viewing-all-available-commands) section in [Access [!DNL Adobe Workfront] 변환 전: [!DNL Slack]](../../workfront-integrations-and-apps/using-workfront-with-slack/access-workfront-from-slack.md).
