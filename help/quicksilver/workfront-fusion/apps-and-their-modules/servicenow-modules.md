---
content-type: reference
product-previous: workfront-fusion
product-area: workfront-integrations
keywords: 커넥터
navigation-topic: apps-and-their-modules
title: ServiceNow 모듈
description: 에서 [!DNL Adobe Workfront Fusion] 시나리오, [!DNL ServiceNow]여러 타사 애플리케이션 및 서비스에 연결할 수 있습니다.
author: Becky
feature: Workfront Fusion
exl-id: b362cd8b-06b3-4f4c-b405-a2afc24abddb
source-git-commit: 885d93dd4383945538e977fd3edbfd55bda88b70
workflow-type: tm+mt
source-wordcount: '1565'
ht-degree: 0%

---

# [!DNL ServiceNow] 모듈

에서 [!DNL Adobe Workfront Fusion] 시나리오, [!DNL ServiceNow]여러 타사 애플리케이션 및 서비스에 연결할 수 있습니다.

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

를 사용하려면 [!DNL ServiceNow] 모듈이면 반드시 [!DNL ServiceNow] 계정이 필요합니다.

## Connect [!DNL ServiceNow] to [!DNL Workfront Fusion]

에 대한 연결을 만들려면 [!DNL ServiceNow] 모듈:

1. 클릭 **[!UICONTROL 추가]** 다음 [!UICONTROL 연결] 첫 번째 구성 시작 시 [!DNL ServiceNow] 모듈.
1. 다음을 입력합니다.

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader"> <p>[!UICONTROL 연결 이름]</p> </td> 
      <td>새 이름을 입력합니다 [!DNL ServiceNow] 연결</td> 
     </tr> 
     <tr> 
      <td role="rowheader"> <p>[!UICONTROL Username]</p> </td> 
      <td>을(를) 입력합니다. [!DNL ServiceNow] 사용자 이름.</td> 
     </tr> 
     <tr> 
      <td role="rowheader"> <p>[!UICONTROL Password]</p> </td> 
      <td>ServiceNow 암호를 입력합니다.</td> 
     </tr> 
     <tr> 
      <td role="rowheader"> <p>[!UICONTROL 인스턴스]</p> </td> 
      <td> <p>사용자의 주소를 입력합니다 [!DNL ServiceNow] 계정 없이 <code>https://</code> (일반적으로 <code>&lt;company>.service-now.com</code>).</p> </td> 
     </tr> 
    </tbody> 
   </table>

## [!UICONTROL ServiceNow] 모듈 및 해당 필드

구성 시 [!DNL ServiceNow] 모듈, [!DNL Workfront Fusion] 아래 나열된 필드를 표시합니다. 이와 함께 추가 [!DNL ServiceNow] 앱이나 서비스에서 액세스 수준과 같은 요소에 따라 필드가 표시될 수 있습니다. 모듈에서 굵게 표시된 제목은 필수 필드를 나타냅니다.

필드 또는 함수 위에 맵 단추가 표시되면 이 단추를 사용하여 해당 필드에 대한 변수와 함수를 설정할 수 있습니다. 자세한 내용은 [의 한 모듈에서 다른 모듈로 정보 매핑 [!DNL Adobe Workfront Fusion]](../../workfront-fusion/mapping/map-information-between-modules.md).

![](assets/map-toggle-350x74.png)

>[!NOTE]
>
>사용자 지정 레코드가 &quot;[!UICONTROL 레코드 유형]&quot; 필드를 사용하려면 사용자 지정 필드를 로드하는 데 시간이 걸릴 수 있습니다.
>
>사용자 지정 레코드가 없으면 드롭다운이 비어 있습니다.

* [[!UICONTROL 레코드 보기]](#watch-records)
* [[!UICONTROL 사용자 지정 API 호출]](#custom-api-call)
* [[!UICONTROL 레코드 읽기]](#read-a-record)
* [[!UICONTROL 사용자 비활성화]](#deactivate-a-user)
* [[!UICONTROL 첨부 파일 다운로드]](#download-an-attachment)
* [[!UICONTROL 첨부 파일 업로드]](#upload-an-attachment)
* [[!UICONTROL 레코드 만들기]](#create-a-record)
* [[!UICONTROL 레코드 업데이트]](#update-a-record)
* [[!UICONTROL 레코드 삭제]](#delete-a-record)
* [[!UICONTROL 레코드 검색]](#search-for-records)

### [!UICONTROL 레코드 보기]

이 트리거 모듈은 레코드가 만들어지거나 업데이트되면 시나리오를 활성화합니다.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td> 
   <td> <p>ServiceNow 계정 연결에 대한 지침은 [!DNL Workfront Fusion]를 참조하십시오. <a href="#connect-servicenow-to-workfront-fusion" class="MCXref xref">Connect [!DNL ServiceNow] [!UICONTROL Workfront Fusion] 변환</a> 참조하십시오.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL 테이블 유형]</td> 
   <td>보려는 테이블이 사용자 지정 테이블인지 표준 테이블인지를 선택합니다.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL 레코드 유형]</td> 
   <td>보려는 레코드 유형을 선택합니다.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Display]</td> 
   <td>표시할 값 유형을 선택합니다.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL 출력]</td> 
   <td>모듈을 출력할 필드를 선택합니다.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Filter]</td> 
   <td>새 레코드 또는 업데이트된 레코드를 보는지 여부를 선택합니다.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL 제한]</td> 
   <td> <p>각 시나리오 실행 주기 동안 모듈이 반환할 최대 레코드 수를 입력하거나 매핑합니다.</p> </td> 
  </tr> 
 </tbody> 
</table>

### [!UICONTROL 사용자 지정 API 호출]

이 작업 모듈을 사용하면 [!DNL ServiceNow] API. 이렇게 하면 다른 방식으로 수행할 수 없는 데이터 흐름 자동화를 만들 수 있습니다 [!DNL ServiceNow] 모듈.

이 모듈을 구성할 때 다음 필드가 표시됩니다.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td> 
   <td> <p>ServiceNow 계정 연결에 대한 지침은 [!DNL Workfront Fusion]를 참조하십시오. <a href="#connect-servicenow-to-workfront-fusion" class="MCXref xref">Connect [!DNL ServiceNow] [!UICONTROL Workfront Fusion] 변환</a> 참조하십시오.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL 상대 URL]</td> 
   <td> <p>모듈이 상호 작용할 웹 서버의 주소를 입력합니다.</p> <p>상대 URL을 입력할 수 있습니다. 즉, 프로토콜을 포함하지 않아도 됩니다(예: <code>http://</code>)을 클릭하여 제품에서 사용할 수 있습니다. 이는 상호 작용이 서버에서 발생함을 웹 서버에 알려줍니다.</p> <p>For example: <code>[!DNL /api/conversations].create</code></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL 메서드]</td> 
   td&gt; <p>API 호출을 구성하는 데 필요한 HTTP 요청 메서드를 선택합니다. 자세한 내용은 <a href="../../workfront-fusion/modules/http-request-methods.md" class="MCXref xref" data-mc-variable-override="">의 HTTP 요청 메서드 [!DNL Adobe Workfront Fusion]</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Headers]</td> 
   <td> <p>요청의 헤더를 표준 JSON 개체 형태로 추가합니다.</p> <p>For example, <code>{"Content-type":"application/json"}</code></p> </td> 
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

### [!UICONTROL 레코드 읽기]

이 작업 모듈은 [!DNL ServiceNow] 시스템 ID를 사용하여 기록합니다.

이 모듈은 연결에 액세스하는 사용자 지정 필드 및 값과 함께 레코드와 연결된 표준 필드를 반환합니다. 이 정보는 시나리오의 후속 모듈에 매핑할 수 있습니다.

이 모듈을 구성할 때 다음 필드가 표시됩니다.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td> 
   <td> <p>ServiceNow 계정 연결에 대한 지침은 [!DNL Workfront Fusion]를 참조하십시오. <a href="#connect-servicenow-to-workfront-fusion" class="MCXref xref">Connect [!DNL ServiceNow] [!UICONTROL Workfront Fusion] 변환</a> 참조하십시오.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Record System ID]</td> 
   <td>고유 번호를 입력하거나 매핑합니다 [!DNL ServiceNow] 모듈을 읽을 레코드의 ID입니다.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL 테이블 유형]</td> 
   <td>읽을 레코드가 사용자 지정 테이블에 있는지 표준 테이블에 있는지 여부를 선택합니다.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL 레코드 유형]</td> 
   <td>유형 선택 [!DNL ServiceNow] 모듈을 읽을 것인지 기록합니다.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Display]</td> 
   <td>표시할 값 유형을 선택합니다.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL 출력]</td> 
   <td>모듈을 출력할 필드를 선택합니다.</td> 
  </tr> 
 </tbody> 
</table>

### [!UICONTROL 사용자 비활성화]

이 작업 모듈은 사용자를 [!DNL ServiceNow] ( 시스템 ID 사용)

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td> 
   <td> <p>ServiceNow 계정 연결에 대한 지침은 [!DNL Workfront Fusion]를 참조하십시오. <a href="#connect-servicenow-to-workfront-fusion" class="MCXref xref">Connect [!DNL ServiceNow] [!UICONTROL Workfront Fusion] 변환</a> 참조하십시오.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL User System ID]</td> 
   <td> 고유 번호를 입력하거나 매핑합니다 [!DNL ServiceNow] 모듈을 비활성화할 사용자의 ID입니다.</td> 
  </tr> 
 </tbody> 
</table>

### [!UICONTROL 첨부 파일 다운로드]

이 작업 모듈은 [!DNL ServiceNow] 레코드.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td> 
   <td> <p>ServiceNow 계정 연결에 대한 지침은 [!DNL Workfront Fusion]를 참조하십시오. <a href="#connect-servicenow-to-workfront-fusion" class="MCXref xref">Connect [!DNL ServiceNow] [!UICONTROL Workfront Fusion] 변환</a> 참조하십시오.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL 첨부 파일 시스템 ID]</td> 
   <td> 고유 번호를 입력하거나 매핑합니다 [!DNL ServiceNow] 모듈을 다운로드할 첨부 파일의 ID입니다.</td> 
  </tr> 
 </tbody> 
</table>

### [!UICONTROL 첨부 파일 업로드]

이 작업 모듈은 첨부 파일을 [!DNL ServiceNow] 레코드.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td> 
   <td> <p>ServiceNow 계정 연결에 대한 지침은 [!DNL Workfront Fusion]를 참조하십시오. <a href="#connect-servicenow-to-workfront-fusion" class="MCXref xref">Connect [!DNL ServiceNow] [!UICONTROL Workfront Fusion] 변환</a> 참조하십시오.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL 테이블 이름]</td> 
   <td>첨부 파일을 업로드할 테이블의 이름을 입력하거나 매핑합니다.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL 시스템 ID]</td> 
   <td>고유 번호를 입력하거나 매핑합니다 [!DNL ServiceNow] 첨부 파일을 업로드할 시스템의 ID입니다.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL 파일 이름]</td> 
   <td>첨부 파일의 이름을 입력하거나 매핑합니다</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL File content]</td> 
   <td>업로드할 파일을 입력하거나 매핑합니다 [!DNL ServiceNow].</td> 
  </tr> 
 </tbody> 
</table>

### [!UICONTROL 레코드 만들기]

이 작업 모듈은 [!DNL ServiceNow] 레코드.

이 모듈을 구성할 때 다음 필드가 표시됩니다.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td> 
   <td> <p>ServiceNow 계정 연결에 대한 지침은 [!DNL Workfront Fusion]를 참조하십시오. <a href="#connect-servicenow-to-workfront-fusion" class="MCXref xref">Connect [!DNL ServiceNow] [!UICONTROL Workfront Fusion] 변환</a> 참조하십시오.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL 테이블 유형]</td> 
   <td>사용자 지정 테이블에서 레코드를 작성할지 표준 테이블에서 생성할지를 선택합니다.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL 레코드 유형]</td> 
   <td>유형 선택 [!DNL ServiceNow] 모듈이 만들 레코드를 기록합니다. 그런 다음 이 레코드 유형에 사용할 수 있는 필드를 채울 수 있습니다.</td> 
  </tr> 
 </tbody> 
</table>

### [!UICONTROL 레코드 업데이트]

이 작업 모듈은 [!DNL ServiceNow] 레코드.

이 모듈을 구성할 때 다음 필드가 표시됩니다.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td> 
   <td> <p>ServiceNow 계정 연결에 대한 지침은 [!DNL Workfront Fusion]를 참조하십시오. <a href="#connect-servicenow-to-workfront-fusion" class="MCXref xref">Connect [!DNL ServiceNow] [!UICONTROL Workfront Fusion] 변환</a> 참조하십시오.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Record System ID]</td> 
   <td>고유 번호를 입력하거나 매핑합니다 [!DNL ServiceNow] 모듈을 업데이트할 레코드의 ID입니다.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL 테이블 유형]</td> 
   <td>업데이트할 레코드가 사용자 지정 테이블에 있는지 표준 테이블에 있는지 여부를 선택합니다.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL 레코드 유형]</td> 
   <td>유형 선택 [!DNL ServiceNow] 모듈을 업데이트할 것을 기록하십시오. 그런 다음 이 레코드 유형에 사용할 수 있는 필드를 채울 수 있습니다.</td> 
  </tr> 
 </tbody> 
</table>

### [!UICONTROL 레코드 삭제]

이 작업 모듈은 인시던트 또는 사용자를 삭제합니다.

이 모듈을 구성할 때 다음 필드가 표시됩니다.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td> 
   <td> <p>ServiceNow 계정 연결에 대한 지침은 [!DNL Workfront Fusion]를 참조하십시오. <a href="#connect-servicenow-to-workfront-fusion" class="MCXref xref">Connect [!DNL ServiceNow] [!UICONTROL Workfront Fusion] 변환</a> 참조하십시오.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL 레코드 유형]</td> 
   <td>인시던트 또는 사용자를 삭제할 것인지 선택합니다.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL 시스템 ID]</td> 
   <td>고유 번호를 입력하거나 매핑합니다 [!DNL ServiceNow] 모듈을 삭제할 레코드의 ID입니다.</td> 
  </tr> 
 </tbody> 
</table>

### [!UICONTROL 레코드 검색]

이 모듈은 선택한 기준을 사용하여 레코드를 검색합니다.

이 모듈은 연결에 액세스하는 사용자 지정 필드 및 값과 함께 레코드와 연결된 표준 필드를 반환합니다. 이 정보는 시나리오의 후속 모듈에 매핑할 수 있습니다.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td> 
   <td> <p>ServiceNow 계정 연결에 대한 지침은 [!DNL Workfront Fusion]를 참조하십시오. <a href="#connect-servicenow-to-workfront-fusion" class="MCXref xref">Connect [!DNL ServiceNow] [!UICONTROL Workfront Fusion] 변환</a> 참조하십시오.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL 테이블 유형]</td> 
   <td>검색할 테이블이 사용자 지정 테이블인지 표준 테이블인지를 선택합니다.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL 레코드 유형]</td> 
   <td>검색할 레코드 유형을 선택합니다.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL 결과 집합]</td> 
   <td>모듈이 기준과 일치하는 모든 레코드를 반환할지 또는 일치하는 첫 번째 레코드만 반환할지 여부를 선택합니다. </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL 최대 레코드 수]</td> 
   <td> <p>각 시나리오 실행 주기 동안 모듈이 반환할 최대 레코드 수를 입력하거나 매핑합니다.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL 검색 유형]</td> 
   <td> <p>모듈을 실행할 검색 유형을 선택합니다</p> 
    <ul> 
     <li> <p><strong>[!UICONTROL Advanced query]</strong> </p> 
      <ul> 
       <li> <p>[!UICONTROL Search Query]</p> <p>사용자 정의 검색 쿼리를 입력합니다. 에 대한 자세한 정보 [!DNL ServiceNow] 사용자 정의 검색 쿼리, <a href="https://docs.servicenow.com/bundle/orlando-platform-user-interface/page/use/common-ui-elements/reference/r_OpAvailableFiltersQueries.html">ServiceNow 쿼리 설명서</a>.</p> </li> 
      </ul> </li> 
     <li> <p><strong>[!UICONTROL Simple]</strong> </p> 
      <ul> 
       <li> <p>[!UICONTROL Search Criteria]</p> <p>모듈을 검색할 기준을 입력합니다. 검색 필터 설정에 대한 자세한 내용은 <a href="../../workfront-fusion/scenarios/add-a-filter-to-a-scenario.md" class="MCXref xref">Adobe Workfront Fusion의 시나리오에 필터 추가</a>.</p> </li> 
       <li> <p>[!UICONTROL 정렬 기준]</p> <p>모듈에서 결과를 정렬할 필드와 오름차순 또는 내림차순으로 정렬할지 여부를 지정합니다.</p> </li> 
      </ul> </li> 
    </ul> <p> </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Display]</td> 
   <td>표시할 값 유형을 선택합니다.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL 출력]</td> 
   <td>모듈을 출력할 필드를 선택합니다.</td> 
  </tr> 
 </tbody> 
</table>
