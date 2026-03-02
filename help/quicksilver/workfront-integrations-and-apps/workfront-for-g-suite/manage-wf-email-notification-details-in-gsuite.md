---
product-area: workfront-integrations
keywords: google,doc,document,sheet,slide
navigation-topic: workfront-for-g-suite
title: Google Workspace에서  [!DNL Adobe Workfront] 알림 세부 정보 관리
description: Google Workspace에서 Adobe [!DNL Workfront] 이(가) 보낸 알림 이메일을 열면 받은 편지함에서 관련 작업 항목 세부 정보를 보고 응답할 수 있습니다. 요청 승인과 같은 작업을 사용할 수 있는 경우 Workfront for Google Workspace에서 직접 이러한 작업을 수행할 수 있습니다.
author: Becky
feature: Workfront Integrations and Apps
recommendations: noDisplay, noCatalog
exl-id: d5ca31d8-3667-4405-a523-3dc248a94746
source-git-commit: ddd1c964c4c885f71dfa30d1790cfbc6e26d6781
workflow-type: tm+mt
source-wordcount: '169'
ht-degree: 0%

---

# [!DNL Adobe Workfront]에서 [!DNL Google Workspace] 알림 세부 정보 관리

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

In [!DNL Google Workspace], when you open a notification email [!DNL Adobe Workfront] has sent, you can view the associated work item details and respond without leaving your [!UICONTROL Inbox]. If actions are available, such as approving a request, you can perform those actions directly from [!DNL Workfront for Google Workspace].

>[!NOTE]
>
> [!DNL Workfront for Google Workspace] supports almost every type of email notification you can receive from [!DNL Workfront] (about 120 different types). [!UICONTROL Daily digest] emails sent from [!DNL Workfront] do not appear in [!DNL Workfront for Google Workspace]. For information about the [!DNL Workfront] email notification types, see [Modify your own email notifications](../../workfront-basics/using-notifications/activate-or-deactivate-your-own-event-notifications.md).

## Access requirements

+++ Expand to view access requirements for the functionality in this article.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront package</td> 
   <td> <p>Any</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront license</td> 
   <td> <p>Standard</p><p>Work or higher</p>
  </tr> 
 </tbody> 
</table>

For information, see [Access requirements in Workfront documentation](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md). 

+++

## Prerequisites

Before you can manage notification details from [!DNL Google Workspace], you must

* Install [!DNL Workfront for Google Workspace]\
   For instructions, see [Install [!DNL Adobe Workfront for Google Workspace]](../../workfront-integrations-and-apps/workfront-for-g-suite/install-workfront-for-gsuite.md).

## Manage [!DNL Adobe Workfront] notification details from [!DNL Google Workspace]

1. If the [!DNL Workfront for Google Workspace] panel is not displayed, click the [!DNL Workfront] icon ![Workfront icon](assets/wf-lion-icon.png) in the [!DNL Google Workspace] add-ons sidebar at the far-right of the page.
1. In [!DNL Google Workspace], open a [!DNL Workfront] notification email.
1. Click **[!UICONTROL View all updates]** if it is displayed near the top of the panel.
1. Click **[!UICONTROL Details]**.
1. Click any available options.

   The options that might display relate to the type of email notification you have opened. For example, if it's an email notification asking you to approve a task, you see **[!UICONTROL Approve]** and **[!UICONTROL Reject]** instead of options such as **[!UICONTROL Work on It]** or **[!UICONTROL Done]**:

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <thead> 
     <tr> 
      <th>Type of email notification</th> 
      <th>Action</th> 
     </tr> 
    </thead> 
    <tbody> 
     <tr> 
      <td>Task or issue</td> 
      <td><strong>[!UICONTROL Approve]</strong> it, <strong>[!UICONTROL Reject]</strong> it, <strong>[!UICONTROL Grant]</strong> access to it, <strong>[!UICONTROL Ignore]</strong> a request for access to it, <strong>[!UICONTROL Work on it]</strong>, or click an option to indicate that you are <strong>[!UICONTROL Done]</strong> with it</td> 
     </tr> 
     <tr> 
      <td>Project</td> 
      <td><strong>[!UICONTROL Approve]</strong> it, <strong>[!UICONTROL Reject]</strong> it, <strong>[!UICONTROL Grant]</strong> access to it, or <strong>[!UICONTROL Ignore]</strong> a request for access to it</td> 
     </tr> 
     <tr> 
      <td>Document</td> 
      <td><strong>[!UICONTROL Approve]</strong> it, <strong>[!UICONTROL Reject]</strong> it, <strong>[!UICONTROL Grant]</strong> access to it, or <strong>[!UICONTROL Ignore]</strong> a request for access to it</td> 
     </tr> 
     <tr> 
      <td>Update </td> 
      <td> <p>View any part of the entire list of updates for the item so that you have the context you need to <strong>[!UICONTROL Post]</strong> a new update or a <strong>[!UICONTROL Reply]</strong>. You can click <strong>[!UICONTROL Notify]</strong> to alert particular users about your reply. </p> <p>For more information, see <a href="../../workfront-integrations-and-apps/workfront-for-g-suite/reply-to-wf-update-notification-from-gsuite.md" class="MCXref xref">Reply to a [!DNL Adobe Workfront] update notification from [!DNL Google Workspace]</a>.</p> </td> 
     </tr> 
     <tr> 
      <td>Approval request</td> 
      <td><strong>[!UICONTROL Approve]</strong> or <strong>[!UICONTROL Reject]</strong> it (you can change your mind by clicking the other option), download it, view its owner, or view its reference number</td> 
     </tr> 
     <tr> 
      <td>A change in a project's status</td> 
      <td> View all the current information about the project, including any custom forms. </td> 
     </tr> 
    </tbody> 
   </table>

   -->
