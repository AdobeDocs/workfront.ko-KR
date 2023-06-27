---
content-type: reference
product-previous: workfront-fusion
product-area: workfront-integrations
navigation-topic: errors
title: Adobe Workfront Fusion에서 오류 처리 실행
description: 롤백 또는 커밋 단계 다음에 나오는 시나리오 실행을 강제로 중지하거나 경로 처리를 중단하고 필요한 경우 보기 큐에 저장한 다음 Adobe Workfront Fusion에서 불완전한 실행을 해결할 수 있습니다.
author: Becky
feature: Workfront Fusion
exl-id: 6258bd4d-31a0-4fbb-b1b4-8e9a5a9dbe36
source-git-commit: a3756f9345cbc9417a6fd110306dfa50aecc81a2
workflow-type: tm+mt
source-wordcount: '384'
ht-degree: 0%

---

# 에서 오류 처리 실행 [!DNL Adobe Workfront Fusion]

경우에 따라 다음에 오는 시나리오 실행을 강제로 중지할 수 있습니다. [롤백](../../workfront-fusion/scenarios/scenario-execution-cycles-phases.md#rollback) 또는 [커밋](../../workfront-fusion/scenarios/scenario-execution-cycles-phases.md#commit) 단계 또는 경로 처리를 중단하고 선택적으로 불완전한 실행 큐에 저장합니다.

현재 오류 처리 지시문은 의 범위에서 사용할 수 없습니다. [오류 처리기 경로](../../workfront-fusion/errors/error-handling.md#error) 및 [!DNL Adobe Workfront Fusion] 는 쉽게 오류를 조건부로 생성 (throw)할 수 있는 모듈을 제공하지 않습니다.

불완전한 실행에 대한 자세한 내용은 [Adobe Workfront Fusion의 불완전한 실행 보기 및 해결](../../workfront-fusion/scenarios/view-and-resolve-incomplete-executions.md).

오류 처리 지시문에 대한 자세한 내용은 [에서 오류 처리를 위한 지시문 [!DNL Adobe Workfront Fusion]](../../workfront-fusion/errors/directives-for-error-handling.md).

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

다음에 대한 정보: [!DNL Adobe Workfront Fusion] 라이센스, 참조 [[!DNL Adobe Workfront Fusion licenses]](../../workfront-fusion/get-started/license-automation-vs-integration.md)

## Throw에 대한 해결 방법

오류를 조건부로 throw하려면 작업 중에 선택적으로 실패할 수 있도록 모듈을 구성할 수 있습니다. 한 가지 가능성은 [!UICONTROL JSON] > [!UICONTROL JSON 구문 분석] 모듈(참조) [JSON 모듈](../../workfront-fusion/apps-and-their-modules/json-modules.md)), 선택적으로 오류를 발생시키도록 구성됩니다(이 경우 BundleValidationError).

그런 다음 오류 처리 지시문 중 하나를 다음 오류 처리 경로에 첨부할 수 있습니다.

* 시나리오 실행을 중지하고 롤백 단계를 수행합니다. [!UICONTROL 롤백]
* 시나리오 실행을 중지하고 커밋 단계를 강제 수행합니다. [!UICONTROL 커밋]
* 경로 처리를 중지합니다. [!UICONTROL 무시]
* 경로 처리를 중지하고 미완료 실행 대기열 폴더에 저장합니다. [!UICONTROL 나누기]

다음 예는 의 사용을 보여줍니다. [!DNL Rollback] 지시문:

![](assets/rollback-directive-350x175.png)
