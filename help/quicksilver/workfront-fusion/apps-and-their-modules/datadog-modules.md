---
content-type: reference
product-previous: workfront-fusion
product-area: workfront-integrations;documents
keywords: 커넥터
navigation-topic: apps-and-their-modules
title: 데이터 수집 모듈
description: 에서 [!DNL Adobe Workfront Fusion] 시나리오, Datadog를 사용하는 워크플로우를 자동화하고 여러 타사 애플리케이션 및 서비스에 연결할 수 있습니다.
author: Becky
feature: Workfront Fusion
exl-id: a0b4352d-a1ce-4459-a58e-71de860b8a90
source-git-commit: 885d93dd4383945538e977fd3edbfd55bda88b70
workflow-type: tm+mt
source-wordcount: '795'
ht-degree: 1%

---

# [!DNL Datadog] 모듈

에서 [!DNL Adobe Workfront Fusion] 시나리오, [!DNL Datadog]여러 타사 애플리케이션 및 서비스에 연결할 수 있습니다.

시나리오 만들기에 대한 지침이 필요한 경우 [에서 시나리오 만들기 [!DNL Adobe Workfront Fusion]](../../workfront-fusion/scenarios/create-a-scenario.md).

모듈에 대한 자세한 내용은 [의 모듈 [!DNL Adobe Workfront Fusion]](../../workfront-fusion/modules/modules.md).

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

## 전제 조건

를 사용하려면 [!DNL Datadog] 모듈이면 반드시 [!DNL Datadog] 계정이 필요합니다.

## Connect [!DNL Datadog] to [!DNL Workfront Fusion] {#connect-datadog-to-workfront-fusion}

### API 키 및 애플리케이션 키 검색 {#retrieve-your-api-key-and-application-key}

연결 [!DNL Datadog] 계정 대상 [!DNL Workfront Fusion] API 키 및 애플리케이션 키를 사용자 정의에서 검색해야 합니다 [!DNL Datadog] 계정이 필요합니다.

1. 에 로그인합니다. [!DNL Datadog] 계정이 필요합니다.
1. 왼쪽 탐색 패널에서 **[!UICONTROL 통합]**&#x200B;를 클릭한 다음 **[!UICONTROL API]**.
1. 기본 화면에서 **[!UICONTROL API 키]**.
1. 자주색 막대를 마우스로 가리키면 API 키가 표시됩니다.
1. 보안 위치에 API 키를 복사합니다.
1. 기본 화면에서 **[!UICONTROL 응용 프로그램 키]**.
1. 자주색 막대를 마우스로 가리키면 응용 프로그램 키가 표시됩니다.
1. 응용 프로그램 키를 보안 위치에 복사합니다.

### 연결 만들기 [!DNL Datadog] in [!DNL Workfront Fusion]

에 대한 연결을 만들 수 있습니다 [!DNL Datadog] 내에서 직접 계정 [!UICONTROL Datadog] 모듈.

1. 어떤 경우에서도 [!UICONTROL Datadog] 모듈 **[!UICONTROL 추가]** 다음 [!UICONTROL 연결] 필드.
1. 다음과 같이 모듈의 필드를 채웁니다.

<table style="table-layout:auto">
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">[!UICONTROL 연결 유형]</td> 
      <td> <p> [!UICONTROL 을 선택합니다 [!DNL Datadog] 응용 프로그램] 옵션을 사용하여 [!DNL Datadog] API.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL 연결 이름]</td> 
      <td> <p> 연결의 이름을 입력합니다.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL Domain] </td> 
      <td> <p>연결할 도메인(미국 또는 EU)을 선택합니다.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL API 키]</td> 
      <td> <p> 을(를) 입력합니다. [!DNL Datadog] API 키. </p> <p>API 키 검색에 대한 지침은 <a href="#retrieve-your-api-key-and-application-key" class="MCXref xref">API 키 및 애플리케이션 키 검색</a> 참조하십시오.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL 응용 프로그램 키]</td> 
      <td> <p> 을(를) 입력합니다. [!DNL Datadog] 응용 프로그램 키 </p> <p>응용 프로그램 키 검색에 대한 지침은 <a href="#retrieve-your-api-key-and-application-key" class="MCXref xref">API 키 및 애플리케이션 키 검색</a> 참조하십시오.</p> </td> 
     </tr> 
    </tbody> 
   </table>

1. 클릭 **[!UICONTROL 계속]** 연결을 만들고 모듈로 돌아갑니다.

## [!DNL Datadog] 모듈 및 해당 필드

구성 시 [!DNL Datadog] 모듈, [!DNL Workfront Fusion] 아래 나열된 필드를 표시합니다. 이와 함께 추가 [!DNL Datadog] 앱이나 서비스에서 액세스 수준과 같은 요소에 따라 필드가 표시될 수 있습니다. 모듈에서 굵게 표시된 제목은 필수 필드를 나타냅니다.

필드 또는 함수 위에 맵 단추가 표시되면 이 단추를 사용하여 해당 필드에 대한 변수와 함수를 설정할 수 있습니다. 자세한 내용은 [의 한 모듈에서 다른 모듈로 정보 매핑 [!DNL Adobe Workfront Fusion]](../../workfront-fusion/mapping/map-information-between-modules.md).

![](assets/map-toggle-350x74.png)

### 액션

* [[!UICONTROL 포스트타임 시리즈 포인트]](#post-timeseries-points)
* [[!UICONTROL API 호출 만들기]](#make-an-api-call)

#### [!UICONTROL 포스트타임 시리즈 포인트]

모듈을 사용하면 그래프로 작성할 수 있는 시계열 데이터를 게시할 수 있습니다 [!DNL Datadog]의 대시보드.

압축된 페이로드의 제한은 3.2MB(3200000) 및 압축된 페이로드의 62MB(62914560)입니다.

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td> 
   <td> <p>연결 방법에 대한 지침은 [!DNL Datadog] 계정 대상 [!DNL Workfront Fusion]를 참조하십시오. <a href="#connect-datadog-to-workfront-fusion" class="MCXref xref">Connect [!DNL Datadog] to [!DNL Workfront Fusion]</a> 참조하십시오.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Series]</td> 
   <td> <p>제출할 시계열 추가 [!DNL Datadog].</p> 
    <ul> 
     <li> <p><strong>[!UICONTROL 지표]</strong> </p> <p>타임라인의 이름을 입력합니다.</p> </li> 
     <li> <p><strong>[!UICONTROL Type]</strong> </p> <p>지표 유형을 선택합니다.</p> </li> 
     <li> <p><strong>[!UICONTROL Interval]</strong> </p> <p> 지표 유형이 비율 또는 카운트인 경우 해당 간격을 정의합니다.</p> </li> 
     <li> <p><strong>[!UICONTROL Points]</strong> </p> <p>지표와 관련된 포인트를 추가합니다.</p> <p>포인트 JSON 배열입니다. 각 포인트에는 다음과 같은 형식이 있습니다. <code>[[POSIX_timestamp, numeric_value], ...] </code></p> <p>참고:  <p>타임스탬프는 초 단위여야 합니다.</p> <p>타임스탬프가 최신 상태여야 합니다. 현재 값은 향후 10분 이하 또는 과거 1시간 이상으로 정의됩니다.</p> <p> 숫자 값 형식은 부동 소수점 값이어야 합니다.</p> </p> <p>이 필드에는 1개 이상의 항목이 포함되어야 합니다.</p> </li> 
     <li> <p><strong>[!UICONTROL Host]</strong> </p> <p>지표를 생성한 호스트의 이름을 입력합니다.</p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL API 호출 만들기]

이 작업 모듈을 사용하여 사용자 지정 API 호출을 수행할 수 있습니다.

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td> 
   <td> <p>연결 방법에 대한 지침은 [!DNL Datadog] 계정 대상 [!DNL Workfront Fusion]를 참조하십시오. <a href="#connect-datadog-to-workfront-fusion" class="MCXref xref">Connect [!DNL Datadog] to [!DNL Workfront Fusion]</a> 참조하십시오.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL URL]</td> 
   <td>상대 경로 입력 <code>https://api.datadoghq.com/api/</code>. 예:<code> /v1/org</code>.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL 메서드]</td> 
   <td> <p>API 호출을 구성하는 데 필요한 HTTP 요청 메서드를 선택합니다. 자세한 내용은 <a href="../../workfront-fusion/modules/http-request-methods.md" class="MCXref xref">의 HTTP 요청 메서드 [!DNL Adobe Workfront Fusion]</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Headers]</td> 
   <td> <p>요청의 헤더를 표준 JSON 개체 형태로 추가합니다.</p> <p>For example, <code>{"Content-type":"application/json"}</code></p> <p>Workfront Fusion이 사용자를 위해 인증 헤더를 추가합니다.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL 쿼리 문자열]</td> 
   <td> <p>표준 JSON 개체 형태로 API 호출에 대한 쿼리를 추가합니다.</p> <p>For example: <code>{"name":"something-urgent"}</code></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Body]</td> 
   <td> <p>표준 JSON 개체 형태로 API 호출에 대한 본문 콘텐츠를 추가합니다.</p> <p>참고:  <p>다음과 같은 조건문을 사용하는 경우 <code>if</code> json에서 따옴표를 조건문 외부에 지정합니다.</p> 
     <div class="example" data-mc-autonum="<b>Example: </b>"> 
      <p> <img src="assets/quotes-in-json-350x120.png" style="width: 350;height: 120;"> </p> 
     </div> </p> </td> 
  </tr> 
 </tbody> 
</table>

**예:** 다음 API 호출은 의 모든 대시보드를 반환합니다 [!DNL Datadog] 계정:

URL: `/v1/dashboard`

메서드: `GET`

![](assets/datadog-api-example.png)

결과는 모듈의 Output에서 Bundle > Body > Dashboard에 있습니다.

이 예제에서는 3개의 대시보드가 반환되었습니다.

![](assets/datadog-api-response-example.png)
