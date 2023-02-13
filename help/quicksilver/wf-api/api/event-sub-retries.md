---
content-type: api
navigation-topic: api-navigation-topic
title: 이벤트 구독 다시 시도
description: 이벤트 구독 다시 시도
author: John
feature: Workfront API
exl-id: b698cb60-4cff-4ccc-87d7-74afb5badc49
source-git-commit: 606d19b8a83b833aba6d6b15231a8683aa2cee40
workflow-type: tm+mt
source-wordcount: '541'
ht-degree: 0%

---

# 이벤트 구독 다시 시도

메시지 전달 시스템을 구현할 때 안정성, 일관성 및 사용자 환경을 보장하기 위해 해결해야 하는 몇 가지 주의해야 할 사항이 있습니다. 메시지 전달 시스템의 단점 중 하나는 메시지가 성공적으로 도착하도록 하고 메시지가 도착하지 않을 때 어떻게 해야 하는지 파악하는 것입니다.

일부 통합에서는 게재 실패를 수락한 다음 메시지를 삭제하고 다음 메시지로 이동할 수 있습니다.  다른 통합에서 메시지 게재 실패를 무시할 수 없습니다. 예를 들어, 금융 통합에서 메시지를 전달하려고 할 수 있지만, 대신 서버가 메시지를 전달할 끝점을 찾을 수 없음을 나타내는 HTTP 상태 코드 404를 수신합니다. 이런 경우 누락된 메시지는 시간을 위해 비용을 지불하지 않거나 조직이 계약 자원에 대한 예산을 초과한다는 의미일 수 있습니다.

## 이벤트 구독 다시 시도를 위한 Adobe Workfront 전략

고객이 Workfront 플랫폼을 일상 지식 작업의 핵심 부분으로 활용하므로 Workfront 이벤트 구독 프레임워크는 각 메시지의 전달을 최대한 시도하도록 하는 메커니즘을 제공합니다.

최대 48시간 동안 게재될 때까지 고객 종단점으로 전달되지 않는 이벤트 트리거된 아웃바운드 메시지는 다시 전송됩니다. 이 시간 동안 게재가 성공하거나 48시간이 경과할 때까지 재시도는 점진적으로 단축되는 빈도에서 발생합니다.

고객은 Workfront 이벤트 구독의 아웃바운드 메시지를 사용하는 모든 엔드포인트가 게재가 성공하면 Workfront에 200 수준 응답 메시지를 다시 반환하도록 설정되도록 해야 합니다.

## 실패한 이벤트 트리거된 아웃바운드 메시지 처리

다음 순서도는 Workfront 이벤트 구독을 사용하여 메시지 게재를 다시 시도하는 전략을 보여줍니다.

![](assets/event-subscription-circuit-breaker-retries-350x234.png)

다음 설명은 순서도에 표시된 단계에 해당합니다.

1. 메시지를 배달하지 못했습니다.
1. 메시지 게재 실패 정보가 기록됩니다.

   메시지 게재 실패 시도가 모두 기록되므로 주어진 실패의 근본 원인 또는 일련의 실패를 확인하기 위해 디버깅을 수행할 수 있습니다.

1. URL 오류가 증가되었습니다.
1. 메시지 시도 카운트가 증가합니다.
1. 이 메시지의 전달을 다시 시도할 때까지 지연을 계산하십시오.
1. 메시지가 메시지 다시 시도 큐에 배치됩니다.

   이전 순서도에 표시된 대로, 메시지 전달 다시 시도를 처리하는 데 사용되는 메시지 큐는 각 메시지에 대한 초기 배달 시도를 처리하는 대기열과 별개입니다. 이를 통해 거의 실시간으로 메시지를 계속 전송할 수 있으므로 메시지 하위 집합 오류로 인해 방해 받지 않습니다.

1. URL 회로 상태가 평가됩니다. 다음 중 하나가 발생합니다.

   * 회로가 열려 있고 현재 게재를 허용하지 않는 경우 5단계에서 프로세스를 다시 시작합니다.
   * 회로가 반쯤 열려 있으면 회로가 현재 열려 있음을 의미하지만 URL을 테스트하여 배달에 대한 문제가 해결되었는지 확인할 수 있는 충분한 시간이 지나갔습니다.
   * 메시지 게재 시도 제한에 도달한 경우(48시간 다시 시도) 메시지가 삭제됩니다

1. URL 회로를 닫고 게재를 허용하는 경우 메시지 전달을 시도합니다. 이 게재가 실패하면 1단계에서 메시지가 다시 시작됩니다

1. URL 회로를 닫고 게재를 허용하는 경우 메시지 전달을 시도합니다. 이 게재가 실패하면 1단계에서 메시지가 다시 시작됩니다.

   <!--
   <li value="10" data-mc-conditions="QuicksilverOrClassic.Draft mode">Workfront disables Event Subscriptions when both of the following criteria are met:
   <ul>
   <!--
   <li data-mc-conditions="QuicksilverOrClassic.Draft mode">The Event Subscription has failed 1000 delivery attempts consecutively</li>
   <li data-mc-conditions="QuicksilverOrClassic.Draft mode">48 hours have passed since the last successful delivery</li>
   </ul></li>
   -->
