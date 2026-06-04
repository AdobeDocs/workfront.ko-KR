---
content-type: overview;reference
product-area: projects
navigation-topic: use-predecessors
title: 작업 종속성 유형 개요
description: 종속성 유형 은 작업 간의 전임 작업 관계를 나타냅니다. 종속 작업은 전임 작업의 시작 또는 완료에 따라 시작 또는 완료가 가능한 시기를 정의합니다.
author: Alina
feature: Work Management
exl-id: 30d1c60d-0632-4a32-b7e7-a9f8e81bf727
TQID: https://experienceleague.adobe.com/AioKERGt0FLv1eBE5-evwa2d35fItwknWI-ZouBECSo
product_v2:
  - id: c4a86a5d-6562-4fc6-aa00-bfa25833aed9
feature_v2:
  - id: a0dacc9f-0e23-495b-8e9f-a77c2e60b40c
subfeature_v2:
  - id: b91c0848-76c4-4da4-8b81-3aade0518dd0
  - id: f0dd7b45-76b5-49d4-afe3-39f436b6fbd3
role_v2:
  - id: b69b2659-1057-424e-8fc5-ed9e016dc554
source-git-commit: 55a9d9feae8cc1128e3427a8874414ba734dd467
workflow-type: tm+mt
source-wordcount: 322
ht-degree: 0%

---

# 작업 종속성 유형 개요

<!-- Audited: 12/2023 -->

종속성 유형 은 작업 간의 전임 작업 관계를 나타냅니다. 종속 작업은 전임 작업의 시작 또는 완료에 따라 시작 또는 완료가 가능한 시기를 정의합니다.

>[!IMPORTANT]
>
>Adobe Workfront에서는 전임 작업 관계가 강제 적용되지 않는 한 종속성 유형에 따라 종속 작업이 시작되거나 종료되지 않도록 제한하지 않습니다. 전임 작업을 적용하는 방법에 대한 자세한 내용은 [전임 작업 적용](../../../manage-work/tasks/use-prdcssrs/enforced-predecessors.md)을 참조하십시오.

작업 간에 이 관계를 설정할 때 전임 작업 관계의 종속성 유형을 지정해야 합니다.

전임 작업에 대한 자세한 내용은 [작업 전임 작업 개요](../../../manage-work/tasks/use-prdcssrs/predecessors-overview.md)를 참조하십시오.

다음은 Workfront 종속성 유형입니다.

* **마침-시작(fs)**: 종속 작업을 시작하려면 먼저 전임 작업을 완료해야 합니다. 다른 종속성 유형이 지정되지 않은 경우 사용되는 기본 종속성 유형입니다.
* **완료-마침(ff)**: 종속 작업을 완료하려면 먼저 전임 작업을 완료해야 합니다.
* **시작-시작(ss)**: 종속 작업을 시작하려면 먼저 전임 작업을 시작해야 합니다. 전임 작업 이(가) 적어도 시작되지 않은 경우 종속 작업을 시작할 수 없습니다.
* **시작-완료(sf)**: 종속 작업을 완료하려면 먼저 전임 작업을 시작해야 합니다. 전임 작업이 시작되기 전에 종속 작업을 시작할 수 있지만 전임 작업이 시작되지 않으면 완료할 수 없습니다.
* **예약된 시작(sd)**: 작업을 완료-시작으로 예약하지만 실제 적용 유형은 완료-완료입니다. 이 옵션을 사용하면 전임 작업이 완료된 후 종속 작업이 시작되도록 예약됩니다. 단, 종속 작업은 언제든지 시작할 수 있지만 전임 작업이 완료될 때까지 완료할 수 없습니다.

>[!NOTE]
>
>종속성 유형에 대한 약자는 작업 목록에서 전임 작업 관계를 정의하는 데 사용됩니다. 자세한 내용은 [작업 전임 작업 개요](/help/quicksilver/manage-work/tasks/use-prdcssrs/predecessors-overview.md)의 [작업 목록에 있는 전임 작업 값의 예](/help/quicksilver/manage-work/tasks/use-prdcssrs/predecessors-overview.md#examples-of-predecessor-values-in-a-task-list)를 참조하십시오.

