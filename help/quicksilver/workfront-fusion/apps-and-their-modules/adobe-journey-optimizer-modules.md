---
filename: adobe-journey-optimizer-modules
content-type: reference
product-previous: workfront-fusion
product-area: workfront-integrations
navigation-topic: apps-and-their-modules
title: Adobe Journey Optimizer 모듈
description: 에서 [!DNL Adobe Workfront Fusion] 시나리오, [!DNL Adobe Journey Optimizer]여러 타사 애플리케이션 및 서비스에 연결할 수 있습니다.
author: Becky
exl-id: 2c1aea46-edbf-42a3-a6e9-f8aea042a48d
source-git-commit: 885d93dd4383945538e977fd3edbfd55bda88b70
workflow-type: tm+mt
source-wordcount: '1554'
ht-degree: 0%

---

# [!DNL Adobe Journey Optimizer] 모듈

<!--
Becky: pull from main, add to TOCs, then push to merge.
-->

에서 [!DNL Adobe Workfront Fusion] 시나리오, [!DNL Adobe Journey Optimizer]여러 타사 애플리케이션 및 서비스에 연결할 수 있습니다. [!DNL Adobe Journey Optimizer] 모듈을 사용하면 레코드를 생성, 읽기, 업데이트 또는 삭제하거나 [!DNL Adobe Journey Optimizer] API.


시나리오 만들기에 대한 지침이 필요한 경우 [시나리오 만들기](../../workfront-fusion/scenarios/create-a-scenario.md).

모듈에 대한 자세한 내용은 [의 모듈 [!DNL Adobe Workfront Fusion]](../../workfront-fusion/modules/modules.md).

## 액세스 요구 사항

이 문서의 기능을 사용하려면 다음 액세스 권한이 있어야 합니다.

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">[!DNL Adobe Workfront] 플랜*</td>
      <td>
        <p>[!UICONTROL Pro] 이상</p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">[!DNL Adobe Workfront] 라이센스*</td>
      <td>
        <p>[!UICONTROL Plan], [!UICONTROL Work]</p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">[!DNL Adobe Workfront Fusion] license**</td>
      <td >
        <p>[!UICONTROL [!DNL Workfront Fusion] 작업 자동화 및 통합을 위한]</p>
      </td>
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

를 사용하기 전에 [!DNL Adobe Journey Optimizer] 커넥터, 다음 전제 조건이 충족되는지 확인해야 합니다.

* 활성 상태여야 합니다. [!DNL Adobe Journey Optimizer] 계정이 필요합니다.

## 연결 만들기 [!DNL Adobe Journey Optimizer]

에 대한 연결을 만들려면 [!DNL Adobe Journey Optimizer] 모듈:

1. 어떤 경우에서도 [!DNL Adobe Journey Optimizer] 모듈 **[!UICONTROL 추가]** 를 클릭합니다.

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
            <p>이 연결의 이름을 입력합니다.</p>
          </td>
        </tr>
        <tr>
          <td role="rowheader">[!UICONTROL Client ID]</td>
          <td>을(를) 입력합니다. [!DNL Adobe] [!UICONTROL 클라이언트 ID]. 이 항목은 [!DNL Adobe Developer Console].</td>
        </tr>
        <tr>
          <td role="rowheader">[!UICONTROL Client Secret]</td>
          <td>을(를) 입력합니다. [!DNL Adobe] [!UICONTROL Client Secret]. 이 항목은 [!DNL Adobe Developer Console].
        </tr>
        <tr>
          <td role="rowheader">[!UICONTROL 기술 계정 ID]</td>
          <td>을(를) 입력합니다. [!DNL Adobe] [!UICONTROL 기술 계정 ID]. 이 항목은 [!DNL Adobe Developer Console].
        </tr>
        <tr>
          <td role="rowheader">[!UICONTROL 조직 ID]</td>
          <td>을(를) 입력합니다. [!DNL Adobe] [!UICONTROL 조직 ID]. 이 항목은 [!DNL Adobe Developer Console].
        </tr>
        <tr>
          <td role="rowheader">[!UICONTROL Meta 범위]</td>
          <td>
            연결에 필요한 메타 범위를 입력합니다.
          </td>
        </tr>
        <tr>
          <td role="rowheader">[!UICONTROL 개인 키]</td>
          <td>
            <p>자격 증명을 만들 때 생성된 개인 키를 [!DNL Adobe Developer Console]. </p>
            <p>개인 키 또는 인증서를 추출하려면 다음을 수행하십시오.</p>
            <ol>
              <li value="1">
                <p>클릭 <b>[!UICONTROL Extract]</b>.</p>
              </li>
              <li value="2">
                <p>추출할 파일 유형을 선택합니다.</p>
              </li>
              <li value="3">
                <p>개인 키 또는 인증서가 포함된 파일을 선택합니다.</p>
              </li>
              <li value="4">
                <p>파일의 암호를 입력합니다.</p>
              </li>
              <li value="5">
                <p>클릭 <b>[!UICONTROL Save]</b> 파일을 추출하고 연결 설정으로 돌아갑니다.</p>
              </li>
            </ol>
          </td>
        </tr>
      </tbody>
    </table>
1. 클릭 **[!UICONTROL 계속]** 연결을 저장하고 모듈로 돌아가려면 를 클릭합니다.

## [!DNL Adobe Journey Optimizer] 모듈 및 해당 필드

구성 시 [!DNL Adobe Journey Optimizer] 모듈, [!DNL Workfront Fusion] 아래 나열된 필드를 표시합니다. 이와 함께 추가 [!DNL Adobe Journey Optimizer] 앱이나 서비스에서 액세스 수준과 같은 요소에 따라 필드가 표시될 수 있습니다. 모듈에서 굵게 표시된 제목은 필수 필드를 나타냅니다.

필드 또는 함수 위에 맵 단추가 표시되면 이 단추를 사용하여 해당 필드에 대한 변수와 함수를 설정할 수 있습니다. 자세한 내용은 [의 한 모듈에서 다른 모듈로 정보 매핑 [!DNL Adobe Workfront Fusion]](../../workfront-fusion/mapping/map-information-between-modules.md).

![](assets/map-toggle-350x74.png)

* [액션](#actions)
* [검색 결과](#searches)

### 액션

* [[!UICONTROL 레코드 만들기]](#create-a-record)
* [[!UICONTROL 사용자 지정 API 호출 만들기]](#make-a-custom-api-call)
* [[!UICONTROL 레코드 삭제]](#delete-a-record)
* [[!UICONTROL 레코드 업데이트]](#update-a-record)

#### [!UICONTROL 레코드 만들기]

이 작업 모듈은 배치, 의사 결정 규칙, 태그, 개인화된 오퍼, 컬렉션 또는 대체 오퍼를 만듭니다.

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">[!UICONTROL Connection]</td>
     <td>연결 생성에 대한 지침은 [!DNL Adobe Journey Optimizer]를 참조하십시오. <a href="#create-a-connection-to-adobe-journey-optimizer" class="MCXref xref" >연결 만들기 [!DNL Adobe Journey Optimizer]</a> 참조하십시오.</td>
    </tr>
    <tr>
      <td role="rowheader">
        [!UICONTROL 레코드 유형]
      </td>
      <td>
        만들 레코드 유형을 선택합니다
        <ul>
        <li><b>[!UICONTROL Placement]</b>: 계속 <a href="#placement-fields" >[!UICONTROL Placement] 필드</a>.</li>
        <li><b>[!UICONTROL Decision Rule]</b>: 계속 <a href="#decision-rule-fields" >[!UICONTROL Decision Rule] 필드</a>.</li>
        <li><b>[!UICONTROL 결정]</b>: 계속 <a href="#decision-fields" >[!UICONTROL Decision] 필드</a>.</li>
        <li><b>[!UICONTROL 태그]</b>: 계속 <a href="#tag-fields" >[!UICONTROL Tag] 필드</a>.</li>
        <li><b>[!UICONTROL Collection]</b>: 계속 <a href="#collection-fields" >[!UICONTROL Collection] 필드</a>.</li>
        <li><b>[!UICONTROL 대체 오퍼]</b>: 계속 <a href="#fallback-offer-fields" >[!UICONTROL 대체 오퍼] 필드</a>.</li>
        <li><b>[!UICONTROL Personalized Offer]</b>: 계속 <a href="#personalized-offer-fields" >[!UICONTROL Personalized Offer] 필드</a>.</li>
        </ul>
      </td>
    </tr>
  </tbody>
</table>

##### [!UICONTROL 배치] 필드

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">[!UICONTROL Name]</td>
     <td>배치 이름을 입력하거나 매핑합니다.</td>
    </tr>
    <tr>
      <td role="rowheader">
        [!UICONTROL Description]
      </td>
      <td>배치에 대한 설명을 입력하거나 매핑합니다.
      </td>
    </tr>
  </tbody>
</table>


##### [!UICONTROL 의사 결정 규칙] 필드

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">[!UICONTROL Name]</td>
     <td>설명 규칙의 이름을 입력하거나 매핑합니다.</td>
    </tr>
    <tr>
      <td role="rowheader">
        [!UICONTROL Description]
      </td>
      <td>결정 규칙에 대한 설명을 입력하거나 매핑합니다.
      </td>
    </tr>
    <tr>
      <td role="rowheader">
        [!UICONTROL Condition]
      </td>
      <td>결정 규칙에 조건을 입력하거나 매핑합니다.
      </td>
    </tr>
  </tbody>
</table>

##### [!UICONTROL 결정] 필드

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">[!UICONTROL Name]</td>
     <td>설명 규칙의 이름을 입력하거나 매핑합니다.</td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL 상태]</td>
      <td>결정 상태를 선택합니다.
      </td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL 시작 날짜]</td>
      <td><p>결정 시작 일자를 입력하거나 매핑합니다.</p><p>지원되는 날짜 형식 목록은 다음을 참조하십시오 <a href="../../workfront-fusion/mapping/type-coercion.md" class="MCXref xref">형식 강제 적용 [!DNL Adobe Workfront Fusion]</a>.</p>
      </td>
    </tr>
   <tr>
      <td role="rowheader">[!UICONTROL 종료 날짜]</td>
      <td><p>결정 종료 일자를 입력하거나 매핑합니다.</p><p>지원되는 날짜 형식 목록은 다음을 참조하십시오 <a href="../../workfront-fusion/mapping/type-coercion.md" class="MCXref xref">형식 강제 적용 [!DNL Adobe Workfront Fusion]</a>.</p>
      </td>
    </tr>
   <tr>
      <td role="rowheader">[!UICONTROL 배치]</td>
      <td>이 결정에 추가할 배치를 선택합니다
      </td>
    </tr>
   <tr>
      <td role="rowheader">[!UICONTROL Collection]</td>
      <td>이 결정에서 고려할 오퍼가 포함된 오퍼 컬렉션을 선택합니다.
      </td>
    </tr>
   <tr>
      <td role="rowheader">[!UICONTROL 대체 오퍼]</td>
      <td>이 결정에 대한 규칙과 일치하지 않는 고객에게 표시될 대체 오퍼를 선택합니다.
      </td>
    </tr>
  </tbody>
</table>

##### [!UICONTROL 태그] 필드

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">[!UICONTROL Name]</td>
     <td>태그의 이름을 입력하거나 매핑합니다.</td>
    </tr>
  </tbody>
</table>

##### [!UICONTROL 컬렉션] 필드

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">[!UICONTROL Name]</td>
     <td>컬렉션 이름을 입력하거나 매핑합니다.</td>
    </tr>
    <tr>
      <td role="rowheader">
        [!UICONTROL 필터 유형]
      </td>
      <td>
      </td>
    </tr>
    <tr>
      <td role="rowheader">
        [!UICONTROL Elements]
      </td>
      <td>컬렉션에 포함할 태그를 선택합니다.
      </td>
    </tr>
  </tbody>
</table>

##### [!UICONTROL 대체 오퍼] 필드

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">[!UICONTROL Name]</td>
     <td>대체 오퍼의 이름을 입력하거나 매핑합니다.</td>
    </tr>
    <tr>
      <td role="rowheader">
        [!UICONTROL 상태]
      </td>
      <td> 대체 오퍼의 상태를 선택합니다.
      </td>
    </tr>
    <tr>
      <td role="rowheader">
        [!UICONTROL Placement]
      </td>
      <td>대체 오퍼에 대한 배치를 입력하거나 매핑합니다.
      </td>
    </tr>
  </tbody>
</table>

##### [!UICONTROL 개인화된 오퍼] 필드

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">[!UICONTROL Name]</td>
     <td>설명 규칙의 이름을 입력하거나 매핑합니다.</td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL 상태]</td>
      <td>결정 상태를 선택합니다.
      </td>
    </tr>
    <tr>
      <td role="rowheader">배치</td>
      <td>개인화된 오퍼에 대한 배치를 선택합니다.
      </td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL 시작 날짜]</td>
      <td><p>개인화된 오퍼의 시작 날짜를 입력하거나 매핑합니다.</p><p>지원되는 날짜 형식 목록은 다음을 참조하십시오 <a href="../../workfront-fusion/mapping/type-coercion.md" class="MCXref xref">형식 강제 적용 [!DNL Adobe Workfront Fusion]</a>.</p>
      </td>
    </tr>
   <tr>
      <td role="rowheader">[!UICONTROL 종료 날짜]</td>
      <td><p>개인화된 오퍼의 종료 날짜를 입력하거나 매핑합니다.</p><p>지원되는 날짜 형식 목록은 다음을 참조하십시오 <a href="../../workfront-fusion/mapping/type-coercion.md" class="MCXref xref">형식 강제 적용 [!DNL Adobe Workfront Fusion]</a>.</p>
      </td>
    </tr>
   <tr>
      <td role="rowheader">[!UICONTROL 의사 결정 규칙]</td>
      <td>개인화된 이 오퍼에 추가할 의사 결정 규칙을 선택합니다.
      </td>
    </tr>
   <tr>
      <td role="rowheader">[!UICONTROL Priority]</td>
      <td>이 오퍼의 우선 순위를 선택합니다. 우선 순위는 다른 오퍼가 아닌 이 오퍼를 표시할지 여부에 영향을 줍니다.
      </td>
    </tr>
   <tr>
      <td role="rowheader">[!UICONTROL 최대 가용량 제한]</td>
      <td>이 오퍼가 표시되는 횟수를 입력하거나 매핑합니다.
      </td>
    </tr>
  </tbody>
</table>

#### [!UICONTROL 레코드 삭제]

이 작업 모듈은 [!DNL Adobe Journey Optimizer].

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">[!UICONTROL Connection]</td>
     <td>연결 생성에 대한 지침은 [!DNL Adobe Journey Optimizer]를 참조하십시오. <a href="#create-a-connection-to-adobe-journey-optimizer" class="MCXref xref" >연결 만들기 [!DNL Adobe Journey Optimizer]</a> 참조하십시오.</td>
    </tr>
    <tr>
      <td role="rowheader">
        [!UICONTROL 레코드 유형]
      </td>
      <td>
        삭제할 레코드 유형을 선택합니다
        <ul>
        <li>[!UICONTROL Placement]</li>
        <li>[!UICONTROL Decision Rule]</li>
        <li>[!UICONTROL 결정]</li>
        <li>[!UICONTROL 태그]</li>
        <li>[!UICONTROL Collection]</li>
        <li>[!UICONTROL 대체 오퍼]</li>
        <li>[!UICONTROL Personalized Offer]</li>
        </ul>
      </td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Placement]/[!UICONTROL Decision]/[!UICONTROL Decision]/[!UICONTROL Tag]/[!UICONTROL Collection]/[!UICONTROL Fallback Offer]/[!UICONTROL Personalized Offer]
      </td>
      <td>
        삭제할 레코드를 선택합니다.
      </td>
    </tr>

</tbody>
</table>

#### [!UICONTROL 사용자 지정 API 호출 만들기]

이 모듈은 [!DNL Adobe Journey Optimizer] API

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
     <td role="rowheader">[!UICONTROL Connection]</td>
     <td>연결 생성에 대한 지침은 [!DNL Adobe Journey Optimizer]를 참조하십시오. <a href="#create-a-connection-to-adobe-journey-optimizer" class="MCXref xref" >연결 만들기 [!DNL Adobe Journey Optimizer]</a> 참조하십시오.</td>
    </tr>
    <tr>
      <td role="rowheader">
        <p>[!UICONTROL Path]</p>
      </td>
      <td>
        <p>다음으로 시작하는 {baseURL}에 대한 상대 경로를 입력하십시오.<code>/</code></p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">
        <p>[!UICONTROL 메서드]</p>
      </td>
      <td>
   <td> <p>API 호출을 구성하는 데 필요한 HTTP 요청 메서드를 선택합니다. 자세한 내용은 <a href="../../workfront-fusion/modules/http-request-methods.md" class="MCXref xref" data-mc-variable-override="">의 HTTP 요청 메서드 [!DNL Adobe Workfront Fusion]</a>.</p> </td> 
      </td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Headers]</td>
      <td>
        <p>요청의 헤더를 표준 JSON 개체 형태로 추가합니다.</p>
        <p>For example, <code>{"Content-type":"application/json"}</code></p>
        <p>Workfront Fusion은 인증 헤더와 x-api-key 헤더를 자동으로 추가합니다.</p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL 쿼리 문자열]  </td>
      <td>
        <p>요청 쿼리 문자열을 입력합니다.</p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Body]</td>
   <td> <p>표준 JSON 개체 형태로 API 호출에 대한 본문 콘텐츠를 추가합니다.</p> <p>참고:  <p>다음과 같은 조건문을 사용하는 경우 <code>if</code> json에서 따옴표를 조건문 외부에 지정합니다.</p> 
     <div class="example" data-mc-autonum="<b>Example: </b>"> 
      <p> <img src="assets/quotes-in-json-350x120.png" style="width: 350;height: 120;"> </p> 
     </div> </p> </td>     </tr>
     <tr>
      <td role="rowheader">[!UICONTROL 제한]  </td>
      <td>
        <p>모듈이 하나의 실행 주기에 반환할 최대 결과 수를 입력합니다.</p>
      </td>
    </tr>
  </tbody>
</table>

#### [!UICONTROL 레코드 삭제]

이 작업 모듈은 [!DNL Adobe Journey Optimizer].

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
     <td role="rowheader">[!UICONTROL Connection]</td>
     <td>연결 생성에 대한 지침은 [!DNL Adobe Journey Optimizer]를 참조하십시오. <a href="#create-a-connection-to-adobe-journey-optimizer" class="MCXref xref" >연결 만들기 [!DNL Adobe Journey Optimizer]</a> 참조하십시오.</td>
    </tr>
    <tr>
      <td role="rowheader">
        [!UICONTROL 레코드 유형]
      </td>
      <td>
        삭제할 레코드 유형을 선택합니다
        <ul>
        <li>[!UICONTROL Placement]</li>
        <li>[!UICONTROL Decision Rule]</li>
        <li>[!UICONTROL 결정]</li>
        <li>[!UICONTROL 태그]</li>
        <li>[!UICONTROL Collection]</li>
        <li>[!UICONTROL 대체 오퍼]</li>
        <li>[!UICONTROL Personalized Offer]</li>
        </ul>
      </td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Placement]/[!UICONTROL Decision]/[!UICONTROL Decision]/[!UICONTROL Tag]/[!UICONTROL Collection]/[!UICONTROL Fallback Offer]/[!UICONTROL Personalized Offer]
      </td>
      <td>
        삭제할 레코드를 선택합니다.
      </td>
    </tr>

</tbody>
</table>

#### [!UICONTROL 레코드 업데이트]

이 작업 모듈은 배치, 결정, 의사 결정 규칙, 태그, 개인화된 오퍼, 컬렉션 또는 대체 오퍼를 만듭니다.

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
     <td role="rowheader">[!UICONTROL Connection]</td>
     <td>연결 생성에 대한 지침은 [!DNL Adobe Journey Optimizer]를 참조하십시오. <a href="#create-a-connection-to-adobe-journey-optimizer" class="MCXref xref" >연결 만들기 [!DNL Adobe Journey Optimizer]</a> 참조하십시오.</td>
    </tr>
    <tr>
      <td role="rowheader">
        [!UICONTROL 레코드 유형]
      </td>
      <td>
        업데이트할 레코드 유형을 선택합니다
        <ul>
        <li>[!UICONTROL Placement]</li>
        <li>[!UICONTROL Decision Rule]</li>
        <li>[!UICONTROL 결정]</li>
        <li>[!UICONTROL 태그]</li>
        <li>[!UICONTROL Collection]</li>
        <li>[!UICONTROL 대체 오퍼]</li>
        <li>[!UICONTROL Personalized Offer]</li>
        </ul>
      </td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Placement]/[!UICONTROL Decision]/[!UICONTROL Decision]/[!UICONTROL Tag]/[!UICONTROL Collection]/[!UICONTROL Fallback Offer]/[!UICONTROL Personalized Offer]
      </td>
      <td>
        업데이트할 레코드를 선택합니다.
      </td>
    </tr>
    <tr>
      <td role="rowheader">
        [!UICONTROL Fields]
      </td>
      <td>업데이트할 각 필드에 대해:
      <ol>
      <li>클릭 <b>[!UICONTROL Add]</b>.</li>
      <li>값을 추가, 바꾸기 또는 제거할지 선택합니다.</li>
      <li>업데이트할 필드를 입력합니다.</li>
      <li>필드에 새 값을 입력합니다.</li>
      </td>
    </tr>

</tbody>
</table>


### 검색 결과

#### [!UICONTROL 레코드 나열]

이 검색 모듈은 선택한 유형의 레코드를 나열하고 지정한 기준에 따라 결과를 반환합니다.

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
     <td role="rowheader">[!UICONTROL Connection]</td>
     <td>연결 생성에 대한 지침은 [!DNL Adobe Journey Optimizer]를 참조하십시오. <a href="#create-a-connection-to-adobe-journey-optimizer" class="MCXref xref" >연결 만들기 [!DNL Adobe Journey Optimizer]</a> 참조하십시오.</td>
    </tr>
    <tr>
      <td role="rowheader">
        <p>[!UICONTROL 레코드 유형]</p>
      </td>
      <td>
        <p>나열할 레코드 유형을 선택합니다.</p>
        <ul>
        <li>[!UICONTROL Placement]</li>
        <li>[!UICONTROL Decision Rule]</li>
        <li>[!UICONTROL 결정]</li>
        <li>[!UICONTROL 태그]</li>
        <li>[!UICONTROL Collection]</li>
        <li>[!UICONTROL 대체 오퍼]</li>
        <li>[!UICONTROL Personalized Offer]</li>
       </ul>
      </td>
    </tr>
    <tr>
      <td role="rowheader">
        <p>[!UICONTROL Query Operator]</p>
      </td>
      <td>
        <p>쿼리의 매개 변수에 적용할 연산자를 선택합니다</p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Fields]</td>
      <td><p>검색을 특정 필드로 제한하려면 필드를 입력합니다. 검색을 제한할 각 필드에 대해 [!UICONTROL 항목 추가]를 클릭하고 필드의 이름을 입력합니다.</p><p>경로 표현식은 다음과 같이 점으로 구분된 경로의 형식입니다 <code>_instance.xdm:name</code>.</p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Order by] </td>
      <td>결과를 정렬할 속성을 입력하거나 매핑합니다.
      </td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL 순서 방향]</td>
   <td>결과를 오름차순 또는 내림차순으로 정렬할지 여부를 선택합니다.
    </td>
     </tr>
  </tbody>
</table>
