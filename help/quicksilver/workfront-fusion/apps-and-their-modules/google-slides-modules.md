---
content-type: reference
product-previous: workfront-fusion
product-area: workfront-integrations;documents
keywords: 커넥터
navigation-topic: apps-and-their-modules
title: Google 슬라이드 모듈
description: Adobe Workfront Fusion Google 슬라이드 모듈을 사용하여 프레젠테이션을 작성, 업데이트, 목록 및/또는 삭제하고 Google 슬라이드 계정의 프레젠테이션에 이미지를 업로드할 수 있습니다.
author: Becky
feature: Workfront Fusion, Digital Content and Documents
exl-id: 680a5328-1d50-4434-beda-7a4670a6e458
source-git-commit: 885d93dd4383945538e977fd3edbfd55bda88b70
workflow-type: tm+mt
source-wordcount: '1575'
ht-degree: 0%

---

# [!DNL Google Slides] 모듈

다음 [!DNL Adobe Workfront Fusion] [!DNL Google Slides] 모듈을 사용하면 프레젠테이션을 만들거나 업데이트하거나 나열하거나 삭제하고 이미지를 프레젠테이션에 업로드할 수 있습니다 [!DNL Google Slides] 계정이 필요합니다.

를 사용하려면 [!DNL Google Slides] with [!DNL Workfront Fusion]를 채울 때는 [!DNL Google] 계정이 필요합니다. 만약 [!DNL Google] 아직 계정을 만들 수 있습니다. [!DNL Google] 계정 도움말 페이지입니다.

또한 [!DNL Google Slides] 다음 위치에서 [!DNL Google Drive].

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

를 사용하려면 [!DNL Google Slides] 모듈이면 반드시 [!DNL Google] 계정이 필요합니다.

## [!DNL Google Slides] 모듈 및 해당 필드

구성 시 [!DNL Google Slides] 모듈, Workfront Fusion에는 아래 나열된 필드가 표시됩니다. 이와 함께 추가 [!DNL Google Slides] 앱이나 서비스에서 액세스 수준과 같은 요소에 따라 필드가 표시될 수 있습니다. 모듈에서 굵게 표시된 제목은 필수 필드를 나타냅니다.

필드 또는 함수 위에 맵 단추가 표시되면 이 단추를 사용하여 해당 필드에 대한 변수와 함수를 설정할 수 있습니다. 자세한 내용은 [의 한 모듈에서 다른 모듈로 정보 매핑 [!DNL Adobe Workfront Fusion]](../../workfront-fusion/mapping/map-information-between-modules.md).

![](assets/map-toggle-350x74.png)

* [프레젠테이션](#presentation)
* [기타](#other)

### 프레젠테이션

* [[!UICONTROL Presentations 보기]](#watch-presentations)
* [[!UICONTROL Presentations 나열]](#list-presentations)
* [[!UICONTROL 프레젠테이션 가져오기]](#get-a-presentation)
* [[!UICONTROL 페이지/축소판 가져오기]](#get-a-pagethumbnail)
* [[!UICONTROL 템플릿에서 프레젠테이션 만들기]](#create-a-presentation-from-a-template)
* [[!UICONTROL 프레젠테이션에 이미지 업로드]](#upload-an-image-to-a-presentation)
* [[!UICONTROL 차트 새로 고침]](#refresh-a-chart)
* [[!UICONTROL 슬라이드 추가/삭제]](#adddelete-a-slide)

#### [!UICONTROL Presentations 보기]

새 프레젠테이션을 만들거나 업데이트할 때 트리거됩니다.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection] </td> 
   <td> <p>연결 방법에 대한 지침은 [!DNL Google Slides] 계정 대상 [!DNL Workfront Fusion]를 참조하십시오. <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">연결 만들기 [!DNL Adobe Workfront Fusion] - 기본 지침</a></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Watch] </td> 
   <td> <p>프레젠테이션을 볼 옵션을 선택합니다.</p> 
    <ul> 
     <li> <p>[!UICONTROL Created Date]</p> </li> 
     <li> <p>[!UICONTROL Modified Date]</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL 제한]</td> 
   <td> <p>한 시나리오 실행 주기 동안 Workfront Fusion의 최대 프레젠테이션 수가 반환되어야 합니다.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Presentations 나열]

모든 프레젠테이션 목록을 검색합니다.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection] </td> 
   <td> <p>연결 방법에 대한 지침은 [!DNL Google Slides] 계정 대상 [!DNL Workfront Fusion]를 참조하십시오. <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">연결 만들기 [!DNL Adobe Workfront Fusion] - 기본 지침</a></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL 드라이브 위치 선택]</td> 
   <td> <p>을(를) 선택합니다 [!DNL Google Drive] 나열할 프레젠테이션의 위치:</p> 
    <ul> 
     <li>[!UICONTROL My Drive]</li> 
     <li>[!UICONTROL Shared With Me]</li> 
     <li>[!UICONTROL [!DNL Google] 공유 드라이브]</li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL 폴더 ID]</td> 
   <td> <p>나열할 프레젠테이션의 폴더 위치를 선택합니다.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL 제한]</td> 
   <td> <p>최대 프레젠테이션 수 [!DNL Workfront Fusion] 한 시나리오 실행 주기 동안 를 반환해야 합니다.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL 프레젠테이션 가져오기]

지정한 프레젠테이션의 최신 버전을 가져옵니다.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection] </td> 
   <td> <p>연결 방법에 대한 지침은 [!DNL Google Slides] 계정 대상 [!DNL Workfront Fusion]를 참조하십시오. <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">연결 만들기 [!DNL Adobe Workfront Fusion] - 기본 지침</a></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL 드라이브 선택]</td> 
   <td> <p>을(를) 선택합니다 [!DNL Google Drive] 나열할 프레젠테이션의 위치:</p> 
    <ul> 
     <li>[!UICONTROL My Drive]</li> 
     <li>[!UICONTROL Shared With Me]</li> 
     <li>[!UICONTROL [!DNL Google] 공유 드라이브]</li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL 프레젠테이션 ID]</td> 
   <td> <p> 검색할 프레젠테이션을 선택합니다.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL 페이지/축소판 가져오기]

지정한 페이지의 최신 버전 또는 프레젠테이션의 페이지 축소판을 가져옵니다.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection] </td> 
   <td> <p>연결 방법에 대한 지침은 [!DNL Google Slides] 계정 대상 [!DNL Workfront Fusion]를 참조하십시오. <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">연결 만들기 [!DNL Adobe Workfront Fusion] - 기본 지침</a></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL 프레젠테이션 ID]</td> 
   <td> <p> 검색할 프레젠테이션 ID를 선택합니다.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Page Object ID]</td> 
   <td> <p> 페이지 개체 세부 정보를 볼 슬라이드를 선택합니다.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL 페이지 축소판 표시]</td> 
   <td> <p> 페이지 축소판 정보를 보려면 확인란을 선택합니다.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL 템플릿에서 프레젠테이션 만들기]

다음과 같은 태그를 모두 변경하여 새 프레젠테이션을 만듭니다. `{{Name}}`, `{{Email}}` 제공된 데이터가 있는 템플릿에서 .

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection] </td> 
   <td> <p>연결 방법에 대한 지침은 [!DNL Google Slides] 계정 대상 [!DNL Workfront Fusion]를 참조하십시오. <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">연결 만들기 [!DNL Adobe Workfront Fusion] - 기본 지침</a></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Title] </td> 
   <td> <p>새 프레젠테이션의 이름을 입력합니다.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL 프레젠테이션 복사]</td> 
   <td> <p> 기존 프레젠테이션을 복사하는 경우 옵션을 선택합니다.</p> 
    <ul> 
     <li>[!UICONTROL By Mapping]</li> 
     <li>[!UICONTROL By Dropdown]</li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL 기존 프레젠테이션 ID 사본]</td> 
   <td> <p> 복사할 기존 프레젠테이션의 경로 또는 프레젠테이션 ID를 입력합니다. 이 필드는 [!UICONTROL By Mapping] 프레젠테이션을 만드는 경우에 나타납니다.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL 드라이브 선택]</td> 
   <td> <p>을(를) 선택합니다 [!DNL Google Drive] 나열할 프레젠테이션의 위치:</p> 
    <ul> 
     <li>[!UICONTROL My Drive]</li> 
     <li>[!UICONTROL Shared With Me]</li> 
     <li>[!UICONTROL [!DNL Google] 공유 드라이브]</li> 
    </ul> <p>이 필드는 [!UICONTROL By Dropdown] 프레젠테이션을 만드는 경우 나타납니다.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL 프레젠테이션 ID]</td> 
   <td> <p> 템플릿으로 사용할 프레젠테이션의 프레젠테이션 ID를 선택합니다.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Values] </td> 
   <td> <p>값을 추가합니다.</p> 
    <ul> 
     <li><strong>[!UICONTROL 태그]</strong>: 프레젠테이션에 바꿀 태그를 입력합니다. For example, <code>&#123;&#123;Name&#125;&#125;</code></li> 
     <li><strong>[!UICONTROL Replaced Value]</strong>: 기존 태그를 바꿀 값을 입력합니다. 예를 들어, 문자열인 경우 <code>&#123;&#123;Name}}</code><code>Sample</code></li></ul></td></tr><tr><td role="rowheader"></td><td><p></p><ul><li></li><li></li><li></li></ul></td></tr><tr><td role="rowheader"><p></p></td><td><p></p></td></tr><tr><td role="rowheader"></td><td><p></p></td></tr><tr><td role="rowheader"></td><td><p></p></td></tr></tbody></table>

#### [!UICONTROL 프레젠테이션에 이미지 업로드]

제공된 데이터로 이미지를 업로드합니다.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection] </td> 
   <td> <p>연결 방법에 대한 지침은 [!DNL Google Slides] 계정 대상 [!DNL Workfront Fusion]를 참조하십시오. <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">연결 만들기 [!DNL Adobe Workfront Fusion] - 기본 지침</a></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL 프레젠테이션 선택]</td> 
   <td> <p>이미지를 업로드할 프레젠테이션을 선택할 방법을 선택합니다.</p> 
    <ul> 
     <li>[!UICONTROL By Mapping]</li> 
     <li>[!DNL By Dropdown]</li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL 드라이브 선택]</td> 
   <td> <p>을(를) 선택합니다 [!DNL Google Drive] 나열할 프레젠테이션의 위치:</p> 
    <ul> 
     <li>[!UICONTROL My Drive]</li> 
     <li>[!UICONTROL Shared With Me]</li> 
     <li>[!UICONTROL [!DNL Google] 공유 드라이브]</li> 
    </ul> <p>이 필드는 [!UICONTROL By Dropdown] 프레젠테이션을 만드는 경우 나타납니다.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL 프레젠테이션 ID]</td> 
   <td> <p> 이미지를 업로드할 프레젠테이션의 프레젠테이션 ID를 선택합니다.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Values]</td> 
   <td> <p>값 값을 추가합니다.</p> 
    <ul> 
     <li><strong>[!UICONTROL 태그]</strong>: URL을 추가할 태그를 입력합니다.</li> 
     <li><strong>[!UICONTROL 이미지 URL]</strong>: 업로드할 이미지의 경로나 URL을 입력합니다.</li> 
    </ul> <p>참고: 이미지는 50MB 미만이어야 하며 25메가픽셀을 초과할 수 없으며 PNG, JPEG 또는 GIF 형식이어야 합니다.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL 차트 새로 고침]

ID로 지정된 프레젠테이션에 저장된 차트 데이터를 새로 고칩니다.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection] </td> 
   <td> <p>연결 방법에 대한 지침은 [!DNL Google Slides] 계정 대상 [!DNL Workfront Fusion]를 참조하십시오. <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">연결 만들기 [!DNL Adobe Workfront Fusion] - 기본 지침</a></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL 드라이브 선택]</td> 
   <td> <p>을(를) 선택합니다 [!DNL Google Drive] 나열할 프레젠테이션의 위치:</p> 
    <ul> 
     <li>[!UICONTROL My Drive]</li> 
     <li>[!UICONTROL Shared With Me]</li> 
     <li>[!UICONTROL [!DNL Google] 공유 드라이브]</li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL 프레젠테이션 ID]</td> 
   <td> <p>새로 고칠 차트가 포함된 프레젠테이션의 프레젠테이션 ID를 선택합니다.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Chart Object ID]</td> 
   <td> <p> 새로 고칠 차트를 선택합니다.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL 슬라이드 추가/삭제]

빈 슬라이드를 만들거나 지정된 프레젠테이션에서 기존 슬라이드를 삭제합니다.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection] </td> 
   <td> <p>연결 방법에 대한 지침은 [!DNL Google Slides] 계정 대상 [!DNL Workfront Fusion]를 참조하십시오. <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">연결 만들기 [!DNL Adobe Workfront Fusion] - 기본 지침</a></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL 메서드 선택]</td> 
   <td> <p>새 슬라이드를 추가할지 아니면 슬라이드를 삭제할지 선택합니다.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!DNL Presentation ID]</td> 
   <td> <p>슬라이드를 추가하거나 삭제할 프레젠테이션의 프레젠테이션 ID를 선택합니다.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL 사전 정의된 레이아웃 유형]</td> 
   <td> <p> 추가한 슬라이드를 사용할 미리 정의된 슬라이드 레이아웃을 선택합니다. 추가 필드(예: [!UICONTROL 제목])에 대한 값을 지정합니다.</p> 
    <ul> 
     <li>[!UICONTROL 자리 표시자가 없는 빈 레이아웃]</li> 
     <li>[!UICONTROL 레이아웃에 캡션이 맨 아래에 있음]</li> 
     <li>제목 및 자막이 있는 [!UICONTROL 레이아웃]</li> 
     <li>[!UICONTROL 레이아웃(제목 및 본문 포함)</li> 
     <li>[!UICONTROL 레이아웃에 제목 및 열 2개]</li> 
     <li>[!UICONTROL 제목 만 있는 레이아웃]</li> 
     <li>[!UICONTROL 레이아웃(섹션 제목 포함)]</li> 
     <li>[!UICONTROL 한 쪽에 제목과 자막이 있고 다른 쪽에는 설명이 있는 레이아웃]</li> 
     <li>[!UICONTROL 하나의 제목과 본문이 단일 열에 정렬되어 있는 레이아웃]</li> 
     <li>[!UICONTROL 기본 점이 있는 레이아웃]</li> 
     <li>[!DNL Layout with a big number heading]</li> 
    </ul> <p>슬라이드를 추가하도록 선택한 경우 이 필드를 사용할 수 있습니다.</p> </td> 
  </tr> 
 </tbody> 
</table>

### 기타

* [[!UICONTROL API 호출 만들기]](#make-an-api-call)
* [[!UICONTROL 프레젠테이션에 링크 삽입]](#insert-links-in-a-presentation)

#### [!UICONTROL API 호출 만들기]

임의 승인된 API 호출을 수행합니다.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection] </td> 
   <td> <p>연결 방법에 대한 지침은 [!DNL Google Slides] 계정 대상 [!DNL Workfront Fusion]를 참조하십시오. <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">연결 만들기 [!DNL Adobe Workfront Fusion] - 기본 지침</a></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL URL]</td> 
   <td> <p>https://developers.google.com/slides/에 상대적인 경로를 입력합니다. 예: 프레젠테이션.</p> <p>사용 가능한 끝점 목록에 대해서는 <a href="https://developers.google.com/slides/reference/rest">[!DNL Google Slides] API 설명서</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL 메서드]</td> 
   <td> <p>API 호출을 구성하는 데 필요한 HTTP 요청 메서드를 선택합니다. 자세한 내용은 <a href="../../workfront-fusion/modules/http-request-methods.md" class="MCXref xref">의 HTTP 요청 메서드 [!DNL Adobe Workfront Fusion]</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Headers]</td> 
   <td> <p>원하는 요청 헤더를 입력합니다. 인증 헤더를 추가할 필요는 없습니다.</p> </td> 
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

>[!INFO]
>
>**예:** API 호출을 사용하여 입력한 프레젠테이션 ID에 대한 프레젠테이션 세부 사항을 가져올 수 있습니다. 에서 프레젠테이션을 열면 URL에서 프레젠테이션 ID를 찾을 수 있습니다. [!DNL Google Slides].
>
>![](assets/api-call-350x13.png)
>
>다음 API 호출은 프레젠테이션 세부 사항을 반환합니다.
>
>![](assets/presentation-details.png)
>
>검색 결과는 아래의 모듈의 출력에 있습니다. [!UICONTROL 번들] > [!UICONTROL 본문] > [!UICONTROL presentationId].
>
>이 예제에서는 요청된 프레젠테이션 세부 정보가 반환되었습니다.
>
>![](assets/presentation-details-2.png)

#### [!UICONTROL 프레젠테이션에 링크 삽입]

이 모듈은 프레젠테이션의 모든 링크를 클릭 가능하게 하거나 일치하는 모든 입력 텍스트에 링크를 삽입합니다.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection] </td> 
   <td> <p>연결 방법에 대한 지침은 [!DNL Google Slides] 계정 대상 [!DNL Workfront Fusion]를 참조하십시오. <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">연결 만들기 [!DNL Adobe Workfront Fusion] - 기본 지침</a></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL 프레젠테이션 선택]</td> 
   <td> <p>이미지를 업로드할 프레젠테이션을 선택할 방법을 선택합니다.</p> 
    <ul> 
     <li>[!UICONTROL By Mapping]</li> 
     <li>[!UICONTROL By Dropdown]</li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL 드라이브 선택]</td> 
   <td> <p>을(를) 선택합니다 [!DNL Google Drive] 나열할 프레젠테이션의 위치:</p> 
    <ul> 
     <li>[!UICONTROL My Drive]</li> 
     <li>[!UICONTROL Shared With Me]</li> 
     <li>[!UICONTROL [!DNL Google] 공유 드라이브]</li> 
    </ul> <p>이 필드는 [!UICONTROL By Dropdown] 프레젠테이션을 만드는 경우 나타납니다.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL 프레젠테이션 ID]</td> 
   <td> <p>나열할 프레젠테이션의 폴더 위치를 선택합니다.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Select]</td> 
   <td> <p>프레젠테이션의 모든 링크를 클릭 가능하게 할지 또는 일치하는 모든 입력 텍스트에 링크를 삽입할지 여부를 선택합니다.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL 텍스트 입력]</td> 
   <td>링크를 추가할 각 텍스트 항목에 대해 항목과 연결된 링크를 목록에 추가합니다. 항목이 프레젠테이션에 나타날 때마다 지정된 사이트에 자동으로 연결됩니다.</td> 
  </tr> 
 </tbody> 
</table>
