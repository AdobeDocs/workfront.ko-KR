---
filename: creative-cloud-libraries-modules
content-type: reference
product-previous: workfront-fusion
product-area: workfront-integrations
navigation-topic: apps-and-their-modules
title: Adobe Creative Cloud 라이브러리 모듈
description: 포함 [!DNL Adobe Workfront Fusion Adobe Creative Cloud] 라이브러리 모듈에서는 요소나 라이브러리를 만들거나 업데이트할 때 시나리오를 시작할 수 있습니다. 요소를 업로드, 검색, 보관 또는 나열하거나 [!DNL Adobe Creative Cloud Libraries] API.
author: Becky
exl-id: 8affa34b-803d-48a5-a986-9fbe0cb8c8f5
source-git-commit: 0915dcce45b271ee18cdd8af5db4f0eb01f3cced
workflow-type: tm+mt
source-wordcount: '1241'
ht-degree: 1%

---

# Adobe Creative Cloud 라이브러리 모듈

포함 [!DNL Adobe Workfront Fusion] [!DNL Adobe Creative Cloud Libraries] 모듈에서는 요소나 라이브러리를 만들거나 업데이트할 때 시나리오를 시작할 수 있습니다. 요소를 업로드, 검색, 보관 또는 나열하거나 [!DNL Adobe Creative Cloud Libraries] API.

시나리오를 만드는 방법에 대한 지침이 필요한 경우 [시나리오 만들기](../../workfront-fusion/scenarios/create-a-scenario.md).

모듈에 대한 자세한 내용은 [의 모듈 [!DNL Adobe Workfront Fusion]](../../workfront-fusion/modules/modules.md).

## 액세스 요구 사항

이 문서의 기능을 사용하려면 다음 액세스 권한이 있어야 합니다.

<table style="table-layout:auto"> 
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

사용 [!DNL Adobe Creative Cloud Libraries] 모듈, 다음 항목이 있어야 합니다. [!UICONTROL Adobe Creative Cloud] 계정입니다.

## [!UICONTROL Adobe Creative Cloud 라이브러리] 모듈 및 해당 필드

를 구성할 때 [!UICONTROL Adobe Creative Cloud 라이브러리] 모듈, [!DNL Workfront Fusion] 아래 나열된 필드를 표시합니다. 이와 함께 추가 [!DNL Adobe Creative Cloud Libraries] 앱이나 서비스의 액세스 수준 등에 따라 필드가 표시될 수 있습니다. 모듈의 굵은 제목은 필수 필드를 나타냅니다.

필드나 함수 위에 맵 단추가 표시되면 이 단추를 사용하여 해당 필드에 대한 변수와 함수를 설정할 수 있습니다. 자세한 내용은 [의 한 모듈에서 다른 모듈로 정보 매핑 [!DNL Adobe Workfront Fusion]](../../workfront-fusion/mapping/map-information-between-modules.md).

![](assets/map-toggle-350x74.png)


* [요소](#elements)

* [라이브러리](#libraries)

* [기타](#other)


### 요소

* [[!UICONTROL 요소 보관]](#archive-an-element)

* [[!UICONTROL 요소 가져오기]](#get-an-element)

* [[!UICONTROL 목록 요소]](#list-elements)

* [[!UICONTROL 요소 업로드]](#upload-an-element)

* [!UICONTROL [라이브러리의 새 요소 보기]](#watch-new-element-in-library)

* [[!UICONTROL 업데이트된 요소 보기]](#watch-updated-elements)


#### [!UICONTROL 요소 보관]

이 작업 모듈은 라이브러리의 요소를 보관합니다.

<table style="table-layout:auto"> 
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">[!UICONTROL Connection]</td>
      <td>연결에 대한 자세한 내용 [!DNL Adobe Creative Cloud] 계정 위치: [!DNL Workfront Fusion], 참조 <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">에 대한 연결 만들기 [!DNL Adobe Workfront Fusion] - 기본 지침</td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL 라이브러리 ID]</td>
      <td >보관하려는 요소가 포함된 라이브러리를 선택합니다.</td>
    </tr>
    <tr>
      <td class="TableStyle-TableStyle-List-options-in-steps-BodyB-Column1-LightGray" role="rowheader">[!UICONTROL 요소 ID]</td>
      <td class="TableStyle-TableStyle-List-options-in-steps-BodyA-Column2-LightGray">보관하려는 요소를 선택합니다.</td>
    </tr>
  </tbody>
</table>

#### [!UICONTROL 요소 가져오기]

이 작업 모듈은 라이브러리에서 단일 요소를 반환합니다.

<table style="table-layout:auto"> 
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">[!UICONTROL Connection]</td>
      <td>연결에 대한 자세한 내용 [!DNL Adobe Creative Cloud] 계정 위치: [!DNL Workfront Fusion], 참조 <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">에 대한 연결 만들기 [!DNL Adobe Workfront Fusion] - 기본 지침</td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL 라이브러리 ID]</td>
      <td >검색할 요소가 포함된 라이브러리를 선택합니다.</td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL 요소 ID]</td>
      <td>검색할 요소의 ID를 입력하거나 매핑합니다.</td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Selector]</td>
      <td>
        <p>모듈이 반환하는 정보 유형을 선택합니다. </p>
        <ul>
          <li>
            <p><b>[!UICONTROL 기본값]</b>
            </p>
            <p>기본 데이터</p>
          </li>
          <li>
            <p><b>[!UICONTROL 세부 정보]</b>
            </p>
            <p>사용 가능한 모든 데이터</p>
          </li>
          <li>
            <p><b>[!UICONTROL 표시]</b>
            </p>
            <p>라이브러리 요소와 연결된 병합된 자산 목록</p>
          </li>
        </ul>
      </td>
    </tr>
  </tbody>
</table>

#### [!UICONTROL 목록 요소]

이 작업 모듈은 라이브러리의 요소 목록을 검색합니다.

<table style="table-layout:auto"> 
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">[!UICONTROL Connection]</td>
      <td>연결에 대한 자세한 내용 [!DNL Adobe Creative Cloud] 계정 위치: [!DNL Workfront Fusion], 참조 <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">에 대한 연결 만들기 [!DNL Adobe Workfront Fusion] - 기본 지침</td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL 라이브러리 ID]</td>
      <td >요소를 나열할 라이브러리를 선택합니다.</td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Order by]</td>
      <td>이름별로 결과를 정렬할지 아니면 요소가 수정된 마지막 날짜별로 결과를 정렬할지 선택합니다.</td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL 유형]</td>
      <td >지정된 MIME 유형으로 식별된 요소로 결과를 제한하려면 MIME 유형을 입력합니다. 예: <code>string</code>.</td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Selector]</td>
      <td>
        <p>모듈이 반환하는 정보 유형을 선택합니다. </p>
        <ul>
          <li>
            <p><b>[!UICONTROL 기본값]</b>
            </p>
            <p>기본 데이터</p>
          </li>
          <li>
            <p><b>[!UICONTROL 세부 정보]</b>
            </p>
            <p>사용 가능한 모든 데이터</p>
          </li>
          <li>
            <p><b>[!UICONTROL 표시]</b>
            </p>
            <p>라이브러리 요소와 연결된 병합된 자산 목록</p>
          </li>
        </ul>
      </td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL 제한]</td>
      <td>각 시나리오 실행 주기 동안 모듈이 반환할 최대 레코드 수를 입력하거나 매핑합니다.</td>
    </tr>
  </tbody>
</table>

#### [!UICONTROL 요소 업로드]

이 작업 모듈은 작은 파일 에셋을 기존 라이브러리에 업로드합니다. 최대 파일 크기는 1GB입니다.

<table style="table-layout:auto"> 
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">[!UICONTROL Connection]</td>
      <td>연결에 대한 자세한 내용 [!DNL Adobe Creative Cloud] 계정 위치: [!DNL Workfront Fusion], 참조 <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">에 대한 연결 만들기 [!DNL Adobe Workfront Fusion] - 기본 지침</td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL 라이브러리 ID]</td>
      <td >요소를 나열할 라이브러리를 선택합니다.</td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL 호출 모드]</td>
      <td>
        <p>이 요청 프로세스를 호출할 처리 모드를 선택하십시오.</p>
        <ul>
          <li>
            <p><b>[!UICONTROL 동기화]</b>
            </p>
            <p>API 호출이 동기적으로 처리됩니다. 처리가 완료되면 응답이 전달됩니다(호출 제한 시간이 초과된 경우 제외).</p>
          </li>
          <li>
            <p><b>[!UICONTROL async]</b>
            </p>
            <p>비동기 모니터 응답이 즉시 반환되고 요청 처리가 비동기적으로 발생합니다. 호출은 완료될 때까지 끝점을 폴링합니다.</p>
          </li>
          <li>
            <p><b>[!UICONTROL sync,async]</b> (기본값)</p>
            <p>요청의 동기 처리를 시도했습니다. 처리가 5000ms를 초과할 경우 비동기 모니터 응답이 반환됩니다. 요청이 완료될 때까지 모니터 URL을 폴링해야 합니다.</p>
          </li>
        </ul>
      </td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL 유형 파일]</td>
      <td >업로드한 파일의 MIME 유형을 입력하거나 매핑합니다.</td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL 소스 파일]</td>
      <td>
        <p>이전 모듈에서 소스 파일을 선택하거나 소스 파일의 이름과 데이터를 매핑합니다.</p>
      </td>
    </tr>
  </tbody>
</table>

#### [!UICONTROL 라이브러리에서 새 요소 보기]

이 트리거 모듈은 요소가 라이브러리에 추가되면 시나리오를 시작합니다.

<table style="table-layout:auto"> 
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">[!UICONTROL Connection]</td>
      <td>연결에 대한 자세한 내용 [!DNL Adobe Creative Cloud] 계정 위치: [!DNL Workfront Fusion], 참조 <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">에 대한 연결 만들기 [!DNL Adobe Workfront Fusion] - 기본 지침</td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL 라이브러리 ID]</td>
      <td >업데이트된 요소를 검사할 라이브러리를 선택합니다.</td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL 제한]</td>
      <td>각 시나리오 실행 주기 동안 모듈이 반환할 최대 레코드 수를 입력하거나 매핑합니다.</td>
    </tr>
  </tbody>
</table>


#### [!UICONTROL 업데이트된 요소 보기]

이 트리거 모듈은 라이브러리의 요소가 업데이트될 때 시나리오를 시작합니다.

<table style="table-layout:auto"> 
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">[!UICONTROL Connection]</td>
      <td>연결에 대한 자세한 내용 [!DNL Adobe Creative Cloud] 계정 위치: [!DNL Workfront Fusion], 참조 <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">에 대한 연결 만들기 [!DNL Adobe Workfront Fusion] - 기본 지침</td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL 라이브러리 ID]</td>
      <td >새 요소를 검사할 라이브러리를 선택합니다.</td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL 제한]</td>
      <td>각 시나리오 실행 주기 동안 모듈이 반환할 최대 레코드 수를 입력하거나 매핑합니다.</td>
    </tr>
  </tbody>
</table>

### 라이브러리

* [[!UICONTROL 새 라이브러리 보기]](#watch-new-libraries)

* [[!UICONTROL 업데이트된 라이브러리 보기]](#watch-updated-libraries)


#### [!UICONTROL 새 라이브러리 보기]

이 트리거 모듈은 새 라이브러리가 생성될 때 시나리오를 시작합니다.

<table style="table-layout:auto"> 
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">[!UICONTROL Connection]</td>
      <td>연결에 대한 자세한 내용 [!DNL Adobe Creative Cloud] 계정 위치: [!DNL Workfront Fusion], 참조 <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">에 대한 연결 만들기 [!DNL Adobe Workfront Fusion] - 기본 지침</td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL 제한]</td>
      <td>각 시나리오 실행 주기 동안 모듈이 반환할 최대 레코드 수를 입력하거나 매핑합니다.</td>
    </tr>
  </tbody>
</table>

#### [!UICONTROL 업데이트된 라이브러리 보기]

이 트리거 모듈은 기존 라이브러리가 업데이트될 때 시나리오를 시작합니다.

<table style="table-layout:auto"> 
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">[!UICONTROL Connection]</td>
      <td>연결에 대한 자세한 내용 [!DNL Adobe Creative Cloud] 계정 위치: [!DNL Workfront Fusion], 참조 <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">에 대한 연결 만들기 [!DNL Adobe Workfront Fusion] - 기본 지침</td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL 제한]</td>
      <td>각 시나리오 실행 주기 동안 모듈이 반환할 최대 레코드 수를 입력하거나 매핑합니다.</td>
    </tr>
  </tbody>
</table>

### 기타

#### [!UICONTROL API 호출 만들기]

이 모듈에서는에 대한 사용자 지정 API 호출을 만듭니다. [!DNL Adobe Creative Cloud Libraries] API.

<table style="table-layout:auto"> 
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">[!UICONTROL Connection]</td>
      <td> <p>Adobe Creative Cloud 계정을 Workfront Fusion에 연결하는 방법에 대한 지침은 <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Adobe Workfront Fusion에 대한 연결 만들기 - 기본 지침</a></p>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL URL]</td>
      <td>
        <p>상대 경로 입력 <code>https://cc-libraries.adobe.io/api</code>.</p>
    <p>For example <code>/v1/libraries</code>.</p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL API version]</td>
      <td>
        <p>버전 선택 [!DNL Adobe Analytics] 연결할 API입니다.</p>
      </td>
    </tr>    <tr>
      <td role="rowheader">[!UICONTROL 메서드]</td>
      <td> <p>API 호출을 구성하는 데 필요한 HTTP 요청 메서드를 선택합니다. 자세한 내용은 <a href="../../workfront-fusion/modules/http-request-methods.md" class="MCXref xref">의 HTTP 요청 메서드 [!DNL Adobe Workfront Fusion]</a>.</p> </td> 
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Headers]</td>
      <td>
        <p>표준 JSON 개체 형태로 요청의 헤더를 추가합니다.</p>
        <p>For example, <code>{"Content-type":"application/json"}</code></p>
        <p>Workfront Fusion은 사용자에게 권한 부여 헤더를 추가합니다.</p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL 쿼리 문자열]</td>
      <td>
        <p>표준 JSON 개체 형식으로 API 호출에 대한 쿼리를 추가합니다.</p>
        <p>For example: <code>{"name":"something-urgent"}</code></p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Body]</td>
   <td> <p>표준 JSON 개체의 형태로 API 호출에 대한 본문 콘텐츠를 추가합니다.</p> <p>참고:  <p>다음과 같은 조건문을 사용할 때 <code>if</code> json에서 따옴표를 조건문 외부에 넣습니다.</p> 
     <div class="example" data-mc-autonum="<b>Example: </b>"> 
      <p> <img src="assets/quotes-in-json-350x120.png" style="width: 350;height: 120;"> </p> 
     </div> </p> </td>     </tr>
       <tr>
      <td role="rowheader">[!UICONTROL 임시 문서 업로드]</td>
      <td>
      <p>임시 문서를 업로드하려면 업로드할 문서의 소스 파일을 입력합니다.</p>
      <p>이전 모듈에서 소스 파일을 선택하거나 소스 파일의 이름과 데이터를 매핑합니다.</p>
    </td>
    </tr>

</tbody>
</table>
