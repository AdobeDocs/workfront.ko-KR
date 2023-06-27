---
product-previous: workfront-fusion
product-area: workfront-integrations
navigation-topic: connections-annd-webhooks
title: 의 인스턴트 트리거(웹후크) [!DNL Adobe Workfront Fusion]
description: 많은 서비스는 서비스에서 특정 변경 사항이 발생할 때마다 즉시 알림을 전송할 수 있도록 웹후크를 제공합니다. 이러한 알림을 처리하려면 인스턴트 트리거를 사용하는 것이 좋습니다. 이 문서에서는 Adobe Workfront Fusion에서 인스턴트 트리거의 사용 및 기능에 대해 설명합니다.
author: Becky
feature: Workfront Fusion
exl-id: 13b3a1bf-9856-4d2c-b1a5-13b044a7c2e5
source-git-commit: 0915dcce45b271ee18cdd8af5db4f0eb01f3cced
workflow-type: tm+mt
source-wordcount: '903'
ht-degree: 0%

---

# 의 인스턴트 트리거(웹후크) [!DNL Adobe Workfront Fusion]

많은 서비스는 서비스에서 특정 변경 사항이 발생할 때마다 즉시 알림을 전송할 수 있도록 웹후크를 제공합니다. 이러한 알림을 처리하려면 인스턴트 트리거를 사용하는 것이 좋습니다. 다음에서 쉽게 알아볼 수 있습니다. [!DNL Adobe Workfront Fusion] 태그 때문에:

![](assets/instant-350x256.png)

서비스가 웹후크를 제공하지 않는 경우 폴링 트리거를 사용하여 서비스를 정기적으로 폴링해야 합니다.

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

## 웹후크의 대기열 보기

들어오는 웹후크의 모든 메시지는 웹후크의 큐에 저장됩니다.

1. 클릭 **[!UICONTROL 웹훅]** 왼쪽 메뉴에 있습니다.
1. 대기열을 보려는 웹후크를 찾습니다.
1. 트럭 아이콘과 받은 웹후크 수가 있는 버튼을 클릭합니다.

   ![](assets/webhooks-truck-icon.png)

   >[!NOTE]
   >
   >들어오는 웹후크 데이터는 옵션 설정 방법과 관계없이 항상 대기열에 저장됩니다 [!UICONTROL 데이터] 기밀임(다음에 설명됨) [의 시나리오 설정 패널 [!DNL Adobe Workfront Fusion]](../../workfront-fusion/scenarios/scenario-settings-panel.md)). 데이터가 시나리오에서 처리되는 즉시 시스템에서 영구적으로 삭제됩니다.

## 인스턴트 트리거 예약

시나리오에 인스턴스 트리거가 포함된 경우 시나리오가 즉시 실행되도록 예약할 수 있습니다.

![](assets/schedule-setting-350x185.png)

이 경우 다음 경우에 시나리오가 즉시 실행됩니다. [!DNL Workfront Fusion] 서비스에서 새 데이터를 받습니다. 시나리오가 실행되면 대기열에 대기 중인 총 보류 중인 웹후크의 수가 계산되고 시나리오는 보류 중인 웹후크의 수만큼 수행되며 주기당 하나의 웹후크를 처리합니다. 자세한 내용은 [의 시나리오 실행, 주기 및 단계 [!DNL Adobe Workfront Fusion]](../../workfront-fusion/scenarios/scenario-execution-cycles-phases.md).

>[!NOTE]
>
>* 주기는 시나리오 실행과 동일하지 않습니다. 1개의 시나리오 실행 내에 여러 주기가 있을 수 있습니다.
>* 즉각적인 트리거가 즉시 실행되도록 스케줄링된 시나리오를 실행할 경우 다음과 같은 예외가 적용됩니다.
>
>     * 두 실행 사이의 간격은 요금제에 따른 최소 간격의 적용을 받지 않습니다.
>
>       예를 들어 시나리오의 실행이 완료되면 웹후크의 대기열이 다시 확인됩니다. 보류 중인 웹후크가 있는 경우 시나리오는 즉시 다시 실행되어 보류 중인 모든 웹후크를 다시 처리합니다.
>   
>     * 최대 주기 수 시나리오 설정이 무시되고 100으로 설정되므로 단일 시나리오 실행 중에 100개 이하의 보류 중인 웹후크가 처리됩니다(한 주기당 이벤트 1개 비율).
>


다른 일정 설정을 사용하는 경우 [!UICONTROL 즉시]를 지정하면 지정한 간격으로 시나리오가 실행됩니다. 간격 동안 여러 개의 웹 후크를 대기열에 수집할 수 있으므로 를 설정하는 것이 좋습니다. [[!UICONTROL 최대 주기 수]](../../workfront-fusion/scenarios/scenario-settings-panel.md#maximum) 한 시나리오 실행에서 더 많은 웹후크를 처리하려면 기본값 1보다 큰 값으로 을 설정합니다.

1. 다음을 클릭합니다. [!UICONTROL 시나리오 설정] 아이콘 ![](assets/gear-icon-settings.png) 을 참조하십시오.
1. 다음에서 **[!UICONTROL 시나리오 설정]** 나타나는 상자에 숫자를 **[!UICONTROL 최대 주기 수]** 시나리오를 실행할 때마다 실행할 큐의 웹 후크 수를 나타내는 상자입니다.

## 비율 제한

현재 속도 제한은 초당 5개의 웹후크입니다. 한도를 초과하면 429 상태 코드가 반환됩니다.

## 비활성 웹후크 만료

120시간 이상 시나리오에 할당되지 않은 웹후크가 제거됩니다.

## Webhook 페이로드

[!DNL Workfront Fusion] 30일 동안 webhook 페이로드를 저장합니다. 생성된 후 30일 이상 지난 Webhook 페이로드에 액세스하면 오류가 발생합니다.&quot;[!UICONTROL 저장소에서 파일을 읽지 못했습니다.]&quot;

## 오류 처리

즉시 트리거를 사용하는 시나리오에서 오류가 있는 경우 시나리오는 다음과 같습니다.

* 즉시 중단 - 시나리오가 실행되도록 설정된 경우 [!UICONTROL 즉시].
* 시나리오가 예약대로 실행되도록 설정된 경우 3번의 실패 시도 후 중지됩니다(오류 3개).

시나리오 실행 중에 오류가 발생하면 즉시 트리거의 롤백 단계 중에 웹후크가 대기열에 다시 배치됩니다. 이러한 상황에서는 시나리오를 수정하고 다시 실행할 수 있습니다. 자세한 내용은 [롤백](../../workfront-fusion/scenarios/scenario-execution-cycles-phases.md#rollback) 이 문서에서 [의 시나리오 실행, 주기 및 단계 [!DNL Adobe Workfront Fusion]](../../workfront-fusion/scenarios/scenario-execution-cycles-phases.md).

시나리오에 Webhook 응답 모듈이 있으면 오류가 Webhook 응답으로 전송됩니다. Webhook 응답 모듈은 항상 마지막으로 실행됩니다(이 경우 [!UICONTROL 자동 커밋] 시나리오 설정의 옵션이 활성화되지 않음). 자세한 내용은 [웹후크에 응답](../../workfront-fusion/apps-and-their-modules/webhooks-updated.md#respondi) 이 문서에서 [웹훅](../../workfront-fusion/apps-and-their-modules/webhooks-updated.md).

## 사용자 지정 웹 후크

자신만의 웹후크를 만들 수 있습니다. 자세한 내용은 [웹훅](../../workfront-fusion/apps-and-their-modules/webhooks-updated.md).

## Webhook 비활성화

다음 중 하나가 적용되는 경우 웹후크는 자동으로 비활성화됩니다.

* 웹후크가 5일 이상 어떤 시나리오에도 연결되지 않았습니다.
* 웹후크는 30일 이상 비활성 상태인 비활성 시나리오에서만 사용됩니다.

비활성화된 웹후크는 시나리오에 연결되어 있지 않고 30일 이상 비활성화된 상태인 경우 자동으로 삭제 및 등록 취소됩니다.


