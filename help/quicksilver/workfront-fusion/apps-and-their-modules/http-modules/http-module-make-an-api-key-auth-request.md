---
content-type: reference
product-previous: workfront-fusion
product-area: workfront-integrations
keywords: 커넥터
navigation-topic: http-modules
title: HTTP &gt; API 키 인증 요청 만들기
description: 이 [!DNL Adobe Workfront Fusion] 작업 모듈은 API 키 인증 권한이 필요한 지정된 URL에 HTTPS 요청을 보내고 응답을 처리합니다.
author: Becky
feature: Workfront Fusion
exl-id: 70bf87c7-6d51-4ef4-9dce-80ad004e613f
source-git-commit: 45540ccc3b9fca98f8aaae86ac4d6574a067a6e4
workflow-type: tm+mt
source-wordcount: '1013'
ht-degree: 0%

---

# HTTP >[!UICONTROL API 키 권한 부여 요청 만들기]

>[!NOTE]
>
>[!DNL Adobe Workfront Fusion]에는 Adobe Workfront 라이선스 외에 [!DNL Adobe Workfront Fusion] 라이선스가 필요합니다.

이 [!DNL Adobe Workfront Fusion] 작업 모듈은 API 키 인증 권한이 필요한 지정된 URL에 HTTPS 요청을 보내고 응답을 처리합니다.

>[!NOTE]
>
>현재 전용 커넥터가 없는 Adobe 제품에 연결하는 경우 Adobe Authenticator 모듈을 사용하는 것이 좋습니다.
>
>자세한 내용은 [Adobe Authenticator 모듈](/help/quicksilver/workfront-fusion/apps-and-their-modules/adobe-authenticator-modules.md)을 참조하세요.

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

[!UICONTROL Adobe Workfront Fusion] 라이선스에 대한 자세한 내용은 [Adobe Workfront Fusion 라이선스](../../../workfront-fusion/get-started/license-automation-vs-integration.md)를 참조하십시오.

## [!UICONTROL HTTP] >[!UICONTROL API 키 권한 부여 요청 만들기] 모듈 구성

[!UICONTROL HTTP] >[!UICONTROL API 키 권한 부여 요청 만들기] 모듈을 구성할 때 [!DNL Adobe Workfront Fusion]에 아래 나열된 필드가 표시됩니다. 모듈의 굵은 제목은 필수 필드를 나타냅니다.

필드나 함수 위에 맵 단추가 표시되면 이 단추를 사용하여 해당 필드에 대한 변수와 함수를 설정할 수 있습니다. 자세한 내용은 [한 모듈에서 다른 모듈로 정보를 매핑 [!DNL Adobe Workfront Fusion]](../../../workfront-fusion/mapping/map-information-between-modules.md)을 참조하십시오.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL 자격 증명]</td> 
   <td> <p>API 키 인증 자격 증명이 포함된 키를 선택합니다. 새 키를 추가하려면 <strong>[!UICONTROL 추가]</strong>를 클릭하고 다음 정보를 구성하십시오.</p> 
    <ul> 
     <li> <p><strong>[!UICONTROL 키 이름]</strong></p> <p>이 API 자격 증명 세트의 이름을 입력합니다.</p> </li> 
     <li> <p><strong>[!UICONTROL 키]</strong> </p> <p>API 키를 입력합니다.</p> </li> 
     <li> <p><strong>[!UICONTROL API 키 배치]</strong> </p> <p>API 키를 헤더에 배치할지 또는 API 호출의 쿼리에 배치할지 선택합니다.</p> </li> 
     <li> <p><strong>[!UICONTROL API 키 매개 변수 이름]</strong> </p> <p>API 호출이 API 키를 식별하는 이름을 입력합니다(예: "apiKey" 또는 "X-API-Key"). 이 정보는 모듈이 연결 중인 웹 서비스의 설명서에서 찾을 수 있습니다.</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL 모든 상태를 오류로 평가(2xx 및 3xx 제외)] </td> 
   <td> <p>이 옵션을 사용하여 오류 처리를 설정합니다.</p> <p>자세한 내용은 <a href="../../../workfront-fusion/errors/error-handling.md" class="MCXref xref">Adobe Workfront Fusion에서 오류 처리</a>를 참조하십시오.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL URL] </td> 
   <td> <p>API 끝점, 웹 사이트 등과 같이 요청을 보낼 URL을 입력합니다.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL 메서드]</p> </td> 
   <td> <p>API 호출을 구성하는 데 필요한 HTTP 요청 메서드를 선택합니다. 자세한 내용은 [!DNL Adobe Workfront Fusion]</a>에서 <a href="../../../workfront-fusion/modules/http-request-methods.md" class="MCXref xref">HTTP 요청 메서드를 참조하십시오.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Headers] </td> 
   <td> <p>표준 JSON 개체 형태로 요청의 헤더를 추가합니다. For example, <code>{"Content-type":"application/json"}</code></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL 쿼리 문자열]</td> 
   <td> <p> 원하는 쿼리 키-값 쌍을 입력합니다.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Body type]</p> </td> 
   <td> <p>HTTP Body는 사용할 데이터 바이트가 있는 경우 헤더 바로 다음에 오는 HTTP 트랜잭션 메시지로 전송됩니다.</p> 
    <ul> 
     <li> <p><strong>[!UICONTROL Raw]</strong> </p> <p>원시 본문 유형은 일반적으로 개발자 설명서에서 전송할 데이터를 지정하지 않는 경우에도 대부분의 HTTP 본문 요청에 적합합니다.</p> <p>[!UICONTROL Content type] 필드에서 데이터를 구문 분석하는 형식을 지정합니다.</p> <p>선택한 콘텐츠 유형에도 불구하고 모듈은 개발자 설명서에서 규정하거나 요구하는 모든 형식으로 데이터를 입력합니다.</p> </li> 
     <li> <p><strong>[!UICONTROL Application/x-www-form-urlencoded]</strong> </p> <p>이 본문 유형은 <code>application/x-www-form-urlencoded</code>을(를) 사용하여 [!UICONTROL POST] 데이터에 대한 것입니다.</p> <p><code>[!UICONTROL application/x-www-form-urlencoded]</code>의 경우 서버로 전송된 HTTP 메시지의 본문은 기본적으로 하나의 쿼리 문자열입니다. 키와 값은 키와 값 사이에 <code>=</code>이(가) 있고 <code>&amp;</code>(으)로 구분된 키-값 쌍으로 인코딩됩니다. </p> <p>이진 데이터의 경우 대신 <code>[!UICONTROL multipart/form-data]</code>을(를) 사용합니다.</p> 
      <div class="example" data-mc-autonum="<b>Example: </b>">
       <span class="autonumber"><span><b>예: </b></span></span> 
       <p>결과 HTTP 요청 형식의 예:</p> 
       <p><code>field1=value1&amp;field2=value2</code> </p> 
      </div> </li> 
     <li> <p><strong>[!UICONTROL Multipart/form-data]</strong> </p> <p>[!UICONTROL Multipart/form-data]는 파일 및 데이터를 전송하는 데 사용되는 HTTP multipart 요청입니다. 일반적으로 서버에 파일을 업로드하는 데 사용됩니다.</p> <p>요청에 전송할 필드를 추가합니다. 각 필드에는 키-값 쌍이 포함되어야 합니다.</p> 
      <ul> 
       <li> <p><strong>[!UICONTROL Text]</strong> </p> <p>요청 본문 내에 보낼 키와 값을 입력합니다.</p> </li> 
       <li> <p><strong>[!UICONTROL 파일]</strong> </p> <p>키를 입력하고 요청 본문에 보낼 소스 파일을 지정합니다.</p> <p>이전 모듈(예: [!UICONTROL HTTP] &gt;[!UICONTROL 파일 가져오기] 또는 [!UICONTROL Google 드라이브] &gt;[!UICONTROL 파일 다운로드)]에서 업로드할 파일을 매핑하거나 파일 이름 및 파일 데이터를 수동으로 입력합니다.</p> </li> 
      </ul> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL 구문 분석 응답]</p> </td> 
   <td> <p>[!UICONTROL JSON] &gt; [!UICONTROL Parse JSON] 또는 [!UICONTROL XML] &gt; [!UICONTROL Parse XML] 모듈을 사용할 필요가 없도록 응답을 자동으로 구문 분석하고 JSON 및 XML 응답을 변환하려면 이 옵션을 활성화합니다.</p> <p>구문 분석된 JSON 또는 XML 컨텐츠를 사용하기 전에 모듈에서 응답 컨텐츠를 인식하고 이를 후속 모듈에 매핑할 수 있도록 모듈을 한 번 수동으로 실행하십시오.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL 시간 초과] </td> 
   <td> <p>요청 시간 제한(초)을 지정합니다(1-300). 기본값은 40초입니다.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL 다른 HTTP 모듈과 쿠키 공유]</td> 
   <td> <p> 이 옵션을 활성화하면 시나리오의 모든 HTTP 모듈과 서버의 쿠키를 공유할 수 있습니다.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL 자체 서명된 인증서]</td> 
   <td> <p> 자체 서명된 인증서를 사용하여 TLS를 사용하려면 인증서를 업로드하십시오.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL 확인되지 않은(자체 서명된) 인증서를 사용하는 연결을 거부합니다.] </td> 
   <td> <p>확인되지 않은 TLS 인증서를 사용하는 연결을 거부하려면 이 옵션을 활성화합니다.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL 리디렉션 따르기]</td> 
   <td> <p> 3xx 응답이 있는 URL 리디렉션을 따르려면 이 옵션을 활성화하십시오.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL 모든 리디렉션 팔로우] </td> 
   <td> <p>모든 응답 코드와 함께 URL 리디렉션을 따르려면 이 옵션을 활성화합니다.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL 배열로 동일한 쿼리 문자열 키를 여러 개 직렬화할 수 없음]</p> </td> 
   <td> <p>기본적으로 [!DNL Workfront Fusion]은(는) 배열과 동일한 URL 쿼리 문자열 매개 변수 키에 대해 여러 값을 처리합니다. 예를 들어 <code>www.test.com?foo=bar&amp;foo=baz</code>은(는) <code>www.test.com?foo[0]=bar&amp;foo[1]=baz</code>(으)로 변환됩니다. 이 기능을 비활성화하려면 이 옵션을 활성화합니다. </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Request compressed content]</td> 
   <td> <p> 웹 사이트의 압축된 버전을 요청하려면 이 옵션을 활성화하십시오.</p> <p>압축된 콘텐츠를 요청하기 위해 <code>[!UICONTROL Accept-Encoding]</code> 헤더를 추가합니다.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Use Mutual TLS]</td> 
   <td> <p>HTTP 요청에서 상호 TLS를 사용하려면 이 옵션을 활성화하십시오.</p> <p>상호 TLS에 대한 자세한 내용은 <a href="../../../workfront-fusion/apps-and-their-modules/http-modules/use-mtls-in-http-modules.md" class="MCXref xref">HTTP 모듈에서 상호 TLS 사용([!DNL Adobe Workfront Fusion]</a>)을 참조하십시오.</p> </td> 
  </tr> 
 </tbody> 
</table>
