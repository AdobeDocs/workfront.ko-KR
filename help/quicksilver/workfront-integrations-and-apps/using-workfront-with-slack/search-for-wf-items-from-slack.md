---
product-area: workfront-integrations
navigation-topic: workfront-for-slack
title: ' [!DNL Adobe Workfront] 에서  [!DNL Slack]개 항목 검색'
description: 설치된  [!DNL Adobe Workfront] 앱에서  [!DNL Slack], if your instance of Slack has had the [!DNL Workfront] 개 항목을 검색할 수 있습니다.
author: Becky
feature: Workfront Integrations and Apps
exl-id: 85821f21-d4fd-4f28-bd7a-0c109a4433a8
source-git-commit: 6178cabbf021fbf92bd8795c5c2bd0346801d64d
workflow-type: tm+mt
source-wordcount: '213'
ht-degree: 6%

---

# [!DNL Adobe Workfront]에서 [!DNL Slack]개 항목 검색

[!DNL Adobe Workfront] 인스턴스에 [!DNL Slack] 앱이 설치된 경우 [!DNL Slack]에서 [!DNL Workfront]개 항목을 검색할 수 있습니다.

[!DNL Workfront]을(를) 사용하여 [!DNL Slack]을(를) 구성하는 방법에 대한 자세한 내용은 [구성 [!DNL Adobe Workfront] for [!DNL Slack]](../../workfront-integrations-and-apps/using-workfront-with-slack/configure-workfront-for-slack.md)을(를) 참조하십시오.

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

[!DNL Workfront]에서 [!DNL Slack]개 항목을 검색하려면 먼저 다음을 수행해야 합니다.

* [!DNL Workfront]에 대해 [!DNL Slack] 구성\
   [!DNL Workfront for Slack] 구성에 대한 지침은 [구성 [!DNL Adobe Workfront for Slack]](../../workfront-integrations-and-apps/using-workfront-with-slack/configure-workfront-for-slack.md)을 참조하십시오.

## [!DNL Workfront]에서 [!DNL Slack]개 항목 검색:

1. [!DNL Slack] 인스턴스에 로그인하고 [!DNL Workfront]에서 [!DNL Slack]에 로그인합니다.\
   [!DNL Workfront]에서 [!DNL Slack]에 로그인하는 방법에 대한 자세한 내용은 [!DNL Workfront]Access[!DNL Slack]from[의 &quot; [!DNL Adobe Workfront] 에서  [!DNL Slack]](../../workfront-integrations-and-apps/using-workfront-with-slack/access-workfront-from-slack.md)에 로그인&quot; 섹션을 참조하십시오.

1. 채널에서 메시지 필드에 다음 명령 중 하나를 입력하십시오.

   `/workfront search <keyword>`

   또는

   `/wf search <keyword>`

   >[!NOTE]
   >
   >명령은 대/소문자를 구분합니다. 키워드는 대/소문자를 구분하지 않으며 대괄호 또는 따옴표 없이 입력해야 합니다.

1. 표시되는 필드에서 다음 중에서 객체 유형을 선택합니다.

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
   * 메모

     한 번에 하나의 객체 유형만 선택할 수 있습니다.\
      검색 기준과 일치하는 항목의 목록이 표시됩니다.

1. 항목 이름을 클릭하여 [!DNL Workfront]에서 새 브라우저 탭에서 엽니다.
