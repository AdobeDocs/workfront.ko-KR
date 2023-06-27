---
content-type: reference
product-previous: workfront-fusion
product-area: workfront-integrations
navigation-topic: errors
title: 에서 오류 처리 [!DNL Adobe Workfront Fusion]
description: 시나리오 실행 중에 오류가 발생하면 일반적으로 실패로 인해 서비스를 사용할 수 없거나, 서비스가 예기치 않은 데이터에 응답하거나, 입력 데이터의 유효성 검사에 실패하기 때문입니다.
author: Becky
feature: Workfront Fusion
exl-id: a08c18a0-1797-4126-827a-1ea7e11d4bad
source-git-commit: a3756f9345cbc9417a6fd110306dfa50aecc81a2
workflow-type: tm+mt
source-wordcount: '616'
ht-degree: 0%

---

# 에서 오류 처리 [!DNL Adobe Workfront Fusion]

시나리오 실행 중에 오류가 발생하면 일반적으로 실패로 인해 서비스를 사용할 수 없거나, 서비스가 예기치 않은 데이터에 응답하거나, 입력 데이터의 유효성 검사에 실패하기 때문입니다.

시나리오 실행 중에 모듈에서 오류가 발생하고 모듈에 연결된 오류 처리 경로가 없으면 의 설명에 따라 기본 오류 처리 논리가 실행됩니다 [에서 처리하는 동안 오류 발생 [!DNL Adobe Workfront Fusion]](../../workfront-fusion/errors/error-processing.md).

모듈에 오류 처리기 경로를 추가하여 기본 오류 처리 논리를 자체 오류 처리 논리로 바꿀 수 있습니다. [!DNL Adobe Workfront Fusion] 는 오류 처리기 경로 끝에 삽입할 수 있는 5개의 다른 지시문을 제공합니다.

자세한 내용은 [에서 오류 처리를 위한 지시문 [!DNL Adobe Workfront Fusion]](../../workfront-fusion/errors/directives-for-error-handling.md).

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

## 오류 처리기 경로

모듈에 오류 처리기 경로를 추가하려면 다음을 수행합니다.

1. 모듈을 마우스 오른쪽 단추로 클릭하고 를 선택합니다 **[!UICONTROL 오류 처리기 추가]**:

   ![](assets/error-handler-route.png)

   이 모듈에는 시나리오에 사용 중인 앱과 디렉티브 목록이 표시됩니다.

1. 오류 처리기를 추가한 모듈이 경로의 마지막 모듈인 경우 지시어 중 하나를 선택합니다.

   또는

   하나 이상의 모듈을 오류 처리기 경로에 추가합니다.

   경로에 모듈을 더 추가하면 [!UICONTROL 무시] 지시문은 기본적으로 적용되며 오류가 발생하면 해당 경로의 후속 모듈이 처리됩니다.


>[!INFO]
>
>이 예제에서 를 실행하는 동안 오류가 발생하는 경우 [!UICONTROL 폴더 만들기] 모듈, [!UICONTROL 무시] 지시문이 자동으로 적용되며 시나리오는 오류 처리기 경로의 다음 모듈로 이동합니다.
>
>그러나 오류가 없으면 시나리오가 [!UICONTROL 폴더 모듈의 모든 파일 나열] 일반 노선에서요.
>
>![](assets/if-there-is-no-error-350x234.png)

오류 처리기 경로는 투명한 원으로 구성되고 일반 경로는 실선 원으로 구성됩니다.

## 오류 처리 지시문

지침이 아래에 간략하게 설명되어 있습니다. 자세한 내용은 [에서 오류 처리를 위한 지시문 [!DNL Adobe Workfront Fusion]](../../workfront-fusion/errors/directives-for-error-handling.md).

시나리오 실행을 계속할지 여부에 따라 다음 카테고리로 그룹화할 수 있는 총 5개의 디렉티브가 있습니다.

다음 지시어는 시나리오 실행이 계속되도록 합니다.

* **[!UICONTROL 다시 시작]**: 오류가 있는 모듈의 대체 출력을 지정할 수 있습니다. 시나리오 실행 상태가 성공으로 표시됩니다.
* **[!UICONTROL 무시]**: 오류를 무시합니다. 시나리오 실행 상태가 성공으로 표시됩니다.
* **[!UICONTROL 나누기]**: 불완전한 실행 큐에 대한 입력을 저장합니다. 시나리오 실행 상태가 경고로 표시됩니다. 자세한 내용은 [에서 불완전한 실행 보기 및 해결 [!DNL Adobe Workfront Fusion]](../../workfront-fusion/scenarios/view-and-resolve-incomplete-executions.md).

오류가 발생할 때 시나리오 실행을 중지해야 하는 경우 다음 지시문 중 하나를 사용합니다.

* **[!UICONTROL 롤백]**: 시나리오 실행을 즉시 중단하고 상태를 오류로 표시
* **[!UICONTROL 커밋]**: 시나리오 실행을 즉시 중지하고 상태를 성공으로 표시합니다

오류 처리에 대한 자세한 내용은 다음을 참조하십시오.

* [에서 오류 처리를 위한 지시문 [!DNL Adobe Workfront Fusion]](../../workfront-fusion/errors/directives-for-error-handling.md)
* [의 고급 오류 처리 [!DNL Adobe Workfront Fusion]](../../workfront-fusion/errors/advanced-error-handling.md)