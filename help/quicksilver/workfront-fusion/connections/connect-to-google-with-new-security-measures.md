---
product-previous: workfront-fusion
product-area: workfront-integrations
keywords: 커넥터
navigation-topic: connections-annd-webhooks
title: 연결 [!DNL Adobe Workfront Fusion] 끝 [!DNL Google Services] 업데이트된 보안 조치 포함
description: Google은 최근 사용자가 API를 사용하는 방법에 대한 제한 사항을 도입했습니다. 이 문서에서는 연결 방법에 대해 설명합니다 [!DNL Adobe Workfront Fusion] Google에 이러한 업데이트 보안 조치를 적용하십시오.
author: Becky
feature: Workfront Fusion
exl-id: 32dfef7a-7942-4025-8cb9-055d4e28090b
source-git-commit: 0915dcce45b271ee18cdd8af5db4f0eb01f3cced
workflow-type: tm+mt
source-wordcount: '669'
ht-degree: 0%

---

# 연결 [!DNL Adobe Workfront Fusion] 끝 [!DNL Google Services] 업데이트된 보안 조치 포함

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
   <td role="rowheader">[!DNL Adobe Workfront Fusion] 라이센스**</td> 
   <td>
   <p>현재 라이선스 요구 사항: 아니요 [!DNL Workfront Fusion] 라이센스 요구 사항.</p>
   <p>또는</p>
   <p>기존 라이선스 요구 사항: [!UICONTROL [!DNL Workfront Fusion] for Work Automation and Integration] </p>
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader">제품</td> 
   <td>
   <p>현재 제품 요구 사항: [!UICONTROL Select] 또는 [!UICONTROL Prime]이 있는 경우 [!DNL Adobe Workfront] 플랜, 조직은 다음을 구매해야 합니다. [!DNL Adobe Workfront Fusion] 뿐만 아니라 [!DNL Adobe Workfront] 이 문서에 설명된 기능을 사용하십시오. [!DNL Workfront Fusion] [!UICONTROL Ultimate]에 포함되어 있습니다. [!DNL Workfront] 계획.</p>
   <p>또는</p>
   <p>레거시 제품 요구 사항: 조직에서 구매해야 함 [!DNL Adobe Workfront Fusion] 뿐만 아니라 [!DNL Adobe Workfront] 이 문서에 설명된 기능을 사용하십시오.</p>
   </td> 
  </tr> 
 </tbody> 
</table>

보유 중인 플랜, 라이선스 유형 또는 액세스 권한을 알아보려면 [!DNL Workfront] 관리자.

다음에 대한 정보: [!DNL Adobe Workfront Fusion] 라이센스, 참조 [[!DNL Adobe Workfront Fusion] 라이선스](../../workfront-fusion/get-started/license-automation-vs-integration.md).

## [!DNL Google Services] 제한 사항

[!DNL Google] 2020년 6월 1일부터 사용자가 API를 사용할 수 있는 방법에 대한 제한 사항이 도입되었습니다. 이러한 보안 조치들은 [!DNL Google] 다음에 대한 개인 데이터 유출 또는 오용 사용자 [!DNL Google]. 제한 사항은 다음과 관련이 있습니다. [!DNL Gmail] 및 [!DNL Google Drive] 앱. 이러한 제한 사항에 대한 자세한 내용은 의 &quot;특정 API 범위에 대한 추가 요구 사항&quot;을 참조하십시오 [[!DNL Google] API 서비스 사용자 데이터 정책](https://developers.google.com/terms/api-services-user-data-policy#additional_requirements_for_specific_api_scopes)

제한된 범위에 액세스하려면 연결된 서비스([!DNL Adobe Workfront Fusion] 또는 API를 통해 사용자의 데이터에 액세스하려는 다른 서비스는 확인되어야 하며 서비스가 데이터를 사용하는 방법에 대해 안전하고 투명하다는 것을 입증하기 위해 평가 서신이 있어야 합니다. [!DNL Workfront Fusion] 다음을 모두 준수 [!DNL Google]제한된 범위에 액세스하기 위한 의 요구 사항. 그러나 대부분의 서드파티 연결 서비스는 [!DNL Workfront Fusion] 평가 서신이 없으므로 이에 따르지 않음 [!DNL Google] 용어. 그렇기 때문에, [!DNL Workfront Fusion] 은(는) 이러한 서비스에 데이터를 보낼 수 없습니다.

## 다음에 대한 예외 [!DNL Google Services] 제한 사항

새로운 제한 사항을 위반하지 않고 평가 서신이 없는 승인되지 않은 서드파티 서비스로 데이터를 보낼 수 있도록 하는 몇 가지 예외가 있습니다. 다음 항목에 따라 다릅니다. [!DNL G Suite] (으)로 [!DNL Workfront Fusion] OAuth 클라이언트, [!DNL G Suite] 다른 OAuth 클라이언트 또는 [!DNL @gmail.com] 및 [!DNL @google.mail.com].

* [다음을 포함한 [!DNL G suite] [!DNL Workfront Fusion] OAuth 클라이언트](#g-suite-with-workfront-fusion-oauth-client)
* [다른 OAuth 클라이언트와 [!DNL G suite]](#g-suite-with-another-oauth-client)
* [[!DNL @gmail.com] 및 [!DNL @googlemail.com]](#gmailcom-and-googlemailcom)

### [!DNL G suite] 포함 [!DNL Workfront Fusion] OAuth 클라이언트

[!DNL Workfront Fusion] 를 사용합니다. [!UICONTROL 도메인 전체 설치] 예외. 도메인 전체 설치는 [!DNL G Suite] 를 사용하면 사용자가 승인되지 않은 서비스를 제한 없이 통합할 수 있습니다. G Suite 사용자의 경우 추가 단계를 수행하지 않아도 되며 승인되지 않은 서비스에 직접 연결할 수 있습니다.

### [!DNL G suite] 다른 OAuth 클라이언트 사용

[!DNL G Suite] 를 사용하는 대신 자체 OAuth 클라이언트를 사용하는 것을 선호하는 사용자 [!DNL Workfront Fusion] OAuth 클라이언트이에 연결할 수 있음 [!DNL Google Services] 다음을 통해 [!UICONTROL 내부] 접근 방식을 사용하십시오. 이 옵션은 고급 사용자를 위한 것입니다. 자세한 내용은 [연결 [!DNL Adobe Workfront Fusion] 끝 [!DNL Google Services] 사용자 정의 OAuth 클라이언트 사용](../../workfront-fusion/connections/connect-fusion-to-google-using-oauth.md).

### [!DNL @gmail.com] 및 [!DNL @googlemail.com] {#gmailcom-and-googlemailcom}

액세스 권한이 있는 사용자 [!DNL Google Services] 에서 [!DNL @gmail.com] 또는 [!DNL @googlemail.com] 연결 가능 대상: [!DNL Google Services] 개인 사용자 사용 접근 방식을 통해. 이 옵션은 고급 사용자를 위한 것입니다. 자세한 내용은 [연결 [!DNL Adobe Workfront Fusion] 끝 [!DNL Google Services] 사용자 정의 OAuth 클라이언트 사용](../../workfront-fusion/connections/connect-fusion-to-google-using-oauth.md).

## FAQ

* [의 앱 [!DNL Adobe Workfront Fusion] 영향을 받습니까?](#what-apps-in-adobe-workfront-fusion-are-affected)
* [[!DNL G Suite] 계정이 있습니까?](#do-i-have-a-g-suite-account)
* [만약 그렇다면 어떻게 해야 하나요 [!DNL @gmail.com] 또는 [!DNL @googlemail.com] 사용자?](#what-should-i-do-if-im-gmailcom-or-googlemailcom-user)
* [[!DNL G Suite] 사용자인 경우 어떻게 해야 합니까?](#what-should-i-do-if-im-a-g-suite-user)

### 의 앱 [!DNL Adobe Workfront Fusion] 영향을 받습니까? {#what-apps-in-adobe-workfront-fusion-are-affected}

[!DNL Google Drive], [!DNL Gmail], 및 이메일(에 연결됨) [!DNL Gmail] 계정).

### 가지고 있어요 [!DNL G Suite] 계정? {#do-i-have-a-g-suite-account}

이메일 주소가 다음으로 끝나는 경우 [!DNL @gmail.com] 또는 [!DNL @googlemail.com] 계정이 다음이 아님 [!DNL G Suite] 계정입니다. 다음의 경우 [!DNL Google] 계정은 @my-company.com과 같은 사용자 정의 도메인으로 끝나고 [!DNL G Suite] 계정입니다.

### 만약 그렇다면 어떻게 해야 하나요 [!DNL @gmail.com] 또는 [!DNL @googlemail.com] 사용자? {#what-should-i-do-if-im-gmailcom-or-googlemailcom-user}

이러한 새 제한 사항은 을 통합하는 경우에만 적용됩니다 [!DNL Google Drive] 또는 [!DNL Gmail]. 을(를)에 연결하려면 [!DNL Google Drive] 또는 [!DNL Gmail], 다음을 수행할 수 있습니다.

* 다음으로 전환 [!DNL G Suite]

  또는

* 사용자 지정 OAuth 클라이언트를 만듭니다. 이 옵션은 고급 사용자를 위한 것입니다.

  자세한 내용은 [연결 [!DNL Adobe Workfront Fusion] 끝 [!DNL Google Services] 사용자 정의 OAuth 클라이언트 사용](../../workfront-fusion/connections/connect-fusion-to-google-using-oauth.md).

다른 서비스를 통합하려는 경우 [!DNL Google Drive] 또는 [!DNL Gmail], 이러한 제한 사항은 적용되지 않습니다.

기타 연결에 대한 지침 [!DNL Google Services] 끝 [!DNL Workfront Fusion], 참조 [모듈의 앱 또는 웹 서비스 연결 [!DNL Workfront Fusion]](../../workfront-fusion/scenarios/create-a-scenario.md#connect) 이 문서에서 [에서 시나리오 만들기 [!DNL Adobe Workfront Fusion]](../../workfront-fusion/scenarios/create-a-scenario.md).

### 만약 내가 학생이라면 어떻게 해야 할까 [!DNL G Suite] 사용자? {#what-should-i-do-if-im-a-g-suite-user}

필요한 작업이 없습니다.
