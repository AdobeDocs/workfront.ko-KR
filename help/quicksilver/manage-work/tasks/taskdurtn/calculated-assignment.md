---
content-type: overview
product-area: projects
navigation-topic: task-duration
title: '기간 유형 개요: 계산된 지정'
description: 계산된 할당은 Adobe Workfront에서 작업에 대해 설정할 수 있는 기간 유형입니다. Workfront의 기간 유형에 대한 일반 정보는 작업 기간 및 기간 유형 개요를 참조하십시오.
author: Alina
feature: Work Management
exl-id: 5f1f6109-5d54-4c3f-9aa5-dc6ce165a1cd
source-git-commit: 0792651822fd85cb3bfbb754aaf949c4fc4038a1
workflow-type: tm+mt
source-wordcount: '481'
ht-degree: 0%

---

# 기간 유형 개요: 계산된 지정

<!-- Audited: 5/2025 -->

계산된 할당은 Adobe Workfront에서 작업에 대해 설정할 수 있는 기간 유형입니다. Workfront의 기간 유형에 대한 일반적인 정보는 [작업 기간 및 기간 유형 개요](../../../manage-work/tasks/taskdurtn/task-duration-and-duration-type.md)를 참조하십시오.

## 계산된 할당 기간 유형 개요

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: This Hub issue has a powerpoint that highlights information that is useful to users when using Calculated Assignment duration type. I don't think we can use the powerpoint, because it's old. I also don't know if the things they discuss are still relevant, since the PP is from 2015. I've closed the issue, but I'm putting a link here just in case the info is useful. https://hub.workfront.com/issue/5a9dd7d5007d02a8966014557c23cc89/updates)</p>
-->

* 계산된 할당 기간 유형을 사용하는 경우 지속 기간과 작업에 대한 계획된 시간 수를 모두 지정해야 합니다. 그런 다음 Workfront에서 계획된 시간의 양을 기간의 시간 수로 나눈 다음 작업에 할당된 자원의 수로 나누어 각 자원의 할당 비율을 계산합니다(할당 계산). 각 자원은 할당 비율에 대해 동일한 값을 갖게 됩니다. 이 경우 각 리소스에 대한 할당 값을 수정할 수 없습니다.
* Workfront 또는 그룹 관리자는 시스템 또는 그룹의 기본 기간 유형을 계산된 지정으로 설정할 수 있습니다. 이 경우 모든 새 작업은 이 기간 유형으로 만들어집니다. 시스템 수준 또는 그룹 수준 프로젝트 환경 설정의 일부로 작업 및 문제 환경 설정을 변경하는 방법에 대한 자세한 내용은 [시스템 전체 작업 및 문제 환경 설정 구성](../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-task-issue-preferences.md)을 참조하십시오.

  이 경우 작업에는 기본적으로 1일 지속 시간과 0시간의 계획된 시간이 있습니다. 프로젝트 관리자가 더 정확한 기간을 설정하고 실제 예상 값으로 계획된 시간 필드를 채우지 않는 한, 리소스는 과소 할당된 것으로 표시됩니다.

계산된 지정은 다음과 같은 경우 기본 기간 유형입니다.

* 할당에 활동 기간이 있지만 작업을 완료하는 데 할당된 전체 기간을 사용하지 않는 경우. 예를 들어 주말까지는 상사에게 보고서를 전달하도록 할당됩니다. 기간은 5일이지만 문서 초안을 작성하는 데 10시간만 소요됩니다.
* 프로젝트 관리자가 서로 독립적으로 계획된 기간 및 계획된 작업량을 예상할 수 있으므로 단일 자원이 작업에 할당되는 경우.

  동일한 결과에 대해 [계산된 작업 기간 유형]을 사용할 수 있지만, 프로젝트 관리자가 계획된 시간의 계산된 값에 영향을 주려면 자원에 대한 퍼센트 할당을 입력해야 합니다. 이를 통해 프로젝트 계획을 더욱 어렵고 많은 시간이 소요됩니다.

각 자원에 대한 할당 비율은 다음과 같이 계산됩니다.

```
Planned Hours / Duration / Number of Resources = Allocation Percentage for each resource
```

예를 들어 아래 설명된 시나리오에서 각 작업의 기간은 3일입니다. 프로젝트 관리자는 기간(3일 또는 24시간)과 계획된 시간을 모두 수동으로 입력하므로 할당 백분율(또는 할당 백분율)이 계산됩니다.

![](assets/calcassign-350x80.png)

## 작업의 기간 유형을 계산된 지정으로 변경

작업의 기간 유형 변경에 대한 자세한 내용은 [작업의 기간 유형 업데이트](../../../manage-work/tasks/taskdurtn/update-duration-type-of-task.md)를 참조하십시오.

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: replaced with new article linked above)</p>
-->

<!--
<ol data-mc-conditions="QuicksilverOrClassic.Draft mode">
<li value="1">Go to a task for which you want to change the Duration Type.</li>
<li value="2"> <p data-mc-conditions="QuicksilverOrClassic.Quicksilver">Click <strong>Task Details</strong> in the left panel, then in the Overview area double click <strong>Duration Type</strong>. </p> </li>
<li value="3">Select <strong>Calculated Assignment</strong> from the drop-down menu.</li>
<li value="4">Click <strong>Save</strong> <strong>Changes</strong>.</li>
</ol>
-->
