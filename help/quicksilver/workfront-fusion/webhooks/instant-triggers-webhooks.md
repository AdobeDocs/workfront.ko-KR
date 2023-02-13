---
product-previous: workfront-fusion
product-area: workfront-integrations
navigation-topic: connections-annd-webhooks
title: 의 즉각적인 트리거(웹 후크) [!DNL Adobe Workfront Fusion]
description: 많은 서비스에서 특정 변경 사항이 발생할 때마다 웹 후크를 제공하여 즉각적인 알림을 제공합니다. 이러한 알림을 처리하려면 인스턴트 트리거를 사용하는 것이 좋습니다. 이 문서에서는 Adobe Workfront Fusion의 즉각적인 트리거의 사용 및 기능에 대해 설명합니다.
author: Becky
feature: Workfront Fusion
exl-id: 13b3a1bf-9856-4d2c-b1a5-13b044a7c2e5
source-git-commit: 04191419ab6079cc34576b5a7532cd1596e4b91d
workflow-type: tm+mt
source-wordcount: '855'
ht-degree: 0%

---

# 의 즉각적인 트리거(웹 후크) [!DNL Adobe Workfront Fusion]

많은 서비스에서 특정 변경 사항이 발생할 때마다 웹 후크를 제공하여 즉각적인 알림을 제공합니다. 이러한 알림을 처리하려면 인스턴트 트리거를 사용하는 것이 좋습니다. 에서 이러한 코드를 쉽게 인식할 수 있습니다 [!DNL Adobe Workfront Fusion] 태그로 인해

![](assets/instant-350x256.png)

서비스에서 웹 후크를 제공하지 않는 경우 폴링 트리거를 사용하여 서비스를 주기적으로 폴링해야 합니다.

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
   <td> <p>[!UICONTROL [!DNL Workfront Fusion] 작업 자동화 및 통합을 위한] </p> <p>[!UICONTROL [!DNL Workfront Fusion] 작업 자동화를 위한]</p>  </td> 
  </tr> 
  <tr> 
   <td role="rowheader">제품</td> 
   <td>조직이 구매해야 합니다 [!DNL Adobe Workfront Fusion] 뿐만 아니라 [!DNL Adobe Workfront] 을 참조하십시오.</td> 
  </tr> 
 </tbody> 
</table>

어떤 계획, 라이센스 유형 또는 액세스 권한을 보유하고 있는지 확인하려면 [!DNL Workfront] 관리자

에 대한 자세한 정보 [!DNL Adobe Workfront Fusion] 라이센스 [[!DNL Adobe Workfront Fusion] 라이선스](../../workfront-fusion/get-started/license-automation-vs-integration.md).

## 웹 후크의 큐 보기

들어오는 웹 후크의 모든 메시지는 웹 후크의 큐에 저장됩니다.

1. 클릭 **[!UICONTROL Webhooks]** 왼쪽 메뉴에 있습니다.
1. 큐를 볼 웹 후크를 찾습니다.
1. 트럭 아이콘과 받은 웹 후크 수가 있는 버튼을 클릭합니다.

   ![](assets/webhooks-truck-icon.png)

   >[!NOTE]
   >
   >수신 웹 후크 데이터는 옵션 설정 방식에 관계없이 항상 큐에 저장됩니다 [!UICONTROL 데이터] 기밀성 [의 시나리오 설정 패널 [!DNL Adobe Workfront Fusion]](../../workfront-fusion/scenarios/scenario-settings-panel.md)). 데이터가 시나리오에서 처리되면 시스템에서 영구적으로 삭제됩니다.

## 인스턴트 트리거 예약

시나리오에 인스턴트 트리거가 포함된 경우 시나리오를 즉시 실행하도록 예약할 수 있습니다.

![](assets/schedule-setting-350x185.png)

이 경우 시나리오가 [!DNL Workfront Fusion] 서비스에서 새 데이터를 받습니다. 시나리오가 실행되면 대기열에서 대기 중인 총 웹 후크 양이 계산되며, 시나리오는 대기 중인 웹 후크가 있는 만큼 여러 사이클을 수행하여 주기당 하나의 웹 후크를 처리합니다. 자세한 내용은 [시나리오 실행, 주기 및 단계 [!DNL Adobe Workfront Fusion]](../../workfront-fusion/scenarios/scenario-execution-cycles-phases.md).

>[!NOTE]
>
>* 순환은 시나리오 실행과 동일하지 않습니다. 1개의 시나리오 실행 내에 여러 사이클이 있을 수 있습니다.
>* 즉시 트리거되도록 예약된 인스턴트 트리거로 시나리오를 실행하면 다음과 같은 예외가 적용됩니다.
   >
   >     * 두 실행 사이의 간격은 가격책정 계획에 따라 최소 간격의 적용을 받지 않습니다.

      >
      >       예를 들어 시나리오의 실행이 완료되면 웹 후크의 큐가 다시 확인됩니다. 보류 중인 웹 후크가 있는 경우 시나리오가 즉시 다시 실행되어 보류 중인 모든 웹 후크를 다시 처리합니다.
   >   
   >     * 최대 주기 수 시나리오 설정이 무시되고 100으로 설정되며, 이는 100개 이하의 보류 중인 웹 후크가 단일 시나리오 실행 동안(한 주기당 이벤트 1개 비율) 처리되지 않음을 의미합니다.
>



다른 스케줄 설정을 사용하는 경우 [!UICONTROL 즉시]인 경우 시나리오는 지정한 간격으로 실행됩니다. 간격 동안 큐에 여러 개의 웹 후크를 수집할 수 있으므로 [[!UICONTROL 최대 주기 수]](../../workfront-fusion/scenarios/scenario-settings-panel.md#maximum) 한 시나리오 실행에서 더 많은 웹 후크를 처리하기 위해 기본값 1보다 높은 값으로 설정하려면 다음을 수행하십시오.

1. 을(를) 클릭합니다. [!UICONTROL 시나리오 설정] 아이콘 ![](assets/gear-icon-settings.png) ( 시나리오 하단에 있습니다.)
1. 에서 **[!UICONTROL 시나리오 설정]** 표시되는 상자에 숫자를 입력합니다 **[!UICONTROL 최대 주기 수]** 상자를 사용하여 시나리오를 실행할 때마다 실행할 큐의 웹 후크 수를 나타냅니다.

## 비율 제한

현재 속도 제한은 초당 5개의 웹 후크입니다. 한도를 초과하면 429 상태 코드가 반환됩니다.

## 비활성 웹 후크의 만료

120시간 이상 시나리오에 할당되지 않은 웹 후크가 제거됩니다.

## Webhook 페이로드

[!DNL Workfront Fusion] 는 30일 동안 웹 후크 페이로드를 저장합니다. 웹 후크 페이로드를 만든 후 30일 이상 액세스하면 &quot; 오류가 발생합니다.[!UICONTROL 저장소에서 파일을 읽지 못했습니다.]&quot;

## 오류 처리

시나리오에서 인스턴트 트리거로 오류가 발생하면 시나리오는 다음과 같습니다.

* 즉시 중지됨 - 시나리오가 실행되도록 설정된 경우 [!UICONTROL 즉시].
* 3번 실패한 시도 후 중지(오류 3개) - 시나리오가 예약된 대로 실행되도록 설정된 경우.

시나리오 실행 중에 오류가 발생하면 인스턴트 트리거의 롤백 단계 동안 웹 후크가 다시 큐에 배치됩니다. 이러한 경우 시나리오를 수정하고 다시 실행할 수 있습니다. 자세한 내용은 [롤백](../../workfront-fusion/scenarios/scenario-execution-cycles-phases.md#rollback) 기사 [시나리오 실행, 주기 및 단계 [!DNL Adobe Workfront Fusion]](../../workfront-fusion/scenarios/scenario-execution-cycles-phases.md).

시나리오에 Webhook 응답 모듈이 있으면 오류가 Webhook 응답으로 전송됩니다. Webhook 응답 모듈은 항상 마지막으로 실행됩니다(이 경우 [!UICONTROL 자동 커밋] 시나리오 설정의 옵션을 활성화하지 않았습니다. 자세한 내용은 [Webhooks에 응답](../../workfront-fusion/apps-and-their-modules/webhooks-updated.md#respondi) 기사 [Webhooks](../../workfront-fusion/apps-and-their-modules/webhooks-updated.md).

## 사용자 정의 웹 후크

고유한 웹 후크를 만들 수 있습니다. 자세한 내용은 [Webhooks](../../workfront-fusion/apps-and-their-modules/webhooks-updated.md).

## Webhook 비활성화

다음 중 하나가 적용되는 경우 웹 후크는 자동으로 비활성화됩니다.

* 웹 후크가 5일 이상 시나리오에 연결되지 않았습니다
* 웹 후크는 30일 이상 비활성 시나리오에서만 사용됩니다.

비활성화된 웹 후크는 모든 시나리오에 연결되어 있지 않고 30일 이상 비활성화된 상태에 있는 경우 자동으로 삭제되고 등록되지 않습니다.


