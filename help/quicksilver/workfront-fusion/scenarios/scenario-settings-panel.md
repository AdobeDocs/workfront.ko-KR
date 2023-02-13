---
product-previous: workfront-fusion
product-area: workfront-integrations
navigation-topic: scenarios
title: Adobe Workfront Fusion의 시나리오 설정 패널
description: 이 문서에서는 [!UICONTROL 시나리오 설정] 패널의 [!DNL Adobe Workfront Fusion] 시나리오.
author: Becky
feature: Workfront Fusion
exl-id: 64a7a39a-f450-4eba-b4db-f31dd22aefdc
source-git-commit: 59941ea1ce523a0d1036138a83f771b058049b34
workflow-type: tm+mt
source-wordcount: '968'
ht-degree: 0%

---

# 의 시나리오 설정 패널 [!DNL Adobe Workfront Fusion]

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

## 시나리오 설정을 엽니다.

1. 에 설명된 대로 시나리오 편집기를 엽니다. [의 시나리오 편집기 [!DNL Adobe Workfront Fusion]](../../workfront-fusion/scenarios/scenario-editor.md).
1. 페이지의 왼쪽 아래 모서리 근처에 있는 톱니바퀴 아이콘을 클릭합니다.

   ![](assets/scenario-settings-350x221.png)

   에서 [!UICONTROL 시나리오 설정] 표시되는 패널에서는 시나리오에 대한 다양한 고급 설정을 구성할 수 있습니다.

## [!UICONTROL 불완전한 실행 저장 허용]

이 옵션은 방법을 결정합니다 [!DNL Adobe Workfront Fusion] 시나리오를 실행하는 동안 오류가 발생하는 경우 발생합니다. 이 옵션을 활성화하면 시나리오가 일시 중지되어 로 이동합니다 [에서 불완전한 실행 보기 및 해결 [!DNL Adobe Workfront Fusion]](../../workfront-fusion/scenarios/view-and-resolve-incomplete-executions.md). 따라서 문제를 해결하고 시나리오가 중지된 위치에서 계속 실행할 수 있습니다. 이 옵션을 비활성화하면 시나리오 실행이 중지되고 롤백 단계가 시작됩니다.

## [!UICONTROL 순차적 처리]

이 옵션은 방법을 결정합니다 [!DNL Workfront Fusion] 오류가 발생하여 시나리오 실행이 [에서 불완전한 실행 보기 및 해결 [!DNL Adobe Workfront Fusion]](../../workfront-fusion/scenarios/view-and-resolve-incomplete-executions.md). 만약 [!UICONTROL 순차적 처리] 옵션이 활성화되어 있으면 모든 불완전한 실행이 해결될 때까지 Workfront Fusion이 작업 시퀀스의 처리를 모두 중지합니다. 만약 [!UICONTROL 순차적 처리] 옵션이 비활성화되어 있으면 시나리오가 해당 일정에 따라 계속 실행되며, 완료되지 않은 실행을 재실행하려는 반복 시도가 발생합니다.

예약에 대한 자세한 내용은 [에서 시나리오 예약 [!DNL Adobe Workfront Fusion]](../../workfront-fusion/scenarios/schedule-a-scenario.md).

## 데이터는 기밀입니다

시나리오가 실행되면 기본적으로 시나리오에서 모듈이 처리한 데이터에 대한 정보를 표시할 수 있습니다. 이 정보를 저장하지 않으려면 [!UICONTROL 데이터는 기밀입니다] 선택 사항입니다.

정보 표시에 대한 자세한 내용은 [의 시나리오 실행 흐름 [!DNL Adobe Workfront Fusion]](../../workfront-fusion/scenarios/scenario-execution-flow.md).

>[!IMPORTANT]
>
>이 옵션을 활성화하면 시나리오 실행 중에 발생할 수 있는 오류를 해결하기 어려울 수 있습니다.

## 데이터 손실 활성화

이 옵션은 다음의 경우 데이터 손실을 활성화하는 것과 관련이 있습니다 [!DNL Workfront Fusion] 의 큐에 번들을 저장하지 못했습니다. [에서 불완전한 실행 보기 및 해결 [!DNL Adobe Workfront Fusion]](../../workfront-fusion/scenarios/view-and-resolve-incomplete-executions.md) (예를 들어, 사용 가능한 공간이 부족하기 때문에) 이 옵션을 활성화하면 전체 시나리오 실행에서 중단이 발생하지 않도록 데이터가 손실됩니다. 이 기능은 가장 높은 우선 순위가 지속적인 실행이고 들어오는 잘못된 데이터가 중요하지 않은 시나리오에 유용합니다.

그 외에 시나리오를 실행할 때 모듈에는 허용되는 최대 크기보다 큰 파일이 가끔 발생할 수 있습니다. 이 경우 [!DNL Workfront Fusion] 의 설정에 따라 [!UICONTROL 데이터 손실 활성화] 옵션을 선택하고 경고 메시지가 표시됩니다.

최대 파일 크기에 대한 자세한 내용은 [의 파일 매핑 기본 정보 [!DNL Adobe Workfront Fusion]](../../workfront-fusion/mapping/about-mapping-files.md).

경고에 대한 자세한 내용은 [에서 처리 중 오류 발생 [!DNL Adobe Workfront Fusion]](../../workfront-fusion/errors/error-processing.md).

## [!UICONTROL 자동 커밋]

다음 [!UICONTROL 자동 커밋] 설정은 트랜잭션에 적용되며 시나리오를 처리하는 방법을 정의합니다. 자동 커밋 옵션이 켜져 있으면 작업 단계를 완료한 후 각 모듈의 커밋 단계가 즉시 시작됩니다. 자동 커밋 옵션을 비활성화하면 모든 모듈에 대해 작업이 실행될 때까지 커밋이 발생하지 않습니다(기본 모드).

트랜잭션에 대한 자세한 내용은 [시나리오 실행, 주기 및 단계 [!DNL Adobe Workfront Fusion]](../../workfront-fusion/scenarios/scenario-execution-cycles-phases.md).

## 최대 주기 수

추가 주기를 설정하면 타사 서비스에 대한 연결 중단을 방지하고 하나의 시나리오 실행 내에서 모든 레코드가 처리되도록 하려는 경우 유용할 수 있습니다.

* 시나리오가 폴링 트리거로 시작하는 경우 설정은 시나리오 실행 중에 허용되는 최대 주기 수를 정의합니다.

   폴링 트리거에 대한 자세한 내용은 [폴링 트리거](../../workfront-fusion/modules/module-types.md#polling) in [모듈 유형](../../workfront-fusion/modules/module-types.md).

* 시나리오가 인스턴트 트리거로 시작하는 경우 설정이 무시되고 보류 중인 모든 이벤트는 단일 시나리오 실행 중에 처리되며 한 주기당 하나의 이벤트입니다.

   인스턴트 트리거에 대한 자세한 내용은 [인스턴트 트리거](../../workfront-fusion/modules/module-types.md#instant) in [모듈 유형](../../workfront-fusion/modules/module-types.md).

* 시나리오가 트리거(인스턴트/폴링)로 시작되지 않는 경우 지정된 최대 주기 수가 항상 수행됩니다.

>[!INFO]
>
>**예:**  [!DNL Workfront] > [!UICONTROL 감시 레코드] 들어오는 새로운 문제를 감시하고 [!DNL Workfront] >[!UICONTROL 개체 변환] 새 요청을 프로젝트로 변환하여 적절한 템플릿에 할당합니다.
>
>![](assets/scenario-settings-ex-1-350x157.png)
>
>A [!UICONTROL 더 많은 주기] 설정은 시나리오 실행을 예약하는 경우에만 적용됩니다. 를 사용하는 경우 [!UICONTROL 한 번 실행] 버튼을 선택하면 주기 설정이 고려됩니다.
>
>### 최대 주기 수는 1로 설정됩니다(기본값)
>
>![](assets/max-number-cycles-1-350x201.png)
>
>다음 [!UICONTROL 반환된 최대 파일 수] 에서 [!UICONTROL Dropbox] >[!UICONTROL 감시 파일] 모듈이 `10`.
>
>![](assets/max-number-cycles-10-350x175.png)
>
>100개의 요청이 [!DNL Workfront], 및 [!UICONTROL 제한] 필드가 10으로 설정되면 하나의 시나리오 실행 후 90개의 파일이 처리되지 않은 상태로 유지됩니다. 다음 10개의 파일은 다음 예약된 시나리오 실행에서 처리됩니다.
>
>### 최대 주기 수는 10으로 설정됩니다.
>
>다음 [!UICONTROL 반환된 최대 파일 수] 에서 [!UICONTROL Dropbox] >[!UICONTROL 감시 파일] 모듈이 `10`.
>
>100개의 파일이 Dropbox 폴더 및 [!UICONTROL 반환된 최대 파일 수] 옵션을 10으로 설정하면 10개의 파일이 첫 번째 주기 동안 처리되고, 두 번째 주기에서는 다음 10개의 파일이 처리되며, 세 번째 주기에서는 다음 10개의 파일이 처리될 때까지 처리됩니다.
>
>모든 파일은 1개의 시나리오 실행 내에서 처리됩니다.
>
>시나리오 세부 정보에서 이미 실행된 주기를 볼 수 있습니다.
>
>![](assets/scenario-detail-350x207.png)
>
>이 페이지에 대한 자세한 내용은 [의 시나리오 세부 사항 [!DNL Adobe Workfront Fusion]](../../workfront-fusion/scenarios/scenario-detail.md).

## 연속 오류 수

시나리오 실행이 비활성화되기 전의 최대 연속 실행 시도 횟수를 정의합니다(제외). [!UICONTROL DataError], [!UICONTROL DuplicateDataError] 및 [!UICONTROL ConnectionError]).

오류에 대한 자세한 내용은 다음을 참조하십시오 [에서 처리 중 오류 발생 [!DNL Adobe Workfront Fusion]](../../workfront-fusion/errors/error-processing.md).

>[!NOTE]
>
>시나리오가 인스턴트 트리거로 시작하는 경우 설정이 무시되고 첫 번째 오류가 발생한 즉시 시나리오가 비활성화됩니다.
