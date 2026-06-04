---
content-type: overview
product-area: projects
navigation-topic: use-predecessors
title: 작업 종속성 루프 개요
description: 작업에 전임 작업 관계를 추가할 때 종속성 루프가 발생할 수 있습니다. 전임 작업에 대한 자세한 내용은 작업 전임 작업 개요를 참조하십시오.
author: Alina
feature: Work Management
exl-id: 142e9637-841c-43d1-b297-e42c28a9e010
TQID: https://experienceleague.adobe.com/cQbPOUES-tmSgZTpXrft8lQby-ubPmI-TZ1PjdGURMc
product_v2:
  - id: c4a86a5d-6562-4fc6-aa00-bfa25833aed9
feature_v2:
  - id: a0dacc9f-0e23-495b-8e9f-a77c2e60b40c
subfeature_v2:
  - id: b91c0848-76c4-4da4-8b81-3aade0518dd0
  - id: f0dd7b45-76b5-49d4-afe3-39f436b6fbd3
role_v2:
  - id: b69b2659-1057-424e-8fc5-ed9e016dc554
topic_v2:
  - id: c1579802-ddd4-4214-8a91-97b2066abe11
source-git-commit: 55a9d9feae8cc1128e3427a8874414ba734dd467
workflow-type: tm+mt
source-wordcount: 263
ht-degree: 0%

---

# 작업 종속성 루프 개요

작업에 전임 작업 관계를 추가할 때 종속성 루프가 발생할 수 있습니다. 전임 작업에 대한 자세한 내용은 [작업 전임 작업 개요](../../../manage-work/tasks/use-prdcssrs/predecessors-overview.md)를 참조하십시오.

## 종속성 루프 개요

종속성 루프는 서로 종속된 두 개 이상의 작업이 완료될 때 발생합니다. Adobe Workfront에서는 종속성 루프를 만드는 경우 작업 간에 전임 작업 관계를 만들 수 없습니다.

**예:** 작업 2는 작업 1의 전임 작업입니다. 즉, 작업 1에서 작업을 시작하려면 먼저 작업 2를 완료해야 합니다.

작업 1을 작업 2의 전임 작업으로 만들려고 하면 작업 2가 완료될 때까지 작업 1을 시작할 수 없지만 작업 1이 완료될 때까지 작업 2를 시작할 수 없으므로 종속성 루프 오류가 발생합니다.

![종속성 루프 오류 메시지](assets/dependency-loop-error-message-350x209.png)

![작업 목록의 종속성 루프](assets/dependency-loop-in-task-list-nwe-350x97.png)

## 종속성 루프에 대한 고려 사항

* 종속성 루프는 두 개 이상의 작업을 포함할 수 있습니다. 때로는 선행 작업 관계와 연결하는 작업의 상위 항목 수가 종속성 루프를 만드는 상위 항목일 수도 있습니다.
* 상위 항목을 하위 항목의 전임 항목으로 만들려고 하는 경우에도 종속성 루프가 발생할 수 있습니다.
* 종속성 루프의 경우 작업 또는 프로젝트를 저장할 수 없습니다. 종속성 루프를 수정하려면 작업 또는 프로젝트를 저장하기 전에 오류 메시지에 나열된 작업 간의 전임 작업 관계를 재평가하고 충돌을 제거해야 합니다.


