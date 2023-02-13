---
content-type: tips-tricks-troubleshooting
product-area: timesheets
navigation-topic: tips-tricks-and-troubleshooting-timesheets
title: 비율이 변경될 때 재무 재계산 작업이 기록 시간에 영향을 주지 않도록 합니다
description: 인상이나 다른 상황으로 인해 사용자 또는 작업 역할에 대한 시간별 비용을 업데이트해야 하지만 이전에 프로젝트에 로그온한 시간에 영향을 주거나 기록 시간의 일부에만 영향을 주고자 하는 경우에는 이 변경을 원하지 않습니다.
author: Alina
feature: Timesheets
exl-id: 29d3124b-cf7a-4a47-95c4-cd5379489810
source-git-commit: 7786d899841cb82cc4d3832fb083c6e2bda2e197
workflow-type: tm+mt
source-wordcount: '188'
ht-degree: 0%

---

# 비율이 변경될 때 재무 재계산 작업이 기록 시간에 영향을 주지 않도록 합니다

## 문제

인상이나 다른 상황으로 인해 사용자 또는 작업 역할에 대한 시간별 비용을 업데이트해야 하지만 이전에 프로젝트에 로그온한 시간에 영향을 주거나 기록 시간의 일부에만 영향을 주고자 하는 경우에는 이 변경을 원하지 않습니다.

## 솔루션

프로젝트에서 청구 레코드로 변경하지 않으려는 시간을 추가하고 청구 레코드의 상태를 청구됨으로 설정합니다.  이 잠금은 이전 비율로 고정되며 재무 재계산 작업에서 무시됩니다.  청구됨 청구 레코드에 속하지 않는 모든 시간은 새 비율로 계산됩니다. 자세한 내용은 [프로젝트 재무 재계산](../../manage-work/projects/project-finances/recalculate-project-finances.md).
