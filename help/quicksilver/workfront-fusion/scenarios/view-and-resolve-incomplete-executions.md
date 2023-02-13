---
product-previous: workfront-fusion
product-area: workfront-integrations
navigation-topic: scenarios
title: 에서 불완전한 실행 보기 및 해결 [!DNL Adobe Workfront Fusion]
description: 다음 [!UICONTROL 완료되지 않은 실행] 폴더에는 오류로 인해 완료되지 않은 시나리오 실행이 저장됩니다. 저장된 각 불완전한 실행은 수동으로 또는 자동으로 해결될 수 있습니다.
author: Becky
feature: Workfront Fusion
exl-id: 60fcda91-b725-4ada-a42c-5c05720d68c2
source-git-commit: 59941ea1ce523a0d1036138a83f771b058049b34
workflow-type: tm+mt
source-wordcount: '578'
ht-degree: 0%

---

# 에서 불완전한 실행 보기 및 해결 [!DNL Adobe Workfront Fusion]

다음 [!UICONTROL 완료되지 않은 실행] 폴더에는 오류로 인해 완료되지 않은 시나리오 실행이 저장됩니다. 저장된 각 불완전한 실행은 수동으로 또는 자동으로 해결될 수 있습니다.

>[!NOTE]
>
>기본적으로 불완전한 실행 저장은 비활성화됩니다. 활성화하려면 [!UICONTROL 불완전한 실행 저장 허용] 시나리오 고급 설정의 옵션.
>
>시나리오 설정에 대한 자세한 내용은 [의 시나리오 설정 패널 [!DNL Adobe Workfront Fusion]](../../workfront-fusion/scenarios/scenario-settings-panel.md).

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
  <td> <p>[!UICONTROL [!DNL Workfront Fusion] 작업 자동화 및 통합을 위한] </p><p>[!UICONTROL [!DNL Workfront Fusion] 작업 자동화를 위한] </p>  </td>  
  </tr> 
  <tr> 
   <td role="rowheader">제품</td> 
   <td>조직이 구매해야 합니다 [!DNL Adobe Workfront Fusion] 뿐만 아니라 [!DNL Adobe Workfront] 을 참조하십시오.</td> 
  </tr> 
 </tbody> 
</table>

어떤 계획, 라이센스 유형 또는 액세스 권한을 보유하고 있는지 확인하려면 [!DNL Workfront] 관리자

에 대한 자세한 정보 [!DNL Adobe Workfront Fusion] 라이센스 [[!DNL Adobe Workfront Fusion] 라이선스](../../workfront-fusion/get-started/license-automation-vs-integration.md).

## 불완전한 실행 보기

모듈에 작동 중에 오류가 발생하면 새 불완전 실행이 불완전 실행 폴더에 추가됩니다. 완료되지 않은 각 실행에는 시나리오의 블루프린트와 실패한 모듈에 매핑할 수 있는 모든 번들이 포함되어 있습니다. 불완전한 실행 목록은 [!UICONTROL 완료되지 않은 실행] 시나리오 세부 사항 페이지의 탭:

![](assets/incomplete-executions-tab-350x102.png)

자세한 내용은 [불완전한 실행으로 이어지는 오류](#errors-resulting-into-incomplete-executions).

>[!NOTE]
>
>조직당 해결되지 않은 실행 폴더의 현재 크기 제한은 500MB입니다. 조직에서 이 제한을 초과하는 경우 다음 오류가 표시될 수 있습니다.
>
>`"There is NOT ENOUGH SPACE to add a bundle to the IEQ. The reason is: Too many incomplete executions."`
>
>자세한 내용은 [데이터 손실 활성화](../../workfront-fusion/scenarios/scenario-settings-panel.md#enable) in [의 시나리오 설정 패널 [!DNL Adobe Workfront Fusion]](../../workfront-fusion/scenarios/scenario-settings-panel.md).

## 불완전한 실행 해결

새로운 불완전한 실행이 저장되면 다음과 같이 해결할 수 있습니다.

1. 을(를) 클릭합니다. **[!UICONTROL 완료되지 않은 실행]** 탭.
1. 확인할 불완전한 실행을 찾아 를 클릭합니다 **[!UICONTROL 세부 사항]**.


   불완전한 실행을 해결하기 전에 모든 모듈 작업의 로그를 보려면 [!UICONTROL 기록] 폴더:

1. 을(를) 클릭합니다. **[!UICONTROL 기록]** 탭.
1. 시나리오의 실패한 실행 로그를 찾아 **[!UICONTROL 세부 사항]**.
1. 모듈의 모든 작업이 표시되는 모듈의 로그를 엽니다.
1. 실패한 작업을 찾아 를 클릭합니다. **[!UICONTROL 해결]**:

   ![](assets/resolve-btn-350x188.png)

## 불완전한 실행과 관련된 옵션

다음 옵션은 [!UICONTROL 시나리오 설정] 패널에서는 불완전한 실행의 저장 여부 및 방법을 결정합니다.

* 불완전한 실행 저장 허용
* 순차적 처리
* 데이터 손실 활성화

이러한 옵션에 대한 자세한 내용은 [의 시나리오 설정 패널 [!DNL Adobe Workfront Fusion]](../../workfront-fusion/scenarios/scenario-settings-panel.md).

## 불완전한 실행으로 이어지는 오류

불완전한 실행을 저장하는 오류의 범주가 몇 가지 있습니다. 여기에는 다음이 포함될 수 있습니다.

* 모듈을 통해 이동하는 모든 데이터를 성공적으로 처리하기 위해 필요한 항목이 누락되어 불완전하거나 잘못된 데이터에서 발생하는 유효성 검사 오류
* 임시 또는 장기 연결 오류로 인해 최종 대상을 사용할 수 없는 경우(예: 이메일 또는 원격 FTP 서버에 연결하는 동안) 오류가 발생합니다.

시나리오의 첫 번째 모듈에서 오류가 발생하면 실행이 즉시 중지되고 불완전한 실행이 저장되지 않습니다.

다른 모듈에서 오류가 발생하여 연결된 오류 처리기 경로가 없는 경우 다음 중 하나가 발생합니다.

* 오류 유형이 `ConnectionError`, `RateLimitError`, `OutOfSpaceError` 또는 `ModuleTimeoutError`를 입력하면 자동 재시도가 포함된 불완전한 실행 레코드가 저장됩니다.
* 오류 유형이 `DataError`, `InvalidConfigurationError`, `InvalidAccessTokenError`, `UnexpectedError`, `MaxFileSizeExceededError`, 또는 `MaxResultsExceededError`: 자동 다시 시도가 없는 불완전한 실행 레코드가 저장됩니다.
* 오류 유형이 위 이외의 다른 경우 실행이 실패합니다.
