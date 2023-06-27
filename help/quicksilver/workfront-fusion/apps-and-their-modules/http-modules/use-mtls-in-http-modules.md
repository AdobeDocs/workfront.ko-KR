---
content-type: reference
product-previous: workfront-fusion
product-area: workfront-integrations
keywords: 커넥터
navigation-topic: http-modules
title: Adobe Workfront Fusion의 HTTP 모듈에서 상호 TLS 사용
description: Adobe Workfront Fusion HTTP 모듈에서 Mutual TLS를 사용하여 정보 트랜잭션의 양쪽에서 상대방의 ID를 확인할 수 있습니다.
author: Becky
feature: Workfront Fusion
exl-id: ace9c404-34de-4bc5-bc77-2e53df36dbd9
source-git-commit: 8b4182ae2b32488a02cacc16fcb6a246fcb571fd
workflow-type: tm+mt
source-wordcount: '663'
ht-degree: 0%

---

# 의 HTTP 모듈에서 상호 TLS 사용 [!DNL Adobe Workfront Fusion]

>[!NOTE]
>
>Adobe Workfront Fusion에는 [!DNL Adobe Workfront Fusion] Adobe Workfront 라이선스 이외의 라이선스.

## 상호 TLS 개요

인터넷을 통해 데이터를 보낼 때는 데이터를 올바른 위치로 이동하거나 올바른 위치에서 가져오는지, 의도한 수신자만 읽을 수 있는지 확인하는 것이 중요합니다. TLS가 활성화된 상태에서 클라이언트(정보를 요청하는 컴퓨터)는 인증서를 사용하여 서버(정보를 제공하는 컴퓨터)의 ID를 확인합니다. 이렇게 하면 보안 HTTP 연결이 설정됩니다.

상호 TLS를 통해 이 신원 확인은 두 가지 방법으로 가능하다. 서버가 해당 ID를 확인하기 위해 인증서를 클라이언트에 보내면 클라이언트의 인증서도 요청합니다. 이렇게 하면 서버가 정보를 오용할 사이트나 사용자에게 보내지 않습니다.

>[!INFO]
>
>**예:**
>
>* **TLS**: 브라우저에 &quot;MyGreatBank.com&quot;을 입력하면 뱅킹 정보를 오용하거나 판매할 수 있는 웹 사이트가 아니라 My Great Bank로 이동하는지 확인하려고 합니다. 그들은 또한 그들의 은행 계좌 정보가 암호화되어 있는지 확인하기를 원한다.
>
>   브라우저(클라이언트)가 MyGreatBank.com(서버)에 연결하면 TLS는 MyGreatBank.com에서 인증서를 요청하여 ID를 확인합니다. 인증서는 와 같은 인증 기관에서 제공합니다. [!DNL DigiCert] 또는 [!DNL Thawte]. 브라우저는 인증 기관을 신뢰하므로 연결을 허용합니다.
>
>* **상호 TLS**: MySoftware.com 는 MyGreatBank.com API의 정보가 필요한 소프트웨어 클라이언트입니다. MyGreatBank는 신뢰할 수 있는 클라이언트만 서버에 연결할 수 있도록 합니다. 따라서 MyGreatBank.com의 ID를 확인하는 일반 TLS 외에 TLS/인증서 기관 프로세스는 MySoftware.com의 요청도 확인합니다.

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

&#42;보유 중인 플랜, 라이선스 유형 또는 액세스 권한을 알아보려면 [!DNL Workfront] 관리자.

&#42;&#42;다음에 대한 정보: [!DNL Adobe Workfront Fusion] 라이센스, 참조 [[!DNL Adobe Workfront Fusion] 라이선스](../../../workfront-fusion/get-started/license-automation-vs-integration.md)

## 제공 [!DNL Workfront Fusion] 공개 인증서


HTTP 요청을 사용하여 웹 서비스에 연결할 때 웹 서비스에는 일반적으로 [!DNL Workfront Fusion] 확인을 위한 공개 인증서. 이렇게 하면 웹 서비스가 인증서가 웹 서비스의 허용 목록에 추가하다에 있는지 확인하는 방법으로 HTTP 요청에 표시된 인증서를 파일에 있는 인증서와 비교할 수 있습니다.

업로드 지침: [!DNL Adobe Workfront Fusion] 웹 서비스에 대한 공개 인증서는 웹 서비스의 설명서를 참조하십시오.

>[!NOTE]
>
>인증서 외에 다른 정보를 제공해야 할 수도 있습니다. 웹 서비스에 필요한 사항에 대한 자세한 내용은 웹 서비스의 API 설명서를 참조하십시오.

다음 링크를 사용하여 Workfront Fusion 공개 인증서를 다운로드할 수 있습니다.

### 2023년 5월 25일 - 2024년 6월 9일 인증서

>[!IMPORTANT]
>
>* 다음 [!DNL Workfront Fusion] 공개 인증서는 2024년 6월 9일에 만료됩니다. 만료되면 웹 서비스에 새 인증서를 업로드해야 합니다. 권장 사항:
>
>   * 만료 날짜를 기록하고 인증서를 웹 서비스에 업로드하도록 미리 알림을 설정하십시오.
>   * 새 인증서를 쉽게 찾으려면 이 페이지에 책갈피를 지정합니다.
>
>* 이는 비 와일드카드 mTLS 인증서입니다.

* [다운로드 [!DNL Workfront Fusion] 인증서 2023](/help/quicksilver/workfront-fusion/apps-and-their-modules/http-modules/assets/fusion-prod-eu-mtls-certificate.pem)
* [다운로드 [!DNL Workfront Fusion] EU 인증서 2023](/help/quicksilver/workfront-fusion/apps-and-their-modules/http-modules/assets/fusion-prod-eu-mtls-certificate.pem)

  유럽연합용

<!--

### Certificates for November 14, 2022 - July 15, 2023

>[!IMPORTANT]
>
>* These [!DNL Workfront Fusion] public certificates expire on July 15, 2023.
>* These are wildcard mTLS certificates.

* [Download [!DNL Workfront Fusion] Certificate 2023](https://cdn.experience.workfront.com/Documentation/Workfront+Fusion+2.0+public+certificates/app_workfrontfusion_com-jul-15-2023+updated.cer)
* [Download [!DNL Workfront Fusion] EU Certificate 2023](https://cdn.experience.workfront.com/Documentation/Workfront+Fusion/app-eu_workfrontfusion_com-jul-15-2023.cer)

   For use in the EU 

   -->

## 에서 상호 TLS 활성화 [!DNL Workfront Fusion] HTTP 모듈

모두 [!DNL Workfront Fusion] [!UICONTROL HTTP] 요청 모듈에는 상호 TLS를 활성화하는 옵션이 있습니다.

에서 상호 TLS를 활성화하려면 [!UICONTROL HTTP] 요청 모듈:

1. 추가 [!UICONTROL HTTP] 시나리오에 모듈을 요청합니다.
1. 모듈 구성을 시작합니다.

   구성에 대한 지침은 [!UICONTROL HTTP] 모듈 요청, 아래의 해당 문서 참조 [[!UICONTROL HTTP] 모듈](../../../workfront-fusion/apps-and-their-modules/http-modules/http-modules-1.md).

1. 사용 **[!UICONTROL 고급 설정 표시]** 모듈 하단 근처에 있습니다.
1. 사용 **[!UICONTROL 상호 TLS 사용]**.
