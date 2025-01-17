---
content-type: reference
product-previous: workfront-fusion
product-area: workfront-integrations
navigation-topic: errors
title: Adobe Workfront Fusion에서 오류 처리 실행
description: Adobe Workfront Fusion 설명서가 새 위치로 이동했습니다. 이 문서는 더 이상 사용되지 않지만, 이 기능을 다루는 새 문서에 대한 링크를 포함합니다.
author: Becky
feature: Workfront Fusion
exl-id: 6258bd4d-31a0-4fbb-b1b4-8e9a5a9dbe36
source-git-commit: 2d6af8b4988bd9aab7381daa79dec79e41408c45
workflow-type: tm+mt
source-wordcount: '415'
ht-degree: 0%

---

# [!DNL Adobe Workfront Fusion]에서 Throw 오류 처리

>[!IMPORTANT]
>
>Adobe Workfront Fusion 설명서가 새 위치로 이동했습니다.
>
>이 문서의 정보는 이제 문서에서 찾을 수 있습니다.
>
>* [구성 `throw` 오류 해결](https://experienceleague.adobe.com/docs/workfront-fusion/using/create-scenarios/configure-error-handling/throw.html)
>
>모든 책갈피를 업데이트하십시오.
>
>이 문서는 더 이상 업데이트되지 않으며 곧 제거될 예정입니다.

경우에 따라 시나리오 실행 후 [롤백](../../workfront-fusion/scenarios/scenario-execution-cycles-phases.md#rollback) 또는 [커밋](../../workfront-fusion/scenarios/scenario-execution-cycles-phases.md#commit) 단계를 강제로 중지하거나 경로 처리를 중단하고 선택적으로 불완전한 실행 큐에 저장할 수 있습니다.

현재 오류 처리 지시문은 [오류 처리기 경로](../../workfront-fusion/errors/error-handling.md#error)의 범위에서 사용할 수 없으며, [!DNL Adobe Workfront Fusion]에서는 오류를 쉽게 조건부 생성(throw)할 수 있는 모듈을 제공하지 않습니다.

불완전한 실행에 대한 자세한 내용은 [Adobe Workfront Fusion에서 불완전한 실행 보기 및 해결](../../workfront-fusion/scenarios/view-and-resolve-incomplete-executions.md)을 참조하십시오.

오류 처리 지시문에 대한 자세한 내용은  [!DNL Adobe Workfront Fusion]](../../workfront-fusion/errors/directives-for-error-handling.md)의 오류 처리에 대한 [지시문을 참조하십시오.

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

[!DNL Adobe Workfront Fusion] 라이선스에 대한 자세한 내용은 [[!DNL Adobe Workfront Fusion licenses]](../../workfront-fusion/get-started/license-automation-vs-integration.md)을(를) 참조하세요.

## Throw에 대한 해결 방법

오류를 조건부로 throw하려면 작업 중에 선택적으로 실패할 수 있도록 모듈을 구성할 수 있습니다. 한 가지 가능성은 선택적으로 오류를 발생시키도록 구성된 [!UICONTROL JSON] > [!UICONTROL JSON 구문 분석] 모듈([JSON 모듈](../../workfront-fusion/apps-and-their-modules/json-modules.md) 참조)을 사용하는 것입니다(이 경우 BundleValidationError).

그런 다음 오류 처리 지시문 중 하나를 다음 오류 처리 경로에 첨부할 수 있습니다.

* 시나리오 실행을 중지하고 롤백 단계를 수행합니다. [!UICONTROL 롤백]
* 시나리오 실행을 중지하고 커밋 단계를 수행하도록 합니다. [!UICONTROL 커밋]
* 경로 처리를 중지합니다. [!UICONTROL 무시]
* 경로 처리를 중지하고 미완료 실행 큐 폴더에 저장합니다. [!UICONTROL 중단]

다음 예제에서는 [!DNL Rollback] 지시문을 사용하는 방법을 보여 줍니다.

![](assets/rollback-directive-350x175.png)
