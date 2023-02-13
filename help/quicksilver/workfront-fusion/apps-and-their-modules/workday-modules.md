---
filename: workday-modules
content-type: reference
product-previous: workfront-fusion
product-area: workfront-integrations
keywords: 커넥터
navigation-topic: apps-and-their-modules
title: Workday 모듈
description: Adobe Workfront Fusion 시나리오에서는 [!DNL Workday]여러 타사 애플리케이션 및 서비스에 연결할 수 있습니다.
author: Becky
exl-id: 535573e0-b6ad-43a2-b7cb-ed32d1dc8d16
source-git-commit: 885d93dd4383945538e977fd3edbfd55bda88b70
workflow-type: tm+mt
source-wordcount: '965'
ht-degree: 2%

---

# [!DNL Workday] 모듈

에서 [!DNL Adobe Workfront Fusion] 시나리오, [!DNL Workday]여러 타사 애플리케이션 및 서비스에 연결할 수 있습니다.

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

를 사용하려면 [!DNL Workday] 모듈:

* 다음 포함 [!DNL Workday] 계정이 필요합니다.

* 에서 OAuth 애플리케이션 만들기 [!DNL Workday]. 자세한 내용은 [!DNL Workday] 설명서.

## Connect [!DNL Workday] to [!DNL Workfront Fusion]

1. 어떤 경우에서도 [!DNL Workfront Fusion] 모듈 [!UICONTROL 추가] 다음 [!UICONTROL 연결] 필드

2. 다음 필드를 채웁니다.

   <table style="table-layout:auto"> 
        <col/>
        <col/>
        <tbody>
            <tr>
                <td role="rowheader">
                    <p role="rowheader">[!UICONTROL 연결 이름]</p>
                </td>
                <td>연결의 이름을 입력합니다</td>
            </tr>
            <tr>
                <td  role="rowheader">[!UICONTROL Workday 호스트]</td>
                <td>사용자의 주소를 입력합니다 [!DNL Workday] 호스트 없이 <code>https://</code>. For example: <code>mycompany.workday.com</code>.</td>
            </tr>
            <tr>
                <td role="rowheader">[!UICONTROL Services URL]</td>
                <td>사용자의 주소를 입력합니다 [!DNL Workday] 웹 서비스 없이 <code>https://</code>. For example: <code>mycompany-services.workday.com</code>.</td>
            </tr>
            <tr>
                <td  role="rowheader">[!UICONTROL 테넌트 이름]</td>
                <td>이 작업에 대한 테넌트를 입력합니다 [!DNL Workday] 계정이 필요합니다. 테넌트는 조직의 식별자이며, Workday에 로그인하는 데 사용하는 URL에서 표시될 수 있습니다. 예: 주소 <code>https://www.myworkday.com/mycompany</code>, 임차인은 입니다. <code>mycompany</code>.</td>
            </tr>
            <tr>
                <td role="rowheader">[!UICONTROL Client ID]</td>
                <td>에 대한 클라이언트 ID를 입력합니다. [!DNL Workday] 이 연결에서 사용하는 응용 프로그램입니다. 에서 응용 프로그램을 만들 때 이를 가져옵니다 [!DNL Workday].</td>
            </tr>
            <tr>
                <td  role="rowheader">[!UICONTROL Client Secret]</td>
                <td>에 대한 클라이언트 암호 입력 [!DNL Workday] 이 연결에서 사용하는 응용 프로그램입니다. 에서 응용 프로그램을 만들 때 이를 가져옵니다 [!DNL Workday].</td>
            </tr>
            <tr>
                <td role="rowheader">[!UICONTROL 세션 시간 초과(분)]</td>
                <td >인증 토큰이 만료된 후 분 수를 입력합니다.</td>
            </tr>
        </tbody>
    </table>


3. 클릭 [!UICONTROL 계속] 연결을 저장하고 모듈로 돌아가려면

## [!DNL Workday] 모듈 및 해당 필드

구성 시 [!DNL Workday] 모듈, [!DNL Workfront Fusion] 아래 나열된 필드를 표시합니다. 이와 함께 추가 [!DNL Workday] 앱이나 서비스에서 액세스 수준과 같은 요소에 따라 필드가 표시될 수 있습니다. 모듈에서 굵게 표시된 제목은 필수 필드를 나타냅니다.

필드 또는 함수 위에 맵 단추가 표시되면 이 단추를 사용하여 해당 필드에 대한 변수와 함수를 설정할 수 있습니다. 자세한 내용은 [의 한 모듈에서 다른 모듈로 정보 매핑 [!DNL Adobe Workfront Fusion]](../../workfront-fusion/mapping/map-information-between-modules.md).

![](assets/map-toggle-350x74.png)

* [개 액션](#action)

* [검색](#search)


### 개 액션

* [[!UICONTROL 레코드 만들기]](#create-a-record)

* [[!UICONTROL 레코드 삭제]](#delete-a-record)

* [[!UICONTROL 사용자 지정 API 호출 만들기]](#make-a-custom-api-call)

* [[!UICONTROL 레코드 업데이트]](#update-a-record)


#### [!UICONTROL 레코드 만들기]

이 작업 모듈은 [!DNL Workday].

<table style="table-layout:auto"> 
    <col/>
    <col/>
    <tbody>
        <tr>
            <td role="rowheader">[!UICONTROL Connection]</td>
            <td>연결 방법에 대한 지침은 [!DNL Workday] Workfront Fusion 계정, <a href="#Connect" class="MCXref xre[!DNL ]f" >Connect [!DNL Workday] to [!DNL Workfront Fusion]</a>.</td>
        </tr>
        <tr>
            <td  role="rowheader">[!UICONTROL 레코드 유형]</td>
            <td>만들려는 레코드 유형을 선택합니다.</td>
        </tr>
        <tr>
            <td role="rowheader">[!UICONTROL ID] </td>
            <td>만들 레코드의 ID를 입력하거나 매핑합니다.</td>
        </tr>
        <tr>
            <td role="rowheader">[!UICONTROL Subresource ID]</td>
            <td >만들려는 하위 리소스의 ID를 입력하거나 매핑합니다.</td>
        </tr>
    </tbody>
</table>

#### [!UICONTROL 레코드 삭제]

이 작업 모듈은 [!DNL Workday].

<table style="table-layout:auto"> 
    <col class="TableStyle-TableStyle-List-options-in-steps-Column-Column1">
    </col>
    <col class="TableStyle-TableStyle-List-options-in-steps-Column-Column2">
    </col>
    <tbody>
        <tr>
            <td role="rowheader">[!UICONTROL Connection]</td>
            <td>연결 방법에 대한 지침은 [!DNL Workday] 계정 대상 [!DNL Workfront Fusion]를 참조하십시오. <a href="#Connect" class="MCXref xre[!DNL ]f" >Connect [!DNL Workday] to [!DNL Workfront Fusion]</a>.</td>
        </tr>
        <tr>
            <td  role="rowheader">[!UICONTROL 레코드 유형]</td>
            <td>삭제할 레코드 유형을 선택합니다.</td>
        </tr>
        <tr>
            <td role="rowheader">[!UICONTROL 특정 레코드 유형]</td>
            <td>삭제할 특정 유형의 레코드를 선택합니다. 선택한 레코드 유형을 기반으로 합니다.</td>
        </tr>
        <tr>
            <td  role="rowheader">[!UICONTROL Subresource ID]</td>
            <td>삭제할 하위 리소스의 ID를 입력하거나 매핑합니다.</td>
        </tr>
        <tr>
            <td role="rowheader">[!UICONTROL ID] </td>
            <td >삭제할 레코드의 ID를 입력하거나 매핑합니다.</td>
        </tr>
    </tbody>
</table>


### [!UICONTROL 사용자 지정 API 호출 만들기]

이 작업 모듈을 사용하면 [!DNL Workday] API. 이렇게 하면 다른 방식으로 수행할 수 없는 데이터 흐름 자동화를 만들 수 있습니다 [!DNL Workday] 모듈.

이 모듈을 구성할 때 다음 필드가 표시됩니다.

이 모듈은 API 호출의 헤더 및 본문과 함께 상태 코드를 반환합니다.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <p>[!DNL Connection]</p> </td> 
            <td>연결 방법에 대한 지침은 [!DNL Workday] 계정 대상 [!DNL Workfront Fusion]를 참조하십시오. <a href="#Connect" class="MCXref xre[!DNL ]f" >Connect [!DNL Workday] to [!DNL Workfront Fusion]</a>.</td>
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL URL]</td> 
   <td>상대 경로 입력 <code style="color: #ff1493;">https://&lt;tenantHostname>/api/&lt;serviceName>/&lt;version>/&lt;tenant></code>.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL 메서드]</td> 
   <td> <p>API 호출을 구성하는 데 필요한 HTTP 요청 메서드를 선택합니다. 자세한 내용은 <a href="../../workfront-fusion/modules/http-request-methods.md" class="MCXref xref">의 HTTP 요청 메서드 [!DNL Adobe Workfront Fusion]</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Headers]</td> 
   <td> <p>요청의 헤더를 표준 JSON 개체 형태로 추가합니다.</p> <p>For example, <code>{"Content-type":"application/json"}</code></p> <p>[!UICONTROL Workfront Fusion]이 사용자를 위해 인증 헤더를 추가합니다.</p> </td> 
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

#### [!UICONTROL 레코드 업데이트]

이 작업 모듈은 [!DNL Workday].

<table style="table-layout:auto"> 
    <col/>
    <col/>
    <tbody>
        <tr>
            <td role="rowheader">[!UICONTROL Connection]</td>
            <td>연결 방법에 대한 지침은 [!DNL Workday] Workfront Fusion 계정, <a href="#Connect" class="MCXref xref" >[!UICONTROL Connect [!DNL Workday] Workfront Fusion으로 변환]</a></td>
        </tr>
        <tr>
            <td  role="rowheader">레코드 유형</td>
            <td>업데이트할 레코드 t[!UICONTROL]를 선택합니다.</td>
        </tr>
        <tr>
            <td role="rowheader">[!UICONTROL ID] </td>
            <td>업데이트할 레코드의 ID를 입력하거나 매핑합니다.</td>
        </tr>
        <tr>
            <td role="rowheader">[!UICONTROL Subresource ID]</td>
            <td >업데이트할 하위 리소스의 ID를 입력하거나 매핑합니다.</td>
        </tr>
    </tbody>
</table>

### 검색

* [[!UICONTROL 레코드 읽기]](#read-a-record)

* [[!UICONTROL 레코드 나열]](#list-records)


#### [!UICONTROL 레코드 읽기]

이 작업 모듈은 단일 레코드를 읽습니다.

<table style="table-layout:auto"> 
    <col class="TableStyle-TableStyle-List-options-in-steps-Column-Column1">
    </col>
    <col class="TableStyle-TableStyle-List-options-in-steps-Column-Column2">
    </col>
    <tbody>
        <tr>
            <td role="rowheader">[!UICONTROL Connection]</td>
            <td>연결 방법에 대한 지침은 [!DNL Workday] Workfront Fusion 계정, <a href="#Connect" class="MCXref xref" >[!UICONTROL Connect [!DNL Workday] Workfront Fusion으로 변환]</a></td>
        </tr>
        <tr>
            <td  role="rowheader">[!UICONTROL 레코드 유형]</td>
            <td>삭제할 레코드 유형을 선택합니다.</td>
        </tr>
        <tr>
            <td role="rowheader">[!UICONTROL 특정 레코드 유형]</td>
            <td>읽을 특정 유형의 레코드를 선택합니다. 선택한 레코드 유형을 기반으로 합니다.</td>
        </tr>
        <tr>
            <td role="rowheader">[!UICONTROL ID] </td>
            <td >삭제할 레코드의 ID를 입력하거나 매핑합니다.</td>
        </tr>
    </tbody>
</table>

#### [!UICONTROL 레코드 나열]

이 검색 모듈은 지정된 형식의 레코드 목록을 검색합니다.

<table style="table-layout:auto"> 
      <col/>
      <col/>
      <tbody>
          <tr>
              <td role="rowheader">[!UICONTROL Connection]</td>
              <td>연결 방법에 대한 지침은 [!DNL Workday] 계정 대상 [!DNL Workfront Fusion]를 참조하십시오. <a href="#Connect" class="MCXref xref" >Connect [!DNL Workday] to [!DNL Workfront Fusion]</a></td>
          </tr>
          <tr>
              <td  role="rowheader">[!UICONTROL 레코드 유형]</td>
              <td>검색할 레코드 유형을 선택합니다.</td>
          </tr>
          <tr>
              <td role="rowheader">[!UICONTROL 제한]</td>
              <td >
                  <p>각 시나리오 실행 주기 동안 모듈이 검색할 최대 레코드 수를 입력하거나 매핑합니다.</p>
              </td>
          </tr>
      </tbody>
  </table>
