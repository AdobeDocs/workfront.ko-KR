---
product-previous: workfront-fusion
product-area: workfront-integrations
navigation-topic: errors
title: 에서 오류 처리 다시 시도 [!DNL Adobe Workfront Fusion]
description: 시간이 지남에 따라 실패 사유가 사라질 가능성이 있는 경우 실패 모듈을 두 번 다시 실행하는 것이 유용한 경우도 있습니다.
author: Becky
feature: Workfront Fusion
exl-id: 1058905c-6c95-4a8c-8956-e1606f1486d9
source-git-commit: a3756f9345cbc9417a6fd110306dfa50aecc81a2
workflow-type: tm+mt
source-wordcount: '683'
ht-degree: 0%

---

# 에서 오류 처리 다시 시도 [!DNL Adobe Workfront Fusion]

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

## 에 대한 해결 방법 [!UICONTROL 다시 시도] 오류 처리 지시문

[!UICONTROL Adobe Workfront Fusion] 는 현재 을(를) 제공하지 않습니다. [!UICONTROL 다시 시도] 오류 처리 지시문이지만 기능을 모방하기 위해 두 가지 해결 방법을 사용할 수 있습니다. 자세한 내용은 [Adobe Workfront Fusion의 오류 처리에 대한 지침](../../workfront-fusion/errors/directives-for-error-handling.md).

### 사용 [!UICONTROL 나누기] 지시문

1. 시나리오 설정 패널에서 다음을 활성화합니다. **[!UICONTROL 미완료 실행 저장 허용]** 옵션을 선택합니다.

   자세한 내용은 [의 시나리오 설정 패널 [!DNL Adobe Workfront Fusion]](../../workfront-fusion/scenarios/scenario-settings-panel.md).

1. 에 설명된 대로 모듈에 오류 처리기 경로를 연결합니다. [에서 오류 처리 [!UICONTROL Adobe Workfront Fusion]](../../workfront-fusion/errors/error-handling.md).
1. 링크 [!UICONTROL 나누기] 지시문을 오류 처리기 라우팅에 추가하고 구성합니다.

   자세한 내용은 [에서 오류 처리를 위한 지시문 [!UICONTROL Adobe Workfront Fusion]](../../workfront-fusion/errors/directives-for-error-handling.md).

   ![](assets/break-directive-350x241.png)

#### 단점

* 최소 재시도 간격은 1분입니다.
* 모듈이 여러 번들을 처리하고 번들 처리가 실패하면 부분 실행(오류를 일으킨 번들만)이 불완전 실행 폴더로 이동되고 다음에 따라 다시 시도하도록 예약됩니다. [!UICONTROL 나누기] 지시문 설정. 하지만 현재 실행은 계속되고 모듈은 후속 번들을 계속 처리합니다. 를 활성화할 수 있습니다.[!UICONTROL 순차적 처리]의 &quot; 옵션 [!UICONTROL 시나리오 설정] 미완료 실행 폴더에 저장된 실행이 성공적으로 해결될 때까지 시나리오가 다시 실행되지 않도록 합니다.

  불완전한 실행에 대한 자세한 내용은 [에서 불완전한 실행 보기 및 해결 [!DNL Adobe Workfront Fusion]](../../workfront-fusion/scenarios/view-and-resolve-incomplete-executions.md).

### 사용 [!UICONTROL 반복] 모듈

1. 다음을 사용합니다. **[!UICONTROL 반복]** 모듈 및 설정 **[!UICONTROL 반복]** 최대 시도 횟수까지의 필드입니다.
1. 잠재적으로 장애가 발생할 수 있는 모듈을 **[!UICONTROL 반복]** 모듈.
1. 이 모듈에 오류 처리기 경로를 연결합니다(참조). [에서 오류 처리 [!DNL Adobe Workfront Fusio]n](../../workfront-fusion/errors/error-handling.md)).
1. 링크 **[!UICONTROL 도구] > [!UICONTROL 수면]** 모듈이 오류 처리기 경로에 추가되고 **[!UICONTROL 지연]** 시도 사이의 시간(초)을 나타내는 필드입니다.

1. 링크 **[!UICONTROL 무시]** 다음 뒤에 지시문 **[!UICONTROL 도구] > [!UICONTROL 수면]** 모듈(참조) [Adobe Workfront Fusion의 오류 처리에 대한 지침](../../workfront-fusion/errors/directives-for-error-handling.md)).

1. 링크 **[!UICONTROL 도구] > [!UICONTROL 변수 설정]** 모듈 뒤에 있는 모듈을 호출하고 모듈의 결과를 라는 변수에 저장하도록 구성합니다(예: ). `Result`.

1. 링크 **[!UICONTROL 배열 집계]** 다음 뒤에 있는 모듈 **[!UICONTROL 도구] > [!UICONTROL 변수 설정]** 및 선택 **[!DNL Repeater]** 소스 모듈 필드의 모듈입니다.

1. 링크 **[!UICONTROL 도구] > [!UICONTROL 변수 가져오기]** 에 대한 모듈 **[!UICONTROL 배열 집계]** 을(를) 모듈화하고 의 값을 가져오도록 구성 `Result` 변수를 채우는 방법에 따라 페이지를 순서대로 표시합니다.

1. 삽입 **[!UICONTROL 도구] > [!UICONTROL 변수 가져오기]** 다음 사이에 있는 모듈 **[!UICONTROL 반복]** 모듈 및 실패할 수 있는 모듈을 구성하고 구성하면 다음과 같은 가치를 얻을 수 있습니다. `Result` 변수를 채우는 방법에 따라 페이지를 순서대로 표시합니다.

1. 사이에 필터 삽입 **[!UICONTROL 도구] > [!UICONTROL 변수 가져오기]** 모듈 및 잠재적인 실패 모듈은 `Result` 변수가 없습니다.

>[!INFO]
>
>**예:** 다음은 가 표시되는 샘플 시나리오입니다. [!UICONTROL HTTP] >[!UICONTROL 요청] 모듈은 잠재적으로 결함이 있는 모듈을 나타냅니다.
>
>![](assets/http-make-request-350x116.png)
>
>실패할 가능성이 있는 모듈의 결과가 너무 복잡하여 간단한 변수에 저장할 수 없는 경우 데이터 저장소를 사용하여 결과를 저장/검색할 수 있습니다. 데이터 저장소에는 하나의 레코드만 포함됩니다. 레코드의 키는 다음과 같을 수 있습니다. `Result`.
>
>데이터 저장소에 대한 자세한 내용은 [의 데이터 저장소 [!DNL Adobe Workfront Fusion]](../../workfront-fusion/modules/data-stores.md)

#### 결점

이 해결 방법은 너무 복잡해 보일 수 있으며 작업 측면에서도 더 까다롭습니다.
