---
content-type: overview
product-area: projects
navigation-topic: task-information
title: 작업에 대한 "시작 가능" 개요
description: 작업을 시작할 준비가 되면 Adobe Workfront은 작업에 시작 가능 표시기를 추가하여 작업 작업을 시작하는 것이 안전한지 쉽게 확인할 수 있습니다. 작업 목록 또는 보고서 보기에서 이 표시기를 볼 수 있습니다.
author: Alina
feature: Work Management
exl-id: 158f8370-9717-4c61-99fa-e3b76a9e61cb
source-git-commit: f2f825280204b56d2dc85efc7a315a4377e551c7
workflow-type: tm+mt
source-wordcount: '390'
ht-degree: 0%

---

# 작업에 대한 &quot;시작 가능&quot; 개요

작업을 시작할 준비가 되면 Adobe Workfront은 작업에 시작 가능 표시기를 추가하여 작업 작업을 시작하는 것이 안전한지 쉽게 확인할 수 있습니다. 작업 목록 또는 보고서 보기에서 이 표시기를 볼 수 있습니다.

작업을 작업할 준비가 되면 작업의 시작 가능 필드가 True로 설정됩니다.

## Workfront이 작업을 &quot;시작 가능&quot;으로 표시하는 방법

Workfront에서는 시작 가능 필드에 대해 작업이 True로 표시되기 전에 다음 사항을 확인합니다.

* 작업에 상위 항목이 있는 경우 상위 항목에 대해 시작 가능 값이 True로 설정되어 있는지 확인합니다. 상위의 값이 False이면 모든 하위 작업의 값이 False로 설정됩니다. 
* 과거 경험이나 선배들이 과연 완성을 했는지도 관심거리다. 작업이 완료되면 작업에 대한 시작 가능 값이 True로 설정됩니다. 작업 선행 작업 또는 해당 부모의 선행 작업 중 완료되지 않았거나 완료 대기 중 승인 상태가 있는 경우 작업에 대한 시작 가능 값이 False로 설정됩니다. 

   작업 선행 작업에 대한 자세한 내용은 [작업 선행 작업 개요](../../../manage-work/tasks/use-prdcssrs/predecessors-overview.md).

## 시작할 준비가 된 작업 식별에 대한 고려 사항

* 작업과 선행 작업 간의 종속성 유형이 시작 시작인 경우 이전 관계를 확인하고 후속 작업을 시작할 수 있기 전에 선행 작업을 시작해야 합니다. 종속성 유형에 대한 자세한 내용은 [작업 종속성 유형 개요](../../../manage-work/tasks/use-prdcssrs/task-dependency-types.md).
* 작업에 프로젝트 간 선행 작업이 있는 경우 선행 작업이 완료되더라도 자동으로 후속 작업에 적용할 수 있는 시작 가능 지표가 트리거되지 않습니다. 후속 작업이 시작 가능 작업으로 표시되기 전에 후속 프로젝트의 타임라인을 수동으로 다시 계산해야 하거나, Workfront에서 자동으로 다시 계산해야 합니다. 프로젝트 타임라인 재계산에 대한 자세한 내용은 [프로젝트 타임라인 다시 계산](../../../manage-work/projects/manage-projects/recalculate-project-timeline.md).

   프로젝트 간 선행 작업에 대한 자세한 내용은 [프로젝트 간 선행 작업 만들기](../../../manage-work/tasks/use-prdcssrs/cross-project-predecessors.md).
