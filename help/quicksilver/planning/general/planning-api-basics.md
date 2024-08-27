---
title: Adobe Workfront Planning API 기본 사항
description: Adobe Workfront Planning API의 목표는 HTTP를 통해 작동하는 REST 풀 아키텍처를 도입하여 Planning과의 통합 구축을 간소화하는 것입니다. 이 문서에서는 사용자가 REST 및 JSON 응답에 익숙하다고 가정하고 Planning API의 접근 방식에 대해 설명합니다.
author: Becky
feature: Workfront Planning
role: User, Admin
recommendations: noDisplay, noCatalog
exl-id: afb58d04-fa75-4eb7-9c19-2a8c1748fbc2
source-git-commit: 20e8d45264f9441d9576c7d4d5521e4f6053a7f3
workflow-type: tm+mt
source-wordcount: '973'
ht-degree: 1%

---


# Adobe Workfront Planning API 기본 사항

{{planning-important-intro}}

Adobe Workfront Planning API의 목표는 HTTP를 통해 작동하는 REST 풀 아키텍처를 도입하여 Planning과의 통합 구축을 간소화하는 것입니다. 이 문서에서는 사용자가 REST 및 JSON 응답에 익숙하다고 가정하고 Planning API의 접근 방식에 대해 설명합니다.

Workfront Planning 스키마에 익숙하면 통합 목적으로 Workfront Planning에서 데이터를 가져오는 데 사용할 수 있는 데이터베이스 관계를 이해하는 데 도움이 됩니다.

Workfront 사용자 정의 양식의 외부 조회 필드에서 계획 API를 호출할 수 있습니다.

외부 조회 필드에 대한 자세한 내용은 [사용자 정의 양식의 외부 조회 필드 예제](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/form-designer/design-a-form/external-lookup-examples.md)를 참조하십시오.

## Workfront Planning API URL

<!--For more details and examples of each operation, see the [Workfront Planning API developer documentation](https://developer.adobe.com/wf-planning/).-->

### 작업

개체는 고유한 URI에 HTTP 요청을 전송하여 조작됩니다. 수행할 작업은 HTTP 메서드에서 지정합니다.

표준 HTTP 메서드는 다음 작업에 해당합니다.

* **GET** - ID별로 개체를 검색하고 쿼리별로 모든 개체를 검색합니다.
* **POST** - 새 개체를 삽입합니다.
* **PUT** - 기존 개체를 편집합니다.
* **DELETE** - 개체를 삭제합니다.

각 작업에 대한 자세한 내용과 예제는 [Workfront Planning API 개발자 설명서](https://developer.adobe.com/wf-planning/)를 참조하십시오.

### 필드 유형 및 필드 유형과 함께 사용되는 검색 수정자

필드가 있는 수정자 및 필터를 사용하여 결과에 반환될 데이터를 제어할 수 있습니다.

<!--For examples, see the [Workfront Planning API developer documentation](https://developer.adobe.com/wf-planning/).-->

#### 검색 수정자 사용

Workfront Planning은 다음 검색 수정자를 지원합니다.

<table>
    <tr>
        <td><b>한정자</b></td>
        <td><b>예</b></td>
        <td><b>설명</b></td>
        <td><b>가능한 값</b></td>
    </tr>
    <tr>
        <td>$contains </td>
        <td><code>"fieldId": { "$contains": "product" } </code> </td>
        <td>필드 값에 필터가 포함된 레코드를 반환합니다.  </td>
        <td>"새 제품 출시"  </td>
    </tr>
    <tr>
        <td>$doesNotContain</td>
        <td><code>"fieldId": { "$doesNotContain": "product" } </code> </td>
        <td>필드 값에 필터가 포함되지 않은 레코드를 반환합니다.  </td>
        <td>"새 론치"  </td>
    </tr>
    <tr>
        <td>$is </td>
        <td><ul><li><code>"fieldId" : { "$is": "new product launch" } </code></li><li><code>"fieldId" : { "new product launch" } </code></li><ul> </td>
        <td>필드 값이 필터와 정확히 일치하는 레코드를 반환합니다.  </td>
        <td>"새 제품 출시"  </td>
    </tr>
    <tr>
        <td>$isNot </td>
        <td><code>"fieldId": { "$isNot": "product" } </code> </td>
        <td>필드 값이 필터와 정확히 일치하지 않는 레코드를 반환합니다.  </td>
        <td>"새 제품 출시"  </td>
    </tr>
    <tr>
        <td>$isEmpty </td>
        <td><ul><li><code>"fieldId": "$isEmpty" </code></li><li><code>"fieldId": { "$isEmpty": null } </code></li><ul> </td>
        <td>필드 값이 비어 있지 않은 레코드를 반환합니다.  </td>
        <td><ul><li>“” </li><li>null </li><ul>  </td>
    </tr>
    <tr>
        <td>$isNotEmpty </td>
        <td><ul><li><code>"fieldId": "$isNotEmpty"  </code></li><li><code>"fieldId": { "$isNotEmpty": null } </code></li><ul> </td>
        <td>필드 값이 비어 있지 않은 레코드를 반환합니다.  </td>
        <td>"새 제품 출시"  </td>
    </tr>
    <tr>
        <td>$greaterThan </td>
        <td><code>"fieldId": { "$greaterThan": 10 } </code> </td>
        <td>필드 값이 필터보다 큰 레코드를 반환합니다.  </td>
        <td><ul><li>20</li><li>25</li><ul> </td>
    </tr>
    <tr>
        <td>$greaterThanOrEqual </td>
        <td><code>"fieldId": { "$greaterThanOrEqual": 10 } </code> </td>
        <td>필드 값이 필터보다 크거나 같은 레코드를 반환합니다.  </td>
        <td><ul><li>10</li><li>20</li><li>25</li> </ul></td>
    </tr>
    <tr>
        <td>$lessThan </td>
        <td><code>"fieldId": { "$lessThan": 10 } </code> </td>
        <td>필드 값이 필터보다 작은 레코드를 반환합니다.  </td>
        <td><ul><li>5</li><li>9</li></td></ul> 
    </tr>
    <tr>
        <td>$lessThanOrEqual </td>
        <td><code>"fieldId": { "$lessThanOrEqual": 10 } </code> </td>
        <td>필드 값이 필터보다 작거나 같은 레코드 반환 </td>
        <td><ul><li>5</li><li>9</li><ul><li>10</li> </td>
    </tr>
    <tr>
        <td>$isAfter </td>
        <td><code>"fieldId": { "$isAfter": "2024-05-14T20:00:00.000Z" } </code> </td>
        <td>필드 값이 필터 뒤에 있는 레코드를 반환합니다.  </td>
        <td>"2024-05-15T20:00:00.000Z"  </td>
    </tr>
    <tr>
        <td>$isBefore </td>
        <td><code>"fieldId": { "$isBefore": "2024-05-14T20:00:00.000Z" } </code> </td>
        <td>필드 값이 필터 앞에 있는 레코드를 반환합니다. </td>
        <td>"2024-05-12T20:00:00.000Z" </td>
    </tr>
    <tr>
        <td>$isBetween </td>
        <td><code>"fieldId": { "$isBetween": ["2024-05-10T20:00:00.000Z", "2024-05-15T20:00:00.000Z"] } </code> </td>
        <td>필드 값이 필터 사이에 있는 레코드를 반환합니다.  </td>
        <td><ul><li>"2024-05-12T20:00:00.000Z" </li><li>"2024-05-14T20:00:00.000Z" </li><ul>  </td>
    </tr>
    <tr>
        <td>$isNotBetween </td>
        <td><code>"fieldId": { "$isNotBetween": ["2024-05-10T20:00:00.000Z", "2024-05-15T20:00:00.000Z"] } </code> </td>
        <td>필드 값이 필터 사이에 없는 레코드를 반환합니다.  </td>
        <td><ul><li>"2024-05-09T20:00:00.000Z"  </li><li>"2024-05-17T20:00:00.000Z"  </li><ul>  </td>
    </tr>
    <tr>
        <td>$isAnyOf </td>
        <td><code>"fieldId": { "$isAnyOf": ["active", "completed"] } </code> </td>
        <td>필드 값이 필터 중 하나인 레코드를 반환합니다.  </td>
        <td><ul><li>"active" </li><li>"완료됨" </li><ul> </td>
    </tr>
    <tr>
        <td>$isNoneOf </td>
        <td><code>"fieldId": { "$isNoneOf": ["active", "completed"] } </code> </td>
        <td>필드 값이 필터가 아닌 레코드를 반환합니다. </td>
        <td><ul><li>"완료됨"  </li><li>"수정됨"  </li><ul> </td>
    </tr>
    <tr>
        <td>$hasAnyOf </td>
        <td><code>"fieldId": { "$hasAnyOf": ["active", "completed"] } </code> </td>
        <td>필드 값에 필터가 있는 레코드를 반환합니다.  </td>
        <td><ul><li>["active", "fixed"]  </li><li>["수정됨", "완료됨", "완료됨"]  </li><ul> </td>
    </tr>
    <tr>
        <td>$hasAllOf </td>
        <td><code>"fieldId": { "$hasAllOf": ["active", "completed"] } </code> </td>
        <td>필드 값에 모든 필터가 있는 레코드를 반환합니다.  </td>
        <td><ul><li>["active", "completed"]   </li><li>["active", "completed", "finished"]   </li><ul> </td>
    </tr>
    <tr>
        <td>$hasNoneOf </td>
        <td><code>"fieldId": { "$hasNoneOf": ["active", "completed"] } </code> </td>
        <td>필드 값에 필터가 없는 레코드를 반환합니다. </td>
        <td>["수정됨", "완료됨"]  </td>
    </tr>
    <tr>
        <td>$isExactly </td>
        <td><code>"fieldId": { "$isExactly": ["active", "completed"] } </code> </td>
        <td>필드 값이 정확히 필터인 레코드를 반환합니다.  </td>
        <td>["active", "completed"]  </td>
    </tr>
</table>

#### 필드 유형

다음은 지원되는 필드 유형 목록과 각 필드 유형에 사용할 수 있는 검색 수정자 목록입니다

| 필드 유형 | 지원되는 검색 수정자 |
|---|---|
| 텍스트 | $contains, $doesNotContain, $is, $isNot, $isEmpty, $isNotEmpty |
| 긴 텍스트 | $contains, $doesNotContain, $is, $isNot, $isEmpty, $isNotEmpty |
| 숫자 | $is, $isNot, $greaterThan, $greaterThanOrEqual, $lessThan, $lessThanOrEqual, $isEmpty, $isNotEmpty |
| 백분율 | $is, $isNot, $greaterThan, $greaterThanOrEqual, $lessThan, $lessThanOrEqual, $isEmpty, $isNotEmpty |
| 통화 | $is, $isNot, $greaterThan, $greaterThanOrEqual, $lessThan, $lessThanOrEqual, $isEmpty, $isNotEmpty |
| 일자 | $is, $isNot, $isAfter, $isBefore, $isBetween, $isNotBetween, $isNotEmpty, $isNotEmpty |
| 단일 선택 | $is, $isNot, $isAnyOf, $isNoneOf, $isEmpty, $isNotEmpty |
| 다중 선택 | $hasAnyOf, $hasAllOf, $isExactly, $hasNoneOf, $isEmpty, $isNotEmpty |
| 부울 | $is |
| 사용자 | $hasAnyOf, $hasAllOf, $isExactly, $hasNoneOf, $isEmpty, $isNotEmpty |
| 공식 | $contains, $doesNotContain, $is, $isNot, $isEmpty, $isNotEmpty |
| url | $contains, $doesNotContain, $is, $isNot, $isEmpty, $isNotEmpty |
| 작성자 | $is, $isNot, $isAnyOf, $isNoneOf |
| 생성 시간 | $is, $isNot, $isAfter, $isBefore, $isBetween, $isNotBetween |
| 업데이트한 사람 | $is, $isNot, $isAnyOf, $isNoneOf, $isEmpty, $isNotEmpty |
| 업데이트 시간 | $is, $isNot, $isAfter, $isBefore, $isBetween, $isNotBetween, $isNotEmpty, $isNotEmpty |
| 참조 | $hasAnyOf, $hasAllOf, $isExactly, $hasNoneOf, $isEmpty, $isNotEmpty |
| 조회 | 연결된 필드에 따라 다릅니다. |

### &quot;And&quot; 및 &quot;Or&quot; 문 사용

API 호출에서는 $and&quot; 및 &quot;$or&quot; 문으로 결합된 여러 기준을 기반으로 하는 필터를 가질 수 있습니다

```
{
  "recordTypeId": "recordTypeId",
  "offset": "integer",
  "limit": "integer",
  "filters": [
    {
      "$or": [
        {
          "launch_date": {
            "$isBetween": [
              "2024-03-31T20:00:00.000Z",
              "2024-04-01T20:00:00.000Z"
            ]
          }
        },
        {
          "$and": [
            {
              "launch_date": {
                "$isBetween": [
                  "2024-03-31T20:00:00.000Z",
                  "2024-04-01T20:00:00.000Z"
                ]
              }
            },
            {
              "status": "active"
            }
          ]
        },
        {
          "$and": [
            {
              "launch_date": {
                "$isBetween": [
                  "2024-04-15T00:00:00.000Z",
                  "2024-04-16T00:00:00.000Z"
                ]
              }
            },
            {
              "status": "planned"
            }
          ]
        }
      ]
    }
  ]
}
```

### 필드 요청 매개 변수 사용

필드 요청 매개 변수를 사용하여 반환해야 하는 특정 필드의 쉼표로 구분된 목록을 지정할 수 있습니다. 이 필드 이름은 대소문자를 구분합니다.

예: 요청

`/v1/records/search?attributes=data,createdBy`

```
{
    "records": [
        {
            "id": "Rc6527ecb35df57c441d92ba00",
            "createdBy": "61a9cc0500002f9fdaa7a6f824f557e1",
            "createdAt": null,
            "updatedBy": null,
            "updatedAt": null,
            "customerId": null,
            "imsOrgId": null,
            "recordTypeId": null,
            "data": {
                "F666c0b58b6fee61a2ea6ea81": [
                    {
                        "externalId": null,
                        "id": "Rc665728ff95730b58bc757b13",
                        "value": null
                    },
....
```

다음과 유사한 응답을 반환합니다.


```
{ 
    "priority": 2, 
    "name": "first task", 
    "ID": "4c7c08fa0000002ff924e298ee148df4", 
    "plannedStartDate": "2010-08-30T09:00:00:000-0600" 
} 
```

### API에서 쿼리 결과 정렬

다음 내용을 API 호출에 추가하면 필드를 기준으로 결과를 정렬할 수 있습니다.


`/v1/records/search`

요청 본문:

```
{
    "recordTypeId": "Rt6527ecb25df57c441d92b9fa",
    "filters": [],
    "sorting": [
        {
            "fieldId": "F6527ecb25df57c441d92b9fc",
            "direction": "asc"
        },
        {
            "fieldId": "F658afcbd4a0273c67c346fd5",
            "direction": "desc"
        }
    ],
    "limit": 500,
    "offset": 0,
    "rowOrderViewId": "V6527ecb75df57c441d92ba03",
    "groupingFieldIds": []
}
```

### 쿼리 제한 및 페이지 매김된 응답

기본적으로 Planning API 요청은 목록의 시작 부분부터 500개의 결과를 반환합니다. 결과 수에 대한 기본 제한을 무시하려면 요청에 `limit` 매개 변수를 사용하고 다른 수(최대 2000개 결과)로 설정할 수 있습니다.

요청에 `offset` 매개 변수를 추가하여 대용량 데이터 세트에 대해 페이지 번호를 매긴 응답을 사용하는 것이 좋습니다. 페이지 매김된 응답을 사용하면 반환되어야 하는 첫 번째 결과의 위치를 지정할 수 있습니다.

예를 들어 결과 2001-4000을 반환하려는 경우 다음 요청을 사용할 수 있습니다. 이 예에서는 2001번째 결과부터 활성 상태인 2000개의 레코드를 반환합니다.

`POST /v1/records/search `



요청 본문:

```
{ 
    "recordTypeId": "recordTypeId", 
    "offset": "2001", 
    "limit": "2000", 
    "filters": [ 
        { "status": "active" } 
    ] 
} 
```

결과에 페이지가 올바르게 매겨졌는지 확인하려면 정렬 매개 변수를 사용하십시오. 이렇게 하면 결과를 같은 순서로 반환할 수 있으므로 페이지 매김이 반복되거나 결과를 건너뛰지 않습니다.

정렬에 대한 자세한 내용은 이 문서에서 [API에서 쿼리 결과 정렬](#sorting-query-results-in-the-api)을(를) 참조하십시오.
