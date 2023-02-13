---
content-type: release-notes
keywords: 메모,분기별,업데이트,릴리스
navigation-topic: 2021-2-release-activity
title: 21.2 요청 개선 사항
description: 이 페이지에서는 미리 보기 환경에 대한 21.2 릴리스로 향상된 모든 요청을 설명합니다. 이러한 개선 사항은 2021년 5월 10일이 있는 프로덕션 환경에서 사용할 수 있습니다. 21.2 릴리스에서 사용할 수 있는 모든 변경 사항 목록은 21.2 릴리스 개요를 참조하십시오.
author: Luke
feature: Product Announcements
exl-id: af9c801f-ae40-439a-8749-ae8d178040ae
source-git-commit: 665732453b33b49421108791a560ab84d51280b9
workflow-type: tm+mt
source-wordcount: '1084'
ht-degree: 0%

---

# 21.2 요청 개선 사항

이 페이지에서는 미리 보기 환경에 대한 21.2 릴리스로 향상된 모든 요청을 설명합니다. 이러한 개선 사항은 2021년 5월 10일이 있는 프로덕션 환경에서 사용할 수 있습니다. 21.2 릴리스에서 사용할 수 있는 모든 변경 사항 목록에 대해서는 다음을 참조하십시오 [21.2 릴리스 개요](../../../product-announcements/product-releases/21.2-release-activity/21-2-release-overview.md).

## 새 요청에 대해 수행하는 지정 유형 제어

>[!NOTE]
>
>새 Adobe Workfront 경험에서만 사용할 수 있습니다.

일관성을 제공하고 사용자가 입력할 수 있는 할당 유형에 관계없이 항상 동일한 필드를 표시하도록 새 요청을 만들 때 지정 필드가 작동하는 방식을 변경했습니다.

요청 대기열을 설정할 때 [할당 대상], [작업 역할] 또는 [팀] 필드를 표시할 수 있도록 설정하면, 요청자는 이 세 가지 할당 유형 중 모두 또는 어느 하나를 수용할 수 있는 동일한 [할당] 필드를 보게 됩니다.

지정 필드에 허용되는 지정 유형에 대한 표시가 있습니다. 예를 들어, 요청 큐를 설정할 때 지정된 사람 및 팀 필드를 활성화하면 &quot;사람, 역할 또는 팀 검색&quot; 대신 &quot;사람 또는 팀 검색&quot;이라는 메시지가 표시됩니다.

자세한 내용은 다음 문서를 참조하십시오.

* [Adobe Workfront 요청 만들기 및 제출](/help/quicksilver/manage-work/requests/create-requests/create-submit-requests.md)
* [요청 큐 만들기](../../../manage-work/requests/create-and-manage-request-queues/create-request-queue.md)

## 요청 만들기 및 초안 관리 개선 사항

>[!NOTE]
>
>새 Adobe Workfront 경험에서만 사용할 수 있습니다.

새 Workfront 경험에서 요청 만들기에 대한 피드백을 계속 통합하면서 새 요청 워크플로우에 몇 가지 개선된 기능을 제공합니다. 다음과 같은 보고서가 포함됩니다.

* 표시 옵션 아이콘에 표시 선택 사항 아이콘을 사용하여 [요청 유형], [항목 그룹] 및 [큐 항목] 필드는 이전에 정의된 옵션을 선택할 수 있는 드롭다운 목록이라는 것을 명확하게 나타냅니다.
* 선택 후 요청 유형, 주제 그룹 또는 큐 주제에 대한 선택을 제거할 수 있다는 것을 &quot;x&quot; 아이콘에 명확하게 표시합니다.
* 초안을 잃지 않고 요청을 떠날 새 요청을 만들 때 닫기 단추를 제공합니다. 이 변경 사항 외에 &quot;취소&quot; 단추의 이름이 &quot;초안 무시&quot;로 변경되었습니다.

새 요청 만들기에 대한 내용은 [Adobe Workfront 요청 만들기 및 제출](/help/quicksilver/manage-work/requests/create-requests/create-submit-requests.md).

이 기능은 이제 [새로운 Workfront 경험을 위한 Collaborator Fundamentals](https://one.workfront.com/s/learningpath1/collaborator-fundamentals-for-the-new-workfront-experience-MCY5AMOQQTGFDVZB4ODS6TXCYE2A) Workfront One에서 학습 경로.

## 요청 워크플로우에 대한 개선 사항

>[!NOTE]
>
>이 기능은 새 Adobe Workfront 경험에서만 사용할 수 있습니다

계속해서 피드백을 수렴하고 통합할 때 Adobe에서는 Adobe Workfront과의 상호 작용을 보다 쉽고 직관적으로 수행할 수 있도록 새로운 요청 워크플로우에 몇 가지 개선 사항을 추가했습니다. 이러한 개선 사항은 다음과 같습니다.

* 큐 설정을 정의할 때 요청 대기열을 만들 때 파일 업로드를 위한 문서 섹션을 배치할 위치를 선택할 수 있습니다. 이 섹션은 요청 양식의 사용자 지정 필드 앞 또는 뒤로 배치할 수 있습니다. 자세한 내용은 [요청 큐 만들기](../../../manage-work/requests/create-and-manage-request-queues/create-request-queue.md).
* 이제 페이지에서 멀리 탐색하면 열 중 하나로 제출된 요청 목록을 정렬하는 작업이 유지됩니다. 자세한 내용은 [제출된 요청 찾기](../../../manage-work/requests/create-requests/locate-submitted-requests.md).
* 새 요청을 만들 때 이제 제출 및 취소 단추가 새 요청 양식 하단에 있습니다. 자세한 내용은 [Workfront 요청 만들기 및 제출](/help/quicksilver/manage-work/requests/create-requests/create-submit-requests.md).

이 기능은 이제 [새로운 Workfront 경험을 위한 Collaborator Fundamentals](https://one.workfront.com/s/learningpath1/collaborator-fundamentals-for-the-new-workfront-experience-MCY5AMOQQTGFDVZB4ODS6TXCYE2A) Workfront One에서 학습 경로.

## 요청 영역의 Submitted 섹션에서 요약 패널 열기

>[!NOTE]
>
>이 기능은 새 Adobe Workfront 경험에서만 사용할 수 있습니다.

Adobe Workfront의 모든 영역에서 경험이 일관되도록 하기 위해 요청 영역의 제출됨 섹션에 열기 요약 아이콘을 추가했습니다. 이제 제출된 문제에 대한 요약 패널을 열고 문제에 대한 자세한 정보를 보거나, 할당하거나, 문서나 설명을 추가할 수 있습니다.

제출된 요청에 대한 자세한 내용은 [제출된 요청 찾기](../../../manage-work/requests/create-requests/locate-submitted-requests.md).

이 기능은 이제 [새로운 Workfront 경험을 위한 Collaborator Fundamentals](https://one.workfront.com/s/learningpath1/collaborator-fundamentals-for-the-new-workfront-experience-MCY5AMOQQTGFDVZB4ODS6TXCYE2A) Workfront One에서 학습 경로.

## 새 요청 양식에서 제거된 새 문제 필드 가져오기

>[!NOTE]
>
>이 기능은 새 Adobe Workfront 경험에서만 사용할 수 있습니다.

이전 릴리스에서 시작된 새 요청 양식의 재설계로 새 요청을 제출할 때 프로젝트 큐 세부 정보 섹션의 새 문제 필드 영역에서 여러 필드가 표시되지 않도록 했습니다. 피드백을 포함하여 필드를 다시 가져오기로 결정했으므로 새 요청 양식에 모두 표시할 수 있습니다.

자세한 내용은 [요청 큐 만들기](../../../manage-work/requests/create-and-manage-request-queues/create-request-queue.md).

## 요청 영역에서 요청을 제출할 때의 새 경험

>[!NOTE]
>
>21.1 릴리스를 사용하여 미리 보기에 추가되지만 21.2 릴리스에서 프로덕션에 포함됩니다.

새 Workfront 환경과 일관성을 유지하고 요청을 제출할 때 효율성을 생성하기 위해 요청 영역에서 새 요청 상자를 다시 디자인했습니다. 다음은 몇 가지 개선 사항입니다.

* 새로운 Workfront 경험의 나머지 부분과 대조된 사용자 인터페이스입니다
* 더 쉽고 직관적인 경험을 위해 새 요청 영역을 제거했습니다
* 보다 효율적인 새로운 문서 요청 방식

요청을 입력할 때 요청 큐, 주제 그룹 또는 큐 항목에 대한 링크를 공유하는 기능.

요청 제출에 대한 자세한 내용은 [Workfront 요청 만들기 및 제출](/help/quicksilver/manage-work/requests/create-requests/create-submit-requests.md).

이 기능은 이제 [새로운 Workfront 경험을 위한 Collaborator Fundamentals](https://one.workfront.com/s/learningpath1/collaborator-fundamentals-for-the-new-workfront-experience-MCY5AMOQQTGFDVZB4ODS6TXCYE2A) Workfront One에서 학습 경로.

## 요청을 제출할 때 요청 큐에 대한 링크 공유

>[!NOTE]
>
>21.1 릴리스를 사용하여 미리 보기에 추가되지만 21.2 릴리스에서 프로덕션에 포함됩니다.

이제 요청을 만들 때 요청 큐, 항목 그룹 또는 큐 항목에 대한 링크를 공유할 수 있게 되었습니다.

새 요청을 제출하기 전에 링크를 요청 큐, 항목 그룹 또는 요청의 큐 항목에 복사하여 다른 사용자와 공유하거나 대시보드에 포함할 수 있습니다.

요청을 제출할 때 요청 큐에 대한 링크 공유에 대한 자세한 내용은 을 참조하십시오 [요청 큐에 대한 링크 공유](../../../manage-work/requests/create-requests/share-link-to-request-queue.md).

이 기능은 이제 [새로운 Workfront 경험을 위한 Collaborator Fundamentals](https://one.workfront.com/s/learningpath1/collaborator-fundamentals-for-the-new-workfront-experience-MCY5AMOQQTGFDVZB4ODS6TXCYE2A) Workfront One에서 학습 경로.
