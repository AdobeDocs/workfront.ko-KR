---
product-area: projects
navigation-topic: manage-issues
title: 피드백 대기에서 진행 중으로 문제 상태 자동 업데이트
description: 문제의 기본 연락처가 필드(사용자 지정 필드 포함)를 업데이트하거나 주석을 추가하여 문제를 업데이트하면 문제 상태가 자동으로 진행 중으로 업데이트됩니다.
author: Alina
feature: Work Management
exl-id: f94bb644-910f-4b46-80fd-fecbdf9cb18a
source-git-commit: f2f825280204b56d2dc85efc7a315a4377e551c7
workflow-type: tm+mt
source-wordcount: '222'
ht-degree: 0%

---

# 피드백 대기에서 진행 중으로 문제 상태 자동 업데이트

문제의 기본 연락처가 필드(사용자 지정 필드 포함)를 업데이트하거나 주석을 추가하여 문제를 업데이트하면 문제 상태가 자동으로 진행 중으로 업데이트됩니다.

이러한 자동 상태를 변경하려면 다음 조건을 충족해야 합니다.

* 요청 큐를 통해 문제를 입력해야 합니다.

   요청 큐 만들기에 대한 내용은 [요청 큐 만들기 및 관리](../../../manage-work/requests/create-and-manage-request-queues/create-manage-request-queues.md) 섹션을 참조하십시오. 요청 만들기에 대한 내용은 [Adobe Workfront 요청 만들기 및 제출](../../../manage-work/requests/create-requests/create-submit-requests.md).

* 요청 큐의 큐 세부 정보에는 다음 설정이 있어야 합니다.
   * **누군가가 요청을 하면 자동으로 승인합니다** 가 로 설정되어 있습니다. **Contribute 액세스**
   * **상태 변경** 고급 설정에서 을 선택합니다.

   ![[대기열 세부 정보]를 선택하면 Contribute 액세스 및 변경 상태가 선택됩니다.](assets/queuedetails-contributeaccess-changestatus.png)

   큐 세부 정보에 대한 자세한 내용은 [요청 큐 만들기](../../../manage-work/requests/create-and-manage-request-queues/create-request-queue.md).

* 문제는 피드백 대기 상태여야 합니다.
* 시스템 수준의 문제에 사용할 수 있는 피드백 대기(AWF) 상태가 있어야 합니다.

   시스템 수준 상태에 대한 자세한 내용은 [상태 만들기 또는 편집](../../../administration-and-setup/customize-workfront/creating-custom-status-and-priority-labels/create-or-edit-a-status.md).
