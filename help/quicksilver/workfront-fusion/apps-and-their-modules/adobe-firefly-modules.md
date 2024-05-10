---
content-type: reference
product-previous: workfront-fusion
product-area: workfront-integrations
keywords: 커넥터
navigation-topic: apps-and-their-modules
title: Adobe Firefly 모듈
description: 다음에서 [!DNL Adobe Workfront Fusion] 시나리오에서는 다음을 사용하는 워크플로를 자동화할 수 있습니다 [!DNL Adobe Firefly]을 여러 타사 응용 프로그램 및 서비스에 연결할 수 있습니다.
author: Becky
feature: Workfront Fusion, Digital Content and Documents
source-git-commit: c932f869de9ff842a7bbb809bc60ec1d53350b51
workflow-type: tm+mt
source-wordcount: '1215'
ht-degree: 0%

---

# [!DNL Adobe Firefly] 모듈

다음에서 [!DNL Adobe Workfront Fusion] 시나리오에서는 다음을 사용하는 워크플로를 자동화할 수 있습니다 [!DNL Adobe Firefly]을 여러 타사 응용 프로그램 및 서비스에 연결할 수 있습니다.

시나리오를 만드는 방법에 대한 지침이 필요한 경우 [시나리오 만들기](../../workfront-fusion/scenarios/create-a-scenario.md).

모듈에 대한 자세한 내용은 [의 모듈 [!DNL Adobe Workfront Fusion]](../../workfront-fusion/modules/modules.md).

## 액세스 요구 사항

이 문서의 기능을 사용하려면 다음 액세스 권한이 있어야 합니다.

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] 플랜</td> 
   <td> <p>임의</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader">[!DNL Adobe Workfront] 라이센스</td> 
   <td> <p>새로운 기능: [!UICONTROL Standard]</p><p>또는</p><p>현재: [!UICONTROL Work] 이상</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront Fusion] 라이센스**</td> 
   <td>
   <p>현재: 아니요 [!DNL Workfront Fusion] 라이센스 요구 사항.</p>
   <p>또는</p>
   <p>레거시: 모두 </p>
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader">제품</td> 
   <td>
   <p>신규:</p> <ul><li>[!UICONTROL Select] 또는 [!UICONTROL Prime] [!DNL Workfront] 플랜: 조직에서 구매해야 합니다. [!DNL Adobe Workfront Fusion].</li><li>[!UICONTROL Ultimate] [!DNL Workfront] 플랜: [!DNL Workfront Fusion] 포함됩니다.</li></ul>
   <p>또는</p>
   <p>현재: 조직에서 구매해야 합니다. [!DNL Adobe Workfront Fusion].</p>
   </td> 
  </tr>
 </tbody> 
</table>

이 표의 정보에 대한 자세한 내용은 [Workfront 설명서의 액세스 요구 사항](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

다음에 대한 정보: [!DNL Adobe Workfront Fusion] 라이센스, 참조 [[!DNL Adobe Workfront Fusion] 라이선스](../../workfront-fusion/get-started/license-automation-vs-integration.md).

## 전제 조건

을(를) 사용하기 전에 [!DNL Adobe Firefly] connector에서 다음 전제 조건이 충족되는지 확인해야 합니다.

* 활성 상태가 있어야 합니다. [!DNL Adobe Firefly] 계정입니다.

## 에 대한 연결 만들기 [!DNL Adobe Firefly]

에 대한 연결을 만들려면 [!DNL Adobe Firefly] 모듈:

1. 클릭 **[!UICONTROL 추가]** 연결 상자 옆에 있습니다.

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
        <td>서비스 계정에 연결할지 또는 개인 계정에 연결할지 선택합니다.</td>
        </tr>
        <tr>
        <td role="rowheader">[!UICONTROL 클라이언트 ID]</td>
        <td>[!UICONTROL Adobe] [!UICONTROL 클라이언트 ID]를 입력합니다. 이 로그는 의 [!UICONTROL 자격 증명] 세부 정보 섹션에서 찾을 수 있습니다. [!DNL Adobe Developer Console]</td>
        </tr>
        <tr>
        <td role="rowheader">[!UICONTROL 클라이언트 암호]</td>
        <td>다음을 입력하십시오. [!DNL Adobe] [!UICONTROL 클라이언트 암호]. 이 로그는 의 [!UICONTROL 자격 증명] 세부 정보 섹션에서 찾을 수 있습니다. [!DNL Adobe Developer Console]</td>
        </tr>
      </tbody>
    </table>

1. 클릭 **[!UICONTROL 계속]** 연결을 저장하고 모듈로 돌아갑니다.

## [!DNL Adobe Firefly] 모듈 및 해당 필드

를 구성할 때 [!DNL Adobe Firefly] 모듈, [!DNL Workfront Fusion] 아래 나열된 필드를 표시합니다. 이와 함께 추가 [!DNL Adobe Firefly] 앱이나 서비스의 액세스 수준 등에 따라 필드가 표시될 수 있습니다. 모듈의 굵은 제목은 필수 필드를 나타냅니다.

필드나 함수 위에 맵 단추가 표시되면 이 단추를 사용하여 해당 필드에 대한 변수와 함수를 설정할 수 있습니다. 자세한 내용은 [의 한 모듈에서 다른 모듈로 정보 매핑 [!DNL Adobe Workfront Fusion]](../../workfront-fusion/mapping/map-information-between-modules.md).

![](assets/map-toggle-350x74.png)

### 사용자 지정 API 호출 만들기

이 작업 모듈은 Firefly API에 대한 사용자 지정 호출을 만듭니다.

사용 가능한 특정 API에 대한 내용은 [ADOBE FIREFLY API](https://developer.adobe.com/firefly-services/docs/firefly-api/) Adobe Developer 설명서에서 확인할 수 있습니다.

<table style="table-layout:auto"> 
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">[!UICONTROL Connection]</td>
      <td>에 대한 연결 만들기에 대한 지침: [!DNL Adobe Firefly], 참조 <a href="#create-a-connection-to-adobe-firefly" class="MCXref xref" >에 대한 연결 만들기 [!DNL Adobe Firefly]</a> 이 문서에서.</td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL URL]</td>
      <td>
        <p>상대 경로 입력 <code>https://firefly-api-enterprise-stage.adobe.io/</code>.</p>
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
      <td role="rowheader">[!UICONTROL Body]</td>
   <td> <p>표준 JSON 개체의 형태로 API 호출에 대한 본문 콘텐츠를 추가합니다.</p> <p>참고:  <p>다음과 같은 조건문을 사용할 때 <code>if</code> json에서 따옴표를 조건문 외부에 넣습니다.</p> 
     <div class="example" data-mc-autonum="<b>Example: </b>"> 
      <p> <img src="assets/quotes-in-json-350x120.png" style="width: 350;height: 120;"> </p> 
     </div> </p> </td>     </tr>
  </tbody>
</table>

### 이미지 확장

이 작업 모듈은 선택적으로 사용자가 제공하는 프롬프트의 콘텐츠로 이미지를 확장합니다.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td> 
   <td>에 대한 연결 만들기에 대한 지침: [!DNL Adobe Campaign], 참조 <a href="#create-a-connection-to-adobe-firefly" class="MCXref xref" >에 대한 연결 만들기 [!DNL Adobe Firefly]</a> 이 문서에서.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL 프롬프트]</td> 
   <td>이미지를 확장할 내용에 대한 프롬프트를 입력하거나 매핑합니다. 프롬프트가 제공되지 않으면 이미지가 원본 이미지와 일치하는 콘텐츠로 확장됩니다.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL 확장된 이미지 형식]</td> 
   <td>확장된 이미지를 저장할 파일 형식을 선택합니다.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL 소스 파일]</td> 
   <td>  <p>이전 모듈에서 소스 파일을 선택하거나 소스 파일의 이미지 파일 이름과 이미지 파일(데이터)을 매핑합니다.</p> </td> 
</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Size]</td> 
   <td>확장된 이미지를 표시할 크기를 선택합니다.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL 시드]</td> 
   <td>정수를 입력하거나 매핑합니다. 다른 이미지 모듈 확장에서 이와 동일한 시드를 사용하여 스타일이 다른 유사한 이미지를 생성할 수 있습니다. </td> 
  </tr> 
 </tbody> 
</table>

## 이미지 채우기

이 작업 모듈은 이미지의 마스킹된 영역을 채우며, 원할 경우 제공하는 프롬프트의 콘텐츠로 채웁니다.


<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td> 
   <td>에 대한 연결 만들기에 대한 지침: [!DNL Adobe Campaign], 참조 <a href="#create-a-connection-to-adobe-firefly" class="MCXref xref" >에 대한 연결 만들기 [!DNL Adobe Firefly]</a> 이 문서에서.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL 프롬프트]</td> 
   <td>이미지를 채울 콘텐츠에 대한 프롬프트를 입력하거나 매핑합니다. 프롬프트가 제공되지 않으면 이미지는 원본 이미지와 일치하는 콘텐츠로 채워집니다.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL 채워진 이미지 형식]</td> 
   <td>채워진 이미지를 저장할 파일 형식을 선택합니다.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Image]</td> 
   <td>  <p> 클릭 <b>이미지 추가</b>. 이전 모듈에서 소스 파일을 선택하거나 소스 파일의 이미지 파일 이름과 이미지 데이터를 매핑합니다.</p> </td> 
</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Mask]</td> 
   <td>  <p> 클릭 <b>마스크 추가</b>. 이전 모듈에서 소스 파일을 선택하거나 소스 파일의 마스크 파일 이름과 마스크 데이터를 매핑합니다. 마스크 파일은 생성된 콘텐츠로 채워질 사용자 지정 마스크를 나타냅니다.</p> </td> 
</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Size]</td> 
   <td>채워진 이미지를 표시할 크기를 선택합니다.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL 시드]</td> 
   <td>정수를 입력하거나 매핑합니다. 다른 이미지 모듈 확장에서 이와 동일한 시드를 사용하여 스타일이 다른 유사한 이미지를 생성할 수 있습니다. </td> 
  </tr> 
 </tbody> 
</table>

## 이미지 생성

이 작업 모듈은 사용자가 제공한 프롬프트를 기반으로 및 이미지를 생성합니다. 선택적 참조 이미지를 제공할 수도 있으며, 생성된 이미지는 참조 이미지의 스타일과 일치합니다.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td> 
   <td>에 대한 연결 만들기에 대한 지침: [!DNL Adobe Campaign], 참조 <a href="#create-a-connection-to-adobe-firefly" class="MCXref xref" >에 대한 연결 만들기 [!DNL Adobe Firefly]</a> 이 문서에서.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL 프롬프트]</td> 
   <td>만들려는 이미지에 대한 프롬프트를 입력하거나 매핑합니다. 프롬프트에 자세히 설명되어 있으면 이미지에 나타나는 내용을 보다 세밀하게 제어할 수 있습니다.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL 생성된 이미지 형식]</td> 
   <td>확장된 이미지를 저장할 파일 형식을 선택합니다. 기본값을 선택하면 참조 이미지가 제공되지 않으면 파일 형식이 JPEG이 됩니다. 기준 이미지가 제공된 경우, 생성된 이미지의 파일 포맷은 기준 이미지와 동일할 것이다.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL 소스 파일]</td> 
   <td>  <p>이전 모듈에서 소스 파일을 선택하거나 소스 파일의 참조 이미지 파일 이름과 참조 이미지 파일(데이터)을 매핑합니다. 생성된 이미지는 참조 이미지의 스타일과 일치하도록 만들어집니다.</p> </td> 
</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL 사전 설정]</td> 
   <td>사전 설정 스타일을 사용하려면 항목 추가 를 클릭하고 사용할 스타일을 입력하거나 매핑합니다.<p>사전 설정 스타일 목록은 다음을 참조하십시오. <a href="https://developer.adobe.com/firefly-services/docs/firefly-api/guides/concepts/styles/" >이미지 모델 스타일</a> Adobe 개발자 설명서에서 참조하십시오.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL 음성 프롬프트]</td> 
   <td>생성된 콘텐츠에서 피하려는 단어를 입력하거나 매핑합니다. </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Content 클래스]</td> 
   <td>생성된 이미지를 사진과 같은 이미지로 할지 또는 생성된 아트와 같은 이미지로 할지 선택합니다. <ul><li><b>사진</b><p>조리개, 셔터 속도(초) 및 시야(밀리미터)의 값을 입력합니다.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL 시드]</td> 
   <td>정수를 입력하거나 매핑합니다. 다른 이미지 모듈 확장에서 이와 동일한 시드를 사용하여 스타일이 다른 유사한 이미지를 생성할 수 있습니다. </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Size]</td> 
   <td>생성된 이미지를 표시할 크기를 선택합니다.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL 강도]</td> 
   <td>생성된 이미지가 사전 설정된 스타일 또는 참조 이미지의 스타일과 일치하는 강도를 나타내는 정수를 입력하거나 매핑합니다. </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL 시각적 강도]</td> 
   <td>사진의 기존 시각적 특성의 전체 강도를 나타내는 정수를 입력하거나 매핑합니다. </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Locale]</td> 
   <td>로케일이 제공되면 모듈은 지정된 로케일과 더 관련이 있는 콘텐츠를 생성합니다. <p>로케일은 ISO 639-1 언어 코드 및 ISO 3166-1 지역에서 제공해야 합니다.</p><p> 예: <code>en-US</code></p></td> 
  </tr> 
 </tbody> 
</table>


