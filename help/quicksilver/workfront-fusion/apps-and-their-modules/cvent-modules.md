---
content-type: reference
product-previous: workfront-fusion
product-area: workfront-integrations;documents
keywords: 커넥터
navigation-topic: apps-and-their-modules
title: 이벤트 모듈
description: 에서 [!DNL Adobe Workfront Fusion] 시나리오에서는 Cvent를 사용하는 워크플로우를 자동화하고 여러 타사 애플리케이션 및 서비스에 연결할 수 있습니다.
author: Becky
feature: Workfront Fusion
exl-id: c95b9764-29a5-4d8c-8e6d-68a3969129e0
source-git-commit: 885d93dd4383945538e977fd3edbfd55bda88b70
workflow-type: tm+mt
source-wordcount: '996'
ht-degree: 1%

---

# [!DNL Cvent] 모듈

에서 [!DNL Adobe Workfront Fusion] 시나리오, [!DNL Cvent]여러 타사 애플리케이션 및 서비스에 연결할 수 있습니다.

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

를 사용하려면 [!DNL Cvent] 모듈이면 반드시 [!DNL Cvent] 계정이 필요합니다.

## Connect [!DNL Cvent] to [!DNL Adobe Workfront Fusion] {#connect-cvent-to-adobe-workfront-fusion}

>[!NOTE]
>
>다음 [!DNL Cvent] 모듈은 [!UICONTROL SOAP] API. 연결을 만들려면 [!DNL Cvent]로 지정하는 경우 다음을 확인해야 합니다.
>
>* 다음을 수행합니다. [!UICONTROL SOAP] 액세스 권한 [!DNL Cvent] API.
>* 다음 [!DNL Workfront Fusion] 조직의에 IP 주소를 추가했습니다허용 목록에 추가하다.
>
>  목록 [!DNL Workfront Fusion] IP 주소. 자세한 내용은 [액세스하기 위한 IP 주소 [!DNL Adobe Workfront Fusion]](../../workfront-fusion/get-started/ip-addresses-for-fusion.md)


에 대한 연결을 만들 수 있습니다 [!DNL Cvent] 내에서 직접 계정 [!DNL Cvent] 모듈.

1. 어떤 경우에서도 [!DNL Cvent] 모듈 **[!UICONTROL 추가]** 다음 [!UICONTROL 연결] 필드.
1. 연결할 영역을 선택합니다.

   * [!UICONTROL 북미]
   * [!UICONTROL 유럽]
   * [!UICONTROL 샌드박스]

1. 클릭 **[!UICONTROL 계속]** 연결을 만들고 모듈로 돌아갑니다.

## [!DNL Cvent] 모듈 및 해당 필드

구성 시 [!DNL Cvent] 모듈, [!DNL Workfront Fusion] 아래 나열된 필드를 표시합니다. 이와 함께 추가 [!DNL Cvent] 앱이나 서비스에서 액세스 수준과 같은 요소에 따라 필드가 표시될 수 있습니다. 모듈에서 굵게 표시된 제목은 필수 필드를 나타냅니다.

필드 또는 함수 위에 맵 단추가 표시되면 이 단추를 사용하여 해당 필드에 대한 변수와 함수를 설정할 수 있습니다. 자세한 내용은 [의 한 모듈에서 다른 모듈로 정보 매핑 [!DNL Adobe Workfront Fusion]](../../workfront-fusion/mapping/map-information-between-modules.md).

![](assets/map-toggle-350x74.png)

* [액션](#actions)
* [검색 결과](#searches)

### 액션

* [[!UICONTROL 사용자 지정 API 호출]](#create-meeting-request)
* [[!UICONTROL 레코드 읽기]](#read-a-record)
* [[!UICONTROL 초대 등록]](#register-invitee)
* [[!UICONTROL 초대 추가]](#add-invitee)
* [[!UICONTROL 연락처 삭제]](#delete-contact)
* [[!UICONTROL 연락처 업데이트]](#update-contact)
* [[!UICONTROL 모임 요청 만들기]](#create-meeting-request)

#### [!UICONTROL 사용자 지정 API 호출]

이 작업 모듈을 사용하면 [!DNL Cvent] API. 이렇게 하면 다른 방식으로 수행할 수 없는 데이터 흐름 자동화를 만들 수 있습니다 [!DNL Cvent] 모듈.

이 모듈을 구성할 때 다음 필드가 표시됩니다.

이 모듈은 API 호출의 헤더 및 본문과 함께 상태 코드를 반환합니다.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Connection]</p> </td> 
   <td> <p>연결 방법에 대한 지침은 [!DNL Cvent] 계정 대상 [!DNL Workfront Fusion]를 참조하십시오. <a href="#connect-cvent-to-adobe-workfront-fusion" class="MCXref xref">Connect [!DNL Cvent] to [!DNL Adobe Workfront Fusion]</a> 참조하십시오.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">작업</td> 
   td&gt; <p>API 호출을 구성하는 데 필요한 HTTP 요청 메서드를 선택합니다. 자세한 내용은 <a href="../../workfront-fusion/modules/http-request-methods.md" class="MCXref xref" data-mc-variable-override="">의 HTTP 요청 메서드 [!DNL Adobe Workfront Fusion]</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">본문(XML)</td> 
   <td> <p>API 호출의 본문을 입력하거나 매핑합니다. 여기에는 XML만 포함되어야 합니다. 모듈에 자동으로 인증 헤더가 포함됩니다. </p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL 레코드 읽기]

이 작업 모듈은 특정 레코드에 대한 정보를 읽습니다.

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Connection]</p> </td> 
   <td> <p>연결 방법에 대한 지침은 [!DNL Cvent] 계정 대상 [!DNL Workfront Fusion]를 참조하십시오. <a href="#connect-cvent-to-adobe-workfront-fusion" class="MCXref xref">Connect [!DNL Cvent] to [!DNL Adobe Workfront Fusion]</a> 참조하십시오.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL 레코드 유형]</p> </td> 
   <td>읽을 레코드의 항목 유형을 선택합니다.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Contact] / [!UICONTROL Event] / [!UICONTROL Invitee ID]</td> 
   <td> <p>읽을 항목의 ID를 입력하거나 매핑합니다.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL 출력]</td> 
   <td> <p>모듈의 출력에 포함할 필드를 선택합니다. 선택한 항목 유형에 따라 필드를 사용할 수 있습니다.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL 초대 등록]

이 작업 모듈은 이벤트에 대한 초대를 등록합니다.

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Connection]</p> </td> 
   <td> <p>연결 방법에 대한 지침은 [!DNL Cvent] 계정 대상 [!DNL Workfront Fusion]를 참조하십시오. <a href="#connect-cvent-to-adobe-workfront-fusion" class="MCXref xref">Connect [!DNL Cvent] to [!DNL Adobe Workfront Fusion]</a> 참조하십시오.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>초대 ID</p> </td> 
   <td> <p>이벤트에 등록할 초대 사용자의 ID를 입력하거나 매핑합니다.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">이벤트 ID</td> 
   <td> <p>초대자를 등록할 이벤트의 ID를 입력하거나 매핑합니다.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL 초대 추가]

이 작업 모듈은 이벤트에 연락처를 초대합니다.

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Connection]</p> </td> 
   <td> <p>연결 방법에 대한 지침은 [!DNL Cvent] 계정 대상 [!DNL Workfront Fusion]를 참조하십시오. <a href="#connect-cvent-to-adobe-workfront-fusion" class="MCXref xref">Connect [!DNL Cvent] to [!DNL Adobe Workfront Fusion]</a> 참조하십시오.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL 연락처 ID]</p> </td> 
   <td> <p>이벤트에 추가할 연락처의 ID를 입력하거나 매핑합니다.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL 이벤트 ID]</td> 
   <td> <p>연락처를 추가할 이벤트의 ID를 입력하거나 매핑합니다.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL 연락처 삭제]

이 작업 모듈은 Cvent에서 단일 연락처를 삭제합니다.

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Connection]</p> </td> 
   <td> <p>연결 방법에 대한 지침은 [!DNL Cvent] 계정 대상 [!DNL Workfront Fusion]를 참조하십시오. <a href="#connect-cvent-to-adobe-workfront-fusion" class="MCXref xref">Connect [!DNL Cvent] to [!DNL Adobe Workfront Fusion]</a> 참조하십시오.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL 연락처 ID]</td> 
   <td> <p>삭제할 연락처의 ID를 입력하거나 매핑합니다.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL 연락처 업데이트]

이 작업 모듈은 ID를 사용하여 기존 연락처를 업데이트합니다.

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Connection]</p> </td> 
   <td> <p>연결 방법에 대한 지침은 [!DNL Cvent] 계정 대상 [!DNL Workfront Fusion]를 참조하십시오. <a href="#connect-cvent-to-adobe-workfront-fusion" class="MCXref xref">Connect [!DNL Cvent] to [!DNL Adobe Workfront Fusion]</a> 참조하십시오.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL 연락처 ID]</p> </td> 
   <td> <p>업데이트할 연락처의 ID를 입력하거나 매핑합니다.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Fields]</td> 
   <td> <p>정보를 입력할 필드를 선택한 다음 해당 필드에 원하는 값을 입력합니다.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL 사용자 지정 필드]</td> 
   <td> <p>정보를 입력할 필드를 선택한 다음 해당 필드에 원하는 값을 입력합니다.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL 모임 요청 만들기]

이 작업 모듈은 계정에 모임 요청을 추가합니다.

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Connection]</p> </td> 
   <td> <p>연결 방법에 대한 지침은 [!DNL Cvent] 계정 대상 [!DNL Workfront Fusion]를 참조하십시오. <a href="#connect-cvent-to-adobe-workfront-fusion" class="MCXref xref">Connect [!DNL Cvent] to [!DNL Adobe Workfront Fusion]</a> 참조하십시오.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL 양식 ID]</p> </td> 
   <td> <p>새 모임 요청을 만드는 데 사용할 양식의 ID를 입력하거나 매핑합니다.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Meeting 요청 필드]</td> 
   <td> <p>정보를 입력할 모임 요청 필드를 선택한 다음 해당 필드에 원하는 값을 입력합니다.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL 이벤트 요청 필드]</td> 
   <td> <p>정보를 입력할 이벤트 요청 필드를 선택한 다음, 해당 필드에 원하는 값을 입력합니다.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL RFP 요청 필드]</td> 
   <td> <p>정보를 입력할 제안 필드에 대한 요청을 선택한 다음, 해당 필드에 원하는 값을 입력합니다.</p> </td> 
  </tr> 
 </tbody> 
</table>

### 검색 결과

#### [!UICONTROL 레코드 나열]

이 검색 모듈은 특정 유형의 모든 레코드에 대한 정보를 검색합니다.

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Connection]</p> </td> 
   <td> <p>연결 방법에 대한 지침은 [!DNL Cvent] 계정 대상 [!DNL Workfront Fusion]를 참조하십시오. <a href="#connect-cvent-to-adobe-workfront-fusion" class="MCXref xref">Connect [!DNL Cvent] to [!DNL Adobe Workfront Fusion]</a> 참조하십시오.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL 레코드 유형]</p> </td> 
   <td> <p>나열할 레코드 유형을 선택합니다.</p> 
    <ul> 
     <li> <p>의 모든 이벤트 [!DNL Cvent] account</p> </li> 
     <li> <p>이벤트의 모든 세션</p> </li> 
     <li> <p>이벤트에 대한 모든 초대자</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL 이벤트 ID]</td> 
   <td> <p>초대자나 세션을 나열하는 경우 해당 초대자나 세션이 연결된 이벤트의 ID를 입력하거나 매핑합니다.</p> </td> 
  </tr> 
 </tbody> 
</table>
