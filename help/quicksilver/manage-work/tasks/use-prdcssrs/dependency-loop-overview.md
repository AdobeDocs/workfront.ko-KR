---
content-type: overview
product-area: projects
navigation-topic: use-predecessors
title: 작업 종속성 루프 개요
description: 작업에 선행 관계를 추가할 때 종속성 루프가 발생할 수 있습니다. 선행 작업에 대한 자세한 내용은 작업 우선 순위 개요를 참조하십시오.
author: Alina
feature: Work Management
exl-id: 142e9637-841c-43d1-b297-e42c28a9e010
source-git-commit: f2f825280204b56d2dc85efc7a315a4377e551c7
workflow-type: tm+mt
source-wordcount: '244'
ht-degree: 0%

---

# 작업 종속성 루프 개요

작업에 선행 관계를 추가할 때 종속성 루프가 발생할 수 있습니다. 선행자에 대한 자세한 내용은 [작업 선행 작업 개요](../../../manage-work/tasks/use-prdcssrs/predecessors-overview.md).

## 종속성 루프 개요

둘 이상의 작업이 완료되어야 하는 경우 종속성 루프가 발생합니다. Adobe Workfront에서는 종속성 루프를 만드는 경우 작업 간에 선행 관계를 만들 수 없습니다.

**예:** 태스크 2는 태스크 1의 전임자입니다. 즉, 태스크 1에서 작업을 시작하기 전에 태스크 2를 완료해야 합니다.

작업 1을 작업 2의 전임자로 만들려고 하면 작업 2가 완료되기 전에는 작업 1을 시작할 수 없지만 작업 1이 완료되기 전에는 작업 2를 시작할 수 없으므로 종속성 루프 오류가 발생합니다.

![](assets/dependency-loop-error-message-350x209.png)

![](assets/dependency-loop-in-task-list-nwe-350x97.png)

## 종속성 루프에 대한 고려 사항

* 종속성 루프에는 두 개 이상의 작업이 포함될 수 있습니다. 종속성 루프를 만드는 작업이 선행 관계를 통해 연결된 작업의 부모 수가 있는 경우가 있습니다.
* 상위를 하위의 선행 하위로 만들려는 경우에도 종속성 루프가 발생할 수 있습니다.
* 종속성 루프의 경우 작업이나 프로젝트를 저장할 수 없습니다. 종속성 루프를 수정하려면 작업이나 프로젝트를 저장하기 전에 오류 메시지에 나열된 작업 간의 선행 관계를 다시 평가하고 충돌을 제거해야 합니다.

 
