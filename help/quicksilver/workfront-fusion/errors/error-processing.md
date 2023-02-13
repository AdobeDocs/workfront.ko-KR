---
content-type: reference
product-previous: workfront-fusion
product-area: workfront-integrations
navigation-topic: errors
title: 에서 처리 중 오류 발생 [!DNL Adobe Workfront Fusion]
description: 시나리오를 실행하는 동안 오류가 발생할 수 있습니다. 일반적으로 서비스에 연결하지 못했거나 유효성 검사에 실패하면 서비스를 사용할 수 없는 경우 발생합니다. 이 문서에서는 발생할 수 있는 일반적인 오류에 대해 설명합니다.
author: Becky
feature: Workfront Fusion
exl-id: 468d7460-3853-4016-bff9-b9d3b87198ed
source-git-commit: 97f91d663df86341a079894cff04d07c18b7bf08
workflow-type: tm+mt
source-wordcount: '1191'
ht-degree: 0%

---

# 에서 처리 중 오류 발생 [!DNL Adobe Workfront Fusion]

시나리오를 실행하는 동안 오류가 발생할 수 있습니다. 일반적으로 서비스에 연결하지 못했거나 유효성 검사에 실패하면 서비스를 사용할 수 없는 경우 발생합니다. 이 문서에서는 발생할 수 있는 일반적인 오류에 대해 설명합니다.

[!DNL Adobe Workfront Fusion] 몇 가지 기본 오류 유형을 구분합니다. 발생한 오류 유형에 따라 다르게 반응합니다.

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

## 연결 오류

`ConnectionError`

연결 오류는 다양한 이유(오버로드, 유지 관리, 중단 등)로 인해 타사 서비스를 사용할 수 없어서 발생하는 가장 일반적인 오류 중 하나입니다. 이 오류의 기본 처리는 발생한 모듈에 따라 달라집니다.

* 첫 번째 모듈에서 오류가 발생하면 시나리오의 실행이 경고 메시지로 종료됩니다. [!DNL Workfront Fusion] 그런 다음 시간 간격을 늘리면 시나리오를 다시 실행하려고 반복적으로 시도합니다(아래에 설명되어 있음). 모든 시도가 실패하면 [!DNL Workfront Fusion] 시나리오를 비활성화합니다.
* 첫 번째 모듈이 아닌 다른 모듈에서 연결 오류가 발생하는 경우 다음 단계는 [불완전한 실행 저장 허용](../../workfront-fusion/scenarios/scenario-settings-panel.md#allow) 시나리오 고급 설정의 옵션:

   * 이 옵션을 활성화하면 시나리오 실행이 [!UICONTROL 완료되지 않은 실행] 폴더 위치 [!DNL Workfront Fusion] 시간 간격이 증가하면 시나리오를 다시 실행하려고 반복적으로 시도합니다. 모든 시도가 실패하면 [에서 불완전한 실행 보기 및 해결 [!DNL Adobe Workfront Fusion]](../../workfront-fusion/scenarios/view-and-resolve-incomplete-executions.md) 사용자가 수동 확인을 기다리는 폴더입니다.
   * 이 옵션을 비활성화하면 시나리오 실행이 오류 후 롤백 단계로 끝납니다. [!DNL Workfront Fusion] 그런 다음 시간 간격을 늘리면 시나리오를 다시 실행하려고 반복해서 시도합니다. 모든 시도가 실패하면 [!DNL Workfront Fusion] 시나리오를 비활성화합니다.

### 시간 간격 증가

오류가 발생할 때 시도 간에 여러 번 증가하는 시간 간격을 지수 백오프라고 합니다. 증가하는 시간 간격은 다음과 같이 설정됩니다.

1. 10분
1. 1시간
1. 3시간
1. 12시간
1. 24시간

시간 간격을 사용하는 주된 이유 [!DNL Workfront Fusion] 자주 실행되는 시나리오가 반복적으로 실패한 시도에서 작업을 사용하지 않도록 하는 것입니다.

>[!INFO]
>
>**예:**
>
>시나리오에는 다음이 포함됩니다 [!DNL Google Sheets] 트리거 [!UICONTROL 보기 행]. [!DNL Google Sheets] 유지 관리로 인해 30분 동안 사용할 수 없습니다. [!DNL Workfront Fusion] 에서 시나리오를 시작하므로 새 행을 검색할 수 없습니다. 시나리오가 중단하고 10분 후에 다시 시도합니다. 이 기간 내에 서비스를 계속 사용할 수 없으므로 [!DNL Workfront Fusion] 새 행에 대한 정보를 가져올 수 없습니다. 시나리오의 다음 실행이 1시간 후에 예약됩니다. [!DNL Google Sheets] 이 시간 내에 다시 사용할 수 있으며 시나리오가 성공적으로 실행됩니다.

## 데이터 오류

`DataError`

항목이 잘못 매핑되고 에서 수행한 유효성 검사를 전달하지 않으면 데이터 오류가 생성됩니다 [!DNL Workfront Fusion] 사용 중인 타사 서비스의 측면에 있는 사이드 또는 입니다. 자세한 내용은 [의 한 모듈에서 다른 모듈로 정보 매핑 [!DNL Adobe Workfront Fusion]](../../workfront-fusion/mapping/map-information-between-modules.md).

이 오류가 발생하면 모듈이 실패한 최대 시나리오가 문제를 해결할 수 있는 불완전한 실행 폴더로 이동됩니다. 그러나 시나리오는 중지되지 않고 일정에 따라 계속 실행됩니다. 데이터 오류가 표시될 때 시나리오 실행을 중지하려면 시나리오 설정 패널에서 순차적 처리 옵션을 활성화합니다.

을 활성화하지 않은 경우 [!UICONTROL 불완전한 실행 저장 허용] 시나리오 설정에서 옵션은 오류가 발생하여 시나리오 실행이 종료되고 롤백이 수행됩니다.

불완전한 실행에 대한 자세한 내용은 [Adobe Workfront Fusion에서 불완전한 실행 보기 및 해결](../../workfront-fusion/scenarios/view-and-resolve-incomplete-executions.md).

시나리오 설정 패널에 대한 자세한 내용은 [Adobe Workfront Fusion의 시나리오 설정 패널](../../workfront-fusion/scenarios/scenario-settings-panel.md).

예약에 대한 자세한 내용은 [Adobe Workfront Fusion에서 시나리오 예약](../../workfront-fusion/scenarios/schedule-a-scenario.md).

## 중복 데이터 오류

`DuplicateDataError`

If [!DNL Workfront Fusion] 중복 데이터를 허용하지 않는 서비스에 동일한 번들을 두 번 삽입하려고 하면 중복 데이터 오류가 생성됩니다. 이 오류가 발생하면 [!DNL Workfront Fusion] 는 데이터 오류와 동일한 방식으로 진행됩니다.

## 잘못된 액세스 토큰 오류

`InvalidAccessTokenError`

다음 경우에 잘못된 액세스 토큰 오류가 발생합니다 [!DNL Workfront Fusion] 타사 서비스에 등록된 계정에 액세스할 수 없습니다. 이 문제는 주로 [!DNL Workfront Fusion] 지정된 서비스의 관리에서 하지만 관련 시나리오는 일정에 따라 계속 실행됩니다.

이 오류가 발생하면 시나리오의 실행이 즉시 중지됩니다. 오류가 발생한 모듈부터 시작하는 나머지 시나리오는 불완전한 실행 폴더로 이동됩니다.

불완전한 실행에 대한 자세한 내용은 [에서 불완전한 실행 보기 및 해결 [!DNL Adobe Workfront Fusion]](../../workfront-fusion/scenarios/view-and-resolve-incomplete-executions.md).

## 비율 제한 오류

`RateLimitError`

지정된 서비스에 의해 설정된 한도를 초과하면 비율 제한 오류가 생성됩니다. 이 오류가 발생하면 [!DNL Workfront Fusion] 는 연결 오류와 동일한 방식으로 진행됩니다. 자세한 내용은 [연결 오류](#connection-error).

## 불완전한 데이터 오류

`IncompleteDataError`

완료되지 않은 데이터 오류는 트리거로만 발생합니다. 이 오류는 트리거가 지정된 서비스에서 필수 데이터를 다운로드하지 못한 경우 생성됩니다.

시나리오 가 `IncompleteDataError`의 추가 동작은 [!UICONTROL 연속된 최대 오류 수]. 자세한 내용은 [연속 오류 수](../../workfront-fusion/scenarios/scenario-settings-panel.md#number) 기사 [Adobe Workfront Fusion의 시나리오 설정 패널](../../workfront-fusion/scenarios/scenario-settings-panel.md).

>[!INFO]
>
>**예:** 시나리오에는 [!DNL Workfront] 트리거 [!UICONTROL 감시 레코드] 문서를 감시하도록 설정합니다. 긴 비디오와 같이 큰 문서를 업로드하는 동안 시나리오가 실행됩니다. 왜냐면 [!UICONTROL Workfront Fusion] 는 여전히 Workfront에 업로드하는 동안 비디오를 다운로드하려고 하면 시나리오가 `IncompleteDataError`.

## 실행 시간 오류

`RuntimeError`

시나리오 실행 중에 다른 오류(위에 언급되지 않음)가 나타나면 으로 보고됩니다. `RunTimeError`.

시나리오 가 `RuntimeError`의 추가 동작은 [!UICONTROL 연속된 최대 오류 수]. 자세한 내용은 [연속 오류 수](../../workfront-fusion/scenarios/scenario-settings-panel.md#number) 기사 [Adobe Workfront Fusion의 시나리오 설정 패널](../../workfront-fusion/scenarios/scenario-settings-panel.md).

>[!NOTE]
>
>시나리오가 인스턴트 트리거로 시작하는 경우 [!UICONTROL 연속된 최대 오류 수] 가 무시되고 첫 번째 오류가 발생한 즉시 시나리오가 비활성화됩니다. 자세한 내용은 [인스턴트 트리거](../../workfront-fusion/modules/module-types.md#instant) 기사 [모듈 유형](../../workfront-fusion/modules/module-types.md).

## 불일치 오류

`InconsistencyError`

위에서 설명한 오류가 커밋 또는 롤백 단계 중에 발생하면 시나리오가 불일치로 종료됩니다. 자세한 내용은 [시나리오 실행, 주기 및 단계 [!DNL Adobe Workfront Fusion]](../../workfront-fusion/scenarios/scenario-execution-cycles-phases.md).

이 오류가 시나리오에 나타나면 시나리오 실행이 즉시 중지됩니다.

## 경고

시나리오를 실행하는 동안 문제에 대한 경고를 받을 수 있습니다. 그러나 시나리오가 성공적으로 완료되는 것을 방지할 수 없습니다.

예를 들어 허용되는 최대 파일 크기를 초과하고 [!UICONTROL 데이터 손실 활성화] 옵션이 비활성화되어 있습니다. 자세한 내용은 [데이터 손실 활성화](../../workfront-fusion/scenarios/scenario-settings-panel.md#enable) 기사 [Adobe Workfront Fusion의 시나리오 설정 패널](../../workfront-fusion/scenarios/scenario-settings-panel.md).
