---
content-type: reference
product-previous: workfront-fusion
product-area: workfront-integrations
navigation-topic: errors
title: 에서 오류 처리 중 [!DNL Adobe Workfront Fusion]
description: 시나리오 실행 중에 오류가 발생하면 일반적으로 오류로 인해 서비스를 사용할 수 없거나, 서비스가 예기치 않은 데이터로 응답하거나, 입력 데이터의 유효성 검사가 실패하기 때문입니다.
author: Becky
feature: Workfront Fusion
exl-id: a08c18a0-1797-4126-827a-1ea7e11d4bad
source-git-commit: e936bbd2837e4aec67d4136b8efcccb6f8454a89
workflow-type: tm+mt
source-wordcount: '572'
ht-degree: 0%

---

# 에서 오류 처리 중 [!DNL Adobe Workfront Fusion]

시나리오 실행 중에 오류가 발생하면 일반적으로 오류로 인해 서비스를 사용할 수 없거나, 서비스가 예기치 않은 데이터로 응답하거나, 입력 데이터의 유효성 검사가 실패하기 때문입니다.

시나리오 실행 중에 모듈에 오류가 발생하고 모듈에 연결된 오류 처리 경로가 없는 경우 기본 오류 처리 논리가 에 설명된 대로 실행됩니다. [에서 처리 중 오류 발생 [!DNL Adobe Workfront Fusion]](../../workfront-fusion/errors/error-processing.md).

모듈에 오류 처리기 경로를 추가하면 기본 오류 처리 논리를 직접 바꿀 수 있습니다. [!DNL Adobe Workfront Fusion] 에서는 오류 처리기 경로의 끝에 삽입할 수 있는 다섯 가지 다른 지시문을 제공합니다.

자세한 내용은 [에서 오류 처리를 위한 지시어 [!DNL Adobe Workfront Fusion]](../../workfront-fusion/errors/directives-for-error-handling.md).

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

## 오류 처리기 경로

모듈에 오류 처리기 경로를 추가하려면 다음을 수행합니다.

1. 모듈을 마우스 오른쪽 버튼으로 클릭하고 를 선택합니다 **[!UICONTROL 오류 처리기 추가]**:

   ![](assets/error-handler-route.png)

   이 모듈은 시나리오에 사용되는 앱과 지시어 목록을 보여줍니다.

1. 오류 핸들러를 추가한 모듈이 경로의 마지막 모듈인 경우 지시어 중 하나를 선택합니다.

   또는

   오류 처리기 경로에 하나 이상의 모듈을 추가합니다.

   경로에 모듈을 더 추가하면 [!UICONTROL 무시] 지시어는 기본적으로 적용되며, 오류가 발생하면 해당 경로의 후속 모듈이 처리됩니다.


>[!INFO]
>
>이 예제에서는 [!UICONTROL 폴더 만들기] 모듈, [!UICONTROL 무시] 지시어가 자동으로 적용되며 시나리오는 오류 처리기 경로의 다음 모듈로 이동합니다.
>
>그러나 오류가 없으면 시나리오가 [!UICONTROL 폴더 모듈에 있는 모든 파일 나열] 정차.
>
>![](assets/if-there-is-no-error-350x234.png)

오류 처리기 경로는 투명한 원으로 구성되고 일반 경로는 솔리드 원으로 구성됩니다.

## 지시 처리 오류

지침은 아래에 간략하게 설명되어 있습니다. 자세한 내용은 [에서 오류 처리를 위한 지시어 [!DNL Adobe Workfront Fusion]](../../workfront-fusion/errors/directives-for-error-handling.md).

시나리오 실행을 계속할지 여부를 기준으로 다음 카테고리로 그룹화할 수 있는 총 5개의 지시어가 있습니다.

다음 지시문은 시나리오 실행이 계속되도록 합니다.

* **[!UICONTROL 다시 시작]**: 오류가 있는 모듈의 대체 출력을 지정할 수 있습니다. 시나리오 실행 상태가 성공으로 표시됩니다
* **[!UICONTROL 무시]**: 은 오류를 무시합니다. 시나리오 실행 상태가 성공으로 표시됩니다
* **[!UICONTROL 브레이크]**: 불완전한 실행 큐에 입력을 저장합니다. 시나리오 실행 상태가 경고로 표시됩니다. 자세한 내용은 [에서 불완전한 실행 보기 및 해결 [!DNL Adobe Workfront Fusion]](../../workfront-fusion/scenarios/view-and-resolve-incomplete-executions.md).

오류가 발생할 때 시나리오 실행을 중지해야 하는 경우 다음 지시문 중 하나를 사용합니다.

* **[!UICONTROL 롤백]**: 시나리오 실행을 즉시 중단하고 상태를 오류로 표시합니다
* **[!UICONTROL 커밋]**: 시나리오 실행을 즉시 중단하고 상태를 성공으로 표시합니다

오류 처리에 대한 자세한 내용은 다음을 참조하십시오.

* [에서 오류 처리를 위한 지시어 [!DNL Adobe Workfront Fusion]](../../workfront-fusion/errors/directives-for-error-handling.md)
* [의 고급 오류 처리 [!DNL Adobe Workfront Fusion]](../../workfront-fusion/errors/advanced-error-handling.md)