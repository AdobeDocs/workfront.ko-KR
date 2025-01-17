---
product-previous: workfront-fusion
product-area: workfront-integrations
navigation-topic: connections-annd-webhooks
title: API 토큰 인증을 사용하는 웹 서비스에  [!DNL Adobe Workfront Fusion] 연결
description: Adobe Workfront Fusion 설명서가 새 위치로 이동했습니다. 이 문서는 더 이상 사용되지 않지만, 이 기능을 다루는 새 문서에 대한 링크를 포함합니다.
author: Becky
feature: Workfront Fusion
exl-id: 0feb745a-1ee0-4b29-92ab-14c12a8647d4
source-git-commit: 2d6af8b4988bd9aab7381daa79dec79e41408c45
workflow-type: tm+mt
source-wordcount: '1008'
ht-degree: 0%

---

# API 토큰 인증을 사용하는 웹 서비스에 [!DNL Adobe Workfront Fusion] 연결

>[!IMPORTANT]
>
>Adobe Workfront Fusion 설명서가 새 위치로 이동했습니다.
>
>이 문서의 정보는 이제 문서에서 찾을 수 있습니다.
>
>* [API 토큰 인증을 사용하는 웹 서비스에 Adobe Workfront Fusion 연결](https://experienceleague.adobe.com/docs/workfront-fusion/using/create-scenarios/connect-to-applications/connect-wf-web-service-uses-api-token-auth.html)
>
>모든 책갈피를 업데이트하십시오.
>
>이 문서는 더 이상 업데이트되지 않으며 곧 제거될 예정입니다.

일부 서비스에서는 [!DNL Adobe Workfront Fusion]과(와) 같은 통합 솔루션으로 시나리오에서 쉽게 사용할 수 있는 앱을 만들 수 없습니다.

이 상황에 대한 해결 방법이 있습니다. [!DNL Workfront Fusion]의 [!UICONTROL HTTP] 모듈을 사용하여 원하는 서비스(앱)를 [!DNL Workfront Fusion]에 연결할 수 있습니다.

이 문서에서는 API 키/API 토큰을 사용하여 거의 모든 웹 서비스를 [!DNL Workfront Fusion]에 연결하는 방법에 대해 설명합니다.

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

## API 토큰을 사용하는 웹 서비스에 연결

API 토큰을 통해 서비스를 연결하는 절차는 대부분의 웹 서비스에서 유사합니다.

1. [새 응용 프로그램을 만들고 API 토큰을 얻기](#create-a-new-application-and-obtain-the-api-token) 섹션에 설명된 대로 웹 서비스의 웹 사이트에서 응용 프로그램을 만듭니다.
1. API 키 또는 API 토큰을 가져옵니다.
1. [!DNL Workfront Fusion]의 [!UICONTROL HTTP] > [!UICONTROL 요청 만들기] 모듈을 시나리오에 추가합니다.
1. 웹 서비스의 API 설명서에 따라 모듈을 설정하고 이 문서의 [[!UICONTROL HTTP] 모듈 설정](#set-up-the-http-module) 섹션에 설명된 대로 시나리오를 실행합니다.

>[!NOTE]
>
>이 문서에서 [!DNL Pushover] 알림 서비스를 예로 사용하겠습니다.

## 새 애플리케이션 만들기 및 API 토큰 가져오기

>[!NOTE]
>
>웹 서비스가 API 키 또는 API 토큰을 만들고 배포하는 방법은 매우 다양합니다. 원하는 웹 서비스에 대한 API 키 및 토큰을 얻는 방법에 대한 지침은 서비스 웹 사이트에서 &quot;API 키&quot; 또는 &quot;API 토큰&quot;을 검색합니다.
>
>푸시 API 키를 얻는 방법에 대한 지침은 찾을 수 있는 예제의 경우에만 포함됩니다.

1. [!DNL Pushover] 계정에 로그인합니다.
1. 페이지 하단에서 **[!UICONTROL 응용 프로그램/API 토큰 만들기]**&#x200B;를 클릭합니다.
1. 응용 프로그램 정보를 입력하고 **[!UICONTROL 응용 프로그램 만들기]**&#x200B;를 클릭합니다.
1. 제공된 API 토큰을 안전한 장소에 저장합니다. 원하는 웹 서비스([!DNL Pushover], 이 경우)에 연결하려면 [!DNL Workfront Fusion] [!UICONTROL HTTP] >[!UICONTROL 요청] 모듈에 필요합니다.

## [!UICONTROL HTTP] 모듈 설정

웹 서비스를 [!DNL Workfront Fusion] 시나리오에 연결하려면 시나리오에서 [!UICONTROL HTTP] >[!UICONTROL 요청 만들기] 모듈을 사용하고 웹 서비스의 API 설명서에 따라 모듈을 설정해야 합니다.

1. 시나리오에 [!UICONTROL HTTP] >[!UICONTROL 요청 만들기] 모듈을 추가합니다.
1. [!DNL Workfront Fusion]을(를) 사용하여 메시지를 푸시하려면 다음과 같이 HTTP 모듈을 설정합니다.

   >[!NOTE]
   >
   >이러한 모듈 설정은 [!DNL Pushover] 웹 서비스 API 설명서에 해당합니다. 설정은 다른 웹 서비스에 대해 다를 수 있습니다. 예를 들어 API 토큰은 [!UICONTROL Header]에 삽입되고 [!UICONTROL Body] 필드에는 삽입되지 않을 수 있습니다.

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">[!UICONTROL URL]</td> 
      <td> <p><code>https://api.pushover.net/1/messages.json</code> </p> <p>URL 필드에는 웹 서비스의 API 설명서에서 찾을 수 있는 끝점이 포함됩니다.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL 메서드]</td> 
      <td> <p><code>[!DNL POST]</code> </p> <p>사용되는 메서드는 해당 끝점에 따라 다릅니다. 메시지 푸시를 위한 푸시 엔드포인트는 POST 메서드를 사용합니다.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"> <p>[!UICONTROL Headers]</p> </td> 
      <td> <p>일부 웹 서비스는 헤더를 사용하여 API 토큰 인증 또는 기타 매개 변수를 지정할 수 있습니다. 메시지 푸시에 대한 푸시 엔드포인트가 모든 요청 유형에 대해 본문(아래 참조)을 사용하므로 이 예에서는 그렇지 않습니다.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"> <p>[!UICONTROL 쿼리 문자열]</p> </td> 
      <td> <p>일부 웹 서비스는 쿼리 문자열을 사용하여 다른 매개 변수를 지정할 수 있습니다. [!DNL Pushover] 웹 서비스가 모든 요청 유형에 대해 [!UICONTROL Body](아래 참조)를 사용하므로 이 예제에서는 그렇지 않습니다.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"> <p>[!UICONTROL Body Type]</p> </td> 
      <td> <p><code>Raw</code> </p> <p>이 설정을 사용하면 아래의 [!UICONTROL 콘텐츠 유형] 필드에서 JSON 콘텐츠 유형을 선택할 수 있습니다.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"> <p>[!UICONTROL 콘텐츠 유형]</p> </td> 
      <td> <p><code>JSON (application/json)</code> </p> <p>JSON은 [!UICONTROL Pushover] 앱에서 요구하는 콘텐츠 유형입니다. 이는 다른 웹 서비스와 다를 수 있습니다.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"> <p>[!UICONTROL 요청 컨텐츠]</p> </td> 
      <td> <p>[!UICONTROL Body] 요청 컨텐츠를 JSON 형식으로 입력합니다. 이 문서의 <a href="#json-body-mapped-using-the-json-create-json-module" class="MCXref xref">[!UICONTROL JSON] &gt; [!UICONTROL JSON] 만들기 모듈</a>을 사용하여 매핑된 JSON 본문에 설명된 대로 [!UICONTROL JSON] &gt; [!UICONTROL JSON] 모듈을 사용할 수 있습니다. 또는 이 문서의 <a href="#json-body-entered-manually" class="MCXref xref">수동으로 입력한 JSON 본문</a>에 설명된 대로 JSON 콘텐츠를 수동으로 입력할 수 있습니다.</p> <p>해당 웹 서비스에 필요한 매개 변수에 대해서는 웹 서비스의 API 설명서 를 참조하십시오.</p> </td> 
     </tr> 
    </tbody> 
   </table>

## 수동으로 입력한 JSON 본문

매개 변수와 값을 JSON 형식으로 지정하십시오.

>[!INFO]
>
>**예:**
>
>```
>{"user":"12345c2ecu1hq42ypqzhswbyam34",
>"token":"123459evz8aepwtxydndydgyumbfx",
>"message":"Hello World!",
>"title":"The Push Notification"}
>```

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL user]</p> </td> 
   <td> <p>사용자 키. [!DNL Pushover] 대시보드에서 찾을 수 있습니다.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL token] </td> 
   <td> <p>생성된 API 토큰/API 키로 [!DNL Pushover] 앱을 만들었습니다.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL message] </td> 
   <td> <p>장치로 전송되는 푸시 알림의 텍스트 콘텐츠입니다.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL title] </td> 
   <td> <p>(선택 사항) 메시지 제목입니다. 값을 입력하지 않으면 앱 이름이 사용됩니다. </p> </td> 
  </tr> 
 </tbody> 
</table>

## [!UICONTROL JSON] >[!UICONTROL JSON 만들기] 모듈을 사용하여 매핑된 JSON 본문

[!UICONTROL JSON 만들기] 모듈을 사용하면 JSON을 더 쉽게 지정할 수 있습니다. 또한 값을 동적으로 정의할 수 있습니다.

JSON 모듈에 대한 자세한 내용은 [JSON 모듈](../../workfront-fusion/apps-and-their-modules/json-modules.md)을 참조하세요.

1. JSON을 생성할 값을 입력하거나 매핑합니다.

   ![](assets/json-values-350x288.png)

1. [!UICONTROL JSON] > [!UICONTROL JSON 만들기] 모듈을 HTTP > 요청 모듈에 연결합니다.
1. [!UICONTROL JSON 만들기] 모듈의 JSON 문자열을 [!UICONTROL HTTP] >[!UICONTROL 요청 만들기] 모듈의 [!UICONTROL 요청 콘텐츠] 필드에 매핑합니다.

   이제 시나리오를 실행하면 푸시 알림이 [!DNL Pushover] 계정에 등록된 장치로 전송됩니다.
