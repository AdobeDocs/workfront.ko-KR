---
content-type: reference
product-area: workfront-integrations
keywords: native,ootb
navigation-topic: workfront-integrations-navigation-topic
title: Adobe Workfront 통합 메서드
description: ' [!DNL Adobe Workfront] 을(를) 타사 응용 프로그램과 통합할 수 있습니다. 이러한 통합을 통해  [!DNL Workfront] 의 유틸리티를 확장하고 조직의 요구 사항에 맞게 조정할 수 있습니다. 제공된 작업에 가장 유용한 통합에 따라 이러한 통합 중 일부 또는 모두를 사용할 수 있습니다.'
feature: Workfront Integrations and Apps, Workfront Fusion
exl-id: bf13a7c9-eab3-4ae3-a060-8a422236122d
source-git-commit: 328d3a8d16ace22100d86efc127874d7edd6cb6d
workflow-type: tm+mt
source-wordcount: '945'
ht-degree: 0%

---

# Adobe Workfront 통합 메서드

[!DNL Adobe Workfront]을(를) 타사 응용 프로그램 및 다른 [!DNL Adobe] 제품과 통합할 수 있습니다. 이러한 통합을 통해 [!DNL Workfront]의 유틸리티를 확장하고 조직의 요구 사항에 맞게 조정할 수 있습니다. 제공된 작업에 가장 유용한 통합에 따라 이러한 통합 중 일부 또는 모두를 사용할 수 있습니다.

## 내장 통합

Workfront은 Workfront에서 직접 구성하거나, 해당 애플리케이션에 Workfront 추가 기능을 설치하여 다른 애플리케이션에서 구성할 수 있는 다양한 통합을 제공합니다. 이러한 기본 제공 통합은 많은 일반적인 사용 사례 시나리오를 다루고 최종 사용자를 위한 사용자 경험을 확장하고 연결하는 데 중점을 둡니다.

Workfront의 내장 통합은 주로 개인 생산성 및 공동 작업에 중점을 둡니다. 이러한 통합을 통해 개별 사용자의 워크플로우가 중단되는 것을 줄여 Workfront 알림을 수신하고, 정보에 액세스하고, 통합 애플리케이션을 종료하지 않고 Workfront 작업 항목에 대해 작업할 수 있습니다.

기본 제공 통합의 이점은 다음과 같습니다.

* 이러한 기본 제공 통합의 대부분은 추가 비용 없이 사용할 수 있습니다. (다른 제품들은 추가 구매가 필요하지 않습니다.)
* 기본 제공 통합은 [!DNL Slack], [!DNL Google Drive] 또는 [!DNL Adobe] 제품(예: [!DNL Adobe Creative Cloud] 또는 [!DNL Adobe Experience Manager] Assets)과 같이 비즈니스에서 사용하는 가장 일반적인 앱의 대부분을 포함합니다. 회사에서 이미 이러한 앱을 사용하고 있는 경우 사용자의 기존 워크플로우로 원활하게 통합됩니다.
* [!DNL Workfront]을(를) 자주 사용하는 응용 프로그램과 통합하면 사용자 간의 채택률을 높일 수 있습니다.

>[!INFO]
>
>**예:**
>
>[!DNL Workfront for Microsoft Teams integration]을(를) 사용하면 [!DNL Microsoft Teams]에서 [!DNL Workfront] 작업 항목에 대한 알림을 받을 수 있습니다. [!DNL Microsoft Teams]을(를) 종료하지 않고 작업 항목의 상태를 승인, 댓글 달기 또는 변경하는 등의 작업을 수행할 수 있습니다. 작업 항목 [!DNL Microsoft Teams]에서 변경한 내용은 [!DNL Workfront]에도 반영됩니다.

현재 사용 가능한 기본 제공 통합 목록을 포함하여 기본 제공 통합에 대한 자세한 내용은 [[!DNL Adobe Workfront] 기본 제공 통합 개요](../workfront-integrations-and-apps/built-in-integrations-non-admin.md)를 참조하십시오.

## 사용자 정의 OAuth2 애플리케이션

Adobe [!DNL Workfront] 관리자는 [!DNL Workfront] 인스턴스에 대한 OAuth2 응용 프로그램을 만들 수 있으며, 이를 통해 다른 응용 프로그램에서 [!DNL Workfront]에 액세스할 수 있습니다. 그런 다음 사용자는 다른 응용 프로그램에 [!DNL Workfront] 데이터에 액세스할 수 있는 권한을 부여할 수 있습니다. 이러한 방식으로 Workfront을 사내 애플리케이션을 포함하여 원하는 애플리케이션과 통합할 수 있습니다.

>[!NOTE]
>
>OAuth2의 컨텍스트에서 &quot;앱 만들기&quot;는 앱과 서버(예: Workfront) 간에 이러한 종류의 액세스 링크를 만드는 프로세스를 말합니다.

[!UICONTROL OAuth2] 응용 프로그램을 만들 때 얻을 수 있는 이점은 다음과 같습니다.

* 사용자는 기본 제공 통합과 유사하게 이러한 통합을 [!DNL Workfront]에서 직접 사용할 수 있습니다.
* [!UICONTROL OAuth2] 응용 프로그램을 설정하거나 사용하면 [!DNL Workfront] API에 익숙해지는 것과 같은 추가 기술 지식이 필요하지 않습니다.
* 조직에서 [!DNL Workfront] 기본 제공 응용 프로그램으로 제공되지 않는 소프트웨어를 사용할 수 있습니다. 이 소프트웨어가 조직의 소유권이더라도 [!UICONTROL OAuth2] 응용 프로그램을 사용하여 이 소프트웨어를 [!DNL Workfront]과(와) 통합할 수 있습니다.

자세한 내용은 [Workfront 통합을 위한 OAuth2 애플리케이션 만들기](../administration-and-setup/configure-integrations/create-oauth-application.md)를 참조하십시오.

## [!DNL Workfront] API

[!DNL Workfront]에서는 Workfront 환경을 확장하고 개선할 수 있는 공용 API(응용 프로그램 프로그래밍 인터페이스)를 제공합니다. [!DNL Workfront] API의 목표는 HTTP를 통해 작동하는 REST 풀 아키텍처를 도입하여 [!DNL Workfront]과의 자체 통합 구축을 간소화하는 것입니다. [!DNL Workfront] API에는 몇 가지 기술 지식이 필요하지만 데이터를 검색, 생성 및 수정하는 데 매우 강력한 도구입니다. 매우 구체적인 기능을 수행하도록 API 호출을 사용자 정의할 수 있습니다.

또한 [!DNL Workfront]은(는) 이벤트 구독 API를 제공합니다. 이벤트 구독이 지원하는 [!DNL Workfront] 개체에서 작업이 발생하면 원하는 끝점에 응답을 보내도록 [!DNL Workfront]을(를) 구성할 수 있습니다. 즉, 서드파티 애플리케이션은 [!DNL Workfront] API를 통해 [!DNL Workfront] 인터랙션이 발생한 직후 업데이트를 받을 수 있습니다.

[!DNL Workfront] API를 사용하면 다음과 같은 이점이 있습니다.

* [!DNL Workfront] API를 사용하여 공개 API를 제공하는 거의 모든 다른 웹 서비스 또는 앱에 연결할 수 있습니다. 따라서 [!DNL Workfront]을(를) 사용하려는 거의 모든 웹 서비스 또는 앱과 통합할 수 있습니다.
* [!DNL Workfront] API의 유연성은 또한 귀사의 독점 소프트웨어로 확장됩니다. 자체 소프트웨어 내에서 [!DNL Workfront] 데이터를 사용하고 수정할 수 있습니다.
* API는 소프트웨어에 매우 일반적이므로 사내 개발자는 API에 익숙할 수 있습니다. [!DNL Workfront]은(는) 가장 일반적인 API 유형인 REST-ful API를 사용하므로 개발자가 속도를 빠르게 향상하는 것이 훨씬 쉽습니다.

>[!INFO]
>
>**예:**
>
>다음 API 호출은 지정된 ID를 사용하여 작업의 업데이트 스트림에 댓글을 추가합니다.
>
>```
>https://`<your domain>`.workfront.com/attask/api-internal/note?noteText=<text of comment>&noteObjCode=TASK&objID=<task ID>&apiKey=<your API key>
>```

[!DNL Workfront] API에 대한 자세한 내용은 [API 기본 사항](../wf-api/general/api-basics.md)을 참조하세요.

이벤트 구독에 대한 자세한 내용은 [이벤트 구독 API](../wf-api/general/event-subs-api.md)를 참조하십시오.

## [!DNL Adobe Workfront Fusion]

[!DNL Workfront Fusion]을(를) 사용하면 워크플로우를 자동화할 수 있습니다. [!DNL Workfront Fusion for Work Automation and Integration] 라이선스를 사용하면 여러 앱 및 웹 서비스에 이러한 자동화를 만들어 앱이 함께 작업을 실행하는 시나리오를 만들 수 있습니다. 시나리오는 모듈을 사용하여 작성한 작업 또는 워크플로를 시각적으로 표현한 것으로, &quot;문서 다운로드&quot; 또는 &quot;프로젝트 만들기&quot;와 같은 개별 작업입니다. 모듈을 서로 연결하여 워크플로우를 정의한 다음 트리거 조건이 충족되면 워크플로우가 자동으로 실행됩니다.

[!DNL Workfront Fusion]의 이점에는 다음이 포함될 수 있습니다.

* 시각적 인터페이스는 워크플로를 이해하고 설정하는 데 도움이 되므로 [!DNL Workfront Fusion]은(는) API만큼 많은 기술 지식이 필요하지 않습니다. 이는 개발 팀 외부의 개인이 사용할 수 있음을 의미하며, 이로 인해 조직의 시간과 비용이 절약될 수 있습니다.
* [!DNL Workfront Fusion]은(는) API를 통해 작동하므로 대부분의 앱과 웹 서비스에 액세스할 수 있습니다. 많은 앱에 API를 호출하는 모듈이 있거나, HTTP, SOAP 또는 JSON 모듈을 사용하여 전용 [!DNL Workfront Fusion] 커넥터가 없는 웹 서비스와 상호 작용할 수 있습니다.

>[!INFO]
>
>**예:**
>
>[!DNL Workfront Fusion]의 다음 [!DNL Workfront] 모듈이 선택한 프로젝트에 주석을 추가하도록 설정되었습니다. 모듈이 실행되면 주석은 Workfront의 프로젝트 업데이트 스트림에 표시됩니다.
>
>![](assets/fusion-example-comment-350x416.png)

[!DNL Workfront Fusion]에 대한 자세한 내용은 [[!DNL Adobe Workfront Fusion]](../workfront-fusion/workfront-fusion-2.md)을(를) 참조하십시오.
