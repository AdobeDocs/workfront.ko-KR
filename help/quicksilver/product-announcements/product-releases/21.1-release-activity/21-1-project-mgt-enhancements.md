---
content-type: release-notes
keywords: 메모,분기별,업데이트
navigation-topic: product-releases
title: 21.1 프로젝트 관리 개선 사항
description: 이 페이지에서는 미리 보기 환경에 대한 21.1 릴리스로 향상된 프로젝트 관리 기능에 대해 설명합니다. 이러한 개선 사항은 2021년 2월 15일이 있는 프로덕션 환경에서 사용할 수 있습니다.
author: Luke
feature: Product Announcements
exl-id: 95e75a28-5ac2-4d1d-acc3-dbc0b295b28f
source-git-commit: 665732453b33b49421108791a560ab84d51280b9
workflow-type: tm+mt
source-wordcount: '972'
ht-degree: 1%

---

# 21.1 프로젝트 관리 개선 사항

이 페이지에서는 미리 보기 환경에 대한 21.1 릴리스로 향상된 프로젝트 관리 기능에 대해 설명합니다. 이러한 개선 사항은 2021년 2월 15일이 있는 프로덕션 환경에서 사용할 수 있습니다.

21.1 릴리스에서 사용할 수 있는 모든 변경 사항 목록에 대해서는 다음을 참조하십시오 [21.1 릴리스 개요](../../../product-announcements/product-releases/21.1-release-activity/21-1-release-overview.md).

## 이제 프로젝트의 지표 섹션에서 내보내기를 사용할 수 있습니다

이제 프로젝트의 상태와 진행 상태를 보다 쉽게 공유하기 위해 프로젝트의 지표 섹션에 있는 전체 대시보드를 .png 파일로 내보낼 수 있습니다.

자세한 내용은 [프로젝트 지표 개요](../../../manage-work/projects/manage-projects/project-metrics.md).

이 기능은 이제 [새로운 Workfront 경험을 위한 계획자 기초, 3부: 프로젝트 관리](https://one.workfront.com/s/learningpath3/planner-fundamentals-for-the-new-workfront-experience-part-3-manage-a-project-MCG6OJL724XRBLHBXEAKGAUZOJ6U) Workfront One에서 학습 경로.

## 프로젝트 또는 작업이 문제 업데이트에서 전환되면 문제 완료율을 업데이트합니다

Adobe는 프로젝트 또는 작업으로 전환된 문제에 대해 문제 완료율이 작동하는 방식을 업데이트했습니다. 새 기능을 사용하면, 문제가 작업 또는 프로젝트로 변환되면 &quot;개체 변경 해결&quot; 설정의 상태가 설정되면 &quot;해결 가능 문제 상태 자동 업데이트&quot; 설정이 활성화되면 문제 완료가 완료된 작업 또는 프로젝트의 완료율과 동기화되어 업데이트 완료율이 업데이트됩니다.

변환 문제에 대한 자세한 내용은 [해결 가능한 객체 해결 및 해결 방법 개요](../../../manage-work/issues/convert-issues/resolving-and-resolvable-objects.md).

## 새 제출된 요청 목록

보다 쉽고 일관되게 제출된 요청을 관리할 수 있도록 하기 위해, Adobe에서는 요청 영역에서 내가 제출한 요청 및 모든 요청 섹션을 제거하고 새 제출됨 목록으로 대체했습니다. 이 목록에는 시스템의 다른 모든 목록과 일치하는 친숙한 모양과 분위기가 있습니다. 이렇게 하면 제출된 요청의 다른 카테고리를 필터링하고 찾기 어려울 수 있는 요청을 빠르게 검색할 수 있습니다.

제출된 요청을 찾는 방법에 대한 자세한 내용은 [제출된 요청 찾기](../../../manage-work/requests/create-requests/locate-submitted-requests.md).

이 기능은 이제 [새로운 Workfront 경험을 위한 Collaborator Fundamentals](https://one.workfront.com/s/learningpath1/collaborator-fundamentals-for-the-new-workfront-experience-MCY5AMOQQTGFDVZB4ODS6TXCYE2A) Workfront One에서 학습 경로.

이 기능은 이제 [새 Workfront 경험의 요청](https://one.workfront.com/s/learningpath3/core-team-requests-in-the-new-workfront-experience-MCHWSSDWRFC5EKXFBXTQ6MJNKE7E) Workfront One에서 학습 경로.

## 새 요청 페이지에서 제거된 필드

>[!NOTE]
>
>릴리스에서 제거되었습니다.

새 요청 페이지의 재설계의 일부로, 프로젝트의 큐 설정 섹션에 설정된 새 문제 필드를 업데이트했습니다.

다음 새 문제 필드는 프로젝트의 문제 섹션에서 문제를 생성할 때만 표시됩니다. 요청 영역에서 요청 큐를 사용하여 문제를 제출할 때는 표시되지 않습니다.

* 심각도
* 계획된 시간
* 계획된 시작 일자
* URL
* 할당 대상:
* 작업 역할
* 팀

새 요청을 제출할 때 공통 필드에서 사용자, Job 역할 또는 팀을 효율적으로 지정하기 위해 지정된 대상, Job 역할 및 팀 필드를 새 요청 페이지의 새 지정 필드로 대체했습니다.

프로젝트에 대한 새 문제 필드 정의에 대한 자세한 내용은 [요청 큐 만들기](../../../manage-work/requests/create-and-manage-request-queues/create-request-queue.md).

## 요청 영역에서 요청을 제출할 때의 새 경험

>[!NOTE]
>
>릴리스에서 제거됨; 는 21.2를 사용하여 미리 보기 및 프로덕션에 유지됩니다.

새 Workfront 환경과 일관성을 유지하고 요청을 제출할 때 효율성을 생성하기 위해 요청 영역에서 새 요청 상자를 다시 디자인했습니다. 다음은 몇 가지 개선 사항입니다.

* 새로운 Workfront 경험의 나머지 부분과 대조된 사용자 인터페이스입니다
* 더 쉽고 직관적인 경험을 위해 새 요청 영역을 제거했습니다
* 보다 효율적인 새로운 문서 요청 방식

요청을 입력할 때 요청 큐, 주제 그룹 또는 큐 항목에 대한 링크를 공유하는 기능.

요청 제출에 대한 자세한 내용은 [Workfront 요청 만들기 및 제출](/help/quicksilver/manage-work/requests/create-requests/create-submit-requests.md).

## 요청을 제출할 때 요청 큐에 대한 링크 공유

>[!NOTE]
>
>릴리스에서 제거됨; 는 21.2를 사용하여 미리 보기 및 프로덕션에 유지됩니다.

이제 요청을 만들 때 요청 큐, 항목 그룹 또는 큐 항목에 대한 링크를 공유할 수 있게 되었습니다.

새 요청을 제출하기 전에 링크를 요청 큐, 항목 그룹 또는 요청의 큐 항목에 복사하여 다른 사용자와 공유하거나 대시보드에 포함할 수 있습니다.

요청을 제출할 때 요청 큐에 대한 링크 공유에 대한 자세한 내용은 을 참조하십시오 [요청 큐에 대한 링크 공유](../../../manage-work/requests/create-requests/share-link-to-request-queue.md).

## 프로젝트에 지정할 그룹을 검색하고 세부 정보를 봅니다

이제 프로젝트에 그룹을 할당할 때 올바른 그룹을 식별하는 것이 더 쉽습니다. 그룹 상자에 있는 그룹 이름을 마우스로 가리킨 다음 이름 옆에 표시되는 정보 아이콘을 클릭하여 그룹 세부 정보 도구 설명을 확인합니다.

이 도구 설명에는 그룹 위에 있는 그룹 계층(있는 경우)과 그룹 관리자가 포함됩니다.

그룹에 대해 구성된 세부 정보에 따라 그룹의 비즈니스 리더 및 설명이 표시될 수도 있습니다.

이 정보를 사용하면 프로젝트에 지정할 올바른 그룹을 선택한다는 것을 확신할 수 있습니다.

자세한 내용은 [프로젝트 개요 영역의 정보 관리](../../../manage-work/projects/manage-projects/understand-project-overview-area.md).

## 새 사용자 위임 보고서

이전에는 작업, 문제 및 프로젝트 승인 위임에 대한 정보를 해당 홈 영역에서 대리자만 볼 수 있었습니다. 이제 계획 사용자는 다른 사용자가 이 정보를 볼 수 있도록 사용자에게 알리는 사용자 위임 보고서를 생성할 수 있습니다.

* 이러한 승인을 다른 사용자에게 위임한 사람
* 이러한 승인을 받은 사용자
* 이러한 위임의 시작 및 종료 일자

자세한 내용은 [사용자 위임 보고서 만들기](../../../reports-and-dashboards/reports/creating-and-managing-reports/create-user-delegation-report.md).
