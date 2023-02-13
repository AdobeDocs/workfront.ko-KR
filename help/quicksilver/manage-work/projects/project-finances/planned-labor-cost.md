---
content-type: overview;how-to-procedural
product-area: projects
navigation-topic: financials
title: 계획된 인건비 계산
description: 프로젝트에서 작업을 계획하면, Adobe Workfront에서 해당 시간당 비용 값을 기준으로 이 작업에 지정된 역할과 사용자에게 할당된 역할에 대한 계획된 인건비 비용을 계산합니다.
author: Alina
feature: Work Management
exl-id: af053e9a-09dc-4b4d-8ed4-f681ed611a59
source-git-commit: f2f825280204b56d2dc85efc7a315a4377e551c7
workflow-type: tm+mt
source-wordcount: '309'
ht-degree: 0%

---

# 계획된 인건비 계산

프로젝트에서 작업을 계획하면, Adobe Workfront에서 해당 시간당 비용 값을 기준으로 이 작업에 지정된 역할과 사용자에게 할당된 역할에 대한 계획된 인건비 비용을 계산합니다.

프로젝트의 계획 노무비는 Job 역할과 연관된 원가 또는 프로젝트에서 작업을 완료하도록 지정된 사용자와 각 역할이나 사용자가 해당 작업을 완료하도록 할 수 있는 계획된 시간(계획됨 시간) 사이의 계산입니다.

## 계획된 인건비 개요

다음 **계획된 인건비** 프로젝트의 모든 태스크의 모든 계획된 노무비를 추가하여 프로젝트의 금액을 계산합니다.

>[!TIP]
>
>문제 또는 프로젝트 자체와 관련된 계획된 인건비 비용이 없습니다.

Workfront은 다음 공식을 사용하여 프로젝트의 계획된 인건비 원가를 계산합니다.

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

태스크 지정 및 원가 유형에 따라 Workfront에서 태스크에 대한 계획 노무비 계산 방법에 대한 자세한 내용은 문서의 &quot;개별 태스크에 대한 원가 유형 수정&quot; 섹션을 참조하십시오 [비용 추적](../../../manage-work/projects/project-finances/track-costs.md).

## 계획된 노무비 찾기

Workfront의 다음 영역에서 프로젝트의 계획 노무비를 찾을 수 있습니다.

* 프로젝트 보고서
* 프로젝트 목록
* 시간 경과에 따라 추적할 수 있는 기준 보고서
* API 사용

보고서 작성 및 Workfront API 사용에 대한 자세한 내용은 다음 문서를 참조하십시오.

* [사용자 지정 보고서 만들기](../../../reports-and-dashboards/reports/creating-and-managing-reports/create-custom-report.md)
* [API 기본 사항](../../../wf-api/general/api-basics.md)
