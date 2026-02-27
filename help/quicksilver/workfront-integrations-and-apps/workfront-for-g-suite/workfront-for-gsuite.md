---
content-type: overview;reference
product-area: workfront-integrations
keywords: google,doc,document,sheet,slide
navigation-topic: workfront-integrations-navigation-topic
title: Google Workspace용 Adobe Workfront
description: Google Workspace용 Adobe Workfront을 사용하면 가장 중요한 작업에 연결할 수 있으며 Gmail, Google Calendar 및 Google 드라이브 내에서 다른 사용자와 공동 작업을 수행할 수 있습니다. 이러한 애플리케이션을 종료하지 않고 이메일 요청 또는 작업 업데이트를 캡처하여 Workfront에 추가할 수 있습니다. 기한, 우선 순위, 문서, 업데이트 및 추가 컨텍스트 등 Workfront에서 일어나고 있는 일을 상자에 입력하지 않고도 확인할 수 있습니다. 승인 결정을 내리거나, 댓글에 답글을 달거나, 새 작업 요청을 수락할 수 있습니다. 또한 이메일을 개인 프로젝트 작업으로 변환하거나 작업과 우선 순위를 다른 사람에게 할당할 수 있습니다.
author: Becky
feature: Workfront Integrations and Apps
recommendations: noDisplay, noCatalog
exl-id: dfced3e9-0338-446e-bf70-fa5d07f3ac1f
source-git-commit: 228fd22f1894689c0d256270350cc82954901641
workflow-type: tm+mt
source-wordcount: '215'
ht-degree: 0%

---

# [!DNL Adobe Workfront for Google Workspace]

>[!IMPORTANT]
>
>보다 안정적이고 확장 가능한 통합을 제공하기 위해 Workfront 자동화 및 통합(Fusion)을 사용하는 현대적이고 유연한 통합 접근 방식으로 전환했습니다. 이 전환 프로세스의 일부로 다음 Google Workspace 기능용 Workfront **을(를) 더 이상 사용할 수 없습니다**.
>
>* Workfront 내에서 Google Workspace 기능 액세스
>
>* Gmail 또는 Google Calendar 사이트 패널에서 Workfront 작업 보기 및 관리
>
>조직의 Google Workspace 통합 요구 사항에 맞게 Workfront 자동화 및 통합을 사용하는 것이 좋습니다.
>
>Workfront 자동화 및 통합에 대한 개요는 [Adobe Workfront Fusion 개요](https://experienceleague.adobe.com/en/docs/workfront-fusion/using/get-started-with-fusion/understand-workfront-fusion/workfront-fusion-overview)를 참조하십시오.
>
>Google Workspace용 Workfront 자동화 및 통합 모듈의 특정 기능에 대한 자세한 내용은 [Gmail 모듈](https://experienceleague.adobe.com/en/docs/workfront-fusion/using/references/apps-and-their-modules/third-party-app-connectors/gmail-modules) 및 [Google 달력 모듈](https://experienceleague.adobe.com/en/docs/workfront-fusion/using/references/apps-and-their-modules/third-party-app-connectors/google-calendar-modules)을 참조하십시오.

<!--

[!DNL Adobe Workfront for Google Workspace] connects you to your most important work and allows you to collaborate with others while staying within [!DNL Gmail], [!DNL Google Calendar], and [!DNL Google Drive]. Without leaving these applications, you can capture emailed requests or work updates and add them to [!DNL Workfront]. You can check what's happening in [!DNL Workfront], including due dates, priority, documents, updates and additional context, without leaving your inbox. You can make approval decisions, reply to comments, or accept new work requests. And you can convert your emails to either personal project tasks or assign work and priority to others.

These Help articles can help you get started using [!DNL Workfront for Google Workspace]:

* [Install [!DNL Adobe Workfront for Google Workspace]](../../workfront-integrations-and-apps/workfront-for-g-suite/install-workfront-for-gsuite.md)
* [Privacy and permissions in Workfront for Google Workspace](../../workfront-integrations-and-apps/workfront-for-g-suite/privacy-and-permissions-in-g-suite.md)
* [Log in and out of [!DNL Adobe Workfront for Google Workspace]](../../workfront-integrations-and-apps/workfront-for-g-suite/log-in-and-out-wf-for-gsuite.md)

These explain how to manage [!DNL Workfront] objects without leaving [!DNL Google Workspace]:

* [Access [!DNL Adobe Workfront] Home content from [!DNL Google Workspace]](../../workfront-integrations-and-apps/workfront-for-g-suite/access-wf-home-content-from-g-suite.md)
* [Update an [!DNL Adobe Workfront] object from [!DNL Google Workspace]](../../workfront-integrations-and-apps/workfront-for-g-suite/update-a-workfront-object-in-gsuite.md)
* [View and manage documents from [!DNL Google Workspace]](../../workfront-integrations-and-apps/workfront-for-g-suite/view-and-manage-documents-in-gsuite.md)
* [View and manage [!DNL Adobe Workfront] object details from [!UICONTROL Google Workspace]](../../workfront-integrations-and-apps/workfront-for-g-suite/view-manage-work-item-details-in-gsuite.md)
* [View [!DNL Adobe Workfront] object updates from [!UICONTROL Google Workspace]](../../workfront-integrations-and-apps/workfront-for-g-suite/view-object-updates-in-gsuite.md)

These explain how to view and respond to details about a work item when you receive a [!DNL Workfront] notification email.

* [Manage [!DNL Adobe Workfront] notification details from [!DNL Google Workspace]](../../workfront-integrations-and-apps/workfront-for-g-suite/manage-wf-email-notification-details-in-gsuite.md)
* [Reply to a [!DNL Adobe Workfront] update notification from [!DNL Google Workspace]](../../workfront-integrations-and-apps/workfront-for-g-suite/reply-to-wf-update-notification-from-gsuite.md)

These explain how you can create [!DNL Workfront] objects and updates using content from non-[!DNL Workfront] emails:

* [Turn [!DNL Google Workspace] emails into [!DNL Adobe Workfront] objects and updates](../../workfront-integrations-and-apps/workfront-for-g-suite/turn-gsuite-emails-into-wf-objects-and-updates.md)
* [Create an [!DNL Adobe Workfront] task in [!DNL Google Workspace] using email content](../../workfront-integrations-and-apps/workfront-for-g-suite/create-wf-task-in-gsuite-using-email-content.md)
* [Create an [!DNL Adobe Workfront] issue in [!DNL Google Workspace] using email content](../../workfront-integrations-and-apps/workfront-for-g-suite/create-wf-issue-in-g-suite-using-email-content.md)
* [Update an [!DNL Adobe Workfront] item from [!DNL Google Workspace] using email content](../../workfront-integrations-and-apps/workfront-for-g-suite/update-wf-item-using-email-content.md)

-->
