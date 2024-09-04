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
source-git-commit: 558ca6a1935d33e2c3c7ea3f4c1bd90a493ef8ff
workflow-type: tm+mt
source-wordcount: '1214'
ht-degree: 0%

---

# [!UICONTROL JSON] 모듈

[!DNL Adobe Workfront Fusion] [!UICONTROL JSON] 앱은 [!DNL Adobe Workfront Fusion]이(가) 데이터 콘텐츠로 더 작업하거나 새 JSON 콘텐츠를 만들 수 있도록 JSON 형식으로 데이터를 처리하는 모듈을 제공합니다.

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
   <p>레거시 라이선스 요구 사항: 작업 자동화 및 통합의 경우 [!UICONTROL [!DNL Workfront Fusion], 작업 자동화의 경우 [!UICONTROL [!DNL Workfront Fusion]]</p>
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

## JSON 구문 분석

* [데이터 구조](#data-structure)
* [컬렉션과 배열 비교](#collection-vs-array)

### 데이터 구조

데이터 구조는 JSON 데이터가 구성되는 방법을 설명하고 개별 JSON 항목을 시나리오의 다른 모듈에 매핑할 수 있도록 합니다. 데이터 구조를 제공하지 않으면 모듈을 수동으로 실행할 수 있으며 [!DNL Workfront Fusion]이(가) 제공된 JSON에서 구조를 작성합니다.

1. 시나리오에 [!UICONTROL JSON 구문 분석] 모듈을 추가합니다.
1. **[!UICONTROL JSON 문자열]** 필드에 데이터 구조를 작성할 JSON을 입력합니다.
1. 아직 [!UICONTROL JSON 구문 분석] 모듈에 다른 모듈을 연결하지 마십시오. [!DNL Workfront Fusion]이(가) JSON 데이터의 구조를 아직 모르기 때문에 [!UICONTROL JSON 구문 분석] 모듈의 데이터를 시나리오의 다른 모듈에 매핑할 수 없습니다.
1. 수동으로 시나리오를 실행합니다. 이렇게 하면 [!UICONTROL JSON 구문 분석] 모듈이 제공한 JSON에서 JSON 구조를 식별할 수 있습니다.
1. 이제 다음 모듈을 연결할 수 있습니다. 이제 JSON 구문 분석 모듈의 항목을 매핑에 사용할 수 있습니다.

자세한 내용은 [!UICONTROL Adobe Workfront Fusion]](../../workfront-fusion/modules/data-structures.md)의 [데이터 구조를 참조하십시오.

### 컬렉션과 배열 비교

JSON 문자열 필드에 컬렉션 `{ ... }`이(가) 포함된 경우 출력은 해당 컬렉션의 항목이 포함된 단일 번들입니다.

>[!INFO]
>
>**예:**
>
>```
>{
>       "name" : "Peter",
>
>    
   "ID" : 1
>}
>```
>
>![](assets/json-collection.png)

JSON 문자열 필드에 배열 `[ ... ]`이(가) 포함된 경우 출력은 일련의 번들입니다. 각 번들에는 배열의 한 요소가 포함되어 있습니다.

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
 {
>       "name" : "Mike",
>       "ID" : 2
>   }
>]
>```
>
>![](assets/json-array.png)

## [!UICONTROL JSON] 모듈 및 해당 필드

[!DNL JSON] 모듈을 구성할 때 [!DNL Workfront Fusion]에 아래 나열된 필드가 표시됩니다. 이러한 필드와 함께 앱이나 서비스의 액세스 수준과 같은 요소에 따라 추가 JSON 필드가 표시될 수 있습니다. 모듈의 굵은 제목은 필수 필드를 나타냅니다.

필드나 함수 위에 맵 단추가 표시되면 이 단추를 사용하여 해당 필드에 대한 변수와 함수를 설정할 수 있습니다. 자세한 내용은 [한 모듈에서 다른 모듈로 정보를 매핑 [!DNL Adobe Workfront Fusion]](../../workfront-fusion/mapping/map-information-between-modules.md)을 참조하십시오.

![](assets/map-toggle-350x74.png)

* [JSON을 XML로 변환](#convert-json-to-xml)
* [JSON 구문 분석](#parse-json)
* [JSON 만들기](#create-json)
* [JSON 변환](#transform-json)

### 집계자

#### [!UICONTROL JSON으로 집계]

이 집계 모듈은 이전 모듈의 출력을 JSON으로 집계합니다.

<table style="table-layout:auto"> 
 <col data-mc-conditions=""> 
 <col data-mc-conditions=""> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Source 모듈] </td> 
   <td> <p>JSON으로 집계할 데이터를 출력하는 모듈을 선택합니다.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL 데이터 구조]</td> 
   <td> <p>JSON을 만드는 데 사용할 데이터 구조를 선택합니다. 데이터 구조는 이 모듈에서 사용할 수 있는 다른 필드를 결정합니다. 자세한 내용은 이 문서에서 <a href="#data-structure" class="MCXref xref">데이터 구조</a>를 참조하십시오.</p> </td> 
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

### 트랜스포머

* [JSON을 XML로 변환](#convert-json-to-xml)
* [JSON 만들기](#create-json)
* [JSON 구문 분석](#parse-json)
* [JSON 변환](#transform-json)

#### [!UICONTROL JSON을 XML로 변환]

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

#### [!UICONTROL JSON 만들기]

이 작업 모듈은 데이터 구조에서 JSON을 생성합니다.

<table style="table-layout:auto"> 
 <col data-mc-conditions=""> 
 <col data-mc-conditions=""> 
 <tbody> 
  <tr> 
   <td role="rowheader">데이터 구조</td> 
   <td> <p>JSON을 만드는 데 사용할 데이터 구조를 선택합니다. 자세한 내용은 이 문서에서 <a href="#data-structure" class="MCXref xref">데이터 구조</a>를 참조하십시오.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL JSON 구문 분석]

이 작업 모듈은 JSON 문자열을 JSON 문자열 내의 데이터에 액세스할 수 있는 데이터 구조로 구문 분석합니다.

<table style="table-layout:auto"> 
 <col data-mc-conditions=""> 
 <col data-mc-conditions=""> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL 데이터 구조]</td> 
   <td> <p>JSON을 만드는 데 사용할 데이터 구조를 선택합니다. 자세한 내용은 이 문서에서 <a href="#data-structure" class="MCXref xref">데이터 구조</a>를 참조하십시오.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL JSON string] </td> 
   <td> <p>구문 분석할 JSON을 입력하거나 매핑합니다.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL JSON 변환]

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
>**예:** 다음 예제에서는 데이터 레코드를 [!DNL Google Sheets]에서 JSON 형식으로 변환하는 방법을 보여 줍니다.
>
>1. 데이터를 가져오려면 시나리오에 [!DNL Google Sheets] > [!UICONTROL 행 선택] 모듈을 배치하십시오. [!DNL Google] 스프레드시트에서 행을 검색하도록 모듈을 설정합니다. **[!UICONTROL &#x200B;반환된 최대 행 수]**&#x200B;을 작은 수로 설정하되 테스트 목적으로 1보다 크게 설정합니다(예: 3개). [!DNL Google Sheets] 모듈을 마우스 오른쪽 단추로 클릭하고 &quot;**[!UICONTROL 이 모듈만 실행]**&quot;을 선택하여 실행합니다. 모듈의 출력을 확인합니다.
>
1. [!DNL Google Sheets] 모듈 뒤에 [!UICONTROL 배열 집계] 모듈을 연결합니다. 모듈의 설정에서 **[!UICONTROL Source 노드]** 필드의 [!DNL Google Sheets] 모듈을 선택합니다. 다른 필드는 현재 상태로 두십시오.
>
1. [!UICONTROL 배열 집계] 모듈 뒤에 [!UICONTROL JSON] > [!UICONTROL JSON 만들기] 모듈을 연결합니다. 모듈의 설정에는 JSON 형식을 설명하는 데이터 구조가 필요합니다. 데이터 구조 설정을 열려면 **[!UICONTROL 추가]**&#x200B;를 클릭하십시오. 이 데이터 구조를 만드는 가장 쉬운 방법은 JSON 샘플에서 자동으로 생성하는 것입니다. **[!UICONTROL 생성기]**&#x200B;를 클릭하고 JSON 샘플을 **[!UICONTROL 샘플 데이터]** 필드에 붙여 넣으십시오.
>
**예:**
>
```
{

"books": [

{

"id": "ID",

"title": "Title",

"author": "Author"

}

]

}
```
>
1. **[!UICONTROL 저장]**&#x200B;을 클릭합니다. 이제 데이터 구조의 [!UICONTROL Specification] 필드에 생성된 구조가 포함됩니다.
1. 데이터 구조의 이름을 좀 더 구체적으로 변경하고 **[!UICONTROL 저장]**&#x200B;을 클릭하세요. 루트 배열 속성에 해당하는 필드는 JSON 모듈의 설정에서 매핑 가능한 필드로 표시됩니다.
>
1. 필드 옆에 있는 **[!UICONTROL 맵]** 단추를 클릭하고 배열 집계 출력의 `Array[]` 항목을 매핑합니다.
>
1. [!UICONTROL JSON] 모듈의 설정을 닫으려면 **[!UICONTROL 확인]**&#x200B;을 클릭하세요.
>
1. [!UICONTROL 배열 집계] 모듈의 설정을 엽니다. **[!UICONTROL Target 구조]**&#x200B;를 [!UICONTROL Custom]에서 루트 배열 특성에 해당하는 [!UICONTROL JSON] 모듈의 필드로 변경합니다. [!DNL Google Sheets] 모듈의 항목을 적절한 필드에 매핑합니다.
>
1. **[!UICONTROL 확인]**&#x200B;을 클릭하여 [!UICONTROL 배열 집계] 모듈의 설정을 닫습니다.
>
1. 시나리오를 실행합니다.
>
[!UICONTROL JSON] 모듈은 올바른 JSON 형식을 출력합니다.
>
1. [!DNL Google Sheets] 모듈의 설정을 열고 [!UICONTROL 반환되는 최대 행 수] 수를 스프레드시트의 행 수보다 크게 늘려 모든 데이터를 처리합니다.

## 문제 해결

### [!UICONTROL JSON 구문 분석] 모듈에서 데이터를 매핑할 수 없습니다.

JSON 콘텐츠가 [!UICONTROL JSON 구문 분석] 모듈에 올바르게 매핑되고 데이터 구조가 올바르게 정의되었는지 확인하십시오. 자세한 내용은 이 문서에서 [데이터 레코드를 JSON으로 변환](#transforming-data-records-to-json)을 참조하십시오.

### JSON에서 조건문을 사용할 때 모듈이 실패합니다.

JSON에서 `if`과(와) 같은 조건문을 사용할 때 따옴표를 조건문 외부에 넣으십시오.

>[!INFO]
>
**예:**
>
![](assets/quotes-in-json-350x120.png)
