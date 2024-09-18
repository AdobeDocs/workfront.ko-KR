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
source-git-commit: 364b668f23f5437e5cca0c4cc4793b17d444fb56
workflow-type: tm+mt
source-wordcount: '467'
ht-degree: 0%

---

# Workfront Data Connect 쿼리 예제

Workfront Data Connect 데이터를 보다 효율적으로 활용할 수 있도록, 이 페이지에는 특정 종류의 쿼리의 구문 및 구조에 익숙해지는 데 사용할 수 있는 기본 예제 쿼리가 포함되어 있습니다.

## 사용자 지정 데이터 쿼리

이 예에서는 쿼리를 작성하여 사용자 정의 양식 및 사용자 정의 필드와 같은 Workfront에서 사용자 정의 데이터를 반환하는 방법을 보여 줍니다.

### 시나리오:

조직은 재무 통합이라는 사용자 정의 양식을 사용합니다. 양식은 모든 프로젝트에 첨부되며 다음 필드를 포함합니다.

* **사업부** - 문자열을 포함하는 사용자 지정 필드입니다.
* **ProjectID** - 숫자 문자열이 포함된 사용자 지정 필드입니다.
* **확장된 프로젝트 이름** - Business Unit, ProjectID 및 기본 Workfront 프로젝트 이름의 값을 단일 문자열로 연결하는 계산된 사용자 지정 데이터 필드입니다.

Data Connect에 대한 쿼리 응답에 이 정보를 포함해야 합니다. 데이터 레이크의 레코드에 대한 사용자 지정 데이터 값이 제목이 `parametervalues`인 열에 포함되어 있습니다. 이 열은 JSON 개체로 저장됩니다.

### 쿼리:

```
SELECT
    projectid,
    parametervalues,
    name,
    parametervalues:"DE:Business Unit"::int as BusinessUnit,
    parametervalues:"DE:Project ID"::int as ProjectID,
    parametervalues:"DE:Expanded Project Name"::text as ExpandedProjectName
FROM PROJECTS_CURRENT
WHERE ExpandedProjectName is not null
```

### 응답:

위의 쿼리는 다음 데이터를 반환합니다.

* `projectid` - 기본 Workfront 프로젝트 ID
* `parametervalues` - JSON 개체를 저장하는 열
* `name` - 기본 Workfront 프로젝트 이름
* `Business Unit` - `parametervalues` 개체에 포함된 사용자 지정 데이터 값
* `Project ID` - `parametervalues` 개체에 포함된 사용자 지정 데이터 값
* `Expanded Project Name` - `parametervalues` 개체에 포함된 사용자 지정 데이터 값

### 설명:

`parametervalues` JSON 개체를 쿼리할 때 다음을 사용하여 각 사용자 지정 데이터 필드에 열로 액세스할 수 있습니다.

`<field_name>:"<parameter_name>"::<data_type> as <column_name>`

* `<field_name>`은(는) 쿼리 중인 테이블의 JSON 개체 이름입니다. 사용자 지정 데이터의 경우 항상 `parametervalues`입니다.
* `<parameter_name>`은(는) 양식 구성 도구에 있는 `parametername` 문자열이지만 항상 이 값과 일치하지는 않을 수 있습니다.

>[!NOTE]
>
>Workfront 양식 구성 도구에서 매개 변수의 이름이 변경되면 JSON 개체에 새 열로 표시됩니다. 따라서 양식 구성 도구에서 열을 만든 후에는 열 이름을 변경하지 않는 것이 좋습니다. 그러나 JSON 개체에 영향을 주지 않고 레이블을 변경할 수 있습니다.
>
>매개 변수 이름에 대한 텍스트 문자열이 잘못된 경우 이 열은 오류가 아닌 NULL 값을 반환합니다.

* `<data_type>`은(는) JSON 개체에서 반환되는 값을 필드에 적합한 데이터 형식으로 변환합니다. 반환되는 값에 대해 호환되지 않는 데이터 유형을 선택하면 데이터 유형 불일치 오류가 발생합니다. 가능한 데이터 유형은 다음과 같습니다.

   * `text`
   * `varchar`
   * `int`
   * `float`
   * `number(len,precision)`(예: `Number(32,4)`은(는) 1234.0987을 반환합니다.)
   * `date`
   * `timestamp`

* `<column_name>`은(는) 각 사용자 지정 데이터 열에 대해 만드는 레이블입니다.

>[!NOTE]
>
>양식에서 지정된 값이 있는 매개 변수만 JSON 개체에 포함됩니다. 양식에서 사용자 지정 데이터 필드가 비어 있으면 표시되지 않습니다.

<!--## Task query 

Join the project and (assignedTo) users tables into a simple task list.



## Hours query

Join owner (users), hour type, and portfolio tables to provide a sum of hours by user and portfolio for the current year.



## Document approvals query

Measure the cycle time and average number of review cycles per asset.-->
