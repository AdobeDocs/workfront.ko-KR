---
product-area: projects
navigation-topic: issue-information
title: 문제 계획된 완료 일자 개요
description: 문제의 계획된 완료 일자는 문제가 완료될 것으로 예상되는 일자입니다.
author: Alina
feature: Work Management
exl-id: bdb206dc-18f8-4f8a-862b-e881408a8408
source-git-commit: 1e69d715f343bfef1e5aee658a1dff12abfc61a0
workflow-type: tm+mt
source-wordcount: '592'
ht-degree: 0%

---

# 문제 계획된 완료 일자 개요

문제의 계획된 완료 일자는 문제가 완료될 것으로 예상되는 일자입니다.

문제의 계획된 완료 일자 를 지정하거나 특정 기준에 따라 Adobe Workfront에 맡겨 계산할 수 있습니다.

문제의 계획된 완료 일자는 프로젝트의 계획된 완료 일자에 영향을 주지 않습니다. 작업의 계획된 완료 일자만 프로젝트의 계획된 완료 일자에 영향을 줍니다. 프로젝트 계획 완료 날짜에 대한 자세한 내용은 [프로젝트 계획 완료 일자 설정](../../../manage-work/projects/planning-a-project/project-planned-completion-date.md)을 참조하십시오.

>[!NOTE]
>
>문제의 계획된 완료 일자는 다음과 같은 방식으로 문제의 커밋 일자 또는 문제의 예상 완료 일자와 다릅니다.
>
>* 커밋 일자는 문제에 할당된 사용자가 문제를 완료할 것으로 수동으로 예상하는 일자입니다. 자세한 내용은 다음 문서를 참조하십시오.
>
>   * [커밋 일자 개요](../../../manage-work/projects/updating-work-in-a-project/overview-of-commit-dates.md)
>   * [커밋 일자와 계획된 완료 일자 간의 상호 작용](../../../manage-work/projects/updating-work-in-a-project/interactions-between-commit-and-planned-completion-dates.md).
>
>* 예상 완료 일자는 문제가 현실적으로 완료될 수 있는 실제 일자를 결정하기 위해 외부 요인을 고려하여 Workfront에서 계산한 일자입니다. 자세한 내용은 [프로젝트, 작업 및 문제의 예상 완료 일자 개요](../../../manage-work/projects/planning-a-project/project-projected-completion-date.md)를 참조하십시오.
>

## 문제의 계획된 완료 일자 수동 설정

문제의 계획된 완료 일자를 업데이트하려면 문제에 대한 편집 액세스 권한과 문제에 대한 관리 권한이 있어야 합니다.

Workfront의 다음 영역에서 문제의 계획된 완료 일자 를 수동으로 설정할 수 있습니다.

* 문제를 만들거나 편집할 때 문제 편집 상자 또는 문제 세부 정보 영역에서 확인할 수 있습니다. 자세한 내용은 [문제 편집](../../../manage-work/issues/manage-issues/edit-issues.md)을 참조하세요.
* 홈 영역에서 문제의 요약 패널에 계획된 완료 일자 가 표시되는 경우. 자세한 내용은 [홈 영역에서 작업 항목 업데이트 또는 편집](../../../workfront-basics/using-home/using-the-home-area/update-and-edit-work-item-home.md)을 참조하세요.
* 문제 헤더에서 확인할 수 있습니다. 자세한 내용은 [새 개체 헤더](../../../workfront-basics/the-new-workfront-experience/new-object-headers.md)를 참조하십시오.
* 보기에 계획된 완료 일자 필드가 표시되는 경우 문제 목록 또는 보고서에서

  자세한 내용은 [목록의 문제 편집](../../../manage-work/issues/manage-issues/edit-issues-in-a-list.md)을 참조하세요.

## Workfront에서 문제에 대한 계획된 완료 일자를 자동으로 계산하는 방법

Workfront이 문제의 계획된 완료 일자를 자동으로 계산할 때 다음 사항이 일자에 영향을 줄 수 있습니다.

* 계획된 시작 일자

  시작 일자 및 계획된 시작 일자는 문제를 처음 생성할 때 문제에 대해 일치해야 합니다.

* 프로젝트의 대기열 세부 정보 섹션에 구성된 기본 기간. 자세한 내용은 [요청 큐 만들기](../../../manage-work/requests/create-and-manage-request-queues/create-request-queue.md)를 참조하세요.

  기본 기간이 0일인 경우, 계획된 완료 일자가 문제의 계획된 시작 일자와 일치합니다.

* 프로젝트 일정

자동으로 설정된 경우 다음 계산에 따라 계획된 완료 일자가 결정됩니다.

```
Planned Completion Date = Planned Start Date (or Entry Date + Default Duration
```

**예:** 예를 들어 작업의 시작 날짜가 1월 14일 금요일이고 기본 기간이 5일인 경우 프로젝트 일정이 하루 8시간 동안 월요일부터 금요일이면 계획된 완료 날짜가 1월 21일 금요일입니다.

다음과 같은 상황이 있습니다.

* 프로젝트에 일정이 없으면 Workfront 시스템의 기본 일정이 고려됩니다. 자세한 내용은 [일정 개요](../../../administration-and-setup/set-up-workfront/configure-timesheets-schedules/schedules-overview.md)를 참조하세요.
* 일정이 월요일~금요일 오전 9시~오후 1시(1일 4시간)이고 Workfront 시스템의 작업 일당 일반 시간이 8시간인 경우 계획된 완료 일자는 1월 27일입니다.

>[!TIP]
>
>Workfront은 계획된 완료 일자를 계산할 때 휴일 및 주말과 같은 스케줄 예외를 고려합니다.


