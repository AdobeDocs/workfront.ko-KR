---
content-type: reference
product-previous: workfront-fusion
product-area: workfront-integrations;documents
keywords: 커넥터
navigation-topic: apps-and-their-modules
title: Google 드라이브 모듈
description: 다음 [!DNL Adobe Workfront Fusion Google Drive] 모듈을 사용하면 의 파일, 폴더 또는 공유 드라이브를 모니터링, 검색, 만들기, 업데이트, 삭제 및 관리할 수 있습니다. [!DNL Google Drive].
author: Becky
feature: Workfront Fusion, Digital Content and Documents
exl-id: 7d620c93-d1bf-4451-9f76-1d6fd850cec9
source-git-commit: 0915dcce45b271ee18cdd8af5db4f0eb01f3cced
workflow-type: tm+mt
source-wordcount: '2956'
ht-degree: 0%

---

# [!DNL Google Drive] 모듈

다음 [!DNL Adobe Workfront Fusion] [!DNL Google Drive] 모듈을 사용하면 의 파일, 폴더 또는 공유 드라이브를 모니터링, 검색, 만들기, 업데이트, 삭제 및 관리할 수 있습니다. [!DNL Google Drive].

다음 기간 [!DNL Adobe Workfront Fusion] 시나리오, 다음을 연결할 수 있습니다 [!DNL Google Drive] 여러 타사 애플리케이션 및 서비스에 대한 계정.

시나리오를 만드는 방법에 대한 지침이 필요한 경우 [에서 시나리오 만들기 [!DNL Adobe Workfront Fusion]](../../workfront-fusion/scenarios/create-a-scenario.md).

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



## 연결 중 [!DNL Google Drive] 끝 [!DNL Workfront Fusion]

다음과 같은 경우 [!DNL @gmail.com] 또는 [!DNL @googlemail.com] 에 OAuth 클라이언트를 만들어야 하는 사용자 [다음 [!DNL Google Cloud Platform]](https://console.developers.google.com/projectselector2/apis/dashboard?supportedpurview=project) 얻기 위하여 [!UICONTROL 클라이언트 ID] 및 [!UICONTROL 클라이언트 암호].

OAuth 클라이언트를 만들고 를 얻는 방법에 대한 단계별 지침 [!UICONTROL 클라이언트 ID] 및 [!UICONTROL 클라이언트 암호]), 다음을 참조하십시오. [연결 [!DNL Adobe Workfront Fusion] 끝 [!DNL Google Services] 사용자 정의 OAuth 클라이언트 사용](../../workfront-fusion/connections/connect-fusion-to-google-using-oauth.md).

연결에 대한 자세한 내용 [!DNL Google Drive] 계정 위치: [!UICONTROL Workfront Fusion], 참조 [에 대한 연결 만들기 [!UICONTROL Adobe Workfront Fusion] - 기본 지침](../../workfront-fusion/connections/connect-to-fusion-general.md)

## [!DNL Google Drive] 모듈 및 해당 필드

를 구성할 때 [!DNL Google Drive] 모듈, [!DNL Workfront Fusion] 아래 나열된 필드를 표시합니다. 이와 함께 추가 [!DNL Google Drive] 앱이나 서비스의 액세스 수준 등에 따라 필드가 표시될 수 있습니다. 모듈의 굵은 제목은 필수 필드를 나타냅니다.

필드나 함수 위에 맵 단추가 표시되면 이 단추를 사용하여 해당 필드에 대한 변수와 함수를 설정할 수 있습니다. 자세한 내용은 [의 한 모듈에서 다른 모듈로 정보 매핑 [!DNL Adobe Workfront Fusion]](../../workfront-fusion/mapping/map-information-between-modules.md).

![](assets/map-toggle-350x74.png)



* [트리거](#triggers)
* [액션](#actions)

### 트리거

* [[!UICONTROL 폴더에서 파일 보기]](#watch-files-in-folder)
* [[!UICONTROL 모든 파일 보기]](#watch-all-files)
* [[!UICONTROL 공유 파일 보기]](#watch-shared-files)
* [[!UICONTROL 댓글 보기]](#watch-comments)

#### [!UICONTROL 폴더에서 파일 보기]

지정된 폴더에서 파일을 추가하거나 수정할 때 파일 세부 정보를 검색합니다.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
    <td>[!UICONTROL Connection] </td>
   <td> <p>연결에 대한 자세한 내용 [!DNL Google Drive] 계정 위치: [!DNL Workfront Fusion], 참조 <a href="#connecting-google-drive-to-workfront-fusion" class="MCXref xref">연결 중 [!DNL Google Drive] [!UICONTROL Workfront Fusion]으로</a></p> </td> 
  </tr> 
  <tr>
    <td>[!UICONTROL 감시할 폴더 선택]</td>
    <td >드라이브에서 파일을 감시할 폴더를 선택합니다.</td>
  </tr> 
  <tr> 
    <td>[!UICONTROL 조사할 파일]</td>
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
    <td >[!UICONTROL 변환 [!DNL Google Documents] 형식을 지정할 파일]</td>
    <td>변환할 파일 형식을 선택합니다 [!DNL Google Documents] 받는 사람.</td>
  </tr> 
  <tr>
    <td>[!UICONTROL 변환 [!DNL Google Spreadsheets] 형식을 지정할 파일]</td>
    <td>변환할 파일 형식을 선택합니다 [!DNL Google Spreadsheets] 받는 사람.</td>
  </tr> 
  <tr>
    <td>[!UICONTROL 변환 [!DNL Google Slides] 형식을 지정할 파일]</td>
    <td>변환할 파일 형식을 선택합니다 [!DNL Google Slides] 받는 사람.</td>
  </tr> 
  <tr>
    <td>[!UICONTROL 변환 [!DNL Google Drawings] 형식을 지정할 파일]</td>
    <td>변환할 파일 형식을 선택합니다 [!DNL Google Drawings] 받는 사람.</td>
  </tr> 
  <tr>
    <td>[!UICONTROL Watch]</td>
    <td>새 파일과 모든 변경 내용을 보는지 아니면 새 파일만 보는지 선택합니다.</td>
  </tr> 
  <tr> 
    <td>[!UICONTROL 다운로드한 최대 파일 수]</td>
    <td>다음에 대한 최대 결과 수 설정 [!DNL Workfront Fusion] 는 한 주기(시나리오 실행당 반복 횟수) 동안 다운로드됩니다.</td>
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL 모든 파일 보기]

에 파일이 있을 때 파일 세부 정보를 검색합니다. [!DNL Google Drive] 이 추가되거나 수정됩니다.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL Connection] </td> 
   <td> <p>연결에 대한 자세한 내용 [!DNL Google Drive] 계정 위치: [!DNL Workfront Fusion], 참조 <a href="#connecting-google-drive-to-workfront-fusion" class="MCXref xref">연결 중 [!DNL Google Drive] [!UICONTROL Workfront Fusion]으로</a></p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL 조사할 파일]</td> 
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
    <td >[!UICONTROL 변환 [!DNL Google Documents] 형식을 지정할 파일]</td>
    <td>변환할 파일 형식을 선택합니다 [!DNL Google Documents] 받는 사람.</td>
  </tr> 
  <tr>
    <td>[!UICONTROL 변환 [!DNL Google Spreadsheets] 형식을 지정할 파일]</td>
    <td>변환할 파일 형식을 선택합니다 [!DNL Google Spreadsheets] 받는 사람.</td>
  </tr> 
  <tr>
    <td>[!UICONTROL 변환 [!DNL Google Slides] 형식을 지정할 파일]</td>
    <td>변환할 파일 형식을 선택합니다 [!DNL Google Slides] 받는 사람.</td>
  </tr> 
  <tr>
    <td>[!UICONTROL 변환 [!DNL Google Drawings] 형식을 지정할 파일]</td>
    <td>변환할 파일 형식을 선택합니다 [!DNL Google Drawings] 받는 사람.</td>
  </tr>  
  <tr> 
   <td>[!UICONTROL Watch]</td> 
   <td>새 파일과 모든 변경 내용을 보는지 아니면 새 파일만 보는지 선택합니다.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL 다운로드한 최대 파일 수]</td> 
   <td>다음에 대한 최대 결과 수 설정 [!DNL Workfront Fusion] 는 한 주기(시나리오 실행당 반복 횟수) 동안 다운로드됩니다.</td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL 공유 파일 보기]

새 파일이 공유되거나 기존 공유 파일이 업데이트될 때 트리거됩니다.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL Connection] </td> 
   <td> <p>연결에 대한 자세한 내용 [!DNL Google Drive] 계정 위치: [!DNL Workfront Fusion], 참조 <a href="#connecting-google-drive-to-workfront-fusion" class="MCXref xref">연결 중 [!DNL Google Drive] [!UICONTROL Workfront Fusion]으로</a></p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL 감시할 폴더 선택]</td> 
   <td>파일을 보려는 공유 폴더를 선택합니다.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL 조사할 파일]</td> 
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
    <td >[!UICONTROL 변환 [!DNL Google Documents] 형식을 지정할 파일]</td>
    <td>변환할 파일 형식을 선택합니다 [!DNL Google Documents] 받는 사람.</td>
  </tr> 
  <tr>
    <td>[!UICONTROL 변환 [!DNL Google Spreadsheets] 형식을 지정할 파일]</td>
    <td>변환할 파일 형식을 선택합니다 [!DNL Google Spreadsheets] 받는 사람.</td>
  </tr> 
  <tr>
    <td>[!UICONTROL 변환 [!DNL Google Slides] 형식을 지정할 파일]</td>
    <td>변환할 파일 형식을 선택합니다 [!DNL Google Slides] 받는 사람.</td>
  </tr> 
  <tr>
    <td>[!UICONTROL 변환 [!DNL Google Drawings] 형식을 지정할 파일]</td>
    <td>변환할 파일 형식을 선택합니다 [!DNL Google Drawings] 받는 사람.</td>
  </tr> 
  <tr> 
   <td>[!UICONTROL Watch]</td> 
   <td>새 파일과 모든 변경 내용을 보는지 아니면 새 파일만 보는지 선택합니다.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL 다운로드한 최대 파일 수]</td> 
   <td>다음에 대한 최대 결과 수 설정 [!DNL Workfront Fusion] 는 한 주기(시나리오 실행당 반복 횟수) 동안 다운로드됩니다.</td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL 댓글 보기]

선택한 파일에서 댓글을 추가하거나 수정할 때 트리거됩니다.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL Connection] </td> 
   <td> <p>연결에 대한 자세한 내용 [!DNL Google Drive] 계정 위치: [!DNL Workfront Fusion], 참조 <a href="#connecting-google-drive-to-workfront-fusion" class="MCXref xref">연결 중 [!DNL Google Drive] [!UICONTROL Workfront Fusion]으로</a></p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL 파일]</td> 
   <td>댓글을 확인할 파일을 선택합니다.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Watch]</td> 
   <td>모든 변경 사항에 대해 감시할지 또는 새 주석에 대해서만 감시할지 선택</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL 반환되는 최대 주석 수]</td> 
   <td>댓글의 최대 수를 설정합니다. [!DNL Workfront Fusion] 는 한 주기(시나리오 실행당 반복 횟수) 동안 를 반환합니다.</td> 
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

에 파일 업로드 [!DNL Google Drive].

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL Connection] </td> 
   <td> <p>연결에 대한 자세한 내용 [!DNL Google Drive] 계정 위치: [!DNL Workfront Fusion], 참조 <a href="#connecting-google-drive-to-workfront-fusion" class="MCXref xref">연결 중 [!DNL Google Drive] [!UICONTROL Workfront Fusion]으로</a></p> </td> 
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
   <td>이전 모듈에서 전달된 파일을 사용할지 또는 파일을 수동으로 매핑할지 여부를 선택합니다.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL 파일 이름]</td> 
   <td>파일 이름을 선택합니다. 이 옵션은 [!UICONTROL source file] 필드에서 "[!UICONTROL Map]"을 선택한 경우에 사용할 수 있습니다.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Data]</td> 
   <td>업로드할 데이터 파일을 선택합니다. 이 옵션은 [!UICONTROL source file] 필드에서 "[!UICONTROL Map]"을 선택한 경우에 사용할 수 있습니다.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Title]</td> 
   <td>새 파일의 제목을 입력합니다.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL 파일 변환]</td> 
   <td>이 옵션을 활성화하면 모듈이 파일을 해당 파일로 변환할 수 있습니다 [!DNL Google] 포맷.</td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL 파일 업데이트]

파일의 메타데이터 또는 컨텐츠를 업데이트합니다.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL Connection] </td> 
   <td> <p>연결에 대한 자세한 내용 [!DNL Google Drive] 계정 위치: [!DNL Workfront Fusion], 참조 <a href="#connecting-google-drive-to-workfront-fusion" class="MCXref xref">연결 중 [!DNL Google Drive] [!UICONTROL Workfront Fusion]으로</a></p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL 대상]</td> 
   <td> <p>파일을 업로드할 대상을 선택합니다.</p> 
    <ul> 
     <li>[!UICONTROL 내 드라이브]</li> 
     <li>[!UICONTROL 나와 공유됨]</li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL 폴더로 이동]</td> 
   <td>파일을 다른 폴더로 이동하려면 파일을 이동할 폴더를 선택합니다.</td> 
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
   <td>[!UICONTROL 파일 컨텐츠 변경]</td> 
   <td>파일 내용을 바꿀 것인지 선택합니다.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL 소스 파일]</td> 
   <td>이전 모듈에서 전달된 파일을 사용할지 또는 파일을 수동으로 매핑할지 여부를 선택합니다. 이전 필드에서 파일의 내용을 변경하도록 선택한 경우 이 필드를 사용할 수 있습니다.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL 파일 이름]</td> 
   <td>파일 이름을 선택합니다. 이 옵션은 [!UICONTROL source file] 필드에서 "[!UICONTROL Map]"을 선택한 경우에 사용할 수 있습니다.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Data]</td> 
   <td>업로드할 데이터 파일을 선택합니다. 이 옵션은 [!UICONTROL source file] 필드에서 "[!UICONTROL Map]"을 선택한 경우에 사용할 수 있습니다.</td> 
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
   <td> <p>연결에 대한 자세한 내용 [!DNL Google Drive] 계정 위치: [!DNL Workfront Fusion], 참조 <a href="#connecting-google-drive-to-workfront-fusion" class="MCXref xref">연결 중 [!DNL Google Drive] [!UICONTROL Workfront Fusion]으로</a></p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL 대상]</td> 
   <td> <p>파일을 업로드할 대상을 선택합니다.</p> 
    <ul> 
     <li>[!UICONTROL 내 드라이브]</li> 
     <li>[!UICONTROL 나와 공유됨]</li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Target 폴더]</td> 
   <td>복사할 파일이 있는 폴더 선택/</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL 파일 ID]</td> 
   <td>업데이트할 파일의 ID를 매핑합니다.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL 사본 이름]</td> 
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
   <td> <p>연결에 대한 자세한 내용 [!DNL Google Drive] 계정 위치: [!DNL Workfront Fusion], 참조 <a href="#connecting-google-drive-to-workfront-fusion" class="MCXref xref">연결 중 [!DNL Google Drive] [!UICONTROL Workfront Fusion]으로</a></p> </td> 
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
   <td> <p>연결에 대한 자세한 내용 [!DNL Google Drive] 계정 위치: [!DNL Workfront Fusion], 참조 <a href="#connecting-google-drive-to-workfront-fusion" class="MCXref xref">연결 중 [!DNL Google Drive] [!UICONTROL Workfront Fusion]으로</a></p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL 파일 ID]</td> 
   <td>휴지통으로 이동할 파일의 ID를 매핑합니다.</td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL 파일 가져오기]

지정된 ID로 파일을 검색합니다.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL Connection] </td> 
   <td> <p>연결에 대한 자세한 내용 [!DNL Google Drive] 계정 위치: [!DNL Workfront Fusion], 참조 <a href="#connecting-google-drive-to-workfront-fusion" class="MCXref xref">연결 중 [!DNL Google Drive] [!UICONTROL Workfront Fusion]으로</a></p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL 변환 [!DNL Google Documents] 형식을 지정할 파일]</td> 
   <td>변환할 파일 형식을 선택합니다 [!DNL Google Documents] 받는 사람.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL 변환 [!DNL Google Spreadsheets] 형식을 지정할 파일]</td> 
   <td>변환할 파일 형식을 선택합니다 [!DNL Google Spreadsheets] 받는 사람.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL 변환 [!DNL Google Slides] 형식을 지정할 파일]</td> 
   <td>변환할 파일 형식을 선택합니다 [!DNL Google Slides] 받는 사람.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL 변환 [!DNL Google Drawings] 형식을 지정할 파일]</td> 
   <td>변환할 파일 형식을 선택합니다 [!DNL Google Drawings] 받는 사람.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL 파일 ID]</td> 
   <td>검색할 파일의 ID를 매핑합니다.</td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL 파일/폴더 검색]

검색 조건에 따라 파일 또는 폴더를 검색합니다.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL Connection] </td> 
   <td> <p>연결에 대한 자세한 내용 [!DNL Google Drive] 계정 위치: [!DNL Workfront Fusion], 참조 <a href="#connecting-google-drive-to-workfront-fusion" class="MCXref xref">연결 중 [!DNL Google Drive] [!UICONTROL Workfront Fusion]으로</a></p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL 대상]</td> 
   <td> <p>검색할 대상을 선택합니다.</p> 
    <ul> 
     <li>[!UICONTROL 내 드라이브]</li> 
     <li>[!UICONTROL 나와 공유됨]</li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL 폴더 나열]</td> 
   <td>파일 또는 폴더를 검색할 폴더로 이동합니다.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL 검색]</td> 
   <td> <p> 파일, 폴더 또는 둘 다 검색할지 선택합니다.</p> </td> 
  </tr> 
  <tr> 
   <td> <p>[!UICONTROL Search]</p> </td> 
   <td> <p>수행할 검색 유형을 선택합니다.</p> 
    <ul> 
     <li> <p><strong>[!UICONTROL 파일/폴더 이름 내 검색]</strong> </p> 
      <ul> 
       <li> <p><strong>[!UICONTROL Query]</strong> </p> <p>검색할 파일 이름 또는 전체 파일 이름(접미사 포함)의 일부를 입력합니다.</p> </li> 
       <li> <p><strong>[!UICONTROL 검색 옵션]</strong> </p> <p>정확한 용어를 검색할지 또는 검색어가 포함된 이름을 검색할지 여부를 선택합니다.</p> </li> 
      </ul> </li> 
     <li> <p><strong>[!UICONTROL Fulltext] 검색</strong> </p> 
      <ul> 
       <li> <p><strong>[!UICONTROL Query]</strong> </p> <p>검색할 검색어를 입력하십시오. [!DNL Google Drive].</p> </li> 
      </ul> </li> 
     <li> <p><strong>사용자 정의 검색 쿼리 입력</strong> </p> 
      <ul> 
       <li> <p><strong>[!UICONTROL Query]</strong> </p> <p>사용자 지정 검색 쿼리를 입력합니다. 자세한 내용은 이 문서의 [!UICONTROL Search for Files] 섹션을 참조하십시오.</p> </li> 
       <li> <p><strong>위에서 선택한 폴더를 쿼리에 추가합니다.</strong> </p> <p>상위 컬렉션에서 폴더를 검색합니다. 이렇게 하면 위에서 선택한 폴더에 직접 있는 모든 파일과 폴더를 찾습니다.</p> </li> 
      </ul> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL 반환되는 최대 결과 수]</td> 
   <td>최대 파일 또는 폴더 수 설정 [!DNL Workfront Fusion] 는 한 실행 주기 동안 를 반환합니다.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL 모듈이 결과를 반환하지 않더라도 라우트 실행을 계속합니다.]</td> 
   <td>모듈이 결과를 반환하지 않는 경우 시나리오가 중지되지 않도록 하려면 이 옵션을 활성화합니다.</td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL 폴더 만들기]

지정한 위치에 폴더를 만듭니다.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL Connection] </td> 
   <td> <p>연결에 대한 자세한 내용 [!DNL Google Drive] 계정 위치: [!DNL Workfront Fusion], 참조 <a href="#connecting-google-drive-to-workfront-fusion" class="MCXref xref">연결 중 [!DNL Google Drive] [!UICONTROL Workfront Fusion]으로</a></p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL 대상]</td> 
   <td> <p>파일을 업로드할 대상을 선택합니다.</p> 
    <ul> 
     <li>[!UICONTROL 내 드라이브]</li> 
     <li>[!UICONTROL 나와 공유됨]</li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL 새 폴더 위치]</td> 
   <td>새 폴더를 만들 위치로 이동합니다.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL 새 폴더의 이름]</td> 
   <td>생성 중인 폴더의 이름을 입력합니다.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL 공유 폴더]</td> 
   <td>[!UICONTROL 공유] 링크를 가진 모든 사람과 폴더를 공유하려면 이 옵션을 선택합니다. 그렇지 않으면 소유자만 공유 링크를 사용할 수 있습니다.</td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL 공유 링크 가져오기]

Google 드라이브의 파일에 대한 공유 링크를 검색합니다.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL Connection] </td> 
   <td> <p>연결에 대한 자세한 내용 [!DNL Google Drive] 계정 위치: [!DNL Workfront Fusion], 참조 <a href="#connecting-google-drive-to-workfront-fusion" class="MCXref xref">연결 중 [!DNL Google Drive] [!UICONTROL Workfront Fusion]으로</a></p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL 파일 ID]</td> 
   <td>공유 링크를 가져올 파일의 ID를 매핑합니다.</td> 
  </tr> 
 </tbody> 
</table>

## 문제 해결

### 파일을 업로드하거나 업데이트할 수 없음

파일 업로드 또는 업데이트가 실패할 경우 다음과 같은 몇 가지 상황이 발생합니다.

* 업로드된 파일이 너무 커서 다음에 대해 허용되는 최대 파일 크기 제한을 초과합니다. [!DNL Google Drive] 플랜 또는 을(를) 초과했습니다. [!DNL Google Drive] 스토리지 제한. 스토리지 계획을 업그레이드하거나 [!DNL Google Drive] 서비스.
* 파일을 업로드할 선택한 폴더가 더 이상 존재하지 않습니다. 시나리오가 중지되고 대상 폴더를 다시 선택해야 합니다.

## 파일 검색

폴더의 목록 파일 모듈에서 다음 부분으로 구성된 자체 쿼리를 사용할 수 있습니다.

* **[!UICONTROL 필드]** - 검색 중인 파일의 속성(예: 속성) `name` 을 선택합니다.

* **[!UICONTROL 연산자]** - 일치 항목을 제공하기 위해 데이터에 대해 수행되는 테스트(예: ) `contains`.

* **[!UICONTROL 값]** - 테스트되는 속성의 콘텐츠(예: 파일 이름) `My cool document`.

절을 연결점과 결합 `and` 또는 `or`및 을 사용하여 쿼리 부정 `not`.

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
   <td>문자열</td> 
   <td><code>contains</code><sup>1</sup>, <code>=</code>, <code>!=</code></td> 
   <td> <p> 파일 이름.</p> </td> 
  </tr> 
  <tr> 
   <td><code>[!UICONTROL fullText]</code> </td> 
   <td>문자열 </td> 
   <td><code>contains</code><sup>2, 3</sup> </td> 
   <td> <p> 이름, 설명, 콘텐츠 및 색인화 가능한 텍스트가 포함된 파일의 전체 텍스트입니다.</p> </td> 
  </tr> 
  <tr> 
   <td><code>[!UICONTROL mimeType]</code> </td> 
   <td> 문자열</td> 
   <td><code>contains</code>, <code>=</code>, <code>!=</code></td> 
   <td> <p> 파일의 MIME 유형입니다.</p> </td> 
  </tr> 
  <tr> 
   <td><code>[!UICONTROL modifiedDate]</code> </td> 
   <td> 날짜<sup>4</sup></td> 
   <td><code> &lt;=</code>, <code>&lt;</code>, <code>=</code>, <code>!=</code>, <code>></code>, <code>>=</code></td> 
   <td> <p> 마지막으로 파일을 수정한 날짜입니다.</p> </td> 
  </tr> 
  <tr> 
   <td><code>[!UICONTROL lastViewedByMeDate]</code> </td> 
   <td> 날짜<sup>4</sup></td> 
   <td><code>&lt;=</code>, <code>&lt;</code>, <code>=</code>, <code>!=</code>, <code>></code>, <code>>=</code></td> 
   <td> <p> 사용자가 마지막으로 파일을 본 날짜입니다.</p> </td> 
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
   <td> <p>파일이 표시되는지 여부입니다.</p> </td> 
  </tr> 
  <tr> 
   <td><code>[!UICONTROL parents]</code></td> 
   <td>컬렉션 </td> 
   <td><code>in </code> </td> 
   <td> <p>[!UICONTROL 상위] 컬렉션에 지정된 ID가 포함되어 있는지 여부입니다.</p> </td> 
  </tr> 
  <tr> 
   <td><code>[!UICONTROL owners]</code></td> 
   <td>컬렉션 </td> 
   <td><code>in </code> </td> 
   <td> <p>파일을 소유하는 사용자입니다.</p> </td> 
  </tr> 
  <tr> 
   <td><code>[!UICONTROL writers]</code></td> 
   <td>컬렉션 </td> 
   <td><code>in </code> </td> 
   <td> <p>파일을 수정할 수 있는 권한이 있는 사용자.</p> </td> 
  </tr> 
  <tr> 
   <td><code>[!UICONTROL readers] </code> </td> 
   <td>컬렉션 </td> 
   <td><code>in </code> </td> 
   <td> <p>파일을 읽을 수 있는 권한이 있는 사용자.</p> </td> 
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

이러한 필드의 연산자에 대해 다음 사항을 고려하십시오.

* 다음 `contains` 연산자는 접두사 일치만 수행합니다. `title`.

  예를 들어 &quot;HelloWorld&quot;라는 제목은 `title contains 'Hello'` 하지만 다음에 대해서는 해당되지 않음 `title contains 'World'`.

* 다음 `contains` 연산자는 전체 문자열 토큰에 대해서만 일치를 수행합니다. `fullText`.

  예를 들어, 문서의 전체 텍스트에 문자열 &quot;HelloWorld&quot;가 포함되어 있으면 쿼리만 `fullText contains 'HelloWorld'` 결과를 반환합니다. 쿼리: `fullText contains 'Hello'` 이 시나리오에서는 결과가 반환되지 않습니다.

* 다음 `contains` 연산자가 큰따옴표로 묶인 경우 정확한 영숫자 구문에서 일치합니다.

  예를 들어 `fullText` Hello there world 문자열이 포함된 다음 쿼리가 `fullText contains '"Hello there"'` 결과를 반환하지만 쿼리는 `fullText contains '"Hello world"'` 그렇지 않습니다.

  또한 검색이 영숫자이기 때문에 `fullText` 의 문서에 문자열 &quot;Hello_world&quot;가 포함된 후 쿼리 `fullText contains '"Hello world"'` 결과를 반환합니다.

* 필드 `type` 날짜는 현재 서로 비교할 수 없으며 상수 날짜에만 해당됩니다.

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
   <td> <p>작은 따옴표 '(으)로 묶습니다. 쿼리에서 작은 따옴표 이스케이프 처리 <code>\'</code>, 예:<code> 'Valentine\'s Day'</code>.</p> </td> 
  </tr> 
  <tr> 
   <td>부울 </td> 
   <td> <p><code>true </code>또는 <code>false</code>.</p> </td> 
  </tr> 
  <tr> 
   <td>일자 </td> 
   <td> <p>RFC 3339 형식, 기본 시간대는 UTC입니다(예: ). <code>2012-06-04T12:00:00-08:00</code>.</p> </td> 
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
   <td> <p>한 문자열의 콘텐츠가 다른 문자열에 있습니다.</p> </td> 
  </tr> 
  <tr> 
   <td><code>=</code> </td> 
   <td> <p> 문자열 또는 부울의 콘텐츠는 다른 것과 같습니다.</p> </td> 
  </tr> 
  <tr> 
   <td><code>!=</code> </td> 
   <td> <p> 문자열 또는 부울의 콘텐츠가 다른 것과 같지 않습니다.</p> </td> 
  </tr> 
  <tr> 
   <td><code>&lt;</code> </td> 
   <td> <p> 날짜가 다른 날짜보다 빠릅니다.</p> </td> 
  </tr> 
  <tr> 
   <td><code>&lt;=</code> </td> 
   <td> <p> 날짜가 다른 날짜보다 빠르거나 같습니다.</p> </td> 
  </tr> 
  <tr> 
   <td><code>></code> </td> 
   <td> <p> 날짜가 다른 날짜보다 늦습니다.</p> </td> 
  </tr> 
  <tr> 
   <td><code>>=</code> </td> 
   <td> <p> 날짜가 다른 날짜보다 이후이거나 같습니다.</p> </td> 
  </tr> 
  <tr> 
   <td><code>in </code> </td> 
   <td> <p>요소는 컬렉션 내에 포함됩니다.</p> </td> 
  </tr> 
  <tr> 
   <td><code>and </code> </td> 
   <td> <p>두 절과 일치하는 파일을 반환합니다.</p> </td> 
  </tr> 
  <tr> 
   <td><code>or </code> </td> 
   <td> <p>두 절 중 하나와 일치하는 파일을 반환합니다.</p> </td> 
  </tr> 
  <tr> 
   <td><code>not </code> </td> 
   <td> <p>검색 절을 부정합니다.</p> </td> 
  </tr> 
  <tr> 
   <td><code>has </code> </td> 
   <td> <p>컬렉션에 매개 변수와 일치하는 요소가 있습니다.</p> </td> 
  </tr> 
 </tbody> 
</table>

복합 절의 경우 괄호를 사용하여 절을 함께 그룹화할 수 있습니다. 예:
`modifiedDate > '2012-06-04T12:00:00' and (mimeType contains 'image/' or mimeType contains 'video/')` 이 검색은 이미지 또는 비디오 MIME 유형이 있는 모든 파일을 반환하며, 마지막 수정은 2012년 6월 4일 이후입니다. 이유 `and` 및 `or` 연산자는 괄호를 사용하지 않고 왼쪽에서 오른쪽으로 평가됩니다. 위의 예제는 2012년 6월 4일 이후에 수정된 이미지만 반환하지만 2012년 6월 4일 이전의 모든 비디오를 반환합니다.

### 예

이 페이지의 모든 예제에서는 인코딩이 해제된 을 보여 줍니다 `<q>q</q>` 매개 변수, 여기서 `title = 'hello'` 다음과 같이 인코딩됨 `title+%3d+%27hello%27`. 클라이언트 라이브러리는 이 인코딩을 자동으로 처리합니다.

* 이름이 &quot;hello&quot;인 파일 검색
  <pre>title = 'hello'</pre>
* 폴더별 MIME 유형을 사용하여 폴더 검색
  <pre>mimeType = 'application/vnd.google-apps.folder'</pre>
* 폴더가 아닌 파일 검색
  <pre>mimeType != 'application/vnd.google-apps.folder'</pre>
* &quot;hello&quot; 및 &quot;goodbye&quot;가 포함된 이름의 파일 검색
  <pre>제목에 'hello'가 포함되어 있고 [!UICONTROL 이름]에 'goodbye'가 포함되어 있습니다.</pre>
* &quot;hello&quot;라는 단어가 포함되지 않은 이름의 파일 검색
  <pre>제목에 'hello'가 포함되어 있지 않음</pre>
* 콘텐츠에 &quot;hello&quot;라는 단어가 포함된 파일 검색
  <pre>fullText에 'hello'가 포함되어 있습니다.</pre>
* 콘텐츠에 &quot;hello&quot;라는 단어가 포함되지 않은 파일 검색
  <pre>fullText에 'hello'가 포함되어 있지 않습니다.</pre>
* 콘텐츠에서 &quot;hello world&quot;라는 정확한 구문이 포함된 파일을 검색합니다.
  <pre>fullText에 "hello world"가 들어 있습니다."fullText에 "hello_world"가 들어 있습니다."</pre>
* &quot;\&quot; 문자가 포함된 쿼리가 있는 파일 검색(예: &quot;\authors&quot;)
  <pre>전체 텍스트에 '\\authors'가 포함되어 있음</pre>
* &quot;test@example.org&quot; 사용자가 쓸 수 있는 파일 검색
  <pre>의 'test@example.org' [!DNL writers]</pre>
* ID 검색 `1234567` 다음에서 `parents` 컬렉션. 그러면 ID가 인 폴더에 직접 있는 모든 파일과 폴더가 검색됩니다 `1234567`.
  <pre>[!UICONTROL 상위]의 '1234567'</pre>
* 별칭 ID 검색 `appDataFolder` 다음에서 `parents` 컬렉션. 이렇게 하면 바로 아래에 있는 모든 파일과 폴더가 [응용 프로그램 데이터 폴더](https://developers.google.com/drive/api/v2/appdata).
  <pre>상위 항목의 'appDataFolder'</pre>
* &quot;test@example.org&quot; 및 &quot;test2@example.org&quot; 사용자가 쓸 수 있는 파일 검색
  <pre>writers의 'test@example.org' 및 writers의 'test2@example.org'</pre>
* 휴지통에 있는 &quot;important&quot; 텍스트가 포함된 파일 검색
  <pre>fullText에 'important'가 포함되어 있고 휴지통으로 이동된 = true</pre>
* 2012년 6월 4일 이후에 수정된 파일 검색
  <pre>modifiedDate &gt; '2012-06-04T12:00:00' // 기본 시간대는 UTC입니다.</pre><pre>modifiedDate &gt; '2012-06-04T12:00:00-08:00'</pre>
* 이름에 &quot;hello&quot;가 있는 인증된 사용자와 공유된 파일 검색
  <pre>sharedWithMe 및 제목에 'hello'가 포함됨</pre>
* 을(를) 사용하여 파일 검색 [사용자 정의 파일 속성](https://developers.google.com/drive/api/v2/properties) 명명된 `additionalID` 값 포함 `8e8aceg2af2ge72e78`.
  <pre>속성에는 { key='additionalID' 및 value='8e8aceg2af2ge72e78' 및 visibility='PRIVATE' }이(가) 있습니다.</pre>

이 안내서의 소스는 다음과 같습니다 [[!DNL Google Drive] 설명서](https://developers.google.com/drive/api/v2/search-shareddrives).
