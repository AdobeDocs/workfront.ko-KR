---
content-type: api
navigation-topic: general-api
title: 이벤트 구독 모범 사례
description: 이벤트 구독 모범 사례
author: Becky
feature: Workfront API
role: Developer
exl-id: 2c6e3567-d5eb-4528-a393-dbf235958ed2
source-git-commit: 3a538a15daad5fa0dced8d45bb260d6087be81ff
workflow-type: tm+mt
source-wordcount: '355'
ht-degree: 0%

---


# 이벤트 구독 모범 사례

서비스를 올바르게 구성하고 이러한 메시지 게재를 트리거하기 위한 이벤트 구독을 만든 후 Adobe Workfront 이벤트 구독 메시지가 Workfront에서 자동으로 전송됩니다. 이벤트 구독을 올바르게 설정하는 방법에 대한 자세한 내용은 [이벤트 구독 게재 요구 사항](../../wf-api/general/setup-event-sub-endpoint.md)을 참조하십시오.


다음은 이벤트 구독을 효과적으로 만드는 데 도움이 되는 몇 가지 모범 사례입니다.

## 모든 필수 요청 본문 필드 제공

모든 필수 요청 본문 필드가 API에 제공되었는지 확인하십시오. 필요한 모든 요청 특성에 대한 자세한 내용은 [이벤트 구독 API](../../wf-api/general/event-subs-api.md)를 참조하십시오.

## 추가 본문 필드를 포함하지 않음

요청에 추가 본문 필드를 포함하지 마십시오. 그렇게 하면 API에서 구독을 만들지 못합니다.

## 이벤트 구독 오버로드 방지

이벤트 구독 서비스는 모든 사용자에게 이벤트를 안정적으로 전달하도록 설계되었습니다. 이를 위해 단일 사용자의 과도한 이벤트 생성으로 모든 사용자에게 잠재적인 서비스 품질 문제가 발생할 수 있는 것을 방지하기 위한 안전 장치를 마련했다. 따라서 짧은 시간 내에 너무 많은 이벤트를 높은 비율로 생성하는 사용자는 샌드박싱과 이벤트 전달 지연을 경험할 수 있습니다.

## 유예 기간 내에 테스트 완료

100개의 메시지 유예 기간 내에 모든 구독 테스트를 완료해 보십시오. 이 유예 기간에 대한 자세한 내용은 [FAQ - 이벤트 구독](../../wf-api/general/event-subs-faq.md)을 참조하세요.

## 표준 이벤트 구독 메시지 게재 요구 사항 충족

구독 끝점이 표준 이벤트 구독 메시지 게재 요구 사항을 준수하는지 확인하십시오. 이러한 요구 사항에 대해 알아보려면 [이벤트 구독 배달 요구 사항](../../wf-api/general/setup-event-sub-endpoint.md)을 참조하세요.

## 허용 목록에 추가하다 전역 IP 주소

허용 목록에 추가하다 이벤트 구독 페이로드를 방화벽을 통해 수신하려면 글로벌 영역별로 IP 주소를 방화벽에 추가해야 합니다. 자세한 내용은 [이벤트 구독 API](../../wf-api/general/event-subs-api.md)를 참조하세요.

## 적절한 액세스 수준 및 인증 보유

이벤트 구독을 생성, 쿼리 또는 삭제하려면 Workfront 사용자가 필요합니다.

* **시스템 관리자**&#x200B;의 액세스 수준
자세한 내용은 [사용자에게 전체 관리 액세스 권한 부여](../../administration-and-setup/add-users/configure-and-grant-access/grant-a-user-full-administrative-access.md) 또는 [사용자에게 특정 영역에 대한 관리 액세스 권한 부여](../../administration-and-setup/add-users/configure-and-grant-access/grant-users-admin-access-certain-areas.md)를 참조하십시오.

* 조직에서 Adobe IMS(Identity Management System)를 사용하는 경우 `X-User-Token` 헤더에 전달된 IMS 사용자 토큰을 포함합니다.
