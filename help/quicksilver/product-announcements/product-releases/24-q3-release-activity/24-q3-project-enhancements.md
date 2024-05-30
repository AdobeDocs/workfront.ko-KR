---
title: 2024년 3분기 프로젝트 개선 사항
description: 2024년 3분기 프로젝트 개선 사항
author: Courtney
feature: Product Announcements
recommendations: noDisplay, noCatalog
exl-id: 27d479d1-338a-429c-9703-8e72ed8d5c95
source-git-commit: 39f5526a7a816da60cb80ea4fe9313a2773e6398
workflow-type: tm+mt
source-wordcount: '410'
ht-degree: 0%

---

# 2024년 3분기 프로젝트 개선 사항

이 페이지에서는 미리보기 환경에 대한 2024년 3분기 릴리스의 모든 프로젝트 개선 사항에 대해 설명합니다. 이러한 개선 사항은 언급된 대로 프로덕션 환경에서 사용할 수 있습니다.

2024년 3분기 릴리스 주기에 이 시점에서 사용할 수 있는 모든 변경 사항의 목록은 을 참조하십시오. [2024년 3분기 릴리스 개요](/help/quicksilver/product-announcements/product-releases/24-q3-release-activity/24-q3-release-overview.md).


## 헤더 또는 세부 정보 섹션에서 작업 및 문제 커밋 일자 및 조건 편집

>[!NOTE]
>
>미리보기 릴리스: 2024년 5월 30일, 빠른 릴리스를 위한 프로덕션: 24.6 릴리스(2024년 6월 13일), 모든 고객을 위한 프로덕션 릴리스: 24.7 릴리스(2024년 7월).

작업 및 문제를 더 쉽게 업데이트할 수 있도록 이제 커밋 일자 및 조건 필드를 레이아웃 템플릿의 작업 및 문제 헤더 및 세부 정보 섹션에 추가할 수 있는 옵션으로 추가했습니다. 이제 사용자는 수정된 레이아웃 템플릿에 할당될 때 페이지의 헤더 또는 세부 정보 섹션에서 이러한 필드를 업데이트할 수 있습니다. 이 개선 사항 이전에는 헤더를 사용자 지정할 때 작업 및 문제의 조건 및 커밋 일자를 추가할 수 없었습니다.

커밋 일자 및 조건 갱신에 대한 자세한 내용은 다음 문서를 참조하십시오.

* [작업 및 문제에 대한 상태 업데이트](/help/quicksilver/manage-work/projects/updating-work-in-a-project/update-condition-for-tasks-and-issues.md).
* [작업 및 문제에 대한 커밋 일자 업데이트](/help/quicksilver/manage-work/projects/updating-work-in-a-project/update-commit-date-on-tasks-and-issues.md).

[이 기능에 대한 비디오 데모를 봅니다.](https://video.tv.adobe.com/v/3429471/){target=_blank}

## 더 관련성 있는 스마트 할당

>[!NOTE]
>
>미리보기 릴리스: 2023년 12월 21일, 빠른 릴리스를 위한 프로덕션: 24.5 릴리스(2024년 5월 16일), 모든 고객을 위한 프로덕션 릴리스: 24.7 릴리스(2024년 7월).

Workfront이 작업에 대한 스마트 할당을 계산하고 제안하는 데 사용하는 알고리즘을 변경했습니다. 새 알고리즘은 작업을 지정하는 Workfront의 작업 목록, 작업 헤더의 지정 영역, 홈 및 요약 패널에서 적용됩니다.

이제 이 알고리즘에서는 스마트 할당을 제안할 때 다음 정보를 살펴봅니다.

* 작업, 프로젝트 및 포트폴리오 이름 간의 유사성.

* 이름이 비슷한 작업에 할당되는 빈도입니다.

새 알고리즘이 일치하는 항목을 찾지 못하면 기존 스마트 할당 계산 기준이 적용됩니다.

다음 사항도 고려하십시오.

* 작업 목록에서 스마트 할당 목록의 이름이 작업 목록에서 &quot;몇 가지 제안 사항&quot;에서 &quot;제안된 할당&quot;으로 변경되었습니다.

* 문제에 대한 스마트 할당 계산 방식에는 변경 사항이 없습니다. 문제 목록의 스마트 할당 목록 이름은 &quot;다음 몇 가지 권장 사항&quot;입니다.

자세한 내용은 [스마트 할당 개요](/help/quicksilver/manage-work/tasks/assign-tasks/smart-assignments.md).
