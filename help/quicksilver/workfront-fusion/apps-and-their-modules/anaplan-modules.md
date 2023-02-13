---
content-type: reference
product-previous: workfront-fusion
product-area: workfront-integrations
keywords: 커넥터
navigation-topic: apps-and-their-modules
title: Anaplan 모듈
description: 에서 [!DNL Adobe Workfront Fusion] 시나리오에서는 Anaplan을 사용하는 워크플로우를 자동화하고 이를 여러 타사 애플리케이션 및 서비스에 연결할 수 있습니다.
author: Becky
feature: Workfront Fusion, Workfront Integrations and Apps
exl-id: 03bcd0a4-c8ec-4f44-b1e1-b57e79595309
source-git-commit: 8963acee01aac6117a731147d9288fddbe3e812f
workflow-type: tm+mt
source-wordcount: '1796'
ht-degree: 1%

---

# [!DNL Anaplan] 모듈

에서 [!DNL Adobe Workfront Fusion] 시나리오, [!DNL Anaplan]여러 타사 애플리케이션 및 서비스에 연결할 수 있습니다.

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

를 사용하기 전에 [!DNL Anaplan] 커넥터, 다음 전제 조건이 충족되는지 확인해야 합니다.

* 활성 상태여야 합니다. [!UICONTROL 안팔란] 계정이 필요합니다.
* 작업 공간, 모델 및 기타 를 구성해야 합니다 [!DNL Anaplan] 개체 [!UICONTROL 안팔란] 이전 [!DNL Workfront Fusion] 그들과 상호 작용할 수 있습니다.

## Connect [!DNL Anaplan] to [!DNL Workfront Fusion] {#connect-anaplan-to-workfront-fusion}

에 대한 연결을 만들려면 [!DNL Anaplan] 모듈:

1. 클릭 **[!UICONTROL 추가]** 다음 [!UICONTROL 연결] 상자.
1. 연결 유형을 선택합니다.

   <table style="table-layout:auto">
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">[!DNL Anaplan] [!UICONTROL Basic]</td> 
      <td> <p>An [!DNL Anaplan] [!UICONTROL Basic] 연결에는 연결을 만들려면 전자 메일 주소와 암호만 필요합니다. </p> <p>연결 이름을 입력한 다음 이메일 주소와 암호를 입력합니다 [!DNL Anaplan] 계정이 필요합니다.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!DNL Anaplan] [!UICONTROL CA 인증서]</td> 
      <td> <p>An [!DNL Anaplan] [!UICONTROL CA Certificate] 연결에 [!UICONTROL 인증서 키], [!UICONTROL Encoded Data] 및 [!UICONTROL Encoded Signed Data]가 필요합니다. 이러한 생성은 [!DNL Anaplan] 계정이 필요합니다. 자세한 내용은 [!DNL Anaplan] 설명서.</p> <p>연결 이름을 입력한 다음, 사용자 ID에서 생성한 [!UICONTROL 인증서 키], [!UICONTROL Encoded Data] 및 [!UICONTROL Encoded Signed Data]를 입력합니다 [!DNL Anaplan] 계정이 필요합니다.</p> </td> 
     </tr> 
    </tbody> 
   </table>

1. 클릭 **[!UICONTROL 계속]** 연결을 저장하고 모듈로 돌아가려면 를 클릭합니다.

## [!DNL Anaplan] 모듈 및 해당 필드

구성 시 [!DNL Anaplan] 모듈, [!DNL Workfront Fusion] 아래 나열된 필드를 표시합니다. 이와 함께 추가 [!DNL Anaplan] 앱이나 서비스에서 액세스 수준과 같은 요소에 따라 필드가 표시될 수 있습니다. 모듈에서 굵게 표시된 제목은 필수 필드를 나타냅니다.

필드 또는 함수 위에 맵 단추가 표시되면 이 단추를 사용하여 해당 필드에 대한 변수와 함수를 설정할 수 있습니다. 자세한 내용은 [의 한 모듈에서 다른 모듈로 정보 매핑 [!DNL Adobe Workfront Fusion]](../../workfront-fusion/mapping/map-information-between-modules.md).

![](assets/map-toggle-350x74.png)

* [Triggers](#triggers)
* [액션](#actions)
* [검색 결과](#searches)

### Triggers

#### [!DNL Watch records]

이 트리거 모듈은 선택한 유형의 레코드를 만들거나 업데이트할 때 시나리오를 시작합니다.

>[!NOTE]
>
>이 모듈은 새 레코드의 데이터를 반환합니다. 수정된 기존 레코드의 데이터를 반환하지 않습니다.

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td> 
   <td>연결 생성에 대한 지침은 [!DNL Anaplan]를 참조하십시오. <a href="#connect-anaplan-to-workfront-fusion" class="MCXref xref">Connect [!DNL Anaplan] to [!DNL Workfront Fusion]</a> 참조하십시오.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">볼 개체 유형</td> 
   <td>보려는 항목 유형을 선택합니다. 시나리오는 이 유형의 레코드가 만들어지거나 업데이트될 때 시작됩니다.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">&lt;object&gt; ID</td> 
   <td>보려는 객체와 연관된 모델 또는 모듈과 같이 Anaplan에 있는 객체의 ID를 입력합니다</td> 
  </tr> 
  <tr> 
   <td role="rowheader">제한</td> 
   <td> <p>각 시나리오 실행 주기 동안 모듈을 [action]에 넣을 최대 레코드 수를 입력하거나 매핑합니다.</p> </td> 
  </tr> 
 </tbody> 
</table>

### 액션

* [[!UICONTROL 목록 항목 만들기]](#create-a-list-item)
* [[!UICONTROL 사용자 지정 API 호출 만들기]](#make-a-custom-api-call)
* [[!UICONTROL 레코드 읽기]](#read-a-record)
* [[!UICONTROL 작업 실행]](#run-an-action)
* [[!UICONTROL 레코드 업데이트]](#update-a-record)
* [[!UICONTROL 파일 업로드]](#upload-a-file)

#### [!UICONTROL 목록 항목 만들기]

이 작업 모듈은 Anaplan의 목록에 새 항목을 추가합니다.

<table style="table-layout:auto">
    <tr>
        <td>[!UICONTROL Connection]</td>
        <td>연결 생성에 대한 지침은 [!DNL Anaplan]를 참조하십시오. <a href="#connect-anaplan-to-workfront-fusion" class="MCXref xref">Connect [!DNL Anaplan] to [!DNL Workfront Fusion]</a> 참조하십시오.</td>
    </tr>
    <tr>
        <td>[!UICONTROL 작업 공간 ID]</td>
        <td>항목을 추가할 목록이 포함된 Anaplan Workspace의 ID를 선택하거나 매핑합니다.</td>
    </tr>
    <tr>
        <td>[!UICONTROL Model ID]</td>
        <td>항목을 추가할 목록이 포함된 모델의 ID를 선택하거나 매핑합니다.</td>
    </tr>
    <tr>
        <td>[!UICONTROL 목록 ID]</td>
        <td>항목을 만들 목록의 ID를 선택하거나 매핑합니다.</td>
    </tr>
    <tr>
        <td>[!UICONTROL Name]</td>
        <td>새 항목의 이름을 입력합니다.</td>
    </tr>
    <tr>
        <td>[!UICONTROL Code]</td>
        <td>새 품목에 대한 코드를 입력합니다. 코드는 이름이 같은 라인 항목을 구분할 수 있도록 사용자가 생성한 코드입니다.</td>
    </tr>
    <tr>
        <td>[!UICONTROL Parent]</td>
        <td>아래에 새 항목을 생성할 상위 항목의 이름을 입력합니다.</td>
    </tr>
    <tr>
        <td>[!UICONTROL Properties]</td>
        <td>항목을 추가하려는 목록에 사용자 지정 속성이 있는 경우 값을 추가할 속성을 선택한 다음 값을 추가합니다.</td>
    </tr>
    <tr>
        <td>[!UICONTROL Subsets]</td>
        <td>항목을 추가하려는 목록에 사용자 지정 하위 세트가 있는 경우 항목을 추가할 하위 세트를 선택한 다음 을 선택합니다 <b>[!UICONTROL Yes]</b> 새 항목을 해당 하위 세트에 추가하려면</td>
    </tr>
</table>

#### [!UICONTROL 사용자 지정 API 호출 만들기]

이 모듈에서 [!DNL Anaplan] API.

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td> 
   <td>연결 생성에 대한 지침은 [!DNL Anaplan]를 참조하십시오. <a href="#connect-anaplan-to-workfront-fusion" class="MCXref xref">Connect [!DNL Anaplan] to [!DNL Workfront Fusion]</a> 참조하십시오.</td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL URL]</p> </td> 
   <td> <p>상대 경로 입력 <code>https://api.anaplan.com/2/0/</code></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL 메서드]</p> </td> 
   <td> <p>API 호출을 구성하는 데 필요한 HTTP 요청 메서드를 선택합니다. 자세한 내용은 <a href="../../workfront-fusion/modules/http-request-methods.md" class="MCXref xref">의 HTTP 요청 메서드 [!DNL Adobe Workfront Fusion]</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Headers]</td> 
   <td> <p>요청의 헤더를 표준 JSON 개체 형태로 추가합니다.</p> <p>For example, <code>{"Content-type":"application/json"}</code></p> <p>[!DNL Workfront Fusion] 인증 헤더를 자동으로 추가합니다.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL 쿼리 문자열] </td> 
   <td> <p>요청 쿼리 문자열을 입력합니다.</p> </td> 
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

#### [!UICONTROL 레코드 삭제]

이 작업 모듈은 기존 레코드를 삭제합니다.

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td> 
   <td>연결 생성에 대한 지침은 [!DNL Anaplan]를 참조하십시오. <a href="#connect-anaplan-to-workfront-fusion" class="MCXref xref">Connect [!DNL Anaplan] to [!DNL Workfront Fusion]</a> 참조하십시오.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL 작업 공간 ID]</td> 
   <td>삭제할 객체가 포함된 Anaplan Workspace의 ID를 선택하거나 매핑합니다.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Model ID]</td> 
   <td>삭제할 객체가 포함된 모델의 ID를 입력하거나 매핑합니다.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">삭제</td> 
   <td> <p>삭제할 객체 유형을 선택합니다.</p> 
    <ul> 
     <li> <p><b>개 액션</b> </p> <p>삭제할 작업을 선택하거나 매핑합니다.</p> </li> 
     <li> <p><b>목록 항목</b> </p> <p>항목을 삭제할 목록을 선택한 다음 삭제할 항목의 ID 또는 코드를 입력하거나 매핑합니다</p>  </li> 
     <li> <p><b>[!UICONTROL File]</b> </p> <p>삭제할 파일을 선택하거나 매핑합니다.</p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL 레코드 읽기]

이 작업 모듈은 단일 레코드를 읽습니다.

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td> 
   <td>연결 생성에 대한 지침은 [!DNL Anaplan]를 참조하십시오. <a href="#connect-anaplan-to-workfront-fusion" class="MCXref xref">Connect [!DNL Anaplan] to [!DNL Workfront Fusion]</a> 참조하십시오.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL 레코드 유형]</td> 
   <td> <p>읽을 레코드 유형을 선택합니다.</p> 
    <ul> 
     <li> <p><b>모델</b> </p> <p>읽을 모델의 ID를 선택하거나 매핑합니다</p> </li> 
     <li> <p><b>모델 목록</b> </p> <p>읽을 목록이 들어 있는 작업 공간 및 모델의 ID를 선택하거나 매핑한 다음 목록을 선택합니다. [!UICONTROL 데이터 유형] 필드에서 데이터를 읽을지 아니면 메타데이터를 읽을지 선택합니다.</p> </li> 
     <li> <p><b>모델 버전</b> </p> <p>읽을 모델의 ID를 선택하거나 매핑합니다.</p> </li> 
     <li> <p><b>사용자</b> </p> <p>사용 중인 계정 소유자 또는 다른 사용자에 대한 데이터를 반환할지 여부를 선택합니다. 다른 사용자를 선택하는 경우 사용자의 이름을 선택합니다.</p> </li> 
     <li> <p><b>작업 공간</b> </p> <p>읽을 작업 공간의 ID를 선택하거나 매핑합니다.</p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL 작업 실행]

이 작업 모듈은 작업을 가져오기, 내보내기, 삭제 또는 처리합니다.

<table style="table-layout:auto"> 
     <col/>
     <col/>
     <tbody>
      <tr>
        <td role="rowheader">[!UICONTROL Connection]</td>
        <td>연결 생성에 대한 지침은 [!DNL Anaplan]를 참조하십시오. <a href="#Connect" class="MCXref xref" >[!UICONTROL Anaplan을 Workfront Fusion에 연결]</a> 참조하십시오.</td>
      </tr>
      <tr>
        <td role="rowheader">[!UICONTROL 작업 공간 ID]</td>
        <td>의 ID를 선택하거나 매핑합니다 [!DNL Anaplan] 작업을 수행할 작업 공간</td>
      </tr>
      <tr >
        <td role="rowheader">[!UICONTROL Model ID]</td>
        <td>작업을 수행할 모델의 ID를 선택하거나 매핑합니다.</td>
      </tr>
      <tr>
        <td role="rowheader">[!UICONTROL 작업 유형]</td>
        <td>
          <p>수행할 작업을 선택합니다</p>
            <ul>
              <li>
                <p><b>[!UICONTROL Delete]</b>
                </p>
                <p>삭제할 작업의 ID를 입력하거나 매핑합니다.</p>
              </li>
              <li>
                <p><b>[!UICONTROL Export]</b>
                </p>
                <p>사용할 내보내기 정의의 ID를 입력하거나 매핑합니다. 다음 파일 형식으로 내보낼 수 있습니다.</p>
                  <ul>
                    <li>
                      <p>XLS</p>
                    </li>
                    <li>
                      <p>XLSX</p>
                    </li>
                    <li>
                      <p>CSV</p>
                    </li>
                  </ul>
                </li>
                <li>
                  <p><b>[!UICONTROL 가져오기] </b>
                  </p>
                  <p style="font-weight: normal;">사용할 가져오기 정의의 ID를 입력하거나 매핑합니다.</p>
                </li>
                <li>
                 <p><b>[!UICONTROL Process]</b>
                 </p>
                  <p>사용할 프로세스 ID를 입력하거나 매핑합니다. </p>
                </li>
              </ul>
            </td>
          </tr>
        </tbody>
      </table>


#### [!UICONTROL 레코드 업데이트]

이 작업 모듈은 [!UICONTROL 안팔란].

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td> 
   <td>연결 생성에 대한 지침은 [!DNL Anaplan]를 참조하십시오. <a href="#connect-anaplan-to-workfront-fusion" class="MCXref xref">Connect [!DNL Anaplan] to [!DNL Workfront Fusion]</a> 참조하십시오.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL 레코드 유형]</td> 
   <td> <p>업데이트할 레코드 유형을 선택합니다.</p> 
    <ul> 
     <li> <p><b>[!UICONTROL List item]</b> </p> <p>필드에 대해서는 다음을 참조하십시오 <a href="#create-a-list-item" class="MCXref xref">목록 항목 만들기</a> 참조하십시오.</p> </li> 
     <li> <p><b>[!UICONTROL Module cell data]</b> </p> <p>셀 데이터를 업데이트하면 해당 데이터를 사용하는 모든 다운스트림 계산도 업데이트됩니다.</p> <p>다음 필드를 채웁니다.</p> 
      <ul> 
       <li> <p><b>[!UICONTROL Model ID]</b> </p> <p>업데이트할 셀이 포함된 모델을 선택하거나 매핑합니다.</p> </li> 
       <li> <p><b>[!UICONTROL 모듈 ID]</b> </p> <p>업데이트할 셀이 포함된 모듈을 선택하거나 매핑합니다</p> </li> 
       <li> <p><b>[!UICONTROL 라인 항목 이름]</b> </p> <p>업데이트할 셀의 라인 항목을 선택하거나 매핑합니다</p> </li> 
       <li> <p style="font-weight: bold;">[!UICONTROL Dimension ID]</p> <p>라인 항목에 있는 차원을 선택하거나 매핑합니다.</p> 
       <p><b>참고: </b> 
       <ul>
       <li> Dimension 키(값)는 다음 중 하나여야 합니다. <code>dimensionName</code> (다음) 또는 <code>dimensionId</code> (ID).</li>
       <li>항목 키(값)는 <code>itemName</code> (텍스트), <code>itemCode</code> (텍스트) 또는 <code>itemId</code> (ID).</li>
       <li>Dimension 및 항목 키는 같은 유형(텍스트 또는 ID)이어야 합니다.
       </ul>
        </p> 
        <p>차원에 대한 자세한 내용을 보려면 [!DNL Anaplan Anapedia].</p> </li> 
       <li> <p><b>[!UICONTROL Value]</b> </p> <p>셀의 새 값을 입력하거나 매핑합니다.</p> </li> 
      </ul> </li> 
     <li> <p><b>[!UICONTROL Model 현재 회계 연도]</b> </p> <p>회계 연도를 갱신할 모델의 작업공간 ID 및 모델 ID를 입력한 다음 모델에 대한 새 연도를 입력하거나 매핑합니다.</p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL 파일 업로드]

이 작업 모듈은 파일을 Anaplan에 업로드합니다. 파일이 이미 Anaplan에 업로드된 것 같습니다. 이 모듈을 사용하여 Anaplan 내의 추가 위치에 업로드할 수 있습니다.
<table style="table-layout:auto">
<col>
<col>
<tbody>
<tr>
<td role="rowheader">[!UICONTROL Connection]</td>
<td>연결 생성에 대한 지침은 [!DNL Anaplan]를 참조하십시오. <a href="#connect-anaplan-to-workfront-fusion" class="MCXref xref">Connect [!DNL Anaplan] to [!DNL Workfront Fusion]</a> 참조하십시오.</td>
</tr>
<tr>
<td role="rowheader">[!UICONTROL 작업 공간 ID]</td>
<td>의 ID를 선택하거나 매핑합니다 [!DNL Anaplan] 파일을 업로드할 작업 공간입니다.</td>
</tr>
<tr>
<td role="rowheader">[!UICONTROL Model ID]</td>
<td>파일을 업로드할 모델의 ID를 선택하거나 매핑합니다.</td>
</tr>
<tr>
<td role="rowheader">[!UICONTROL 파일 ID]</td>
<td>업로드할 파일의 ID를 선택하거나 매핑합니다.</td>
</tr>
</tbody>
</table>
</div>

### 검색 결과

#### [!UICONTROL 레코드 가져오기]

이 검색 모듈은 선택한 유형의 모든 액세스 가능한 레코드를 반환합니다.

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td> 
   <td>연결 생성에 대한 지침은 [!DNL Anaplan]를 참조하십시오. <a href="#connect-anaplan-to-workfront-fusion" class="MCXref xref">Connect [!DNL Anaplan] to [!DNL Workfront Fusion]</a> 참조하십시오.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL 레코드 유형]</td> 
   <td> <p>검색할 레코드 유형을 선택합니다.</p> 
      <ul> 
       <li> <p><b>[!UICONTROL Workspaces]</b> </p> </li> 
       <li> <p><b>[!UICONTROL Models]</b> </p> </li> 
       <li> <p><b>[!UICONTROL Line items]</b> </p> <p>를 포함하는 모델의 ID를 선택하거나 매핑합니다 [!DNL line] 검색할 항목입니다.</p> </li> 
       <li> <p><b>[!UICONTROL 모델 목록]</b> </p> <p>검색할 모델 목록이 포함된 작업공간 및 모델 ID의 ID를 선택하거나 매핑합니다.</p> </li> 
       <li> <p><b>[!UICONTROL Model Calendar]</b> </p> <p>검색할 모델 달력이 포함된 작업 공간의 ID를 선택하거나 매핑합니다.</p> </li> 
       <li> <p><b>모델 버전</b> </p> </li> 
       <li> <p>검색할 모델 버전이 포함된 모델의 ID를 선택하거나 매핑합니다. [!UICONTROL]</p> </li> 
       <li> <p><b>[!UICONTROL Users]</b> </p> </li> 
       <li> <p><b>[!UICONTROL Views]</b> </p> <p>모듈별로 뷰를 선택할지 모델별로 선택할지 여부를 선택한 다음 검색할 뷰가 포함된 모듈이나 모델의 ID를 선택하거나 매핑합니다.</p> </li> 
      </ul> 
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL 작업 공간 크기 반환]</td> 
   <td>작업 공간의 현재 크기에 대한 예측을 반환하려면 이 옵션을 활성화합니다. 이 추정은 작업 공간에 포함된 모든 모듈의 크기를 기반으로 합니다.</td> 
  </tr> 
 </tbody> 
</table>
