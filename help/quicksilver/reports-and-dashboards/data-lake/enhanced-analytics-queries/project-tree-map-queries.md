---
content-type: overview;reference
product-area: reports and dashboards
navigation-topic: data connect
title: 프로젝트 트리맵 쿼리
description: 향상된 Analytics 쿼리
author: Courtney
feature: Reports and Dashboards
recommendations: noDisplay, noCatalog
exl-id: 3943703a-0d0b-46d3-a708-52987d330523
source-git-commit: b18a7835c6de131c125b77c6688057638c62fa4a
workflow-type: tm+mt
source-wordcount: '110'
ht-degree: 0%

---

# 프로젝트 트리맵 쿼리

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

## 프로젝트 계획된 시간 중단

```
WITH task_daily_work as ( 
    SELECT 
        taskid, 
        projectid, 
        workrequired, 
        percentcomplete, 
        calendardate, 
        (workrequired - (workrequired * percentcomplete)) as remainingMinutes 
    FROM tasks_daily_history 
) 
 
SELECT 
    p.name, 
    p.projectid, 
    sum(tdw.workrequired) as projectTotalWork, 
    sum(tdw.remainingMinutes) as projectRemainingWork, 
    tdw.calendardate 
FROM projects_current p 
    JOIN task_daily_work tdw ON p.projectid = tdw.projectid 
GROUP BY p.projectid, p.name, tdw.calendardate
```

### 프로젝트 계획된 시간 중단: 번다운

```
WITH task_daily_work as ( 
    SELECT 
        taskid, 
        projectid, 
        workrequired, 
        percentcomplete, 
        calendardate, 
        (workrequired - (workrequired * percentcomplete)) as remainingMinutes 
    FROM tasks_daily_history 
) 
 
SELECT 
    p.name, 
    p.projectid, 
    sum(tdw.workrequired) as projectTotalWork, 
    sum(tdw.remainingMinutes) as projectRemainingWork, 
    tdw.calendardate 
FROM projects_current p 
    JOIN task_daily_work tdw ON p.projectid = tdw.projectid 
GROUP BY p.projectid, p.name, tdw.calendardate
```

## 프로젝트 계획 기간 중단됨 

```
WITH task_daily_work as ( 
    SELECT 
        taskid, 
        projectid, 
        planneddurationminutes, 
        percentcomplete, 
        calendardate, 
        (planneddurationminutes - (planneddurationminutes * percentcomplete)) as remainingDurationMinutes 
    FROM tasks_daily_history 
) 
 
SELECT 
    p.name, 
    p.projectid, 
    sum(tdw.planneddurationminutes) as projectTotalWork, 
    sum(tdw.remainingDurationMinutes) as projectRemainingWork, 
    tdw.calendardate 
FROM projects_current p 
    JOIN task_daily_work tdw ON p.projectid = tdw.projectid 
GROUP BY p.projectid, p.name, tdw.calendardate
```

### 프로젝트 계획된 기간 중단: 번다운

```
WITH task_daily_work as ( 
    SELECT 
        taskid, 
        projectid, 
        planneddurationminutes, 
        percentcomplete, 
        calendardate, 
        (planneddurationminutes - (planneddurationminutes * percentcomplete)) as remainingDurationMinutes 
    FROM tasks_daily_history 
) 
 
SELECT 
    p.name, 
    p.projectid, 
    sum(tdw.planneddurationminutes) as projectTotalWork, 
    sum(tdw.remainingDurationMinutes) as projectRemainingWork, 
    tdw.calendardate 
FROM projects_current p 
    JOIN task_daily_work tdw ON p.projectid = tdw.projectid 
GROUP BY p.projectid, p.name, tdw.calendardate
```
