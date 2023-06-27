---
content-type: reference
product-previous: workfront-fusion
product-area: workfront-integrations
keywords: 커넥터
navigation-topic: apps-and-their-modules
title: Split.io 모듈
description: 다음에서 [!DNL Adobe Workfront Fusion] 시나리오에서는 다음을 사용하는 워크플로를 자동화할 수 있습니다 [!DNL Split.io]을 여러 타사 응용 프로그램 및 서비스에 연결할 수 있습니다.
author: Becky
feature: Workfront Fusion
exl-id: 4576a2e4-b495-430e-a9de-4e1ec7379ab8
source-git-commit: 0915dcce45b271ee18cdd8af5db4f0eb01f3cced
workflow-type: tm+mt
source-wordcount: '1821'
ht-degree: 0%

---

# [!DNL Split.io] 모듈

다음에서 [!DNL Adobe Workfront Fusion] 시나리오에서는 다음을 사용하는 워크플로를 자동화할 수 있습니다 [!DNL Split.io]을 여러 타사 응용 프로그램 및 서비스에 연결할 수 있습니다.

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

사용 [!DNL Split.io] 모듈, 다음이 있어야 합니다. [!DNL Split.io] 계정입니다.

## 연결 [!DNL Split.io] 끝 [!DNL Workfront Fusion] {#connect-split-io-to-workfront-fusion}

에 대한 연결을 만들 수 있습니다. [!DNL Split.io] 내에서 직접 계정 [!DNL Split.io] 모듈.

1. 다음 중 하나 [!DNL Split.io] 모듈, 클릭 **[!UICONTROL 추가]** 다음 옆에 [!UICONTROL 연결] 필드.
1. 연결의 이름을 입력합니다.
1. 다음을 입력하십시오. [!DNL Split.io] API 키.

   에 대한 자세한 내용 [!DNL Split.io] API 키, 참조 [API 키](https://help.split.io/hc/en-us/articles/360019916211-API-keys) 다음에서 [!DNL Split.io] 설명서를 참조하십시오.

1. 클릭 **[!UICONTROL 계속]** 를 클릭하여 연결을 만들고 모듈로 돌아갑니다.

## [!DNL Split.io] 모듈 및 해당 필드

를 구성할 때 [!DNL split.io] 모듈, [!DNL Workfront Fusion] 아래 나열된 필드를 표시합니다. 이와 함께 추가 [!DNL split.io] 앱이나 서비스의 액세스 수준 등에 따라 필드가 표시될 수 있습니다. 모듈의 굵은 제목은 필수 필드를 나타냅니다.

필드나 함수 위에 맵 단추가 표시되면 이 단추를 사용하여 해당 필드에 대한 변수와 함수를 설정할 수 있습니다. 자세한 내용은 [의 한 모듈에서 다른 모듈로 정보 매핑 [!DNL Adobe Workfront Fusion]](../../workfront-fusion/mapping/map-information-between-modules.md).

![](assets/map-toggle-350x74.png)

* [액션](#actions)
* [검색 결과](#searches)

### 액션

* [[!UICONTROL 사용자 정의 API 호출]](#custom-api-call)
* [[!UICONTROL 분할 가져오기]](#get-split)
* [[!UICONTROL 환경에서 분할 정의 가져오기]](#get-split-definition-in-environment)
* [[!UICONTROL 분할 만들기]](#create-split)
* [[!UICONTROL 분할 삭제]](#delete-split)
* [[!UICONTROL 환경에서 분할 정의 만들기]](#create-split-definition-in-environment)
* [[!UICONTROL 환경에서 분할 정의 제거]](#remove-split-definition-from-environment)
* [[!UICONTROL 환경의 분할 정의 부분 업데이트]](#partial-update-split-definition-in-environment)
* [[!UICONTROL 태그 연결]](#associate-tags)

#### [!UICONTROL 사용자 정의 API 호출]

이 작업 모듈에서는 다음을 위한 사용자 지정 인증 호출을 만들 수 있습니다. [!DNL split.io] API. 이렇게 하면 다른 사용자가 수행할 수 없는 데이터 흐름 자동화를 만들 수 있습니다 [!DNL split.io] 모듈.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td> 
   <td> <p>연결에 대한 자세한 내용 [!DNL Split.io] 계정 위치: [!DNL Workfront Fusion], 참조 <a href="#connect-split-io-to-workfront-fusion" class="MCXref xref">연결 [!DNL Split.io] [!UICONTROL Workfront Fusion]으로 </a> 이 문서에서.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL URL]</td> 
   <td>상대 경로 입력 <code>https://api.split.io/internal/api/v2/</code>.</td> 
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
  <tr> 
   <td role="rowheader">[!UICONTROL 제한]</td> 
   <td>각 시나리오 실행 주기 동안 모듈이 사용할 최대 레코드 수를 입력하거나 매핑합니다.</td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL 분할 가져오기]

이 작업 모듈은 분할을 검색합니다.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td> 
   <td> <p>연결에 대한 자세한 내용 [!DNL Split.io] 계정 위치: [!DNL Workfront Fusion], 참조 <a href="#connect-split-io-to-workfront-fusion" class="MCXref xref">연결 [!DNL Split.io] [!UICONTROL Workfront Fusion]으로 </a> 이 문서에서.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL 작업 공간 ID]</td> 
   <td>검색할 분할이 포함된 작업공간을 선택하거나 매핑합니다.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL 분할 이름]</td> 
   <td> <p>검색할 분할 이름을 입력하거나 매핑합니다.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL 환경에서 분할 정의 가져오기]

이 작업 모듈은 지정된 환경에서 특정 분할 정의를 검색합니다.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td> 
   <td> <p>연결에 대한 자세한 내용 [!DNL Split.io] 계정 위치: [!DNL Workfront Fusion], 참조 <a href="#connect-split-io-to-workfront-fusion" class="MCXref xref">연결 [!DNL Split.io] [!UICONTROL Workfront Fusion]으로 </a> 이 문서에서.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL 작업 공간 ID]</td> 
   <td>검색할 분할 정의가 포함된 작업공간을 선택하거나 매핑합니다.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL 환경 이름 또는 ID]</td> 
   <td>검색할 분할 정의가 포함된 환경을 선택하거나 매핑합니다.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL 분할 이름]</td> 
   <td> <p>분할 정의를 검색할 분할 이름을 입력하거나 매핑합니다.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL 분할 만들기]

이 작업 모듈은 트래픽 유형이 지정된 경우 조직에서 새 분할을 생성합니다.

>[!NOTE]
>
>API는 어떤 환경에서도 분할을 구성하지 않습니다.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td> 
   <td> <p>연결에 대한 자세한 내용 [!DNL Split.io] 계정 위치: [!DNL Workfront Fusion], 참조 <a href="#connect-split-io-to-workfront-fusion" class="MCXref xref">연결 [!DNL Split.io] [!UICONTROL Workfront Fusion]으로 </a> 이 문서에서.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL 작업 공간 ID]</td> 
   <td>분할을 생성할 작업공간을 선택하거나 매핑합니다.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL 트래픽 유형 ID 또는 이름]</td> 
   <td>분할을 만드는 데 사용할 트래픽 유형을 선택하거나 매핑합니다.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL 분할 이름]</td> 
   <td> <p>생성할 분할의 이름을 입력하거나 매핑합니다.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL 분할 설명]</td> 
   <td>만들려는 분할에 대한 [!UICONTROL 분할] 설명을 입력하거나 매핑합니다.</td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL 분할 삭제]

이 작업 모듈은 조직에서 분할을 삭제합니다. 이렇게 하면 모든 환경에서 분할 정의를 자동으로 구성 해제합니다.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td> 
   <td> <p>연결에 대한 자세한 내용 [!DNL Split.io] 계정 위치: [!DNL Workfront Fusion], 참조 <a href="#connect-split-io-to-workfront-fusion" class="MCXref xref">연결 [!DNL Split.io] [!UICONTROL Workfront Fusion]으로 </a> 이 문서에서.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL 작업 공간 ID]</td> 
   <td>분할을 삭제할 작업공간을 선택하거나 매핑합니다.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL 분할 이름]</td> 
   <td> <p>삭제할 분할 이름을 입력하거나 매핑합니다.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL 환경에서 분할 정의 만들기]

이 작업 모듈은 특정 환경에 대한 분할 정의를 구성합니다.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td> 
   <td> <p>연결에 대한 자세한 내용 [!DNL Split.io] 계정 위치: [!DNL Workfront Fusion], 참조 <a href="#connect-split-io-to-workfront-fusion" class="MCXref xref">연결 [!DNL Split.io] [!UICONTROL Workfront Fusion]으로 </a> 이 문서에서.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL 작업 공간 ID]</td> 
   <td>분할 정의를 생성할 작업공간을 선택하거나 매핑합니다.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL 환경 이름 또는 ID]</td> 
   <td>분할 정의를 생성할 환경을 선택하거나 매핑합니다.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL 분할 이름]</td> 
   <td> <p>정의를 생성할 분할의 이름을 입력하거나 매핑합니다.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Comments]</td> 
   <td>분할 정의에 추가할 주석을 입력하거나 매핑합니다.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL 규칙]</td> 
   <td> <p>정의에 추가하려는 각 타겟팅 규칙에 대해 다음을 클릭하십시오. <b>[!UICONTROL 항목 추가]</b>를 클릭한 다음 규칙을 입력하거나 매핑합니다.</p> <p>타깃팅 규칙에 대한 자세한 내용은 <a href="https://docs.split.io/reference#create-split-definition-in-environment">환경에서 분할 정의 만들기</a> 다음에서 [!DNL Split.io] 설명서를 참조하십시오.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL 기본 규칙]</td> 
   <td> <p>다른 규칙의 사양을 충족하지 않는 트래픽에 대해 분할에서 사용할 규칙을 입력하거나 매핑합니다.</p> <p>타깃팅 규칙에 대한 자세한 내용은 <a href="https://docs.split.io/reference#create-split-definition-in-environment">환경에서 분할 정의 만들기</a> 다음에서 [!DNL Split.io] 설명서를 참조하십시오.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL 기본 처리]</td> 
   <td> <p>분할이 종료되거나 고객이 트래픽 할당에 포함되지 않은 경우 분할에서 사용할 처리를 입력하거나 매핑합니다.</p> <p>치료에 대한 자세한 내용은 <a href="https://docs.split.io/reference#create-split-definition-in-environment">환경에서 분할 정의 만들기</a> 다음에서 [!DNL Split.io] 설명서를 참조하십시오.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Treatments]</td> 
   <td> <p>정의에 추가할 각 처리에 대해 다음을 클릭합니다. <b>[!UICONTROL 항목 추가]</b>를 클릭한 다음 처리를 입력하거나 매핑합니다.</p> <p>치료에 대한 자세한 내용은 <a href="https://docs.split.io/reference#create-split-definition-in-environment">환경에서 분할 정의 만들기</a> 다음에서 [!DNL Split.io] 설명서를 참조하십시오.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL 환경에서 분할 정의 제거]

이 작업 모듈은 특정 환경에 대한 분할 정의의 구성을 해제합니다.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td> 
   <td> <p>연결에 대한 자세한 내용 [!DNL Split.io] 계정 위치: [!DNL Workfront Fusion], 참조 <a href="#connect-split-io-to-workfront-fusion" class="MCXref xref">연결 [!DNL Split.io] [!UICONTROL Workfront Fusion]으로 </a> 이 문서에서.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL 작업 공간 ID]</td> 
   <td>분할 정의를 제거할 작업공간을 선택하거나 매핑합니다.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL 환경 이름 또는 ID]</td> 
   <td>분할 정의를 제거할 환경을 선택하거나 매핑합니다.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL 분할 이름]</td> 
   <td> <p>정의를 제거할 분할의 이름을 입력하거나 매핑합니다.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Comments]</td> 
   <td>분할 정의에 추가할 주석을 입력하거나 매핑합니다.</td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL 환경의 분할 정의 부분 업데이트]

이 작업 모듈은 특정 환경에 대한 분할 정의를 업데이트합니다.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td> 
   <td> <p>연결에 대한 자세한 내용 [!DNL Split.io] 계정 위치: [!DNL Workfront Fusion], 참조 <a href="#connect-split-io-to-workfront-fusion" class="MCXref xref">연결 [!DNL Split.io] [!UICONTROL Workfront Fusion]으로 </a> 이 문서에서.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL 작업 공간 ID]</td> 
   <td>분할 정의를 업데이트할 작업공간을 선택하거나 매핑합니다.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL 환경 이름 또는 ID]</td> 
   <td>분할 정의를 업데이트할 환경을 선택하거나 매핑합니다.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL 분할 이름]</td> 
   <td> <p>정의를 갱신할 분할의 이름을 입력하거나 매핑합니다.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL 콘텐츠 업데이트]</td> 
   <td> <p>업데이트할 분할의 각 속성에 대해 <b>[!UICONTROL 항목 추가]</b> 원하는 변경 내용을 입력하거나 매핑합니다.</p> <p>자세한 내용은 <a href="https://docs.split.io/reference#partial-update-split-definition-in-environment">환경의 분할 정의 부분 업데이트</a> 다음에서 [!DNL Split.io] 설명서를 참조하십시오.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Comments]</td> 
   <td>분할 정의에 추가할 주석을 입력하거나 매핑합니다.</td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL 태그 연결]

이 작업 모듈은 지정된 개체에 태그를 추가합니다.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td> 
   <td> <p>연결에 대한 자세한 내용 [!DNL Split.io] 계정 위치: [!DNL Workfront Fusion], 참조 <a href="#connect-split-io-to-workfront-fusion" class="MCXref xref">연결 [!DNL Split.io] [!UICONTROL Workfront Fusion]으로 </a> 이 문서에서.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL 작업 공간 ID]</td> 
   <td>태그를 추가할 작업 영역을 선택하거나 매핑합니다.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL 개체 이름]</td> 
   <td>태그를 추가할 개체의 이름을 입력하거나 매핑합니다.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL 개체 유형]</td> 
   <td> <p>태그를 추가할 개체 유형을 입력하거나 매핑합니다.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL 태그]</td> 
   <td> <p>추가할 각 태그에 대해 <b>[!UICONTROL 항목 추가]</b> 태그를 입력하거나 매핑합니다.</p> </td> 
  </tr> 
 </tbody> 
</table>

### 검색 결과

* [[!UICONTROL 작업 공간 가져오기]](#get-workspaces)
* [[!UICONTROL 환경 가져오기]](#get-environments)
* [[!UICONTROL 분할 가져오기]](#get-splits)
* [[!UICONTROL 환경의 목록 분할 정의]](#list-split-definitions-in-an-environment)
* [[!UICONTROL 트래픽 유형 가져오기]](#get-traffic-types)

#### [!UICONTROL 작업 공간 가져오기]

이 검색 모듈은 조직의 작업 공간을 검색합니다.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td> 
   <td> <p>연결에 대한 자세한 내용 [!DNL Split.io] 계정 위치: [!DNL Workfront Fusion], 참조 <a href="#connect-split-io-to-workfront-fusion" class="MCXref xref">연결 [!DNL Split.io] [!UICONTROL Workfront Fusion]으로 </a> 이 문서에서.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL 제한]</td> 
   <td>각 시나리오 실행 주기 동안 모듈이 검색할 최대 작업 공간 수를 입력하거나 매핑합니다.</td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL 환경 가져오기]

이 검색 모듈은 환경 목록을 검색합니다.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td> 
   <td> <p>연결에 대한 자세한 내용 [!DNL Split.io] 계정 위치: [!DNL Workfront Fusion], 참조 <a href="#connect-split-io-to-workfront-fusion" class="MCXref xref">연결 [!DNL Split.io] [!UICONTROL Workfront Fusion]으로 </a> 이 문서에서.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL 작업 공간 ID]</td> 
   <td>나열할 환경이 포함된 작업 영역을 선택하거나 매핑합니다.</td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL 분할 가져오기]

이 검색 모듈은 분할 목록을 검색합니다.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td> 
   <td> <p>연결에 대한 자세한 내용 [!DNL Split.io] 계정 위치: [!DNL Workfront Fusion], 참조 <a href="#connect-split-io-to-workfront-fusion" class="MCXref xref">연결 [!DNL Split.io] [!UICONTROL Workfront Fusion]으로 </a> 이 문서에서.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL 작업 공간 ID]</td> 
   <td>나열할 분할이 포함된 작업공간을 선택하거나 매핑합니다.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL 제한]</td> 
   <td>각 시나리오 실행 주기 동안 모듈이 검색할 최대 분할 수를 입력하거나 매핑합니다.</td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL 환경의 목록 분할 정의]

이 검색 모듈은 주어진 환경에서 분할 정의 목록을 검색합니다.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td> 
   <td> <p>연결에 대한 자세한 내용 [!DNL Split.io] 계정 위치: [!DNL Workfront Fusion], 참조 <a href="#connect-split-io-to-workfront-fusion" class="MCXref xref">연결 [!DNL Split.io] [!UICONTROL Workfront Fusion]으로 </a> 이 문서에서.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL 작업 공간 ID]</td> 
   <td>나열할 분할 정의가 포함된 작업공간을 선택하거나 매핑합니다.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL 환경 이름 또는 ID]</td> 
   <td>나열할 분할 정의가 포함된 환경을 선택하거나 매핑합니다.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL 제한]</td> 
   <td>각 시나리오 실행 주기 동안 모듈이 검색할 분할 정의의 최대 수를 입력하거나 매핑합니다.</td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL 트래픽 유형 가져오기]

이 검색 모듈은 트래픽 유형 목록을 검색합니다.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td> 
   <td> <p>연결에 대한 자세한 내용 [!DNL Split.io] 계정 위치: [!DNL Workfront Fusion], 참조 <a href="#connect-split-io-to-workfront-fusion" class="MCXref xref">연결 [!DNL Split.io] [!UICONTROL Workfront Fusion]으로 </a> 이 문서에서.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL 작업 공간 ID]</td> 
   <td>나열할 트래픽 유형이 포함된 작업 영역을 선택하거나 매핑합니다.</td> 
  </tr> 
 </tbody> 
</table>
