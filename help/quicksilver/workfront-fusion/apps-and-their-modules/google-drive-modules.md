---
content-type: reference
product-previous: workfront-fusion
product-area: workfront-integrations;documents
keywords: 커넥터
navigation-topic: apps-and-their-modules
title: Google 드라이브 모듈
description: 다음 [!DNL Adobe Workfront Fusion Google Drive] 모듈을 사용하면 파일, 폴더 또는 공유 드라이브를 모니터링, 검색, 생성, 업데이트, 삭제 및 관리할 수 있습니다 [!DNL Google Drive].
author: Becky
feature: Workfront Fusion, Digital Content and Documents
exl-id: 7d620c93-d1bf-4451-9f76-1d6fd850cec9
source-git-commit: 885d93dd4383945538e977fd3edbfd55bda88b70
workflow-type: tm+mt
source-wordcount: '2908'
ht-degree: 0%

---

# [!DNL Google Drive] 모듈

다음 [!DNL Adobe Workfront Fusion] [!DNL Google Drive] 모듈을 사용하면 파일, 폴더 또는 공유 드라이브를 모니터링, 검색, 생성, 업데이트, 삭제 및 관리할 수 있습니다 [!DNL Google Drive].

다음 [!DNL Adobe Workfront Fusion] 시나리오, [!DNL Google Drive] 여러 타사 애플리케이션 및 서비스에 계정을 설정합니다.

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



## 연결 중 [!DNL Google Drive] to [!DNL Workfront Fusion]

만약 [!DNL @gmail.com] 또는 [!DNL @googlemail.com] 사용자가 OAuth 클라이언트를 만들어야 합니다. [a [!DNL Google Cloud Platform]](https://console.developers.google.com/projectselector2/apis/dashboard?supportedpurview=project) 얻기 위해서 [!UICONTROL 클라이언트 ID] 및 [!UICONTROL 클라이언트 암호].

OAuth 클라이언트를 만들고 가져오는 방법에 대한 단계별 지침입니다 [!UICONTROL 클라이언트 ID] 및 [!UICONTROL 클라이언트 암호]). [Connect [!DNL Adobe Workfront Fusion] to [!DNL Google Services] 사용자 지정 OAuth 클라이언트 사용](../../workfront-fusion/connections/connect-fusion-to-google-using-oauth.md).

연결 방법에 대한 지침은 [!DNL Google Drive] 계정 대상 [!UICONTROL Workfront Fusion]를 참조하십시오. [연결 만들기 [!UICONTROL Adobe Workfront Fusion] - 기본 지침](../../workfront-fusion/connections/connect-to-fusion-general.md)

## [!DNL Google Drive] 모듈 및 해당 필드

구성 시 [!DNL Google Drive] 모듈, [!DNL Workfront Fusion] 아래 나열된 필드를 표시합니다. 이와 함께 추가 [!DNL Google Drive] 앱이나 서비스에서 액세스 수준과 같은 요소에 따라 필드가 표시될 수 있습니다. 모듈에서 굵게 표시된 제목은 필수 필드를 나타냅니다.

필드 또는 함수 위에 맵 단추가 표시되면 이 단추를 사용하여 해당 필드에 대한 변수와 함수를 설정할 수 있습니다. 자세한 내용은 [의 한 모듈에서 다른 모듈로 정보 매핑 [!DNL Adobe Workfront Fusion]](../../workfront-fusion/mapping/map-information-between-modules.md).

![](assets/map-toggle-350x74.png)



* [Triggers](#triggers)
* [액션](#actions)

### Triggers

* [[!UICONTROL 폴더에서 파일 보기]](#watch-files-in-folder)
* [[!UICONTROL 모든 파일 보기]](#watch-all-files)
* [[!UICONTROL 공유 파일 보기]](#watch-shared-files)
* [[!UICONTROL 댓글 보기]](#watch-comments)

#### [!UICONTROL 폴더에서 파일 보기]

지정된 폴더에서 파일을 추가하거나 수정할 때 파일 세부 사항을 검색합니다.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
    <td>[!UICONTROL Connection] </td>
   <td> <p>연결 방법에 대한 지침은 [!DNL Google Drive] 계정 대상 [!DNL Workfront Fusion]를 참조하십시오. <a href="#connecting-google-drive-to-workfront-fusion" class="MCXref xref">연결 중 [!DNL Google Drive] [!UICONTROL Workfront Fusion] 변환</a></p> </td> 
  </tr> 
  <tr>
    <td>[!UICONTROL 모니터링할 폴더 선택]</td>
    <td >드라이브에서 파일을 볼 폴더를 선택합니다.</td>
  </tr> 
  <tr> 
    <td>[!UICONTROL 감시할 파일]</td>
   <td> <p>보려는 파일 유형을 선택합니다.</p> 
    <ul> 
     <li>[!UICONTROL All]</li> 
     <li>[!DNL Google Documents]</li> 
     <li>[!DNL Google Spreadsheets]</li> 
     <li>[!DNL Google Slides]</li> 
     <li>[!DNL Google Drawings]</li> 
    </ul> </td> 
  </tr> 
  <tr> 
    <td >[!UICONTROL Convert [!DNL Google Documents] 파일 형식]</td>
    <td>변환할 파일 형식을 선택합니다 [!DNL Google Documents] 대상.</td>
  </tr> 
  <tr>
    <td>[!UICONTROL Convert [!DNL Google Spreadsheets] 파일 형식]</td>
    <td>변환할 파일 형식을 선택합니다 [!DNL Google Spreadsheets] 대상.</td>
  </tr> 
  <tr>
    <td>[!UICONTROL Convert [!DNL Google Slides] 파일 형식]</td>
    <td>변환할 파일 형식을 선택합니다 [!DNL Google Slides] 대상.</td>
  </tr> 
  <tr>
    <td>[!UICONTROL Convert [!DNL Google Drawings] 파일 형식]</td>
    <td>변환할 파일 형식을 선택합니다 [!DNL Google Drawings] 대상.</td>
  </tr> 
  <tr>
    <td>[!UICONTROL Watch]</td>
    <td>새 파일 및 모든 변경 내용을 감시할지 아니면 새 파일만 감시할지를 선택합니다.</td>
  </tr> 
  <tr> 
    <td>[!UICONTROL 다운로드한 최대 파일 수]</td>
    <td>최대 결과 수 설정 [!DNL Workfront Fusion] 한 주기 동안 다운로드됩니다(시나리오 실행당 반복 횟수).</td>
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL 모든 파일 보기]

파일에 있을 때 파일 세부 사항을 검색합니다. [!DNL Google Drive] 가 추가되거나 수정됩니다.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL Connection] </td> 
   <td> <p>연결 방법에 대한 지침은 [!DNL Google Drive] 계정 대상 [!DNL Workfront Fusion]를 참조하십시오. <a href="#connecting-google-drive-to-workfront-fusion" class="MCXref xref">연결 중 [!DNL Google Drive] [!UICONTROL Workfront Fusion] 변환</a></p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL 감시할 파일]</td> 
   <td> <p>보려는 파일 유형을 선택합니다.</p> 
    <ul> 
     <li>[!UICONTROL All]</li> 
     <li>[!DNL Google Documents]</li> 
     <li>[!DNL Google Spreadsheets]</li> 
     <li>[!DNL Google Slides]</li> 
     <li>[!DNL Google Drawings]</li> 
    </ul> </td> 
  </tr> 
  <tr> 
    <td >[!UICONTROL Convert [!DNL Google Documents] 파일 형식]</td>
    <td>변환할 파일 형식을 선택합니다 [!DNL Google Documents] 대상.</td>
  </tr> 
  <tr>
    <td>[!UICONTROL Convert [!DNL Google Spreadsheets] 파일 형식]</td>
    <td>변환할 파일 형식을 선택합니다 [!DNL Google Spreadsheets] 대상.</td>
  </tr> 
  <tr>
    <td>[!UICONTROL Convert [!DNL Google Slides] 파일 형식]</td>
    <td>변환할 파일 형식을 선택합니다 [!DNL Google Slides] 대상.</td>
  </tr> 
  <tr>
    <td>[!UICONTROL Convert [!DNL Google Drawings] 파일 형식]</td>
    <td>변환할 파일 형식을 선택합니다 [!DNL Google Drawings] 대상.</td>
  </tr>  
  <tr> 
   <td>[!UICONTROL Watch]</td> 
   <td>새 파일 및 모든 변경 내용을 감시할지 아니면 새 파일만 감시할지를 선택합니다.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL 다운로드한 최대 파일 수]</td> 
   <td>최대 결과 수 설정 [!DNL Workfront Fusion] 한 주기 동안 다운로드됩니다(시나리오 실행당 반복 횟수).</td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL 공유 파일 보기]

새 파일을 공유하거나 기존 공유 파일이 업데이트될 때 트리거됩니다.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL Connection] </td> 
   <td> <p>연결 방법에 대한 지침은 [!DNL Google Drive] 계정 대상 [!DNL Workfront Fusion]를 참조하십시오. <a href="#connecting-google-drive-to-workfront-fusion" class="MCXref xref">연결 중 [!DNL Google Drive] [!UICONTROL Workfront Fusion] 변환</a></p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL 모니터링할 폴더 선택]</td> 
   <td>에서 파일을 볼 공유 폴더를 선택합니다.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL 감시할 파일]</td> 
   <td> <p>보려는 파일 유형을 선택합니다.</p> 
    <ul> 
     <li>[!UICONTROL All]</li> 
     <li>[!DNL Google Documents]</li> 
     <li>[!DNL Google Spreadsheets]</li> 
     <li>[!DNL Google Slides]</li> 
     <li>[!DNL Google Drawings]</li> 
    </ul> </td> 
  </tr> 
  <tr> 
    <td >[!UICONTROL Convert [!DNL Google Documents] 파일 형식]</td>
    <td>변환할 파일 형식을 선택합니다 [!DNL Google Documents] 대상.</td>
  </tr> 
  <tr>
    <td>[!UICONTROL Convert [!DNL Google Spreadsheets] 파일 형식]</td>
    <td>변환할 파일 형식을 선택합니다 [!DNL Google Spreadsheets] 대상.</td>
  </tr> 
  <tr>
    <td>[!UICONTROL Convert [!DNL Google Slides] 파일 형식]</td>
    <td>변환할 파일 형식을 선택합니다 [!DNL Google Slides] 대상.</td>
  </tr> 
  <tr>
    <td>[!UICONTROL Convert [!DNL Google Drawings] 파일 형식]</td>
    <td>변환할 파일 형식을 선택합니다 [!DNL Google Drawings] 대상.</td>
  </tr> 
  <tr> 
   <td>[!UICONTROL Watch]</td> 
   <td>새 파일 및 모든 변경 내용을 감시할지 아니면 새 파일만 감시할지를 선택합니다.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL 다운로드한 최대 파일 수]</td> 
   <td>최대 결과 수 설정 [!DNL Workfront Fusion] 한 주기 동안 다운로드됩니다(시나리오 실행당 반복 횟수).</td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL 댓글 보기]

선택한 파일에서 주석이 추가 또는 수정될 때 트리거됩니다.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL Connection] </td> 
   <td> <p>연결 방법에 대한 지침은 [!DNL Google Drive] 계정 대상 [!DNL Workfront Fusion]를 참조하십시오. <a href="#connecting-google-drive-to-workfront-fusion" class="MCXref xref">연결 중 [!DNL Google Drive] [!UICONTROL Workfront Fusion] 변환</a></p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL File]</td> 
   <td>메모를 확인할 파일을 선택합니다.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Watch]</td> 
   <td>모든 변경 사항을 감시할지 아니면 새 주석만 감시할지 선택합니다</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL 반환된 최대 주석 수]</td> 
   <td>최대 주석 수 설정 [!DNL Workfront Fusion] 한 주기 동안(시나리오 실행당 반복 횟수)가 반환됩니다.</td> 
  </tr> 
 </tbody> 
</table>

### 액션

* [[!UICONTROL 파일 업로드]](#upload-a-file)
* [[!UICONTROL 파일 업데이트]](#update-a-file)
* [[!UICONTROL 파일 복사]](#copy-a-file)
* [[!UICONTROL 파일 삭제]](#delete-a-file)
* [[!UICONTROL 파일/폴더를 휴지통으로 이동]](#move-a-filefolder-to-trash)
* [[!UICONTROL 파일 가져오기]](#get-a-file)
* [[!UICONTROL 파일/폴더 검색]](#search-for-filesfolders)
* [[!UICONTROL 폴더 만들기]](#create-a-folder)
* [[!UICONTROL 공유 링크 가져오기]](#get-a-share-link)

#### [!UICONTROL 파일 업로드]

파일에 업로드 [!DNL Google Drive].

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL Connection] </td> 
   <td> <p>연결 방법에 대한 지침은 [!DNL Google Drive] 계정 대상 [!DNL Workfront Fusion]를 참조하십시오. <a href="#connecting-google-drive-to-workfront-fusion" class="MCXref xref">연결 중 [!DNL Google Drive] [!UICONTROL Workfront Fusion] 변환</a></p> </td> 
  </tr> 
  <tr> 
   <td>[!DNL Destination]</td> 
   <td> <p>파일을 업로드할 대상을 선택합니다.</p> 
    <ul> 
     <li>[!DNL My Drive]</li> 
     <li>[!DNL Shared with Me]</li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Target 폴더]</td> 
   <td>파일을 업로드할 폴더를 선택합니다. </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL 소스 파일]</td> 
   <td>이전 모듈에서 전달된 파일을 사용할지, 수동으로 매핑할지 여부를 선택합니다.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL 파일 이름]</td> 
   <td>파일 이름을 선택합니다. [!UICONTROL source file] 필드에서 "[!UICONTROL Map]"을 선택하면 이 옵션을 사용할 수 있습니다.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Data]</td> 
   <td>업로드할 데이터 파일을 선택합니다. [!UICONTROL source file] 필드에서 "[!UICONTROL Map]"을 선택하면 이 옵션을 사용할 수 있습니다.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Title]</td> 
   <td>새 파일의 제목을 입력합니다.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL 파일 변환]</td> 
   <td>이 옵션을 활성화하면 모듈에서 파일을 해당 페이지로 변환할 수 있습니다 [!DNL Google] 형식 지정</td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL 파일 업데이트]

파일의 메타데이터 또는 콘텐츠를 업데이트합니다.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL Connection] </td> 
   <td> <p>연결 방법에 대한 지침은 [!DNL Google Drive] 계정 대상 [!DNL Workfront Fusion]를 참조하십시오. <a href="#connecting-google-drive-to-workfront-fusion" class="MCXref xref">연결 중 [!DNL Google Drive] [!UICONTROL Workfront Fusion] 변환</a></p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL 대상]</td> 
   <td> <p>파일을 업로드할 대상을 선택합니다.</p> 
    <ul> 
     <li>[!UICONTROL My Drive]</li> 
     <li>[!UICONTROL Shared with Me]</li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL 폴더로 이동]</td> 
   <td>파일을 다른 폴더로 이동하려면 파일을 이동시킬 폴더를 선택합니다.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL 파일 ID]</td> 
   <td>업데이트할 파일의 ID를 매핑합니다.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Title]</td> 
   <td>업데이트된 파일의 제목을 입력합니다.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL 파일 콘텐츠 변경]</td> 
   <td>파일의 내용을 바꾸는지 여부를 선택합니다.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL 소스 파일]</td> 
   <td>이전 모듈에서 전달된 파일을 사용할지, 수동으로 매핑할지 여부를 선택합니다. 이 필드는 이전 필드에서 파일의 내용을 변경하도록 선택한 경우 사용할 수 있습니다.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL 파일 이름]</td> 
   <td>파일 이름을 선택합니다. [!UICONTROL source file] 필드에서 "[!UICONTROL Map]"을 선택하면 이 옵션을 사용할 수 있습니다.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Data]</td> 
   <td>업로드할 데이터 파일을 선택합니다. [!UICONTROL source file] 필드에서 "[!UICONTROL Map]"을 선택하면 이 옵션을 사용할 수 있습니다.</td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL 파일 복사]

파일을 새 위치에 복사합니다.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL Connection] </td> 
   <td> <p>연결 방법에 대한 지침은 [!DNL Google Drive] 계정 대상 [!DNL Workfront Fusion]를 참조하십시오. <a href="#connecting-google-drive-to-workfront-fusion" class="MCXref xref">연결 중 [!DNL Google Drive] [!UICONTROL Workfront Fusion] 변환</a></p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL 대상]</td> 
   <td> <p>파일을 업로드할 대상을 선택합니다.</p> 
    <ul> 
     <li>[!UICONTROL My Drive]</li> 
     <li>[!UICONTROL Shared with Me]</li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Target 폴더]</td> 
   <td>복사할 파일이 있는 폴더를 선택합니다./</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL 파일 ID]</td> 
   <td>업데이트할 파일의 ID를 매핑합니다.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL 복사본의 이름입니다.]</td> 
   <td>새 파일의 제목을 입력합니다. 원래 파일 이름을 변경하지 않으려면 이 필드를 비워 둡니다.</td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL 파일 삭제]

파일 또는 폴더를 영구적으로 삭제합니다.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL Connection] </td> 
   <td> <p>연결 방법에 대한 지침은 [!DNL Google Drive] 계정 대상 [!DNL Workfront Fusion]를 참조하십시오. <a href="#connecting-google-drive-to-workfront-fusion" class="MCXref xref">연결 중 [!DNL Google Drive] [!UICONTROL Workfront Fusion] 변환</a></p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL 파일 ID]</td> 
   <td>삭제할 파일의 ID를 매핑합니다.</td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL 파일/폴더를 휴지통으로 이동]

파일 또는 폴더를 휴지통으로 이동합니다.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL Connection] </td> 
   <td> <p>연결 방법에 대한 지침은 [!DNL Google Drive] 계정 대상 [!DNL Workfront Fusion]를 참조하십시오. <a href="#connecting-google-drive-to-workfront-fusion" class="MCXref xref">연결 중 [!DNL Google Drive] [!UICONTROL Workfront Fusion] 변환</a></p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL 파일 ID]</td> 
   <td>이동할 파일의 ID를 휴지통으로 매핑합니다.</td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL 파일 가져오기]

ID가 지정된 파일을 검색합니다.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL Connection] </td> 
   <td> <p>연결 방법에 대한 지침은 [!DNL Google Drive] 계정 대상 [!DNL Workfront Fusion]를 참조하십시오. <a href="#connecting-google-drive-to-workfront-fusion" class="MCXref xref">연결 중 [!DNL Google Drive] [!UICONTROL Workfront Fusion] 변환</a></p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Convert [!DNL Google Documents] 파일 형식]</td> 
   <td>변환할 파일 형식을 선택합니다 [!DNL Google Documents] 대상.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Convert [!DNL Google Spreadsheets] 파일 형식]</td> 
   <td>변환할 파일 형식을 선택합니다 [!DNL Google Spreadsheets] 대상.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Convert [!DNL Google Slides] 파일 형식]</td> 
   <td>변환할 파일 형식을 선택합니다 [!DNL Google Slides] 대상.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Convert [!DNL Google Drawings] 파일 형식]</td> 
   <td>변환할 파일 형식을 선택합니다 [!DNL Google Drawings] 대상.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL 파일 ID]</td> 
   <td>검색할 파일의 ID를 매핑합니다.</td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL 파일/폴더 검색]

검색 기준에 따라 파일 또는 폴더를 검색합니다.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL Connection] </td> 
   <td> <p>연결 방법에 대한 지침은 [!DNL Google Drive] 계정 대상 [!DNL Workfront Fusion]를 참조하십시오. <a href="#connecting-google-drive-to-workfront-fusion" class="MCXref xref">연결 중 [!DNL Google Drive] [!UICONTROL Workfront Fusion] 변환</a></p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL 대상]</td> 
   <td> <p>검색할 대상을 선택합니다.</p> 
    <ul> 
     <li>[!UICONTROL My Drive]</li> 
     <li>[!UICONTROL Shared with Me]</li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL 폴더 나열]</td> 
   <td>파일 또는 폴더를 검색할 폴더로 이동합니다.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Retrieve]</td> 
   <td> <p> 파일, 폴더 또는 둘 다를 검색할지 여부를 선택합니다.</p> </td> 
  </tr> 
  <tr> 
   <td> <p>[!UICONTROL Search]</p> </td> 
   <td> <p>수행할 검색 유형을 선택합니다.</p> 
    <ul> 
     <li> <p><strong>[!UICONTROL 파일/폴더 이름 내에서 검색]</strong> </p> 
      <ul> 
       <li> <p><strong>[!UICONTROL Query]</strong> </p> <p>검색할 파일 이름 또는 전체 파일 이름(접미사 포함)의 일부를 입력합니다.</p> </li> 
       <li> <p><strong>[!UICONTROL 검색 옵션]</strong> </p> <p>정확한 용어를 검색할지 또는 검색어가 포함된 이름을 검색할지 선택합니다.</p> </li> 
      </ul> </li> 
     <li> <p><strong>[!UICONTROL Fulltext] 검색</strong> </p> 
      <ul> 
       <li> <p><strong>[!UICONTROL Query]</strong> </p> <p>검색어에 원하는 검색어를 입력하십시오. [!DNL Google Drive].</p> </li> 
      </ul> </li> 
     <li> <p><strong>사용자 지정 검색 쿼리 입력</strong> </p> 
      <ul> 
       <li> <p><strong>[!UICONTROL Query]</strong> </p> <p>사용자 정의 검색 쿼리를 입력합니다. 자세한 내용은 이 문서의 [!UICONTROL 파일 검색] 섹션을 참조하십시오.</p> </li> 
       <li> <p><strong>위에 선택한 폴더를 쿼리에 추가합니다</strong> </p> <p>상위 컬렉션에서 폴더를 검색합니다. 위에서 선택한 폴더에 직접 있는 모든 파일과 폴더를 찾습니다.</p> </li> 
      </ul> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL 반환된 최대 결과 수]</td> 
   <td>최대 파일 또는 폴더 수 설정 [!DNL Workfront Fusion] 은 한 실행 주기 동안 반환됩니다.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL 모듈이 결과를 반환하지 않더라도 경로 실행을 계속합니다.]</td> 
   <td>모듈에서 결과를 반환하지 않을 경우 시나리오가 중지되지 않도록 하려면 이 옵션을 활성화합니다.</td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL 폴더 만들기]

지정된 위치에 폴더를 만듭니다.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL Connection] </td> 
   <td> <p>연결 방법에 대한 지침은 [!DNL Google Drive] 계정 대상 [!DNL Workfront Fusion]를 참조하십시오. <a href="#connecting-google-drive-to-workfront-fusion" class="MCXref xref">연결 중 [!DNL Google Drive] [!UICONTROL Workfront Fusion] 변환</a></p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL 대상]</td> 
   <td> <p>파일을 업로드할 대상을 선택합니다.</p> 
    <ul> 
     <li>[!UICONTROL My Drive]</li> 
     <li>[!UICONTROL Shared with Me]</li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL 새 폴더 위치]</td> 
   <td>새 폴더를 만들 위치로 이동합니다.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL 새 폴더의 이름]</td> 
   <td>만들 폴더의 이름을 입력합니다.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL 공유 폴더]</td> 
   <td>[!UICONTROL 공유] 링크를 사용하여 모든 사람과 폴더를 공유하려면 이 옵션을 선택합니다. 그렇지 않으면, 공유 링크는 소유자만을 위한 것입니다.</td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL 공유 링크 가져오기]

Google 드라이브에서 파일에 대한 공유 링크를 검색합니다.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL Connection] </td> 
   <td> <p>연결 방법에 대한 지침은 [!DNL Google Drive] 계정 대상 [!DNL Workfront Fusion]를 참조하십시오. <a href="#connecting-google-drive-to-workfront-fusion" class="MCXref xref">연결 중 [!DNL Google Drive] [!UICONTROL Workfront Fusion] 변환</a></p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL 파일 ID]</td> 
   <td>공유 링크를 가져올 파일의 ID를 매핑합니다.</td> 
  </tr> 
 </tbody> 
</table>

## 문제 해결

### 파일을 업로드하거나 업데이트할 수 없습니다

파일을 업로드하거나 업데이트하지 못하는 경우가 있습니다.

* 업로드된 파일이 너무 커서 허용되는 최대 파일 크기 제한을 초과합니다. [!DNL Google Drive] 계획을 초과했거나 [!DNL Google Drive] 저장소 제한. 스토리지 계획을 업그레이드하거나 [!DNL Google Drive] 서비스.
* 파일을 업로드해야 하는 선택한 폴더가 더 이상 존재하지 않습니다. 시나리오가 중단되고 대상 폴더를 다시 선택해야 합니다.

## 파일 검색

폴더의 모듈 목록 파일에서 다음 부분으로 구성된 고유한 쿼리를 사용할 수 있습니다.

* **[!UICONTROL 필드]** - 검색 중인 파일의 속성(예: 속성) `name` 섹션에 있는 마지막 항목이 될 필요가 없습니다.

* **[!UICONTROL 연산자]** - 데이터에 대해 수행되어 일치하는 항목을 제공하는 테스트(예: `contains`.

* **[!UICONTROL 값]** - 테스트 대상 속성의 컨텐트(예: 파일 이름)입니다 `My cool document`.

절을 결합과 결합 `and` 또는 `or`, 및 을 사용하여 쿼리를 무효화합니다. `not`.

* [필드](#fields)
* [값 유형](#value-types)
* [연산자](#operators)
* [예](#examples)

### 필드

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th>필드 </th> 
   <th>값 유형 </th> 
   <th>연산자</th> 
   <th> <p> 설명</p> </th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td><code>[!UICONTROL title]</code></td> 
   <td>string</td> 
   <td><code>contains</code><sup>1</sup>, <code>=</code>, <code>!=</code></td> 
   <td> <p> 파일 이름입니다.</p> </td> 
  </tr> 
  <tr> 
   <td><code>[!UICONTROL fullText]</code> </td> 
   <td>string </td> 
   <td><code>contains</code><sup>2, 3</sup> </td> 
   <td> <p> 이름, 설명, 컨텐츠 및 색인 가능 텍스트를 포함한 파일의 전체 텍스트입니다.</p> </td> 
  </tr> 
  <tr> 
   <td><code>[!UICONTROL mimeType]</code> </td> 
   <td> string</td> 
   <td><code>contains</code>, <code>=</code>, <code>!=</code></td> 
   <td> <p> 파일의 MIME 유형입니다.</p> </td> 
  </tr> 
  <tr> 
   <td><code>[!UICONTROL modifiedDate]</code> </td> 
   <td> 날짜<sup>4</sup></td> 
   <td><code> &lt;=</code>, <code>&lt;</code>, <code>=</code>, <code>!=</code>, <code>></code>, <code>>=</code></td> 
   <td> <p> 파일에 대한 마지막 수정 날짜입니다.</p> </td> 
  </tr> 
  <tr> 
   <td><code>[!UICONTROL lastViewedByMeDate]</code> </td> 
   <td> 날짜<sup>4</sup></td> 
   <td><code>&lt;=</code>, <code>&lt;</code>, <code>=</code>, <code>!=</code>, <code>></code>, <code>>=</code></td> 
   <td> <p> 사용자가 파일을 마지막으로 본 날짜입니다.</p> </td> 
  </tr> 
  <tr> 
   <td><code>[!UICONTROL trashed]</code></td> 
   <td>부울 </td> 
   <td><code>=</code>, <code>!=</code></td> 
   <td> <p> 파일이 휴지통에 있는지 여부.</p> </td> 
  </tr> 
  <tr> 
   <td><code>[!UICONTROL starred]</code></td> 
   <td>부울 </td> 
   <td><code>=</code>, <code>!=</code></td> 
   <td> <p>파일이 구분되었는지 여부.</p> </td> 
  </tr> 
  <tr> 
   <td><code>[!UICONTROL parents]</code></td> 
   <td>컬렉션 </td> 
   <td><code>in </code> </td> 
   <td> <p>[!UICONTROL parent] 컬렉션에 지정된 ID가 포함되어 있는지 여부입니다.</p> </td> 
  </tr> 
  <tr> 
   <td><code>[!UICONTROL owners]</code></td> 
   <td>컬렉션 </td> 
   <td><code>in </code> </td> 
   <td> <p>파일을 소유한 사용자.</p> </td> 
  </tr> 
  <tr> 
   <td><code>[!UICONTROL writers]</code></td> 
   <td>컬렉션 </td> 
   <td><code>in </code> </td> 
   <td> <p>파일을 수정할 권한이 있는 사용자입니다.</p> </td> 
  </tr> 
  <tr> 
   <td><code>[!UICONTROL readers] </code> </td> 
   <td>컬렉션 </td> 
   <td><code>in </code> </td> 
   <td> <p>파일을 읽을 수 있는 권한이 있는 사용자입니다.</p> </td> 
  </tr> 
  <tr> 
   <td><code>[!UICONTROL sharedWithMe]</code> </td> 
   <td>부울 </td> 
   <td><code>=</code>, <code>!=</code></td> 
   <td> <p> 사용자의 "나와 공유" 컬렉션에 있는 파일입니다.</p> </td> 
  </tr> 
  <tr> 
   <td><code>[!UICONTROL properties] </code> </td> 
   <td>컬렉션</td> 
   <td><code>has </code> </td> 
   <td> <p> 공용 사용자 지정 파일 속성입니다.</p> </td> 
  </tr> 
 </tbody> 
</table>

다음 필드의 연산자에 대해 다음 사항을 고려하십시오.

* 다음 `contains` 연산자는 접두어에 대한 일치만 수행합니다 `title`.

   예를 들어 &quot;HelloWorld&quot; 라는 제목이 `title contains 'Hello'` 하지만 `title contains 'World'`.

* 다음 `contains` 연산자는 전체 문자열 토큰에서만 일치를 수행합니다 `fullText`.

   예를 들어 문서의 전체 텍스트에 &quot;HelloWorld&quot; 문자열이 포함된 경우 쿼리만 포함됩니다 `fullText contains 'HelloWorld'` 결과 반환 다음과 같은 쿼리 `fullText contains 'Hello'` 이 시나리오에서 결과를 반환하지 않습니다.

* 다음 `contains` 연산자가 큰 따옴표로 묶으면 완전 일치 영숫자 구문에서 일치합니다.

   예를 들어 `fullText` 문서에서 &quot;Hello there world&quot; 문자열을 포함시킨 다음 `fullText contains '"Hello there"'` 결과는 반환하지만 쿼리는 `fullText contains '"Hello world"'` 그렇지 않습니다.

   또한 검색이 영숫자인 경우 `fullText` 문서에서 &quot;Hello_world&quot; 문자열을 포함하는 다음 쿼리를 수행합니다 `fullText contains '"Hello world"'` 결과 반환

* 필드 `type` 날짜는 현재 서로 비교할 수 없으며 상수 날짜만 해당됩니다.

### 값 유형

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th>값 유형</th> 
   <th> <p> 메모</p> </th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td>문자열 </td> 
   <td> <p>작은 따옴표로 묶습니다. 을 사용하여 쿼리에서 작은 따옴표 이스케이프 처리 <code>\'</code>예,<code> 'Valentine\'s Day'</code>.</p> </td> 
  </tr> 
  <tr> 
   <td>부울 </td> 
   <td> <p><code>true </code>또는 <code>false</code>.</p> </td> 
  </tr> 
  <tr> 
   <td>일자 </td> 
   <td> <p>RFC 3339 형식, 기본 시간대는 UTC(예: <code>2012-06-04T12:00:00-08:00</code>.</p> </td> 
  </tr> 
 </tbody> 
</table>

### 연산자

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th>연산자 </th> 
   <th> <p>메모</p> </th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td><code>contains</code></td> 
   <td> <p>한 문자열의 컨텐츠가 다른 문자열에 있습니다.</p> </td> 
  </tr> 
  <tr> 
   <td><code>=</code> </td> 
   <td> <p> 문자열 또는 부울의 컨텐츠는 다른 문자열과 같습니다.</p> </td> 
  </tr> 
  <tr> 
   <td><code>!=</code> </td> 
   <td> <p> 문자열 또는 부울의 컨텐츠가 다른 문자열과 같지 않습니다.</p> </td> 
  </tr> 
  <tr> 
   <td><code>&lt;</code> </td> 
   <td> <p> 날짜가 다른 날짜보다 빠릅니다.</p> </td> 
  </tr> 
  <tr> 
   <td><code>&lt;=</code> </td> 
   <td> <p> 날짜가 다른 날짜보다 작거나 같습니다.</p> </td> 
  </tr> 
  <tr> 
   <td><code>></code> </td> 
   <td> <p> 날짜가 다른 날짜보다 늦습니다.</p> </td> 
  </tr> 
  <tr> 
   <td><code>>=</code> </td> 
   <td> <p> 날짜가 다른 날짜보다 이후이거나 같은 날짜입니다.</p> </td> 
  </tr> 
  <tr> 
   <td><code>in </code> </td> 
   <td> <p>요소는 컬렉션 내에 포함되어 있습니다.</p> </td> 
  </tr> 
  <tr> 
   <td><code>and </code> </td> 
   <td> <p>두 절에 모두 일치하는 파일을 반환합니다.</p> </td> 
  </tr> 
  <tr> 
   <td><code>or </code> </td> 
   <td> <p>두 절 중 하나와 일치하는 파일을 반환합니다.</p> </td> 
  </tr> 
  <tr> 
   <td><code>not </code> </td> 
   <td> <p>검색 절을 무효화합니다.</p> </td> 
  </tr> 
  <tr> 
   <td><code>has </code> </td> 
   <td> <p>컬렉션에 매개 변수와 일치하는 요소가 포함되어 있습니다.</p> </td> 
  </tr> 
 </tbody> 
</table>

복합 절의 경우 괄호를 사용하여 절을 함께 그룹화할 수 있습니다. 예:
`modifiedDate > '2012-06-04T12:00:00' and (mimeType contains 'image/' or mimeType contains 'video/')` 이 검색은 2012년 6월 4일 이후에 마지막으로 수정한 이미지 또는 비디오 MIME 유형의 모든 파일을 반환합니다. 왜냐면 `and` 및 `or` 연산자는 괄호를 사용하지 않고 왼쪽에서 오른쪽으로 평가됩니다. 위의 예에서는 2012년 6월 4일 이후에 수정된 이미지만 반환하지만, 2012년 6월 4일 이전이라도 모든 비디오를 반환합니다.

### 예

이 페이지의 모든 예는 인코딩되지 않은 항목을 보여줍니다 `<q>q</q>` 매개 변수, 위치 `title = 'hello'` 는 다음과 같이 인코딩됩니다. `title+%3d+%27hello%27`. 클라이언트 라이브러리는 이 인코딩을 자동으로 처리합니다.

* 이름이 &quot;hello&quot;인 파일을 검색합니다.

   <pre>title = 'hello'</pre>
* 폴더별 MIME 유형을 사용하여 폴더를 검색합니다

   <pre>mimeType = 'application/vnd.google-apps.folder'</pre>
* 폴더가 아닌 파일을 검색합니다.

   <pre>mimeType != 'application/vnd.google-apps.folder'</pre>
* &quot;hello&quot; 및 &quot;goodye&quot;라는 단어가 포함된 이름으로 파일을 검색합니다

   <pre>제목에 'hello'가 포함되어 있고 [!UICONTROL name]에 'goodbye'가 포함되어 있습니다.</pre>
* &quot;hello&quot;라는 단어가 포함되지 않은 이름으로 파일을 검색합니다

   <pre>제목에 'hello'가 없음</pre>
* 컨텐츠에서 &quot;hello&quot;라는 단어가 포함된 파일을 검색합니다

   <pre>fullText에 'hello'가 포함되어 있습니다.</pre>
* 콘텐츠에 &quot;hello&quot;라는 단어가 포함되지 않은 파일을 검색합니다

   <pre>fullText에 'hello'가 없습니다.</pre>
* 컨텐츠에서 정확한 &quot;hello world&quot; 구문을 포함하는 파일을 검색합니다

   <pre>fullText에 '"hello world"'fullText에 '"hello_world"'가 들어 있습니다.</pre>
* &quot;\&quot; 문자(예: &quot;\authors&quot;)가 포함된 쿼리로 파일을 검색합니다.

   <pre>fullText에 '\\authors'가 포함되어 있습니다.</pre>
* &quot;test@example.org&quot; 사용자가 쓸 수 있는 파일을 검색합니다.

   <pre>의 'test@example.org' [!DNL writers]</pre>
* ID 검색 `1234567` 에서 `parents` 컬렉션. ID가 인 폴더에 바로 있는 모든 파일과 폴더를 찾습니다 `1234567`.

   <pre>[!UICONTROL 부모]의 '1234567'</pre>
* 별칭 ID 검색 `appDataFolder` 에서 `parents` 컬렉션. 이렇게 하면 [응용 프로그램 데이터 폴더](https://developers.google.com/drive/api/v2/appdata).

   <pre>부모의 'appDataFolder'</pre>
* &quot;test@example.org&quot; 및 &quot;test2@example.org&quot; 사용자가 쓸 수 있는 파일을 검색합니다.

   <pre>'test@example.org', 'test2@example.org', 'writer'</pre>
* 휴지통에 있는 &quot;중요&quot; 텍스트가 포함된 파일을 검색합니다

   <pre>fullText에 '중요'와 trashed = true가 포함되어 있습니다.</pre>
* 2012년 6월 4일 이후에 수정된 파일 검색

   <pre>modifiedDate &gt; '2012-06-04T12:00:00' // 기본 시간대는 UTC입니다.</pre><pre>modifiedDate &gt; '2012-06-04T12:00:00-08:00'</pre>
* 이름에 &quot;hello&quot;로 권한이 있는 사용자와 공유된 파일을 검색합니다.

   <pre>sharedWithMe 및 제목에 'hello'가 포함됩니다.</pre>
* 다음 항목이 있는 파일 검색 [사용자 지정 파일 속성](https://developers.google.com/drive/api/v2/properties) 명명된 이름 `additionalID` 값 사용 `8e8aceg2af2ge72e78`.

   <pre>속성은 { key='additionalID' 및 value='8e8aceg2af2ge72e78' 및 visibility='PRIVATE' }</pre>

이 안내서의 소스는 다음과 같습니다. [[!DNL Google Drive] 설명서](https://developers.google.com/drive/api/v2/search-shareddrives).
