---
content-type: overview;reference
product-area: projects
navigation-topic: use-predecessors
title: 작업 종속성 유형 개요
description: 종속성 유형은 작업 간의 이전 관계를 의미합니다. 종속 작업은 이전 작업의 시작 또는 완료에 따라 시작 또는 완료 시점을 정의합니다.
author: Alina
feature: Work Management
exl-id: 30d1c60d-0632-4a32-b7e7-a9f8e81bf727
source-git-commit: f2f825280204b56d2dc85efc7a315a4377e551c7
workflow-type: tm+mt
source-wordcount: '283'
ht-degree: 0%

---

# 작업 종속성 유형 개요

종속성 유형은 작업 간의 이전 관계를 의미합니다. 종속 작업은 이전 작업의 시작 또는 완료에 따라 시작 또는 완료 시점을 정의합니다.

>[!IMPORTANT]
>
>Adobe Workfront은 이전 관계가 강제 적용되지 않는 한 종속 작업의 시작 또는 종료를 종속성 유형에 따라 제한하지 않습니다. 이전 버전 실행에 대한 자세한 내용은 [선행 작업 적용](../../../manage-work/tasks/use-prdcssrs/enforced-predecessors.md).

작업 간에 이 관계를 설정할 때 선행 관계의 종속성 유형을 지정해야 합니다.

선행자에 대한 자세한 내용은 [작업 선행 작업 개요](../../../manage-work/tasks/use-prdcssrs/predecessors-overview.md).

다음은 Workfront 종속성 유형입니다.

* **Finish-Start(fs)**: 종속 작업을 시작하려면 선행 작업이 완료되어야 합니다. 다른 종속성 유형이 지정되지 않은 경우 사용되는 기본 종속성 유형입니다.
* **마침(ff)**: 종속 작업이 완료되기 전에 선행 작업이 완료되어야 합니다.
* **시작(ss)**: 종속 작업을 시작하려면 먼저 선행 작업을 시작해야 합니다. 선행 작업이 적어도 시작되지 않으면 종속 작업을 시작할 수 없습니다.
* **시작 완료(sf)**: 종속 작업이 완료되기 전에 선행 작업을 시작해야 합니다. 선행 작업이 시작되기 전에 종속 작업을 시작할 수 있지만 선행 작업이 시작되지 않으면 작업을 완료할 수 없습니다.
* **예약된 시작(sd)**: 작업이 완료 시작으로 예약되지만 실제 적용 유형은 완료 완료입니다. 이 작업을 사용하면 종속 작업이 완료된 후에 작업이 시작되도록 예약됩니다. 그러나 강제 적용으로 인해 종속 작업이 언제든 시작될 수 있지만 선행 작업이 완료될 때까지 완료되지 않습니다.
