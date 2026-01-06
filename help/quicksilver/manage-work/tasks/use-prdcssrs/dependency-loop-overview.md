---
content-type: overview
product-area: projects
navigation-topic: use-predecessors
title: 작업 종속성 루프 개요
description: 작업에 전임 작업 관계를 추가할 때 종속성 루프가 발생할 수 있습니다. 전임 작업에 대한 자세한 내용은 작업 전임 작업 개요를 참조하십시오.
author: Alina
feature: Work Management
exl-id: 142e9637-841c-43d1-b297-e42c28a9e010
source-git-commit: dbc4404501e20b3f1905a5eebd13734a65db27ae
workflow-type: tm+mt
source-wordcount: '253'
ht-degree: 0%

---

# 작업 종속성 루프 개요

작업에 전임 작업 관계를 추가할 때 종속성 루프가 발생할 수 있습니다. 전임 작업에 대한 자세한 내용은 [작업 전임 작업 개요](../../../manage-work/tasks/use-prdcssrs/predecessors-overview.md)를 참조하십시오.

## 종속성 루프 개요

종속성 루프는 서로 종속된 두 개 이상의 작업이 완료될 때 발생합니다. Adobe Workfront에서는 종속성 루프를 만드는 경우 작업 간에 전임 작업 관계를 만들 수 없습니다.

**예:** 작업 2는 작업 1의 전임 작업입니다. 즉, 작업 1에서 작업을 시작하려면 먼저 작업 2를 완료해야 합니다.

작업 1을 작업 2의 전임 작업으로 만들려고 하면 작업 2가 완료될 때까지 작업 1을 시작할 수 없지만 작업 1이 완료될 때까지 작업 2를 시작할 수 없으므로 종속성 루프 오류가 발생합니다.

![](assets/dependency-loop-error-message-350x209.png)

![](assets/dependency-loop-in-task-list-nwe-350x97.png)

## 종속성 루프에 대한 고려 사항

* 종속성 루프는 두 개 이상의 작업을 포함할 수 있습니다. 때로는 선행 작업 관계와 연결하는 작업의 상위 항목 수가 종속성 루프를 만드는 상위 항목일 수도 있습니다.
* 상위 항목을 하위 항목의 전임 항목으로 만들려고 하는 경우에도 종속성 루프가 발생할 수 있습니다.
* 종속성 루프의 경우 작업 또는 프로젝트를 저장할 수 없습니다. 종속성 루프를 수정하려면 작업 또는 프로젝트를 저장하기 전에 오류 메시지에 나열된 작업 간의 전임 작업 관계를 재평가하고 충돌을 제거해야 합니다.


