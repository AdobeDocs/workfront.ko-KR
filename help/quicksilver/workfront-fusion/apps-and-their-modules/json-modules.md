---
content-type: reference
product-previous: workfront-fusion
product-area: workfront-integrations
navigation-topic: apps-and-their-modules
title: JSON 모듈
description: Adobe Workfront Fusion JSON 앱은 Adobe Workfront Fusion이 데이터 콘텐츠로 더 이상 작동하거나 새 JSON 콘텐츠를 만들 수 있도록 JSON 형식으로 데이터를 처리하는 모듈을 제공합니다.
author: Becky
feature: Workfront Fusion
exl-id: 60540608-9d2e-4e10-9fb2-5388dda64784
source-git-commit: 0915dcce45b271ee18cdd8af5db4f0eb01f3cced
workflow-type: tm+mt
source-wordcount: '1205'
ht-degree: 0%

---

# [!UICONTROL JSON] 모듈

다음 [!DNL Adobe Workfront Fusion] [!UICONTROL JSON] 앱은 JSON 형식으로 데이터를 처리하는 모듈을 제공하므로 [!DNL Adobe Workfront Fusion] 는 데이터 콘텐츠로 추가로 작업하거나 새 JSON 콘텐츠를 만들 수 있습니다.

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
   <p>기존 라이선스 요구 사항: [!UICONTROL [!DNL Workfront Fusion] 작업 자동화 및 통합용], [!UICONTROL [!DNL Workfront Fusion] 작업 자동화용]</p>
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

## JSON 구문 분석

* [데이터 구조](#data-structure)
* [컬렉션과 배열 비교](#collection-vs-array)

### 데이터 구조

데이터 구조는 JSON 데이터가 구성되는 방법을 설명하고 개별 JSON 항목을 시나리오의 다른 모듈에 매핑할 수 있도록 합니다. 데이터 구조를 제공하지 않는 경우 모듈을 수동으로 실행하고 [!DNL Workfront Fusion] 은 제공된 JSON에서 구조를 빌드합니다.

1. 추가 [!UICONTROL JSON 구문 분석] 시나리오를 위한 모듈입니다.
1. 다음에서 **[!UICONTROL JSON 문자열]** 필드에 데이터 구조를 작성하려는 JSON을 입력합니다.
1. 다른 모듈을 [!UICONTROL JSON 구문 분석] 모듈이 아직 로드되지 않았습니다. 이유 [!DNL Workfront Fusion] 은 JSON 데이터의 구조를 아직 모르며 의 데이터를 매핑할 수 없습니다. [!UICONTROL JSON 구문 분석] 를 시나리오의 다른 모듈에 연결합니다.
1. 수동으로 시나리오를 실행합니다. 이렇게 하면 [!UICONTROL JSON 구문 분석] 제공한 JSON에서 JSON 구조를 식별하는 모듈입니다.
1. 이제 다음 모듈을 연결할 수 있습니다. 이제 JSON 구문 분석 모듈의 항목을 매핑에 사용할 수 있습니다.

자세한 내용은 [의 데이터 구조 [!UICONTROL Adobe Workfront Fusion]](../../workfront-fusion/modules/data-structures.md).

### 컬렉션과 배열 비교

JSON 문자열 필드에 컬렉션이 포함된 경우 `{ ... }`: 출력은 컬렉션의 항목을 포함하는 단일 번들입니다.

>[!INFO]
>
>**예:**
>
>```
>{
>       "name" : "Peter",
>
>    
>   "ID" : 1
>}
>```
>
>![](assets/json-collection.png)

JSON 문자열 필드에 배열이 포함된 경우 `[ ... ]`, 출력은 일련의 번들입니다. 각 번들에는 배열의 한 요소가 포함되어 있습니다.

>[!INFO]
>
>**예:**
>
>```
>[
>   {
>       "name" : "Peter",
>       "ID" : 1
>   },
>
>  
> {
>       "name" : "Mike",
>       "ID" : 2
>   }
>]
>```
>
>![](assets/json-array.png)

## [!UICONTROL JSON] 모듈 및 해당 필드

를 구성할 때 [!DNL JSON] 모듈, [!DNL Workfront Fusion] 아래 나열된 필드를 표시합니다. 이러한 필드와 함께 앱이나 서비스의 액세스 수준과 같은 요소에 따라 추가 JSON 필드가 표시될 수 있습니다. 모듈의 굵은 제목은 필수 필드를 나타냅니다.

필드나 함수 위에 맵 단추가 표시되면 이 단추를 사용하여 해당 필드에 대한 변수와 함수를 설정할 수 있습니다. 자세한 내용은 [의 한 모듈에서 다른 모듈로 정보 매핑 [!DNL Adobe Workfront Fusion]](../../workfront-fusion/mapping/map-information-between-modules.md).

![](assets/map-toggle-350x74.png)

* [JSON으로 집계](#aggregate-to-json)
* [JSON을 XML로 변환](#convert-json-to-xml)
* [JSON 구문 분석](#parse-json)
* [JSON 만들기](#create-json)
* [JSON 변환](#transform-json)

### [!UICONTROL JSON으로 집계]

이 집계 모듈은 이전 모듈의 출력을 JSON으로 집계합니다.

<table style="table-layout:auto"> 
 <col data-mc-conditions=""> 
 <col data-mc-conditions=""> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL 소스 모듈] </td> 
   <td> <p>JSON으로 집계할 데이터를 출력하는 모듈을 선택합니다.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL 데이터 구조]</td> 
   <td> <p>JSON을 만드는 데 사용할 데이터 구조를 선택합니다. 데이터 구조는 이 모듈에서 사용할 수 있는 다른 필드를 결정합니다. 자세한 내용은 <a href="#data-structure" class="MCXref xref">데이터 구조</a> 이 문서에서.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL 들여쓰기]</td> 
   <td> <p> 탭을 사용하여 JSON을 들여쓰는지, 공백 2개를 사용할지 또는 공백 4개를 사용할지 선택합니다.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Group by]</td> 
   <td>집계된 출력을 그룹화할 표현식을 정의합니다. 이 표현식은 하나 이상의 매핑된 항목을 포함할 수 있습니다. 그런 다음 집계된 데이터는 이 표현식의 값을 사용하여 그룹으로 구분됩니다. 각 그룹은 키(평가된 표현식)와 값(집계된 텍스트)을 사용하여 별도의 번들로 출력합니다. 키는 후속 모듈에서 필터로 사용할 수 있습니다.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL 빈 집계 후 처리 중지]</td> 
   <td>결과가 없을 때 시나리오를 중지하려면 이 옵션을 활성화하십시오.</td> 
  </tr> 
 </tbody> 
</table>

### [!UICONTROL JSON을 XML로 변환]

이 작업 모듈은 JSON 문자열을 XML로 변환합니다.

<table style="table-layout:auto"> 
 <col data-mc-conditions=""> 
 <col data-mc-conditions=""> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL JSON string] </td> 
   <td> <p>XML로 변환할 JSON을 입력하거나 매핑합니다.</p> </td> 
  </tr> 
 </tbody> 
</table>

### [!UICONTROL JSON 구문 분석]

이 작업 모듈은 JSON 문자열을 JSON 문자열 내의 데이터에 액세스할 수 있는 데이터 구조로 구문 분석합니다.

<table style="table-layout:auto"> 
 <col data-mc-conditions=""> 
 <col data-mc-conditions=""> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL 데이터 구조]</td> 
   <td> <p>JSON을 만드는 데 사용할 데이터 구조를 선택합니다. 자세한 내용은 <a href="#data-structure" class="MCXref xref">데이터 구조</a> 이 문서에서.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL JSON string] </td> 
   <td> <p>구문 분석할 JSON을 입력하거나 매핑합니다.</p> </td> 
  </tr> 
 </tbody> 
</table>

### [!UICONTROL JSON 만들기]

이 작업 모듈은 데이터 구조에서 JSON을 생성합니다.

<table style="table-layout:auto"> 
 <col data-mc-conditions=""> 
 <col data-mc-conditions=""> 
 <tbody> 
  <tr> 
   <td role="rowheader">데이터 구조</td> 
   <td> <p>JSON을 만드는 데 사용할 데이터 구조를 선택합니다. 자세한 내용은 <a href="#data-structure" class="MCXref xref">데이터 구조</a> 이 문서에서.</p> </td> 
  </tr> 
 </tbody> 
</table>

### [!UICONTROL JSON 변환]

이 작업 모듈은 개체를 json 문자열로 변환합니다.

<table style="table-layout:auto"> 
 <col data-mc-conditions=""> 
 <col data-mc-conditions=""> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL 개체]</td> 
   <td> <p>JSON으로 변형할 개체를 입력하거나 매핑합니다.</p> </td> 
  </tr> 
 </tbody> 
</table>

## 데이터 레코드를 JSON으로 변환

>[!INFO]
>
>**예:** 다음 예제에서는 데이터 레코드를 변환하는 방법을 보여 줍니다 [!DNL Google Sheets] JSON 형식으로 변환:
>
>1. 배치 [!DNL Google Sheets] > [!UICONTROL 행 선택] 데이터를 가져오기 위한 시나리오의 모듈입니다. 에서 행을 검색하도록 모듈 설정 [!DNL Google] 스프레드시트입니다. 설정&#x200B;:**[!UICONTROL 반환되는 최대 행 수]** 테스트 목적으로 1보다 큰 작은 숫자(예: 3개)로 실행 [!DNL Google Sheets] 모듈을 마우스 오른쪽 단추로 클릭하고 &quot;**[!UICONTROL 이 모듈만 실행]**.&quot; 모듈의 출력을 확인합니다.
>
1. 연결 [!UICONTROL 배열 집계] 다음 뒤에 있는 모듈 [!DNL Google Sheets] 모듈. 모듈의 설정에서 다음을 선택합니다. [!DNL Google Sheets] 의 모듈 **[!UICONTROL 소스 노드]** 필드. 다른 필드는 현재 상태로 두십시오.
>
1. 연결 [!UICONTROL JSON] > [!UICONTROL JSON 만들기] 다음 뒤에 있는 모듈 [!UICONTROL 배열 집계] 모듈. 모듈의 설정에는 JSON 형식을 설명하는 데이터 구조가 필요합니다. 클릭 **[!UICONTROL 추가]** 를 클릭하여 데이터 구조 설정을 엽니다. 이 데이터 구조를 만드는 가장 쉬운 방법은 JSON 샘플에서 자동으로 생성하는 것입니다. 클릭 **[!UICONTROL 생성기]** 및 JSON 샘플을 **[!UICONTROL 샘플 데이터]** 필드:
>
**예:**
>   
>```
>{
>
>"books": [
>
>{
>
>"id": "ID",
>
>"title": "Title",
>
>"author": "Author"
>
>}
>
>]
>
>}
>```
>
1. **[!UICONTROL 저장]**&#x200B;을 클릭합니다. 다음 [!UICONTROL 사양] 이제 데이터 구조의 필드에 생성된 구조가 포함됩니다.
1. 데이터 구조의 이름을 보다 구체적으로 변경하고 **[!UICONTROL 저장]**. 루트 배열 속성에 해당하는 필드는 JSON 모듈의 설정에서 매핑 가능한 필드로 표시됩니다.
>
1. 다음을 클릭합니다. **[!UICONTROL 맵]** 필드 옆에 있는 버튼을 클릭하고 `Array[]` 배열 집계 출력의 항목입니다.
>
1. 클릭 **[!UICONTROL 확인]** 닫으려면 다음을 수행하십시오. [!UICONTROL JSON] 모듈의 설정입니다.
>
1. 의 설정을 엽니다. [!UICONTROL 배열 집계] 모듈. 변경 **[!UICONTROL Target 구조]** 출처: [!UICONTROL 사용자 정의] (으)로 [!UICONTROL JSON] 루트 배열 특성에 해당하는 모듈의 필드. 에서 항목 매핑 [!DNL Google Sheets] 모듈을 적절한 필드에 연결합니다.
>
1. 클릭 **[!UICONTROL 확인]** 닫으려면 다음을 수행하십시오. [!UICONTROL 배열 집계] 모듈의 설정입니다.
>
1. 시나리오를 실행합니다.
>
다음 [!UICONTROL JSON] 모듈은 올바른 JSON 형식을 출력합니다.
>
1. 의 설정을 엽니다. [!DNL Google Sheets] 모듈 및 증가 [!UICONTROL 반환되는 최대 행 수] 모든 데이터를 처리할 스프레드시트의 행 수보다 큰 수입니다.

## 문제 해결

### 에서 데이터를 매핑할 수 없음 [!UICONTROL JSON 구문 분석] 모듈

JSON 콘텐츠가 [!UICONTROL JSON 구문 분석] 및 가 데이터 구조가 올바르게 정의되었는지 확인합니다. 자세한 내용은 [데이터 레코드를 JSON으로 변환](#transforming-data-records-to-json) 이 문서에서.

### JSON에서 조건문을 사용할 때 모듈이 실패합니다.

다음과 같은 조건문을 사용할 때 `if` json에서 따옴표를 조건문 외부에 넣습니다.

>[!INFO]
>
**예:**
>
![](assets/quotes-in-json-350x120.png)
