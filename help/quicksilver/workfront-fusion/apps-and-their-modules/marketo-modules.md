---
content-type: reference
product-previous: workfront-fusion
product-area: workfront-integrations
keywords: 커넥터
navigation-topic: apps-and-their-modules
title: Marketo 모듈
description: 다음에서 [!DNL Adobe Workfront Fusion] 시나리오에서는 다음을 사용하는 워크플로를 자동화할 수 있습니다 [!DNL Marketo]을 여러 타사 응용 프로그램 및 서비스에 연결할 수 있습니다.
author: Becky
feature: Workfront Fusion
exl-id: 7f6dace5-ab50-45da-a926-1a8919057f7b
source-git-commit: c51169c18bef8ac8126a04c08deb88d830517b0b
workflow-type: tm+mt
source-wordcount: '2068'
ht-degree: 0%

---

# [!DNL Marketo] 모듈

다음에서 [!DNL Adobe Workfront Fusion] 시나리오에서는 다음을 사용하는 워크플로를 자동화할 수 있습니다 [!DNL Marketo]을 여러 타사 응용 프로그램 및 서비스에 연결할 수 있습니다.

Marketo 커넥터에 대한 비디오 소개는 다음을 참조하십시오.

* [Marketo](https://video.tv.adobe.com/v/3427026/){target=_blank}

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

사용 [!DNL Marketo] 모듈, 다음이 있어야 합니다. [!DNL Marketo] 계정입니다.

## 연결 [!DNL Marketo] Workfront Fusion으로 {#connect-marketo-to-workfront-fusion}

에 대한 연결을 만들 수 있습니다. [!DNL Marketo] 내부에서 직접 계정 생성 [!DNL Marketo] 모듈.

1. 다음 중 하나 [!DNL Marketo] 모듈, 클릭 **[!UICONTROL 추가]** 다음 옆에 [!UICONTROL 연결] 필드.
1. 다음을 입력하십시오. [!DNL Marketo] 계정 또는 [!DNL Marketo] [!UICONTROL 먼치킨] ID 계정에 할당된 기본 URL 또는 끝점의 고유한 부분으로, 액세스하는 데 사용합니다. [!DNL Marketo] 를 통해 [!UICONTROL 나머지] API. 이 위치를 찾는 방법에 대한 지침은 [기본 URL](https://developers.marketo.com/rest-api/base-url/) 다음에서 [!DNL Marketo] 설명서를 참조하십시오.
1. 다음을 입력하십시오. [!UICONTROL 클라이언트 ID] 및 [!UICONTROL 클라이언트 암호]. 위치를 찾는 방법에 대한 자세한 내용은 [인증](https://developers.marketo.com/rest-api/authentication/) 다음에서 [!DNL Marketo] 설명서를 참조하십시오.
1. 클릭 **[!UICONTROL 계속]** 를 클릭하여 연결을 만들고 모듈로 돌아갑니다.

## [!DNL Marketo] 모듈 및 해당 필드

를 구성할 때 [!DNL Marketo] 모듈, [!DNL Workfront Fusion] 아래 나열된 필드를 표시합니다. 이와 함께 추가 [!DNL Marketo] 앱이나 서비스의 액세스 수준 등에 따라 필드가 표시될 수 있습니다. 모듈의 굵은 제목은 필수 필드를 나타냅니다.

필드나 함수 위에 맵 단추가 표시되면 이 단추를 사용하여 해당 필드에 대한 변수와 함수를 설정할 수 있습니다. 자세한 내용은 [의 한 모듈에서 다른 모듈로 정보 매핑 [!DNL Adobe Workfront Fusion]](../../workfront-fusion/mapping/map-information-between-modules.md).

![](assets/map-toggle-350x74.png)

* [트리거](#triggers)
* [액션](#actions)
* [검색 결과](#searches)

### 트리거

* [[!UICONTROL 레코드 보기]](#watch-records)
* [[!UICONTROL 이벤트 보기(인스턴트)]](#watch-events-instant)

#### [!UICONTROL 레코드 보기]

이 트리거 모듈은 레코드가 생성되거나 업데이트될 때 시나리오를 시작합니다.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Connection]</p> </td> 
   <td> <p>연결에 대한 자세한 내용 [!DNL Marketo] 계정 위치: [!DNL Workfront Fusion], 참조 <a href="#connect-marketo-to-workfront-fusion" class="MCXref xref">연결 [!DNL Marketo] 끝 [!DNL Workfront Fusion]</a> 이 문서에서.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL 레코드 유형]</td> 
   <td> <p>만들려는 레코드 유형을 선택합니다.</p> 
    <ul> 
     <li> <p><strong>[!UICONTROL Activity]</strong> </p> <p>보려는 활동 유형을 선택합니다. </p> <p>모듈은 새 활동만 감시합니다.<br></p> </li> 
     <li> <p><strong>[!UICONTROL 리드]</strong> </p> <p>새 레코드, 업데이트된 레코드, 새 레코드와 업데이트된 레코드 모두 또는 특정 필드 업데이트를 감시할지 여부를 선택합니다. 특정 필드 업데이트를 시청하도록 선택하는 경우 모듈에서 시청하려는 필드를 선택합니다.</p> </li> 
     <li> <p><strong>[!UICONTROL 프로그램]</strong> </p> <p>새 레코드, 업데이트된 레코드 또는 새 레코드와 업데이트된 레코드를 모두 감시할지 여부를 선택합니다.</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL 출력]</td> 
   <td> <p>이 모듈에 대한 출력 번들에 포함할 정보를 선택합니다.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL 제한]</td> 
   <td> <p>각 시나리오 실행 주기 동안 모듈이 반환할 최대 레코드 수를 입력하거나 매핑합니다.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL 이벤트 보기(인스턴트)]

이 트리거 모듈은 레코드가 생성되거나 업데이트될 때 시나리오를 시작합니다.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Webhook]</p> </td> 
   <td> <p>모듈에서 사용할 웹후크를 입력합니다.</p> <p>웹후크에 대한 자세한 내용은 <a href="../../workfront-fusion/webhooks/instant-triggers-webhooks.md" class="MCXref xref">의 인스턴트 트리거(웹후크) [!DNL Adobe Workfront Fusion]</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL 제한]</td> 
   <td> <p>각 시나리오 실행 주기 동안 모듈이 반환할 최대 레코드 수를 입력하거나 매핑합니다.</p> </td> 
  </tr> 
 </tbody> 
</table>

### 액션

* [[!UICONTROL 사용자 정의 API 호출]](#custom-api-call)
* [[!UICONTROL 레코드 만들기]](#create-a-record)
* [[!UICONTROL 레코드 업데이트]](#update-a-record)
* [[!UICONTROL 파일 다운로드]](#download-a-file)
* [[!UICONTROL 파일 업로드]](#upload-a-file)
* [[!UICONTROL 레코드 읽기]](#read-a-record)
* [[!UICONTROL 목록에 리드 추가]](#add-leads-to-a-list)
* [[!UICONTROL 목록에서 리드 제거]](#remove-leads-from-a-list)
* [[!UICONTROL 캠페인 예약]](#schedule-a-campaign)
* [[!UICONTROL 프로그램 복사]](#copy-a-program)

#### [!UICONTROL 사용자 정의 API 호출]

이 작업 모듈에서는 다음을 위한 사용자 지정 인증 호출을 만들 수 있습니다. [!DNL Marketo] API. 이렇게 하면 다른 사용자가 수행할 수 없는 데이터 흐름 자동화를 만들 수 있습니다 [!DNL Marketo] 모듈.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Connection]</p> </td> 
   <td> <p>연결에 대한 자세한 내용 [!DNL Marketo] 계정 위치: [!DNL Workfront Fusion], 참조 <a href="#connect-marketo-to-workfront-fusion" class="MCXref xref">연결 [!DNL Marketo] 끝 [!DNL Workfront Fusion]</a> 이 문서에서.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL URL]</td> 
   <td>상대 경로 입력 <code>https://{your-base-url}.mktorest.com/</code>.</td> 
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
  <tr> 
   <td role="rowheader">[!UICONTROL 제한]</td> 
   <td> <p>각 시나리오 실행 주기 동안 모듈이 사용할 최대 레코드 수를 입력하거나 매핑합니다.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL 레코드 만들기]

이 작업 모듈은에 새 레코드를 만듭니다. [!DNL Marketo]

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Connection]</p> </td> 
   <td> <p>연결에 대한 자세한 내용 [!DNL Marketo] 계정 위치: [!DNL Workfront Fusion], 참조 <a href="#connect-marketo-to-workfront-fusion" class="MCXref xref">연결 [!DNL Marketo] 끝 [!DNL Workfront Fusion]</a> 이 문서에서.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL 레코드 유형]</td> 
   <td> <p>만들려는 레코드 유형을 선택합니다.</p> 
    <ul> 
     <li> <p>[!UICONTROL Company]</p> </li> 
     <li> <p>[!UICONTROL 폴더]</p> </li> 
     <li> <p>[!UICONTROL 리드]</p> </li> 
     <li> <p>[!UICONTROL 프로그램]</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL 매핑할 필드 선택]</td> 
   <td>회사 또는 가망 고객을 생성하는 경우 신규 레코드 생성 시 값을 설정할 필드를 선택한 다음 해당 필드에 대한 값을 입력합니다.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL 프로그램 유형]</td> 
   <td>프로그램을 만드는 경우 만들려는 프로그램 유형을 선택합니다.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL 프로그램 채널] </td> 
   <td>프로그램을 만드는 경우 프로그램을 만들려는 프로그램 채널을 선택합니다.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Folder] / [!UICONTROL Program Name]</td> 
   <td>폴더 또는 프로그램을 생성하는 경우 새 레코드의 이름을 입력하거나 매핑합니다.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL 설명]</td> 
   <td> <p>폴더 또는 프로그램을 생성하는 경우 새 레코드에 대한 설명을 입력하거나 매핑합니다.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL 상위 폴더 ID]</td> 
   <td>폴더 또는 프로그램을 만드는 경우 새 레코드를 만들 상위 폴더의 ID를 입력하거나 매핑합니다.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL 비용]</td> 
   <td>프로그램을 생성하는 경우 비용을 추가합니다.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL 태그]</td> 
   <td>프로그램을 만드는 경우 태그를 추가합니다</td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL 레코드 업데이트]

이 작업 모듈은 해당 ID를 사용하여 기존 레코드를 업데이트합니다.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Connection]</p> </td> 
   <td> <p>연결에 대한 자세한 내용 [!DNL Marketo] 계정 위치: [!DNL Workfront Fusion], 참조 <a href="#connect-marketo-to-workfront-fusion" class="MCXref xref">연결 [!DNL Marketo] 끝 [!DNL Workfront Fusion]</a> 이 문서에서.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL 레코드 유형]</td> 
   <td> <p>만들려는 레코드 유형을 선택합니다.</p> 
    <ul> 
     <li> <p>[!UICONTROL Company]</p> </li> 
     <li> <p>[!UICONTROL 리드]</p> </li> 
     <li> <p>[!UICONTROL 프로그램]</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Company] / [!UICONTROL Lead] / [!UICONTROL Program ID]</td> 
   <td>업데이트할 레코드의 ID를 입력하거나 매핑합니다.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL 매핑할 필드 선택]</td> 
   <td>회사 또는 가망 고객을 갱신하는 경우 값을 갱신할 필드를 선택한 다음 해당 필드에 대한 값을 입력합니다.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL 프로그램 이름]</td> 
   <td>프로그램을 업데이트하는 경우 프로그램의 새 이름을 입력하거나 매핑합니다.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL 설명]</td> 
   <td> <p>프로그램을 갱신하는 경우 프로그램에 대한 새 설명을 입력하거나 매핑합니다.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL 시작 날짜]</td> 
   <td>프로그램을 갱신하는 경우 프로그램의 신규 시작 일자를 입력하거나 맵핑합니다.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL 종료 날짜]</td> 
   <td>프로그램을 갱신하는 경우 프로그램의 신규 종료 일자를 입력하거나 맵핑합니다.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL 비용]</td> 
   <td>프로그램을 업데이트하는 경우 비용을 추가합니다.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL 태그]</td> 
   <td>프로그램을 업데이트하는 경우 태그를 추가합니다</td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL 파일 다운로드]

이 작업 모듈은 파일 ID를 사용하여 파일을 다운로드합니다.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Connection]</p> </td> 
   <td> <p>연결에 대한 자세한 내용 [!DNL Marketo] 계정 위치: [!DNL Workfront Fusion], 참조 <a href="#connect-marketo-to-workfront-fusion" class="MCXref xref">연결 [!DNL Marketo] 끝 [!DNL Workfront Fusion]</a> 이 문서에서.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL 파일 ID]</td> 
   <td>다운로드할 파일의 ID를 매핑합니다.</td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL 파일 업로드]

이 작업 모듈은에 새 파일을 업로드합니다 [!UICONTROL Marketo].

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Connection]</p> </td> 
   <td> <p>연결에 대한 자세한 내용 [!DNL Marketo] 계정 위치: [!DNL Workfront Fusion], 참조 <a href="#connect-marketo-to-workfront-fusion" class="MCXref xref">연결 [!DNL Marketo] 끝 [!DNL Workfront Fusion]</a> 이 문서에서.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL 소스 파일]</td> 
   <td>이전 모듈에서 소스 파일을 선택하거나 소스 파일의 이름과 데이터를 매핑합니다.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL 폴더 ID]</td> 
   <td>새 파일을 저장할 폴더의 ID를 입력하거나 매핑합니다.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL 설명]</td> 
   <td>업로드한 파일에 대한 설명을 입력합니다.</td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL 레코드 읽기]

이 작업 모듈은 해당 ID를 사용하여 레코드에 대한 정보를 읽습니다.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Connection]</p> </td> 
   <td> <p>연결에 대한 자세한 내용 [!DNL Marketo] 계정 위치: [!DNL Workfront Fusion], 참조 <a href="#connect-marketo-to-workfront-fusion" class="MCXref xref">연결 [!DNL Marketo] 끝 [!DNL Workfront Fusion]</a> 이 문서에서.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL 레코드 유형]</td> 
   <td> <p>만들려는 레코드 유형을 선택합니다.</p> 
    <ul> 
     <li> <p>[!UICONTROL Campaign]</p> </li> 
     <li> <p>[!UICONTROL Company]</p> </li> 
     <li> <p>[!UICONTROL 리드]</p> </li> 
     <li> <p>[!UICONTROL 목록]</p> </li> 
     <li> <p>[!UICONTROL 프로그램]</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL 출력]</td> 
   <td>이 모듈에 대한 출력 번들에 포함할 정보를 선택합니다. 필드는 선택한 [!UICONTROL 레코드 종류]에 따라 사용할 수 있습니다.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL &lt;object&gt; ID]</td> 
   <td>정보를 검색할 개체의 ID를 입력하거나 매핑합니다.</td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL 목록에 리드 추가]

이 작업 모듈은 리드 ID를 사용하여 하나 이상의 리드를 목록에 추가합니다.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Connection]</p> </td> 
   <td> <p>연결에 대한 자세한 내용 [!DNL Marketo] 계정 위치: [!DNL Workfront Fusion], 참조 <a href="#connect-marketo-to-workfront-fusion" class="MCXref xref">연결 [!DNL Marketo] 끝 [!DNL Workfront Fusion]</a> 이 문서에서.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL 목록 ID]</td> 
   <td>리드를 추가할 목록의 ID를 입력하거나 매핑합니다.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL 리드 ID]</td> 
   <td> <p>목록에 추가할 각 리드에 대해 다음을 클릭합니다. <b>[!UICONTROL 추가]</b>을 클릭한 후 추가할 잠재 고객의 ID를 입력하거나 매핑합니다. 목록에 추가할 모듈에 대해 최대 300개의 리드를 추가할 수 있습니다.</p> <p>맵 토글을 클릭하여 목록에 추가하려는 기존 리드 컬렉션을 매핑합니다.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL 목록에서 리드 제거]

이 작업 모듈은 리드 ID를 사용하여 목록에서 하나 이상의 리드를 제거합니다.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Connection]</p> </td> 
   <td> <p>연결에 대한 자세한 내용 [!DNL Marketo] 계정 위치: [!DNL Workfront Fusion], 참조 <a href="#connect-marketo-to-workfront-fusion" class="MCXref xref">연결 [!DNL Marketo] 끝 [!DNL Workfront Fusion]</a> 이 문서에서.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL 목록 ID]</td> 
   <td>리드를 제거할 목록의 ID를 입력하거나 매핑합니다.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL 리드 ID]</td> 
   <td> <p>목록에서 제거할 각 리드에 대해 다음을 클릭합니다. <b>[!UICONTROL 추가]</b>그런 다음 제거할 잠재 고객의 ID를 입력하거나 매핑합니다. 목록에서 제거할 모듈에 대해 최대 300개의 리드를 추가할 수 있습니다. </p> <p>맵 토글을 클릭하여 목록에서 제거할 기존 리드 컬렉션을 매핑합니다.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL 캠페인 예약]

이 작업 모듈은 특정 날짜에 대한 기존 캠페인을 예약합니다.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Connection]</p> </td> 
   <td> <p>연결에 대한 자세한 내용 [!DNL Marketo] 계정 위치: [!DNL Workfront Fusion], 참조 <a href="#connect-marketo-to-workfront-fusion" class="MCXref xref">연결 [!DNL Marketo] 끝 [!DNL Workfront Fusion]</a> 이 문서에서.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL 캠페인 ID]</td> 
   <td>예약하려는 캠페인의 ID를 입력하거나 매핑합니다.</td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Schedule for Date]</p> </td> 
   <td>캠페인을 실행할 날짜를 선택합니다. 이 필드를 비워 두면 시나리오가 시작된 후 5분 후에 캠페인이 실행됩니다.</td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL 프로그램 복사]

이 작업 모듈은 기존 프로그램의 ID를 사용하여 프로그램의 복사본을 만듭니다.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Connection]</p> </td> 
   <td> <p>연결에 대한 자세한 내용 [!DNL Marketo] 계정 위치: [!DNL Workfront Fusion], 참조 <a href="#connect-marketo-to-workfront-fusion" class="MCXref xref">연결 [!DNL Marketo] 끝 [!DNL Workfront Fusion]</a> 이 문서에서.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL 기존 프로그램 ID]</td> 
   <td>복사할 프로그램의 ID를 입력하거나 매핑합니다.</td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL 새 프로그램 이름]</p> </td> 
   <td> <p>새 프로그램의 이름 입력 또는 매핑</p> <p> </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL 폴더 ID]</td> 
   <td>새 프로그램을 배치할 폴더의 ID를 입력하거나 매핑합니다.</td> 
  </tr> 
 </tbody> 
</table>

### 검색 결과

* [[!UICONTROL 목록 레코드]](#list-records)
* [[!UICONTROL 레코드 검색]](#update-a-record)

#### [!UICONTROL 목록 레코드]

이 작업 모듈은 특정 유형의 모든 레코드를 검색합니다.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Connection]</p> </td> 
   <td> <p>연결에 대한 자세한 내용 [!DNL Marketo] 계정 위치: [!DNL Workfront Fusion], 참조 <a href="#connect-marketo-to-workfront-fusion" class="MCXref xref">연결 [!DNL Marketo] 끝 [!DNL Workfront Fusion]</a> 이 문서에서.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL 레코드 유형]</td> 
   <td> <p>나열할 레코드 유형을 선택합니다.</p> 
    <ul> 
     <li> <p>[!UICONTROL 모든 캠페인 읽기]</p> </li> 
     <li> <p>[!UICONTROL 모든 프로그램 읽기]</p> </li> 
     <li> <p>[!UICONTROL 리드 모두 읽기] </p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL 필드]</td> 
   <td>가망 고객 검색을 선택한 경우 목록에서 가망 고객을 검색할지 프로그램에서 가망 고객을 검색할지 선택합니다.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL 출력]</td> 
   <td>이 모듈에 대한 출력 번들에 포함할 정보를 선택합니다. 필드는 선택한 [!UICONTROL 레코드 종류]에 따라 사용할 수 있습니다.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL 제한]</td> 
   <td> <p>각 시나리오 실행 주기 동안 모듈이 반환할 최대 레코드 수를 입력하거나 매핑합니다.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL 레코드 검색]

이 검색 모듈은 특정 검색 기준과 일치하는 레코드 목록을 검색합니다.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Connection]</p> </td> 
   <td> <p>연결에 대한 자세한 내용 [!DNL Marketo] 계정 위치: [!DNL Workfront Fusion], 참조 <a href="#connect-marketo-to-workfront-fusion" class="MCXref xref">연결 [!DNL Marketo] 끝 [!DNL Workfront Fusion]</a> 이 문서에서.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL 레코드 유형]</td> 
   <td> <p>검색할 레코드 유형을 선택합니다.</p> 
    <ul> 
     <li> <p>[!UICONTROL Campaigns]</p> </li> 
     <li> <p>[!UICONTROL 리드]</p> </li> 
     <li> <p>[!UICONTROL 프로그램]</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL 필드]</p> </td> 
   <td> <p>이름, 프로그램 이름 또는 작업 영역 이름으로 검색할지 여부를 선택합니다.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL 값]</td> 
   <td>검색할 각 값에 대해 <b>[!UICONTROL 항목 추가]</b> 값을 입력합니다.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Output]</td> 
   <td> <p>이 모듈에 대한 출력 번들에 포함할 정보를 선택합니다.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL 제한]</td> 
   <td> <p>각 시나리오 실행 주기 동안 모듈이 반환할 최대 레코드 수를 입력하거나 매핑합니다.</p> </td> 
  </tr> 
 </tbody> 
</table>
