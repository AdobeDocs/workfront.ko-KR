---
content-type: overview
product-area: workfront-integrations
navigation-topic: workfront-for-salesforce
title: Adobe Workfront for Salesforce 개요
description: Salesforce용  [!DNL Adobe Workfront] 을(를) 설치하여 Salesforce 사용자가 Salesforce을 종료하지 않고도 요청을 제출 [!DNL Workfront] 하고 자동으로 프로젝트를 만들 수 있습니다.
author: Becky
feature: Workfront Integrations and Apps
recommendations: noDisplay, noCatalog
exl-id: 65d4cdae-1d34-4a8a-a1c0-706cd41fc75e
source-git-commit: ddd1c964c4c885f71dfa30d1790cfbc6e26d6781
workflow-type: tm+mt
source-wordcount: '110'
ht-degree: 0%

---

# [!DNL Adobe Workfront for Salesforce] 개요

<!-- Audited: 5/2025 -->

>[!IMPORTANT]
>
>보다 안정적이고 확장 가능한 통합을 제공하기 위해 Workfront 자동화 및 통합(Fusion)을 사용하는 현대적이고 유연한 통합 접근 방식으로 전환했습니다. 이 전환 프로세스의 일부로 Salesforce 통합 **용 Workfront을 더 이상 사용할 수 없습니다**.
>
>조직의 Salesforce 통합 요구 사항에 맞게 Workfront 자동화 및 통합을 사용하는 것이 좋습니다.
>
>Workfront 자동화 및 통합에 대한 개요는 [Adobe Workfront Fusion 개요](https://experienceleague.adobe.com/en/docs/workfront-fusion/using/get-started-with-fusion/understand-workfront-fusion/workfront-fusion-overview)를 참조하십시오.
>
>Salesforce용 Workfront 자동화 및 통합 모듈의 특정 기능에 대한 자세한 내용은 [Salesforce 모듈](https://experienceleague.adobe.com/en/docs/workfront-fusion/using/references/apps-and-their-modules/third-party-app-connectors/salesforce-modules)을 참조하십시오.

<!--

You can install [!DNL Adobe Workfront for Salesforce] to allow your [!DNL Salesforce] users to submit [!DNL Workfront] requests and automatically create projects without ever leaving [!DNL Salesforce].

As a [!DNL Workfront] administrator, you can download and configure [!DNL Workfront for Salesforce]. Then, you can share it with all other [!DNL Salesforce] users.

For more information about installing [!DNL Workfront for Salesforce], see [Install [!DNL Adobe Workfront for Salesforce]](../../workfront-integrations-and-apps/using-workfront-with-salesforce/install-workfront-for-salesforce.md).

For more information about configuring the [!DNL Workfront] section in [!DNL Salesforce] for all users, see [Configure the [!DNL Adobe Workfront] section for [!DNL Salesforce] users](../../workfront-integrations-and-apps/using-workfront-with-salesforce/configure-wf-section-for-salesforce-users.md).

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
   <td> <p>Standard</p>
   <p>Plan</p> </td> 
  </tr> 
 </tbody> 
</table>

For information, see [Access requirements in Workfront documentation](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md). 

+++

## [!DNL Workfront for Salesforce]

You can do the following when using [!DNL Workfront for Salesforce]:

* Manually create new [!DNL Workfront] requests from [!DNL Salesforce] within an Opportunity or an Account.

   For more information, see [Submit [!DNL Adobe Workfront] requests from [!DNL Salesforce] objects](../../workfront-integrations-and-apps/using-workfront-with-salesforce/submit-workfront-requests-from-salesforce-objects.md).

* Automatically trigger the creation of projects in [!DNL Workfront] when certain criteria are met in [!DNL Salesforce]. Your [!DNL Salesforce] system administrator must configure triggers for creating projects from [!DNL Salesforce].

   For more information about creating [!DNL Workfront] projects from [!DNL Salesforce], see [Create [!DNL Adobe Workfront] projects from [!DNL Salesforce] objects](../../workfront-integrations-and-apps/using-workfront-with-salesforce/create-wf-projects-from-salesforce-objects.md).

Consider the following when working with [!DNL Workfront] for [!DNL Salesforce]:

* We support both the [!DNL Salesforce Classic] and [!DNL Lightning Experience] frameworks.
* Items can be created only from [!DNL Salesforce] to [!DNL Workfront].
* You can view some information about the [!DNL Workfront] items in [!DNL Salesforce]. This information cannot be customized.

   For a list of [!DNL Workfront] fields that you can view from [!DNL Salesforce], see  [Submit [!DNL Adobe Workfront] requests from [!DNL Salesforce] objects](../../workfront-integrations-and-apps/using-workfront-with-salesforce/submit-workfront-requests-from-salesforce-objects.md)  and [Create [!DNL Adobe Workfront] projects from [!DNL Salesforce] objects](../../workfront-integrations-and-apps/using-workfront-with-salesforce/create-wf-projects-from-salesforce-objects.md).

* You can directly access items linked to [!DNL Salesforce] by clicking the [!UICONTROL Go to Salesforce] link from Workfront.

   You cannot view any information about the [!DNL Salesforce] items in [!DNL Workfront], but there's a link in Workfront that takes you to the item in Salesforce so you can review it there.

   [!UICONTROL The Go to Salesforce] link displays in the following areas:

    * The [!UICONTROL Details] section of a project or an issue.
    * The header of a project or an issue.

      Your system or group administrator must add the [!UICONTROL Integrations] field to your Layout Template to view the [!UICONTROL Go to Salesforce] link in the project or issue header.
    * The [!DNL Summary] panel  of an issue when selecting the issue in a list, after clicking [!UICONTROL Open Summary] ![Summary panel icon](assets/summary-panel-icon.png) in the list's toolbar.

      >[!NOTE]
      >
      >The [!UICONTROL Go to Salesforce] link is visible to all [!DNL Workfront] users who can view the project or the issue. You must have a [!DNL Salesforce] account to be able to go to the [!DNL Salesforce] Opportunity or Account where the issue was logged.

* Updating fields on one item in one application does not update any information on linked items in the other application.

-->
