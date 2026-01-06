---
content-type: overview
product-area: projects
navigation-topic: task-information
title: 작업에 대한 '시작 가능' 개요
description: 작업을 시작할 준비가 되면 Adobe Workfront은 작업 시작 가능 표시기를 작업에 추가하여 작업을 시작하는 것이 안전함을 쉽게 식별합니다. 이 표시기는 작업 목록 또는 보고서 보기에서 볼 수 있습니다.
author: Alina
feature: Work Management
exl-id: 158f8370-9717-4c61-99fa-e3b76a9e61cb
source-git-commit: dbc4404501e20b3f1905a5eebd13734a65db27ae
workflow-type: tm+mt
source-wordcount: '431'
ht-degree: 0%

---

# 작업에 대한 &quot;시작 가능&quot; 개요

작업을 시작할 준비가 되면 Adobe Workfront은 작업 시작 가능 표시기를 작업에 추가하여 작업을 시작하는 것이 안전함을 쉽게 식별합니다. 이 표시기는 작업 목록 또는 보고서 보기에서 볼 수 있습니다.

작업을 수행할 준비가 되면 해당 작업의 시작 가능 필드가 True로 설정됩니다.

## Workfront이 작업을 &quot;시작 가능&quot;으로 표시하는 방법

Workfront은 시작 가능 필드에 대해 작업을 True로 표시하기 전에 다음 사항을 확인합니다.

* 작업에 상위 항목이 있는 경우 True로 설정된 상위 항목에 대해 시작 가능 여부 값입니다. 상위 값이 False이면 모든 하위 작업의 값이 Can Start도 False로 설정됩니다.
* 과제의 전임자와 부모의 전임자가 모두 완결되었는지 여부. 작업이 완료되면 작업의 시작 가능 값이 True로 설정됩니다. 작업 전임 작업이나 상위 작업의 전임 작업이 완료되지 않았거나 승인 보류 중 상태인 경우 작업에 대한 시작 가능 값이 False로 설정됩니다.
* 작업 종속성 유형이 시작-시작 또는 시작-완료인지 여부. 종속성 유형이 시작-시작 또는 시작-완료인 경우 종속 작업은 전임 작업이 진행 중인 후(또는 전임 작업의 완료율이 1%보다 큰 후) &quot;시작 가능&quot; 플래그가 True로 설정됩니다.

  작업 전임 작업에 대한 자세한 내용은 [작업 전임 작업 개요](../../../manage-work/tasks/use-prdcssrs/predecessors-overview.md)를 참조하십시오.

## 시작할 준비가 된 작업 식별에 대한 고려 사항

* 작업과 해당 전임 작업 간의 종속성 유형이 시작-시작인 경우 전임 작업 관계가 해결된 것으로 간주되고 후임 작업을 시작할 수 있으려면 먼저 전임 작업이 시작되어야 합니다. 종속성 유형에 대한 자세한 내용은 [작업 종속성 유형 개요](../../../manage-work/tasks/use-prdcssrs/task-dependency-types.md)를 참조하십시오.
* 작업에 프로젝트 간 전임 작업이 있는 경우 전임 작업이 완료되어도 후임 작업에 자동으로 적용할 수 있는 시작 가능 표시기가 트리거되지 않습니다. 후속 작업이 시작 가능 작업으로 표시되기 전에 후속 작업의 프로젝트 타임라인을 수동으로 다시 계산하거나 Workfront에서 자동으로 다시 계산해야 합니다. 프로젝트 타임라인 다시 계산에 대한 자세한 내용은 [프로젝트 타임라인 다시 계산](../../../manage-work/projects/manage-projects/recalculate-project-timeline.md)을 참조하십시오.

  프로젝트 간 전임 작업에 대한 자세한 내용은 [프로젝트 간 전임 작업 만들기](../../../manage-work/tasks/use-prdcssrs/cross-project-predecessors.md)를 참조하십시오.
