---
content-type: reference
product-area: reports and dashboards
navigation-topic: data connect
title: Data Connect 쿼리 예
description: 예제 쿼리를 사용하여 특정 종류의 쿼리의 구문 및 구조를 숙지할 수 있습니다.
author: Nolan
feature: Reports and Dashboards
exl-id: f2da081c-bdce-4012-9797-75be317079ef
source-git-commit: c8a25bcc8c9b56a649ca7764918c86f9cdd5b3e2
workflow-type: tm+mt
source-wordcount: '923'
ht-degree: 0%

---

# Workfront Data Connect 쿼리 예제

Workfront Data Connect 데이터를 보다 효율적으로 활용할 수 있도록, 이 페이지에는 특정 종류의 쿼리의 구문 및 구조에 익숙해지는 데 사용할 수 있는 기본 예제 쿼리가 포함되어 있습니다.

## 사용자 지정 데이터 쿼리

이 예에서는 쿼리를 작성하여 사용자 정의 양식 및 사용자 정의 필드와 같은 Workfront에서 사용자 정의 데이터를 반환하는 방법을 보여 줍니다.

### 시나리오

조직은 재무 통합이라는 사용자 정의 양식을 사용합니다. 양식은 모든 프로젝트에 첨부되며 다음 필드를 포함합니다.

* **사업부**: 문자열을 포함하는 사용자 지정 필드입니다.
* **ProjectID**: 숫자 문자열이 포함된 사용자 지정 필드입니다.
* **확장된 프로젝트 이름**: 비즈니스 단위, ProjectID 및 기본 Workfront 프로젝트 이름의 값을 단일 문자열로 연결하는 계산된 사용자 지정 데이터 필드입니다.

Data Connect에 대한 쿼리 응답에 이 정보를 포함해야 합니다. 데이터 레이크의 레코드에 대한 사용자 지정 데이터 값이 제목이 `parametervalues`인 열에 포함되어 있습니다. 이 열은 JSON 개체로 저장됩니다.

### 쿼리

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

### 응답

위의 쿼리는 다음 데이터를 반환합니다.

* `projectid`: 기본 Workfront 프로젝트 ID입니다.
* `parametervalues`: JSON 개체를 저장하는 열입니다.
* `name`: 기본 Workfront 프로젝트 이름입니다.
* `Business Unit`: `parametervalues` 개체에 포함된 사용자 지정 데이터 값입니다.
* `Project ID`: `parametervalues` 개체에 포함된 사용자 지정 데이터 값입니다.
* `Expanded Project Name`: `parametervalues` 개체에 포함된 사용자 지정 데이터 값입니다.

### 설명

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

## 상태 시간 쿼리

이 예에서는 프로젝트가 이전에 할당된 상태에서 소비한 시간을 측정하는 방법을 보여 줍니다. 상태에서 작업 또는 문제 시간을 측정하거나 객체에 다른 속성(사용자 정의 데이터 값 포함)이 적용된 시간을 측정하도록 쉽게 조정할 수 있습니다.

### 시나리오

조직 리더쉽은 작업 수명주기의 각 단계에서 너무 많은 시간을 소비하고 있다고 생각합니다. 프로세스를 개선하기 위한 권장 사항을 만들기 전에 시간이 지남에 따라 프로젝트 상태가 변경되는 빈도와 프로젝트가 지정된 상태에 머무르는 일 수에 대한 기준선 측정을 만들어야 합니다.

PROJECTS_EVENT 데이터 보기를 사용하여 프로젝트 객체에 대해 각 상태 변경 목록을 가져옵니다. 새 상태를 이전 상태와 비교하고, 이전에 할당된 상태의 유효 시간 범위를 가져온 다음, 해당 상태에서 보낸 일수를 계산합니다.

프로젝트당 각 상태에서 보낸 시간의 이 원시 출력을 사용하여 시각화를 작성하거나 데이터를 추가로 집계하여 상태, 프로젝트 유형 또는 연도별 상태 기간 평균을 작성할 수 있습니다. 그런 다음 이 기준선은 리더십의 기대에 부응하기 위해 측정할 수 있는 벤치마크를 설정하는 데 사용됩니다.

다음 쿼리는 Data Connect PROJECTS_EVENTS 데이터 보기를 사용하여 각 프로젝트 상태 변경 이벤트를 비교하고 상태의 시간을 표시합니다.

### 쿼리

```
-- Calculate the begin/end effective timestamp and duration in days 

SELECT 

    projectid, 
    name as project_name, 
    prev_status as previous_status, 
    status, 
    status_change_date as status_begin_effective_timestamp, 
    case 
        when status_change_date is null then NULL
        else
            nvl(lead(status_change_date) ignore nulls over (partition by projectid order by status_change_date), current_timestamp) 
    end as status_end_effective_timestamp, 
    datediff('DAYS',status_change_date, nvl(lead(status_change_date) ignore nulls over (partition by projectid order by status_change_date), current_timestamp)) as status_duration_days 

FROM 
    ( -- Filter to just the records that have changed 
     SELECT projectid, 
        name, 
        prev_status, 
        status, 
        begin_effective_timestamp as status_change_date    
     FROM 
        (  -- Calculate records where previous status is different 
          SELECT DISTINCT  
           pe.projectid, 
           pe.name AS name, 
           pe.STATUS, 
           nvl(lag(pe.STATUS) over (partition by pe.projectid order by pe.BEGIN_EFFECTIVE_TIMESTAMP), status) prev_status, 
           begin_effective_timestamp 

          FROM projects_event pe 
         -- Set any WHERE conditions to limit the results as needed 
         --WHERE 
            -- pe.PROJECTID = '5ebe…c1e1' 
        ) 
        WHERE prev_status != status 
    ) 
    order by status_change_date; 
```

### 응답

위의 쿼리는 다음 데이터를 반환합니다.

* `PROJECTID`: 상태 변경 이벤트와 연결된 Workfront 프로젝트 ID입니다.
* `PROJECT_NAME`: Workfront 프로젝트 이름입니다.
* `PREVIOUS_STATUS`: 변경 바로 전의 프로젝트 상태입니다.
* `STATUS`: 변경 후 프로젝트의 상태입니다.
* `STATUS_BEGIN_EFFECTIVE_TIMESTAMP`: 이전 상태가 설정된 경우 변경 이벤트 타임스탬프입니다.
* `STATUS_END_EFFECTIVE_TIMESTAMP`: 업데이트된 상태 값이 설정된 경우 변경 이벤트 타임스탬프입니다.
* `STATUS_DURATION_DAYS`: 최종 유효 타임스탬프와 시작 유효 타임스탬프의 차이(일)입니다.

### 설명

이 쿼리는 Data Connect의 변경 이벤트 추적 기능을 사용합니다.  이전 이벤트와 다른 새 상태 값이 있었던 이벤트가 트리거된 날짜를 결정합니다. 

쿼리를 처음부터 끝까지 검사합니다. 

1. 이전 상태가 다른 레코드 계산: 
   * 모든 변경 이벤트에 대해 lag() 함수를 사용하여 상태의 이전 값을 식별합니다. 

2. 변경된 레코드만 필터링: 

   * 1단계의 계산에서 이전 상태가 인 레코드를 선택합니다.= 현재 상태. 

3. 시작/종료 유효 타임스탬프 및 기간(일) 계산: 

   * `<status_begin_effective_timestamp>`: 2단계에서 계산됩니다. 

   * `<status_end_effective_timestamp>`: 다음(lead())을 기준으로 계산됩니다. `<status_begin_effective_timestamp>`: `<status_begin_effective_timestamp>`이(가) NULL이 아닌 경우에만 상태를 표시합니다. 
   * `<status_duration_days>`: `<status_begin_effective_timestamp>`과(와) `<status_end_effective_timestamp>` 간의 데이터 차이입니다. 

>[!NOTE]
>
>PowerBI 또는 Tableau에서 이 쿼리를 자체 &quot;보기&quot;로 사용하는 것이 좋습니다.  `<object>_event view`에서 다른 필드를 가져오려면 이 쿼리의 출력을 `<object>_event view`(으)로 다시 조인합니다.  조인 필드는 다음과 같습니다. <br>
>&#x200B;>projects_event의 경우 
>&#x200B;>`From projects_event p`
>&#x200B;>`Join <above query> c on c.projectid = p.projectid  `
>&#x200B;>`and c. status_begin_effective_timestamp = p begin_effective_timestamp`



<!--## Task query 

Join the project and (assignedTo) users tables into a simple task list.



## Hours query

Join owner (users), hour type, and portfolio tables to provide a sum of hours by user and portfolio for the current year.



## Document approvals query

Measure the cycle time and average number of review cycles per asset.-->
