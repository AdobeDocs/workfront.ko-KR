---
content-type: reference
product-previous: workfront-fusion
product-area: workfront-integrations
keywords: 커넥터
navigation-topic: apps-and-their-modules
title: Adobe Photoshop 모듈
description: Adobe Photoshop 모듈을 사용하면 Adobe Photoshop 계정의 이벤트를 기반으로 Adobe Workfront Fusion 시나리오를 시작하고, 계약 및 기타 레코드를 생성, 읽기 또는 업데이트하고, 설정한 기준을 사용하여 레코드를 검색하고, 문서를 업로드할 수 있습니다.
author: Becky
feature: Workfront Fusion, Digital Content and Documents
exl-id: f20192ea-e363-4fba-8bd2-b1d50443918d
source-git-commit: 6bcf404432129a812b5e4d840b59e72f036ec723
workflow-type: tm+mt
source-wordcount: '1547'
ht-degree: 0%

---

# [!DNL Adobe Photoshop]개 모듈

[!DNL Adobe Workfront Fusion] 시나리오에서는 [!DNL Adobe Photoshop]을(를) 사용하는 워크플로를 자동화하고 여러 타사 응용 프로그램 및 서비스에 연결할 수 있습니다.


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

[!DNL Adobe Photoshop] 커넥터를 사용하려면 먼저 다음 전제 조건을 충족하는지 확인해야 합니다.

* 활성 [!DNL Adobe Photoshop] 계정이 있어야 합니다.

## [!DNL Adobe Photoshop]에 연결 만들기

[!DNL Adobe Photoshop] 모듈에 대한 연결을 만들려면:

1. 연결 상자 옆에 있는 **[!UICONTROL 추가]**&#x200B;를 클릭합니다.

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
        <td role="rowheader">[!UICONTROL 클라이언트 ID]</td>
        <td>[!UICONTROL Adobe] [!UICONTROL 클라이언트 ID]를 입력합니다. 이 로그는 의 [!UICONTROL 자격 증명] 세부 정보 섹션에서 찾을 수 있습니다. [!DNL Adobe Developer Console]</td>
        </tr>
        <tr>
        <td role="rowheader">[!UICONTROL 클라이언트 암호]</td>
        <td>[!DNL Adobe] [!UICONTROL 클라이언트 암호]를 입력하십시오. 이 로그는 의 [!UICONTROL 자격 증명] 세부 정보 섹션에서 찾을 수 있습니다. [!DNL Adobe Developer Console]</td>
        </tr>
        <tr>
        <td role="rowheader">[!UICONTROL 기술 계정 ID]</td>
        <td>[!DNL Adobe] [!UICONTROL 기술 계정 ID]를 입력하십시오. 이 로그는 의 [!UICONTROL 자격 증명] 세부 정보 섹션에서 찾을 수 있습니다. [!DNL Adobe Developer Console]</td>
        </tr>
        <tr>
        <td role="rowheader">[!UICONTROL 조직 ID]</td>
        <td>[!DNL Adobe] [!UICONTROL 조직 ID]를 입력하십시오. 이 로그는 의 [!UICONTROL 자격 증명] 세부 정보 섹션에서 찾을 수 있습니다. [!DNL Adobe Developer Console]</td>
        </tr>
        <tr>
        <td role="rowheader">[!UICONTROL 개인 키]</td>
        <td>
          <p>[!DNL Adobe Developer Console]에서 자격 증명을 만들 때 생성된 개인 키를 입력하십시오. </p>
          <p>개인 키 또는 인증서를 추출하려면 다음을 수행하십시오.</p>
          <ol>
            <li value="1">
              <p><b>[!UICONTROL Extract]</b>을(를) 클릭합니다.</p>
            </li>
            <li value="2">
              <p>추출 중인 파일 유형을 선택합니다.</p>
            </li>
            <li value="3">
              <p>개인 키 또는 인증서가 포함된 파일을 선택합니다.</p>
            </li>
            <li value="4">
              <p>파일의 암호를 입력합니다.</p>
            </li>
            <li value="5">
              <p><b>저장</b>을 클릭하여 파일을 추출하고 [!UICONTROL ]e 연결 설정으로 돌아갑니다.</p>
            </li>
          </ol>
        </td>
        </tr>
      </tbody>
    </table>

1. 연결을 저장하고 모듈로 돌아가려면 **[!UICONTROL 계속]**&#x200B;을 클릭하세요.

## [!DNL Adobe Photoshop]개 모듈 및 해당 필드

[!DNL Adobe Photoshop] 모듈을 구성할 때 [!DNL Workfront Fusion]에 아래 나열된 필드가 표시됩니다. 앱 또는 서비스의 액세스 수준과 같은 요소에 따라 이러한 필드와 함께 [!DNL Adobe Photoshop] 필드가 추가로 표시될 수 있습니다. 모듈의 굵은 제목은 필수 필드를 나타냅니다.

필드나 함수 위에 맵 단추가 표시되면 이 단추를 사용하여 해당 필드에 대한 변수와 함수를 설정할 수 있습니다. 자세한 내용은 [한 모듈에서 다른 모듈로 정보를 매핑 [!DNL Adobe Workfront Fusion]](../../workfront-fusion/mapping/map-information-between-modules.md)을 참조하십시오.

![](assets/map-toggle-350x74.png)


### 액션

* [새 PSD 만들기](#create-a-new-psd)
* [텍스트 레이어 편집](#edit-text-layers)
* [깊이 흐림 효과 실행](#execute-depth-blur)
* [Photoshop 작업 실행](#execute-photoshop-actions)
* [제품 자르기 실행](#execute-product-crop)
* [레이어 정보 가져오기](#get-layer-info)
* [사용자 지정 API 호출 만들기](#make-a-custom-api-call)

#### 새 PSD 만들기

이 작업 모듈은 선택 가능한 레이어로 새 PSD을 만들고 렌디션을 생성하거나 PSD으로 저장합니다.

이 모듈과 관련된 필드는 Adobe Photoshop 설명서에서 [새 PSD 만들기](https://developer.adobe.com/photoshop/photoshop-api-docs/api/#tag/Photoshop/operation/documentCreate)를 참조하십시오.

#### 텍스트 레이어 편집

이 작업 모듈은 Photoshop 파일의 텍스트 레이어를 편집합니다.

<table style="table-layout:auto"> 
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">[!UICONTROL Connection]</td>
      <td>[!DNL Adobe Photoshop]에 대한 연결을 만드는 방법에 대한 지침은 이 문서에서 <a href="#create-a-connection-to-adobe-photoshop" class="MCXref xref" >[!DNL Adobe Photoshop]</a>에 대한 연결 만들기 를 참조하십시오.</td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL 입력 파일 저장소]</td>
      <td>
        <p>편집할 파일이 저장된 파일 서비스를 선택합니다.</p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">
        <p>[!UICONTROL 입력 파일 URL]</p>
      </td>
   <td> 편집할 파일의 URL 또는 경로를 입력하거나 매핑합니다. </td> 
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL 누락된 글꼴 관리]</td>
      <td>
        <p>문서에 누락된 글꼴이 하나 이상 있는 경우 수행할 작업을 선택합니다. 글꼴이 제공되지 않으면 모듈은 기본 글꼴을 사용합니다.</p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Default font]  </td>
      <td>
        <p>문서의 전역 기본값으로 사용할 글꼴의 전체 포스트스크립트 이름을 입력합니다. 이 글꼴은 글꼴이 누락되고 해당 레이어에 대해 특별히 제공된 다른 글꼴이 없는 텍스트 레이어에 사용됩니다. 이 글꼴이 누락된 경우 누락된 글꼴 관리에 지정된 옵션이 적용됩니다.</p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL 레이어]</td>
   <td> <p>레이어 옵션에 대한 자세한 내용은 Adobe Photoshop 설명서에서 <a href="https://developer.adobe.com/photoshop/photoshop-api-docs/api/#tag/Photoshop/operation/text">텍스트 레이어 편집</a>을 참조하십시오.</p>  </td>     </tr>
    <tr>
      <td role="rowheader">[!UICONTROL 출력 파일 저장소]</td>
      <td>
        <p>편집한 파일을 저장할 파일 서비스를 선택합니다.</p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">
        <p>[!UICONTROL 출력 파일 URL]</p>
      </td>
   <td> 편집된 파일이 저장되는 위치의 URL 또는 경로를 입력하거나 매핑합니다. </td> 
    </tr>
    <tr>
      <td role="rowheader">
        <p>[!UICONTROL 출력 파일 유형]</p>
      </td>
   <td> 편집한 파일의 파일 유형을 선택합니다. </td> 
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL 덮어쓰기]</td>
      <td>
        <p>새로 편집한 파일이 이미 있는 출력 파일을 덮어쓸지 여부를 선택합니다.</p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">
        <p>[!UICONTROL Compression]</p>
      </td>
   <td> 출력 파일의 압축 레벨을 선택합니다. </td> 
    </tr>
  </tbody>
</table>

#### 깊이 흐림 효과 실행

이 작업 모듈은 선택한 파일에 대해 깊이 흐림 효과를 실행합니다.

<table style="table-layout:auto"> 
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">[!UICONTROL Connection]</td>
      <td>[!DNL Adobe Photoshop]에 대한 연결을 만드는 방법에 대한 지침은 이 문서에서 <a href="#create-a-connection-to-adobe-photoshop" class="MCXref xref" >[!DNL Adobe Photoshop]</a>에 대한 연결 만들기 를 참조하십시오.</td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL 입력 파일 저장소]</td>
      <td>
        <p>편집할 파일이 저장된 파일 서비스를 선택합니다.</p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">
        <p>[!UICONTROL 입력 파일 URL]</p>
      </td>
   <td> 편집할 파일의 URL 또는 경로를 입력하거나 매핑합니다. </td> 
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL 출력 파일 저장소]</td>
      <td>
        <p>편집한 파일을 저장할 파일 서비스를 선택합니다.</p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">
        <p>[!UICONTROL 출력 파일 URL]</p>
      </td>
   <td> 편집된 파일이 저장되는 위치의 URL 또는 경로를 입력하거나 매핑합니다. </td> 
    </tr>
    <tr>
      <td role="rowheader">
        <p>[!UICONTROL 출력 파일 유형]</p>
      </td>
   <td> 편집한 파일의 파일 유형을 선택합니다. </td> 
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL 기타 필드]</td>
      <td>
        <p>다른 깊이 흐림 효과 옵션에 대한 자세한 내용은 Adobe Photoshop API 설명서의 <a href="https://developer.adobe.com/photoshop/photoshop-api-docs/api/#tag/Photoshop/operation/depthBlur">깊이 흐림 효과 실행 </a>을(를) 참조하십시오.</p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL 덮어쓰기]</td>
      <td>
        <p>새로 편집한 파일이 이미 있는 출력 파일을 덮어쓸지 여부를 선택합니다.</p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">
        <p>[!UICONTROL Compression]</p>
      </td>
   <td> 출력 파일의 압축 레벨을 선택합니다. </td> 
    </tr>
  </tbody>
</table>

#### Photoshop 작업 실행

이 작업 모듈은 선택한 이미지에 대해 Photoshop 작업을 실행합니다.

<table style="table-layout:auto"> 
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">[!UICONTROL Connection]</td>
      <td>[!DNL Adobe Photoshop]에 대한 연결을 만드는 방법에 대한 지침은 이 문서에서 <a href="#create-a-connection-to-adobe-photoshop" class="MCXref xref" >[!DNL Adobe Photoshop]</a>에 대한 연결 만들기 를 참조하십시오.</td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL 입력 파일 저장소]</td>
      <td>
        <p>편집할 파일이 저장된 파일 서비스를 선택합니다.</p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">
        <p>[!UICONTROL 입력 파일 URL]</p>
      </td>
   <td> 편집할 파일의 URL 또는 경로를 입력하거나 매핑합니다. </td> 
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Actions 파일 저장소]</td>
      <td>
        <p>작업 파일이 저장된 파일 서비스를 선택합니다.</p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">
        <p>[!UICONTROL 작업 파일 URL]</p>
      </td>
   <td> 작업 파일의 URL 또는 경로를 입력하거나 매핑합니다. </td> 
    </tr>
     <tr>
      <td role="rowheader">
        <p>[!UICONTROL Action name]</p>
      </td>
   <td> 특정 작업만 실행하려는 경우 ActionSet에서 재생할 작업을 지정할 수 있습니다. </td> 
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL 글꼴 / 패턴 / 브러시 저장소]</td>
      <td>
        <p>사용할 파일이 저장된 파일 서비스를 선택합니다.</p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">
        <p>[!UICONTROL Font / Pattern / Brush file URL]</p>
      </td>
   <td> 사용할 파일의 URL 또는 경로를 입력하거나 매핑합니다. </td> 
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL 출력 파일 저장소]</td>
      <td>
        <p>편집한 파일을 저장할 파일 서비스를 선택합니다.</p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">
        <p>[!UICONTROL 출력 파일 URL]</p>
      </td>
   <td> 편집된 파일이 저장되는 위치의 URL 또는 경로를 입력하거나 매핑합니다. </td> 
    </tr>
    <tr>
      <td role="rowheader">
        <p>[!UICONTROL 출력 파일 유형]</p>
      </td>
   <td> 편집한 파일의 파일 유형을 선택합니다. </td> 
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL 덮어쓰기]</td>
      <td>
        <p>새로 편집한 파일이 이미 있는 출력 파일을 덮어쓸지 여부를 선택합니다.</p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">
        <p>[!UICONTROL Compression]</p>
      </td>
   <td> 출력 파일의 압축 레벨을 선택합니다. </td> 
    </tr>
  </tbody>
</table>

#### 제품 자르기 실행

이 작업 모듈은 선택한 이미지에 대해 제품 자르기를 실행합니다.

<table style="table-layout:auto"> 
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">[!UICONTROL Connection]</td>
      <td>[!DNL Adobe Photoshop]에 대한 연결을 만드는 방법에 대한 지침은 이 문서에서 <a href="#create-a-connection-to-adobe-photoshop" class="MCXref xref" >[!DNL Adobe Photoshop]</a>에 대한 연결 만들기 를 참조하십시오.</td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL 입력 파일 저장소]</td>
      <td>
        <p>자를 파일이 저장된 파일 서비스를 선택합니다.</p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">
        <p>[!UICONTROL 입력 파일 URL]</p>
      </td>
   <td> 자를 파일의 URL 또는 경로를 입력하거나 매핑합니다. </td> 
    </tr>
    <tr>
      <td role="rowheader">
        <p>[!UICONTROL Unit]</p>
      </td>
   <td> 높이 및 너비 조정을 픽셀 단위로 설명할지 아니면 백분율로 설명할지 선택합니다. </td> 
    </tr>
    <tr>
      <td role="rowheader">
        <p>[!UICONTROL 너비]</p>
      </td>
   <td> 추가할 너비 패딩의 양을 입력하거나 매핑합니다. </td> 
    </tr>
    <tr>
      <td role="rowheader">
        <p>[!UICONTROL 높이]</p>
      </td>
   <td> 추가할 높이 패딩 양을 입력하거나 매핑합니다. </td> 
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL 출력 파일 저장소]</td>
      <td>
        <p>편집한 파일을 저장할 파일 서비스를 선택합니다.</p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">
        <p>[!UICONTROL 출력 파일 URL]</p>
      </td>
   <td> 편집된 파일이 저장되는 위치의 URL 또는 경로를 입력하거나 매핑합니다. </td> 
    </tr>
    <tr>
      <td role="rowheader">
        <p>[!UICONTROL 출력 파일 유형]</p>
      </td>
   <td> 편집한 파일의 파일 유형을 선택합니다. </td> 
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL 덮어쓰기]</td>
      <td>
        <p>새로 편집한 파일이 이미 있는 출력 파일을 덮어쓸지 여부를 선택합니다.</p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">
        <p>[!UICONTROL Compression]</p>
      </td>
   <td> 출력 파일의 압축 레벨을 선택합니다. </td> 
    </tr>
  </tbody>
</table>

#### 레이어 정보 가져오기

이 작업 모듈은 지정된 PSD 파일에서 레이어 정보를 검색합니다.

<table style="table-layout:auto"> 
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">[!UICONTROL Connection]</td>
      <td>[!DNL Adobe Photoshop]에 대한 연결을 만드는 방법에 대한 지침은 이 문서에서 <a href="#create-a-connection-to-adobe-photoshop" class="MCXref xref" >[!DNL Adobe Photoshop]</a>에 대한 연결 만들기 를 참조하십시오.</td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL 입력 파일 저장소]</td>
      <td>
        <p>레이어 정보를 검색할 파일이 저장되어 있는 파일 서비스를 선택합니다.</p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">
        <p>[!UICONTROL 입력 파일 URL]</p>
      </td>
   <td> 레이어 정보를 검색할 파일의 URL 또는 경로를 입력하거나 매핑합니다. </td> 
    </tr>
    <tr>
      <td role="rowheader">
        <p>[!UICONTROL 썸네일]</p>
      </td>
   <td> </td> 
    </tr>
  </tbody>
</table>

#### 사용자 지정 API 호출 만들기

이 작업 모듈은 Photoshop API에 대한 사용자 지정 호출을 만듭니다.

<table style="table-layout:auto"> 
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">[!UICONTROL Connection]</td>
      <td>[!DNL Adobe Photoshop]에 대한 연결을 만드는 방법에 대한 지침은 이 문서에서 <a href="#create-a-connection-to-adobe-photoshop" class="MCXref xref" >[!DNL Adobe Photoshop]</a>에 대한 연결 만들기 를 참조하십시오.</td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL URL]</td>
      <td>
        <p><code>https://image.adobe.io/pie/psdService</code>과(와) 관련된 경로를 입력하십시오. 예: <code>/photoshopActions</code></p>
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
        <p>요청 쿼리 문자열을 입력합니다.</p>
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
