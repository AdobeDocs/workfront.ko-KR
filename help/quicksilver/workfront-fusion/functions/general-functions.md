---
content-type: reference
product-previous: workfront-fusion
product-area: workfront-integrations
navigation-topic: functions
title: Adobe Workfront Fusion의 일반 함수
description: Adobe Workfront Fusion 매핑 패널에서 다음과 같은 일반 기능을 사용할 수 있습니다.
author: Becky
feature: Workfront Fusion
exl-id: 74bfda4e-5690-4b8c-ac58-20cf261f188d
source-git-commit: 4cca9738ad9537247234faa0b1c441163d4e315f
workflow-type: tm+mt
source-wordcount: '364'
ht-degree: 0%

---

# [!DNL Adobe Workfront Fusion]의 일반 함수

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

## [!UICONTROL get(개체 또는 배열, 경로)]

개체 또는 배열의 값 경로를 반환합니다. 중첩된 오브젝트에 액세스하려면 점 표기법을 사용하십시오. 배열의 첫 번째 항목은 인덱스 1입니다.

>[!INFO]
>
>**예:**
>
>* `get( array ; 1 + 1 )`
>* `get( array ; 5.raw_name )`
>* `get( object ; raw_name )`
>* `get( object ; raw_name.sub_raw_name )`

## [!UICONTROL if (expression; value1; value2)]

식이 true로 평가되면 `value1`을(를) 반환합니다. 그렇지 않으면 `value2`을(를) 반환합니다.

둘 이상의 식이 true로 평가되는 경우에만 값을 반환하는 if 문을 만들려면 `and` 키워드를 사용합니다.

`if` 문을 결합하려면 `and` 및 `or` 연산자를 사용합니다.

![and 연산자](/help/quicksilver/workfront-fusion/functions/assets/and-in-if-statement.png)

>[!INFO]
>
>**예:**
>
>* `if( 1 = 1 ; A ; B )`
>
>    A 반환
>
>* `if( 1 = 2 ; A ; B )`
>
>   B 반환
>
>* `if( 1 = 2 and 1 = 2 ; A ; B )`
>
>    B 반환
>   

## [!UICONTROL ifempty (value1; value2)]

이 값이 비어 있지 않으면 `value1`을(를) 반환합니다. 그렇지 않으면 `value2`을(를) 반환합니다.

>[!INFO]
>
>**예:**
>
>* `ifempty(` `A` `;` `B` )
>
>   A 반환
>
>* `ifempty(` `unknown` `;` `B` )
>
>   B 반환
>
>* `ifempty(` `""` `;` `B` )
>
>   B 반환

## [!UICONTROL switch(expression; value1; result1; [value2; result2; ...]; [else])]

값 목록에 대해 하나의 값(식이라고 함)을 평가하고 첫 번째 일치하는 값에 해당하는 결과를 반환합니다. `else` 값을 포함하려면 최종 식 또는 값 뒤에 추가하십시오.

>[!INFO]
>
>**예:**
>
>* `switch( B ; A ; 1 ; B ; 2 ; C ; 3 )`
>
>   반환 2
>
>* `switch( C ; A ; 1 ; B ; 2 ; C ; 3 )`
>
>   반환 3
>
>* `switch( X ; A ; 1 ; B ; 2 ; C ; 3 ; 4 )`
>
>   반환 4
>   
>   이 함수에서 4는 식이 적용되지 않는 경우 반환되는 값입니다(`else` 값).

## [!UICONTROL 생략(object; key1; [key2; ...])]

개체의 지정된 키를 생략하고 나머지 키를 반환합니다.

>[!INFO]
>
>**예:**
>
>`omit(` 사용자 `;` 암호 `)`
>
>암호를 제외한 사용자 정보의 컬렉션을 반환합니다.

## [!UICONTROL pick(object; key1; [key2; ...])]

개체에서 지정된 키만 선택합니다.

>[!INFO]
>
>**예:**
>
>`pick(` 사용자 `;` 암호 `;` 전자 메일 `)`
>
>사용자의 암호와 전자 메일 주소만 모아 놓은 컬렉션을 반환합니다.
