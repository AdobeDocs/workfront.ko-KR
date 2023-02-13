---
content-type: reference
product-previous: workfront-fusion
product-area: workfront-integrations
keywords: 커넥터
navigation-topic: http-modules
title: Adobe Workfront Fusion에서 HTTP 모듈에서 상호 TLS 사용
description: Adobe Workfront Fusion HTTP 모듈에서 Mutual TLS를 사용할 수 있으므로 정보 거래의 양측에서 상대방의 ID를 확인할 수 있습니다.
author: Becky
feature: Workfront Fusion
exl-id: ace9c404-34de-4bc5-bc77-2e53df36dbd9
source-git-commit: 595d6e3e0a7d87240644bf20efd425917f4d953d
workflow-type: tm+mt
source-wordcount: '632'
ht-degree: 0%

---

# 의 HTTP 모듈에서 상호 TLS 사용 [!DNL Adobe Workfront Fusion]

>[!NOTE]
>
>Adobe Workfront Fusion에는 [!DNL Adobe Workfront Fusion] 라이센스 외에 Adobe Workfront 라이센스도 포함되어 있습니다.

## 상호 TLS 개요

인터넷을 통해 데이터를 보낼 때 데이터가 올바른 위치에 전달되거나 수신자만이 읽을 수 있도록 하는 것이 중요합니다. TLS가 활성화되면 클라이언트(정보 요청 컴퓨터)는 인증서를 사용하여 서버 ID(컴퓨터 제공 정보)를 확인합니다. 이렇게 하면 보안 HTTP 연결이 설정됩니다.

상호 TLS를 사용하면 이러한 ID 확인을 두 가지 방법으로 수행할 수 있습니다. 서버가 인증서를 전송하여 ID를 클라이언트에게 확인하면 클라이언트의 인증서도 요청합니다. 따라서 서버가 정보를 오용하는 사이트나 사용자에게 보내지 않습니다.

>[!INFO]
>
>**예:**
>
>* **TLS**: 어떤 사람이 브라우저에 &quot;MyGreatBank.com&quot;을 입력하면, 은행 정보를 오용하거나 팔 수 있는 웹사이트가 아닌 My Great Bank에 갈 것임을 확인하고 싶어합니다. 그들은 또한 그들의 은행 계좌 정보가 암호화되어 있는지 확인하기를 원합니다.
   >
   >   브라우저(클라이언트)가 MyGreatBank.com(서버)에 연결되면 TLS에서는 ID를 확인하기 위해 MyGreatBank.com의 인증서가 필요합니다. 인증서는 다음과 같은 인증 기관에서 제공합니다. [!DNL DigiCert] 또는 [!DNL Thawte]. 브라우저가 인증 기관을 신뢰하므로 연결을 허용합니다.
>
>* **상호 TLS**: MySoftware.com은 MyGreatBank.com API의 정보를 필요로 하는 소프트웨어 클라이언트입니다. MyGreatBank에서는 신뢰할 수 있는 클라이언트만 서버에 연결할 수 있습니다. 따라서 MyGreatBank.com의 ID를 확인하는 일반 TLS 외에도 TLS/인증 기관 프로세스에서는 MySoftware.com에서 요청을 확인합니다.


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
   <td> <p>작업 자동화 및 통합을 위한 [!UICONTROL Workfront Fusion] </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">제품</td> 
   <td>조직이 구매해야 합니다 [!DNL Adobe Workfront Fusion] 뿐만 아니라 [!DNL Adobe Workfront] 을 참조하십시오.</td> 
  </tr> 
 </tbody> 
</table>

&#42;어떤 계획, 라이센스 유형 또는 액세스 권한을 보유하고 있는지 확인하려면 [!DNL Workfront] 관리자

&#42;&#42;에 대한 자세한 정보 [!DNL Adobe Workfront Fusion] 라이센스 [[!DNL Adobe Workfront Fusion] 라이선스](../../../workfront-fusion/get-started/license-automation-vs-integration.md)

## 사용자 제공 [!DNL Workfront Fusion] 공개 인증서


HTTP 요청을 사용하여 웹 서비스에 연결하면 웹 서비스에는 일반적으로 [!DNL Workfront Fusion] 확인을 위한 공개 인증서 이렇게 하면 웹 서비스에서 인증서가 웹 서비스의에 있는지 확인하는 방법으로 HTTP 요청에 제공된 인증서를 파일의 인증서와 비교할 수 허용 목록에 추가하다 있습니다.

업로드에 대한 지침은 [!DNL Adobe Workfront Fusion] 웹 서비스에 대한 공개 인증서에서 웹 서비스의 설명서를 참조하십시오.

>[!NOTE]
>
>인증서 외에 다른 정보를 제공해야 할 수 있습니다. 웹 서비스에 필요한 작업에 대한 자세한 내용은 웹 서비스의 API 설명서를 참조하십시오.

다음 링크를 사용하여 Workfront Fusion 공개 인증서를 다운로드할 수 있습니다.

### 2022년 11월 14일 - 2023년 7월 15일 인증서

>[!IMPORTANT]
>
>다음 [!DNL Workfront Fusion] 공개 인증서는 2023년 7월 15일에 만료됩니다. 만료되면 웹 서비스에 새 인증서를 업로드해야 합니다. 다음 사항을 권장합니다.
>
>* 만료 날짜를 기록하고 웹 서비스에 인증서를 업로드하도록 직접 미리 알림을 설정하십시오.
>* 이 페이지에 책갈피를 지정하여 새 인증서를 쉽게 찾을 수 있습니다.
>


* [다운로드 [!DNL Workfront Fusion] 인증서 2023](https://cdn.experience.workfront.com/Documentation/Workfront+Fusion+2.0+public+certificates/app_workfrontfusion_com-jul-15-2023+updated.cer)
* [다운로드 [!DNL Workfront Fusion] EU 인증서 2023](https://cdn.experience.workfront.com/Documentation/Workfront+Fusion/app-eu_workfrontfusion_com-jul-15-2023.cer)

   EU에서 사용

<!--

Previous US cert

* [Download [!DNL Workfront Fusion] Certificate 2023](https://cdn.experience.workfront.com/Documentation/Workfront+Fusion/app_workfrontfusion_com-jul-15-2023.cer)

### Certificates for November 17, 2021 - November 14, 2022

>[!IMPORTANT]
>
>These certificates expire on November 14, 2022. Upload the new certificates to the web service as soon as possible.

* [Download Workfront Fusion Certificate 2022](https://cdn.experience.workfront.com/Documentation/Workfront+Fusion+2.0+public+certificates/app_workfrontfusion_com_certificate-chain-2022.crt) 
* [Download Workfront Fusion EU Certificate 2022](https://cdn.experience.workfront.com/Documentation/Workfront+Fusion+2.0+public+certificates/app-eu_workfrontfusion_com_certificate-chain-2022.crt)

  For use in the EU

  -->

## 에서 상호 TLS 활성화 [!DNL Workfront Fusion] HTTP 모듈

모두 [!DNL Workfront Fusion] [!UICONTROL HTTP] 요청 모듈에는 상호 TLS를 활성화하는 옵션이 있습니다.

에서 상호 TLS를 활성화하려면 [!UICONTROL HTTP] 요청 모듈:

1. 추가 [!UICONTROL HTTP] 시나리오에 모듈을 요청합니다.
1. 모듈 구성을 시작합니다.

   구성에 대한 지침은 [!UICONTROL HTTP] 요청 모듈에서는 아래의 해당 문서를 참조하십시오. [[!UICONTROL HTTP] 모듈](../../../workfront-fusion/apps-and-their-modules/http-modules/http-modules-1.md).

1. 활성화 **[!UICONTROL 고급 설정 표시]** 모듈 아래쪽에 있습니다.
1. 활성화 **[!UICONTROL 상호 TLS 사용]**.
