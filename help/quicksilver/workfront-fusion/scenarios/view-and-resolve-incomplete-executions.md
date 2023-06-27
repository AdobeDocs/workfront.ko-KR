---
product-previous: workfront-fusion
product-area: workfront-integrations
navigation-topic: scenarios
title: 에서 불완전한 실행 보기 및 해결 [!DNL Adobe Workfront Fusion]
description: 다음 [!UICONTROL 불완전한 실행] 오류로 인해 정상적으로 완료되지 않은 시나리오 실행이 폴더에 저장됩니다. 저장된 각 불완전한 실행은 수동 또는 자동으로 해결할 수 있습니다.
author: Becky
feature: Workfront Fusion
exl-id: 60fcda91-b725-4ada-a42c-5c05720d68c2
source-git-commit: 0915dcce45b271ee18cdd8af5db4f0eb01f3cced
workflow-type: tm+mt
source-wordcount: '626'
ht-degree: 0%

---

# 에서 불완전한 실행 보기 및 해결 [!DNL Adobe Workfront Fusion]

다음 [!UICONTROL 불완전한 실행] 오류로 인해 정상적으로 완료되지 않은 시나리오 실행이 폴더에 저장됩니다. 저장된 각 불완전한 실행은 수동 또는 자동으로 해결할 수 있습니다.

>[!NOTE]
>
>기본적으로 미완료 실행 저장은 비활성화되어 있습니다. 활성화하려면 [!UICONTROL 미완료 실행 저장 허용] 시나리오 고급 설정의 옵션입니다.
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
   <td role="rowheader">[!UICONTROL Adobe Workfront Fusion] 라이선스**</td> 
  <td>
   <p>현재 라이선스 요구 사항: 아니요 [!DNL Workfront Fusion] 라이센스 요구 사항.</p>
   <p>또는</p>
   <p>기존 라이선스 요구 사항: [!UICONTROL [!DNL Workfront Fusion] 작업 자동화 및 통합용], [!UICONTROL [!DNL Workfront Fusion] 작업 자동화용]</p>
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

## 미완료 실행 보기

작업 중 모듈에 오류가 발생하면 미완료 실행 폴더에 새로운 미완료 실행이 추가됩니다. 각 불완전한 실행에는 시나리오의 블루프린트와 실패한 모듈에 매핑할 수 있는 모든 번들이 포함됩니다. 미완료 실행 목록은 다음을 클릭하여 열 수 있습니다. [!UICONTROL 불완전한 실행] 시나리오 세부 정보 페이지의 탭은 다음과 같습니다.

![](assets/incomplete-executions-tab-350x102.png)

자세한 내용은 [불완전한 실행으로 이어지는 오류](#errors-resulting-into-incomplete-executions).

>[!NOTE]
>
>조직당 해결되지 않은 미완료 실행 폴더의 현재 크기 제한은 500MB입니다. 조직에서 이 제한을 초과하는 경우 다음 오류가 표시될 수 있습니다.
>
>`"There is NOT ENOUGH SPACE to add a bundle to the IEQ. The reason is: Too many incomplete executions."`
>
>자세한 내용은 [데이터 손실 활성화](../../workfront-fusion/scenarios/scenario-settings-panel.md#enable) 위치: [의 시나리오 설정 패널 [!DNL Adobe Workfront Fusion]](../../workfront-fusion/scenarios/scenario-settings-panel.md).

## 불완전한 실행 해결

새 미완료 실행이 저장되면 다음과 같이 해결할 수 있습니다.

1. 다음을 클릭합니다. **[!UICONTROL 불완전한 실행]** 탭.
1. 해결하려는 불완전한 실행을 찾아 을(를) 클릭합니다 **[!UICONTROL 세부 사항]**.


   불완전한 실행을 해결하기 전에 모든 모듈 작업의 로그를 보려면 [!UICONTROL 기록] 폴더:

1. 다음을 클릭합니다. **[!UICONTROL 기록]** 탭.
1. 실패한 시나리오의 실행 로그를 찾아 **[!UICONTROL 세부 사항]**.
1. 모든 모듈의 작업이 표시되는 모듈의 로그를 엽니다.
1. 실패한 작업을 찾은 다음 를 클릭합니다. **[!UICONTROL 해결]**:

   ![](assets/resolve-btn-350x188.png)

## 불완전한 실행과 관련된 옵션

의 다음 옵션 [!UICONTROL 시나리오 설정] 패널 미완료 실행이 저장되는지 여부 및 저장 방법을 결정합니다.

* 미완료 실행 저장 허용
* 순차적 처리
* 데이터 손실 활성화

이러한 옵션에 대한 자세한 내용은 [의 시나리오 설정 패널 [!DNL Adobe Workfront Fusion]](../../workfront-fusion/scenarios/scenario-settings-panel.md).

## 불완전한 실행으로 이어지는 오류

불완전한 실행을 저장하는 몇 가지 범주의 오류가 있습니다. 여기에는 다음이 포함될 수 있습니다.

* 주로 모듈을 통해 모든 데이터를 성공적으로 처리하기 위해 필요한 누락된 항목으로 인해 불완전하거나 잘못된 데이터에서 발생하는 유효성 검사 오류.
* 일시적 또는 장기간 연결 실패(예: 이메일 또는 원격 FTP 서버에 연결하는 중)로 인해 최종 대상을 사용할 수 없을 때 발생하는 오류.

시나리오의 첫 번째 모듈에 오류가 발생하면 실행이 즉시 중지되며 불완전한 실행은 저장되지 않습니다.

다른 모듈에서 오류가 발생하고 첨부된 오류 처리기 경로가 없으면 다음 중 하나가 발생합니다.

* 오류 유형이 다음과 같은 경우 `ConnectionError`, `RateLimitError`, `OutOfSpaceError` 또는 `ModuleTimeoutError`, 자동 재시도가 있는 불완전한 실행 레코드가 저장됩니다.
* 오류 유형이 다음과 같은 경우 `DataError`, `InvalidConfigurationError`, `InvalidAccessTokenError`, `UnexpectedError`, `MaxFileSizeExceededError`, 또는 `MaxResultsExceededError`, 자동 재시도가 없는 불완전한 실행 레코드가 저장됩니다.
* 오류 유형이 위의 유형 이외의 유형이면 실행이 실패합니다.
