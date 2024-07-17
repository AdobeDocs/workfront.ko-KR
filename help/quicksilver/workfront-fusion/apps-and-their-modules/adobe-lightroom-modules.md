---
content-type: reference
product-previous: workfront-fusion
product-area: workfront-integrations
keywords: 커넥터
navigation-topic: apps-and-their-modules
title: Adobe Lightroom 모듈
description: Adobe Lightroom 모듈을 사용하면 Adobe Lightroom 계정의 이벤트를 기반으로 Adobe Workfront Fusion 시나리오를 시작할 수 있습니다.
author: Becky
feature: Workfront Fusion, Digital Content and Documents
exl-id: e48bdf18-49f0-436e-9182-16c9da2b3169
source-git-commit: 0a01acd56b3ea10d1cccc31a21e434da55b1ec13
workflow-type: tm+mt
source-wordcount: '2244'
ht-degree: 0%

---

# [!DNL Adobe Lightroom]개 모듈

<!--Add Connection info-->

[!DNL Adobe Workfront Fusion] 시나리오에서는 [!DNL Adobe Lightroom]을(를) 사용하는 워크플로를 자동화하고 여러 타사 응용 프로그램 및 서비스에 연결할 수 있습니다.

시나리오를 만드는 방법에 대한 지침은 [시나리오 만들기](../../workfront-fusion/scenarios/create-a-scenario.md)를 참조하십시오.

모듈에 대한 자세한 내용은 [의 모듈 [!DNL Adobe Workfront Fusion]](../../workfront-fusion/modules/modules.md)을 참조하세요.

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
      <td >
        <p>작업 자동화 및 통합을 위한 [!UICONTROL Workfront Fusion]</p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">제품</td>
      <td>조직에서 이 문서에 설명된 기능을 사용하려면 [!DNL Adobe Workfront Fusion]과(와) [!DNL Adobe Workfront]을(를) 구입해야 합니다.</td>
    </tr>
    </tr>
  </tbody>
</table>


&#42;플랜, 라이선스 유형 또는 액세스 권한을 확인하려면 [!DNL Workfront] 관리자에게 문의하세요.

&#42;&#42;[!DNL Adobe Workfront Fusion] 라이선스에 대한 자세한 내용은 [!DNL [Adobe Workfront Fusion] licenses](../../workfront-fusion/get-started/license-automation-vs-integration.md)을(를) 참조하세요.

## 전제 조건

[!DNL Adobe Lightroom] 커넥터를 사용하려면 먼저 다음 전제 조건을 충족하는지 확인해야 합니다.

* 활성 [!DNL Adobe Lightroom] 계정이 있어야 합니다.

## Adobe Lightroom에 대한 연결 만들기



## Adobe Lightroom 모듈 및 해당 필드

[!DNL Adobe Lightroom] 모듈을 구성할 때 [!DNL Workfront Fusion]에 아래 나열된 필드가 표시됩니다. 앱 또는 서비스의 액세스 수준과 같은 요소에 따라 이러한 필드와 함께 [!DNL Adobe Lightroom] 필드가 추가로 표시될 수 있습니다. 모듈의 굵은 제목은 필수 필드를 나타냅니다.

필드나 함수 위에 맵 단추가 표시되면 이 단추를 사용하여 해당 필드에 대한 변수와 함수를 설정할 수 있습니다. 자세한 내용은 [한 모듈에서 다른 모듈로 정보를 매핑 [!DNL Adobe Workfront Fusion]](../../workfront-fusion/mapping/map-information-between-modules.md)을 참조하십시오.

![](assets/map-toggle-350x74.png)

* [기타](#other)
* [자산](#assets)
* [앨범](#albums)

### 기타

* [상태 검사](#health-check)
* [사용자 카탈로그 메타데이터 검색](#retrieve-user-catalog-metadata)

#### 상태 검사

이 작업 모듈은 Lightroom 서버 버전 ID를 검색하여 Lightroom 서비스가 현재 실행 중인지 확인합니다.

<table style="table-layout:auto"> 
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">[!UICONTROL Connection]</td>
      <td>[!DNL Adobe Lightroom]에 대한 연결을 만드는 방법에 대한 지침은 이 문서에서 <a href="#create-a-connection-to-adobe-lightroom" class="MCXref xref" >[!DNL Adobe Lightroom]</a>에 대한 연결 만들기 를 참조하십시오.</td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL 자격 증명]</td>
      <td>
        <p>특정 서버가 실행 중인지 확인하기 위해 특정 인증서를 제공하려면 항목 추가를 누르고 인증서를 입력합니다.</p><p>인증 헤더가 자동으로 추가됩니다.</p>
      </td>
    </tr>
  </tbody>
</table>

#### 사용자 카탈로그 메타데이터 검색

<table style="table-layout:auto"> 
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">[!UICONTROL Connection]</td>
      <td>[!DNL Adobe Lightroom]에 대한 연결을 만드는 방법에 대한 지침은 이 문서에서 <a href="#create-a-connection-to-adobe-lightroom" class="MCXref xref" >[!DNL Adobe Lightroom]</a>에 대한 연결 만들기 를 참조하십시오.</td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL 자격 증명]</td>
      <td>
        <p>올바른 사용자 계정에 액세스할 수 있도록 특정 자격 증명을 제공하려면 항목 추가를 누르고 자격 증명을 입력합니다.</p><p>인증 헤더가 자동으로 추가됩니다.</p>
      </td>
    </tr>
  </tbody>
</table>

### 자산

* [에셋 원본 파일 만들기](#create-an-asset-external-xmp-develop-setting-file)
* [에셋 만들기](#create-an-asset)
* [외부 XMP 개발 설정 파일 에셋 만들기](#create-an-asset-external-xmp-develop-setting-file)
* [원본 파일에 대한 렌디션 생성](#generate-renditions-for-an-original-file)
* [카탈로그 자산 가져오기](#get-a-catalog-asset)
* [최신 자산 외부 XMP 개발 설정 받기](#get-the-latest-asset-external-xmp-develop-setting-file)
* [최신 자산 렌디션 가져오기](#get-the-latest-asset-rendition)
* [에셋 검색](#retrieve-assets)

#### 에셋 원본 파일 만들기

이 작업 모듈은 자산에 대한 원본 파일을 만들고 업로드합니다.


<table style="table-layout:auto"> 
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">[!UICONTROL Connection]</td>
      <td>[!DNL Adobe Lightroom]에 대한 연결을 만드는 방법에 대한 지침은 이 문서에서 <a href="#create-a-connection-to-adobe-lightroom" class="MCXref xref" >[!DNL Adobe Lightroom]</a>에 대한 연결 만들기 를 참조하십시오.</td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL 카탈로그 ID]</td>
      <td>
        <p>자산이 포함된 카탈로그의 ID를 입력하거나 매핑합니다.</p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL 자산 ID]</td>
      <td>
        <p>파일을 만들고 업로드할 자산의 ID를 입력하거나 매핑합니다.</p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL 콘텐츠의 길이(바이트)]</td>
      <td>
        <p>콘텐츠의 길이를 바이트 단위로 입력하거나 매핑합니다.</p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL 바이트 범위]</td>
      <td>
        <p>RFC 2616에서 정의한 첫 번째 바이트와 마지막 바이트 및 엔티티 길이를 포함하여 요청에 대한 바이트 범위를 입력하거나 매핑합니다. 데이터가 너무 커서 한 번의 호출로 업로드할 수 없는 경우에만 포함해야 합니다.</p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL 컨텐츠 유형]</td>
      <td>
        <p>새 파일의 컨텐츠 유형을 선택합니다.</p>
      </td>
    </tr>
  </tbody>
</table>

#### 에셋 만들기

이 작업 모듈은 초기 메타데이터 및 가져오기 정보를 사용하여 새 에셋을 만듭니다.


<table style="table-layout:auto"> 
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">[!UICONTROL Connection]</td>
      <td>[!DNL Adobe Lightroom]에 대한 연결을 만드는 방법에 대한 지침은 이 문서에서 <a href="#create-a-connection-to-adobe-lightroom" class="MCXref xref" >[!DNL Adobe Lightroom]</a>에 대한 연결 만들기 를 참조하십시오.</td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL 카탈로그 ID]</td>
      <td>
        <p>자산을 만들 카탈로그의 ID를 입력하거나 매핑합니다.</p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL 자산 ID]</td>
      <td>
        <p>새 에셋의 ID를 입력하거나 매핑합니다.</p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL 자산 유형]</td>
      <td>
        <p>자산이 이미지인지 비디오인지를 선택합니다.</p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL 날짜/시간 사용자 생성됨]</td>
      <td>
        <p><code>YYYY-MM-DDT00:00:00-00:00</code> 형식으로 날짜를 입력하거나 매핑합니다.</p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL 날짜/시간 사용자 업데이트됨]</td>
      <td>
        <p><code>YYYY-MM-DDT00:00:00-00:00</code> 형식으로 날짜를 입력하거나 매핑합니다.</p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL 날짜 캡처됨]</td>
      <td>
        <p><code>YYYY-MM-DDT00:00:00-00:00</code> 형식으로 날짜를 입력하거나 매핑합니다.</p>
      </td>
    </tr>
  </tbody>
</table>

#### 외부 XMP 개발 설정 파일 에셋 만들기

이 작업 모듈은 두 가지 워크플로우를 지원합니다. 첫 번째 워크플로우는 자산에 대한 외부 XMP 개발 설정 파일을 업로드하는 것입니다. 두 번째 워크플로우는 다른 자산의 외부 xmp 개발 설정 파일에서 복사하여 외부 XMP 개발 설정 파일을 만드는 것입니다.

<table style="table-layout:auto"> 
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">[!UICONTROL Connection]</td>
      <td>[!DNL Adobe Lightroom]에 대한 연결을 만드는 방법에 대한 지침은 이 문서에서 <a href="#create-a-connection-to-adobe-lightroom" class="MCXref xref" >[!DNL Adobe Lightroom]</a>에 대한 연결 만들기 를 참조하십시오.</td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL 콘텐츠의 길이(바이트)]</td>
      <td>
        <p>콘텐츠의 길이를 바이트 단위로 입력하거나 매핑합니다.</p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL 새 파일을 업로드하거나 XMP/개발 파일을 복사합니다.]</td>
      <td>
        <p>새 파일을 업로드할지 또는 기존 에셋에서 파일을 복사할지 여부를 선택합니다.</p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL 카탈로그 ID]</td>
      <td>
        <p>자산이 포함된 카탈로그의 ID를 입력하거나 매핑합니다.</p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL 자산 ID]</td>
      <td>
        <p>파일을 업로드하거나 복사할 에셋의 ID를 입력하거나 매핑합니다.</p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">XMP/develop 파일에 대한 [!UICONTROL 링크]</td>
      <td>
        <p>업로드하거나 복사할 파일에 대한 링크를 입력하거나 매핑합니다.</p><p>이 파일은 파일을 복사하는 경우 JSON이어야 하고, 파일을 업로드하는 경우 XML이어야 합니다.</p>
      </td>
    </tr>
  </tbody>
</table>

#### 원본 파일에 대한 렌디션 생성

이 작업 모듈은 원본 파일에 대한 렌디션을 비동기적으로 생성합니다.

<table style="table-layout:auto"> 
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">[!UICONTROL Connection]</td>
      <td>[!DNL Adobe Lightroom]에 대한 연결을 만드는 방법에 대한 지침은 이 문서에서 <a href="#create-a-connection-to-adobe-lightroom" class="MCXref xref" >[!DNL Adobe Lightroom]</a>에 대한 연결 만들기 를 참조하십시오.</td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL 렌디션 유형(세미콜론으로 구분)]</td>
      <td>
        <p>만들려는 표현물의 표현물 유형을 입력합니다. 두 개 이상의 문자를 입력할 경우 세미콜론(;)으로 구분하십시오. <p>가능한 유형:</p><ul><li><code>fullsize</code></li><li><code>2560</code></li></ul></p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL 콘텐츠의 길이(바이트)]</td>
      <td>
        <p>콘텐츠의 길이를 바이트 단위로 입력하거나 매핑합니다.</p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL 카탈로그 ID]</td>
      <td>
        <p>자산이 포함된 카탈로그의 ID를 입력하거나 매핑합니다.</p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL 자산 ID]</td>
      <td>
        <p>파일의 렌디션을 만들려는 에셋의 ID를 입력하거나 매핑합니다.</p>
      </td>
    </tr>
  </tbody>
</table>

#### 카탈로그 자산 가져오기

이 작업 모듈은 카탈로그의 단일 에셋에 대한 정보를 검색합니다. 카탈로그는 이 모듈에 사용된 연결에 자격 증명이 표시된 사용자가 소유해야 합니다.

<table style="table-layout:auto"> 
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">[!UICONTROL Connection]</td>
      <td>[!DNL Adobe Lightroom]에 대한 연결을 만드는 방법에 대한 지침은 이 문서에서 <a href="#create-a-connection-to-adobe-lightroom" class="MCXref xref" >[!DNL Adobe Lightroom]</a>에 대한 연결 만들기 를 참조하십시오.</td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL 카탈로그 ID]</td>
      <td>
        <p>자산이 포함된 카탈로그의 ID를 입력하거나 매핑합니다.</p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL 자산 ID]</td>
      <td>
        <p>정보를 검색할 에셋의 ID를 입력하거나 매핑합니다.</p>
      </td>
    </tr>
  </tbody>
</table>


#### 최신 자산 외부 XMP 개발 설정 파일 가져오기

이 작업 모듈은 가장 최근의 자산 외부 XMP 설정 파일을 검색합니다.

<table style="table-layout:auto"> 
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">[!UICONTROL Connection]</td>
      <td>[!DNL Adobe Lightroom]에 대한 연결을 만드는 방법에 대한 지침은 이 문서에서 <a href="#create-a-connection-to-adobe-lightroom" class="MCXref xref" >[!DNL Adobe Lightroom]</a>에 대한 연결 만들기 를 참조하십시오.</td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL 카탈로그 ID]</td>
      <td>
        <p>자산이 포함된 카탈로그의 ID를 입력하거나 매핑합니다.</p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL 자산 ID]</td>
      <td>
        <p>XMP 개발 설정 파일과 연결된 에셋의 ID를 입력하거나 매핑합니다.</p>
      </td>
    </tr>
  </tbody>
</table>

#### 최신 자산 렌디션 가져오기

이 작업 모듈은 지정된 유형의 최신 자산 렌디션을 검색합니다.

<table style="table-layout:auto"> 
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">[!UICONTROL Connection]</td>
      <td>[!DNL Adobe Lightroom]에 대한 연결을 만드는 방법에 대한 지침은 이 문서에서 <a href="#create-a-connection-to-adobe-lightroom" class="MCXref xref" >[!DNL Adobe Lightroom]</a>에 대한 연결 만들기 를 참조하십시오.</td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL 카탈로그 ID]</td>
      <td>
        <p>자산이 포함된 카탈로그의 ID를 입력하거나 매핑합니다.</p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL 자산 ID]</td>
      <td>
        <p>XMP 개발 설정 파일과 연결된 에셋의 ID를 입력하거나 매핑합니다.</p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL 렌디션 유형]</td>
      <td>
        <p>검색할 렌디션 유형을 선택합니다.</p>
      </td>
    </tr>
  </tbody>
</table>

#### 에셋 검색

이 작업 모듈은 이 모듈에 사용된 연결에 자격 증명이 표시된 사용자가 소유한 자산을 검색합니다.

<table style="table-layout:auto"> 
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">[!UICONTROL Connection]</td>
      <td>[!DNL Adobe Lightroom]에 대한 연결을 만드는 방법에 대한 지침은 이 문서에서 <a href="#create-a-connection-to-adobe-lightroom" class="MCXref xref" >[!DNL Adobe Lightroom]</a>에 대한 연결 만들기 를 참조하십시오.</td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL 카탈로그 ID]</td>
      <td>
        <p>자산이 포함된 카탈로그의 ID를 입력하거나 매핑합니다.</p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL 시작 타임스탬프]</td>
      <td>
        <p>타임스탬프를 입력하거나 매핑합니다. 모듈은 이 타임스탬프 후에 업데이트된 레코드를 반환합니다.</p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL 전에 캡처된 자산 반환]</td>
      <td>
        <p><code>YYYY-MM-DDT00:00:00</code> 형식의 날짜를 입력하십시오. 모듈은 이 날짜 이전에 캡처된 결과를 반환합니다.</p><p> 이 필드는 필드 <code>Return assets captured after</code>과(와) 함께 사용할 수 없습니다.</p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL 반환되는 최대 자산 수]</td>
      <td>
        <p>한 실행 주기 동안 [!DNL Workfront Fusion]이(가) 반환할 최대 자산 수를 설정하십시오. 이 숫자는 100보다 작거나 같아야 합니다.</p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL SHA256 원본 파일의 해시 값]</td>
      <td>
        <p></p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL 스택 내에 있는 자산을 숨기시겠습니까?"]</td>
      <td>
        <p></p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL 자산 하위 유형 값]</td>
      <td>
        <p></p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL 자산 ID]</td>
      <td>
        <p>쉼표로 구분하여 최대 100개의 자산 ID를 입력하거나 매핑합니다.</p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL 제외할 자산 유형]</td>
      <td>
        <p>전체 또는 미완료 에셋을 제외하려면 을 선택합니다. 모든 에셋을 포함하려면 이 필드를 비워 둡니다.</p>
      </td>
    <tr>
      <td role="rowheader">[!UICONTROL 그룹 값]</td>
      <td>
        <p></p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL 이름 값]</td>
      <td>
        <p></p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL 즐겨찾기 상태]</td>
      <td>
        <p></p>
      </td>
    </tr>
    </tr>
  </tbody>
</table>

### 앨범

* [앨범에 에셋 추가](#add-assets-to-an-album)
* [앨범 만들기](#create-an-album)
* [앨범 삭제](#delete-an-album)
* [앨범 받기](#get-an-album)
* [앨범의 에셋 나열](#list-assets-of-an-album)
* [앨범 검색](#retrieve-albums)
* [앨범 업데이트](#update-album)

#### 앨범에 에셋 추가

이 작업 모듈은 지정된 앨범에 하나 이상의 에셋을 추가합니다. 하나의 실행 주기에서 최대 50개의 자산을 추가할 수 있습니다.

<table style="table-layout:auto"> 
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">[!UICONTROL Connection]</td>
      <td>[!DNL Adobe Lightroom]에 대한 연결을 만드는 방법에 대한 지침은 이 문서에서 <a href="#create-a-connection-to-adobe-lightroom" class="MCXref xref" >[!DNL Adobe Lightroom]</a>에 대한 연결 만들기 를 참조하십시오.</td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL 카탈로그 ID]</td>
      <td>
        <p>자산을 추가할 앨범이 포함된 카탈로그의 ID를 입력하거나 매핑합니다.</p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL 앨범 ID]</td>
      <td>
        <p>에셋을 추가할 앨범의 ID를 입력하거나 매핑합니다.</p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Assets]</td>
      <td>
        <p>앨범에 추가할 각 에셋에 대해 <b>항목 추가</b>를 클릭하고 다음 필드를 입력하십시오.</p>
      </td>
    <tr>
      <td role="rowheader">[!UICONTROL 자산 ID]</td>
      <td>
        <p>앨범에 추가할 자산의 ID를 입력하거나 매핑합니다.</p>
      </td>
    <tr>
      <td role="rowheader">[!UICONTROL 이 자산은 앨범 커버입니까?]</td>
      <td>
        <p>이 자산을 앨범을 나타내는 이미지로 표시할지 여부를 선택합니다.</p>
      </td>
    <tr>
      <td role="rowheader">[!UICONTROL Order]</td>
      <td>
        <p></p>
      </td>
    <tr>
      <td role="rowheader">[!UICONTROL 메타데이터]</td>
      <td>
        <p>에셋에 포함할 메타데이터를 입력하거나 매핑합니다. 최대 길이가 1-24자인 단일 텍스트 문자열이어야 합니다.</p>
      </td>
    <tr>
      <td role="rowheader">[!UICONTROL Remote ID]</td>
      <td>
        <p>에셋의 식별자를 입력합니다.</p>
      </td>
    </tr>
  </tbody>
</table>

#### 앨범 만들기

이 작업 모듈은 Lightroom에서 새 앨범을 만듭니다.

<table style="table-layout:auto"> 
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">[!UICONTROL Connection]</td>
      <td>[!DNL Adobe Lightroom]에 대한 연결을 만드는 방법에 대한 지침은 이 문서에서 <a href="#create-a-connection-to-adobe-lightroom" class="MCXref xref" >[!DNL Adobe Lightroom]</a>에 대한 연결 만들기 를 참조하십시오.</td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL 카탈로그 ID]</td>
      <td>
        <p>앨범을 만들 카탈로그의 ID를 입력하거나 매핑합니다.</p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL 앨범 ID]</td>
      <td>
        <p>새 앨범의 ID를 입력하거나 매핑합니다.</p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL 하위 유형]</td>
      <td>
        <p>앨범의 하위 유형을 선택합니다.</p>
      </td>
    <tr>
      <td role="rowheader">[!UICONTROL API 키]</td>
      <td>
        <p>앨범을 만드는 서비스의 API 키를 입력합니다.</p>
      </td>
    <tr>
      <td role="rowheader">[!UICONTROL 날짜/시간 사용자 생성됨]</td>
      <td>
        <p><code>YYYY-MM-DDT00:00:00-00:00Z</code> 형식으로 날짜를 입력하거나 매핑합니다.</p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL 날짜/시간 사용자 업데이트됨]</td>
      <td>
        <p><code>YYYY-MM-DDT00:00:00-00:00Z</code> 형식으로 날짜를 입력하거나 매핑합니다.</p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Album name]</td>
      <td>
        <p>새 앨범의 이름을 입력하거나 매핑합니다.</p>
      </td>
    <tr>
      <td role="rowheader">[!UICONTROL 표지 ID]</td>
      <td>
        <p>이 앨범의 표지로 사용할 자산의 ID를 입력하거나 매핑합니다.</p>
      </td>
    <tr>
      <td role="rowheader">[!UICONTROL Remote ID]</td>
      <td>
        <p>에셋의 식별자를 입력합니다.</p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL 만든 날짜]</td>
      <td>
        <p><code>YYYY-MM-DDT00:00:00-00:00Z</code> 형식으로 날짜를 입력하거나 매핑합니다.</p>
      </td>
    <tr>
      <td role="rowheader">[!UICONTROL 업데이트된 날짜]</td>
      <td>
        <p><code>YYYY-MM-DDT00:00:00-00:00Z</code> 형식으로 날짜를 입력하거나 매핑합니다.</p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL 앨범이 삭제되었습니까?]</td>
      <td>
        <p>외부 제휴 콘텐츠가 삭제된 경우 이 옵션을 활성화합니다.</p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">제휴 콘텐츠를 편집할 위치의 [!UICONTROL URL]</td>
      <td>
        <p>사용자가 이 앨범의 콘텐츠를 편집할 수 있는 URL이 있는 경우 여기에 URL을 입력하십시오.</p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">제휴 콘텐츠를 볼 위치의 [!UICONTROL URL]</td>
      <td>
        <p>사용자가 이 앨범의 콘텐츠를 볼 수 있는 URL이 있는 경우 여기에 URL을 입력하십시오.</p>
      </td>
    </tr>
  </tbody>
</table>

#### 앨범 삭제

이 작업 모듈은 앨범을 삭제합니다.

삭제된 앨범은 현재 삭제 중인 것과 동일한 클라이언트 앱에 의해 만들어졌어야 하며 하위 유형 `project` 또는 `project_set`이어야 합니다.

<table style="table-layout:auto"> 
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">[!UICONTROL Connection]</td>
      <td>[!DNL Adobe Lightroom]에 대한 연결을 만드는 방법에 대한 지침은 이 문서에서 <a href="#create-a-connection-to-adobe-lightroom" class="MCXref xref" >[!DNL Adobe Lightroom]</a>에 대한 연결 만들기 를 참조하십시오.</td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL 카탈로그 ID]</td>
      <td>
        <p>삭제할 앨범이 포함된 카탈로그의 ID를 입력하거나 매핑합니다.</p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL 앨범 ID]</td>
      <td>
        <p>삭제할 앨범의 ID를 입력하거나 매핑합니다.</p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL 하위 앨범을 삭제하시겠습니까?]</td>
      <td>
        <p>삭제된 앨범의 하위 앨범을 삭제할지 여부를 선택합니다.</p>
      </td>
    </tr>
  </tbody>
</table>

### 앨범 받기

이 작업 모듈은 지정된 앨범을 검색합니다.

<table style="table-layout:auto"> 
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">[!UICONTROL Connection]</td>
      <td>[!DNL Adobe Lightroom]에 대한 연결을 만드는 방법에 대한 지침은 이 문서에서 <a href="#create-a-connection-to-adobe-lightroom" class="MCXref xref" >[!DNL Adobe Lightroom]</a>에 대한 연결 만들기 를 참조하십시오.</td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL 카탈로그 ID]</td>
      <td>
        <p>검색할 앨범이 포함된 카탈로그의 ID를 입력하거나 매핑합니다.</p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL 앨범 ID]</td>
      <td>
        <p>검색할 앨범의 ID를 입력하거나 매핑합니다.</p>
      </td>
    </tr>
  </tbody>
</table>

#### 앨범의 에셋 나열

이 작업 모듈은 지정된 앨범의 자산 목록을 검색합니다.



#### 앨범 검색

이 작업 모듈은 지정된 카탈로그의 앨범 목록을 검색합니다.

<table style="table-layout:auto"> 
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">[!UICONTROL Connection]</td>
      <td>[!DNL Adobe Lightroom]에 대한 연결을 만드는 방법에 대한 지침은 이 문서에서 <a href="#create-a-connection-to-adobe-lightroom" class="MCXref xref" >[!DNL Adobe Lightroom]</a>에 대한 연결 만들기 를 참조하십시오.</td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL 카탈로그 ID]</td>
      <td>
        <p>검색할 앨범이 포함된 카탈로그의 ID를 입력하거나 매핑합니다.</p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL 하위 유형]</td>
      <td>
        <p>검색할 앨범의 ID를 입력하거나 매핑합니다.</p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL 현재 결과 앞에 오는 앨범의 이름]</td>
      <td>
        <p>결과에 페이지를 매기려면 이전 페이지에서 마지막 앨범의 이름을 입력하거나 매핑하십시오.</p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL 반환되는 최대 앨범 수]</td>
      <td>
        <p>한 실행 주기 동안 [!DNL Workfront Fusion]이(가) 반환할 최대 자산 수를 설정하십시오. 이 필드의 기본값은 100입니다. 제한 경계의 여러 앨범에 동일한 <code>name_after</code> 값이 있는 경우 이 모듈은 이 제한보다 더 많은 앨범을 반환할 수 있습니다.</p>
      </td>
    </tr>
  </tbody>
</table>

#### 앨범 업데이트

이 작업 모듈은 지정된 앨범을 업데이트합니다.

업데이트된 앨범은 현재 업데이트 중인 것과 동일한 클라이언트 앱에서 만들었어야 하며 하위 유형 `project` 또는 `project_set`이어야 합니다.

<table style="table-layout:auto"> 
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">[!UICONTROL Connection]</td>
      <td>[!DNL Adobe Lightroom]에 대한 연결을 만드는 방법에 대한 지침은 이 문서에서 <a href="#create-a-connection-to-adobe-lightroom" class="MCXref xref" >[!DNL Adobe Lightroom]</a>에 대한 연결 만들기 를 참조하십시오.</td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL 카탈로그 ID]</td>
      <td>
        <p>업데이트할 앨범이 포함된 카탈로그의 ID를 입력하거나 매핑합니다.</p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL 앨범 ID]</td>
      <td>
        <p>업데이트할 앨범의 ID를 입력하거나 매핑합니다.</p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">기타 필드</td>
      <td>
      <td>이 모듈의 다른 필드에 대한 설명은 이 문서의 <a href="#create-an-album" class="MCXref xref" >앨범 만들기</a>를 참조하십시오.</td>
      </td>
    </tr>
  </tbody>
</table>
