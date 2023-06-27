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
source-git-commit: 0915dcce45b271ee18cdd8af5db4f0eb01f3cced
workflow-type: tm+mt
source-wordcount: '1306'
ht-degree: 0%

---

# [!DNL Google Team Drive] 모듈

다음 [!DNL Adobe Workfront Fusion] [!DNL Google Team Drive] 모듈을 사용하면 파일을 모니터링, 업로드, 업데이트, 복사, 삭제 또는 검색하고 [!DNL Google Shared Drive].

를 사용하려면 [!DNL Google Team Drive] 포함 [!DNL Adobe Workfront Fusion], 다음을 보유해야 합니다. [!DNL G Suite] 계정입니다. 파일이 없는 경우 [!DNL G Suite] 계정 위치: [[!DNL G Suite] 등록 사이트](https://gsuite.google.com/signup/businessstarter/welcome).

다음에서 [!DNL Adobe Workfront Fusion] 시나리오에서는 다음을 사용하는 워크플로를 자동화할 수 있습니다 [!DNL Google Team Drive]을 여러 타사 응용 프로그램 및 서비스에 연결할 수 있습니다.

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

## 전제 조건

사용 [!DNL Google Team Drive] 모듈, 다음이 있어야 합니다. [!DNL Google Team Drive].

## [!DNL Google Team Drive] 모듈 및 해당 필드

를 구성할 때 [!DNL Google Team Drive] 모듈, [!DNL Workfront Fusion] 아래 나열된 필드를 표시합니다. 이와 함께 추가 [!DNL Google Team Drive] 앱이나 서비스의 액세스 수준 등에 따라 필드가 표시될 수 있습니다. 모듈의 굵은 제목은 필수 필드를 나타냅니다.

표시되는 모듈 대화 상자 필드입니다 **굵게** (에서) [!DNL Workfront Fusion] 시나리오, **아님** 이 문서 문서에서)는 필수입니다.

필드나 함수 위에 맵 단추가 표시되면 이 단추를 사용하여 해당 필드에 대한 변수와 함수를 설정할 수 있습니다. 자세한 내용은 [의 한 모듈에서 다른 모듈로 정보 매핑 [!DNL Adobe Workfront Fusion]](../../workfront-fusion/mapping/map-information-between-modules.md).

![](assets/map-toggle-350x74.png)

### 트리거

#### [!UICONTROL 파일 보기]

지정된 폴더에서 새 파일이 추가 및/또는 수정되면 파일 세부 정보를 반환합니다.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL Connection] </td> 
   <td> <p>연결에 대한 자세한 내용 [!DNL Google Team Drive] 계정 위치: [!DNL Workfront Fusion], 참조 <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">에 대한 연결 만들기 [!DNL Adobe Workfront Fusion] - 기본 지침</a></p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Team Drive]</td> 
   <td> <p> 보려는 공유 드라이브를 선택합니다.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL 폴더] </td> 
   <td> <p>공유 드라이브 내의 폴더를 선택합니다.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL 조사할 파일]</td> 
   <td> <p> 보려는 파일 유형을 선택합니다.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL 변환 [!DNL Google Documents] 형식을 지정할 파일] </td> 
   <td> <p>감시할 형식 선택 [!DNL Google Documents] 로 변환된 파일입니다.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL 변환 [!DNL Google Sheets] 형식을 지정할 파일] </td> 
   <td> <p>감시할 형식 선택 [!DNL Google Sheets] 로 변환된 파일입니다.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL 변환 [!DNL Google Slides] 형식을 지정할 파일] </td> 
   <td> <p>감시할 형식 선택 [!DNL Google Slides] 로 변환된 파일입니다.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL 변환 [!DNL Google Drawings] 형식을 지정할 파일] </td> 
   <td> <p>감시할 형식 선택 [!DNL Google Drawings] 로 변환된 파일입니다.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Watch]</td> 
   <td> <p> 새 파일과 수정된 파일에 대해 폴더를 모니터링할지 또는 새 파일에만 대해 모니터링할지 선택합니다.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL 다운로드한 최대 파일 수]</td> 
   <td> <p> 최대 파일 수 설정 [!DNL Workfront Fusion] 는 한 실행 주기 동안 를 반환합니다.</p> </td> 
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
   <td> <p>연결에 대한 자세한 내용 [!DNL Google Team Drive] 계정 위치: [!DNL Workfront Fusion], 참조 <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">에 대한 연결 만들기 [!DNL Adobe Workfront Fusion] - 기본 지침</a></p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Team Drive] </td> 
   <td> <p>파일을 업로드할 공유 드라이브를 선택합니다.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL 폴더] </td> 
   <td> <p>공유 드라이브 내의 폴더를 선택합니다.</p> </td> 
  </tr> 
  <tr> 
   <td> <p>[!UICONTROL 소스 파일]</p> </td> 
   <td> <p>공유 드라이브에 업로드할 파일을 지정합니다.</p> <p>이전 모듈에서 업로드할 파일을 매핑합니다(예: [!UICONTROL HTTP] &gt;[!UICONTROL 파일 가져오기] 또는 [!UICONTROL Dropbox] &gt;[!UICONTROL 파일 가져오기)]를 선택하거나 파일 이름과 파일 데이터를 수동으로 입력합니다.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Title]</td> 
   <td> <p> 공유 폴더에 표시될 파일의 제목을 입력합니다.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL 파일 변환]</td> 
   <td> <p> 파일을 공유 폴더의 해당 Google 형식으로 변환하려면 이 옵션을 활성화합니다.</p> </td> 
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
   <td> <p>연결에 대한 자세한 내용 [!DNL Google Team Drive] 계정 위치: [!DNL Workfront Fusion], 참조 <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">에 대한 연결 만들기 [!DNL Adobe Workfront Fusion] - 기본 지침</a></p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Team Drive]</td> 
   <td> <p> 업데이트할 파일이 포함된 공유 드라이브를 선택합니다.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL 폴더] </td> 
   <td> <p>공유 드라이브 내의 폴더를 선택합니다.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL 파일 ID]</td> 
   <td> <p> 업데이트할 파일의 ID를 입력합니다(매핑).</p> </td> 
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
   <td> <p> 이 옵션을 활성화하여 파일을 해당하는 파일로 변환합니다. [!DNL Google] 공유 폴더의 형식입니다.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL 파일 복사]

지정한 파일을 선택한 폴더에 복사합니다.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL Connection] </td> 
   <td> <p>연결에 대한 자세한 내용 [!DNL Google Team Drive] 계정 위치: [!DNL Workfront Fusion], 참조 <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">에 대한 연결 만들기 [!DNL Adobe Workfront Fusion] - 기본 지침</a></p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Team Drive]</td> 
   <td> <p> 복사할 파일이 포함된 공유 드라이브를 선택합니다.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL 폴더] </td> 
   <td> <p>파일을 복사할 대상 폴더를 선택합니다.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL 파일 ID]</td> 
   <td> <p> 복사할 파일의 ID를 입력합니다(매핑).</p> </td> 
  </tr> 
  <tr> 
   <td> <p>[!UICONTROL 복사 파일의 이름]</p> </td> 
   <td> <p>대상 위치에서 새 파일 이름을 변경하려면 해당 파일 이름을 입력합니다.</p> </td> 
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
   <td> <p>연결에 대한 자세한 내용 [!DNL Google Team Drive] 계정 위치: [!DNL Workfront Fusion], 참조 <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">에 대한 연결 만들기 [!DNL Adobe Workfront Fusion] - 기본 지침</a></p> </td> 
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
   <td> <p>연결에 대한 자세한 내용 [!DNL Google Team Drive] 계정 위치: [!DNL Workfront Fusion], 참조 <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">에 대한 연결 만들기 [!DNL Adobe Workfront Fusion] - 기본 지침</a></p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL 파일 ID]</td> 
   <td> <p> 휴지통으로 이동할 파일의 ID를 입력하거나 매핑합니다.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL 파일 가져오기]

지정된 파일에 대한 세부 정보를 검색합니다.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL Connection] </td> 
   <td> <p>연결에 대한 자세한 내용 [!DNL Google Team Drive] 계정 위치: [!DNL Workfront Fusion], 참조 <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">에 대한 연결 만들기 [!DNL Adobe Workfront Fusion] - 기본 지침</a></p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL 변환 [!DNL Google Documents] 형식을 지정할 파일] </td> 
   <td> <p>원하는 형식 선택 [!DNL Google Documents] 로 변환된 파일입니다.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL 변환 [!DNL Google Sheets] 형식을 지정할 파일] </td> 
   <td> <p>원하는 형식 선택 [!DNL Google Sheets] 로 변환된 파일입니다.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL 변환 [!DNL Google Slides] 형식을 지정할 파일] </td> 
   <td> <p>원하는 형식 선택 [!DNL Google Slides] 로 변환된 파일입니다.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL 변환 [!DNL Google Drawings] 형식을 지정할 파일] </td> 
   <td> <p>원하는 형식 선택 [!DNL Google Drawings] 로 변환된 파일입니다.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL 파일 ID]</td> 
   <td> <p> 검색할 파일의 ID를 입력하거나 매핑합니다.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL 파일 목록 가져오기]

검색어를 기반으로 파일 및/또는 폴더 세부 정보를 검색합니다.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL Connection] </td> 
   <td> <p>연결에 대한 자세한 내용 [!DNL Google Team Drive] 계정 위치: [!DNL Workfront Fusion], 참조 <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">에 대한 연결 만들기 [!DNL Adobe Workfront Fusion] - 기본 지침</a></p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Team Drive]</td> 
   <td> <p> 파일을 나열할 공유 드라이브를 선택합니다.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL 폴더] </td> 
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
     <li style="font-weight: bold;"> <p>[!UICONTROL 파일 이름 내 검색]</p> <p style="font-weight: normal;">[!UICONTROL Search for exact term Search] 옵션을 선택한 경우 파일 이름(파일 확장자 포함)을 입력하거나 [!UICONTROL Search for names contains the search for the search term] 옵션을 선택한 경우 이름의 일부를 입력합니다.</p> </li> 
     <li> <p style="font-weight: bold;">[!UICONTROL 전체 텍스트 검색]</p> <p>파일 이름, 설명 및 내용을 검색할 검색어를 입력합니다.</p> </li> 
     <li> <p style="font-weight: bold;">[!UICONTROL 사용자 지정 검색 쿼리]</p> <p>다음을 입력합니다. [!DNL Google] 검색어. 자세한 내용은 다음을 참조하십시오. [!DNL Google]의 <a href="https://developers.google.com/drive/api/v2/ref-search-terms">검색 쿼리 설명서</a>. 예: <code>fullText contains '"Hello world"'</code></p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL 검색]</td> 
   <td>파일을 검색할지, 폴더를 검색할지 또는 둘 다 검색할지 선택합니다.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL 반환되는 최대 결과 수]</td> 
   <td> <p> 최대 파일 또는 폴더 수 설정 [!DNL Workfront Fusion] 는 한 실행 주기 동안 를 반환합니다.</p> </td> 
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
   <td> <p>연결에 대한 자세한 내용 [!DNL Google Team Drive] 계정 위치: [!DNL Workfront Fusion], 참조 <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">에 대한 연결 만들기 [!DNL Adobe Workfront Fusion] - 기본 지침</a></p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Team Drive]</td> 
   <td> <p> 폴더를 만들 공유 드라이브를 선택합니다.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL 폴더] </td> 
   <td> <p>폴더를 만들 폴더를 선택합니다.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL 새 폴더의 이름]</td> 
   <td> <p> 새 폴더의 이름을 입력합니다.</p> </td> 
  </tr> 
 </tbody> 
</table>
