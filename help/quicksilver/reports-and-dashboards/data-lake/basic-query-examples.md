---
content-type: reference
product-area: reports and dashboards
navigation-topic: data connect
title: Data Connect 쿼리 예
description: 예제 쿼리를 사용하여 특정 종류의 쿼리의 구문 및 구조를 숙지할 수 있습니다.
author: Nolan
feature: Reports and Dashboards
recommendations: noDisplay, noCatalog
exl-id: f2da081c-bdce-4012-9797-75be317079ef
source-git-commit: 84f7f80314e4acafb0414b806f7b1e1e4b2845fc
workflow-type: tm+mt
source-wordcount: '246'
ht-degree: 0%

---

# Workfront Data Connect 쿼리 예제

Workfront Data Connect 데이터를 보다 효율적으로 활용할 수 있도록, 이 페이지에는 특정 종류의 쿼리의 구문 및 구조에 익숙해지는 데 사용할 수 있는 기본 예제 쿼리가 포함되어 있습니다.

## 사용자 지정 데이터 쿼리

이 예에서는 쿼리를 작성하여 사용자 정의 양식 및 사용자 정의 필드와 같은 Workfront에서 사용자 정의 데이터를 반환하는 방법을 보여 줍니다.

### 시나리오:

Finance Integration이라는 사용자 정의 양식을 활용하는 조직 양식은 모든 프로젝트에 첨부되며 다음 필드를 포함합니다.

* **사업부** - 문자열을 포함하는 사용자 지정 필드입니다.
* **ProjectID** - 숫자 문자열이 포함된 사용자 지정 필드입니다.
* **확장된 프로젝트 이름** - Business Unit, ProjectID 및 기본 Workfront 프로젝트 이름의 값을 단일 문자열로 연결하는 계산된 사용자 지정 데이터 필드입니다.

Data Connect에 대한 쿼리 응답에 이 정보를 포함해야 합니다. 데이터 레이크의 레코드에 대한 사용자 지정 데이터 값이 제목이 `parameterValues`인 열에 포함되어 있습니다. 이 열은 JSON 개체로 저장됩니다.

### 쿼리:

```
SELECT
    projectid,
    parametervalues,
    name,
    parametervalues:"DE:Business Unit" :: int as BusinessUnit,
    parametervalues:"DE:Project ID" :: int as ProjectID,
    parametervalues:"DE:Expanded Project Name" :: text as ExpandedProjectName
FROM PROJECTS_CURRENT
WHERE ExpandedProjectName is not null
```

### 응답

위의 쿼리는 다음 데이터를 반환합니다.

* `projectid` - 기본 Workfront 프로젝트 ID
* `parametervalues` - JSON 개체를 저장하는 열
* `name` - 기본 Workfront 프로젝트 이름
* `Business Unit` - `parametervalues` 개체에 포함된 사용자 지정 데이터 값
* `Project ID` - `parametervalues` 개체에 포함된 사용자 지정 데이터 값
* `Expanded Project Name` - `parametervalues` 개체에 포함된 사용자 지정 데이터 값

<!--## Task query 

Join the project and (assignedTo) users tables into a simple task list.



## Hours query

Join owner (users), hour type, and portfolio tables to provide a sum of hours by user and portfolio for the current year.



## Document approvals query

Measure the cycle time and average number of review cycles per asset.-->
