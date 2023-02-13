---
content-type: reference
product-previous: workfront-fusion
product-area: workfront-integrations
keywords: 커넥터
navigation-topic: apps-and-their-modules
title: HTTP &gt; 기타 모듈
description: 다음 [!DNL Adobe Workfront Fusion] HTTP 앱은 HTTP(Hypertext Transfer Protocol) 프로토콜을 기반으로 통신을 위한 다양한 모듈을 제공합니다. HTTP는 World Wide Web을 위한 데이터 통신의 기반입니다. 모듈을 사용하여 웹 페이지 및 파일을 다운로드하고, 웹 후크 및 API 엔드포인트 등을 호출할 수 있습니다.
author: Becky
feature: Workfront Fusion
exl-id: ff2cd098-d1d7-43a3-9f00-15e0f6e92332
source-git-commit: 885d93dd4383945538e977fd3edbfd55bda88b70
workflow-type: tm+mt
source-wordcount: '427'
ht-degree: 0%

---

# HTTP > 기타 모듈

>[!NOTE]
>
>[!UICONTROL Adobe Workfront Fusion] 를 사용하려면 [!UICONTROL Adobe Workfront Fusion] 라이센스 [!UICONTROL Adobe Workfront] 라이센스.

다음 [!DNL Adobe Workfront Fusion] [!UICONTROL HTTP] 앱은 HTTP(Hypertext Transfer Protocol) 프로토콜을 기반으로 통신을 위한 다양한 모듈을 제공합니다. HTTP는 World Wide Web을 위한 데이터 통신의 기반입니다. 모듈을 사용하여 웹 페이지 및 파일을 다운로드하고, 웹 후크 및 API 엔드포인트 등을 호출할 수 있습니다.

모듈의 올바른 선택은 액세스하려는 리소스가 사용하는 인증/인증 메커니즘에 따라 다릅니다. 다음은 모듈의 예입니다

* 주로 특정 유형의 인증/인증을 사용하지 않는 리소스를 위한 범용 모듈로 요청:
* 기본 인증 요청 만들기:을 사용하는 리소스 [!DNL HTTP] 기본 인증(BA)
* OAuth 2.0 요청 수행: OAuth 2.0 인증 프로토콜을 사용하는 리소스
* 클라이언트 인증서 인증 요청 만들기: 클라이언트측 인증서가 필요한 인증 프로토콜을 사용하는 리소스입니다.
* API 키 인증 요청 만들기: 를 사용하도록 선택할 수 있습니다.

## 모듈 요청

특정 요청 모듈 지침에 대해서는 다음 문서를 참조하십시오.

* [[!UICONTROL HTTP] >[!UICONTROL 요청 수행] 모듈](../../../workfront-fusion/apps-and-their-modules/http-modules/http-module-make-a-request.md)
* [[!UICONTROL HTTP] >[!UICONTROL 기본 인증 요청 만들기] 모듈](../../../workfront-fusion/apps-and-their-modules/http-modules/http-module-make-a-basic-auth-request.md)
* [[!UICONTROL HTTP] > [!UICONTROL OAuth 2.0 요청 만들기] 모듈](../../../workfront-fusion/apps-and-their-modules/http-modules/http-module-make-an-oauth-2-request.md)
* [[!UICONTROL HTTP] >[!UICONTROL 클라이언트 인증서 인증 요청 만들기] 모듈](../../../workfront-fusion/apps-and-their-modules/http-modules/http-module-make-a-client-cert-auth-request.md)
* [[!UICONTROL HTTP] >[!UICONTROL API 키 인증 요청 만들기]](../../../workfront-fusion/apps-and-their-modules/http-modules/http-module-make-an-api-key-auth-request.md)

## 기타 작업 모듈

* [[!UICONTROL 파일 가져오기]](#get-a-file)
* [[!UICONTROL 대상 URL 확인]](#resolve-a-target-url)

### [!UICONTROL 파일 가져오기]

이 작업 모듈은 지정된 URL에서 파일을 다운로드합니다. 파일이 다운로드되면 시나리오의 다른 모듈을 사용하여 파일(파일 데이터 매핑)을 추가로 처리할 수 있습니다.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL URL] </td> 
   <td> <p>다운로드할 파일의 URL을 입력하거나 매핑합니다. </p> </td> 
  </tr> 
 </tbody> 
</table>

### [!UICONTROL 대상 URL 확인]

이 작업 모듈은 HTTP 리디렉션 체인을 확인하고 대상 URL을 반환합니다.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL URL] </td> 
   <td> <p>확인할 URL(예: )을 입력하거나 매핑합니다. [!DNL bit.ly] URL.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL 메서드] </td> 
   <td> <p>[!UICONTROL HEAD] 메서드를 사용할지, [!UICONTROL GET] 메서드를 사용할지 여부를 선택합니다.</p> </td> 
  </tr> 
 </tbody> 
</table>

## 반복기 모듈

### [!UICONTROL 헤더 검색]

이 모듈은 지정된 HTTP 모듈에서 개별 번들로 각 헤더(이름 및 값)를 반환합니다.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL 소스 모듈]</td> 
   <td> <p> 헤더를 검색할 모듈을 선택합니다.</p> </td> 
  </tr> 
 </tbody> 
</table>

## JSON 웹 토큰 생성(JWT)

내장된 함수의 도움을 받아 JWT 토큰을 생성할 수 있습니다.

머리글:

![](assets/jwt-header-350x19.png)

복사 및 붙여넣기 코드:

```
{{replace(replace(replace(base64("{""alg"":""HS256"",""typ"":""JWT""}"); "/=/g"; emptystring); "/\+/g"; "-"); "/\//g"; "_")}}
```

페이로드:

![](assets/jwt-payload-350x17.png)

복사 및 붙여넣기 코드:

```
{{replace(replace(replace(base64("{""iss"":""key"",""exp"":" + (timestamp + 60) + "}"); "/=/g"; emptystring); "/\+/g"; "-"); "/\//g"; "_")}}
```

토큰:

![](assets/jwt-token-350x15.png)

복사 및 붙여넣기 코드:

```
{{1.value}}.{{2.value}}.{{replace(replace(replace(sha256(1.value + "." + 2.value; "base64"; "secret"); "/=/g"; emptystring); "/\+/g"; "-"); "/\//g"; "_")}}
```
