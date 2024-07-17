---
content-type: reference
product-previous: workfront-fusion
product-area: workfront-integrations
keywords: 커넥터
navigation-topic: apps-and-their-modules
title: SharePoint 모듈
description: ' [!DNL Adobe Workfront Fusion] 시나리오에서는 SharePoint을 사용하는 워크플로를 자동화할 수 있을 뿐만 아니라 여러 타사 응용 프로그램 및 서비스에 연결할 수도 있습니다.'
author: Becky
feature: Workfront Fusion
exl-id: 16d49031-06d2-4c86-bac4-f58cd9b2f1f5
source-git-commit: 8b4182ae2b32488a02cacc16fcb6a246fcb571fd
workflow-type: tm+mt
source-wordcount: '2850'
ht-degree: 0%

---

# [!DNL SharePoint]개 모듈

[!DNL Adobe Workfront Fusion] 시나리오에서는 [!DNL SharePoint]을(를) 사용하는 워크플로를 자동화하고 여러 타사 응용 프로그램 및 서비스에 연결할 수 있습니다.

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

[!DNL SharePoint] 모듈을 사용하려면 [!DNL SharePoint] 계정이 있어야 합니다.

## [!DNL SharePoint]을(를) [!DNL Workfront Fusion]에 연결 {#connect-sharepoint-to-workfront-fusion}

* [ [!DNL Microsoft] 계정을 사용하여  [!DNL SharePoint] to [!DNL Workfront Fusion] 연결](#connect-sharepoint-to-workfront-fusion-using-a-microsoft-account)
* [고급 설정을 사용하여  [!DNL SharePoint] to [!DNL Workfront Fusion] 연결](#connect-sharepoint-to-workfront-fusion-using-advanced-settings)

### [!DNL Microsoft] 계정을 사용하여 [!DNL SharePoint]을(를) [!DNL Workfront Fusion]에 연결

[!DNL Microsoft] 계정을 사용하여 [!DNL SharePoint]에 연결할 수 있습니다. [!DNL Sharepoint] 계정을 [!DNL Workfront Fusion]에 연결하는 방법에 대한 지침은 [연결 만들기 [!DNL Adobe Workfront Fusion] - 기본 지침](../../workfront-fusion/connections/connect-to-fusion-general.md)을 참조하세요.

### 고급 설정을 사용하여 [!DNL SharePoint]을(를) [!DNL Workfront Fusion]에 연결

[!DNL Microsoft] 계정 없이 [!DNL SharePoint]을(를) [!DNL Workfront Fusion]에 연결하려면 클라이언트 ID, 클라이언트 암호 및 테넌트 ID가 필요합니다.

1. **[!DNL SharePoint]** 상자 위쪽에 있는 **[!UICONTROL 추가]**&#x200B;를 클릭하여 **[!UICONTROL 연결 만들기]** 상자를 엽니다.

1. (선택 사항) 기본 **[!UICONTROL 연결 이름]**&#x200B;을 변경합니다.
1. **[!UICONTROL 고급 설정 표시]**&#x200B;를 클릭합니다.
1. [!DNL SharePoint] **[!UICONTROL 클라이언트 ID]** 및 **[!UICONTROL 클라이언트 암호]**&#x200B;를 입력하십시오.

1. **[!UICONTROL 계속]**&#x200B;을 클릭합니다.
1. 아직 로그인하지 않은 경우 표시되는 로그인 창에서 자격 증명을 입력하여 앱에 로그인합니다.
1. (조건부) **[!UICONTROL 허용]** 단추가 표시되면 단추를 클릭하여 앱을 [!DNL Workfront Fusion]에 연결합니다.

## [!DNL SharePoint]개 모듈 및 해당 필드

[!DNL SharePoint] 모듈을 구성할 때 [!DNL Workfront Fusion]에 아래 나열된 필드가 표시됩니다. 앱 또는 서비스의 액세스 수준과 같은 요소에 따라 이러한 필드와 함께 [!DNL SharePoint] 필드가 추가로 표시될 수 있습니다. 모듈의 굵은 제목은 필수 필드를 나타냅니다.

필드나 함수 위에 맵 단추가 표시되면 이 단추를 사용하여 해당 필드에 대한 변수와 함수를 설정할 수 있습니다. 자세한 내용은 [한 모듈에서 다른 모듈로 정보를 매핑 [!DNL Adobe Workfront Fusion]](../../workfront-fusion/mapping/map-information-between-modules.md)을 참조하십시오.

![](assets/map-toggle-350x74.png)

* [드라이브 항목](#drive-item)
* [항목](#item)
* [목록](#list)
* [페이지(Beta)](#page-beta)
* [Site](#site)
* [기타](#other)

### 드라이브 항목

* [파일 만들기](#create-a-file)
* [폴더 만들기](#create-a-folder)
* [파일 가져오기](#get-a-file)
* [감시 폴더 항목](#watch-folder-items)

#### 변경 사항 가져오기

이 모듈은 SharePoint에서 수행한 변경 사항을 반환합니다.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td> 
   <td> <p>[!DNL SharePoint] 계정을 [!DNL Workfront Fusion]에 연결하는 방법에 대한 지침은 이 문서에서 <a href="#connect-sharepoint-to-workfront-fusion" class="MCXref xref" data-mc-variable-override="">[!DNL SharePoint]을(를) [!DNL Workfront Fusion]</a>에 연결 을 참조하십시오.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL 사이트, 드라이브 및 폴더 ID 입력]</td> 
   <td> <p>변경 사항을 검색할 폴더의 위치를 식별하는 방법을 선택합니다.</p> 
    <ul> 
     <li> <p><strong>[!UICONTROL Enter manually]</strong> </p> <p>표시되는 필드에 <strong>[!UICONTROL 사이트 ID]</strong>, <strong>[!UICONTROL 목록 ID]</strong> 및 <strong>[!UICONTROL 폴더 ID]</strong>을(를) 입력하거나 매핑합니다.</p> </li> 
     <li> <p><strong>[!UICONTROL 팔로우하는 목록에서 선택]</strong> </p> <p>변경 사항을 검색할 위치를 선택합니다. </p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Token]</td> 
   <td> </td> 
  </tr>  </tbody> 
</table>

#### 폴더 만들기

이 작업 모듈은 SharePoint에 새 폴더를 만듭니다.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td> 
   <td> <p>[!DNL SharePoint] 계정을 [!DNL Workfront Fusion]에 연결하는 방법에 대한 지침은 이 문서에서 <a href="#connect-sharepoint-to-workfront-fusion" class="MCXref xref" data-mc-variable-override="">[!DNL SharePoint]을(를) [!DNL Workfront Fusion]</a>에 연결 을 참조하십시오.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL 사이트, 드라이브 및 폴더 ID 입력]</td> 
   <td> <p>만들려는 폴더의 위치를 식별하는 방법을 선택합니다.</p> 
    <ul> 
     <li> <p><strong>[!UICONTROL Enter manually]</strong> </p> <p>표시되는 필드에 <strong>[!UICONTROL 사이트 ID]</strong>, <strong>[!UICONTROL 목록 ID]</strong> 및 <strong>[!UICONTROL 폴더 ID]</strong>을(를) 입력하거나 매핑합니다.</p> </li> 
     <li> <p><strong>[!UICONTROL 팔로우하는 목록에서 선택]</strong> </p> <p>폴더를 만들 위치를 선택합니다. </p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL 폴더 이름]</td> 
   <td>새 폴더의 이름을 입력하거나 매핑합니다.</td> 
  </tr>
  </tbody> 
</table>

#### 파일 가져오기

이 작업 모듈은 지정된 SharePoint 파일을 검색합니다.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td> 
   <td> <p>[!DNL SharePoint] 계정을 [!DNL Workfront Fusion]에 연결하는 방법에 대한 지침은 이 문서에서 <a href="#connect-sharepoint-to-workfront-fusion" class="MCXref xref" data-mc-variable-override="">[!DNL SharePoint]을(를) [!DNL Workfront Fusion]</a>에 연결 을 참조하십시오.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL 사이트, 드라이브 및 폴더 ID 입력]</td> 
   <td> <p>가져올 파일의 위치를 식별하는 방법을 선택하십시오.</p> 
    <ul> 
     <li> <p><strong>[!UICONTROL Enter manually]</strong> </p> <p>표시되는 필드에 <strong>[!UICONTROL 사이트 ID]</strong>, <strong>[!UICONTROL 목록 ID]</strong> 및 <strong>[!UICONTROL 파일 ID]</strong>을(를) 입력하거나 매핑합니다.</p> </li> 
     <li> <p><strong>[!UICONTROL 팔로우하는 목록에서 선택]</strong> </p> <p>파일 위치를 선택합니다. </p> </li> 
    </ul> </td> 
  </tr> 
</tbody> 
</table>

#### 감시 폴더 항목

이 트리거 모듈은 선택한 폴더에서 항목이 업데이트될 때 시나리오를 시작합니다.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td> 
   <td> <p>[!DNL SharePoint] 계정을 [!DNL Workfront Fusion]에 연결하는 방법에 대한 지침은 이 문서에서 <a href="#connect-sharepoint-to-workfront-fusion" class="MCXref xref" data-mc-variable-override="">[!DNL SharePoint]을(를) [!DNL Workfront Fusion]</a>에 연결 을 참조하십시오.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL 사이트, 드라이브 및 폴더 ID 입력]</td> 
   <td> <p>가져올 파일의 위치를 식별하는 방법을 선택하십시오.</p> 
    <ul> 
     <li> <p><strong>[!UICONTROL Enter manually]</strong> </p> <p>표시되는 필드에 <strong>[!UICONTROL 사이트 ID]</strong>, <strong>[!UICONTROL 목록 ID]</strong> 및 <strong>[!UICONTROL 폴더 ID]</strong>을(를) 입력하거나 매핑합니다.</p> </li> 
     <li> <p><strong>[!UICONTROL 팔로우하는 목록에서 선택]</strong> </p> <p>감시할 폴더의 위치를 선택합니다. </p> </li> 
    </ul> </td> 
  </tr> 
   <td role="rowheader">[!UICONTROL 제한]</td> 
   <td>시나리오 실행 주기 동안 [!DNL Workfront Fusion]이(가) 반환해야 하는 최대 항목 수를 입력하십시오.</td> 
  <tr>
  </tr>
</tbody> 
</table>

### 항목

* [[!UICONTROL 항목 복사]](#copy-an-item)
* [[!UICONTROL 항목 만들기]](#create-an-item)
* [[!UICONTROL 항목 삭제]](#delete-an-item)
* [[!UICONTROL 항목 가져오기]](#get-an-item)
* [[!UICONTROL 목록 항목]](#list-items)
* [[!UICONTROL 항목 이동]](#move-an-item)
* [[!UICONTROL 항목 업데이트]](#update-an-item)
* [[!UICONTROL 항목 보기](예약됨)](#watch-items-scheduled)


#### [!UICONTROL 항목 복사]

이 작업 모듈은 SharePoint 목록의 기존 항목을 복사합니다.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td> 
   <td> <p>[!DNL SharePoint] 계정을 [!DNL Workfront Fusion]에 연결하는 방법에 대한 지침은 이 문서에서 <a href="#connect-sharepoint-to-workfront-fusion" class="MCXref xref" data-mc-variable-override="">[!DNL SharePoint]을(를) [!DNL Workfront Fusion]</a>에 연결 을 참조하십시오.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">사이트, 드라이브 및 폴더 ID 입력</td> 
   <td> <p>복사할 항목이 들어 있는 사이트 및 목록을 식별하는 방법을 선택합니다.</p> 
    <ul> 
     <li> <p><strong>[!UICONTROL Enter manually]</strong> </p> <p>표시되는 필드에 <strong>[!UICONTROL 사이트 ID]</strong>, <strong>[!UICONTROL 목록 ID]</strong> 및 <strong>[!UICONTROL 항목 ID]</strong>을(를) 입력하거나 매핑합니다.</p> </li> 
     <li> <p><strong>[!UICONTROL 팔로우하는 목록에서 선택]</strong> </p> <p>항목 유형 필드에서 필드를 이동할 것인지 폴더를 이동할 것인지 선택합니다.  복사할 항목이 들어 있는 사이트를 선택한 다음 목록을 선택하고 항목을 선택합니다. </p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL 대상 ID]</td> 
   <td> 항목을 복사할 폴더의 ID를 입력하거나 매핑합니다. </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL 새 이름]</td> 
   <td>항목의 새 복사본에 대한 이름을 입력하거나 매핑합니다. </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL 항목 만들기]

이 작업 모듈은 SharePoint 목록에 새 항목을 만듭니다.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td> 
   <td> <p>[!DNL SharePoint] 계정을 [!DNL Workfront Fusion]에 연결하는 방법에 대한 지침은 이 문서에서 <a href="#connect-sharepoint-to-workfront-fusion" class="MCXref xref" data-mc-variable-override="">[!DNL SharePoint]을(를) [!DNL Workfront Fusion]</a>에 연결 을 참조하십시오.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL 항목 만들기]</td> 
   <td> <p>항목을 만들 사이트 및 목록을 식별하는 방법을 선택합니다.</p> 
    <ul> 
     <li> <p><strong>[!UICONTROL Enter manually]</strong> </p> <p>표시되는 필드에 <strong>[!UICONTROL 사이트 ID]</strong> 및 <strong>[!UICONTROL 목록 ID]</strong>을(를) 입력하거나 매핑합니다.</p> </li> 
     <li> <p><strong>[!UICONTROL 목록에서 선택]</strong> </p> <p>항목을 만들 목록이 포함된 사이트를 선택한 다음 목록을 선택합니다. </p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL 필드]</td> 
   <td>새 항목에 대해 설정하려는 각 필드에 필드의 키(필드 식별)와 해당 필드에 대해 새 항목에 사용할 값을 입력합니다.</td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL 항목 삭제]

이 작업 모듈은 SharePoint 목록의 기존 항목을 삭제합니다.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td> 
   <td> <p>[!DNL SharePoint] 계정을 [!DNL Workfront Fusion]에 연결하는 방법에 대한 지침은 이 문서에서 <a href="#connect-sharepoint-to-workfront-fusion" class="MCXref xref" data-mc-variable-override="">[!DNL SharePoint]을(를) [!DNL Workfront Fusion]</a>에 연결 을 참조하십시오.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL 항목 업데이트]</td> 
   <td> <p>삭제하려는 항목이 포함된 사이트 및 목록을 식별하는 방법을 선택합니다.</p> 
    <ul> 
     <li> <p><strong>[!UICONTROL Enter manually]</strong> </p> <p>표시되는 필드에 <strong>[!UICONTROL 사이트 ID]</strong>, <strong>[!UICONTROL 목록 ID]</strong> 및 <strong>[!UICONTROL 항목 ID]</strong>을(를) 입력하거나 매핑합니다.</p> </li> 
     <li> <p><strong>[!UICONTROL 목록에서 선택]</strong> </p> <p>삭제할 항목이 포함된 사이트를 선택한 다음 목록을 선택하고 항목을 선택합니다. </p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL 항목 가져오기]

이 작업 모듈은 지정된 항목의 데이터를 반환합니다.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td> 
   <td> <p>[!DNL SharePoint] 계정을 [!DNL Workfront Fusion]에 연결하는 방법에 대한 지침은 이 문서에서 <a href="#connect-sharepoint-to-workfront-fusion" class="MCXref xref" data-mc-variable-override="">[!DNL SharePoint]을(를) [!DNL Workfront Fusion]</a>에 연결 을 참조하십시오.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL 항목 가져오기]</td> 
   <td> <p>가져오려는 항목이 포함된 사이트 및 목록을 식별하는 방법을 선택합니다.</p> 
    <ul> 
     <li> <p><strong>[!UICONTROL Enter manually]</strong> </p> <p>표시되는 필드에 <strong>[!UICONTROL 사이트 ID]</strong>, <strong>[!UICONTROL 목록 ID]</strong> 및 <strong>[!UICONTROL 항목 ID]</strong>을(를) 입력하거나 매핑합니다.</p> </li> 
     <li> <p><strong>[!UICONTROL 목록에서 선택]</strong> </p> <p>항목을 검색할 목록이 포함된 사이트를 선택한 다음 목록을 선택하고 항목을 선택합니다. </p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL 목록 항목]

이 작업 모듈은 지정된 목록의 모든 항목 목록을 검색합니다.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td> 
   <td> <p>[!DNL SharePoint] 계정을 [!DNL Workfront Fusion]에 연결하는 방법에 대한 지침은 이 문서에서 <a href="#connect-sharepoint-to-workfront-fusion" class="MCXref xref" data-mc-variable-override="">[!DNL SharePoint]을(를) [!DNL Workfront Fusion]</a>에 연결 을 참조하십시오.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL 목록 항목]</td> 
   <td> <p>항목을 검색할 목록을 식별하는 방법을 선택합니다.</p> 
    <ul> 
     <li> <p><strong>[!UICONTROL Enter manually]</strong> </p> <p>표시되는 필드에 <strong>[!UICONTROL 사이트 ID]</strong> 및 <strong>[!UICONTROL 목록 ID]</strong>을(를) 입력하거나 매핑합니다.</p> </li> 
     <li> <p><strong>[!UICONTROL 목록에서 선택]</strong> </p> <p>항목을 검색할 목록이 포함된 사이트를 선택한 다음 목록을 선택합니다. </p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL 제한]</td> 
   <td> <p>각 시나리오 실행 주기 동안 모듈이 반환할 최대 항목 수를 입력하거나 매핑합니다.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL 항목 이동]

이 작업 모듈은 SharePoint 목록의 기존 항목을 복사합니다.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td> 
   <td> <p>[!DNL SharePoint] 계정을 [!DNL Workfront Fusion]에 연결하는 방법에 대한 지침은 이 문서에서 <a href="#connect-sharepoint-to-workfront-fusion" class="MCXref xref" data-mc-variable-override="">[!DNL SharePoint]을(를) [!DNL Workfront Fusion]</a>에 연결 을 참조하십시오.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">사이트, 드라이브 및 폴더 ID 입력</td> 
   <td> <p>이동할 항목이 포함된 사이트 및 목록을 식별하는 방법을 선택합니다.</p> 
    <ul> 
     <li> <p><strong>[!UICONTROL Enter manually]</strong> </p> <p>표시되는 필드에 <strong>[!UICONTROL 사이트 ID]</strong>, <strong>[!UICONTROL 목록 ID]</strong> 및 <strong>[!UICONTROL 항목 ID]</strong>을(를) 입력하거나 매핑합니다.</p> </li> 
     <li> <p><strong>[!UICONTROL 팔로우하는 목록에서 선택]</strong> </p> <p>항목 유형 필드에서 필드를 이동할 것인지 폴더를 이동할 것인지 선택합니다. 복사할 항목이 들어 있는 사이트를 선택한 다음 목록을 선택하고 항목을 선택합니다. </p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL 대상 ID]</td> 
   <td> 항목을 이동할 폴더의 ID를 입력하거나 매핑합니다. </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL 새 이름]</td> 
   <td>이동된 항목의 이름을 입력하거나 매핑합니다. </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL 항목 업데이트]

이 작업 모듈은 SharePoint 목록의 기존 항목을 업데이트합니다.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td> 
   <td> <p>[!DNL SharePoint] 계정을 [!DNL Workfront Fusion]에 연결하는 방법에 대한 지침은 이 문서에서 <a href="#connect-sharepoint-to-workfront-fusion" class="MCXref xref" data-mc-variable-override="">[!DNL SharePoint]을(를) [!DNL Workfront Fusion]</a>에 연결 을 참조하십시오.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL 항목 업데이트]</td> 
   <td> <p>업데이트하려는 항목이 포함된 사이트 및 목록을 식별하는 방법을 선택합니다.</p> 
    <ul> 
     <li> <p><strong>[!UICONTROL Enter manually]</strong> </p> <p>표시되는 필드에 <strong>[!UICONTROL 사이트 ID]</strong>, <strong>[!UICONTROL 목록 ID]</strong> 및 <strong>[!UICONTROL 항목 ID]</strong>을(를) 입력하거나 매핑합니다.</p> </li> 
     <li> <p><strong>[!UICONTROL 목록에서 선택]</strong> </p> <p>업데이트할 항목이 들어 있는 사이트를 선택한 다음 목록을 선택하고 항목을 선택합니다. </p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL 필드]</td> 
   <td>신규 품목에 대해 갱신할 각 필드에 대해 필드의 키(필드 식별)와 해당 필드에 대해 품목을 보유할 신규 값을 입력합니다.</td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL 항목 보기](예약됨)

이 트리거 모듈은 항목을 만들거나 수정할 때 시나리오를 시작합니다.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td> 
   <td> <p>[!DNL SharePoint] 계정을 [!DNL Workfront Fusion]에 연결하는 방법에 대한 지침은 이 문서에서 <a href="#connect-sharepoint-to-workfront-fusion" class="MCXref xref" data-mc-variable-override="">[!DNL SharePoint]을(를) [!DNL Workfront Fusion]</a>에 연결 을 참조하십시오.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL 감시 목록]</td> 
   <td>생성 시간(새 항목)별로 또는 수정 시간(업데이트된 항목)별로 목록을 시청할지 여부를 선택합니다.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Enter Site and List ID]</td> 
   <td> <p>보려는 사이트 및 목록을 식별하는 방법을 선택합니다.</p> 
    <ul> 
     <li> <p><strong>[!UICONTROL Enter manually]</strong> </p> <p>표시되는 필드에 <strong>[!UICONTROL 사이트 ID]</strong> 및 <strong>[!UICONTROL 목록 ID]</strong>을(를) 입력하거나 매핑합니다.</p> </li> 
     <li> <p><strong>[!UICONTROL 팔로우하는 목록에서 선택]</strong> </p> <p>보려는 사이트를 선택한 다음 목록을 선택합니다. 이러한 드롭다운은 팔로우한 사이트만 검색합니다.</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL 제한]</td> 
   <td> <p>각 시나리오 실행 주기 동안 모듈이 반환할 최대 항목 수를 입력하거나 매핑합니다.</p> </td> 
  </tr> 
 </tbody> 
</table>

### 목록

* [[!UICONTROL 목록 만들기]](#create-a-list)
* [[!UICONTROL 목록 가져오기]](#get-a-list)
* [[!UICONTROL 목록]](#list-lists)
* [[!UICONTROL 시청 목록]](#watch-lists)

#### [!UICONTROL 목록 만들기]

이 작업 모듈은 SharePoint에 새 목록을 만듭니다.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td> 
   <td> <p>[!DNL SharePoint] 계정을 [!DNL Workfront Fusion]에 연결하는 방법에 대한 지침은 이 문서에서 <a href="#connect-sharepoint-to-workfront-fusion" class="MCXref xref" data-mc-variable-override="">[!DNL SharePoint]을(를) [!DNL Workfront Fusion]</a>에 연결 을 참조하십시오.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL 사이트 ID 입력]</td> 
   <td> <p>목록을 만들 사이트 및 목록을 식별하는 방법을 선택합니다.</p> 
    <ul> 
     <li> <p><strong>[!UICONTROL Enter manually]</strong> </p> <p>목록을 만들 <strong>[!UICONTROL 사이트 ID]</strong>을(를) 입력하거나 매핑합니다.</p> </li> 
     <li> <p><strong>[!UICONTROL 목록에서 선택]</strong> </p> <p>목록을 만들 사이트를 선택합니다. </p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Display Name]</td> 
   <td>새 목록의 이름을 입력하거나 매핑합니다.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL 설명]</td> 
   <td>새 목록에 대한 설명을 입력하거나 매핑합니다.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL 열 추가]</td> 
   <td>새 목록에 대해 설정할 각 열에 대해 필드에 <strong>[!UICONTROL 이름]</strong>을(를) 입력하고 새 열에 사용할 값의 <strong>[!UICONTROL 유형]</strong>을(를) 선택합니다.</td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL 목록 가져오기]

이 작업 모듈은 지정된 목록의 데이터를 반환합니다.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td> 
   <td> <p>[!DNL SharePoint] 계정을 [!DNL Workfront Fusion]에 연결하는 방법에 대한 지침은 이 문서에서 <a href="#connect-sharepoint-to-workfront-fusion" class="MCXref xref" data-mc-variable-override="">[!DNL SharePoint]을(를) [!DNL Workfront Fusion]</a>에 연결 을 참조하십시오.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL 목록 가져오기]</td> 
   <td> <p>가져오려는 항목이 포함된 사이트 및 목록을 식별하는 방법을 선택합니다.</p> 
    <ul> 
     <li> <p><strong>[!UICONTROL Enter manually]</strong> </p> <p>표시되는 필드에 <strong>[!UICONTROL 사이트 ID]</strong> 및 <strong>목록 ID</strong>을(를) 입력하거나 매핑합니다.</p> </li> 
     <li> <p><strong>[!UICONTROL 목록에서 선택]</strong> </p> <p>검색할 목록이 포함된 사이트를 선택한 다음 목록을 선택합니다. </p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL 목록]

이 작업 모듈은 지정된 목록의 모든 항목 목록을 검색합니다.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td> 
   <td> <p>[!DNL SharePoint] 계정을 [!DNL Workfront Fusion]에 연결하는 방법에 대한 지침은 이 문서에서 <a href="#connect-sharepoint-to-workfront-fusion" class="MCXref xref" data-mc-variable-override="">[!DNL SharePoint]을(를) [!DNL Workfront Fusion]</a>에 연결 을 참조하십시오.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL 목록]</td> 
   <td> <p>목록을 검색할 사이트를 식별하는 방법을 선택합니다.</p> 
    <ul> 
     <li> <p><strong>[!UICONTROL Enter manually]</strong> </p> <p><strong>[!UICONTROL 사이트 ID]</strong>을(를) 입력하거나 매핑합니다.</p> </li> 
     <li> <p><strong>[!UICONTROL 목록에서 선택]</strong> </p> <p>검색할 목록이 포함된 사이트를 선택합니다. 드롭다운은 팔로우하는 사이트만 검색합니다.</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL 제한]</td> 
   <td> <p>각 시나리오 실행 주기 동안 모듈이 반환할 최대 목록 수를 입력하거나 매핑합니다.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL 시청 목록]

이 트리거 모듈은 목록을 만들거나 수정할 때 시나리오를 시작합니다.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td> 
   <td> <p>[!DNL SharePoint] 계정을 [!DNL Workfront Fusion]에 연결하는 방법에 대한 지침은 이 문서에서 <a href="#connect-sharepoint-to-workfront-fusion" class="MCXref xref" data-mc-variable-override="">[!DNL SharePoint]을(를) [!DNL Workfront Fusion]</a>에 연결 을 참조하십시오.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL 감시 목록]</td> 
   <td>생성 시간(새 항목)별로 또는 수정 시간(업데이트된 항목)별로 목록을 시청할지 여부를 선택합니다.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Enter Site and List ID]</td> 
   <td> <p>보려는 사이트 및 목록을 식별하는 방법을 선택합니다.</p> 
    <ul> 
     <li> <p><strong>[!UICONTROL Enter manually]</strong> </p> <p>보려는 목록이 있는 <strong>[!UICONTROL 사이트 ID]</strong>을(를) 입력하거나 매핑하십시오.</p> </li> 
     <li> <p><strong>[!UICONTROL 팔로우하는 목록에서 선택]</strong> </p> <p>보려는 사이트를 선택합니다. 드롭다운은 팔로우하는 사이트만 검색합니다.</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL 제한]</td> 
   <td> <p>각 시나리오 실행 주기 동안 모듈이 반환할 최대 목록 수를 입력하거나 매핑합니다.</p> </td> 
  </tr> 
 </tbody> 
</table>

### 페이지(Beta)

>[!NOTE]
>
>[!DNL Microsoft Graph]에서 `beta` 버전의 API는 변경될 수 있습니다. 프로덕션 응용 프로그램에서는 이러한 API를 사용할 수 없습니다.

#### [!UICONTROL 페이지 가져오기]

이 작업 모듈은 지정된 페이지의 데이터를 반환합니다.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td> 
   <td> <p>[!DNL SharePoint] 계정을 [!DNL Workfront Fusion]에 연결하는 방법에 대한 지침은 이 문서에서 <a href="#connect-sharepoint-to-workfront-fusion" class="MCXref xref" data-mc-variable-override="">[!DNL SharePoint]을(를) [!DNL Workfront Fusion]</a>에 연결 을 참조하십시오.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL 페이지 가져오기]</td> 
   <td> <p>검색할 페이지를 식별하는 방법을 선택합니다.</p> 
    <ul> 
     <li> <p><strong>[!UICONTROL Enter manually]</strong> </p> <p><strong>[!UICONTROL 사이트 ID]</strong> 및 <strong>[!UICONTROL 페이지 ID]</strong>을(를) 입력하거나 매핑합니다.</p> </li> 
     <li> <p><strong>[!UICONTROL 목록에서 선택]</strong> </p> <p>검색할 페이지가 포함된 사이트를 선택한 다음 페이지를 선택합니다.</p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

### Site

* [[!UICONTROL 사이트 가져오기]](#get-a-site)
* [[!UICONTROL 사이트 검색]](#search-sites)

#### [!UICONTROL 사이트 가져오기]

이 작업 모듈은 지정된 사이트의 데이터를 반환합니다.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td> 
   <td> <p>[!DNL SharePoint] 계정을 [!DNL Workfront Fusion]에 연결하는 방법에 대한 지침은 이 문서에서 <a href="#connect-sharepoint-to-workfront-fusion" class="MCXref xref" data-mc-variable-override="">[!DNL SharePoint]을(를) [!DNL Workfront Fusion]</a>에 연결 을 참조하십시오.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL 사이트 가져오기]</td> 
   <td> <p>검색할 페이지를 식별하는 방법을 선택합니다.</p> 
    <ul> 
     <li> <p><strong>[!UICONTROL Enter manually]</strong> </p> <p><strong>[!UICONTROL 사이트 ID]</strong>을(를) 입력하거나 매핑합니다.</p> </li> 
     <li> <p><strong>[!UICONTROL 목록에서 선택]</strong> </p> <p>검색할 사이트를 선택합니다.</p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL 사이트 검색]

이 작업 모듈은 지정한 매개 변수로 사이트를 검색합니다.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td> 
   <td> <p>[!DNL SharePoint] 계정을 [!DNL Workfront Fusion]에 연결하는 방법에 대한 지침은 이 문서에서 <a href="#connect-sharepoint-to-workfront-fusion" class="MCXref xref" data-mc-variable-override="">[!DNL SharePoint]을(를) [!DNL Workfront Fusion]</a>에 연결 을 참조하십시오.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Keyword of Display Name]</td> 
   <td> <p>사이트를 검색할 검색어를 입력하거나 매핑합니다.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL 제한]</td> 
   <td> <p>각 시나리오 실행 주기 동안 모듈이 반환할 최대 사이트 수를 입력하거나 매핑합니다.</p> </td> 
  </tr> 
 </tbody> 
</table>

### 기타

#### 변경 사항 가져오기

이 모듈은 SharePoint 폴더에서 만든 추가, 업데이트 및 삭제 작업을 검색합니다.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td> 
   <td> <p>[!DNL SharePoint] 계정을 [!DNL Workfront Fusion]에 연결하는 방법에 대한 지침은 이 문서에서 <a href="#connect-sharepoint-to-workfront-fusion" class="MCXref xref" data-mc-variable-override="">[!DNL SharePoint]을(를) [!DNL Workfront Fusion]</a>에 연결 을 참조하십시오.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL 사이트, 드라이브 및 폴더 ID 입력]</td> 
   <td> <p>업데이트하려는 항목이 포함된 사이트 및 목록을 식별하는 방법을 선택합니다.</p> 
    <ul> 
     <li> <p><strong>[!UICONTROL Enter manually]</strong> </p> <p>표시되는 필드에 <strong>[!UICONTROL 사이트 ID]</strong>, <strong>[!UICONTROL 드라이브 ID]</strong> 및 <strong>[!UICONTROL 폴더 ID]</strong>을(를) 입력하거나 매핑합니다.</p> </li> 
     <li> <p><strong>[!UICONTROL 목록에서 선택]</strong> </p> <p>업데이트할 항목이 있는 사이트를 선택한 다음 드라이브를 선택하고 폴더를 선택합니다. </p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Token]</td> 
   <td> 토큰은 모듈이 변경 사항 검색을 시작해야 하는 시점을 식별합니다.  </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL API 호출 만들기]

이 모듈에서는 사용자 지정 API 호출을 수행할 수 있습니다.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td> 
   <td> <p>[!DNL SharePoint] 계정을 [!DNL Workfront Fusion]에 연결하는 방법에 대한 지침은 이 문서에서 <a href="#connect-sharepoint-to-workfront-fusion" class="MCXref xref" data-mc-variable-override="">[!DNL SharePoint]을(를) [!DNL Workfront Fusion]</a>에 연결 을 참조하십시오.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL URL]</p> </td> 
   <td> <p><code>https://graph.microsoft.com</code>과(와) 관련된 경로를 입력하십시오. 예:<code> /beta/sites</code></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL 메서드]</p> </td> 
   <td> <p>API 호출을 구성하는 데 필요한 HTTP 요청 메서드를 선택합니다. 자세한 내용은 [!DNL Adobe Workfront Fusion]</a>에서 <a href="../../workfront-fusion/modules/http-request-methods.md" class="MCXref xref" data-mc-variable-override="">HTTP 요청 메서드를 참조하십시오.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Headers]</td> 
   <td> <p>표준 JSON 개체 형식으로 요청의 헤더를 추가합니다(예: <code>{"Content-type":"application/json"}</code>). [!DNL Workfront Fusion]이(가) 권한 부여 헤더를 추가합니다.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL 쿼리 문자열]</td> 
   <td> <p> 표준 JSON 개체 형식으로 API 호출에 대한 쿼리를 추가합니다.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL 유형]</td> 
   <td>API 호출에서 전송할 데이터 유형을 선택합니다.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Body]</td> 
   <td> <p>표준 JSON 개체의 형태로 API 호출에 대한 본문 콘텐츠를 추가합니다.</p> <p>참고:  <p>JSON에서 <code>if</code>과(와) 같은 조건문을 사용할 때 따옴표를 조건문 외부에 넣으십시오.</p> 
     <div class="example" data-mc-autonum="<b>Example: </b>"> 
      <p> <img src="assets/quotes-in-json-350x120.png" style="width: 350;height: 120;"> </p> 
     </div> </p> </td> 
  </tr> 
 </tbody> 
</table>

#### 이벤트 보기

이 즉시 트리거 모듈은 SharePoint에서 항목이 추가, 업데이트 또는 삭제될 때 시나리오를 시작합니다.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
  <!--
   <td role="rowheader">[!UICONTROL Connection]</td> 
   <td> <p>For instructions about connecting your [!DNL SharePoint] account to [!DNL Workfront Fusion], see <a href="#connect-sharepoint-to-workfront-fusion" class="MCXref xref" data-mc-variable-override="">Connect [!DNL SharePoint] to [!DNL Workfront Fusion]</a> in this article.</p> </td> 
  </tr> 
  -->
  <tr> 
   <td role="rowheader">[!UICONTROL Webhook]</td> 
   <td> <p>기존 웹후크를 선택하거나 추가 를 클릭하여 새 웹후크를 생성합니다.</p> 
   </td> 
  </tr> 
 </tbody> 
</table>

