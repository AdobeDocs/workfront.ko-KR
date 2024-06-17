---
product-area: workfront-integrations
navigation-topic: workfront-for-outlook
title: 설정 [!DNL Adobe Workfront] 대상 [!DNL Outlook]
description: 다음 [!DNL Adobe Workfront] [!DNL Outlook] 추가 기능을 사용하면 키를 수행할 수 있습니다 [!DNL Workfront] Outlook에서 직접 작업.
author: Becky
feature: Workfront Integrations and Apps
exl-id: 57f0560b-68c2-4654-863e-bd728e76da29
source-git-commit: 4cab7bed6cb4c25d96e70ccce2ece7f6d156f435
workflow-type: tm+mt
source-wordcount: '738'
ht-degree: 0%

---

# 설정 [!DNL Adobe Workfront for Outlook]

<!-- Audited: 12/2023 -->

다음 [!DNL Adobe Workfront] [!DNL Outlook] 추가 기능을 사용하여 다음 키를 수행할 수 있습니다 [!DNL Workfront] Outlook에서 직접 작업:

* 이메일의 정보로 기존 프로젝트, 작업 또는 문제를 업데이트합니다. 자세한 내용은 [에서 기존 개체 업데이트 [!DNL Outlook] 이메일](../../workfront-integrations-and-apps/using-workfront-with-outlook/update-an-existing-object-from-an-outlook-email.md).
* 만들기 [!DNL Workfront] 다음 내의 이메일을 기반으로 한 요청: [!DNL Outlook]. 자세한 내용은 [에서 Adobe Workfront 요청 만들기 [!DNL Outlook] 이메일](../../workfront-integrations-and-apps/using-workfront-with-outlook/create-a-wf-request-from-an-outlook-email.md).
* 의 작업으로 이메일 추가 [!UICONTROL 내 작업] 영역입니다. 자세한 내용은 [추가 [!DNL Outlook] 작업 목록에 작업으로 전자 메일 보내기](../../workfront-integrations-and-apps/using-workfront-with-outlook/add-outlook-email-as-task-to-your-work-list.md).
* 을(를) 통해 댓글에 회신 [!DNL Workfront] 용 추가 기능 [!DNL Outlook]. 다음에 대한 Workfront의 댓글 회신에 대한 자세한 정보: [!DNL Outlook], 참조 [의 댓글에 회신 [!DNL Outlook]](../../workfront-integrations-and-apps/using-workfront-with-outlook/reply-to-a-comment-from-outlook.md).
* 작업 및 문제를 처음부터 만들거나 기존 이메일에서 만듭니다(드래그 앤 드롭 기능 사용). 자세한 내용은 을 참조하십시오. [추가 [!DNL Outlook] 작업 또는 문제로 프로젝트에 이메일 보내기](../../workfront-integrations-and-apps/using-workfront-with-outlook/add-outlook-email-to-project-as-task-or-issue.md).

다음을 추가해야 합니다. [!DNL Workfront] 에 추가 기능 [!DNL Outlook] 계정 사용 전 [!DNL Workfront for Outlook].

를 설치할 수 없는 경우 [!DNL Workfront] 추가 기능 [!DNL Outlook] 계정, 다음 연락처로 문의 [!DNL Workfront] 관리자가 다음을 확인합니다. [!DNL Outlook] 조직에 대한 추가 기능이 활성화되어 있습니다.

을(를) 활성화하는 방법에 대한 자세한 내용 [!DNL Outlook] 조직에 대한 통합은 다음을 참조하십시오. [사용 [!DNL Adobe Workfront for Outlook]](../../administration-and-setup/configure-integrations/enable-workfront-for-outlook.md).

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

이 표의 정보에 대한 자세한 내용은 [Workfront 설명서의 액세스 요구 사항](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## 전제 조건

사용자 [!DNL Workfront] 관리자가 활성화해야 함 [!DNL Outlook for Office] 포함 [!DNL Workfront] 이 통합을 사용하기 전에

## 시스템 요구 사항

다음 응용 프로그램을 사용할 수 있습니다.

* **[!DNL Outlook]웹:** 다음 [!DNL Workfront] 를 사용할 때 추가 기능을 사용할 수 있습니다. [!DNL Outlook] 데스크탑 또는 모바일 디바이스의 웹 브라우저에서. 이 기능은 를 사용할 때도 사용할 수 있습니다 [!DNL Outlook] 웹 앱.
* **[!DNL Outlook]데스크탑 애플리케이션:** 다음 [!DNL Workfront] 추가 기능은 를 사용할 때 사용할 수 있습니다. [!DNL Windows] 및 [!DNL Mac] 데스크탑 버전 [!DNL Outlook] 에 포함됨 [!DNL Office] 패키지.

다음 [!DNL Workfront] 용 추가 기능 [!DNL Outlook] 는 다음 요구 사항을 충족하는 환경에서 지원됩니다.

* [클라이언트 요구 사항](#client-requirements-client-requirements)
* [메일 서버 요구 사항](#mail-server-requirements-mail-server-requirements)

### 클라이언트 요구 사항 {#client-requirements}

Workfront은 다음 버전의 를 지원합니다 [!DNL Outlook]:

* [!DNL Outlook 2013] 또는 나중에 [!DNL Windows]
*[!DNL  Outlook 2016] 또는 나중에 [!DNL Windows]
* [!DNL Outlook] 날짜 [!DNL Mac] ([!DNL Microsoft 365])
* [!DNL Outlook] 날짜 [!DNL Windows] ([!DNL Microsoft 365])
* [!DNL Outlook] 웹에서

다음에 연결되어 있어야 합니다. [!DNL Exchange Server] 또는 [!DNL Office 365] 직접 연결 사용.

클라이언트를 구성할 때 사용자는 다음 계정 유형 중 하나를 선택해야 합니다.

* [!DNL Exchange]
* [!DNL Office 365]
* [!DNL Outlook.com]&#x200B;**&#x200B;**&#x200B;클라이언트&#x200B;이 POP3 또는 IMAP에 연결하도록 구성된 경우 [!DNL Workfront] 추가 기능이 로드되지 않습니다.

### 메일 서버 요구 사항 {#mail-server-requirements}

에 연결할 때 기본적으로 메일 서버 요구 사항이 충족됩니다. [!DNL Office 365] 또는 [!DNL Outlook.com]. 단, 의 온프레미스 설치에 연결되어 있는 경우 [!DNL Exchange Server], 다음 요구 사항이 적용됩니다.

* Workfront은 모든 [!DNL Exchange On-Premise] 서버
* [!DNL Exchange Web Services] (EWS)를 활성화해야 하며 인터넷에 노출되어야 합니다.
* 서버가 유효한 ID 토큰을 발급하려면 서버에 유효한 인증 인증서가 있어야 합니다. 의 새로운 설치 [!DNL Exchange Server] 기본 인증 인증서를 포함합니다.

  <!--this used to be here but Dev asked for it to be taken out - logged issue for editing this article on 4-26-2023: For more information, see [Digital certificates and encryption in [!DNL Exchange 2016]](https://technet.microsoft.com/en-us/library/dd351044(v=exchg.160).aspx) and [Set-AuthConfig](https://technet.microsoft.com/en-us/library/jj215766(v=exchg.160).aspx).-->

* 에 액세스하려면 [!DNL Workfront] 에서 추가 기능 [[!DNL Office] 저장](https://store.office.com/), 클라이언트 액세스 서버는 와 통신할 수 있어야 합니다.  [https://store.office.com](https://store.office.com/).

지원되는 환경에 대한 자세한 내용은 [[!DNL Microsoft Office 365] 홈 페이지](https://products.office.com/en-us/office-365-home).

## 추가 기능 설치

다음에서 Outlook용 Workfront 추가 기능을 가져올 수 있습니다. [Microsoft 스토어](https://appsource.microsoft.com/en-us/product/office/WA104380943?tab=Overview).

### [!DNL Outlook 365]에 대한 [!DNL Workfront] {#workfront-for-outlook-365}

1. 위치 [!DNL Outlook 365]를 클릭하고 **[!UICONTROL 추가 기능 찾아보기]** 아이콘 ![](assets/outlook-add-in-26x26.png)office 365 인터페이스 상단에서 **[!UICONTROL 추가 기능 관리]**.

1. 다음에서 **[!UICONTROL 추가 기능 검색]** 상자, 검색 **[!DNL Workfront]** 그런 다음 누르기 [!UICONTROL 입력].

1. 클릭 **[!UICONTROL 추가]**.

### [!DNL Workfront] 대상 [!DNL Outlook] 웹에서 {#workfront-for-outlook-on-the-web}

1. 열기 [!DNL Microsoft Outlook] 웹 브라우저에서.
1. 다음을 클릭합니다. **[!UICONTROL 찾아보기] 추가 기능** 아이콘 ![](assets/outlook-add-in-web-version-20x20.png).

   아이콘을 찾으려면 다음을 참조하십시오. [에서 추가 기능 사용 [!DNL Outlook] 웹에서](https://support.microsoft.com/en-us/office/using-add-ins-in-outlook-on-the-web-8f2ce816-5df4-44a5-958c-f7f9d6dabdce#bkmk_addaddinsicon) Microsoft 설명서에서 확인할 수 있습니다.

1. 검색 대상 **[!DNL Workfront]** 다음에서 **[!UICONTROL 추가 기능 검색]** 필드, 누르기 **[!UICONTROL 입력]**.

1. 목록에 나타나면 **추가**.

### [!DNL Workfront for Outlook] 날짜 [!UICONTROL Windows] 또는 [!DNL Mac] {#workfront-for-outlook-on-windows-or-mac}

1. 클릭 **[!UICONTROL 홈]** > **[!UICONTROL 저장]** 리본에.

1. 검색 대상 **[!DNL Workfront]** 다음에서 **[!UICONTROL 검색]** 필드, 누르기 **[!UICONTROL 입력]**.

1. 토글을 클릭하여 **[!UICONTROL [!DNL Workfront]추가 기능]**.

## 에 로그인 [!DNL Workfront] 출처: [!DNL Outlook]

1. 위치 [!DNL Outlook]을(를) 클릭하고 이메일 메시지를 선택한 다음 **[!DNL Workfront]** 이메일 헤더의 아이콘
1. 프롬프트의 안내에 따라 다음으로 로그인합니다. [!DNL Workfront] 향상된 인증, OAuth 2.0 또는 SAML(Security Assertion Markup Language) URL 사용.

   사용자가에 로그인하기 전에 [!DNL Workfront] saml을 사용한 추가 기능, a [!DNL Workfront] 관리자가 먼저 활성화해야 함 [!DNL Office 365] saml 2.0 솔루션을 사용하여 인증할 추가 기능입니다. 자세한 내용은 섹션을 참조하십시오 [구성 [!DNL Adobe Workfront] SAML 2.0 사용](../../administration-and-setup/add-users/single-sign-on/configure-workfront-saml-2.md#enable-saml-with-office-365) 이 문서에서 [구성 [!DNL Adobe Workfront] SAML 2.0 사용](../../administration-and-setup/add-users/single-sign-on/configure-workfront-saml-2.md).

   >[!NOTE]
   >
   >* 의 도메인을 입력하라는 메시지가 표시되면 [!DNL Workfront] 계정, 다음 형식을 사용하여 입력: *yourCompany&#39;sDomain.my.workfront.com*. 회사의 도메인은 일반적으로 회사의 이름입니다.
   >* 향상된 인증은 [!DNL Workfront] 관리자가 이 통합을 위해 활성화합니다.

