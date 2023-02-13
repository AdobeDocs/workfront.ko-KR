---
content-type: reference
product-previous: workfront-fusion
product-area: workfront-integrations;documents
keywords: 커넥터
navigation-topic: apps-and-their-modules
title: 기본 모듈
description: 에서 [!DNL Adobe Workfront Fusion] 시나리오, [!DNL Bynder]여러 타사 애플리케이션 및 서비스에 연결할 수 있습니다.
author: Becky
feature: Workfront Fusion
exl-id: e4dc9588-334a-41a3-85d1-996cb819c3fa
source-git-commit: 885d93dd4383945538e977fd3edbfd55bda88b70
workflow-type: tm+mt
source-wordcount: '1616'
ht-degree: 0%

---

# [!DNL Bynder] 모듈

에서 [!DNL Adobe Workfront Fusion] 시나리오, [!DNL Bynder]여러 타사 애플리케이션 및 서비스에 연결할 수 있습니다.

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

를 사용하려면 [!DNL Bynder] 모듈이면 반드시 [!DNL Bynder] 계정이 필요합니다.

## Connect [!DNL Bynder] Workfront Fusion으로  {#connect-bynder-to-workfront-fusion}

* [연결 만들기 [!DNL Bynder] 변환 전: [!DNL Workfront Fusion]](#create-a-connection-to-bynder-from-workfront-fusion)
* [생성 [!UICONTROL 클라이언트 ID] 및 [!UICONTROL 클라이언트 암호] in [!DNL Bynder] (선택 사항)](#generate-a-client-id-and-client-secret-in-bynder-optional)

### 연결 만들기 [!DNL Bynder] 변환 전: [!DNL Workfront Fusion]

연결을 만들 수 있습니다 [!DNL Workfront Fusion] 아래와 같이 [!DNL Bynder] 내에서 직접 계정 [!DNL Bynder] 모듈.

1. 어떤 경우에서도 [!DNL Bynder] 모듈 **[!UICONTROL 추가]** 다음 [!UICONTROL 연결] 필드.
1. 을(를) 선택합니다 [!DNL Bynder] 연결할 도메인입니다.
1. (선택 사항) **[!UICONTROL 고급 설정]**&#x200B;를 입력한 다음 를 입력합니다. [!UICONTROL 클라이언트 ID] 및 [!UICONTROL 클라이언트 암호].

   클라이언트 ID 및 클라이언트 암호 생성에 대한 지침은 [에서 클라이언트 ID 및 클라이언트 암호 생성 [!DNL Bynder] (선택 사항)](#generate-a-client-id-and-client-secret-in-bynder-optional) 참조하십시오.

1. 에서 [!UICONTROL 로그인] 창에서 사용자 이름(이메일 주소)과 암호를 입력합니다.
1. 클릭 **[!UICONTROL 계속]** 연결을 만들고 모듈로 돌아갑니다.

### 생성 [!UICONTROL 클라이언트 ID] 및 [!UICONTROL 클라이언트 암호] in [!DNL Bynder] (선택 사항)

클라이언트 ID 및 클라이언트 암호를 사용하여 연결을 만들려면 [!DNL Bynder] 계정이 필요합니다. 에서 앱을 만들 때 클라이언트 ID 및 클라이언트 암호 가 생성됩니다 [!DNL Bynder].

에서 앱을 만드는 방법에 대한 지침은 [!DNL Bynder]를 참조하십시오. [Oauth 2.0 앱](https://developer-docs.bynder.com/api/authentication-oauth2-oauth-apps/) 에서 [!DNL Bynder] 설명서.

>[!NOTE]
>
>에서 앱을 만들 때 [!DNL Bynder]을 입력하여 다음을 `redirect uri`:
>
>`https://app.workfrontfusion.com/oauth/cb/workfront-bynder`

## [!DNL Bynder] 모듈 및 해당 필드

구성 시 [!DNL Bynder] 모듈, [!DNL Workfront Fusion] 아래 나열된 필드를 표시합니다. 이와 함께 추가 [!DNL Bynder] 앱이나 서비스에서 액세스 수준과 같은 요소에 따라 필드가 표시될 수 있습니다. 모듈에서 굵게 표시된 제목은 필수 필드를 나타냅니다.

필드 또는 함수 위에 맵 단추가 표시되면 이 단추를 사용하여 해당 필드에 대한 변수와 함수를 설정할 수 있습니다. 자세한 내용은 [의 한 모듈에서 다른 모듈로 정보 매핑 [!DNL Adobe Workfront Fusion]](../../workfront-fusion/mapping/map-information-between-modules.md).

![](assets/map-toggle-350x74.png)

* [액션](#actions)
* [검색 결과](#searches)
* [Triggers](#triggers)

### 액션

* [[!UICONTROL 사용자 지정 API 호출]](#custom-api-call)
* [[!UICONTROL 자산 메타데이터 읽기]](#read-asset-metadata)
* [[!UICONTROL 자산 메타데이터 업데이트]](#update-asset-metadata)
* [[!UICONTROL 컬렉션에 자산 추가]](#add-assets-to-a-collection)
* [[!UICONTROL 컬렉션에서 자산 제거]](#remove-assets-from-collection)
* [[!UICONTROL 자산에 태그 추가]](#add-a-tag-to-assets)
* [[!UICONTROL 태그 제거] 자산에서](#remove-a-tag-from-assets)
* [[!UICONTROL 자산 다운로드]](#download-asset)
* [[!UICONTROL 자산 업로드]](#upload-asset)

#### [!UICONTROL 사용자 지정 API 호출]

이 작업 모듈을 사용하면 [!DNL Bynder] API. 이렇게 하면 다른 방식으로 수행할 수 없는 데이터 흐름 자동화를 만들 수 있습니다 [!DNL Bynder] 모듈.

이 모듈을 구성할 때 다음 필드가 표시됩니다.

이 모듈은 API 호출의 헤더 및 본문과 함께 상태 코드를 반환합니다.

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
    <td role="rowheader"> <p>[!UICONTROL Connection]</p> </td> 
   <td> <p>연결 방법에 대한 지침은 [!DNL Bynder] 계정 대상 [!DNL Workfront Fusion]를 참조하십시오. <a href="#connect-bynder-to-workfront-fusion" class="MCXref xref">Connect [!DNL Bynder] to [!DNL Workfront Fusion] </a> 참조하십시오.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">URL</td> 
   <td>상대 경로 입력 <code>https://{your-bynder-domain}/api/{api-version}/</code>.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL 메서드]</td> 
   td&gt; <p>API 호출을 구성하는 데 필요한 HTTP 요청 메서드를 선택합니다. 자세한 내용은 <a href="../../workfront-fusion/modules/http-request-methods.md" class="MCXref xref" data-mc-variable-override="">의 HTTP 요청 메서드 [!DNL Adobe Workfront Fusion]</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Headers]</td> 
   <td> <p>요청의 헤더를 표준 JSON 개체 형태로 추가합니다.</p> <p>For example: <code>{"Content-type":"application/json"}</code></p> <p>Workfront Fusion이 사용자를 위해 인증 헤더를 추가합니다.</p> </td> 
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

#### [!UICONTROL 자산 메타데이터 읽기]

이 작업 모듈은 자산의 메타데이터를 읽습니다.

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Connection]</p> </td> 
   <td> <p>연결 방법에 대한 지침은 [!DNL Bynder] 계정 대상 [!DNL Workfront Fusion]를 참조하십시오. <a href="#connect-bynder-to-workfront-fusion" class="MCXref xref">Connect [!DNL Bynder] to [!DNL Workfront Fusion] </a> 참조하십시오.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Asset ID]</td> 
   <td>메타데이터를 검색할 자산의 ID를 입력하거나 매핑합니다.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL 출력]</td> 
   <td> <p>이 모듈의 출력 번들에 포함할 정보를 선택합니다.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL 자산 메타데이터 업데이트]

이 작업 모듈은 기존 자산의 메타데이터를 업데이트합니다.

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
    <td role="rowheader"> <p>[!UICONTROL Connection]</p> </td> 
   <td> <p>연결 방법에 대한 지침은 [!DNL Bynder] 계정 대상 [!DNL Workfront Fusion]를 참조하십시오. <a href="#connect-bynder-to-workfront-fusion" class="MCXref xref">Connect [!DNL Bynder] to [!DNL Workfront Fusion] </a> 참조하십시오.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Asset ID]</td> 
   <td>메타데이터를 업데이트할 자산의 ID를 입력하거나 매핑합니다.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Fields]</td> 
   <td> <p>정보를 입력할 필드를 선택한 다음 메타데이터를 업데이트할 정보를 해당 필드에 입력하거나 매핑합니다. </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Metadata]</p> </td> 
   <td>업데이트할 옵션을 선택한 다음 해당 속성에 정보를 입력하거나 매핑합니다. 지표 속성은 자산의 특정 필드를 나타내지 않는 자산에 대한 정보입니다.</td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL 컬렉션에 자산 추가]

이 작업 모듈은 컬렉션에 하나 이상의 자산을 추가합니다.

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
    <td role="rowheader"> <p>[!UICONTROL Connection]</p> </td> 
   <td> <p>연결 방법에 대한 지침은 [!DNL Bynder] 계정 대상 [!DNL Workfront Fusion]를 참조하십시오. <a href="#connect-bynder-to-workfront-fusion" class="MCXref xref">Connect [!DNL Bynder] to [!DNL Workfront Fusion] </a> 참조하십시오.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Collection ID]</td> 
   <td> <p>자산을 추가할 컬렉션의 ID를 입력하거나 매핑합니다.</p> <p> </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL 자산 ID]</td> 
   <td> <p>컬렉션에 추가할 각 자산에 대해 <strong>[!UICONTROL 항목 추가]</strong>를 입력한 다음 자산 ID를 입력하거나 매핑합니다.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL 컬렉션에서 자산 제거]

이 작업 모듈은 컬렉션에서 하나 이상의 자산을 제거합니다.

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
    <td role="rowheader"> <p>[!UICONTROL Connection]</p> </td> 
   <td> <p>연결 방법에 대한 지침은 [!DNL Bynder] 계정 대상 [!DNL Workfront Fusion]를 참조하십시오. <a href="#connect-bynder-to-workfront-fusion" class="MCXref xref">Connect [!DNL Bynder] to [!DNL Workfront Fusion] </a> 참조하십시오.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Collection ID]</td> 
   <td> <p>자산을 제거할 컬렉션의 ID를 입력하거나 매핑합니다.</p> <p> </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL 자산 ID]</td> 
   <td> <p>컬렉션에서 제거할 각 자산에 대해 <strong>[!UICONTROL 항목 추가]</strong>를 입력한 다음 자산 ID를 입력하거나 매핑합니다.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL 자산에 태그 추가]

하나 이상의 자산에 태그 추가

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
    <td role="rowheader"> <p>[!UICONTROL Connection]</p> </td> 
   <td> <p>연결 방법에 대한 지침은 [!DNL Bynder] 계정 대상 [!DNL Workfront Fusion]를 참조하십시오. <a href="#connect-bynder-to-workfront-fusion" class="MCXref xref">Connect [!DNL Bynder] to [!DNL Workfront Fusion] </a> 참조하십시오.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL 태그 ID]</td> 
   <td> <p>자산에 추가할 태그의 ID를 입력하거나 매핑합니다.</p> <p> </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL 자산 ID]</td> 
   <td> <p>태깅할 각 자산에 대해 <strong>[!UICONTROL 항목 추가]</strong>를 입력한 다음 자산 ID를 입력하거나 매핑합니다.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL 자산에서 태그 제거]

하나 이상의 자산에서 태그 제거

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
    <td role="rowheader"> <p>[!UICONTROL Connection]</p> </td> 
   <td> <p>연결 방법에 대한 지침은 [!DNL Bynder] 계정 대상 [!DNL Workfront Fusion]를 참조하십시오. <a href="#connect-bynder-to-workfront-fusion" class="MCXref xref">Connect [!DNL Bynder] to [!DNL Workfront Fusion] </a> 참조하십시오.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL 태그 ID]</td> 
   <td> <p>자산에서 제거할 태그의 ID를 입력하거나 매핑합니다.</p> <p> </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL 자산 ID]</td> 
   <td> <p>태그를 제거할 각 자산에 대해 <strong>[!UICONTROL 항목 추가]</strong>를 입력한 다음 자산 ID를 입력하거나 매핑합니다.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL 자산 다운로드]

이 작업 모듈은 단일 자산을 다운로드합니다.

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
    <td role="rowheader"> <p>[!UICONTROL Connection]</p> </td> 
   <td> <p>연결 방법에 대한 지침은 [!DNL Bynder] 계정 대상 [!DNL Workfront Fusion]를 참조하십시오. <a href="#connect-bynder-to-workfront-fusion" class="MCXref xref">Connect [!DNL Bynder] to [!DNL Workfront Fusion] </a> 참조하십시오.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Asset ID]</td> 
   <td>다운로드할 자산의 ID를 입력하거나 매핑합니다.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Asset version]</td> 
   <td> <p>다운로드할 자산의 버전을 입력하거나 매핑합니다. 최신 버전의 자산을 다운로드하려면 필드를 비워 둡니다.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL 자산 업로드]

이 작업 모듈은 단일 자산을 업로드합니다.

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
    <td role="rowheader"> <p>[!UICONTROL Connection]</p> </td> 
   <td> <p>연결 방법에 대한 지침은 [!DNL Bynder] 계정 대상 [!DNL Workfront Fusion]를 참조하십시오. <a href="#connect-bynder-to-workfront-fusion" class="MCXref xref">Connect [!DNL Bynder] to [!DNL Workfront Fusion] </a> 참조하십시오.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL 다른 이름으로 저장]</td> 
   <td> <p>업로드 중인 파일을 저장할 방법을 선택합니다.</p> 
    <ul> 
     <li> <p><strong>[!UICONTROL 새 자산]</strong> </p> <p>정보를 입력할 필드 및 메타 속성을 선택한 다음 해당 필드에 정보를 입력합니다.</p> <p>업로드된 자산에 사용할 브랜드의 ID를 입력하거나 매핑합니다.</p> </li> 
     <li> <p><strong>[!UICONTROL 새 자산 버전]</strong> </p> <p>새 버전을 업로드할 자산의 ID를 입력합니다.</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL 소스 파일]</td> 
   <td>이전 모듈에서 소스 파일을 선택하거나 소스 파일의 이름과 데이터를 매핑합니다.</td> 
  </tr> 
 </tbody> 
</table>

### 검색 결과

* [[!UICONTROL 목록 레코드]](#list-record)
* [[!UICONTROL 자산 검색]](#search-for-assets)

#### [!UICONTROL 목록 레코드]

이 검색 모듈은 특정 유형의 모든 항목을 검색합니다.

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
    <td role="rowheader"> <p>[!UICONTROL Connection]</p> </td> 
   <td> <p>연결 방법에 대한 지침은 [!DNL Bynder] 계정 대상 [!DNL Workfront Fusion]를 참조하십시오. <a href="#connect-bynder-to-workfront-fusion" class="MCXref xref">Connect [!DNL Bynder] to [!DNL Workfront Fusion] </a> 참조하십시오.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL 레코드 유형]</td> 
   <td> <p>나열할 레코드 유형을 선택합니다.</p> 
    <ul> 
     <li> <p><strong>[!UICONTROL 모든 컬렉션 읽기]</strong> </p> </li> 
     <li> <p><strong>[!UICONTROL 모든 태그에 대한 정보 읽기]</strong> </p> </li> 
     <li> <p><strong>[!UICONTROL 컬렉션의 모든 자산 읽기]</strong> </p> <p>자산을 나열할 컬렉션의 ID를 입력하거나 매핑합니다.</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL 출력]</td> 
   <td> <p>모듈의 출력에 포함할 필드를 선택합니다.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL 제한]</td> 
   <td> <p>각 시나리오 실행 주기 동안 모듈이 반환할 최대 자산 수를 입력하거나 매핑합니다.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL 자산 검색]

이 검색 모듈은 제공한 기준에 따라 자산을 검색합니다.

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
    <td role="rowheader"> <p>[!UICONTROL Connection]</p> </td> 
   <td> <p>연결 방법에 대한 지침은 [!DNL Bynder] 계정 대상 [!DNL Workfront Fusion]를 참조하십시오. <a href="#connect-bynder-to-workfront-fusion" class="MCXref xref">Connect [!DNL Bynder] to [!DNL Workfront Fusion] </a> 참조하십시오.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Criteria]</td> 
   <td> <p>검색 기준을 입력합니다. </p> 
    <ul> 
     <li> <p><strong>[!UICONTROL Field]</strong> </p> <p>검색에 사용할 필드를 선택합니다</p> </li> 
     <li> <p><strong>[!UICONTROL 논리 연산자]</strong> </p> <p>검색에 사용할 연산자를 선택합니다.</p> </li> 
     <li> <p><strong>[!UICONTROL Value]</strong> </p> <p>선택한 필드에서 찾을 값을 입력하거나 매핑합니다. 값 유형은 선택한 필드의 데이터 유형과 같아야 합니다. </p> <p>데이터 유형에 대한 자세한 내용은 <a href="../../workfront-fusion/mapping/item-data-types.md" class="MCXref xref">의 항목 데이터 유형 [!DNL Adobe Workfront Fusion]</a>.</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL 결과 집합]</td> 
   <td>일치하는 첫 번째 자산을 반환할지 아니면 일치하는 모든 자산을 반환할지 선택합니다.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL 정렬 기준]</td> 
   <td> <p>정렬할 필드를 선택합니다.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL 정렬 방향]</td> 
   <td> <p>오름차순 또는 내림차순 정렬 여부를 선택합니다.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL 출력]</td> 
   <td> <p>모듈의 출력에 포함할 필드를 선택합니다.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL 제한]</td> 
   <td> <p>각 시나리오 실행 주기 동안 모듈이 반환할 최대 자산 수를 입력하거나 매핑합니다.</p> </td> 
  </tr> 
 </tbody> 
</table>

### Triggers

#### [!UICONTROL 자산 보기]

이 트리거 모듈은 자산을 만들거나 업데이트할 때 시나리오를 시작합니다.

<table style="table-layout:auto">
 <col data-mc-conditions=""> 
 <col data-mc-conditions=""> 
 <tbody> 
  <tr> 
    <td role="rowheader"> <p>[!UICONTROL Connection]</p> </td> 
   <td> <p>연결 방법에 대한 지침은 [!DNL Bynder] 계정 대상 [!DNL Workfront Fusion]를 참조하십시오. <a href="#connect-bynder-to-workfront-fusion" class="MCXref xref">Connect [!DNL Bynder] to [!DNL Workfront Fusion] </a> 참조하십시오.</p> </td> 
  </tr> 
  <tr> <!--
    <td role="rowheader" data-mc-conditions="QuicksilverOrClassic.Draft mode">Event type</td>
   --> <!--
    <td data-mc-conditions="QuicksilverOrClassic.Draft mode">Select whether you want to start the scenario when a new asset is created or when an existing asset is updated.</td>
   --> 
  </tr> 
  <tr>
     <td role="rowheader" data-mc-conditions="QuicksilverOrClassic.Draft mode">[!UICONTROL Collections]</td>
   <td> <p>새 자산에 대해 보려는 컬렉션을 선택합니다. 모든 컬렉션을 보려면 이 필드를 비워 둡니다.</p> </td> 
  </tr> 
  <tr> <!--
    <td role="rowheader" data-mc-conditions="QuicksilverOrClassic.Draft mode">Outputs</td>
   --> <!--
    <td data-mc-conditions="QuicksilverOrClassic.Draft mode">Select the fields that you want to include in the output.</td>
   --> 
  </tr> 
  <tr> 
    <td role="rowheader" data-mc-conditions="QuicksilverOrClassic.Draft mode">[!UICONTROL 제한]</td>

<td> <p>각 시나리오 실행 주기 동안 모듈이 반환할 최대 레코드 수를 입력합니다.</p> </td> 
  </tr> 
 </tbody> 
</table>
