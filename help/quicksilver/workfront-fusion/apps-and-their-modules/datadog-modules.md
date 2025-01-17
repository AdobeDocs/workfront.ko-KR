---
content-type: reference
product-previous: workfront-fusion
product-area: workfront-integrations;documents
keywords: 커넥터
navigation-topic: apps-and-their-modules
title: Datadog 모듈
description: Adobe Workfront Fusion 설명서가 새 위치로 이동했습니다. 이 문서는 더 이상 사용되지 않지만, 이 기능을 다루는 새 문서에 대한 링크를 포함합니다.
author: Becky
feature: Workfront Fusion
exl-id: a0b4352d-a1ce-4459-a58e-71de860b8a90
source-git-commit: efbe888d370e20c895dc40f18f999f2d01ec6337
workflow-type: tm+mt
source-wordcount: '916'
ht-degree: 0%

---

# [!DNL Datadog]개 모듈

>[!IMPORTANT]
>
>Adobe Workfront Fusion 설명서가 새 위치로 이동했습니다.
>
>이 문서의 정보는 이제 문서에서 찾을 수 있습니다.
>
>* [Datadog 모듈](https://experienceleague.adobe.com/docs/workfront-fusion/using/references/apps-and-their-modules/third-party-app-connectors/datadog-modules.html)
>
>모든 책갈피를 업데이트하십시오.
>
>이 문서는 더 이상 업데이트되지 않으며 곧 제거될 예정입니다.

[!DNL Adobe Workfront Fusion] 시나리오에서는 [!DNL Datadog]을(를) 사용하는 워크플로를 자동화하고 여러 타사 응용 프로그램 및 서비스에 연결할 수 있습니다.

시나리오를 만드는 방법에 대한 지침이 필요하면 [시나리오 만들기 [!DNL Adobe Workfront Fusion]](../../workfront-fusion/scenarios/create-a-scenario.md)를 참조하십시오.

모듈에 대한 자세한 내용은 [의 모듈 [!DNL Adobe Workfront Fusion]](../../workfront-fusion/modules/modules.md)을 참조하세요.

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

## 전제 조건

[!DNL Datadog] 모듈을 사용하려면 [!DNL Datadog] 계정이 있어야 합니다.

## Datadog API 정보

Datadog 커넥터에서는 다음을 사용합니다.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">API 태그</td> 
   <td>1.0.11</td> 
  </tr>
 </tbody> 
 </table>

## [!DNL Datadog]을(를) [!DNL Workfront Fusion]에 연결 {#connect-datadog-to-workfront-fusion}

### API 키 및 애플리케이션 키 검색 {#retrieve-your-api-key-and-application-key}

[!DNL Datadog] 계정을 [!DNL Workfront Fusion]에 연결하려면 [!DNL Datadog] 계정에서 API 키와 응용 프로그램 키를 검색해야 합니다.

1. [!DNL Datadog] 계정에 로그인합니다.
1. 왼쪽 탐색 패널에서 **[!UICONTROL 통합]**&#x200B;을 클릭한 다음 **[!UICONTROL API]**&#x200B;를 클릭합니다.
1. 기본 화면에서 **[!UICONTROL API 키]**&#x200B;를 클릭합니다.
1. 보라색 막대 위로 마우스를 가져가 API 키를 표시합니다.
1. API 키를 보안 위치에 복사합니다.
1. 기본 화면에서 **[!UICONTROL 응용 프로그램 키]**&#x200B;를 클릭합니다.
1. 보라색 막대 위로 마우스를 가져가면 애플리케이션 키가 표시됩니다.
1. 응용 프로그램 키를 보안 위치에 복사합니다.

### [!DNL Workfront Fusion]의 [!DNL Datadog]에 연결 만들기

[!UICONTROL Datadog] 모듈 내에서 직접 [!DNL Datadog] 계정에 연결할 수 있습니다.

1. [!UICONTROL Datadog] 모듈에서 [!UICONTROL 연결] 필드 옆에 있는 **[!UICONTROL 추가]**&#x200B;를 클릭합니다.
1. 다음과 같이 모듈의 필드를 채웁니다.

<table style="table-layout:auto">
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">[!UICONTROL 연결 유형]</td> 
      <td> <p> [!DNL Datadog] API에 대한 전체 액세스 권한을 얻으려면 [!UICONTROL [!DNL Datadog] Application] 옵션을 선택하십시오.</p> </td> 
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
      <td> <p> [!DNL Datadog] API 키를 입력하십시오. </p> <p>API 키 검색에 대한 지침은 이 문서에서 <a href="#retrieve-your-api-key-and-application-key" class="MCXref xref">API 키 및 응용 프로그램 키 검색</a>을 참조하십시오.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL 응용 프로그램 키]</td> 
      <td> <p> [!DNL Datadog] 응용 프로그램 키를 입력하십시오. </p> <p>응용 프로그램 키 검색에 대한 지침은 이 문서에서 <a href="#retrieve-your-api-key-and-application-key" class="MCXref xref">API 키 및 응용 프로그램 키 검색</a>을 참조하십시오.</p> </td> 
     </tr> 
    </tbody> 
   </table>

1. 연결을 만들고 모듈로 돌아가려면 **[!UICONTROL 계속]**&#x200B;을 클릭하세요.

## [!DNL Datadog]개 모듈 및 해당 필드

[!DNL Datadog] 모듈을 구성할 때 [!DNL Workfront Fusion]에 아래 나열된 필드가 표시됩니다. 앱 또는 서비스의 액세스 수준과 같은 요소에 따라 이러한 필드와 함께 [!DNL Datadog] 필드가 추가로 표시될 수 있습니다. 모듈의 굵은 제목은 필수 필드를 나타냅니다.

필드나 함수 위에 맵 단추가 표시되면 이 단추를 사용하여 해당 필드에 대한 변수와 함수를 설정할 수 있습니다. 자세한 내용은 [한 모듈에서 다른 모듈로 정보를 매핑 [!DNL Adobe Workfront Fusion]](../../workfront-fusion/mapping/map-information-between-modules.md)을 참조하십시오.

![](assets/map-toggle-350x74.png)

### 액션

* [[!UICONTROL 시계열 점수 게시]](#post-timeseries-points)
* [[!UICONTROL API 호출 만들기]](#make-an-api-call)

#### [!UICONTROL 시계열 점수 게시]

모듈을 사용하면 [!DNL Datadog]의 대시보드에 그래프로 표시할 수 있는 시계열 데이터를 게시할 수 있습니다.

압축 페이로드의 제한은 압축 해제된 페이로드의 경우 3.2메가바이트(3200000) 및 62메가바이트(62914560)입니다.

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td> 
   <td> <p>[!DNL Datadog] 계정을 [!DNL Workfront Fusion]에 연결하는 방법에 대한 지침은 이 문서에서 <a href="#connect-datadog-to-workfront-fusion" class="MCXref xref">[!DNL Datadog]을(를) [!DNL Workfront Fusion]</a>에 연결 을 참조하십시오.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Series]</td> 
   <td> <p>[!DNL Datadog]에 제출할 시계열을 추가합니다.</p> 
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
   <td> <p>[!DNL Datadog] 계정을 [!DNL Workfront Fusion]에 연결하는 방법에 대한 지침은 이 문서에서 <a href="#connect-datadog-to-workfront-fusion" class="MCXref xref">[!DNL Datadog]을(를) [!DNL Workfront Fusion]</a>에 연결 을 참조하십시오.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL URL]</td> 
   <td><code>https://api.datadoghq.com/api/</code>과(와) 관련된 경로를 입력하십시오. 예: <code> /v1/org</code>.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL 메서드]</td> 
   <td> <p>API 호출을 구성하는 데 필요한 HTTP 요청 메서드를 선택합니다. 자세한 내용은 [!DNL Adobe Workfront Fusion]</a>에서 <a href="../../workfront-fusion/modules/http-request-methods.md" class="MCXref xref">HTTP 요청 메서드를 참조하십시오.</p> </td> 
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
   <td> <p>표준 JSON 개체의 형태로 API 호출에 대한 본문 콘텐츠를 추가합니다.</p> <p>참고:  <p>JSON에서 <code>if</code>과(와) 같은 조건문을 사용할 때 따옴표를 조건문 외부에 넣으십시오.</p> 
     <div class="example" data-mc-autonum="<b>Example: </b>"> 
      <p> <img src="assets/quotes-in-json-350x120.png" style="width: 350;height: 120;"> </p> 
     </div> </p> </td> 
  </tr> 
 </tbody> 
</table>

**예:** 다음 API 호출은 [!DNL Datadog] 계정의 모든 대시보드를 반환합니다.

URL: `/v1/dashboard`

메서드: `GET`

![](assets/datadog-api-example.png)

결과는 번들 > 본문 > 대시보드 아래에 있는 모듈의 출력에서 찾을 수 있습니다.

이 예에서는 3개의 대시보드가 반환되었습니다.

![](assets/datadog-api-response-example.png)
