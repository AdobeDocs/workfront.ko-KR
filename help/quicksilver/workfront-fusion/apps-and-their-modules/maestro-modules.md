---
content-type: reference
product-previous: workfront-fusion
product-area: workfront-integrations
keywords: 커넥터
navigation-topic: apps-and-their-modules
title: Adobe Maestro 모듈
description: 포함 [!DNL Adobe Maestro] 모듈, 다음을 시작할 수 있습니다. [!DNL Adobe Workfront Fusion] 의 이벤트를 기반으로 한 시나리오 [!DNL Adobe] Maestro 계정, 계약 및 기타 레코드를 생성, 읽기 또는 업데이트하고, 설정한 기준을 사용하여 레코드를 검색하고, 문서를 업로드합니다.
author: Becky
feature: Workfront Fusion
hide: true
hidefromtoc: true
source-git-commit: fe0c867b218879c1d0d969112eb62878782a40ad
workflow-type: tm+mt
source-wordcount: '1007'
ht-degree: 0%

---

# [!DNL Adobe Maestro] 모듈

포함 [!DNL Adobe Maestro] 모듈에서 이벤트가 Maestro에서 발생할 때 시나리오를 트리거할 수 있습니다. 또한 레코드를 생성, 읽기, 업데이트 및 삭제하거나 [!DNL Adobe Maestro] 계정입니다.

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

## 에 대한 연결 만들기 [!DNL Adobe Maestro]

에 대한 연결을 만들 수 있습니다. [!DNL Maestro] 내에서 직접 계정 [!DNL Workfront Fusion] 모듈.

1. 다음 중 하나 [!DNL Maestro] 앱 모듈에서 **[!UICONTROL 추가]** 다음 옆에 [!UICONTROL 연결] 상자.
1. 이 연결의 이름을 입력하십시오.
1. 프로덕션 환경에 연결할지 아니면 비프로덕션 환경에 연결할지 선택합니다.
1. 서비스 계정에 연결할지 또는 개인 계정에 연결할지 선택합니다.
1. 클릭 **[!UICONTROL SAML 로그인]** 를 클릭하여 연결을 만들고 모듈로 돌아갑니다.

## [!DNL Adobe Maestro] 모듈 및 해당 필드

### 이벤트 보기

이 트리거 모듈은 Maestro에서 레코드, 레코드 유형 또는 작업 영역이 생성, 업데이트 또는 삭제될 때 시나리오를 시작합니다.

<table style="table-layout:auto"> 
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">[!UICONTROL Webhook]</td>
      <td>사용할 웹후크를 선택하거나 추가 를 클릭하여 새 웹후크를 만듭니다.</td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Connection]</td>
      <td>에 대한 연결 만들기에 대한 지침: [!DNL Adobe Maestro], 참조 <a href="#create-a-connection-to-adobe-maestro" class="MCXref xref" >에 대한 연결 만들기 [!DNL Adobe Maestro]</a> 이 문서에서.</td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL 개체 유형]</td>
      <td>레코드, 레코드 종류 또는 작업 영역을 감시할지 여부를 선택합니다.</td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Objects to watch]</td>
      <td>새로운 항목을 감시할지 여부를 선택합니다. 업데이트, 새 레코드 및 업데이트 또는 삭제된 레코드.</td>
    </tr>
     <tr>
      <td role="rowheader">
        <p>[!UICONTROL 이 연결에 의해 수행된 업데이트 제외]</p>
      </td>
      <td>이 모듈에서 사용한 연결에 의해 변경이 있을 때 시나리오가 트리거되지 않도록 하려면 이 옵션을 활성화합니다. 이렇게 하면 이 시나리오가 트리거 작업을 수행하는 경우 시나리오의 다른 인스턴스가 트리거되지 않습니다.</td> 
      </tr>
  </tbody>
</table>

### 레코드 유형 삭제

이 작업 모듈은 해당 ID로 Maestro의 단일 레코드 유형을 삭제합니다.

>[!WARNING]
>
>Maestro에서 레코드 유형을 삭제하면 레코드 유형 테이블의 모든 레코드도 삭제됩니다.

<table style="table-layout:auto"> 
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">[!UICONTROL Connection]</td>
      <td>에 대한 연결 만들기에 대한 지침: [!DNL Adobe Maestro], 참조 <a href="#create-a-connection-to-adobe-maestro" class="MCXref xref" >에 대한 연결 만들기 [!DNL Adobe Maestro]</a> 이 문서에서.</td>
    </tr>
     <tr>
      <td role="rowheader">
        <p>[!UICONTROL 레코드 유형 ID]</p>
      </td>
      <td>삭제할 필드의 ID를 입력하거나 매핑합니다.</td> 
      </tr>
  </tbody>
</table>

### 사용자 지정 API 호출 만들기

이 모듈에서는에 대한 사용자 지정 API 호출을 만듭니다. [!DNL Adobe Maestro] API.

<table style="table-layout:auto"> 
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">[!UICONTROL Connection]</td>
      <td>에 대한 연결 만들기에 대한 지침: [!DNL Adobe Maestro], 참조 <a href="#create-a-connection-to-adobe-maestro" class="MCXref xref" >에 대한 연결 만들기 [!DNL Adobe Maestro]</a> 이 문서에서.</td>
    </tr>
     <tr>
      <td role="rowheader">
        <p>[!UICONTROL 경로]</p>
      </td>
      <td>
        <p>https://&lt;WORKFRONT_DOMAIN&gt;/attask/api/&lt;API_VERSION&gt;/ 관련 경로 입력</p>
      </td>
    </tr>
     <tr>
      <td role="rowheader">
        <p>[!UICONTROL API version]</p>
      </td>
      <td>
        <p>사용할 API 버전을 선택합니다. 버전을 선택하지 않으면 기본적으로 최신 버전이 사용됩니다.</p>
      </td>
    </tr>
     <tr>
      <td role="rowheader">
        <p>[!UICONTROL API 경로 재정의]</p>
      </td>
      <td>
        <p>https://&lt;WORKFRONT_DOMAIN&gt;/attask/api/&lt;API_VERSION&gt;/ 관련 경로 입력</p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">
        <p>[!UICONTROL 메서드]</p>
      </td>
   <td> <p>API 호출을 구성하는 데 필요한 HTTP 요청 메서드를 선택합니다. 자세한 내용은 <a href="../../workfront-fusion/modules/http-request-methods.md" class="MCXref xref" data-mc-variable-override="">의 HTTP 요청 메서드 [!DNL Adobe Workfront Fusion]</a>.</p> </td> 
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Headers]</td>
      <td>
        <p>표준 JSON 개체 형태로 요청의 헤더를 추가합니다.</p>
        <p>For example, <code>{"Content-type":"application/json"}</code></p>
        <p>[!DNL Workfront Fusion] 인증 헤더를 자동으로 추가합니다.</p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL 쿼리 문자열]  </td>
      <td>
        <p>쿼리 문자열에 추가할 각 키/값 쌍에 대해 <b>항목 추가</b> 키와 값을 입력합니다.</p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Body]</td>
   <td> <p>표준 JSON 개체의 형태로 API 호출에 대한 본문 콘텐츠를 추가합니다.</p> <p>참고:  <p>다음과 같은 조건문을 사용할 때 <code>if</code> json에서 따옴표를 조건문 외부에 넣습니다.</p> 
     <div class="example" data-mc-autonum="<b>Example: </b>"> 
      <p> <img src="assets/quotes-in-json-350x120.png" style="width: 350;height: 120;"> </p> 
     </div> </p> </td>     </tr>
  </tbody>
</table>

<!--

### Delete a field

This action module deletes a single field in Maestro by its ID.

>[!WARNING]
>
>Deleting a field in Maestro deletes it and any data in it from every object of that record type in Maestro.

<table style="table-layout:auto"> 
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">[!UICONTROL Connection]</td>
      <td>For instructions on creating a connection to [!DNL Adobe Maestro], see <a href="#create-a-connection-to-adobe-maestro" class="MCXref xref" >Create a connection to [!DNL Adobe Maestro]</a> in this article.</td>
    </tr>
     <tr>
      <td role="rowheader">
        <p>[!UICONTROL Field ID]</p>
      </td>
      <td>Enter or map the ID of the record type you want to delete.</td> 
      </tr>
  </tbody>
</table>

### Get a field 


This action module retrieves a single field in Maestro by its ID.

<table style="table-layout:auto"> 
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">[!UICONTROL Connection]</td>
      <td>For instructions on creating a connection to [!DNL Adobe Maestro], see <a href="#create-a-connection-to-adobe-maestro" class="MCXref xref" >Create a connection to [!DNL Adobe Maestro]</a> in this article.</td>
    </tr>
     <tr>
      <td role="rowheader">
        <p>[!UICONTROL Field ID]</p>
      </td>
      <td>Enter or map the ID of the field you want to delete.</td> 
      </tr>
  </tbody>
</table>

-->

### 레코드 만들기

이 작업은 Maestro에서 단일 레코드를 만듭니다.

<table style="table-layout:auto"> 
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">[!UICONTROL Connection]</td>
      <td>에 대한 연결 만들기에 대한 지침: [!DNL Adobe Maestro], 참조 <a href="#create-a-connection-to-adobe-maestro" class="MCXref xref" >에 대한 연결 만들기 [!DNL Adobe Maestro]</a> 이 문서에서.</td>
    </tr>
     <tr>
      <td role="rowheader">
        <p>[!UICONTROL 레코드 유형 ID]</p>
      </td>
      <td>생성할 레코드 유형을 입력하거나 매핑합니다. 사용 가능한 레코드 유형은 Maestro 계정을 기반으로 합니다.</td> 
      </tr>
     <tr>
      <td role="rowheader">
        <p>기타 필드</p>
      </td>
      <td>이 필드는 선택한 레코드 종류를 기반으로 합니다.</td> 
      </tr>
     <tr>
  </tbody>
</table>

### 레코드 삭제

이 작업 모듈은 Maestro에서 지정된 레코드를 삭제합니다.

<table style="table-layout:auto"> 
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">[!UICONTROL Connection]</td>
      <td>에 대한 연결 만들기에 대한 지침: [!DNL Adobe Maestro], 참조 <a href="#create-a-connection-to-adobe-maestro" class="MCXref xref" >에 대한 연결 만들기 [!DNL Adobe Maestro]</a> 이 문서에서.</td>
    </tr>
     <tr>
      <td role="rowheader">
        <p>[!UICONTROL 레코드 ID]</p>
      </td>
      <td>삭제할 레코드의 ID를 입력하거나 매핑합니다.</td> 
      </tr>
  </tbody>
</table>

<!--

### Get all records

This action module retrieves all records from an [!DNL Adobe Maestro] account.

<table style="table-layout:auto"> 
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">[!UICONTROL Connection]</td>
      <td>For instructions on creating a connection to [!DNL Adobe Maestro], see <a href="#create-a-connection-to-adobe-maestro" class="MCXref xref" >Create a connection to [!DNL Adobe Maestro]</a> in this article.</td>
    </tr>
     <tr>
      <td role="rowheader">
        <p>[!UICONTROL Maximum number of returned records]</p>
      </td>
      <td>Enter or map the maximum number of records you want the module to return during each scenario execution cycle.</td> 
      </tr>
  </tbody>
</table>

-->

### 레코드 가져오기

이 작업 모듈은에서 단일 레코드를 검색합니다. [!DNL Adobe Maestro], 해당 ID로 지정됩니다.

<table style="table-layout:auto"> 
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">[!UICONTROL Connection]</td>
      <td>에 대한 연결 만들기에 대한 지침: [!DNL Adobe Maestro], 참조 <a href="#create-a-connection-to-adobe-maestro" class="MCXref xref" >에 대한 연결 만들기 [!DNL Adobe Maestro]</a> 이 문서에서.</td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL 레코드 ID]</td>
      <td>검색할 레코드의 ID를 입력하거나 매핑합니다.</td>
    </tr>
  </tbody>
</table>

### 레코드 유형별 레코드 가져오기

이 작업 모듈은 지정된 유형의 모든 레코드를 검색합니다.

<table style="table-layout:auto"> 
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">[!UICONTROL Connection]</td>
      <td>에 대한 연결 만들기에 대한 지침: [!DNL Adobe Maestro], 참조 <a href="#create-a-connection-to-adobe-maestro" class="MCXref xref" >에 대한 연결 만들기 [!DNL Adobe Maestro]</a> 이 문서에서.</td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL 작업 영역]</td>
      <td>검색할 레코드가 포함된 작업 영역을 선택하거나 매핑합니다.</td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL 레코드 유형]</td>
      <td>검색할 레코드 유형을 선택합니다.</td>
    </tr>
     <tr>
      <td role="rowheader">
        <p>[!UICONTROL 반환되는 최대 레코드 수]</p>
      </td>
      <td>각 시나리오 실행 주기 동안 모듈이 반환할 최대 레코드 수를 입력하거나 매핑합니다.</td> 
  </tbody>
</table>

### 레코드 유형 가져오기

이 작업 모듈은 의 레코드 유형 목록을 검색합니다. [!DNL Adobe Maestro] 계정입니다.

<table style="table-layout:auto"> 
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">[!UICONTROL Connection]</td>
      <td>에 대한 연결 만들기에 대한 지침: [!DNL Adobe Maestro], 참조 <a href="#create-a-connection-to-adobe-maestro" class="MCXref xref" >에 대한 연결 만들기 [!DNL Adobe Maestro]</a> 이 문서에서.</td>
    </tr>
  </tbody>
</table>

### 레코드 업데이트

이 작업은 Maestro의 단일 레코드를 업데이트합니다.

<table style="table-layout:auto"> 
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">[!UICONTROL Connection]</td>
      <td>에 대한 연결 만들기에 대한 지침: [!DNL Adobe Maestro], 참조 <a href="#create-a-connection-to-adobe-maestro" class="MCXref xref" >에 대한 연결 만들기 [!DNL Adobe Maestro]</a> 이 문서에서.</td>
    </tr>
     <tr>
      <td role="rowheader">
        <p>[!UICONTROL 레코드 ID]</p>
      </td>
      <td>업데이트할 레코드 유형을 입력하거나 매핑합니다. 사용 가능한 레코드 유형은 Maestro 계정을 기반으로 합니다.</td> 
      </tr>
     <tr>
      <td role="rowheader">
        <p>기타 필드</p>
      </td>
      <td>이 필드는 선택한 레코드 종류를 기반으로 합니다.</td> 
      </tr>
     <tr>
  </tbody>
</table>

### 레코드 검색

이 작업 모듈은 지정한 조건에 따라 레코드 목록을 검색합니다.

>[!NOTE]
>
>이 모듈은 제작 중입니다.

