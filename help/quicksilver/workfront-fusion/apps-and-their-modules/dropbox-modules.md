---
content-type: reference
product-previous: workfront-fusion
product-area: workfront-integrations;documents
keywords: 커넥터
navigation-topic: apps-and-their-modules
title: Dropbox 모듈
description: ' [!DNL Adobe Workfront Fusion] 시나리오에서는 Dropbox을 사용하는 워크플로를 자동화하고 여러 타사 응용 프로그램 및 서비스에 연결할 수 있습니다.이를 통해 Dropbox의 파일 및 폴더에 대한 모니터링, 검색, 검색, 목록 작성, 편집 등의 작업을 자동화할 수 있습니다.'
author: Becky
feature: Workfront Fusion, Digital Content and Documents
exl-id: a35631d7-40ac-4e7f-9a37-ad3879c0b6a2
source-git-commit: 55485da1ea650121b5537a3f19d8102623ed4f43
workflow-type: tm+mt
source-wordcount: '3230'
ht-degree: 0%

---

# [!DNL Dropbox]개 모듈

[!DNL Adobe Workfront Fusion] 시나리오에서는 [!UICONTROL Dropbox] 또는 [!DNL Dropbox Business]을(를) 사용하는 워크플로를 자동화하고 여러 타사 응용 프로그램 및 서비스에 연결할 수 있습니다. 이를 통해 [!UICONTROL Dropbox]에서 파일 및 폴더를 모니터링, 검색, 검색, 나열, 만들기 및 편집과 같은 활동을 자동화할 수 있습니다.

시나리오를 만드는 방법에 대한 지침이 필요하면 [시나리오 만들기 [!DNL Adobe Workfront Fusion]](../../workfront-fusion/scenarios/create-a-scenario.md)를 참조하십시오.

모듈에 대한 자세한 내용은 [의 모듈 [!DNL Adobe Workfront Fusion]](../../workfront-fusion/modules/modules.md)을 참조하세요.

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
   <p>현재 라이선스 요구 사항: [!DNL Workfront Fusion] 라이선스 요구 사항이 없습니다.</p>
   <p>또는</p>
   <p>레거시 라이선스 요구 사항: 작업 자동화 및 통합을 위한 [!UICONTROL [!DNL Workfront Fusion]] </p>
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader">제품</td> 
   <td>
   <p>현재 제품 요구 사항: [!UICONTROL Select] 또는 [!UICONTROL Prime] [!DNL Adobe Workfront] 플랜이 있는 경우 조직에서 이 문서에 설명된 기능을 사용하려면 [!DNL Adobe Workfront Fusion]과(와) [!DNL Adobe Workfront]을(를) 구매해야 합니다. [!DNL Workfront Fusion]이(가) [!UICONTROL Ultimate] [!DNL Workfront] 계획에 포함되어 있습니다.</p>
   <p>또는</p>
   <p>레거시 제품 요구 사항: 이 문서에 설명된 기능을 사용하려면 조직에서 [!DNL Adobe Workfront Fusion]과(와) [!DNL Adobe Workfront]을(를) 구매해야 합니다.</p>
   </td> 
  </tr> 
 </tbody> 
</table>

보유 중인 플랜, 라이선스 유형 또는 액세스 권한을 확인하려면 [!DNL Workfront] 관리자에게 문의하세요.

[!DNL Adobe Workfront Fusion] 라이선스에 대한 자세한 내용은 [[!DNL Adobe Workfront Fusion] 라이선스](../../workfront-fusion/get-started/license-automation-vs-integration.md)를 참조하세요.

## 전제 조건

* [!DNL Dropbox] 모듈을 사용하려면 [!DNL Dropbox] 계정이 있어야 합니다.

>[!IMPORTANT]
>
>Dropbox은 사용자가 50명을 초과하는 응용 프로그램을 승인해야 합니다.
>
>자세한 내용을 보려면 Dropbox 개발자 안내서에서 &quot;프로덕션 승인&quot;을 검색하십시오.

## Dropbox API 정보

Dropbox 커넥터는 다음을 사용합니다.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">기본 URL</td> 
   <td> https://api.dropboxapi.com/2    </td> 
  </tr> 
  <tr> 
   <td role="rowheader">API 버전</td> 
   <td> 2 </td> 
  </tr> 
  <tr> 
   <td role="rowheader">API 태그</td> 
   <td><ul><li><p>Dropbox</p><p>v5.3.9</p></li><li><p>Dropbox Business</p><p>v1.0.12</p></li></ul></td> 
  </tr>
 </tbody> 
 </table>


## [!DNL Dropbox]에 연결 만들기

[!DNL Dropbox] 모듈에 대한 연결을 만들려면:

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
        <tr>
        <td role="rowheader">[!UICONTROL 환경]</td>
        <td>이 연결이 프로덕션 환경용인지 아니면 비프로덕션 환경용인지 선택합니다.</td>
        </tr>
        <tr>
        <td role="rowheader">[!UICONTROL 유형]</td>
        <td>서비스 계정에 연결할지 또는 개인 계정에 연결할지 선택합니다.</td>
        </tr>
        </tr>
        <tr>
        <td role="rowheader">[!UICONTROL 클라이언트 ID]</td>
        <td>[!UICONTROL Dropbox] [!UICONTROL 클라이언트 ID]를 입력합니다. </tr>
        <tr>
        <td role="rowheader">[!UICONTROL 클라이언트 암호]</td>
        <td>[!DNL Dropbox] [!UICONTROL 클라이언트 암호]를 입력하십시오. </td>
        </tr>
        <tr>
        <td role="rowheader">[!UICONTROL 계정 유형]</td>
        <td>개인 Dropbox 계정에 연결할지 아니면 비즈니스(Dropbox 비즈니스) 계정에 연결할지 선택합니다.</td>
        </tr>
      </tbody>
    </table>

1. 연결을 저장하고 모듈로 돌아가려면 **[!UICONTROL 계속]**&#x200B;을 클릭하세요.## [!DNL Dropbox] 모듈 및 해당 필드

## [!DNL Dropbox]개 모듈 및 해당 필드

[!DNL Dropbox] 모듈을 구성할 때 [!DNL Workfront Fusion]에 아래 나열된 필드가 표시됩니다. 앱 또는 서비스의 액세스 수준과 같은 요소에 따라 이러한 필드와 함께 [!DNL Dropbox] 필드가 추가로 표시될 수 있습니다. 모듈의 굵은 제목은 필수 필드를 나타냅니다.

필드나 함수 위에 맵 단추가 표시되면 이 단추를 사용하여 해당 필드에 대한 변수와 함수를 설정할 수 있습니다. 자세한 내용은 [한 모듈에서 다른 모듈로 정보를 매핑 [!DNL Adobe Workfront Fusion]](../../workfront-fusion/mapping/map-information-between-modules.md)을 참조하십시오.

![](assets/map-toggle-350x74.png)

* [트리거 모듈](#trigger-modules)
* [ [!DNL Dropbox] 파일 및 폴더 가져오기 모듈](#modules-for-getting-dropbox-files-and-folders)
* [ [!DNL Dropbox] 파일 및 폴더를 만들고 편집하기 위한 모듈](#modules-for-creating-and-editing-dropbox-files-and-folders)
* [기타 모듈](#other-modules)

### 트리거 모듈

#### [!UICONTROL 파일 보기]

이 트리거 유형 모듈은 지정된 폴더의 파일이 수정되면 파일 세부 정보를 반환합니다.

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL Connection] </td> 
   <td> <p>[!DNL Dropbox] 계정을 [!DNL Workfront Fusion]에 연결하는 방법에 대한 지침은 이 문서에서 <a href="#create-a-connection-to-dropbox" class="MCXref xref">[!DNL Dropbox]</a>에 연결 만들기 를 참조하십시오.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL 폴더] </td> 
   <td> <p>변경 내용을 감시할 폴더를 선택합니다.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Watch 또한 하위 폴더]</td> 
   <td> <p> 선택한 폴더의 하위 폴더에서 수정된 파일을 모니터링하려면 이 옵션을 활성화합니다.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL 제한] </td> 
   <td> <p>각 시나리오 실행 주기 동안 모듈이 반환할 최대 레코드 수를 입력하거나 매핑합니다.</p> </td> 
  </tr> 
 </tbody> 
</table>

### [!DNL Dropbox]개의 파일 및 폴더를 가져오는 모듈

* [[!UICONTROL 파일/폴더 검색]](#search-filesfolders)
* [[!UICONTROL 파일 다운로드]](#download-a-file)
* [[!UICONTROL 폴더 메타데이터 가져오기]](#get-a-folder-metadata)
* [[!UICONTROL 폴더에 있는 모든 파일/하위 폴더 나열]](#list-all-filessubfolders-in-a-folder)
* [[!UICONTROL 파일 수정 버전 나열]](#list-file-revisions)

#### [!UICONTROL 파일/폴더 검색]

이 검색 모듈은 지정한 검색 쿼리와 일치하는 [!DNL Dropbox]의 개체에서 레코드를 찾습니다.

이 정보는 시나리오의 후속 모듈에 매핑할 수 있습니다.

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL Connection] </td> 
   <td> <p>[!DNL Dropbox] 계정을 [!DNL Workfront Fusion]에 연결하는 방법에 대한 지침은 이 문서에서 <a href="#create-a-connection-to-dropbox" class="MCXref xref">[!DNL Dropbox]</a>에 연결 만들기 를 참조하십시오.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Search] </td> 
   <td> <p>검색어를 입력합니다.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL 폴더] </td> 
   <td> <p>검색할 폴더를 선택합니다. 폴더를 선택하지 않으면 이 모듈은 전체 [!DNL Dropbox]을(를) 검색합니다.</p> </td> 
  </tr> 
  <tr> 
   <td>파일 상태</td> 
   <td> <p> 검색을 선택한 파일 상태로 제한하려면 파일 상태를 선택합니다.</p> </td> 
  </tr> 
  <tr> 
   <td>파일 범주</td> 
   <td> <p> 선택한 범주로 검색을 제한하려면 파일 범주를 선택합니다.</p> </td> 
  </tr> 
  <tr> 
   <td>파일 확장명</td> 
   <td> <p> 검색할 파일 확장자를 선택합니다.</p> </td> 
  </tr> 
  <tr> 
   <td>제한 </td> 
   <td> <p>각 시나리오 실행 주기 동안 모듈이 반환할 최대 레코드 수를 입력하거나 매핑합니다.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL 파일 다운로드]

이 작업 모듈은 폴더에서 파일을 다운로드합니다.

파일과 해당 위치를 지정합니다.

모듈은 파일의 ID와 연결된 필드, 그리고 연결이 액세스하는 모든 사용자 지정 필드 및 값을 반환합니다. 이 정보는 시나리오의 후속 모듈에 매핑할 수 있습니다.

>[!NOTE]
>
>이 모듈은 파일을 후속 모듈에 제공하는 데 유용합니다.

이 모듈을 구성할 때 다음 필드가 표시됩니다.

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL Connection] </td> 
   <td> <p>[!DNL Dropbox] 계정을 [!DNL Workfront Fusion]에 연결하는 방법에 대한 지침은 이 문서에서 <a href="#create-a-connection-to-dropbox" class="MCXref xref">[!DNL Dropbox]</a>에 연결 만들기 를 참조하십시오.</p> </td> 
  </tr> 
  <tr> 
   <td>파일 선택 방법</td> 
   <td> <p> 파일 경로를 매핑할지 또는 수동으로 파일을 선택할지 선택합니다.</p> </td> 
  </tr> 
  <tr> 
   <td> <p>파일 경로 / 파일</p> </td> 
   <td> <p style="font-weight: bold;">파일 경로</p> <p>대상 경로를 입력하거나 파일에 매핑합니다.</p> <p style="font-weight: bold;">파일</p> <p>메뉴에서 파일을 선택합니다.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL 폴더 메타데이터 가져오기]

이 작업 모듈은 공유 폴더 세부 정보를 검색합니다.

폴더의 ID를 지정합니다.

모듈은 연결이 액세스하는 사용자 지정 필드 및 값과 함께 폴더 ID 및 연결된 필드를 반환합니다. 이 정보는 시나리오의 후속 모듈에 매핑할 수 있습니다.

이 모듈을 구성할 때 다음 필드가 표시됩니다.

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL Connection] </td> 
   <td> <p>[!DNL Dropbox] 계정을 [!DNL Workfront Fusion]에 연결하는 방법에 대한 지침은 이 문서에서 <a href="#create-a-connection-to-dropbox" class="MCXref xref">[!DNL Dropbox]</a>에 연결 만들기 를 참조하십시오.</p> </td> 
  </tr> 
  <tr> 
   <td>공유 폴더 ID</td> 
   <td> <p> 세부 정보를 검색할 폴더의 ID를 입력하거나 매핑합니다.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL 폴더에 있는 모든 파일/하위 폴더 나열]

이 작업 모듈은 특정 폴더에 있는 파일 또는 폴더를 나열합니다.

폴더의 ID를 지정합니다.

이 모듈은 파일 또는 폴더의 ID와 연결된 필드를 연결이 액세스하는 사용자 지정 필드 및 값과 함께 반환합니다. 이 정보는 시나리오의 후속 모듈에 매핑할 수 있습니다.

이 모듈을 구성할 때 다음 필드가 표시됩니다.

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL Connection] </td> 
   <td> <p>[!DNL Dropbox] 계정을 [!DNL Workfront Fusion]에 연결하는 방법에 대한 지침은 이 문서에서 <a href="#create-a-connection-to-dropbox" class="MCXref xref">[!DNL Dropbox]</a>에 연결 만들기 를 참조하십시오.</p> </td> 
  </tr> 
  <tr> 
   <td>목록 </td> 
   <td> <p>파일 또는 폴더를 검색할지 선택합니다.</p> </td> 
  </tr> 
  <tr> 
   <td>다운로드 가능한 파일만 표시</td> 
   <td> <p> 다운로드 가능한 파일만 반환하려면 이 옵션을 활성화합니다. Google Docs와 같은 일부 유형의 파일은 다운로드할 수 없습니다.</p> </td> 
  </tr> 
  <tr> 
   <td>폴더 </td> 
   <td> <p>파일 또는 폴더를 검색할 폴더를 입력하거나 매핑합니다.</p> </td> 
  </tr> 
  <tr> 
   <td>제한 </td> 
   <td> <p>각 시나리오 실행 주기 동안 모듈이 나열할 최대 레코드 수를 입력하거나 매핑합니다.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL 파일 수정 버전 나열]

이 작업 모듈은 특정 파일의 모든 파일 개정 버전(버전 내역)을 검색합니다.\
파일의 ID를 지정합니다.

모듈은 연결에서 액세스하는 모든 사용자 지정 필드 및 값과 함께 레코드와 연결된 모든 표준 필드를 반환합니다. 이 정보는 시나리오의 후속 모듈에 매핑할 수 있습니다.

이 모듈을 구성할 때 다음 필드가 표시됩니다.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL Connection] </td> 
   <td> <p>[!DNL Dropbox] 계정을 [!DNL Workfront Fusion]에 연결하는 방법에 대한 지침은 이 문서에서 <a href="#create-a-connection-to-dropbox" class="MCXref xref">[!DNL Dropbox]</a>에 연결 만들기 를 참조하십시오.</p> </td> 
  </tr> 
  <tr> 
   <td>파일 선택 방법</td> 
   <td> <p> 파일 경로를 매핑할지 또는 수동으로 파일을 선택할지 선택합니다.</p> </td> 
  </tr> 
  <tr> 
   <td> <p>파일 경로 / 파일</p> </td> 
   <td> <p style="font-weight: bold;">파일 경로</p> <p>대상 경로를 입력하거나 파일에 매핑합니다.</p> <p style="font-weight: bold;">파일</p> <p>메뉴에서 파일을 선택합니다.</p> </td> 
  </tr> 
  <tr> 
   <td> <p>제한</p> </td> 
   <td> <p>각 시나리오 실행 주기 동안 모듈이 나열할 최대 레코드 수를 입력하거나 매핑합니다.</p> </td> 
  </tr> 
 </tbody> 
</table>

### [!DNL Dropbox]개의 파일 및 폴더를 만들고 편집하는 모듈입니다.

* [파일 [!UICONTROL 업로드]](#upload-a-file)
* [[!UICONTROL 폴더 만들기]](#create-a-folder)
* [[!UICONTROL 텍스트 파일 만들기/덮어쓰기]](#createoverwrite-a-text-file)
* [[!UICONTROL 공유 링크 만들기/업데이트]](#createupdate-a-share-link)
* [[!UICONTROL 파일 복원]](#restore-a-file)
* [[!UICONTROL 파일/폴더 이동]](#move-a-filefolder)
* [[!UICONTROL 파일/폴더 이름 바꾸기]](#rename-a-filefolder)
* [[!UICONTROL 파일/폴더 삭제]](#delete-a-filefolder)

#### [!UICONTROL 파일 업로드]

이 작업 모듈은 파일을 폴더로 업로드합니다.

파일 위치, 업로드할 파일 및 파일의 새 이름(선택 사항)과 같은 정보를 지정합니다.

모듈은 파일의 ID와 연결된 필드, 그리고 연결이 액세스하는 모든 사용자 지정 필드 및 값을 반환합니다. 이 정보는 시나리오의 후속 모듈에 매핑할 수 있습니다.

이 모듈을 구성할 때 다음 필드가 표시됩니다.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL Connection] </td> 
   <td> <p>[!DNL Dropbox] 계정을 [!DNL Workfront Fusion]에 연결하는 방법에 대한 지침은 이 문서에서 <a href="#create-a-connection-to-dropbox" class="MCXref xref">[!DNL Dropbox]</a>에 연결 만들기 를 참조하십시오.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL 폴더]</td> 
   <td> <p> 파일을 업로드할 [!DNL Dropbox]의 폴더를 선택하십시오.</p> </td> 
  </tr> 
  <tr> 
   <td> <p>[!UICONTROL Source 파일]</p> </td> 
   <td> <p>위에서 선택한 [!DNL Dropbox] 폴더에 추가할 파일을 입력하거나 매핑합니다.</p> <p style="font-weight: bold;">[!UICONTROL 파일 이름]</p> <p>파일 확장자를 포함하여 파일 이름을 입력하거나 매핑합니다.</p> <p style="font-weight: bold;">[!UICONTROL 파일 데이터]</p> <p>파일 데이터([!UICONTROL Google Drive] &gt;[!UICONTROL 파일 가져오기)와 같은 이전 모듈의)를 입력하거나 매핑합니다.</p> <p>참고: 업로드된 파일의 최대 크기는 150MB입니다.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL 기존 파일 덮어쓰기]</td> 
   <td> <p> 기존 파일을 새 파일로 바꾸려면 이 옵션을 활성화합니다. 이 옵션을 비활성화하면 업로드된 파일의 이름이 바뀝니다.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL 폴더 만들기]

이 작업 모듈은 새 폴더를 만듭니다.

폴더의 경로 및 이름을 지정합니다.

모듈은 연결이 액세스하는 사용자 지정 필드 및 값과 함께 폴더 ID 및 연결된 필드를 반환합니다. 이 정보는 시나리오의 후속 모듈에 매핑할 수 있습니다.

이 모듈을 구성할 때 다음 필드가 표시됩니다.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL Connection] </td> 
   <td> <p>[!DNL Dropbox] 계정을 [!DNL Workfront Fusion]에 연결하는 방법에 대한 지침은 이 문서에서 <a href="#create-a-connection-to-dropbox" class="MCXref xref">[!DNL Dropbox]</a>에 연결 만들기 를 참조하십시오.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL 폴더 이름] </td> 
   <td> <p>새 폴더의 이름을 입력합니다.</p> </td> 
  </tr> 
  <tr> 
   <td> <p>[!UICONTROL 폴더]</p> </td> 
   <td> <p>새 폴더를 만들 경로를 입력하거나 매핑합니다.</p> <p>참고:   <p>[!DNL Dropbox Business] 계정(팀 공간 포함)을 사용하는 경우 슬래시 <code>/</code>을(를) 제거하거나 <strong>[!UICONTROL 여기를 클릭]하여 폴더를 선택</strong>하여 루트에 팀 폴더를 만들어야 합니다.</p> <p>슬래시가 제거되지 않으면 오류 <code>[409] path/malformed_path/..</code>이(가) 반환됩니다.</p> </p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL 자동 이름 변경]</td> 
   <td> <p> 대상 위치에 이름이 같은 폴더가 이미 있는 경우 새 폴더의 이름을 변경하려면 이 옵션을 활성화합니다.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL 텍스트 파일 만들기/덮어쓰기]

이 작업 모듈은 DOC 파일을 만들거나 기존 파일의 콘텐츠를 덮어씁니다.

소스 파일과 폴더를 지정합니다.

모듈은 연결이 액세스하는 사용자 지정 필드 및 값과 함께 폴더 ID 및 연결된 필드를 반환합니다. 이 정보는 시나리오의 후속 모듈에 매핑할 수 있습니다.

이 모듈을 구성할 때 다음 필드가 표시됩니다.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL Connection] </td> 
   <td> <p>[!DNL Dropbox] 계정을 [!DNL Workfront Fusion]에 연결하는 방법에 대한 지침은 이 문서에서 <a href="#create-a-connection-to-dropbox" class="MCXref xref">[!DNL Dropbox]</a>에 연결 만들기 를 참조하십시오.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Select to]</td> 
   <td> <p> DOC 파일을 작성할지 또는 덮어쓸지 여부를 선택합니다.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL 폴더] </td> 
   <td> <p>파일을 만들 대상 위치를 선택합니다.</p> </td> 
  </tr> 
  <tr> 
   <td> <p>[!UICONTROL Source 파일]</p> </td> 
   <td> <p>추가할 파일을 [!DNL Dropbox] 폴더에 입력하거나 매핑합니다.</p> <p style="font-weight: bold;">파일 이름</p> <p>확장명 없이 새 DOC 파일의 파일 이름을 입력합니다.</p> <p style="font-weight: bold;">파일 컨텐츠</p> <p>DOC 파일의 텍스트 내용을 입력합니다.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL 공유 링크 만들기/업데이트]

이 작업 모듈은 파일에 대한 공개 링크를 만듭니다.

파일 및 링크에 대한 정보를 지정합니다.

모듈은 연결이 액세스하는 사용자 지정 필드 및 값과 함께 링크의 ID 및 연결된 필드를 반환합니다. 이 정보는 시나리오의 후속 모듈에 매핑할 수 있습니다.

이 모듈을 구성할 때 다음 필드가 표시됩니다.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL Connection] </td> 
   <td> <p>[!DNL Dropbox] 계정을 [!DNL Workfront Fusion]에 연결하는 방법에 대한 지침은 이 문서에서 <a href="#create-a-connection-to-dropbox" class="MCXref xref">[!DNL Dropbox]</a>에 연결 만들기 를 참조하십시오.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL 파일 선택 방법]</td> 
   <td> <p> 파일 경로를 매핑할지 또는 입력할지를 선택하거나 파일을 수동으로 선택합니다.</p> </td> 
  </tr> 
  <tr> 
   <td> <p>[!UICONTROL 파일 경로 / 파일]</p> </td> 
   <td> <p style="font-weight: bold;">[!UICONTROL 파일 경로]</p> <p>대상 경로를 입력하거나 파일에 매핑합니다.</p> <p style="font-weight: bold;">[!UICONTROL 파일]</p> <p>메뉴에서 파일을 선택합니다.</p> </td> 
  </tr> 
  <tr> 
   <td> <p>[!UICONTROL 요청된 가시성]</p> </td> 
   <td> <p>링크가 공개 링크인지 팀 링크인지 암호 제한인지 선택합니다.</p> <p>참고: [!UICONTROL Team only] 및 [!UICONTROL Access with password] 옵션은 [!DNL Dropbox Pro] 이상 버전을 가진 사용자만 사용할 수 있습니다.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL 링크의 만료 날짜]</td> 
   <td> <p> 링크가 만료되어 더 이상 액세스할 수 없게 되는 날짜 및 시간을 입력합니다. 이 필드를 비워 두면 링크가 만료되지 않습니다. 지원되는 날짜 및 시간 형식 목록을 보려면 [!DNL Adobe Workfront Fusion]</a>의 <a href="../../workfront-fusion/mapping/type-coercion.md" class="MCXref xref" data-mc-variable-override="">형식 변환을 참조하십시오.</p> <p>참고: [!UICONTROL Team only] 및 [!UICONTROL Access with password] 옵션은 [!UICONTROL Dropbox Pro] 이상 버전을 보유한 사용자만 사용할 수 있습니다.</p> </td> 
  </tr> 
  <tr> 
   <td> <p>[!UICONTROL 링크의 액세스 수준]</p> </td> 
   <td> <p>링크 수신자에 대한 권한을 설정합니다.</p> <p>링크를 사용하는 <strong>[!UICONTROL 뷰어]</strong> 사용자는 콘텐츠를 보고 댓글을 달 수 있습니다.</p> <p>링크를 사용하는 <strong>[!UICONTROL Editor]</strong> 사용자는 콘텐츠를 편집하고 보고 댓글을 달 수 있습니다.</p> <p>링크를 사용하는 <strong>[!UICONTROL Max]</strong> 사용자는 링크를 설정할 수 있는 최대 액세스 수준을 받습니다.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL 파일 복원]

이 작업 모듈은 파일의 이전 버전을 복원합니다.

원하는 파일 및 개정 번호를 지정합니다.

이 모듈은 버전 ID 및 연결된 모든 필드를, 연결이 액세스하는 모든 사용자 지정 필드 및 값과 함께 반환합니다. 이 정보는 시나리오의 후속 모듈에 매핑할 수 있습니다.

이 모듈을 구성할 때 다음 필드가 표시됩니다.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL Connection] </td> 
   <td> <p>[!DNL Dropbox] 계정을 [!DNL Workfront Fusion]에 연결하는 방법에 대한 지침은 이 문서에서 <a href="#create-a-connection-to-dropbox" class="MCXref xref">[!DNL Dropbox]</a>에 연결 만들기 를 참조하십시오.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL 파일 선택 방법]</td> 
   <td> <p> 파일 경로를 매핑할지 또는 입력할지를 선택하거나 파일을 수동으로 선택합니다.</p> </td> 
  </tr> 
  <tr> 
   <td> <p>[!UICONTROL 파일 경로] / [!UICONTROL 파일]</p> </td> 
   <td> <p><strong>[!UICONTROL 파일 경로]</strong> </p> <p>대상 경로를 입력하거나 파일에 매핑합니다.</p> <p><strong>[!UICONTROL 파일]</strong> </p> <p>메뉴에서 파일을 선택합니다.</p> </td> 
  </tr> 
  <tr> 
   <td> <p>[!UICONTROL Revision]</p> </td> 
   <td> <p>복원할 개정의 개정 번호를 입력하거나 매핑합니다.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL 파일/폴더 이동]

이 작업 모듈은 파일 또는 폴더를 다른 위치로 이동합니다.

파일 또는 폴더와 그 이동 방법 및 위치를 지정합니다.

모듈은 파일 또는 폴더의 ID와 연결된 필드를 연결이 액세스하는 사용자 지정 필드 및 값과 함께 반환합니다. 이 정보는 시나리오의 후속 모듈에 매핑할 수 있습니다.

이 모듈을 구성할 때 다음 필드가 표시됩니다.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL Connection] </td> 
   <td> <p>[!DNL Dropbox] 계정을 [!DNL Workfront Fusion]에 연결하는 방법에 대한 지침은 이 문서에서 <a href="#create-a-connection-to-dropbox" class="MCXref xref">[!DNL Dropbox]</a>에 연결 만들기 를 참조하십시오.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL 파일 선택 방법] </td> 
   <td> <p>파일 경로를 매핑할지 또는 입력할지를 선택하거나 파일을 수동으로 선택합니다.</p> </td> 
  </tr> 
  <tr> 
   <td> <p>[!UICONTROL 파일/폴더 경로] / [!UICONTROL 파일/폴더]</p> </td> 
   <td> <p style="font-weight: bold;">[!UICONTROL 파일/폴더 경로]</p> <p>파일 또는 폴더에 대상 경로를 입력하거나 매핑합니다.</p> <p style="font-weight: bold;">[!UICONTROL 파일/폴더]</p> <p>메뉴에서 파일 또는 폴더를 선택합니다.</p> </td> 
  </tr> 
  <tr> 
   <td> <p>[!UICONTROL To Folder]</p> </td> 
   <td> <p>파일 또는 폴더의 대상 위치를 입력하거나 매핑합니다.</p> </td> 
  </tr> 
  <tr> 
   <td> <p>[!UICONTROL 새 이름]</p> </td> 
   <td> <p>새 위치에 파일 또는 폴더의 새 이름을 입력합니다.</p> </td> 
  </tr> 
  <tr> 
   <td> <p>[!UICONTROL 자동 이름 바꾸기]</p> </td> 
   <td> <p>이 옵션을 활성화하면 동일한 이름의 파일 또는 폴더가 있는 경우 모듈에서 파일 또는 폴더 이름 뒤에 ([!UICONTROL NUMBER])를 추가하여 새 파일 또는 폴더의 이름을 바꿉니다. 그렇지 않으면 대상 위치의 파일 또는 폴더를 덮어씁니다.</p> </td> 
  </tr> 
  <tr> 
   <td> <p>[!UICONTROL 소유권 이전 허용]</p> </td> 
   <td> <p>이 옵션을 활성화하면 이동하는 컨텐츠에 대한 소유권 이전이 발생하는 경우에도 소유자가 이동할 수 있습니다.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL 파일/폴더 이름 바꾸기]

이 작업 모듈은 파일 또는 폴더의 이름을 변경합니다.

파일 또는 폴더와 새 이름을 지정합니다.

모듈은 파일 또는 폴더의 ID와 연결된 필드를 연결이 액세스하는 사용자 지정 필드 및 값과 함께 반환합니다. 이 정보는 시나리오의 후속 모듈에 매핑할 수 있습니다.

이 모듈을 구성할 때 다음 필드가 표시됩니다.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL Connection] </td> 
   <td> <p>[!DNL Dropbox] 계정을 [!DNL Workfront Fusion]에 연결하는 방법에 대한 지침은 이 문서에서 <a href="#create-a-connection-to-dropbox" class="MCXref xref">[!DNL Dropbox]</a>에 연결 만들기 를 참조하십시오.</p> </td> 
  </tr> 
  <tr> 
   <td>파일 선택 방법</td> 
   <td> <p> 파일 경로를 매핑할지 또는 입력할지를 선택하거나 파일을 수동으로 선택합니다.</p> </td> 
  </tr> 
  <tr> 
   <td> <p>파일/폴더 경로/파일/폴더</p> </td> 
   <td> <p style="font-weight: bold;">파일/폴더 경로</p> <p>파일 또는 폴더에 대상 경로를 입력하거나 매핑합니다.</p> <p style="font-weight: bold;">파일/폴더</p> <p>메뉴에서 파일 또는 폴더를 선택합니다.</p> </td> 
  </tr> 
  <tr> 
   <td>이름 바꾸기 </td> 
   <td> <p>파일 확장명을 포함하여 파일에 대한 [!UICONTROL 대상 이름]을 입력합니다.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL 파일/폴더 삭제]

이 작업 모듈은 파일 또는 폴더를 삭제합니다.

파일 또는 폴더를 지정합니다.

모듈은 연결에서 액세스하는 사용자 지정 필드 및 값과 함께 레코드 및 관련 필드의 ID를 반환합니다. 이 정보는 시나리오의 후속 모듈에 매핑할 수 있습니다.

이 모듈을 구성할 때 다음 필드가 표시됩니다.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL Connection] </td> 
   <td> <p>[!DNL Dropbox] 계정을 [!DNL Workfront Fusion]에 연결하는 방법에 대한 지침은 이 문서에서 <a href="#create-a-connection-to-dropbox" class="MCXref xref">[!DNL Dropbox]</a>에 연결 만들기 를 참조하십시오.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL 파일 선택 방법]</td> 
   <td> <p> 파일 경로를 매핑할지 또는 입력할지를 선택하거나 파일을 수동으로 선택합니다.</p> </td> 
  </tr> 
  <tr> 
   <td> <p>[!UICONTROL 파일 경로] / [!UICONTROL 파일]</p> </td> 
   <td> <p style="font-weight: bold;">[!UICONTROL 파일 경로]</p> <p>대상 경로를 입력하거나 파일에 매핑합니다.</p> <p style="font-weight: bold;">[!UICONTROL 파일]</p> <p>메뉴에서 파일을 선택합니다.</p> </td> 
  </tr> 
 </tbody> 
</table>

### 기타 모듈

#### [!UICONTROL API 호출 만들기]

이 작업 모듈을 사용하면 [!DNL Dropbox] API에 대해 사용자 지정 인증된 호출을 수행할 수 있습니다. 이렇게 하면 다른 [!DNL Dropbox] 모듈에서 수행할 수 없는 데이터 흐름 자동화를 만들 수 있습니다.

이 모듈을 구성할 때 다음 필드가 표시됩니다.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL Connection] </td> 
   <td> <p>[!DNL Dropbox] 계정을 [!DNL Workfront Fusion]에 연결하는 방법에 대한 지침은 이 문서에서 <a href="#create-a-connection-to-dropbox" class="MCXref xref">[!DNL Dropbox]</a>에 연결 만들기 를 참조하십시오.</p> </td> 
  </tr> 
  <tr> 
   <td> <p>[!UICONTROL URL]</p> </td> 
   <td> <p>상대 경로를 입력하십시오. <code>https://api.dropboxapi.com</code>을(를) 기준으로 한 경로를 입력하십시오. For example, <code>/2/files/list_folder</code></p> <p>참고: 사용 가능한 끝점 목록은 <a href="https://www.dropbox.com/developers/documentation/http/documentation">Dropbox API v2 설명서</a>를 참조하세요.</p> </td> 
  </tr> 
  <tr> 
   <td> <p>[!UICONTROL 메서드]</p> </td> 
   <td> <p>API 호출을 구성하는 데 필요한 HTTP 요청 메서드를 선택합니다. 자세한 내용은 [!DNL Adobe Workfront Fusion]</a>에서 <a href="../../workfront-fusion/modules/http-request-methods.md" class="MCXref xref" data-mc-variable-override="">HTTP 요청 메서드를 참조하십시오.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Headers] </td> 
   <td> <p>원하는 요청 헤더를 입력합니다. [!DNL Workfront Fusion]이(가) 인증 헤더를 자동으로 추가합니다.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL 쿼리 문자열]</td> 
   <td> <p> 요청 쿼리 문자열을 입력합니다.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Body] </td> 
   <td> <p>표준 JSON 개체의 형태로 API 호출에 대한 본문 콘텐츠를 추가합니다.</p> <p>참고:   <p>JSON에서 <code>if</code>과(와) 같은 조건문을 사용할 때 따옴표를 조건문 외부에 넣으십시오.</p> 
     <div class="example" data-mc-autonum="<b>Example: </b>">  
      <p> <img src="assets/quotes-in-json-350x120.png" style="width: 350;height: 120;"> </p> 
     </div> </p> </td> 
  </tr> 
 </tbody> 
</table>

>[!INFO]
>
>**예:** 다음 API 호출은 [!DNL Dropbox] 계정의 [!DNL /Text files] 폴더에서 처음 10개의 파일을 반환합니다.
>
>URL: `/2/files/list_folder`
>
>본문:
> 
>`{`
>
>`"path": "/Text files",`
>
>`"limit": 10,`
>
>`"recursive": false,`
>
>`"include_deleted": false`
>
>`}`
>
>검색 일치 항목은 [!UICONTROL 번들] > [!UICONTROL 본문] > 항목 아래의 모듈 출력에서 찾을 수 있습니다.
>
>이 예에서는 10개의 티켓이 반환되었습니다.

## 일반적인 문제

* [파일을 업로드하거나 업데이트할 수 없음](#unable-to-upload-or-update-a-file)
* [공유 링크를 통해 참조된 이미지가 렌더링되지 않음](#image-referenced-via-a-shared-link-does-not-render)

### 파일을 업로드하거나 업데이트할 수 없음

파일 업로드 또는 업데이트가 실패할 경우 다음과 같은 몇 가지 상황이 발생합니다.

* 업로드한 파일이 너무 커서 [!DNL Dropbox] 계획에 허용된 최대 파일 크기를 초과하거나 [!DNL Dropbox] 계정의 저장소 할당량을 모두 사용했습니다. [!DNL Dropbox] 계정에서 기존 파일을 삭제하거나 플랜을 업그레이드해야 합니다.
* 이전에 선택한 파일 업로드 대상 폴더는 더 이상 존재하지 않습니다. 시나리오가 중지되며 대상 폴더를 다시 선택해야 합니다.

### 공유 링크를 통해 참조된 이미지가 렌더링되지 않음

[!UICONTROL Dropbox] >[!UICONTROL 공유 링크 만들기]에서 반환된 URL은 이미지에 직접 연결되지 않고 [!DNL Dropbox] 페이지로 연결됩니다. 이미지를 강제로 다운로드하려면 후행 `?dl=0`을(를) `?dl=1`(으)로 바꾸십시오. 이미지를 렌더링하려면(예: 웹 브라우저나 Facebook Messenger에서) URL에 `&raw=1`을(를) 추가하십시오.

웹 사이트 또는 다른 [!DNL Workfront Fusion] 모듈에 대한 이미지의 직접 또는 원시 링크를 가져와야 하는 경우 다음과 같은 방법으로 초기 공유 URL을 수정해야 합니다.

원래 URL:

`https://www.dropbox.com/s/ia8qtvs20f3a5ux/Screen%20Shot%202018-10-15%20at%204.21.11%20PM.png?dl=0`

1. `www`에서 `dl`(으)로 바꾸기
1. `?dl=0` 제거.

최종 URL:

`https://dl.dropbox.com/s/ia8qtvs20f3a5ux/Screen%20Shot%202018-10-15%20at%204.21.11%20PM.png`

URL을 자동으로 수정하려면 `replace()` 함수를 두 번 사용합니다.

* www를 dl로 바꾸기

  ![](assets/www-to-dl-350x32.png)

* ?dl=0 제거

  ![](assets/remove-dl0-350x33.png)

한 단계로 진행하려면 다음 함수를 결합합니다.

![](assets/replace-both-350x47.png)

복사하여 필드에 붙여넣을 수도 있습니다. `1.url`을(를) URL로 바꾸십시오.

```
{{replace(replace(1.url; "?dl=0"; ""); "www"; "dl")}}
```
