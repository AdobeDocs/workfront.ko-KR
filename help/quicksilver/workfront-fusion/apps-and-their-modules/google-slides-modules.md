---
content-type: reference
product-previous: workfront-fusion
product-area: workfront-integrations;documents
keywords: 커넥터
navigation-topic: apps-and-their-modules
title: Google 슬라이드 모듈
description: Adobe Workfront Fusion Google 슬라이드 모듈을 사용하면 프레젠테이션을 생성, 업데이트, 나열 및/또는 삭제하고 이미지를 Google 슬라이드 계정의 프레젠테이션에 업로드할 수 있습니다.
author: Becky
feature: Workfront Fusion, Digital Content and Documents
exl-id: 680a5328-1d50-4434-beda-7a4670a6e458
source-git-commit: 0915dcce45b271ee18cdd8af5db4f0eb01f3cced
workflow-type: tm+mt
source-wordcount: '1623'
ht-degree: 0%

---

# [!DNL Google Slides] 모듈

다음 [!DNL Adobe Workfront Fusion] [!DNL Google Slides] 모듈을 사용하면 프레젠테이션을 생성, 업데이트, 나열 및/또는 삭제하고 이미지를 의 프레젠테이션에 업로드할 수 있습니다. [!DNL Google Slides] 계정입니다.

를 사용하려면 [!DNL Google Slides] 포함 [!DNL Workfront Fusion], 다음을 보유해야 합니다. [!DNL Google] 계정입니다. A가 없다면 [!DNL Google] 아직 다음 위치에서 계정을 만들 수 있습니다. [!DNL Google] 계정 도움말 페이지

필요한 사항 [!DNL Google Slides] (으)로 [!DNL Google Drive].

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

사용 [!DNL Google Slides] 모듈, 다음이 있어야 합니다. [!DNL Google] 계정입니다.

## [!DNL Google Slides] 모듈 및 해당 필드

를 구성할 때 [!DNL Google Slides] 모듈 Workfront Fusion에는 아래 나열된 필드가 표시됩니다. 이와 함께 추가 [!DNL Google Slides] 앱이나 서비스의 액세스 수준 등에 따라 필드가 표시될 수 있습니다. 모듈의 굵은 제목은 필수 필드를 나타냅니다.

필드나 함수 위에 맵 단추가 표시되면 이 단추를 사용하여 해당 필드에 대한 변수와 함수를 설정할 수 있습니다. 자세한 내용은 [의 한 모듈에서 다른 모듈로 정보 매핑 [!DNL Adobe Workfront Fusion]](../../workfront-fusion/mapping/map-information-between-modules.md).

![](assets/map-toggle-350x74.png)

* [프레젠테이션](#presentation)
* [기타](#other)

### 프레젠테이션

* [[!UICONTROL Presentations 시청]](#watch-presentations)
* [[!UICONTROL 목록 Presentations]](#list-presentations)
* [[!UICONTROL 프레젠테이션 받기]](#get-a-presentation)
* [[!UICONTROL 페이지/썸네일 가져오기]](#get-a-pagethumbnail)
* [[!UICONTROL 템플릿에서 프레젠테이션 만들기]](#create-a-presentation-from-a-template)
* [[!UICONTROL 프레젠테이션에 이미지 업로드]](#upload-an-image-to-a-presentation)
* [[!UICONTROL 차트 새로 고침]](#refresh-a-chart)
* [[!UICONTROL 슬라이드 추가/삭제]](#adddelete-a-slide)

#### [!UICONTROL Presentations 시청]

새 프레젠테이션을 만들거나 업데이트할 때 트리거됩니다.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection] </td> 
   <td> <p>연결에 대한 자세한 내용 [!DNL Google Slides] 계정 위치: [!DNL Workfront Fusion], 참조 <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">에 대한 연결 만들기 [!DNL Adobe Workfront Fusion] - 기본 지침</a></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Watch] </td> 
   <td> <p>프레젠테이션을 시청하려면 다음 옵션을 선택합니다.</p> 
    <ul> 
     <li> <p>[!UICONTROL 만든 날짜]</p> </li> 
     <li> <p>[!UICONTROL 수정 날짜]</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL 제한]</td> 
   <td> <p>한 시나리오 실행 주기 동안 Workfront Fusion이 반환해야 하는 최대 프레젠테이션 수입니다.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL 목록 Presentations]

모든 프레젠테이션 목록을 검색합니다.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection] </td> 
   <td> <p>연결에 대한 자세한 내용 [!DNL Google Slides] 계정 위치: [!DNL Workfront Fusion], 참조 <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">에 대한 연결 만들기 [!DNL Adobe Workfront Fusion] - 기본 지침</a></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL 드라이브 위치 선택]</td> 
   <td> <p>다음 항목 선택 [!DNL Google Drive] 나열할 프레젠테이션이 있는 위치:</p> 
    <ul> 
     <li>[!UICONTROL 내 드라이브]</li> 
     <li>[!UICONTROL 나와 공유됨]</li> 
     <li>[!UICONTROL [!DNL Google] 공유 드라이브]</li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL 폴더 ID]</td> 
   <td> <p>나열할 프레젠테이션의 폴더 위치를 선택합니다.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL 제한]</td> 
   <td> <p>최대 프레젠테이션 수 [!DNL Workfront Fusion] 한 시나리오 실행 주기 중에 를 반환해야 합니다.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL 프레젠테이션 받기]

지정된 프레젠테이션의 최신 버전을 가져옵니다.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection] </td> 
   <td> <p>연결에 대한 자세한 내용 [!DNL Google Slides] 계정 위치: [!DNL Workfront Fusion], 참조 <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">에 대한 연결 만들기 [!DNL Adobe Workfront Fusion] - 기본 지침</a></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL 드라이브 선택]</td> 
   <td> <p>다음 항목 선택 [!DNL Google Drive] 나열할 프레젠테이션이 있는 위치:</p> 
    <ul> 
     <li>[!UICONTROL 내 드라이브]</li> 
     <li>[!UICONTROL 나와 공유됨]</li> 
     <li>[!UICONTROL [!DNL Google] 공유 드라이브]</li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL 프레젠테이션 ID]</td> 
   <td> <p> 검색할 프레젠테이션을 선택합니다.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL 페이지/썸네일 가져오기]

프레젠테이션에 있는 페이지의 축소판 또는 지정된 페이지의 최신 버전을 가져옵니다.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection] </td> 
   <td> <p>연결에 대한 자세한 내용 [!DNL Google Slides] 계정 위치: [!DNL Workfront Fusion], 참조 <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">에 대한 연결 만들기 [!DNL Adobe Workfront Fusion] - 기본 지침</a></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL 프레젠테이션 ID]</td> 
   <td> <p> 검색할 프레젠테이션 ID를 선택합니다.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL 페이지 개체 ID]</td> 
   <td> <p> 페이지 개체 세부 사항을 보려는 슬라이드를 선택합니다.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL 페이지 썸네일 표시]</td> 
   <td> <p> 페이지 썸네일 정보를 보려면 확인란을 선택합니다.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL 템플릿에서 프레젠테이션 만들기]

다음과 같은 태그를 모두 교체하여 새 프레젠테이션을 만듭니다. `{{Name}}`, `{{Email}}` 제공된 데이터가 있는 템플릿에서

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection] </td> 
   <td> <p>연결에 대한 자세한 내용 [!DNL Google Slides] 계정 위치: [!DNL Workfront Fusion], 참조 <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">에 대한 연결 만들기 [!DNL Adobe Workfront Fusion] - 기본 지침</a></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Title] </td> 
   <td> <p>새 프레젠테이션의 이름을 입력하십시오.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL 프레젠테이션 복사]</td> 
   <td> <p> 기존 프레젠테이션을 복사하는 경우 다음 옵션을 선택합니다.</p> 
    <ul> 
     <li>[!UICONTROL By Mapping]</li> 
     <li>[!UICONTROL By Dropdown]</li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL 기존 프레젠테이션 ID 사본]</td> 
   <td> <p> 복사할 기존 프레젠테이션의 경로 또는 프레젠테이션 ID를 입력합니다. [!UICONTROL By Mapping] 프레젠테이션을 만드는 경우 이 필드가 나타납니다.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL 드라이브 선택]</td> 
   <td> <p>다음 항목 선택 [!DNL Google Drive] 나열할 프레젠테이션이 있는 위치:</p> 
    <ul> 
     <li>[!UICONTROL 내 드라이브]</li> 
     <li>[!UICONTROL 나와 공유됨]</li> 
     <li>[!UICONTROL [!DNL Google] 공유 드라이브]</li> 
    </ul> <p>[!UICONTROL By Dropdown] 프레젠테이션을 만드는 경우 이 필드가 나타납니다.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL 프레젠테이션 ID]</td> 
   <td> <p> 템플릿으로 사용할 프레젠테이션의 프레젠테이션 ID를 선택합니다.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL 값] </td> 
   <td> <p>값을 추가합니다.</p> 
    <ul> 
     <li><strong>[!UICONTROL 태그]</strong>: 프레젠테이션에서 바꿀 태그를 입력합니다. For example, <code>&#123;&#123;Name&#125;&#125;</code></li> 
     <li><strong>[!UICONTROL Replaced Value]</strong>: 기존 태그를 대체할 값을 입력합니다. 예를 들어 문자열을 나타내는 경우 <tr><ul><tr><tr><tr><code>&#123;&#123;Name&#125;&#125;/code> in the presentation and the replaced value is Sample, then the <code>&#123;&#123;Name}}</code> will be replaced by <code>Sample</code>.</li> 
    </ul> </td> 
  </tr> 
   
   <td role="rowheader">[!UICONTROL New Drive Location]</td> 
   <td> <p>Select the [!DNL Google Drive] where you want to store or add the new presentation:</p> 
     
     <li>[!UICONTROL My Drive]</li> 
     <li>[!UICONTROL Shared With Me]</li> 
     <li>[!UICONTROL [!DNL Google] Shared Drive]</li> 
    </ul> </td> 
  </tr> 
   
   <td role="rowheader"> <p>[!UICONTROL New Document's Location]</p> </td> 
   <td> <p>Select the folder where you want to store or add the presentation.</p> </td> 
  </tr> 
   
   <td role="rowheader">[!UICONTROL Shared] </td> 
   <td> <p>Select if you want to share the presentation.</p> </td> 
  </tr> 
   
   <td role="rowheader">[!UICONTROL Sharing with Other's Email Address]</td> 
   <td> <p> Enter the email address with whom you want to share the presentation. If you are not entering an email address and selecting only shared field, the presentation is shareable to anyone.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL 프레젠테이션에 이미지 업로드]

제공된 데이터가 있는 이미지를 업로드합니다.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection] </td> 
   <td> <p>연결에 대한 자세한 내용 [!DNL Google Slides] 계정 위치: [!DNL Workfront Fusion], 참조 <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">에 대한 연결 만들기 [!DNL Adobe Workfront Fusion] - 기본 지침</a></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL 프레젠테이션 선택]</td> 
   <td> <p>이미지를 업로드할 프레젠테이션을 선택할 방법을 선택하십시오.</p> 
    <ul> 
     <li>[!UICONTROL By Mapping]</li> 
     <li>[!DNL By Dropdown]</li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL 드라이브 선택]</td> 
   <td> <p>다음 항목 선택 [!DNL Google Drive] 나열할 프레젠테이션이 있는 위치:</p> 
    <ul> 
     <li>[!UICONTROL 내 드라이브]</li> 
     <li>[!UICONTROL 나와 공유됨]</li> 
     <li>[!UICONTROL [!DNL Google] 공유 드라이브]</li> 
    </ul> <p>[!UICONTROL By Dropdown] 프레젠테이션을 만드는 경우 이 필드가 나타납니다.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL 프레젠테이션 ID]</td> 
   <td> <p> 이미지를 업로드할 프레젠테이션의 프레젠테이션 ID를 선택합니다.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL 값]</td> 
   <td> <p>값 값을 추가합니다.</p> 
    <ul> 
     <li><strong>[!UICONTROL 태그]</strong>: URL을 추가할 태그를 입력합니다.</li> 
     <li><strong>[!UICONTROL 이미지 URL]</strong>: 업로드할 이미지의 경로 또는 URL을 입력합니다.</li> 
    </ul> <p>참고: 이미지 크기는 50MB 미만이어야 하고, 2,500만 픽셀을 초과할 수 없으며, PNG, JPEG 또는 GIF 형식이어야 합니다.</p> </td> 
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
   <td> <p>연결에 대한 자세한 내용 [!DNL Google Slides] 계정 위치: [!DNL Workfront Fusion], 참조 <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">에 대한 연결 만들기 [!DNL Adobe Workfront Fusion] - 기본 지침</a></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL 드라이브 선택]</td> 
   <td> <p>다음 항목 선택 [!DNL Google Drive] 나열할 프레젠테이션이 있는 위치:</p> 
    <ul> 
     <li>[!UICONTROL 내 드라이브]</li> 
     <li>[!UICONTROL 나와 공유됨]</li> 
     <li>[!UICONTROL [!DNL Google] 공유 드라이브]</li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL 프레젠테이션 ID]</td> 
   <td> <p>새로 고침할 차트가 포함된 프레젠테이션의 프레젠테이션 ID를 선택합니다.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL 차트 개체 ID]</td> 
   <td> <p> 새로 고침할 차트를 선택합니다.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL 슬라이드 추가/삭제]

지정한 프레젠테이션에서 빈 슬라이드를 만들거나 기존 슬라이드를 삭제합니다.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection] </td> 
   <td> <p>연결에 대한 자세한 내용 [!DNL Google Slides] 계정 위치: [!DNL Workfront Fusion], 참조 <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">에 대한 연결 만들기 [!DNL Adobe Workfront Fusion] - 기본 지침</a></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL 메서드 선택]</td> 
   <td> <p>새 슬라이드를 추가할지 또는 슬라이드를 삭제할지 선택합니다.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!DNL Presentation ID]</td> 
   <td> <p>슬라이드를 추가하거나 삭제할 프레젠테이션의 프레젠테이션 ID를 선택합니다.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL 사전 정의된 레이아웃 유형]</td> 
   <td> <p> 추가된 슬라이드에서 사용할 미리 정의된 슬라이드 레이아웃을 선택합니다. 추가 필드(예: [!UICONTROL Title])에 대한 값을 지정하십시오.</p> 
    <ul> 
     <li>[!UICONTROL 자리 표시자 없는 빈 레이아웃]</li> 
     <li>맨 아래에 캡션이 있는 [!UICONTROL 레이아웃]</li> 
     <li>제목 및 부제가 있는 [!UICONTROL 레이아웃]</li> 
     <li>제목 및 본문이 있는 [!UICONTROL 레이아웃]</li> 
     <li>제목과 두 개의 열이 있는 [!UICONTROL 레이아웃]</li> 
     <li>제목만 있는 [!UICONTROL 레이아웃]</li> 
     <li>섹션 제목이 있는 [!UICONTROL 레이아웃]</li> 
     <li>한쪽에는 제목과 부제가 있고 다른 한쪽에는 설명이 있는 [!UICONTROL 레이아웃]</li> 
     <li>한 개의 제목과 한 개의 본문이 있는 [!UICONTROL 레이아웃이 단일 열로 정렬됨]</li> 
     <li>[!UICONTROL 레이아웃(주 지점 포함)]</li> 
     <li>[!DNL Layout with a big number heading]</li> 
    </ul> <p>이 필드는 슬라이드를 추가하도록 선택한 경우 사용할 수 있습니다.</p> </td> 
  </tr> 
 </tbody> 
</table>

### 기타

* [[!UICONTROL API 호출 만들기]](#make-an-api-call)
* [[!UICONTROL 프레젠테이션에 링크 삽입]](#insert-links-in-a-presentation)

#### [!UICONTROL API 호출 만들기]

임의의 승인된 API 호출을 수행합니다.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection] </td> 
   <td> <p>연결에 대한 자세한 내용 [!DNL Google Slides] 계정 위치: [!DNL Workfront Fusion], 참조 <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">에 대한 연결 만들기 [!DNL Adobe Workfront Fusion] - 기본 지침</a></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL URL]</td> 
   <td> <p>https://developers.google.com/slides/에 상대적인 경로를 입력합니다. 예: 프레젠테이션</p> <p>사용 가능한 엔드포인트 목록은 <a href="https://developers.google.com/slides/reference/rest">[!DNL Google Slides] API 설명서</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL 메서드]</td> 
   <td> <p>API 호출을 구성하는 데 필요한 HTTP 요청 메서드를 선택합니다. 자세한 내용은 <a href="../../workfront-fusion/modules/http-request-methods.md" class="MCXref xref">의 HTTP 요청 메서드 [!DNL Adobe Workfront Fusion]</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Headers]</td> 
   <td> <p>원하는 요청 헤더를 입력합니다. 인증 헤더를 추가할 필요가 없습니다.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL 쿼리 문자열]</td> 
   <td> <p> 요청 쿼리 문자열을 입력합니다.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Body]</td> 
   <td> <p>표준 JSON 개체의 형태로 API 호출에 대한 본문 콘텐츠를 추가합니다.</p> <p>참고:  <p>다음과 같은 조건문을 사용할 때 <code>if</code> json에서 따옴표를 조건문 외부에 넣습니다.</p> 
     <div class="example" data-mc-autonum="<b>Example: </b>"> 
      <p> <img src="assets/quotes-in-json-350x120.png" style="width: 350;height: 120;"> </p> 
     </div> </p> </td> 
  </tr> 
 </tbody> 
</table>

>[!INFO]
>
>**예:** API 호출을 사용하여 입력한 프레젠테이션 ID에 대한 프레젠테이션 세부 사항을 가져올 수 있습니다. 에서 프레젠테이션을 열면 URL에서 프레젠테이션 ID를 찾을 수 있습니다 [!DNL Google Slides].
>
>![](assets/api-call-350x13.png)
>
>다음 API 호출은 프레젠테이션 세부 정보를 반환합니다.
>
>![](assets/presentation-details.png)
>
>검색 일치 항목은 아래의 모듈 출력에서 찾을 수 있습니다. [!UICONTROL 번들] > [!UICONTROL 본문] > [!UICONTROL presentationId].
>
>이 예제에서 요청된 프레젠테이션 세부 사항이 반환되었습니다.
>
>![](assets/presentation-details-2.png)

#### [!UICONTROL 프레젠테이션에 링크 삽입]

이 모듈은 프레젠테이션의 모든 링크를 클릭 가능으로 만들거나 일치하는 모든 입력 텍스트에 링크를 삽입합니다.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection] </td> 
   <td> <p>연결에 대한 자세한 내용 [!DNL Google Slides] 계정 위치: [!DNL Workfront Fusion], 참조 <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">에 대한 연결 만들기 [!DNL Adobe Workfront Fusion] - 기본 지침</a></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL 프레젠테이션 선택]</td> 
   <td> <p>이미지를 업로드할 프레젠테이션을 선택할 방법을 선택하십시오.</p> 
    <ul> 
     <li>[!UICONTROL By Mapping]</li> 
     <li>[!UICONTROL By Dropdown]</li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL 드라이브 선택]</td> 
   <td> <p>다음 항목 선택 [!DNL Google Drive] 나열할 프레젠테이션이 있는 위치:</p> 
    <ul> 
     <li>[!UICONTROL 내 드라이브]</li> 
     <li>[!UICONTROL 나와 공유됨]</li> 
     <li>[!UICONTROL [!DNL Google] 공유 드라이브]</li> 
    </ul> <p>[!UICONTROL By Dropdown] 프레젠테이션을 만드는 경우 이 필드가 나타납니다.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL 프레젠테이션 ID]</td> 
   <td> <p>나열할 프레젠테이션의 폴더 위치를 선택합니다.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Select]</td> 
   <td> <p>프레젠테이션의 모든 링크를 클릭할 수 있도록 할지, 모든 일치 입력 텍스트에 링크를 삽입할지 여부를 선택합니다.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL 텍스트 입력]</td> 
   <td>링크를 추가할 각 텍스트 항목에 대해 항목과 관련 링크를 목록에 추가합니다. 항목이 프레젠테이션에 나타날 때마다 지정된 사이트에 자동으로 연결됩니다.</td> 
  </tr> 
 </tbody> 
</table>
