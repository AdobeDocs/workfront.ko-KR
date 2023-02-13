---
content-type: reference
product-previous: workfront-fusion
product-area: workfront-integrations
navigation-topic: errors
title: Adobe Workfront Fusion에서 오류 처리 실행
description: 경우에 따라 시나리오 실행을 강제로 중지하거나 롤백 또는 커밋 단계를 수행하여 라우트의 처리를 중지하고 선택적으로 [보기] 큐에 저장하고 Adobe Workfront Fusion의 불완전한 실행을 해결할 수 있습니다.
author: Becky
feature: Workfront Fusion
exl-id: 6258bd4d-31a0-4fbb-b1b4-8e9a5a9dbe36
source-git-commit: c57a796ccbfb36bce58d49345e7515dd524604c5
workflow-type: tm+mt
source-wordcount: '340'
ht-degree: 0%

---

# 에서 오류 처리 실행 [!DNL Adobe Workfront Fusion]

경우에 따라 시나리오 실행을 강제로 중지하고 다음에 [롤백](../../workfront-fusion/scenarios/scenario-execution-cycles-phases.md#rollback) 또는 [커밋](../../workfront-fusion/scenarios/scenario-execution-cycles-phases.md#commit) 단계 또는 경로 처리를 중지하고 필요에 따라 불완전한 실행 대기열에 저장합니다.

현재 오류 처리 지시문은 [오류 처리기 경로](../../workfront-fusion/errors/error-handling.md#error) 및 [!DNL Adobe Workfront Fusion] 은 조건부로 쉽게 오류를 생성(throw)할 수 있는 모듈을 제공하지 않습니다.

불완전한 실행에 대한 자세한 내용은 [Adobe Workfront Fusion에서 불완전한 실행 보기 및 해결](../../workfront-fusion/scenarios/view-and-resolve-incomplete-executions.md).

오류 처리 지시어에 대한 자세한 내용은 [에서 오류 처리를 위한 지시어 [!DNL Adobe Workfront Fusion]](../../workfront-fusion/errors/directives-for-error-handling.md).

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

에 대한 자세한 정보 [!DNL Adobe Workfront Fusion] 라이센스 [[!DNL Adobe Workfront Fusion licenses]](../../workfront-fusion/get-started/license-automation-vs-integration.md)

## Throw에 대한 해결 방법

조건부로 오류를 throw하려면 해당 작업 중에 선택적으로 오류가 발생하도록 모듈을 구성할 수 있습니다. 한가지 가능성은 [!UICONTROL JSON] > [!UICONTROL JSON 구문 분석] 모듈(참조) [JSON 모듈](../../workfront-fusion/apps-and-their-modules/json-modules.md)), 선택적으로 오류를 발생하도록 구성된 경우(이 경우 BundleValidationError):

그런 다음 오류 처리 지시문 중 하나를 오류 처리 경로에 첨부할 수 있습니다.

* 시나리오 실행을 중지하고 롤백 단계를 수행하도록 합니다. [!UICONTROL 롤백]
* 시나리오 실행을 중지하고 커밋 단계를 수행하도록 합니다. [!UICONTROL 커밋]
* 경로 처리를 중지합니다. [!UICONTROL 무시]
* 경로 처리를 중지하고 불완전한 실행 폴더에 저장합니다. [!UICONTROL 브레이크]

다음 예제는 [!DNL Rollback] 지시문:

![](assets/rollback-directive-350x175.png)
