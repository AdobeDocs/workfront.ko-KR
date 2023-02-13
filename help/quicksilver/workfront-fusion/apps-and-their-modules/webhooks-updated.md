---
content-type: reference
product-previous: workfront-fusion
product-area: workfront-integrations
navigation-topic: apps-and-their-modules
title: Webhooks
description: 웹 후크는 이벤트에 의해 트리거되는 HTTP 호출입니다. 웹 후크를 사용하여 인스턴트 트리거 모듈을 활성화할 수 있습니다. 인터넷에 연결되어 있고 HTTP 요청이 허용되는 모든 애플리케이션은 웹 후크를 Adobe Workfront Fusion으로 보낼 수 있습니다.
author: Becky
feature: Workfront Fusion
exl-id: 987544a4-5840-40d4-9438-41a000aa22ee
source-git-commit: 885d93dd4383945538e977fd3edbfd55bda88b70
workflow-type: tm+mt
source-wordcount: '1391'
ht-degree: 0%

---

# Webhooks

웹 후크는 이벤트에 의해 트리거되는 HTTP 호출입니다. 웹 후크를 사용하여 인스턴트 트리거 모듈을 활성화할 수 있습니다. 인터넷에 연결되어 있고 HTTP 요청이 허용되는 모든 애플리케이션은 웹 후크를 Adobe Workfront Fusion으로 보낼 수 있습니다.

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

&#42;어떤 계획, 라이선스 유형 또는 액세스 권한을 보유하고 있는지 알아보려면 Workfront 관리자에게 문의하십시오.

&#42;&#42;에 대한 자세한 정보 [!DNL Adobe Workfront Fusion] 라이센스 [[!DNL Adobe Workfront Fusion] 라이선스](../../workfront-fusion/get-started/license-automation-vs-integration.md)

## 에서 웹 후크 사용 [!DNL Workfront Fusion]

>[!NOTE]
>
>타사 웹 후크(나가는 웹 후크)를 호출하려면 HTTP 모듈 중 하나를 사용합니다. 자세한 내용은 [HTTP 모듈](../../workfront-fusion/apps-and-their-modules/http-modules/http-modules-1.md).

웹후크를 사용하여 앱을 [!DNL Workfront Fusion]:

1. 추가 **[!UICONTROL Webhooks]** >**[!UICONTROL 사용자 지정 웹 후크]** 시나리오에 즉시 트리거 모듈을 추가합니다.

1. 클릭 **[!UICONTROL 추가]** webhook 필드 옆에 새 웹 후크의 이름을 입력합니다.
1. (선택 사항) **[!UICONTROL 고급 설정]**.
1. 에서 **[!UICONTROL IP 제한 사항]** 필드에 모듈에서 데이터를 허용할 수 있는 IP 주소의 쉼표로 구분된 목록을 입력합니다.
1. **[!UICONTROL 저장]**&#x200B;을 클릭합니다

웹 후크를 만들면 고유 URL이 표시됩니다. 웹 후크가 데이터를 보내는 주소입니다. Workfront Fusion은 이 주소로 전송된 데이터의 유효성을 검사한 다음 시나리오에서 처리하기 위해 켜집니다.

>[!NOTE]
>
>웹 후크를 만들면 한 번에 두 개 이상의 시나리오에서 사용할 수 있습니다.

### 웹 후크의 데이터 구조 구성 {#configure-the-webhook-s-data-structure}

들어오는 페이로드의 데이터 구조를 인식하려면 [!DNL Workfront Fusion] 는 표시된 주소로 보내는 샘플 데이터를 구문 분석합니다. 해당 서비스 또는 앱을 웹 후크에 호출하는 서비스 또는 앱을 변경하여 샘플 데이터를 제공할 수 있습니다. 예를 들어 파일을 제거할 수 있습니다.

또는 아래 절차에 따라 를 통해 샘플 데이터를 전송할 수 있습니다. [!UICONTROL HTTP] > [!UICONTROL 요청 수행] 모듈.

1. 을(를) 사용하여 새 시나리오 만들기 **[!UICONTROL HTTP]** > **[!UICONTROL 요청 수행]** 모듈

1. 다음 값으로 모듈을 구성합니다.

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader"><p>[!UICONTROL URL] </p></td> 
      <td>웹 후크의 URL을 입력합니다. 이 URL은 웹 후크를 설정하는 데 사용한 [!UICONTROL Webhooks] 모듈에서 찾을 수 있습니다.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL 메서드] </td> 
      <td><p>[!UICONTROL POST]</p></td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL Body type]</td> 
      <td><p> [!UICONTROL Raw]</p></td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL 컨텐츠 유형]</td> 
      <td><p> JSON(application/json)</p></td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL 요청 콘텐츠]</td> 
      <td><p>웹 후크에 원시 JSON이 필요합니다.</p></td> 
     </tr> 
    </tbody> 
   </table>

   ![](assets/new-scenario-set-up-like-this-350x446.png)

1. 다음 아이콘을 사용하여 시나리오를 엽니다. [!UICONTROL Webhooks] 모듈 을 포함합니다.
1. 웹 후크 모듈에서 **[!UICONTROL 데이터 구조 다시 결정]**.

   Webhooks 모듈에서 다른 모듈의 연결을 끊을 필요가 없습니다.

1. 을 사용하여 시나리오로 전환합니다. [!UICONTROL HTTP] 모듈 및 실행
1. Webhooks 모듈을 사용하여 시나리오에 다시 전환합니다.

   A &quot;[!UICONTROL 확인됨]&quot; 메시지는 모듈이 데이터 구조를 성공적으로 결정했음을 의미합니다.

   ![](assets/successfully-determined-350x175.png)

1. 클릭 **[!UICONTROL 확인]** 를 눌러 데이터 구조를 저장합니다.

   이제 매핑 패널에서 웹 후크의 항목을 사용하여 시나리오의 후속 모듈에서 사용할 수 있습니다.

## 대기열

웹 후크가 데이터를 수신하고 해당 데이터를 예상하는 활성 시나리오가 없는 경우 데이터가 큐에 저장됩니다. 시나리오를 활성화하면 큐에서 대기하는 모든 번들을 순차적으로 처리합니다.

>[!IMPORTANT]
>
>웹 후크 큐는 동일한 웹 후크를 사용하는 시나리오 간에 공유됩니다. 시나리오 중 하나가 비활성화되면 들어오는 모든 데이터가 큐에 저장됩니다.

## 지원되는 수신 데이터 형식

[!DNL Workfront Fusion] 에서는 3개의 수신 데이터 형식을 지원합니다. [!UICONTROL 쿼리 문자열], [!UICONTROL 양식 데이터] 및 [!UICONTROL JSON].

[!DNL Workfront Fusion] 선택한 데이터 구조에 대해 들어오는 모든 데이터를 확인합니다. 그런 다음 시나리오의 설정에 따라 데이터가 처리를 위해 큐에 저장되거나 즉시 처리됩니다.

데이터의 일부가 유효성 검사를 통과하지 못하면 [!DNL Workfront Fusion] 400 HTTP 상태 코드를 반환하고 HTTP 응답 본문에 들어오는 데이터가 유효성 검사에 실패한 이유를 지정합니다. 들어오는 데이터의 유효성 검사가 성공하면 Workfront Fusion에서 &quot;[!UICONTROL 200개 수락됨]&quot; 상태.

* [[!UICONTROL 쿼리 문자열]](#query-string)
* [[!UICONTROL 양식 데이터]](#form-data)
* [[!UICONTROL JSON]](#json)

### [!UICONTROL 쿼리 문자열]

```
GET https://app.workfrontfusion.com/wh/<yourunique32characterslongstring>?name=<yourname>&job=automate
```

### [!UICONTROL 양식 데이터]

```
POST https://app.workfrontfusion.com/wh/<yourunique32characterslongstring>

Content-Type: application/x-www-form-urlencoded

name=<yourname>&job=automate
```

#### 다중 부분 양식 데이터

```
POST https://app.workfrontfusion.com/wh/<yourunique32characterslongstring>


Content-Type: multipart/form-data; boundary=---generatedboundary

---generatedboundary

Content-Disposition: form-data; name="file"; filename="file.txt"


Content-Type: text/plain


Content of file.txt


---generatedboundary

Content-Disposition: form-data; name="name"

Workfront Fusion

---generatedboundary
```

로 인코딩된 파일을 수신하려면 `multipart/form-data`를 채울 때는 `collection` 중첩 필드가 포함된 유형 필드 `name`, `mime`, 및 `data`. 필드 `name` is `text` 를 입력하고 업로드한 파일의 이름을 포함합니다. 다음 `mime` is `text` MIME 형식의 파일을 입력하고 포함합니다. 필드 `data` is `buffer` 을 입력하고 전송할 파일에 대한 이진 데이터를 포함합니다.

MIME 형식에 대한 자세한 내용은 [MIME 모듈](../../workfront-fusion/apps-and-their-modules/mime.md).

### [!UICONTROL JSON]

```
POST https://app.workfrontfusion.com/wh/<yourunique32characterslongstring>

Content-Type: application/json

{"name": "Workfront Fusion", "job": "automate"}
```

>[!TIP]
>
>원래 JSON에 액세스하려면 웹 후크를 설정할 때 JSON 패스스루를 활성화합니다.
>
>1. 클릭 **[!UICONTROL 추가]** 새 웹 후크를 추가합니다.
>1. 클릭 **[!UICONTROL 고급 설정 표시]**.
>1. 클릭 **[!UICONTROL JSON 통과]**.

>


## Webhook 헤더

웹 후크의 헤더에 액세스하려면 웹 후크를 설정할 때 요청 헤더 가져오기 를 활성화합니다.

1. 클릭 **[!UICONTROL 추가]** 새 웹 후크를 추가합니다.
1. 클릭 **[!UICONTROL 고급 설정 표시]**.
1. 클릭 **[!UICONTROL 요청 헤더 가져오기]**.

의 조합으로 특정 헤더 값을 추출할 수 있습니다 `map()` 및 `get()` 함수 위에 있어야 합니다.

>[!INFO]
>
>**예:**
>
>아래 예는 의 값을 추출하는 공식을 보여줍니다 `authorization` 헤더 `Headers[]` 배열입니다. 일치하는 경우 추출된 값과 지정된 텍스트를 비교하여 웹 후크만 전달하는 필터에 수식이 사용됩니다.
>
>![](assets/set-up-a-filter-350x169.png)
>
>지정된 키로 배열 요소를 가져오는 방법에 대한 자세한 내용은 [배열의 요소를 지정된 키에 매핑](../../workfront-fusion/mapping/map-information-between-modules.md#mapping) 기사 [Adobe Workfront Fusion에서 한 모듈의 정보를 다른 모듈에 매핑](../../workfront-fusion/mapping/map-information-between-modules.md).

## Webhooks에 응답

웹 후크 호출에 대한 기본 응답은 &quot;Accepted&quot;입니다. 응답이 사용자 지정 웹 후크 모듈을 실행하는 동안 웹 후크를 호출한 앱에 반환됩니다.

* [웹 후크에 대한 응답 테스트](#test-the-response-to-a-webhook)
* [HTML 응답 예](#html-response-example)
* [리디렉션 예](#redirect-example)

### 웹 후크에 대한 응답 테스트

1. 다음을 포함합니다 **[!UICONTROL 사용자 지정 웹 후크]** 모듈의 수준을 제어합니다.
1. 모듈에 새 웹 후크를 추가합니다.
1. 웹 후크 URL을 클립보드에 복사합니다.
1. 시나리오를 실행합니다.

   번개 아이콘은 [!UICONTROL 사용자 지정 웹 후크] 모듈이 회전하는 점으로 변경됩니다. 이제 모듈이 웹 후크 호출을 기다리고 있음을 보여줍니다.

1. 새 브라우저 창을 열고, 주소 표시줄에 복사한 URL을 붙여 넣은 다음 키를 누릅니다 **[!UICONTROL Enter 키]**.

   다음 [!UICONTROL 사용자 지정 웹 후크] 모듈이 트리거되고 브라우저에 새 페이지가 표시됩니다.

웹 후크의 응답을 사용자 지정하려면 Webhook Response 모듈을 사용합니다.

모듈 구성에는 두 개의 필드가 포함되어 있습니다. [!UICONTROL 상태] 및 [!UICONTROL 본문].

* 다음 [!UICONTROL 상태] 필드에는 성공 시 2xx와 같은 HTTP 응답 상태 코드가 포함됩니다(예: `200` 3xx의 리디렉션(예: `307` 임시 리디렉션의 경우), 클라이언트 오류(예: `400` 잘못된 요청) 등입니다.

* 다음 [!UICONTROL 본문] 필드에는 웹 후크 호출에서 수락하는 모든 항목이 포함되어 있습니다. 단순 텍스트, HTML, XML, JSON 등이 될 수 있습니다.

   >[!TIP]
   >
   >을 설정하는 것이 좋습니다 `Content-Type` 헤더 를 해당 MIME 유형으로: `text/plain` 일반 텍스트의 경우 `text/html` HTML, `application/json` JSON용, `application/xml` XML 등에 사용됩니다. MIME 유형에 대한 자세한 내용은 [MIME 모듈](../../workfront-fusion/apps-and-their-modules/mime.md).

응답 전송 시간 제한은 40초입니다. 해당 기간 내에 응답을 사용할 수 없는 경우 Workfront Fusion은 &#39;200 수락됨&#39; 상태를 반환합니다.

### HTML 응답 예

>[!INFO]
>
>**예:**
>
>구성 [!UICONTROL Webhook 응답] 모듈은 다음과 같습니다.
>
><table style="table-layout:auto"> 
&gt; <col> 
&gt; <col> 
&gt; <tbody> 
&gt;  <tr> 
&gt;   <td role="rowheader">[!UICONTROL 상태] </td> 
&gt;   <td> <p>2xx 성공 HTTP 상태 코드(예: 200)</p> </td> 
&gt;  </tr> 
&gt;  <tr> 
&gt;   <td role="rowheader">[!UICONTROL Body] </td> 
&gt;   <td> <p>HTML 코드</p> </td> 
&gt;  </tr> 
&gt;  <tr> 
&gt;   <td role="rowheader"> <p>[!UICONTROL 사용자 지정 헤더]</p> </td> 
&gt;   <td> 
&gt;    <ul> 
&gt;     <li><strong>키</strong>: 컨텐츠 유형</li> 
&gt;     <li><strong>값</strong>: 텍스트/html</li> 
&gt;    </ul> </td> 
&gt;  </tr> 
&gt; </tbody> 
&gt;</table>
>
>![](assets/custom-headers-350x235.png)
>
>이렇게 하면 웹 브라우저에 표시되는 HTML 응답이 생성됩니다.
>
>![](assets/html-response-350x70.png)

### 리디렉션 예

>[!INFO]
>
>**예:** 구성 [!UICONTROL Webhook 응답] 모듈은 다음과 같습니다.
>
><table style="table-layout:auto"> 
&gt; <col> 
&gt; <col> 
&gt; <tbody> 
&gt;  <tr> 
&gt;   <td role="rowheader">[!UICONTROL 상태] </td> 
&gt;   <td> <p>3xx 리디렉션 HTTP 상태 코드(예: 303)</p> </td> 
&gt;  </tr> 
&gt;  <tr> 
&gt;   <td role="rowheader"> <p>[!UICONTROL 사용자 지정 헤더]</p> </td> 
&gt;   <td> 
&gt;    <ul> 
&gt;     <li><strong>[!UICONTROL Key]</strong>: 위치</li> 
&gt;     <li><strong>[!UICONTROL Value]</strong>: 리디렉션할 URL입니다.</li> 
&gt;    </ul> </td> 
&gt;  </tr> 
&gt; </tbody> 
&gt;</table>
>
>![](assets/webhook-response-350x279.png)

## Webhook 비활성화

다음 중 하나가 적용되는 경우 웹 후크는 자동으로 비활성화됩니다.

* 웹 후크가 5일 이상 시나리오에 연결되지 않았습니다
* 웹 후크는 30일 이상 비활성 시나리오에서만 사용됩니다.

비활성화된 웹 후크는 모든 시나리오에 연결되어 있지 않고 30일 이상 비활성화된 상태에 있는 경우 자동으로 삭제되고 등록되지 않습니다.


## 문제 해결

### 매핑 패널에서 항목이 누락됨

다음에 나오는 모듈 설정의 매핑 패널에서 일부 항목이 누락된 경우 [!UICONTROL Webhooks] > [!UICONTROL 사용자 지정 웹 후크] 모듈을 클릭하고 **[!UICONTROL Webhooks] > [!UICONTROL 사용자 지정 웹 후크]** 모듈을 열고 를 클릭합니다. **[!UICONTROL 데이터 구조 재결정]**:

![](assets/redetermine-data-structure-btn-350x195.png)

그런 다음 섹션에 설명된 단계를 수행합니다 [웹 후크의 데이터 구조 구성](#configure-the-webhook-s-data-structure) 참조하십시오.
