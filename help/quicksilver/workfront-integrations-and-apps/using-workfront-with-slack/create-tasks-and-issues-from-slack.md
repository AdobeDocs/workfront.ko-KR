---
product-area: workfront-integrations;projects
navigation-topic: workfront-for-slack
title: Slack에서 작업 및 문제 만들기
description: Slack용  [!DNL Adobe Workfront] 을(를) 설치 및 구성한 후에는 Slack에서 작업 및 문제를 만들어 Workfront의 프로젝트와 연결할 수 있습니다.
author: Becky
feature: Workfront Integrations and Apps
exl-id: cf4a514a-fe69-4c2f-8e35-5738dfaab24e
source-git-commit: 6178cabbf021fbf92bd8795c5c2bd0346801d64d
workflow-type: tm+mt
source-wordcount: '431'
ht-degree: 0%

---

# [!DNL Slack]에서 작업 및 문제 만들기

[!DNL Adobe Workfront for Slack]을(를) 설치 및 구성한 후 [!DNL Slack]에서 작업 및 문제를 만들고 [!DNL Workfront]의 프로젝트와 연결할 수 있습니다.

[!DNL Workfront]을(를) 사용하여 [!DNL Slack]을(를) 구성하는 방법에 대한 자세한 내용은 [구성 [!DNL Adobe Workfront for Slack]](../../workfront-integrations-and-apps/using-workfront-with-slack/configure-workfront-for-slack.md)을(를) 참조하십시오.

액세스 수준에서 작업 및 문제를 만들 수 있는 액세스 권한이 있어야 하며 연결 중인 프로젝트에 대해 [!UICONTROL 기여] 권한이 있어야 합니다.

액세스 수준에 대한 자세한 내용은 [액세스 수준 개요](../../administration-and-setup/add-users/access-levels-and-object-permissions/access-levels-overview.md)를 참조하십시오. 개체에 대한 사용 권한에 대한 자세한 내용은 [개체에 대한 사용 권한 공유 개요](../../workfront-basics/grant-and-request-access-to-objects/sharing-permissions-on-objects-overview.md)를 참조하십시오.

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

[!DNL Slack]에서 작업 및 문제를 만들려면 먼저 다음을 수행해야 합니다.

* Slack에 대해 [!DNL Workfront] 구성\
   [!DNL Workfront for Slack] 구성에 대한 지침은 [구성 [!DNL Adobe Workfront for Slack]](../../workfront-integrations-and-apps/using-workfront-with-slack/configure-workfront-for-slack.md)을 참조하십시오.

## [!DNL Slack]에서 작업 만들기

1. [!DNL Slack] 인스턴스에 로그인하고 [!DNL Workfront]에서 [!DNL Slack]에 로그인합니다.\
   [!DNL Slack]에서 Workfront에 로그인하는 방법에 대한 자세한 내용은 [!DNL Workfront]액세스[!DNL Slack]시작[의 &quot; [!DNL Adobe Workfront] 에서  [!DNL Slack]](../../workfront-integrations-and-apps/using-workfront-with-slack/access-workfront-from-slack.md)에 로그인&quot; 섹션을 참조하십시오.

1. 모든 채널에서 메시지 필드에 다음 명령을 입력합니다.

   `/workfront add task <Task Name>`

   >[!NOTE]
   >
   >명령은 대/소문자를 구분합니다. `/wf` 대신 `/workfront`(으)로 명령을 시작할 수 있습니다.
   >  
   >작업 이름은 [!DNL Workfront] 인터페이스에 나타나는 대로 대괄호 또는 따옴표 없이 입력해야 합니다.

1. (선택 사항) 새 작업을 연결할 프로젝트의 이름을 입력하고 목록에 나타나면 선택합니다.\
   선택한 프로젝트에 작업이 추가되었다는 확인 메시지가 표시됩니다.
1. (선택 사항) 확인 메시지에서 작업 이름을 클릭하여 새 브라우저 탭에서 [!DNL Workfront]에 엽니다.

## [!DNL Slack]에서 문제 만들기

1. [!DNL Slack] 인스턴스에 로그인하고 [!DNL Workfront]에서 [!DNL Slack]에 로그인합니다.\
   [!DNL Workfront]에서 [!DNL Slack]에 로그인하는 방법에 대한 자세한 내용은 [!DNL Workfront]Access[!DNL Slack]from[의 &quot; [!DNL Adobe Workfront] 에서  [!DNL Slack]](../../workfront-integrations-and-apps/using-workfront-with-slack/access-workfront-from-slack.md)에 로그인&quot; 섹션을 참조하십시오.

1. 모든 채널에서 메시지 필드에 다음 명령을 입력합니다.

   `/workfront add issue <Issue Name>`

   >[!NOTE]
   >
   >명령은 대/소문자를 구분합니다. &#39;/workfront&#39; 대신 &#39;/wf&#39;로 명령을 시작할 수 있습니다. \
   >문제 이름은 [!DNL Workfront] 인터페이스에 나타나는 대로 대괄호 또는 따옴표 없이 입력해야 합니다.

1. (선택 사항) 새 문제를 연결할 프로젝트의 이름을 입력하고 목록에 나타나면 선택합니다.\
   선택한 프로젝트에 문제가 추가되었다는 확인 메시지가 표시됩니다.
1. (선택 사항) 확인 메시지에서 문제의 이름을 클릭하여 새 브라우저 탭에서 [!DNL Workfront]에 엽니다.
