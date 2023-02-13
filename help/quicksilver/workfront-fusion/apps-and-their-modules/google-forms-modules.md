---
content-type: reference
product-previous: workfront-fusion
product-area: workfront-integrations;documents
keywords: 커넥터
navigation-topic: apps-and-their-modules
title: Google Forms 모듈
description: 다음 [!DNL Adobe Workfront Fusion Google Forms] 모듈을 사용하면 Google Forms에서 응답을 모니터링, 선택, 추가, 업데이트 또는 삭제할 수 있습니다.
author: Becky
feature: Workfront Fusion
exl-id: 45c86879-bc4e-4134-b63c-02410b9de43b
source-git-commit: 885d93dd4383945538e977fd3edbfd55bda88b70
workflow-type: tm+mt
source-wordcount: '1382'
ht-degree: 0%

---

# [!DNL Google Forms] 모듈

다음 [!DNL Adobe Workfront Fusion] [!DNL Google Forms] 모듈을 사용하면 사용자의 [!DNL Google Forms].

를 사용하려면 [!DNL Google Docs] with [!DNL Adobe Workfront Fusion]를 채울 때는 [!DNL Google] 계정이 필요합니다. 만약 [!DNL Google] 아직 계정을 만들 수 있습니다. [!DNL Google] 계정 도움말 페이지입니다.

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

를 사용하려면 [!DNL Google Forms] 모듈이면 반드시 [!DNL Google] 계정이 필요합니다.

## 양식에서 스프레드시트 생성

양식 응답을 사용하려면 응답의 스프레드시트를 만들어야 합니다.

1. 양식을 엽니다.
1. 로 이동합니다. **[!UICONTROL 응답]** 탭.
1. 을(를) 클릭합니다. **[!UICONTROL 스프레드시트 만들기]** 아이콘 ![](assets/spreadsheet-icon.png).

1. 새 스프레드시트를 생성할지 기존 스프레드시트를 생성할지를 선택합니다
1. Click **[!UICONTROL Create]**.

## [!DNL Google Forms] 모듈 및 해당 필드

구성 시 [!DNL Google Forms] 모듈, [!DNL Workfront Fusion] 아래 나열된 필드를 표시합니다. 이와 함께 추가 [!DNL Google Forms] 앱이나 서비스에서 액세스 수준과 같은 요소에 따라 필드가 표시될 수 있습니다. 모듈에서 굵게 표시된 제목은 필수 필드를 나타냅니다.

필드 또는 함수 위에 맵 단추가 표시되면 이 단추를 사용하여 해당 필드에 대한 변수와 함수를 설정할 수 있습니다. 자세한 내용은 [의 한 모듈에서 다른 모듈로 정보 매핑 [!DNL Adobe Workfront Fusion]](../../workfront-fusion/mapping/map-information-between-modules.md).

![](assets/map-toggle-350x74.png)

* [Triggers](#triggers)
* [액션](#actions)
* [검색 결과](#searches)

### Triggers

#### [!UICONTROL 응답 보기]

양식에 새로운 응답이 있는지 확인합니다.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td> 
   <td> <p>연결 방법에 대한 지침은 [!DNL Google] 계정 대상 [!DNL Workfront Fusion]를 참조하십시오. <a href="../../workfront-fusion/scenarios/create-a-scenario.md#connect" class="MCXref xref">모듈의 앱 또는 웹 서비스를 [!DNL Workfront Fusion]</a> 기사 <a href="../../workfront-fusion/scenarios/create-a-scenario.md" class="MCXref xref">에서 시나리오 만들기 [!DNL Adobe Workfront Fusion]</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Spreadsheet]</td> 
   <td> <p>새로운 응답을 보려는 양식의 응답이 포함된 스프레드시트를 선택합니다.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Sheet]</td> 
   <td> <p> 양식 응답이 포함된 시트를 선택합니다.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Row with headers]</td> 
   <td>표의 머리글 행을 지정합니다. 기본 행은 다음과 같습니다 <code>A1:Z1</code>.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Value Render Option]</td> 
   <td> <p>출력에서 값을 렌더링할 방법을 지정합니다.</p> 
    <ul> 
     <li> <p><strong>[!UICONTROL 형식이 지정된 값]</strong> </p> <p>값은 셀의 서식에 따라 응답에서 계산되고 형식이 지정됩니다. 서식은 요청하는 사용자의 로케일이 아니라 스프레드시트의 로케일을 기반으로 합니다. 예를 들어 <code>A1</code> is <code>1. 23</code> 및 <code>A2 </code>is <code>=A1</code> 형식으로 된 다음 <code>A2</code> 반환 <code>$1. 23</code> .</p> </li> 
     <li> <p><strong>[!UICONTROL 형식이 지정되지 않은 값]</strong> </p> <p>값은 계산되지만 답장에서 형식화되지 않습니다. 예를 들어 <code>A1</code> is <code>1. 23</code> 및 <code>A2 </code>is <code>=A1</code> 형식으로 된 다음 <code>A2</code> 숫자 반환 <code>1. 23</code> .</p> </li> 
     <li> <p><strong>[!UICONTROL 공식]</strong> </p> <p>값은 계산되지 않습니다. 응답에는 수식이 포함됩니다. 예를 들어 <code>A1</code> is <code>1. 23</code> 및 <code>A2 </code>is <code>=A1</code> 형식으로 된 다음 <code>A2</code> 반환 <code>=A1</code>.</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL 날짜 및 시간 렌더링 옵션]</td> 
   <td>출력에 날짜, 시간 및 기간을 나타낼 방법을 선택합니다. [!UICONTROL Value Render Option]이 [!UICONTROL Formatted Value]로 설정된 경우 이 필드는 무시됩니다.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL 제한]</td> 
   <td> <p> 최대 응답 수 설정 [!DNL Workfront Fusion] 은 한 번의 사이클로 작동합니다.</p> </td> 
  </tr> 
 </tbody> 
</table>

### 액션

* [[!UICONTROL 응답 추가]](#add-a-response)
* [[!UICONTROL 응답 업데이트]](#update-a-response)
* [[!UICONTROL 응답 삭제]](#delete-a-response)

#### [!UICONTROL 응답 추가]

이 모듈은 양식의 스프레드시트 하단에 새 응답을 추가합니다.

이 모듈을 구성할 때 다음 필드가 표시됩니다.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td> 
   <td> <p>연결 방법에 대한 지침은 [!DNL Google] 계정 대상 [!DNL Workfront Fusion]를 참조하십시오. <a href="../../workfront-fusion/scenarios/create-a-scenario.md#connect" class="MCXref xref">모듈의 앱 또는 웹 서비스를 [!DNL Workfront Fusion]</a> 기사 <a href="../../workfront-fusion/scenarios/create-a-scenario.md" class="MCXref xref">에서 시나리오 만들기 [!DNL Adobe Workfront Fusion]</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Spreadsheet]</td> 
   <td> <p>응답을 추가할 시트가 포함된 스프레드시트를 선택합니다.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Sheet]</td> 
   <td> <p> 양식 응답이 포함된 시트를 선택합니다.</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader"> <p>[!UICONTROL Values]</p> </td> 
   <td> <p>시트 열에 원하는 값을 입력합니다.</p> <p>올바른 형식의 [!UICONTROL 타임스탬프] 열에 대해 다음 값을 사용하십시오.</p><pre>formatDate(now;DD/MM/YYYY HH:mm;UTC)</pre> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader">[!UICONTROL 값 입력 옵션]</td> 
   <td> 
    <ul> 
     <li> <p><strong>[!UICONTROL Raw]</strong> </p> <p> 사용자가 입력하는 값은 구문 분석되지 않고 있는 그대로 저장됩니다. </p> </li> 
     <li> <p><strong>[!UICONTROL 사용자가 입력됨]</strong></p> <p>값은 사용자가 UI에 입력한 것처럼 구문 분석됩니다. 숫자는 숫자로 유지되지만, 문자열은 를 통해 셀에 텍스트를 입력할 때 적용되는 것과 동일한 규칙을 따라 숫자, 날짜 또는 기타 형식으로 변환할 수 있습니다 [!DNL Google Sheets] UI.</p> </li> 
    </ul> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader">[!UICONTROL 데이터 삽입 옵션]</td> 
   <td> <p>새 데이터를 입력할 때 기존 데이터가 변경되는 방법을 지정합니다. </p> 
    <ul> 
     <li> <p><strong>[!UICONTROL Overwrite]</strong> </p> <p>새 데이터는 쓰기 영역의 기존 데이터를 덮어씁니다. 시트 끝에 데이터를 추가하면 새 행이나 열이 삽입되므로 데이터를 작성할 수 있습니다.</p> </li> 
     <li> <p><strong>[!UICONTROL 행 삽입]</strong></p> <p>새 데이터에 대한 행이 삽입됩니다.</p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL 응답 업데이트]

이 모듈은 선택한 응답을 업데이트합니다.

이 모듈을 구성할 때 다음 필드가 표시됩니다.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td> 
   <td> <p>연결 방법에 대한 지침은 [!DNL Google] 계정 대상 [!DNL Workfront Fusion]를 참조하십시오. <a href="../../workfront-fusion/scenarios/create-a-scenario.md#connect" class="MCXref xref">모듈의 앱 또는 웹 서비스를 [!DNL Workfront Fusion]</a> 기사 <a href="../../workfront-fusion/scenarios/create-a-scenario.md" class="MCXref xref">에서 시나리오 만들기 [!DNL Adobe Workfront Fusion]</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Spreadsheet]</td> 
   <td> <p>응답을 업데이트할 시트가 포함된 스프레드시트를 선택합니다.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Sheet]</td> 
   <td> <p> 양식 응답이 포함된 시트를 선택합니다.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL 행 번호]</p> </td> 
   <td> <p>갱신할 행 번호를 입력하거나 매핑합니다.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Values]</p> </td> 
   <td> <p>원하는 열에 새 값을 입력합니다.</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader">[!UICONTROL 값 입력 옵션]</td> 
   <td> 
    <ul> 
     <li> <p><strong>[!UICONTROL Raw]</strong> </p> <p> 사용자가 입력하는 값은 구문 분석되지 않고 있는 그대로 저장됩니다. </p> </li> 
     <li> <p><strong>[!UICONTROL 사용자가 입력됨]</strong></p> <p>값은 사용자가 UI에 입력한 것처럼 구문 분석됩니다. 숫자는 숫자로 유지되지만, 문자열은 를 통해 셀에 텍스트를 입력할 때 적용되는 것과 동일한 규칙을 따라 숫자, 날짜 또는 기타 형식으로 변환할 수 있습니다 [!DNL Google Sheets] UI.</p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL 응답 삭제]

이 모듈은 선택한 응답을 삭제합니다.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td> 
   <td> <p>연결 방법에 대한 지침은 [!DNL Google] 계정 대상 [!DNL Workfront Fusion]를 참조하십시오. <a href="../../workfront-fusion/scenarios/create-a-scenario.md#connect" class="MCXref xref">모듈의 앱 또는 웹 서비스를 [!DNL Workfront Fusion]</a> 기사 <a href="../../workfront-fusion/scenarios/create-a-scenario.md" class="MCXref xref">에서 시나리오 만들기 [!DNL Adobe Workfront Fusion]</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Spreadsheet]</td> 
   <td> <p>응답을 삭제할 시트가 포함된 스프레드시트를 선택합니다.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Sheet]</td> 
   <td> <p> 양식 응답이 포함된 시트를 선택합니다.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL 행 번호]</p> </td> 
   <td> <p>삭제할 행 번호를 입력하거나 매핑합니다.</p> </td> 
  </tr> 
 </tbody> 
</table>

### 검색 결과

* [[!UICONTROL 응답 검색]](#search-responses)
* [[!UICONTROL 응답 검색(고급)])](#search-responses-advanced)

#### [!UICONTROL 응답 검색]

이 모듈은 지정된 기준과 일치하는 응답을 반환합니다.

<table style="table-layout:auto"> 
 <col data-mc-conditions=""> 
 <col data-mc-conditions=""> 
 <tbody> 
    <td>연결</td>
   <td> <p>연결 방법에 대한 지침은 [!DNL Google] 계정 대상 [!DNL Workfront Fusion]를 참조하십시오. <a href="../../workfront-fusion/scenarios/create-a-scenario.md#connect" class="MCXref xref">모듈의 앱 또는 웹 서비스를 [!DNL Workfront Fusion]</a> 기사 <a href="../../workfront-fusion/scenarios/create-a-scenario.md" class="MCXref xref">에서 시나리오 만들기 [!DNL Adobe Workfront Fusion]</a>.</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
    <td>[!UICONTROL Spreadsheet]</td>
   <td> <p>검색할 양식을 선택합니다.</p> </td> 
  </tr> 
  <tr data-mc-conditions="">
    <td>[!UICONTROL Sheet] </td>
   <td> <p>양식 응답이 포함된 시트를 선택합니다.</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
    <td>[!UICONTROL 열 범위]</td>
   <td> <p> 검색할 열 범위를 선택합니다.</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader">[!UICONTROL Filter]</td> 
   <td> <p>응답별로 검색할 필터를 정의합니다.</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
    <td>[!UICONTROL 정렬 순서] </td>
   <td> <p>반환된 응답을 오름차순 또는 내림차순으로 정렬할지 여부를 선택합니다.</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
    <td>[!UICONTROL Order By]</td>
   <td> <p> 반환된 응답을 주문하려는 열을 선택합니다.</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader">[!UICONTROL Value Render Option]</td> 
   <td> <p>출력에서 값을 렌더링할 방법을 지정합니다.</p> 
    <ul> 
     <li> <p><strong>[!UICONTROL 형식이 지정된 값]</strong></p> <p>값은 셀의 서식에 따라 응답에서 계산되고 형식이 지정됩니다. 서식은 요청하는 사용자의 로케일이 아니라 스프레드시트의 로케일을 기반으로 합니다. 예를 들어 <code>A1</code> is <code>1. 23</code> 및 <code>A2 </code>is <code>=A1</code> 형식으로 된 다음 <code>A2</code> 반환 <code>$1. 23</code> .</p> </li> 
     <li> <p><strong>[!UICONTROL 형식이 지정되지 않은 값]</strong> </p> <p>값은 계산되지만 답장에서 형식화되지 않습니다. 예를 들어 <code>A1</code> is <code>1. 23</code> 및 <code>A2 </code>is <code>=A1</code> 형식으로 된 다음 <code>A2</code> 숫자 반환 <code>1. 23</code> .</p> </li> 
     <li> <p><strong>[!UICONTROL 공식]</strong> </p> <p>값은 계산되지 않습니다. 응답에는 수식이 포함됩니다. 예를 들어 <code>A1</code> is <code>1. 23</code> 및 <code>A2 </code>is <code>=A1</code> 형식으로 된 다음 <code>A2</code> 반환 <code>=A1</code>.</p> </li> 
    </ul> </td> 
  </tr> 
  <tr data-mc-conditions="">
    <td>[!UICONTROL 날짜 및 시간 렌더링 옵션]</td>
    <td>출력에 날짜, 시간 및 기간을 나타낼 방법을 선택합니다. [!UICONTROL Value Render] 옵션이 형식이 지정된 값으로 설정되어 있으면 이 필드가 무시됩니다. </td>
  </tr> 
  <tr>
    <td role="rowheader" data-mc-conditions="QuicksilverOrClassic.Draft mode">[!UICONTROL 반환된 최대 응답 수]</td>
   <td> <p> 최대 응답 수 설정 [!DNL Workfront Fusion] 한 주기 동안 를 반환합니다.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL 응답 검색(고급)]

이 모듈은 [[!DNL Google Charts Query Language]](https://developers.google.com/chart/interactive/docs/querylanguage). 이 모듈은 행 번호를 반환하지 않습니다.

<table style="table-layout:auto"> 
 <col data-mc-conditions=""> 
 <col data-mc-conditions=""> 
 <tbody> 
  <tr> 
    <td>[!UICONTROL Connection]</td>
   <td> <p>연결 방법에 대한 지침은 [!DNL Google] 계정 대상 [!DNL Workfront Fusion]를 참조하십시오. <a href="../../workfront-fusion/scenarios/create-a-scenario.md#connect" class="MCXref xref">모듈의 앱 또는 웹 서비스를 [!DNL Workfront Fusion]</a> 기사 <a href="../../workfront-fusion/scenarios/create-a-scenario.md" class="MCXref xref">에서 시나리오 만들기 [!DNL Adobe Workfront Fusion]</a>.</p> </td> 
  </tr> 
  <tr>
    <td>[!UICONTROL Spreadsheet]</td>
   <td> <p>검색할 시트가 포함된 스프레드시트를 선택합니다.</p> </td> 
  </tr> 
  <tr>
    <td>[!UICONTROL Sheet]</td>
   <td> <p> 양식 응답이 포함된 시트를 선택합니다.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Filter]</td> 
   <td> <p>을(를) 사용하여 검색 쿼리를 정의합니다. <a href="https://developers.google.com/chart/interactive/docs/querylanguage">[!DNL Google Charts Query Language]</a>.</p> <p>예: <code>select * where C = "John"</code> C 열이 "John"인 행의 모든 값을 검색합니다.</p> </td> 
  </tr> 
  <tr>
    <td>[!UICONTROL 반환된 최대 행 수]</td>
   <td> <p> 최대 응답 수 설정 [!DNL Workfront Fusion] 한 주기 동안 를 반환합니다.</p> </td> 
  </tr> 
 </tbody> 
</table>
