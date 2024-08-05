---
product-area: workfront-integrations
navigation-topic: workfront-for-outlook
title: ' [!DNL Adobe Workfront] for [!DNL Outlook] 설정'
description: ' [!DNL Adobe Workfront] [!DNL Outlook] 추가 기능을 사용하면 Outlook에서 직접  [!DNL Workfront] 주요 작업을 수행할 수 있습니다.'
author: Becky
feature: Workfront Integrations and Apps
exl-id: 57f0560b-68c2-4654-863e-bd728e76da29
source-git-commit: e4f722bab4c4024ca796af8413e7d6b69f6a89a7
workflow-type: tm+mt
source-wordcount: '684'
ht-degree: 0%

---

# [!DNL Adobe Workfront for Outlook] 설정

<!-- Audited: 12/2023 -->

[!DNL Adobe Workfront] [!DNL Outlook] 추가 기능을 사용하면 Outlook에서 직접 다음 주요 [!DNL Workfront] 작업을 수행할 수 있습니다.

* 이메일의 정보로 기존 프로젝트, 작업 또는 문제를 업데이트합니다. 자세한 내용은 [전자 메일 [!DNL Outlook] 에서 기존 개체 업데이트](../../workfront-integrations-and-apps/using-workfront-with-outlook/update-an-existing-object-from-an-outlook-email.md)를 참조하십시오.
* [!DNL Outlook] 내의 전자 메일을 기반으로 [!DNL Workfront] 요청을 만듭니다. 자세한 내용은 [전자 메일 [!DNL Outlook] 에서 Adobe Workfront 요청 만들기](../../workfront-integrations-and-apps/using-workfront-with-outlook/create-a-wf-request-from-an-outlook-email.md)를 참조하세요.
* [!UICONTROL 내 작업] 영역에 전자 메일을 작업으로 추가합니다. 자세한 내용은 [작업 목록에 작업으로 전자 메일 추가](../../workfront-integrations-and-apps/using-workfront-with-outlook/add-outlook-email-as-task-to-your-work-list.md)를 참조하십시오. [!DNL Outlook] 
* [!DNL Outlook]의 [!DNL Workfront] 추가 기능을 통해 댓글에 회신합니다. [!DNL Outlook]에 대한 Workfront의 댓글에 회신하는 방법에 대한 자세한 내용은 [댓글에 회신 [!DNL Outlook]](../../workfront-integrations-and-apps/using-workfront-with-outlook/reply-to-a-comment-from-outlook.md)을 참조하세요.
* 작업 및 문제를 처음부터 만들거나 기존 이메일에서 만듭니다(드래그 앤 드롭 기능 사용). 자세한 내용은 [프로젝트에 작업 또는 문제로 이메일 추가 [!DNL Outlook] 를 참조하십시오](../../workfront-integrations-and-apps/using-workfront-with-outlook/add-outlook-email-to-project-as-task-or-issue.md).

[!DNL Workfront for Outlook]을(를) 사용하려면 먼저 [!DNL Workfront] 추가 기능을 [!DNL Outlook] 계정에 추가해야 합니다.

[!DNL Outlook] 계정으로 [!DNL Workfront] 추가 기능을 설치할 수 없는 경우 [!DNL Workfront] 관리자에게 문의하여 조직에 [!DNL Outlook] 추가 기능이 활성화되어 있는지 확인하십시오.

조직에 대해 [!DNL Outlook] 통합을 활성화하는 방법에 대한 자세한 내용은 [활성화 [!DNL Adobe Workfront for Outlook]](../../administration-and-setup/configure-integrations/enable-workfront-for-outlook.md)를 참조하십시오.

## 액세스 요구 사항

+++ 을 확장하여 이 문서의 기능에 대한 액세스 요구 사항을 봅니다.

이 문서의 단계를 수행하려면 다음 액세스 권한이 있어야 합니다.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] 플랜</td> 
   <td> <p>임의</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] 라이센스</td> 
   <td> 
   <p>새 플랜: [!UICONTROL Standard]</p> 
   <p>현재 계획:[!UICONTROL Work], [!UICONTROL Plan]</p> </td> 
  </tr> 
 </tbody> 
</table>

이 표의 정보에 대한 자세한 내용은 [Workfront 설명서의 액세스 요구 사항](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)을 참조하십시오.

+++

## 전제 조건

이 통합을 사용하려면 [!DNL Workfront] 관리자가 [!DNL Workfront]에서 [!DNL Outlook for Office]을(를) 사용하도록 설정해야 합니다.

## 시스템 요구 사항

다음 응용 프로그램을 사용할 수 있습니다.

* **[!DNL Outlook]웹:** [!DNL Workfront] 추가 기능은 데스크톱 또는 모바일 장치에서 웹 브라우저에서 [!DNL Outlook]을(를) 사용할 때 사용할 수 있습니다. 이 기능은 [!DNL Outlook] 웹 앱을 사용할 때도 사용할 수 있습니다.
* **[!DNL Outlook]데스크톱 응용 프로그램:** [!DNL Office] 패키지에 포함된 [!DNL Outlook]의 [!DNL Windows] 및 [!DNL Mac] 데스크톱 버전을 사용하는 경우 [!DNL Workfront] 추가 기능을 사용할 수 있습니다.

[!DNL Outlook]용 [!DNL Workfront] 추가 기능은 다음 요구 사항을 충족하는 환경에서 지원됩니다.

* [클라이언트 요구 사항](#client-requirements-client-requirements)
* [메일 서버 요구 사항](#mail-server-requirements-mail-server-requirements)

### 클라이언트 요구 사항 {#client-requirements}

Workfront은 다음 버전의 [!DNL Outlook]을(를) 지원합니다.

* [!DNL Windows]의 [!DNL Outlook 2013] 이상
[!DNL Windows]의 *[!DNL  Outlook 2016] 이상
* [!DNL Mac]의 [!DNL Outlook]([!DNL Microsoft 365])
* [!DNL Windows]의 [!DNL Outlook]([!DNL Microsoft 365])
* 웹에서 [!DNL Outlook]

직접 연결을 사용하여 [!DNL Exchange Server] 또는 [!DNL Office 365]에 연결해야 합니다.

클라이언트를 구성할 때 사용자는 다음 계정 유형 중 하나를 선택해야 합니다.

* [!DNL Exchange]
* [!DNL Office 365]
* [!DNL Outlook.com]{&#x200B;1&#x200B;}**&#x200B;클라이언트가 POP3 또는 IMAP에 연결하도록 구성된 경우 [!DNL Workfront] 추가 기능이 로드되지 않습니다.**

### 메일 서버 요구 사항 {#mail-server-requirements}

[!DNL Office 365] 또는 [!DNL Outlook.com]에 연결할 때 메일 서버 요구 사항이 기본적으로 충족됩니다. 그러나 [!DNL Exchange Server]의 On-Premise 설치에 연결된 경우 다음 요구 사항이 적용됩니다.

* Workfront은 모든 [!DNL Exchange On-Premise] 서버를 지원합니다.
* [!DNL Exchange Web Services](EWS)을(를) 사용하도록 설정해야 하며 인터넷에 노출되어야 합니다.
* 서버가 유효한 ID 토큰을 발급하려면 서버에 유효한 인증 인증서가 있어야 합니다. [!DNL Exchange Server]의 새 설치에 기본 인증 인증서가 포함되어 있습니다.

  <!--this used to be here but Dev asked for it to be taken out - logged issue for editing this article on 4-26-2023: For more information, see [Digital certificates and encryption in [!DNL Exchange 2016]](https://technet.microsoft.com/en-us/library/dd351044(v=exchg.160).aspx) and [Set-AuthConfig](https://technet.microsoft.com/en-us/library/jj215766(v=exchg.160).aspx).-->

* [[!DNL Office] Store](https://store.office.com/)에서 [!DNL Workfront] 추가 기능에 액세스하려면 클라이언트 액세스 서버가 [https://store.office.com](https://store.office.com/)과(와) 통신할 수 있어야 합니다.

지원되는 환경에 대한 자세한 내용은 [[!DNL Microsoft Office 365] 홈 페이지](https://products.office.com/en-us/office-365-home)를 참조하세요.

## 추가 기능 설치

[Microsoft 스토어](https://appsource.microsoft.com/en-us/product/office/WA104380943?tab=Overview)에서 Outlook용 Workfront 추가 기능을 가져올 수 있습니다.

### [!DNL Outlook 365]에 대한 [!DNL Workfront] {#workfront-for-outlook-365}

1. [!DNL Outlook 365]에서 Office 365 인터페이스 상단의 **[!UICONTROL 추가 기능 찾아보기]** 아이콘 ![](assets/outlook-add-in-26x26.png)을 클릭한 다음 **[!UICONTROL 추가 기능 관리]**&#x200B;를 클릭합니다.

1. **[!UICONTROL 추가 기능 검색]** 상자에서 **[!DNL Workfront]**&#x200B;을 검색한 다음 [!UICONTROL Enter]를 누릅니다.

1. **[!UICONTROL 추가]**&#x200B;를 클릭합니다.

### 웹에서 [!DNL Outlook]에 대한 [!DNL Workfront] {#workfront-for-outlook-on-the-web}

1. 웹 브라우저에서 [!DNL Microsoft Outlook] 열기
1. **[!UICONTROL 찾아보기] 추가 기능** 아이콘 ![](assets/outlook-add-in-web-version-20x20.png)을(를) 클릭합니다.

   아이콘을 찾으려면 Microsoft 설명서에서 [웹에서  [!DNL Outlook] 추가 기능 사용](https://support.microsoft.com/en-us/office/using-add-ins-in-outlook-on-the-web-8f2ce816-5df4-44a5-958c-f7f9d6dabdce#bkmk_addaddinsicon)을 참조하세요.

1. **[!UICONTROL 추가 기능 검색]** 필드에서 **[!DNL Workfront]**&#x200B;을(를) 검색한 다음 **[!UICONTROL Enter]**&#x200B;를 누릅니다.

1. 목록에 나타나면 **추가**&#x200B;를 클릭합니다.

### [!UICONTROL Windows] 또는 [!DNL Mac]의 [!DNL Workfront for Outlook] {#workfront-for-outlook-on-windows-or-mac}

1. 리본에서 **[!UICONTROL 홈]** > **[!UICONTROL 스토어]**&#x200B;를 클릭합니다.

1. **[!UICONTROL 검색]** 필드에서 **[!DNL Workfront]**&#x200B;을(를) 검색한 다음 **[!UICONTROL Enter]**&#x200B;를 누릅니다.

1. **[!UICONTROL [!DNL Workfront]추가 기능]**&#x200B;을 사용하도록 설정하려면 토글을 클릭하십시오.

## [!DNL Outlook]에서 [!DNL Workfront]에 로그인

1. [!DNL Outlook]에서 전자 메일 메시지를 선택한 다음 전자 메일 헤더의 **[!DNL Workfront]** 아이콘을 클릭합니다.
1. 로그인 페이지에서 **Workfront에 로그인**&#x200B;을 클릭합니다.
1. 메시지에 따라 OAuth 2.0을 사용하여 [!DNL Workfront]에 로그인합니다. <!--Enhanced Authentication or your Security Assertion Markup Language (SAML) URL.-->

   <!--Before users can log in to the [!DNL Workfront] add-in using SAML, a [!DNL Workfront] administrator must first enable [!DNL Office 365] add-ins to authenticate using a SAML 2.0 solution. For more information, see the section [Configure [!DNL Adobe Workfront] with SAML 2.0](../../administration-and-setup/add-users/single-sign-on/configure-workfront-saml-2.md#enable-saml-with-office-365) in the article [Configure [!DNL Adobe Workfront] with SAML 2.0](../../administration-and-setup/add-users/single-sign-on/configure-workfront-saml-2.md).-->

   >[!NOTE]
   >
   >* [!DNL Workfront] 계정의 도메인을 입력하라는 메시지가 표시되면 *yourCompany&#39;sDomain.my.workfront.com* 형식을 사용하여 입력하세요. 회사의 도메인은 일반적으로 회사의 이름입니다.

<!--ADDITIONAL BULLET REMOVED FROM NOTE BOX: Enhanced Authentication is not available until a Workfront administrator enables it for this integration.-->
