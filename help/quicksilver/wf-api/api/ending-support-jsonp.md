---
content-type: api
navigation-topic: api-navigation-topic
title: JSONP에 대한 지원 종료
description: JSONP에 대한 지원 종료
author: Becky
feature: Workfront API
role: Developer
exl-id: 681336c2-2f41-4746-8cba-be077f556742
source-git-commit: 3e339e2bfb26e101f0305c05f620a21541394993
workflow-type: tm+mt
source-wordcount: '206'
ht-degree: 0%

---

# JSONP에 대한 지원 종료

JSONP(Javascript with Padding)는 알려진 보안 취약성을 가진 이전 표준이므로 Adobe Workfront은 2018년 11월부터 더 이상 JSONP를 지원하지 않습니다. 이 결정은 Workfront 플랫폼을 현대화하기 위한 우리의 보다 큰 이니셔티브를 지원합니다.

JSONP는 원본 간 또는 사이트 간 요청을 수행할 수 있는 표준입니다. 많은 Workfront 고객 및 파트너는 JSONP를 사용하여 통합의 일부로 자체 도메인의 시스템에서 Workfront에 액세스합니다. JSONP를 사용하면 Workfront 애플리케이션이 Workfront이 아닌 도메인의 요청을 처리할 수 있습니다.

JSONP를 Workfront 통합의 일부로 사용하는 경우 CORS(원본 간 리소스 공유) 표준을 사용하도록 통합을 업데이트해야 합니다. 이 업데이트를 수행하려면 다음을 수행해야 합니다.

1. Workfront 지원 팀에 요청을 제출하여 허용 목록에 추가하다에 원본 간 요청을 하는 데 사용 중인 도메인을 포함하십시오.

   도메인을 CORS용 허용 목록에 추가하다Workfront 에 추가하려면 844-306-HELP(4357)의 고객 지원 센터에 문의하거나 지원 티켓을 온라인으로 제출하십시오.

   >[!NOTE]
   >
   >CORS용 허용 목록에 추가하다에 도메인 추가는 2018년 8월 1일 이전에 JSONP를 사용한 고객에게만 지원됩니다.


1. CORS를 사용하려면 통합 코드를 변경합니다.
