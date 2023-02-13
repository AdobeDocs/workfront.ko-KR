---
content-type: reference
product-previous: workfront-fusion
product-area: workfront-integrations
navigation-topic: functions
title: Adobe Workfront Fusion의 배열 기능
description: Adobe Workfront Fusion 매핑 패널에서 다음 배열 기능을 사용할 수 있습니다.
author: Becky
feature: Workfront Fusion
exl-id: bf065d00-5d84-47e1-8169-bf9e01e2429d
source-git-commit: c57a796ccbfb36bce58d49345e7515dd524604c5
workflow-type: tm+mt
source-wordcount: '603'
ht-degree: 0%

---

# Adobe Workfront Fusion의 배열 기능

## 액세스 요구 사항

이 문서의 기능을 사용하려면 다음 액세스 권한이 있어야 합니다.

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] 플랜*</td> 
   <td> <p>[!DNL Pro] 이상</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader">[!DNL Adobe Workfront] 라이센스*</td> 
   <td> <p>[!UICONTROL Plan], [!UICONTROL Work]</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Adobe Workfront Fusion] 라이센스**</td> 
   <td> <p>[!UICONTROL [!DNL Workfront Fusion] 작업 자동화 및 통합을 위한] </p><p>[!UICONTROL [!DNL Workfront Fusion] 작업 자동화를 위한]</p>  </td> 
  </tr> 
  <tr> 
   <td role="rowheader">제품</td> 
   <td>조직이 구매해야 합니다 [!DNL Adobe Workfront Fusion] 뿐만 아니라 [!DNL Adobe Workfront] 을 참조하십시오.</td> 
  </tr> 
 </tbody> 
</table>

어떤 계획, 라이센스 유형 또는 액세스 권한을 보유하고 있는지 확인하려면 [!DNL Workfront] 관리자

에 대한 자세한 정보 [!DNL Adobe Workfront Fusion] 라이센스 [[!DNL Adobe Workfront Fusion] 라이선스](../../workfront-fusion/get-started/license-automation-vs-integration.md).

## [!UICONTROL 추가(배열) value1; value2; ...)]

매개 변수에 지정된 값을 배열에 추가하고 해당 배열을 반환합니다.

## [!UICONTROL 포함(배열) value)]

배열에 값이 포함되어 있는지 확인합니다.

## [!UICONTROL distinct(배열) [key])]

배열 내에서 중복을 제거합니다. &quot;[!UICONTROL key]복잡한 개체 내의 속성에 액세스하기 위한 &quot; 인수입니다. 중첩 속성에 액세스하려면 점 표기법을 사용하십시오. 배열의 첫 번째 항목은 인덱스 1입니다.

>[!INFO]
>
>**예:** `distinct(Contacts[];name)`
>
>&quot;name&quot; 속성을 비교하여 연락처 배열 내의 중복을 제거합니다

## [!UICONTROL 평면화(배열)]

지정한 깊이까지 모든 하위 배열 요소가 연결된 새 배열을 만듭니다.


## [!UICONTROL 조인(배열) 구분 기호)]

각 항목 사이에 지정된 구분자를 사용하여 배열의 모든 항목을 문자열로 연결합니다.

## [!UICONTROL 키(개체)]

지정된 개체 또는 배열의 속성 배열을 반환합니다.

## [!UICONTROL length (배열)]

배열에 있는 항목의 수를 반환합니다.

## [!UICONTROL 맵(복잡한 배열) key;[필터링 키];[필터링 가능한 값])]

복잡한 배열 값을 포함하는 기본 배열을 반환합니다. 이 함수를 사용하면 값을 필터링할 수 있습니다. 키에 원시 변수 이름을 사용합니다.

>[!INFO]
>
>**예:**
>
>* `map(Emails[];email)`
  >
>  전자 메일이 있는 기본 배열 반환
>
>* `map(Emails[];email;label;work;home)`
  >
>  작업 또는 홈과 동일한 레이블이 있는 이메일이 있는 기본 배열을 반환합니다

자세한 내용은 [의 한 모듈에서 다른 모듈로 정보 매핑 [!UICONTROL Adobe Workfront Fusion]](../../workfront-fusion/mapping/map-information-between-modules.md)


## [!UICONTROL 병합(배열1; array2; ...)]

하나 이상의 스토리지를 하나의 스토리지에 병합합니다.

## [!UICONTROL 제거(배열) value1; value2; ...)]

배열의 매개 변수에 지정된 값을 제거합니다. 이 함수는 텍스트나 숫자의 기본 배열에서만 유효합니다.

## [!UICONTROL 역방향(배열)]

배열의 첫 번째 요소는 마지막 요소가 되고, 두 번째 요소는 다음으로 끝나야 합니다.

## [!UICONTROL 슬라이스(배열) start; [end])]

선택한 항목만 포함하는 새 배열을 반환합니다.

## [!UICONTROL sort (array; [주문]; [key])]

배열의 값을 정렬합니다. 의 유효한 값 `order` 매개 변수:

* `asc`

   (기본값) - 오름차순: Number 유형의 경우 1, 2, 3, ... 텍스트 유형의 경우 A, B, C, a, b, c,..

* `desc`

   내림차순: ..., Number 유형의 경우 3, 2, 1. .., c, b, a, C, B, A(텍스트 유형).

* `asc ci`

   대소문자 구분 오름차순: 텍스트 유형의 경우 A, A, B, C, c,..

* `desc ci`

   대/소문자 구분 안 함 내림차순: .., C, c, B, A, Text 유형의 경우.

를 사용하십시오 `key` 매개 변수를 사용하여 복잡한 개체 내의 속성에 액세스합니다.

키에 원시 변수 이름을 사용합니다.

중첩 속성에 액세스하려면 점 표기법을 사용하십시오.

배열의 첫 번째 항목은 인덱스 1입니다.

>[!INFO]
>
>**예:**
>
>* `sort(Contacts[];name)`
   >
   >    기본 오름차순으로 &quot;name&quot; 속성으로 연락처 배열을 정렬합니다.
>
>* `sort(Contacts[];desc;name)`
   >
   >   연락처 배열을 &quot;name&quot; 속성으로 내림차순으로 정렬합니다.
>
>* `sort(Contacts[];asc ci;name)`
   >
   >    대/소문자를 구분하지 않는 오름차순으로 &quot;name&quot; 속성으로 연락처 배열을 정렬합니다.
>
>* `sort(Emails[];sender.name)`
   >
   >    &quot;sender.name&quot; 속성으로 이메일 배열을 정렬합니다.


## [!UICONTROL arrayDifference [array1, array2, mode]]

두 배열 간의 차이를 반환합니다.

다음 값 중 하나를 입력합니다. `mode` 매개 변수.

* `classic`: 모든 요소가 포함된 새 배열을 반환합니다. `array1` 에 존재하지 않습니다 `array2`.

* `symmetric`: 두 배열에 공통되지 않는 요소의 배열을 반환합니다.

   즉, 함수는 `array1` 에 존재하지 않습니다 `array2`, 및 `array2` 에 존재하지 않습니다 `array1`.

   >[!INFO]
   >
   >**예:**
   >
   >다음 배열이 주어집니다.
   >
   >
   ```
   >myArray = [1,2,3,4,5]
   >```
   >
   >
   ```
   >yourArray = [3,4,5,6,7]
   >```
   >
   >* `arrayDifference [myArray, yourArray, classic]`
      >
      >    반환 `[1,2]`
   >
   >* `arrayDifference [yourArray, myArray, classic]`
      >
      >    반환 `[6,7]`
   >
   >* `arrayDifference [myArray, yourArray, symmetric]`
      >
      >    반환 `[1,2,6,7]`

