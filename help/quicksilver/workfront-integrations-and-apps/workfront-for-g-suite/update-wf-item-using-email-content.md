---
product-area: workfront-integrations;projects
keywords: google,doc,document,sheet,slide
navigation-topic: workfront-for-g-suite
title: 이메일 콘텐츠를 사용하여 Google Workspace에서  [!DNL Adobe Workfront] 항목 업데이트
description: Adobe Workfront이 아닌 이메일의 정보로 기존 프로젝트, 작업 또는 문제를 업데이트할 수 있습니다.
author: Becky
feature: Workfront Integrations and Apps
recommendations: noDisplay, noCatalog
exl-id: 2ac392f5-98a3-4ab6-a0e3-cda378f0f68b
last-update: 2026-04-01T18:03:50Z
git-commit-file: b03dbe8e217593e0f3a6fcd522148dcd8b7670b8
source-git-commit: 18301970abddd8ed98abccf42562d950422bfa7c
workflow-type: tm+mt
source-wordcount: '145'
ht-degree: 0%

---

# 전자 메일 콘텐츠를 사용하여 [!DNL Adobe Workfront]에서 [!DNL Google Workspace] 항목 업데이트

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

You can update an existing project, task, or issue with information from a non-[!DNL Adobe Workfront] email.

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

Before you can update a [!DNL Workfront] item using email content from [!DNL Google Workspace], you must

* Install [!DNL Workfront for Google Workspace]\
   For instructions, see [Install [!DNL Adobe Workfront for Google Workspace]](../../workfront-integrations-and-apps/workfront-for-g-suite/install-workfront-for-gsuite.md).

## Update a [!DNL Workfront] item using email content from [!DNL Google Workspace]

1. If the [!UICONTROL Workfront for Google Workspace] panel is not displayed, click the Workfront icon ![Workfront icon](assets/wf-lion-icon.png) in the [!DNL Google Workspace] add-ons sidebar at the far-right of the page.
1. With the email message open in [!DNL Google Workspace], click **[!UICONTROL Post as a new update]** in the [!DNL Google Workspace] panel.
1. Under **[!UICONTROL Type]**, click the drop-down arrow, then click the type of object where you want to add the update.
1. Click the **[!UICONTROL Search for]** option, start typing the name of the object where you want to add the update, then select the item when it appears in the list below.

   This option varies, depending on what you selected in step 3. It might be **[!UICONTROL Search for a project]**, **[!UICONTROL Search for a task]**, or **[!UICONTROL Search for an issue]**.

   >[!NOTE]
   >
   >When you are typing the name of a task, ad hoc personal tasks are excluded from the list of name that appears below.

1. Make any of these optional changes:

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">[!UICONTROL Update]</td> 
      <td>Edit any part of this text, which is taken from the email's subject line and body text.</td> 
     </tr> 
     <tr data-mc-conditions=""> 
      <td role="rowheader">[!UICONTROL Include email attachments]</td> 
      <td><p>(Available only if the email contains at least one attachment.) Click this option to save attachments in the [!UICONTROL Documents] tab for the task or issue. </p><p>If you do not want to save an attachment, click the X to the right of its name. </p><p>If the email contains links to documents in [!DNL Google Drive], the links are saved to the [!UICONTROL Overview] tab of the task or issue you are creating. </p><p>Important: <span style="color: #ff1493;"><span style="color: #000000;">In order for this to work, your</span></span>[!DNL Workfront] administrator<span style="color: #ff1493;"><span style="color: #000000;"> must authorize [!DNL Google Drive] to work with [!DNL Workfront]</span></span></p>
      <p>If you enable this option, it remains enabled for other emails you convert to tasks, issues, and updates.</p></td> 
     </tr> 
     <tr data-mc-conditions=""> 
      <td role="rowheader">Notify</td> 
      <td>Click <strong>[!UICONTROL Notify]</strong>, click the <strong>[!UICONTROL Search for a user or team]</strong> option that appears, then start typing the name of the person or team and click it when it appears in the list below. Repeat this for each person and team you want to add, then click <strong>[!UICONTROL Save]</strong>.</td> 
     </tr> 
    </tbody> 
   </table>

1. Click **[!UICONTROL Update]**.

   When you refresh your browser, a message with a link at the bottom of the [!DNL Workfront for Google Workspace] panel confirms that you have converted the email to an update:

   You can click the link to go to the [!UICONTROL Updates] tab in [!DNL Workfront] for the object you specified in step 4.

   You can repeat these steps to convert the same email to updates, task, and issues (see [Create an Adobe Workfront issue in [!DNL Google Workspace] using email content](../../workfront-integrations-and-apps/workfront-for-g-suite/create-wf-issue-in-g-suite-using-email-content.md)). When you refresh your browser or return to the email at another time, all links you have created for the email are listed at the bottom of the [!UICONTROL Workfront for Google Workspace] panel.

1. (Optional) Continue to work with the update in the [!DNL Workfront] add-on panel by doing any of the following:

   * To add another update on the **[!UICONTROL Updates]** tab, click **[!UICONTROL Start a new update]** and type the information.

   * To reply to an update on the **[!UICONTROL Updates]** tab, click **[!UICONTROL Reply]** and type your reply.

      For both of the options above, you can click **[!UICONTROL Notify]** to specify recipients for the reply as in step 5. When you are ready, click **[!UICONTROL Post]** to add the update or reply.

   * Click the **[!UICONTROL Details]** tab to view the details for the new project, task, or issue.

   -->
