---
title: Adobe Workfront Planning API 기본 사항
description: Adobe Workfront Planning API의 목표는 HTTP를 통해 작동하는 REST 풀 아키텍처를 도입하여 Planning과의 통합 구축을 간소화하는 것입니다. 이 문서에서는 사용자가 REST 및 JSON 응답에 익숙하다고 가정하고 Planning API의 접근 방식에 대해 설명합니다.
author: Becky
feature: Workfront Planning
role: User, Admin
recommendations: noDisplay, noCatalog
exl-id: afb58d04-fa75-4eb7-9c19-2a8c1748fbc2
TQID: https://experienceleague.adobe.com/SGwYFV5aZJGwfUy7ejVTaOkn0v4Dt-HJLI5hDWKVhMo
product_v2: id: c4a86a5d-6562-4fc6-aa00-bfa25833aed9
feature_v2: id: d968a1bc-9a90-4926-a531-bcf272c32aadid: f48b5020-b9cd-4d99-bc6e-42c35e90c1f8
subfeature_v2: id: e147ce9d-7675-49bd-8a32-44f27d865560
role_v2: id: b69b2659-1057-424e-8fc5-ed9e016dc554id: c66ffd68-0f65-42bb-aa23-b4020f12e0bd
topic_v2: id: eddd9b14-83bd-4ff4-9072-54a4a484abb7
source-git-commit: e458b7274f0f80c8be395bdc8ad91eaf6cfd0876
workflow-type: tm+mt
source-wordcount: 2232
ht-degree: 2%

---

# Adobe Workfront Planning API 기본 사항

{{planning-important-intro}}

<!--

Lilit asked me to hide everything in this current article and replace it with her version of it. I kept just the Field type and search modifier section. The rest of the article is a re-write of the original from Lilit. 

She also said we need to reword how we organize the version features, after we get more versions released but for now, she calls out what's different in V1 than the current (V2) with almost every feature. 

-->

Adobe Workfront Planning API의 목표는 HTTP를 통해 작동하는 RESTful 아키텍처를 도입하여 Planning과의 통합 빌드를 간소화하는 것입니다. 이 문서에서는 사용자가 REST 및 JSON 응답에 익숙하다고 가정합니다.

전체 끝점 참조, 요청/응답 스키마 및 버전별 세부 정보는 [Workfront Planning API 개발자 설명서](https://developer.adobe.com/wf-planning)를 참조하십시오.

## 인증

Workfront Planning API는 인증에 OAuth 2.0을 사용합니다. 자격 증명은 Adobe Developer Console을 통해 설정됩니다.

통합 유형에 따라 다음 두 가지 흐름이 지원됩니다.

* **JWT(서버 간 인증)**: 사용자 상호 작용 없이 자동화된 통합 및 백엔드 서비스입니다. OAuth 서버 간 자격 증명(클라이언트 자격 증명 부여 — 사용자 로그인 또는 동의 단계 없이 애플리케이션이 클라이언트 ID 및 암호를 사용하여 액세스 토큰을 얻기 위해 직접 인증함)을 사용합니다.

  자세한 내용은 [서버 간 인증](https://developer.adobe.com/developer-console/docs/guides/authentication/ServerToServerAuthentication/)을 참조하십시오.

* **사용자 인증(인증 코드 흐름)**: 특정 사용자를 대신하여 동작하는 통합용. OAuth 웹 앱 또는 단일 페이지 앱 자격 증명(인증 코드 부여 — 사용자가 로그인하고 동의하면 애플리케이션이 액세스 토큰에 대해 교환하는 인증 코드를 받습니다)을 사용합니다.

  자세한 내용은 [사용자 인증](https://developer.adobe.com/developer-console/docs/guides/authentication/UserAuthentication/)을 참조하세요.

시작하려면 Adobe Developer Console에서 프로젝트를 만들고 Workfront Planning API를 추가하여 자격 증명을 획득합니다.

자격 증명을 설정하려면 Workfront에서 OAuth2 애플리케이션을 만드십시오.

자세한 내용은 [Workfront 통합을 위한 OAuth2 애플리케이션 만들기](/help/quicksilver/administration-and-setup/configure-integrations/create-oauth-application.md)를 참조하십시오.

>[!NOTE]
>
>`/login` 끝점 및 API 키 인증은 Workfront Planning에서 지원되지 않습니다. `sessionID` 또는 `apiKey` 매개 변수를 사용하지 마십시오.


## API 버전 관리

Planning API는 URL 경로를 통해 버전이 지정됩니다.

다음은 현재 지원되는 버전입니다.

<!--

(*****************add deprecation date column above, when we have one*****************)

-->

| 버전 | 릴리스 일자 |
|-----------|----------------|
| 버전 1 | 2024년 7월 |
| 버전 2 | 2026년 5월 |

>[!NOTE]
>
>Workfront Fusion용 Workfront Planning 커넥터가 API 버전 2로 업데이트되지 않았으며 추가 공지가 있을 때까지 버전 1을 계속 사용합니다.

현재 지원되는 버전에 대한 자세한 내용은 문서 [Workfront Planning API 개발자 설명서](https://developer.adobe.com/wf-planning)를 참조하십시오.

모든 통합에서 버전을 명시적으로 타깃팅하는 것이 좋습니다.

```
https://{customer-domain}/maestro/api/v2/...
```

새로운 주요 버전이 출시되면 사용 중단 날짜가 전달될 때까지 이전 버전을 계속 사용할 수 있습니다.

API 변경 사항을 계속 알려면 Workfront 릴리스 노트를 따르십시오.


## URL 구조 및 작업

개체는 고유한 URI에 HTTP 요청을 전송하여 조작됩니다. 작업은 HTTP 메서드에서 지정합니다.

| 메서드 | 작업 |
|----------|----------------------------------------------------------------------|
| GET | ID 또는 검색/목록 개체로 단일 개체 검색 |
| POST | 새 개체 만들기 |
| PUT | 기존 개체 바꾸기(전체 업데이트) |
| PATCH | 기존 개체 부분 업데이트(제공된 필드만 수정됨) |
| DELETE | 개체 삭제 |

>[!NOTE]
>
>**버전1 참고:** `PATCH`은(는) 버전 1에서 지원되지 않습니다. 모든 업데이트에 `PUT` 사용


전체 끝점 경로 및 요청/응답 예제는 [developer.adobe.com/wf-planning](https://developer.adobe.com/wf-planning)의 **API 참조**&#x200B;를 참조하십시오.

## HTTP 상태 코드

Planning API는 표준 HTTP 상태 코드를 반환합니다.

| 코드 | 의미 |
|------------------------|-------------------------------------------------|
| 200개 | 성공적인 GET, PUT 또는 PATCH |
| 201 생성됨 | POST 성공(리소스 생성됨) |
| 204 콘텐츠 없음 | 성공한 DELETE |
| 207 다중 상태 | 대량 작업이 완료되었으며 일부 항목은 성공하고 일부는 실패했습니다. 결과가 혼합되었습니다. 자세한 내용은 개별 항목 응답을 확인하십시오. |
| 400 잘못된 요청 | 잘못된 요청 — 자세한 내용은 오류 응답 을 참조하십시오. |
| 401 승인되지 않음 | 누락되었거나 잘못된 인증 토큰 |
| 403 금지 | 인증되었지만 권한이 충분하지 않음 |
| 404 찾을 수 없음 | 리소스가 존재하지 않음 |
| 충돌 | 쓰기 충돌이 발생했습니다. 다른 요청에 의해 리소스가 수정되었습니다. 최신 버전으로 다시 시도하십시오. |
| 429개의 요청이 너무 많음 | 요금 한도 초과됨 |

>[!NOTE]
>
>**버전 1 참고:** 버전 1은 POST 및 DELETE을 포함하여 성공한 모든 작업에 대해 `200 OK`을(를) 반환합니다.


## 오류 처리

Planning API는 일관된 형식으로 오류를 반환합니다. 각 오류 응답에는 사람이 읽을 수 있는 메시지, 기계가 읽을 수 있는 오류 코드 및 지원 에스컬레이션을 위한 요청 ID가 포함됩니다.

오류 응답 예:

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

프로그래밍 방식의 오류 처리를 수행하려면 `status`이(가) 아닌 `errorCode`을(를) 사용하십시오. 가장 구체적인 장애 분류 방법을 제공합니다.

>[!NOTE]
>
>**버전 1 참고:** 버전 1 오류 응답에서는 문자열 `errorCode` 대신 숫자 `type` 필드(예: `40001`)를 사용하고 최상위 `detail` 필드 대신 `report` 개체에 세부 정보를 래핑합니다.

## 레코드 필터링

특정 기준과 일치하는 레코드만 반환하려면 레코드 검색 요청에 `filter` 매개 변수를 사용하십시오. POST 요청의 경우 `filter`은(는) 요청 본문의 JSON 속성입니다. GET 요청의 경우 `filter`은(는) JSON으로 인코딩된 필터 그룹이 포함된 쿼리 매개 변수입니다. 필터는 명시적 논리 연산자가 있는 형식화된 복합 구조를 사용합니다.

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

필터를 `AND`/`OR` 연산자를 사용하여 중첩하여 복합 조건을 만들 수 있습니다.

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
>**버전 1 참고:** 버전 1은 `filters` 개체에서 Mongo 스타일의 형식화되지 않은 연산자를 사용합니다. 연산자 앞에는 `$`(예: `$and`, `$or`, `$is`, `$contains`, `$isBetween`)이 붙습니다. 페이지 매김 매개 변수(`offset`, `limit`) 및 `recordTypeId`이(가) URL 경로 및 쿼리 매개 변수가 아닌 요청 본문에 전달됩니다.


## 필드 유형 및 검색 수정자

필드가 있는 수정자 및 필터를 사용하여 결과에 반환될 데이터를 제어할 수 있습니다.

예를 들어 [Workfront Planning API 개발자 설명서](https://developer.adobe.com/wf-planning/)를 참조하십시오.

### 검색 수정자 사용

Workfront Planning은 다음 검색 수정자를 지원합니다.


<table style="table-layout:auto"> 
  <colgroup><col class="c1"><col class="c2"><col class="c3"><col class="c4"></colgroup>
  <thead>
    <tr>
      <th>한정자</th>
      <th>예</th>
      <th>설명</th>
      <th>가능한 값</th>
    </tr>
  </thead>
  <tbody>
    <tr><td class="modifier">포함</td><td class="example">{"fieldId":"&lt;id&gt;","condition":"CONTAINS","value":"product"}</td><td>필드 값에 필터가 포함된 레코드를 반환합니다.</td><td class="possible">"새 제품 출시"</td></tr>
    <tr><td class="modifier">DOES_NOT_CONTAIN</td><td class="example">{"fieldId":"&lt;id&gt;","condition":"DOES_NOT_CONTAIN","value":"product"}</td><td>필드 값에 필터가 포함되지 않은 레코드를 반환합니다.</td><td class="possible">"새 론치"</td></tr>
    <tr><td class="modifier">다음과 같음</td><td class="example">{"fieldId":"&lt;id&gt;","condition":"IS","value":"새 제품 출시"}</td><td>필드 값이 필터와 정확히 일치하는 레코드를 반환합니다.</td><td class="possible">"새 제품 출시"</td></tr>
    <tr><td class="modifier">IS_NOT</td><td class="example">{"fieldId":"&lt;id&gt;","condition":"IS_NOT","value":"product"}</td><td>필드 값이 필터와 정확히 일치하지 않는 레코드를 반환합니다.</td><td class="possible">"새 제품 출시"</td></tr>
    <tr><td class="modifier">IS_EMPTY</td><td class="example">{"fieldId":"&lt;id&gt;","condition":"IS_EMPTY"}</td><td>필드 값이 비어 있는 레코드를 반환합니다.</td><td class="possible">"" 또는 null</td></tr>
    <tr><td class="modifier">IS_NOT_EMPTY</td><td class="example">{"fieldId":"&lt;id&gt;","condition":"IS_NOT_EMPTY"}</td><td>필드 값이 비어 있지 않은 레코드를 반환합니다.</td><td class="possible">"새 제품 출시"</td></tr>
    <tr><td class="modifier">GREATER_THAN</td><td class="example">{"fieldId":"&lt;id&gt;","condition":"GREATER_THAN","value":"10"}</td><td>필드 값이 필터보다 큰 레코드를 반환합니다.</td><td class="possible">"11"</td></tr>
    <tr><td class="modifier">GREATER_THAN_OR_EQUAL</td><td class="example">{"fieldId":"&lt;id&gt;","condition":"GREATER_THAN_OR_EQUAL","value":"10"}</td><td>필드 값이 필터보다 크거나 같은 레코드를 반환합니다.</td><td class="possible">"10", "11"</td></tr>
    <tr><td class="modifier">LESS_THAN</td><td class="example">{"fieldId":"&lt;id&gt;","condition":"LESS_THAN","value":"10"}</td><td>필드 값이 필터보다 작은 레코드를 반환합니다.</td><td class="possible">"9"</td></tr>
    <tr><td class="modifier">LESS_THAN_OR_EQUAL</td><td class="example">{"fieldId":"&lt;id&gt;","condition":"LESS_THAN_OR_EQUAL","value":"10"}</td><td>필드 값이 필터보다 작거나 같은 레코드를 반환합니다.</td><td class="possible">"9", "10"</td></tr>
    <tr><td class="modifier">IS_BETWEEN</td><td class="example">{"fieldId":"&lt;id&gt;","condition":"IS_BETWEEN","value":["2024-01-01","2024-12-31"]}</td><td>필드 값이 두 필터 값 사이에 속하는 레코드를 반환합니다.</td><td class="possible">["2024-03-01","2024-06-30"]</td></tr>
    <tr><td class="modifier">IS_NOT_BETWEEN</td><td class="example">{"fieldId":"&lt;id&gt;","condition":"IS_NOT_BETWEEN","value":["2024-01-01","2024-12-31"]}</td><td>필드 값이 두 필터 값 사이에 속하지 않는 레코드를 반환합니다.</td><td class="possible">["2023-01-01","2025-06-30"]</td></tr>
    <tr><td class="modifier">IS_AFTER</td><td class="example">{"fieldId":"&lt;id&gt;","condition":"IS_AFTER","value":"2024-01-01"}</td><td>날짜 필드 값이 필터 이후인 레코드를 반환합니다.</td><td class="possible">"2024-06-01"</td></tr>
    <tr><td class="modifier">IS_BEFORE</td><td class="example">{"fieldId":"&lt;id&gt;","condition":"IS_BEFORE","value":"2024-12-31"}</td><td>날짜 필드 값이 필터 앞에 있는 레코드를 반환합니다.</td><td class="possible">"2024-06-01"</td></tr>
    <tr><td class="modifier">IS_ANY_OF</td><td class="example">{"fieldId":"&lt;id&gt;","condition":"IS_ANY_OF","value":["Active","Planned"]}</td><td>필드 값이 필터 목록의 값과 일치하는 레코드를 반환합니다.</td><td class="possible">["활성","계획됨","완료"]</td></tr>
    <tr><td class="modifier">IS_NONE_OF</td><td class="example">{"fieldId":"&lt;id&gt;","condition":"IS_NONE_OF","value":["Active","Planned"]}</td><td>필드 값이 필터 목록에 있는 값 중 어느 것과도 일치하지 않는 레코드를 반환합니다</td><td class="possible">["활성","계획됨"]</td></tr>
    <tr><td class="modifier">HAS_ANY_OF</td><td class="example">{"fieldId":"&lt;id&gt;","condition":"HAS_ANY_OF","value":["Tag1","Tag2"]}</td><td>다중 값 필드에 필터 값이 포함된 레코드를 반환합니다.</td><td class="possible">["Tag1","Tag2"]</td></tr>
    <tr><td class="modifier">HAS_ALL_OF</td><td class="example">{"fieldId":"&lt;id&gt;","condition":"HAS_ALL_OF","value":["Tag1","Tag2"]}</td><td>다중 값 필드에 모든 필터 값이 포함된 레코드를 반환합니다.</td><td class="possible">["Tag1","Tag2"]</td></tr>
    <tr><td class="modifier">IS_EXACTLY</td><td class="example">{"fieldId":"&lt;id&gt;","condition":"IS_EXACTLY","value":["Tag1"]}</td><td>다중 값 필드에 필터 값이 정확히 포함되고 다른 값은 포함되지 않은 레코드를 반환합니다.</td><td class="possible">["Tag1"]</td></tr>
    <tr><td class="modifier">HAS_NONE_OF</td><td class="example">{"fieldId":"&lt;id&gt;","condition":"HAS_NONE_OF","value":["Tag1"]}</td><td>다중 값 필드에 필터 값이 포함되지 않은 레코드를 반환합니다.</td><td class="possible">["Tag1"]</td></tr>
  </tbody>
</table>


>[!NOTE]
>
>버전 1 참고: V1 수정자 이름은 `$-prefixed camelCase`을(를) 사용합니다(예: `$contains`, `$isNot`, `$isEmpty`, `$greaterThan`, `$greaterThanOrEqual`, `$lessThan`, `$lessThanOrEqual`, `$isBetween`, `$isNotBetween`, `$isAnyOf`, `$hasAllOf`). 각 수정자의 동작은 동일합니다.


## 필드 유형별 지원되는 필터 조건

| 필드 유형 | 지원되는 조건 |
|-----------------------------|--------------------------------------------------------------------------------------------------------------|
| 텍스트, 긴 텍스트 | CONTAINS, DOES_NOT_CONTAIN, IS, IS_NOT, IS_EMPTY, IS_NOT_EMPTY |
| 숫자, 백분율, 통화 | IS, IS_NOT, GREATER_THAN, GREATER_THAN_OR_EQUAL, LESS_THAN, LESS_THAN_OR_EQUAL, IS_EMPTY, IS_NOT_EMPTY |
| 일자 | IS, IS_NOT, IS_AFTER, IS_BEFORE, IS_BETWEEN, IS_NOT_BETWEEN, IS_EMPTY, IS_NOT_EMPTY |
| 단일 선택 | IS, IS_NOT, IS_ANY_OF, IS_NONE_OF, IS_EMPTY, IS_NOT_EMPTY |
| 다중 선택, 사용자 | HAS_ANY_OF, HAS_ALL_OF, IS_EXACTLY, HAS_NONE_OF, IS_EMPTY, IS_NOT_EMPTY |
| 부울 | 다음과 같음 |
| 공식 | CONTAINS, DOES_NOT_CONTAIN, IS, IS_NOT, IS_EMPTY, IS_NOT_EMPTY |
| 작성자 | IS, IS_NOT, IS_ANY_OF, IS_NONE_OF |
| 업데이트한 사람 | IS, IS_NOT, IS_ANY_OF, IS_NONE_OF, IS_EMPTY, IS_NOT_EMPTY |
| 생성 시간 | IS, IS_NOT, IS_AFTER, IS_BEFORE, IS_BETWEEN, IS_NOT_BETWEEN |
| 업데이트 시간 | IS, IS_NOT, IS_AFTER, IS_BEFORE, IS_BETWEEN, IS_NOT_BETWEEN, IS_EMPTY, IS_NOT_EMPTY |
| 참조 | HAS_ANY_OF, HAS_ALL_OF, IS_EXACTLY, HAS_NONE_OF, IS_EMPTY, IS_NOT_EMPTY |
| 조회 | 연결된 필드 유형에 따라 다릅니다. |

>[!NOTE]
>
>**버전 1 참고:** 버전 1에서는 접두사가 있는 `$` 연산자 이름(예: `$contains`, `$greaterThan`, `$isAnyOf`, `$hasAllOf`)을 사용합니다. 필드 유형당 지원되는 조건 집합이 동일합니다.

## 사람 필드별 필터링

사람 필드 필터(`user`, `created-by`, `updated-by`, `approved-by`)는 Adobe IMS 사용자 ID와 Workfront 사용자 ID를 모두 허용합니다. 일반 문자열 값은 Adobe IMS 사용자 ID로 해석됩니다.

식별자 유형을 설정하여 Workfront 사용자 ID를 확인하려면 `id` 및 `idType` 매개 변수를 명시적으로 전달해야 합니다. `idType`에 지원되는 값은 Workfront 사용자 ID의 경우 &quot;`WF`&quot;이고, Adobe IMS 사용자 ID의 경우 &quot;`IMS`&quot;입니다.

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
> 버전 1 참고: V1은 사용자의 IMS ID로만 필터링을 지원합니다.

## 외부 ID별 외부 참조 필드 필터링

외부 참조 필드는 레코드를 다른 Adobe 시스템(예: Workfront 프로젝트 또는 AEM Assets)의 개체에 연결합니다. 내부적으로 Planning은 이러한 객체에 Planning 레코드 ID를 지정합니다. 원본 개체 ID로 이러한 필드를 직접 필터링하려면 필터 조건에 `"matchExternalId": true`을(를) 추가하십시오.

이 플래그는 `referenceOptions.isExternal`이(가) `true`인 참조 필드에만 유효하며 외부 참조 필드가 아닌 필드에는 무시됩니다. 단일 문자열 값을 확인할 수 없으면 요청이 `400 Bad Request`(으)로 실패합니다. 목록 값이 제공되면 해결되지 않은 항목은 변경되지 않은 상태로 전달되고 단순히 일치하지 않습니다.

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
>버전 1 참고: V1은 외부 개체 ID에 의한 필터링을 지원하지 않습니다.

## 외부 연결 필드

Planning 레코드 유형은 다른 Planning 레코드 유형 대신 다른 Adobe 시스템의 객체에 레코드를 연결하는 외부 참조 필드를 호스팅할 수 있습니다.

API를 통해 외부 참조 필드를 만들려면 새 `REFERENCE` 필드에 대한 `referenceOptions.recordTypeId`을(를) 원하는 외부 레코드 종류의 ID로 설정하십시오. 서버가 대상 레코드 형식에서 `referenceOptions.isExternal=true` 및 연결 메타데이터(`connectionName, objectName`)를 자동으로 파생합니다.

지원되는 외부 오브젝트 유형에는 Workfront 오브젝트(프로젝트, 작업, 프로그램, 포트폴리오, 회사, 그룹, 팀, 사용자) 및 AEM Assets(에셋, 콘텐츠 조각)가 포함됩니다.

>[!NOTE]
>
>버전 1 참고: V1은 외부 연결 필드 만들기를 지원하지 않습니다.


## 정렬

요청에 `sort` 배열을 포함하여 모든 필드별로 결과를 정렬합니다.

```
json
{
  "sort": [
    { "fieldId": "F6527ecb25df57c441d92b9fc", "direction": "asc" },
    { "fieldId": "F658afcbd4a0273c67c346fd5", "direction": "desc" }
  ]
}
```

여러 정렬 필드는 순서대로 평가됩니다. 페이지 매김할 때 항상 정렬을 적용하여 페이지 간에 일관된 순서를 유지합니다.

결과를 그룹화하려면 정렬과 함께 그룹 배열을 포함합니다.

```
{ 
  "sort": [{ "fieldId": "F001", "direction": "asc" }], 
  "group": [{ "fieldId": "F002", "direction": "asc" }] 
} 
```

>[!NOTE]
>
>버전 1 참고: V1은 `sorting`(`sort`이(가) 아님), `groupingFieldIds`(필드 ID 배열, `group` 개체가 아님) 및 이제 사용되지 않는 `rowOrderViewId`을(를) 사용하여 기존 보기의 행 순서를 적용합니다. 이러한 V1 매개 변수는 버전에서 지원되지 않습니다.

## 필드 도법

응답에서 반환되는 필드를 제한하려면 `fieldIds` 또는 `fieldAliases` 쿼리 매개 변수를 쉼표로 구분된 목록으로 사용하십시오. 이렇게 하면 응답 페이로드 크기가 줄어들며 대량 또는 지연 시간에 민감한 통합에 권장됩니다.

>[!NOTE]
>
>**버전 1 참고:** 버전 1은 `?fieldIds=` 또는 `?fieldAliases=`이(가) 아닌 프로젝션(예: `?attributes=data,createdBy`)에 `?attributes=`을(를) 사용합니다.

## 쪽 매기기

Planning API는 큰 데이터 세트를 관리하기 위해 페이지 매김된 응답을 지원합니다.

* **커서 기반 페이지 매김**&#x200B;은(는) 작업 공간, 레코드 종류, 필드 및 보기에 사용됩니다. 다음 페이지를 검색하려면 이전 응답의 `cursor` 값을 전달하십시오. 커서 기반 응답에는 페이지가 더 많은지 여부를 나타내는 hasMore 플래그가 포함됩니다.
* **페이지 기반 페이지 매김**&#x200B;이 레코드 검색에 사용됩니다. 쿼리 매개 변수로 `page` 및 `size`을(를) 사용합니다. 페이지 매김할 때 항상 정렬을 적용하여 페이지 간에 일관된 순서를 유지합니다. 페이지 매김은 0을 기반으로 하므로 두 번째 페이지의 결과를 검색하려면 &quot;`page=1`&quot;을(를) 매개 변수로 사용하십시오.

예를 들어 다음 요청을 사용하여 레코드 검색에서 500개의 레코드 중 두 번째 페이지를 검색합니다.

```
POST /v2/record-types/{recordTypeId}/records/search?page=1&size=500 
{ 
  "sort": [{ "fieldId": "F6527ecb25df57c441d92b9fc", "direction": "asc" }], 
  "filter": { "operator": "AND", "conditions": [ 
    { "fieldId": "<fieldId>", "condition": "IS", "value": "active" } 
  ] } 
} 
```

모든 페이지가 매겨진 응답에는 더 많은 결과를 사용할 수 있는지 여부를 나타내는 구조화된 포락선이 포함됩니다. 페이지 매김할 때 항상 정렬을 적용하여 페이지 간에 일관된 순서를 유지합니다.

>[!NOTE]
>
> **버전 1 참고:** V1은 요청 본문에 전달된 `offset` 및 `limit`을(를) 사용합니다(기본값 500, 최대 2,000). 레코드 2001-4000을 검색하려면 요청 본문에 &quot;`offset`&quot;: &quot;`2000`&quot;, &quot;`limit`&quot;: &quot;`2000`&quot;을(를) 설정하십시오. 응답이 `totalCount` 필드가 있는 플랫 레코드 배열을 반환합니다.

## 대량 작업

Planning API는 단일 요청에서 레코드의 벌크 만들기, 업데이트, 패치 및 삭제를 지원합니다. 끝점 경로, 요청 형식 및 작업당 레코드 제한에 대해서는 [developer.adobe.com/wf-planning](https://developer.adobe.com/wf-planning)의 **API 참조**&#x200B;을(를) 참조하십시오.

>[!NOTE]
>
>**버전 1 참고:** 대량 작업은 버전 1에서 사용할 수 없습니다.


## 권한

엔티티에 대한 권한은 리소스 엔드포인트 자체와 별개로 전용 권한 API를 통해 관리됩니다. 이를 통해 현재 권한을 읽고, 공유 목록을 관리하고, 데이터 작업과 독립적으로 액세스 요청을 처리할 수 있습니다. 자세한 내용은 문서 [Workfront 계획 API](https://developer.adobe.com/wf-planning)의 &quot;API 참조&quot; 섹션을 참조하십시오.

>[!NOTE]
>
>**버전 1 참고:** 버전 1은 공개 권한 API를 표시하지 않습니다. 권한 수준은 리소스 응답 DTO에 직접 포함됩니다.

## Workfront 사용자 정의 양식에서 Planning API 사용

Workfront 사용자 정의 양식의 외부 조회 필드에서 Planning API를 호출하여 Workfront 개체 내에서 직접 Planning 데이터를 표시할 수 있습니다. 자세한 내용은 [사용자 지정 양식의 외부 조회 필드 예제](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/form-designer/design-a-form/external-lookup-examples.md)를 참조하십시오.

## 관련 리소스

API 관련 추가 설명서는 다음 문서를 참조하십시오.

* [Workfront 계획 API](https://developer.adobe.com/wf-planning) 개발자 설명서 및 참조
* [Adobe Workfront Planning 시작](/help/quicksilver/planning/general/planning-overview.md)
* [Adobe Workfront Planning 액세스 개요](/help/quicksilver/planning/access/access-overview.md)
* [Workfront 통합을 위한 OAuth2 애플리케이션 만들기](/help/quicksilver/administration-and-setup/configure-integrations/create-oauth-application.md)

<!--

Our version of this article before Lilit replaced it with the above: 

The goal for the Adobe Workfront Planning API is to simplify building integrations with Planning by introducing a REST-ful architecture that operates over HTTP. This document assumes you are familiar with REST and JSON responses and describes the approach taken by the Planning API.  

A familiarity with the Workfront Planning schema will assist you in understanding the database relationships that can be utilized to pull data out of Workfront Planning for integration purposes. 

You can call the planning API from an External lookup field in a Workfront custom form.

For more information on External lookup fields, see [Examples of the External lookup field in a custom form](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/form-designer/design-a-form/external-lookup-examples.md).

>[!NOTE]
>
>When using the Planning API, all user-related information will be returned using the Adobe Identity Management System (IMS) user ID, and not the Workfront user ID.
>
>For information, see [Manage users in the Adobe Admin Console](/help/quicksilver/administration-and-setup/add-users/create-and-manage-users/admin-console.md).  

## Workfront Planning API versions

* Version 1 - released in July 2024 

  For more information, see the section [Workfront Planning API Version 1](#workfront-planning-api-version-1) in this article. 

* Version 2 - released in May 2026

  For more information, see the section [Workfront Planning API Version 2](#workfront-planning-api-version-2) in this article.


## Workfront Planning API Version 1

Workfront Planning API Version 1 was released in July 2024.

The following sections described functionality that was made available in the Workfront API Version 1. 

All future API version will contain the same functionality, unless otherwise specified. 

### Operations 

Objects are manipulated by sending an HTTP request to their unique URI. The operation to be performed is specified by the HTTP method. 

The standard HTTP methods correspond to the following operations: 

* **GET** - Retrieves an object by ID, searches for all objects by a query 
* **POST** - Inserts a new object 
* **PUT** - Edits an existing object 
* **DELETE** - Deletes an object 

For more details and examples of each operation, see the [Workfront Planning API developer documentation](https://developer.adobe.com/wf-planning/).

### Field types and search modifiers used with them 

You can use modifiers and filters with fields to control what data will be returned in results. 

For examples, see the [Workfront Planning API developer documentation](https://developer.adobe.com/wf-planning/).

#### Using search modifiers 

Workfront Planning supports the following search modifiers: 

<table>
    <tr>
        <td><b>Modifier</b></td>
        <td><b>Example</b></td>
        <td><b>Description</b></td>
        <td><b>Possible Values</b></td>
    </tr>
    <tr>
        <td>$contains </td>
        <td><code>"fieldId": { "$contains": "product" } </code> </td>
        <td>Returns records whose field value contains the filter  </td>
        <td>"New Product Launch"  </td>
    </tr>
    <tr>
        <td>$doesNotContain</td>
        <td><code>"fieldId": { "$doesNotContain": "product" } </code> </td>
        <td>Returns records where the field value does not contain the filter  </td>
        <td>"New Launch"  </td>
    </tr>
    <tr>
        <td>$is </td>
        <td><ul><li><code>"fieldId" : { "$is": "new product launch" } </code></li><li><code>"fieldId" : { "new product launch" } </code></li><ul> </td>
        <td>Returns records whose field value exactly match the filter  </td>
        <td>"New Product Launch"  </td>
    </tr>
    <tr>
        <td>$isNot </td>
        <td><code>"fieldId": { "$isNot": "product" } </code> </td>
        <td>Returns records whose field value exactly is not match the filter  </td>
        <td>"New Product Launch"  </td>
    </tr>
    <tr>
        <td>$isEmpty </td>
        <td><ul><li><code>"fieldId": "$isEmpty" </code></li><li><code>"fieldId": { "$isEmpty": null } </code></li><ul> </td>
        <td>Returns records whose field value is empty  </td>
        <td><ul><li>"" </li><li>null </li><ul>  </td>
    </tr>
    <tr>
        <td>$isNotEmpty </td>
        <td><ul><li><code>"fieldId": "$isNotEmpty"  </code></li><li><code>"fieldId": { "$isNotEmpty": null } </code></li><ul> </td>
        <td>Returns records whose field value is not empty  </td>
        <td>"New Product Launch"  </td>
    </tr>
    <tr>
        <td>$greaterThan </td>
        <td><code>"fieldId": { "$greaterThan": 10 } </code> </td>
        <td>Returns records whose field value is greater than the filter  </td>
        <td><ul><li>20</li><li>25</li><ul> </td>
    </tr>
    <tr>
        <td>$greaterThanOrEqual </td>
        <td><code>"fieldId": { "$greaterThanOrEqual": 10 } </code> </td>
        <td>Returns records whose field value is greater than or equal the filter  </td>
        <td><ul><li>10</li><li>20</li><li>25</li> </ul></td>
    </tr>
    <tr>
        <td>$lessThan </td>
        <td><code>"fieldId": { "$lessThan": 10 } </code> </td>
        <td>Returns records whose field value is less than the filter  </td>
        <td><ul><li>5</li><li>9</li></td></ul> 
    </tr>
    <tr>
        <td>$lessThanOrEqual </td>
        <td><code>"fieldId": { "$lessThanOrEqual": 10 } </code> </td>
        <td>Returns records whose field value is less than or equal the filter </td>
        <td><ul><li>5</li><li>9</li><ul><li>10</li> </td>
    </tr>
    <tr>
        <td>$isAfter </td>
        <td><code>"fieldId": { "$isAfter": "2024-05-14T20:00:00.000Z" } </code> </td>
        <td>Returns records whose field value is after the filter  </td>
        <td>"2024-05-15T20:00:00.000Z"  </td>
    </tr>
    <tr>
        <td>$isBefore </td>
        <td><code>"fieldId": { "$isBefore": "2024-05-14T20:00:00.000Z" } </code> </td>
        <td>Returns records whose field value is before the filter </td>
        <td>"2024-05-12T20:00:00.000Z" </td>
    </tr>
    <tr>
        <td>$isBetween </td>
        <td><code>"fieldId": { "$isBetween": ["2024-05-10T20:00:00.000Z", "2024-05-15T20:00:00.000Z"] } </code> </td>
        <td>Returns records whose field value is between the filter  </td>
        <td><ul><li>"2024-05-12T20:00:00.000Z" </li><li>"2024-05-14T20:00:00.000Z" </li><ul>  </td>
    </tr>
    <tr>
        <td>$isNotBetween </td>
        <td><code>"fieldId": { "$isNotBetween": ["2024-05-10T20:00:00.000Z", "2024-05-15T20:00:00.000Z"] } </code> </td>
        <td>Returns records whose field value is not between the filter  </td>
        <td><ul><li>"2024-05-09T20:00:00.000Z"  </li><li>"2024-05-17T20:00:00.000Z"  </li><ul>  </td>
    </tr>
    <tr>
        <td>$isAnyOf </td>
        <td><code>"fieldId": { "$isAnyOf": ["active", "completed"] } </code> </td>
        <td>Returns records whose field value is any of the filter  </td>
        <td><ul><li>"active" </li><li>"completed" </li><ul> </td>
    </tr>
    <tr>
        <td>$isNoneOf </td>
        <td><code>"fieldId": { "$isNoneOf": ["active", "completed"] } </code> </td>
        <td>Returns records whose field value is none of the filter </td>
        <td><ul><li>"finished"  </li><li>"fixed"  </li><ul> </td>
    </tr>
    <tr>
        <td>$hasAnyOf </td>
        <td><code>"fieldId": { "$hasAnyOf": ["active", "completed"] } </code> </td>
        <td>Returns records whose field value has any of the filter  </td>
        <td><ul><li>["active", "fixed"]  </li><li>["fixed", "completed", "finished"]  </li><ul> </td>
    </tr>
    <tr>
        <td>$hasAllOf </td>
        <td><code>"fieldId": { "$hasAllOf": ["active", "completed"] } </code> </td>
        <td>Returns records whose field value has all of the filter  </td>
        <td><ul><li>["active", "completed"]   </li><li>["active", "completed", "finished"]   </li><ul> </td>
    </tr>
    <tr>
        <td>$hasNoneOf </td>
        <td><code>"fieldId": { "$hasNoneOf": ["active", "completed"] } </code> </td>
        <td>Returns records whose field value has none of the filter </td>
        <td>["fixed", "finished"]  </td>
    </tr>
    <tr>
        <td>$isExactly </td>
        <td><code>"fieldId": { "$isExactly": ["active", "completed"] } </code> </td>
        <td>Returns records whose field value is exactly the filter  </td>
        <td>["active", "completed"]  </td>
    </tr>
</table>
 
#### Field types 

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

### Using "And" and "Or" statements 

In the API call you can have filters that are based on several criteria combined by $and" and "$or" statements  

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

### Using the fields request parameter 

You can use the fields request parameter to specify a comma-separated list of specific fields that should be returned. These field names are case-sensitive.  

For example, the request 

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

returns a response similar to the following: 

  
```
{ 
    "priority": 2, 
    "name": "first task", 
    "ID": "4c7c08fa0000002ff924e298ee148df4", 
    "plannedStartDate": "2010-08-30T09:00:00:000-0600" 
} 
```

### Sorting query results in the API 

You can sort your results by any field if you append the following to your API call: 


`/v1/records/search`

Request body:

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

### Query limits and paginated responses 

By default, Planning API requests return 500 results, starting from the beginning of the list. To override the default limitation for number of results, you can use the `limit` parameter in your requests and set it to a different number, up to 2000 results.  

We recommend that you consider using paginated responses for large datasets by adding the `offset` parameter to your requests. Paginated responses allow you to specify the location of the first result that should be returned. 

For example, if you want to return the results 2001-4000, you can use the following request. This example returns 2000 records that are in active status, starting from the 2001st result: 

`POST /v1/records/search`


Request body: 

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

To make sure your results are properly paginated, use a sorting parameter. This allows the results to be returned in the same order, so that the pagination does not repeat or skip results. 

For more information on sorting, see [Sorting query results in the API](#sorting-query-results-in-the-api) in this article.


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