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
source-git-commit: 0915dcce45b271ee18cdd8af5db4f0eb01f3cced
workflow-type: tm+mt
source-wordcount: '332'
ht-degree: 2%

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

## [!UICONTROL 평균 ([값 배열]) average(value1; [value2], ...)]

특정 배열에 있는 숫자 값의 평균 값 또는 개별적으로 입력한 숫자 값의 평균 값을 반환합니다.

## [!UICONTROL ceil(숫자)]

지정된 숫자보다 크거나 같은 가장 작은 정수를 반환합니다.

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

지정된 숫자보다 작거나 같은 가장 큰 정수를 반환합니다.

>[!INFO]
>
>**예:**
>
>* `floor(` `1.2` `)`
>
>   1 반환
>
>* `floor(` `1.9` `)`
>
>   1 반환
>
>* `floor(` `4` `)`
>
>   반환 4

## [!UICONTROL formatNumber(숫자, 소수점, [decimalSeparator]; [천 단위 구분 기호])]

요청한 형식으로 숫자를 반환합니다. 기본적으로 소수점은 쉼표(,)이고 천 단위 구분 기호는 마침표(.)입니다.

>[!INFO]
>
>**예:**
>
>`formatNumber( 123456789 ; 3 ; , ; . )`
>
>반환 123.456.789,000

## [!UICONTROL 최대 ([값 배열]), max(value1;value2; ...)]

지정된 배열에서 가장 큰 숫자를 반환하거나 개별적으로 입력한 숫자 중 가장 큰 숫자를 반환합니다.

## [!UICONTROL 분 ([값 배열]), min(value1; value2; ...)]

지정된 배열에서 가장 작은 숫자를 반환하거나 개별적으로 입력한 숫자 중 가장 작은 숫자를 반환합니다.

## [!UICONTROL parseNumber(숫자, 소수점 구분 기호)]

문자열을 숫자로 구문 분석하고 숫자를 반환합니다. 예를 들어 parseNumber(1 756,456;,)

## [!UICONTROL round (숫자)]

숫자 값을 가장 가까운 정수로 반올림합니다.

>[!INFO]
>
>**예:**
>
>* `round(` `1.2` `)`
>
>   1 반환
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

## [!UICONTROL 합계 ([값 배열]), sum(value1; value2; ...)]

지정된 배열의 값 합계 또는 개별적으로 입력한 숫자 합계를 반환합니다.
