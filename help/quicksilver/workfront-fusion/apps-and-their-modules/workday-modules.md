---
filename: workday-modules
content-type: reference
product-previous: workfront-fusion
product-area: workfront-integrations
keywords: 커넥터
navigation-topic: apps-and-their-modules
title: Workday 모듈
description: Adobe Workfront Fusion 시나리오에서는  [!DNL Workday]을(를) 사용하는 워크플로를 자동화하고 여러 타사 애플리케이션 및 서비스에 연결할 수 있습니다.
author: Becky
feature: Workfront Fusion
exl-id: 535573e0-b6ad-43a2-b7cb-ed32d1dc8d16
source-git-commit: 27fb07b7b19bab25bb7ee925e722ccace3bea628
workflow-type: tm+mt
source-wordcount: '1030'
ht-degree: 1%

---

# [!DNL Workday]개 모듈

[!DNL Adobe Workfront Fusion] 시나리오에서는 [!DNL Workday]을(를) 사용하는 워크플로를 자동화하고 여러 타사 응용 프로그램 및 서비스에 연결할 수 있습니다.

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

[!DNL Workday] 모듈을 사용하려면 다음을 수행해야 합니다.

* [!DNL Workday] 계정이 있습니다.

* [!DNL Workday]에서 OAuth 응용 프로그램을 만듭니다. 자세한 내용은 [!DNL Workday] 설명서를 참조하십시오.

## Workday API 정보

Workday 커넥터는 다음을 사용합니다.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">기본 URL</td> 
   <td>https://{{connection.servicesUrl}}/api</td> 
  </tr>
  <tr> 
   <td role="rowheader">API 태그</td> 
   <td>v1.6.4</td> 
  </tr>
 </tbody> 
 </table>

## [!DNL Workday]을(를) [!DNL Workfront Fusion]에 연결

1. [!DNL Workfront Fusion] 모듈에서 [!UICONTROL 연결] 필드 옆의 [!UICONTROL 추가]를 클릭합니다

2. 다음 필드를 채웁니다.

   <table style="table-layout:auto"> 
        <col/>
        <col/>
        <tbody>
            <tr>
                <td role="rowheader">
                    <p role="rowheader">[!UICONTROL 연결 이름]</p>
                </td>
                <td>연결 이름 입력</td>
            </tr>
            <tr>
                <td  role="rowheader">[!UICONTROL Workday 호스트]</td>
                <td><code>https://</code> 없이 [!DNL Workday] 호스트의 주소를 입력하십시오. 예: <code>mycompany.workday.com</code>.</td>
            </tr>
            <tr>
                <td role="rowheader">[!UICONTROL Services URL]</td>
                <td><code>https://</code> 없이 [!DNL Workday] 웹 서비스의 주소를 입력하십시오. 예: <code>mycompany-services.workday.com</code>.</td>
            </tr>
            <tr>
                <td  role="rowheader">[!UICONTROL 테넌트 이름]</td>
                <td>이 [!DNL Workday] 계정의 테넌트를 입력하십시오. 테넌트는 조직의 식별자이며, Workday에 로그인하는 데 사용하는 URL에서 볼 수 있습니다. 예: 주소 <code>https://www.myworkday.com/mycompany</code>에서 테넌트는 <code>mycompany</code>입니다.</td>
            </tr>
            <tr>
                <td role="rowheader">[!UICONTROL 클라이언트 ID]</td>
                <td>이 연결에서 사용하는 [!DNL Workday] 응용 프로그램의 클라이언트 ID를 입력하십시오. [!DNL Workday]에서 응용 프로그램을 만들 때 이 오류가 발생합니다.</td>
            </tr>
            <tr>
                <td  role="rowheader">[!UICONTROL 클라이언트 암호]</td>
                <td>이 연결에서 사용하는 [!DNL Workday] 응용 프로그램의 클라이언트 암호를 입력하십시오. [!DNL Workday]에서 응용 프로그램을 만들 때 이 오류가 발생합니다.</td>
            </tr>
            <tr>
                <td role="rowheader">[!UICONTROL 세션 시간 초과(분)]</td>
                <td >인증 토큰이 만료된 후 시간(분)을 입력합니다.</td>
            </tr>
        </tbody>
    </table>


3. 연결을 저장하고 모듈로 돌아가려면 [!UICONTROL 계속]을 클릭하세요.

## [!DNL Workday]개 모듈 및 해당 필드

[!DNL Workday] 모듈을 구성할 때 [!DNL Workfront Fusion]에 아래 나열된 필드가 표시됩니다. 앱 또는 서비스의 액세스 수준과 같은 요소에 따라 이러한 필드와 함께 [!DNL Workday] 필드가 추가로 표시될 수 있습니다. 모듈의 굵은 제목은 필수 필드를 나타냅니다.

필드나 함수 위에 맵 단추가 표시되면 이 단추를 사용하여 해당 필드에 대한 변수와 함수를 설정할 수 있습니다. 자세한 내용은 [한 모듈에서 다른 모듈로 정보를 매핑 [!DNL Adobe Workfront Fusion]](../../workfront-fusion/mapping/map-information-between-modules.md)을 참조하십시오.

![](assets/map-toggle-350x74.png)

* [액션](#action)

* [검색](#search)


### 액션

* [[!UICONTROL 레코드 만들기]](#create-a-record)

* [[!UICONTROL 레코드 삭제]](#delete-a-record)

* [[!UICONTROL 사용자 지정 API 호출 만들기]](#make-a-custom-api-call)

* [[!UICONTROL 레코드 업데이트]](#update-a-record)


#### [!UICONTROL 레코드 만들기]

이 작업 모듈은 [!DNL Workday]에 단일 레코드를 만듭니다.

<table style="table-layout:auto"> 
    <col/>
    <col/>
    <tbody>
        <tr>
            <td role="rowheader">[!UICONTROL Connection]</td>
            <td>[!DNL Workday] 계정을 Workfront Fusion에 연결하는 방법에 대한 지침은 <a href="#Connect" class="MCXref xre[!DNL ]f" >[!DNL Workday]을(를) [!DNL Workfront Fusion]</a>에 연결 을 참조하십시오.</td>
        </tr>
        <tr>
            <td  role="rowheader">[!UICONTROL 레코드 유형]</td>
            <td>만들려는 레코드 유형을 선택합니다.</td>
        </tr>
        <tr>
            <td role="rowheader">[!UICONTROL ID] </td>
            <td>만들려는 레코드의 ID를 입력하거나 매핑합니다.</td>
        </tr>
        <tr>
            <td role="rowheader">[!UICONTROL 하위 리소스 ID]</td>
            <td >만들려는 하위 리소스의 ID를 입력하거나 매핑합니다.</td>
        </tr>
    </tbody>
</table>

#### [!UICONTROL 레코드 삭제]

이 작업 모듈은 [!DNL Workday]에서 단일 레코드를 삭제합니다.

<table style="table-layout:auto"> 
    <col class="TableStyle-TableStyle-List-options-in-steps-Column-Column1">
    </col>
    <col class="TableStyle-TableStyle-List-options-in-steps-Column-Column2">
    </col>
    <tbody>
        <tr>
            <td role="rowheader">[!UICONTROL Connection]</td>
            <td>[!DNL Workday] 계정을 [!DNL Workfront Fusion]에 연결하는 방법에 대한 지침은 <a href="#Connect" class="MCXref xre[!DNL ]f" >[!DNL Workday]을(를) [!DNL Workfront Fusion]</a>에 연결 을 참조하십시오.</td>
        </tr>
        <tr>
            <td  role="rowheader">[!UICONTROL 레코드 유형]</td>
            <td>삭제할 레코드 유형을 선택합니다.</td>
        </tr>
        <tr>
            <td role="rowheader">[!UICONTROL 특정 레코드 유형]</td>
            <td>삭제하려는 특정 레코드 유형을 선택합니다. 선택한 레코드 종류를 기반으로 합니다.</td>
        </tr>
        <tr>
            <td  role="rowheader">[!UICONTROL 하위 리소스 ID]</td>
            <td>삭제할 하위 리소스의 ID를 입력하거나 매핑합니다.</td>
        </tr>
        <tr>
            <td role="rowheader">[!UICONTROL ID] </td>
            <td >삭제할 레코드의 ID를 입력하거나 매핑합니다.</td>
        </tr>
    </tbody>
</table>


### [!UICONTROL 사용자 지정 API 호출 만들기]

이 작업 모듈을 사용하면 [!DNL Workday] API에 대해 사용자 지정 인증된 호출을 수행할 수 있습니다. 이렇게 하면 다른 [!DNL Workday] 모듈에서 수행할 수 없는 데이터 흐름 자동화를 만들 수 있습니다.

이 모듈을 구성할 때 다음 필드가 표시됩니다.

이 모듈은 API 호출의 헤더 및 본문과 함께 상태 코드를 반환합니다.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <p>[!DNL Connection]</p> </td> 
            <td>[!DNL Workday] 계정을 [!DNL Workfront Fusion]에 연결하는 방법에 대한 지침은 <a href="#Connect" class="MCXref xre[!DNL ]f" >[!DNL Workday]을(를) [!DNL Workfront Fusion]</a>에 연결 을 참조하십시오.</td>
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL URL]</td> 
   <td><code style="color: #ff1493;">https://&lt;tenantHostname>/api/&lt;serviceName>/&lt;version>/&lt;tenant></code>과(와) 관련된 경로를 입력하십시오.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL 메서드]</td> 
   <td> <p>API 호출을 구성하는 데 필요한 HTTP 요청 메서드를 선택합니다. 자세한 내용은 [!DNL Adobe Workfront Fusion]</a>에서 <a href="../../workfront-fusion/modules/http-request-methods.md" class="MCXref xref">HTTP 요청 메서드를 참조하십시오.</p> </td> 
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
   <td> <p>표준 JSON 개체의 형태로 API 호출에 대한 본문 콘텐츠를 추가합니다.</p> <p>참고:  <p>JSON에서 <code>if</code>과(와) 같은 조건문을 사용할 때 따옴표를 조건문 외부에 넣으십시오.</p> 
     <div class="example" data-mc-autonum="<b>Example: </b>"> 
      <p> <img src="assets/quotes-in-json-350x120.png" style="width: 350;height: 120;"> </p> 
     </div> </p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL 레코드 업데이트]

이 작업 모듈은 [!DNL Workday]의 단일 레코드를 업데이트합니다.

<table style="table-layout:auto"> 
    <col/>
    <col/>
    <tbody>
        <tr>
            <td role="rowheader">[!UICONTROL Connection]</td>
            <td>[!DNL Workday] 계정을 Workfront Fusion에 연결하는 방법은 <a href="#Connect" class="MCXref xref" >[!UICONTROL [!DNL Workday]을(를) Workfront Fusion에 연결</a>을 참조하십시오.</td>
        </tr>
        <tr>
            <td  role="rowheader">레코드 유형</td>
            <td>업데이트하려는 레코드 종류 t[!UICONTROL ]를 선택합니다.</td>
        </tr>
        <tr>
            <td role="rowheader">[!UICONTROL ID] </td>
            <td>업데이트할 레코드의 ID를 입력하거나 매핑합니다.</td>
        </tr>
        <tr>
            <td role="rowheader">[!UICONTROL 하위 리소스 ID]</td>
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
            <td>[!DNL Workday] 계정을 Workfront Fusion에 연결하는 방법은 <a href="#Connect" class="MCXref xref" >[!UICONTROL [!DNL Workday]을(를) Workfront Fusion에 연결</a>을 참조하십시오.</td>
        </tr>
        <tr>
            <td  role="rowheader">[!UICONTROL 레코드 유형]</td>
            <td>삭제할 레코드 유형을 선택합니다.</td>
        </tr>
        <tr>
            <td role="rowheader">[!UICONTROL 특정 레코드 유형]</td>
            <td>읽고자 하는 특정 레코드 유형을 선택합니다. 선택한 레코드 종류를 기반으로 합니다.</td>
        </tr>
        <tr>
            <td role="rowheader">[!UICONTROL ID] </td>
            <td >삭제할 레코드의 ID를 입력하거나 매핑합니다.</td>
        </tr>
    </tbody>
</table>

#### [!UICONTROL 레코드 나열]

이 검색 모듈은 지정된 유형의 레코드 목록을 검색합니다.

<table style="table-layout:auto"> 
      <col/>
      <col/>
      <tbody>
          <tr>
              <td role="rowheader">[!UICONTROL Connection]</td>
              <td>[!DNL Workday] 계정을 [!DNL Workfront Fusion]에 연결하는 방법에 대한 지침은 <a href="#Connect" class="MCXref xref" >[!DNL Workday]을(를) [!DNL Workfront Fusion]</a>에 연결</td>
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
