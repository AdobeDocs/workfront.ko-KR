---
product-previous: workfront-fusion
product-area: workfront-integrations
navigation-topic: functions
title: 에서 함수를 사용하여 항목 매핑 [!DNL Adobe Workfront Fusion]
description: 항목을 매핑할 때 함수를 사용하여 단순 공식이나 복잡한 공식을 만들 수 있습니다.
author: Becky
feature: Workfront Fusion
exl-id: e64d9b1e-8576-43db-ac29-0d386a482fbc
source-git-commit: 97f91d663df86341a079894cff04d07c18b7bf08
workflow-type: tm+mt
source-wordcount: '488'
ht-degree: 0%

---

# 에서 함수를 사용하여 항목 매핑 [!DNL Adobe Workfront Fusion]

항목을 매핑할 때 함수를 사용하여 단순 공식이나 복잡한 공식을 만들 수 있습니다.

에서 사용할 수 있는 함수 [!DNL Adobe Workfront Fusion] 는 Excel 및 일부 프로그래밍 언어에서 사용되는 함수와 유사합니다. 일반 논리, 수학, 텍스트, 날짜 및 배열을 평가합니다. 이 매개 변수를 사용하면 텍스트를 대문자로 변환, 트리밍 텍스트, 날짜를 다른 형식으로 변환하는 등의 항목 값에 대한 조건부 로직 및 변형을 수행할 수 있습니다. 자세한 내용은 [Adobe Workfront Fusion에서 한 모듈의 정보를 다른 모듈에 매핑](../../workfront-fusion/mapping/map-information-between-modules.md).

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

## 필드에 함수 삽입

필드를 클릭하면 [!UICONTROL 매핑] 패널이 표시됩니다. 매핑 패널에는 몇 가지 탭이 있습니다.

![](assets/functions-toolbar-350x189.png)

첫 번째 탭 ![](assets/toolbar-icon-functions-you-map-from-other-modules.png) (패널을 열 때 표시됨)에는 다른 모듈에서 매핑할 수 있는 항목이 표시됩니다.

다른 탭에는 다음과 같은 유형의 함수가 포함되어 있습니다.

* **일반 함수** ![](assets/toolbar-icon-general-function.png) - 다음을 참조하십시오. [의 일반 함수 [!DNL Adobe Workfront Fusion]](../../workfront-fusion/functions/general-functions.md) 추가 정보.

* **수학 함수** ![](assets/toolbar-icon-math-functions.png) - 다음을 참조하십시오. [의 수학 함수 [!DNL Adobe Workfront Fusion]](../../workfront-fusion/functions/math-functions.md) 추가 정보.

* **텍스트 및 이진 함수** ![](assets/toolbar-icon-text&binary-functions.png) - 다음을 참조하십시오. [의 문자열 함수 [!DNL Adobe Workfront Fusion]](../../workfront-fusion/functions/string-functions.md) 추가 정보.

* **날짜 및 시간** ![](assets/toolbar-icon-date&time-functions.png) - 다음을 참조하십시오. [의 날짜 및 시간 함수 [!DNL Adobe Workfront Fusion]](../../workfront-fusion/functions/date-and-time-functions.md) 자세한 내용은 아래 문서를 참조하십시오.

   * [의 날짜 및 시간 형식에 대한 토큰 [!DNL Adobe Workfront Fusion]](../../workfront-fusion/functions/tokens-for-date-and-time-formatting.md)
   * [의 날짜 및 시간 구문 분석에 대한 토큰 [!DNL Adobe Workfront Fusion]](../../workfront-fusion/functions/tokens-for-date-and-time-parsing.md)

* **어레이 작업 기능** ![](assets/toolbar-icon-functions-for-arrays.png) - 다음을 참조하십시오. [의 배열 함수 [!DNL Adobe Workfront Fusion]](../../workfront-fusion/functions/array-functions.md) 추가 정보.

필드에 함수를 삽입하려면 다음을 수행하십시오.

1. 함수 이름을 클릭합니다.

   또는

   함수를 필드로 드래그합니다.

>[!INFO]
>
>**예:** 일부 데이터 유형에서는 사용자가 특정 수 이상의 문자를 입력할 수 없습니다. 하위 문자열 함수를 사용하여 값을 특정 문자 수로 제한할 수 있습니다.
>
>이 예에서 하위 문자열 함수는 프로젝트 이름을 50자로 제한합니다.
>
>![](assets/example-meet-length-restriction-350x184.png)

## 함수 중첩

함수를 서로 중첩할 수 있습니다.

## 사용 [!DNL Google Sheets] 함수

If [!DNL Workfront Fusion] 사용할 함수는 없지만 [!DNL Google Sheets]로 지정하는 경우 다음 절차에 따라 사용할 수 있습니다.

1. in [!DNL Google Sheets]를 눌러 빈 스프레드시트를 새로 만듭니다.
1. in [!DNL Workfront Fusion]시나리오를 엽니다.
1. 추가 **[!DNL Google Sheets]** >**[!UICONTROL 셀 업데이트]** 모듈에 대해 고려합니다.

   모듈 추가에 대한 지침은 [시나리오에서 모듈 추가](../../workfront-fusion/scenarios/create-a-scenario.md#add) 기사 [에서 시나리오 만들기 [!DNL Adobe Workfront Fusion]](../../workfront-fusion/scenarios/create-a-scenario.md).

1. 모듈을 구성합니다.

   1. 에서 새로 만든 스프레드시트를 선택합니다 **[!UICONTROL 스프레드시트]** 필드.
   1. 가 포함된 공식을 삽입합니다. [!DNL Google Sheets] 함수 내에 있어야 합니다. **[!UICONTROL 값]** 필드.

      이전 모듈의 출력을 평소대로 사용할 수 있습니다.

      ![](assets/exploit-google-sheet-functions-350x218.png)

1. 를 삽입합니다. **[!UICONTROL Google 시트] >[!UICONTROL 셀 가져오기]** 계산 결과를 가져오는 모듈입니다.
1. 4단계에서 사용한 것과 동일한 셀 ID를 사용하여 모듈을 구성합니다.

   ![](assets/exploit-google-sheet-functions-2-350x187.png)
