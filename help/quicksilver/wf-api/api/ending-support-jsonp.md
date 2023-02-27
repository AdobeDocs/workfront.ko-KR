---
content-type: api
navigation-topic: api-navigation-topic
title: JSONP에 대한 지원 종료
description: JSONP에 대한 지원 종료
author: Becky
feature: Workfront API
exl-id: 681336c2-2f41-4746-8cba-be077f556742
source-git-commit: f050c8b95145552c9ed67b549608c16115000606
workflow-type: tm+mt
source-wordcount: '203'
ht-degree: 0%

---

# JSONP에 대한 지원 종료

JSONP(Padding이 있는 Javascript)는 알려진 보안 취약점이 있는 이전 표준이므로, Adobe Workfront은 2018년 11월부터 JSONP를 더 이상 지원하지 않습니다. 이 결정은 Workfront 플랫폼을 현대화하는 우리의 더 큰 계획을 지원합니다.

JSONP는 교차 사이트 또는 교차 사이트 요청을 수행할 수 있는 표준입니다. 많은 Workfront 고객 및 파트너는 JSONP를 사용하여 통합의 일부로 자체 도메인의 시스템에서 Workfront에 액세스합니다. JSONP를 사용하면 Workfront이 아닌 도메인의 요청을 Workfront 애플리케이션에서 처리할 수 있습니다.

Workfront 통합의 일부로 JSONP를 사용하는 경우 CORS(Cross-Origin Resource Sharing) 표준을 사용하도록 통합을 업데이트해야 합니다. 이 업데이트를 수행하려면 다음을 수행해야 합니다.

1. Workfront 지원 팀에 교차 도메인 요청을 하는 데 사용 중인 도메인을 갖도록 요청을 허용 목록에 추가하다 제출합니다.

   도메인을 CORS에 대한에 허용 목록에 추가하다 추가하려면 Workfront 고객 지원 센터(844-306-HELP(4357)에 문의하거나 온라인으로 지원 티켓을 제출하십시오.

   >[!NOTE]
   >
   >CORS용에 도메인허용 목록에 추가하다를 추가하는 것은 2018년 8월 1일 이전에 JSONP를 사용하는 고객에게만 지원됩니다.


1. CORS를 사용하도록 통합 코드를 변경합니다.
