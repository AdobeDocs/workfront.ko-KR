---
content-type: reference
product-previous: workfront-fusion
product-area: workfront-integrations
keywords: 커넥터
navigation-topic: apps-and-their-modules
title: Allocadia 모듈
description: Adobe Workfront Fusion 설명서가 새 위치로 이동했습니다. 이 문서는 더 이상 사용되지 않지만, 이 기능을 다루는 새 문서에 대한 링크를 포함합니다.
author: Becky
feature: Workfront Fusion
exl-id: f1edefd1-9fe0-48fc-bea2-c3f9facf7363
source-git-commit: efbe888d370e20c895dc40f18f999f2d01ec6337
workflow-type: tm+mt
source-wordcount: '1467'
ht-degree: 0%

---

# [!DNL Allocadia]개 모듈

>[!IMPORTANT]
>
>Adobe Workfront Fusion 설명서가 새 위치로 이동했습니다.
>
>이 문서의 정보는 이제 문서에서 찾을 수 있습니다.
>
>* [Allocadia 모듈](https://experienceleague.adobe.com/docs/workfront-fusion/using/references/apps-and-their-modules/third-party-app-connectors/allocadia-modules.html)
>
>모든 책갈피를 업데이트하십시오.
>
>이 문서는 더 이상 업데이트되지 않으며 곧 제거될 예정입니다.

[!DNL Adobe Workfront Fusion] 시나리오에서는 [!DNL Allocadia]을(를) 사용하는 워크플로를 자동화하고 여러 타사 응용 프로그램 및 서비스에 연결할 수 있습니다.

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

[!DNL Allocadia] 모듈을 사용하려면 [!DNL Allocadia] 계정이 있어야 합니다.

## [!DNL Allocadia] API 정보

Allocadia 커넥터는 다음을 사용합니다.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">API 버전</td> 
   <td> v1 </td> 
  </tr> 
  <tr> 
   <td role="rowheader">API 태그</td> 
   <td>v1.7.6</td> 
  </tr>
 </tbody> 
</table>

## [!DNL Allocadia]을(를) [!DNL Workfront Fusion]에 연결

[!DNL Allocadia] 모듈 내에서 직접 [!DNL Allocadia] 계정에 연결할 수 있습니다.

1. [!DNL Allocadia] 모듈에서 [!UICONTROL 연결] 필드 옆에 있는 **[!UICONTROL 추가]**&#x200B;를 클릭합니다.
1. 북미 서버를 사용할지 유럽 서버를 사용할지 선택합니다.
1. 사용자 이름과 암호를 입력합니다.
1. 연결을 만들고 모듈로 돌아가려면 **[!UICONTROL 계속]**&#x200B;을 클릭하세요.

## [!DNL Allocadia]개 모듈 및 해당 필드

[!DNL Allocadia] 모듈을 구성할 때 [!DNL Workfront Fusion]에 아래 나열된 필드가 표시됩니다. 앱 또는 서비스의 액세스 수준과 같은 요소에 따라 이러한 필드와 함께 [!DNL Allocadia] 필드가 추가로 표시될 수 있습니다. 모듈의 굵은 제목은 필수 필드를 나타냅니다.

필드나 함수 위에 맵 단추가 표시되면 이 단추를 사용하여 해당 필드에 대한 변수와 함수를 설정할 수 있습니다. 자세한 내용은 [한 모듈에서 다른 모듈로 정보를 매핑 [!DNL Adobe Workfront Fusion]](../../workfront-fusion/mapping/map-information-between-modules.md)을 참조하십시오.

![](assets/map-toggle-350x74.png)

* [트리거](#triggers)
* [액션](#actions)
* [검색 결과](#searches)

### 트리거

#### [!UICONTROL 레코드 보기]

이 트리거 모듈은 특정 유형의 객체가 추가, 업데이트 또는 둘 다 될 때 시나리오를 실행합니다. 모듈은 연결에서 액세스하는 모든 사용자 지정 필드 및 값과 함께 레코드 또는 레코드와 연결된 모든 표준 필드를 반환합니다. 이 정보는 시나리오의 후속 모듈에 매핑할 수 있습니다.

이 모듈을 구성할 때 다음 필드가 표시됩니다.

<table style="table-layout:auto"> <table style="table-layout:auto"> <col> 
 <col> 
 <tbody> 
  <tr> 
   td role="rowheader"&gt; <p>[!UICONTROL Connection]</p> </td> 
   <td> <p>Allocadia 계정을 [!DNL Workfront Fusion]에 연결하는 방법에 대한 지침은 이 문서의 <a href="#connect-allocadia-to-workfront-fusion" class="MCXref xref">[!UICONTROL Connect Allocadia]를 Workfront Fusion</a>에 참조하십시오.</p> </td> 
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

#### [!UICONTROL 사용자 지정 API 호출]

이 작업 모듈을 사용하면 [!DNL Allocadia] API에 대해 사용자 지정 인증된 호출을 수행할 수 있습니다. 이렇게 하면 다른 [!DNL Allocadia] 모듈에서 수행할 수 없는 데이터 흐름 자동화를 만들 수 있습니다.

작업은 지정한 엔티티 유형(Allocadia 객체 유형)을 기반으로 합니다.

이 모듈을 구성할 때 다음 필드가 표시됩니다.

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Connection]</p> </td> 
   <td> <p>[!DNL Allocadia] 계정을 [!DNL Workfront Fusion]에 연결하는 방법에 대한 지침은 이 문서에서 <a href="#connect-allocadia-to-workfront-fusion" class="MCXref xref">[!DNL Allocadia]을(를) [!DNL Workfront Fusion]</a>에 연결 을 참조하십시오.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL URL]</td> 
   <td><code>https://api-na.allocadia.com/{version}</code> 또는 <code>https://api-eu.allocadia.com/{version}</code>과(와) 관련된 경로를 입력하십시오.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL 메서드]</td> 
   <td> <p>API 호출을 구성하는 데 필요한 HTTP 요청 메서드를 선택합니다. 자세한 내용은 [!DNL Adobe Workfront Fusion]</a>에서 <a href="../../workfront-fusion/modules/http-request-methods.md" class="MCXref xref" data-mc-variable-override="">HTTP 요청 메서드를 참조하십시오.</p> </td> 
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
   <td> <p>표준 JSON 개체의 형태로 API 호출에 대한 본문 콘텐츠를 추가합니다.</p> <p>참고:  <p>JSON에서 <code>if</code>과(와) 같은 조건문을 사용할 때 따옴표를 조건문 외부에 넣으십시오.</p> 
     <div class="example" data-mc-autonum="<b>Example: </b>"> 
      <p> <img src="assets/quotes-in-json-350x120.png" style="width: 350;height: 120;"> </p> 
     </div> </p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL 레코드 읽기]

이 작업 모듈은 [!DNL Allocadia]의 단일 레코드에서 데이터를 읽습니다.

레코드의 ID를 지정합니다.

모듈은 연결에서 액세스하는 모든 사용자 지정 필드 및 값과 함께 레코드와 연결된 모든 표준 필드를 반환합니다. 이 정보는 시나리오의 후속 모듈에 매핑할 수 있습니다.

이 모듈을 구성할 때 다음 필드가 표시됩니다.

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
   td role="rowheader"&gt; <p>[!UICONTROL Connection]</p> </td> 
   <td> <p>[!DNL Allocadia] 계정을 [!DNL Workfront Fusion]에 연결하는 방법에 대한 지침은 이 문서에서 <a href="#connect-allocadia-to-workfront-fusion" class="MCXref xref">[!DNL Allocadia]을(를) [!DNL Workfront Fusion]</a>에 연결 을 참조하십시오.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL 엔티티 유형]</td> 
   <td>모듈에서 읽을 [!DNL Allocadia] 레코드의 형식을 선택하십시오.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL 출력]</td> 
   <td> <p>모듈의 출력에 포함할 필드를 선택합니다. 사용 가능한 필드는 선택한 [!UICONTROL Entity Type]에 따라 다릅니다.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL ID]</td> 
   <td>모듈에서 읽을 레코드의 고유 [!DNL Allocadia] ID를 입력하거나 매핑합니다.</td> 
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
   <td> <p>[!DNL Allocadia] 계정을 [!DNL Workfront Fusion]에 연결하는 방법에 대한 지침은 이 문서에서 <a href="#connect-allocadia-to-workfront-fusion" class="MCXref xref">[!DNL Allocadia]을(를) [!DNL Workfront Fusion]</a>에 연결 을 참조하십시오.</p> </td> 
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
   <td> <p>[!DNL Allocadia] 계정을 [!DNL Workfront Fusion]에 연결하는 방법에 대한 지침은 이 문서에서 <a href="#connect-allocadia-to-workfront-fusion" class="MCXref xref">[!DNL Allocadia]을(를) [!DNL Workfront Fusion]</a>에 연결 을 참조하십시오.</p> </td> 
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
   <td> <p>[!UICONTROL Allocadia] 계정을 [!DNL Workfront Fusion]에 연결하는 방법에 대한 지침은 이 문서의 <a href="#connect-allocadia-to-workfront-fusion" class="MCXref xref">[!DNL Allocadia]을(를) [!DNL Workfront Fusion]</a>에 연결 을 참조하십시오.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL 엔티티 유형]</td> 
   <td>모듈을 업데이트할 [!DNL Allocadia] 레코드의 형식을 선택하십시오. 다른 필드는 선택한 엔티티 유형에 따라 나타납니다.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL 예산]</td> 
   <td> <p>레코드를 갱신할 예산을 선택합니다. </p> </td> 
  </tr> 
 </tbody> 
</table>

### 검색 결과

#### [!UICONTROL 레코드 검색]

이 검색 모듈은 지정한 검색 쿼리와 일치하는 [!DNL Allocadia]의 개체에서 레코드를 찾습니다.

이 정보는 시나리오의 후속 모듈에 매핑할 수 있습니다.

원하는 레코드 유형을 지정합니다.

이 모듈을 구성할 때 다음 필드가 표시됩니다.

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
   td role="rowheader"&gt; <p>[!UICONTROL Connection]</p> </td> 
   <td> <p>[!DNL Allocadia] 계정을 [!DNL Workfront Fusion]에 연결하는 방법에 대한 지침은 이 문서에서 <a href="#connect-allocadia-to-workfront-fusion" class="MCXref xref">[!DNL Allocadia]을(를) [!DNL Workfront Fusion]</a>에 연결 을 참조하십시오.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL 엔티티 유형]</td> 
   <td>모듈에서 검색할 [!DNL Allocadia] 레코드의 형식을 선택하십시오. </td> 
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
   <td>검색할 필드를 선택하고 작업을 선택한 다음 검색할 값을 입력하거나 매핑합니다. [!DNL AND] 또는 [!DNL OR] 규칙을 추가하여 검색을 추가로 필터링할 수 있습니다.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL 출력]</td> 
   <td> <p>모듈의 출력에 포함할 필드를 선택합니다. 사용 가능한 필드는 선택한 엔티티 유형에 따라 다릅니다.</p> </td> 
  </tr> 
 </tbody> 
</table>
