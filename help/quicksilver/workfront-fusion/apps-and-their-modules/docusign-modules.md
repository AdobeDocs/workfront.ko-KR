---
title: DocuSign 모듈
description: 다음 [!DNL Adobe Workfront Fusion DocuSign] 모듈을 사용하면 포락선 상태를 모니터링 및 검색하고, 봉투를 검색 및 검색하거나, 문서를 다운로드하여 전송하여 로그인할 수 있습니다 [!DNL DocuSign] 계정이 필요합니다.
author: Becky
draft: Probably
feature: Workfront Fusion, Digital Content and Documents
exl-id: a6ebfe6f-dc3f-41f7-8129-bbc5775cff33
source-git-commit: 885d93dd4383945538e977fd3edbfd55bda88b70
workflow-type: tm+mt
source-wordcount: '1911'
ht-degree: 0%

---

# DocuSign 모듈

다음 [!DNL Adobe Workfront Fusion] [!DNL DocuSign] 모듈을 사용하면 포락선 상태를 모니터링 및 검색하고, 봉투를 검색 및 검색하거나, 문서를 다운로드하여 전송하여 로그인할 수 있습니다 [!DNL DocuSign] 계정이 필요합니다.

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

를 사용하려면 [!DNL DocuSign] 모듈이면 반드시 [!DNL DocuSign] 계정이 필요합니다.

## Connect [!DNL DocuSign] to [!DNL Workfront Fusion] {#connect-docusign-to-workfront-fusion}

에 대한 연결을 만들려면 [!DNL DocuSign] 모듈:

1. 클릭 **[!UICONTROL 추가]** 다음 [!UICONTROL 연결] 첫 번째 구성 시작 시 [!DNL DocuSign] 모듈.
1. 다음을 입력합니다.

<table style="table-layout:auto">
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader"> <p>[!UICONTROL 연결 이름]</p> </td> 
      <td>새 이름을 입력합니다 [!DNL DocuSign] 연결</td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL 계정 유형]</td> 
      <td>연결할 계정이 프로덕션 계정인지 데모 계정인지 여부를 선택합니다.</td> 
     </tr> 
    </tbody> 
   </table>

1. 에 설명된 대로 계속 [연결 만들기 [!DNL Adobe Workfront Fusion] - 기본 지침](../../workfront-fusion/connections/connect-to-fusion-general.md#connect).

## [!DNL DocuSign] 모듈 및 해당 필드

구성 시 [!DNL DocuSign] 모듈, [!DNL Workfront Fusion] 아래 나열된 필드를 표시합니다. 이와 함께 추가 [!DNL DocuSign] 앱이나 서비스에서 액세스 수준과 같은 요소에 따라 필드가 표시될 수 있습니다. 모듈에서 굵게 표시된 제목은 필수 필드를 나타냅니다.

필드 또는 함수 위에 맵 단추가 표시되면 이 단추를 사용하여 해당 필드에 대한 변수와 함수를 설정할 수 있습니다. 자세한 내용은 [의 한 모듈에서 다른 모듈로 정보 매핑 [!DNL Adobe Workfront Fusion]](../../workfront-fusion/mapping/map-information-between-modules.md).

![](assets/map-toggle-350x74.png)

* [Triggers](#triggers)
* [액션](#actions)

### Triggers

#### [!UICONTROL 봉투 보기]

이 트리거 모듈은 봉투를 전송, 전달, 서명, 완료 또는 거부할 때 시나리오를 시작합니다.

<table style="table-layout:auto">
 <col data-mc-conditions=""> 
 <col data-mc-conditions=""> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection] </td> 
   <td> <p>연결 방법에 대한 지침은 [!DNL DocuSign] 계정 대상 [!DNL Workfront Fusion]를 참조하십시오. <a href="../../workfront-fusion/scenarios/create-a-scenario.md#connect" class="MCXref xref">모듈의 앱 또는 웹 서비스를 [!DNL Workfront Fusion]</a> 기사 <a href="../../workfront-fusion/scenarios/create-a-scenario.md" class="MCXref xref">에서 시나리오 만들기 [!DNL Adobe Workfront Fusion]</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Account] </td> 
   <td> <p>보려는 레코드가 포함된 계정을 선택합니다.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL 이벤트 유형]</td> 
   <td> <p> 보려는 이벤트 유형을 선택합니다.</p> 
    <ul> 
     <li>[!UICONTROL 문서 완료]</li> 
     <li>[!UICONTROL 문서가 거부되었습니다.]</li> 
     <li>[!UICONTROL Document sent]</li> 
     <li>[!UICONTROL Document signed]</li> 
     <li>[!UICONTROL 받은 편지함의 새 문서]</li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL 출력 필드]</p> </td> 
   <td> <p>모듈 출력에 포함할 필드를 선택합니다.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL 제한]</td> 
   <td>각 시나리오 실행 주기 동안 모듈이 작업할 최대 레코드 수를 입력하거나 매핑합니다.</td> 
  </tr> 
 </tbody> 
</table>

### 액션

* [[!UICONTROL 사용자 지정 API 호출]](#custom-api-call)
* [[!UICONTROL 문서 다운로드]](#download-a-document)
* [[!UICONTROL 봉투 읽기]](#read-an-envelope)
* [[!UICONTROL 포락선에 파일 업로드]](#upload-a-file-to-an-envelope)
* [[!UICONTROL 새 봉투 만들기]](#create-a-new-envelope)
* [[!UICONTROL 봉투에 수신자 추가]](#add-recipient-to-envelope)
* [[!UICONTROL 사용자 지정 필드 추가]](#add-custom-field)
* [[!UICONTROL 사용자 지정 필드 수정]](#modify-custom-field)
* [[!UICONTROL 봉투 보내기]](#send-envelope)

#### [!UICONTROL 사용자 지정 API 호출]

이 작업 모듈을 사용하여 사용자 지정 API 호출을 수행할 수 있습니다.

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL Connection]</td> 
   <td> <p>연결 방법에 대한 지침은 [!DNL DocuSign] 계정 대상 [!DNL Workfront Fusion]를 참조하십시오. <a href="#connect-docusign-to-workfront-fusion" class="MCXref xref">Connect [!DNL DocuSign] to [!DNL Workfront Fusion]</a> 참조하십시오.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Account]</td> 
   <td>액세스할 계정을 입력하거나 매핑합니다 [!DNL DocuSign] API.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL URL]</td> 
   <td> <p>모듈이 상호 작용할 웹 서버의 주소를 입력합니다.</p> <p>상대 URL을 입력할 수 있습니다. 즉, 프로토콜을 포함하지 않아도 됩니다(예: <code>http://</code>)을 클릭하여 제품에서 사용할 수 있습니다. 이는 상호 작용이 서버에서 발생함을 웹 서버에 알려줍니다.</p> <p>For example: <code>[!DNL /api/conversations].create</code></p> <p>팁: 사용 가능한 끝점 목록에 대해서는 <a href="https://developers.docusign.com/esign-rest-api/reference">[!DNL DocuSign] API 참조</a>.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL 메서드]</td> 
   td&gt; <p>API 호출을 구성하는 데 필요한 HTTP 요청 메서드를 선택합니다. 자세한 내용은 <a href="../../workfront-fusion/modules/http-request-methods.md" class="MCXref xref" data-mc-variable-override="">의 HTTP 요청 메서드 [!DNL Adobe Workfront Fusion]</a>.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Headers]</td> 
   <td> <p>요청의 헤더를 표준 JSON 개체 형태로 추가합니다. 요청의 콘텐츠 유형을 결정합니다.</p> <p>For example,<code> {"Content-type":"application/json"}</code></p> <p>참고: 오류가 발생하여 출처를 확인하기 어려운 경우, [!DNL Workfront] 설명서. 사용자 지정 API 호출이 422 HTTP 요청 오류를 반환하는 경우 "Content-Type":"text/plain" 헤더를 사용해 보십시오.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL 쿼리 문자열]</td> 
   <td> <p>표준 JSON 개체 형태로 API 호출에 대한 쿼리를 추가합니다.</p> <p>For example: <code>{"name":"something-urgent"}</code></p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Body]</td> 
   <td> <p>표준 JSON 개체 형태로 API 호출에 대한 본문 콘텐츠를 추가합니다.</p> <p>참고:  <p>다음과 같은 조건문을 사용하는 경우 <code>if</code> json에서 따옴표를 조건문 외부에 지정합니다.</p> 
     <div class="example" data-mc-autonum="<b>Example: </b>"> 
      <p> <img src="assets/quotes-in-json-350x120.png" style="width: 350;height: 120;"> </p> 
     </div> </p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL 제한]</td> 
   <td>한 실행 주기 동안 작업할 최대 결과 수를 입력하거나 매핑합니다.</td> 
  </tr> 
 </tbody> 
</table>

>[!INFO]
>
>**예:** 목록 봉투
>
>다음 API 호출은 [!DNL DocuSign] 계정:
>
>**URL**: `/v2.1/accounts/{accountId}/envelopes/`
>
>**메서드**: `GET`
>
>**쿼리 문자열**:
>
>* **키**: `from_date`
>
>* **값**: `YYYY-MM-DD`
>
>요청이 계정의 봉투에 대한 상태 변경 확인을 시작하는 시기를 지정합니다.
>
>![](assets/example-docusign-setup-350x770.png)
>
>결과는 모듈의 Output(번들 > Body > Envelope)에서 찾을 수 있습니다.
>
>이 예제에서는 6개의 봉투가 반환되었습니다.
>
>![](assets/docusign-example-output-350x677.png)

#### [!UICONTROL 문서 다운로드]

이 작업 모듈은 단일 문서를 다운로드합니다.

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td> 
   <td> <p>연결 방법에 대한 지침은 [!DNL DocuSign] 계정 대상 [!DNL Workfront Fusion]를 참조하십시오. <a href="#connect-docusign-to-workfront-fusion" class="MCXref xref">Connect [!DNL DocuSign] to [!DNL Workfront Fusion]</a> 참조하십시오.</p> </td>
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Account] </td> 
   <td> <p>다운로드할 문서가 포함된 계정을 선택합니다.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Envelope ID]</td> 
   <td> <p> 다운로드할 봉투의 ID를 입력하거나 매핑합니다.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL 문서 ID]</p> </td> 
   <td> <p>다운로드할 문서의 ID를 입력하거나 매핑합니다.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Certificate]</td> 
   <td>선택 <strong>[!UICONTROL Yes]</strong> 다운로드 시 봉투 서명 인증서를 포함하려면 다음을 수행하십시오.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Documents by User ID]</td> 
   <td>선택 <strong>[!UICONTROL Yes]</strong> 수신자가 사용자 ID로 문서를 검색하도록 허용하려는 경우. 예를 들어, 사용자가 서로 다른 시각성을 가진 두 개의 서로 다른 공정순서 주문에 포함된 경우, 이 옵션을 사용하면 두 공정순서 모두에서 모든 문서를 반환합니다.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Encrypt]</td> 
   <td>선택 <strong>[!UICONTROL Yes]</strong> 응답에서 반환되는 PDF 바이트가 [!DNL DocuSign] 계정이 필요합니다.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Language]</td> 
   <td>언어를 선택합니다.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL 변경 사항 표시]</td> 
   <td>로 설정된 경우 <strong>[!UICONTROL Yes]</strong>따라서 반환된 PDF에 대해 변경된 모든 필드는 노란색으로 강조 표시되고 선택적 서명 또는 이니셜은 빨간색으로 윤곽선이 표시됩니다.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL 워터마크]</td> 
   <td> <p>선택 <strong>[!UICONTROL No]</strong> PDF 문서에서 워터마크를 제거하려면</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL 봉투 읽기]

이 작업 모듈은 Envelope에 대한 정보를 읽습니다. [!DNL DocuSign] 봉투 ID 사용.

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td> 
   <td> <p>연결 방법에 대한 지침은 [!DNL DocuSign] 계정 대상 [!DNL Workfront Fusion]를 참조하십시오. <a href="#connect-docusign-to-workfront-fusion" class="MCXref xref">Connect [!DNL DocuSign] to [!DNL Workfront Fusion]</a> 참조하십시오.</p> </td>
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Account] </td> 
   <td> <p>정보를 읽을 문서가 포함된 계정을 선택합니다.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Envelope ID]</td> 
   <td> <p> 정보를 읽을 문서가 포함된 ID를 입력하거나 매핑합니다.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL 출력]</td> 
   <td>모듈의 출력에 표시할 속성을 선택합니다. </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL 포락선에 파일 업로드]

이 모듈은 지정된 파일을 DocuSign의 기존 봉투에 업로드합니다.

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td> 
   <td> <p>연결 방법에 대한 지침은 [!DNL DocuSign] 계정 대상 [!DNL Workfront Fusion]를 참조하십시오. <a href="#connect-docusign-to-workfront-fusion" class="MCXref xref">Connect [!DNL DocuSign] to [!DNL Workfront Fusion]</a> 참조하십시오.</p> </td>
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Account] </td> 
   <td> <p>파일을 업로드할 봉투를 포함하는 계정을 선택합니다.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Envelope ID]</td> 
   <td> <p> 파일을 업로드할 봉투 ID를 입력하거나 매핑합니다.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL 소스 파일]</td> 
   <td>이전 모듈에서 소스 파일을 선택하거나 소스 파일의 이름과 데이터를 입력합니다.</td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL 새 봉투 만들기]

이 작업 모듈은 템플릿에서 새 봉투를 만듭니다. 새 봉투의 ID와 새 봉투의 상태를 반환합니다.

<table style="table-layout:auto">
 <col data-mc-conditions=""> 
 <col data-mc-conditions=""> 
 <tbody> 
  <tr> 
    <td role="rowheader">[!UICONTROL Connection] </td>

<td> <p>DocuSign 계정을 Workfront Fusion에 연결하는 방법에 대한 지침은 <a href="../../workfront-fusion/scenarios/create-a-scenario.md#connect" class="MCXref xref">모듈의 앱 또는 웹 서비스를 Workfront Fusion에 연결</a> 기사 <a href="../../workfront-fusion/scenarios/create-a-scenario.md" class="MCXref xref">Adobe Workfront Fusion에서 시나리오 만들기</a>.</p> </td> 
  </tr> 
  <tr> 
    <td role="rowheader">[!UICONTROL Account] </td>
   <td> <p>파일을 업로드할 봉투를 포함하는 계정을 선택합니다.</p> </td> 
  </tr> 
  <tr> 
    <td role="rowheader" >[!UICONTROL Template]</td>
   <td> <p> 새 포락선을 만들 템플릿을 선택합니다. 템플릿은 선택한 [!UICONTROL 계정]에 따라 사용할 수 있습니다.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">
     [!UICONTROL 생성 후]
   </td> 
   <td> <p>봉투를 초안으로 저장할지 또는 서명을 위해 전송할지를 선택합니다.</p> </td> 
  </tr> 
  <tr> 
    <td role="rowheader" >[!UICONTROL 템플릿 수신자]</td>
    <td>이 봉투의 받는 사람 선택</td>
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL 봉투에 수신자 추가]

이 작업 모듈은 수신자를 하나 이상 기존 포락선에 추가합니다. 봉투를 이미 보낸 경우 수신자에게 이메일이 전송됩니다. 이 모듈은 이미 완료된 봉투에 적합하지 않습니다.

<table style="table-layout:auto">
 <col data-mc-conditions=""> 
 <col data-mc-conditions=""> 
 <tbody> 
  <tr data-mc-conditions=""> 
    <td>[!UICONTROL Connection] </td>
   <td> <p>DocuSign 계정을 Workfront Fusion에 연결하는 방법에 대한 지침은 <a href="../../workfront-fusion/scenarios/create-a-scenario.md#connect" class="MCXref xref">모듈의 앱 또는 웹 서비스를 Workfront Fusion에 연결</a> 기사 <a href="../../workfront-fusion/scenarios/create-a-scenario.md" class="MCXref xref">Adobe Workfront Fusion에서 시나리오 만들기</a>.</p> </td> 
  </tr> 
  <tr data-mc-conditions="">
    <td>[!UICONTROL Account] </td>
   <td> <p>수신자를 추가할 봉투가 포함된 계정을 선택합니다.</p> </td> 
  </tr> 
  <tr> 
    <td>[!UICONTROL Envelope ID]</td>
    <td>수신자를 추가할 봉투의 ID를 선택하거나 매핑합니다.</td>
  </tr> 
  <tr data-mc-conditions="">
    <td role="rowheader">[!UICONTROL Recipient type]</td>
   <td> <p> 봉투에 추가할 수신자 유형을 선택합니다.</p> 
    <ul> 
     <li> <p>[!UICONTROL Agent]</p> </li> 
     <li> <p>[!UICONTROL Copy]</p> </li> 
     <li> <p>[!UICONTROL Certified Delivery]</p> </li> 
     <li> <p>[!UICONTROL In-Person Signer]</p> </li> 
     <li> <p>[!UICONTROL Interference]</p> </li> 
     <li> <p>[!UICONTROL Signer]</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
    <td>[!UICONTROL Email]</td>
   <td> <p>봉투에 추가할 수신자의 전자 메일 주소를 입력하거나 매핑합니다.</p> </td> 
  </tr> 
  <tr> 
    <td>[!UICONTROL Name]</td>
   <td>봉투에 추가할 수신자의 이름을 입력하거나 매핑합니다.</td> 
  </tr> 
  <tr>
    <td>[!UICONTROL 라우팅 순서]</td>
   <td> <p>수신자의 공정순서 번호를 입력하거나 매핑합니다. 라우팅 번호는 수신자가 문서를 받고 서명하는 순서를 결정합니다.</p> </td> 
  </tr> 
  <tr> 
    <td role="rowheader">[!UICONTROL Email Body]</td>
   <td>수신자에게 이메일의 본문(콘텐츠)을 입력하거나 매핑합니다.</td> 
  </tr> 
  <tr>
    <td role="rowheader">[!UICONTROL Email Subject]</td>
   <td>수신자에게 보낼 전자 메일의 제목을 입력하거나 매핑합니다.</td> 
  </tr> 
    <td role="rowheader">[!UICONTROL Private 메시지]</td>
   <td> <li> <p>선택한 수신자만 개인 메시지와 일반 메시지를 봅니다. 비공개 메시지는 1000자로 제한됩니다.</p> </li> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Authentication]</td> 
   <td> <p>수신자의 ID를 확인하는 데 사용할 인증 방법을 선택합니다.</p> 
    <ul> 
     <li> <p><strong>[!UICONTROL None]</strong> </p> </li> 
     <li> <p><strong>[!UICONTROL Access code]</strong> </p> <p>액세스 코드를 입력하거나 매핑합니다.</p> </li> 
     <li> <p><strong>[!UICONTROL Phone]</strong> </p> <p>전화 번호를 입력하거나 매핑합니다</p> </li> 
     <li> <p><strong>[!UICONTROL SMS]</strong> </p> <p>전화 번호를 입력하거나 매핑합니다</p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL 사용자 지정 필드 추가]

이 작업 모듈은 문서에 사용자 정의 필드를 추가합니다

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td> 
   <td> <p>연결 방법에 대한 지침은 [!DNL DocuSign] 계정 대상 [!DNL Workfront Fusion]를 참조하십시오. <a href="#connect-docusign-to-workfront-fusion" class="MCXref xref">Connect [!DNL DocuSign] to [!DNL Workfront Fusion]</a> 참조하십시오.</p> </td>
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Account] </td> 
   <td> <p>사용자 지정 필드를 추가할 문서가 포함된 계정을 선택합니다.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Envelope ID]</td> 
   <td> <p> 사용자 지정 필드를 추가할 문서가 포함된 봉투의 ID를 입력하거나 매핑합니다.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL 필드 이름]</td> 
   <td>추가할 새 필드의 이름을 입력하거나 매핑합니다.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL 필수]</td> 
   <td>추가된 필드를 필수 필드로 사용하려면 이 옵션을 활성화합니다.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Show field]</td> 
   <td>필드를 표시하려면 이 옵션을 활성화합니다.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Value]</td> 
   <td>추가된 필드의 값(콘텐츠)을 입력하거나 매핑합니다. </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL 사용자 지정 필드 수정]

이 작업 모듈은 필드 이름을 사용하여 사용자 지정 필드를 수정합니다.

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td> 
   <td> <p>연결 방법에 대한 지침은 [!DNL DocuSign] 계정 대상 [!DNL Workfront Fusion]를 참조하십시오. <a href="#connect-docusign-to-workfront-fusion" class="MCXref xref">Connect [!DNL DocuSign] to [!DNL Workfront Fusion]</a> 참조하십시오.</p> </td>
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Account] </td> 
   <td> <p>사용자 지정 필드를 수정할 문서가 포함된 계정을 선택합니다.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Envelope ID]</td> 
   <td> <p> 사용자 정의 필드를 수정할 문서가 포함된 봉투의 ID를 입력하거나 매핑합니다.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL 필드 ID]</td> 
   <td>수정할 필드의 ID를 입력하거나 매핑합니다.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL 필드 이름]</td> 
   <td>수정할 필드의 이름을 입력하거나 매핑합니다.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL 필수]</td> 
   <td>수정된 필드를 필수 필드로 지정하려면 이 옵션을 활성화합니다.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Show field]</td> 
   <td>필드를 표시하려면 이 옵션을 활성화합니다.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Value]</td> 
   <td>수정된 필드의 값(컨텐츠)을 입력하거나 매핑합니다. </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL 봉투 보내기]

이 작업 모듈은 수신자에게 초안 봉투를 보냅니다.

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td> 
   <td> <p>연결 방법에 대한 지침은 [!DNL DocuSign] 계정 대상 [!DNL Workfront Fusion]를 참조하십시오. <a href="#connect-docusign-to-workfront-fusion" class="MCXref xref">Connect [!DNL DocuSign] to [!DNL Workfront Fusion]</a> 참조하십시오.</p> </td>
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Account] </td> 
   <td> <p>수신자에게 보낼 초안 봉투가 포함된 계정을 선택합니다.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Envelope ID]</td> 
   <td> <p> 수신자에게 보낼 초안 봉투의 ID를 입력하거나 매핑합니다.</p> </td> 
  </tr> 
 </tbody> 
</table>
