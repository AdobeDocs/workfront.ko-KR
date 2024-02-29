---
content-type: reference
product-previous: workfront-fusion
product-area: workfront-integrations
navigation-topic: functions
title: Adobe Workfront Fusion의 배열 함수
description: Adobe Workfront Fusion 매핑 패널에서 다음 배열 함수를 사용할 수 있습니다.
author: Becky
feature: Workfront Fusion
exl-id: bf065d00-5d84-47e1-8169-bf9e01e2429d
source-git-commit: 5860e75d0a6521abbe082668749f78058fe7a114
workflow-type: tm+mt
source-wordcount: '679'
ht-degree: 0%

---

# Adobe Workfront Fusion의 배열 함수

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
   <td role="rowheader">[!UICONTROL Adobe Workfront Fusion] 라이선스**</td> 
   <td>
   <p>현재 라이선스 요구 사항: 아니요 [!DNL Workfront Fusion] 라이센스 요구 사항.</p>
   <p>또는</p>
   <p>기존 라이선스 요구 사항: [!UICONTROL [!DNL Workfront Fusion] for Work Automation and Integration] </p>
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

## [!UICONTROL add (array; value1; value2; ...)]

매개 변수에 지정된 값을 배열에 추가하고 해당 배열을 반환합니다.

## [!UICONTROL 포함(배열, 값)]

배열에 값이 포함되어 있는지 확인합니다.

## [!UICONTROL distinct(배열; [key])]

배열 내의 중복을 제거합니다. 사용[!UICONTROL key]복잡한 오브젝트 내의 속성에 액세스하기 위한 &quot;인수. 중첩된 속성에 액세스하려면 점 표기법을 사용하십시오. 배열의 첫 번째 항목은 인덱스 1입니다.

>[!INFO]
>
>**예:** `distinct(Contacts[];name)`
>
>&quot;name&quot; 속성을 비교하여 연락처 배열 내의 중복을 제거합니다.

## [!UICONTROL 평면화(배열)]

지정된 깊이까지 모든 하위 배열 요소가 재귀적으로 연결된 새 배열을 만듭니다.


## [!UICONTROL 조인(배열, 구분 기호)]

각 항목 사이에 지정된 구분 기호를 사용하여 배열의 모든 항목을 문자열로 연결합니다.

## [!UICONTROL keys (object)]

특정 개체 또는 배열의 속성 배열을 반환합니다.

## [!UICONTROL length(배열)]

배열의 항목 수를 반환합니다.

## [!UICONTROL 맵(복합 배열, 키;[필터링용 키];[필터링에 가능한 값])]

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

자세한 내용은 [의 한 모듈에서 다른 모듈로 정보 매핑 [!UICONTROL Adobe Workfront Fusion]](../../workfront-fusion/mapping/map-information-between-modules.md)


## [!UICONTROL merge(array1, array2, ...)]

하나 이상의 배열을 하나의 배열로 병합합니다.

## [!UICONTROL 제거(array; value1; value2; ...)]

배열의 매개 변수에 지정된 값을 제거합니다. 이 함수는 텍스트나 숫자의 기본 배열에만 적용됩니다.

## [!UICONTROL 역방향(배열)]

배열의 첫 번째 요소는 마지막 요소가 되고, 두 번째 요소는 다음-마지막 요소가 됩니다.

## [!UICONTROL slice(배열, 시작, [종료])]

선택한 항목만 포함하는 새 배열을 반환합니다.

## [!UICONTROL sort(array; [주문]; [key])]

배열의 값을 정렬합니다. 의 유효한 값 `order` 매개 변수:

* `asc`

  (기본값) - 숫자 유형의 오름차순: 1, 2, 3, ... A, B, C, a, b, c, ... (텍스트 유형)

* `desc`

  내림차순: ..., 3, 2, 1(숫자 유형). ..., c, b, a, C, B, A(텍스트 유형).

* `asc ci`

  대/소문자를 구분하지 않는 오름차순: Text 유형의 경우 A, a, B, b, C, c, ...

* `desc ci`

  대소문자를 구분하지 않는 내림차순: ..., C, B, b, A, a(텍스트 유형).

사용 `key` 매개 변수를 사용하여 복잡한 개체 내의 속성에 액세스합니다.

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

## [!UICONTROL arrayDifference [array1, array2, mode]]

두 배열 간의 차이점을 반환합니다.

다음 값 중 하나를 입력합니다 `mode` 매개 변수.

* `classic`: 의 모든 요소를 포함하는 새 배열을 반환합니다. `array1` 존재하지 않는 `array2`.

* `symmetric`: 두 배열에 공통되지 않는 요소의 배열을 반환합니다.

  즉, 이 함수는 의 모든 요소를 포함하는 배열을 반환합니다. `array1` 존재하지 않는 `array2`, 및 의 모든 요소 `array2` 존재하지 않는 `array1`.

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
  >    반환 `[1,2]`
  >
  >* `arrayDifference [yourArray, myArray, classic]`
  >
  >    반환 `[6,7]`
  >
  >* `arrayDifference [myArray, yourArray, symmetric]`
  >
  >    반환 `[1,2,6,7]`

## toArray

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
