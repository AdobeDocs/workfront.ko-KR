---
content-type: reference
product-area: user-management;agile-and-teams
navigation-topic: people-teams-and-groups
title: 팀 요청 개요
description: 팀 요청은 메인 메뉴의 팀 영역에 있습니다.
author: Lisa
feature: People Teams and Groups
exl-id: c131c021-8bc0-4a48-a873-9ee0e189bcab
source-git-commit: 9693ac3792fec3eca6218a228f2067519ed433ac
workflow-type: tm+mt
source-wordcount: '469'
ht-degree: 0%

---

# 팀 요청 개요

## 팀 요청 이해

팀 요청이 [!UICONTROL 기본 메뉴]의 [!UICONTROL 팀] 영역에 있습니다. 팀 요청을 보려면 왼쪽 패널의 [!UICONTROL 팀 요청] 아이콘 ![요청 아이콘](assets/request-icon.png)을 클릭하십시오.

>[!NOTE]
>
>애자일 팀에는 팀 요청이 없습니다.

[!UICONTROL 팀 요청] 탭에는 현재 드롭다운 목록에서 선택된 팀에 대한 할당 대기 중인 요청이 표시됩니다. 괄호로 묶인 숫자는 작업할 준비가 된 항목의 수를 나타냅니다.

팀 요청은 특정 사용자에게 지정되지 않은 보류 중인 작업 항목을 나타냅니다. 대신 팀에 할당되고 해당 팀의 모든 구성원이 해당 항목에 대한 책임을 수락하도록 자원할 수 있습니다. 사용자가 팀 요청에 대해 작업을 자원하는 경우 해당 사용자는 작업 할당을 자신의 것으로 수락합니다. 작업은 팀 외에 개별 사용자에게 할당됩니다.

>[!NOTE]
>
>공동 작업 할당에는 팀 요청을 사용할 수 없습니다. 여러 사용자를 할당하여 작업을 함께 진행하려면 팀 요청이 아닌 [!UICONTROL 고급 할당]을 통해 진행하십시오. 자세한 내용은 [고급 할당 만들기](../../manage-work/tasks/assign-tasks/create-advanced-assignments.md)를 참조하십시오.

## [!UICONTROL 시작 준비] 및 [!UICONTROL 모두] 옵션 이해

팀 요청 섹션의 맨 위에는 [!UICONTROL 시작할 준비] 및 [!UICONTROL 모두]와 같은 두 가지 옵션이 있습니다.

[!UICONTROL 시작 준비] 옵션은 다음 조건을 모두 충족하는 작업 및 문제만 표시합니다.

* 모든 전임 작업은 전임 작업 종속성 유형에 대한 조건을 충족했습니다.\
  예를 들어 전임 작업 관계의 유형이 [!UICONTROL 마침-시작]인 경우(전임 작업은 종속 작업을 시작하기 전에 완료해야 함) 전임 작업을 [!UICONTROL 완료](으)로 표시해야 합니다. 전임 작업 종속성 유형에 대한 자세한 내용은 [작업 종속성 유형 개요](../../manage-work/tasks/use-prdcssrs/task-dependency-types.md)를 참조하십시오.

* 로그인한 사용자는 이러한 작업 및 문제(작업 요청의 경우)에 할당된 사용자이거나 선택한 팀이 이러한 작업 및 문제(팀 요청의 경우)에 할당된 팀입니다.
* 프로젝트 상태가 [!UICONTROL 현재]입니다.
* [!UICONTROL 예상 시작 일자] 또는 [!UICONTROL 계획된 시작 일자]가 오늘 날짜로부터 2주 이내에 지나거나 시작할 예정입니다(또는 [!UICONTROL 예상 시작 일자] 또는 [!UICONTROL 계획된 시작 일자]가 정의되지 않음).
* [!UICONTROL 핸드오프 일자]이(가) 이미 발생했거나 현재 날짜로부터 2주 이내에 발생합니다.

>[!NOTE]
>
>작업이 처음 세 가지 기준을 충족하고 현재 날짜로부터 2주 이내에 전달 날짜가 있는 경우, 계획된/예상 날짜가 2주 이상 지난 경우에도 [!UICONTROL 시작할 준비가 되었습니다]로 표시됩니다. 작업에 전달 날짜가 없는 경우 계획/예상 날짜는 현재 날짜의 2주 이내여야 합니다.

[!UICONTROL 모두] 옵션에는 로그인한 사용자에게 할당된 현재 프로젝트의 모든 작업 및 문제 또는 팀에 할당된 모든 작업 또는 문제가 표시됩니다.
