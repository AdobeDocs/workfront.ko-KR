---
content-type: release-notes
navigation-topic: 2020-2-release-activity
title: 2020.2 프로젝트 개선 사항
description: 이 페이지에서는 프로덕션 환경에 대한 2020.2 릴리스의 모든 프로젝트 개선 사항에 대해 설명합니다. 이러한 개선 사항은 2020년 5월 11일이 있는 주에 프로덕션 환경에서 사용할 수 있습니다.
author: Luke
feature: Product Announcements
recommendations: noDisplay, noCatalog
exl-id: 150bc838-d6a5-445a-af77-62c4ed74dd1b
source-git-commit: 99aac8d1621370f901704f58affd9e3e18497c4e
workflow-type: tm+mt
source-wordcount: '798'
ht-degree: 0%

---

# 2020.2 프로젝트 개선 사항

이 페이지에서는 프로덕션 환경에 대한 2020.2 릴리스의 모든 프로젝트 개선 사항에 대해 설명합니다. 이러한 개선 사항은 2020년 5월 11일이 있는 주에 프로덕션 환경에서 사용할 수 있습니다.

2020.2 릴리스에서 사용할 수 있는 모든 변경 사항의 목록은 을 참조하십시오. [2020.2 릴리스 개요](../../../product-announcements/product-releases/2020.2.-release-activity/2020-2-release-overview.md).

## Workfront 관리자의 경우: 새 프로젝트에 대한 프로젝트 상태가 숨겨지거나 잠금 해제된 경우 새 안전 장치

설정에서는 프로젝트가 생성될 때 모든 새 프로젝트가 특정 상태를 갖도록 환경 설정을 구성합니다. 프로젝트가 새 프로젝트인 경우에도 Workfront에서 제대로 작동하려면 프로젝트에 항상 상태가 필요하므로 이는 중요합니다.

관리자가 새 프로젝트에 대해 구성된 상태를 숨기거나 잠금 해제하더라도 새 프로젝트가 항상 상태를 유지하도록 하기 위해, 새 프로젝트에 대한 새 상태를 다시 구성할 때까지 이제 시스템은 상태 목록의 첫 번째 상태를 모든 새 프로젝트에 할당합니다.

모든 새 프로젝트의 상태에 대한 기본 설정을 지정하는 방법에 대한 자세한 내용은 [시스템 전체 프로젝트 환경 설정 구성](../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-project-preferences.md) (또는 Adobe Workfront Classic을 사용하는 경우 다음을 참조하십시오.) [프로젝트 환경 설정 지정](https://one.workfront.com/s/article/Setting-Project-Preferences-1883392298)).

**다음 환경에서 사용할 수 있습니다.**

* Adobe Workfront 클래식
* 새로운 Adobe Workfront 환경

## Workfront 관리자를 위한: 프로젝트 환경 설정의 디자인 개선

이제 프로젝트 환경 설정을 지정하는 환경이 보다 직관적이고 사용하기 쉬워졌습니다.

* 제목이 옵션 레이블보다 커서 원하는 항목을 더 빨리 찾을 수 있습니다.
* 구분선과 여분 공백은 각 구역을 구분하므로 현재 하고 있는 작업에 보다 쉽게 집중할 수 있습니다.
* &quot;근무일당 일반 시간&quot;과 같은 옵션에 대해 잘못된 숫자를 입력하면 저장을 클릭한 후 경고 메시지가 표시되지 않고 바로 나타납니다.
* 옵션 레이블은 세부 정보 영역 및 보고서와 같은 Workfront의 다른 곳에서도 해당 인터페이스 텍스트와 일치합니다.

프로젝트 환경 설정 영역에 대한 자세한 내용은 [시스템 전체 프로젝트 환경 설정 구성](../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-project-preferences.md) (또는 Adobe Workfront Classic을 사용하는 경우 다음을 참조하십시오.) [프로젝트 환경 설정 지정](https://one.workfront.com/s/article/Setting-Project-Preferences-1883392298)).

**다음 환경에서 사용할 수 있습니다.**

* Adobe Workfront 클래식
* 새로운 Adobe Workfront 환경

## 선택한 필터, 보기 및 그룹화가 보고서 목록에 유지됩니다.

이제 사용자가 Workfront에 로그아웃했다가 다시 로그인하는 경우에도 특정 보고서에 적용된 마지막 필터, 보기 또는 그룹화가 선택됩니다.

이전에는, 사용자가 보고서 목록에 필터, 보기 또는 그룹화를 적용한 다음 해당 페이지에서 나가면 다음에 사용자가 동일한 보고서로 이동할 때 기본 필터, 보기 또는 그룹화가 표시됩니다.

**다음 환경에서 사용할 수 있습니다.**

* 새로운 Adobe Workfront 환경
* Adobe Workfront 클래식

## 작업을 다른 프로젝트로 이동하고 복사하면 작업이 프로젝트의 타임라인 내에 맞춰질 수 있을 때 작업 제한이 유지됩니다

작업을 복사하거나 다른 프로젝트로 이동할 때 Workfront에서 작업의 날짜별 작업 제한 사항을 처리하는 방법을 개선했습니다. 날짜별 작업 제한의 예로는 다음과 같아야 함, 다음까지 완료해야 함, 고정 날짜 및 이후에 시작 등이 있습니다.

예를 들어, Must Start On 제약 조건이 있는 작업을 작업의 시작 일자 이전의 계획된 시작 일자가 있는 다른 프로젝트로 이동하거나 복사할 경우 작업은 복사되거나 이동된 후에도 제약 조건을 유지합니다. 작업의 시작 일자 이후 계획된 시작 일자가 있는 프로젝트로 Must Start On 제약 조건이 있는 작업을 이동하거나 복사하면 작업 제한 사항이 가능한 한 빨리 로 변경됩니다.

이 변경 전에 작업 제한 사항은 항상 가능한 한 빨리 로 변경됩니다.

작업 이동에 대한 자세한 내용은 [작업 이동](../../../manage-work/tasks/manage-tasks/move-tasks.md) (또는 Adobe Workfront Classic을 사용하는 경우 다음을 참조하십시오.) [작업 이동](https://one.workfront.com/s/article/Moving-Tasks-2081996259)).

작업 복사에 대한 자세한 내용은 [작업 복사 및 복제](../../../manage-work/tasks/manage-tasks/copy-and-duplicate-tasks.md) (또는 Adobe Workfront Classic을 사용하는 경우 다음을 참조하십시오.) [작업 복사 및 복제](https://one.workfront.com/s/article/Copy-and-Duplicate-Tasks-218695605)).

모든 Task Constraints에 대한 개요는 [작업 제한 개요](../../../manage-work/tasks/task-constraints/task-constraint-overview.md) (또는 Adobe Workfront Classic을 사용하는 경우 다음을 참조하십시오.) [작업 제한 개요](https://one.workfront.com/s/article/Task-Constraint-Overview-453396848)).

**다음 환경에서 사용할 수 있습니다.**

* Adobe Workfront 클래식
* 새로운 Adobe Workfront 환경

## 세부 정보 탭 또는 작업 목록을 변경하는 동안 데이터 손실 방지

변경 사항을 수동으로 저장할 때 프로젝트 수준의 작업 목록에 있는 객체 또는 작업에 대한 세부 정보 페이지의 정보를 업데이트할 때 데이터 손실을 방지하기 위해 이제 헤더의 정보를 편집하기 전에 저장하지 않은 변경 사항이 있음을 알리는 경고 메시지가 표시됩니다. 변경 사항을 저장하기 전에 허용되는 유일한 작업은 즐겨찾기에 개체를 구독하거나 추가하는 것입니다.

목록에서 작업을 편집하는 방법에 대한 자세한 내용은 [목록에서 작업 편집](../../../manage-work/tasks/manage-tasks/edit-tasks-in-a-list.md)

**다음 환경에서 사용할 수 있습니다.**

* 새로운 Adobe Workfront 환경

