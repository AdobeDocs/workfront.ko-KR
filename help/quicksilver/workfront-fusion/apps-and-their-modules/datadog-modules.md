---
content-type: reference
product-previous: workfront-fusion
product-area: workfront-integrations;documents
keywords: 커넥터
navigation-topic: apps-and-their-modules
title: Datadog 모듈
description: 다음에서 [!DNL Adobe Workfront Fusion] 시나리오에서는 Datadog를 사용하는 워크플로를 자동화할 수 있을 뿐만 아니라 여러 타사 애플리케이션 및 서비스에 연결할 수도 있습니다.
author: Becky
feature: Workfront Fusion
exl-id: a0b4352d-a1ce-4459-a58e-71de860b8a90
source-git-commit: 0915dcce45b271ee18cdd8af5db4f0eb01f3cced
workflow-type: tm+mt
source-wordcount: '843'
ht-degree: 1%

---

# [!DNL Datadog] 모듈

다음에서 [!DNL Adobe Workfront Fusion] 시나리오에서는 다음을 사용하는 워크플로를 자동화할 수 있습니다 [!DNL Datadog]을 여러 타사 응용 프로그램 및 서비스에 연결할 수 있습니다.

시나리오를 만드는 방법에 대한 지침이 필요한 경우 [에서 시나리오 만들기 [!DNL Adobe Workfront Fusion]](../../workfront-fusion/scenarios/create-a-scenario.md).

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

## 전제 조건

사용 [!DNL Datadog] 모듈, 다음이 있어야 합니다. [!DNL Datadog] 계정입니다.

## 연결 [!DNL Datadog] 끝 [!DNL Workfront Fusion] {#connect-datadog-to-workfront-fusion}

### API 키 및 애플리케이션 키 검색 {#retrieve-your-api-key-and-application-key}

을(를) 연결하려면 [!DNL Datadog] 계정 위치: [!DNL Workfront Fusion] 에서 API 키 및 애플리케이션 키를 검색해야 합니다. [!DNL Datadog] 계정입니다.

1. 에 로그인 [!DNL Datadog] 계정입니다.
1. 왼쪽 탐색 패널에서 을 클릭합니다. **[!UICONTROL 통합]**&#x200B;을 클릭한 다음 을 클릭합니다 **[!UICONTROL API]**.
1. 기본 화면에서 다음을 클릭합니다. **[!UICONTROL API 키]**.
1. 보라색 막대 위로 마우스를 가져가 API 키를 표시합니다.
1. API 키를 보안 위치에 복사합니다.
1. 기본 화면에서 다음을 클릭합니다. **[!UICONTROL 애플리케이션 키]**.
1. 보라색 막대 위로 마우스를 가져가면 애플리케이션 키가 표시됩니다.
1. 응용 프로그램 키를 보안 위치에 복사합니다.

### 에 대한 연결 만들기 [!DNL Datadog] 위치: [!DNL Workfront Fusion]

에 대한 연결을 만들 수 있습니다. [!DNL Datadog] 내에서 직접 계정 [!UICONTROL Datadog] 모듈.

1. 다음 중 하나 [!UICONTROL Datadog] 모듈, 클릭 **[!UICONTROL 추가]** 다음 옆에 [!UICONTROL 연결] 필드.
1. 다음과 같이 모듈의 필드를 채웁니다.

<table style="table-layout:auto">
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">[!UICONTROL 연결 유형]</td> 
      <td> <p> [!UICONTROL] 선택 [!DNL Datadog] 에 대한 전체 액세스 권한을 얻기 위한 Application] 옵션 [!DNL Datadog] API.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL 연결 이름]</td> 
      <td> <p> 연결의 이름을 입력합니다.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL Domain] </td> 
      <td> <p>연결할 도메인(미국 또는 유럽 연합)을 선택합니다.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL API 키]</td> 
      <td> <p> 다음을 입력하십시오. [!DNL Datadog] API 키. </p> <p>API 키 검색에 대한 지침은 <a href="#retrieve-your-api-key-and-application-key" class="MCXref xref">API 키 및 애플리케이션 키 검색</a> 이 문서에서.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL 응용 프로그램 키]</td> 
      <td> <p> 다음을 입력하십시오. [!DNL Datadog] 애플리케이션 키. </p> <p>응용 프로그램 키 검색에 대한 지침은 <a href="#retrieve-your-api-key-and-application-key" class="MCXref xref">API 키 및 애플리케이션 키 검색</a> 이 문서에서.</p> </td> 
     </tr> 
    </tbody> 
   </table>

1. 클릭 **[!UICONTROL 계속]** 를 클릭하여 연결을 만들고 모듈로 돌아갑니다.

## [!DNL Datadog] 모듈 및 해당 필드

를 구성할 때 [!DNL Datadog] 모듈, [!DNL Workfront Fusion] 아래 나열된 필드를 표시합니다. 이와 함께 추가 [!DNL Datadog] 앱이나 서비스의 액세스 수준 등에 따라 필드가 표시될 수 있습니다. 모듈의 굵은 제목은 필수 필드를 나타냅니다.

필드나 함수 위에 맵 단추가 표시되면 이 단추를 사용하여 해당 필드에 대한 변수와 함수를 설정할 수 있습니다. 자세한 내용은 [의 한 모듈에서 다른 모듈로 정보 매핑 [!DNL Adobe Workfront Fusion]](../../workfront-fusion/mapping/map-information-between-modules.md).

![](assets/map-toggle-350x74.png)

### 액션

* [[!UICONTROL 시계열 점수 게시]](#post-timeseries-points)
* [[!UICONTROL API 호출 만들기]](#make-an-api-call)

#### [!UICONTROL 시계열 점수 게시]

모듈을 사용하면 그래프로 표시할 수 있는 시계열 데이터를 게시할 수 있습니다 [!DNL Datadog]의 대시보드.

압축 페이로드의 제한은 압축 해제된 페이로드의 경우 3.2메가바이트(3200000) 및 62메가바이트(62914560)입니다.

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td> 
   <td> <p>연결에 대한 자세한 내용 [!DNL Datadog] 계정 위치: [!DNL Workfront Fusion], 참조 <a href="#connect-datadog-to-workfront-fusion" class="MCXref xref">연결 [!DNL Datadog] 끝 [!DNL Workfront Fusion]</a> 이 문서에서.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Series]</td> 
   <td> <p>제출하려는 시계열 추가 [!DNL Datadog].</p> 
    <ul> 
     <li> <p><strong>[!UICONTROL 지표]</strong> </p> <p>시계열의 이름을 입력합니다.</p> </li> 
     <li> <p><strong>[!UICONTROL 유형]</strong> </p> <p>지표 유형을 선택합니다.</p> </li> 
     <li> <p><strong>[!UICONTROL Interval]</strong> </p> <p> 지표 유형이 비율 또는 개수인 경우 해당 간격을 정의합니다.</p> </li> 
     <li> <p><strong>[!UICONTROL Points]</strong> </p> <p>지표와 관련된 포인트를 추가합니다.</p> <p>포인트의 JSON 배열입니다. 각 점의 형식은 다음과 같습니다. <code>[[POSIX_timestamp, numeric_value], ...] </code></p> <p>참고:  <p>타임스탬프는 초 단위여야 합니다.</p> <p>타임스탬프는 현재여야 합니다. 현재를 미래 10분 이하 또는 과거 1시간 이상으로 정의한다.</p> <p> 숫자 값 형식은 부동 소수로만 지정할 수 있습니다.</p> </p> <p>이 필드에는 최소 1개의 항목이 포함되어야 합니다.</p> </li> 
     <li> <p><strong>[!UICONTROL 호스트]</strong> </p> <p>지표를 생성한 호스트의 이름을 입력합니다.</p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL API 호출 만들기]

이 작업 모듈을 사용하면 사용자 지정 API 호출을 수행할 수 있습니다.

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td> 
   <td> <p>연결에 대한 자세한 내용 [!DNL Datadog] 계정 위치: [!DNL Workfront Fusion], 참조 <a href="#connect-datadog-to-workfront-fusion" class="MCXref xref">연결 [!DNL Datadog] 끝 [!DNL Workfront Fusion]</a> 이 문서에서.</p> </td> 
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
   <td> <p>표준 JSON 개체 형태로 요청의 헤더를 추가합니다.</p> <p>For example, <code>{"Content-type":"application/json"}</code></p> <p>Workfront Fusion은 사용자에게 권한 부여 헤더를 추가합니다.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL 쿼리 문자열]</td> 
   <td> <p>표준 JSON 개체 형식으로 API 호출에 대한 쿼리를 추가합니다.</p> <p>For example: <code>{"name":"something-urgent"}</code></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Body]</td> 
   <td> <p>표준 JSON 개체의 형태로 API 호출에 대한 본문 콘텐츠를 추가합니다.</p> <p>참고:  <p>다음과 같은 조건문을 사용할 때 <code>if</code> json에서 따옴표를 조건문 외부에 넣습니다.</p> 
     <div class="example" data-mc-autonum="<b>Example: </b>"> 
      <p> <img src="assets/quotes-in-json-350x120.png" style="width: 350;height: 120;"> </p> 
     </div> </p> </td> 
  </tr> 
 </tbody> 
</table>

**예:** 다음 API 호출은 [!DNL Datadog] 계정:

URL: `/v1/dashboard`

메서드: `GET`

![](assets/datadog-api-example.png)

결과는 번들 > 본문 > 대시보드 아래에 있는 모듈의 출력에서 찾을 수 있습니다.

이 예에서는 3개의 대시보드가 반환되었습니다.

![](assets/datadog-api-response-example.png)
