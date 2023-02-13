---
content-type: reference
product-previous: workfront-fusion
product-area: workfront-integrations;documents
keywords: 커넥터
navigation-topic: apps-and-their-modules
title: Microsoft Office 365 Excel 모듈
description: 에서 [!DNL Adobe Workfront Fusion] 시나리오는 Microsoft 365 Excel을 사용하는 워크플로우를 자동화하고 여러 타사 애플리케이션 및 서비스에 연결할 수 있습니다.
author: Becky
feature: Workfront Fusion, Digital Content and Documents
exl-id: 9aa3739d-6800-4eb1-a17f-32fdfd8ed0f2
source-git-commit: 885d93dd4383945538e977fd3edbfd55bda88b70
workflow-type: tm+mt
source-wordcount: '2577'
ht-degree: 0%

---

# [!DNL Microsoft Office 365 Excel] 모듈

에서 [!DNL Adobe Workfront Fusion] 시나리오, [!DNL Microsoft 365 Excel]여러 타사 애플리케이션 및 서비스에 연결할 수 있습니다.

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
   <td> <p>[!UICONTROL [!DNL Workfront Fusion] 작업 자동화 및 통합을 위한] </p>  </td>  
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

를 사용하려면 [!DNL Microsoft office 365 Excel], Microsoft 계정이 있어야 합니다.

## [!DNL Microsoft Office 365 Excel] 모듈 및 해당 필드

구성 시 [!DNL Microsoft 365 Excel] 모듈, [!DNL Workfront Fusion] 아래 나열된 필드를 표시합니다. 이와 함께 추가 [!DNL Microsoft 365 Excel] 앱이나 서비스에서 액세스 수준과 같은 요소에 따라 필드가 표시될 수 있습니다. 모듈에서 굵게 표시된 제목은 필수 필드를 나타냅니다.

필드 또는 함수 위에 맵 단추가 표시되면 이 단추를 사용하여 해당 필드에 대한 변수와 함수를 설정할 수 있습니다. 자세한 내용은 [의 한 모듈에서 다른 모듈로 정보 매핑 [!DNL Adobe Workfront Fusion]](../../workfront-fusion/mapping/map-information-between-modules.md).

![](assets/map-toggle-350x74.png)

* [통합 문서](#workbook)
* [워크시트](#worksheet)
* [테이블](#table)
* [기타](#other)

### 통합 문서

* [통합 문서 보기](#watch-workbooks)
* [통합 문서 검색](#search-workbooks)
* [통합 문서 다운로드](#download-a-workbook)

#### [!UICONTROL 통합 문서 보기]

이 트리거 모듈은 통합 문서를 만들 때 시나리오를 시작합니다.

<table style="table-layout:auto"> 
 <col data-mc-conditions=""> 
 <col data-mc-conditions=""> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Connection]</p> </td> 
   <td> <p>연결 방법에 대한 지침은 [!DNL Office 365] 계정 대상 [!DNL Workfront Fusion]를 참조하십시오. <a href="../../workfront-fusion/scenarios/create-a-scenario.md#connect" class="MCXref xref">모듈의 앱 또는 웹 서비스를 [!DNL Workfront Fusion]</a> 기사 <a href="../../workfront-fusion/scenarios/create-a-scenario.md" class="MCXref xref">에서 시나리오 만들기 [!DNL Adobe Workfront Fusion]</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Folder]</td> 
   <td> <p>새 통합 문서에서 보려는 폴더를 선택합니다.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Filter]</p> </td> 
   <td> <p>선택한 기준에 맞는 통합 문서만 표시하도록 필터를 설정할 수 있습니다.</p> <p>각 필터에 대해 필터를 평가할 필드, 연산자 및 필터를 허용할 값을 입력합니다. AND 또는 OR 규칙을 추가하여 두 개 이상의 필터를 사용할 수 있습니다.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL 제한]</td> 
   <td> <p>각 시나리오 실행 주기 동안 모듈이 반환할 최대 통합 문서 수를 입력하거나 매핑합니다.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL 통합 문서 검색]

이 작업 모듈은 [!DNL Excel] 통합 문서.

<table style="table-layout:auto"> 
 <col data-mc-conditions=""> 
 <col data-mc-conditions=""> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Connection]</p> </td> 
   <td> <p>연결 방법에 대한 지침은 [!DNL Office 365] 계정 대상 [!DNL Workfront Fusion]를 참조하십시오. <a href="../../workfront-fusion/scenarios/create-a-scenario.md#connect" class="MCXref xref">모듈의 앱 또는 웹 서비스를 [!DNL Workfront Fusion]</a> 기사 <a href="../../workfront-fusion/scenarios/create-a-scenario.md" class="MCXref xref">에서 시나리오 만들기 [!DNL Adobe Workfront Fusion]</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Folder]</td> 
   <td> <p>통합 문서를 검색할 폴더를 선택합니다.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Filter]</p> </td> 
   <td> <p>선택한 기준에 맞는 통합 문서만 검색하도록 필터를 설정할 수 있습니다.</p> <p>각 필터에 대해 필터를 평가할 필드, 연산자 및 필터를 허용할 값을 입력합니다. AND 또는 OR 규칙을 추가하여 두 개 이상의 필터를 사용할 수 있습니다.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL 제한]</td> 
   <td> <p>각 시나리오 실행 주기 동안 모듈이 반환할 최대 워크시트 수를 입력하거나 매핑합니다.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL 통합 문서 다운로드]

이 작업 모듈은 지정된 Excel 통합 문서의 컨텐츠를 다운로드합니다.

<table style="table-layout:auto"> 
 <col data-mc-conditions=""> 
 <col data-mc-conditions=""> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Connection]</p> </td> 
   <td> <p>연결 방법에 대한 지침은 [!DNL Office 365] 계정 대상 [!DNL Workfront Fusion]를 참조하십시오. <a href="../../workfront-fusion/scenarios/create-a-scenario.md#connect" class="MCXref xref">모듈의 앱 또는 웹 서비스를 [!DNL Workfront Fusion]</a> 기사 <a href="../../workfront-fusion/scenarios/create-a-scenario.md" class="MCXref xref">에서 시나리오 만들기 [!DNL Adobe Workfront Fusion]</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL 통합 문서 다운로드]</td> 
   <td> <p>다운로드할 모듈의 통합 문서를 식별하는 방법을 선택합니다.</p> 
    <ul> 
     <li> <p><strong>[!UICONTROL ID를 수동으로 입력]</strong> </p> <p>[!UICONTROL 통합 문서 ID] 필드에서 모듈을 다운로드할 특정 통합 문서의 ID를 입력하거나 매핑합니다.</p> </li> 
     <li> <p><strong>[!UICONTROL 경로에서 선택하여]</strong> </p> <p>[!UICONTROL 통합 문서] 필드에서 모듈을 다운로드할 통합 문서를 선택합니다.</p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

### 워크시트

* [[!UICONTROL 워크시트 행 조회]](#watch-worksheet-rows)
* [[!UICONTROL 목록 워크시트]](#list-worksheets)
* [[!UICONTROL 워크시트 행 나열]](#list-worksheet-rows)
* [[!UICONTROL 워크시트 추가]](#add-a-worksheet)
* [[!UICONTROL 워크시트 행 추가]](#add-a-worksheet-row)
* [[!UICONTROL 워크시트 행 업데이트]](#update-a-worksheet-row)
* [[!UICONTROL 워크시트 행 삭제]](#delete-a-worksheet-row)

#### [!UICONTROL 워크시트 행 조회]

이 트리거 모듈은 시트에 새 행이 추가되면 시나리오를 시작합니다.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Connection]</p> </td> 
   <td> <p>연결 방법에 대한 지침은 [!DNL Office 365] 계정 대상 [!DNL Workfront Fusion]를 참조하십시오. <a href="../../workfront-fusion/scenarios/create-a-scenario.md#connect" class="MCXref xref">모듈의 앱 또는 웹 서비스를 [!DNL Workfront Fusion]</a> 기사 <a href="../../workfront-fusion/scenarios/create-a-scenario.md" class="MCXref xref">에서 시나리오 만들기 [!DNL Adobe Workfront Fusion]</a>.</p> </td> 
  </tr> 
  <tr> 
    <td role="rowheader" >[!UICONTROL Workbook] </td>
   <td> <p>새 행을 검사할 워크시트가 들어 있는 통합 문서를 선택합니다.</p> </td> 
  </tr> 
  <tr>
    <td role="rowheader" >[!UICONTROL Worksheet] </td>
   <td> <p>새 행을 보려는 Excel 시트를 선택합니다.</p> </td> 
  </tr> 
  <tr> 
    <td role="rowheader" >[!UICONTROL 제한]</td>
   <td> <p>각 시나리오 실행 주기 동안 모듈이 반환할 최대 워크시트 행 수를 입력하거나 매핑합니다.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL 목록 워크시트]

이 작업 모듈은 지정된 통합 문서의 워크시트 목록을 검색합니다.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Connection]</p> </td> 
   <td> <p>연결 방법에 대한 지침은 [!DNL Office 365] 계정 대상 [!DNL Workfront Fusion]를 참조하십시오. <a href="../../workfront-fusion/scenarios/create-a-scenario.md#connect" class="MCXref xref">모듈의 앱 또는 웹 서비스를 [!DNL Workfront Fusion]</a> 기사 <a href="../../workfront-fusion/scenarios/create-a-scenario.md" class="MCXref xref">에서 시나리오 만들기 [!DNL Adobe Workfront Fusion]</a>.</p> </td> 
  </tr> 
  <tr> 
    <td role="rowheader" >[!UICONTROL Workbook] </td>
   <td> <p>모듈이 나열할 워크시트가 포함된 통합 문서를 선택합니다.</p> </td> 
  </tr> 
  <tr> 
    <td role="rowheader" >[!UICONTROL 제한]</td>
   <td> <p>각 시나리오 실행 주기 동안 모듈이 반환할 최대 워크시트 수를 입력하거나 매핑합니다.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL 워크시트 행 나열]

이 작업 모듈은 지정된 워크시트의 행 목록을 검색합니다.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Connection]</p> </td> 
   <td> <p>연결 방법에 대한 지침은 [!DNL Office 365] 계정 대상 [!DNL Workfront Fusion]를 참조하십시오. <a href="../../workfront-fusion/scenarios/create-a-scenario.md#connect" class="MCXref xref">모듈의 앱 또는 웹 서비스를 [!DNL Workfront Fusion]</a> 기사 <a href="../../workfront-fusion/scenarios/create-a-scenario.md" class="MCXref xref">에서 시나리오 만들기 [!DNL Adobe Workfront Fusion]</a>.</p> </td> 
  </tr> 
  <tr>
    <td role="rowheader" >[!UICONTROL Workbook] </td>
   <td> <p>나열할 행이 포함된 워크시트를 포함하는 통합 문서를 선택합니다.</p> </td> 
  </tr> 
  <tr> 
    <td role="rowheader" >[!UICONTROL Worksheet] </td>
   <td> <p>나열할 행이 포함된 워크시트를 선택합니다.</p> </td> 
  </tr> 
  <tr> 
    <td role="rowheader" >[!UICONTROL 제한]</td>
   <td> <p>각 시나리오 실행 주기 동안 모듈이 반환할 최대 워크시트 행 수를 입력하거나 매핑합니다.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL 워크시트 추가]

이 작업 모듈은 선택한 통합 문서 내에 새 워크시트를 만듭니다.

<table style="table-layout:auto"> 
 <col data-mc-conditions=""> 
 <col data-mc-conditions=""> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Connection]</p> </td> 
   <td> <p>연결 방법에 대한 지침은 [!DNL Office 365] 계정 대상 [!DNL Workfront Fusion]를 참조하십시오. <a href="../../workfront-fusion/scenarios/create-a-scenario.md#connect" class="MCXref xref">모듈의 앱 또는 웹 서비스를 [!DNL Workfront Fusion]</a> 기사 <a href="../../workfront-fusion/scenarios/create-a-scenario.md" class="MCXref xref">에서 시나리오 만들기 [!DNL Adobe Workfront Fusion]</a>.</p> </td> 
  </tr> 
  <tr>
    <td role="rowheader" >[!UICONTROL Workbook] </td>
   <td> <p>워크시트를 추가할 통합 문서를 선택합니다.</p> </td> 
  </tr> 
  <tr> 
    <td role="rowheader" >[!UICONTROL Name] </td>
   <td> <p>새 워크시트의 이름을 입력하거나 매핑합니다.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL 워크시트 행 추가]

이 작업 모듈은 선택한 워크시트에 새 행을 추가합니다.

<table style="table-layout:auto"> 
 <col data-mc-conditions=""> 
 <col data-mc-conditions=""> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Connection]</p> </td> 
   <td> <p>연결 방법에 대한 지침은 [!DNL Office 365] 계정 대상 [!DNL Workfront Fusion]를 참조하십시오. <a href="../../workfront-fusion/scenarios/create-a-scenario.md#connect" class="MCXref xref">모듈의 앱 또는 웹 서비스를 [!DNL Workfront Fusion]</a> 기사 <a href="../../workfront-fusion/scenarios/create-a-scenario.md" class="MCXref xref">에서 시나리오 만들기 [!DNL Adobe Workfront Fusion]</a>.</p> </td> 
  </tr> 
  <tr> 
    <td role="rowheader" >[!UICONTROL Workbook] </td>
   <td> <p>행을 추가할 워크시트를 포함하는 통합 문서를 선택합니다.</p> </td> 
  </tr> 
  <tr> 
    <td role="rowheader" >[!UICONTROL Worksheet] </td>
   <td> <p>행을 추가할 워크시트를 선택합니다.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL 입력 중인 값 유형]</p> </td> 
   <td> <p>워크시트에 입력할 값 유형을 선택합니다. </p> 
    <ul> 
     <li> <p><strong>[!UICONTROL 공식]</strong> </p> <p> Excel에서는 지정된 표현식을 평가하려고 합니다. 수식의 함수 이름은 영어로 되어 있습니다. 예: <code>[!DNL =SUM(A1:A10)]</code></p> </li> 
     <li> <p><strong>[!UICONTROL 공식 로컬]</strong> </p> <p>Excel에서는 지정된 표현식을 평가하려고 합니다. 함수 이름은 Excel 애플리케이션의 언어로 표시됩니다. 예: <code>=SUM(A1, 1.5)</code> vs <code>=SUMME(A1; 1,5)</code></p> </li> 
     <li> <p><strong>[!UICONTROL Value]</strong> </p> <p>값이 평가되지 않습니다. </p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
    <td role="rowheader" >[!UICONTROL 행]</td>
    <td>각 열에 새 행에 열 값을 입력합니다.</td>
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL 워크시트 행 업데이트]

이 작업 모듈은 기존 워크시트 행을 갱신합니다.

<table style="table-layout:auto"> 
 <col data-mc-conditions=""> 
 <col data-mc-conditions=""> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Connection]</p> </td> 
   <td> <p>연결 방법에 대한 지침은 [!DNL Office 365] 계정 대상 [!DNL Workfront Fusion]를 참조하십시오. <a href="../../workfront-fusion/scenarios/create-a-scenario.md#connect" class="MCXref xref">모듈의 앱 또는 웹 서비스를 [!DNL Workfront Fusion]</a> 기사 <a href="../../workfront-fusion/scenarios/create-a-scenario.md" class="MCXref xref">에서 시나리오 만들기 [!DNL Adobe Workfront Fusion]</a>.</p> </td> 
  </tr> 
  <tr> 
    <td role="rowheader" >[!UICONTROL Workbook] </td>
   <td> <p>업데이트할 행이 포함된 워크시트를 포함하는 통합 문서를 선택합니다.</p> </td> 
  </tr> 
  <tr> 
    <td role="rowheader" >[!UICONTROL Worksheet] </td>
   <td> <p>갱신할 행이 포함된 워크시트를 선택합니다.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL 입력 중인 값 유형]</p> </td> 
   <td> <p>워크시트에 입력할 값 유형을 선택합니다. </p> 
    <ul> 
     <li> <p><strong>[!UICONTROL 공식]</strong> </p> <p> Excel에서는 지정된 표현식을 평가하려고 합니다. 수식의 함수 이름은 영어로 되어 있습니다. 예: <code>[!DNL =SUM(A1:A10)]</code></p> </li> 
     <li> <p><strong>[!UICONTROL 공식 로컬]</strong> </p> <p>Excel에서는 지정된 표현식을 평가하려고 합니다. 함수 이름은 Excel 애플리케이션의 언어로 표시됩니다. 예: <code>=SUM(A1, 1.5)</code> vs <code>=SUMME(A1; 1,5)</code></p> </li> 
     <li> <p><strong>[!UICONTROL Value]</strong> </p> <p>값이 평가되지 않습니다. </p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL 행 ID]</td> 
   <td>업데이트할 행 수를 선택합니다.</td> 
  </tr> 
  <tr> 
    <td role="rowheader" >[!UICONTROL 행]</td>
    <td>각 열에 새 행에 열 값을 입력합니다.</td>
   —&gt; 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL 워크시트 행 삭제]

이 작업 모듈은 워크시트에서 행을 삭제합니다.

<table style="table-layout:auto"> 
 <col data-mc-conditions=""> 
 <col data-mc-conditions=""> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Connection]</p> </td> 
   <td> <p>연결 방법에 대한 지침은 [!DNL Office 365] 계정 대상 [!DNL Workfront Fusion]를 참조하십시오. <a href="../../workfront-fusion/scenarios/create-a-scenario.md#connect" class="MCXref xref">모듈의 앱 또는 웹 서비스를 [!DNL Workfront Fusion]</a> 기사 <a href="../../workfront-fusion/scenarios/create-a-scenario.md" class="MCXref xref">에서 시나리오 만들기 [!DNL Adobe Workfront Fusion]</a>.</p> </td> 
  </tr> 
  <tr> 
    <td role="rowheader" >[!UICONTROL Workbook] </td>
   <td> <p>삭제할 행이 포함된 워크시트를 포함하는 통합 문서를 선택합니다.</p> </td> 
  </tr> 
  <tr> 
    <td role="rowheader" >[!UICONTROL Worksheet]</td>
   <td> <p> 삭제할 행이 포함된 워크시트를 선택합니다.</p> </td> 
  </tr> 
  <tr> 
    <td role="rowheader" >[!UICONTROL 행 ID]</td>
   <td>삭제할 행의 ID를 입력하거나 매핑합니다.</td> 
  </tr> 
 </tbody> 
</table>

### 테이블

* [[!UICONTROL 테이블 행 보기]](#watch-table-rows)
* [[!UICONTROL 테이블 나열]](#list-tables)
* [[!UICONTROL 테이블 행 나열]](#list-table-rows)
* [[!UICONTROL 테이블 가져오기]](#get-a-table)
* [[!UICONTROL 표 추가]](#add-a-table)
* [[!UICONTROL 표 행 추가]](#add-a-table-row)
* [[!UICONTROL 표 업데이트]](#update-a-table)
* [[!UICONTROL 표 삭제]](#delete-a-table)

#### [!UICONTROL 테이블 행 보기]

이 트리거는 새 행이 테이블에 추가되면 시나리오를 시작합니다.

>[!NOTE]
>
>여기 표는 통합 문서에 포함된 테이블 요소를 나타냅니다. 전체 표(통합 문서/시트)가 아닙니다.

![](assets/embedded-table-350x420.png)

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Connection]</p> </td> 
   <td> <p>연결 방법에 대한 지침은 [!DNL Office 365] 계정 대상 [!DNL Workfront Fusion]를 참조하십시오. <a href="../../workfront-fusion/scenarios/create-a-scenario.md#connect" class="MCXref xref">모듈의 앱 또는 웹 서비스를 [!DNL Workfront Fusion]</a> 기사 <a href="../../workfront-fusion/scenarios/create-a-scenario.md" class="MCXref xref">에서 시나리오 만들기 [!DNL Adobe Workfront Fusion]</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Workbook]</p> </td> 
   <td> <p>보려는 테이블이 포함된 통합 문서를 선택합니다.</p> </td> 
  </tr> 
  <tr> 
    <td role="rowheader" >[!UICONTROL Worksheet] </td>
   <td> <p> 보려는 테이블이 포함된 워크시트를 선택합니다.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL 테이블]</p> </td> 
   <td> <p>보려는 테이블을 선택합니다.</p> </td> 
  </tr> 
  <tr> 
    <td role="rowheader" >[!UICONTROL 제한]</td>
   <td> <p>각 시나리오 실행 주기 동안 모듈이 반환할 최대 행 수를 입력하거나 매핑합니다.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL 테이블 나열]

이 검색 모듈은 모든 테이블 개체 목록을 검색합니다.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Connection]</p> </td> 
   <td> <p>연결 방법에 대한 지침은 [!DNL Office 365] 계정 대상 [!DNL Workfront Fusion]를 참조하십시오. <a href="../../workfront-fusion/scenarios/create-a-scenario.md#connect" class="MCXref xref">모듈의 앱 또는 웹 서비스를 [!DNL Workfront Fusion]</a> 기사 <a href="../../workfront-fusion/scenarios/create-a-scenario.md" class="MCXref xref">에서 시나리오 만들기 [!DNL Adobe Workfront Fusion]</a>.</p> </td> 
  </tr> 
  <tr>
    <td role="rowheader" >[!UICONTROL Workbook] </td>
   <td> <p>나열할 테이블이 포함된 통합 문서를 선택합니다.</p> </td> 
  </tr> 
  <tr> 
    <td role="rowheader" >[!UICONTROL Worksheet] </td>
   <td> <p>나열할 테이블이 포함된 워크시트를 선택합니다</p> </td> 
  </tr> 
  <tr> 
    <td role="rowheader" >[!UICONTROL 제한]</td>
   <td> <p>각 시나리오 실행 주기 동안 모듈이 반환할 최대 테이블 수를 입력하거나 매핑합니다.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL 테이블 행 나열]

이 검색 모듈은 통합 문서에 있는 모든 테이블 행 목록을 검색합니다.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Connection]</p> </td> 
   <td> <p>연결 방법에 대한 지침은 [!DNL Office 365] 계정 대상 [!DNL Workfront Fusion]를 참조하십시오. <a href="../../workfront-fusion/scenarios/create-a-scenario.md#connect" class="MCXref xref">모듈의 앱 또는 웹 서비스를 [!DNL Workfront Fusion]</a> 기사 <a href="../../workfront-fusion/scenarios/create-a-scenario.md" class="MCXref xref">에서 시나리오 만들기 [!DNL Adobe Workfront Fusion]</a>.</p> </td> 
  </tr> 
  <tr> 
    <td role="rowheader" >[!UICONTROL Workbook] </td>
   <td> <p>나열할 행이 포함된 표를 포함하는 통합 문서를 선택합니다.</p> </td> 
  </tr> 
  <tr> 
    <td role="rowheader" >[!UICONTROL Worksheet] </td>
   <td> <p>나열할 행이 포함된 테이블을 포함하는 워크시트를 선택합니다</p> </td> 
  </tr> 
  <tr> 
    <td role="rowheader" >[!UICONTROL 테이블] </td>
   <td> <p>나열할 행이 포함된 테이블을 선택합니다.</p> </td> 
  </tr> 
  <tr> 
    <td role="rowheader" >[!UICONTROL 제한]</td>
   <td> <p>각 시나리오 실행 주기 동안 모듈이 반환할 최대 테이블 행 수를 입력하거나 매핑합니다.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL 테이블 가져오기]

이 작업 모듈은 지정된 테이블의 메타데이터를 검색합니다.

<table style="table-layout:auto"> 
 <col data-mc-conditions=""> 
 <col data-mc-conditions=""> 
 <tbody> 
  <tr> 
   <td role="rowheader"> 
     <p >[!UICONTROL Connection]</p>
   </td> 
   <td> 
     <p>Office 365 계정 연결에 대한 지침은 [!DNL Workfront Fusion]를 참조하십시오. <a href="../../workfront-fusion/scenarios/create-a-scenario.md#connect" class="MCXref xref">모듈의 앱 또는 웹 서비스를 [!DNL Workfront Fusion]</a> 기사 <a href="../../workfront-fusion/scenarios/create-a-scenario.md" class="MCXref xref">에서 시나리오 만들기 [!DNL Adobe Workfront Fusion]</a>.</p>
    --&gt; </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL 테이블 가져오기]</td> 
   <td> <p>검색할 테이블을 식별할 방법을 선택합니다.</p> 
    <ul> 
     <li> <p><strong>[!UICONTROL 수동으로 Enter]</strong> </p> <p>[!UICONTROL 통합 문서 ID] 필드에서 검색할 테이블이 포함된 통합 문서의 ID를 입력하거나 매핑합니다.</p> <p>[!UICONTROL 테이블 이름] 필드에 검색할 테이블의 이름을 입력하거나 매핑합니다.</p> </li> 
     <li> <p><strong>[!UICONTROL 목록에서 선택]</strong> </p> <p>검색할 테이블이 포함된 통합 문서와 워크시트를 선택한 다음 테이블을 선택합니다.</p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL 표 추가]

이 작업 모듈은 Excel 워크시트 내에 테이블 요소를 만듭니다.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Connection]</p> </td> 
   <td> <p>연결 방법에 대한 지침은 [!DNL Office 365] 계정 대상 [!DNL Workfront Fusion]를 참조하십시오. <a href="../../workfront-fusion/scenarios/create-a-scenario.md#connect" class="MCXref xref">모듈의 앱 또는 웹 서비스를 [!DNL Workfront Fusion]</a> 기사 <a href="../../workfront-fusion/scenarios/create-a-scenario.md" class="MCXref xref">에서 시나리오 만들기 [!DNL Adobe Workfront Fusion]</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Workbook] </td> 
   <td> <p>테이블을 추가할 워크시트가 들어 있는 통합 문서를 선택합니다.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Worksheet] </td> 
   <td> <p>테이블을 추가할 워크시트를 선택합니다.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL에 헤더 있음]</td> 
   <td> <p>첫 번째 행을 테이블 헤더로 정의하려면 이 옵션을 활성화합니다.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Address]</p> </td> 
   <td> <p>왼쪽 상단과 오른쪽 하단의 셀을 표시하여 표의 크기를 설정합니다. 예: <code>A1:C10</code> 3개의 열과 10개의 행이 있는 테이블을 만듭니다.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL 표 행 추가]

이 작업 모듈은 기존 테이블을 수정합니다.

<table style="table-layout:auto"> 
 <col data-mc-conditions=""> 
 <col data-mc-conditions=""> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Connection]</p> </td> 
   <td> <p>연결 방법에 대한 지침은 [!DNL Office 365] 계정 대상 [!DNL Workfront Fusion]를 참조하십시오. <a href="../../workfront-fusion/scenarios/create-a-scenario.md#connect" class="MCXref xref">모듈의 앱 또는 웹 서비스를 [!DNL Workfront Fusion]</a> 기사 <a href="../../workfront-fusion/scenarios/create-a-scenario.md" class="MCXref xref">에서 시나리오 만들기 [!DNL Adobe Workfront Fusion]</a>.</p> </td> 
  </tr> 
  <tr> 
    <td role="rowheader" >[!UICONTROL Workbook] </td>
   <td> <p>행을 추가할 표를 포함하는 통합 문서를 선택합니다.</p> </td> 
  </tr> 
  <tr> 
    <td role="rowheader" >[!UICONTROL Worksheet] </td>
   <td> <p>행을 추가할 테이블이 포함된 워크시트를 선택합니다.</p> </td> 
  </tr> 
  <tr> 
    <td role="rowheader" >[!UICONTROL 테이블]</td>
   <td>행을 추가할 테이블을 선택합니다.</td> 
  </tr> 
  <tr>
    <td role="rowheader" >[!UICONTROL 행]</td>
    <td>각 열에 새 행에 열 값을 입력합니다.</td>
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL 행 ID]</p> </td> 
   <td> <p>테이블의 특정 위치에 행을 추가하려면 행 번호를 입력하거나 매핑합니다. 모듈은 이 행 뒤에 새 행을 삽입합니다.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL 표 업데이트]

이 작업 모듈은 기존 테이블을 업데이트합니다.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Connection]</p> </td> 
   <td> <p>연결 방법에 대한 지침은 [!DNL Office 365] 계정 대상 [!DNL Workfront Fusion]를 참조하십시오. <a href="../../workfront-fusion/scenarios/create-a-scenario.md#connect" class="MCXref xref">모듈의 앱 또는 웹 서비스를 [!DNL Workfront Fusion]</a> 기사 <a href="../../workfront-fusion/scenarios/create-a-scenario.md" class="MCXref xref">에서 시나리오 만들기 [!DNL Adobe Workfront Fusion]</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL 테이블 업데이트]</td> 
   <td> <p>업데이트할 테이블을 식별할 방법을 선택합니다.</p> 
    <ul> 
     <li> <p><strong>수동으로 입력</strong> </p> <p>[!UICONTROL 통합 문서 ID] 필드에서 업데이트할 테이블이 포함된 통합 문서의 ID를 입력하거나 매핑합니다.</p> <p>[!UICONTROL 테이블 이름] 필드에 업데이트할 테이블의 이름을 입력하거나 매핑합니다.</p> </li> 
     <li> <p><strong>[!UICONTROL 목록에서 선택]</strong> </p> <p>업데이트할 테이블이 포함된 통합 문서와 워크시트를 선택한 다음 테이블을 선택합니다.</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL 테이블] </td> 
   <td> <p>업데이트할 테이블을 선택합니다.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Name]</td> 
   <td> <p>테이블의 이름을 변경하려면 테이블의 새 이름을 입력하거나 매핑합니다.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL 머리글 표시]</td> 
   <td> <p>업데이트된 테이블의 헤더를 표시하려면 이 옵션을 활성화합니다.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL 합계 표시]</td> 
   <td>테이블의 합계 값을 표시하려면 이 옵션을 활성화합니다.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Style]</td> 
   <td>새 표의 스타일을 선택합니다.</td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL 표 삭제]

이 작업 모듈은 [!DNL Excel] 워크시트.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Connection]</p> </td> 
   <td> <p>연결 방법에 대한 지침은 [!DNL Office 365] 계정 대상 [!DNL Workfront Fusion]를 참조하십시오. <a href="../../workfront-fusion/scenarios/create-a-scenario.md#connect" class="MCXref xref">모듈의 앱 또는 웹 서비스를 [!DNL Workfront Fusion]</a> 기사 <a href="../../workfront-fusion/scenarios/create-a-scenario.md" class="MCXref xref">에서 시나리오 만들기 [!DNL Adobe Workfront Fusion]</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL 테이블 가져오기]</td> 
   <td> <p>삭제할 테이블을 식별하는 방법을 선택합니다.</p> 
    <ul> 
     <li> <p><strong>[!UICONTROL 수동으로 Enter]</strong> </p> <p>[!UICONTROL 통합 문서 ID] 필드에서 삭제할 테이블이 포함된 통합 문서의 ID를 입력하거나 매핑합니다.</p> <p>[!UICONTROL 테이블 이름] 필드에 삭제할 테이블의 이름을 입력하거나 매핑합니다.</p> </li> 
     <li> <p><strong>[!UICONTROL 목록에서 선택]</strong> </p> <p>삭제할 테이블이 포함된 통합 문서와 워크시트를 선택한 다음 테이블을 선택합니다.</p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

### 기타

* [[!UICONTROL 데이터 검색]](#retrieve-data)
* [[!UICONTROL API 호출 만들기]](#make-an-api-call)

#### [!UICONTROL 데이터 검색]

이 작업은 정의된 워크시트 범위에서 데이터를 검색하고 각 행에 대한 번들을 반환합니다.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Connection]</p> </td> 
   <td> <p>연결 방법에 대한 지침은 [!DNL Office 365] 계정 대상 [!DNL Workfront Fusion]를 참조하십시오. <a href="../../workfront-fusion/scenarios/create-a-scenario.md#connect" class="MCXref xref">모듈의 앱 또는 웹 서비스를 [!DNL Workfront Fusion]</a> 기사 <a href="../../workfront-fusion/scenarios/create-a-scenario.md" class="MCXref xref">에서 시나리오 만들기 [!DNL Adobe Workfront Fusion]</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Workbook] </td> 
   <td> <p>검색할 데이터가 포함된 통합 문서를 선택합니다.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Worksheet] </td> 
   <td> <p>검색할 데이터가 포함된 워크시트를 선택합니다.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL 범위] </td> 
   <td> <p>왼쪽 상단과 오른쪽 하단의 셀을 표시하여 데이터를 검색할 시트의 영역을 지정합니다. 예: <code>A1:D10</code></p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL API 호출 만들기]

이 작업 모듈을 사용하여 사용자 지정 API 호출을 수행할 수 있습니다.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Connection]</p> </td> 
   <td> <p>연결 방법에 대한 지침은 [!DNL Office 365] 계정 대상 [!DNL Workfront Fusion]를 참조하십시오. <a href="../../workfront-fusion/scenarios/create-a-scenario.md#connect" class="MCXref xref">모듈의 앱 또는 웹 서비스를 [!DNL Workfront Fusion]</a> 기사 <a href="../../workfront-fusion/scenarios/create-a-scenario.md" class="MCXref xref">에서 시나리오 만들기 [!DNL Adobe Workfront Fusion]</a>.</p> </td> 
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
   <td> <p>표준 JSON 개체 형태로 API 호출에 대한 본문 콘텐츠를 추가합니다.</p> <p>참고:   <p>다음과 같은 조건문을 사용하는 경우 <code>if</code> json에서 따옴표를 조건문 외부에 지정합니다.</p> 
     <div class="example" data-mc-autonum="<b>Example: </b>">  
      <p> <img src="assets/quotes-in-json-350x120.png" style="width: 350;height: 120;"> </p> 
     </div> </p> </td> 
  </tr> 
 </tbody> 
</table>
