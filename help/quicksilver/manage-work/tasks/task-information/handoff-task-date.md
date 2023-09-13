---
content-type: overview
product-area: projects
navigation-topic: task-information
title: 작업 전달 일자 개요
description: 제출 날짜는 작업이 작업에 사용 가능한 날짜입니다. 이는 일반적으로 전임 작업이 해결되었으며 작업 할당자가 작업을 시작할 수 있음을 의미합니다.
author: Alina
feature: Work Management
exl-id: caf2dbba-5311-418d-8c82-ddcc256f9926
source-git-commit: b774a74863bb35e3477a69ff11189c40a6d66437
workflow-type: tm+mt
source-wordcount: '723'
ht-degree: 2%

---

# 작업 전달 일자 개요

제출 날짜는 작업이 작업에 사용 가능한 날짜입니다. 이는 일반적으로 전임 작업이 해결되었으며 작업 할당자가 작업을 시작할 수 있음을 의미합니다.

>[!TIP]
>
>문제 및 프로젝트에 대한 전달 날짜가 없습니다.

## Adobe Workfront에서 전달 날짜를 계산하는 방법

>[!NOTE]
>
>핸드오프 일자는 프로젝트 상태가 다음 상태와 동일한 경우에만 계산됩니다.
>
>* 보류 중
>* 현재
>* 완료
>* 중단
>

Workfront에서는 작업의 전달 날짜를 계산하기 위해 다음 규칙을 사용합니다.

* **작업에 불완전한 전임 작업이 있는 경우**: 작업에 대한 전달 날짜가 null입니다.
* **작업에 전체 전임 작업이 있는 경우**: 전달 일자가 전임 작업의 실제 완료 일자와 동일합니다. 전임 작업이 지연되는 경우 Workfront은 다음 공식을 사용하여 후임 작업의 전달 날짜를 계산합니다.

  `Successor Handoff Date = Predecessor Actual Completion Date + Lag`

  지연 시간에 대한 자세한 내용은 [지연 유형 개요](../use-prdcssrs/lag-types.md).

  후속 작업에 두 명 이상의 전임 작업이 있는 경우 전달 날짜는 전임 작업의 최신 실제 완료 날짜를 기준으로 계산됩니다. 예를 들어 두 전임 작업의 실제 완료 날짜가 2022년 11월 8일과 2022년 11월 20일인 경우 후임 작업의 전달 날짜는 2022년 11월 20일입니다.

  >[!NOTE]
  >
  >   실제 완료 일자 또는 전임 작업 기준으로 후임 작업의 전달 일자 계산은 전임 작업이 적용되었는지 여부와 동일합니다. 강제 전임 작업에 대한 자세한 내용은 [전임 작업 시행](../use-prdcssrs/enforced-predecessors.md).


* **작업에 전임 작업 및**:

   * **계획된 시작 일자가 과거입니다.**: 작업에 강제 제한 세트가 없는 경우 전달 일자는 프로젝트의 계획된 시작 일자와 동일합니다. 작업에 강제 제한이 있는 경우 아래 &quot;계획된 일자에 대해 작업에 강제 제한이 있는 경우&quot; 섹션을 참조하십시오.
   * **계획된 시작 일자는 미래(현재 일자 이후의 일자)입니다.**: 작업에 강제 제한 설정이 없는 경우 전달 날짜는 작업의 계획된 시작 날짜와 동일합니다. 작업에 강제 제한이 있는 경우 아래 &quot;계획된 일자에 대해 작업에 강제 제한이 있는 경우&quot; 섹션을 참조하십시오.

>[!NOTE]
>
>작업에 프로젝트 간 전임 작업이 있는 경우 후임 작업의 전달 날짜는 다음 중 하나가 발생할 때만 다시 계산됩니다.
>
>* 후임 프로젝트의 타임라인을 수동으로 다시 계산합니다. 타임라인을 다시 계산하려면 프로젝트에 대한 관리 권한이 있어야 합니다.
>* 후임 프로젝트 타임라인은 밤에 자동으로 다시 계산됩니다.
>
>프로젝트의 타임라인을 다시 계산하는 방법에 대한 자세한 내용은 [프로젝트 타임라인 다시 계산](../../../manage-work/projects/manage-projects/recalculate-project-timeline.md).

* **작업에 계획된 일자에 대한 강제 제한이 있는 경우**: 전달 일자는 제한 유형 및 작업의 실제 시작 일자 여부에 따라 다릅니다.\
  다음은 작업에 대한 강제 제한 사항입니다.

   * 일자에 시작
   * 다음까지 완료:
   * 다음 이후에 시작:
   * 다음 이전에 시작
   * 고정 날짜

  다음과 같은 시나리오가 있습니다.

   * **작업의 제한 사항이 다음 일자에 시작 또는 다음 이후에 시작:**: 작업 제한 일자가 과거이고 작업에 대한 실제 시작 일자가 없는 경우(작업이 아직 시작되지 않음) 전달 일자는 작업을 시작할 수 있는 가장 가까운 날짜입니다. 작업이 시작된 경우 전달 날짜는 프로젝트의 시작 날짜와 같습니다.
   * **작업의 제한 사항이 다음보다 늦지 않게 완료 또는 시작해야 함:**: 작업 제한 일자가 미래이고 작업에 대한 실제 시작 일자가 없는 경우(작업이 아직 시작되지 않음) 전달 일자는 작업의 계획된 시작 일자입니다. 작업에 실제 시작 일자가 있는 경우 핸드오프 일자가 프로젝트의 시작 일자입니다.
   * **작업에 고정 일자 제한이 있는 경우**: 전달 일자는 전임 작업이 있는지 여부와 전임 작업이 완료되었는지 여부와 관계없이 작업의 계획된 시작 일자입니다.

<!--these are old descriptions, edited by Anna As. on August 25, 2023 in this issue - https://experience.adobe.com/#/@adobeinternalworkfront/so:hub-Hub/workfront/issue/64c0032500018fabd4fc484167eb10dc/updates
   * When the task has a constraint of Must Start On or Start No Earlier Than, the Handoff Date is the Constraint date, unless there is an Actual Start Date on the task. If there is an Actual Start Date on the task, the Handoff Date is the Actual Completion Date of the predecessor.
   * When the task has a constraint of Must Finish On or Start No Later Than, the Handoff Date is always the Actual Completion Date of the predecessor, regardless of whether there is an Actual Start Date on the task or not. 
   * When the task has a constraint of Fixed Dates, the Handoff Date is the Planned Start Date of the task, regardless of whether it has a predecessor or not and regardless of whether the predecessor is completed or not.

-->

## 제출 일자 찾기

작업 보고서 또는 작업 목록 보기에 작업의 전달 날짜를 표시할 수 있습니다.\
보고서 빌드에 대한 자세한 내용은 [사용자 지정 보고서 만들기](../../../reports-and-dashboards/reports/creating-and-managing-reports/create-custom-report.md).
