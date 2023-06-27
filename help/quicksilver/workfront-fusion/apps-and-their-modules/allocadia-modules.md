---
content-type: reference
product-previous: workfront-fusion
product-area: workfront-integrations
keywords: 커넥터
navigation-topic: apps-and-their-modules
title: Allocadia 모듈
description: 다음에서 [!DNL Adobe Workfront Fusion] 시나리오에서는 Allocadia를 사용하는 워크플로를 자동화할 수 있을 뿐만 아니라 여러 타사 애플리케이션 및 서비스에 연결할 수도 있습니다.
author: Becky
feature: Workfront Fusion
exl-id: f1edefd1-9fe0-48fc-bea2-c3f9facf7363
source-git-commit: a3756f9345cbc9417a6fd110306dfa50aecc81a2
workflow-type: tm+mt
source-wordcount: '1401'
ht-degree: 0%

---

# [!DNL Allocadia] 모듈

다음에서 [!DNL Adobe Workfront Fusion] 시나리오에서는 다음을 사용하는 워크플로를 자동화할 수 있습니다 [!DNL Allocadia]을 여러 타사 응용 프로그램 및 서비스에 연결할 수 있습니다.

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

사용 [!DNL Allocadia] 모듈, 다음 항목이 있어야 합니다. [!DNL Allocadia] 계정입니다.

## 연결 [!DNL Allocadia] 끝 [!DNL Workfront Fusion]

에 대한 연결을 만들 수 있습니다. [!DNL Allocadia] 내에서 직접 계정 [!DNL Allocadia] 모듈.

1. 다음 중 하나 [!DNL Allocadia] 모듈, 클릭 **[!UICONTROL 추가]** 다음 옆에 [!UICONTROL 연결] 필드.
1. 북미 서버를 사용할지 유럽 서버를 사용할지 선택합니다.
1. 사용자 이름과 암호를 입력합니다.
1. 클릭 **[!UICONTROL 계속]** 를 클릭하여 연결을 만들고 모듈로 돌아갑니다.

## [!DNL Allocadia] 모듈 및 해당 필드

를 구성할 때 [!DNL Allocadia] 모듈, [!DNL Workfront Fusion] 아래 나열된 필드를 표시합니다. 이와 함께 추가 [!DNL Allocadia] 앱이나 서비스의 액세스 수준 등에 따라 필드가 표시될 수 있습니다. 모듈의 굵은 제목은 필수 필드를 나타냅니다.

필드나 함수 위에 맵 단추가 표시되면 이 단추를 사용하여 해당 필드에 대한 변수와 함수를 설정할 수 있습니다. 자세한 내용은 [의 한 모듈에서 다른 모듈로 정보 매핑 [!DNL Adobe Workfront Fusion]](../../workfront-fusion/mapping/map-information-between-modules.md).

![](assets/map-toggle-350x74.png)

* [트리거](#triggers)
* [액션](#actions)
* [검색 결과](#searches)

### 트리거

#### [!UICONTROL 녹화 시청]

이 트리거 모듈은 특정 유형의 객체가 추가, 업데이트 또는 둘 다 될 때 시나리오를 실행합니다. 모듈은 연결에서 액세스하는 모든 사용자 지정 필드 및 값과 함께 레코드 또는 레코드와 연결된 모든 표준 필드를 반환합니다. 이 정보는 시나리오의 후속 모듈에 매핑할 수 있습니다.

이 모듈을 구성할 때 다음 필드가 표시됩니다.

<table style="table-layout:auto"> <table style="table-layout:auto"> <col> 
 <col> 
 <tbody> 
  <tr> 
   td role="rowheader"&gt; <p>[!UICONTROL Connection]</p> </td> 
   <td> <p>에 Allocadia 계정을 연결하는 방법에 대한 지침 [!DNL Workfront Fusion], 참조 <a href="#connect-allocadia-to-workfront-fusion" class="MCXref xref">[!UICONTROL Connect Allocadia]를 Workfront Fusion에 연결</a> 이 문서에서.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">필터</td> 
   <td> <p>시나리오가 새 레코드만 볼 것인지 [!UICONTROL 업데이트된 레코드만 볼 것인지 새 레코드와 업데이트된 레코드를 볼 것인지를 선택합니다.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">엔티티 유형</td> 
   <td>모듈에서 감시할 Allocadia 레코드 유형을 선택합니다.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">출력</td> 
   <td> <p>모듈의 출력에 포함할 필드를 선택합니다. 사용 가능한 필드는 선택한 엔티티 유형에 따라 다릅니다.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">제한</td> 
   <td> <p>각 시나리오 실행 주기 동안 모듈이 지켜볼 최대 레코드 수를 입력하거나 매핑합니다.</p> </td> 
  </tr> 
 </tbody> 
</table>

### 액션

* [사용자 정의 API 호출](#custom-api-call)
* [레코드 읽기](#read-record)
* [레코드 만들기](#create-record)
* [레코드 삭제](#delete-record)
* [레코드 업데이트](#update-record)

#### [!UICONTROL 사용자 정의 API 호출]

이 작업 모듈에서는 다음을 위한 사용자 지정 인증 호출을 만들 수 있습니다. [!DNL Allocadia] API. 이렇게 하면 다른 사용자가 수행할 수 없는 데이터 흐름 자동화를 만들 수 있습니다 [!DNL Allocadia] 모듈.

작업은 지정한 엔티티 유형(Allocadia 객체 유형)을 기반으로 합니다.

이 모듈을 구성할 때 다음 필드가 표시됩니다.

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Connection]</p> </td> 
   <td> <p>연결에 대한 자세한 내용 [!DNL Allocadia] 계정 위치: [!DNL Workfront Fusion], 참조 <a href="#connect-allocadia-to-workfront-fusion" class="MCXref xref">연결 [!DNL Allocadia] 끝 [!DNL Workfront Fusion]</a> 이 문서에서.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL URL]</td> 
   <td>상대 경로 입력 <code>https://api-na.allocadia.com/{version}</code> 또는 <code>https://api-eu.allocadia.com/{version}</code>.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL 메서드]</td> 
   <td> <p>API 호출을 구성하는 데 필요한 HTTP 요청 메서드를 선택합니다. 자세한 내용은 <a href="../../workfront-fusion/modules/http-request-methods.md" class="MCXref xref" data-mc-variable-override="">의 HTTP 요청 메서드 [!DNL Adobe Workfront Fusion]</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Headers]</td> 
   <td> <p>표준 JSON 개체 형태로 요청의 헤더를 추가합니다.</p> <p>For example, <code>{"Content-type":"application/json"}</code></p> <p>[!DNL Workfront Fusion] 인증 헤더를 추가합니다.</p> </td> 
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

#### [!UICONTROL 레코드 읽기]

이 작업 모듈은 의 단일 레코드에서 데이터를 읽습니다. [!DNL Allocadia].

레코드의 ID를 지정합니다.

모듈은 연결에서 액세스하는 모든 사용자 지정 필드 및 값과 함께 레코드와 연결된 모든 표준 필드를 반환합니다. 이 정보는 시나리오의 후속 모듈에 매핑할 수 있습니다.

이 모듈을 구성할 때 다음 필드가 표시됩니다.

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
   td role="rowheader"&gt; <p>[!UICONTROL Connection]</p> </td> 
   <td> <p>연결에 대한 자세한 내용 [!DNL Allocadia] 계정 위치: [!DNL Workfront Fusion], 참조 <a href="#connect-allocadia-to-workfront-fusion" class="MCXref xref">연결 [!DNL Allocadia] 끝 [!DNL Workfront Fusion]</a> 이 문서에서.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL 엔티티 유형]</td> 
   <td>유형 선택 [!DNL Allocadia] 모듈에서 읽을 레코드를 기록합니다.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL 출력]</td> 
   <td> <p>모듈의 출력에 포함할 필드를 선택합니다. 사용 가능한 필드는 선택한 [!UICONTROL Entity Type]에 따라 다릅니다.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL ID]</td> 
   <td>고유 항목 입력 또는 매핑 [!DNL Allocadia] 모듈에서 읽을 레코드의 ID입니다.</td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL 레코드 만들기]

이 작업 모듈은 레코드를 만듭니다.

모듈은 연결에서 액세스하는 사용자 지정 필드 및 값과 함께 레코드 및 관련 필드의 ID를 반환합니다. 이 정보는 시나리오의 후속 모듈에 매핑할 수 있습니다.

이 모듈을 구성할 때 다음 필드가 표시됩니다.

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
   td role="rowheader"&gt; <p>[!UICONTROL Connection]</p> </td> 
   <td> <p>연결에 대한 자세한 내용 [!DNL Allocadia] 계정 위치: [!DNL Workfront Fusion], 참조 <a href="#connect-allocadia-to-workfront-fusion" class="MCXref xref">연결 [!DNL Allocadia] 끝 [!DNL Workfront Fusion]</a> 이 문서에서.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL 엔티티 유형]</td> 
   <td>라인 항목 또는 열 선택에 따라 새 레코드를 생성할지 여부를 선택합니다.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL 예산]</td> 
   <td> <p>레코드를 생성할 예산을 선택합니다.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!DNL Column choices]</td> 
   <td>새 레코드를 만드는 데 사용할 열을 선택합니다.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!DNL Label]</td> 
   <td>새 레코드에 대한 레이블 입력 또는 매핑</td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL 레코드 삭제]

이 작업 모듈은 특정 레코드를 삭제합니다.

레코드의 ID를 지정합니다.

모듈은 연결에서 액세스하는 사용자 지정 필드 및 값과 함께 레코드 및 관련 필드의 ID를 반환합니다. 이 정보는 시나리오의 후속 모듈에 매핑할 수 있습니다.

이 모듈을 구성할 때 다음 필드가 표시됩니다.

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
   td role="rowheader"&gt; <p>[!UICONTROL Connection]</p> </td> 
   <td> <p>연결에 대한 자세한 내용 [!DNL Allocadia] 계정 위치: [!DNL Workfront Fusion], 참조 <a href="#connect-allocadia-to-workfront-fusion" class="MCXref xref">연결 [!DNL Allocadia] 끝 [!DNL Workfront Fusion]</a> 이 문서에서.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL 엔티티 유형]</td> 
   <td> <p>삭제할 엔티티 유형을 선택합니다.</p> 
    <ul> 
     <li> <p><strong>[!UICONTROL 라인 항목]</strong> </p> <p>라인 항목 ID 입력</p> </li> 
     <li> <p><strong>[!UICONTROL 열 선택]</strong> </p> <p>레코드를 삭제할 예산을 선택한 다음 열 ID와 선택 ID를 입력합니다.</p> </li> 
     <li> <p><strong>[!UICONTROL 예측 태그]</strong> </p> <p>레코드를 삭제할 예산을 선택한 다음 태그 ID를 입력합니다.</p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL 레코드 업데이트]

이 작업 모듈은 라인 항목, 사용자 또는 열 선택과 같은 레코드를 업데이트합니다.

레코드의 ID를 지정합니다.

모듈은 연결에서 액세스하는 사용자 지정 필드 및 값과 함께 레코드 및 관련 필드의 ID를 반환합니다. 이 정보는 시나리오의 후속 모듈에 매핑할 수 있습니다.

이 모듈을 구성할 때 다음 필드가 표시됩니다.

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Connection]</p> </td> 
   <td> <p>[!UICONTROL Allocadia] 계정 연결에 대한 지침입니다. [!DNL Workfront Fusion], 참조 <a href="#connect-allocadia-to-workfront-fusion" class="MCXref xref">연결 [!DNL Allocadia] 끝 [!DNL Workfront Fusion]</a> 이 문서에서.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL 엔티티 유형]</td> 
   <td>유형 선택 [!DNL Allocadia] 모듈을 업데이트할 레코드입니다. 다른 필드는 선택한 엔티티 유형에 따라 나타납니다.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL 예산]</td> 
   <td> <p>레코드를 갱신할 예산을 선택합니다. </p> </td> 
  </tr> 
 </tbody> 
</table>

### 검색 결과

#### [!UICONTROL 레코드 검색]

이 검색 모듈은 의 개체에서 레코드를 찾습니다. [!DNL Allocadia] 지정한 검색 쿼리와 일치하는 쿼리입니다.

이 정보는 시나리오의 후속 모듈에 매핑할 수 있습니다.

원하는 레코드 유형을 지정합니다.

이 모듈을 구성할 때 다음 필드가 표시됩니다.

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
   td role="rowheader"&gt; <p>[!UICONTROL Connection]</p> </td> 
   <td> <p>연결에 대한 자세한 내용 [!DNL Allocadia] 계정 위치: [!DNL Workfront Fusion], 참조 <a href="#connect-allocadia-to-workfront-fusion" class="MCXref xref">연결 [!DNL Allocadia] 끝 [!DNL Workfront Fusion]</a> 이 문서에서.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL 엔티티 유형]</td> 
   <td>유형 선택 [!DNL Allocadia] 모듈에서 검색할 레코드를 기록합니다. </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL 예산]</td> 
   <td> <p>검색할 예산을 선택합니다. </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL 결과 집합]</td> 
   <td>모듈이 모든 일치 레코드를 반환할지, 첫 번째 일치 레코드만 반환할지 여부를 선택합니다.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL 레코드의 최대 개수]</td> 
   <td> <p>각 시나리오 실행 주기 동안 모듈이 반환할 최대 레코드 수를 입력하거나 매핑합니다.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL 검색 기준]</td> 
   <td>검색할 필드를 선택하고 작업을 선택한 다음 검색할 값을 입력하거나 매핑합니다. 다음을 추가할 수 있습니다. [!DNL AND] 또는 [!DNL OR] 검색을 추가로 필터링하는 규칙입니다.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL 출력]</td> 
   <td> <p>모듈의 출력에 포함할 필드를 선택합니다. 사용 가능한 필드는 선택한 엔티티 유형에 따라 다릅니다.</p> </td> 
  </tr> 
 </tbody> 
</table>
