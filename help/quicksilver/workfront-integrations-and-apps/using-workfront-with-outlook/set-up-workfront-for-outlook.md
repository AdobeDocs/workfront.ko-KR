---
product-area: workfront-integrations
navigation-topic: workfront-for-outlook
title: 설정 [!DNL Adobe Workfront] 대상 [!DNL Outlook]
description: Adobe Workfront Fusion은 Outlook과의 통합을 제공합니다. 이 문서에서는 자체 워크플로우에서 이 통합을 사용할 수 있는 방법을 설명합니다.
author: Becky
feature: Workfront Integrations and Apps
exl-id: 57f0560b-68c2-4654-863e-bd728e76da29
source-git-commit: 61a107e1ee8a415fd94e73fc65fa5f59f7de02d1
workflow-type: tm+mt
source-wordcount: '761'
ht-degree: 0%

---

# 설정 [!DNL Adobe Workfront for Outlook]

다음 [!DNL Adobe Workfront] [!DNL Outlook] 추가 기능을 사용하면 다음 키를 수행할 수 있습니다 [!DNL Workfront] Outlook에서 직접 작업:

* 전자 메일의 정보로 기존 프로젝트, 작업 또는 문제를 업데이트합니다. 자세한 내용은 [에서 기존 개체 업데이트 [!DNL Outlook] 이메일](../../workfront-integrations-and-apps/using-workfront-with-outlook/update-an-existing-object-from-an-outlook-email.md).
* 만들기 [!DNL Workfront] 내 이메일을 기반으로 요청 [!DNL Outlook]. 자세한 내용은 [에서 Adobe Workfront 요청 만들기 [!DNL Outlook] 이메일](../../workfront-integrations-and-apps/using-workfront-with-outlook/create-a-wf-request-from-an-outlook-email.md).
* 전자 메일을 작업으로 추가 [!UICONTROL 내 작업] 영역. 자세한 내용은 [추가 [!DNL Outlook] 작업 목록에 작업으로 전자 메일 보내기](../../workfront-integrations-and-apps/using-workfront-with-outlook/add-outlook-email-as-task-to-your-work-list.md).
* 을 통해 댓글에 답글 달기 [!DNL Workfront] 용 추가 기능 [!DNL Outlook]. 다음에 대한 Workfront의 의견에 응답하는 방법에 대한 정보 [!DNL Outlook]를 참조하십시오. [댓글에 회신 [!DNL Outlook]](../../workfront-integrations-and-apps/using-workfront-with-outlook/reply-to-a-comment-from-outlook.md).
* 처음부터 작업 및 문제를 만들거나 기존 이메일에서 만듭니다(드래그 앤 드롭 기능 사용). 자세한 내용은 [추가 [!DNL Outlook] 작업 또는 문제로 프로젝트에 전자 메일 보내기](../../workfront-integrations-and-apps/using-workfront-with-outlook/add-outlook-email-to-project-as-task-or-issue.md).

를 추가해야 합니다 [!DNL Workfront] 에 추가 [!DNL Outlook] 계정을 사용하기 전에 [!DNL Workfront for Outlook].

을(를) 설치할 수 없는 경우 [!DNL Workfront] 을 사용하여 추가 [!DNL Outlook] 계정, [!DNL Workfront] 관리자가 [!DNL Outlook] 조직에 대해 추가 기능이 활성화되어 있습니다.

를 활성화하는 방법에 대한 자세한 내용은 [!DNL Outlook] 조직에 대한 통합은 다음을 참조하십시오. [활성화 [!DNL Adobe Workfront for Outlook]](../../administration-and-setup/configure-integrations/enable-workfront-for-outlook.md).

## 액세스 요구 사항

이 문서의 절차를 수행하려면 다음 액세스 권한이 있어야 합니다.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] 플랜*</td> 
   <td> <p>모든</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] 라이센스*</td> 
   <td> <p>[!UICONTROL Work], [!UICONTROL Plan]</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;어떤 계획, 라이센스 유형 또는 액세스 권한을 보유하고 있는지 확인하려면 [!DNL Workfront] 관리자

## 전제 조건

사용자 [!DNL Workfront] 관리자 활성화 [!DNL Outlook for Office] with [!DNL Workfront] 먼저 이 통합을 사용합니다.

## 시스템 요구 사항

다음 응용 프로그램을 사용할 수 있습니다.

* **[!DNL Outlook]웹:** 다음 [!DNL Workfront] 추가 기능은 [!DNL Outlook] 데스크탑 또는 모바일 장치의 웹 브라우저에서 이 기능은 [!DNL Outlook] 웹 앱.
* **[!DNL Outlook]데스크탑 애플리케이션:** 다음 [!DNL Workfront] 추가 기능은 [!DNL Windows] 및 [!DNL Mac] 데스크탑 버전 [!DNL Outlook] 포함 [!DNL Office] 패키지.

다음 [!DNL Workfront] 용 추가 기능 [!DNL Outlook] 는 다음 요구 사항을 충족하는 환경에서 지원됩니다.

* [클라이언트 요구 사항](#client-requirements-client-requirements)
* [메일 서버 요구 사항](#mail-server-requirements-mail-server-requirements)

### 클라이언트 요구 사항 {#client-requirements}

Adobe는 다음 버전을 지원합니다 [!DNL Outlook]:

* [!DNL Outlook 2013] 또는 나중에 [!DNL Windows]
*[!DNL  Outlook 2016] 또는 나중에 [!DNL Windows]
* [!DNL Outlook] on [!DNL Mac] ([!DNL Microsoft 365])
* [!DNL Outlook] on [!DNL Windows] ([!DNL Microsoft 365])
* [!DNL Outlook] 웹

에 연결되어 있어야 합니다 [!DNL Exchange Server] 또는 [!DNL Office 365] 직접 연결 사용.

클라이언트를 구성할 때는 다음 계정 유형 중 하나를 선택해야 합니다.

* [!DNL Exchange]
* [!DNL Office 365]
* [!DNL Outlook.com]&#x200B;**&#x200B;**&#x200B;클라이언트&#x200B;이 POP3 또는 IMAP와 연결하도록 구성된 경우 [!DNL Workfront] 추가 기능이 로드되지 않습니다.

### 메일 서버 요구 사항 {#mail-server-requirements}

에 연결하면 메일 서버 요구 사항이 기본적으로 충족됩니다 [!DNL Office 365] 또는 [!DNL Outlook.com]. 그러나 On-Premise 설치에 연결된 경우 [!DNL Exchange Server], 다음 요구 사항이 적용됩니다.

* Adobe는 모든 것을 지원합니다 [!DNL Exchange On-Premise] 서버
* [!DNL Exchange Web Services] (EWS)는 사용하도록 설정되어야 하며 인터넷에 노출되어야 합니다.
* 서버에서 유효한 ID 토큰을 발급하려면 서버에 유효한 인증 인증서가 있어야 합니다. 새 설치 [!DNL Exchange Server] 기본 인증 인증서를 포함합니다.

   <!--this used to be here but Dev asked for it to be taken out - logged issue for editing this article on 4-26-2023: For more information, see [Digital certificates and encryption in [!DNL Exchange 2016]](https://technet.microsoft.com/en-us/library/dd351044(v=exchg.160).aspx) and [Set-AuthConfig](https://technet.microsoft.com/en-us/library/jj215766(v=exchg.160).aspx).-->

* 에 액세스하려면 [!DNL Workfront] 에서 추가 [[!DNL Office] 스토어](https://store.office.com/)로 지정하는 경우 클라이언트 액세스 서버가  [https://store.office.com](https://store.office.com/).

지원되는 환경에 대한 자세한 내용은 [[!DNL Microsoft Office 365] 홈 페이지](https://products.office.com/en-us/office-365-home).

## 추가 기능 설치

설정에 대한 자세한 정보 [!DNL Workfront] 용 추가 기능 [!DNL Outlook]를 참조하십시오. [[!DNL Workfront] - 공동 작업 관리](https://appsource.microsoft.com/en-us/product/office/WA104380943?tab=Overview)

* [ [!DNL Outlook 365]에 대한 [!DNL Workfront]](#workfront-for-outlook-365-workfront-for-outlook-365)
* [[!DNL Workfront] 대상 [!DNL Outlook] 웹](#workfront-for-outlook-on-the-web-workfront-for-outlook-on-the-web)
* [[!DNL Workfront] 대상 [!DNL Outlook] on [!DNL Windows] 또는 [!DNL Mac]](#workfront-for-outlook-on-windows-or-mac-workfront-for-outlook-on-windows-or-mac)

### [!DNL Outlook 365]에 대한 [!DNL Workfront] {#workfront-for-outlook-365}

1. in [!DNL Outlook 365]를 클릭하고 **[!UICONTROL 추가 기능 찾아보기]** 아이콘 ![](assets/outlook-add-in-26x26.png)Office 365 인터페이스 맨 위에서 **[!UICONTROL 추가 기능 관리]**.

1. 에서 **[!UICONTROL 추가 기능 검색]** box, 검색 **[!DNL Workfront]** 키를 누른 다음 [!UICONTROL Enter 키].

1. 클릭 **[!UICONTROL 추가]**.

### [!DNL Workfront] 대상 [!DNL Outlook] 웹 {#workfront-for-outlook-on-the-web}

1. 열기 [!DNL Microsoft Outlook] 참조하십시오.
1. 을(를) 클릭합니다. **[!UICONTROL 찾아보기] 추가 기능** 아이콘 ![](assets/outlook-add-in-web-version-20x20.png).

   아이콘을 찾으려면 [에서 추가 기능 사용 [!DNL Outlook] 웹](https://support.microsoft.com/en-us/office/using-add-ins-in-outlook-on-the-web-8f2ce816-5df4-44a5-958c-f7f9d6dabdce#bkmk_addaddinsicon) ( Microsoft 설명서)를 참조하십시오.

1. 검색 대상 **[!DNL Workfront]** 에서 **[!UICONTROL 추가 기능 검색]** field 를 누른 다음 **[!UICONTROL Enter 키]**.

1. 목록에 표시되면 **추가**.

### [!DNL Workfront for Outlook] on [!UICONTROL Windows] 또는 [!DNL Mac] {#workfront-for-outlook-on-windows-or-mac}

1. 클릭 **[!UICONTROL 홈]** > **[!UICONTROL 스토어]** 리본 위에

1. 검색 대상 **[!DNL Workfront]** 에서 **[!UICONTROL 검색]** field 를 누른 다음 **[!UICONTROL Enter 키]**.

1. 토글을 클릭하여 **[!UICONTROL [!DNL Workfront]추가 기능]**.

## 에 로그인합니다. [!DNL Workfront] 변환 전: [!DNL Outlook]

1. in [!DNL Outlook]에서 이메일 메시지를 선택한 다음 **[!DNL Workfront]** 아이콘 을 클릭하여 제품에서 사용할 수 있습니다.
1. 화면의 지침에 따라 로그인하십시오 [!DNL Workfront] 고급 인증, OAuth 2.0 또는 SAML(Security Assertion Markup Language) URL을 사용합니다.

   사용자가에 로그인하기 전에 [!DNL Workfront] saml을 사용하여 추가 기능 [!DNL Workfront] 먼저 활성화 [!DNL Office 365] saml 2.0 솔루션을 사용하여 인증하는 추가 기능입니다. 자세한 내용은 섹션을 참조하십시오 [구성 [!DNL Adobe Workfront] SAML 2.0 사용](../../administration-and-setup/add-users/single-sign-on/configure-workfront-saml-2.md#enable-saml-with-office-365) 기사 [구성 [!DNL Adobe Workfront] SAML 2.0 사용](../../administration-and-setup/add-users/single-sign-on/configure-workfront-saml-2.md).

   >[!NOTE]
   >
   >* 도메인 입력 메시지가 표시되면 [!DNL Workfront] 다음 형식으로 입력하십시오. *yourCompany&#39;sDomain.my.workfront.com*. 일반적으로 회사의 도메인은 회사의 이름입니다.
   >* Enhanced Authentication 은 [!DNL Workfront] 관리자가 이 통합을 위해 이 통합을 사용하도록 설정합니다.


