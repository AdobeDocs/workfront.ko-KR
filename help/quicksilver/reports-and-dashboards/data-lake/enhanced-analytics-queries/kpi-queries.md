---
content-type: overview;reference
product-area: reports and dashboards
navigation-topic: data connect
title: KPI 쿼리
description: 향상된 Analytics 쿼리
author: Courtney
feature: Reports and Dashboards
recommendations: noDisplay, noCatalog
hide: true
hidefromtoc: true
source-git-commit: eccecaece64b78aa19444407b182ea80b2115a63
workflow-type: tm+mt
source-wordcount: '385'
ht-degree: 2%

---


# KPI 쿼리

이 문서의 쿼리를 사용하여 고급 Analytics의 시각화와 유사한 데이터 시각화를 만들 수 있습니다.

>[!IMPORTANT]
>
>쿼리는 향상된 Analytics에 표시된 결과와 유사한 결과를 생성하지만 정확히 일치하지 않을 수 있습니다.


## 전제 조건

시작하기 전에 다음을 수행해야 합니다

1. Business Intelligence(BI) 도구와의 연결 설정:
   1. [Snowflake에 대한 Reader 계정 또는 연결 만들기](/help/quicksilver/reports-and-dashboards/data-lake/create-a-reader-account.md)
   1. [Workfront Data Connect에 연결 설정](/help/quicksilver/reports-and-dashboards/data-lake/share-data-externally.md)

연결을 설정한 후에는 이 문서의 쿼리를 사용하여 데이터를 추출하고 시각화할 수 있습니다.

## 프로젝트 완료됨

프로젝트 완료 KPI는 필터링된 기간 내에 완료된 프로젝트 수와 이전 기간 이후 증가하거나 감소된 백분율을 보여줍니다. 이 숫자 아래에 이전 기간에 완료된 프로젝트 수와 이전 기간의 일 수를 볼 수 있습니다.

![KPI 프로젝트 완료됨](assets/kpi-projects-completed-350x182.png)

### 쿼리

```
WITH completedProjectsInRange as ( 
SELECT COUNT(t0.PROJECTID) as PROJECT_COUNT FROM PROJECTS_CURRENT t0 
WHERE t0.ACTUALCOMPLETIONDATE >= '2025-01-01' 
AND t0.ACTUALCOMPLETIONDATE <= '2025-01-31' 
), completedProjectsPreviousRange as ( 
SELECT COUNT(t0.PROJECTID) as PROJECT_COUNT FROM PROJECTS_CURRENT t0 
WHERE t0.ACTUALCOMPLETIONDATE >= '2024-12-01' 
AND t0.ACTUALCOMPLETIONDATE <= '2024-12-31' 
), rawChange as ( 
SELECT (a.PROJECT_COUNT - b.PROJECT_COUNT) as CHANGE_FROM_PREVIOUS_PERIOD FROM completedProjectsInRange a, completedProjectsPreviousRange b 
), percentChange as ( 
SELECT  
CASE 
WHEN a.PROJECT_COUNT = b.PROJECT_COUNT THEN 0.00 
WHEN b.PROJECT_COUNT > 0 THEN ((a.PROJECT_COUNT - b.PROJECT_COUNT) / b.PROJECT_COUNT * 100) 
END AS PERCENT_CHANGE_FROM_PREVIOUS_PERIOD 
FROM completedProjectsInRange a, completedProjectsPreviousRange b 
) 
SELECT 
a.PROJECT_COUNT, 
b.PROJECT_COUNT as PREVIOUS_PROJECT_COUNT, 
c.CHANGE_FROM_PREVIOUS_PERIOD, 
d.PERCENT_CHANGE_FROM_PREVIOUS_PERIOD 
FROM completedProjectsInRange a, completedProjectsPreviousRange b, rawChange c, 
percentChange d
```

## 프로젝트가 정시에 완료됨

정시에 완료된 프로젝트 KPI는 필터링된 기간 내에 정시에 완료된 프로젝트의 백분율과 이전 기간 이후 백분율이 증가 또는 감소했는지 보여 줍니다. 이 숫자 아래에 이전 기간의 일수는 물론 이전 기간의 정시에 완료된 프로젝트의 백분율도 표시됩니다.

![KPI 프로젝트가 정시에 완료됨](assets/kpi-projects-completed-on-time-350x180.png)

## 평균 프로젝트 기간

평균 프로젝트 기간 KPI는 필터링된 기간 내에 실제 종료 일자가 있는 프로젝트의 평균 완료 시간(일, 주 또는 년)과 이전 기간 이후 백분율 증가 또는 감소를 표시합니다. 이 숫자 아래에 이전 기간의 일 수뿐만 아니라 이전 기간의 실제 종료 일자가 있는 프로젝트의 평균 완료 시간을 볼 수 있습니다.

![KPI 평균 프로젝트 기간](assets/kpi-avg.-project-duration-350x168.png)

## 프로젝트별 평균 작업

Avg, Tasks per project KPI는 필터링된 기간 내에 프로젝트에 할당된 작업의 평균 수와 이전 기간 이후 증가하거나 감소된 백분율을 보여줍니다. 이 숫자 아래에는 이전 기간의 평균 프로젝트 할당 작업 수와 이전 기간의 일 수를 볼 수 있습니다.

![프로젝트당 KPI 평균 작업](assets/kpi-average-tasks-per-project-350x179.png)