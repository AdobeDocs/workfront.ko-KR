---
product-area: projects
navigation-topic: manage-issues
title: 문제 상태를 피드백 대기에서 진행 중으로 자동 업데이트
description: 문제의 기본 담당자가 필드(사용자 정의 필드 포함)를 업데이트하거나 댓글을 추가하여 문제를 업데이트하면 문제 상태가 자동으로 진행 중으로 업데이트됩니다.
author: Alina
feature: Work Management
exl-id: f94bb644-910f-4b46-80fd-fecbdf9cb18a
source-git-commit: 393f858ba3711b367cf06ad846ea60be0d6d9034
workflow-type: tm+mt
source-wordcount: '281'
ht-degree: 0%

---

# 문제 상태를 피드백 대기에서 진행 중으로 자동 업데이트

<!--Audited: 109/2025-->

문제의 기본 담당자가 필드(사용자 정의 필드 포함)를 업데이트하거나 댓글을 추가하여 문제를 업데이트하면 문제 상태가 자동으로 진행 중으로 업데이트됩니다.

이 자동 상태 변경이 발생하려면 다음 조건을 충족해야 합니다.

* 이 문제는 요청 대기열을 사용하여 추가해야 합니다.

  요청 큐 만들기에 대한 자세한 내용은 [요청 큐 만들기 및 관리](../../../manage-work/requests/create-and-manage-request-queues/create-manage-request-queues.md) 섹션을 참조하십시오.

  요청 대기열에 요청을 제출하는 방법에 대한 자세한 내용은 [Adobe Workfront 요청 만들기 및 제출](../../../manage-work/requests/create-requests/create-submit-requests.md)을 참조하십시오.

* 요청 대기열의 대기열 세부 정보에 다음 설정이 있어야 합니다.
   * **다른 사람이 요청을 하면 자동으로 부여**&#x200B;가 **액세스 권한 제공**(으)로 설정됩니다.
   * **상태 변경**&#x200B;이 선택됨

  ![큐 세부 정보에서 Contribute 액세스 및 상태 변경을 선택할 수 있습니다.](assets/queuedetails-contributeaccess-changestatus.png)

  >[!IMPORTANT]
  >
  >  요청 대기열을 설정할 때 기본 담당자가 제출하는 문제에 대한 액세스 권한을 정의할 수 있습니다.
  >
  >요청 대기열을 설정할 때 상태 변경 설정을 선택 해제할 경우 요청 대기열 설정에서 상태 변경 옵션을 선택 해제한 경우에도 시스템 관리자는 항상 문제 상태를 변경할 수 있는 액세스 권한을 보유합니다.

  대기열 세부 정보에 대한 자세한 내용은 [요청 대기열 만들기](../../../manage-work/requests/create-and-manage-request-queues/create-request-queue.md)를 참조하십시오.

* 문제는 피드백 대기 중 상태여야 합니다.
* 시스템 수준의 문제에 사용할 수 있는 피드백 대기(AWF) 상태가 있어야 합니다.

  시스템 수준 상태에 대한 자세한 내용은 [상태 만들기 또는 편집](../../../administration-and-setup/customize-workfront/creating-custom-status-and-priority-labels/create-or-edit-a-status.md)을 참조하세요.
