---
content-type: reference
product-previous: workfront-fusion
product-area: workfront-integrations
navigation-topic: functions
title: Adobe Workfront Fusion의 일반 함수
description: Adobe Workfront Fusion 매핑 패널에서 다음과 같은 일반적인 기능을 사용할 수 있습니다.
author: Becky
feature: Workfront Fusion
exl-id: 74bfda4e-5690-4b8c-ac58-20cf261f188d
source-git-commit: c57a796ccbfb36bce58d49345e7515dd524604c5
workflow-type: tm+mt
source-wordcount: '255'
ht-degree: 2%

---

# 의 일반 함수 [!DNL Adobe Workfront Fusion]

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

## [!UICONTROL get (개체 또는 배열) path)]

개체 또는 배열의 값 경로를 반환합니다. 중첩된 개체에 액세스하려면 점 표기법을 사용하십시오. 배열의 첫 번째 항목은 인덱스 1입니다.

>[!INFO]
>
>**예:**
>
>* `get( array ; 1 + 1 )`
>* `get( array ; 5.raw_name )`
>* `get( object ; raw_name )`
>* `get( object ; raw_name.sub_raw_name )`


## [!UICONTROL if value1; value2)]

를 반환합니다 `value1` 표현식이 true로 평가되는 경우; 그렇지 않으면 반환 `value2`.

>[!INFO]
>
>**예:**
>
>* `if( 1 = 1 ; A ; B )`
   >
   >    반환
>
>* `if( = 2 ; A ; B )`
   >
   >   반환 B


## [!UICONTROL empty(값1; value2)]

를 반환합니다 `value1` 이 값이 비어 있지 않은 경우 그렇지 않으면 반환 `value2`.

>[!INFO]
>
>**예:**
>
>* `ifempty(` `A` `;` `B` )
   >
   >   반환
>
>* `ifempty(` `unknown` `;` `B` )
   >
   >   반환 B
>
>* `ifempty(` `""` `;` `B` )
   >
   >   반환 B


## [!UICONTROL 스위치(표현식) value1; result1; [value2; result2; ...]; [else])]

값 목록에 대해 하나의 값(표현식이라고 함)을 평가합니다. 첫 번째 일치 값에 해당하는 결과를 반환합니다.

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
>  반환 4

## [!UICONTROL compose(object) key1; [key2; ...])]

개체의 지정된 키를 생략하고 나머지 키를 반환합니다.

>[!INFO]
>
>**예:**
>
>`omit(` 사용자 `;` 암호 `)`
>
>암호를 제외하고 사용자 정보 컬렉션을 반환합니다.

## [!UICONTROL pick(object) key1; [key2; ...])]

객체에서 지정된 키만 선택합니다.

>[!INFO]
>
>**예:**
>
>`pick(` 사용자 `;` 암호 `;` 이메일 `)`
>
>사용자의 암호 및 전자 메일 주소만 컬렉션을 반환합니다.
