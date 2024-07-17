---
content-type: reference
product-previous: workfront-fusion
product-area: workfront-integrations
navigation-topic: errors
title: ' [!DNL Adobe Workfront Fusion]에서 처리하는 동안 오류 발생'
description: 시나리오를 실행하는 동안 오류가 발생하는 경우가 있습니다. 이 문제는 일반적으로 서비스에 연결하지 못해서 서비스를 사용할 수 없거나 유효성 검사가 실패하면 발생합니다. 이 문서에서는 일반적인 오류를 설명합니다.
author: Becky
feature: Workfront Fusion
exl-id: 468d7460-3853-4016-bff9-b9d3b87198ed
source-git-commit: a3756f9345cbc9417a6fd110306dfa50aecc81a2
workflow-type: tm+mt
source-wordcount: '1246'
ht-degree: 0%

---

# [!DNL Adobe Workfront Fusion]에서 처리하는 동안 오류 발생

시나리오를 실행하는 동안 오류가 발생하는 경우가 있습니다. 이 문제는 일반적으로 서비스에 연결하지 못해서 서비스를 사용할 수 없거나 유효성 검사가 실패하면 발생합니다. 이 문서에서는 일반적인 오류를 설명합니다.

[!DNL Adobe Workfront Fusion]은(는) 몇 가지 기본 오류 유형을 구별합니다. 발생한 오류 유형에 따라 다르게 반응합니다.

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

[!DNL Adobe Workfront Fusion] 라이선스에 대한 자세한 내용은 [[!DNL Adobe Workfront Fusion] 라이선스](../../workfront-fusion/get-started/license-automation-vs-integration.md)를 참조하세요.

## 연결 오류

`ConnectionError`

연결 오류는 다양한 이유(오버로드, 유지 관리, 중단 등)로 인해 서드파티 서비스를 사용할 수 없기 때문에 발생하는 가장 일반적인 오류 중 하나입니다. 이 오류의 기본 처리는 발생한 모듈에 따라 달라집니다.

* 첫 번째 모듈에서 오류가 발생하면 경고 메시지와 함께 시나리오 실행이 종료된다. 그런 다음 [!DNL Workfront Fusion]은(는) 시간 간격을 늘려 시나리오를 다시 실행하려고 반복적으로 시도합니다(아래에 설명). 모든 시도가 실패하면 [!DNL Workfront Fusion]은(는) 시나리오를 비활성화합니다.
* 첫 번째 모듈이 아닌 다른 모듈에서 연결 오류가 발생하는 경우 다음 단계는 시나리오 고급 설정의 [불완전한 실행 저장 허용](../../workfront-fusion/scenarios/scenario-settings-panel.md#allow) 옵션에 따라 다릅니다.

   * 이 옵션을 사용하면 시나리오 실행이 [!UICONTROL 불완전 실행] 폴더로 이동됩니다. [!DNL Workfront Fusion]은(는) 시간 간격을 늘려 시나리오를 다시 실행하려고 반복적으로 시도합니다. 모든 시도가 실패하면, 사용자의 수동 해결을 기다리는 미완료 실행 폴더에 실행이 유지됩니다.

     불완전한 실행에 대한 자세한 내용은 [불완전한 실행 보기 및 해결 [!DNL Adobe Workfront Fusion]](../../workfront-fusion/scenarios/view-and-resolve-incomplete-executions.md)을 참조하십시오.
   * 이 옵션이 비활성화되면 오류 발생 후 롤백 단계가 발생하여 시나리오 실행이 종료됩니다. 그런 다음 [!DNL Workfront Fusion]은(는) 시간 간격을 늘려 시나리오를 다시 실행하려고 반복적으로 시도합니다. 모든 시도가 실패하면 [!DNL Workfront Fusion]은(는) 시나리오를 비활성화합니다.

### 시간 간격 늘리기

오류가 발생할 때 시도 사이에 시간 간격을 곱하게 늘리는 알고리즘을 지수 백오프라고 한다. 증가하는 시간 간격은 다음과 같이 설정됩니다.

1. 10분
1. 1시간
1. 3시간
1. 12시간
1. 24시간

[!DNL Workfront Fusion]에서 늘어나는 시간 간격을 사용하는 주된 이유는 자주 실행되는 시나리오가 반복적으로 실패하는 시도에서 작업을 소모하는 것을 방지하기 위해서입니다.

>[!INFO]
>
>**예:**
>
>시나리오에 [!DNL Google Sheets] 트리거 [!UICONTROL 행 보기]가 포함되어 있습니다. [!DNL Workfront Fusion]이(가) 시나리오를 시작할 때 유지 관리로 인해 [!DNL Google Sheets]을(를) 30분 동안 사용할 수 없으므로 새 행을 검색할 수 없습니다. 시나리오가 중지되었다가 10분 후에 다시 시도합니다. [!DNL Google Sheets]을(를) 계속 사용할 수 없으므로 [!DNL Workfront Fusion]에서 새 행에 대한 정보를 가져올 수 없습니다. 다음 시나리오 실행이 1시간 후에 예약됩니다. [!DNL Google Sheets]을(를) 지금 다시 사용할 수 있으며 시나리오가 성공적으로 실행됩니다.

## 데이터 오류

`DataError`

항목이 잘못 매핑되어 사용 중인 서드파티 서비스의 [!DNL Workfront Fusion] 측이나 측에서 수행한 유효성 검사를 통과하지 못할 경우 데이터 오류가 발생합니다.

이 오류가 발생하면 모듈이 실패한 위치까지 시나리오가 문제를 해결할 수 있는 미완료 실행 폴더로 이동됩니다. 그러나 시나리오는 중지되지 않고 일정에 따라 계속 실행됩니다. 데이터 오류가 나타날 때 시나리오 실행을 중지하려면 시나리오 설정 패널에서 순차적 처리 옵션을 활성화합니다.

시나리오 설정에서 [!UICONTROL 불완전한 실행 저장 허용] 옵션을 활성화하지 않은 경우 오류가 발생하여 시나리오 실행이 종료되고 롤백이 수행됩니다.

매핑에 대한 자세한 내용은 [한 모듈에서 다른 모듈로 정보를 매핑 [!DNL Adobe Workfront Fusion]](../../workfront-fusion/mapping/map-information-between-modules.md)을 참조하십시오.

불완전한 실행에 대한 자세한 내용은 [Adobe Workfront Fusion에서 불완전한 실행 보기 및 해결](../../workfront-fusion/scenarios/view-and-resolve-incomplete-executions.md)을 참조하십시오.

시나리오 설정 패널에 대한 자세한 내용은 [Adobe Workfront Fusion의 시나리오 설정 패널](../../workfront-fusion/scenarios/scenario-settings-panel.md)을 참조하십시오.

일정에 대한 자세한 내용은 [Adobe Workfront Fusion에서 시나리오 예약](../../workfront-fusion/scenarios/schedule-a-scenario.md)을 참조하십시오.

## 중복 데이터 오류

`DuplicateDataError`

[!DNL Workfront Fusion]에서 중복 데이터를 허용하지 않는 서비스에 동일한 번들을 두 번 삽입하려고 하면 중복 데이터 오류가 생성됩니다. 이 오류가 발생하면 [!DNL Workfront Fusion]이(가) 데이터 오류와 같은 방식으로 진행됩니다.

## 잘못된 액세스 토큰 오류

`InvalidAccessTokenError`

[!DNL Workfront Fusion]이(가) 서드파티 서비스에 등록된 계정에 액세스할 수 없을 때 잘못된 액세스 토큰 오류가 발생합니다. 지정된 서비스의 관리에서 [!DNL Workfront Fusion]에 대한 액세스 권한을 취소하는 경우 일반적으로 이러한 문제가 발생하지만 관련 시나리오가 일정에 따라 계속 실행됩니다.

이 오류가 발생하면 시나리오 실행이 즉시 중지됩니다. 오류가 발생한 모듈에서 시작하는 나머지 시나리오는 불완전 실행 폴더로 이동됩니다.

불완전한 실행에 대한 자세한 내용은 [불완전한 실행 보기 및 해결 [!DNL Adobe Workfront Fusion]](../../workfront-fusion/scenarios/view-and-resolve-incomplete-executions.md)을 참조하십시오.

## 속도 제한 오류

`RateLimitError`

특정 서비스에서 설정한 제한을 초과하면 비율 제한 오류가 생성됩니다. 이 오류가 발생하면 [!DNL Workfront Fusion]이(가) 연결 오류와 같은 방식으로 진행됩니다.

자세한 내용은 [연결 오류](#connection-error)를 참조하십시오.

## 불완전한 데이터 오류

`IncompleteDataError`

불완전한 데이터 오류는 트리거에서만 발생합니다. 이 오류는 트리거가 지정된 서비스에서 필요한 데이터를 다운로드하지 못하는 경우 생성됩니다.

시나리오가 `IncompleteDataError`(으)로 종료되면 추가 동작은 [!UICONTROL 최대 연속 오류 수] 설정에 따라 달라집니다.

자세한 내용은 문서 [Adobe Workfront Fusion의 시나리오 설정 패널](../../workfront-fusion/scenarios/scenario-settings-panel.md)에서 [연속 오류 수](../../workfront-fusion/scenarios/scenario-settings-panel.md#number)를 참조하십시오.

>[!INFO]
>
>**예:**
>
>시나리오에서는 문서 확인을 위해 [!DNL Workfront] 트리거 [!UICONTROL 레코드 확인]을(를) 설정했습니다. 긴 비디오와 같은 큰 문서를 업로드하는 동안 시나리오가 실행됩니다. [!UICONTROL Workfront Fusion]이 Workfront에 업로드하는 동안 비디오를 다운로드하려고 시도하므로 시나리오는 `IncompleteDataError`과(와) 함께 종료됩니다.

## 실행 시간 오류

`RuntimeError`

시나리오 실행 중에 다른 오류(위에 언급되지 않음)가 나타나면 `RunTimeError`(으)로 보고됩니다.

시나리오가 `RuntimeError`(으)로 종료되면 추가 동작은 [!UICONTROL 최대 연속 오류 수] 설정에 따라 달라집니다. 자세한 내용은 문서 [Adobe Workfront Fusion의 시나리오 설정 패널](../../workfront-fusion/scenarios/scenario-settings-panel.md)에서 [연속 오류 수](../../workfront-fusion/scenarios/scenario-settings-panel.md#number)를 참조하십시오.

>[!NOTE]
>
>시나리오가 인스턴트 트리거로 시작하는 경우 [!UICONTROL 최대 연속 오류 수] 설정이 무시되고 첫 번째 오류가 발생하면 시나리오가 즉시 비활성화됩니다. 자세한 내용은 문서 [모듈 유형](../../workfront-fusion/modules/module-types.md)에서 [인스턴스 트리거](../../workfront-fusion/modules/module-types.md#instant)를 참조하십시오.

## 불일치 오류

`InconsistencyError`

커밋 또는 롤백 단계 중에 위에서 설명한 오류가 발생하면 일관성 없는 오류로 시나리오가 종료됩니다. 자세한 내용은  [!DNL Adobe Workfront Fusion]](../../workfront-fusion/scenarios/scenario-execution-cycles-phases.md)의 [시나리오 실행, 주기 및 단계를 참조하십시오.

이 오류가 시나리오에 표시되면 시나리오 실행이 즉시 중지됩니다.

## 경고

시나리오를 실행하는 동안 문제에 대해 알리는 경고가 표시될 수 있습니다. 그러나 시나리오가 성공적으로 완료되는 것을 막지는 않습니다.

예를 들어 최대 허용 파일 크기를 초과하고 [!UICONTROL 데이터 손실 사용] 옵션이 비활성화되면 경고가 나타날 수 있습니다. 자세한 내용은 문서 [Adobe Workfront Fusion의 시나리오 설정 패널](../../workfront-fusion/scenarios/scenario-settings-panel.md)에서 [데이터 손실 사용](../../workfront-fusion/scenarios/scenario-settings-panel.md#enable)을 참조하십시오.
