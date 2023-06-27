---
title: 모듈 확장
description: 다음에서 [!DNL Adobe Workfront Fusion] 시나리오에서는 다음을 사용하는 워크플로를 자동화할 수 있습니다 [!UICONTROL 확장]을 여러 타사 응용 프로그램 및 서비스에 연결할 수 있습니다.
author: Becky
draft: Probably
feature: Workfront Fusion
exl-id: d46935bc-4f6c-4502-bd2f-3927f33241e1
source-git-commit: 0915dcce45b271ee18cdd8af5db4f0eb01f3cced
workflow-type: tm+mt
source-wordcount: '1586'
ht-degree: 1%

---

# [!DNL Widen] 모듈

다음에서 [!DNL Adobe Workfront Fusion] 시나리오에서는 다음을 사용하는 워크플로를 자동화할 수 있습니다 [!UICONTROL 확장]을 여러 타사 응용 프로그램 및 서비스에 연결할 수 있습니다.

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

사용 [!UICONTROL 확장] 모듈, 다음이 있어야 합니다. [!UICONTROL 확장] 계정입니다.

## 연결 [!DNL Widen] 끝 [!DNL Workfront Fusion] {#connect-widen-to-workfront-fusion}

에 대한 연결을 만들 수 있습니다. [!DNL Widen] 내에서 직접 계정 [!DNL Widen] 모듈.

1. 다음 중 하나 [!DNL Widen] 모듈, 클릭 **[!UICONTROL 추가]** 다음 옆에 [!UICONTROL 연결] 필드.
1. 다음 항목 선택 [!DNL Widen] 연결할 도메인입니다.
1. 에 대한 토큰 입력 [!DNL Widen] 계정입니다. 이 토큰을 찾는 방법에 대한 지침은 [[!DNL Widen] API FAQ](https://community.widen.com/collective/s/article/API-FAQs).
1. 클릭 **[!UICONTROL 계속]** 를 클릭하여 연결을 만들고 모듈로 돌아갑니다.

## [!DNL Widen] 모듈 및 해당 필드

를 구성할 때 [!DNL Widen] 모듈, [!DNL Workfront Fusion] 아래 나열된 필드를 표시합니다. 이와 함께 추가 [!DNL Widen] 앱이나 서비스의 액세스 수준 등에 따라 필드가 표시될 수 있습니다. 모듈의 굵은 제목은 필수 필드를 나타냅니다.

필드나 함수 위에 맵 단추가 표시되면 이 단추를 사용하여 해당 필드에 대한 변수와 함수를 설정할 수 있습니다. 자세한 내용은 [의 한 모듈에서 다른 모듈로 정보 매핑 [!DNL Adobe Workfront Fusion]](../../workfront-fusion/mapping/map-information-between-modules.md).

![](assets/map-toggle-350x74.png)

* [트리거 모듈](#trigger-modules)
* [작업 모듈](#action-modules)
* [모듈 검색](#search-modules)

### 트리거 모듈

#### [!UICONTROL 자산 보기]

이 트리거 모듈은 자산이 생성되거나 업데이트될 때 시나리오를 시작합니다.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td> 
  <td> <p>연결에 대한 자세한 내용 [!DNL Widen] 계정 위치: [!DNL Workfront Fusion], 참조 <a href="#connect-widen-to-workfront-fusion" class="MCXref xref">연결 [!DNL Widen] 끝 [!DNL Workfront Fusion] </a> 이 문서에서.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL 이벤트 유형]</td> 
   <td> <p>새 에셋 또는 업데이트된 에셋을 시청할지 여부를 선택합니다.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Expand]</td> 
   <td> <p>에셋 필드 외에 모듈 출력에 포함할 속성을 선택합니다.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL 출력]</td> 
   <td>모듈 출력에 포함할 필드를 선택합니다.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL 제한]</td> 
   <td> <p>각 시나리오 실행 주기 동안 모듈이 사용할 최대 자산 수를 입력하거나 매핑합니다.</p> </td> 
  </tr> 
 </tbody> 
</table>

### 작업 모듈

* [[!UICONTROL 사용자 정의 API 호출]](#custom-api-call)
* [[!UICONTROL 에셋 정보 읽기]](#read-asset-info)
* [[!UICONTROL 컬렉션에 자산 추가]](#add-assets-to-collections)
* [[!UICONTROL 컬렉션에서 에셋 제거]](#remove-assets-from-collection)
* [[!UICONTROL 자산 메타데이터 업데이트]](#update-asset-metadata)
* [[!UICONTROL 파일 다운로드]](#download-file)
* [[!UICONTROL 업로드] 파일](#upload-a-file)

#### [!UICONTROL 사용자 정의 API 호출]

이 작업 모듈에서는 다음을 위한 사용자 지정 인증 호출을 만들 수 있습니다. [!DNL Widen] API. 이렇게 하면 다른 사용자가 수행할 수 없는 데이터 흐름 자동화를 만들 수 있습니다 [!DNL Widen] 모듈.

이 모듈을 구성할 때 다음 필드가 표시됩니다.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td> 
   <td> <p>연결에 대한 자세한 내용 [!DNL Widen] 계정 위치: [!DNL Workfront Fusion], 참조 <a href="#connect-widen-to-workfront-fusion" class="MCXref xref">연결 [!DNL Widen] 끝 [!DNL Workfront Fusion] </a> 이 문서에서.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL API Version]</td> 
   <td>최신 버전의 를 사용할지 여부를 선택합니다. [!DNL Widen] API 또는 버전 1.0</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL URL]</td> 
   <td>API 호출에 대한 URL을 입력하거나 매핑합니다.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL 메서드]</td> 
   <td> <p>API 호출을 구성하는 데 필요한 HTTP 요청 메서드를 선택합니다. 자세한 내용은 <a href="../../workfront-fusion/modules/http-request-methods.md" class="MCXref xref">의 HTTP 요청 메서드 [!DNL Adobe Workfront Fusion]</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Headers]</td> 
   <td> <p>표준 JSON 개체 형태로 요청의 헤더를 추가합니다.</p> <p>For example, <code>{"Content-type":"application/json"}</code></p> <p>[!UICONTROL Workfront Fusion]이 사용자에게 권한 부여 헤더를 추가합니다.</p> </td> 
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

#### [!UICONTROL 에셋 정보 읽기]

이 작업 모듈은 고유 ID로 개별 자산을 검색합니다.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td> 
  <td> <p>연결에 대한 자세한 내용 [!DNL Widen] 계정 위치: [!DNL Workfront Fusion], 참조 <a href="#connect-widen-to-workfront-fusion" class="MCXref xref">연결 [!DNL Widen] 끝 [!DNL Workfront Fusion] </a> 이 문서에서.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL 자산 ID]</td> 
   <td> <p>정보를 읽을 자산의 ID를 입력하거나 매핑합니다.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Expand]</td> 
   <td> <p>에셋 필드 외에 모듈 출력에 포함할 속성을 선택합니다.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL 출력]</td> 
   <td>모듈 출력에 포함할 필드를 선택합니다.</td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL 컬렉션에 자산 추가]

이 작업 모듈은 컬렉션에 하나 이상의 에셋을 추가합니다.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td> 
  <td> <p>연결에 대한 자세한 내용 [!DNL Widen] 계정 위치: [!DNL Workfront Fusion], 참조 <a href="#connect-widen-to-workfront-fusion" class="MCXref xref">연결 [!DNL Widen] 끝 [!DNL Workfront Fusion] </a> 이 문서에서.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL 컬렉션 ID]</td> 
   <td> <p>에셋을 추가할 각 컬렉션에 대해:</p> 
    <ol> 
     <li value="1"> <p> 클릭 <strong>[!UICONTROL 추가]</strong>.</p> </li> 
     <li value="2"> <p>[!UICONTROL 컬렉션 ID]를 입력하거나 매핑합니다.</p> </li> 
     <li value="3"> <p>클릭 <strong>[!UICONTROL 항목 추가]</strong>.</p> </li> 
    </ol> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL 자산 ID]</td> 
   <td> <p>컬렉션에 추가할 각 에셋에 대해 다음 작업을 수행하십시오.</p> 
    <ol> 
     <li value="1"> <p> 클릭 <strong>[!UICONTROL 추가]</strong>.</p> </li> 
     <li value="2"> <p>자산 ID를 입력하거나 매핑합니다.</p> </li> 
     <li value="3"> <p>클릭 <strong>[!UICONTROL 항목 추가]</strong>.</p> </li> 
    </ol> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL 제한]</td> 
   <td> <p>각 시나리오 실행 주기 동안 모듈이 사용할 최대 자산 수를 입력하거나 매핑합니다.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL 컬렉션에서 에셋 제거]

이 작업 모듈은 컬렉션에서 하나 이상의 자산을 제거합니다.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td> 
  <td> <p>연결에 대한 자세한 내용 [!DNL Widen] 계정 위치: [!DNL Workfront Fusion], 참조 <a href="#connect-widen-to-workfront-fusion" class="MCXref xref">연결 [!DNL Widen] 끝 [!DNL Workfront Fusion] </a> 이 문서에서.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL 컬렉션 ID]</td> 
   <td> <p>에서 에셋을 제거할 각 컬렉션에 대해:</p> 
    <ol> 
     <li value="1"> <p> 클릭 <strong>[!UICONTROL 추가]</strong>.</p> </li> 
     <li value="2"> <p>컬렉션 ID를 입력하거나 매핑합니다.</p> </li> 
     <li value="3"> <p>클릭 <strong>[!UICONTROL 항목 추가]</strong>.</p> </li> 
    </ol> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">자산 ID</td> 
   <td> <p>컬렉션에서 제거할 각 에셋에 대해 다음 작업을 수행하십시오.</p> 
    <ol> 
     <li value="1"> <p> 클릭 <strong>[!UICONTROL 추가]</strong>.</p> </li> 
     <li value="2"> <p>자산 ID를 입력하거나 매핑합니다.</p> </li> 
     <li value="3"> <p>클릭 <strong>[!UICONTROL 항목 추가]</strong>.</p> </li> 
    </ol> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL 제한]</td> 
   <td> <p>각 시나리오 실행 주기 동안 모듈이 사용할 최대 자산 수를 입력하거나 매핑합니다.</p> </td> 
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
  <td> <p>연결에 대한 자세한 내용 [!DNL Widen] 계정 위치: [!DNL Workfront Fusion], 참조 <a href="#connect-widen-to-workfront-fusion" class="MCXref xref">연결 [!DNL Widen] 끝 [!DNL Workfront Fusion] </a> 이 문서에서.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL 자산 ID]</td> 
   <td> <p>메타데이터를 업데이트할 에셋의 ID를 입력하거나 매핑합니다.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL 메타데이터 유형]</td> 
   <td> <p>업데이트할 메타데이터의 메타데이터 유형을 선택합니다.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL 메타데이터]</td> 
   <td>업데이트할 메타데이터 필드를 선택합니다. 각 필드에 대해 새 필드 값을 입력합니다.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL 제한]</td> 
   <td> <p>각 시나리오 실행 주기 동안 모듈이 사용할 최대 자산 수를 입력하거나 매핑합니다.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL 파일 다운로드]

이 작업 모듈은 에서 자산을 다운로드합니다. [!DNL Widen] 계정입니다.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td> 
  <td> <p>연결에 대한 자세한 내용 [!DNL Widen] 계정 위치: [!DNL Workfront Fusion], 참조 <a href="#connect-widen-to-workfront-fusion" class="MCXref xref">연결 [!DNL Widen] 끝 [!DNL Workfront Fusion] </a> 이 문서에서.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL 자산 ID]</td> 
   <td> <p>다운로드하려는 에셋의 ID를 입력하거나 매핑합니다.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL 파일 업로드]

이 작업 모듈은 파일을 [!DNL Widen] 계정입니다.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td> 
  <td> <p>연결에 대한 자세한 내용 [!DNL Widen] 계정 위치: [!DNL Workfront Fusion], 참조 <a href="#connect-widen-to-workfront-fusion" class="MCXref xref">연결 [!DNL Widen] 끝 [!DNL Workfront Fusion] </a> 이 문서에서.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL 업로드 프로필]</td> 
   <td> <p>모듈에서 사용할 업로드 프로필을 선택합니다.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL 업로드 메서드]</td> 
   <td> <p>파일 업로드 방법을 선택합니다.</p> 
    <ul> 
     <li> <p><strong>[!UICONTROL From File]</strong> </p> <p>이전 모듈에서 소스 파일을 선택하거나 매핑합니다.</p> </li> 
     <li> <p><strong>URL별 [!UICONTROL]</strong> </p> <p>업로드할 파일의 URL을 입력하거나 매핑합니다.</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL 파일 이름]</td> 
   <td>업로드한 파일의 이름을 입력하거나 매핑합니다.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL 메타데이터 유형]</td> 
   <td>업로드할 파일의 메타데이터 유형을 선택합니다.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL 메타데이터]</td> 
   <td>파일 업로드에 포함할 메타데이터 필드를 선택합니다. 각 필드에 대해 필드에 대한 [!UICONTROL 값]을 입력합니다.</td> 
  </tr> 
 </tbody> 
</table>

### 모듈 검색

* [[!UICONTROL 컬렉션 자산 읽기]](#read-collection-assets)
* [[!UICONTROL 에셋 검색]](#search-assets)

#### [!UICONTROL 컬렉션 자산 읽기]

이 작업 모듈은 컬렉션 내의 자산 목록을 검색합니다.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td> 
  <td> <p>연결에 대한 자세한 내용 [!DNL Widen] 계정 위치: [!DNL Workfront Fusion], 참조 <a href="#connect-widen-to-workfront-fusion" class="MCXref xref">연결 [!DNL Widen] 끝 [!DNL Workfront Fusion] </a> 이 문서에서.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL 컬렉션 ID]</td> 
   <td> <p>읽을 자산을 포함하는 컬렉션의 ID를 입력하거나 매핑합니다.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL 시작]</td> 
   <td>나열할 첫 번째 항목의 번호를 입력하거나 매핑합니다. 이것은 레코드에 페이지를 매기는 방법입니다.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Max]</td> 
   <td> <p>각 시나리오 실행 주기 동안 모듈이 반환할 최대 레코드 수를 입력하거나 매핑합니다.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL 정렬 기준]</td> 
   <td> <p>에셋을 정렬할 속성을 선택합니다. </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Order]</td> 
   <td>에셋을 오름차순으로 정렬할지 아니면 내림차순으로 정렬할지 선택합니다.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL 출력]</td> 
   <td>모듈 출력에 포함할 필드를 선택합니다.</td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL 에셋 검색]

이 검색 모듈은 특정 검색 기준과 일치하는 에셋 목록을 검색합니다.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td> 
  <td> <p>연결에 대한 자세한 내용 [!DNL Widen] 계정 위치: [!DNL Workfront Fusion], 참조 <a href="#connect-widen-to-workfront-fusion" class="MCXref xref">연결 [!DNL Widen] 끝 [!DNL Workfront Fusion] </a> 이 문서에서.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL 검색 쿼리]</td> 
   <td> <p>에셋을 검색할 기준을 입력합니다.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL 정렬 기준]</td> 
   <td> <p>에셋을 정렬할 방법을 선택합니다. </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Order]</td> 
   <td>에셋을 오름차순으로 정렬할지 아니면 내림차순으로 정렬할지 선택합니다.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Include deleted]</td> 
   <td>삭제된 에셋을 검색에 포함하려면 이 옵션을 활성화합니다.</td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Include archived]</p> </td> 
   <td> <p>보관된 자산을 검색에 포함하려면 이 옵션을 활성화합니다.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL 검색 문서 텍스트]</td> 
   <td>이 옵션을 활성화하면 검색에 문서 텍스트가 포함되고, false를 활성화하면 검색 기준과 일치하는 제목이 있는 자산만 포함됩니다.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL 제한]</td> 
   <td> <p>각 시나리오 실행 주기 동안 모듈이 반환할 최대 레코드 수를 입력하거나 매핑합니다.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Offset]</td> 
   <td>세부 정보를 검색할 첫 번째 항목의 번호를 입력하거나 매핑합니다. 이것은 레코드에 페이지를 매기는 방법입니다.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Scroll]</td> 
   <td>스크롤을 허용하려면 이 옵션을 활성화합니다.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Expand]</td> 
   <td> <p>에셋 필드 외에 모듈 출력에 포함할 속성을 선택합니다.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL 출력]</td> 
   <td>모듈 출력에 포함할 필드를 선택합니다.</td> 
  </tr> 
 </tbody> 
</table>
