---
product-previous: workfront-fusion
product-area: workfront-integrations
navigation-topic: scenarios
title: ' [!DNL Adobe Workfront Fusion]에서 불완전한 실행 보기 및 해결'
description: Adobe Workfront Fusion 설명서가 새 위치로 이동했습니다. 이 문서는 더 이상 사용되지 않지만, 이 기능을 다루는 새 문서에 대한 링크를 포함합니다.
author: Becky
feature: Workfront Fusion
exl-id: 60fcda91-b725-4ada-a42c-5c05720d68c2
source-git-commit: 2d6af8b4988bd9aab7381daa79dec79e41408c45
workflow-type: tm+mt
source-wordcount: '675'
ht-degree: 5%

---

# [!DNL Adobe Workfront Fusion]에서 불완전한 실행 보기 및 해결

>[!IMPORTANT]
>
>Adobe Workfront Fusion 설명서가 새 위치로 이동했습니다.
>
>이 문서의 정보는 이제 문서에서 찾을 수 있습니다.
>
>* [불완전한 실행 보기 및 해결](https://experienceleague.adobe.com/docs/workfront-fusion/using/manage-scenarios/view-and-resolve-incomplete-executions.html)
>
>모든 책갈피를 업데이트하십시오.
>
>이 문서는 더 이상 업데이트되지 않으며 곧 제거될 예정입니다.

[!UICONTROL 미완료 실행] 폴더는 오류로 인해 정상적으로 완료되지 않은 시나리오 실행을 저장합니다. 저장된 각 불완전한 실행은 수동 또는 자동으로 해결할 수 있습니다.

>[!NOTE]
>
>기본적으로 미완료 실행 저장은 비활성화되어 있습니다. 활성화하려면 시나리오 고급 설정에서 [!UICONTROL 불완전한 실행 저장 허용] 옵션을 활성화하십시오.
>
>시나리오 설정에 대한 자세한 내용은  [!DNL Adobe Workfront Fusion]](../../workfront-fusion/scenarios/scenario-settings-panel.md)의 [시나리오 설정 패널을 참조하십시오.

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
   <p>레거시 라이선스 요구 사항: 작업 자동화 및 통합의 경우 [!UICONTROL [!DNL Workfront Fusion], 작업 자동화의 경우 [!UICONTROL [!DNL Workfront Fusion]]</p>
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

## 미완료 실행 보기

작업 중 모듈에 오류가 발생하면 미완료 실행 폴더에 새로운 미완료 실행이 추가됩니다. 각 불완전한 실행에는 시나리오의 블루프린트와 실패한 모듈에 매핑할 수 있는 모든 번들이 포함됩니다. 시나리오 세부 정보 페이지에서 [!UICONTROL 불완전 실행] 탭을 클릭하여 불완전 실행 목록을 열 수 있습니다.

<!--

![](assets/incomplete-executions-tab-350x102.png)

-->

자세한 내용은 [불완전한 실행으로 인한 오류](#errors-resulting-into-incomplete-executions)를 참조하십시오.

>[!NOTE]
>
>조직당 해결되지 않은 미완료 실행 폴더의 현재 크기 제한은 500MB입니다. 조직에서 이 제한을 초과하는 경우 다음 오류가 표시될 수 있습니다.
>
>`"There is NOT ENOUGH SPACE to add a bundle to the IEQ. The reason is: Too many incomplete executions."`
>
>자세한 내용은 [시나리오 설정 패널 [!DNL Adobe Workfront Fusion]](../../workfront-fusion/scenarios/scenario-settings-panel.md)의 [데이터 손실 사용](../../workfront-fusion/scenarios/scenario-settings-panel.md#enable)을 참조하세요.

## 불완전한 실행 해결

새 미완료 실행이 저장되면 다음과 같이 해결할 수 있습니다.

1. **[!UICONTROL 미완료 실행]** 탭을 클릭합니다.
1. 해결할 불완전한 실행을 찾은 다음 **[!UICONTROL 세부 정보]**&#x200B;을(를) 클릭합니다.


   불완전한 실행을 해결하기 전에 모든 모듈의 작업 로그를 보려면 [!UICONTROL History] 폴더에서 불완전한 실행을 해결할 수 있습니다.

1. **[!UICONTROL 기록]** 탭을 클릭합니다.
1. 실패한 시나리오의 실행 로그를 찾아 **[!UICONTROL 세부 정보]**&#x200B;를 클릭합니다.
1. 모든 모듈의 작업이 표시되는 모듈의 로그를 엽니다.
1. 실패한 작업을 찾은 다음 **[!UICONTROL 해결]**&#x200B;을 클릭합니다.

   ![](assets/resolve-btn-350x188.png)

## 불완전한 실행과 관련된 옵션

[!UICONTROL 시나리오 설정] 패널의 다음 옵션에 따라 불완전한 실행의 저장 여부와 저장 방법이 결정됩니다.

* 미완료 실행 저장 허용
* 순차적 처리
* 데이터 손실 활성화

이러한 옵션에 대한 자세한 내용은 [시나리오 설정 패널 [!DNL Adobe Workfront Fusion]](../../workfront-fusion/scenarios/scenario-settings-panel.md)을 참조하세요.

## 불완전한 실행으로 이어지는 오류

불완전한 실행을 저장하는 몇 가지 범주의 오류가 있습니다. 여기에는 다음이 포함될 수 있습니다.

* 주로 모듈을 통해 모든 데이터를 성공적으로 처리하기 위해 예상되는 누락된 항목 때문에 불완전하거나 잘못된 데이터로 인해 발생하는 유효성 검사 오류.
* 일시적 또는 장기간 연결 실패(예: 이메일 또는 원격 FTP 서버에 연결하는 중)로 인해 최종 대상을 사용할 수 없을 때 발생하는 오류.

시나리오의 첫 번째 모듈에서 오류가 발생하면 실행이 즉시 중지되고 불완전한 실행은 저장되지 않습니다.

다른 모듈에서 오류가 발생하고 첨부된 오류 처리기 경로가 없으면 다음 중 하나가 발생합니다.

* 오류 유형이 `ConnectionError`, `RateLimitError`, `OutOfSpaceError` 또는 `ModuleTimeoutError`인 경우 자동 다시 시도와 함께 불완전한 실행 레코드가 저장됩니다.
* 오류 유형이 `DataError`, `InvalidConfigurationError`, `InvalidAccessTokenError`, `UnexpectedError`, `MaxFileSizeExceededError` 또는 `MaxResultsExceededError`인 경우 자동 다시 시도 없이 불완전한 실행 레코드가 저장됩니다.
* 오류 유형이 위와 다른 경우 실행이 실패합니다.
