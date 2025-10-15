---
content-type: overview
product-area: projects
navigation-topic: task-information
title: 작업 원래 기간 및 원래 계획된 시간 개요
description: 프로젝트 계획의 일부로, 프로젝트에 있는 모든 작업의 계획된 시간 및 기간(또는 계획된 기간)에 대한 값을 결정해야 합니다.
author: Alina
feature: Work Management
exl-id: 96d77d9f-3d5f-457e-a4ad-10edc371a991
source-git-commit: 7427706f6ce6cad3370b91269c1b4e7a10ed09f9
workflow-type: tm+mt
source-wordcount: '578'
ht-degree: 1%

---

# 원래 작업 기간 및 원래 계획된 시간 개요

프로젝트 계획의 일부로, 프로젝트에 있는 모든 작업의 계획된 시간 및 기간(또는 계획된 기간)에 대한 값을 결정해야 합니다.

작업의 계획된 시간에 대한 자세한 내용은 [계획된 시간 개요](../../../manage-work/tasks/task-information/planned-hours.md)를 참조하십시오.

작업 기간에 대한 자세한 내용은 [작업 기간 및 기간 유형 개요](../../../manage-work/tasks/taskdurtn/task-duration-and-duration-type.md)를 참조하십시오.

이러한 값은 작업 세부 사항 탭에서 또는 작업을 편집하는 동안 볼 수 있습니다.

작업 목록 또는 작업 보고서에 대한 보기를 작성하는 경우 작업에 대한 최초 계획된 시간 및 최초 기간 필드도 추가로 볼 수 있습니다.

## 원래 계획된 시간

작업의 원래 계획된 시간은 작업이 상위 작업이 되기 전에 원래 있었던 계획된 시간 수를 나타냅니다. 작업이 상위 작업이 되면 하위 작업의 계획된 시간이 상위 작업에 롤업되어 상위 작업의 계획된 시간을 나타냅니다.

작업 보고서 또는 목록에 원래 계획된 시간 필드를 표시하면 작업이 하위 작업의 계획된 시간을 상속하기 전의 원래 계획된 시간 수를 볼 수 있습니다.

>[!NOTE]
>
>작업을 생성할 때 최초 계획된 시간 수는 0입니다. 작업이 상위 작업이 되면 이 필드의 값은 작업이 상위로 변경되기 전의 작업 계획된 시간 수로 채워집니다. 이 값은 작업이 독립 실행형 작업으로 되돌아가는 경우에도 이 필드에 남아 있습니다.

## 원래 기간

원래 작업 기간은 작업이 상위 작업이 되기 전에 원래 있었던 기간(분)입니다. 작업이 상위가 되면 가장 이른 하위의 계획된 시작 일자와 마지막 하위의 계획된 완료 일자 사이의 기간이 상위 작업에 롤업되고 상위 작업의 기간이 됩니다. 이렇게 하면 원래 작업의 기간이 대체됩니다.

작업 보고서 또는 목록에 원래 기간 필드를 표시하면 하위 작업의 기간을 상속하기 전 작업 기간의 원래 일 수를 볼 수 있습니다.

>[!NOTE]
>
>작업을 만들 때 원래 기간은 0입니다. 작업이 상위 작업이 되면 이 필드의 값은 작업이 상위 작업으로 변경되기 전의 작업 기간으로 채워집니다. 이 값은 작업이 독립 실행형 작업으로 되돌아가는 경우에도 이 필드에 남아 있습니다. 이 값은 분 단위로 표시됩니다.

## 예

예를 들어, 두 작업이 독립형 작업인 경우 최초 지속 시간과 최초 계획된 시간은 0입니다.

![original_planned_hours_and_duration_without_parent.png](assets/original-planned-hours-and-duration-without-parent-350x38.png)

첫 번째 작업이 두 번째 작업의 상위가 되면 원래 기간 및 원래 계획된 시간 필드가 상위가 되기 전의 작업 기간 및 계획된 시간 값으로 채워집니다. 원래 기간(분)이 표시됩니다. 하위 항목의 기간 및 계획된 시간이 상위 항목의 기간 및 계획된 시간이 됩니다.

![original_and_planned_hours_with_a_parent_task.png](assets/original-and-planned-hours-with-a-parent-task-350x38.png)

상위가 다시 독립형 태스크가 되면 기간 및 계획된 시간은 원래 값으로 되돌아가지만 원래 기간 및 원래 계획된 시간은 채워진 상태로 유지됩니다. 0으로 되돌리지는 않습니다.

![original_duration_and_planned_hours_after_reverse_of_a_parent.png](assets/original-duration-and-planned-hours-after-reversal-of-a-parent-350x39.png)
