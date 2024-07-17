---
product-previous: workfront-fusion
product-area: workfront-integrations
navigation-topic: errors
title: ' [!DNL Adobe Workfront Fusion]에서 오류 처리 다시 시도'
description: 시간이 지남에 따라 실패 사유가 사라질 가능성이 있는 경우 실패 모듈을 두 번 다시 실행하는 것이 유용한 경우도 있습니다.
author: Becky
feature: Workfront Fusion
exl-id: 1058905c-6c95-4a8c-8956-e1606f1486d9
source-git-commit: a3756f9345cbc9417a6fd110306dfa50aecc81a2
workflow-type: tm+mt
source-wordcount: '683'
ht-degree: 0%

---

# [!DNL Adobe Workfront Fusion]에서 오류 처리 다시 시도

시간이 지남에 따라 실패 원인이 전달될 가능성이 있는 경우 실패한 모듈을 다시 실행하는 것이 유용한 경우도 있습니다.

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

## [!UICONTROL 다시 시도] 오류 처리 지시문에 대한 해결 방법

[!UICONTROL Adobe Workfront Fusion]은(는) 현재 [!UICONTROL Retry] 오류 처리 지시문을 제공하지 않지만 두 가지 해결 방법을 사용하여 해당 기능을 모방할 수 있습니다. 자세한 내용은 [Adobe Workfront Fusion의 오류 처리에 대한 지시문](../../workfront-fusion/errors/directives-for-error-handling.md)을 참조하십시오.

### [!UICONTROL Break] 지시문 사용

1. 시나리오 설정 패널에서 **[!UICONTROL 불완전한 실행 저장 허용]** 옵션을 활성화합니다.

   자세한 내용은 [시나리오 설정 패널 [!DNL Adobe Workfront Fusion]](../../workfront-fusion/scenarios/scenario-settings-panel.md)을 참조하세요.

1. [!UICONTROL Adobe Workfront Fusion]](../../workfront-fusion/errors/error-handling.md)의 [오류 처리에 설명된 대로 모듈에 오류 처리기 경로를 연결합니다.
1. [!UICONTROL Break] 지시문을 오류 처리기 경로에 연결하고 구성합니다.

   자세한 내용은 [!UICONTROL Adobe Workfront Fusion]](../../workfront-fusion/errors/directives-for-error-handling.md)에서 오류 처리에 대한 [지시문을 참조하십시오.

   ![](assets/break-directive-350x241.png)

#### 단점

* 최소 재시도 간격은 1분입니다.
* 모듈이 여러 번들을 처리하고 번들 처리가 실패하면 부분 실행(오류를 일으킨 번들만)이 불완전한 실행 폴더로 이동되고 [!UICONTROL Break] 지시문 설정에 따라 다시 시도하도록 예약됩니다. 하지만 현재 실행은 계속되고 모듈은 후속 번들을 계속 처리합니다. [!UICONTROL 시나리오 설정]에서 &quot;[!UICONTROL 순차적 처리]&quot; 옵션을 사용하면 미완료 실행 폴더에 저장된 실행이 정상적으로 해결될 때까지 시나리오가 다시 실행되지 않도록 할 수 있습니다.

  불완전한 실행에 대한 자세한 내용은 [불완전한 실행 보기 및 해결 [!DNL Adobe Workfront Fusion]](../../workfront-fusion/scenarios/view-and-resolve-incomplete-executions.md)을 참조하십시오.

### [!UICONTROL 반복] 모듈 사용

1. **[!UICONTROL 반복]** 모듈을 사용하고 해당 **[!UICONTROL 반복]** 필드를 최대 시도 횟수로 설정하십시오.
1. 실패할 가능성이 있는 모듈을 **[!UICONTROL 반복]** 모듈에 연결합니다.
1. 이 모듈에 오류 처리기 경로를 연결합니다( [!DNL Adobe Workfront Fusio]n](../../workfront-fusion/errors/error-handling.md)의 [오류 처리 참조).
1. **[!UICONTROL 도구] > [!UICONTROL 절전 모드]** 모듈을 오류 처리기 경로에 연결하고 **[!UICONTROL 지연]** 필드를 시도 간격(초)으로 설정합니다.

1. **[!UICONTROL 도구] > [!UICONTROL 절전 모드]** 모듈 뒤에 **[!UICONTROL Ignore]** 지시문을 연결합니다(Adobe Workfront Fusion의 오류 처리에 대한 [지시문 참조](../../workfront-fusion/errors/directives-for-error-handling.md)).

1. 실패할 가능성이 있는 모듈 뒤에 **[!UICONTROL 도구] > [!UICONTROL 변수 설정]** 모듈을 연결하고 모듈의 결과를 이름이 `Result`인 변수에 저장하도록 구성합니다.

1. **[!UICONTROL 도구] > [!UICONTROL 변수 설정]** 뒤에 **[!UICONTROL 배열 집계]** 모듈을 연결하고 Source 모듈 필드에서 **[!DNL Repeater]** 모듈을 선택합니다.

1. **[!UICONTROL 도구] > [!UICONTROL 변수 가져오기]** 모듈을 **[!UICONTROL 배열 집계]** 모듈에 연결하고 `Result` 변수의 값을 가져오도록 구성하십시오.

1. **[!UICONTROL Repeater]** 모듈과 실패할 가능성이 있는 모듈 사이에 **[!UICONTROL Tools] > [!UICONTROL 변수 가져오기]** 모듈을 삽입하고 `Result` 변수의 값을 가져오도록 구성합니다.

1. 이 **[!UICONTROL 도구] > [!UICONTROL 변수 가져오기]** 모듈과 실패할 가능성이 있는 모듈 사이에 필터를 삽입하여 `Result` 변수가 없는 경우에만 계속합니다.

>[!INFO]
>
>**예:** 다음은 [!UICONTROL HTTP] >[!UICONTROL 요청 만들기] 모듈이 잠재적으로 실패한 모듈을 나타내는 샘플 시나리오입니다.
>
>![](assets/http-make-request-350x116.png)
>
>실패할 가능성이 있는 모듈의 결과가 너무 복잡하여 간단한 변수에 저장할 수 없는 경우 데이터 저장소를 사용하여 결과를 저장/검색할 수 있습니다. 데이터 저장소에는 하나의 레코드만 포함됩니다. 레코드의 키(예: `Result`)는 다음과 같습니다.
>
>데이터 저장소에 대한 자세한 내용은 [데이터 저장소 [!DNL Adobe Workfront Fusion]](../../workfront-fusion/modules/data-stores.md)를 참조하세요.

#### 결점

이 해결 방법은 너무 복잡해 보일 수 있으며 작업 측면에서도 더 까다롭습니다.
