---
content-type: reference
product-area: reports and dashboards
navigation-topic: data connect
title: Data Connect 쿼리 예
description: 예제 쿼리를 사용하여 특정 종류의 쿼리의 구문 및 구조를 숙지할 수 있습니다.
author: Courtney
feature: Reports and Dashboards
exl-id: f2da081c-bdce-4012-9797-75be317079ef
last-update: 2026-04-01T18:03:50.000Z
git-commit-file: b03dbe8e217593e0f3a6fcd522148dcd8b7670b8
TQID: https://experienceleague.adobe.com/flDonZVaLR3bTF2aZcY9iy2ZnWbfrdhctL7J8esvxng
product_v2:
  - id: c4a86a5d-6562-4fc6-aa00-bfa25833aed9
role_v2:
  - id: b69b2659-1057-424e-8fc5-ed9e016dc554
topic_v2:
  - id: aa2f3246-cb95-4b30-8899-fdf7d73550cc
  - id: c2be0313-b3ae-45e0-b454-d20bf54b23f2
source-git-commit: edee967a5c19d86fd471c4571a0b458f72bf370e
workflow-type: tm+mt
source-wordcount: 2201
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

이 쿼리는 Data Connect의 변경 이벤트 추적 기능을 사용합니다. 이전 이벤트와 다른 새 상태 값이 발생한 이벤트가 트리거된 날짜를 결정합니다. 

쿼리를 처음부터 끝까지 검사합니다. 

1. 이전 상태가 다른 레코드 계산: 
   * 모든 변경 이벤트에 대해 lag() 함수를 사용하여 상태의 이전 값을 식별합니다. 

2. 변경된 레코드만 필터링: 

   * 1단계의 계산에서 이전 상태가 현재 상태인 레코드!= 선택합니다. 

3. 시작/종료 유효 타임스탬프 및 기간(일) 계산: 

   * `<status_begin_effective_timestamp>`: 2단계에서 계산됩니다. 

   * `<status_end_effective_timestamp>`: 다음(lead())을 기준으로 계산됩니다. `<status_begin_effective_timestamp>`: `<status_begin_effective_timestamp>`이(가) NULL이 아닌 경우에만 상태를 표시합니다. 
   * `<status_duration_days>`: `<status_begin_effective_timestamp>`과(와) `<status_end_effective_timestamp>` 간의 데이터 차이입니다. 

>[!NOTE]
>
>PowerBI 또는 Tableau에서 이 쿼리를 자체 &quot;보기&quot;로 사용하는 것이 좋습니다. `<object>_event view`에서 다른 필드를 가져오려면, 이 쿼리의 출력을 `<object>_event view`(으)로 다시 조인하십시오. 조인 필드는 다음과 같습니다. <br>
>projects_event: 
>`From projects_event p`>`Join <above query> c on c.projectid = p.projectid  `>`and c. status_begin_effective_timestamp = p begin_effective_timestamp`

## Planning: 단일 레코드 유형 쿼리

이 예에서는 Data Connect 데이터 레이크에 저장된 단일 레코드 유형에 대해 Workfront Planning 데이터를 쿼리하는 방법을 보여 줍니다.

### 시나리오

조직은 Workfront Planning을 사용하여 캠페인을 추적합니다. 각 캠페인 레코드에는 이름, 상태, 시작 날짜, 종료 날짜 및 소유자가 포함됩니다. 대시보드에서 사용할 모든 활성 캠페인과 주요 세부 정보 목록을 가져오려고 합니다.

* Planning 레코드 유형 데이터는 PLANNINGRECORD_CURRENT 뷰에 저장됩니다.
* 각 행은 단일 레코드를 나타내며 모든 필드 값은 FIELD_VALUES라는 JSON 열에 저장됩니다.
* 레코드 종류는 RECORDTYPEID 열로 식별됩니다.
* 레코드의 작업 영역은 WORKSPACEID 열(또는 사람이 읽을 수 있는 필터의 경우 WORKSPACENAME 열)로 식별됩니다.

### 쿼리

```sql
SELECT
  recordid,
  FIELD_VALUES:"Name"::text AS campaign_name,
  FIELD_VALUES:"Status"::text AS campaign_status,
  FIELD_VALUES:"Start Date"::date AS start_date,
  FIELD_VALUES:"End Date"::date AS end_date,
  FIELD_VALUES:"Owner"::text AS owner
FROM PLANNINGRECORD_CURRENT
WHERE WORKSPACEID = '<your_campaign_workspace_id>'
AND RECORDTYPEID = '<your_campaign_record_type_id>'
AND FIELD_VALUES:"Status"::text = 'Active'
ORDER BY start_date ASC
```

### 응답

위의 쿼리는 다음 데이터를 반환합니다.

* **recordid**: 캠페인에 대한 고유한 계획 레코드 ID입니다.
* **campaign_name**: FIELD_VALUES JSON 개체에서 추출한 캠페인의 이름입니다.
* **campaign_status**: 캠페인의 현재 상태입니다.
* **start_date**: 날짜 데이터 형식으로 캐스팅된 캠페인의 시작 날짜입니다.
* **end_date**: 날짜 데이터 형식으로 캐스팅되는 캠페인의 종료 날짜입니다.
* **소유자**: 캠페인 소유자로 할당된 사용자 또는 팀의 이름입니다.

### 설명

Data Connect의 계획 레코드는 레코드 유형에 관계없이 단일 테이블 구조를 공유합니다. RECORDTYPEID 열은 쿼리를 특정 레코드 종류(이 경우 캠페인)로 범위를 지정하는 데 사용됩니다. `<your_campaign_record_type_id>`을(를) 쿼리할 레코드 형식의 ID로 바꾸십시오. ID는 Workfront Planning 레코드 형식 설정에서 또는 RECORDTYPE_CURRENT를 쿼리하여 찾을 수 있습니다.

필드 값은 FIELD_VALUES 열에 JSON 개체로 저장되며 사용자 정의 양식 데이터에 사용된 것과 동일한 콜론 표기법 구문을 사용하여 액세스됩니다.

```
<field_column>:"<field_name>"::<data_type> AS <alias>
```

필드 이름 참조는 대문자, 간격 및 이모지를 포함하여 Planning 레코드 유형 필드 구성에 정의된 필드 이름과 정확히 일치해야 합니다.

>[!NOTE]
>
>Planning 레코드 유형 ID는 Workfront Planning에서 레코드 유형을 볼 때 URL에서 찾을 수 있습니다. &quot;Rt...&quot;로 시작하는 URL의 경로입니다. 레코드 유형은 Data Connect 내에서 다음 SQL 호출을 통해서도 찾을 수 있습니다.
>
>
>```sql
>SELECT
>ID AS recordtypeid,
>DISPLAYNAME AS record_type_name,
>WORKSPACEID
>FROM RECORDTYPE_CURRENT
>ORDER BY record_type_name ASC
>```

## Planning: 연결된 레코드 유형 쿼리

이 예에서는 두 개의 연결된 Planning 레코드 유형(상위 레코드 유형 및 연결된 레코드 유형)에 걸쳐 데이터를 쿼리하는 방법을 보여 줍니다.

### 시나리오

조직은 Workfront Planning에서 캠페인 레코드를 Tactic 레코드에 연결합니다. 각 캠페인을 관련 전술의 주요 세부 사항과 함께 표시하는 보고서를 생성하려는 경우 특히 전술명, 전략 우선순위, 예산 배분을 제시해 리더십이 전술별로 구성된 캠페인 활동을 검토할 수 있게 하고자 한다.

Data Connect에서 기본 Planning 레코드 유형 간의 연결은 PLANNINGRECORD_CURRENT의 FIELD_VALUES_RAW 열에 직접 저장됩니다. &quot;Tactics&quot;라는 참조 필드의 경우 값은 연결된 레코드의 RECORDID가 있는 ID 속성이 각각 포함된 연결된 레코드 개체의 JSON 배열입니다. Snowflake의 LATERAL FLATTEN을 사용하여 이 배열을 행으로 확장하고 연결된 레코드 유형에 연결합니다.

### 쿼리

```sql
SELECT
  c.RECORDID AS campaign_id,
  c.FIELD_VALUES:"Name"::text AS campaign_name,
  c.FIELD_VALUES:"Status"::text AS campaign_status,
  t.FIELD_VALUES:"Name"::text AS tactic_name,
  t.FIELD_VALUES:"Strategic Priority"::text AS strategic_priority,
  t.FIELD_VALUES:"Budget Allocation"::float AS budget_allocation
FROM PLANNINGRECORD_CURRENT c,
INNER JOIN REFERENCE_CURRENT R 
ON r.FROM_REFERENCEID = c.REFERENCE_IDS:"Tactics"::text
INNER JOIN PLANNINGRECORD_CURRENT t
-- Join to the Tactic record using the connected record ID from the array
ON t.RECORDID = r.TO_RECORDID
WHERE c.RECORDTYPEID = '<your_campaign_record_type_id>'
ORDER BY tactic_name, campaign_name
```

### 응답

위의 쿼리는 다음 데이터를 반환합니다.

* **campaign_id**: 캠페인에 대한 고유한 계획 레코드 ID입니다.
* **campaign_name**: 캠페인 레코드의 이름.
* **campaign_status**: 캠페인의 현재 상태입니다.
* **tactic_name**: 연결된 전술 레코드의 이름입니다.
* **strategic_priority**: 연결된 전술 레코드의 전략 우선 순위 필드 값입니다.
* **budget_allocation**: 연결된 전술 레코드의 예산 할당 필드 값이 부동 소수점으로 캐스팅되었습니다.

### 설명 - 수정된 KP

기본 Planning 레코드 유형 간의 연결은 REFERENCE_CURRENT 조인 테이블에 저장됩니다.  REFERENCE_CURRENT 조인 테이블은 RecordType 간의 조인에 사용됩니다.   RecordType 사이에 조인할 때는 TO_RECORDID 필드를 사용해야 합니다.

PLANNINGRECORD 뷰의 REFERENCE_ID 열에는 해당 계획 레코드에 적용할 수 있는 모든 REFERENCEID 필드 목록이 포함됩니다. field_value와 동일한 JSON 표기법을 활용하여 ID에 액세스할 수 있습니다.

```
<reference_ids>:"<reference_name>"::text
```

REFERENCE_CURRENT 보기에는 TO_RECORDID가 PLANNINGRECORD 보기의 다른 계획 `recordId` 필드를 가리키는 레코드가 하나 이상 _*.

REFERENCE_CURRENT 및 PLANNINGRECORD에 대한 동일한 조인 패턴을 사용하여 다른 REFERENCE 필드를 추가 계획 레코드에 조인하려면 위의 _*에 뷰를 추가합니다.


## Planning: Workfront Workflow 데이터 쿼리에 연결된 레코드 유형

이 예에서는 REFERENCE_CURRENT 뷰에 외부 개체 참조를 저장하는 Planning의 기본 연결 기능을 사용하여 Workfront Planning 레코드 유형(이 경우 프로젝트)을 기본 Workfront Workflow 개체에 조인하는 방법을 보여 줍니다.

### 시나리오

조직은 Planning의 기본 연결 기능을 사용하여 Workfront Planning의 캠페인 레코드를 Workfront Projects에 연결합니다. 캠페인 관리자가 Planning 작업 공간 컨텍스트를 종료하지 않고 게재 진행률을 추적할 수 있도록 연결된 프로젝트(특히 프로젝트의 현재 완료율, 계획된 완료 일자 및 할당된 프로젝트 소유자)의 라이브 실행 데이터와 함께 캠페인 세부 사항을 표시하는 결합된 보고서를 생성하려고 합니다.

### 쿼리

```sql
SELECT
  c.RECORDID AS campaign_id,
  c.FIELD_VALUES:"Name"::text AS campaign_name,
  c.FIELD_VALUES:"Status"::text AS campaign_status,
  conn.TO_EXTERNALID AS linked_project_id,
  p.name AS project_name,
  p.percentcomplete AS project_percent_complete,
  p.plannedcompletiondate AS project_planned_completion,
  p.ownerid AS project_owner_id,
  u.name AS project_owner_name
FROM WORKFRONT.PLANNING.PLANNINGRECORD_CURRENT c
-- Join to the references table to find Workfront Project connections
INNER JOIN WORKFRONT.PLANNING.REFERENCE_CURRENT conn
ON conn.REFERENCE_ID = c.REFERENCE_IDS:"ProjectId"::text
-- Join to the Workfront Projects table on the external ID
INNER JOIN WORKFRONT.WF.PROJECTS_CURRENT p
ON p.projectid = conn.TO_EXTERNALID
-- Join to Users to resolve the project owner name
LEFT JOIN WORKFRONT.WF.USERS_CURRENT u
ON u.userid = p.ownerid
WHERE c.RECORDTYPEID = '<your_campaign_record_type_id>'
AND p.completiontype != 'CPL' -- Exclude completed projects
ORDER BY campaign_name
```

### 응답

위의 쿼리는 다음 데이터를 반환합니다.

* **campaign_id**: 캠페인에 대한 고유한 계획 레코드 ID입니다.
* **campaign_name**: 캠페인 레코드의 이름.
* **campaign_status**: Planning의 현재 캠페인 상태입니다.
* **linked_project_id**: 연결된 Workfront 프로젝트를 식별하는 REFERENCE_CURRENT.TO_EXTERNALID의 Workfront 프로젝트 ID입니다.
* **project_name**: PROJECTS_CURRENT의 기본 Workfront 프로젝트 이름입니다.
* **project_percent_complete**: 프로젝트의 현재 완료율 값입니다.
* **project_planned_completion**: 연결된 Workfront 프로젝트의 계획된 완료 날짜입니다.
* **project_owner_id**: 프로젝트 소유자의 Workfront 사용자 ID.
* **project_owner_name**: USERS_CURRENT에 가입하여 해결된 프로젝트 소유자의 표시 이름입니다.

### 설명

Planning 레코드 유형에서 기본 Workfront Workflow 객체로의 연결은 REFERENCE_CURRENT에 저장됩니다. 이 보기의 각 행은 하나의 방향 링크를 나타냅니다. TO_EXTERNALID에는 연결된 Workfront 객체의 ID가 저장됩니다. Workfront 연결을 나타내는 행은 `TO_EXTERNALCONNECTIONNAME = 'workfront'` 및 Workfront 개체 유형의 API 코드(예: PROJ for Projects)에 해당하는 TO_EXTERNALOBJECTNAME 값으로 식별됩니다.

PLANNINGRECORD 테이블의 REFERENCE_ID 열에는 해당 레코드에 적용할 수 있는 모든 REFERENCEID 필드 목록이 포함되어 있습니다.  field_value와 동일한 JSON 표기법을 활용하여 ID에 액세스할 수 있습니다.\
PLANNINGRECORD_CURRENT의 단일 REFERENCE_ID에는 REFERENCE_CURRENT 테이블에 하나 이상의 참조 링크가 포함되어 있을 수 있습니다. 이 링크는 Workfront 테이블에서 특정 객체 유형의 객체에 연결됩니다.

```
<reference_ids>:"<reference_name>"::text
```

Planning 뷰(PLANNINGRECORD_CURRENT, REFERENCE_CURRENT)는 WORKFRONT.PLANNING 스키마에 있는 반면 기본 Workfront Workflow 뷰(PROJECTS_CURRENT, USERS_CURRENT 등)는 Workfront.WF 스키마에 있습니다. 스키마 간 조인에는 정규화된 테이블 이름이 필요합니다.

쿼리는 세 개의 조인을 수행합니다.

1. **참조 테이블**&#x200B;에 대한 Planning 레코드: REFERENCE_CURRENT가 각 캠페인 레코드에서 시작된 모든 연결을 찾기 위해 `TO_RECORDID = c.RECORDID`에 결합됩니다. `TO_EXTERNALCONNECTIONNAME = 'workfront'` 및 `TO_EXTERNALOBJECTNAME = 'PROJ'`의 필터에서는 결과를 특별히 Workfront 프로젝트에 대한 연결을 나타내는 행으로 좁힙니다.
1. **Workfront 프로젝트에 대한 참조 테이블:** TO_EXTERNALID에는 연결된 프로젝트에 대한 기본 Workfront projectid가 있습니다. 라이브 프로젝트 데이터를 검색하기 위해 `PROJECTS_CURRENT.projectid`에 직접 연결됩니다.
1. **사용자에게 프로젝트:** USERS_CURRENT에 대한 LEFT JOIN은 프로젝트의 ownerid 외래 키를 사람이 읽을 수 있는 이름으로 확인합니다. 여기에 LEFT JOIN을 사용하여 할당된 소유자가 없는 프로젝트가 여전히 결과에 포함됩니다.

>[!NOTE]
>
>Planning 외부 테이블에 조인할 때 쿼리에서 TO_RECORDID 필드를 사용하지 마십시오.  외부 테이블에 조인할 때는 필요하지 않습니다.
>
>이 패턴은 TO_EXTERNALOBJECTNAME 필터를 적절한 객체 API 코드(예: 포트폴리오의 경우 PORT 또는 프로그램의 경우 PRGM)로 변경하고 해당 WORKFRONT.WF 테이블에 가입하여 Planning에서 프로젝트, 포트폴리오 또는 프로그램 등 연결을 지원하는 모든 Workfront Workflow 객체에 적용할 수 있습니다. 각 오브젝트 유형에 대한 올바른 테이블 및 ID 열 이름은 Workfront Data Connect 데이터 사전을 참조하십시오.

다른 REFERENCE 필드를 추가 외부 레코드에 연결하려면 REFERENCE_CURRENT 및 Workfront Workflow 뷰에 동일한 조인 패턴이 위의 쿼리에 추가됩니다.

외부 및 Planningrecord 값은 REFERENCE_CURRENT 테이블에 여러 번 조인하고 적절한 조인 패턴을 사용하여 동일한 쿼리에서 조인할 수 있습니다.


<!--
## Task query 

Join the project and (assignedTo) users tables into a simple task list.



## Hours query

Join owner (users), hour type, and portfolio tables to provide a sum of hours by user and portfolio for the current year.



## Document approvals query

Measure the cycle time and average number of review cycles per asset.
-->
