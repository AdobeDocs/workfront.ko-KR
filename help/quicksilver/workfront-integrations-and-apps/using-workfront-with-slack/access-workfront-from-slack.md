---
product-area: workfront-integrations
navigation-topic: workfront-for-slack
title: ' [!DNL Adobe Workfront] 에서  [!DNL Slack]액세스'
description: ' [!DNL Adobe Workfront] 을(를)  [!DNL Slack] 과(와) 통합하여 Slack에서  [!DNL Workfront] 에 액세스하거나 [!DNL Workfront] 슬래시 명령을 사용하여 특정 작업을 수행할 수 있습니다. 통합은  [!DNL Slack] 모바일 앱을 포함한  [!DNL Slack] 환경에서 사용할 수 있습니다.'
author: Becky
feature: Workfront Integrations and Apps
exl-id: 5f531217-3bd6-4156-8b9f-eabc95d4df10
source-git-commit: 6178cabbf021fbf92bd8795c5c2bd0346801d64d
workflow-type: tm+mt
source-wordcount: '1106'
ht-degree: 1%

---

# [!DNL Adobe Workfront]에서 [!DNL Slack] 액세스

[!DNL Adobe Workfront]을(를) [!DNL Slack]과(와) 통합하면 [!DNL Workfront]에서 [!DNL Slack]에 액세스하거나 슬래시 명령을 사용하여 [!DNL Workfront]에서 특정 작업을 수행할 수 있습니다. [!DNL Slack] 모바일 앱을 포함한 모든 [!DNL Slack] 환경에서 통합을 사용할 수 있습니다.

[!DNL Slack]의 [!DNL Workfront]을(를) 사용하려면 사용자 또는 [!DNL Slack] 관리자가 [!DNL Workfront] 인스턴스에 [!DNL Slack] 앱을 설치해야 합니다. 자세한 내용은 [Slack용 Adobe Workfront 구성](../../workfront-integrations-and-apps/using-workfront-with-slack/configure-workfront-for-slack.md)을 참조하십시오.

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

## 슬래시 명령 정보 {#about-slash-commands}

[!DNL Slack]을(를) 사용하는 경우 메시지 필드 내부에 메시지를 입력합니다. 슬래시로 메시지를 시작하면 명령이 되고 단순 메시지와는 다르게 동작합니다. 명령은 [!DNL Slack]에게 작업을 수행하도록 지시합니다.

[!DNL Workfront] 채널에서 슬래시 명령을 입력하여 [!DNL Slack]에서 [!DNL Slack] 인스턴스에 액세스할 수 있습니다.

[!DNL Slack]에서 슬래시 명령을 사용하여 [!DNL Workfront]에 액세스할 때는 다음 사항을 기억하십시오.

* 슬래시 명령은 대/소문자를 구분합니다.
* [!DNL Workfront]에 대한 명령은 입력하려는 채널에 관계없이 사용자에게만 표시됩니다.
* 명령은 항상 `/workfront` 또는 `/wf`(으)로 시작해야 하며 그 뒤에는 공백과 [!DNL Workfront]에서 수행할 작업의 이름이 와야 합니다.

  이는 명령이 [!DNL Workfront] 앱용임을 나타냅니다. [!DNL Workfront]에 대한 명령은 [!DNL Workfront] 인스턴스로 [!DNL Slack] 앱을 이미 구성한 경우에만 작동합니다.

[!DNL Workfront]에 대해 Slack에서 실행할 수 있는 모든 명령 목록을 보려면 [Access [!DNL Workfront] 의 슬래시 명령에서 [!DNL Slack]](#access-workfront-from-a-slash-command-in-slack-access-workfront-from-a-slash-command-in-slack)를 참조하십시오.

## [!DNL Workfront]에서 [!DNL Slack]에 로그인 {#log-in-to-workfront-from-slack}

Slack의 메시지 필드에 명령을 입력하면 먼저 [!DNL Workfront]에 로그인하라는 메시지가 표시됩니다.\
[!DNL Workfront]의 [!DNL Slack] 명령에 대한 전체 목록을 보려면 이 문서의 [ 섹션에 있는  [!DNL Workfront] 슬래시 명령에서  [!DNL Slack]](#access-workfront-from-a-slash-command-in-slack-access-workfront-from-a-slash-command-in-slack)액세스를 참조하십시오.

[!DNL Workfront]에서 [!DNL Slack]에 로그인하려면:

1. [!DNL Slack] 인스턴스에 로그인합니다.
1. 채널에서 다음 명령 중 하나를 입력합니다.\
   `/workfront log in`

   또는

   `/wf log in`

1. 응답에 표시된 [!DNL Workfront] **[!UICONTROL 로그인]** 링크를 클릭합니다.\
   [!DNL Workfront] 자격 증명에 대한 필드가 있는 새 탭이 열립니다.

1. 메시지에 따라 향상된 인증, OAuth 2.0 또는 SAML(Security Assertion Markup Language) URL을 사용하여 [!DNL Workfront]에 로그인합니다.

   >[!NOTE]
   >
   >* [!DNL Workfront] 계정의 호스트를 입력하라는 메시지가 표시되면 *yourCompany&#39;sDomain.my.workfront.com* 형식을 사용하여 입력하십시오. 회사의 도메인은 일반적으로 회사의 이름입니다.
   >* 향상된 인증은 [!DNL Workfront] 관리자가 이 통합에 사용하도록 설정할 때까지 사용할 수 없습니다.


   [!DNL Workfront]의 [!DNL Slack] 알림에 대한 구성 페이지가 열립니다.

1. (선택 사항) [!DNL Workfront]에서 수신하지 않을 [!DNL Slack] 알림을 비활성화합니다.

   [!DNL Workfront]에 대한 [!DNL Slack] 설정 구성에 대한 자세한 내용은 이 문서의 [설정 구성](#configure-settings-configure-settings) 섹션을 참조하십시오

1. [!DNL Slack] 채널로 다시 이동합니다.

   [!DNL Workfront] 인스턴스에서 [!DNL Slack]에 로그인했습니다.

## [!DNL Workfront]에서 [!DNL Slack] 액세스

* [슬래시 명령 정보](#about-slash-commands-about-slash-commands)
* [ [!DNL Workfront] 의 공유 링크에서  [!DNL Slack]액세스](#access-workfront-from-a-shared-link-in-slack-access-workfront-from-a-shared-link-in-slack)

## [!DNL Workfront]의 슬래시 명령에서 [!DNL Slack]에 액세스 {#access-workfront-from-a-slash-command-in-slack}

1. [!DNL Slack] 인스턴스에 로그인하고 [!DNL Workfront]에서 [!DNL Slack]에 로그인합니다.\
   [!DNL Workfront]에서 [!DNL Slack]에 로그인하는 방법에 대한 자세한 내용은 [다음에 로그인 [!DNL Workfront] 부터 [!DNL Slack]](#log-in-to-workfront-from-slack-log-in-to-workfront-from-slack)을 참조하세요.

1. 모든 채널에서 메시지 필드에 다음 명령을 입력합니다.

   `/workfront help`

   또는

   `/wf help`

1. 다음 명령 중에서 선택합니다.

   * `/wf home`

     작업, 문제 및 승인 목록에 액세스할 수 있는 단추를 표시합니다. 단추 중 하나를 클릭하면 [!DNL Slack]에서 각 목록의 처음 20개 항목이 표시됩니다.

     [!DNL Workfront]에서 [!DNL Slack] 작업 항목을 관리하는 방법에 대한 자세한 내용은 [작업 및 승인 관리 [!DNL Slack]](../../workfront-integrations-and-apps/using-workfront-with-slack/manage-your-work-and-approvals-from-slack.md)를 참조하십시오.

   * `/wf add task <TaskName>`

     [!DNL Workfront] 인터페이스에 표시되는 작업 이름을 포함합니다.

     [!DNL Workfront]에 작업을 추가합니다.

     Slack에서 [!DNL Workfront]에 작업을 추가하는 방법에 대한 자세한 내용은 [!DNL Slack]작업 및 문제 만들기[의 &quot; [!DNL Slack]](../../workfront-integrations-and-apps/using-workfront-with-slack/create-tasks-and-issues-from-slack.md)에서 작업 만들기&quot; 섹션을 참조하십시오.

   * `/wf add issue <Issue Name>`

     [!DNL Workfront] 인터페이스에 표시되는 문제의 이름을 포함합니다.

     [!DNL Workfront]에 문제 추가

     [!DNL Workfront]에서 [!DNL Slack]에 문제를 추가하는 방법에 대한 자세한 내용은 [!DNL Slack]작업 및 문제 만들기[의 &quot; [!DNL Slack]](../../workfront-integrations-and-apps/using-workfront-with-slack/create-tasks-and-issues-from-slack.md)에서 문제 만들기&quot; 섹션을 참조하십시오.

   * `/wf favorites`

     [!DNL Workfront] 즐겨찾기 목록을 표시합니다.

     [!DNL Slack]에서 즐겨찾기에 액세스하는 방법에 대한 자세한 내용은 [즐겨찾기 및 최근 항목 액세스[!UICONTROL  문서의 ]다음 위치에서  [!DNL Slack]](../../workfront-integrations-and-apps/using-workfront-with-slack/access-favorites-and-recent-items-from-slack.md#accessing-favorites)즐겨찾기[ 목록 액세스 [!DNL Slack]](../../workfront-integrations-and-apps/using-workfront-with-slack/access-favorites-and-recent-items-from-slack.md) 섹션을 참조하십시오.

   * `/wf recent`

     [!DNL Workfront]에서 가장 최근에 액세스한 항목 목록을 표시합니다.

     [!DNL Slack]에서 최근 항목 액세스에 대한 자세한 내용은 [다음에서 [!UICONTROL 최근 항목 액세스] 목록 [!DNL Slack]](../../workfront-integrations-and-apps/using-workfront-with-slack/access-favorites-and-recent-items-from-slack.md#accessing-recent-items) section in the [[!UICONTROL Access your favorites] 및 [!UICONTROL 최근 항목 [!DNL Slack]]](../../workfront-integrations-and-apps/using-workfront-with-slack/access-favorites-and-recent-items-from-slack.md) 문서를 참조하십시오.

   * `wf tasks`

     작업 목록을 표시합니다.

     [!DNL Slack]에서 작업 관리에 대한 자세한 내용은 [!DNL Slack]작업 및 승인 관리[의 &quot; [!DNL Slack]](../../workfront-integrations-and-apps/using-workfront-with-slack/manage-your-work-and-approvals-from-slack.md)에서 작업 관리&quot; 섹션을 참조하십시오.

   * `/wf issues`

     문제 목록을 표시합니다.

     [!DNL Slack]에서 문제를 관리하는 방법에 대한 자세한 내용은 [!DNL Slack]작업 및 승인 관리[의 &quot; [!DNL Slack]](../../workfront-integrations-and-apps/using-workfront-with-slack/manage-your-work-and-approvals-from-slack.md)에서 문제 관리&quot; 섹션을 참조하십시오.

   * `/wf approvals`에 [!DNL Workfront] 승인이 표시됩니다.\

     [!DNL Slack]의 승인 관리에 대한 자세한 내용은 [!DNL Slack]작업 및 승인 관리[의 &quot; [!DNL Slack]](../../workfront-integrations-and-apps/using-workfront-with-slack/manage-your-work-and-approvals-from-slack.md)에서 승인 관리&quot; 섹션을 참조하십시오.

   * `/wf search <keyword>`

     키워드를 포함합니다.

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
      * 참고 \

        [!DNL Slack]에서 검색하는 방법에 대한 자세한 내용은 [Slack에서  [!DNL Adobe Workfront] 항목 검색](../../workfront-integrations-and-apps/using-workfront-with-slack/search-for-wf-items-from-slack.md)을 참조하십시오.
   * `/wf log in`

     [!DNL Workfront]에서 [!DNL Slack]에 로그인합니다.

   * `/wf log out `

     [!DNL Workfront]에서 [!DNL Slack]에서 로그아웃합니다. 다른 응용 프로그램의 다른 브라우저 탭에서 별도의 [!DNL Workfront] 인스턴스가 열려 있는 경우 [!DNL Workfront]에 로그인한 상태로 유지됩니다.
   * `/wf settings`

     [!DNL Workfront]에서 [!DNL Slack] 설정을 구성할 수 있는 액세스 권한을 제공합니다.

     Slack에서 [!DNL Workfront] 설정을 구성하는 방법에 대한 자세한 내용은 [설정 구성](#configure-settings-configure-settings)을 참조하십시오.

   * `/wf help`
[!DNL Workfront]에 대한 전체 명령 목록을 표시합니다.


   * `Visit Workfront Help`: 새 브라우저 탭에서 [!UICONTROL  도움말 사이트의 ]Slack[!DNL Workfront] 섹션을 엽니다.


1. (선택 사항) 명령의 메시지를 삭제하려면 해당 명령이 포함된 Slack 메시지의 오른쪽 상단 모서리로 마우스를 가져간 후 {&#x200B;0}메시지 동작 표시&#x200B;**[!UICONTROL 를 클릭한 다음]**&#x200B;메시지 삭제&#x200B;**[!UICONTROL 를 클릭합니다.]**

1. (선택 사항 및 조건부) **[!UICONTROL 삭제]**&#x200B;를 클릭하여 이 메시지 삭제를 확인합니다.

### [!DNL Workfront]의 공유 링크에서 [!DNL Slack]에 액세스 {#access-workfront-from-a-shared-link-in-slack}

[!DNL Workfront]에서 사용자와 공유된 개체에 연결된 링크에서 [!DNL Slack]개의 개체에 액세스할 수 있습니다.

공유 링크에서 [!DNL Workfront]에 액세스하는 방법에 대한 자세한 내용은 [공유 링크에서  [!DNL Adobe Workfront] 개체 [!DNL Slack]](../../workfront-integrations-and-apps/using-workfront-with-slack/access-wf-objects-from-shared-linked-in-slack.md)를 참조하십시오.

## 설정 구성 {#configure-settings}

1. [!DNL Slack] 메시지 필드 안에 다음 명령을 입력하십시오.

   `/workfront settings`

   또는

   `/wf settings`

   모든 설정은 기본적으로 활성화되어 있습니다.

1. Workfront 설정을 비활성화하려면 다음 옵션 중에서 선택을 취소합니다.

   * **[!UICONTROL 일반 설정]** 영역에서 **[!UICONTROL URL을 [!DNL Workfront] 채널에 붙여 넣을 때 [!DNL Slack]Slack]**&#x200B;의 개체에 URL을 공유할 때 [!DNL Slack]에서 [!DNL Workfront] 개체에 대한 추가 정보를 추가하지 않도록 하려면 [!UICONTROL 추가 설명, 기한 또는 요청자 이름{5&#x200B;} 설정을 사용하지 않도록 설정하십시오.]

   * **[!UICONTROL 알림 설정]** 영역에서 Workfront에서 수신을 중지할 알림을 비활성화하십시오.\

     [!DNL Workfront]에서 [!DNL Slack]개의 알림을 받는 방법에 대한 자세한 내용은 [수신 [!DNL Adobe Workfront] 알림 [!DNL Slack]](../../workfront-integrations-and-apps/using-workfront-with-slack/receive-workfront-notifications-in-slack.md)을 참조하세요.

## [!DNL Workfront]에서 [!DNL Slack]에서 로그아웃

1. [!DNL Slack] 메시지 필드 안에 다음 명령을 입력하십시오.\
   `/workfront log out` 또는\
   `/wf log out`\
   [!DNL Workfront]에서 로그아웃되었다는 확인 메시지가 표시됩니다.\
   다른 응용 프로그램의 다른 브라우저 탭에서 별도의 [!DNL Workfront] 인스턴스가 열려 있는 경우 [!DNL Workfront]에 로그인한 상태로 유지됩니다.
