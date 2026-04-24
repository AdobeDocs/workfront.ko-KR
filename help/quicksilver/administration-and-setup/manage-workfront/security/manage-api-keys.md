---
user-type: administrator
product-area: system-administration;user-management
navigation-topic: security
title: API 키 관리
description: API 보안 취약점을 최소화하기 위해 Adobe Workfront 관리자는 애플리케이션이 사용자를 대신하여 Workfront에 액세스할 수 있도록 하는 데 사용되는 API 키를 관리할 수 있습니다.
author: Becky
feature: System Setup and Administration
role: Admin
exl-id: 1176d899-0585-430d-87f2-0823bda2f1be
last-update: 2026-04-01T18:03:50Z
git-commit-file: b03dbe8e217593e0f3a6fcd522148dcd8b7670b8
source-git-commit: be11c7417023ce2f310fce3e0cf77724d101b89e
workflow-type: tm+mt
source-wordcount: '740'
ht-degree: 3%

---

# API 키 관리

<!--
DON'T DELETE, DRAFT OR HIDE THIS ARTICLE. IT IS LINKED TO THE PRODUCT, THROUGH THE CONTEXT SENSITIVE HELP LINKS.</p>
-->



>[!IMPORTANT]
>
>Workfront에서는 더 이상 `/login` 끝점 또는 API 키를 사용하지 않는 것이 좋습니다. 대신 다음 인증 방법 중 하나를 사용하십시오.
>
>* JWT를 사용한 서버 인증
>* OAuth2를 통한 사용자 인증
>
>이러한 인증 방법 설정에 대한 지침은 [Workfront 통합을 위한 OAuth2 애플리케이션 만들기](/help/quicksilver/administration-and-setup/configure-integrations/create-oauth-application.md)를 참조하십시오.
>
>Workfront에서 서버 인증을 사용하는 방법에 대한 지침은 [JWT 흐름을 사용하여 조직의 사용자 지정 OAuth 2 애플리케이션 구성 및 사용](/help/quicksilver/wf-api/api/oauth-app-jwt-flow.md)을 참조하십시오.
>
>Workfront에서 사용자 인증을 사용하는 방법에 대한 지침은 [인증 코드 흐름을 사용하여 조직의 사용자 지정 OAuth 2 애플리케이션 구성 및 사용](/help/quicksilver/wf-api/api/oauth-app-code-token-flow.md)을 참조하십시오.

API 보안 취약점을 최소화하기 위해 Adobe Workfront 관리자는 애플리케이션이 사용자를 대신하여 Workfront에 액세스할 수 있도록 하는 데 사용되는 API 키를 관리할 수 있습니다.

현재 관리자 API 키를 재설정 또는 제거하고, 만료되도록 API 키를 구성하고, 모든 사용자에 대한 API 키를 제거할 수 있습니다.

Workfront API를 활용하는 애플리케이션의 예는 다음과 같습니다.

* Dropbox, Google 드라이브 및 Workfront DAM과 같은 문서 통합
* Workfront 모바일 애플리케이션

>[!IMPORTANT]
>
>API 키를 재설정하거나 제거할 때 Workfront API를 활용하고 이 API 키를 통해 Workfront에 대해 인증하는 모든 애플리케이션은 Workfront에 다시 액세스하도록 다시 구성해야 합니다.

## 액세스 요구 사항

+++ 이 문서의 기능에 대한 액세스 요구 사항을 보려면 확장하십시오.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront 패키지</td> 
   <td><p>Any</p></td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront 라이선스</td> 
   <td><p>표준</p><p>플랜</p></td> 
  </tr> 
  <tr> 
   <td role="rowheader">액세스 수준 구성</td> 
   <td> <p>Workfront 관리자여야 합니다.</p> </p> </td> 
  </tr> 
 </tbody> 
</table>

자세한 내용은 [Workfront 설명서의 액세스 요구 사항](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)을 참조하십시오.

+++

## Workfront API 키

Workfront의 각 사용자에게는 고유한 API 키가 있습니다. 이 키는 사용자가 Workfront API를 활용하는 통합(예: Workfront 모바일 앱 또는 문서 통합)에 액세스할 때 사용자별로 생성됩니다.

>[!NOTE]
>
> 프로덕션 환경에서 생성하는 API 키는 주별 새로 고침 중에 미리보기 환경에 복사됩니다. 미리보기 환경에서 생성하는 모든 API 키는 주별 새로 고침 중에 프로덕션 API 키로 덮어쓰여집니다.

Workfront 관리자에게도 고유한 API 키가 있습니다. 애플리케이션이 관리자 API 키를 사용하여 Workfront에 액세스하면 애플리케이션이 Workfront에 대한 관리자 액세스 권한을 갖습니다.

## 관리자 API 키 관리

관리자 사용자 계정에 대한 API 키를 생성, 재설정 또는 제거할 수 있습니다.

{{step-1-to-setup}}

1. **시스템 >** **고객 정보**&#x200B;를 클릭합니다.
1. (조건부) 다음 작업 중 하나를 수행합니다.

   API 키를 생성하려면: **API 키 설정** 섹션에서 **API 키 생성**&#x200B;을 클릭하세요.

   또는\
   API 키를 다시 설정하려면 **API 키 설정** 섹션에서 **다시 설정**&#x200B;을 클릭한 다음 **다시 설정**&#x200B;을 클릭합니다.

   또는

   API 키를 제거하려면: **API 키 설정** 섹션에서 **제거**&#x200B;를 클릭한 다음 **제거**&#x200B;를 클릭합니다.

<!--

   Remove me October 2026

## Generate an API Key for Non-Admin Users

You can generate and manage API Keys for users in roles other than Workfront administrator.

>[!NOTE]
>
>This is not available if your organization's Workfront instance is enabled with Adobe IMS. See your network or IT administrator if you need more information.

1. (Conditional) If your organization uses Single Sign-On (SSO) access management, temporarily disable the option requiring SSO authentication.

   {{step-1-to-setup}} 
   
   1. Expand **System**, then click **Single Sign-on (SSO)**. 
   1. In the **Type** field, select the type of SSO your organization uses.
   1. With the type selected, scroll down and clear the **Enable** checkbox. 
      ![Enable SSO](assets/sysadmin-security-sso-disable-31620-350x320.png)  
   1. Click **Save**.


1. In the address bar of a browser, enter the following API call:

   `<domain>`.my.workfront.com/attask/api/v7.0/user?action=generateApiKey&username=**username**&password=**password**&method=PUT

   Replace `<domain>` with your Workfront domain name, and username and password with the user's Workfront credentials.

1. (Conditional) Enable the option requiring SSO authentication if you disabled it in Step 1.

   {{step-1-to-setup}}
   
   1. Expand **System**, then click **Single Sign-on (SSO)**.
   
   1. Select your SSO method in the **Type** drop down menu.
   1. Check the checkbox requiring SSO authentication.

   -->

## API 키가 만료되는 시기 구성

API 키가 시스템의 모든 사용자에 대해 만료되도록 구성할 수 있습니다. 사용자의 API 키가 만료되면 사용자는 Workfront API를 사용하여 Workfront에 액세스하는 모든 애플리케이션에 다시 인증해야 합니다. API 키가 만료되는 빈도를 변경할 수 있습니다. 사용자의 암호가 만료될 때 API 키가 만료되는지 여부를 구성할 수도 있습니다.

{{step-1-to-setup}}

1. **시스템** > **고객 정보**&#x200B;를 클릭합니다.
1. **API 키 설정** 영역의 **생성 후**, **API 키가**&#x200B;에 만료됩니다. 드롭다운 목록에서 API 키를 만료하려는 시간대를 선택합니다.

   이 옵션을 변경하면 변경한 시점부터 새 일정이 시작됩니다. 예를 들어 이 옵션을 *1개월*&#x200B;에서 *6개월*(으)로 변경하면 변경한 시점부터 6개월이 API 키가 만료됩니다.

   기본적으로 API 키는 매월 만료됩니다.

1. 사용자의 암호가 만료되는 시점에 만료되도록 API 키를 구성하려면 **사용자의 암호가 만료될 때 API 키 제거**&#x200B;를 사용하도록 설정하십시오.

   기본적으로 이 옵션은 활성화되어 있지 않습니다.

   사용자 암호를 만료되도록 구성하는 방법에 대한 자세한 내용은 [시스템 보안 환경 설정 구성](../../../administration-and-setup/manage-workfront/security/configure-security-preferences.md)을 참조하십시오.

1. **저장**&#x200B;을 클릭합니다.

## 모든 사용자에 대한 API 키 제거

Workfront 시스템과 관련된 특정 보안 침해가 우려되는 경우 모든 사용자에 대해 동시에 API 키를 제거할 수 있습니다.

>[!IMPORTANT]
>
>모든 사용자에 대한 API 키를 제거하면 시스템의 모든 사용자에 대한 모든 API 키가 무효화됩니다. 이 작업을 수행하면 Workfront에서 새 API 키를 생성하고 모든 통합을 업데이트할 때까지 Workfront의 모든 통합이 실패합니다.

{{step-1-to-setup}}

1. **시스템**&#x200B;을 확장한 다음 **고객 정보**&#x200B;를 클릭합니다.

1. **API 키 설정** 영역에서 **모든 API 키 제거**&#x200B;를 클릭한 다음 **제거** **모두**&#x200B;를 클릭합니다.

<!--

Remove me October 2026

## Restricting API logins with an X.509 certificate

>[!IMPORTANT]
>
>The procedure described in this section applies only to organizations that have not yet been onboarded to the Adobe Business Platform. Logging in to Workfront through the Workfront API is not available if your organization has been onboarded to the Adobe Business Platform.
>
>For a list of procedures that differ based on whether your organization has been onboarded to the Adobe Business Platform, see [Administration differences between Adobe Workfront and Adobe Business Platform](../../../administration-and-setup/get-started-wf-administration/actions-in-admin-console.md).

>[!NOTE]
>
>This is not available if your organization's Workfront instance is enabled with Adobe IMS. See your network or IT administrator if you need more information.

Third-party applications can communicate with Workfront through the API. To increase the security of your Workfront site, you can configure Workfront to restrict API login requests by uploading an X.509 certificate to Workfront. Once enabled, all login requests through the API must include a client certificate in addition to username and password.

* [Obtain the X.509 certificate](#obtain-the-x-509-certificate) 
* [Upload the certificate to Workfront](#upload-the-certificate-to-workfront) 
* [Verify API login calls are restricted](#verify-api-login-calls-are-restricted)

### Obtain the X.509 certificate {#obtain-the-x-509-certificate}

Obtain a valid X.509 certificate from a trusted Certificate Authority (such as Verisign), and save it to a temporary location on your workstation. 

### Upload the certificate to Workfront {#upload-the-certificate-to-workfront}

After you have obtained the X.509 certificate from your Certificate Authority, you need to upload it to Workfront.

1. Click the **Main Menu** icon ![Main menu icon](assets/main-menu-icon.png) in the upper-right corner of Adobe Workfront, then click **Setup** ![Gear settings icon](assets/gear-icon-settings.png).  

1. Expand **System**, then click **Customer Info**.

1. In the **API Key Settings** area, select **Require X.509 Certificate for API logins**.
1. Click **Change Certificate**.
1. On your workstation, browse to and select the X.509 certificate that you previously downloaded.
1. (Optional) Click **View Details** next to the certificate name to view the following details about the certificate:

   * Subject Common Name
   * Subject Organization
   * Subject Organization Unit
   * Issuer Common Name
   * Issuer Organization
   * Issuer Organization Unit
   * Serial Number
   * Issue Date
   * Expiration Date

1. Click **Save**. 

### Verify API login calls are restricted {#verify-api-login-calls-are-restricted}

Prior to configuring your instance of Workfront to require an X.509 certificate, perform an API request to the `/login` endpoint using valid username and password parameters. You will receive a 200 response that contains a sessionID.

After making the X.509 certificate a requirement via the customer info page in your instance of Workfront, make another login attempt. This time you will receive a 500 error response with the following message: "Untrusted request. Please contact your system administrator and attach certificate."

After confirming that the X.509 certificate is required, perform the same login request with an additional parameter for apiCertificate set to the value of your certificate. If this operation was performed correctly you will receive a 200 response that contains a valid sessionID.

-->
