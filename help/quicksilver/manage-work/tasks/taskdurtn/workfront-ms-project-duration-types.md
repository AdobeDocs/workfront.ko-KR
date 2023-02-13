---
content-type: tips-tricks-troubleshooting
product-area: projects
navigation-topic: tips-tricks-and-troubleshooting-projects
title: Adobe Workfront 및 Microsoft 프로젝트의 기간 유형
description: Adobe Workfront에서 사용할 수 있는 기간 유형은 작업 유형이라고 하는 Microsoft 프로젝트의 지속 시간과 다릅니다. Workfront과 Microsoft 프로젝트 간에 프로젝트를 내보내거나 가져올 때 혼동될 수 있습니다.
author: Alina
feature: Work Management
exl-id: 986ecf91-693d-4ee1-bc56-355a2819ae41
source-git-commit: f2f825280204b56d2dc85efc7a315a4377e551c7
workflow-type: tm+mt
source-wordcount: '256'
ht-degree: 2%

---

# Adobe Workfront 및 Microsoft 프로젝트의 기간 유형

Adobe Workfront에서 사용할 수 있는 기간 유형은 작업 유형이라고 하는 Microsoft 프로젝트의 지속 시간과 다릅니다. Workfront과 Microsoft 프로젝트 간에 프로젝트를 내보내거나 가져올 때 혼동될 수 있습니다.

Workfront과 Microsoft 프로젝트 간 프로젝트 가져오기 및 내보내기에 대한 자세한 내용은 다음 문서를 참조하십시오.

* [Microsoft 프로젝트로 프로젝트 내보내기](../../../manage-work/projects/manage-projects/export-project-to-ms-project.md)
* [Microsoft 프로젝트에서 프로젝트 가져오기](../../../manage-work/projects/create-projects/import-project-from-ms-project.md)

## Workfront 및 Microsoft 프로젝트의 기간 유형

Workfront에는 4가지 작업 기간 유형이 있습니다.

* 단순
* 작업량 고정
* 계산된 작업
* 계산된 할당

자세한 내용은 [작업 기간 및 기간 유형 개요](../../../manage-work/tasks/taskdurtn/task-duration-and-duration-type.md).

이러한 기간 유형은 Microsoft Project에서 인식할 수 없습니다. 현재 Microsoft Project에는 Workfront의 기간 유형과 유사한 세 가지 작업 유형이 있습니다.

* 고정 단위
* 고정 작업 시간
* 고정 기간

## 기간 유형은 Workfront에서 MS Project로 내보낼 때 변경됩니다

프로젝트를 Workfront에서 Microsoft 프로젝트로 내보낼 때 작업 기반 작업이 고정 작업이 됩니다. 단순, 계산된 작업 및 계산된 할당은 고정 단위가 됩니다.

## 기간 유형은 MS Project에서 Workfront으로 가져올 때 변경됩니다

Microsoft Project에서 Workfront으로 프로젝트를 가져올 때 고정 단위는 작업 제어가 됩니다. 고정 작업 및 고정 지속 시간은 Workfront 관리자가 시스템에 대해 선택한 기본 기간 유형을 받습니다. 자세한 내용은 [시스템 전체 작업 및 문제 환경 설정 구성](../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-task-issue-preferences.md).

<!--
<note type="warning">
When a task has Calculated Work as the Duration Type and the default Duration Type in Setup is set as Calculated Assignment, then MS Project assignment allocations will be lost during the import.
<MadCap:conditionalText data-mc-conditions="QuicksilverOrClassic.Draft mode">
(drafting this because it is misleading)
</MadCap:conditionalText>
</note>
-->
