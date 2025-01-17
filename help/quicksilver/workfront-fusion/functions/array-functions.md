---
content-type: reference
product-previous: workfront-fusion
product-area: workfront-integrations
navigation-topic: functions
title: Adobe Workfront Fusion의 배열 함수
description: Adobe Workfront Fusion 설명서가 새 위치로 이동했습니다. 이 문서는 더 이상 사용되지 않지만, 이 기능을 다루는 새 문서에 대한 링크를 포함합니다.
author: Becky
feature: Workfront Fusion
exl-id: bf065d00-5d84-47e1-8169-bf9e01e2429d
source-git-commit: 2d6af8b4988bd9aab7381daa79dec79e41408c45
workflow-type: tm+mt
source-wordcount: '725'
ht-degree: 1%

---

# Adobe Workfront Fusion의 배열 함수

>[!IMPORTANT]
>
>Adobe Workfront Fusion 설명서가 새 위치로 이동했습니다.
>
>이 문서의 정보는 이제 문서에서 찾을 수 있습니다.
>
>* [배열 함수](https://experienceleague.adobe.com/docs/workfront-fusion/using/references/mapping-panel/functions/array-functions.html)
>
>모든 책갈피를 업데이트하십시오.
>
>이 문서는 더 이상 업데이트되지 않으며 곧 제거될 예정입니다.

## 액세스 요구 사항

이 문서의 기능을 사용하려면 다음 액세스 권한이 있어야 합니다.

<table style="table-layout:auto"> 
 <col>  
 <col>  
 <tbody>  
  <tr>  
   <td role="rowheader">[!DNL Adobe Workfront] 플랜</td>  
   <td> <p>임의</p> </td>  
  </tr>  
  <tr data-mc-conditions="">  
   <td role="rowheader">[!DNL Adobe Workfront] 라이센스</td>  
   <td> <p>새로운 기능: [!UICONTROL Standard]</p><p>또는</p><p>현재: [!UICONTROL Work] 이상</p> </td>  
  </tr>  
  <tr>  
   <td role="rowheader">[!DNL Adobe Workfront Fusion] 라이센스**</td>  
   <td> 
   <p>현재: [!DNL Workfront Fusion] 라이선스 요구 사항이 없습니다.</p> 
   <p>또는</p> 
   <p>레거시: 모두 </p> 
   </td>  
  </tr>  
  <tr>  
   <td role="rowheader">제품</td>  
   <td> 
   <p>신규:</p> <ul><li>[!UICONTROL Select] 또는 [!UICONTROL Prime] [!DNL Workfront] 플랜: 조직에서 [!DNL Adobe Workfront Fusion]을(를) 구매해야 합니다.</li><li>[!UICONTROL Ultimate] [!DNL Workfront] 계획: [!DNL Workfront Fusion]이(가) 포함되어 있습니다.</li></ul> 
   <p>또는</p> 
   <p>현재: 조직에서 [!DNL Adobe Workfront Fusion]을(를) 구매해야 합니다.</p> 
   </td>  
  </tr> 
 </tbody>  
</table>

이 표의 정보에 대한 자세한 내용은 [Workfront 설명서의 액세스 요구 사항](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)을 참조하십시오.

[!DNL Adobe Workfront Fusion] 라이선스에 대한 자세한 내용은 [[!DNL Adobe Workfront Fusion] 라이선스](../../workfront-fusion/get-started/license-automation-vs-integration.md)를 참조하세요.

## 함수

* [가입](#join-array-separator)
* [length](#length-array)
* [키](#keys-object)
* [조각](#slice-array-start-end)
* [병합](#merge-array1-array2)
* [포함](#contains-array-value)
* [제거](#remove-array-value1-value2)
* [추가](#add-array-value1-value2)
* [맵](#map-complex-array-keykey-for-filteringpossible-values-for-filtering)
* [무작위 재생]
* [sort](#sort-array-order-key)
* [역방향](#reverse-array)
* [평면화](#flatten-array)
* [distinct](#distinct-array-key)
* [toCollection]
* [toArray](#toarray)
* [arrayDifference](#arraydifference-array1-array2-mode)
* [중복 제거]

### [!UICONTROL 조인(배열, 구분 기호)]

각 항목 사이에 지정된 구분 기호를 사용하여 배열의 모든 항목을 문자열로 연결합니다.

### [!UICONTROL 길이(배열)]

배열의 항목 수를 반환합니다.

### [!UICONTROL 키(개체)]

특정 개체 또는 배열의 속성 배열을 반환합니다.

### [!UICONTROL 슬라이스(배열; 시작; [끝])]

선택한 항목만 포함하는 새 배열을 반환합니다.

### [!UICONTROL 병합(array1; array2; ...)]

하나 이상의 배열을 하나의 배열로 병합합니다.

### [!UICONTROL 포함(배열; 값)]

배열에 값이 포함되어 있는지 확인합니다.

### [!UICONTROL 제거(array; value1; value2; ...)]

배열의 매개 변수에 지정된 값을 제거합니다. 이 함수는 텍스트나 숫자의 기본 배열에만 적용됩니다.

### [!UICONTROL add(array; value1; value2; ...)]

매개 변수에 지정된 값을 배열에 추가하고 해당 배열을 반환합니다.

### [!UICONTROL 맵(복합 배열; 키;[필터링용 키];[필터링용 가능한 값])]

복합 배열의 값을 포함하는 기본 배열을 반환합니다. 이 함수를 사용하면 값을 필터링할 수 있습니다. 키에 원시 변수 이름을 사용합니다.

>[!INFO]
>
>**예:**
>
>* `map(Emails[];email)`
>
>  이메일이 포함된 기본 배열을 반환합니다.
>
>* `map(Emails[];email;label;work;home)`
>
>  작업 또는 홈과 동일한 레이블을 갖는 이메일이 포함된 기본 배열을 반환합니다.

자세한 내용은 [!UICONTROL Adobe Workfront Fusion]](../../workfront-fusion/mapping/map-information-between-modules.md)에서 [한 모듈에서 다른 모듈로 정보 매핑 을 참조하십시오

### 무작위 재생

### [!UICONTROL 정렬(배열; [순서]; [키])]

배열의 값을 정렬합니다. `order` 매개 변수의 올바른 값은 다음과 같습니다.

* `asc`

  (기본값) - 숫자 유형의 오름차순: 1, 2, 3, ... A, B, C, a, b, c, ... (텍스트 유형)

* `desc`

  내림차순: ..., 3, 2, 1(숫자 유형). ..., c, b, a, C, B, A(텍스트 유형).

* `asc ci`

  대/소문자를 구분하지 않는 오름차순: Text 유형의 경우 A, a, B, b, C, c, ...

* `desc ci`

  대소문자를 구분하지 않는 내림차순: ..., C, B, b, A, a(텍스트 유형).

복잡한 개체 내의 속성에 액세스하려면 `key` 매개 변수를 사용하십시오.

키에 원시 변수 이름을 사용합니다.

중첩된 속성에 액세스하려면 점 표기법을 사용하십시오.

배열의 첫 번째 항목은 인덱스 1입니다.

>[!INFO]
>
>**예:**
>
>* `sort(Contacts[];name)`
>
>    기본 오름차순으로 &quot;name&quot; 속성을 기준으로 연락처 배열 정렬
>
>* `sort(Contacts[];desc;name)`
>
>   &quot;name&quot; 속성을 기준으로 연락처 배열을 내림차순으로 정렬합니다.
>
>* `sort(Contacts[];asc ci;name)`
>
>    대소문자를 구분하지 않는 오름차순으로 &quot;name&quot; 속성으로 연락처 배열 정렬
>
>* `sort(Emails[];sender.name)`
>
>    &quot;sender.name&quot; 속성별로 이메일 배열 정렬

### [!UICONTROL 역방향(배열)]

배열의 첫 번째 요소는 마지막 요소가 되고, 두 번째 요소는 다음-마지막 요소가 됩니다.

### [!UICONTROL 병합(배열)]

지정된 깊이까지 모든 하위 배열 요소가 재귀적으로 연결된 새 배열을 만듭니다.

### [!UICONTROL distinct(배열; [키])]

배열 내의 중복을 제거합니다. 복잡한 개체 내의 속성에 액세스하려면 &quot;[!UICONTROL key]&quot; 인수를 사용하십시오. 중첩된 속성에 액세스하려면 점 표기법을 사용하십시오. 배열의 첫 번째 항목은 인덱스 1입니다.

>[!INFO]
>
>**예:** `distinct(Contacts[];name)`
>
>&quot;name&quot; 속성을 비교하여 연락처 배열 내의 중복을 제거합니다.

### toCollection

### toArray

이 함수는 컬렉션을 키-값 쌍의 배열로 변환합니다.

>[!INFO]
>
>**예:**
>
>주어진 컬렉션
>
>`{ key1: "value1", key2: "value2:}`
>
>함수
>
>`toArray({ key1: "value1", key2: "value2:})`
>
>키-값 쌍의 배열 반환
>
>`[{ key1: "value1"}, { key2: "value2"}]`

### [!UICONTROL arrayDifference [array1, array2, mode]]

두 배열 간의 차이점을 반환합니다.

`mode` 매개 변수에 대해 다음 값 중 하나를 입력하십시오.

* `classic`: `array2`에 없는 `array1`의 모든 요소를 포함하는 새 배열을 반환합니다.

* `symmetric`: 두 배열에 공통되지 않는 요소의 배열을 반환합니다.

  즉, 이 함수는 `array2`에 없는 `array1`의 모든 요소와 `array1`에 없는 `array2`의 모든 요소를 포함하는 배열을 반환합니다.

  >[!INFO]
  >
  >**예:**
  >
  >다음 배열이 지정된 경우:
  >
  >```
  >myArray = [1,2,3,4,5]
  >```
  >
  >```
  >yourArray = [3,4,5,6,7]
  >```
  >
  >* `arrayDifference [myArray, yourArray, classic]`
  >
  >    `[1,2]` 반환
  >
  >* `arrayDifference [yourArray, myArray, classic]`
  >
  >    `[6,7]` 반환
  >
  >* `arrayDifference [myArray, yourArray, symmetric]`
  >
  >    `[1,2,6,7]` 반환

### 중복 제거

## 키워드

### emptyarray
