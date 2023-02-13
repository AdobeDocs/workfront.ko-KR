---
content-type: overview
product-area: projects
navigation-topic: task-duration
title: '기간 유형 개요: 계산된 할당'
description: 계산된 할당은 Adobe Workfront에서 작업에 대해 설정할 수 있는 기간 유형입니다. Workfront의 기간 유형에 대한 일반적인 정보는 작업 기간 및 기간 유형 개요를 참조하십시오.
author: Alina
feature: Work Management
exl-id: 5f1f6109-5d54-4c3f-9aa5-dc6ce165a1cd
source-git-commit: f2f825280204b56d2dc85efc7a315a4377e551c7
workflow-type: tm+mt
source-wordcount: '478'
ht-degree: 0%

---

# 기간 유형 개요: 계산된 할당

계산된 할당은 Adobe Workfront에서 작업에 대해 설정할 수 있는 기간 유형입니다. Workfront의 기간 유형에 대한 일반적인 내용은 [작업 기간 및 기간 유형 개요](../../../manage-work/tasks/taskdurtn/task-duration-and-duration-type.md).

## 계산된 지정 기간 유형 개요

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: This Hub issue has a powerpoint that highlights information that is useful to users when using Calculated Assignment duration type. I don't think we can use the powerpoint, because it's old. I also don't know if the things they discuss are still relevant, since the PP is from 2015. I've closed the issue, but I'm putting a link here just in case the info is useful. https://hub.workfront.com/issue/5a9dd7d5007d02a8966014557c23cc89/updates)</p>
-->

* 계산된 지정 기간 유형을 사용하는 경우 작업에 대해 기간 및 계획 시간 수를 모두 지정해야 합니다. 그런 다음 Workfront은 계획 시간의 양을 지속 기간의 시간 단위로 나눈 다음, 태스크에 지정된 자원 수로 각 자원에 대한 할당 퍼센트(발령 계산)를 계산합니다. 각 리소스는 할당 비율에 대해 동일한 값을 갖습니다. 이 경우 각 리소스에 대한 할당 값을 수정할 수 없습니다.
* Workfront 또는 그룹 관리자는 시스템 또는 그룹의 기본 기간 유형을 계산된 할당으로 설정할 수 있습니다. 이 경우 이 기간 유형을 사용하여 새 작업이 모두 생성됩니다. 시스템 수준 또는 그룹 수준 프로젝트 환경 설정의 일부로 작업 및 문제 환경 설정 변경에 대한 자세한 내용은 [시스템 전체 작업 및 문제 환경 설정 구성](../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-task-issue-preferences.md).

   이 경우 작업의 기본값은 1일 기간 및 기본값인 0시간 계획입니다. 프로젝트 관리자가 보다 정확한 지속 시간을 설정하고 계획 시간 필드를 실제 예상 값으로 채우지 않으면 리소스가 덜 할당된 것으로 표시됩니다.

계산된 할당은 다음 상황에서 기본 기간 유형입니다.

* 발령에 활동 창이 있지만 전체 기간 할당된 기간을 사용하여 해당 작업을 완료하지 않는 경우 예를 들어, 주말까지 관리자에게 보고서를 전달하도록 지정됩니다. 5일 기간이 있지만 문서 초안을 작성하는 데 10시간밖에 걸리지 않습니다.
* 프로젝트 관리자가 서로 독립적으로 계획된 기간과 계획 작업량을 예측할 수 있으므로 단일 자원이 태스크에 지정되는 경우

   동일한 결과에 대해 계산된 작업 기간 유형을 사용할 수 있지만, 계획 시간의 계산된 값에 영향을 주려면 프로젝트 관리자가 자원에 대한 퍼센트 할당을 입력해야 합니다. 따라서 프로젝트 계획이 더 어렵고 시간이 많이 걸립니다.

각 자원에 대한 할당 비율은 다음과 같이 계산됩니다.

```
Planned Hours / Duration / Number of Resources = Allocation Percentage for each resource
```

예를 들어 아래 요약된 시나리오에서 각 작업의 기간은 3일입니다. 프로젝트 관리자는 기간(3일 또는 24시간)과 계획 시간을 모두 수동으로 입력하므로 할당 퍼센트(또는 지정 퍼센트)가 계산됩니다.

![](assets/calcassign-350x80.png)

## 작업의 기간 유형을 계산된 할당으로 변경합니다.

작업의 기간 유형 변경에 대한 자세한 내용은 [작업의 기간 유형 업데이트](../../../manage-work/tasks/taskdurtn/update-duration-type-of-task.md).

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
