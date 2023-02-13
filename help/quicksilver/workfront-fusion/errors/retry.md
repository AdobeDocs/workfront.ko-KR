---
product-previous: workfront-fusion
product-area: workfront-integrations
navigation-topic: errors
title: 에서 오류 처리 다시 시도 [!DNL Adobe Workfront Fusion]
description: 경우에 따라 실패 이유가 시간이 지남에 따라 실행될 가능성이 있는 경우 실패한 모듈을 두 번 다시 실행하는 것이 유용합니다.
author: Becky
feature: Workfront Fusion
exl-id: 1058905c-6c95-4a8c-8956-e1606f1486d9
source-git-commit: 97f91d663df86341a079894cff04d07c18b7bf08
workflow-type: tm+mt
source-wordcount: '639'
ht-degree: 0%

---

# 에서 오류 처리 다시 시도 [!DNL Adobe Workfront Fusion]

경우에 따라 실패 이유가 시간이 지남에 따라 실행될 가능성이 있는 경우 실패한 모듈을 다시 실행하는 것이 유용합니다.

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

## 해결 방법 [!UICONTROL 다시 시도] 오류 처리 지시문

[!UICONTROL Adobe Workfront Fusion] 현재 은 을 제공하지 않습니다 [!UICONTROL 다시 시도] 오류 처리 지시문을 사용하면 두 해결 방법을 사용하여 기능을 모방할 수 있습니다. 자세한 내용은 [Adobe Workfront Fusion의 오류 처리를 위한 지시어](../../workfront-fusion/errors/directives-for-error-handling.md).

### 를 사용하십시오 [!UICONTROL 브레이크] 지시문

1. 시나리오 설정 패널에서 **[!UICONTROL 완료되지 않은 실행 저장 허용]** 선택 사항입니다.

   자세한 내용은 [의 시나리오 설정 패널 [!DNL Adobe Workfront Fusion]](../../workfront-fusion/scenarios/scenario-settings-panel.md).

1. 에 설명된 대로 모듈에 오류 처리기 경로를 첨부합니다. [에서 오류 처리 중 [!UICONTROL Adobe Workfront Fusion]](../../workfront-fusion/errors/error-handling.md).
1. 링크 [!UICONTROL 브레이크] 오류 처리기 경로에 대한 지시문 및 구성합니다.

   자세한 내용은 [에서 오류 처리를 위한 지시어 [!UICONTROL Adobe Workfront Fusion]](../../workfront-fusion/errors/directives-for-error-handling.md).

   ![](assets/break-directive-350x241.png)

#### 단점

* 최소 재시도 간격은 1분입니다.
* 모듈이 여러 번들을 처리하고 있고 번들을 처리하지 못하는 경우 부분 실행(오류를 일으킨 번만)이 불완전한 실행 폴더로 이동되고 이 폴더에 따라 다시 시도하도록 예약됩니다 [!UICONTROL 브레이크] 지시어 설정. 그러나 현재 실행이 계속 되고 모듈은 후속 번들을 계속 처리합니다. 을(를) 활성화할 수 있습니다.[!UICONTROL 순차적 처리]&quot; 옵션을 선택합니다 [!UICONTROL 시나리오 설정] 완료되지 않은 실행 폴더에 저장된 실행이 성공적으로 해결될 때까지 시나리오가 다시 실행되지 않도록 하기 위해

불완전한 실행에 대한 자세한 내용은 [에서 불완전한 실행 보기 및 해결 [!DNL Adobe Workfront Fusion]](../../workfront-fusion/scenarios/view-and-resolve-incomplete-executions.md).

### 를 사용하십시오 [!UICONTROL 반복] 모듈

1. 를 사용하십시오 **[!UICONTROL 반복]** 모듈 및 설정 [!UICONTROL 반복] 최대 시도 횟수에 대한 필드입니다.
1. 결함이 발생할 수 있는 모듈을 **[!UICONTROL 반복]** 모듈.
1. 이 모듈에 오류 처리기 경로 연결(참조) [에서 오류 처리 중 [!DNL Adobe Workfront Fusio]n](../../workfront-fusion/errors/error-handling.md)).
1. 링크 **[!UICONTROL 도구] > [!UICONTROL Sleep]** 모듈을 오류 처리기 경로에 지정하고 설정합니다. **[!UICONTROL 지연]** 필드를 시도 사이의 시간(초)으로 지정합니다.

1. 링크 **[!UICONTROL 무시]** 다음 지시문 **[!UICONTROL 도구] > [!UICONTROL Sleep]** 모듈(참조) [Adobe Workfront Fusion의 오류 처리를 위한 지시어](../../workfront-fusion/errors/directives-for-error-handling.md)).

1. 링크 **[!UICONTROL 도구] > [!UICONTROL 변수 설정]** 모듈 다음에 모듈을 추가하고 모듈의 결과를 라는 변수에 저장하도록 구성합니다(예: `Result`.

1. 링크 **[!UICONTROL 어레이 누적]** 모듈 뒤 **[!UICONTROL 도구] > [!UICONTROL 변수 설정]** 그리고 **[!DNL Repeater]** 모듈 을 포함합니다.

1. 링크 **[!UICONTROL 도구] > [!UICONTROL 변수 가져오기]** 모듈로 **[!UICONTROL 어레이 누적]** 를 모듈로 구성한 다음 이 값을 `Result` 변수를 채우는 방법을 설명합니다.

1. 를 삽입합니다. **[!UICONTROL 도구] > [!UICONTROL 변수 가져오기]** 모듈 간 **[!UICONTROL 반복]** 모듈 및 잠재적으로 결함이 발생할 수 있는 모듈을 구성하여 `Result` 변수를 채우는 방법을 설명합니다.

1. 사이에 필터 삽입 **[!UICONTROL 도구] > [!UICONTROL 변수 가져오기]** 모듈 및 잠재적으로 장애가 발생할 수 있는 모듈은 `Result` 변수가 없습니다.

>[!INFO]
>
>**예:** 다음은 [!UICONTROL HTTP] >[!UICONTROL 요청 수행] 모듈은 잠재적으로 결함이 발생할 수 있는 모듈을 나타냅니다.
>
>![](assets/http-make-request-350x116.png)
>
>오류가 발생할 수 있는 모듈의 결과가 너무 복잡하여 단순 변수에 저장할 수 없는 경우 결과를 저장/검색하기 위해 데이터 저장소를 사용할 수 있습니다. 데이터 저장소는 하나의 레코드만 포함합니다. 레코드의 키는 다음과 같습니다. `Result`.
>
>데이터 저장소에 대한 자세한 내용은 [데이터 저장소 [!DNL Adobe Workfront Fusion]](../../workfront-fusion/modules/data-stores.md)

#### Drawback

이 해결 방법은 너무 복잡해 보일 수 있으며, 운영 측면에서도 더 까다로울 수 있습니다.
