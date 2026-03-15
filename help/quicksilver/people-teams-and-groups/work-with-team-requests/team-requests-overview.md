---
content-type: reference
product-area: user-management;agile-and-teams
navigation-topic: people-teams-and-groups
title: 팀 요청 개요
description: 팀 요청은 기본 메뉴의 팀 영역에서 찾을 수 있습니다.
author: Courtney
feature: People Teams and Groups
exl-id: c131c021-8bc0-4a48-a873-9ee0e189bcab
source-git-commit: 4261febe4af8628508083fa18e4767e3fd3e1136
workflow-type: tm+mt
source-wordcount: '469'
ht-degree: 0%

---

# 팀 요청 개요

## 팀 요청 이해

팀 요청이 [!UICONTROL 기본 메뉴]의 [!UICONTROL 팀] 영역에 있습니다. 왼쪽 패널에서 [!UICONTROL 팀 요청] 아이콘 ![요청 아이콘](assets/request-icon.png)을 클릭하여 팀 요청을 봅니다.

>[!NOTE]
>
>애자일 팀은 팀 요청이 없습니다.

[!UICONTROL 팀 요청] 탭에는 드롭다운 목록에서 현재 선택된 팀에 대한 할당 대기 요청이 표시됩니다. 괄호로 묶인 숫자는 작업 준비가 완료된 항목 수를 나타냅니다.

팀 요청은 특정 사용자에게 할당되지 않은 보류 중인 작업 항목을 나타냅니다. 대신 팀에 할당되며 해당 팀의 모든 구성원이 자발적으로 항목에 대한 책임을 수락할 수 있습니다. 사용자가 팀 요청 작업을 지원하면 사용자는 자신의 작업 할당을 수락합니다. 작업은 팀 외에도 개별 사용자에게 할당됩니다.

>[!NOTE]
>
>팀 요청은 공동 작업 할당에 사용할 수 없습니다. 한 작업을 함께 작업하려면 여러 사용자를 할당해야 하는 경우 팀 요청이 아닌 [!UICONTROL 고급 할당]을 통해 이 작업을 수행하십시오. 자세한 내용은 [고급 할당 만들기](../../manage-work/tasks/assign-tasks/create-advanced-assignments.md)를 참조하십시오.

## [!UICONTROL 시작 준비 완료] 및 [!UICONTROL 모두] 옵션 이해

팀 요청 섹션의 맨 위에는 두 가지 옵션이 있습니다. [!UICONTROL 시작 준비 완료] 및 [!UICONTROL 모두].

[!UICONTROL 시작 준비] 옵션은 다음 조건을 모두 충족하는 작업 및 문제만 표시합니다.

* 모든 선행자는 선행자 종속성 유형에 대한 조건을 충족했습니다.\
  예를 들어 이전 관계 유형이 [!UICONTROL Finish-Start]인 경우(이전 작업은 종속 작업을 시작하기 전에 완료해야 함) 이전 작업은 [!UICONTROL Complete]로 표시되어야 합니다. 이전 종속성 유형에 대한 자세한 내용은 [작업 종속성 유형 개요](../../manage-work/tasks/use-prdcssrs/task-dependency-types.md)를 참조하십시오.

* 로그인한 사용자는 이러한 작업 및 문제에 할당된 사용자이거나(작업 요청의 경우) 선택한 팀이 이러한 작업 및 문제(팀 요청의 경우)에 할당된 사용자입니다.
* 프로젝트 상태가 [!UICONTROL 현재] 상태입니다.
* [!UICONTROL 예상 시작 날짜] 또는 [!UICONTROL 계획된 시작 날짜]가 지났거나 오늘 날짜로부터 2주 이내에 시작되도록 예약되어 있습니다([!UICONTROL 예상 시작 날짜] 또는 [!UICONTROL 계획된 시작 날짜]가 정의되지 않음).
* [!UICONTROL Handoff 날짜]이(가) 이미 발생했거나 현재 날짜로부터 2주 이내에 발생합니다.

>[!NOTE]
>
>작업이 처음 세 가지 기준을 충족하고 현재 날짜로부터 2주 이내에 Handoff 날짜가 있는 경우 계획/예상 날짜가 2주 이후인 경우에도 [!UICONTROL 시작 준비]로 표시됩니다. 작업에 Handoff 날짜가 없는 경우 계획/예상 날짜는 현재 날짜의 2주 이내여야 합니다.

[!UICONTROL 모두] 옵션에는 로그인한 사용자에게 할당된 현재 프로젝트의 모든 작업 및 문제 또는 팀에 할당된 모든 작업 또는 문제가 표시됩니다.
