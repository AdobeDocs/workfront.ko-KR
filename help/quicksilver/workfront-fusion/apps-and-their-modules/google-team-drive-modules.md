---
content-type: reference
product-previous: workfront-fusion
product-area: workfront-integrations;agile-and-teams;user-management
keywords: 커넥터
navigation-topic: apps-and-their-modules
title: Google 팀 드라이브 모듈
description: 다음 [!DNL Adobe Workfront Fusion Google Team Drive] 모듈을 사용하면 파일을 모니터링, 업로드, 업데이트, 복사, 삭제 또는 검색하고 [!DNL Google Shared] 드라이브.
author: Becky
feature: Workfront Fusion
exl-id: 8b4c057f-bb98-44d1-9b71-cbeaa402a1c3
source-git-commit: 885d93dd4383945538e977fd3edbfd55bda88b70
workflow-type: tm+mt
source-wordcount: '1258'
ht-degree: 0%

---

# [!DNL Google Team Drive] 모듈

다음 [!DNL Adobe Workfront Fusion] [!DNL Google Team Drive] 모듈을 사용하면 파일을 모니터링, 업로드, 업데이트, 복사, 삭제 또는 검색하고 [!DNL Google Shared Drive].

를 사용하려면 [!DNL Google Team Drive] with [!DNL Adobe Workfront Fusion]를 채울 때는 [!DNL G Suite] 계정이 필요합니다. 없는 경우 [!DNL G Suite] 계정 [[!DNL G Suite] 사이트 등록](https://gsuite.google.com/signup/businessstarter/welcome).

에서 [!DNL Adobe Workfront Fusion] 시나리오, [!DNL Google Team Drive]여러 타사 애플리케이션 및 서비스에 연결할 수 있습니다.

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

를 사용하려면 [!DNL Google Team Drive] 모듈이면 반드시 [!DNL Google Team Drive].

## [!DNL Google Team Drive] 모듈 및 해당 필드

구성 시 [!DNL Google Team Drive] 모듈, [!DNL Workfront Fusion] 아래 나열된 필드를 표시합니다. 이와 함께 추가 [!DNL Google Team Drive] 앱이나 서비스에서 액세스 수준과 같은 요소에 따라 필드가 표시될 수 있습니다. 모듈에서 굵게 표시된 제목은 필수 필드를 나타냅니다.

에 표시되는 모듈 대화 상자 필드 **굵게** ( [!DNL Workfront Fusion] 시나리오, **not** 이 설명서 문서)는 필수입니다.

필드 또는 함수 위에 맵 단추가 표시되면 이 단추를 사용하여 해당 필드에 대한 변수와 함수를 설정할 수 있습니다. 자세한 내용은 [의 한 모듈에서 다른 모듈로 정보 매핑 [!DNL Adobe Workfront Fusion]](../../workfront-fusion/mapping/map-information-between-modules.md).

![](assets/map-toggle-350x74.png)

### Triggers

#### [!UICONTROL 감시 파일]

지정된 폴더에 새 파일을 추가하거나 수정할 때 파일 세부 정보를 반환합니다.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL Connection] </td> 
   <td> <p>연결 방법에 대한 지침은 [!DNL Google Team Drive] 계정 대상 [!DNL Workfront Fusion]를 참조하십시오. <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">연결 만들기 [!DNL Adobe Workfront Fusion] - 기본 지침</a></p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Team Drive]</td> 
   <td> <p> 보려는 공유 드라이브를 선택합니다.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Folder] </td> 
   <td> <p>공유 드라이브 내의 폴더를 선택합니다.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL 감시할 파일]</td> 
   <td> <p> 보려는 파일 유형을 선택합니다.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Convert [!DNL Google Documents] 파일 형식] </td> 
   <td> <p>감시하려는 형식을 선택합니다 [!DNL Google Documents] 로 변환된 파일</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Convert [!DNL Google Sheets] 파일 형식] </td> 
   <td> <p>감시하려는 형식을 선택합니다 [!DNL Google Sheets] 로 변환된 파일</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Convert [!DNL Google Slides] 파일 형식] </td> 
   <td> <p>감시하려는 형식을 선택합니다 [!DNL Google Slides] 로 변환된 파일</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Convert [!DNL Google Drawings] 파일 형식] </td> 
   <td> <p>감시하려는 형식을 선택합니다 [!DNL Google Drawings] 로 변환된 파일</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Watch]</td> 
   <td> <p> 새 파일과 수정된 파일에 대한 폴더를 모니터링할지 또는 새 파일에 대해서만 모니터링할지 여부를 선택합니다.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL 다운로드한 최대 파일 수]</td> 
   <td> <p> 최대 파일 수 설정 [!DNL Workfront Fusion] 은 한 실행 주기 동안 반환됩니다.</p> </td> 
  </tr> 
 </tbody> 
</table>

### 액션

* [[!UICONTROL 파일 업로드]](#upload-a-file)
* [[!UICONTROL 파일 업데이트]](#update-a-file)
* [[!UICONTROL 파일 복사]](#copy-a-file)
* [[!UICONTROL 파일 삭제]](#delete-a-file)
* [[!UICONTROL 파일을 휴지통으로 이동]](#move-a-file-to-trash)
* [[!UICONTROL 파일 가져오기]](#get-a-file)
* [[!UICONTROL 파일 목록 가져오기]](#get-a-file-list)
* [[!UICONTROL 폴더 만들기]](#create-a-folder)

#### [!UICONTROL 파일 업로드]

지정된 공유 드라이브에 파일을 업로드합니다.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL Connection] </td> 
   <td> <p>연결 방법에 대한 지침은 [!DNL Google Team Drive] 계정 대상 [!DNL Workfront Fusion]를 참조하십시오. <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">연결 만들기 [!DNL Adobe Workfront Fusion] - 기본 지침</a></p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Team Drive] </td> 
   <td> <p>파일을 업로드할 공유 드라이브를 선택합니다.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Folder] </td> 
   <td> <p>공유 드라이브 내의 폴더를 선택합니다.</p> </td> 
  </tr> 
  <tr> 
   <td> <p>[!UICONTROL 소스 파일]</p> </td> 
   <td> <p>공유 드라이브에 업로드할 파일을 지정합니다.</p> <p>이전 모듈에서 업로드할 파일을 매핑합니다(예: [!UICONTROL HTTP] &gt;[!UICONTROL 파일 가져오기] 또는 [!UICONTROL Dropbox] &gt;[!UICONTROL 파일 가져오기)]] 또는 파일 이름과 파일 데이터를 수동으로 입력합니다.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Title]</td> 
   <td> <p> 공유 폴더에 표시할 파일의 제목을 입력합니다.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL 파일 변환]</td> 
   <td> <p> 이 옵션을 활성화하여 공유 폴더의 해당 Google 형식으로 파일을 변환합니다.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL 파일 업데이트]

파일 이름 및/또는 파일 내용을 변경할 수 있습니다.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL Connection] </td> 
   <td> <p>연결 방법에 대한 지침은 [!DNL Google Team Drive] 계정 대상 [!DNL Workfront Fusion]를 참조하십시오. <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">연결 만들기 [!DNL Adobe Workfront Fusion] - 기본 지침</a></p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Team Drive]</td> 
   <td> <p> 업데이트할 파일이 포함된 공유 드라이브를 선택합니다.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Folder] </td> 
   <td> <p>공유 드라이브 내의 폴더를 선택합니다.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL 파일 ID]</td> 
   <td> <p> 업데이트할 파일의 ID를 입력(매핑)합니다.</p> </td> 
  </tr> 
  <tr> 
   <td> <p>[!UICONTROL 소스 파일]</p> </td> 
   <td>이전 모듈에서 소스 파일을 선택하거나 소스 파일의 이름과 데이터를 매핑합니다.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Title] </td> 
   <td> <p>업데이트된 파일의 새 제목을 입력합니다.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL 파일 변환]</td> 
   <td> <p> 파일을 해당 파일로 변환하려면 이 옵션을 활성화합니다 [!DNL Google] 형식을 공유 폴더로 지정합니다.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL 파일 복사]

지정된 파일을 선택한 폴더에 복사합니다.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL Connection] </td> 
   <td> <p>연결 방법에 대한 지침은 [!DNL Google Team Drive] 계정 대상 [!DNL Workfront Fusion]를 참조하십시오. <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">연결 만들기 [!DNL Adobe Workfront Fusion] - 기본 지침</a></p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Team Drive]</td> 
   <td> <p> 복사할 파일이 들어 있는 공유 드라이브를 선택합니다.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Folder] </td> 
   <td> <p>파일을 복사할 대상 폴더를 선택합니다.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL 파일 ID]</td> 
   <td> <p> 복사할 파일의 ID를 입력(매핑)합니다.</p> </td> 
  </tr> 
  <tr> 
   <td> <p>[!UICONTROL 복사 파일의 이름]</p> </td> 
   <td> <p>대상 위치에서 변경하려면 새 파일 이름을 입력합니다.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL 파일 삭제]

지정된 파일을 삭제합니다.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL Connection] </td> 
   <td> <p>연결 방법에 대한 지침은 [!DNL Google Team Drive] 계정 대상 [!DNL Workfront Fusion]를 참조하십시오. <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">연결 만들기 [!DNL Adobe Workfront Fusion] - 기본 지침</a></p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL 파일 ID]</td> 
   <td> <p> 삭제할 파일의 ID를 입력하거나 매핑합니다.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL 파일을 휴지통으로 이동]

지정된 파일을 휴지통으로 이동합니다.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL Connection] </td> 
   <td> <p>연결 방법에 대한 지침은 [!DNL Google Team Drive] 계정 대상 [!DNL Workfront Fusion]를 참조하십시오. <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">연결 만들기 [!DNL Adobe Workfront Fusion] - 기본 지침</a></p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL 파일 ID]</td> 
   <td> <p> 휴지통으로 이동할 파일의 ID를 입력하거나 매핑합니다.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL 파일 가져오기]

지정한 파일에 대한 세부 정보를 검색합니다.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL Connection] </td> 
   <td> <p>연결 방법에 대한 지침은 [!DNL Google Team Drive] 계정 대상 [!DNL Workfront Fusion]를 참조하십시오. <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">연결 만들기 [!DNL Adobe Workfront Fusion] - 기본 지침</a></p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Convert [!DNL Google Documents] 파일 형식] </td> 
   <td> <p>원하는 형식을 선택합니다 [!DNL Google Documents] 로 변환된 파일</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Convert [!DNL Google Sheets] 파일 형식] </td> 
   <td> <p>원하는 형식을 선택합니다 [!DNL Google Sheets] 로 변환된 파일</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Convert [!DNL Google Slides] 파일 형식] </td> 
   <td> <p>원하는 형식을 선택합니다 [!DNL Google Slides] 로 변환된 파일</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Convert [!DNL Google Drawings] 파일 형식] </td> 
   <td> <p>원하는 형식을 선택합니다 [!DNL Google Drawings] 로 변환된 파일</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL 파일 ID]</td> 
   <td> <p> 검색할 파일의 ID를 입력하거나 매핑합니다.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL 파일 목록 가져오기]

검색어를 기준으로 파일 및/또는 폴더 세부 사항을 검색합니다.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL Connection] </td> 
   <td> <p>연결 방법에 대한 지침은 [!DNL Google Team Drive] 계정 대상 [!DNL Workfront Fusion]를 참조하십시오. <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">연결 만들기 [!DNL Adobe Workfront Fusion] - 기본 지침</a></p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Team Drive]</td> 
   <td> <p> 파일을 나열할 공유 드라이브를 선택합니다.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Folder] </td> 
   <td> <p>파일을 나열할 폴더를 선택합니다.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Search] </td> 
   <td> <p>수행할 검색 유형을 선택합니다. 아래를 참조하십시오.</p> </td> 
  </tr> 
  <tr> 
   <td> <p>[!UICONTROL Query]</p> </td> 
   <td> 
    <ul> 
     <li style="font-weight: bold;"> <p>[!UICONTROL 파일 이름 내에서 검색]</p> <p style="font-weight: normal;">[!UICONTROL Search for exact term Search] 옵션이 선택된 경우 파일 이름(파일 확장명 포함)을 입력하거나, [!UICONTROL Search for name with the term] 옵션이 선택된 경우 이름 부분을 입력합니다.</p> </li> 
     <li> <p style="font-weight: bold;">[!UICONTROL 전체 텍스트 검색]</p> <p>파일 이름, 설명 및 내용을 검색할 검색어를 입력합니다.</p> </li> 
     <li> <p style="font-weight: bold;">[!UICONTROL 사용자 지정 검색 쿼리]</p> <p>을(를) 입력합니다. [!DNL Google] 검색어. 자세한 내용은 [!DNL Google]s <a href="https://developers.google.com/drive/api/v2/ref-search-terms">검색 쿼리 설명서</a>. 예: <code>fullText contains '"Hello world"'</code></p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Retrieve]</td> 
   <td>파일, 폴더 또는 둘 다 검색할지 여부를 선택합니다.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL 반환된 최대 결과 수]</td> 
   <td> <p> 최대 파일 또는 폴더 수 설정 [!DNL Workfront Fusion] 은 한 실행 주기 동안 반환됩니다.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL 폴더 만들기]

새 폴더를 만듭니다.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL Connection] </td> 
   <td> <p>연결 방법에 대한 지침은 [!DNL Google Team Drive] 계정 대상 [!DNL Workfront Fusion]를 참조하십시오. <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">연결 만들기 [!DNL Adobe Workfront Fusion] - 기본 지침</a></p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Team Drive]</td> 
   <td> <p> 폴더를 만들 공유 드라이브를 선택합니다.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Folder] </td> 
   <td> <p>에서 폴더를 만들 폴더를 선택합니다.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL 새 폴더의 이름]</td> 
   <td> <p> 새 폴더의 이름을 입력합니다.</p> </td> 
  </tr> 
 </tbody> 
</table>
