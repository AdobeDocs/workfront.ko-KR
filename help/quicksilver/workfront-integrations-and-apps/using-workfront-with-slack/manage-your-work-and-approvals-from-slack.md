---
product-area: workfront-integrations;projects
navigation-topic: workfront-for-slack
title: Slack에서 작업 및 승인 관리
description: 홈 작업 목록에 액세스하고, 작업 및 문제에 대한 작업을 검토 및 동의하고, Slack에서 직접 승인을 검토하거나 결정할 수 있습니다.
author: Becky
feature: Workfront Integrations and Apps
exl-id: 802a2f16-d827-455e-9e49-f58f4c5fc482
source-git-commit: 6178cabbf021fbf92bd8795c5c2bd0346801d64d
workflow-type: tm+mt
source-wordcount: '907'
ht-degree: 1%

---

# [!DNL Slack]에서 작업 및 승인 관리

[!DNL Adobe Workfront for Slack]을(를) 설치한 후 다음을 수행할 수 있습니다.

* [!UICONTROL 에서 ]홈[!DNL Slack] 항목의 액세스 목록
* [!DNL Slack]의 작업 및 문제를 검토하고 수락합니다.
* [!DNL Slack]의 승인 검토 및 결정

[!DNL Workfront]을(를) 사용하여 [!DNL Slack]을(를) 구성하는 방법에 대한 자세한 내용은 [구성 [!DNL Adobe Workfront for Slack]](../../workfront-integrations-and-apps/using-workfront-with-slack/configure-workfront-for-slack.md)을(를) 참조하십시오.

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

[!DNL Slack]에서 작업 및 승인을 관리하려면 먼저 다음을 수행해야 합니다.

* [!DNL Workfront for Slack] 구성\
  [!DNL Workfront for Slack] 구성에 대한 지침은 [구성 [!DNL Adobe Workfront for Slack]](../../workfront-integrations-and-apps/using-workfront-with-slack/configure-workfront-for-slack.md)을 참조하십시오.

## [!DNL Slack]에서 작업 관리

1. [!DNL Slack] 인스턴스에 로그인하고 [!DNL Workfront]에서 [!DNL Slack]에 로그인합니다.\
   [!DNL Workfront]에서 [!DNL Slack]에 로그인하는 방법에 대한 자세한 내용은 [!DNL Workfront]Access[!DNL Slack]from[의 &quot; [!DNL Adobe Workfront] 에서  [!DNL Slack]](../../workfront-integrations-and-apps/using-workfront-with-slack/access-workfront-from-slack.md)에 로그인&quot; 섹션을 참조하십시오.

1. 모든 채널에서 메시지 필드에 다음 명령을 입력합니다.

   `/workfront home`

   >[!NOTE]
   >
   >* 명령은 대/소문자를 구분합니다.
   >* `/wf` 대신 `/workfront`(으)로 명령을 시작할 수 있습니다.

   작업, 문제 및 승인 목록에 액세스할 수 있는 버튼이 표시됩니다. 단추 중 하나를 클릭하면 [!DNL Slack]에서 각 목록의 처음 20개 항목이 표시됩니다.

1. (선택 사항) 모든 작업을 표시하려면 **[!UICONTROL 작업]**&#x200B;을 클릭합니다.

   [!DNL Slack]의 작업 관리에 대한 자세한 내용은 [다음 항목에서 작업 관리 [!DNL Slack]](#manage-your-tasks-from-slack-manage-your-tasks-from-slack)를 참조하십시오.

1. (선택 사항) **[!UICONTROL 문제]**&#x200B;를 클릭하여 모든 문제를 표시합니다.

   [!DNL Slack]의 문제 관리에 대한 자세한 내용은 [다음 항목에서 문제 관리 [!DNL Slack]](#manage-your-issues-from-slack-manage-your-issues-from-slack)를 참조하십시오.

1. (선택 사항) **[!UICONTROL 승인]**&#x200B;을 클릭하여 결정을 기다리는 모든 승인을 표시합니다.\
   [!DNL Slack]에서 승인을 관리하는 방법에 대한 자세한 내용은 [승인 관리 [!DNL Slack]](#manage-your-approvals-from-slack-manage-your-approvals-from-slack)를 참조하십시오.

## [!DNL Slack]에서 작업 관리 {#manage-your-tasks-from-slack}

1. [!DNL Slack] 인스턴스에 로그인하고 [!DNL Workfront]에서 [!DNL Slack]에 로그인합니다.\
   [!DNL Workfront]에서 [!DNL Slack]에 로그인하는 방법에 대한 자세한 내용은 [!DNL Workfront]Access[!DNL Slack]from[의 &quot; [!DNL Adobe Workfront] 에서  [!DNL Slack]](../../workfront-integrations-and-apps/using-workfront-with-slack/access-workfront-from-slack.md)에 로그인&quot; 섹션을 참조하십시오.

1. 채널에서 메시지 필드에 다음 명령 중 하나를 입력하십시오.

   `/workfront home`을(를) 클릭한 다음 **[!UICONTROL 작업]**&#x200B;을(를) 클릭합니다.

   또는

   `/workfront tasks`

   >[!NOTE]
   >
   >* 명령은 대/소문자를 구분합니다.
   >* `/wf` 대신 `/workfront`(으)로 명령을 시작할 수 있습니다.

   목록의 처음 20개 작업이 표시됩니다.

1. 추가 작업을 표시하려면 **[!UICONTROL +`<remaining number>` 자세히]**&#x200B;를 클릭하십시오.
1. 작업 항목에 대한 다음 정보를 검토하는 것이 좋습니다.

   * **[!UICONTROL 이름]**
   * **[!UICONTROL 프로젝트 이름]** 또는 **[!DNL Parent Object Name]**

   * 작업 항목의 **[!DNL Planned Completion Date]**&#x200B;입니다.
   * **[!DNL Assigned By Name]**: 작업을 귀하에게 할당한 사용자의 이름입니다.
   * **[!UICONTROL 상태]**

1. (선택 사항) 항목 이름을 클릭하여 별도의 브라우저 탭에서 Workfront으로 엽니다.
1. (선택 사항) **[!UICONTROL 상태]** 필드에서 새 상태를 선택합니다.
1. (선택 사항) **[!UICONTROL 로그 시간]**&#x200B;을 클릭한 다음 **[!UICONTROL 시간 유형]** 및 시간을 선택하여 항목에 시간을 기록합니다.

   >[!NOTE]
   >
   >* 최대 12시간 30분까지 전체 또는 30분 단위로 시간만 기록할 수 있습니다.
   >* 기록된 시간은 오늘로 입력됩니다. [!DNL Slack]의 과거 또는 미래 날짜에 대한 시간을 기록할 수 없습니다.

   시간이 기록되었다는 확인 메시지가 표시됩니다.

1. (선택 사항) 작업을 수락하려면 **[!UICONTROL 작업]**&#x200B;을 클릭하세요. [!UICONTROL 작업] 단추가 사라집니다.

## [!DNL Slack]에서 문제 관리 {#manage-your-issues-from-slack}

1. [!DNL Slack] 인스턴스에 로그인하고 [!DNL Workfront]에서 [!DNL Slack]에 로그인합니다.\
   [!DNL Workfront]에서 [!DNL Slack]에 로그인하는 방법에 대한 자세한 내용은 [다음에 로그인 [!DNL Workfront] 부터 [!DNL Slack]](../../workfront-integrations-and-apps/using-workfront-with-slack/access-workfront-from-slack.md#logging-in-to-workfront) section in [Access [!DNL Adobe Workfront] 부터 [!DNL Slack]](../../workfront-integrations-and-apps/using-workfront-with-slack/access-workfront-from-slack.md)을 참조하십시오.

1. 채널에서 메시지 필드에 다음 명령 중 하나를 입력하십시오.

   `/workfront home`을(를) 클릭한 다음 **[!UICONTROL 문제]**&#x200B;를 클릭합니다.

   또는

   `/workfront issues`

   >[!NOTE]
   >
   >* 명령은 대/소문자를 구분합니다.
   >* `/wf` 대신 `/workfront`(으)로 명령을 시작할 수 있습니다.

   목록의 처음 20개 문제가 표시됩니다.

1. 추가 항목을 표시하려면 **[!UICONTROL + 나머지 `<number>` 추가]**&#x200B;을(를) 클릭합니다.
1. 작업 항목에 대한 다음 정보를 검토하는 것이 좋습니다.

   * **[!UICONTROL 이름]**
   * **[!UICONTROL 프로젝트]** 이름 또는 상위 개체 이름
   * **[!UICONTROL 기한:]** 일자: 작업 항목의 계획된 완료 일자입니다.
   * **[!DNL Requested by]** 이름: 기본 담당자(문제) 또는 할당한 사용자(작업)입니다.

1. (선택 사항) 문제 이름을 클릭하여 별도의 브라우저 탭에서 Workfront으로 엽니다.
1. (선택 사항) 아직 수락하지 않은 문제에 대한 작업을 시작하려면 **[!DNL Work on it]**&#x200B;을(를) 클릭하십시오.

   [!UICONTROL 작업] 단추가 사라집니다.

## [!DNL Slack]에서 승인 관리 {#manage-your-approvals-from-slack}

1. [!DNL Slack] 인스턴스에 로그인하고 [!DNL Workfront]에서 [!DNL Slack]에 로그인합니다.\
   [!DNL Workfront]에서 [!DNL Slack]에 로그인하는 방법에 대한 자세한 내용은 [!DNL Workfront]Access[!DNL Slack]from[의 &quot; [!DNL Adobe Workfront] 에서  [!DNL Slack]](../../workfront-integrations-and-apps/using-workfront-with-slack/access-workfront-from-slack.md)에 로그인&quot; 섹션을 참조하십시오.

1. 채널에서 메시지 필드에 다음 명령 중 하나를 입력하십시오.

   `/workfront home`을(를) 클릭한 다음 **[!UICONTROL 승인]**&#x200B;을 클릭합니다.

   또는

   `/workfront approvals`

   >[!NOTE]
   >
   >* 명령은 대/소문자를 구분합니다.
   >* `/wf` 대신 `/workfront`(으)로 명령을 시작할 수 있습니다.

   **[!UICONTROL 승인]** 목록의 처음 20개 항목이 표시됩니다. 항목을 요청한 사용자의 이름이나 항목이 속한 프로젝트의 이름과 같은 항목에 대한 추가 정보도 표시됩니다.

1. 추가 항목을 표시하려면 **[!UICONTROL + 나머지 `<number>` 추가]**&#x200B;을(를) 클릭합니다.

1. 다음 객체에 대한 승인 관리를 고려하십시오.

   * **프로젝트**

     프로젝트의 상태 변경을 수락하거나 거부하려면 **[!UICONTROL 승인]** 또는 **[!UICONTROL 거부]**&#x200B;을 클릭하세요.

   * **작업**

     작업의 상태 변경을 수락하거나 거부하려면 **[!UICONTROL 승인]** 또는 **[!UICONTROL 거부]**&#x200B;를 클릭하십시오.

   * **문제**

     문제의 상태 변경을 수락하거나 거부하려면 **[!UICONTROL 승인]** 또는 **[!DNL Reject]**&#x200B;을(를) 클릭하십시오.

   * **문서**

     문서를 승인하려면 **[!UICONTROL 승인]**, 거부하려면 **[!UICONTROL 거부]**, 승인하지만 문서에 추가 변경이 필요함을 나타내려면 **[!UICONTROL 변경]**&#x200B;을 클릭합니다.\
     (선택 사항) 문서 축소판 위로 마우스를 가져가면 돋보기를 클릭하고 문서를 미리 볼 수 있습니다.

   * **증명**&#x200B;증명 이름을 클릭하여 [!DNL Workfront]에서 별도의 탭에서 열고 승인을 관리합니다.
   * **액세스 요청**

     요청된 개체에 향상된 권한을 부여하려면 **[!UICONTROL 액세스 권한 부여]**&#x200B;를 클릭하고, 추가 액세스 요청을 무시하려면 **[!UICONTROL 무시]**&#x200B;를 클릭하십시오.

1. (선택 사항) 승인을 위해 제출한 개체의 이름을 클릭하여 [!DNL Workfront]에서 새 브라우저 탭에서 엽니다.
