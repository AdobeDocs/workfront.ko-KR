---
content-type: reference
product-previous: workfront-fusion
product-area: workfront-integrations
keywords: 커넥터
navigation-topic: apps-and-their-modules
title: SharePoint 모듈
description: 에서 [!DNL Adobe Workfront Fusion] 시나리오 SharePoint을 사용하는 워크플로우를 자동화하고 여러 타사 애플리케이션 및 서비스에 연결할 수 있습니다.
author: Becky
feature: Workfront Fusion
exl-id: 16d49031-06d2-4c86-bac4-f58cd9b2f1f5
source-git-commit: 83914e54638ffbef2b3ccee12c71b84ca7cc61d2
workflow-type: tm+mt
source-wordcount: '2660'
ht-degree: 0%

---

# [!DNL SharePoint] 모듈

에서 [!DNL Adobe Workfront Fusion] 시나리오, [!DNL SharePoint]여러 타사 애플리케이션 및 서비스에 연결할 수 있습니다.

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

를 사용하려면 [!DNL SharePoint] 모듈이면 반드시 [!DNL SharePoint] 계정이 필요합니다.

## Connect [!DNL SharePoint] to [!DNL Workfront Fusion] {#connect-sharepoint-to-workfront-fusion}

* [Connect [!DNL SharePoint] to [!DNL Workfront Fusion] 사용 [!DNL Microsoft] account](#connect-sharepoint-to-workfront-fusion-using-a-microsoft-account)
* [Connect [!DNL SharePoint] to [!DNL Workfront Fusion] 고급 설정 사용](#connect-sharepoint-to-workfront-fusion-using-advanced-settings)

### Connect [!DNL SharePoint] to [!DNL Workfront Fusion] 사용 [!DNL Microsoft] account

을(를) 사용할 수 있습니다 [!DNL Microsoft] 연결을 만들 계정 [!DNL SharePoint]. 연결 방법에 대한 지침은 [!DNL Sharepoint] 계정 대상 [!DNL Workfront Fusion]를 참조하십시오. [연결 만들기 [!DNL Adobe Workfront Fusion] - 기본 지침](../../workfront-fusion/connections/connect-to-fusion-general.md)

### Connect [!DNL SharePoint] to [!DNL Workfront Fusion] 고급 설정 사용

연결하려면 [!DNL SharePoint] to [!DNL Workfront Fusion] 없이 [!DNL Microsoft] account에는 클라이언트 ID, 클라이언트 암호 및 테넌트 ID가 필요합니다.

1. 클릭 **[!UICONTROL 추가]** 위쪽 **[!DNL SharePoint]** 상자를 열어 **[!UICONTROL 연결 만들기]** 상자.

1. (선택 사항) 기본값 변경 **[!UICONTROL 연결 이름]**.
1. 클릭 **[!UICONTROL 고급 설정 표시]**.
1. 을(를) 입력합니다. [!DNL SharePoint] **[!UICONTROL 클라이언트 ID]** 및 **[!UICONTROL 클라이언트 암호]**.

1. 클릭 **[!UICONTROL 계속]**.
1. 표시되는 로그인 창에서 아직 로그인하지 않은 경우 앱에 로그인할 자격 증명을 입력합니다.
1. (조건부) **[!UICONTROL 허용]** 단추가 표시되면 단추를 클릭하여 앱을 연결할 수 있습니다 [!DNL Workfront Fusion].

## [!DNL SharePoint] 모듈 및 해당 필드

구성 시 [!DNL SharePoint] 모듈, [!DNL Workfront Fusion] 아래 나열된 필드를 표시합니다. 이와 함께 추가 [!DNL SharePoint] 앱이나 서비스에서 액세스 수준과 같은 요소에 따라 필드가 표시될 수 있습니다. 모듈에서 굵게 표시된 제목은 필수 필드를 나타냅니다.

필드 또는 함수 위에 맵 단추가 표시되면 이 단추를 사용하여 해당 필드에 대한 변수와 함수를 설정할 수 있습니다. 자세한 내용은 [의 한 모듈에서 다른 모듈로 정보 매핑 [!DNL Adobe Workfront Fusion]](../../workfront-fusion/mapping/map-information-between-modules.md).

![](assets/map-toggle-350x74.png)

* [드라이브 항목](#drive-item)
* [항목](#item)
* [목록](#list)
* [페이지(베타)](#page-beta)
* [사이트](#site)
* [기타](#other)

### 드라이브 항목

* [파일 만들기](#create-a-file)
* [폴더 만들기](#create-a-folder)
* [파일 가져오기](#get-a-file)
* [감시 폴더 항목](#watch-folder-items)

#### 변경 내용 가져오기

이 모듈은 SharePoint에 수행된 변경 사항을 반환합니다.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td> 
   <td> <p>연결 방법에 대한 지침은 [!DNL SharePoint] 계정 대상 [!DNL Workfront Fusion]를 참조하십시오. <a href="#connect-sharepoint-to-workfront-fusion" class="MCXref xref" data-mc-variable-override="">Connect [!DNL SharePoint] to [!DNL Workfront Fusion]</a> 참조하십시오.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL 사이트, 드라이브 및 폴더 ID 입력]</td> 
   <td> <p>에서 변경 내용을 검색할 폴더의 위치를 식별할 방법을 선택합니다.</p> 
    <ul> 
     <li> <p><strong>[!UICONTROL 수동으로 Enter]</strong> </p> <p>을 입력하거나 매핑합니다 <strong>[!UICONTROL 사이트 ID]</strong>, <strong>[!UICONTROL 목록 ID]</strong>, 및 <strong>[!UICONTROL 폴더 ID]</strong> 표시됩니다.</p> </li> 
     <li> <p><strong>[!UICONTROL 팔로우하는 목록에서 선택합니다.]</strong> </p> <p>변경 사항을 검색할 위치를 선택합니다. </p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Token]</td> 
   <td> </td> 
  </tr>  </tbody> 
</table>

#### 폴더 만들기

이 작업 모듈은 SharePoint에서 새 폴더를 만듭니다.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td> 
   <td> <p>연결 방법에 대한 지침은 [!DNL SharePoint] 계정 대상 [!DNL Workfront Fusion]를 참조하십시오. <a href="#connect-sharepoint-to-workfront-fusion" class="MCXref xref" data-mc-variable-override="">Connect [!DNL SharePoint] to [!DNL Workfront Fusion]</a> 참조하십시오.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL 사이트, 드라이브 및 폴더 ID 입력]</td> 
   <td> <p>만들 폴더의 위치를 식별할 방법을 선택합니다.</p> 
    <ul> 
     <li> <p><strong>[!UICONTROL 수동으로 Enter]</strong> </p> <p>을 입력하거나 매핑합니다 <strong>[!UICONTROL 사이트 ID]</strong>, <strong>[!UICONTROL 목록 ID]</strong>, 및 <strong>[!UICONTROL 폴더 ID]</strong> 표시됩니다.</p> </li> 
     <li> <p><strong>[!UICONTROL 팔로우하는 목록에서 선택합니다.]</strong> </p> <p>폴더를 만들 위치를 선택합니다. </p> </li> 
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
   <td> <p>연결 방법에 대한 지침은 [!DNL SharePoint] 계정 대상 [!DNL Workfront Fusion]를 참조하십시오. <a href="#connect-sharepoint-to-workfront-fusion" class="MCXref xref" data-mc-variable-override="">Connect [!DNL SharePoint] to [!DNL Workfront Fusion]</a> 참조하십시오.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL 사이트, 드라이브 및 폴더 ID 입력]</td> 
   <td> <p>가져올 파일의 위치를 식별하는 방법을 선택합니다.</p> 
    <ul> 
     <li> <p><strong>[!UICONTROL 수동으로 Enter]</strong> </p> <p>을 입력하거나 매핑합니다 <strong>[!UICONTROL 사이트 ID]</strong>, <strong>[!UICONTROL 목록 ID]</strong>, 및 <strong>[!UICONTROL 파일 ID]</strong> 표시됩니다.</p> </li> 
     <li> <p><strong>[!UICONTROL 팔로우하는 목록에서 선택합니다.]</strong> </p> <p>파일의 위치를 선택합니다. </p> </li> 
    </ul> </td> 
  </tr> 
</tbody> 
</table>

#### 감시 폴더 항목

이 트리거 모듈은 선택한 폴더에서 항목이 업데이트되면 시나리오를 시작합니다.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td> 
   <td> <p>연결 방법에 대한 지침은 [!DNL SharePoint] 계정 대상 [!DNL Workfront Fusion]를 참조하십시오. <a href="#connect-sharepoint-to-workfront-fusion" class="MCXref xref" data-mc-variable-override="">Connect [!DNL SharePoint] to [!DNL Workfront Fusion]</a> 참조하십시오.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL 사이트, 드라이브 및 폴더 ID 입력]</td> 
   <td> <p>가져올 파일의 위치를 식별하는 방법을 선택합니다.</p> 
    <ul> 
     <li> <p><strong>[!UICONTROL 수동으로 Enter]</strong> </p> <p>을 입력하거나 매핑합니다 <strong>[!UICONTROL 사이트 ID]</strong>, <strong>[!UICONTROL 목록 ID]</strong>, 및 <strong>[!UICONTROL 폴더 ID]</strong> 표시됩니다.</p> </li> 
     <li> <p><strong>[!UICONTROL 팔로우하는 목록에서 선택합니다.]</strong> </p> <p>보려는 폴더의 위치를 선택합니다. </p> </li> 
    </ul> </td> 
  </tr> 
   <td role="rowheader">[!UICONTROL 제한]</td> 
   <td>최대 항목 수를 입력합니다 [!DNL Workfront Fusion] 한 시나리오 실행 주기 동안 를 반환해야 합니다.</td> 
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
* [[!UICONTROL 감시 항목] (예약됨)](#watch-items-scheduled)


#### [!UICONTROL 항목 복사]

이 작업 모듈은 SharePoint 목록에 있는 기존 항목을 복사합니다.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td> 
   <td> <p>연결 방법에 대한 지침은 [!DNL SharePoint] 계정 대상 [!DNL Workfront Fusion]를 참조하십시오. <a href="#connect-sharepoint-to-workfront-fusion" class="MCXref xref" data-mc-variable-override="">Connect [!DNL SharePoint] to [!DNL Workfront Fusion]</a> 참조하십시오.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">사이트, 드라이브 및 폴더 ID 입력</td> 
   <td> <p>복사할 항목이 들어 있는 사이트 및 목록을 식별하는 방법을 선택합니다.</p> 
    <ul> 
     <li> <p><strong>[!UICONTROL 수동으로 Enter]</strong> </p> <p>을 입력하거나 매핑합니다 <strong>[!UICONTROL 사이트 ID]</strong>, <strong>[!UICONTROL 목록 ID]</strong>, 및 <strong>[!UICONTROL 항목 ID]</strong> 표시됩니다.</p> </li> 
     <li> <p><strong>[!UICONTROL 팔로우하는 목록에서 선택]</strong> </p> <p>항목 유형 복사 필드에서 필드를 이동할지 폴더를 이동할지 선택합니다.  복사할 항목이 들어 있는 사이트를 선택한 다음 목록을 선택한 다음 항목을 선택합니다. </p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL 대상 ID]</td> 
   <td>  </td> 
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
   <td> <p>연결 방법에 대한 지침은 [!DNL SharePoint] 계정 대상 [!DNL Workfront Fusion]를 참조하십시오. <a href="#connect-sharepoint-to-workfront-fusion" class="MCXref xref" data-mc-variable-override="">Connect [!DNL SharePoint] to [!DNL Workfront Fusion]</a> 참조하십시오.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL 항목 만들기]</td> 
   <td> <p>항목을 만들 사이트 및 목록을 식별하는 방법을 선택합니다.</p> 
    <ul> 
     <li> <p><strong>[!UICONTROL 수동으로 Enter]</strong> </p> <p>을 입력하거나 매핑합니다 <strong>[!UICONTROL 사이트 ID]</strong> 및 <strong>[!UICONTROL 목록 ID]</strong> 표시됩니다.</p> </li> 
     <li> <p><strong>[!UICONTROL 목록에서 선택]</strong> </p> <p>항목을 만들 목록이 들어 있는 사이트를 선택한 다음 목록을 선택합니다. </p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Fields]</td> 
   <td>새 항목에 대해 설정하려는 각 필드에 필드의 키(필드를 식별)와 해당 필드에 대해 새 항목을 사용할 값을 입력합니다.</td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL 항목 삭제]

이 작업 모듈은 SharePoint 목록에 있는 기존 항목을 삭제합니다.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td> 
   <td> <p>연결 방법에 대한 지침은 [!DNL SharePoint] 계정 대상 [!DNL Workfront Fusion]를 참조하십시오. <a href="#connect-sharepoint-to-workfront-fusion" class="MCXref xref" data-mc-variable-override="">Connect [!DNL SharePoint] to [!DNL Workfront Fusion]</a> 참조하십시오.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL 항목 업데이트]</td> 
   <td> <p>삭제할 항목을 포함하는 사이트 및 목록을 식별하는 방법을 선택합니다.</p> 
    <ul> 
     <li> <p><strong>[!UICONTROL 수동으로 Enter]</strong> </p> <p>을 입력하거나 매핑합니다 <strong>[!UICONTROL 사이트 ID]</strong>, <strong>[!UICONTROL 목록 ID]</strong>, 및 <strong>[!UICONTROL 항목 ID]</strong> 표시됩니다.</p> </li> 
     <li> <p><strong>[!UICONTROL 목록에서 선택]</strong> </p> <p>삭제할 항목이 포함된 사이트를 선택한 다음 목록을 선택한 다음 항목을 선택합니다. </p> </li> 
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
   <td> <p>연결 방법에 대한 지침은 [!DNL SharePoint] 계정 대상 [!DNL Workfront Fusion]를 참조하십시오. <a href="#connect-sharepoint-to-workfront-fusion" class="MCXref xref" data-mc-variable-override="">Connect [!DNL SharePoint] to [!DNL Workfront Fusion]</a> 참조하십시오.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL 항목 가져오기]</td> 
   <td> <p>가져올 항목이 들어 있는 사이트 및 목록을 식별하는 방법을 선택합니다.</p> 
    <ul> 
     <li> <p><strong>[!UICONTROL 수동으로 Enter]</strong> </p> <p>을 입력하거나 매핑합니다 <strong>[!UICONTROL 사이트 ID]</strong>, <strong>[!UICONTROL 목록 ID]</strong>, 및 <strong>[!UICONTROL 항목 ID]</strong> 표시됩니다.</p> </li> 
     <li> <p><strong>[!UICONTROL 목록에서 선택]</strong> </p> <p>항목을 검색할 목록이 포함된 사이트를 선택한 다음 목록을 선택한 다음 항목을 선택합니다. </p> </li> 
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
   <td> <p>연결 방법에 대한 지침은 [!DNL SharePoint] 계정 대상 [!DNL Workfront Fusion]를 참조하십시오. <a href="#connect-sharepoint-to-workfront-fusion" class="MCXref xref" data-mc-variable-override="">Connect [!DNL SharePoint] to [!DNL Workfront Fusion]</a> 참조하십시오.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL List Items]</td> 
   <td> <p>항목을 검색할 목록을 식별할 방법을 선택합니다.</p> 
    <ul> 
     <li> <p><strong>[!UICONTROL 수동으로 Enter]</strong> </p> <p>을 입력하거나 매핑합니다 <strong>[!UICONTROL 사이트 ID]</strong> 및 <strong>[!UICONTROL 목록 ID]</strong> 표시됩니다.</p> </li> 
     <li> <p><strong>[!UICONTROL 목록에서 선택]</strong> </p> <p>항목을 검색할 목록이 들어 있는 사이트를 선택한 다음 목록을 선택합니다. </p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL 제한]</td> 
   <td> <p>각 시나리오 실행 주기 동안 모듈이 반환할 최대 항목 수를 입력하거나 매핑합니다.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL 항목 이동]

이 작업 모듈은 SharePoint 목록에 있는 기존 항목을 복사합니다.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td> 
   <td> <p>연결 방법에 대한 지침은 [!DNL SharePoint] 계정 대상 [!DNL Workfront Fusion]를 참조하십시오. <a href="#connect-sharepoint-to-workfront-fusion" class="MCXref xref" data-mc-variable-override="">Connect [!DNL SharePoint] to [!DNL Workfront Fusion]</a> 참조하십시오.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">사이트, 드라이브 및 폴더 ID 입력</td> 
   <td> <p>이동할 항목이 들어 있는 사이트 및 목록을 식별하는 방법을 선택합니다.</p> 
    <ul> 
     <li> <p><strong>[!UICONTROL 수동으로 Enter]</strong> </p> <p>을 입력하거나 매핑합니다 <strong>[!UICONTROL 사이트 ID]</strong>, <strong>[!UICONTROL 목록 ID]</strong>, 및 <strong>[!UICONTROL 항목 ID]</strong> 표시됩니다.</p> </li> 
     <li> <p><strong>[!UICONTROL 팔로우하는 목록에서 선택]</strong> </p> <p>항목 유형 복사 필드에서 필드를 이동할지 폴더를 이동할지 선택합니다. 복사할 항목이 들어 있는 사이트를 선택한 다음 목록을 선택한 다음 항목을 선택합니다. </p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL 대상 ID]</td> 
   <td>  </td> 
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
   <td> <p>연결 방법에 대한 지침은 [!DNL SharePoint] 계정 대상 [!DNL Workfront Fusion]를 참조하십시오. <a href="#connect-sharepoint-to-workfront-fusion" class="MCXref xref" data-mc-variable-override="">Connect [!DNL SharePoint] to [!DNL Workfront Fusion]</a> 참조하십시오.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL 항목 업데이트]</td> 
   <td> <p>업데이트할 항목이 들어 있는 사이트 및 목록을 식별하는 방법을 선택합니다.</p> 
    <ul> 
     <li> <p><strong>[!UICONTROL 수동으로 Enter]</strong> </p> <p>을 입력하거나 매핑합니다 <strong>[!UICONTROL 사이트 ID]</strong>, <strong>[!UICONTROL 목록 ID]</strong>, 및 <strong>[!UICONTROL 항목 ID]</strong> 표시됩니다.</p> </li> 
     <li> <p><strong>[!UICONTROL 목록에서 선택]</strong> </p> <p>업데이트할 항목이 포함된 사이트를 선택한 다음 목록을 선택한 다음 항목을 선택합니다. </p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Fields]</td> 
   <td>새 항목에 대해 업데이트할 각 필드에 대해 필드의 키(필드를 식별)와 해당 필드에 대해 항목이 가질 새 값을 입력합니다.</td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL 감시 항목] (예약됨)

이 트리거 모듈은 항목이 만들어지거나 수정되면 시나리오를 시작합니다.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td> 
   <td> <p>연결 방법에 대한 지침은 [!DNL SharePoint] 계정 대상 [!DNL Workfront Fusion]를 참조하십시오. <a href="#connect-sharepoint-to-workfront-fusion" class="MCXref xref" data-mc-variable-override="">Connect [!DNL SharePoint] to [!DNL Workfront Fusion]</a> 참조하십시오.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL 감시 목록]</td> 
   <td>만들기 시간(새 항목) 또는 수정 시간(업데이트된 항목)별로 목록을 감시할지 여부를 선택합니다.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL 사이트 및 목록 ID 입력]</td> 
   <td> <p>보려는 사이트 및 목록을 식별하는 방법을 선택합니다.</p> 
    <ul> 
     <li> <p><strong>[!UICONTROL 수동으로 Enter]</strong> </p> <p>을 입력하거나 매핑합니다 <strong>[!UICONTROL 사이트 ID]</strong> 및 <strong>[!UICONTROL 목록 ID]</strong> 표시됩니다.</p> </li> 
     <li> <p><strong>[!UICONTROL 팔로우하는 목록에서 선택합니다.]</strong> </p> <p>보려는 사이트를 선택한 다음 목록을 선택합니다. 이러한 드롭다운은 팔로우 사이트만 검색합니다.</p> </li> 
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
* [[!UICONTROL 목록 목록]](#list-lists)
* [[!UICONTROL 감시 목록]](#watch-lists)

#### [!UICONTROL 목록 만들기]

이 작업 모듈은 SharePoint에서 새 목록을 만듭니다.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td> 
   <td> <p>연결 방법에 대한 지침은 [!DNL SharePoint] 계정 대상 [!DNL Workfront Fusion]를 참조하십시오. <a href="#connect-sharepoint-to-workfront-fusion" class="MCXref xref" data-mc-variable-override="">Connect [!DNL SharePoint] to [!DNL Workfront Fusion]</a> 참조하십시오.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL 사이트 ID 입력]</td> 
   <td> <p>목록을 만들 사이트 및 목록을 식별하는 방법을 선택합니다.</p> 
    <ul> 
     <li> <p><strong>[!UICONTROL 수동으로 Enter]</strong> </p> <p>을 입력하거나 매핑합니다 <strong>[!UICONTROL 사이트 ID]</strong> 목록을 만들 위치.</p> </li> 
     <li> <p><strong>[!UICONTROL 목록에서 선택]</strong> </p> <p>목록을 만들 사이트를 선택합니다. </p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL 표시 이름]</td> 
   <td>새 목록의 이름을 입력하거나 매핑합니다.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Description]</td> 
   <td>새 목록에 대한 설명을 입력하거나 매핑합니다.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL 열 추가]</td> 
   <td>새 목록에 대해 설정할 각 열에 대해 <strong>[!UICONTROL Name]</strong> 필드에 대해 을(를) 선택하고 을(를) 선택합니다. <strong>[!UICONTROL Type]</strong> 새 열에 포함할 값.</td> 
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
   <td> <p>연결 방법에 대한 지침은 [!DNL SharePoint] 계정 대상 [!DNL Workfront Fusion]를 참조하십시오. <a href="#connect-sharepoint-to-workfront-fusion" class="MCXref xref" data-mc-variable-override="">Connect [!DNL SharePoint] to [!DNL Workfront Fusion]</a> 참조하십시오.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL 목록 가져오기]</td> 
   <td> <p>가져올 항목이 들어 있는 사이트 및 목록을 식별하는 방법을 선택합니다.</p> 
    <ul> 
     <li> <p><strong>[!UICONTROL 수동으로 Enter]</strong> </p> <p>을 입력하거나 매핑합니다 <strong>[!UICONTROL 사이트 ID]</strong> 및 <strong>목록 ID</strong> 표시됩니다.</p> </li> 
     <li> <p><strong>[!UICONTROL 목록에서 선택]</strong> </p> <p>검색할 목록이 포함된 사이트를 선택한 다음 목록을 선택합니다. </p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL 목록 목록]

이 작업 모듈은 지정된 목록의 모든 항목 목록을 검색합니다.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td> 
   <td> <p>연결 방법에 대한 지침은 [!DNL SharePoint] 계정 대상 [!DNL Workfront Fusion]를 참조하십시오. <a href="#connect-sharepoint-to-workfront-fusion" class="MCXref xref" data-mc-variable-override="">Connect [!DNL SharePoint] to [!DNL Workfront Fusion]</a> 참조하십시오.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL 목록]</td> 
   <td> <p>목록을 검색할 사이트를 식별하는 방법을 선택합니다.</p> 
    <ul> 
     <li> <p><strong>[!UICONTROL 수동으로 Enter]</strong> </p> <p>을 입력하거나 매핑합니다 <strong>[!UICONTROL 사이트 ID]</strong>.</p> </li> 
     <li> <p><strong>[!UICONTROL 목록에서 선택]</strong> </p> <p>검색할 목록이 포함된 사이트를 선택합니다. 드롭다운은 팔로우하는 사이트만 검색합니다.</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL 제한]</td> 
   <td> <p>각 시나리오 실행 주기 동안 모듈이 반환할 최대 목록 수를 입력하거나 매핑합니다.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL 감시 목록]

이 트리거 모듈은 목록을 만들거나 수정할 때 시나리오를 시작합니다.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td> 
   <td> <p>연결 방법에 대한 지침은 [!DNL SharePoint] 계정 대상 [!DNL Workfront Fusion]를 참조하십시오. <a href="#connect-sharepoint-to-workfront-fusion" class="MCXref xref" data-mc-variable-override="">Connect [!DNL SharePoint] to [!DNL Workfront Fusion]</a> 참조하십시오.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL 감시 목록]</td> 
   <td>만들기 시간(새 항목) 또는 수정 시간(업데이트된 항목)별로 목록을 감시할지 여부를 선택합니다.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL 사이트 및 목록 ID 입력]</td> 
   <td> <p>보려는 사이트 및 목록을 식별하는 방법을 선택합니다.</p> 
    <ul> 
     <li> <p><strong>[!UICONTROL 수동으로 Enter]</strong> </p> <p>을 입력하거나 매핑합니다 <strong>[!UICONTROL 사이트 ID]</strong> 보려는 목록이 있는 위치입니다.</p> </li> 
     <li> <p><strong>[!UICONTROL 팔로우하는 목록에서 선택합니다.]</strong> </p> <p>보려는 사이트를 선택합니다. 드롭다운은 사용자가 따르는 사이트만 검색합니다.</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL 제한]</td> 
   <td> <p>각 시나리오 실행 주기 동안 모듈이 반환할 최대 목록 수를 입력하거나 매핑합니다.</p> </td> 
  </tr> 
 </tbody> 
</table>

### 페이지(베타)

>[!NOTE]
>
>의 API `beta` 버전 [!DNL Microsoft Graph] 변경될 수 있습니다. 프로덕션 애플리케이션에서 이러한 API의 사용이 지원되지 않습니다.

#### [!UICONTROL 페이지 가져오기]

이 작업 모듈은 지정된 페이지의 데이터를 반환합니다.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td> 
   <td> <p>연결 방법에 대한 지침은 [!DNL SharePoint] 계정 대상 [!DNL Workfront Fusion]를 참조하십시오. <a href="#connect-sharepoint-to-workfront-fusion" class="MCXref xref" data-mc-variable-override="">Connect [!DNL SharePoint] to [!DNL Workfront Fusion]</a> 참조하십시오.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL 페이지 가져오기]</td> 
   <td> <p>검색할 페이지를 식별하는 방법을 선택합니다.</p> 
    <ul> 
     <li> <p><strong>[!UICONTROL 수동으로 Enter]</strong> </p> <p>을 입력하거나 매핑합니다 <strong>[!UICONTROL 사이트 ID]</strong>및 <strong>[!UICONTROL 페이지 ID]</strong>.</p> </li> 
     <li> <p><strong>[!UICONTROL 목록에서 선택]</strong> </p> <p>검색할 페이지가 포함된 사이트를 선택한 다음 페이지를 선택합니다.</p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

### 사이트

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
   <td> <p>연결 방법에 대한 지침은 [!DNL SharePoint] 계정 대상 [!DNL Workfront Fusion]를 참조하십시오. <a href="#connect-sharepoint-to-workfront-fusion" class="MCXref xref" data-mc-variable-override="">Connect [!DNL SharePoint] to [!DNL Workfront Fusion]</a> 참조하십시오.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL 사이트 가져오기]</td> 
   <td> <p>검색할 페이지를 식별하는 방법을 선택합니다.</p> 
    <ul> 
     <li> <p><strong>[!UICONTROL 수동으로 Enter]</strong> </p> <p>을 입력하거나 매핑합니다 <strong>[!UICONTROL 사이트 ID]</strong>.</p> </li> 
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
   <td> <p>연결 방법에 대한 지침은 [!DNL SharePoint] 계정 대상 [!DNL Workfront Fusion]를 참조하십시오. <a href="#connect-sharepoint-to-workfront-fusion" class="MCXref xref" data-mc-variable-override="">Connect [!DNL SharePoint] to [!DNL Workfront Fusion]</a> 참조하십시오.</p> </td> 
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

#### [!UICONTROL API 호출 만들기]

이 모듈에서 사용자 지정 API 호출을 수행할 수 있습니다.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td> 
   <td> <p>연결 방법에 대한 지침은 [!DNL SharePoint] 계정 대상 [!DNL Workfront Fusion]를 참조하십시오. <a href="#connect-sharepoint-to-workfront-fusion" class="MCXref xref" data-mc-variable-override="">Connect [!DNL SharePoint] to [!DNL Workfront Fusion]</a> 참조하십시오.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL URL]</p> </td> 
   <td> <p>상대 경로 입력 <code>https://graph.microsoft.com</code>. 예:<code> /beta/sites</code></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL 메서드]</p> </td> 
   <td> <p>API 호출을 구성하는 데 필요한 HTTP 요청 메서드를 선택합니다. 자세한 내용은 <a href="../../workfront-fusion/modules/http-request-methods.md" class="MCXref xref" data-mc-variable-override="">의 HTTP 요청 메서드 [!DNL Adobe Workfront Fusion]</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Headers]</td> 
   <td> <p>요청의 헤더를 표준 JSON 개체 형태로 추가합니다. 예: <code>{"Content-type":"application/json"}</code>. [!DNL Workfront Fusion] 사용자를 위해 인증 헤더를 추가합니다.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL 쿼리 문자열]</td> 
   <td> <p> 표준 JSON 개체 형태로 API 호출에 대한 쿼리를 추가합니다.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Type]</td> 
   <td>API 호출에서 전송할 데이터 유형을 선택합니다.</td> 
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

#### 이벤트 보기

이 인스턴트 트리거 모듈은 SharePoint에서 항목이 추가, 업데이트 또는 삭제될 때 시나리오를 시작합니다.

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
   <td> <p>기존 웹 후크를 선택하거나 추가 를 클릭하여 새 웹 후크를 만듭니다.</p> 
   </td> 
  </tr> 
 </tbody> 
</table>

