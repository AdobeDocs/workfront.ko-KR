---
content-type: reference
product-area: workfront-integrations
keywords: native,ootb
navigation-topic: workfront-integrations-navigation-topic
title: Adobe Workfront 통합 방법
description: 통합할 수 있습니다 [!DNL Adobe Workfront] 타사 애플리케이션에서 사용할 수 있습니다. 이러한 통합은 [!DNL Workfront] 조직의 요구 사항에 맞게 조정할 수 있습니다. 주어진 작업에 가장 유용한 통합에 따라 이러한 통합을 모두 사용하거나 사용할 수 있습니다.
feature: Workfront Integrations and Apps, Workfront Fusion
exl-id: bf13a7c9-eab3-4ae3-a060-8a422236122d
source-git-commit: 328d3a8d16ace22100d86efc127874d7edd6cb6d
workflow-type: tm+mt
source-wordcount: '946'
ht-degree: 0%

---

# Adobe Workfront 통합 방법

통합할 수 있습니다 [!DNL Adobe Workfront] 타사 애플리케이션과 기타 [!DNL Adobe] 제품. 이러한 통합은 [!DNL Workfront] 조직의 요구 사항에 맞게 조정할 수 있습니다. 주어진 작업에 가장 유용한 통합에 따라 이러한 통합을 모두 사용하거나 사용할 수 있습니다.

## 내장 통합

Workfront은 Workfront에서 직접 또는 해당 애플리케이션용 Workfront 추가 기능을 설치하여 다른 애플리케이션에서 구성할 수 있는 다양한 통합을 제공합니다. 이러한 내장 통합은 많은 일반적인 사용 사례 시나리오를 포함하며, 최종 사용자를 위한 사용자 경험 확장 및 연결에 중점을 둡니다.

Workfront 내장 통합은 주로 개인 생산성 및 공동 작업에 중점을 둡니다. 이러한 통합을 통해 개별 사용자의 워크플로우에서 중단이 감소되어, 통합 애플리케이션을 종료하지 않고도 Workfront 알림을 받고, 정보에 액세스하고, Workfront 작업 항목에 대해 작업할 수 있습니다.

기본 제공 통합의 장점은 다음과 같습니다.

* 이러한 기본 제공 통합 중 다수는 추가 비용 없이 사용할 수 있습니다. (다른 사용자는 추가 구매를 필요로 합니다.)
* 내장된 통합은 다음과 같이 기업이 사용하는 대부분의 일반적인 앱을 포함합니다 [!DNL Slack], [!DNL Google Drive], 또는 [!DNL Adobe] 와 같은 제품 [!DNL Adobe Creative Cloud] 또는 [!DNL Adobe Experience Manager] 자산. 회사에서 이러한 앱을 이미 사용하고 있다면 통합은 사용자의 기존 워크플로우에 원활하게 통합됩니다.
* 통합 [!DNL Workfront] 자주 사용되는 애플리케이션을 사용하면 사용자 간의 채택률을 높일 수 있습니다.

>[!INFO]
>
>**예:**
>
>사용 [!DNL Workfront for Microsoft Teams integration], 에서 알림을 받을 수 있습니다. [!DNL Microsoft Teams] 정보 [!DNL Workfront] 작업 항목입니다. 떠나지 않고 [!DNL Microsoft Teams]작업 항목의 승인, 주석 달기 또는 상태 변경과 같은 작업을 수행할 수 있습니다. 작업 항목에 대한 변경 내용은 [!DNL Microsoft Teams] 에 반영됩니다. [!DNL Workfront] 또한.

현재 사용 가능한 기본 통합 목록을 포함한 기본 제공 통합에 대한 자세한 내용은 다음을 참조하십시오 [[!DNL Adobe Workfront] 내장 통합 개요](../workfront-integrations-and-apps/built-in-integrations-non-admin.md).

## 사용자 지정 OAuth2 애플리케이션

Adobe [!DNL Workfront] 관리자는 자신의 인스턴스에 대해 OAuth2 응용 프로그램을 만들 수 있습니다 [!DNL Workfront]: 다른 응용 프로그램이 액세스할 수 있도록 합니다 [!DNL Workfront]. 그런 다음 사용자는 다른 응용 프로그램에 액세스하여 액세스할 수 있는 권한을 부여할 수 있습니다 [!DNL Workfront] 데이터. 이러한 방식으로 사내 애플리케이션을 포함하여 원하는 애플리케이션과 Workfront을 통합할 수 있습니다.

>[!NOTE]
>
>OAuth2 컨텍스트에서 &quot;앱 만들기&quot;는 앱과 Workfront 같은 서버 간에 이러한 종류의 액세스 링크를 만드는 프로세스를 말합니다.

만들기 이점 [!UICONTROL OAuth2] 응용 프로그램에는 다음이 포함될 수 있습니다.

* 사용자는에서 바로 이러한 통합을 사용할 수 있습니다 [!DNL Workfront]: 기본 제공 통합과 유사합니다.
* 설정 또는 사용 [!UICONTROL OAuth2] 응용 프로그램에는 과 같은 추가적인 기술 지식이 필요하지 않습니다 [!DNL Workfront] API.
* 조직에서 [!DNL Workfront] 기본 제공 애플리케이션. 이 소프트웨어를 [!DNL Workfront] 사용 [!UICONTROL OAuth2] 애플리케이션이 조직에 속해 있더라도

자세한 내용은 [Workfront 통합을 위한 OAuth2 애플리케이션 만들기](../administration-and-setup/configure-integrations/create-oauth-application.md).

## [!DNL Workfront] API

[!DNL Workfront] 은 Workfront 경험을 확장 및 향상시킬 수 있는 공용 API(애플리케이션 프로그래밍 인터페이스)를 제공합니다. 에 대한 목표 [!DNL Workfront] API는 와의 자체 통합 구축을 간소화하는 것입니다 [!DNL Workfront] http를 통해 작동하는 REST ful 아키텍처를 도입했습니다. 다음 [!DNL Workfront] API는 일부 기술 지식이 필요하지만 데이터를 검색, 생성 및 수정하는 강력한 도구입니다. API 호출을 사용자 지정하여 매우 구체적인 기능을 수행할 수 있습니다.

게다가, [!DNL Workfront] 은 이벤트 구독 API를 제공합니다. 작업 발생 시 [!DNL Workfront] 이벤트 구독에서 지원하는 개체를 구성할 수 있습니다 [!DNL Workfront] 를 입력하여 원하는 종단점에 대한 응답을 보냅니다. 즉, 타사 애플리케이션이 [!DNL Workfront] 를 통한 상호 작용 [!DNL Workfront] API가 발생한 후 바로 API입니다.

사용 시 이점 [!DNL Workfront] API에는 다음을 포함할 수 있습니다.

* 를 사용할 수 있습니다 [!DNL Workfront] 공용 API를 제공하는 거의 모든 다른 웹 서비스 또는 앱에 연결하는 API입니다. 따라서 통합할 수 있습니다 [!DNL Workfront] 사용할 거의 모든 웹 서비스 또는 앱과 함께 사용할 수 있습니다.
* 다음 [!DNL Workfront] API의 유연성은 비즈니스 전용 소프트웨어로도 확장됩니다. 을 사용하고 수정할 수 있습니다 [!DNL Workfront] 소프트웨어를 통해 데이터를 얻을 수 있습니다.
* API는 소프트웨어에 매우 일반적이므로 사내 개발자는 API에 익숙할 것입니다. [!DNL Workfront] 는 가장 일반적인 유형의 API인 REST-ful API를 사용하므로 개발자가 빠르게 작업할 수 있습니다.

>[!INFO]
>
>**예:**
>
>다음 API 호출에서는 지정된 ID를 사용하여 작업의 업데이트 스트림에 주석을 답니다.
>
>
```
>https://`<your domain>`.workfront.com/attask/api-internal/note?noteText=<text of comment>&noteObjCode=TASK&objID=<task ID>&apiKey=<your API key>
>```

에 대한 자세한 정보 [!DNL Workfront] API입니다. 자세한 내용은 [API 기본 사항](../wf-api/general/api-basics.md).

이벤트 가입에 대한 자세한 내용은 [이벤트 구독 API](../wf-api/general/event-subs-api.md).

## [!DNL Adobe Workfront Fusion]

[!DNL Workfront Fusion] 워크플로우를 자동화할 수 있습니다. 사용 [!DNL Workfront Fusion for Work Automation and Integration] 라이센스를 취득하면 여러 앱 및 웹 서비스에서 이러한 자동화를 만들어 앱을 함께 사용하여 작업을 실행하는 시나리오를 만들 수 있습니다. 시나리오는 &quot;문서 다운로드&quot; 또는 &quot;프로젝트 만들기&quot;와 같은 개별 작업인 모듈을 사용하여 만들어진 작업 또는 워크플로우의 시각적 표현입니다. 모듈을 함께 연결하여 워크플로우를 정의한 다음 트리거 조건이 충족되면 워크플로우가 자동으로 실행됩니다.

장점 [!DNL Workfront Fusion] 에는 다음 항목이 포함될 수 있습니다.

* [!DNL Workfront Fusion] 는 시각적 인터페이스가 워크플로우를 이해하고 설정하는 데 도움이 되므로 API만큼 기술 지식이 필요하지 않습니다. 즉, 개발 팀 외부의 개인이 사용할 수 있으므로 조직의 시간과 비용을 절약할 수 있습니다.
* 이후 [!DNL Workfront Fusion] 는 API를 통해 작동하며 대부분의 앱 및 웹 서비스에 액세스할 수 있습니다. 많은 앱에 API를 호출하는 모듈이 있거나 HTTP, SOAP 또는 JSON 모듈을 사용하여 전용 앱이 없는 웹 서비스와 상호 작용할 수 있습니다 [!DNL Workfront Fusion] 커넥터.

>[!INFO]
>
>**예:**
>
>다음 [!DNL Workfront] 모듈 [!DNL Workfront Fusion] 이(가) 선택된 프로젝트에 주석을 추가하도록 설정되어 있습니다. 모듈이 실행되면 Workfront에서 프로젝트의 업데이트 스트림에 주석이 표시됩니다.
>
>![](assets/fusion-example-comment-350x416.png)

에 대한 자세한 정보 [!DNL Workfront Fusion]를 참조하십시오. [[!DNL Adobe Workfront Fusion]](../workfront-fusion/workfront-fusion-2.md).
