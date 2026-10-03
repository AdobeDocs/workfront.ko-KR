---
user-type: administrator
content-type: how-to
product-area: system-administration
navigation-topic: manage-workfront
title: Workfront에서 이벤트 구독 구성
description: Adobe Workfront 관리자는 설정 영역에서 이벤트 구독을 만들고, 보고, 삭제하여 Workfront 이벤트를 외부 엔드포인트로 보낼 수 있습니다.
feature: System Setup and Administration
role: Admin
author: Courtney
source-git-commit: 5a44679115dcfda871e2fe40c0c8443649fc43cf
workflow-type: tm+mt
source-wordcount: '385'
ht-degree: 5%
---

# Workfront에서 이벤트 구독 구성

{{highlighted-preview-article-level}}

Adobe Workfront 관리자는 설정 영역에서 이벤트 구독을 만들고, 보고, 삭제할 수 있습니다. 이벤트 구독은 지정된 이벤트가 발생할 때 Workfront 이벤트 정보를 외부 끝점으로 보냅니다.

Workfront에서 이벤트 구독을 만들고 삭제할 수 있지만 기존 구독을 편집할 수는 없습니다. 구독을 변경해야 하는 경우 구독을 삭제하고 새 구독을 만드십시오.

이벤트 구독에 대한 자세한 내용은 [이벤트 구독](/help/quicksilver/wf-api/api/event-subscriptions.md)의 문서를 참조하십시오.

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
   <td>Workfront 관리자여야 합니다.</td>
  </tr>
 </tbody>
</table>

자세한 내용은 [Workfront 설명서의 액세스 요구 사항](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)을 참조하십시오.

+++

## 이벤트 구독 만들기

{{step-1-to-setup}}

1. 왼쪽 탐색 패널에서 **시스템**&#x200B;을 클릭한 다음 **이벤트 구독**&#x200B;을 클릭합니다.
1. **새 이벤트 구독**&#x200B;을 클릭합니다.
1. **개체** 필드에서 모니터링할 Workfront 개체를 선택합니다.
1. **이벤트 유형** 필드에서 개체를 만들거나 업데이트하거나 삭제하거나 공유할 때 이벤트 구독을 트리거할지 여부를 선택합니다.
1. **Webhook URL** 필드에 이벤트 페이로드를 받을 끝점을 입력합니다.
1. **인증 토큰** 필드에 엔드포인트에 대한 요청을 인증하는 데 사용되는 토큰을 입력하십시오.
1. Workfront에서 페이로드를 전송하기 전에 인코딩하도록 하려면 페이로드를 Base64로 전송하는 옵션을 활성화합니다.
1. 필요한 경우 하나 이상의 필터를 추가하여 구독을 트리거하는 이벤트를 제한합니다. 사용 가능한 필터는 선택한 개체를 기반으로 합니다.
1. Click **Create**.

끝점 요구 사항에 대한 자세한 내용은 [이벤트 구독 배달 요구 사항](/help/quicksilver/wf-api/general/setup-event-sub-endpoint.md)을 참조하십시오.

## 이벤트 구독 보기

{{step-1-to-setup}}

1. 왼쪽 탐색 패널에서 **시스템**&#x200B;을 클릭한 다음 **이벤트 구독**&#x200B;을 클릭합니다.

이벤트 구독 페이지에서 환경에 대해 구성된 구독을 검토할 수 있습니다. 조직에 있는 총 구독 수와 이러한 구독 중 활성, 비활성화 또는 동결된 구독 수를 확인할 수 있습니다.

* **비활성화된 구독**: 반복된 게재 오류로 인해 이러한 구독이 자동으로 비활성화되었습니다.
* **동결된 구독**: 이 구독은 게재 문제로 인해 일시적으로 중단됩니다.

## 이벤트 구독 삭제

{{step-1-to-setup}}

1. 왼쪽 탐색 패널에서 **시스템**&#x200B;을 클릭한 다음 **이벤트 구독**&#x200B;을 클릭합니다.
1. 제거할 이벤트 구독을 선택합니다.
1. **삭제**&#x200B;를 클릭합니다.
