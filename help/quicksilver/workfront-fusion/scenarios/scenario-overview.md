---
content-type: overview
product-previous: workfront-fusion
product-area: workfront-integrations
navigation-topic: scenarios
title: Adobe Workfront Fusion 시나리오 개요
description: Adobe Workfront Fusion에는 Adobe Workfront 라이선스 외에 Adobe Workfront Fusion 라이센스가 필요합니다.
author: Becky
feature: Workfront Fusion
exl-id: 13d6230d-51f6-4f68-8697-30f8ce6c8599
source-git-commit: 59941ea1ce523a0d1036138a83f771b058049b34
workflow-type: tm+mt
source-wordcount: '395'
ht-degree: 0%

---

# [!DNL Adobe Workfront Fusion] 시나리오 개요

>[!NOTE]
>
>[!DNL Adobe Workfront Fusion] 를 사용하려면 [!DNL Adobe Workfront Fusion] 라이센스 [!DNL Adobe Workfront license].

>[!IMPORTANT]
>
>[!DNL Workfront Fusion] 시나리오와 혼동해서는 안 됩니다 [!DNL Workfront Scenario Planner] 시나리오. 에 대한 자세한 정보 [!DNL Workfront Scenario Planner] 시나리오 [다음 [!DNL Scenario Planner] 개요](../../scenario-planner/scenario-planner-overview.md).

의 역할 [!DNL Adobe Workfront Fusion] 동일한 작업을 반복해서 반복하지 않고 새로운 작업에 집중할 수 있도록 프로세스를 자동화하는 것입니다. 앱과 서비스 내에서 및 앱과 서비스 간에 작업을 연결하여 데이터를 자동으로 전송 및 변환하는 시나리오를 만드는 방식으로 작동합니다. 사용자가 만드는 시나리오는 앱 또는 서비스의 데이터를 감시하고 원하는 결과를 제공하기 위해 해당 데이터를 처리합니다.

시나리오는 앱 내에서 또는 앱과 웹 서비스 간에 데이터를 전송하는 방법을 나타내는 일련의 모듈로 구성됩니다.

## 예: 내 프로세스 자동화 [!DNL Adobe Workfront]

>[!NOTE]
>
>이 기능은 다음 라이센스에 사용할 수 있습니다.
>
>* [!UICONTROL [!DNL Workfront Fusion] 작업 자동화를 위한]
>* [!UICONTROL [!DNL Workfront Fusion] 작업 자동화 및 통합을 위한]
>


[!DNL Workfront Fusion] 는 내에서 간단하거나 복잡한 워크플로우를 자동화할 수 있도록 해줍니다 [!DNL Workfront]를 업데이트하여 시간을 절약하고 프로세스가 일관되게 실행되도록 합니다.

이 예제에서 시나리오는 작업 또는 문제 의 지정된 필드가 변경되면 트리거됩니다 [!DNL Workfront]. 트리거되면 시나리오가 관련 프로젝트의 정보를 가져와서 프로젝트의 특정 역할에 지정된 사용자에 대해 맞춤 업데이트를 만듭니다.

![](assets/fusion-template-example-350x102.png)

## 예: 연결 중 [!DNL Workfront] 다른 앱 또는 웹 서비스를 통해

>[!NOTE]
>
>이 기능은 다음 라이센스에 사용할 수 있습니다.
>
>* [!UICONTROL [!DNL Workfront Fusion] 작업 자동화 및 통합을 위한]
>


[!DNL Workfront Fusion] 다른 앱 및 웹 서비스에 연결할 수도 있습니다. 다른 애플리케이션에서 데이터를 액세스, 가져오기, 조작 또는 내보내면서 Workfront과 통합하거나 서로 통합할 수 있습니다. 많은 응용 프로그램이 전용 [!DNL Workfront Fusion] 커넥터. 액세스하려는 응용 프로그램에 대한 전용 커넥터가 없는 경우 [!DNL Workfront Fusion]s [!UICONTROL HTTP] 또는 [!UICONTROL SOAP] api를 통해 애플리케이션에 연결할 모듈입니다.

이 예제에서 시나리오는 사용자가 [!DNL Excel] 스프레드시트. 시나리오는 사용자가 로그인되어 있는지 여부를 확인합니다 [!DNL Workfront]. 없는 경우 시나리오에서 사용자를 [!DNL Workfront] 그리고 Workfront 사용자 ID를 다시 스프레드시트에 추가합니다.

![](assets/fusion-integration-example--350x171.png)

전용 커넥터 목록은 다음을 참조하십시오. [앱 및 해당 모듈](../../workfront-fusion/apps-and-their-modules/apps-and-their-modules.md).

>[!IMPORTANT]
>
>[!DNL Adobe Workfront Fusion] 거의 모든 웹 서비스에 연결할 수 있습니다. 작업할 앱에 전용 기능이 없는 경우 [!DNL Workfront Fusion] 커넥터, 다음 모듈을 사용하여 웹 서비스에 직접 연결할 수 있습니다.
>
>* [[!UICONTROL HTTP] 모듈](../../workfront-fusion/apps-and-their-modules/http-modules/http-modules-1.md)
>* [[!UICONTROL SOAP] 모듈](../../workfront-fusion/apps-and-their-modules/soap-module.md)
>* [[!UICONTROL JSON] 모듈](../../workfront-fusion/apps-and-their-modules/json-modules.md)
>

