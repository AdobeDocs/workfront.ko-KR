---
title: 모듈 확대
description: 에서 [!DNL Adobe Workfront Fusion] 시나리오, [!UICONTROL 넓이]여러 타사 애플리케이션 및 서비스에 연결할 수 있습니다.
author: Becky
draft: Probably
feature: Workfront Fusion
exl-id: d46935bc-4f6c-4502-bd2f-3927f33241e1
source-git-commit: 885d93dd4383945538e977fd3edbfd55bda88b70
workflow-type: tm+mt
source-wordcount: '1538'
ht-degree: 1%

---

# [!DNL Widen] 모듈

에서 [!DNL Adobe Workfront Fusion] 시나리오, [!UICONTROL 넓이]여러 타사 애플리케이션 및 서비스에 연결할 수 있습니다.

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

를 사용하려면 [!UICONTROL 넓이] 모듈이면 반드시 [!UICONTROL 넓이] 계정이 필요합니다.

## Connect [!DNL Widen] to [!DNL Workfront Fusion] {#connect-widen-to-workfront-fusion}

에 대한 연결을 만들 수 있습니다 [!DNL Widen] 내에서 직접 계정 [!DNL Widen] 모듈.

1. 어떤 경우에서도 [!DNL Widen] 모듈 **[!UICONTROL 추가]** 다음 [!UICONTROL 연결] 필드.
1. 을(를) 선택합니다 [!DNL Widen] 연결할 도메인입니다.
1. 토큰에 사용할 토큰을 입력합니다 [!DNL Widen] 계정이 필요합니다. 이 토큰을 찾는 방법에 대한 지침은 [[!DNL Widen] API FAQ](https://community.widen.com/collective/s/article/API-FAQs).
1. 클릭 **[!UICONTROL 계속]** 연결을 만들고 모듈로 돌아갑니다.

## [!DNL Widen] 모듈 및 해당 필드

구성 시 [!DNL Widen] 모듈, [!DNL Workfront Fusion] 아래 나열된 필드를 표시합니다. 이와 함께 추가 [!DNL Widen] 앱이나 서비스에서 액세스 수준과 같은 요소에 따라 필드가 표시될 수 있습니다. 모듈에서 굵게 표시된 제목은 필수 필드를 나타냅니다.

필드 또는 함수 위에 맵 단추가 표시되면 이 단추를 사용하여 해당 필드에 대한 변수와 함수를 설정할 수 있습니다. 자세한 내용은 [의 한 모듈에서 다른 모듈로 정보 매핑 [!DNL Adobe Workfront Fusion]](../../workfront-fusion/mapping/map-information-between-modules.md).

![](assets/map-toggle-350x74.png)

* [트리거 모듈](#trigger-modules)
* [작업 모듈](#action-modules)
* [검색 모듈](#search-modules)

### 트리거 모듈

#### [!UICONTROL 자산 보기]

이 트리거 모듈은 자산을 만들거나 업데이트할 때 시나리오를 시작합니다.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td> 
  <td> <p>연결 방법에 대한 지침은 [!DNL Widen] 계정 대상 [!DNL Workfront Fusion]를 참조하십시오. <a href="#connect-widen-to-workfront-fusion" class="MCXref xref">Connect [!DNL Widen] to [!DNL Workfront Fusion] </a> 참조하십시오.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL 이벤트 유형]</td> 
   <td> <p>새 자산을 볼지 아니면 업데이트된 자산을 볼지 선택합니다.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Expand]</td> 
   <td> <p>자산 필드 외에 모듈 출력에 포함할 속성을 선택합니다.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL 출력]</td> 
   <td>모듈 출력에 포함할 필드를 선택합니다.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL 제한]</td> 
   <td> <p>각 시나리오 실행 주기 동안 모듈이 작업할 최대 자산 수를 입력하거나 매핑합니다.</p> </td> 
  </tr> 
 </tbody> 
</table>

### 작업 모듈

* [[!UICONTROL 사용자 지정 API 호출]](#custom-api-call)
* [[!UICONTROL 자산 정보 읽기]](#read-asset-info)
* [[!UICONTROL 컬렉션에 자산 추가]](#add-assets-to-collections)
* [[!UICONTROL 컬렉션에서 자산 제거]](#remove-assets-from-collection)
* [[!UICONTROL 자산 메타데이터 업데이트]](#update-asset-metadata)
* [[!UICONTROL 파일 다운로드]](#download-file)
* [[!UICONTROL 업로드] 파일](#upload-a-file)

#### [!UICONTROL 사용자 지정 API 호출]

이 작업 모듈을 사용하면 [!DNL Widen] API. 이렇게 하면 다른 방식으로 수행할 수 없는 데이터 흐름 자동화를 만들 수 있습니다 [!DNL Widen] 모듈.

이 모듈을 구성할 때 다음 필드가 표시됩니다.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td> 
   <td> <p>연결 방법에 대한 지침은 [!DNL Widen] 계정 대상 [!DNL Workfront Fusion]를 참조하십시오. <a href="#connect-widen-to-workfront-fusion" class="MCXref xref">Connect [!DNL Widen] to [!DNL Workfront Fusion] </a> 참조하십시오.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL API 버전]</td> 
   <td>최신 버전의 를 사용할지 여부를 선택합니다 [!DNL Widen] API 또는 버전 1.0</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL URL]</td> 
   <td>API 호출용 URL을 입력하거나 매핑합니다.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL 메서드]</td> 
   <td> <p>API 호출을 구성하는 데 필요한 HTTP 요청 메서드를 선택합니다. 자세한 내용은 <a href="../../workfront-fusion/modules/http-request-methods.md" class="MCXref xref">의 HTTP 요청 메서드 [!DNL Adobe Workfront Fusion]</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Headers]</td> 
   <td> <p>요청의 헤더를 표준 JSON 개체 형태로 추가합니다.</p> <p>For example, <code>{"Content-type":"application/json"}</code></p> <p>[!UICONTROL Workfront Fusion]이 사용자를 위해 인증 헤더를 추가합니다.</p> </td> 
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

#### [!UICONTROL 자산 정보 읽기]

이 작업 모듈은 고유한 ID로 개별 자산을 검색합니다.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td> 
  <td> <p>연결 방법에 대한 지침은 [!DNL Widen] 계정 대상 [!DNL Workfront Fusion]를 참조하십시오. <a href="#connect-widen-to-workfront-fusion" class="MCXref xref">Connect [!DNL Widen] to [!DNL Workfront Fusion] </a> 참조하십시오.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Asset ID]</td> 
   <td> <p>정보를 읽을 자산의 ID를 입력하거나 매핑합니다.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Expand]</td> 
   <td> <p>자산 필드 외에 모듈 출력에 포함할 속성을 선택합니다.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL 출력]</td> 
   <td>모듈 출력에 포함할 필드를 선택합니다.</td> 
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
   <td role="rowheader">[!UICONTROL Connection]</td> 
  <td> <p>연결 방법에 대한 지침은 [!DNL Widen] 계정 대상 [!DNL Workfront Fusion]를 참조하십시오. <a href="#connect-widen-to-workfront-fusion" class="MCXref xref">Connect [!DNL Widen] to [!DNL Workfront Fusion] </a> 참조하십시오.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL 컬렉션 ID]</td> 
   <td> <p>자산을 추가할 각 컬렉션에 대해:</p> 
    <ol> 
     <li value="1"> <p> 클릭 <strong>[!UICONTROL Add]</strong>.</p> </li> 
     <li value="2"> <p>[!UICONTROL Collection ID]를 입력하거나 매핑합니다.</p> </li> 
     <li value="3"> <p>클릭 <strong>[!UICONTROL 항목 추가]</strong>.</p> </li> 
    </ol> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Assets ID]</td> 
   <td> <p>컬렉션에 추가할 각 자산에 대해:</p> 
    <ol> 
     <li value="1"> <p> 클릭 <strong>[!UICONTROL Add]</strong>.</p> </li> 
     <li value="2"> <p>자산 ID를 입력하거나 매핑합니다.</p> </li> 
     <li value="3"> <p>클릭 <strong>[!UICONTROL 항목 추가]</strong>.</p> </li> 
    </ol> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL 제한]</td> 
   <td> <p>각 시나리오 실행 주기 동안 모듈이 작업할 최대 자산 수를 입력하거나 매핑합니다.</p> </td> 
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
   <td role="rowheader">[!UICONTROL Connection]</td> 
  <td> <p>연결 방법에 대한 지침은 [!DNL Widen] 계정 대상 [!DNL Workfront Fusion]를 참조하십시오. <a href="#connect-widen-to-workfront-fusion" class="MCXref xref">Connect [!DNL Widen] to [!DNL Workfront Fusion] </a> 참조하십시오.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL 컬렉션 ID]</td> 
   <td> <p>자산을 제거할 각 컬렉션에 대해:</p> 
    <ol> 
     <li value="1"> <p> 클릭 <strong>[!UICONTROL Add]</strong>.</p> </li> 
     <li value="2"> <p>컬렉션 ID를 입력하거나 매핑합니다.</p> </li> 
     <li value="3"> <p>클릭 <strong>[!UICONTROL 항목 추가]</strong>.</p> </li> 
    </ol> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">자산 ID</td> 
   <td> <p>컬렉션에서 제거할 각 자산에 대해:</p> 
    <ol> 
     <li value="1"> <p> 클릭 <strong>[!UICONTROL Add]</strong>.</p> </li> 
     <li value="2"> <p>자산 ID를 입력하거나 매핑합니다.</p> </li> 
     <li value="3"> <p>클릭 <strong>[!UICONTROL 항목 추가]</strong>.</p> </li> 
    </ol> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL 제한]</td> 
   <td> <p>각 시나리오 실행 주기 동안 모듈이 작업할 최대 자산 수를 입력하거나 매핑합니다.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL 자산 메타데이터 업데이트]

이 작업 모듈은 자산의 메타데이터 필드를 업데이트합니다.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td> 
  <td> <p>연결 방법에 대한 지침은 [!DNL Widen] 계정 대상 [!DNL Workfront Fusion]를 참조하십시오. <a href="#connect-widen-to-workfront-fusion" class="MCXref xref">Connect [!DNL Widen] to [!DNL Workfront Fusion] </a> 참조하십시오.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Asset ID]</td> 
   <td> <p>메타데이터를 업데이트할 자산의 ID를 입력하거나 매핑합니다.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL 메타데이터 유형]</td> 
   <td> <p>업데이트할 메타데이터의 메타데이터 유형을 선택합니다.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Metadata]</td> 
   <td>업데이트할 메타데이터 필드를 선택합니다. 각 필드에 필드의 새 값을 입력합니다.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL 제한]</td> 
   <td> <p>각 시나리오 실행 주기 동안 모듈이 작업할 최대 자산 수를 입력하거나 매핑합니다.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL 파일 다운로드]

이 작업 모듈은 [!DNL Widen] 계정이 필요합니다.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td> 
  <td> <p>연결 방법에 대한 지침은 [!DNL Widen] 계정 대상 [!DNL Workfront Fusion]를 참조하십시오. <a href="#connect-widen-to-workfront-fusion" class="MCXref xref">Connect [!DNL Widen] to [!DNL Workfront Fusion] </a> 참조하십시오.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Asset ID]</td> 
   <td> <p>다운로드할 자산의 ID를 입력하거나 매핑합니다.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL 파일 업로드]

이 작업 모듈은 파일을 [!DNL Widen] 계정이 필요합니다.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td> 
  <td> <p>연결 방법에 대한 지침은 [!DNL Widen] 계정 대상 [!DNL Workfront Fusion]를 참조하십시오. <a href="#connect-widen-to-workfront-fusion" class="MCXref xref">Connect [!DNL Widen] to [!DNL Workfront Fusion] </a> 참조하십시오.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Upload Profile]</td> 
   <td> <p>모듈에서 사용할 업로드 프로필을 선택합니다.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Upload Method]</td> 
   <td> <p>파일을 업로드할 방법을 선택합니다.</p> 
    <ul> 
     <li> <p><strong>[!UICONTROL From File]</strong> </p> <p>이전 모듈에서 소스 파일을 선택하거나 매핑합니다.</p> </li> 
     <li> <p><strong>[!UICONTROL By URL]</strong> </p> <p>업로드할 파일의 URL을 입력하거나 매핑합니다.</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL 파일 이름]</td> 
   <td>업로드된 파일의 이름을 입력하거나 매핑합니다.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL 메타데이터 유형]</td> 
   <td>업로드할 파일의 메타데이터 유형을 선택합니다.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Metadata]</td> 
   <td>파일 업로드에 포함할 메타데이터 필드를 선택합니다. 각 필드에 필드의 [!UICONTROL 값]을 입력합니다.</td> 
  </tr> 
 </tbody> 
</table>

### 검색 모듈

* [[!UICONTROL 컬렉션 자산 읽기]](#read-collection-assets)
* [[!UICONTROL 자산 검색]](#search-assets)

#### [!UICONTROL 컬렉션 자산 읽기]

이 작업 모듈은 컬렉션 내의 자산 목록을 검색합니다.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td> 
  <td> <p>연결 방법에 대한 지침은 [!DNL Widen] 계정 대상 [!DNL Workfront Fusion]를 참조하십시오. <a href="#connect-widen-to-workfront-fusion" class="MCXref xref">Connect [!DNL Widen] to [!DNL Workfront Fusion] </a> 참조하십시오.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Collection ID]</td> 
   <td> <p>읽을 자산이 들어 있는 컬렉션의 ID를 입력하거나 매핑합니다.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL 시작]</td> 
   <td>나열할 첫 번째 항목의 번호를 입력하거나 매핑합니다. 레코드 페이지를 매기는 방법입니다.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Max]</td> 
   <td> <p>각 시나리오 실행 주기 동안 모듈이 반환할 최대 레코드 수를 입력하거나 매핑합니다.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL 정렬 기준]</td> 
   <td> <p>자산을 정렬할 속성을 선택합니다. </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Order]</td> 
   <td>자산을 오름차순으로 정렬할지 또는 내림차순으로 정렬할지 선택합니다.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL 출력]</td> 
   <td>모듈 출력에 포함할 필드를 선택합니다.</td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL 자산 검색]

이 검색 모듈은 특정 검색 기준과 일치하는 자산 목록을 검색합니다.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td> 
  <td> <p>연결 방법에 대한 지침은 [!DNL Widen] 계정 대상 [!DNL Workfront Fusion]를 참조하십시오. <a href="#connect-widen-to-workfront-fusion" class="MCXref xref">Connect [!DNL Widen] to [!DNL Workfront Fusion] </a> 참조하십시오.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Search Query]</td> 
   <td> <p>자산을 검색할 기준을 입력합니다.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL 정렬 기준]</td> 
   <td> <p>자산을 정렬할 방법을 선택합니다. </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Order]</td> 
   <td>자산을 오름차순으로 정렬할지 또는 내림차순으로 정렬할지 선택합니다.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL 삭제됨 포함]</td> 
   <td>검색에 삭제된 자산을 포함하려면 이 옵션을 활성화합니다.</td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL 보관된 항목 포함]</p> </td> 
   <td> <p>검색에 보관된 자산을 포함하려면 이 옵션을 활성화합니다.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL 검색 문서 텍스트]</td> 
   <td>검색에 문서 텍스트를 포함하려면 이 옵션을 활성화하거나, 검색 조건과 일치하는 자산만 포함하려면 false를 사용합니다.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL 제한]</td> 
   <td> <p>각 시나리오 실행 주기 동안 모듈이 반환할 최대 레코드 수를 입력하거나 매핑합니다.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Offset]</td> 
   <td>상세내역을 검색할 첫 번째 항목의 번호를 입력하거나 매핑합니다. 레코드 페이지를 매기는 방법입니다.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Scroll]</td> 
   <td>스크롤을 허용하려면 이 옵션을 활성화하십시오.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Expand]</td> 
   <td> <p>자산 필드 외에 모듈 출력에 포함할 속성을 선택합니다.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL 출력]</td> 
   <td>모듈 출력에 포함할 필드를 선택합니다.</td> 
  </tr> 
 </tbody> 
</table>
