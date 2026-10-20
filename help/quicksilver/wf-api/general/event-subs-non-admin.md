---
content-type: api
navigation-topic: general-api
title: 관리자가 아닌 사용자로 이벤트 구독 관리
description: Workfront 액세스가 허용되면 권한 및 시스템 구성에서 허용하는 범위 내에 있는 이벤트 구독을 만들고, 보고, 삭제할 수 있습니다.
author: Courtney
feature: Workfront API
role: Developer
source-git-commit: f0cde465a56d0cc936e8c886f4a120dec5fe5f73
workflow-type: tm+mt
source-wordcount: '342'
ht-degree: 5%
---

# 관리자가 아닌 사용자로 이벤트 구독 관리

Workfront 액세스가 허용되면 설정 영역에서 이벤트 구독을 만들고, 보고, 삭제할 수 있습니다. 그러나 액세스는 역할에 대해 그리고 조직의 시스템 구성에 의해 승인된 구독 및 작업으로 제한됩니다.

이 기능은 Workfront 관리자와 같은 방식으로 모든 사용자가 사용할 수 없습니다. 필요한 액세스 권한이 있는 사용자는 부여된 범위 내에서만 이벤트 구독을 관리할 수 있습니다.

예를 들어, 사용 권한을 사용하면 정의된 작업 세트에 대한 특정 개체 유형, 이벤트 유형 또는 구독만 관리할 수 있습니다. 액세스 및 구성에서 허용하는 범위 밖에서는 이벤트 구독을 관리할 수 없습니다.

관리자 관리 설정에 대해서는 [Workfront에서 이벤트 구독 구성](/help/quicksilver/administration-and-setup/manage-workfront/manage-event-subscriptions/configure-event-subscriptions-in-workfront.md)을 참조하십시오.

이벤트 구독 API에 대한 자세한 내용은 [이벤트 구독 API](/help/quicksilver/wf-api/general/event-subs-api.md)를 참조하십시오.

>[!NOTE]
>
>사용자는 자신의 권한과 조직의 시스템 구성이 허용하는 범위 내에서만 이벤트 구독을 관리할 수 있습니다. 액세스는 관리자 액세스와 자동으로 동일하지 않습니다.

## 액세스 요구 사항

+++ 이 문서의 기능에 대한 액세스 요구 사항을 보려면 확장하십시오.

<table style="table-layout:auto">
 <col>
 <col>
 <tbody>
  <tr>
   <td role="rowheader">Adobe Workfront 패키지</td>
   <td>Any</td>
  </tr>
  <tr>
   <td role="rowheader">Adobe Workfront 라이선스</td>
   <td>
    <p>표준</p>
    <p>플랜</p>
   </td>
  </tr>
  <tr>
   <td role="rowheader">액세스 수준 구성</td>
   <td>
    <p>이벤트 구독을 관리하려면 적절한 액세스 권한이 있어야 합니다.</p>
    <p>액세스는 권한 및 조직의 시스템 구성에서 허용된 구독 및 작업으로 제한됩니다.</p>
   </td>
  </tr>
 </tbody>
</table>

자세한 내용은 [Workfront 설명서의 액세스 요구 사항](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)을 참조하십시오.

+++

## 이벤트 구독 작업

{{step-1-to-setup}}

1. 왼쪽 탐색 패널에서 **시스템**&#x200B;을 클릭한 다음 **이벤트 구독**&#x200B;을 클릭합니다.
1. 사용 가능한 구독을 검토하십시오.
1. 승인된 범위 내에 있는 구독만 만들거나, 보거나, 삭제합니다.

예상한 옵션이 표시되지 않거나 구독을 만들거나 관리할 수 없는 경우 Workfront 관리자에게 문의하여 액세스 권한이 역할, 권한 또는 시스템 구성으로 제한되는지 확인하십시오.

## 관련 문서

* [Workfront에서 이벤트 구독 구성](/help/quicksilver/administration-and-setup/manage-workfront/manage-event-subscriptions/configure-event-subscriptions-in-workfront.md)
* [이벤트 구독 API](/help/quicksilver/wf-api/general/event-subs-api.md)
