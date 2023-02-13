---
content-type: reference
product-previous: workfront-fusion
product-area: workfront-integrations;documents
keywords: 커넥터
navigation-topic: apps-and-their-modules
title: Google 문서 모듈
description: Adobe Workfront Fusion [!DNL Google Docs] 모듈을 사용하면 [!DNL Google Docs] 및 [!DNL Google Docs] ( [!DNL G Suite] 사용자)
author: Becky
feature: Workfront Fusion, Digital Content and Documents
exl-id: fbe7d628-d833-43ce-83b8-8e4e6a812fd1
source-git-commit: 885d93dd4383945538e977fd3edbfd55bda88b70
workflow-type: tm+mt
source-wordcount: '4042'
ht-degree: 0%

---

# [!DNL Google Docs] 모듈

다음 [!DNL Adobe Workfront Fusion] [!DNL Google Docs] 모듈을 사용하면 [!DNL Google Docs] 및 [!DNL Google Docs] (으)로 [!DNL G Suite] 사용자 참조).

를 사용하려면 [!DNL Google Docs] with [!DNL Adobe Workfront Fusion]를 채울 때는 [!DNL Google] 계정이 필요합니다. 만약 [!DNL Google] 아직 계정을 만들 수 있습니다. [!DNL Google] 계정 도움말 페이지입니다.

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

를 사용하려면 [!DNL Google Docs] 모듈, Google 계정이 있어야 합니다.

## [!DNL Google Docs] 모듈 및 해당 필드

구성 시 [!DNL Google Docs] 모듈, [!UICONTROL Workfront Fusion] 아래 나열된 필드를 표시합니다. 이와 함께 추가 [!DNL Google Docs] 앱이나 서비스에서 액세스 수준과 같은 요소에 따라 필드가 표시될 수 있습니다. 모듈에서 굵게 표시된 제목은 필수 필드를 나타냅니다.

필드 또는 함수 위에 맵 단추가 표시되면 이 단추를 사용하여 해당 필드에 대한 변수와 함수를 설정할 수 있습니다. 자세한 내용은 [의 한 모듈에서 다른 모듈로 정보 매핑 [!DNL Adobe Workfront Fusion]](../../workfront-fusion/mapping/map-information-between-modules.md).

![](assets/map-toggle-350x74.png)

### 문서

* [[!UICONTROL 문서 보기]](#watch-documents)
* [[!UICONTROL 문서 나열]](#list-documents)
* [[!UICONTROL 문서의 내용 가져오기]](#get-content-of-a-document)
* [[!UICONTROL 문서 만들기]](#create-a-document)
* [[!UICONTROL 템플릿에서 문서 만들기]](#create-a-document-from-a-template)
* [[!UICONTROL 문서에 단락 삽입]](#insert-a-paragraph-to-a-document)
* [[!UICONTROL 문서에 이미지 삽입]](#insert-an-image-to-a-document)
* [[!UICONTROL 이미지를 새 이미지로 바꾸기]](#replace-an-image-with-a-new-image)
* [[!UICONTROL 문서의 텍스트 바꾸기]](#replace-text-in-a-document)
* [[!UICONTROL 문서 다운로드]](#download-a-document)
* [[!UICONTROL 문서 삭제]](#delete-a-document)

#### [!UICONTROL 문서 보기]

이 트리거 모듈은 선택한 폴더에서 새 문서를 만들거나 수정할 때 문서 세부 사항을 반환합니다.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td> 
   <td> <p>연결 방법에 대한 지침은 [!DNL Google] 계정 대상 [!DNL Workfront Fusion]를 참조하십시오. <a href="../../workfront-fusion/scenarios/create-a-scenario.md#connect" class="MCXref xref">모듈의 앱 또는 웹 서비스를 [!DNL Workfront Fusion]</a> 기사 <a href="../../workfront-fusion/scenarios/create-a-scenario.md" class="MCXref xref">에서 시나리오 만들기 [!DNL Adobe Workfront Fusion]</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Watch Documents]</td> 
   <td> <p style="color: #000000;">만든 문서([!UICONTROL By Created Date])나 수정된 문서([!UICONTROL By Modified Date])를 보는지 여부를 선택합니다.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL 드라이브 선택]</td> 
   <td> <p>모니터링할 드라이브 유형을 선택합니다.</p> 
    <ul> 
     <li> <p><strong>[!UICONTROL My Drive]</strong> </p> <p>작성되거나 수정된 문서를 감시하려는 폴더를 선택합니다.</p> </li> 
     <li> <p><strong>[!UICONTROL Shared With Me]</strong> </p> <p>작성되거나 수정된 문서를 감시하려는 폴더를 선택합니다.</p> </li> 
     <li> <p><strong>[!UICONTROL [!DNL Google] 공유 드라이브]</strong> (사용 가능) [!DNL G Suite] 사용자만 해당)</p> <p>[!UICONTROL 도메인 관리자 액세스 사용] 여부를 선택합니다. [!UICONTROL Yes]를 선택하면 도메인 관리자로 요청이 발생하고 요청자가 관리자인 모든 공유 드라이브가 반환됩니다.</p> <p>보려는 공유 드라이브를 선택합니다.</p> <p>참고: 을(를) 선택한 경우 [!DNL Google Shared Drive] 이 필드의 옵션 및 사용자가 [!DNL G Suite] user, error <code>[400] Invalid Value</code> 가 반환됩니다.</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL 제한] </td> 
   <td> <p>한 실행 주기에 Workfront Fusion이 반환하는 최대 문서 수를 설정합니다.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL 문서 나열]

이 작업 모듈은 선택한 폴더에서 문서 목록을 검색합니다.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td> 
   <td> <p>연결 방법에 대한 지침은 [!DNL Google] 계정 대상 [!DNL Workfront Fusion]를 참조하십시오. <a href="../../workfront-fusion/scenarios/create-a-scenario.md#connect" class="MCXref xref">모듈의 앱 또는 웹 서비스를 [!DNL Workfront Fusion]</a> 기사 <a href="../../workfront-fusion/scenarios/create-a-scenario.md" class="MCXref xref">에서 시나리오 만들기 [!DNL Adobe Workfront Fusion]</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL 드라이브 선택]</td> 
   <td> <p>문서를 나열할 드라이브 유형을 선택합니다.</p> 
    <ul> 
     <li> <p><strong>[!UICONTROL My Drive]</strong> </p> <p>문서를 나열할 폴더를 선택합니다.</p> </li> 
     <li> <p><strong>[!UICONTROL Shared With Me]</strong> </p> <p>문서를 나열할 폴더를 선택합니다.</p> </li> 
     <li> <p><strong>[!UICONTROL [!DNL Google] 공유 드라이브]</strong> (사용 가능) [!DNL G Suite] 사용자만 해당)</p> <p>[!UICONTROL 도메인 관리자 액세스 사용] 여부를 선택합니다. [!UICONTROL Yes]를 선택하면 도메인 관리자로 요청이 발생하고 요청자가 관리자인 모든 공유 드라이브가 반환됩니다.</p> <p>문서를 나열할 공유 드라이브를 선택합니다.</p> <p>참고: 을(를) 선택한 경우 [!DNL Google Docs] 이 필드의 옵션 및 사용자가 [!DNL G Suite] user, error <code>[400] Invalid Value</code> 가 반환됩니다.</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL 제한] </td> 
   <td> <p>최대 문서 수 설정 [!DNL Workfront Fusion] 한 실행 주기에서 를 반환합니다.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL 문서의 내용 가져오기]

이 작업 모듈은 지정된 문서를 검색합니다.

권한을 확장해야 할 수 있습니다.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td> 
   <td> <p>연결 방법에 대한 지침은 [!DNL Google] 계정 대상 [!DNL Workfront Fusion]를 참조하십시오. <a href="../../workfront-fusion/scenarios/create-a-scenario.md#connect" class="MCXref xref">모듈의 앱 또는 웹 서비스를 [!DNL Workfront Fusion]</a> 기사 <a href="../../workfront-fusion/scenarios/create-a-scenario.md" class="MCXref xref">에서 시나리오 만들기 [!DNL Adobe Workfront Fusion]</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL 문서의 내용 가져오기]</td> 
   <td> <p>문서의 문서 ID를 매핑할지 또는 드롭다운 메뉴에서 수동으로 문서를 선택할지를 선택합니다.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL 드라이브 선택]</td> 
   <td> <p>검색할 문서가 포함된 드라이브 유형을 선택합니다.</p> 
    <ul> 
     <li> <p><strong>[!UICONTROL My Drive]</strong> </p> <p>검색할 문서가 포함된 폴더를 선택합니다.</p> </li> 
     <li> <p><strong>[!UICONTROL Shared With Me]</strong> </p> <p>검색할 문서가 포함된 폴더를 선택합니다.</p> </li> 
     <li> <p><strong>[!UICONTROL [!DNL Google] 공유 드라이브]</strong> (사용 가능) [!DNL G Suite] 사용자만 해당)</p> <p>[!UICONTROL 도메인 관리자 액세스 사용] 여부를 선택합니다. [!UICONTROL Yes]를 선택하면 도메인 관리자로 요청이 발생하고 요청자가 관리자인 모든 공유 드라이브가 반환됩니다.</p> <p>검색할 문서가 포함된 공유 드라이브를 선택합니다.</p> <p>참고: 을(를) 선택한 경우 [!DNL Google Docs] 이 필드의 옵션 및 사용자가 [!DNL G Suite] user, error <code>[400] Invalid Value</code> 가 반환됩니다.</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Filter]</p> </td> 
   <td> <p>모듈의 출력에 반환할 개체를 선택합니다.</p> 
    <ul> 
     <li>[!UICONTROL Image](기본값)</li> 
     <li>[!UICONTROL Drawing]</li> 
     <li>[!UICONTROL Chart]</li> 
    </ul> <p>참고:  <p>이러한 개체를 추가로 매핑하려면 이 모듈의 출력에 [!UICONTROL 인라인 개체 배열] 값을 사용하십시오( [!UICONTROL inlineObjects] 대신).</p> <p>[!UICONTROL 인라인 개체 배열] 개체는 문서에 나타나는 것과 동일한 순서로 정렬됩니다. 더 쉽게 처리할 수 있습니다.</p> </p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL 문서 만들기]

이 작업 모듈을 사용하면 선택한 폴더에 새 문서를 만들 수 있습니다.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td> 
   <td> <p>연결 방법에 대한 지침은 [!DNL Google] 계정 대상 [!DNL Workfront Fusion]를 참조하십시오. <a href="../../workfront-fusion/scenarios/create-a-scenario.md#connect" class="MCXref xref">모듈의 앱 또는 웹 서비스를 [!DNL Workfront Fusion]</a> 기사 <a href="../../workfront-fusion/scenarios/create-a-scenario.md" class="MCXref xref">에서 시나리오 만들기 [!DNL Adobe Workfront Fusion]</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Name] </td> 
   <td> <p>문서의 이름을 입력합니다.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Content]</td> 
   <td> <p>문서의 내용을 입력합니다. HTML이 지원됩니다.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL 드라이브 선택]</td> 
   <td> <p>문서를 만들 드라이브 유형을 선택합니다.</p> 
    <ul> 
     <li> <p><strong>[!UICONTROL My Drive]</strong> </p> <p>문서를 만들 폴더를 선택합니다.</p> </li> 
     <li> <p><strong>[!UICONTROL Shared With Me]</strong> </p> <p>문서를 만들 폴더를 선택합니다.</p> </li> 
     <li> <p><strong>[!UICONTROL [!DNL Google] 공유 드라이브]</strong> (사용 가능) [!DNL G Suite] 사용자만 해당)</p> <p>[!UICONTROL 도메인 관리자 액세스 사용] 여부를 선택합니다. [!UICONTROL Yes]를 선택하면 도메인 관리자로 요청이 발생하고 요청자가 관리자인 모든 공유 드라이브가 반환됩니다.</p> <p>문서를 만들 공유 드라이브를 선택합니다.</p> <p>참고: 을(를) 선택한 경우 [!DNL Google Docs] 이 필드의 옵션 및 사용자가 [!DNL G Suite] user, error <code>[400] Invalid Value</code> 가 반환됩니다.</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL 헤더 삽입]</td> 
   <td> <p> 이 옵션을 사용하여 문서에 헤더를 삽입한 다음 머리글의 텍스트를 입력하거나 매핑합니다.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL 바닥글 삽입] </td> 
   <td> <p>문서에 바닥글을 삽입한 다음 머리글의 텍스트를 입력하거나 매핑하려면 이 옵션을 활성화합니다.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL 템플릿에서 문서 만들기]

이 작업 모듈은 기존 템플릿 문서의 사본을 만들고 태그를 바꿉니다. 또한 이 모듈을 사용하면 사용자가 URL별로 이미지를 새 이미지로 바꿀 수 있습니다.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td> 
   <td> <p>연결 방법에 대한 지침은 [!DNL Google] 계정 대상 [!DNL Workfront Fusion]를 참조하십시오. <a href="../../workfront-fusion/scenarios/create-a-scenario.md#connect" class="MCXref xref">모듈의 앱 또는 웹 서비스를 [!DNL Workfront Fusion]</a> 기사 <a href="../../workfront-fusion/scenarios/create-a-scenario.md" class="MCXref xref">에서 시나리오 만들기 [!DNL Adobe Workfront Fusion]</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL 템플릿에서 문서 만들기]</p> </td> 
   <td> 
    <ul> 
     <li><strong>[!UICONTROL By Mapping]</strong> <br>문서 템플릿을 매핑하려면 이 옵션을 선택합니다.</li> 
     <li><strong>[!UICONTROL By Dropdown]</strong> <br>드롭다운 메뉴에서 문서 템플릿을 선택하려면 이 옵션을 선택합니다.</li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL 드라이브 선택]</td> 
   <td> <p>템플릿이 있는 드라이브 유형을 선택합니다. 이 옵션은 이전 필드에서 [!UICONTROL By Dropdown]을 선택한 경우 사용할 수 있습니다.</p> 
    <ul> 
     <li> <p><strong>[!UICONTROL My Drive]</strong> </p> <p>템플릿이 있는 폴더를 선택합니다.</p> </li> 
     <li> <p><strong>[!UICONTROL Shared With Me]</strong> </p> <p>템플릿이 있는 폴더를 선택합니다.</p> </li> 
     <li> <p><strong>[!UICONTROL [!DNL Google] 공유 드라이브]</strong> (사용 가능) [!DNL G Suite] 사용자만 해당)</p> <p>[!UICONTROL 도메인 관리자 액세스 사용] 여부를 선택합니다. [!UICONTROL Yes]를 선택하면 도메인 관리자로 요청이 발생하고 요청자가 관리자인 모든 공유 드라이브가 반환됩니다.</p> <p>템플릿이 있는 공유 드라이브를 선택합니다.</p> <p>참고: 을(를) 선택한 경우 [!DNL Google Docs] 이 필드의 옵션 및 사용자가 [!DNL G Suite] user, error <code>[400] Invalid Value</code> 가 반환됩니다.</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Values]</p> </td> 
   <td> <p>새 문서의 변수 대신 입력할 값을 입력합니다.</p> 
    <ul> 
     <li><strong>[!UICONTROL Tags]</strong> <br>문서 템플릿에 포함된 태그를 입력합니다. 사용 안 함 <code>&#123;&#123;&#125;&#125;</code>. 예: 사용 <code>name</code> 대신 <code>&#123;&#123;name&#125;&#125;</code>.</li> 
     <li><strong>[!UICONTROL Replaced Value]</strong><br>태그의 값을 입력합니다.</li> 
    </ul> <p>예:<code> &#123;&#123;name&#125;&#125;</code> 소스 문서의 변수는 여기에 이름 필드로 표시되며, 여기에서 값(예: )을 삽입할 수 있습니다 <code>John</code>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Images Replacement]</p> </td> 
   <td> <p>현재 이미지를 바꿀 [!UICONTROL 이미지 개체 ID] 및 [!UICONTROL 이미지 URL]에 대한 링크를 입력합니다.</p> <p>참고: [!UICONTROL 문서 가져오기] 모듈을 사용하여 이미지 ID를 검색할 수 있습니다. 이 모듈은 ID가 [!UICONTROL 인라인 개체 배열]에 포함되어 있습니다.</p> <p>의 이미지에 대체 텍스트를 추가하는 것이 좋습니다 [!DNL Google] 문서. </p> <p>에 대체 텍스트 를 추가하려면 [!DNL Google Docs] 이미지:</p> 
    <ol> 
     <li value="1">이미지를 마우스 오른쪽 단추로 클릭합니다.</li> 
     <li value="2">[!UICONTROL 대체 텍스트] 옵션을 선택합니다.</li> 
     <li value="3">[!UICONTROL Title] 필드에 [!UICONTROL ALT 텍스트]를 입력하고 [!UICONTROL OK]를 클릭합니다.</li> 
    </ol> <p>이미지에 대체 텍스트를 추가한 후에는 괄호로 묶인 필드 이름에 대체 텍스트가 표시됩니다.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Title] </td> 
   <td> <p>새 문서의 이름을 입력합니다.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL 드라이브 선택]</td> 
   <td> <p>템플릿이 있는 드라이브 유형을 선택합니다. 이 옵션은 이전 필드에서 [!UICONTROL By Dropdown]을 선택한 경우 사용할 수 있습니다.</p> 
    <ul> 
     <li> <p><strong>[!UICONTROL My Drive]</strong> </p> <p>문서를 만들 폴더를 선택합니다.</p> </li> 
     <li> <p><strong>[!UICONTROL Shared With Me]</strong> </p> <p>문서를 만들 폴더를 선택합니다.</p> </li> 
     <li> <p><strong>[!UICONTROL [!DNL Google] 공유 드라이브]</strong> (사용 가능) [!DNL G Suite] 사용자만 해당)</p> <p>[!UICONTROL 도메인 관리자 액세스 사용] 여부를 선택합니다. [!UICONTROL Yes]를 선택하면 도메인 관리자로 요청이 발생하고 요청자가 관리자인 모든 공유 드라이브가 반환됩니다.</p> <p>문서를 만들 공유 드라이브를 선택합니다.</p> <p>참고: 을(를) 선택한 경우 [!DNL Google Docs] 이 필드의 옵션 및 사용자가 [!DNL G Suite] user, error <code>[400] Invalid Value</code> 가 반환됩니다.</p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL 문서에 단락 삽입]

이 작업 모듈은 새 단락을 기존 문서에 추가하거나 삽입합니다.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td> 
   <td> <p>연결 방법에 대한 지침은 [!DNL Google] 계정 대상 [!DNL Workfront Fusion]를 참조하십시오. <a href="../../workfront-fusion/scenarios/create-a-scenario.md#connect" class="MCXref xref">모듈의 앱 또는 웹 서비스를 [!DNL Workfront Fusion]</a> 기사 <a href="../../workfront-fusion/scenarios/create-a-scenario.md" class="MCXref xref">에서 시나리오 만들기 [!DNL Adobe Workfront Fusion]</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL 문서 선택]</p> </td> 
   <td> 
    <ul> 
     <li><strong>[!UICONTROL By Mapping]</strong> <br>문서를 매핑하려면 이 옵션을 선택합니다.</li> 
     <li><strong>[!UICONTROL By Dropdown]</strong> <br> 드롭다운 메뉴에서 문서를 선택하려면 이 옵션을 선택합니다.</li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL 드라이브 선택]</td> 
   <td> <p>단락을 추가할 문서가 있는 드라이브 유형을 선택합니다. 이 옵션은 이전 필드에서 [!UICONTROL By Dropdown]을 선택한 경우 사용할 수 있습니다.</p> 
    <ul> 
     <li> <p><strong>[!UICONTROL My Drive]</strong> </p> <p>단락을 추가할 문서가 있는 폴더를 선택한 다음 문서를 선택합니다.</p> </li> 
     <li> <p><strong>[!UICONTROL Shared With Me]</strong> </p> <p>단락을 추가할 문서가 있는 폴더를 선택한 다음 문서를 선택합니다.</p> </li> 
     <li> <p><strong>[!UICONTROL [!DNL Google] 공유 드라이브]</strong> (사용 가능) [!DNL G Suite] 사용자만 해당)</p> <p>[!UICONTROL 도메인 관리자 액세스 사용] 여부를 선택합니다. [!UICONTROL Yes]를 선택하면 도메인 관리자로 요청이 발생하고 요청자가 관리자인 모든 공유 드라이브가 반환됩니다.</p> <p>단락을 추가할 문서가 있는 공유 드라이브를 선택한 다음 문서를 선택합니다.</p> <p>참고: 을(를) 선택한 경우 [!DNL Google Docs] 이 필드의 옵션 및 사용자가 [!DNL G Suite] user, error <code>[400] Invalid Value</code> 가 반환됩니다.</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL 단락 삽입]</p> </td> 
   <td> <p>문서에 새 텍스트를 삽입할 방법을 선택합니다.</p> 
    <ul> 
     <li> <p><strong>[!UICONTROL 위치 지정 기준]</strong> </p> 
      <ul> 
       <li> <p><strong>[!UICONTROL By Index]</strong> </p> 
        <ul> 
         <li> <p><strong>[!UICONTROL Index]</strong> </p> <p>텍스트를 삽입할 색인 번호를 입력합니다. [!UICONTROL 문서 가져오기] 모듈을 사용하여 인덱스 번호를 검색할 수 있습니다.</p> <p>문서에 모든 문자(숨김 포함)를 표시하려면 [!UICONTROL 표시] 추가 기능을 사용할 수 있습니다. [!UICONTROL 추가 기능] &gt; [!UICONTROL 추가 기능 가져오기]에서 추가 기능을 찾을 수 있습니다. [!UICONTROL Show]를 검색하고 [!UICONTROL Show] 추가 기능을 설치합니다.</p> </li> 
         <li> <p><strong>[!UICONTROL 삽입된 텍스트]</strong> </p> <p>문서에 삽입할 텍스트를 입력합니다.</p> </li> 
        </ul> </li> 
       <li> <p><strong>[!UICONTROL 세그먼트 ID별]</strong> </p> <p>텍스트 내용을 삽입할 머리글 및 바닥글을 선택하고 해당 필드에 삽입할 텍스트를 입력합니다.</p> <p>머리글이나 바닥글에 텍스트가 이미 포함되어 있으면 기존 텍스트 앞에 새 텍스트가 추가됩니다.</p> </li> 
      </ul> </li> 
     <li> <p><strong>[!UICONTROL 문서 본문에 를 추가하여]</strong> </p> <p>문서 본문 내용 끝에 입력한 텍스트를 추가합니다.</p> <p>목록 및 글머리 기호를 포함하여 현재 삽입 인덱스의 단락에 있는 새 단락의 스타일이 복사됩니다.</p> </li> 
    </ul> 
    <ul> 
     <li> <p><strong>[!UICONTROL 세그먼트 끝에 를 추가하여(머리글 및 바닥글)]</strong> </p> <p>텍스트 내용을 삽입할 머리글 및 바닥글을 선택하고 해당 필드에 삽입할 텍스트를 입력합니다.</p> <p>머리글 또는 바닥글에 텍스트가 이미 포함되어 있으면 기존 텍스트 뒤에 새 텍스트가 추가됩니다.</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Supported Text]</td> 
   <td>문서에 추가할 텍스트를 입력하거나 매핑합니다</td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL 문서에 이미지 삽입]

이 작업 모듈은 URL의 이미지를 문서에 삽입합니다.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td> 
   <td> <p>연결 방법에 대한 지침은 [!DNL Google] 계정 대상 [!DNL Workfront Fusion]를 참조하십시오. <a href="../../workfront-fusion/scenarios/create-a-scenario.md#connect" class="MCXref xref">모듈의 앱 또는 웹 서비스를 [!DNL Workfront Fusion]</a> 기사 <a href="../../workfront-fusion/scenarios/create-a-scenario.md" class="MCXref xref">에서 시나리오 만들기 [!DNL Adobe Workfront Fusion]</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL 문서 선택]</p> </td> 
   <td> 
    <ul> 
     <li><strong>[!UICONTROL By Mapping]</strong> <br>문서 템플릿을 매핑하려면 이 옵션을 선택합니다.</li> 
     <li><strong>[!UICONTROL By Dropdown]</strong> <br> 드롭다운 메뉴에서 문서를 선택하려면 이 옵션을 선택합니다.</li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL 드라이브 선택]</td> 
   <td> <p>이미지를 추가할 문서가 있는 드라이브 유형을 선택합니다. 이 옵션은 이전 필드에서 [!UICONTROL By Dropdown]을 선택한 경우 사용할 수 있습니다.</p> 
    <ul> 
     <li> <p><strong>[!UICONTROL My Drive]</strong> </p> <p>이미지를 추가할 문서가 있는 폴더를 선택한 다음 문서를 선택합니다.</p> </li> 
     <li> <p><strong>[!UICONTROL Shared With Me]</strong> </p> <p>이미지를 추가할 문서가 있는 폴더를 선택한 다음 문서를 선택합니다.</p> </li> 
     <li> <p><strong>[!UICONTROL [!DNL Google] 공유 드라이브]</strong> (사용 가능) [!DNL G Suite] 사용자만 해당)</p> <p>[!UICONTROL 도메인 관리자 액세스 사용] 여부를 선택합니다. [!UICONTROL Yes]를 선택하면 도메인 관리자로 요청이 발생하고 요청자가 관리자인 모든 공유 드라이브가 반환됩니다.</p> <p>이미지를 추가할 문서가 있는 공유 드라이브를 선택하고 문서를 선택합니다.</p> <p>참고: 을(를) 선택한 경우 [!DNL Google Docs] 이 필드의 옵션 및 사용자가 [!DNL G Suite] user, error <code>[400] Invalid Value</code> 가 반환됩니다.</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL 이미지 삽입]</p> </td> 
   <td> <p>문서에 새 이미지를 삽입할 방법을 선택합니다.</p> 
    <ul> 
     <li> <p><strong>[!UICONTROL 위치 지정 기준]</strong> </p> 
      <ul> 
       <li> <p><strong>[!UICONTROL By Index]</strong> </p> 
        <ul> 
         <li> <p><strong>[!UICONTROL Index]</strong> </p> <p>이미지를 삽입할 인덱스 번호를 입력합니다. [!UICONTROL 문서 가져오기] 모듈을 사용하여 [!UICONTROL 인덱스 번호]를 검색할 수 있습니다.</p> <p>문서에 모든 문자(숨김 포함)를 표시하려면 [!UICONTROL 표시] 추가 기능을 사용할 수 있습니다. [!UICONTROL 추가 기능] &gt; [!UICONTROL 추가 기능 가져오기]에서 추가 기능을 찾을 수 있습니다. [!UICONTROL Show]를 검색하고 [!UICONTROL Show] 추가 기능을 설치합니다.</p> </li> 
         <li> <p><strong>[!UICONTROL 이미지 URL]</strong> </p> <p>문서에 삽입할 이미지의 URL을 입력합니다.</p> <p>최대 이미지 크기는 50MB입니다. 25메가픽셀을 초과할 수 없습니다. PNG, JPEG 또는 GIF 형식만 지원됩니다.</p> </li> 
        </ul> </li> 
       <li> <p><strong>[!UICONTROL 세그먼트 ID별]</strong> </p> <p>이미지를 삽입할 머리글 및 바닥글을 선택하고 해당 필드에 이미지 URL을 입력합니다.</p> <p>최대 이미지 크기는 50MB입니다. 이미지는 25메가픽셀을 초과할 수 없습니다. PNG, JPEG 또는 GIF 형식만 지원됩니다.</p> </li> 
      </ul> </li> 
     <li> <p><strong>[!UICONTROL 문서 본문에 를 추가하여]</strong> </p> <p>문서의 본문 내용 끝에 특정 이미지를 추가합니다.</p> </li> 
    </ul> 
    <ul> 
     <li> <p><strong>[!UICONTROL 세그먼트 끝에 를 추가하여(머리글 및 바닥글)]</strong> </p> <p>이미지를 삽입할 머리글 및 바닥글을 선택하고 해당 필드에 삽입할 이미지 URL을 입력합니다.</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL 포인트/폭 크기(포인트)]</p> </td> 
   <td> <p>삽입된 이미지의 크기를 정의합니다. 종횡비는 유지된다.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL 이미지를 새 이미지로 바꾸기]

이 작업 모듈은 기존 이미지를 대체합니다. 원본 이미지의 종횡비는 그대로 유지됩니다.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td> 
   <td> <p>연결 방법에 대한 지침은 [!DNL Google] 계정 대상 [!DNL Workfront Fusion]를 참조하십시오. <a href="../../workfront-fusion/scenarios/create-a-scenario.md#connect" class="MCXref xref">모듈의 앱 또는 웹 서비스를 [!DNL Workfront Fusion]</a> 기사 <a href="../../workfront-fusion/scenarios/create-a-scenario.md" class="MCXref xref">에서 시나리오 만들기 [!DNL Adobe Workfront Fusion]</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL 문서 선택]</p> </td> 
   <td> 
    <ul> 
     <li><strong>[!UICONTROL By Mapping]</strong> <br>문서 템플릿을 매핑하려면 이 옵션을 선택합니다.</li> 
     <li><strong>[!UICONTROL By Dropdown]</strong> <br> 드롭다운 메뉴에서 문서를 선택하려면 이 옵션을 선택합니다.</li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL 드라이브 선택]</td> 
   <td> <p>이미지를 바꿀 문서가 있는 드라이브 유형을 선택합니다. 이 옵션은 이전 필드에서 [!UICONTROL By Dropdown]을 선택한 경우 사용할 수 있습니다.</p> 
    <ul> 
     <li> <p><strong>[!UICONTROL My Drive]</strong> </p> <p>이미지를 바꿀 문서가 있는 폴더를 선택한 다음 문서를 선택합니다.</p> </li> 
     <li> <p><strong>[!UICONTROL Shared With Me]</strong> </p> <p>이미지를 바꿀 문서가 있는 폴더를 선택한 다음 문서를 선택합니다.</p> </li> 
     <li> <p><strong>[!UICONTROL [!DNL Google] 공유 드라이브]</strong> (사용 가능) [!DNL G Suite] 사용자만 해당)</p> <p>[!UICONTROL 도메인 관리자 액세스 사용] 여부를 선택합니다. [!UICONTROL Yes]를 선택하면 도메인 관리자로 요청이 발생하고 요청자가 관리자인 모든 공유 드라이브가 반환됩니다.</p> <p>이미지를 바꿀 문서가 있는 공유 드라이브를 선택한 다음 문서를 선택합니다.</p> <p>참고: 을(를) 선택한 경우 [!DNL Google Docs] 이 필드의 옵션 및 사용자가 [!DNL G Suite] user, error <code>[400] Invalid Value</code> 가 반환됩니다.</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL 이미지 URL]</p> </td> 
   <td> <p>기존 이미지를 바꿀 새 이미지의 URL을 입력하거나 매핑합니다.</p> <p>이미지는 문서에 나타나는 순서대로 나열됩니다. 예, <code>Body: Image No. 1</code> 는 문서의 첫 번째 이미지입니다.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL 문서의 텍스트 바꾸기]

이 작업 모듈은 문서의 텍스트를 대체합니다.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td> 
   <td> <p>연결 방법에 대한 지침은 [!DNL Google] 계정 대상 [!DNL Workfront Fusion]를 참조하십시오. <a href="../../workfront-fusion/scenarios/create-a-scenario.md#connect" class="MCXref xref">모듈의 앱 또는 웹 서비스를 [!DNL Workfront Fusion]</a> 기사 <a href="../../workfront-fusion/scenarios/create-a-scenario.md" class="MCXref xref">에서 시나리오 만들기 [!DNL Adobe Workfront Fusion]</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL 문서 선택]</p> </td> 
   <td> 
    <ul> 
     <li><strong>[!UICONTROL By Mapping]</strong> <br>문서 템플릿을 매핑하려면 이 옵션을 선택합니다.</li> 
     <li><strong>[!UICONTROL By Dropdown]</strong> <br> 드롭다운 메뉴에서 문서를 선택하려면 이 옵션을 선택합니다.</li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL 드라이브 선택]</td> 
   <td> <p>텍스트를 추가할 문서가 있는 드라이브 유형을 선택합니다. 이 옵션은 이전 필드에서 [!UICONTROL By Dropdown]을 선택한 경우 사용할 수 있습니다.</p> 
    <ul> 
     <li> <p><strong>[!UICONTROL My Drive]</strong> </p> <p>텍스트를 추가할 문서가 있는 폴더를 선택한 다음 문서를 선택합니다.</p> </li> 
     <li> <p><strong>[!UICONTROL Shared With Me]</strong> </p> <p>텍스트를 추가할 문서가 있는 폴더를 선택한 다음 문서를 선택합니다.</p> </li> 
     <li> <p><strong>[!UICONTROL [!DNL Google] 공유 드라이브]</strong> (사용 가능) [!DNL G Suite] 사용자만 해당)</p> <p>[!UICONTROL 도메인 관리자 액세스 사용] 여부를 선택합니다. [!UICONTROL Yes]를 선택하면 도메인 관리자로 요청이 발생하고 요청자가 관리자인 모든 공유 드라이브가 반환됩니다.</p> <p>텍스트를 추가할 문서가 있는 공유 드라이브를 선택하고 문서를 선택합니다.</p> <p>참고: 을(를) 선택한 경우 [!DNL Google Docs] 이 필드의 옵션 및 사용자가 [!DNL G Suite] user, error <code>[400] Invalid Value</code> 가 반환됩니다.</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL 텍스트 바꾸기]</p> </td> 
   <td> <p>바꿀 각 텍스트를 추가합니다.</p> 
    <ul> 
     <li> <p><strong>[!UICONTROL 바꿀 이전 텍스트]</strong> </p> <p>바꿀 텍스트를 입력합니다.</p> </li> 
     <li> <p><strong>[!UICONTROL 삽입할 새 텍스트]</strong> </p> <p>새 텍스트를 입력합니다.</p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL 문서 다운로드]

이 작업 모듈은 선택한 문서를 변환하고 다운로드합니다.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td> 
   <td> <p>연결 방법에 대한 지침은 [!DNL Google] 계정 대상 [!DNL Workfront Fusion]를 참조하십시오. <a href="../../workfront-fusion/scenarios/create-a-scenario.md#connect" class="MCXref xref">모듈의 앱 또는 웹 서비스를 [!DNL Workfront Fusion]</a> 기사 <a href="../../workfront-fusion/scenarios/create-a-scenario.md" class="MCXref xref">에서 시나리오 만들기 [!DNL Adobe Workfront Fusion]</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL 드라이브 선택]</td> 
   <td> <p>다운로드할 문서가 있는 드라이브 유형을 선택합니다.</p> 
    <ul> 
     <li> <p><strong>[!UICONTROL My Drive]</strong> </p> <p>다운로드할 문서가 있는 폴더를 선택하고 문서를 선택합니다.</p> </li> 
     <li> <p><strong>[!UICONTROL Shared With Me]</strong> </p> <p>다운로드할 문서가 있는 폴더를 선택하고 문서를 선택합니다.</p> </li> 
     <li> <p><strong>[!UICONTROL [!DNL Google] 공유 드라이브]</strong> (사용 가능) [!DNL G Suite] 사용자만 해당)</p> <p>[!UICONTROL 도메인 관리자 액세스 사용] 여부를 선택합니다. [!UICONTROL Yes]를 선택하면 도메인 관리자로 요청이 발생하고 요청자가 관리자인 모든 공유 드라이브가 반환됩니다.</p> <p>다운로드할 문서가 있는 공유 드라이브를 선택하고 문서를 선택합니다.</p> <p>참고: 을(를) 선택한 경우 [!DNL Google Docs] 이 필드의 옵션 및 사용자가 [!DNL G Suite] user, error <code>[400] Invalid Value</code> 가 반환됩니다.</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Type] </p> </td> 
   <td> <p>다운로드한 문서의 대상 파일 형식을 선택합니다.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL 문서 삭제]

이 작업 모듈은 문서를 삭제합니다.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td> 
   <td> <p>연결 방법에 대한 지침은 [!DNL Google] 계정 대상 [!DNL Workfront Fusion]를 참조하십시오. <a href="../../workfront-fusion/scenarios/create-a-scenario.md#connect" class="MCXref xref">모듈의 앱 또는 웹 서비스를 [!DNL Workfront Fusion]</a> 기사 <a href="../../workfront-fusion/scenarios/create-a-scenario.md" class="MCXref xref">에서 시나리오 만들기 [!DNL Adobe Workfront Fusion]</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL 드라이브 선택]</td> 
   <td> <p>삭제할 문서가 있는 드라이브 유형을 선택합니다.</p> 
    <ul> 
     <li> <p><strong>[!UICONTROL My Drive]</strong> </p> <p>삭제할 문서가 있는 폴더를 선택한 다음 문서를 선택합니다.</p> </li> 
     <li> <p><strong>[!UICONTROL Shared With Me]</strong> </p> <p>삭제할 문서가 있는 폴더를 선택한 다음 문서를 선택합니다.</p> </li> 
     <li> <p><strong>[!UICONTROL [!DNL Google] 공유 드라이브]</strong> (사용 가능) [!DNL G Suite] 사용자만 해당)</p> <p>[!UICONTROL 도메인 관리자 액세스 사용] 여부를 선택합니다. [!UICONTROL Yes]를 선택하면 도메인 관리자로 요청이 발생하고 요청자가 관리자인 모든 공유 드라이브가 반환됩니다.</p> <p>삭제할 문서가 있는 공유 드라이브를 선택하고 문서를 선택합니다.</p> <p>참고: 을(를) 선택한 경우 [!DNL Google Docs] 이 필드의 옵션 및 사용자가 [!DNL G Suite] user, error <code>[400] Invalid Value</code> 가 반환됩니다.</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL 공유 드라이브]</td> 
   <td> <p>다운로드할 문서가 포함된 드라이브를 선택한 다음 문서를 선택합니다. 이 옵션은 선택한 경우 사용할 수 있습니다 [!DNL Google Docs] ([!UICONTROL Choose a Drive] 필드에서)를 클릭합니다.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL 문서 ID]</td> 
   <td> <p> 에서 하나 이상의 이미지를 바꿀 문서를 선택하거나 매핑합니다.</p> </td> 
  </tr> 
 </tbody> 
</table>

### 기타

* [[!UICONTROL API 호출 만들기]](#make-an-api-call)
* [[!UICONTROL 문서의 모든 링크 클릭 가능]](#make-all-links-in-a-document-clickable)

#### [!UICONTROL API 호출 만들기]

이 작업 모듈을 사용하여 사용자 지정 API 호출을 수행할 수 있습니다.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection] </td> 
   <td> <p>연결 방법에 대한 지침은 [!DNL Google] 계정 대상 [!DNL Workfront Fusion]를 참조하십시오. <a href="../../workfront-fusion/scenarios/create-a-scenario.md#connect" class="MCXref xref">모듈의 앱 또는 웹 서비스를 [!DNL Workfront Fusion]</a> 기사 <a href="../../workfront-fusion/scenarios/create-a-scenario.md" class="MCXref xref">에서 시나리오 만들기 [!DNL Adobe Workfront Fusion]</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL URL]</td> 
   <td> <p>상대 경로 입력 <code>https://docs.googleapis.com/</code>. 예: <code>/v1/documents/{presentationID}</code>. </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL 메서드]</td> 
   <td> <p>API 호출을 구성하는 데 필요한 HTTP 요청 메서드를 선택합니다. 자세한 내용은 <a href="../../workfront-fusion/modules/http-request-methods.md" class="MCXref xref">의 HTTP 요청 메서드 [!DNL Adobe Workfront Fusion]</a>.</p> <p> </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Headers]</td> 
   <td> <p>요청의 헤더를 표준 JSON 개체 형태로 추가합니다. 예: <code>{"Content-type":"application/json"}</code>. [!DNL Workfront Fusion] 사용자를 위해 인증 헤더를 추가합니다.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL 쿼리 문자열]</td> 
   <td> <p> 요청 쿼리 문자열을 입력합니다.</p> </td> 
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

**예:** 다음 API 호출은 Google 문서에 지정된 문서에 대한 세부 정보를 검색합니다.

**URL:**

/v1/documents/1ujkf-GDgB0TQSYPrxbCSK4Uso54tHVMqHZEVZZxB6aY

**메서드:**

[!UICONTROL GET]

![](assets/api-call-example.png)

검색된 문서의 세부 사항은 아래의 모듈의 출력에 있습니다 [!UICONTROL 번들] > [!UICONTROL 본문].

![](assets/api-output.png)

#### [!UICONTROL 문서의 모든 링크 클릭 가능]

이 작업 모듈은 문서의 모든 링크를 찾아 클릭 가능하게 합니다.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td> 
   <td> <p>연결 방법에 대한 지침은 [!DNL Google] 계정 대상 [!DNL Workfront Fusion]를 참조하십시오. <a href="../../workfront-fusion/scenarios/create-a-scenario.md#connect" class="MCXref xref">모듈의 앱 또는 웹 서비스를 [!DNL Workfront Fusion]</a> 기사 <a href="../../workfront-fusion/scenarios/create-a-scenario.md" class="MCXref xref">에서 시나리오 만들기 [!DNL Adobe Workfront Fusion]</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL 문서에서 모든 링크 만들기]</p> </td> 
   <td> 
    <ul> 
     <li><strong>[!UICONTROL By Mapping]</strong> <br>문서 템플릿을 매핑하려면 이 옵션을 선택합니다.</li> 
     <li><strong>[!UICONTROL By Dropdown]</strong> <br> 드롭다운 메뉴에서 문서를 선택하려면 이 옵션을 선택합니다.</li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL 드라이브 선택]</td> 
   <td> <p>링크를 클릭할 수 있는 문서가 있는 드라이브 유형을 선택합니다. 이 옵션은 이전 필드에서 [!UICONTROL By Dropdown]을 선택한 경우 사용할 수 있습니다.</p> 
    <ul> 
     <li> <p><strong>[!UICONTROL My Drive]</strong> </p> <p>링크를 클릭할 문서가 있는 폴더를 선택한 다음 문서를 선택합니다.</p> </li> 
     <li> <p><strong>[!UICONTROL Shared With Me]</strong> </p> <p>링크를 클릭할 문서가 있는 폴더를 선택한 다음 문서를 선택합니다.</p> </li> 
     <li> <p><strong>[!UICONTROL [!DNL Google] 공유 드라이브]</strong> (사용 가능) [!DNL G Suite] 사용자만 해당)</p> <p>[!UICONTROL 도메인 관리자 액세스 사용] 여부를 선택합니다. [!UICONTROL Yes]를 선택하면 도메인 관리자로 요청이 발생하고 요청자가 관리자인 모든 공유 드라이브가 반환됩니다.</p> <p>링크를 클릭할 문서가 있는 공유 드라이브를 선택한 다음 문서를 선택합니다.</p> <p>참고: 을(를) 선택한 경우 [!DNL Google Docs] 이 필드의 옵션 및 사용자가 [!DNL G Suite] user, error <code>[400] Invalid Value</code> 가 반환됩니다.</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL 공유 드라이브]</td> 
   <td> <p>링크를 업데이트할 문서가 포함된 드라이브를 선택한 다음 문서를 선택합니다. 이 옵션은 선택한 경우 사용할 수 있습니다 [!DNL Google Docs] ([!UICONTROL Choose a Drive field]에서)</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL 문서 ID]</td> 
   <td> <p> 링크를 업데이트할 문서를 선택하거나 매핑합니다.</p> </td> 
  </tr> 
 </tbody> 
</table>
