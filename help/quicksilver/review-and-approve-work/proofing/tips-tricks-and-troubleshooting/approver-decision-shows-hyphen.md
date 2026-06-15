---
content-type: tips-tricks-troubleshooting
product-area: documents
navigation-topic: tips-tricks-and-troubleshooting-proofing-within-workfront
title: 승인자 결정 시 증명 승인 보고서에 하이픈이 표시됨
description: 증명 승인 보고서의 승인자 결정 필드에 하이픈이 있으면 수신자가 더 이상 증명에서 의사 결정 역할에 있지 않음을 나타냅니다.
author: Courtney
role_v2: id: b69b2659-1057-424e-8fc5-ed9e016dc554
topic_v2: id: c1579802-ddd4-4214-8a91-97b2066abe11
source-git-commit: 25d403b9266c31a39c1dce6c1c45ad96ee90af28
workflow-type: tm+mt
source-wordcount: 287
ht-degree: 0%

---

# 승인자 결정 시 증명 승인 보고서에 하이픈이 표시됨

## 문제

증명 승인 보고서에서, 결정 날짜 필드에 날짜가 표시되고 결정 대기 중 이 False임에도 불구하고 수신자의 승인자 결정 필드에 하이픈(-)이 표시됩니다.

![승인자 결정에 증명 승인 보고서에 하이픈이 표시됨](assets/approver-decision-hyphen.png)

## 원인

승인자 결정 필드에 하이픈이 있으면 수신자는 더 이상 증명에서 결정 역할을 하지 않습니다. 이 문제는 다음과 같은 경우에 발생할 수 있습니다.

* 수신자가 증명에 추가되고 결정을 내렸으며 나중에 워크플로우에서 제거되었습니다. 수신자가 증명을 다시 방문할 경우 증명 시스템이 의사 결정 변경으로 방문을 기록합니다. 수신자가 더 이상 승인자가 아니므로 시스템에서 새 결정을 하이픈으로 기록합니다.
* 수신자의 증명 역할이 검토자와 같이 승인 권한이 포함되지 않은 역할로 변경되었습니다. 증명에서 각 역할이 수행할 수 있는 작업에 대한 자세한 내용은 [증명 역할 개요](../../../review-and-approve-work/proofing/proofing-overview/proof-roles.md)를 참조하십시오.
* 수신자의 증명 권한 프로필이 결정 후 다운그레이드되었습니다.

## 보고서에서 이것이 의미하는 바는 무엇입니까?

하이픈은 의도적으로 사용하는 것입니다. 시스템은 수신자가 증명을 승인할 때까지 기다리지 않으며 수신자는 더 이상 증명에 대한 의사 결정 역할을 하지 않습니다.

결정 날짜 필드에는 수신자의 가장 최근 결정 활동의 날짜가 여전히 표시되지만, 더 이상 수신자의 결정이 보고서에 계산되지 않습니다.

증명 승인 보고서를 만들고 사용하는 방법에 대한 자세한 내용은 [증명 승인 보고서 사용](../../../review-and-approve-work/proofing/managing-proofs-within-workfront/proof-approval-report.md)을 참조하세요.
