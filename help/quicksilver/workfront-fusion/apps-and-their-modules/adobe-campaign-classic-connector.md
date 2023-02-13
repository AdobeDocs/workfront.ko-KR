---
content-type: reference
product-previous: workfront-fusion
product-area: workfront-integrations
keywords: 커넥터
navigation-topic: apps-and-their-modules
title: Adobe Campaign Classic 모듈
description: 사용 [!DNL Adobe Campaign Classic] 모듈, 시작 [!DNL Adobe Workfront Fusion] 시나리오의 이벤트 기반 [!DNL Adobe Campaign Classic] 계정, 계약 및 기타 레코드를 생성, 읽기 또는 갱신하고 설정한 기준을 사용하여 레코드를 검색하고 문서를 업로드합니다.
author: Becky
feature: Workfront Fusion
exl-id: 84e8fa35-0c3c-46bd-8886-88c6d8d9e1d5
source-git-commit: 885d93dd4383945538e977fd3edbfd55bda88b70
workflow-type: tm+mt
source-wordcount: '1146'
ht-degree: 1%

---

# [!DNL Adobe Campaign Classic] 모듈

사용 [!DNL Adobe Campaign Classic] 모듈, 시작 [!DNL Adobe Workfront Fusion] 시나리오의 이벤트 기반 [!DNL Adobe Campaign Classic] 계정, 레코드 생성, 읽기 또는 업데이트, 설정한 기준을 사용하여 레코드 검색, 사용자 지정 API 호출 수행

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
   <td> <p>[!UICONTROL [!DNL Workfront Fusion] 작업 자동화 및 통합을 위한] </p>  </td> 
  </tr> 
  <tr> 
   <td role="rowheader">제품</td> 
   <td>조직이 구매해야 합니다 [!DNL Adobe Workfront Fusion] 뿐만 아니라 [!DNL Adobe Workfront] 을 참조하십시오.</td> 
  </tr> 
 </tbody> 
</table>

어떤 계획, 라이센스 유형 또는 액세스 권한을 보유하고 있는지 확인하려면 [!DNL Workfront] 관리자

에 대한 자세한 정보 [!DNL Adobe Workfront Fusion] 라이센스 [[!DNL Adobe Workfront Fusion] 라이선스](../../workfront-fusion/get-started/license-automation-vs-integration.md).

## Connect [!DNL Adobe Campaign Classic] to [!DNL Adobe Workfront Fusion]

1. 어떤 경우에서도 [!DNL Adobe Campaign Classic] 모듈 **[!UICONTROL 추가]** 다음 [!UICONTROL 연결] 필드.
1. 연결에 사용할 기본 URL을 입력합니다 [!DNL Adobe Campaign Classic] 인스턴스.
1. 사용자 이름과 암호를 입력합니다.
1. 클릭 **[!UICONTROL 계속]** 연결을 만들고 모듈로 돌아갑니다.

## [!DNL Adobe Campaign Classic] 모듈 및 해당 필드

구성 시 [!DNL Adobe Campaign Classic] 모듈, [!DNL Workfront Fusion] 아래 나열된 필드를 표시합니다. 이와 함께 추가 [!DNL Adobe Campaign Classic] 앱이나 서비스에서 액세스 수준과 같은 요소에 따라 필드가 표시될 수 있습니다. 모듈에서 굵게 표시된 제목은 필수 필드를 나타냅니다.

필드 또는 함수 위에 맵 단추가 표시되면 이 단추를 사용하여 해당 필드에 대한 변수와 함수를 설정할 수 있습니다. 자세한 내용은 [의 한 모듈에서 다른 모듈로 정보 매핑 [!DNL Adobe Workfront Fusion]](../../workfront-fusion/mapping/map-information-between-modules.md).

![](assets/map-toggle-350x74.png)

* [Triggers](#triggers)
* [액션](#actions)
* [검색 결과](#searches)

### Triggers

#### [!UICONTROL 레코드 보기]

이 예약된 트리거 모듈은 레코드가 변경될 때 시나리오를 시작합니다.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td> 
   <td>연결 생성에 대한 지침은 [!DNL Adobe Campaign Classic]를 참조하십시오. <a href="#connect-adobe-campaign-connector-to-adobe-workfront-fusion" class="MCXref xref" >연결 만들기 [!DNL Adobe Campaign Classic]</a> 참조하십시오.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Filter]</td> 
   <td>새 레코드, 업데이트된 레코드 또는 둘 다를 감시할지 여부를 선택합니다.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Resource]</td> 
   <td>감시하려는 리소스를 선택합니다.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL 출력에 포함할 필드]</td> 
   <td>모듈의 출력에 포함할 필드를 선택합니다.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL 출력에 포함할 사용자 지정 필드]</td> 
   <td>출력에 포함할 각 사용자 지정 필드에 대해 <b>[!UICONTROL Add]</b> 사용자 정의 필드의 이름을 입력합니다.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL 반환된 최대 결과 수]</td> 
   <td>각 시나리오 실행 주기 동안 모듈이 반환할 최대 레코드 수를 입력하거나 매핑합니다.</td> 
  </tr> 
 </tbody> 
</table>


### 액션

* [[!UICONTROL 레코드 만들기]](#create-a-record)
* [[!UICONTROL 사용자 지정 API 호출 만들기]](#make-a-custom-api-call)
* [[!UICONTROL 레코드 삭제]](#delete-record)
* [[!UICONTROL 작업 수행]](#perform-an-action)
* [[!UICONTROL 레코드 읽기]](#-read-a-record)
* [[!UICONTROL 구독 또는 구독 취소]](#subscribe-or-unsubscribe)
* [[!UICONTROL 레코드 업데이트]](#update-record)

#### [!UICONTROL 레코드 만들기]

이 작업 모듈은 [!DNL Adobe Campaign Classic].

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td>
   <td>연결 생성에 대한 지침은 [!DNL Adobe Campaign Classic]를 참조하십시오. <a href="#connect-adobe-campaign-connector-to-adobe-workfront-fusion" class="MCXref xref" >연결 만들기 [!DNL Adobe Campaign Classic]</a> 참조하십시오.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Resource]</td> 
   <td>유형 선택 [!DNL Adobe Campaign Classic] 만들 레코드.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Fields] </td> 
   <td>레코드를 만들 때 값을 설정할 필드를 선택한 다음 해당 필드의 값을 채웁니다. 필드는 선택한 레코드 유형에 따라 다릅니다.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL 사용자 지정 필드]</td> 
   <td> 새 레코드에 추가할 각 사용자 지정 필드에 대해 <b>[!UICONTROL 항목 추가]</b> 필드의 이름과 값을 입력하거나 매핑합니다. </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL 사용자 지정 API 호출 만들기]

이 모듈은 [!DNL Adobe Campaign Classic] API

<table style="table-layout:auto"> 
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">[!UICONTROL Connection]</td>
   <td>연결 생성에 대한 지침은 [!DNL Adobe Campaign Classic]를 참조하십시오. <a href="#connect-adobe-campaign-connector-to-adobe-workfront-fusion" class="MCXref xref" >연결 만들기 [!DNL Adobe Campaign Classic]</a> 참조하십시오.</td> 
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Action]</td>
      <td><p>API 호출이 수행할 작업을 선택합니다.</p>
      <p>[!UICONTROL 쿼리 실행]</p>
      <p>[!UICONTROL Write]</p>
      <p>[!UICONTROL 최근 엔터티를 가져오는 경우]</p>
      <p>[!UICONTROL 모두 선택]</p>
      <p>[!UICONTROL 푸시 이벤트]</p>
    </td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Headers]</td>
      <td>
        <p>요청의 헤더를 표준 JSON 개체 형태로 추가합니다.</p>
        <p>For example, <code>{"Content-type":"application/json"}</code></p>
        <p>[!DNL Workfront Fusion] [!UICONTROL x-security] 토큰 헤더를 자동으로 추가합니다.</p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL XML Body]</td>
   <td> <p>세션 요소 없이 XML에서 API 호출에 대한 본문 콘텐츠를 추가합니다. </td>     </tr>
  </tbody>
</table>

#### [!UICONTROL 레코드 삭제]

이 작업 모듈은 [!DNL Adobe Campaign Classic].

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td>
   <td>연결 생성에 대한 지침은 [!DNL Adobe Campaign Classic]를 참조하십시오. <a href="#connect-adobe-campaign-connector-to-adobe-workfront-fusion" class="MCXref xref" >연결 만들기 [!DNL Adobe Campaign Classic]</a> 참조하십시오.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Resource]</td> 
   <td>삭제할 리소스 유형을 선택합니다.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL ID]</td> 
   <td>삭제할 리소스의 ID를 입력하거나 매핑합니다.</td> 
  </tr> 
 </tbody> 
</table>


#### [!UICONTROL 작업 수행]

이 작업 모듈은 [!DNL Adobe Campaign Classic] API.

특정 작업 및 필드에 대한 자세한 내용은 [[!DNL Adobe Campaign] - API 설명서](https://experienceleague.adobe.com/developer/campaign-api/api/p-14.html).

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td>
   <td>연결 생성에 대한 지침은 [!DNL Adobe Campaign Classic]를 참조하십시오. <a href="#connect-adobe-campaign-connector-to-adobe-workfront-fusion" class="MCXref xref" >연결 만들기 [!DNL Adobe Campaign Classic]</a> 참조하십시오.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Action]</td> 
   <td><p>객체에 대해 수행할 작업을 선택합니다.</p>
   <ul>
   <li><p><b>[!DNL List]</b></p><p> 사용 가능한 필드에 대해서는 <a href="#search" class="MCXref xref" >[!UICONTROL Search]</a> 참조하십시오. </p></li>
     <li><p><b>[!UICONTROL Get]</b></p><p> 사용 가능한 필드에 대해서는 <a href="#search" class="MCXref xref" >[!UICONTROL Search]</a> 참조하십시오. </p></li> 
   <li><p><b>[!UICONTROL Create]</b></p><p> 사용 가능한 필드에 대해서는 <a href="#create-a-record" class="MCXref xref" >[!UICONTROL 레코드 만들기]</a> 참조하십시오. </p></li>
   <li><p><b>[!UICONTROL 업데이트]</b></p><p> 사용 가능한 필드에 대해서는 <a href="#update-record" class="MCXref xref" >[!UICONTROL 레코드 업데이트]</a> 참조하십시오. </p></li>
   <li><p><b>[!UICONTROL Delete]</b></p><p> 사용 가능한 필드에 대해서는 <a href="#delete-record" class="MCXref xref" >[!UICONTROL 레코드 삭제]</a> 참조하십시오. </p></li>
   </ul>
   </td>
</tr> 
 </tbody> 
</table>

#### [!UICONTROL 레코드 읽기]

이 작업 모듈은 레코드를 [!DNL Adobe Campaign Classic].

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td>
   <td>연결 생성에 대한 지침은 [!DNL Adobe Campaign Classic]를 참조하십시오. <a href="#connect-adobe-campaign-connector-to-adobe-workfront-fusion" class="MCXref xref" >연결 만들기 [!DNL Adobe Campaign Classic]</a> 참조하십시오.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Resource]</td> 
   <td>유형 선택 [!DNL Adobe Campaign Classic] 읽을 레코드</td> 
  </tr> 
    <tr> 
   <td role="rowheader">[!UICONTROL ID] </td> 
   <td>읽을 레코드의 ID를 매핑의 입력합니다.</td> 
  </tr> 
 <tr> 
   <td role="rowheader">[!UICONTROL 출력에 포함할 필드] </td> 
   <td>모듈의 출력에 포함할 필드를 선택합니다.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL 출력에 포함할 사용자 지정 필드]</td> 
   <td>출력에 포함할 각 사용자 지정 필드에 대해 <b>[!UICONTROL Add]</b> 사용자 정의 필드의 이름을 입력합니다.</td> 
  </tr> 
 </tbody> 
</table>


#### [!UICONTROL 구독 또는 구독 취소]

이 작업 모듈은 정보 서비스에 사용자를 가입시키거나 사용자 가입을 해지합니다.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td>
   <td>연결 생성에 대한 지침은 [!DNL Adobe Campaign Classic]를 참조하십시오. <a href="#connect-adobe-campaign-connector-to-adobe-workfront-fusion" class="MCXref xref" >연결 만들기 [!DNL Adobe Campaign Classic]</a> 참조하십시오.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL 가입 또는 가입 해지]</td> 
   <td>정보 서비스의 구독 또는 구독 취소 여부를 선택합니다.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL 서비스 이름]</td> 
   <td>가입하거나 가입을 해지할 서비스를 선택합니다.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Recipient email address] </td> 
   <td>정보 서비스를 구독하거나 구독을 취소할 사용자의 이메일 주소를 입력하거나 매핑합니다.</td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL 레코드 업데이트]

이 작업 모듈은 [!DNL Adobe Campaign Classic].

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td>
   <td>연결 생성에 대한 지침은 [!DNL Adobe Campaign Classic]를 참조하십시오. <a href="#connect-adobe-campaign-connector-to-adobe-workfront-fusion" class="MCXref xref" >연결 만들기 [!DNL Adobe Campaign Classic]</a> 참조하십시오.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Resource]</td> 
   <td>유형 선택 [!DNL Adobe Campaign Classic] 만들 레코드.</td> 
  </tr> 
    <tr> 
   <td role="rowheader">[!UICONTROL ID] </td> 
   <td>업데이트할 레코드의 ID를 매핑의 입력합니다.</td> 
  </tr> 
<tr> 
   <td role="rowheader">[!UICONTROL Fields] </td> 
   <td>값을 업데이트할 필드를 선택한 다음 해당 필드의 값을 입력합니다. 필드는 선택한 레코드 유형에 따라 다릅니다.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL 사용자 지정 필드]</td> 
   <td> 업데이트할 각 사용자 지정 필드에 대해 <b>[!UICONTROL 항목 추가]</b> 필드의 이름과 값을 입력하거나 매핑합니다. </td> 
  </tr> 
 </tbody> 
</table>

### 검색 결과

#### [!UICONTROL 검색]

이 검색 모듈은 지정된 기준에 따라 레코드를 반환합니다.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td>
   <td>연결 생성에 대한 지침은 [!DNL Adobe Campaign Classic]를 참조하십시오. <a href="#connect-adobe-campaign-connector-to-adobe-workfront-fusion" class="MCXref xref" >연결 만들기 [!DNL Adobe Campaign Classic]</a> 참조하십시오.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Resource]</td> 
   <td>유형 선택 [!DNL Adobe Campaign Classic] 만들 레코드.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL 제한] </td> 
   <td>각 시나리오 실행 주기 동안 모듈이 반환할 최대 레코드 수를 입력하거나 매핑합니다.</td> 
  </tr> 
 </tbody> 
</table>
