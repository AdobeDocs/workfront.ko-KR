---
filename: figma-modules
content-type: reference
product-previous: workfront-fusion
product-area: workfront-integrations
navigation-topic: apps-and-their-modules
title: Figma 모듈
description: 사용 [!DNL Adobe Workfront Fusion] 그림 모듈에서는 주석, 파일, 파일 버전 또는 프로젝트 목록을 검색할 수 있습니다. 주석을 게시하거나 Figuma API를 호출할 수도 있습니다.
author: Becky
exl-id: d88db592-32d4-4765-952f-9ffb58cf1720
source-git-commit: 885d93dd4383945538e977fd3edbfd55bda88b70
workflow-type: tm+mt
source-wordcount: '2261'
ht-degree: 1%

---

# [!DNL Figma] 모듈

사용 [!DNL Adobe Workfront Fusion] [!DNL Figma] 모듈, 주석, 파일, 파일 버전 또는 프로젝트 목록을 검색할 수 있습니다. 댓글을 게시하거나 을 호출할 수도 있습니다 [!DNL Figma] API.

시나리오 만들기에 대한 지침이 필요한 경우 [시나리오 만들기](../../workfront-fusion/scenarios/create-a-scenario.md).

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

를 사용하려면 [!DNL Figma] 모듈이면 반드시 [!DNL Figma] 계정이 필요합니다.

## [!DNL Figma] 모듈 및 해당 필드

구성 시 [!DNL Figma] 모듈, [!DNL Workfront Fusion] 아래 나열된 필드를 표시합니다. 이와 함께 추가 [!DNL Figma] 앱이나 서비스에서 액세스 수준과 같은 요소에 따라 필드가 표시될 수 있습니다. 모듈에서 굵게 표시된 제목은 필수 필드를 나타냅니다.

필드 또는 함수 위에 맵 단추가 표시되면 이 단추를 사용하여 해당 필드에 대한 변수와 함수를 설정할 수 있습니다. 자세한 내용은 [의 한 모듈에서 다른 모듈로 정보 매핑 [!DNL Adobe Workfront Fusion]](../../workfront-fusion/mapping/map-information-between-modules.md).

![](assets/map-toggle-350x74.png)

* [댓글](#comments)

* [프로젝트 및 파일](#projects-and-files)

* [구성 요소 및 스타일](#components-and-styles)

* [기타](#other)


### 댓글

* [댓글 삭제](#delete-a-comment)

* [주석 나열](#list-comments)

* [댓글 게시](#post-a-comment)


#### [!UICONTROL 댓글 삭제]

이 작업 모듈은 파일에서 단일 주석을 삭제합니다.

<table style="table-layout:auto"> 
  <col/>
  <col />
  <tbody>
    <tr>
      <td role="rowheader">[!UICONTROL Connection]</td>
      <td> <p>연결 방법에 대한 지침은 [!DNL Figma] 계정 대상 [!DNL Workfront Fusion]를 참조하십시오. <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">연결 만들기 [!DNL Adobe Workfront Fusion] - 기본 지침</a></p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL 파일 ID]</td>
      <td>주석을 삭제할 파일의 파일 ID를 입력하거나 매핑합니다. </td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Comment]</td>
      <td>삭제할 주석의 텍스트를 입력합니다.</td>
    </tr>
  </tbody>
</table>

#### [!UICONTROL 주석 나열]

이 검색 모듈은 [!DNL Figma].

<table style="table-layout:auto"> 
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">[!UICONTROL Connection]</td>
      <td> <p>연결 방법에 대한 지침은 [!DNL Figma] 계정 대상 [!DNL Workfront Fusion]를 참조하십시오. <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">연결 만들기 [!DNL Adobe Workfront Fusion] - 기본 지침</a></p>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL 파일 ID]</td>
      <td>
        <p>주석을 검색할 파일의 파일 ID를 입력하거나 매핑합니다. </p>
        <ul>
          <li>
            <p>ID를 모를 경우 <b>[!UICONTROL 파일 찾기]</b> 및 파일과 연결된 프로젝트의 ID를 입력하거나 매핑한 다음 파일을 선택합니다.</p>
          </li>
          <li>
            <p>프로젝트의 ID를 모를 경우 <b>[!UICONTROL 프로젝트 찾기]</b> 그리고 파일이 연결된 프로젝트를 소유하는 팀의 ID를 입력하거나 매핑한 다음 프로젝트를 선택한 다음 파일을 선택합니다.</p>
          </li>
        </ul>
      </td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL 제한]</td>
      <td>각 시나리오 실행 주기 동안 모듈이 반환할 최대 댓글 수를 입력하거나 매핑합니다.</td>
    </tr>
  </tbody>
</table>


#### [!UICONTROL 댓글 게시]

이 작업 모듈은 Figma 파일에 주석을 게시합니다.

<table style="table-layout:auto"> 
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">[!UICONTROL Connection]</td>
      <td> <p>연결 방법에 대한 지침은 [!DNL Figma] 계정 대상 [!DNL Workfront Fusion]를 참조하십시오. <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">연결 만들기 [!DNL Adobe Workfront Fusion] - 기본 지침</a></p>
    </tr>
    <tr>
      <td  role="rowheader">[!UICONTROL 파일 ID]</td>
      <td>
        <p>댓글을 게시할 파일의 파일 ID를 입력하거나 매핑합니다. </p>
        <ul>
          <li>
            <p>파일의 ID를 모를 경우 <b>[!UICONTROL 파일 찾기]</b> 및 파일과 연결된 프로젝트의 ID를 입력하거나 매핑한 다음 파일을 선택합니다.</p>
          </li>
          <li>
            <p>파일의 ID를 찾고 프로젝트의 ID를 모르는 경우 를 클릭합니다 <b>[!UICONTROL 프로젝트 찾기]</b> 및 파일이 연결된 프로젝트를 소유하는 팀의 ID를 입력하거나 매핑합니다. 프로젝트를 선택한 다음 파일을 선택합니다.</p>
          </li>
        </ul>
      </td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Comment]</td>
      <td>설명 텍스트를 입력합니다.</td>
    </tr>
  </tbody>
</table>


### 프로젝트 및 파일

* [파일 또는 이미지 가져오기](#get-a-file-or-image)

* [파일 버전 기록 나열](#list-file-version-history)

* [프로젝트 파일 나열](#list-project-files)

* [프로젝트 나열](#list-projects)


#### [!UICONTROL 파일 또는 이미지 가져오기]

이 작업 모듈은 Figuma 라이브러리에서 단일 파일 또는 이미지를 검색합니다

<table style="table-layout:auto"> 
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">[!UICONTROL Connection]</td>
      <td> <p>연결 방법에 대한 지침은 [!DNL Figma] 계정 대상 [!DNL Workfront Fusion]를 참조하십시오. <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">연결 만들기 [!DNL Adobe Workfront Fusion] - 기본 지침</a></p>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL 개체 유형]</td>
      <td>
        <p>검색할 객체 유형을 선택합니다.</p>
        <ul>
          <li>
            <p><b>[!UICONTROL File]</b>
            </p>
            <p>이 모듈은 [!UICONTROL Key]에서 참조하는 문서를 JSON 개체로 반환합니다. 파일 키는 Figma 파일 URL에서 구문 분석할 수 있습니다.</p>
            <p>필드에 대해서는 다음을 참조하십시오 <a href="#Get2" class="MCXref xref" >[!UICONTROL 파일 또는 이미지 가져오기: 파일]</a>.</p>
          </li>
          <li>
            <p><b>[!UICONTROL 파일 노드]</b>
            </p>
            <p>ID에서 참조하는 노드를 JSON 개체로 반환합니다. 노드는 [!DNL Figma] [!UICONTROL Key]에 의해 참조되는 파일입니다.</p>
            <p>필드에 대해서는 다음을 참조하십시오 <a href="#Get3" class="MCXref xref" >[!UICONTROL 파일 또는 이미지 가져오기: 파일 노드]</a>.</p>
          </li>
          <li>
            <p><b>[!UICONTROL Image]</b>
            </p>
            <p>모듈은 파일에서 이미지를 렌더링합니다.</p>
            <p>필드에 대해서는 다음을 참조하십시오 <a href="#Get4" class="MCXref xref" >[!UICONTROL 파일 또는 이미지 가져오기: 이미지]</a>.</p>
          </li>
          <li>
            <p><b>[!UICONTROL 이미지 채우기]</b>
            </p>
            <p>이 모듈은 문서에 이미지 채우기에 있는 모든 이미지에 대한 다운로드 링크를 반환합니다. 이미지 채우기는 다음과 같습니다 [!DNL Figma] 사용자가 제공한 모든 이미지를 나타냅니다. 이미지를 로 드래그할 때 [!DNL Figma], [!DNL Figma] 이미지를 나타내는 단일 채우기로 사각형을 만들고, 사용자는 사각형 및 채우기 상의 속성을 변형할 수 있습니다.</p>
            <p>필드에 대해서는 다음을 참조하십시오 <a href="#Get5" class="MCXref xref" >[!UICONTROL 파일 또는 이미지 가져오기: 이미지 채우기]</a>.</p>
          </li>
        </ul>
      </td>
    </tr>
  </tbody>
</table>


##### [!UICONTROL 파일 또는 이미지 가져오기: 파일]

<table style="table-layout:auto"> 
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">[!UICONTROL 파일 키]</td>
      <td>JSON을 반환할 파일을 선택합니다.</td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL 버전 ID]</td>
      <td>모듈이 반환할 파일 버전을 입력하거나 매핑합니다. 현재 모듈의 경우 이 필드를 비워 둡니다.</td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL 노드 ID]</td>
      <td>
        <p>문서의 하위 집합만 반환하려면 모듈이 반환할 노드를 입력합니다. 이 모듈은 나열된 노드, 해당 하위 및 루트 노드와 나열된 노드 사이의 모든 항목을 반환합니다.</p>
        <p>반환할 각 노드에 대해 <b>[!UICONTROL Add]</b> 노드의 텍스트를 입력합니다.</p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Depth]</td>
      <td>
        <p>결과를 반환할 문서 트리 깊이를 나타내는 정수를 입력하거나 매핑합니다. </p>
        <div class="example"><span class="autonumber"><span><b>예: </b></span></span>
          <ul>
            <li>
              <p>페이지만 반환하려면 를 입력합니다. <code>1</code>.</p>
            </li>
            <li>
              <p>페이지 및 최상위 객체를 반환하려면 를 입력합니다. <code>2</code>.</p>
            </li>
          </ul>
        </div>
        <p>모든 노드를 반환하려면 이 필드를 비워 둡니다.</p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Geometry]</td>
      <td>벡터 데이터를 반환하려면 를 입력합니다. <code>paths</code>.</td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL 플러그인 데이터]</td>
      <td>플러그인 ID 및/또는 문자열 "[!UICONTROL shared]"를 쉼표로 구분한 목록입니다. 해당 플러그인이 작성한 문서에 있는 모든 데이터는 <code>pluginData</code> 및 <code>sharedPluginData</code> 속성을 사용합니다.</td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Branch data]</td>
      <td>요청한 파일에 대한 분기 메타데이터를 반환하려면 이 옵션을 활성화합니다. 파일이 분기이면 기본 파일의 키가 반환된 응답에 포함됩니다. 파일에 분기가 있는 경우 해당 메타데이터가 반환된 응답에 포함됩니다. 기본: <code>false</code>.</td>
    </tr>
  </tbody>
</table>

##### [!UICONTROL 파일 또는 이미지 가져오기: 파일 노드]

<table style="table-layout:auto"> 
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">[!UICONTROL 파일 키]</td>
      <td>JSON을 반환할 파일을 선택합니다.</td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL 노드 ID]</td>
      <td>
        <p>모듈에서 반환하고 변환할 노드를 입력합니다</p>
        <p>반환할 각 노드에 대해 <b>[!UICONTROL Add]</b> 노드의 텍스트를 입력합니다.</p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL 버전 ID]</td>
      <td>모듈이 반환할 파일 버전을 입력하거나 매핑합니다. 현재 모듈의 경우 이 필드를 비워 둡니다.</td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Depth]</td>
      <td>
        <p>결과를 반환할 문서 트리 깊이를 나타내는 정수를 입력하거나 매핑합니다. </p>
        <div class="example"><span class="autonumber"><span><b>예: </b></span></span>
          <ul>
            <li>
              <p>페이지만 반환하려면 를 입력합니다. <code>1</code>.</p>
            </li>
            <li>
              <p>페이지 및 최상위 객체를 반환하려면 를 입력합니다. <code>2</code>.</p>
            </li>
          </ul>
        </div>
        <p>모든 노드를 반환하려면 이 필드를 비워 둡니다.</p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Geometry]</td>
      <td>벡터 데이터를 반환하려면 를 입력합니다. <code>paths</code>.</td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL 플러그인 데이터]</td>
      <td>플러그인 ID 및/또는 문자열 "shared"가 쉼표로 구분된 목록입니다. 해당 플러그인이 작성한 문서에 있는 모든 데이터는 pluginData 및 sharedPluginData 속성의 결과에 포함됩니다.</td>
    </tr>
  </tbody>
</table>


##### 파일 또는 이미지 가져오기: 이미지

<table style="table-layout:auto"> 
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">[!UICONTROL 파일 키]</td>
      <td>JSON을 반환할 파일을 선택합니다.</td>
    </tr>
    <tr>
      <td role="rowheader" [!UICONTROL>노드 ID]</td>
      <td>
        <p>모듈을 렌더링할 노드를 입력합니다.</p>
        <p>렌더링할 각 노드에 대해 <b>[!UICONTROL Add]</b> 노드의 텍스트를 입력합니다.</p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Scale]</td>
      <td>이미지의 크기를 조절하려면 배율 인수를 입력하거나 매핑합니다. 이 숫자는 0.01에서 4 사이여야 합니다.</td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL 형식]</td>
      <td>
        <p>이미지 출력의 형식을 선택합니다.</p>
        <ul>
          <li>
            <p>JPG</p>
          </li>
          <li>
            <p>PNG</p>
          </li>
          <li>
            <p>SVG</p>
          </li>
          <li>
            <p>PDF</p>
          </li>
        </ul>
      </td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL SVG - ID 포함]</td>
      <td>모든 SVG 요소에 대한 ID 속성을 포함하려면 이 옵션을 활성화합니다. 기본값: [!UICONTROL false].</td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL SVG - 획 간소화]</td>
      <td>이 옵션을 사용하면 내부/외부 선을 단순화하고 가능한 경우 획 특성을 사용할 수 있습니다. &lt;mask&gt;. 기본값: [!UICONTROL true].</td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL 절대 경계 사용]</td>
      <td>잘렸는지 여부 또는 그 주위의 공간이 비어 있는지에 상관없이 노드의 전체 크기를 사용하려면 이 옵션을 활성화합니다. 자르지 않고 텍스트 노드를 내보내려면 이 옵션을 사용합니다. 기본값: [!UICONTROL false].</td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL 버전 ID]</td>
      <td>모듈이 반환할 파일 버전을 입력하거나 매핑합니다. 현재 모듈의 경우 이 필드를 비워 둡니다.</td>
    </tr>
  </tbody>
</table>

##### 파일 또는 이미지 가져오기: 이미지 채우기

<table style="table-layout:auto"> 
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">[!UICONTROL 파일 키]</td>
      <td>JSON을 반환할 파일을 선택합니다.</td>
    </tr>
  </tbody>
</table>

### [!UICONTROL 파일 버전 기록 나열]

이 검색 모듈은 [!UICONTROL 피그마].
<table style="table-layout:auto"> 
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">[!UICONTROL Connection]</td>
      <td> <p>연결 방법에 대한 지침은 [!DNL Figma] 계정 대상 [!DNL Workfront Fusion]를 참조하십시오. <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">연결 만들기 [!DNL Adobe Workfront Fusion] - 기본 지침</a></p>
    <tr>
      <td role="rowheader">[!UICONTROL 파일 ID]</td>
      <td>
        <p>버전 기록을 검색할 파일의 파일 ID를 입력하거나 매핑합니다. </p>
        <ul>
          <li>
            <p>파일의 ID를 모를 경우 <b>[!UICONTROL 파일 찾기]</b> 및 파일과 연결된 프로젝트의 ID를 입력하거나 매핑한 다음 파일을 선택합니다.</p>
          </li>
          <li>
            <p>파일의 ID를 찾고 프로젝트의 ID를 모르는 경우 를 클릭합니다 <b>[!UICONTROL 프로젝트 찾기]</b> 및 파일이 연결된 프로젝트를 소유하는 팀의 ID를 입력하거나 매핑합니다. 프로젝트를 선택한 다음 파일을 선택합니다.</p>
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

#### [!UICONTROL 프로젝트 파일 나열]

이 검색 모듈은 지정된 프로젝트의 모든 파일 목록을 반환합니다.

<table style="table-layout:auto"> 
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">[!UICONTROL Connection]</td>
      <td> <p>연결 방법에 대한 지침은 [!DNL Figma] 계정 대상 [!DNL Workfront Fusion]를 참조하십시오. <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">연결 만들기 [!DNL Adobe Workfront Fusion] - 기본 지침</a></p>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL 파일 ID]</td>
      <td>
        <p>파일을 검색할 프로젝트에 프로젝트 ID를 입력하거나 매핑합니다. </p>
        <ul>
          <li>
            <p>프로젝트의 ID를 모를 경우 <b>[!UICONTROL 프로젝트 찾기]</b> 프로젝트를 연결된 팀의 ID를 입력하거나 매핑한 다음 프로젝트를 선택합니다.</p>
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

#### [!UICONTROL 프로젝트 나열]

이 검색 모듈은 지정된 팀 내의 모든 프로젝트 목록을 반환합니다.

<table style="table-layout:auto"> 
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">[!UICONTROL Connection]</td>
      <td> <p>연결 방법에 대한 지침은 [!DNL Figma] 계정 대상 [!DNL Workfront Fusion]를 참조하십시오. <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">연결 만들기 [!DNL Adobe Workfront Fusion] - 기본 지침</a></p>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Team ID]</td>
      <td>파일을 검색할 프로젝트의 프로젝트 ID를 입력하거나 매핑합니다. 팀 ID는 Figma의 팀 페이지 URL에서 찾을 수 있습니다</td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL 제한]</td>
      <td>각 시나리오 실행 주기 동안 모듈이 반환할 최대 레코드 수를 입력하거나 매핑합니다.</td>
    </tr>
  </tbody>
</table>


### 구성 요소 및 스타일

#### [!UICONTROL 스타일 또는 구성 요소 가져오기]

이 작업 모듈은 단일 스타일 또는 구성 요소나 스타일 또는 구성 요소 세트를 검색합니다.

<table style="table-layout:auto"> 
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">[!UICONTROL Connection]</td>
      <td> <p>연결 방법에 대한 지침은 [!DNL Figma] 계정 대상 [!DNL Workfront Fusion]를 참조하십시오. <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">연결 만들기 [!DNL Adobe Workfront Fusion] - 기본 지침</a></p>
    </tr>
    <tr>
      <td role="rowheader">&lt;[!UICONTROL Object&gt; 키]</td>
      <td>검색할 객체의 키(고유 식별자)를 입력합니다.</td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Team ID]</td>
      <td>레코드나 레코드가 연관된 팀의 ID를 입력하거나 매핑합니다.</td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL 페이지 크기]</td>
      <td>페이지당 반환되는 숫자나 결과를 입력하거나 매핑합니다. 기본값: 30.</td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL After]</td>
      <td>
        <p>결과 검색을 시작할 결과 번호를 입력하거나 매핑합니다. 결과를 게시하려면 [!UICONTROL 페이지 크기] 필드와 결합할 수 있습니다.</p>
        <p>이 값은 개체 ID에 해당하지 않습니다.</p>
        <p>이 필드는 [!UICONTROL Before] 필드와 함께 사용할 수 없습니다.</p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Before]</td>
      <td>
        <p>결과 검색을 시작할 결과 수를 입력하거나 매핑합니다. 결과를 게시하려면 [!UICONTROL 페이지 크기] 필드와 결합할 수 있습니다.</p>
        <p>이 값은 개체 ID에 해당하지 않습니다.</p>
        <p>이 필드는 [!UICONTROL After] 필드와 함께 사용할 수 없습니다.</p>
      </td>
    </tr>
  </tbody>
</table>


### 기타

* [API 호출 만들기](#make-an-api-call)

* [이벤트 보기](#watch-events)


#### [!UICONTROL API 호출 만들기]

이 작업 모듈을 사용하면 인증을 통해 생각하지 않고도 Figma API에 대해 사용자 지정 인증 호출을 수행할 수 있습니다. 이렇게 하면 다른 Figma 모듈에서 수행할 수 없는 데이터 흐름 자동화를 만들 수 있습니다.

<table style="table-layout:auto"> 
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">[!UICONTROL Connection]</td>
      <td> <p>연결 방법에 대한 지침은 [!DNL Figma] 계정 대상 [!DNL Workfront Fusion]를 참조하십시오. <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">연결 만들기 [!DNL Adobe Workfront Fusion] - 기본 지침</a></p>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL URL]</td>
      <td>
        <p>상대 경로 입력 <code>https://api.figma.com/v1/</code>.</p>
        <p>For example: <code>[!DNL files/7179110/comments]</code></p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL 메서드]</td>
      <td> <p>API 호출을 구성하는 데 필요한 HTTP 요청 메서드를 선택합니다. 자세한 내용은 <a href="../../workfront-fusion/modules/http-request-methods.md" class="MCXref xref" data-mc-variable-override="">의 HTTP 요청 메서드 [!DNL Adobe Workfront Fusion]</a>.</p> </td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Headers]</td>
      <td>
        <p>요청의 헤더를 표준 JSON 개체 형태로 추가합니다.</p>
        <p>For example, <code>{"Content-type":"application/json"}</code></p>
        <p>[!DNL Workfront Fusion] 사용자를 위해 인증 헤더를 추가합니다.</p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL 쿼리 문자열]</td>
      <td>
        <p>표준 JSON 개체 형태로 API 호출에 대한 쿼리를 추가합니다.</p>
        <p>For example: <code>{"name":"something-urgent"}</code></p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Body]</td>
   <td> <p>표준 JSON 개체 형태로 API 호출에 대한 본문 콘텐츠를 추가합니다.</p> <p>참고:  <p>다음과 같은 조건문을 사용하는 경우 <code>if</code> json에서 따옴표를 조건문 외부에 지정합니다.</p> 
     <div class="example" data-mc-autonum="<b>Example: </b>"> 
      <p> <img src="assets/quotes-in-json-350x120.png" style="width: 350;height: 120;"> </p> 
     </div> </p> </td>     </tr>
  </tbody>
</table>

#### [!UICONTROL 이벤트 보기]

이 트리거 모듈은 의 특정 팀에 대해 다음 이벤트 중 하나가 발생하면 시나리오를 시작합니다 [!DNL Figma] 팀 공간

* 파일 업데이트

* 파일 버전 업데이트

* 파일 삭제

* 라이브러리 게시

* 파일 주석

<table style="table-layout:auto"> 
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">[!UICONTROL Webhook]</td>
      <td>
        <p>모듈이 감시하는 웹 후크를 선택합니다.</p>
        <p>새 웹 후크를 추가하려면 다음을 수행합니다.</p>
        <ol>
          <li value="1">
            <p>클릭 <b>[!UICONTROL Add]</b> 를 클릭하십시오.</p>
          </li>
          <li value="2">
            <p>이 웹 후크에 사용할 연결을 선택합니다. 연결 방법에 대한 지침은 [!DNL Figma] [!UICONTROL Workfront Fusion]에 대한 계정입니다. <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">[!UICONTROL Adobe Workfront Fusion] - 기본 지침에 대한 연결을 만듭니다.</a></p>
          </li>
          <li value="3">
            <p>모듈에서 보려는 이벤트 유형을 선택합니다.</p>
          </li>
          <li value="4">
            <p>웹 후크를 검사할 이벤트의 팀 ID를 입력합니다.</p>
          </li>
          <li value="5">
            <p>웹 후크에서 볼 이벤트의 [!UICONTROL 상태] 또는 [!UICONTROL 설명]을 입력합니다.</p>
          </li>
          <li value="6">
            <p>클릭 <b>[!UICONTROL Save]</b> 웹 후크를 저장하고 모듈로 돌아가려면 를 클릭합니다.</p>
          </li>
        </ol>
      </td>
    </tr>
  </tbody>
</table>
