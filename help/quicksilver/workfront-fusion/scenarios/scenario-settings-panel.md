---
product-previous: workfront-fusion
product-area: workfront-integrations
navigation-topic: scenarios
title: Adobe Workfront Fusion의 시나리오 설정 패널
description: 이 문서에서는  [!DNL Adobe Workfront Fusion] 시나리오의 [!UICONTROL 시나리오 설정] 패널에서 사용할 수 있는 설정에 대해 설명합니다.
author: Becky
feature: Workfront Fusion
exl-id: 64a7a39a-f450-4eba-b4db-f31dd22aefdc
source-git-commit: b9914daa1e176d115226019d6ddf02b0953bc4d6
workflow-type: tm+mt
source-wordcount: '1206'
ht-degree: 0%

---

# [!DNL Adobe Workfront Fusion]의 시나리오 설정 패널

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

## 시나리오 설정을 엽니다.

1. [시나리오 편집기  [!DNL Adobe Workfront Fusion]](../../workfront-fusion/scenarios/scenario-editor.md)에 설명된 대로 시나리오 편집기를 엽니다.
1. 페이지의 왼쪽 아래 모서리 근처에 있는 톱니바퀴 아이콘을 클릭합니다.

   ![](assets/scenario-settings-350x221.png)

   표시되는 [!UICONTROL 시나리오 설정] 패널에서 시나리오에 대한 다양한 고급 설정을 구성할 수 있습니다.

## [!UICONTROL 불완전한 실행 저장 허용]

이 옵션은 시나리오를 실행하는 동안 오류가 발생하는 경우 [!DNL Adobe Workfront Fusion]의 진행 방식을 결정합니다. 이 옵션을 사용하면 시나리오가 일시 중지되고 [다음 위치에서 불완전한 실행 보기 및 해결 [!DNL Adobe Workfront Fusion]](../../workfront-fusion/scenarios/view-and-resolve-incomplete-executions.md)로 이동됩니다. 이렇게 하면 문제를 해결하고 시나리오가 중지된 위치에서 계속 실행할 수 있습니다. 이 옵션이 비활성화되면 시나리오 실행이 중지되고 롤백 단계가 시작됩니다.

## [!UICONTROL 순차적 처리]

이 옵션은 모든 실행을 순서대로 수행하도록 하며 주로 웹후크 및 미완료 실행과 관련이 있습니다.

순차적 처리가 활성화된 경우 시나리오의 병렬 실행이 비활성화됩니다.

### 즉시 웹훅

웹후크 트리거가 `instant`(으)로 구성되어 있고 &quot;순차적 처리&quot;가 활성화된 경우 모든 즉시 웹후크 페이로드는 대기열에 추가되고 도착하는 순서대로 처리됩니다. 이 기능은 외부 시스템의 이벤트를 정확한 순서로 처리할 때 유용할 수 있습니다.

>[!NOTE]
>
>다음 페이로드가 시작되기 전에 각 페이로드가 처리되므로 자동 처리가 지연됩니다.

### 불완전한 실행

&quot;미완료 실행&quot;도 활성화된 경우 시나리오를 실행하는 동안 오류가 발생하면 시나리오가 일시 중지됩니다. 그런 다음 다음 다음 중 하나가 발생합니다.

* 순차적 처리 옵션이 **활성화됨**&#x200B;인 경우, Workfront Fusion은 모든 불완전한 실행이 해결될 때까지 기존 시퀀스의 처리를 중지합니다.
* 순차적 처리 옵션이 **사용 안 함**&#x200B;인 경우, 시나리오는 불완전한 실행을 다시 실행하려고 반복적으로 시도하면서 일정에 따라 계속 실행됩니다.

불완전한 실행에 대한 자세한 내용은 [Adobe Workfront Fusion에서 불완전한 실행 보기 및 해결](/help/quicksilver/workfront-fusion/scenarios/view-and-resolve-incomplete-executions.md)을 참조하십시오.

<!--

This option determines how [!DNL Workfront Fusion] proceeds if an error occurs and the execution of a scenario is moved to the [View and resolve incomplete executions in [!DNL Adobe Workfront Fusion]](../../workfront-fusion/scenarios/view-and-resolve-incomplete-executions.md). If the [!UICONTROL Sequential processing] option is enabled, Workfront Fusion stops processing the task sequence altogether until all incomplete executions are resolved. If the [!UICONTROL Sequential processing] option is disabled, the scenario continues to run according to its schedule, accompanied by repeated attempts to rerun the incomplete executions.-->

>[!NOTE]
>
>순차적 처리는 시나리오 실행에 지연을 발생시킬 수 있다. 인스턴스 시나리오가 트리거되거나 예약된 시나리오가 실행되도록 설정된 경우 큐에 미완료 실행이 있는 경우 해당 시나리오는 큐에서 모든 실행이 완료되기 전에 실행됩니다.
>
>시나리오의 사용 사례에 순차적 처리가 필요하지 않은 경우 순차적 처리 옵션을 비활성화하는 것이 좋습니다.

예약에 대한 자세한 내용은 [다음 위치에서 시나리오 예약 [!DNL Adobe Workfront Fusion]](../../workfront-fusion/scenarios/schedule-a-scenario.md)을 참조하세요.

## 데이터는 기밀입니다

시나리오가 실행되면 기본적으로 시나리오의 모듈에서 처리된 데이터에 대한 정보를 표시할 수 있습니다. 이 정보를 저장하지 않으려면 [!UICONTROL Data is confidential] 옵션을 사용하도록 설정하십시오.

정보 표시에 대한 자세한 내용은 [시나리오 실행 흐름  [!DNL Adobe Workfront Fusion]](../../workfront-fusion/scenarios/scenario-execution-flow.md)을(를) 참조하십시오.

>[!IMPORTANT]
>
>이 옵션을 활성화하면 시나리오 실행 중에 발생할 수 있는 오류를 해결하기 어려울 수 있습니다.

## 데이터 손실 활성화

이 옵션은 [!DNL Workfront Fusion]이(가) [보기 및  [!DNL Adobe Workfront Fusion]](../../workfront-fusion/scenarios/view-and-resolve-incomplete-executions.md)의 불완전한 실행 확인 큐에 번들을 저장하지 못하는 경우(예: 사용 가능한 공간이 부족하기 때문에) 데이터 손실을 사용하도록 설정하는 것과 관련이 있습니다. 이 옵션을 활성화하면 전체 시나리오 실행에서 중단이 발생하지 않도록 데이터가 손실됩니다. 이 기능은 가장 높은 우선 순위가 연속 실행이고 들어오는 잘못된 데이터가 그다지 중요하지 않은 시나리오에 유용합니다.

그 외에도 시나리오를 실행할 때 모듈에서 최대 허용 크기보다 큰 파일이 발생할 수 있습니다. 이 경우 [!DNL Workfront Fusion]은(는) [!UICONTROL 데이터 손실 사용] 옵션의 설정에 따라 진행되며 경고 메시지가 표시됩니다.

최대 파일 크기에 대한 자세한 내용은 [매핑 파일 정보 [!DNL Adobe Workfront Fusion]](../../workfront-fusion/mapping/about-mapping-files.md)를 참조하십시오.

경고에 대한 자세한 내용은 [다음 위치에서 오류 처리 [!DNL Adobe Workfront Fusion]](../../workfront-fusion/errors/error-processing.md)를 참조하십시오.

## [!UICONTROL 자동 커밋]

[!UICONTROL 자동 커밋] 설정은 트랜잭션에 적용되며 시나리오를 처리하는 방법을 정의합니다. 자동 커밋 옵션이 켜져 있으면 각 모듈의 커밋 단계는 작업 단계를 완료한 후 즉시 시작됩니다. 자동 커밋 옵션이 비활성화되면 모든 모듈에 대해 작업이 실행될 때까지 커밋이 발생하지 않습니다(기본 모드).

트랜잭션에 대한 자세한 내용은 [시나리오 실행, 주기 및 단계  [!DNL Adobe Workfront Fusion]](../../workfront-fusion/scenarios/scenario-execution-cycles-phases.md)을(를) 참조하십시오.

## 최대 주기 수

주기를 더 설정하면 서드파티 서비스에 대한 연결 중단을 방지하고 모든 레코드가 하나의 시나리오 실행 내에서 처리되도록 하려는 경우 유용할 수 있습니다.

* 시나리오가 폴링 트리거로 시작하는 경우 설정은 시나리오 실행 중에 허용된 최대 주기 수를 정의합니다.

  폴링 트리거에 대한 자세한 내용은 [모듈 유형](../../workfront-fusion/modules/module-types.md)의 [폴링 트리거](../../workfront-fusion/modules/module-types.md#polling)를 참조하십시오.

* 시나리오가 인스턴트 트리거로 시작되면 설정이 무시되고 보류 중인 모든 이벤트가 한 사이클당 하나의 이벤트씩 단일 시나리오 실행 중에 처리됩니다.

  인스턴트 트리거에 대한 자세한 내용은 [모듈 유형](../../workfront-fusion/modules/module-types.md)의 [인스턴트 트리거](../../workfront-fusion/modules/module-types.md#instant)를 참조하십시오.

* 시나리오가 트리거로 시작되지 않는 경우(인스턴스/폴링) 지정된 최대 사이클 수가 항상 수행됩니다.

>[!INFO]
>
>**예:** [!DNL Workfront] > [!UICONTROL 레코드 보기]에서 들어오는 새로운 문제를 감시하고 [!DNL Workfront] >[!UICONTROL 개체 변환]에서 새 요청을 프로젝트로 변환하고 적절한 템플릿을 할당합니다.
>
>![](assets/scenario-settings-ex-1-350x157.png)
>
>시나리오 실행을 예약하는 경우에만 [!UICONTROL 주기 더] 설정이 적용됩니다. [!UICONTROL 한 번 실행] 단추를 사용하면 주기 설정이 고려됩니다.
>
>### 최대 주기 수가 1(기본값)로 설정됩니다.
>
>![](assets/max-number-cycles-1-350x201.png)
>
>[!UICONTROL Workfront] >[!UICONTROL 레코드 보기] 모듈에서 [!UICONTROL 반환된 최대 파일 수]이(가) `10`(으)로 설정되었습니다.
>100개의 요청이 [!DNL Workfront]에 제출되고 [!UICONTROL Limit] 필드가 10으로 설정된 경우 시나리오 실행 후 90개의 파일이 처리되지 않은 상태로 남습니다. 다음 10개의 파일이 다음에 예약된 시나리오 실행에서 처리됩니다.
>
>### 최대 주기 수는 10으로 설정됩니다.
>
>[!UICONTROL Dropbox] >[!UICONTROL 파일 보기] 모듈의 [!UICONTROL 최대 반환 파일 수]이(가) `10`(으)로 설정되어 있습니다.
>
>Dropbox 폴더에 100개의 파일이 추가되고 [!UICONTROL 최대 반환 파일 수] 옵션이 10으로 설정된 경우 모든 파일이 처리될 때까지 첫 번째 주기 동안 10개의 파일이 처리되고, 두 번째 주기 동안 다음 10개의 파일이 처리되고, 세 번째 주기 동안 다음 10개의 파일이 처리됩니다.
>
>모든 파일은 시나리오 실행 1개 내에서 처리됩니다.
>
>시나리오 세부 정보에서 이미 실행된 주기를 확인할 수 있습니다.
>
>![](assets/scenario-detail-350x207.png)
>
>이 페이지에 대한 자세한 내용은 [시나리오 세부 정보 [!DNL Adobe Workfront Fusion]](../../workfront-fusion/scenarios/scenario-detail.md)를 참조하세요.

## 연속 오류 수

시나리오 실행이 비활성화되기 전에 최대 연속 실행 시도 횟수를 정의합니다([!UICONTROL DataError], [!UICONTROL DuplicateDataError] 및 [!UICONTROL ConnectionError] 제외).

오류에 대한 자세한 내용은 [오류 처리 중 [!DNL Adobe Workfront Fusion]](../../workfront-fusion/errors/error-processing.md)을(를) 참조하십시오.

>[!NOTE]
>
>시나리오가 즉각적인 트리거로 시작하는 경우 설정이 무시되고 첫 번째 오류가 발생하면 시나리오가 즉시 비활성화됩니다.
