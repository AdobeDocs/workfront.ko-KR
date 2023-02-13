---
product-previous: workfront-fusion
product-area: workfront-integrations
keywords: 커넥터
navigation-topic: connections-annd-webhooks
title: Connect [!DNL Adobe Workfront Fusion] to [!DNL Google Services] 업데이트된 보안 조치
description: Google은 최근 사용자가 API를 사용할 수 있는 방법에 대한 제한을 도입했습니다. 이 문서에서는 연결 방법에 대해 설명합니다 [!DNL Adobe Workfront Fusion] Google에게 이 업데이트 보안 조치를 처리합니다.
author: Becky
feature: Workfront Fusion
exl-id: 32dfef7a-7942-4025-8cb9-055d4e28090b
source-git-commit: fcaa2136310cad8ef478020a9bae34bbe5520c6d
workflow-type: tm+mt
source-wordcount: '621'
ht-degree: 0%

---

# Connect [!DNL Adobe Workfront Fusion] to [!DNL Google Services] 업데이트된 보안 조치

## 액세스 요구 사항

이 문서의 기능을 사용하려면 다음 액세스 권한이 있어야 합니다.

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] 플랜*</td> 
   <td> <p>[!UICONTROL Pro] 이상</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader">[!DNL Adobe Workfront] 라이센스*</td> 
   <td> <p>[!UICONTROL Plan], [!UICONTROL Work]</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront Fusion] license**</td> 
   <td> <p>[!UICONTROL [!DNL Workfront Fusion] 작업 자동화 및 통합을 위한] </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">제품</td> 
   <td>조직이 구매해야 합니다 [!DNL Adobe Workfront Fusion] 뿐만 아니라 [!DNL Adobe Workfront] 을 참조하십시오.</td> 
  </tr> 
 </tbody> 
</table>

어떤 계획, 라이센스 유형 또는 액세스 권한을 보유하고 있는지 확인하려면 [!DNL Workfront] 관리자

에 대한 자세한 정보 [!DNL Adobe Workfront Fusion] 라이센스 [[!DNL Adobe Workfront Fusion] 라이선스](../../workfront-fusion/get-started/license-automation-vs-integration.md).

## [!DNL Google Services] 제한 사항

[!DNL Google] 2020년 6월 1일부터 사용자가 API를 사용할 수 있는 방법에 대한 제한을 도입했습니다. 이러한 보안 조치는 [!DNL Google] 개인 데이터가 유출되거나 오용되지 않는 사용자 [!DNL Google]. 제한 사항은 [!DNL Gmail] 및 [!DNL Google Drive] 앱을 사용할 수 없습니다. 이러한 제한 사항에 대한 자세한 내용은 [[!DNL Google] API 서비스 사용자 데이터 정책](https://developers.google.com/terms/api-services-user-data-policy#additional_requirements_for_specific_api_scopes)

제한된 범위에 액세스하려면 연결된 서비스([!DNL Adobe Workfront Fusion] 또는 API를 통해 사용자의 데이터에 액세스하려는 기타 모든 서비스)는 확인되어야 하며 서비스의 데이터 사용 방법에 대해 안전하고 투명하게 확인을 위해 평가 서신이 있어야 합니다. [!DNL Workfront Fusion] 모든 [!DNL Google]제한된 범위 액세스에 대한 의 요구 사항입니다. 그러나 대부분의 타사 연결 서비스는 [!DNL Workfront Fusion] 평가서가 없으므로 [!DNL Google] 약관. 그것 때문에 [!DNL Workfront Fusion] 은(는) 이러한 서비스에 데이터를 보낼 수 없습니다.

## 예외 [!DNL Google Services] 제한 사항

새로운 제한 사항을 위반하지 않고 평가서가 없는 승인되지 않은 타사 서비스에 데이터를 보낼 수 있는 몇 가지 예외가 있습니다. 두 차원은 서로 다릅니다 [!DNL G Suite] 사용 [!DNL Workfront Fusion] OAuth 클라이언트, [!DNL G Suite] 다른 OAuth 클라이언트 사용 또는 [!DNL @gmail.com] 및 [!DNL @google.mail.com].

* [[!DNL G 세트] [!DNL Workfront Fusion] OAuth 클라이언트](#g-suite-with-workfront-fusion-oauth-client)
* [다른 OAuth 클라이언트가 있는 [!DNL G suite]](#g-suite-with-another-oauth-client)
* [[!DNL @gmail.com] 및 [!DNL @googlemail.com]](#gmailcom-and-googlemailcom)

### [!DNL G suite] with [!DNL Workfront Fusion] OAuth 클라이언트

[!DNL Workfront Fusion] 사용 [!UICONTROL 도메인 전체 설치] 예외. 도메인 전체 설치는 [!DNL G Suite] 사용자 및 를 사용하면 제한 없이 승인되지 않은 서비스를 통합할 수 있습니다. G Suite 사용자인 경우 추가 단계를 수행하지 않아도 되며 승인되지 않은 서비스에 직접 연결할 수 있습니다.

### [!DNL G suite] 다른 OAuth 클라이언트 사용

[!DNL G Suite] 를 사용하는 대신 고유한 OAuth 클라이언트를 사용하는 사용자 [!DNL Workfront Fusion] OAuth 클라이언트가 연결할 수 있음 [!DNL Google Services] 사용 [!UICONTROL 내부] 접근 방식을 사용합니다. 이 옵션은 고급 사용자를 위한 것입니다. 자세한 내용은 [Connect [!DNL Adobe Workfront Fusion] to [!DNL Google Services] 사용자 지정 OAuth 클라이언트 사용](../../workfront-fusion/connections/connect-fusion-to-google-using-oauth.md).

### [!DNL @gmail.com] 및 [!DNL @googlemail.com] {#gmailcom-and-googlemailcom}

액세스할 사용자 [!DNL Google Services] through [!DNL @gmail.com] 또는 [!DNL @googlemail.com] 연결 가능 [!DNL Google Services] 개인 사용 방법을 사용합니다. 이 옵션은 고급 사용자를 위한 것입니다. 자세한 내용은 [Connect [!DNL Adobe Workfront Fusion] to [!DNL Google Services] 사용자 지정 OAuth 클라이언트 사용](../../workfront-fusion/connections/connect-fusion-to-google-using-oauth.md).

## FAQ

* [의 앱 [!DNL Adobe Workfront Fusion] 영향을 받습니까?](#what-apps-in-adobe-workfront-fusion-are-affected)
* [[!DNL G Suite] 계정이 있습니까?](#do-i-have-a-g-suite-account)
* [만약 내가 [!DNL @gmail.com] 또는 [!DNL @googlemail.com] 사용하시겠습니까?](#what-should-i-do-if-im-gmailcom-or-googlemailcom-user)
* [[!DNL G Suite] 사용자는 어떻게 해야 합니까?](#what-should-i-do-if-im-a-g-suite-user)

### 의 앱 [!DNL Adobe Workfront Fusion] 영향을 받습니까? {#what-apps-in-adobe-workfront-fusion-are-affected}

[!DNL Google Drive], [!DNL Gmail], 및 이메일(에 연결됨) [!DNL Gmail] 계정)에 액세스할 수 없습니다.

### 혹시 하나 있나요 [!DNL G Suite] 계정? {#do-i-have-a-g-suite-account}

이메일 주소가 [!DNL @gmail.com] 또는 [!DNL @googlemail.com] 계정이 아닙니다. [!DNL G Suite] 계정이 필요합니다. 만약 [!DNL Google] 계정은 @my-company.com과 같은 사용자 지정 도메인으로 끝나는 경우 [!DNL G Suite] 계정이 필요합니다.

### 만약 내가 [!DNL @gmail.com] 또는 [!DNL @googlemail.com] 사용하시겠습니까? {#what-should-i-do-if-im-gmailcom-or-googlemailcom-user}

이러한 새 제한 사항은 통합하려는 경우에만 적용됩니다 [!DNL Google Drive] 또는 [!DNL Gmail]. 연결하려는 경우 [!DNL Google Drive] 또는 [!DNL Gmail], 다음 작업을 수행할 수 있습니다.

* 다음으로 전환 [!DNL G Suite]

   또는

* 사용자 지정 OAuth 클라이언트를 만듭니다. 이 옵션은 고급 사용자를 위한 것입니다.

   자세한 내용은 [Connect [!DNL Adobe Workfront Fusion] to [!DNL Google Services] 사용자 지정 OAuth 클라이언트 사용](../../workfront-fusion/connections/connect-fusion-to-google-using-oauth.md).

다음 이외의 서비스를 통합하려는 경우 [!DNL Google Drive] 또는 [!DNL Gmail]에는 이러한 제한 사항이 적용되지 않습니다.

기타 연결에 대한 지침 [!DNL Google Services] to [!DNL Workfront Fusion]를 참조하십시오. [모듈의 앱 또는 웹 서비스를 [!DNL Workfront Fusion]](../../workfront-fusion/scenarios/create-a-scenario.md#connect) 기사 [에서 시나리오 만들기 [!DNL Adobe Workfront Fusion]](../../workfront-fusion/scenarios/create-a-scenario.md).

### 만약 내가.. [!DNL G Suite] 사용하시겠습니까? {#what-should-i-do-if-im-a-g-suite-user}

필요한 작업이 없습니다.
