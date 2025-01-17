---
product-previous: workfront-fusion
product-area: workfront-integrations
navigation-topic: functions
title: ' [!DNL Adobe Workfront Fusion]에서 함수를 사용하여 항목 매핑'
description: Adobe Workfront Fusion 설명서가 새 위치로 이동했습니다. 이 문서는 더 이상 사용되지 않지만, 이 기능을 다루는 새 문서에 대한 링크를 포함합니다.
author: Becky
feature: Workfront Fusion
exl-id: e64d9b1e-8576-43db-ac29-0d386a482fbc
source-git-commit: 2d6af8b4988bd9aab7381daa79dec79e41408c45
workflow-type: tm+mt
source-wordcount: '566'
ht-degree: 1%

---

# [!DNL Adobe Workfront Fusion]에서 함수를 사용하여 항목 매핑

>[!IMPORTANT]
>
>Adobe Workfront Fusion 설명서가 새 위치로 이동했습니다.
>
>이 문서의 정보는 이제 문서에서 찾을 수 있습니다.
>
>* [함수를 사용하여 항목 매핑](https://experienceleague.adobe.com/docs/workfront-fusion/using/create-scenarios/map-data/map-using-functions.html)
>
>모든 책갈피를 업데이트하십시오.
>
>이 문서는 더 이상 업데이트되지 않으며 곧 제거될 예정입니다.

항목을 매핑할 때 함수를 사용하여 단순 또는 복합 공식을 만들 수 있습니다. [!DNL Adobe Workfront Fusion]에서 사용할 수 있는 함수는 Excel 및 일부 프로그래밍 언어의 함수와 유사합니다.

* 일반적인 논리, 수학, 텍스트, 날짜 및 배열을 평가합니다.
* 텍스트를 대문자로 변환, 텍스트 트리밍, 날짜를 다른 형식으로 변환 등과 같은 항목 값의 조건부 논리 및 변환을 수행할 수 있도록 해 줍니다.

자세한 내용은 [Adobe Workfront Fusion에서 한 모듈에서 다른 모듈로 정보 매핑](../../workfront-fusion/mapping/map-information-between-modules.md)을 참조하십시오.


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


## 매핑 탭 개요

필드에 대한 [!UICONTROL 매핑] 패널을 열려면 다음을 수행하십시오.

1. 왼쪽 패널에서 **시나리오**&#x200B;를 클릭합니다.
1. 시나리오를 선택합니다.

![](assets/open-functions-bar.png)


### 매핑 패널 탭

다음은 매핑 패널의 탭입니다.

* **일반 함수** ![](assets/toolbar-icon-general-function.png) - 자세한 내용은 [일반 함수 [!DNL Adobe Workfront Fusion]](../../workfront-fusion/functions/general-functions.md)를 참조하십시오.

* **연산 함수** ![](assets/toolbar-icon-math-functions.png) - 자세한 내용은 [연산 함수 [!DNL Adobe Workfront Fusion]](../../workfront-fusion/functions/math-functions.md)를 참조하십시오.

* **텍스트 및 이진 함수** ![](assets/toolbar-icon-text&binary-functions.png) - 자세한 내용은 [String 함수 [!DNL Adobe Workfront Fusion]](../../workfront-fusion/functions/string-functions.md)를 참조하십시오.

* **날짜 및 시간** ![](assets/toolbar-icon-date&time-functions.png) - 자세한 내용은 [날짜 및 시간 함수 [!DNL Adobe Workfront Fusion]](../../workfront-fusion/functions/date-and-time-functions.md) 및 아래 문서를 참조하십시오.

   * [ [!DNL Adobe Workfront Fusion]의 날짜 및 시간 형식에 대한 토큰](../../workfront-fusion/functions/tokens-for-date-and-time-formatting.md)
   * [ [!DNL Adobe Workfront Fusion]의 날짜 및 시간 구문 분석에 대한 토큰](../../workfront-fusion/functions/tokens-for-date-and-time-parsing.md)

* **배열을 사용하는 함수** ![](assets/toolbar-icon-functions-for-arrays.png) - 자세한 내용은 [배열 함수 [!DNL Adobe Workfront Fusion]](../../workfront-fusion/functions/array-functions.md)를 참조하십시오.

* **다른 함수 매핑** ![](assets/toolbar-icon-functions-you-map-from-other-modules.png)은(는) 다른 모듈에서 매핑할 수 있는 항목을 표시합니다. 이 탭을 항상 사용할 수는 없습니다.

![](assets/functions-toolbar-350x189.png)

## 필드에 함수 삽입

함수를 필드에 삽입하려면 다음 작업을 수행하십시오.

1. 함수 이름을 클릭합니다.

   또는

   함수를 필드로 드래그합니다.


>[!BEGINSHADEBOX]

**예:** 일부 데이터 형식을 사용하면 사용자가 특정 문자 수를 초과하여 입력할 수 없습니다. 하위 문자열 함수를 사용하여 값을 특정 문자 수로 제한할 수 있습니다.

이 예에서 하위 문자열 함수는 프로젝트 이름을 50자로 제한합니다.

![](assets/example-meet-length-restriction-350x184.png)

>[!ENDSHADEBOX]

## 함수 중첩

함수를 서로 중첩할 수 있습니다.

## [!DNL Google Sheets]개 함수 사용

[!DNL Workfront Fusion]에 사용할 함수가 없지만 [!DNL Google Sheets]에 포함된 함수가 있는 경우 다음 단계를 수행하여 사용할 수 있습니다.

1. [!DNL Google Sheets]에서 빈 스프레드시트를 새로 만듭니다.
1. [!DNL Workfront Fusion]에서 시나리오를 엽니다.
1. 시나리오에 **[!DNL Google Sheets]** >**[!UICONTROL 셀 업데이트]** 모듈을 추가합니다.

   모듈을 추가하는 방법에 대한 지침은 문서 [시나리오 만들기 [!DNL Adobe Workfront Fusion]](../../workfront-fusion/scenarios/create-a-scenario.md)에서 [시나리오에 모듈 추가](../../workfront-fusion/scenarios/create-a-scenario.md#add)를 참조하십시오.

1. 모듈을 구성합니다.

   1. **[!UICONTROL 스프레드시트]** 필드에서 새로 만든 스프레드시트를 선택합니다.
   1. [!DNL Google Sheets] 함수가 포함된 수식을 **[!UICONTROL Value]** 필드에 삽입하십시오.

      이전 모듈의 출력을 평소대로 사용할 수 있습니다.

      ![](assets/exploit-google-sheet-functions-350x218.png)

1. 계산된 결과를 얻으려면 **[!UICONTROL Google 시트] >[!UICONTROL 셀 가져오기]** 모듈을 삽입하십시오.
1. 4단계에서 사용한 것과 동일한 셀 ID를 사용하여 모듈을 구성합니다.

   ![](assets/exploit-google-sheet-functions-2-350x187.png)
