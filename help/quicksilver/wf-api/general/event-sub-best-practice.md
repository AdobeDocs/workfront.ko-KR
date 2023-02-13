---
content-type: api
navigation-topic: general-api
title: 이벤트 구독 우수 사례
description: 이벤트 구독 우수 사례
author: John
feature: Workfront API
exl-id: 2c6e3567-d5eb-4528-a393-dbf235958ed2
source-git-commit: 50675b7af3fcd2188a18391732a93a7b67454db9
workflow-type: tm+mt
source-wordcount: '269'
ht-degree: 0%

---


# 이벤트 구독 우수 사례

Adobe Workfront 이벤트 구독 메시지는 서비스를 올바르게 구성하고 이벤트 구독을 만들어 메시지 게재를 트리거하면 Workfront에서 자동으로 전송됩니다. 이벤트 구독을 제대로 설정하는 방법에 대한 자세한 내용은 [이벤트 구독 게재 요구 사항](../../wf-api/general/setup-event-sub-endpoint.md).


아래 나열된 몇 가지 우수 사례는 이벤트 구독을 효과적으로 만드는 데 도움이 됩니다.

## 모든 필수 요청 본문 필드를 제공합니다

모든 필수 요청 본문 필드가 API에 제공되는지 확인하십시오. 모든 필수 요청 속성에 대한 자세한 내용은 [이벤트 구독 API](../../wf-api/general/event-subs-api.md).

## 추가 본문 필드를 포함하지 마십시오

요청에 추가 본문 필드를 포함하지 마십시오. 이 경우 API에서 구독을 만들지 못하는 오류가 발생합니다.

## 유예 기간 내에 테스트 완료

100개 메시지 유예 기간 내에 모든 구독 테스트를 수행해 보십시오. 이 유예 기간에 대한 자세한 내용은 [FAQ - 이벤트 구독](../../wf-api/general/event-subs-faq.md).

## 표준 이벤트 구독 메시지 전달 요구 사항 충족

구독 종단점이 표준 이벤트 구독 메시지 배달 요구 사항을 준수하는지 확인합니다. 이러한 요구 사항에 대해 알아보려면 [이벤트 구독 게재 요구 사항](../../wf-api/general/setup-event-sub-endpoint.md).

## 글로벌 허용 목록에 추가하다 지역별 IP 주소

방화벽을 통해 이벤트 구독 페이로드를 수신하려면 글로벌 지역별 IP 주소허용 목록에 추가하다를에 추가해야 합니다. 자세한 내용은 [이벤트 구독 API](../../wf-api/general/event-subs-api.md).

## 올바른 액세스 수준 및 API 키 보유

이벤트 구독을 만들거나, 쿼리하거나, 삭제하려면 Workfront 사용자에게 다음이 필요합니다.

* 액세스 수준 **시스템 관리자**
자세한 내용은 [사용자에게 전체 관리자 액세스 권한 부여](../../administration-and-setup/add-users/configure-and-grant-access/grant-a-user-full-administrative-access.md) 또는 [특정 영역에 대한 관리자 액세스 권한 부여](../../administration-and-setup/add-users/configure-and-grant-access/grant-users-admin-access-certain-areas.md).

* API 키

   <!--
  <p data-mc-conditions="QuicksilverOrClassic.Draft mode">To learn more, see .</p>
  -->
