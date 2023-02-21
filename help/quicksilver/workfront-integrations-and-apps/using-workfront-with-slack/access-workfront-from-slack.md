---
product-area: workfront-integrations
navigation-topic: workfront-for-slack
title: '액세스 [!DNL Adobe Workfront] 변환 전: [!DNL Slack]'
description: 통합 [!DNL Adobe Workfront] with [!DNL Slack] 액세스 권한 부여 [!DNL Workfront] Slack에서 또는 [!DNL Workfront] 슬래시 명령 사용. 통합은 모든 위치에서 사용할 수 있습니다 [!DNL Slack] 환경(다음을 포함) [!DNL Slack] 모바일 앱.
author: Becky
feature: Workfront Integrations and Apps
exl-id: 5f531217-3bd6-4156-8b9f-eabc95d4df10
source-git-commit: 65bfeafe67a10c72e87a02e0ece285df619fcb81
workflow-type: tm+mt
source-wordcount: '1075'
ht-degree: 1%

---

# 액세스 [!DNL Adobe Workfront] 변환 전: [!DNL Slack]

통합 [!DNL Adobe Workfront] with [!DNL Slack] 액세스 권한 부여 [!DNL Workfront] 변환 전: [!DNL Slack]또는 [!DNL Workfront] 슬래시 명령 사용. 통합은 모든 위치에서 사용할 수 있습니다 [!DNL Slack] 환경(다음을 포함) [!DNL Slack] 모바일 앱.

사용자 또는 사용자 [!DNL Slack] 관리자는 설치 [!DNL Workfront] 앱 [!DNL Slack] 를 사용하기 전에 인스턴스를 사용하십시오. [!DNL Workfront] 변환 전: [!DNL Slack]. 자세한 내용은 [Slack에 대한 Adobe Workfront 구성](../../workfront-integrations-and-apps/using-workfront-with-slack/configure-workfront-for-slack.md).

## 슬래시 명령 {#about-slash-commands}

사용 시 [!DNL Slack]: 메시지 필드 내에 메시지를 입력합니다. 메시지를 슬래시로 시작하면 명령이 되고 간단한 메시지와 다르게 동작합니다. 명령은 [!DNL Slack] 를 눌러 작업을 수행합니다.

에 액세스할 수 있습니다 [!DNL Workfront] 인스턴스: [!DNL Slack] 슬래시 명령을 [!DNL Slack] 채널.

에서 슬래시 명령을 사용할 때는 다음 사항을 기억하십시오 [!DNL Slack] 액세스 권한 [!DNL Workfront]:

* 슬래시 명령은 대/소문자를 구분합니다.
* 다음 명령 [!DNL Workfront] 입력하는 채널에 관계없이 만 표시됩니다.
* 명령은 항상 `/workfront` 또는 `/wf`, 뒤에 공백 및 수행할 작업 이름이 옵니다. [!DNL Workfront].

   이는 명령이 [!DNL Workfront] 앱. 다음 명령 [!DNL Workfront] 작업을 이미 구성한 경우에만 [!DNL Workfront] 앱 [!DNL Slack] 인스턴스.

Slack에서 실행할 수 있는 모든 명령 목록 [!DNL Workfront]를 참조하십시오. [액세스 [!DNL Workfront] 의 슬래시 명령에서 [!DNL Slack]](#access-workfront-from-a-slash-command-in-slack-access-workfront-from-a-slash-command-in-slack).

## 에 로그인합니다. [!DNL Workfront] 변환 전: [!DNL Slack] {#log-in-to-workfront-from-slack}

Slack의 메시지 필드에 명령을 입력하면 로그인하라는 메시지가 표시됩니다 [!DNL Workfront] 먼저\
전체 목록 [!DNL Workfront] 명령 [!DNL Slack]를 참조하고 [액세스 [!DNL Workfront] 의 슬래시 명령에서 [!DNL Slack]](#access-workfront-from-a-slash-command-in-slack-access-workfront-from-a-slash-command-in-slack) 섹션에 자세히 설명되어 있습니다.

에 로그인하려면 [!DNL Workfront] 변환 전: [!DNL Slack]:

1. 에 로그인합니다. [!DNL Slack] 인스턴스.
1. 채널에서 다음 명령 중 하나를 입력합니다.\
   `/workfront log in`

   또는

   `/wf log in`

1. 을(를) 클릭합니다. [!DNL Workfront] **[!UICONTROL 로그인]** 링크에 표시됩니다.\
   필드가 포함된 새 탭이 열립니다 [!DNL Workfront] 자격 증명.

1. 화면의 지침에 따라 로그인하십시오 [!DNL Workfront] 고급 인증, OAuth 2.0 또는 SAML(Security Assertion Markup Language) URL을 사용합니다.

   >[!NOTE]
   >
   >* 호스트의 호스트를 입력하라는 메시지가 표시되면 [!DNL Workfront] 다음 형식으로 입력하십시오. *yourCompany&#39;sDomain.my.workfront.com*. 일반적으로 회사의 도메인은 회사의 이름입니다.
   >* Enhanced Authentication 은 [!DNL Workfront] 관리자가 이 통합을 위해 이 통합을 사용하도록 설정합니다.



   에 대한 구성 페이지 [!DNL Workfront] 알림 [!DNL Slack] 엽니다.

1. (선택 사항) 임의 항목 비활성화 [!DNL Workfront] 수신하지 않으려는 알림 [!DNL Slack].

   구성에 대한 자세한 내용 [!DNL Workfront] 설정 [!DNL Slack]를 참조하고 [설정 구성](#configure-settings-configure-settings) 이 문서의 섹션

1. 다음 위치로 돌아갑니다 [!DNL Slack] 채널.

   로그인되어 있습니다. [!DNL Workfront] 다음 [!DNL Slack] 인스턴스.

## 액세스 [!DNL Workfront] 변환 전: [!DNL Slack]

* [슬래시 명령](#about-slash-commands-about-slash-commands)
* [액세스 [!DNL Workfront] 공유 링크를 통해 [!DNL Slack]](#access-workfront-from-a-shared-link-in-slack-access-workfront-from-a-shared-link-in-slack)

## 액세스 [!DNL Workfront] 의 슬래시 명령에서 [!DNL Slack] {#access-workfront-from-a-slash-command-in-slack}

1. 에 로그인합니다. [!DNL Slack] 인스턴스 및 로그인 [!DNL Workfront] 변환 전: [!DNL Slack].\
   로그인하는 방법에 대한 자세한 정보 [!DNL Workfront] 변환 전: [!DNL Slack]를 참조하십시오. [에 로그인합니다. [!DNL Workfront] 변환 전: [!DNL Slack]](#log-in-to-workfront-from-slack-log-in-to-workfront-from-slack)

1. 채널에서 메시지 필드에 다음 명령을 입력합니다.

   `/workfront help`

   또는

   `/wf help`

1. 다음 명령 중에서 선택합니다.

   * `/wf home`

      작업, 문제 및 승인 목록에 액세스할 수 있는 단추를 표시합니다. 버튼 중 하나를 클릭하면 각 목록에 있는 처음 20개 항목이 표시됩니다. [!DNL Slack].

      관리에 대한 자세한 정보 [!DNL Workfront] 작업 항목 [!DNL Slack]를 참조하십시오. [다음 위치에서 작업 및 승인 관리 [!DNL Slack]](../../workfront-integrations-and-apps/using-workfront-with-slack/manage-your-work-and-approvals-from-slack.md).

   * `/wf add task <TaskName>`

      작업 이름을 다음과 같이 포함합니다. [!DNL Workfront] 인터페이스.

      작업 추가 [!DNL Workfront].

      작업 추가에 대한 자세한 정보 [!DNL Workfront] Slack에서 &quot;작업 만들기: [!DNL Slack]&quot; 섹션 [작업 및 문제 만들기 [!DNL Slack]](../../workfront-integrations-and-apps/using-workfront-with-slack/create-tasks-and-issues-from-slack.md).

   * `/wf add issue <Issue Name>`

      문제에 표시될 문제 이름을 [!DNL Workfront] 인터페이스.

      에 문제 추가 [!DNL Workfront]

      에 문제를 추가하는 방법에 대한 자세한 정보 [!DNL Workfront] 변환 전: [!DNL Slack]에서 &quot;문제 만들기&quot;를 참조하십시오 [!DNL Slack]&quot; 섹션 [작업 및 문제 만들기 [!DNL Slack]](../../workfront-integrations-and-apps/using-workfront-with-slack/create-tasks-and-issues-from-slack.md).

   * `/wf favorites`

      목록 표시 [!DNL Workfront] 즐겨찾기.

      즐겨찾기 액세스에 대한 자세한 내용은 [!DNL Slack]를 참조하고 [액세스 [!UICONTROL 즐겨찾기] 목록 [!DNL Slack]](../../workfront-integrations-and-apps/using-workfront-with-slack/access-favorites-and-recent-items-from-slack.md#accessing-favorites) 의 섹션 [즐겨찾기 및 최근 항목에 액세스 [!DNL Slack]](../../workfront-integrations-and-apps/using-workfront-with-slack/access-favorites-and-recent-items-from-slack.md) 문서.

   * `/wf recent`

      에서 가장 최근에 액세스한 항목 목록을 표시합니다 [!DNL Workfront].

      최근 항목 액세스에 대한 자세한 내용은 [!DNL Slack]를 참조하고 [액세스 [!UICONTROL 최근 항목] 목록 [!DNL Slack]](../../workfront-integrations-and-apps/using-workfront-with-slack/access-favorites-and-recent-items-from-slack.md#accessing-recent-items) section in the [[!UICONTROL Access your favorites] 및 [!UICONTROL 최근 항목 [!DNL Slack]]](../../workfront-integrations-and-apps/using-workfront-with-slack/access-favorites-and-recent-items-from-slack.md) 문서.

   * `wf tasks`

      작업 목록을 표시합니다.

      작업 관리에 대한 자세한 내용은 [!DNL Slack]를 보려면 &quot;다음 위치에서 작업 관리&quot;를 참조하십시오. [!DNL Slack]&quot; 섹션 [작업 및 승인 관리 [!DNL Slack]](../../workfront-integrations-and-apps/using-workfront-with-slack/manage-your-work-and-approvals-from-slack.md).

   * `/wf issues`

      문제 목록을 표시합니다.

      문제 관리에 대한 자세한 내용은 [!DNL Slack]를 참조하려면 &quot;다음 위치에서 문제 관리&quot;를 참조하십시오. [!DNL Slack]&quot; 섹션 [작업 및 승인 관리 [!DNL Slack]](../../workfront-integrations-and-apps/using-workfront-with-slack/manage-your-work-and-approvals-from-slack.md).

   * `/wf approvals` 를 표시합니다 [!DNL Workfront] 승인\.

      승인을 관리하는 방법에 대한 자세한 내용은 [!DNL Slack]를 보려면 &quot;다음 위치에서 승인 관리&quot;를 참조하십시오. [!DNL Slack]&quot; 섹션 [다음 위치에서 작업 및 승인 관리 [!DNL Slack]](../../workfront-integrations-and-apps/using-workfront-with-slack/manage-your-work-and-approvals-from-slack.md).

   * `/wf search <keyword>`

      키워드 포함.

      특정 키워드를 검색합니다. 다음 유형 객체를 검색할 수 있습니다.

      * 프로젝트
      * 작업
      * 문제
      * 보고서
      * 사람
      * 템플릿
      * 문서
      * 포트폴리오
      * 프로그램
      * 대시보드
      * 회사
      * 참고  \

         검색 방법에 대한 자세한 내용 [!DNL Slack]를 참조하십시오. [검색 대상 [!DNL Adobe Workfront] Slack의 항목](../../workfront-integrations-and-apps/using-workfront-with-slack/search-for-wf-items-from-slack.md).
   * `/wf log in`

      에 로그인합니다. [!DNL Workfront] 변환 전: [!DNL Slack].

   * `/wf log out `

      로그아웃합니다. [!DNL Workfront] 변환 전: [!DNL Slack]. 에 계속 로그인되어 있습니다. [!DNL Workfront] 별거이면 [!DNL Workfront] 인스턴스가 다른 애플리케이션의 다른 브라우저 탭에서 열립니다.
   * `/wf settings`

      구성에 대한 액세스 권한을 제공합니다. [!DNL Workfront] 설정 [!DNL Slack].

      구성에 대한 자세한 내용 [!DNL Workfront] Slack의 설정은 [설정 구성](#configure-settings-configure-settings).

   * `/wf help`
에 대한 전체 명령 목록을 표시합니다. [!DNL Workfront].


   * `Visit Workfront Help`: 를 엽니다. [!UICONTROL Slack] 섹션에 [!DNL Workfront] 새 브라우저 탭의 도움말 사이트


1. (선택 사항) 명령의 메시지를 삭제하려면 명령을 포함하는 Slack 메시지의 오른쪽 위 모서리에서 마우스를 가져간 후 를 &#x200B; 클릭합니다&#x200B;**[!UICONTROL 메시지 작업 표시]**&#x200B;를 클릭한 다음 **[!UICONTROL 메시지 삭제]**.

1. (선택 사항 및 조건부) **[!UICONTROL 삭제]** 이 메시지를 삭제할지 확인하려면

### 액세스 [!DNL Workfront] 공유 링크를 통해 [!DNL Slack] {#access-workfront-from-a-shared-link-in-slack}

액세스할 수 있습니다 [!DNL Workfront] 링크에서 사용자와 공유되는 객체에 대한 객체 [!DNL Slack].

액세스 방법에 대한 자세한 정보 [!DNL Workfront] 공유 링크에서 다음을 참조하십시오. [액세스 [!DNL Adobe Workfront] 의 공유 링크의 개체 [!DNL Slack]](../../workfront-integrations-and-apps/using-workfront-with-slack/access-wf-objects-from-shared-linked-in-slack.md).

## 설정 구성 {#configure-settings}

1. 내부 [!DNL Slack] 메시지 필드에 다음 명령을 입력합니다.

   `/workfront settings`

   또는

   `/wf settings`

   모든 설정은 기본적으로 활성화되어 있습니다.

1. Workfront에 대한 설정을 비활성화하려면 다음 옵션 중에서 선택 취소합니다.

   * 에서 **[!UICONTROL 일반 설정]** 영역, 비활성화 **[!UICONTROL 붙여넣을 때 [!DNL Workfront] 의 URL [!DNL Slack] 채널, 추가 설명, 기한 또는 요청자 이름 표시]**&#x200B;원하지 않는 경우 &#x200B; 설정 [!DNL Slack] 에 대한 추가 정보를 추가하려면 [!DNL Workfront] 개체의 URL을 공유할 때 [!UICONTROL Slack].

   * 에서 **[!UICONTROL 알림 설정]** 영역에서 Workfront의 수신을 중지할 알림을 비활성화합니다.\

      수신에 대한 정보 [!DNL Workfront] 알림 [!DNL Slack]를 참조하십시오. [수신 [!DNL Adobe Workfront] 알림 [!DNL Slack]](../../workfront-integrations-and-apps/using-workfront-with-slack/receive-workfront-notifications-in-slack.md).

## 로그아웃됨 [!DNL Workfront] 변환 전: [!DNL Slack]

1. 내부 [!DNL Slack] 메시지 필드에 다음 명령을 입력합니다.\
   `/workfront log out` 또는\
   `/wf log out`\
   로그아웃되었다는 확인 메시지가 표시됩니다 [!DNL Workfront].\
   에 계속 로그인되어 있습니다. [!DNL Workfront] 별거이면 [!DNL Workfront] 인스턴스가 다른 애플리케이션의 다른 브라우저 탭에서 열립니다.
