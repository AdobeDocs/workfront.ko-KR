---
content-type: overview
product-area: documents
navigation-topic: proofing-overview
title: 자동화된 워크플로우 단계 개요
description: 증명 단계는 서로 다른 사용자가 증명을 검토하는 시간의 세그먼트입니다. 증명이 한 단계에서 다음 단계로 이동되면 Adobe Workfront은 검토자에게 작업할 시간이 되면 알려 줍니다.
author: Courtney
feature: Digital Content and Documents
exl-id: a03d2cf2-edb3-43b7-a739-32600f2ae2a0
source-git-commit: 54f4c136cfaaaaaa90a4fc64d3ffd06816cff9cb
workflow-type: tm+mt
source-wordcount: '401'
ht-degree: 0%

---

# 자동화된 워크플로우 단계 개요

증명 단계는 서로 다른 사용자가 증명을 검토하는 시간의 세그먼트입니다. 증명이 한 단계에서 다음 단계로 이동되면 Adobe Workfront은 검토자에게 작업할 시간이 되면 알려 줍니다.

![stage_diagram.png](assets/stages-diagram-350x63.png)

단계는 두 가지 서로 다른 상황에서 발생합니다.

* [자동화된 워크플로우를 사용하여 증명 만들기](#create-a-proof-with-an-automated-workflow)
* [증명에 따라 다양한 검토자의 마감일 지정](#assign-deadlines-for-different-reviewers-on-a-proof)

## 자동화된 워크플로우를 사용하여 증명 만들기 {#create-a-proof-with-an-automated-workflow}

증명에 자동화된 워크플로우를 추가하면 발생하는 검토 작업 단계를 설정합니다.

자동 워크플로우로 증명 단계를 설정하면

* 연속 또는 동시에 실행되도록 단계를 구성할 수 있습니다.
* 이전 단계가 완료된 후에만 일부 단계가 활성화되도록 구성할 수 있습니다.
* 몇 단계는 비공개로 할 수 있습니다 이 기능은 예를 들어, 클라이언트와 공유되기 전에 증명을 검토하고 결과 주석이 클라이언트에 표시되지 않도록 하는 에이전시에 유용합니다.

자동화된 워크플로우를 사용하여 증명을 위한 단계를 만드는 방법에 대한 지침은 [자동화된 워크플로우를 사용하여 고급 증명 만들기](../../../review-and-approve-work/proofing/creating-proofs-within-workfront/create-automated-proof-workflow.md).

>[!NOTE]
>
>사용자가 특정 단계에 포함되지 않지만 문서에 액세스할 수 있고 증명을 여는 경우 시스템에서 *Workfront*.
>
>증명을 연 사용자에게는 문서 증명을 여는 비수신자를 위한 설정 > 검토 및 승인 > 역할에 지정된 역할이 할당됩니다.

## 증명에 따라 다양한 검토자의 마감일 지정 {#assign-deadlines-for-different-reviewers-on-a-proof}

증명 시 검토자에게 서로 다른 언어 교정 기한을 지정하면 시스템에서 마감일 마다 스테이지를 만들고 해당 단계의 각 마감일 동안 검토자를 그룹화합니다. 

**예:** 예를 들어 검토자가 4명인 증명을 만들 경우:

* 검토자인 올리비아와 토니의 경우, 당신은 지금부터 며칠 후에 14시에 마감일을 지정하게 된다.
* Aaron과 Amy에게, 당신은 며칠 후에 17시에 마감일을 지정합니다.
* 마감일을 직접 지정하지는 않습니다.

시스템은 이러한 세 개의 검토자 그룹 각각에 대한 스테이지를 만듭니다.

![stage.png](assets/stages-350x239.png)

증명을 다른 검토자와 공유하고 최종 기한을 지정하지 않으면 Workfront에서 사용자를 3단계에 추가합니다. 여기서 마감일은 없습니다. 
