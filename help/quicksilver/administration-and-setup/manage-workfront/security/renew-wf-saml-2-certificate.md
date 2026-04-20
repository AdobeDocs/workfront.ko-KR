---
user-type: administrator
product-area: system-administration
keywords: SAML 2.0,보안,인증서,관리자,면제,구성,메타데이터
navigation-topic: security
title: Adobe Workfront SAML 2.0 메타데이터 인증서 갱신
description: Adobe Workfront 서버는 인증 및 권한 부여에 SAML 2.0 프로토콜을 사용합니다. 업데이트되면 새 인증서는 1년 동안 유효합니다. ID 공급자에서 인증서를 갱신할 때가 되면 Workfront에서 이 변경이 발생해야 한다는 경고 메시지가 표시됩니다. Workfront 관리자는 시스템 수준에서 이 변경 사항을 관리할 수 있습니다.
author: Becky
feature: System Setup and Administration
role: Admin
exl-id: 4b481215-36a1-4945-828a-1598502529d8
last-update: 2026-04-01T18:03:50Z
git-commit-file: b03dbe8e217593e0f3a6fcd522148dcd8b7670b8
source-git-commit: aeb471fd63269d30a675e44fe1a47db6141eb9ed
workflow-type: tm+mt
source-wordcount: '133'
ht-degree: 0%

---

# Adobe Workfront SAML 2.0 메타데이터 인증서 갱신

>[!IMPORTANT]
>
>이 페이지에 설명된 절차는 Admin Console에 아직 온보딩되지 않은 조직에만 적용됩니다. 조직이 Adobe Admin Console에 온보딩된 경우 조치가 필요하지 않습니다.
>
>이제 모든 조직이 Adobe Admin Console에 온보딩되었으므로 이 기능은 더 이상 사용되지 않습니다.

<!--

Remove me October 2026

The Adobe Workfront servers utilize the SAML 2.0 protocol for authentication and authorization. Once updated, the new certificate remains valid for one year. When it is time for you to renew the certificate on your identity provider, you receive a warning in Workfront alerting you that this change must occur. As a Workfront administrator, you can manage this change at the system level.


>[!NOTE]
>
>This is not available if your organization's Workfront instance is enabled with Adobe IMS. See your network or IT administrator if you need more information.

## Access requirements

+++ Expand to view access requirements for the functionality in this article.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront package</td> 
   <td><p>Any</p></td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront license</td> 
   <td><p>Standard</p><p>Plan</p></td> 
  </tr> 
  <tr> 
   <td role="rowheader">Access level configurations</td> 
   <td> <p>You must be a Workfront administrator.</p> </p> </td> 
  </tr> 
 </tbody> 
</table>

For information, see [Access requirements in Workfront documentation](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md). 

+++

## Configure SAML 2.0 within Workfront

To review the warning message and acknowledge the update of the SAML 2.0 metadata in your identity provider:

{{step-1-to-setup}}

1. Click **System** > **Single Sign-On**.

1. In the **Type** drop-down menu, select **SAML 2.0**.

1. Click **Download SAML 2.0 Metadata**.

   This downloads the renewed Workfront certificate for SAML 2.0, which contains the correct metadata for your server.

1. In your identity provider, copy your current Assertion Consumer Service (ACS) URL (also known as the Reply URL) to a safe place. 

   >[!CAUTION]
   >
   >Before you upload the Workfront metadata to your Single Sign-On (SSO) provider in Step 6, copy your current Assertion Consumer Service (ACS) URL to a safe place. This URL, also known as the Reply URL, is found on your SSO provider's Workfront configuration page. 
   >
   >
   >If the ACS URL changes after you upload the Workfront metadata, this means that the metadata might contain an incorrect ACS URL. You must change it back to the one you copied in order to avoid breaking your Single Sign-On connection. Your updated certificate will still be correct after you do this.

1. In your identity provider server, update the new certificate you downloaded.
1. (Conditional) If the Assertion Consumer Service (ACS) URL or Reply URL has changed in your identity provider, change it back to the URL you copied in Step 5.
1. In Workfront, on the **Single Sign-on (SSO) page**, make sure that this option is selected: **The new Workfront certificate has already been uploaded to the Identity Provider**.

   >[!NOTE]
   >
   >* This option is visible only if all of the following apply:
   >   * Your organization is already set up for SAML 2.0
   >   * The current certificate is ready to expire
   >   * The new certificate is available
   >* When this field is selected, Workfront administrators can log in to Workfront with their SSO credentials or their Workfront credentials.

1. Click **Save**.

   The warning message no longer displays because you acknowledged the renewal of the SAML 2.0 certificate on the server of your identity provider.

1. Click **Test Connection** to test your configuration.

   You should see a message confirming that the connection was successful.

For more information, or for assistance with the manual configuration of metadata, please contact our Support Team, as explained in [Contact Customer Support](../../../workfront-basics/tips-tricks-and-troubleshooting/contact-customer-support.md).

-->
