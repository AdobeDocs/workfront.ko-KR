---
content-type: api
navigation-topic: api-navigation-topic
title: 이벤트 구독 다시 시도
description: 이벤트 구독 다시 시도
author: Becky
feature: Workfront API
role: Developer
exl-id: b698cb60-4cff-4ccc-87d7-74afb5badc49
source-git-commit: 3e339e2bfb26e101f0305c05f620a21541394993
workflow-type: tm+mt
source-wordcount: '548'
ht-degree: 0%

---

# 이벤트 구독 다시 시도

메시지 게재 시스템을 구현할 때 안정성, 일관성 및 양호한 사용자 경험을 보장하기 위해 몇 가지 주의 사항을 해결해야 합니다. 메시지 전달 시스템의 단점 중 하나는 메시지가 대상에 성공적으로 도달하도록 하고 메시지가 도달하지 못할 때 수행할 작업을 파악하는 것입니다.

일부 통합은 게재 실패를 수락한 후 메시지를 삭제하고 다음 메시지로 이동할 수 있습니다.  다른 통합에서는 메시지 전달 실패를 무시할 수 없습니다. 예를 들어 재무 통합에서 메시지 전달을 시도할 수 있지만 대신 서버가 메시지를 전달할 끝점을 찾을 수 없음을 나타내는 404의 HTTP 상태 코드를 받습니다. 이러한 경우, 메시지가 누락되면 누군가가 자신의 시간 동안 급여를 받지 못하거나 조직이 계약된 자원에 대한 예산을 초과 집행하는 것을 의미할 수 있습니다.

## 이벤트 구독 다시 시도를 위한 Adobe Workfront 전략

고객은 Workfront 플랫폼을 일상적인 지식 작업의 핵심 요소로 활용하기 때문에 Workfront 이벤트 구독 프레임워크는 각 메시지 게재를 가능한 한 최대한 시도하는 메커니즘을 제공합니다.

고객 엔드포인트에 게재되지 않는 이벤트 트리거된 아웃바운드 메시지는 최대 48시간 동안 게재에 성공할 때까지 재전송됩니다. 이 시간 동안 게재가 성공하거나 48시간이 경과할 때까지 점진적으로 줄어든 빈도로 다시 시도합니다.

고객은 Workfront 이벤트 구독의 아웃바운드 메시지를 사용하는 모든 엔드포인트가 배달이 성공하면 Workfront에 200개 수준의 응답 메시지를 다시 반환하도록 설정되었는지 확인해야 합니다.

## 실패한 이벤트 트리거 아웃바운드 메시지 처리

다음 순서도는 Workfront 이벤트 구독으로 메시지 게재를 다시 시도하는 전략을 보여 줍니다.

![](assets/event-subscription-circuit-breaker-retries-350x234.png)

다음 설명은 순서도에 표시된 단계에 해당합니다.

1. 메시지를 배달하지 못했습니다.
1. 메시지 게재 실패 정보가 기록됩니다.

   메시지 전달에 실패한 모든 시도가 기록되므로 주어진 실패 또는 일련의 실패의 근본 원인을 파악하기 위해 디버깅을 수행할 수 있습니다.

1. URL 오류가 증가했습니다.
1. 메시지 시도 횟수가 증가합니다.
1. 이 메시지의 게재가 다시 시도될 때까지의 지연 시간을 계산합니다.
1. 메시지가 메시지 다시 시도 큐에 배치됩니다.

   앞의 순서도에서 보듯이, 메시지 게재 다시 시도 처리에 사용되는 메시지 대기열은 각 메시지에 대한 초기 게재 시도를 처리하는 대기열과 별개의 대기열입니다. 이를 통해 메시지의 거의 실시간 흐름이 메시지 하위 집합의 장애에 의해 방해받지 않고 계속될 수 있습니다.

1. URL 회로 상태가 평가됩니다. 다음 중 하나가 발생합니다.

   * 회로가 열려 있고 현재 전달을 허용하지 않는 경우 5단계에서 프로세스를 재시작합니다.
   * 회로가 반 열려 있는 경우 현재 회로가 열려 있지만 URL을 전달하는 데 문제가 해결되었는지 테스트할 수 있는 시간이 충분히 지났음을 의미합니다.
   * 메시지 게재 시도 제한에 도달한 경우(재시도 후 48시간) 메시지는 삭제됩니다

1. URL 회로가 닫혀 있고 게재를 허용하는 경우 메시지 게재를 시도합니다. 이 게재가 실패하면 메시지가 1단계에서 다시 시작됩니다

1. URL 회로가 닫혀 있고 게재를 허용하는 경우 메시지 게재를 시도합니다. 이 게재가 실패하면 메시지가 1단계에서 다시 시작됩니다.

   <!--
   <li value="10" data-mc-conditions="QuicksilverOrClassic.Draft mode">Workfront disables Event Subscriptions when both of the following criteria are met:
   <ul>
   <!--
   <li data-mc-conditions="QuicksilverOrClassic.Draft mode">The Event Subscription has failed 1000 delivery attempts consecutively</li>
   <li data-mc-conditions="QuicksilverOrClassic.Draft mode">48 hours have passed since the last successful delivery</li>
   </ul></li>
   -->
