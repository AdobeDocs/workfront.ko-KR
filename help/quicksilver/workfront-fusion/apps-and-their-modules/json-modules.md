---
content-type: reference
product-previous: workfront-fusion
product-area: workfront-integrations
navigation-topic: apps-and-their-modules
title: JSON 모듈
description: Adobe Workfront Fusion JSON 앱에서는 데이터 컨텐츠에서 추가로 작업하거나 새 JSON 컨텐츠를 만들 수 있도록 JSON 형식으로 데이터를 처리하는 모듈을 제공합니다.
author: Becky
feature: Workfront Fusion
exl-id: 60540608-9d2e-4e10-9fb2-5388dda64784
source-git-commit: 885d93dd4383945538e977fd3edbfd55bda88b70
workflow-type: tm+mt
source-wordcount: '1157'
ht-degree: 0%

---

# [!UICONTROL JSON] 모듈

다음 [!DNL Adobe Workfront Fusion] [!UICONTROL JSON] 앱에서 JSON 형식으로 데이터를 처리하는 모듈을 제공하므로 [!DNL Adobe Workfront Fusion] 는 데이터 콘텐츠로 추가로 작업하거나 새 JSON 콘텐츠를 만들 수 있습니다.

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
   <td> <p>[!UICONTROL [!DNL Workfront Fusion] 작업 자동화 및 통합을 위한] </p> <p>[!UICONTROL [!DNL Workfront Fusion] 작업 자동화를 위한] </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">제품</td> 
   <td>조직이 구매해야 합니다 [!DNL Adobe Workfront Fusion] 뿐만 아니라 [!DNL Adobe Workfront] 을 참조하십시오.</td> 
  </tr> 
 </tbody> 
</table>

어떤 계획, 라이센스 유형 또는 액세스 권한을 보유하고 있는지 확인하려면 [!DNL Workfront] 관리자

에 대한 자세한 정보 [!DNL Adobe Workfront Fusion] 라이센스 [[!DNL Adobe Workfront Fusion] 라이선스](../../workfront-fusion/get-started/license-automation-vs-integration.md).

## JSON 구문 분석

* [데이터 구조](#data-structure)
* [컬렉션과 어레이 비교](#collection-vs-array)

### 데이터 구조

데이터 구조는 JSON 데이터를 구성하는 방법을 설명하고 시나리오의 다른 모듈에 개별 JSON 항목을 매핑하도록 합니다. 데이터 구조를 제공하지 않는 경우 수동으로 모듈을 실행하고 [!DNL Workfront Fusion] 은 제공된 JSON에서 구조를 구축합니다.

1. 추가 [!UICONTROL JSON 구문 분석] 모듈에 대해 캐시합니다.
1. 에서 **[!UICONTROL JSON 문자열]** 필드에서 데이터 구조를 작성할 JSON을 입력합니다.
1. 다른 모듈은 [!UICONTROL JSON 구문 분석] 모듈이 아직 없습니다. 왜냐면 [!DNL Workfront Fusion] 아직 JSON 데이터의 구조를 알지 못하며, 아직 의 데이터를 매핑할 수 없습니다 [!UICONTROL JSON 구문 분석] 모듈이 시나리오의 다른 모듈에 적용됩니다.
1. 시나리오를 수동으로 실행합니다. 이를 통해 [!UICONTROL JSON 구문 분석] 제공한 JSON에서 JSON 구조를 식별하는 모듈입니다.
1. 이제 다음 모듈을 연결할 수 있습니다. 이제 구문 분석 JSON 모듈의 항목을 매핑에 사용할 수 있습니다.

자세한 내용은 [의 데이터 구조 [!UICONTROL Adobe Workfront Fusion]](../../workfront-fusion/modules/data-structures.md).

### 컬렉션과 어레이 비교

JSON 문자열 필드에 컬렉션이 포함되어 있는 경우 `{ ... }`: 출력은 컬렉션의 항목을 포함하는 단일 번들입니다.

>[!INFO]
>
>**예:**
>
>
```
>{
>       "name" : "Peter",
>
>    
   "ID" : 1
>}
>```
>
>![](assets/json-collection.png)

JSON 문자열 필드에 배열이 포함되어 있는 경우 `[ ... ]`를 입력하면 출력에는 일련의 번들이 포함되어 있습니다. 각 번들에는 배열의 한 요소가 포함됩니다.

>[!INFO]
>
>**예:**
>
>
```
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

구성 시 [!DNL JSON] 모듈, [!DNL Workfront Fusion] 아래 나열된 필드를 표시합니다. 이와 함께 앱이나 서비스의 액세스 수준과 같은 요소에 따라 추가 JSON 필드가 표시될 수 있습니다. 모듈에서 굵게 표시된 제목은 필수 필드를 나타냅니다.

필드 또는 함수 위에 맵 단추가 표시되면 이 단추를 사용하여 해당 필드에 대한 변수와 함수를 설정할 수 있습니다. 자세한 내용은 [의 한 모듈에서 다른 모듈로 정보 매핑 [!DNL Adobe Workfront Fusion]](../../workfront-fusion/mapping/map-information-between-modules.md).

![](assets/map-toggle-350x74.png)

* [JSON에 합계](#aggregate-to-json)
* [JSON을 XML로 변환](#convert-json-to-xml)
* [JSON 구문 분석](#parse-json)
* [JSON 만들기](#create-json)
* [JSON 변환](#transform-json)

### [!UICONTROL JSON에 합계]

이 누적 모듈은 이전 모듈의 출력을 JSON으로 집계합니다.

<table style="table-layout:auto"> 
 <col data-mc-conditions=""> 
 <col data-mc-conditions=""> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL 소스 모듈] </td> 
   <td> <p>JSON에 집계할 데이터를 출력하는 모듈을 선택합니다.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL 데이터 구조]</td> 
   <td> <p>JSON을 만드는 데 사용할 데이터 구조를 선택합니다. 데이터 구조는 이 모듈에서 사용할 수 있는 다른 필드를 결정합니다. 자세한 내용은 <a href="#data-structure" class="MCXref xref">데이터 구조</a> 참조하십시오.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL 들여쓰기]</td> 
   <td> <p> 탭, 두 공백 또는 네 개의 공백을 사용하여 JSON을 들여쓰는지 여부를 선택합니다.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Group by]</td> 
   <td>집계된 출력을 그룹화할 표현식을 정의합니다. 이 표현식은 하나 이상의 매핑된 항목을 포함할 수 있습니다. 그런 다음 집계된 데이터는 이 표현식의 값을 사용하여 그룹으로 분리됩니다. 각 그룹은 키(평가된 표현식)와 값(집계된 텍스트)으로 별도의 번들로 출력됩니다. 키를 후속 모듈에서 필터로 사용할 수 있습니다.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL 빈 집계 후 처리 중지]</td> 
   <td>결과가 없는 경우 시나리오를 중지하려면 이 옵션을 활성화합니다.</td> 
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
   <td role="rowheader">[!UICONTROL JSON 문자열] </td> 
   <td> <p>XML로 변환할 JSON을 입력하거나 매핑합니다.</p> </td> 
  </tr> 
 </tbody> 
</table>

### [!UICONTROL JSON 구문 분석]

이 작업 모듈은 JSON 문자열을 데이터 구조로 구문 분석하므로 JSON 문자열 내의 데이터에 액세스할 수 있습니다.

<table style="table-layout:auto"> 
 <col data-mc-conditions=""> 
 <col data-mc-conditions=""> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL 데이터 구조]</td> 
   <td> <p>JSON을 만드는 데 사용할 데이터 구조를 선택합니다. 자세한 내용은 <a href="#data-structure" class="MCXref xref">데이터 구조</a> 참조하십시오.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL JSON 문자열] </td> 
   <td> <p>구문 분석할 JSON을 입력하거나 매핑합니다.</p> </td> 
  </tr> 
 </tbody> 
</table>

### [!UICONTROL JSON 만들기]

이 작업 모듈은 데이터 구조에서 JSON을 만듭니다.

<table style="table-layout:auto"> 
 <col data-mc-conditions=""> 
 <col data-mc-conditions=""> 
 <tbody> 
  <tr> 
   <td role="rowheader">데이터 구조</td> 
   <td> <p>JSON을 만드는 데 사용할 데이터 구조를 선택합니다. 자세한 내용은 <a href="#data-structure" class="MCXref xref">데이터 구조</a> 참조하십시오.</p> </td> 
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
   <td role="rowheader">[!UICONTROL Object]</td> 
   <td> <p>변형할 개체를 JSON으로 입력하거나 매핑합니다.</p> </td> 
  </tr> 
 </tbody> 
</table>

## 데이터 레코드를 JSON으로 변환

>[!INFO]
>
>**예:** 다음 예제에서는 데이터 레코드를 [!DNL Google Sheets] JSON 형식으로 :
>
>1. 배치 [!DNL Google Sheets] > [!UICONTROL 행 선택] 모듈의 데이터를 가져옵니다. 모듈에서 행을 검색하도록 모듈을 설정합니다 [!DNL Google] 스프레드시트. 을 &#x200B; 설정합니다.**[!UICONTROL 반환된 최대 행 수]** 작은 숫자에 추가하되, 테스트 목적으로 하나 이상이면 됩니다(예: 3). 를 실행합니다 [!DNL Google Sheets] 마우스 오른쪽 단추를 클릭하고 &quot;**[!UICONTROL 이 모듈만 실행]**.&quot; 모듈의 출력을 확인합니다.
1. 연결 [!UICONTROL 어레이 누적] 모듈 뒤 [!DNL Google Sheets] 모듈. 모듈의 설정에서 을(를) 선택합니다. [!DNL Google Sheets] 의 모듈 **[!UICONTROL 소스 노드]** 필드. 다른 필드는 현재 상태로 둡니다.
1. Connect [!UICONTROL JSON] > [!UICONTROL JSON 만들기] 모듈 뒤 [!UICONTROL 어레이 누적] 모듈. 모듈의 설정에는 JSON 형식을 설명하는 데이터 구조가 필요합니다. 클릭 **[!UICONTROL 추가]** 데이터 구조 설정을 엽니다. 이 데이터 구조를 만드는 가장 쉬운 방법은 JSON 샘플에서 자동으로 생성하는 것입니다. 클릭 **[!UICONTROL 생성기]** JSON 샘플을 **[!UICONTROL 샘플 데이터]** 필드:

   **예:**
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
1. **[!UICONTROL 저장]**&#x200B;을 클릭합니다. 다음 [!UICONTROL 사양] 이제 데이터 구조의 필드에 생성된 구조가 포함됩니다.
1. 데이터 구조 이름을 좀 더 구체적으로 변경하고 을(를) 클릭합니다 **[!UICONTROL 저장]**. 루트 배열 속성에 해당하는 필드가 JSON 모듈 설정에서 매핑 가능한 필드로 표시됩니다.
1. 을(를) 클릭합니다. **[!UICONTROL 맵]** 필드 옆에 있는 버튼을 클릭하여 `Array[]` 배열 누적 출력의 항목이 표시됩니다.
1. 클릭 **[!UICONTROL 확인]** 를 [!UICONTROL JSON] 모듈의 설정.
1. 설치 프로그램을 엽니다. [!UICONTROL 어레이 누적] 모듈. 변경 **[!UICONTROL Target 구조]** 변환 전: [!UICONTROL 사용자 지정] 변환 후 [!UICONTROL JSON] 루트 배열 특성에 해당하는 모듈의 필드입니다. 에서 항목 매핑 [!DNL Google Sheets] 모듈이 해당 필드에 삽입됩니다.
1. 클릭 **[!UICONTROL 확인]** 를 [!UICONTROL 어레이 누적] 모듈의 설정.
1. 시나리오를 실행합니다.
   다음 [!UICONTROL JSON] 모듈은 올바른 JSON 형식을 출력합니다.
1. 설치 프로그램을 엽니다. [!DNL Google Sheets] 모듈 및 증가 [!UICONTROL 반환된 최대 행 수] 숫자를 스프레드시트의 행 수보다 크게 하여 모든 데이터를 처리합니다.


## 문제 해결

### 에서 데이터를 매핑할 수 없습니다. [!UICONTROL JSON 구문 분석] 모듈

JSON 콘텐츠가 [!UICONTROL JSON 구문 분석] 모듈 및 데이터 구조가 올바르게 정의되어 있는지 확인합니다. 자세한 내용은 [데이터 레코드를 JSON으로 변환](#transforming-data-records-to-json) 참조하십시오.

### JSON에서 조건문을 사용할 때 모듈이 실패합니다

다음과 같은 조건문을 사용하는 경우 `if` json에서 따옴표를 조건문 외부에 지정합니다.

>[!INFO]
**예:**
![](assets/quotes-in-json-350x120.png)
