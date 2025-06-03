---
content-type: overview
product-area: projects
navigation-topic: task-duration
title: '기간 유형 개요: 단순'
description: 단순 기간 유형은 Adobe Workfront에서 작업에 대해 설정할 수 있는 기간 유형입니다.
author: Alina
feature: Work Management
exl-id: 9bb472db-1448-467e-93ca-611453e1c00a
source-git-commit: 0792651822fd85cb3bfbb754aaf949c4fc4038a1
workflow-type: tm+mt
source-wordcount: '322'
ht-degree: 0%

---

# 기간 유형 개요: 단순

<!-- Audited: 5/2025 -->

단순 기간 유형은 Adobe Workfront에서 작업에 대해 설정할 수 있는 기간 유형입니다. Workfront의 기간 유형에 대한 자세한 내용은 [작업 기간 및 기간 유형 개요](../../../manage-work/tasks/taskdurtn/task-duration-and-duration-type.md)를 참조하십시오.

## 단순 기간 유형 개요

Workfront 또는 그룹 관리자는 시스템 또는 그룹의 기본 기간 유형을 단순으로 설정할 수 있습니다. 이 경우 모든 새 작업이 이 기간 유형으로 만들어집니다.

시스템 수준 또는 그룹 수준 프로젝트 환경 설정의 일부로 작업 및 문제 환경 설정을 변경하는 방법에 대한 자세한 내용은 [시스템 전체 작업 및 문제 환경 설정 구성](../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-task-issue-preferences.md)을 참조하십시오.

작업에 단순 기간 유형이 있는 경우 다음과 같은 문제가 발생합니다.

* 프로젝트 관리자는 할당자 간에 해당 시간을 배포하는 방법을 수정할 때 작업의 기간 및 계획된 시간을 모두 수정할 수 있습니다.

  자세한 내용은 [간단한 기간 유형으로 작업의 계획된 시간 및 기간 업데이트](../../../manage-work/tasks/taskdurtn/update-planned-hours-duration-for-simple-duration-task.md)를 참조하십시오.

  >[!IMPORTANT]
  >
  >처음 작업을 만들고 [단순 기간] 유형을 지정하지만 [기간]을 지정하지 않으면 Workfront에서 작업에 대해 지정한 [계획된 시간]을 기준으로 작업의 기간을 계산합니다. 단순 기간 작업의 기간을 수동으로 수정하는 경우, Workfront은 계획된 시간을 수동으로 정의하려는 것으로 간주하므로 해당 기간에 대한 일치를 중지합니다.
  >
  >Workfront은 다음 공식을 사용하여 기간이 수동으로 수정되지 않은 작업의 기간을 계산합니다.
  >
  > `Task Duration = Task Planned Hours / Typical hours per work day`
  >
  >Workfront 관리자는 인스턴스 설정의 프로젝트 환경 설정 영역에서 `Typical hours per work day`을(를) 정의합니다.

* 할당 비율은 숨겨져 있지만 할당 시간을 편집할 수 있습니다.
* 모든 신규 고객은 시스템 수준 기간 유형이 단순으로 설정되어 있습니다.

## 작업의 기간 유형을 단순으로 변경

작업의 기간 유형 변경에 대한 자세한 내용은 [작업의 기간 유형 업데이트](../../../manage-work/tasks/taskdurtn/update-duration-type-of-task.md)를 참조하십시오.

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: replaced with new article linked above)</p>
-->

<!--
<ol data-mc-conditions="QuicksilverOrClassic.Draft mode">
<li value="1">Go to a task for which you want to change the Duration Type.</li>
<li value="2"> <p data-mc-conditions="QuicksilverOrClassic.Quicksilver">Click <strong>Task Details</strong> in the left panel, then in the Overview area double click <strong>Duration Type</strong>. </p> </li>
<li value="3"> <p>Select <strong>Simple</strong> from the drop-down menu.</p> </li>
<li value="4">Click <strong>Save</strong> <strong>Changes</strong><strong>.</strong></li>
</ol>
-->
