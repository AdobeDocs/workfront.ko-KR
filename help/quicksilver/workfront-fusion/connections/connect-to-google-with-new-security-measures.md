---
product-previous: workfront-fusion
product-area: workfront-integrations
keywords: 커넥터
navigation-topic: connections-annd-webhooks
title: 보안 조치를 업데이트하여  [!DNL Adobe Workfront Fusion] to [!DNL Google Services] 연결
description: Adobe Workfront Fusion 설명서가 새 위치로 이동했습니다. 이 문서는 더 이상 사용되지 않지만, 이 기능을 다루는 새 문서에 대한 링크를 포함합니다.
author: Becky
feature: Workfront Fusion
exl-id: 32dfef7a-7942-4025-8cb9-055d4e28090b
source-git-commit: 2d6af8b4988bd9aab7381daa79dec79e41408c45
workflow-type: tm+mt
source-wordcount: '706'
ht-degree: 0%

---

# 업데이트된 보안 조치를 사용하여 [!DNL Adobe Workfront Fusion]을(를) [!DNL Google Services]에 연결

>[!IMPORTANT]
>
>Adobe Workfront Fusion 설명서가 새 위치로 이동했습니다.
>
>이 문서의 정보는 이제 문서에서 찾을 수 있습니다.
>
>* [업데이트된 보안 조치를 사용하여 Adobe Workfront Fusion을 Google Services에 연결](https://experienceleague.adobe.com/docs/workfront-fusion/using/create-scenarios/connect-to-applications/connect-to-google-with-new-security-measures.html)
>
>모든 책갈피를 업데이트하십시오.
>
>이 문서는 더 이상 업데이트되지 않으며 곧 제거될 예정입니다.

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
   <p>현재 라이선스 요구 사항: [!DNL Workfront Fusion] 라이선스 요구 사항이 없습니다.</p>
   <p>또는</p>
   <p>레거시 라이선스 요구 사항: 작업 자동화 및 통합을 위한 [!UICONTROL [!DNL Workfront Fusion]] </p>
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader">제품</td> 
   <td>
   <p>현재 제품 요구 사항: [!UICONTROL Select] 또는 [!UICONTROL Prime] [!DNL Adobe Workfront] 플랜이 있는 경우 조직에서 이 문서에 설명된 기능을 사용하려면 [!DNL Adobe Workfront Fusion]과(와) [!DNL Adobe Workfront]을(를) 구매해야 합니다. [!DNL Workfront Fusion]이(가) [!UICONTROL Ultimate] [!DNL Workfront] 계획에 포함되어 있습니다.</p>
   <p>또는</p>
   <p>레거시 제품 요구 사항: 이 문서에 설명된 기능을 사용하려면 조직에서 [!DNL Adobe Workfront Fusion]과(와) [!DNL Adobe Workfront]을(를) 구매해야 합니다.</p>
   </td> 
  </tr> 
 </tbody> 
</table>

보유 중인 플랜, 라이선스 유형 또는 액세스 권한을 확인하려면 [!DNL Workfront] 관리자에게 문의하세요.

[!DNL Adobe Workfront Fusion] 라이선스에 대한 자세한 내용은 [[!DNL Adobe Workfront Fusion] 라이선스](../../workfront-fusion/get-started/license-automation-vs-integration.md)를 참조하세요.

## [!DNL Google Services] 제한

[!DNL Google]은(는) 2020년 6월 1일부터 사용자의 API 사용 방법에 대한 제한을 도입했습니다. 이러한 보안 조치를 통해 [!DNL Google] 사용자가 [!DNL Google]에서 개인 데이터를 유출하거나 사용하지 않도록 보호할 수 있습니다. 제한 사항은 [!DNL Gmail] 및 [!DNL Google Drive] 앱과 관련되어 있습니다. 이러한 제한 사항에 대한 자세한 내용은 [[!DNL Google] API 서비스 사용자 데이터 정책](https://developers.google.com/terms/api-services-user-data-policy#additional_requirements_for_specific_api_scopes)의 &quot;특정 API 범위에 대한 추가 요구 사항&quot;을 참조하십시오

제한된 범위에 액세스하려면 연결된 서비스([!DNL Adobe Workfront Fusion] 또는 API를 통해 사용자의 데이터에 액세스하려는 기타 서비스)를 확인하고 서비스가 안전하고 데이터 사용 방법에 대해 투명하게 제공된다는 것을 입증하는 평가 서신을 보유해야 합니다. [!DNL Workfront Fusion]은(는) 제한된 범위에 액세스하기 위한 [!DNL Google]의 모든 요구 사항을 준수합니다. 그러나 [!DNL Workfront Fusion]의 서드파티 연결 서비스 대부분은 평가 서신이 없으므로 [!DNL Google] 약관을 준수하지 않습니다. 따라서 [!DNL Workfront Fusion]은(는) 이러한 서비스에 데이터를 보낼 수 없습니다.

## [!DNL Google Services] 제한에 대한 예외

새로운 제한 사항을 위반하지 않고 평가 서신이 없는 승인되지 않은 서드파티 서비스로 데이터를 보낼 수 있도록 하는 몇 가지 예외가 있습니다. [!DNL Workfront Fusion] OAuth 클라이언트의 [!DNL Google Workspace], 다른 OAuth 클라이언트의 [!DNL Google Workspace] 또는 [!DNL @gmail.com] 및 [!DNL @google.mail.com]에 따라 다릅니다.

* [[!DNL Google Workspace]( [!DNL Workfront Fusion] OAuth 클라이언트 포함)](#g-suite-with-workfront-fusion-oauth-client)
* [다른 OAuth 클라이언트가 있는 [!DNL Google Workspace]](#g-suite-with-another-oauth-client)
* [[!DNL @gmail.com] 및 [!DNL @googlemail.com]](#gmailcom-and-googlemailcom)

### [!DNL Workfront Fusion] OAuth 클라이언트를 사용하는 [!DNL Google Workspace]

[!DNL Workfront Fusion]이(가) [!UICONTROL 도메인 전체 설치] 예외를 사용합니다. 도메인 전체 설치는 [!DNL Google Workspace]명의 사용자에게 적합하며 사용자가 승인되지 않은 서비스를 제한 없이 통합할 수 있도록 합니다. Google Workspace 사용자의 경우 추가 단계를 수행하지 않아도 되며 승인되지 않은 서비스에 직접 연결할 수 있습니다.

### 다른 OAuth 클라이언트가 있는 [!DNL Google Workspace]

[!DNL Workfront Fusion] OAuth 클라이언트를 사용하는 대신 자체 OAuth 클라이언트를 사용하는 사용자 [!DNL Google Workspace]명은 [!UICONTROL 내부] 사용 방법을 통해 [!DNL Google Services]에 연결할 수 있습니다. 이 옵션은 고급 사용자를 위한 것입니다. 지침은 [연결 [!DNL Adobe Workfront Fusion] to [!DNL Google Services] 사용자 지정 OAuth 클라이언트 사용](../../workfront-fusion/connections/connect-fusion-to-google-using-oauth.md)을 참조하십시오.

### [!DNL @gmail.com] 및 [!DNL @googlemail.com] {#gmailcom-and-googlemailcom}

[!DNL @gmail.com] 또는 [!DNL @googlemail.com]을(를) 통해 [!DNL Google Services]에 액세스하는 사용자는 개인 사용 방법을 통해 [!DNL Google Services]에 연결할 수 있습니다. 이 옵션은 고급 사용자를 위한 것입니다. 지침은 [연결 [!DNL Adobe Workfront Fusion] to [!DNL Google Services] 사용자 지정 OAuth 클라이언트 사용](../../workfront-fusion/connections/connect-fusion-to-google-using-oauth.md)을 참조하십시오.

## FAQ

* [ [!DNL Adobe Workfront Fusion] 의 영향을 받는 앱은 무엇입니까?](#what-apps-in-adobe-workfront-fusion-are-affected)
* [ [!DNL Google Workspace] 계정이 있습니까?](#do-i-have-a-g-suite-account)
* [내가 [!DNL @gmail.com] 또는 [!DNL @googlemail.com] 사용자인 경우 어떻게 해야 합니까?](#what-should-i-do-if-im-gmailcom-or-googlemailcom-user)
* [사용자가  [!DNL Google Workspace] 명인 경우 어떻게 해야 합니까?](#what-should-i-do-if-im-a-g-suite-user)

### [!DNL Adobe Workfront Fusion]의 영향을 받는 앱은 무엇입니까? {#what-apps-in-adobe-workfront-fusion-are-affected}

[!DNL Google Drive], [!DNL Gmail] 및 전자 메일([!DNL Gmail] 계정에 연결됨)입니다.

### [!DNL Google Workspace] 계정이 있습니까? {#do-i-have-a-g-suite-account}

메일 주소가 [!DNL @gmail.com] 또는 [!DNL @googlemail.com](으)로 끝나는 경우 귀하의 계정은 [!DNL Google Workspace] 계정이 아닙니다. [!DNL Google] 계정이 @my-company.com과 같은 사용자 정의 도메인으로 끝나는 경우 [!DNL Google Workspace] 계정입니다.

### [!DNL @gmail.com] 또는 [!DNL @googlemail.com] 사용자인 경우 어떻게 해야 합니까? {#what-should-i-do-if-im-gmailcom-or-googlemailcom-user}

이러한 새 제한 사항은 [!DNL Google Drive] 또는 [!DNL Gmail]을(를) 통합하는 경우에만 적용됩니다. [!DNL Google Drive] 또는 [!DNL Gmail]에 연결하려면 다음을 수행할 수 있습니다.

* [!DNL Google Workspace](으)로 전환

  또는

* 사용자 지정 OAuth 클라이언트를 만듭니다. 이 옵션은 고급 사용자를 위한 것입니다.

  지침은 [연결 [!DNL Adobe Workfront Fusion] to [!DNL Google Services] 사용자 지정 OAuth 클라이언트 사용](../../workfront-fusion/connections/connect-fusion-to-google-using-oauth.md)을 참조하십시오.

[!DNL Google Drive] 또는 [!DNL Gmail] 이외의 다른 서비스를 통합하려는 경우에는 이러한 제한이 적용되지 않습니다.

다른 [!DNL Google Services]을(를) [!DNL Workfront Fusion]에 연결하는 방법에 대한 지침은 문서 [시나리오 만들기 [!DNL Adobe Workfront Fusion]](../../workfront-fusion/scenarios/create-a-scenario.md)에서 [모듈의 앱 또는 웹 서비스 연결 [!DNL Workfront Fusion]](../../workfront-fusion/scenarios/create-a-scenario.md#connect)을(를) 참조하십시오.

### [!DNL Google Workspace] 사용자인 경우 어떻게 해야 합니까? {#what-should-i-do-if-im-a-g-suite-user}

필요한 작업이 없습니다.
