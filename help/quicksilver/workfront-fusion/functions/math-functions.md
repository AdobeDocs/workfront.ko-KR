---
content-type: reference
product-previous: workfront-fusion
product-area: workfront-integrations
navigation-topic: functions
title: Adobe Workfront Fusion의 수학 함수
description: Adobe Workfront Fusion 설명서가 새 위치로 이동했습니다. 이 문서는 더 이상 사용되지 않지만, 이 기능을 다루는 새 문서에 대한 링크를 포함합니다.
author: Becky
feature: Workfront Fusion
exl-id: 8a3c7a89-62b5-45e9-b857-8beedd0e5af4
source-git-commit: 2d6af8b4988bd9aab7381daa79dec79e41408c45
workflow-type: tm+mt
source-wordcount: '366'
ht-degree: 1%

---

# [!DNL Adobe Workfront Fusion]의 연산 함수

>[!IMPORTANT]
>
>Adobe Workfront Fusion 설명서가 새 위치로 이동했습니다.
>
>이 문서의 정보는 이제 문서에서 찾을 수 있습니다.
>
>* [계산 함수](https://experienceleague.adobe.com/docs/workfront-fusion/using/references/mapping-panel/functions/math-functions.html)
>
>모든 책갈피를 업데이트하십시오.
>
>이 문서는 더 이상 업데이트되지 않으며 곧 제거될 예정입니다.

<!--Audited: 4/2024-->

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

## [!UICONTROL 평균([값 배열]) 평균(value1; [값2], ...)]

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

## [!UICONTROL 층(숫자)]

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

## [!UICONTROL max([값 배열]), max(value1;value2; ...)]

지정된 배열에서 가장 큰 숫자를 반환하거나 개별적으로 입력한 숫자 중 가장 큰 숫자를 반환합니다.

## [!UICONTROL 분([값 배열]), min(value1; value2; ...)]

지정된 배열에서 가장 작은 숫자를 반환하거나 개별적으로 입력한 숫자 중 가장 작은 숫자를 반환합니다.

## [!UICONTROL 라운드(숫자)]

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

## [!UICONTROL 합계([값 배열]), sum(value1; value2; ...)]

지정된 배열의 값 합계 또는 개별적으로 입력한 숫자 합계를 반환합니다.

## [!UICONTROL parseNumber(숫자, 소수점 구분 기호)]

문자열을 숫자로 구문 분석하고 숫자를 반환합니다. 예를 들어 parseNumber(1 756,456;,)

## [!UICONTROL formatNumber(number; decimalPOINTS; [decimalSeparator]; [thousandsSeparator])]

요청한 형식으로 숫자를 반환합니다. 기본적으로 소수점은 쉼표(,)이고 천 단위 구분 기호는 마침표(.)입니다.

>[!INFO]
>
>**예:**
>
>`formatNumber( 123456789 ; 3 ; , ; . )`
>
>반환 123.456.789,000
