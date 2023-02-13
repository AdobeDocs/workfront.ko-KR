---
content-type: reference
product-previous: workfront-fusion
product-area: workfront-integrations
navigation-topic: functions
title: Adobe Workfront Fusion의 수학 함수
description: Adobe Workfront Fusion 매핑 패널에서 다음 수학 함수를 사용할 수 있습니다.
author: Becky
feature: Workfront Fusion
exl-id: 8a3c7a89-62b5-45e9-b857-8beedd0e5af4
source-git-commit: c57a796ccbfb36bce58d49345e7515dd524604c5
workflow-type: tm+mt
source-wordcount: '288'
ht-degree: 1%

---

# 의 수학 함수 [!DNL Adobe Workfront Fusion]

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

## [!UICONTROL 평균 ([값 배열]) average(value1; [value2],..)]

특정 배열에 있는 숫자 값의 평균 값 또는 개별적으로 입력한 숫자 값의 평균 값을 반환합니다.

## [!UICONTROL ceil(숫자)]

지정된 숫자보다 크거나 같은 최소 정수를 반환합니다.

>[!INFO]
>
>**예:**
>
>* `ceil(` `1.2` `)`
   >
   >   반환 2
>
>* `ceil(` `4` `)`
   >
   >   반환 4


## [!UICONTROL floor(숫자)]

지정한 수보다 작거나 같은 가장 큰 정수를 반환합니다.

>[!INFO]
>
>**예:**
>
>* `floor(` `1.2` `)`
   >
   >   반환 1
>
>* `floor(` `1.9` `)`
   >
   >   반환 1
>
>* `floor(` `4` `)`
   >
   >   반환 4


## [!UICONTROL formatNumber (number; decimalPOINTS; [decimalSeparator]; [천 단위 구분 기호])]

요청된 형식의 숫자를 반환합니다. 기본적으로 소수점 은 쉼표(,)이고 천 단위 구분 기호는 마침표(.)입니다.

>[!INFO]
>
>**예:**
>
>`formatNumber( 123456789 ; 3 ; , ; . )`
>
>123.456.789,000 반환

## [!UICONTROL 최대 ([값 배열]), max(value1;value2; ...)]

지정된 배열에서 가장 큰 수나 개별적으로 입력한 숫자 중에서 가장 큰 숫자를 반환합니다.

## [!UICONTROL min ([값 배열]), min(value1; value2; ...)]

지정된 배열의 가장 작은 숫자 또는 개별적으로 입력한 숫자 중에서 가장 작은 숫자를 반환합니다.

## [!UICONTROL parseNumber (number; 소수점 구분 기호)]

숫자가 있는 문자열을 구문 분석하고 숫자를 반환합니다. 예를 들어 parseNumber(1 756,456;,)

## [!UICONTROL round (number)]

숫자 값을 가장 가까운 정수로 반올림합니다.

>[!INFO]
>
>**예:**
>
>* `round(` `1.2` `)`
   >
   >   반환 1
>
>* `round(` `1.5` `)`
   >
   >   반환 2
>
>* `round(` `1.7` `)`
   >
   >   반환 2
> 
>* `round(` `2` `)`
   >
   >   반환 2


## [!UICONTROL sum ([값 배열]), sum(value1; value2; ...)]

지정된 배열에 있는 값의 합계 또는 개별적으로 입력한 숫자의 합계를 반환합니다.
