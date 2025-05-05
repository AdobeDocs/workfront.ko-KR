---
product-area: projects
navigation-topic: create-tasks
title: 작업 만들기 개요
description: 프로젝트를 만든 후에만 프로젝트에서 작업을 만들 수 있습니다.
author: Alina
feature: Work Management
exl-id: 7bd6578e-9288-4793-ba07-a0c126c479b9
source-git-commit: f2f825280204b56d2dc85efc7a315a4377e551c7
workflow-type: tm+mt
source-wordcount: '889'
ht-degree: 0%

---

# 작업 만들기 개요

프로젝트를 만든 후에만 프로젝트에서 작업을 만들 수 있습니다.

예를 들어 프로젝트를 만든 후 작업을 추가하고 수정하여 프로젝트 계획을 구성할 수 있습니다. 프로젝트 만들기에 대한 자세한 내용은 [프로젝트 만들기](../../../manage-work/projects/create-projects/create-project.md)를 참조하십시오. 작업 만들기에 대한 자세한 내용은 [프로젝트에서 작업 만들기](../../../manage-work/tasks/create-tasks/create-tasks-in-project.md)를 참조하십시오.

이 문서에서는 작업 생성 시 적용되는 기본값과 고려 사항, 제한 사항에 대해 설명합니다.

## 프로젝트에서 작업을 생성하는 방법

다음과 같은 방법으로 프로젝트에 작업을 생성할 수 있습니다.

* [프로젝트에서 작업 만들기](../../../manage-work/tasks/create-tasks/create-tasks-in-project.md)에 설명된 대로 처음부터 새로 만듭니다.
* [작업 복사 및 복제](../../../manage-work/tasks/manage-tasks/copy-and-duplicate-tasks.md)에 설명된 대로 작업을 동일한 프로젝트 또는 새 프로젝트에 복사하거나 동일한 프로젝트의 작업을 복제합니다.
* [작업 이동](../../../manage-work/tasks/manage-tasks/move-tasks.md)에 설명된 대로 작업을 프로젝트에서 다른 프로젝트로 이동합니다.

## 작업 생성 제한 사항

올바른 액세스 및 권한이 있으면 프로젝트에 작업을 만들 수 있습니다. 그러나 작업을 만들 수 없는 경우는 다음과 같습니다.

* Adobe Workfront 관리자 또는 그룹 관리자는 프로젝트 환경 설정 영역에서 완료 또는 중단 상태인 프로젝트에 작업을 추가할 수 있어야 합니다. 프로젝트 환경 설정 지정에 대한 자세한 내용은 [시스템 전체 프로젝트 환경 설정 구성](../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-project-preferences.md)을 참조하십시오.
* 승인 보류 중인 프로젝트에 작업을 추가할 수 없습니다.

## 프로젝트에 허용된 최대 작업 수

프로젝트에는 최대 5,000개의 작업이 포함될 수 있습니다. 한도에 도달했을 때, 한도를 충족했을 때, 한도를 초과하려고 할 때 프로젝트에 경고 메시지가 표시됩니다.

이 제한이 적용되었을 때의 프로젝트 작업 수에 따라 Workfront 인스턴스에서 단일 프로젝트에 5,000개 이상의 작업을 허용할 수 있습니다.

단일 프로젝트에 5,000개 이상의 작업을 포함할 수 있는 경우 다음 사항에 유의하십시오.

* Workfront 환경에 대한 작업 제한은 가장 큰 프로젝트의 현재 작업 수와 추가 10%로 설정됩니다.

  예를 들어 Workfront 인스턴스의 프로젝트에 10,000개의 작업이 포함된 경우 Workfront 인스턴스 전체의 각 프로젝트에 대한 제한은 11,000개입니다.

* 소규모 프로젝트는 성능을 향상시키고 대규모 프로젝트에 수반되는 관리 문제를 최소화합니다.

## 프로젝트에 작업을 추가할 때 작업 기본값

Workfront에서 작업을 생성할 때 작업에 대해 자동으로 업데이트하는 기본 정보에는 두 가지 유형이 있습니다.

* 시스템 수준 기본 정보

  Workfront 관리자 또는 그룹 관리자는 프로젝트 환경 설정의 작업 및 문제 영역에서 작업에 대한 시스템 수준 기본값을 설정합니다. 작업 및 문제 환경 설정에 대한 자세한 내용은 [시스템 전체 작업 및 문제 환경 설정 구성](../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-task-issue-preferences.md) 또는 [그룹에 대한 작업 및 문제 환경 설정 구성](../../../administration-and-setup/manage-groups/create-and-manage-groups/configure-task-issue-preferences-group.md)을 참조하십시오.

* 프로젝트 수준 기본 정보

  이 섹션의 나머지 부분에서는 프로젝트 관리자가 프로젝트에 추가된 모든 새 작업에 대해 정의할 수 있는 프로젝트 수준 기본값을 설명합니다

프로젝트에 작업을 추가할 때 프로젝트 설정 방법에 따라 Workfront이 승인 프로세스 또는 사용자 정의 양식을 작업에 자동으로 첨부할 수 있습니다.

기본으로 이러한 작업을 추가하도록 프로젝트를 구성하는 방법에 대한 자세한 내용은 [프로젝트 편집](../../../manage-work/projects/manage-projects/edit-projects.md) 문서의 &quot;작업&quot; 섹션을 참조하십시오.

프로젝트 수준에서 프로젝트에 추가된 작업과 연결할 기본 정보를 정의할 때는 다음 사항을 고려하십시오.

* 작업 승인 프로세스 및 사용자 정의 양식에 대한 기본 설정을 정의하려면 프로젝트에 대한 관리 권한이 있어야 합니다.
* 모든 새 작업은 프로젝트 편집 시 승인 프로세스와 사용자 정의 양식을 정의하여 만들어집니다.
* 작업 편집 상자를 사용하여 작업을 추가할 때는 이러한 기본 설정을 수정할 수 있지만 인라인 편집에서 작업을 추가할 때는 수정할 수 없습니다.
* 템플릿의 작업에 대한 승인 프로세스 및 사용자 정의 양식을 정의할 수 있습니다.

   * 이 템플릿에서 프로젝트를 만들면 승인 프로세스 및 사용자 정의 양식이 프로젝트에 자동으로 적용됩니다.
   * 템플릿이 기존 프로젝트에 첨부된 경우 프로젝트는 원래 작업 승인 프로세스 및 사용자 정의 양식 설정이 정의된 경우 이를 유지합니다. 정의되지 않은 경우 템플릿의 설정이 프로젝트의 설정이 됩니다.
   * 템플릿이 기존 프로젝트에 첨부된 경우 템플릿에서 프로젝트에 추가된 작업은 프로젝트의 작업 설정에 관계없이 승인 프로세스 및 템플릿에 있었던 사용자 정의 양식 설정을 유지합니다.

  프로젝트에 템플릿을 첨부하는 방법에 대한 자세한 내용은 [프로젝트에 템플릿 첨부](../../../manage-work/projects/create-and-manage-templates/attach-template-to-project.md)를 참조하십시오.

* 프로젝트를 복사하면 작업 기본 설정이 새 프로젝트로 전송됩니다.

  프로젝트 복사에 대한 자세한 내용은 [프로젝트 복사](../../../manage-work/projects/manage-projects/copy-project.md)를 참조하십시오.

* 한 프로젝트에서 다른 프로젝트로 작업을 복사할 때 대상 프로젝트에 작업에 대한 기본 설정이 다를 경우 복사 프로세스에서 작업을 지우지 않는 한 복사된 작업은 원래 프로젝트의 기본 설정을 유지합니다.
* 동일한 프로젝트에서 작업을 복제하면 사용자 정의 양식 및 승인 프로세스가 중복 작업으로 전송됩니다.

  작업 복사 및 복제에 대한 자세한 내용은 [&#128279;](../../../manage-work/tasks/manage-tasks/copy-and-duplicate-tasks.md) [작업 복사 및 복제](../../../manage-work/tasks/manage-tasks/copy-and-duplicate-tasks.md)를 참조하십시오.

* 작업을 다른 프로젝트로 이동하면 새 프로젝트의 작업 기본 설정에 관계없이 기본 작업 설정이 원래 프로젝트의 작업에 저장됩니다.

  작업 이동에 대한 자세한 내용은 [작업 이동](../../../manage-work/tasks/manage-tasks/move-tasks.md)을 참조하십시오.
