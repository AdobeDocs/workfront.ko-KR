---
content-type: release-notes
keywords: 메모,분기별,업데이트,릴리스
navigation-topic: 2021-2-release-activity
title: 21.2 요청 개선 사항
description: 이 페이지에서는 미리보기 환경에 대한 21.2 릴리스의 모든 요청 개선 사항에 대해 설명합니다. 이러한 개선 사항은 2021년 5월 10일이 있는 주에 프로덕션 환경에서 사용할 수 있습니다. 21.2 릴리스에서 사용할 수 있는 모든 변경 사항 목록은 21.2 릴리스 개요 를 참조하십시오.
author: Luke
feature: Product Announcements
recommendations: noDisplay, noCatalog
exl-id: af9c801f-ae40-439a-8749-ae8d178040ae
source-git-commit: b18a7835c6de131c125b77c6688057638c62fa4a
workflow-type: tm+mt
source-wordcount: '1053'
ht-degree: 0%

---

# 21.2 요청 개선 사항

이 페이지에서는 미리보기 환경에 대한 21.2 릴리스의 모든 요청 개선 사항에 대해 설명합니다. 이러한 개선 사항은 2021년 5월 10일이 있는 주에 프로덕션 환경에서 사용할 수 있습니다. 21.2 릴리스에서 사용할 수 있는 모든 변경 사항 목록을 보려면 [21.2 릴리스 개요](../../../product-announcements/product-releases/21.2-release-activity/21-2-release-overview.md)를 참조하십시오.

## 새 요청에 대해 수행하는 할당 유형을 제어합니다.

>[!NOTE]
>
>새로운 Adobe Workfront 경험에서만 사용할 수 있습니다.

일관성을 제공하고 사용자가 입력할 수 있는 할당 유형에 관계없이 항상 동일한 필드를 표시하도록 새 요청을 만들 때 할당 필드가 작동하는 방식을 변경했습니다.

요청 대기열을 설정할 때 할당 대상, 작업 역할 또는 팀 필드가 표시되도록 설정하면 요청자에게 이 세 가지 할당 유형 모두 또는 모두를 수용할 수 있는 동일한 할당 필드가 표시됩니다.

할당 필드에는 허용되는 할당 유형이 표시됩니다. 예를 들어, 요청 대기열을 설정할 때 할당 대상 및 팀 필드를 활성화한 경우 &quot;사람, 역할 또는 팀 검색&quot; 대신 &quot;사람 또는 팀 검색&quot;을 선택하라는 메시지가 표시됩니다.

자세한 내용은 다음 문서를 참조하십시오.

* [Adobe Workfront 요청 만들기 및 제출](/help/quicksilver/manage-work/requests/create-requests/create-submit-requests.md)
* [요청 대기열 만들기](../../../manage-work/requests/create-and-manage-request-queues/create-request-queue.md)

## 요청 생성 및 초안 관리 개선 사항

>[!NOTE]
>
>새로운 Adobe Workfront 경험에서만 사용할 수 있습니다.

새로운 Workfront 경험에서 요청을 만드는 방법에 대한 피드백을 계속 통합하면서 새로운 요청 워크플로에 대한 몇 가지 사항이 개선되었습니다. 여기에는 다음이 포함됩니다.

* 옵션 표시 아이콘을 사용하여 요청 유형, 주제 그룹 및 대기열 주제 필드가 이전에 정의한 옵션을 선택할 수 있는 드롭다운 목록임을 명확히 표시합니다.
* 요청 유형, 주제 그룹 또는 대기열 주제를 선택한 후에는 제거할 수 있음을 &quot;x&quot; 아이콘으로 명확하게 표시합니다.
* 초안을 손실하지 않고 요청을 떠나도록 새 요청을 만들 때 닫기 단추를 제공합니다. 이 변경 사항 외에 &quot;폐기&quot; 버튼의 이름이 &quot;초안 폐기&quot;로 변경되었습니다.

새 요청 만들기에 대한 자세한 내용은 [Adobe Workfront 요청 만들기 및 제출](/help/quicksilver/manage-work/requests/create-requests/create-submit-requests.md)을 참조하십시오.

이 기능은 이제 Workfront One의 [새 Workfront 경험을 위한 공동 작업자 기본 사항](https://experienceleague.adobe.com/ko/docs/workfront-learn/tutorials-workfront/manage-work/issues-requests/make-a-request)에 포함되어 있습니다.

## 요청 워크플로에 대한 개선 사항

>[!NOTE]
>
>이 기능은 새로운 Adobe Workfront 환경에서만 사용할 수 있습니다

귀하의 피드백을 계속 듣고 통합함에 따라 Adobe Workfront과의 상호 작용을 더 쉽고 직관적으로 할 수 있도록 새로운 요청 워크플로에 몇 가지 개선 사항을 추가했습니다. 향상된 기능은 다음과 같습니다.

* 대기열 설정을 정의할 때 요청 대기열을 만들 때 파일 업로드를 위해 문서 섹션을 배치할 위치를 선택할 수 있습니다. 이 섹션은 요청 양식의 사용자 정의 필드 앞 또는 뒤에 배치할 수 있습니다. 자세한 내용은 [요청 큐 만들기](../../../manage-work/requests/create-and-manage-request-queues/create-request-queue.md)를 참조하세요.
* 이제 페이지에서 나가면 열 중 하나를 기준으로 제출된 요청 목록 정렬이 유지됩니다. 자세한 내용은 [제출된 요청 찾기](../../../manage-work/requests/create-requests/locate-submitted-requests.md)를 참조하십시오.
* 이제 새 요청을 만들 때 제출 및 취소 버튼이 새 요청 양식 하단에 있습니다. 자세한 내용은 [Workfront 요청 만들기 및 제출](/help/quicksilver/manage-work/requests/create-requests/create-submit-requests.md)을 참조하십시오.

이 기능은 이제 Workfront One의 [새 Workfront 경험을 위한 공동 작업자 기본 사항](https://experienceleague.adobe.com/ko/docs/workfront-learn/tutorials-workfront/manage-work/issues-requests/make-a-request)에 포함되어 있습니다.

## 요청 영역의 제출됨 섹션에서 요약 패널 열기

>[!NOTE]
>
>이 기능은 새로운 Adobe Workfront 환경에서만 사용할 수 있습니다.

Adobe Workfront의 모든 영역에서 경험을 일관되게 유지하기 위해 요약 열기 아이콘을 요청 영역의 제출됨 섹션에 추가했습니다. 이제 제출된 문제에 대한 요약 패널을 열고 문제에 대한 자세한 내용을 보고 할당하거나 문서 또는 댓글을 추가할 수 있습니다.

제출된 요청에 대한 자세한 내용은 [제출된 요청 찾기](../../../manage-work/requests/create-requests/locate-submitted-requests.md)를 참조하십시오.

이 기능은 이제 Workfront One의 [새 Workfront 경험을 위한 공동 작업자 기본 사항](https://experienceleague.adobe.com/ko/docs/workfront-learn/tutorials-workfront/manage-work/issues-requests/make-a-request)에 포함되어 있습니다.

## 새 요청 양식에서 제거된 새 문제 필드 다시 가져오기

>[!NOTE]
>
>이 기능은 새로운 Adobe Workfront 환경에서만 사용할 수 있습니다.

이전 릴리스와 함께 시작된 새 요청 양식 재설계로 인해 새 요청을 제출할 때 프로젝트 대기열 세부 정보 섹션의 새 문제 필드 영역에 표시되는 여러 필드를 방지할 수 있었습니다. 피드백을 통합한 후 필드를 다시 가져와 모든 필드를 새 요청 양식에 표시하도록 결정했습니다.

자세한 내용은 [요청 큐 만들기](../../../manage-work/requests/create-and-manage-request-queues/create-request-queue.md)를 참조하세요.

## 요청 영역에서 요청을 제출할 때의 새로운 경험

>[!NOTE]
>
>21.1 릴리스로 미리보기에 추가되지만 프로덕션 환경에는 21.2 릴리스에 포함됩니다.

요청을 제출할 때 새로운 Workfront 경험과의 일관성을 확보하고 효율성을 창출하기 위해 요청 영역에서 새 요청 상자를 다시 설계했습니다. 다음은 몇 가지 개선 사항입니다.

* 는 새 Workfront 경험의 나머지와 함께 구성된 사용자 인터페이스입니다
* 보다 쉽고 직관적인 경험을 위해 새 요청 영역을 제거했습니다.
* 요청에 문서를 첨부하는 새롭고 효율적인 방법

요청을 입력할 때 요청 대기열, 주제 그룹 또는 대기열 주제에 대한 링크를 공유하는 기능.

요청 제출에 대한 자세한 내용은 [Workfront 요청 만들기 및 제출](/help/quicksilver/manage-work/requests/create-requests/create-submit-requests.md)을 참조하십시오.

이 기능은 이제 Workfront One의 [새 Workfront 경험을 위한 공동 작업자 기본 사항](https://experienceleague.adobe.com/ko/docs/workfront-learn/tutorials-workfront/manage-work/issues-requests/make-a-request)에 포함되어 있습니다.

## 요청을 제출할 때 요청 대기열에 대한 링크 공유

>[!NOTE]
>
>21.1 릴리스로 미리보기에 추가되지만 프로덕션 환경에는 21.2 릴리스에 포함됩니다.

이제 요청을 만들 때 요청 대기열, 주제 그룹 또는 대기열 주제에 대한 링크를 공유할 수 있습니다.

새 요청을 제출하기 전에 요청 대기열, 주제 그룹 또는 요청의 대기열 주제에 대한 링크를 복사하여 다른 사용자와 공유하거나 대시보드에 포함할 수 있습니다.

요청을 제출할 때 요청 대기열에 대한 링크를 공유하는 방법에 대한 자세한 내용은 [요청 대기열에 대한 링크 공유](../../../manage-work/requests/create-requests/share-link-to-request-queue.md)를 참조하십시오.

이 기능은 이제 Workfront One의 [새 Workfront 경험을 위한 공동 작업자 기본 사항](https://experienceleague.adobe.com/ko/docs/workfront-learn/tutorials-workfront/manage-work/issues-requests/make-a-request)에 포함되어 있습니다.
