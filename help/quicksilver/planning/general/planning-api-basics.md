---
title: Adobe Workfront Planning API 기본 사항
description: Adobe Workfront Planning API의 목표는 HTTP를 통해 작동하는 REST 풀 아키텍처를 도입하여 Planning과의 통합 구축을 간소화하는 것입니다. 이 문서에서는 사용자가 REST 및 JSON 응답에 익숙하다고 가정하고 Planning API의 접근 방식에 대해 설명합니다.
author: Becky
feature: Workfront Planning
role: User, Admin
recommendations: noDisplay, noCatalog
exl-id: afb58d04-fa75-4eb7-9c19-2a8c1748fbc2
source-git-commit: f11daa69f72c32418298ac75f81b0fb64835d99b
workflow-type: tm+mt
source-wordcount: '1079'
ht-degree: 2%

---


# Adobe Workfront Planning API 기본 사항

{{planning-important-intro}}

<!--
Lilit asked me to hide everything in this current article and replace it with her version of it. I kept just the Field type and search modifier section. The rest of the article is a re-write of the original from Lilit. 

She also said we need to reword how we organize the version features, after we get more versions released but for now, she calls out what's different in V1 than the current (V2) with almost every feature. 
-->

<!--
To comment out when we release V2 - everything else under this gets hidden after V2 release: 

# Adobe Workfront Planning API Basics

The goal of the Adobe Workfront Planning API is to simplify building integrations with Planning by introducing a RESTful architecture that operates over HTTP. This document assumes you are familiar with REST and JSON responses.

For complete endpoint reference, request/ response schemas, and version-specific details, see the [Workfront Planning API developer documentation](https://developer.adobe.com/wf-planning).

## Authentication

The Workfront Planning API uses OAuth 2.0 for authentication. Credentials are set up via the Adobe Developer Console. 

We support the following two flows depending on your integration type:

* **Server-to-server authentication (JWT)**: For automated integrations and backend services with no user interaction. Uses the OAuth Server-to-Server credential (client credentials grant — your application authenticates directly using its client ID and secret to obtain an access token, with no user login or consent step). 

    For information, see [Server to Server authentication](https://developer.adobe.com/developer-console/docs/guides/authentication/ServerToServerAuthentication/).

* **User authentication (Authorization Code flow)**: for integrations acting on behalf of a specific user. Uses the OAuth Web App or Single Page App credential (authorization code grant — the user logs in and consents, after which your application receives an authorization code it exchanges for an access token). 

    For information, see [User Authentication](https://developer.adobe.com/developer-console/docs/guides/authentication/UserAuthentication/).

To get started, create a project in the Adobe Developer Console and add the Workfront Planning API to obtain your credentials. 

To set up credentials, create an OAuth2 application in Workfront. 

For information, see [Create OAuth2 applications for Workfront integrations](/help/quicksilver/administration-and-setup/configure-integrations/create-oauth-application.md). 

>[!NOTE]
>
>The `/login` endpoint and API key authentication are not supported for Workfront Planning. Do not use `sessionID` or `apiKey` parameters.


## API versioning

The Planning API is versioned via the URL path. 

The following are current supported versions: 

| Version   | Release date   |
|-----------|----------------|
| Version 1 | July 2024 |
| Version 2 | May 2026   |

(*****************add deprecation date column above, when we have one*****************)


For more information about the current supported versions, see the article [Workfront Planning API developer documentation](https://developer.adobe.com/wf-planning).

We recommend explicitly targeting a version in all integrations:

```
https://{customer-domain}/maestro/api/v2/...

```

When a new major version is released, the previous version will continue to be available until a deprecation date is communicated.

Follow the Workfront release notes to stay informed of API changes.


## URL structure and operations

Objects are manipulated by sending an HTTP request to their unique URI. The operation is specified by the HTTP method.

| Method   | Operation                                                            |
|----------|----------------------------------------------------------------------|
| GET      | Retrieve a single object by ID, or search/list objects               |
| POST     | Create a new object                                                  |
| PUT      | Replace an existing object (full update)                             |
| PATCH    | Partially update an existing object (only provided fields are modified) |
| DELETE   | Delete an object                                                     |

>[!NOTE]
>
>**Version1 note:** `PATCH` is not supported in Version 1. Use `PUT` for all updates.


For full endpoint paths and request/response examples, see the **API reference** at [developer.adobe.com/wf-planning](https://developer.adobe.com/wf-planning).

## HTTP status codes

The Planning API returns standard HTTP status codes:

| Code                   | Meaning                                         |
|------------------------|-------------------------------------------------|
| 200 OK                 | Successful GET, PUT, or PATCH                   |
| 201 Created            | Successful POST (resource created)              |
| 204 No Content         | Successful DELETE                               |
| 207 Multi-Status          | Bulk operation completed with mixed results, where some items succeeded and some failed. Check individual item responses for details.                              |
| 400 Bad Request        | Invalid request — see error response for details |
| 401 Unauthorized       | Missing or invalid authentication token         |
| 403 Forbidden          | Authenticated but insufficient permissions      |
| 404 Not Found          | Resource does not exist                         |
| 409 Conflict           | Write conflict, the resource was modified by another request. Retry with the latest version.                          |
| 429 Too Many Requests  | Rate limit exceeded                             |

>[!NOTE]
>
>**Version 1 note:** Version 1 returns `200 OK` for all successful operations, including POST and DELETE.


## Error handling

The Planning API returns errors in a consistent format. Each error response includes a human-readable message, a machine-readable error code, and a request ID for support escalation.

Example error response:

```
json
{
  "title": "Validation failed",
  "status": 400,
  "detail": "Request validation failed. See 'errors' for details.",
  "errorCode": "VALIDATION_FAILED",
  "requestId": "req-123",
  "errors": [
    { "field": "name", "message": "must not be blank" }
  ]
}

```

Use `errorCode` (not `status`) to drive programmatic error handling. It provides the most specific classification of the failure.

>[!NOTE]
>
>**Version 1 note:** Version 1 error responses use a numeric `type` field (e.g. `40001`) instead of a string `errorCode`, and wrap detail in a `report` object rather than a top-level `detail` field.

## Filtering records

Use the `filter` parameter in record search requests to return only records matching specific criteria. For POST requests, `filter` is a JSON property in the request body. For GET requests, `filter` is a query parameter containing a JSON-encoded filter group. Filters use a typed composite structure with explicit logical operators.  

```
json
{
  "filter": {
    "operator": "AND",
    "conditions": [
      { "fieldId": "<fieldId>", "condition": "IS", "value": "Active" },
      { "fieldId": "<fieldId>", "condition": "CONTAINS", "value": "marketing" }
    ]
  }
}

```

Filters can be nested using `AND` / `OR` operators to build compound conditions:

```
json
{
  "filter": {
    "operator": "OR",
    "conditions": [
      {
        "operator": "AND",
        "conditions": [
          { "fieldId": "<fieldId>", "condition": "BETWEEN", "value": ["2024-03-31T20:00:00.000Z", "2024-04-01T20:00:00.000Z"] },
          { "fieldId": "<fieldId>", "condition": "IS", "value": "active" }
        ]
      },
      {
        "operator": "AND",
        "conditions": [
          { "fieldId": "<fieldId>", "condition": "IS_BETWEEN", "value": ["2024-04-15T00:00:00.000Z", "2024-04-16T00:00:00.000Z"] },
          { "fieldId": "<fieldId>", "condition": "IS", "value": "planned" }
        ]
      }
    ]
  }
}

```

>[!NOTE]
>
>**Version 1 note:** Version 1 uses Mongo-style untyped operators in a `filters` object. Operators are prefixed with `$` (e.g. `$and`, `$or`, `$is`, `$contains`, `$isBetween`). Pagination parameters (`offset`, `limit`) and `recordTypeId` are passed in the request body rather than as URL path and query parameters.


## Field types and search modifiers

You can use modifiers and filters with fields to control what data will be returned in results. 

For examples, see the [Workfront Planning API developer documentation](https://developer.adobe.com/wf-planning/).

### Using search modifiers 

Workfront Planning supports the following search modifiers: 


<table style="table-layout:auto"> 
  <colgroup><col class="c1"><col class="c2"><col class="c3"><col class="c4"></colgroup>
  <thead>
    <tr>
      <th>Modifier</th>
      <th>Example</th>
      <th>Description</th>
      <th>Possible values</th>
    </tr>
  </thead>
  <tbody>
    <tr><td class="modifier">CONTAINS</td><td class="example">{"fieldId":"&lt;id&gt;","condition":"CONTAINS","value":"product"}</td><td>Returns records whose field value contains the filter</td><td class="possible">"New Product Launch"</td></tr>
    <tr><td class="modifier">DOES_NOT_CONTAIN</td><td class="example">{"fieldId":"&lt;id&gt;","condition":"DOES_NOT_CONTAIN","value":"product"}</td><td>Returns records where the field value does not contain the filter</td><td class="possible">"New Launch"</td></tr>
    <tr><td class="modifier">IS</td><td class="example">{"fieldId":"&lt;id&gt;","condition":"IS","value":"new product launch"}</td><td>Returns records whose field value exactly matches the filter</td><td class="possible">"New Product Launch"</td></tr>
    <tr><td class="modifier">IS_NOT</td><td class="example">{"fieldId":"&lt;id&gt;","condition":"IS_NOT","value":"product"}</td><td>Returns records whose field value does not exactly match the filter</td><td class="possible">"New Product Launch"</td></tr>
    <tr><td class="modifier">IS_EMPTY</td><td class="example">{"fieldId":"&lt;id&gt;","condition":"IS_EMPTY"}</td><td>Returns records whose field value is empty</td><td class="possible">"" or null</td></tr>
    <tr><td class="modifier">IS_NOT_EMPTY</td><td class="example">{"fieldId":"&lt;id&gt;","condition":"IS_NOT_EMPTY"}</td><td>Returns records whose field value is not empty</td><td class="possible">"New Product Launch"</td></tr>
    <tr><td class="modifier">GREATER_THAN</td><td class="example">{"fieldId":"&lt;id&gt;","condition":"GREATER_THAN","value":"10"}</td><td>Returns records whose field value is greater than the filter</td><td class="possible">"11"</td></tr>
    <tr><td class="modifier">GREATER_THAN_OR_EQUAL</td><td class="example">{"fieldId":"&lt;id&gt;","condition":"GREATER_THAN_OR_EQUAL","value":"10"}</td><td>Returns records whose field value is greater than or equal to the filter</td><td class="possible">"10", "11"</td></tr>
    <tr><td class="modifier">LESS_THAN</td><td class="example">{"fieldId":"&lt;id&gt;","condition":"LESS_THAN","value":"10"}</td><td>Returns records whose field value is less than the filter</td><td class="possible">"9"</td></tr>
    <tr><td class="modifier">LESS_THAN_OR_EQUAL</td><td class="example">{"fieldId":"&lt;id&gt;","condition":"LESS_THAN_OR_EQUAL","value":"10"}</td><td>Returns records whose field value is less than or equal to the filter</td><td class="possible">"9", "10"</td></tr>
    <tr><td class="modifier">IS_BETWEEN</td><td class="example">{"fieldId":"&lt;id&gt;","condition":"IS_BETWEEN","value":["2024-01-01","2024-12-31"]}</td><td>Returns records whose field value falls between the two filter values</td><td class="possible">["2024-03-01","2024-06-30"]</td></tr>
    <tr><td class="modifier">IS_NOT_BETWEEN</td><td class="example">{"fieldId":"&lt;id&gt;","condition":"IS_NOT_BETWEEN","value":["2024-01-01","2024-12-31"]}</td><td>Returns records whose field value does not fall between the two filter values</td><td class="possible">["2023-01-01","2025-06-30"]</td></tr>
    <tr><td class="modifier">IS_AFTER</td><td class="example">{"fieldId":"&lt;id&gt;","condition":"IS_AFTER","value":"2024-01-01"}</td><td>Returns records whose date field value is after the filter</td><td class="possible">"2024-06-01"</td></tr>
    <tr><td class="modifier">IS_BEFORE</td><td class="example">{"fieldId":"&lt;id&gt;","condition":"IS_BEFORE","value":"2024-12-31"}</td><td>Returns records whose date field value is before the filter</td><td class="possible">"2024-06-01"</td></tr>
    <tr><td class="modifier">IS_ANY_OF</td><td class="example">{"fieldId":"&lt;id&gt;","condition":"IS_ANY_OF","value":["Active","Planned"]}</td><td>Returns records whose field value matches any value in the filter list</td><td class="possible">["Active","Planned","Complete"]</td></tr>
    <tr><td class="modifier">IS_NONE_OF</td><td class="example">{"fieldId":"&lt;id&gt;","condition":"IS_NONE_OF","value":["Active","Planned"]}</td><td>Returns records whose field value matches none of the values in the filter list</td><td class="possible">["Active","Planned"]</td></tr>
    <tr><td class="modifier">HAS_ANY_OF</td><td class="example">{"fieldId":"&lt;id&gt;","condition":"HAS_ANY_OF","value":["Tag1","Tag2"]}</td><td>Returns records whose multi-value field contains any of the filter values</td><td class="possible">["Tag1","Tag2"]</td></tr>
    <tr><td class="modifier">HAS_ALL_OF</td><td class="example">{"fieldId":"&lt;id&gt;","condition":"HAS_ALL_OF","value":["Tag1","Tag2"]}</td><td>Returns records whose multi-value field contains all of the filter values</td><td class="possible">["Tag1","Tag2"]</td></tr>
    <tr><td class="modifier">IS_EXACTLY</td><td class="example">{"fieldId":"&lt;id&gt;","condition":"IS_EXACTLY","value":["Tag1"]}</td><td>Returns records whose multi-value field contains exactly the filter values and no others</td><td class="possible">["Tag1"]</td></tr>
    <tr><td class="modifier">HAS_NONE_OF</td><td class="example">{"fieldId":"&lt;id&gt;","condition":"HAS_NONE_OF","value":["Tag1"]}</td><td>Returns records whose multi-value field contains none of the filter values</td><td class="possible">["Tag1"]</td></tr>
  </tbody>
</table>
 
### Field types 

Below is the list of supported field types and what search modifiers can be used with each of those field types  

| Field Type | Supported search modifiers |
|---|---|
| text |$contains, $doesNotContain, $is, $isNot, $isEmpty, $isNotEmpty |
| long-text | $contains, $doesNotContain, $is, $isNot, $isEmpty, $isNotEmpty |
| number | $is, $isNot, $greaterThan, $greaterThanOrEqual, $lessThan, $lessThanOrEqual, $isEmpty, $isNotEmpty |
| percentage | $is, $isNot, $greaterThan, $greaterThanOrEqual, $lessThan, $lessThanOrEqual, $isEmpty, $isNotEmpty |
| currency | $is, $isNot, $greaterThan, $greaterThanOrEqual, $lessThan, $lessThanOrEqual, $isEmpty, $isNotEmpty |
| date | $is, $isNot, $isAfter, $isBefore, $isBetween, $isNotBetween, $isEmpty, $isNotEmpty |
| single-select | $is, $isNot, $isAnyOf, $isNoneOf, $isEmpty, $isNotEmpty |
| multi-select | $hasAnyOf, $hasAllOf, $isExactly, $hasNoneOf, $isEmpty, $isNotEmpty |
| boolean | $is |
| user | $hasAnyOf, $hasAllOf, $isExactly, $hasNoneOf, $isEmpty, $isNotEmpty |
| formula | $contains, $doesNotContain, $is, $isNot, $isEmpty, $isNotEmpty |
| url | $contains, $doesNotContain, $is, $isNot, $isEmpty, $isNotEmpty |
| created-by | $is, $isNot, $isAnyOf, $isNoneOf |
| created-at | $is, $isNot, $isAfter, $isBefore, $isBetween, $isNotBetween |
| updated-by | $is, $isNot, $isAnyOf, $isNoneOf, $isEmpty, $isNotEmpty |
| updated-at | $is, $isNot, $isAfter, $isBefore, $isBetween, $isNotBetween, $isEmpty, $isNotEmpty |
| reference | $hasAnyOf, $hasAllOf, $isExactly, $hasNoneOf, $isEmpty, $isNotEmpty |
| lookup | Depends on the linked field |

## Supported filter conditions by field type

| Field Type                  | Supported Conditions                                                                                         |
|-----------------------------|--------------------------------------------------------------------------------------------------------------|
| text, long-text             | CONTAINS, DOES_NOT_CONTAIN, IS, IS_NOT, IS_EMPTY, IS_NOT_EMPTY                                              |
| number, percentage, currency| IS, IS_NOT, GREATER_THAN, GREATER_THAN_OR_EQUAL, LESS_THAN, LESS_THAN_OR_EQUAL, IS_EMPTY, IS_NOT_EMPTY      |
| date                        | IS, IS_NOT, IS_AFTER, IS_BEFORE, IS_BETWEEN, IS_NOT_BETWEEN, IS_EMPTY, IS_NOT_EMPTY                         |
| single-select               | IS, IS_NOT, IS_ANY_OF, IS_NONE_OF, IS_EMPTY, IS_NOT_EMPTY                                                   |
| multi-select, user          | HAS_ANY_OF, HAS_ALL_OF, IS_EXACTLY, HAS_NONE_OF, IS_EMPTY, IS_NOT_EMPTY                                    |
| boolean                     | IS                                                                              |
| formula               | CONTAINS, DOES_NOT_CONTAIN, IS, IS_NOT, IS_EMPTY, IS_NOT_EMPTY                                               |
| created-by       | IS, IS_NOT, IS_ANY_OF, IS_NONE_OF                                                                             |
| updated-by        | IS, IS_NOT, IS_ANY_OF, IS_NONE_OF, IS_EMPTY, IS_NOT_EMPTY                                                                              |
| created-at      | IS, IS_NOT, IS_AFTER, IS_BEFORE, IS_BETWEEN, IS_NOT_BETWEEN                                                  |
| updated-at      | IS, IS_NOT, IS_AFTER, IS_BEFORE, IS_BETWEEN, IS_NOT_BETWEEN, IS_EMPTY, IS_NOT_EMPTY                                                   |
| reference                   | HAS_ANY_OF, HAS_ALL_OF, IS_EXACTLY, HAS_NONE_OF, IS_EMPTY, IS_NOT_EMPTY                                    |
| lookup                      | Depends on the linked field type                                                                             |

>[!NOTE]
>
>**Version 1 note:** Version 1 uses `$`-prefixed operator names (e.g. `$contains`, `$greaterThan`, `$isAnyOf`, `$hasAllOf`). The set of supported conditions per field type is the same.

## Filtering by People fields 

People field filters (`user`, `created-by`, `updated-by`, `approved-by`) accept both Adobe IMS user IDs and Workfront user IDs. A plain string value is interpreted as an Adobe IMS user ID. 

To set the identifier type to check the Workfront user ID, you need to explicitly pass `id` and `idType` parameters. Supported values for `idType` are "`WF`" for Workfront user IDs, and "`IMS`" for Adobe IMS user IDs. 

```
{ 
  "filter": { 
   "operator": "AND", 
    "conditions": [ 
      { 
        "fieldId": "<userFieldId>", 
        "condition": "HAS_ANY_OF", 
        "value": [ 
          { "id": "63e3b13000078c1795146248182d15dc", "idType": "WF" } 
        ] 
      } 
    ] 
  } 
} 

```

>[!NOTE]
>
> Version 1 note: V1 only supports filtering by users' IMS ID.  

## Filtering External Reference Fields by External ID 

External reference fields link records to objects in other Adobe systems (such as Workfront projects or AEM Assets). Internally, Planning assigns Planning record IDs to these objects. To filter such fields directly by their original object ID, add `"matchExternalId": true` to a filter condition. 

This flag is only valid for reference fields where `referenceOptions.isExternal` is `true`; it is ignored for non-external reference fields. If a single string value cannot be resolved, the request fails with `400 Bad Request`. If a list value is supplied, unresolved entries pass through unchanged and simply do not match. 

```
{ 
  "filter": { 
    "operator": "AND", 
    "conditions": [ 
      { 
        "fieldId": "<externalReferenceFieldId>", 
        "condition": "IS_ANY_OF", 
        "value": [ 
          "5f6a4f6e00000123456789abcdef0123", 
          "/content/dam/wknd/en/adventures/bali-surf-camp" 
        ], 
        "matchExternalId": true 
      } 
    ] 
  } 
} 

```
 
>[!NOTE]
>
>Version 1 note: V1 does not support filtering by external object IDs. 

## External Connection Fields 

Planning record types can host external reference fields that link records to objects in other Adobe systems instead of other Planning record types. 

To create an external reference field via the API, set `referenceOptions.recordTypeId` on a new `REFERENCE` field to the ID of the desired external record type. The server automatically derives `referenceOptions.isExternal=true` and the connection metadata (`connectionName, objectName`) from the target record type. 

Supported external object types include Workfront objects (projects, tasks, programs, portfolios, companies, groups, teams, users) and AEM Assets (assets, content fragments). 

>[!NOTE]
>
>Version 1 note: V1 does not support creating external connection fields. 


## Sorting

Sort results by any field by including a `sort` array in your request:

```
json
{
  "sort": [
    { "fieldId": "F6527ecb25df57c441d92b9fc", "direction": "asc" },
    { "fieldId": "F658afcbd4a0273c67c346fd5", "direction": "desc" }
  ]
}

```

Multiple sort fields are evaluated in order. Always apply a sort when paginating to ensure consistent ordering across pages.

To group results, include a group array alongside sort: 

```
{ 
  "sort": [{ "fieldId": "F001", "direction": "asc" }], 
  "group": [{ "fieldId": "F002", "direction": "asc" }] 
} 

```

>[!NOTE]
>
>Version 1 note: V1 uses `sorting` (not `sort`), `groupingFieldIds` (array of field IDs, not `group` objects), and the now-deprecated `rowOrderViewId` to apply an existing view's row order. None of these V1 parameters are supported in Version 2. 


---

## Field projection

To limit which fields are returned in a response, use the `fieldIds` or `fieldAliases` query parameters with a comma-separated list. This reduces response payload size and is recommended for high-volume or latency-sensitive integrations.

>[!NOTE]
>
>**Version 1 note:** Version 1 uses `?attributes=` for projection (e.g. `?attributes=data,createdBy`) rather than `?fieldIds=` or `?fieldAliases=`.

## Pagination

The Planning API supports paginated responses to manage large datasets.

* **Cursor-based pagination** is used for workspaces, record types, fields, and views. Pass a `cursor` value from the previous response to retrieve the next page. Cursor-based responses include a hasMore flag to indicate if there are more pages or not.
* **Page-based pagination** is used for record search. Use `page` and `size` as query parameters. Always apply a sort when paginating to ensure consistent ordering across pages. Note that pagination is zero-based, so in order to retrieve the results of the second page, use "`page=1`" as the parameter.   

For example, use the following request to retrieve the second page of 500 records from a record search: 

```
POST /v2/record-types/{recordTypeId}/records/search?page=1&size=500 
{ 
  "sort": [{ "fieldId": "F6527ecb25df57c441d92b9fc", "direction": "asc" }], 
  "filter": { "operator": "AND", "conditions": [ 
    { "fieldId": "<fieldId>", "condition": "IS", "value": "active" } 
  ] } 
} 

```

All paginated responses include a structured envelope indicating whether more results are available. Always apply a sort when paginating to ensure consistent ordering across pages.

>[!NOTE]
>
> **Version 1 note:** V1 uses `offset` and `limit` passed in the request body (default 500, max 2,000). To retrieve records 2001–4000, set "`offset`": "`2000`", "`limit`": "`2000`" in the request body. The response returns a flat records array with a `totalCount` field.

## Bulk operations

The Planning API supports bulk create, update, patch, and delete of records in a single request. Refer to the **API reference** at [developer.adobe.com/wf-planning](https://developer.adobe.com/wf-planning) for endpoint paths, request formats, and per-operation record limits.

>[!NOTE]
>
>**Version 1 note:** Bulk operations are not available in Version 1.


## Permissions

Permissions to entities are managed through a dedicated Permissions API, separate from the resource endpoints themselves. This allows you to read current permissions, manage the sharing list, and handle access requests independently of data operations. For more information, see the "API references" section in the article [Workfront Planning API](https://developer.adobe.com/wf-planning).

>[!NOTE]
>
>**Version 1 note:** Version 1 does not expose a public Permissions API. Permission level is embedded directly in resource response DTOs.

## Using the Planning API with Workfront custom forms

You can call the Planning API from an External lookup field in a Workfront custom form to surface Planning data directly within Workfront objects. For more information, see [Examples of the External lookup field in a custom form](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/form-designer/design-a-form/external-lookup-examples.md).

## Related resources

For more API-related documentation, also see the following articles:

* [Workfront Planning API](https://developer.adobe.com/wf-planning) developer documentation and reference
* [Get started with Adobe Workfront Planning](/help/quicksilver/planning/general/planning-overview.md)
* [Adobe Workfront Planning access overview](/help/quicksilver/planning/access/access-overview.md)
* [Create OAuth2 applications for Workfront integrations](/help/quicksilver/administration-and-setup/configure-integrations/create-oauth-application.md)

-->

Adobe Workfront Planning API의 목표는 HTTP를 통해 작동하는 REST 풀 아키텍처를 도입하여 Planning과의 통합 구축을 간소화하는 것입니다. 이 문서에서는 사용자가 REST 및 JSON 응답에 익숙하다고 가정하고 Planning API의 접근 방식에 대해 설명합니다.

Workfront Planning 스키마에 익숙하면 통합 목적으로 Workfront Planning에서 데이터를 가져오는 데 사용할 수 있는 데이터베이스 관계를 이해하는 데 도움이 됩니다.

Workfront 사용자 정의 양식의 외부 조회 필드에서 계획 API를 호출할 수 있습니다.

외부 조회 필드에 대한 자세한 내용은 [사용자 정의 양식의 외부 조회 필드 예제](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/form-designer/design-a-form/external-lookup-examples.md)를 참조하십시오.

>[!NOTE]
>
>Planning API를 사용하는 경우 모든 사용자 관련 정보는 Workfront 사용자 ID가 아닌 Adobe Identity Management System(IMS) 사용자 ID를 사용하여 반환됩니다.
>
>자세한 내용은 [Adobe Admin Console에서 사용자 관리](/help/quicksilver/administration-and-setup/add-users/create-and-manage-users/admin-console.md)를 참조하십시오.

## Workfront Planning API 버전

* 버전 1 - 2024년 7월에 릴리스됨

  자세한 내용은 이 문서의 [Workfront Planning API 버전 1](#workfront-planning-api-version-1) 섹션을 참조하십시오.
  <!--
    Maybe retitle the "Workfront Planning API" section below to "Workfront Planning API Version 1" when Version 2 releases
    -->

<!--
* Version 2 - released in May 2026

    For more information, see the section [Workfront Planning API Version 2](#workfront-planning-api-version-2) in this article.
-->

## Workfront Planning API 버전 1

Workfront Planning API 버전 1은 2024년 7월에 릴리스되었습니다.

다음 섹션에서는 Workfront API 버전 1에서 사용할 수 있는 기능에 대해 설명합니다.

별도로 지정하지 않는 한 모든 향후 API 버전에는 동일한 기능이 포함됩니다.

<!--
Becky had put the title of this article as"Workfront Planning API URL", but she did not document what that URL is; asking dev and hiding it for now
-->

<!--
For more details and examples of each operation, see the [Workfront Planning API developer documentation](https://developer.adobe.com/wf-planning/).
-->

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
        <td>필드 값이 비어 있는 레코드를 반환합니다.  </td>
        <td><ul><li>"" </li><li>null </li><ul>  </td>
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
| 번호 | $is, $isNot, $greaterThan, $greaterThanOrEqual, $lessThan, $lessThanOrEqual, $isEmpty, $isNotEmpty |
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
..
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

`POST /v1/records/search`



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

<!--

Lilit did not want this organized like this - keeping this for reference: 

## Workfront Planning API Version 2

Version of the Workfront Planning API was released in May 2026. 

In addition to all the information contained in Version 1, the following enhancements were added in Version 2: 

* Search by the user's Workfront ID field instead of the user's IMS ID.

    This is applicable to custom People fields, as well as system fields such as Created By and Last Updated By fields.

* Ability to search by external connections (Workfront or AEM objects) via the API.

* Ability to link cross-workspace shared records through API. 

* Support all CRUD operations for workspaces, record types, fields, and views. 

* Enable permissions sharing for all sharable entities via API. 

    This includes workspaces, record types, and views. (***********and in the future also records and fields.*********)

* Support for uploading record thumbnail through API. 

-->