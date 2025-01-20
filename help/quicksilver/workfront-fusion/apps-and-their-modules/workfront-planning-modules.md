---
content-type: reference
product-previous: workfront-fusion
product-area: workfront-integrations
keywords: 커넥터
navigation-topic: apps-and-their-modules
title: Adobe Workfront Planning 모듈
description: Adobe Workfront Fusion 설명서가 새 위치로 이동했습니다. 이 문서는 더 이상 사용되지 않지만, 이 기능을 다루는 새 문서에 대한 링크를 포함합니다.
author: Becky
feature: Workfront Fusion
hide: true
hidefromtoc: true
exl-id: 892fdaf3-935e-4e66-a01c-9e9b6e0daf3e
source-git-commit: efbe888d370e20c895dc40f18f999f2d01ec6337
workflow-type: tm+mt
source-wordcount: '1207'
ht-degree: 0%

---

# [!DNL Adobe Workfront Planning]개 모듈

>[!IMPORTANT]
>
>Adobe Workfront Fusion 설명서가 새 위치로 이동했습니다.
>
>이 문서의 정보는 이제 문서에서 찾을 수 있습니다.
>
>* [Adobe Workfront 계획 모듈](https://experienceleague.adobe.com/docs/workfront-fusion/using/references/apps-and-their-modules/adobe-connectors/workfront-planning-modules.html)
>
>모든 책갈피를 업데이트하십시오.
>
>이 문서는 더 이상 업데이트되지 않으며 곧 제거될 예정입니다.

[!DNL Adobe Workfront Planning] 모듈을 사용하면 Workfront Planning에서 이벤트가 발생할 때 시나리오를 트리거할 수 있습니다. 레코드를 만들고, 읽고, 업데이트하고 삭제하거나 [!DNL Adobe Workfront Planning] 계정에 대한 사용자 지정 API 호출을 수행할 수도 있습니다.

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

## Adobe Workfront Planning API 정보

Adobe Workfront Planning 커넥터는 다음을 사용합니다.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">기본 URL</td> 
   <td>https://&lbrace;&lbrace;connection.host&rbrace;&rbrace;/maestro/api/&lbrace;&lbrace;common.maestroApiVersion&rbrace;&rbrace;/</td> 
  </tr>
  <tr> 
   <td role="rowheader">API 태그</td> 
   <td>v1.13.7</td> 
  </tr>
 </tbody> 
 </table>

## [!DNL Adobe Workfront Planning]에 연결 만들기

[!DNL Workfront Fusion] 모듈 내에서 직접 [!DNL Workfront Planning] 계정에 연결할 수 있습니다.

1. [!DNL Adobe Workfront Planning] 모듈에서 [연결] 상자 옆에 있는 **[!UICONTROL 추가]**&#x200B;를 클릭합니다.

1. 다음 필드를 채웁니다.

   <table style="table-layout:auto"> 
      <col class="TableStyle-TableStyle-List-options-in-steps-Column-Column1">
      </col>
      <col class="TableStyle-TableStyle-List-options-in-steps-Column-Column2">
      </col>
      <tbody>
        <tr>
          <td role="rowheader">[!UICONTROL 연결 이름]</td>
          <td>
            <p>이 연결의 이름을 입력하십시오.</p>
          </td>
        </tr>
        <tr>
          <td role="rowheader">[!UICONTROL 환경]</td>
          <td>프로덕션 환경에 연결할지 아니면 비프로덕션 환경에 연결할지 선택합니다.</td>
        </tr>
        <tr>
          <td role="rowheader">[!UICONTROL 유형]</td>
          <td>서비스 계정에 연결할지 개인 계정에 연결할지 선택합니다.</td>
        </tr>
        <tr>
          <td role="rowheader">[!UICONTROL 클라이언트 ID]<p>(선택 사항)</p></td>
          <td>[!DNL Adobe] [!UICONTROL 클라이언트 ID]를 입력하십시오. 이는 [!DNL Adobe Developer Console]의 [!UICONTROL 자격 증명 세부 정보] 섹션에서 찾을 수 있습니다.</td>
        </tr>
        <tr>
          <td role="rowheader">[!UICONTROL 클라이언트 암호]<p>(선택 사항)</p></td>
          <td>[!DNL Adobe] [!UICONTROL 클라이언트 암호]를 입력하십시오. 이는 [!DNL Adobe Developer Console]의 [!UICONTROL 자격 증명 세부 정보] 섹션에서 찾을 수 있습니다.
        </tr>
        <tr>
          <td role="rowheader">[!UICONTROL 인증 URL]<p>(선택 사항)</p></td>
          <td>Workfront 인스턴스가 이 연결을 인증하는 데 사용할 URL을 입력하십시오. <p>기본값은 <code>https://oauth.my.workfront.com/integrations/oauth2</code>입니다.</p>
        </tr>
        <tr>
          <td role="rowheader">[!UICONTROL 호스트 접두사]</td>
          <td>호스트 접두사를 입력합니다.<p>기본값은 <code>origin-</code>입니다.</p>
        </tr>
      </tbody>
    </table>
1. 연결을 저장하고 모듈로 돌아가려면 **[!UICONTROL 계속]**&#x200B;을 클릭하세요.

## [!DNL Adobe Workfront Planning]개 모듈 및 해당 필드

### 트리거

#### 이벤트 보기

이 트리거 모듈은 기록, 레코드 유형 또는 작업 영역이 Workfront Planning에서 생성, 업데이트 또는 삭제될 때 시나리오를 시작합니다.

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
      <td>[!DNL Adobe Workfront Planning]에 대한 연결을 만드는 방법에 대한 지침은 이 문서에서 <a href="#create-a-connection-to-adobe-workfront planning" class="MCXref xref" >[!DNL Adobe Workfront Planning]</a>에 대한 연결 만들기 를 참조하십시오.</td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL 개체 유형]</td>
      <td>레코드, 레코드 종류 또는 작업 영역을 감시할지 여부를 선택합니다.</td>
    </tr>
     <tr data-mc-conditions=""> 
      <td> <p>[!UICONTROL 이벤트 필터]</p> </td> 
      <td> <p>선택한 기준을 충족하는 레코드만 보도록 필터를 설정할 수 있습니다.</p> <p>각 필터에 대해 필터를 평가할 필드, 연산자 및 필터를 허용할 값을 입력합니다. AND 규칙을 추가하여 두 개 이상의 필터를 사용할 수 있습니다.</p> <p>참고: 기존 [!DNL Workfront] 웹후크에서 필터를 편집할 수 없습니다. [!DNL Workfront] 이벤트 구독에 대해 다른 필터를 설정하려면 현재 웹후크를 제거하고 새 필터를 만드십시오.</p> <p>이벤트 필터에 대한 자세한 내용은 Workfront 모듈 문서의 [!DNL Workfront] &gt; [!UICONTROL Watch Events] 모듈에서 <a href="/help/quicksilver/workfront-fusion/apps-and-their-modules/workfront-modules.md#event-subscription-filters-in-the-workfront--watch-events-modules" class="MCXref xref">이벤트 구독 필터</a>를 참조하십시오.</p> </td> 
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

### 액션

* [레코드 유형 삭제](#delete-a-record-type)
* [사용자 정의 AI 호출 만들기](#make-a-custom-api-call)

#### 레코드 유형 삭제

이 작업 모듈은 해당 ID로 Workfront Planning에서 단일 레코드 유형을 삭제합니다.

>[!WARNING]
>
>Workfront Planning에서 레코드 유형을 삭제하면 레코드 유형 테이블의 모든 레코드도 삭제됩니다.

<table style="table-layout:auto"> 
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">[!UICONTROL Connection]</td>
      <td>[!DNL Adobe Workfront Planning]에 대한 연결을 만드는 방법에 대한 지침은 이 문서에서 <a href="#create-a-connection-to-adobe-workfront planning" class="MCXref xref" >[!DNL Adobe Workfront Planning]</a>에 대한 연결 만들기 를 참조하십시오.</td>
    </tr>
     <tr>
      <td role="rowheader">
        <p>[!UICONTROL 레코드 유형 ID]</p>
      </td>
      <td>삭제할 필드의 ID를 입력하거나 매핑합니다.</td> 
      </tr>
  </tbody>
</table>

#### 사용자 지정 API 호출 만들기

이 모듈은 [!DNL Adobe Workfront Planning] API에 대한 사용자 지정 API 호출을 만듭니다.

<table style="table-layout:auto"> 
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">[!UICONTROL Connection]</td>
      <td>[!DNL Adobe Workfront Planning]에 대한 연결을 만드는 방법에 대한 지침은 이 문서에서 <a href="#create-a-connection-to-adobe-workfront planning" class="MCXref xref" >[!DNL Adobe Workfront Planning]</a>에 대한 연결 만들기 를 참조하십시오.</td>
    </tr>
     <tr>
      <td role="rowheader">
        <p>[!UICONTROL URL]</p>
      </td>
      <td>
        <p>상대 경로 입력 <code>https://(YOUR_WORKFRONT_DOMAIN)/maestro/api/</code></p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">
        <p>[!UICONTROL 메서드]</p>
      </td>
   <td> <p>API 호출을 구성하는 데 필요한 HTTP 요청 메서드를 선택합니다. 자세한 내용은 [!DNL Adobe Workfront Fusion]</a>에서 <a href="../../workfront-fusion/modules/http-request-methods.md" class="MCXref xref" data-mc-variable-override="">HTTP 요청 메서드를 참조하십시오.</p> </td> 
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
        <p>쿼리 문자열에 추가할 각 키/값 쌍에 대해 <b>항목 추가</b>를 클릭하고 키와 값을 입력하십시오.</p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Body]</td>
   <td> <p>표준 JSON 개체의 형태로 API 호출에 대한 본문 콘텐츠를 추가합니다.</p> <p>참고:  <p>JSON에서 <code>if</code>과(와) 같은 조건문을 사용할 때 따옴표를 조건문 외부에 넣으십시오.</p> 
     <div class="example" data-mc-autonum="<b>Example: </b>"> 
      <p> <img src="assets/quotes-in-json-350x120.png" style="width: 350;height: 120;"> </p> 
     </div> </p> </td>     </tr>
  </tbody>
</table>

<!--
### Searches

#### Search records

This action module retrieves a list of records based on criteria you specify.

-->

### 미분류


#### 레코드 만들기

이 작업을 수행하면 Workfront Planning에 단일 레코드가 만들어집니다.

<table style="table-layout:auto"> 
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">[!UICONTROL Connection]</td>
      <td>[!DNL Adobe Workfront Planning]에 대한 연결을 만드는 방법에 대한 지침은 이 문서에서 <a href="#create-a-connection-to-adobe-workfront planning" class="MCXref xref" >[!DNL Adobe Workfront Planning]</a>에 대한 연결 만들기 를 참조하십시오.</td>
    </tr>
     <tr>
      <td role="rowheader">
        <p>[!UICONTROL 레코드 유형 ID]</p>
      </td>
      <td>생성할 레코드 유형을 입력하거나 매핑합니다. 사용 가능한 레코드 유형은 Workfront Planning 계정을 기반으로 합니다.</td> 
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

이 작업 모듈은 Workfront Planning에서 지정된 레코드를 삭제합니다.

<table style="table-layout:auto"> 
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">[!UICONTROL Connection]</td>
      <td>[!DNL Adobe Workfront Planning]에 대한 연결을 만드는 방법에 대한 지침은 이 문서에서 <a href="#create-a-connection-to-adobe-workfront planning" class="MCXref xref" >[!DNL Adobe Workfront Planning]</a>에 대한 연결 만들기 를 참조하십시오.</td>
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

This action module retrieves all records from an [!DNL Adobe Workfront Planning] account.

<table style="table-layout:auto"> 
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">[!UICONTROL Connection]</td>
      <td>For instructions on creating a connection to [!DNL Adobe Workfront Planning], see <a href="#create-a-connection-to-adobe-workfront planning" class="MCXref xref" >Create a connection to [!DNL Adobe Workfront Planning]</a> in this article.</td>
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

이 작업 모듈은 ID로 지정된 [!DNL Adobe Workfront Planning]에서 단일 레코드를 검색합니다.

<table style="table-layout:auto"> 
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">[!UICONTROL Connection]</td>
      <td>[!DNL Adobe Workfront Planning]에 대한 연결을 만드는 방법에 대한 지침은 이 문서에서 <a href="#create-a-connection-to-adobe-workfront planning" class="MCXref xref" >[!DNL Adobe Workfront Planning]</a>에 대한 연결 만들기 를 참조하십시오.</td>
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
      <td>[!DNL Adobe Workfront Planning]에 대한 연결을 만드는 방법에 대한 지침은 이 문서에서 <a href="#create-a-connection-to-adobe-workfront planning" class="MCXref xref" >[!DNL Adobe Workfront Planning]</a>에 대한 연결 만들기 를 참조하십시오.</td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Workspace]</td>
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

이 작업 모듈은 [!DNL Adobe Workfront Planning] 계정의 레코드 종류 목록을 검색합니다.

<table style="table-layout:auto"> 
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">[!UICONTROL Connection]</td>
      <td>[!DNL Adobe Workfront Planning]에 대한 연결을 만드는 방법에 대한 지침은 이 문서에서 <a href="#create-a-connection-to-adobe-workfront planning" class="MCXref xref" >[!DNL Adobe Workfront Planning]</a>에 대한 연결 만들기 를 참조하십시오.</td>
    </tr>
  </tbody>
</table>

### 레코드 업데이트

이 작업은 Workfront Planning의 단일 레코드를 업데이트합니다.

<table style="table-layout:auto"> 
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">[!UICONTROL Connection]</td>
      <td>[!DNL Adobe Workfront Planning]에 대한 연결을 만드는 방법에 대한 지침은 이 문서에서 <a href="#create-a-connection-to-adobe-workfront planning" class="MCXref xref" >[!DNL Adobe Workfront Planning]</a>에 대한 연결 만들기 를 참조하십시오.</td>
    </tr>
     <tr>
      <td role="rowheader">
        <p>[!UICONTROL 레코드 ID]</p>
      </td>
      <td>업데이트할 레코드 유형을 입력하거나 매핑합니다. 사용 가능한 레코드 유형은 Workfront Planning 계정을 기반으로 합니다.</td> 
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
