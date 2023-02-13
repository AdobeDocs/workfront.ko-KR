---
content-type: reference
product-previous: workfront-fusion
product-area: workfront-integrations;documents
keywords: 커넥터
navigation-topic: apps-and-their-modules
title: 비즈니스 모듈용 Microsoft OneDrive
description: 에서 [!DNL Adobe Workfront Fusion] 시나리오, [!DNL Microsoft OneDrive for Business]여러 타사 애플리케이션 및 서비스에 연결할 수 있습니다.
author: Becky
feature: Workfront Fusion
exl-id: b7175cb9-aade-49b7-a28b-25fc9805a078
source-git-commit: 885d93dd4383945538e977fd3edbfd55bda88b70
workflow-type: tm+mt
source-wordcount: '1039'
ht-degree: 0%

---

# [!DNL Microsoft OneDrive for Business] 모듈

에서 [!DNL Adobe Workfront Fusion] 시나리오, [!DNL Microsoft OneDrive for Business]여러 타사 애플리케이션 및 서비스에 연결할 수 있습니다.

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

를 사용하려면 [!DNL Microsoft OneDrive for Business] with [!DNL Adobe Workfront Fusion], 필요한 경우 [!DNL Microsoft] 계정이 필요합니다.

연결 방법에 대한 지침은 [!DNL OneDrive for Business] 계정 대상 [!DNL Workfront Fusion]를 참조하십시오. [Adobe 연결 만들기 [!DNL Workfront Fusion] - 기본 지침](../../workfront-fusion/connections/connect-to-fusion-general.md)

## [!DNL Microsoft OneDrive for Business] 모듈 및 해당 필드

구성 시 [!DNL Microsoft OneDrive for Business] 모듈, [!DNL Workfront Fusion] 아래 나열된 필드를 표시합니다. 이와 함께 추가 [!DNL Microsoft OneDrive for Business] 앱이나 서비스에서 액세스 수준과 같은 요소에 따라 필드가 표시될 수 있습니다. 모듈에서 굵게 표시된 제목은 필수 필드를 나타냅니다.

필드 또는 함수 위에 맵 단추가 표시되면 이 단추를 사용하여 해당 필드에 대한 변수와 함수를 설정할 수 있습니다. 자세한 내용은 [의 한 모듈에서 다른 모듈로 정보 매핑 [!DNL Adobe Workfront Fusion]](../../workfront-fusion/mapping/map-information-between-modules.md).

![](assets/map-toggle-350x74.png)

* [Triggers](#triggers)
* [액션](#actions)

### Triggers

* [[!UICONTROL 감시 파일]](#watch-files)
* [[!UICONTROL 폴더 감시]](#watch-folders)

#### [!UICONTROL 감시 파일]

이 트리거 모듈은 감시 중인 폴더에 새 파일을 추가하거나 업데이트하면 활성화됩니다.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Connection]</p> </td> 
   <td> <p>연결 방법에 대한 지침은 [!DNL Office 365] 계정 대상 [!DNL Workfront Fusion]를 참조하십시오. <a href="../../workfront-fusion/scenarios/create-a-scenario.md#connect" class="MCXref xref">모듈의 앱 또는 웹 서비스를 [!DNL Workfront Fusion]</a> 기사 <a href="../../workfront-fusion/scenarios/create-a-scenario.md" class="MCXref xref">에서 시나리오 만들기 [!DNL Adobe Workfront Fusion]</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL 드라이브 ID]</p> </td> 
   <td> <p>보려는 드라이브를 선택합니다.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Folder]</td> 
   <td> <p> 보려는 폴더를 선택합니다. 시나리오 내에서는 하나의 폴더만 모니터링할 수 있습니다.</p> <p>팁: 여러 폴더를 추적하려면 각 폴더에 대해 독립적인 시나리오를 만드십시오.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL 보고 싶습니다]</p> </td> 
   <td> <p>새 파일 및 모든 변경 내용을 표시할지 아니면 새 파일만 보할지를 선택합니다.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL 반환된 최대 행 수]</td> 
   <td> <p> 최대 결과 수 설정 [!DNL Workfront Fusion] 은 한 번의 사이클로 작동합니다.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL 폴더 감시]

이 트리거 모듈은 감시 중인 폴더에 새 폴더가 추가되면 활성화됩니다.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Connection]</p> </td> 
   <td> <p>연결 방법에 대한 지침은 [!DNL Office 365] 계정 대상 [!DNL Workfront Fusion]를 참조하십시오. <a href="../../workfront-fusion/scenarios/create-a-scenario.md#connect" class="MCXref xref">모듈의 앱 또는 웹 서비스를 [!DNL Workfront Fusion]</a> 기사 <a href="../../workfront-fusion/scenarios/create-a-scenario.md" class="MCXref xref">에서 시나리오 만들기 [!DNL Adobe Workfront Fusion]</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL 드라이브 ID]</p> </td> 
   <td> <p>보려는 드라이브를 선택합니다.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Folder]</td> 
   <td> <p> 보려는 폴더를 선택합니다. 시나리오 내에서는 하나의 폴더만 모니터링할 수 있습니다.</p> <p>팁: 여러 폴더를 추적하려면 각 폴더에 대해 독립적인 시나리오를 만드십시오.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL 보고 싶습니다]</p> </td> 
   <td> <p>새 폴더 및 모든 변경 내용을 표시할지 아니면 새 폴더만 표시할지 여부를 선택합니다.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL 반환된 최대 행 수]</td> 
   <td> <p> 최대 결과 수 설정 [!DNL Workfront Fusion] 은 한 번의 사이클로 작동합니다.</p> </td> 
  </tr> 
 </tbody> 
</table>

### 액션

* [[!UICONTROL 파일 업로드]](#upload-a-file)
* [[!UICONTROL 파일 삭제]](#delete-a-file)
* [[!UICONTROL 파일 가져오기]](#get-a-file)
* [[!UICONTROL 폴더 만들기]](#create-a-folder)
* [[!UICONTROL 폴더 삭제]](#delete-a-folder)
* [[!UICONTROL 공유 링크 가져오기]](#get-a-sharing-link)

#### [!UICONTROL 파일 업로드]

이 작업 모듈은 이진 또는 텍스트 파일을 지정된 폴더에 업로드합니다

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL Connection] </td> 
   <td> <p>연결 방법에 대한 지침은 [!DNL Office 365] 계정 대상 [!DNL Workfront Fusion]를 참조하십시오. <a href="../../workfront-fusion/scenarios/create-a-scenario.md#connect" class="MCXref xref">모듈의 앱 또는 웹 서비스를 [!DNL Workfront Fusion]</a> 기사 <a href="../../workfront-fusion/scenarios/create-a-scenario.md" class="MCXref xref">에서 시나리오 만들기 [!DNL Adobe Workfront Fusion]</a>.</p> </td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL 드라이브 ID]</td> 
   <td> <p>파일을 업로드할 드라이브를 선택합니다.</p> </td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Folder] </td> 
   <td> <p>드라이브 내의 폴더를 선택합니다.</p> </td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td> <p>[!UICONTROL 소스 파일]</p> </td> 
   <td> <p>이전 모듈에서 소스 파일을 선택하거나 소스 파일의 이름과 데이터를 매핑합니다.</p> </td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL 이름이 같은 파일이 있는 경우]</td> 
   <td> <p> 업로드하려는 파일과 이름이 같은 파일이 이미 있는 경우 수행할 작업을 선택합니다.</p> 
    <ul> 
     <li>[!UICONTROL 기존 파일 바꾸기]</li> 
     <li>[!UICONTROL 새 파일 이름 바꾸기]</li> 
     <li>[!UICONTROL 오류가 발생하여 끝남]</li> 
    </ul> </td> 
   <td> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL 파일 삭제]

이 작업 모듈은 지정된 파일을 휴지통으로 이동합니다.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL Connection] </td> 
   <td> <p>연결 방법에 대한 지침은 [!DNL Office 365] 계정 대상 [!DNL Workfront Fusion]를 참조하십시오. <a href="../../workfront-fusion/scenarios/create-a-scenario.md#connect" class="MCXref xref">모듈의 앱 또는 웹 서비스를 [!DNL Workfront Fusion]</a> 기사 <a href="../../workfront-fusion/scenarios/create-a-scenario.md" class="MCXref xref">에서 시나리오 만들기 [!DNL Adobe Workfront Fusion]</a>.</p> </td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL 드라이브 ID]</td> 
   <td> <p>파일을 삭제할 드라이브를 선택합니다.</p> </td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL 파일 ID]</td> 
   <td> <p>삭제할 파일의 ID를 입력합니다. </p> </td> 
   <td> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL 파일 가져오기]

이 작업 모듈은 주어진 ID를 가진 파일을 검색합니다.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL Connection] </td> 
   <td> <p>연결 방법에 대한 지침은 [!DNL Office 365] 계정 대상 [!DNL Workfront Fusion]를 참조하십시오. <a href="../../workfront-fusion/scenarios/create-a-scenario.md#connect" class="MCXref xref">모듈의 앱 또는 웹 서비스를 [!DNL Workfront Fusion]</a> 기사 <a href="../../workfront-fusion/scenarios/create-a-scenario.md" class="MCXref xref">에서 시나리오 만들기 [!DNL Adobe Workfront Fusion]</a>.</p> </td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL 드라이브 ID]</td> 
   <td> <p>파일을 검색할 드라이브를 선택합니다.</p> </td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL 파일 ID]</td> 
   <td> <p>검색할 파일의 ID를 입력합니다. </p> </td> 
   <td> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL 폴더 만들기]

지정된 상위 폴더 내에 폴더를 만듭니다.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td><strong>[!UICONTROL Connection]</strong> </td> 
   <td> <p>연결 방법에 대한 지침은 [!DNL Office 365] 계정 대상 [!DNL Workfront Fusion]를 참조하십시오. <a href="../../workfront-fusion/scenarios/create-a-scenario.md#connect" class="MCXref xref">모듈의 앱 또는 웹 서비스를 [!DNL Workfront Fusion]</a> 기사 <a href="../../workfront-fusion/scenarios/create-a-scenario.md" class="MCXref xref">에서 시나리오 만들기 [!DNL Adobe Workfront Fusion]</a>.</p> </td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td><strong>[!UICONTROL 드라이브 ID]</strong> </td> 
   <td> <p>새 폴더를 만들 드라이브를 선택합니다.</p> </td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td><strong>[!UICONTROL Folder]</strong> </td> 
   <td> <p>에서 새 폴더를 만들 폴더를 선택합니다.</p> </td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td><strong>[!UICONTROL 폴더 이름]</strong> </td> 
   <td>새 폴더의 이름을 입력하거나 매핑합니다.</td> 
   <td> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL 폴더 삭제]

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL Connection] </td> 
   <td> <p>연결 방법에 대한 지침은 [!DNL Office 365] 계정 대상 [!DNL Workfront Fusion]를 참조하십시오. <a href="../../workfront-fusion/scenarios/create-a-scenario.md#connect" class="MCXref xref">모듈의 앱 또는 웹 서비스를 [!DNL Workfront Fusion]</a> 기사 <a href="../../workfront-fusion/scenarios/create-a-scenario.md" class="MCXref xref">에서 시나리오 만들기 [!DNL Adobe Workfront Fusion]</a>.</p> </td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL 드라이브 ID]</td> 
   <td> <p>파일을 삭제할 드라이브를 선택합니다.</p> </td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL 폴더 ID]</td> 
   <td> <p>삭제할 폴더의 ID를 입력하거나 매핑합니다. </p> </td> 
   <td> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL 공유 링크 가져오기]

이 모듈은 공유할 수 있는 링크를 검색하여 지정한 파일에 액세스할 수 있습니다.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL Connection] </td> 
   <td> <p>연결 방법에 대한 지침은 [!DNL Office 365] 계정 대상 [!DNL Workfront Fusion]를 참조하십시오. <a href="../../workfront-fusion/scenarios/create-a-scenario.md#connect" class="MCXref xref">모듈의 앱 또는 웹 서비스를 [!DNL Workfront Fusion]</a> 기사 <a href="../../workfront-fusion/scenarios/create-a-scenario.md" class="MCXref xref">에서 시나리오 만들기 [!DNL Adobe Workfront Fusion]</a>.</p> </td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL 드라이브 ID]</td> 
   <td> <p>파일을 업로드할 드라이브를 선택합니다.</p> </td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Enter]</td> 
   <td> <p>파일 ID 또는 파일 경로를 사용하여 파일을 선택할지 선택합니다. 표시되는 필드에 파일 ID 또는 경로를 입력합니다.</p> </td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td> <p>[!UICONTROL 권한 유형]</p> </td> 
   <td> <p>링크를 받는 사람에게 읽기/쓰기 권한이 있는지 아니면 읽기 전용 권한이 있는지 여부를 선택합니다.</p> </td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL 범위]</td> 
   <td> <p> 링크를 가진 모든 사람이 파일에 액세스할 수 있도록 할지 또는 조직 구성원만 액세스할 수 있도록 할지 여부를 선택합니다.</p> </td> 
   <td> </td> 
  </tr> 
 </tbody> 
</table>
