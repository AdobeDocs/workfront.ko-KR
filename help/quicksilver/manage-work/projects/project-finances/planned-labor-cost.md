---
content-type: overview;how-to-procedural
product-area: projects
navigation-topic: financials
title: 계획된 인건비 계산
description: 프로젝트에 대한 작업을 계획할 때 Adobe Workfront은 시간당 비용 값을 기반으로 이 작업에 할당된 역할 및 사용자의 계획된 인건비를 계산합니다.
author: Lisa
feature: Work Management
exl-id: af053e9a-09dc-4b4d-8ed4-f681ed611a59
source-git-commit: 6afa65f921864403c10541d283ef717dce81aed7
workflow-type: tm+mt
source-wordcount: '309'
ht-degree: 0%

---

# 계획된 인건비 계산

프로젝트에 대한 작업을 계획할 때 Adobe Workfront은 시간당 비용 값을 기반으로 이 작업에 할당된 역할 및 사용자의 계획된 인건비를 계산합니다.

프로젝트의 계획된 인건비는 프로젝트의 작업을 완료하기 위해 할당된 작업 역할 또는 사용자와 관련된 비용과 각 역할 또는 사용자가 해당 작업을 완료하는 데 소요될 수 있는 계획된 시간(계획된 시간) 사이의 계산입니다.

## 계획된 인건비 개요

프로젝트의 **계획된 인건비**&#x200B;는 프로젝트에 있는 모든 작업의 계획된 인건비를 모두 더하여 계산됩니다.

>[!TIP]
>
>문제 또는 프로젝트 자체와 연관된 계획된 인건비는 없습니다.

Workfront은 다음 공식을 사용하여 프로젝트의 계획된 인건비를 계산합니다.

```
Project Planned Labor Cost= SUM(Tasks Planned Labor Cost)
```

태스크 계획 노무비는 다음을 기준으로 계산됩니다.

* 작업에 대한 리소스 수 및 작업에 대한 개별 할당
* 작업의 비용 유형입니다.

태스크 계획 노무비는 다음 공식을 사용하여 계산됩니다.

```
Task Planned Cost = Planned Hours x User or Job Role Cost Per Hour
```

Workfront에서 작업 할당 및 비용 유형에 따라 작업의 계획된 인건비를 계산하는 방법에 대한 자세한 내용은 [비용 추적](../../../manage-work/projects/project-finances/track-costs.md) 문서의 &quot;개별 작업의 비용 유형 수정&quot; 섹션을 참조하십시오.

## 계획된 인건비 찾기

Workfront의 다음 영역에서 프로젝트의 계획된 인건비를 찾을 수 있습니다.

* 프로젝트 보고서
* 프로젝트 목록
* 시간 경과에 따라 추적할 수 있는 기준선 보고서
* API를 통해

보고서 만들기 및 Workfront API 사용에 대한 자세한 내용은 다음 문서를 참조하십시오.

* [사용자 지정 보고서 만들기](../../../reports-and-dashboards/reports/creating-and-managing-reports/create-custom-report.md)
* [API 기본 사항](../../../wf-api/general/api-basics.md)
