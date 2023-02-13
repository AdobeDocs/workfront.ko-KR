---
content-type: reference
product-previous: workfront-fusion
product-area: workfront-integrations;documents
keywords: 커넥터
navigation-topic: apps-and-their-modules
title: Microsoft OneDrive 모듈
description: 에서 [!DNL Adobe Workfront Fusion] 시나리오 OneDrive를 사용하는 워크플로우를 자동화하고 여러 타사 애플리케이션 및 서비스에 연결할 수 있습니다.
author: Becky
feature: Workfront Fusion
exl-id: 13a25c6c-bdf1-467d-bd90-ebd763c59235
source-git-commit: 885d93dd4383945538e977fd3edbfd55bda88b70
workflow-type: tm+mt
source-wordcount: '3934'
ht-degree: 0%

---

# [!DNL Microsoft OneDrive] 모듈

에서 [!DNL Adobe Workfront Fusion] 시나리오, [!DNL OneDrive]여러 타사 애플리케이션 및 서비스에 연결할 수 있습니다.

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

를 사용하려면 [!DNL OneDrive] 모듈이면 반드시 [!DNL Microsoft OneDrive] 계정이 필요합니다.

## 연결 [!DNL OneDrive] 서비스 대상 [!DNL Workfront Fusion]

연결 방법에 대한 지침은 [!DNL OneDrive] 계정 대상 [!UICONTROL Workfront Fusion]를 참조하십시오. [연결 만들기 [!UICONTROL Adobe Workfront Fusion] - 기본 지침](../../workfront-fusion/connections/connect-to-fusion-general.md)

## [!DNL Microsoft OneDrive] 모듈 및 해당 필드

구성 시 [!DNL OneDrive] 모듈, [!DNL Workfront Fusion] 아래 나열된 필드를 표시합니다. 이와 함께 추가 [!DNL OneDrive] 앱이나 서비스에서 액세스 수준과 같은 요소에 따라 필드가 표시될 수 있습니다. 모듈에서 굵게 표시된 제목은 필수 필드를 나타냅니다.

필드 또는 함수 위에 맵 단추가 표시되면 이 단추를 사용하여 해당 필드에 대한 변수와 함수를 설정할 수 있습니다. 자세한 내용은 [의 한 모듈에서 다른 모듈로 정보 매핑 [!DNL Adobe Workfront Fusion]](../../workfront-fusion/mapping/map-information-between-modules.md).

![](assets/map-toggle-350x74.png)

* [파일/폴더](#filefolder)
* [기타](#other)

### 파일/폴더

* [[!UICONTROL 감시 파일/폴더]](#watch-filesfolders)
* [[!UICONTROL 파일/폴더 검색]](#search-filesfolders)
* [[!UICONTROL 파일 가져오기]](#get-a-file)
* [[!UICONTROL 파일 다운로드]](#download-a-file)
* [[!UICONTROL 파일 업로드]](#upload-a-file)
* [[!UICONTROL 폴더 만들기]](#create-a-folder)
* [[!UICONTROL 공유 링크 가져오기]](#get-a-share-link)
* [[!UICONTROL 파일/폴더 이동]](#move-a-filefolder)
* [[!UICONTROL 파일 복사]](#copy-a-file)
* [[!UICONTROL 파일/폴더 삭제]](#delete-a-filefolder)

#### [!UICONTROL 감시 파일/폴더]

이 트리거 모듈은 파일 또는 폴더를 만들거나 업데이트할 때 시나리오를 시작합니다.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td> 
   <td>연결 방법에 대한 지침은 [!DNL OneDrive] 계정 대상 [!DNL Workfront Fusion]를 참조하십시오. <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">연결 만들기 [!DNL Adobe Workfront Fusion] - 기본 지침</a></td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Watch 파일/폴더]</td> 
   <td> <p>파일 또는 폴더를 보는 방법을 선택합니다.</p> 
    <ul> 
     <li> <p><b>[!UICONTROL By Created Time]</b> </p> <p>새 파일 또는 폴더를 확인하십시오.</p> </li> 
     <li> <p><b>[!UICONTROL By Updated Time]</b> </p> <p>업데이트된 기존 파일 또는 폴더를 확인하십시오.</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL [!DNL OneDrive] 위치]</td> 
   <td> <p>보려는 위치 선택:</p> 
    <ul> 
     <li> <p><b>[!UICONTROL My Drive]</b> </p> <p>모듈에서 드라이브 ID를 입력하도록 할지 여부를 선택합니다.</p> 
      <ul> 
       <li> <p><b>[!UICONTROL Yes]</b> </p> <p>모듈을 볼 드라이브의 ID를 입력합니다.</p> </li> 
       <li> <p><b>[!UICONTROL No]</b> </p> <p>모듈에서 볼 폴더로 이동합니다. 쿼리를 입력하여 반환된 결과를 필터링할 수도 있습니다.</p> </li> 
      </ul> </li> 
     <li> <p><b>[!UICONTROL Shared With Me]</b> </p> <p>모듈은 드라이브 소유자와 공유된 파일을 확인합니다.</p> </li> 
     <li> <p><b>[!UICONTROL Site's Drive]</b> </p> <p>모듈에서 볼 SharePoint 사이트를 선택합니다. 사용 가능한 사이트는 사이트 다음에 로그인한 사용자가 옵니다.</p> </li> 
     <li> <p><b>[!UICONTROL 그룹 드라이브]</b> </p> <p>모듈을 볼 드라이브를 가진 그룹을 선택합니다.</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL 항목 유형 선택]</td> 
   <td> <p>파일, 폴더 또는 둘 다를 감시할지 여부를 선택합니다.</p> <p>참고: [!UICONTROL Shared With Me] 드라이브에 있는 폴더는 볼 수 없습니다.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL 제한]</td> 
   <td> <p>각 시나리오 실행 주기 동안 모듈이 반환할 최대 레코드 수를 입력하거나 매핑합니다.</p> </td> 
  </tr> 
 </tbody> 
</table>



#### [!UICONTROL 파일/폴더 검색]

이 검색 모듈은 설정한 기준에 따라 파일 및 폴더를 반환합니다.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td> 
   <td>연결 방법에 대한 지침은 [!DNL OneDrive] 계정 대상 [!DNL Workfront Fusion]를 참조하십시오. <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">연결 만들기 [!DNL Adobe Workfront Fusion] - 기본 지침</a></td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL [!DNL OneDrive] 위치]</td> 
   <td> <p>검색할 위치를 선택합니다.</p> 
    <ul> 
     <li> <p><b>[!UICONTROL My Drive]</b> </p> <p>모듈에서 드라이브 ID를 입력하도록 할지 여부를 선택합니다.</p> 
      <ul> 
       <li> <p><b>[!UICONTROL Yes]</b> </p> <p>모듈을 검색할 드라이브의 ID를 입력합니다.</p> </li> 
       <li> <p><b>[!UICONTROL No]</b> </p> <p>모듈이 검색할 폴더로 이동합니다. 쿼리를 입력하여 반환된 결과를 필터링할 수도 있습니다.</p> </li> 
      </ul> </li> 
     <li> <p><b>[!UICONTROL Shared With Me]</b> </p> <p>이 모듈은 드라이브 소유자와 공유된 파일을 검색합니다.</p> </li> 
     <li> <p><b>[!UICONTROL Site's Drive]</b> </p> <p>을(를) 선택합니다 [!DNL SharePoint] 모듈이 검색할 사이트입니다. 사용 가능한 사이트는 사이트 다음에 로그인한 사용자가 옵니다.</p> </li> 
     <li> <p><b>[!UICONTROL 그룹 드라이브]</b> </p> <p>모듈을 검색할 드라이브가 있는 그룹을 선택합니다.</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL 항목 유형 선택]</td> 
   <td> <p>파일, 폴더 또는 둘 다를 검색할지 여부를 선택합니다.</p> <p>참고: [!UICONTROL Shared With Me] 드라이브에서 폴더를 검색할 수 없습니다.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL 제한]</td> 
   <td> <p>각 시나리오 실행 주기 동안 모듈이 반환할 최대 레코드 수를 입력하거나 매핑합니다.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL 파일 가져오기]

이 작업 모듈은 지정된 파일의 메타데이터를 가져옵니다.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td> 
   <td>연결 방법에 대한 지침은 [!DNL OneDrive] 계정 대상 [!DNL Workfront Fusion]를 참조하십시오. <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">연결 만들기 [!DNL Adobe Workfront Fusion] - 기본 지침</a></td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Enter(파일 ID 및 파일 경로)]</td> 
   <td>파일을 파일 ID 또는 파일 경로로 식별할지 선택합니다.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL 파일 ID 입력] / [!UICONTROL 파일 경로]</td> 
   <td> <p>파일 ID 또는 파일 경로를 입력할 방법을 선택합니다.</p> 
    <ul> 
     <li> <p><b>[!UICONTROL 수동으로 입력]</b> </p> <p>ID 또는 경로를 직접 입력하거나 이전 모듈에서 매핑하려면 이 옵션을 선택합니다.</p> </li> 
     <li> <p><b>[!UICONTROL 목록에서 선택]</b> </p> <p>사용 가능한 파일 또는 경로 목록에서 선택하려면 이 옵션을 선택합니다. </p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL [!DNL OneDrive] 위치]</td> 
   <td> <p>검색할 위치를 선택합니다.</p> 
    <ul> 
     <li> <p><b>[!UICONTROL My Drive]</b> </p> <p>모듈에서 드라이브 ID를 입력하도록 할지 여부를 선택합니다.</p> 
      <ul> 
       <li> <p><b>[!UICONTROL Yes]</b> </p> <p>가져올 파일이 포함된 드라이브의 ID를 입력합니다.</p> </li> 
       <li> <p><b>[!UICONTROL No]</b> </p> </li> 
      </ul> </li> 
     <li> <p><b>[!UICONTROL Site's Drive]</b> </p> <p>가져올 파일이 포함된 SharePoint 사이트를 선택합니다. 사용 가능한 사이트는 사이트 다음에 로그인한 사용자가 옵니다.</p> </li> 
     <li> <p><b>[!UICONTROL 그룹 드라이브]</b> </p> <p>가져올 파일이 드라이브에 포함된 그룹을 선택합니다.</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL 드라이브 ID]</td> 
   <td> <p>가져올 파일이 포함된 드라이브를 선택하거나 매핑합니다. [!UICONTROL Enable to Enter a Drive ID] 필드에서 [!UICONTROL No]를 선택한 경우에는 이 필드를 사용할 수 없습니다.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL File] / [!UICONTROL File ID] / [!UICONTROL File Path]</td> 
   <td> <p>[!UICONTROL 수동으로 입력]을 선택한 경우 가져올 파일의 파일 ID나 경로를 입력하거나 매핑합니다.</p> <p>목록에서 [!UICONTROL 선택]을 선택한 경우 가져올 파일을 선택합니다.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL 파일 다운로드]

이 작업 모듈은 지정된 파일을 다운로드합니다.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td> 
   <td>연결 방법에 대한 지침은 [!DNL OneDrive] 계정 대상 [!DNL Workfront Fusion]를 참조하십시오. <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">연결 만들기 [!DNL Adobe Workfront Fusion] - 기본 지침</a></td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Enter(파일 ID 및 파일 경로)]</td> 
   <td>파일을 파일 ID 또는 파일 경로로 식별할지 선택합니다.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">파일 ID / 파일 경로 입력</td> 
   <td> <p>파일 ID 또는 파일 경로를 입력할 방법을 선택합니다.</p> 
    <ul> 
     <li> <p><b>[!UICONTROL 수동으로 입력]</b> </p> <p>ID 또는 경로를 직접 입력하거나 이전 모듈에서 매핑하려면 이 옵션을 선택합니다.</p> </li> 
     <li> <p><b>[!UICONTROL 목록에서 선택]</b> </p> <p>사용 가능한 파일 또는 경로 목록에서 선택하려면 이 옵션을 선택합니다. </p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL [!DNL OneDrive] 위치]</td> 
   <td> <p>다운로드할 파일이 포함된 위치를 선택합니다.</p> 
    <ul> 
     <li> <p><b>[!UICONTROL My Drive]</b> </p> <p>모듈에서 드라이브 ID를 입력하도록 할지 여부를 선택합니다.</p> 
      <ul> 
       <li> <p><b>[!UICONTROL Yes]</b> </p> <p>다운로드할 파일이 포함된 드라이브의 ID를 입력합니다.</p> </li> 
       <li> <p><b>[!UICONTROL No]</b> </p> </li> 
      </ul> </li> 
     <li> <p><b>[!UICONTROL Site's Drive]</b> </p> <p>다운로드할 파일이 포함된 SharePoint 사이트를 선택합니다. 사용 가능한 사이트는 사이트 다음에 로그인한 사용자가 옵니다.</p> </li> 
     <li> <p><b>[!UICONTROL 그룹 드라이브]</b> </p> <p>다운로드할 파일이 드라이브에 포함된 그룹을 선택합니다.</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL 드라이브 ID]</td> 
   <td> <p>다운로드할 파일이 포함된 드라이브를 선택하거나 매핑합니다. [!UICONTROL Enable to Enter a Drive ID] 필드에서 [!UICONTROL No]를 선택한 경우에는 이 필드를 사용할 수 없습니다.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL File] / [!UICONTROL File ID] / [!UICONTROL File Path]</td>
   <td> <p>[!UICONTROL 수동으로 입력]을 선택한 경우 다운로드할 파일의 파일 ID나 경로를 입력하거나 매핑합니다.</p> <p>목록에서 [!UICONTROL 선택]을 선택한 경우 다운로드할 파일을 선택합니다.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL PDF으로 변환]</td> 
   <td> <p>파일을 PDF 파일로 변환하려면 이 옵션을 활성화합니다. 다음 파일 형식에서 변환할 수 있습니다.</p> 
    <table style="table-layout:auto"> 
     <col> 
     <col> 
     <col> 
     <tbody> 
      <tr> 
       <td> 
        <ul> 
         <li> <p> <p>CSV</p> </p> </li> 
         <li> <p> <p>문서</p> </p> </li> 
         <li> <p> <p>DOCX</p> </p> </li> 
         <li> <p> <p>ODP</p> </p> </li> 
         <li> <p> <p>ODS</p> </p> </li> 
         <li> <p> <p>ODT</p> </p> </li> 
        </ul> </td> 
       <td> 
        <ul> 
         <li> <p> <p>POT</p> </p> </li> 
         <li> <p> <p>POTM</p> </p> </li> 
         <li> <p> <p>포토x</p> </p> </li> 
         <li> <p> <p>PPS</p> </p> </li> 
         <li> <p> <p>PPSX</p> </p> </li> 
         <li> <p> <p>PPSXM</p> </p> </li> 
        </ul> </td> 
       <td> 
        <ul> 
         <li> <p>PPT</p> </li> 
         <li> <p>PPTM</p> </li> 
         <li> <p>PPTX</p> </li> 
         <li> <p>RTF</p> </li> 
         <li> <p>XLS</p> </li> 
         <li> <p>XLSX</p> </li> 
        </ul> </td> 
      </tr> 
     </tbody> 
    </table> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL 파일 업로드]

이 작업 모듈은 파일을 지정된 폴더에 업로드합니다.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td> 
   <td>연결 방법에 대한 지침은 [!DNL OneDrive] 계정 대상 [!DNL Workfront Fusion]를 참조하십시오. <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">연결 만들기 [!DNL Adobe Workfront Fusion] - 기본 지침</a></td> 
  </tr> 
  <tr> 
   <td role="rowheader">입력(폴더 위치 ID 및 경로)</td> 
   <td>대상 폴더를 ID별로 식별할지 또는 경로별로 식별할지를 선택합니다.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL [!DNL OneDrive] 위치]</td> 
   <td> <p>파일을 업로드할 위치를 선택합니다.</p> 
    <ul> 
     <li> <p><b>[!UICONTROL My Drive]</b> </p> <p>모듈에서 드라이브 ID를 입력하도록 할지 여부를 선택합니다.</p> 
      <ul> 
       <li> <p><b>[!UICONTROL Yes]</b> </p> <p>가져올 파일이 포함된 드라이브를 선택합니다.</p> </li> 
       <li> <p><b>[!UICONTROL No]</b> </p> </li> 
      </ul> </li> 
     <li> <p><b>[!UICONTROL Site's Drive]</b> </p> <p>을(를) 선택합니다 [!DNL SharePoint] 파일을 업로드할 폴더가 포함된 사이트입니다. 사용 가능한 사이트는 사이트 다음에 로그인한 사용자가 옵니다.</p> </li> 
     <li> <p><b>[!UICONTROL 그룹 드라이브]</b> </p> <p>파일을 업로드할 폴더가 포함된 그룹을 선택합니다.</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL 드라이브 ID]</td> 
   <td> <p>파일을 업로드할 폴더를 포함하는 드라이브를 선택합니다. [!UICONTROL Enable to Enter a Drive ID] 필드에서 [!UICONTROL No]를 선택한 경우에는 이 필드를 사용할 수 없습니다.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL 소스 파일]</td> 
   <td> <p>이전 모듈에서 소스 파일을 선택하거나 소스 파일의 이름과 데이터를 매핑합니다.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL 이름이 같은 파일이 있는 경우]</td> 
   <td>이름이 같은 파일이 이미 있는 경우 진행할 방법을 선택합니다.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Description]</td> 
   <td>업로드된 파일에 설명을 추가합니다.</td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL 폴더 만들기]

이 작업 모듈은 지정된 드라이브에 새 폴더를 만듭니다.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td> 
   <td>연결 방법에 대한 지침은 [!DNL OneDrive] 계정 대상 [!DNL Workfront Fusion]를 참조하십시오. <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">연결 만들기 [!DNL Adobe Workfront Fusion] - 기본 지침</a></td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL [!DNL OneDrive] 위치]</td> 
   <td> <p>폴더를 만들 위치를 선택합니다.</p> 
    <ul> 
     <li> <p><b>[!UICONTROL My Drive]</b> </p> <p>모듈에서 드라이브 ID를 입력하도록 할지 여부를 선택합니다.</p> 
      <ul> 
       <li> <p><b>[!UICONTROL Yes]</b> </p> <p>폴더를 만들 드라이브를 선택합니다.</p> </li> 
       <li> <p><b>[!UICONTROL No]</b> </p> </li> 
      </ul> </li> 
     <li> <p><b>[!UICONTROL Site's Drive]</b> </p> <p>을(를) 선택합니다 [!DNL SharePoint] 폴더를 만들 사이트입니다. 사용 가능한 사이트는 사이트 다음에 로그인한 사용자가 옵니다.</p> </li> 
     <li> <p><b>[!UICONTROL 그룹 드라이브]</b> </p> <p>폴더를 만들 드라이브를 소유하는 그룹을 선택합니다.</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL 드라이브 ID]</td> 
   <td> <p>폴더를 만들 드라이브를 선택합니다. [!UICONTROL Enable to Enter a Drive ID] 필드에서 [!UICONTROL No]를 선택한 경우에는 이 필드를 사용할 수 없습니다.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Folder]</td> 
   <td>새 폴더를 하위 폴더로 만들려면 해당 폴더를 의 하위 폴더로 이동합니다.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL 새 폴더 이름]</td> 
   <td> <p>새 폴더의 이름을 입력하거나 매핑합니다.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL 동일한 이름의 폴더가 있는 경우]</td> 
   <td>이름이 같은 파일이 이미 있는 경우 진행할 방법을 선택합니다.</td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL 공유 링크 가져오기]

이 작업 모듈은 지정된 파일에 대한 공유 링크를 반환합니다.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td> 
   <td>연결 방법에 대한 지침은 [!DNL OneDrive] 계정 대상 [!DNL Workfront Fusion]를 참조하십시오. <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">연결 만들기 [!DNL Adobe Workfront Fusion] - 기본 지침</a></td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Enter(파일 ID 및 파일 경로)]</td> 
   <td>파일을 파일 ID 또는 파일 경로로 식별할지 선택합니다.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL 파일 ID 입력] / [!UICONTROL 파일 경로]</td> 
   <td> <p>파일 ID 또는 파일 경로를 입력할 방법을 선택합니다.</p> 
    <ul> 
     <li> <p><b>[!UICONTROL 수동으로 입력]</b> </p> <p>ID 또는 경로를 직접 입력하거나 이전 모듈에서 매핑하려면 이 옵션을 선택합니다.</p> </li> 
     <li> <p><b>[!UICONTROL 목록에서 선택]</b> </p> <p>사용 가능한 파일 또는 경로 목록에서 선택하려면 이 옵션을 선택합니다. </p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL [!DNL OneDrive] 위치]</td> 
   <td> <p>공유 링크를 검색할 위치 선택:</p> 
    <ul> 
     <li> <p><b>[!UICONTROL My Drive]</b> </p> <p>모듈에서 드라이브 ID를 입력하도록 할지 여부를 선택합니다.</p> 
      <ul> 
       <li> <p><b>[!UICONTROL Yes]</b> </p> <p>공유 링크를 검색할 파일이 포함된 드라이브의 ID를 입력합니다.</p> </li> 
       <li> <p><b>[!UICONTROL No]</b> </p> </li> 
      </ul> </li> 
     <li> <p><b>[!UICONTROL Site's Drive]</b> </p> <p>공유 링크를 검색할 파일이 포함된 SharePoint 사이트를 선택합니다. 사용 가능한 사이트는 사이트 다음에 로그인한 사용자가 옵니다.</p> </li> 
     <li> <p><b>[!UICONTROL 그룹 드라이브]</b> </p> <p>공유 링크를 검색할 파일이 드라이브에 포함된 그룹을 선택합니다.</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL 드라이브 ID]</td> 
   <td> <p>공유 링크를 검색할 파일이 포함된 드라이브를 선택하거나 매핑합니다. [!UICONTROL Enable to Enter a Drive ID] 필드에서 [!UICONTROL No]를 선택한 경우에는 이 필드를 사용할 수 없습니다.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL File] / [!UICONTROL File ID] / [!UICONTROL File Path]</td> 
   <td> <p>[!UICONTROL 수동으로 입력]을 선택한 경우 공유 링크를 검색할 파일의 파일 ID나 경로를 입력하거나 매핑합니다.</p> <p>목록에서 [!UICONTROL Select]를 선택한 경우 공유 링크를 검색할 파일을 선택합니다.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL 권한 유형]</td> 
   <td> <p>링크를 가진 사람이 파일을 읽고 쓸 수 있도록 할지, 아니면 읽기 전용인지를 선택합니다.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL 범위]</td> 
   <td>링크를 가진 모든 사람이 파일을 사용할 수 있도록 할지, 링크를 가진 조직의 구성원만 파일을 사용할 수 있도록 할지를 선택합니다.</td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL 파일/폴더 이동]

이 작업 모듈은 파일이나 폴더를 새 폴더 위치로 이동합니다

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td> 
   <td>연결 방법에 대한 지침은 [!DNL OneDrive] 계정 대상 [!DNL Workfront Fusion]를 참조하십시오. <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">연결 만들기 [!DNL Adobe Workfront Fusion] - 기본 지침</a></td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Enter(파일 ID 및 파일 경로)]</td> 
   <td>파일을 파일 ID 또는 파일 경로로 식별할지 선택합니다.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL 파일 ID/파일 경로 입력]</td> 
   <td> <p>파일 ID 또는 파일 경로를 입력할 방법을 선택합니다.</p> 
    <ul> 
     <li> <p><b>[!UICONTROL 수동으로 입력]</b> </p> <p>ID 또는 경로를 직접 입력하거나 이전 모듈에서 매핑하려면 이 옵션을 선택합니다.</p> </li> 
     <li> <p><b>[!UICONTROL 목록에서 선택]</b> </p> <p>사용 가능한 파일 또는 경로 목록에서 선택하려면 이 옵션을 선택합니다. </p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL [!DNL OneDrive] 위치]</td> 
   <td> <p>이동할 파일 또는 폴더가 포함된 위치를 선택합니다.</p> 
    <ul> 
     <li> <p><b>[!UICONTROL My Drive]</b> </p> <p>모듈에서 드라이브 ID를 입력하도록 할지 여부를 선택합니다.</p> 
      <ul> 
       <li> <p><b>[!UICONTROL Yes]</b> </p> <p>이동할 파일 또는 폴더가 포함된 드라이브의 ID를 입력합니다.</p> </li> 
       <li> <p><b>[!UICONTROL No]</b> </p> </li> 
      </ul> </li> 
     <li> <p><b>[!UICONTROL Site's Drive]</b> </p> <p>을(를) 선택합니다 [!DNL SharePoint] 이동할 파일 또는 폴더가 포함된 사이트입니다. 사용 가능한 사이트는 사이트 다음에 로그인한 사용자가 옵니다.</p> </li> 
     <li> <p><b>[!UICONTROL 그룹 드라이브]</b> </p> <p>이동할 파일 또는 폴더가 포함된 그룹을 선택합니다.</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL 드라이브 ID]</td> 
   <td> <p>이동할 파일이나 폴더가 포함된 드라이브를 선택하거나 매핑합니다. [!UICONTROL Enable to Enter a Drive ID] 필드에서 [!UICONTROL No]를 선택한 경우에는 이 필드를 사용할 수 없습니다.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL File/Folder] 선택</td> 
   <td>파일을 이동할지 또는 폴더를 이동할지를 선택합니다.</td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p role="rowheader">[!UICONTROL File] / [!UICONTROL File ID] / [!UICONTROL File Path]</p> <p role="rowheader">[!UICONTROL Folder] / [!UICONTROL Folder ID] / [!UICONTROL Folder Path]</p> </td> 
   <td> <p>[!UICONTROL 수동으로 입력]을 선택한 경우 이동할 파일 또는 폴더의 ID나 경로를 입력하거나 매핑합니다.</p> <p>목록에서 [!UICONTROL Select]를 선택한 경우 이동할 파일 또는 폴더를 선택합니다.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL 새 폴더 위치 입력]</td> 
   <td> <p>파일이나 폴더를 이동할 위치를 입력할 방법을 선택합니다.</p> 
    <ul> 
     <li> <p><b>[!UICONTROL 수동으로 입력]</b> </p> <p>ID 또는 경로를 직접 입력하거나 이전 모듈에서 매핑하려면 이 옵션을 선택합니다.</p> </li> 
     <li> <p><b>[!UICONTROL 목록에서 선택]</b> </p> <p>사용 가능한 파일 또는 경로 목록에서 선택하려면 이 옵션을 선택합니다. </p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL [!DNL OneDrive] 위치]</td> 
   <td> <p>파일 또는 폴더를 이동할 위치를 선택합니다.</p> 
    <ul> 
     <li> <p><b>[!UICONTROL My Drive]</b> </p> <p>모듈에서 드라이브 ID를 입력하도록 할지 여부를 선택합니다.</p> 
      <ul> 
       <li> <p><b>[!UICONTROL Yes]</b> </p> <p>파일이나 폴더를 이동할 드라이브의 ID를 입력합니다.</p> </li> 
       <li> <p><b>[!UICONTROL No]</b> </p> </li> 
      </ul> </li> 
     <li> <p><b>[!UICONTROL Site's Drive]</b> </p> <p>을(를) 선택합니다 [!DNL SharePoint] 파일 또는 폴더를 이동할 사이트입니다. 사용 가능한 사이트는 사이트 다음에 로그인한 사용자가 옵니다.</p> </li> 
     <li> <p><b>[!UICONTROL 그룹 드라이브]</b> </p> <p>파일이나 폴더를 이동할 드라이브가 있는 그룹을 선택합니다.</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL 드라이브 ID]</td> 
   <td> <p>파일이나 폴더를 이동할 폴더가 포함된 드라이브를 선택하거나 매핑합니다. [!UICONTROL Enable to Enter a Drive ID] 필드에서 [!UICONTROL No]를 선택한 경우에는 이 필드를 사용할 수 없습니다.</p> <p>이 필드를 비워 두면 같은 내에서만 파일이나 폴더를 이동할 수 있습니다 [!DNL OneDrive].</p> <p>파일 및 폴더를 [!UICONTROL My Drive]에서 [!UICONTROL Site's Drive] 또는 [!UICONTROL Group's Drive]로 이동할 수 있습니다. </p> <p>파일을 [!UICONTROL 사이트의 드라이브]에서 같은 사이트의 동일한 드라이브로만 이동할 수 있습니다.</p> <p>[!UICONTROL 그룹의 드라이브]에서 같은 그룹의 같은 드라이브로만 파일을 이동할 수 있습니다.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Folder]</td> 
   <td>파일이나 폴더를 이동할 폴더를 입력하거나 매핑합니다.</td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL 파일 복사]

이 작업 모듈은 파일을 새 폴더 위치에 복사합니다

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td> 
   <td>연결 방법에 대한 지침은 [!DNL OneDrive] 계정 대상 [!DNL Workfront Fusion]를 참조하십시오. <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">연결 만들기 [!DNL Adobe Workfront Fusion] - 기본 지침</a></td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Enter(파일 ID 및 파일 경로)]</td> 
   <td>파일을 파일 ID 또는 파일 경로로 식별할지 선택합니다.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL 파일 ID 입력] / [!UICONTROL 파일 경로]</td> 
   <td> <p>파일 ID 또는 파일 경로를 입력할 방법을 선택합니다.</p> 
    <ul> 
     <li> <p><b>[!UICONTROL 수동으로 입력]</b> </p> <p>ID 또는 경로를 직접 입력하거나 이전 모듈에서 매핑하려면 이 옵션을 선택합니다.</p> </li> 
     <li> <p><b>[!UICONTROL 목록에서 선택]</b> </p> <p>사용 가능한 파일 또는 경로 목록에서 선택하려면 이 옵션을 선택합니다. </p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL [!DNL OneDrive] 위치]</td> 
   <td> <p>복사할 파일이 들어 있는 위치를 선택합니다.</p> 
    <ul> 
     <li> <p><b>[!UICONTROL My Drive]</b> </p> <p>모듈에서 드라이브 ID를 입력하도록 할지 여부를 선택합니다.</p> 
      <ul> 
       <li> <p><b>[!UICONTROL Yes]</b> </p> <p>복사할 파일 또는 폴더가 포함된 드라이브의 ID를 입력합니다.</p> </li> 
       <li> <p><b>[!UICONTROL No]</b> </p> </li> 
      </ul> </li> 
     <li> <p><b>[!UICONTROL Site's Drive]</b> </p> <p>이동할 파일이 포함된 SharePoint 사이트를 선택합니다. 사용 가능한 사이트는 사이트 다음에 로그인한 사용자가 옵니다.</p> </li> 
     <li> <p><b>[!UICONTROL 그룹 드라이브]</b> </p> <p>복사할 파일이 드라이브에 있는 그룹을 선택합니다.</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL 드라이브 ID]</td> 
   <td> <p>복사할 파일이 들어 있는 드라이브를 선택하거나 매핑합니다. [!UICONTROL Enable to Enter a Drive ID] 필드에서 [!UICONTROL No]를 선택한 경우에는 이 필드를 사용할 수 없습니다.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p role="rowheader">[!UICONTROL File] / [!UICONTROL File ID] / [!UICONTROL File Path]</p> </td> 
   <td> <p>[!UICONTROL 수동으로 입력]을 선택한 경우 복사할 파일의 ID나 경로를 입력하거나 매핑합니다.</p> <p>목록에서 [!UICONTROL Select]를 선택한 경우 복사할 파일을 선택합니다.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL 새 폴더 위치 입력]</td> 
   <td> <p>파일을 복사할 위치 또는 위치를 입력할 방법을 선택합니다.</p> 
    <ul> 
     <li> <p><b>[!UICONTROL 수동으로 입력]</b> </p> <p>ID 또는 경로를 직접 입력하거나 이전 모듈에서 매핑하려면 이 옵션을 선택합니다.</p> </li> 
     <li> <p><b>[!UICONTROL 목록에서 선택]</b> </p> <p>사용 가능한 폴더 목록에서 선택하려면 이 옵션을 선택합니다. </p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL 새 OneDrive 위치]</td> 
   <td> <p>필터를 복사할 위치를 선택합니다. 목록에서 새 폴더 위치를 선택하도록 선택한 경우 이 옵션을 사용할 수 있습니다.</p> 
    <ul> 
     <li> <p><b>[!UICONTROL My Drive]</b> </p> <p>모듈에서 드라이브 ID를 입력하도록 할지 여부를 선택합니다.</p> 
      <ul> 
       <li> <p><b>[!UICONTROL Yes]</b> </p> <p>파일을 복사할 드라이브의 ID를 입력합니다.</p> </li> 
       <li> <p><b>[!UICONTROL No]</b> </p> </li> 
      </ul> </li> 
     <li> <p><b>[!UICONTROL Site's Drive]</b> </p> <p>을(를) 선택합니다 [!DNL SharePoint] 파일을 복사할 사이트입니다. 사용 가능한 사이트는 사이트 다음에 로그인한 사용자가 옵니다.</p> </li> 
     <li> <p><b>[!UICONTROL 그룹 드라이브]</b> </p> <p>파일을 복사할 드라이브가 있는 그룹을 선택합니다.</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL 드라이브 ID]</td> 
   <td> <p>파일을 복사할 폴더가 포함된 드라이브를 선택하거나 매핑합니다. [!UICONTROL Enable to Enter a Drive ID] 필드에서 [!UICONTROL No]를 선택한 경우에는 이 필드를 사용할 수 없습니다.</p> <p>이 필드를 비워 두면 파일 또는 폴더는 동일한 [!UICONTROL OneDrive] 내에서만 복사할 수 있습니다.</p> <p>파일 및 폴더를 [!UICONTROL My Drive]에서 [!UICONTROL Site's Drive] 또는 [!UICONTROL Group's Drive]로 복사할 수 있습니다. </p> <p>[!UICONTROL Site's Drive]에서 파일을 동일한 사이트의 동일한 드라이브에만 복사할 수 있습니다.</p> <p>[!UICONTROL 그룹의 드라이브]에서 같은 그룹의 같은 드라이브에만 파일을 복사할 수 있습니다.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Folder]</td> 
   <td>복사 또는 폴더를 이동할 폴더를 입력하거나 매핑합니다.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL 복사된 새 파일 이름]</td> 
   <td> <p>파일의 새 복사본을 위한 이름을 입력하거나 매핑합니다. 원본 파일 이름을 변경하지 않으려면 이 필드를 비워 둘 수 있습니다.</p> <p>이름에는 파일 확장명이 포함되어야 합니다. 예:<code> file.txt</code></p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL 파일/폴더 삭제]

이 작업 모듈은 선택한 파일을 삭제합니다.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td> 
   <td>연결 방법에 대한 지침은 [!DNL OneDrive] 계정 대상 [!DNL Workfront Fusion]를 참조하십시오. <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">연결 만들기 [!DNL Adobe Workfront Fusion] - 기본 지침</a></td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Enter(파일/폴더 ID 및 경로)]</td> 
   <td>파일을 파일 ID 또는 파일 경로로 식별할지 선택합니다.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL 파일/폴더 ID 입력 /파일/폴더 경로 입력]</td> 
   <td> <p>파일 ID 또는 파일 경로를 입력할 방법을 선택합니다.</p> 
    <ul> 
     <li> <p><b>[!UICONTROL 수동으로 입력]</b> </p> <p>ID 또는 경로를 직접 입력하거나 이전 모듈에서 매핑하려면 이 옵션을 선택합니다.</p> </li> 
     <li> <p><b>[!UICONTROL 목록에서 선택]</b> </p> <p>사용 가능한 파일 또는 경로 목록에서 선택하려면 이 옵션을 선택합니다. </p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL [!DNL OneDrive] 위치]</td> 
   <td> <p>검색할 위치를 선택합니다.</p> 
    <ul> 
     <li> <p><b>[!UICONTROL My Drive]</b> </p> <p>모듈에서 드라이브 ID를 입력하도록 할지 여부를 선택합니다.</p> 
      <ul> 
       <li> <p><b>[!UICONTROL Yes]</b> </p> <p>삭제할 파일 또는 폴더가 포함된 드라이브의 ID를 입력합니다.</p> </li> 
       <li> <p><b>[!UICONTROL No]</b> </p> </li> 
      </ul> </li> 
     <li> <p><b>[!UICONTROL Site's Drive]</b> </p> <p>을(를) 선택합니다 [!DNL SharePoint] 삭제할 파일 또는 폴더가 포함된 사이트입니다. 사용 가능한 사이트는 사이트 다음에 로그인한 사용자가 옵니다.</p> </li> 
     <li> <p><b>[!UICONTROL 그룹 드라이브]</b> </p> <p>삭제할 파일 또는 폴더가 포함된 그룹을 선택합니다.</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL 드라이브 ID]</td> 
   <td> <p>삭제할 파일 또는 폴더가 포함된 드라이브를 선택하거나 매핑합니다. [!UICONTROL Enable to Enter a Drive ID] 필드에서 [!UICONTROL No]를 선택한 경우에는 이 필드를 사용할 수 없습니다.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL File/Folder] 선택</td> 
   <td>파일을 삭제할지 또는 폴더를 삭제할지 선택합니다.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL File] / [!UICONTROL File ID] / [!UICONTROL File Path]</td>
   <td> <p>[!UICONTROL 수동으로 입력]을 선택한 경우 삭제할 파일의 파일 ID나 경로를 입력하거나 매핑합니다.</p> <p>목록에서 [!UICONTROL Select]를 선택한 경우 삭제할 파일을 선택합니다.</p> </td> 
  </tr> 
 </tbody> 
</table>

### 기타

#### [!UICONTROL API 호출 만들기]

이 모듈은 사용자 지정 API 호출을 수행합니다.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td> 
   <td>연결 방법에 대한 지침은 [!DNL OneDrive] 계정 대상 [!DNL Workfront Fusion]를 참조하십시오. <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">연결 만들기 [!DNL Adobe Workfront Fusion] - 기본 지침</a></td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL URL]</td> 
   <td>상대 경로 입력 <code>https://graph.microsoft.com</code>. 예:<code> /v1.0/me/drive/root/children</code></td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL 메서드]</td> 
   td&gt; <p>API 호출을 구성하는 데 필요한 HTTP 요청 메서드를 선택합니다. 자세한 내용은 <a href="../../workfront-fusion/modules/http-request-methods.md" class="MCXref xref" data-mc-variable-override="">의 HTTP 요청 메서드 [!DNL Adobe Workfront Fusion]</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Headers]</td> 
   <td> <p>요청의 헤더를 표준 JSON 개체 형태로 추가합니다.</p> <p>For example, <code>{"Content-type":"application/json"}</code></p> <p>Workfront Fusion이 사용자를 위해 인증 헤더를 추가합니다.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL 쿼리 문자열]</td> 
   <td> <p>표준 JSON 개체 형태로 API 호출에 대한 쿼리를 추가합니다.</p> <p>For example: <code>{"name":"something-urgent"}</code></p> </td> 
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



## 파일을 업로드하거나 업데이트할 수 없는 경우

파일을 업로드하거나 업데이트하는 데 실패할 수 있는 몇 가지 문제가 있습니다.

* 업로드된 파일이 너무 커서 사용자의 최대 파일 크기 제한을 초과합니다. [!DNL OneDrive] 계획이나 사용자가 [!DNL OneDrive] 계정의 저장소 할당량입니다. 저장 공간을 더 확보하려면 기존 파일을 [!DNL OneDrive] 또는 업그레이드 [!DNL OneDrive] 계정이 필요합니다.
* OneDrive에서는 이름이 같은 두 파일을 하나의 폴더에 업로드할 수 없습니다. 대상 폴더에 업로드 중인 파일과 이름이 같은 파일이 포함되어 있으면 시나리오 실행이 오류 때문에 종료됩니다. 방법은 업로드되는 파일의 이름을 단순히 바꾸는 것입니다. 파일을 업데이트하는 것이 목표라면 [!UICONTROL 파일 업데이트] 작업.
* 파일을 업로드하고 있는 이전에 선택한 폴더가 더 이상 존재하지 않습니다. 시나리오가 중단되므로 대상 폴더를 다시 선택해야 합니다.
