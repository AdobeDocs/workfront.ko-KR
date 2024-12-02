---
content-type: api
navigation-topic: api-navigation-topic
title: 이벤트 구독 다시 시도
description: 이벤트 구독 다시 시도
author: Becky
feature: Workfront API
role: Developer
exl-id: b698cb60-4cff-4ccc-87d7-74afb5badc49
source-git-commit: 05f8dc8770c185720520fc631e19c75b925a70bf
workflow-type: tm+mt
source-wordcount: '394'
ht-degree: 0%

---

# 이벤트 구독 다시 시도

메시지 게재 시스템을 구현할 때 안정성, 일관성 및 양호한 사용자 경험을 보장하기 위해 몇 가지 주의 사항을 해결해야 합니다. 메시지 전달 시스템의 단점 중 하나는 메시지가 대상에 성공적으로 도달하도록 하고 메시지가 도달하지 못할 때 수행할 작업을 파악하는 것입니다.

일부 통합은 게재 실패를 수락한 후 메시지를 삭제하고 다음 메시지로 이동할 수 있습니다.  다른 통합에서는 메시지 전달 실패를 무시할 수 없습니다. 예를 들어 재무 통합에서 메시지 전달을 시도할 수 있지만 대신 서버가 메시지를 전달할 끝점을 찾을 수 없음을 나타내는 404의 HTTP 상태 코드를 받습니다. 이러한 경우, 메시지가 누락되면 누군가가 자신의 시간 동안 급여를 받지 못하거나 조직이 계약된 자원에 대한 예산을 초과 집행하는 것을 의미할 수 있습니다.

## 이벤트 구독 다시 시도를 위한 Adobe Workfront 전략

고객은 Workfront 플랫폼을 일상적인 지식 작업의 핵심 요소로 활용하기 때문에 Workfront 이벤트 구독 프레임워크는 각 메시지 게재를 가능한 한 최대한 시도하는 메커니즘을 제공합니다.

고객 엔드포인트에 게재되지 않는 이벤트 트리거된 아웃바운드 메시지는 최대 48시간 동안 게재에 성공할 때까지 재전송됩니다. 이 시간 동안 게재가 성공하거나 11번의 시도가 있을 때까지 점진적으로 증가한 빈도로 다시 시도합니다.

이러한 재시도 횟수의 공식은 다음과 같습니다.

`((2^attempt) - 1) * 84800ms`

첫 번째 재시도는 1.5분 후, 두 번째는 거의 5분이며, 11번째는 약 48시간이다.

고객은 Workfront 이벤트 구독의 아웃바운드 메시지를 사용하는 모든 엔드포인트가 배달이 성공하면 Workfront에 200개 수준의 응답 메시지를 다시 반환하도록 설정되었는지 확인해야 합니다.

## 비활성화 및 고정된 구독 규칙

* 구독 URL이 100회 이상 시도하여 실패율이 70%를 넘거나 연속 실패가 2,000개인 경우 **비활성화됨**&#x200B;입니다.
* 구독 URL이 2,000개가 넘는 연속 오류가 있고 마지막 성공이 72시간 이상이거나 일정 중 50,000개가 넘는 연속 오류가 있는 경우 **frozen**&#x200B;입니다.
* **사용 안 함** 구독 URL은 10분마다 계속 배달을 시도하고 배달이 성공하면 다시 사용할 수 있게 됩니다.
* API 요청을 통해 수동으로 활성화되지 않는 한 **frozen** 구독 URL은 배달을 시도하지 않습니다.




<!--

## Handling Failed Event-Triggered Outbound Messages

The following flowchart shows the strategy for reattempting message deliveries with Workfront Event Subscriptions:

![](assets/event-subscription-circuit-breaker-retries-350x234.png)

The following explanations correspond with the steps depicted in the flowchart:

1. Message fails to be delivered. 
1. Message delivery failure information is logged.

   All failed attempts to deliver a message are logged so that debugging may be performed to determine the root cause of a given failure or series of failures. 

1. URL failures incremented. 
1. Message attempt count is incremented. 
1. Calculate the delay until this message's delivery will be attempted again. 
1. Message is placed onto the message retry queue.

   As shown in the preceding flowchart, the message queue used for processing message delivery retries is a separate queue from the one that processes the initial delivery attempt for each message. This allows the near real-time flow of messages to continue unimpeded by the failure of any subset of messages. 

1. URL circuit status is evaluated. One of the following occurs:

   * If the circuit is open and not allowing deliveries at this time, restart the process at step 5.
   * If the circuit is half-open, this implies that our circuit is currently open, but enough time has passed to allow testing of the URL to see if the problem with delivering to it has been resolved.
   * If the message delivery attempt limits have been reached (48 hours of retrying) then the message is dropped

1. If the URL circuit is closed and allowing deliveries, attempt to deliver the message. If this delivery fails, the message will restart at step 1 

1. If the URL circuit is closed and allowing deliveries, attempt to deliver the message. If this delivery fails, the message will restart at step 1.
   -->
