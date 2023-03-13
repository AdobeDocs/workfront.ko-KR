---
content-type: api
navigation-topic: general-api
title: 이벤트 구독 API
description: 이벤트 구독 API
author: Becky
feature: Workfront API
exl-id: c3646a5d-42f4-4af8-9dd0-e84977506b79
source-git-commit: 34810c67de5578479ae56cd72865656a89d35aa9
workflow-type: tm+mt
source-wordcount: '2111'
ht-degree: 3%

---


# 이벤트 구독 API

<!--BOB clean this up-->

<!--
{{highlighted-preview}}
-->

이벤트 구독이 지원하는 Adobe Workfront 개체에서 작업이 발생하면 원하는 끝점에 응답을 보내도록 Workfront을 구성할 수 있습니다. 즉, 서드파티 애플리케이션은 업데이트 발생 직후 Workfront API를 통해 Workfront 상호 작용에서 업데이트를 받을 수 있습니다. 일반적으로 기록되는 데이터 변경 사항에서 5초 이내에 웹후크 알림을 받을 수 있습니다. 평균적으로 고객은 기록되는 데이터 변경 사항에서 1초 이내에 웹후크 알림을 받습니다.  

허용 목록에 추가하다 귀하의 방화벽을 통해 이벤트 구독 페이로드를 수신하려면 다음 IP 주소를 귀하의 방화벽에 추가해야 합니다.

**유럽 지역 고객의 경우:**

* 52.30.133.50
* 52.208.159.124
* 54.220.93.204
* 52.17.130.201
* 34.254.76.122
* 34.252.250.191

**유럽 이외의 지역 고객의 경우:**

* 54.244.142.219
* 44.241.82.96
* 52.36.154.34
* 34.211.224.9
* 54.218.48.56
* 52.39.217.230

다음 항목은 이벤트 구독 API를 지원합니다.

## 이벤트 구독에서 지원하는 오브젝트

다음 Workfront 개체는 이벤트 구독에서 지원됩니다.

* 할당
* 회사
* 대시보드
* 문서
* 경비
* 시간
* 문제
* 참고
* 포트폴리오
* 프로그램
* 프로젝트
* 보고서
* 작업
* 템플릿
* 타임시트
* 사용자

이벤트 구독 오브젝트에서 지원하는 필드 목록은 다음을 참조하십시오. [이벤트 구독 리소스 필드](../../wf-api/api/event-sub-resource-fields.md).

## 이벤트 구독 인증

이벤트 구독을 생성, 쿼리 또는 삭제하려면 Workfront 사용자에게 다음이 필요합니다.

* 이벤트 구독을 사용하려면 &quot;시스템 관리자&quot;의 액세스 수준이 필요합니다.
* A `sessionID`  이벤트 구독 API를 사용하려면 헤더가 필요합니다.

   자세한 내용은 [인증](api-basics.md#authentication) 위치: [API 기본 사항](api-basics.md).

## 구독 리소스 구성

구독 리소스에는 다음 필드가 포함되어 있습니다.

* objId (선택 사항)

   * **문자열** - 이벤트가 실행되는 지정된 objCode의 개체 ID입니다. 이 필드가 지정되지 않으면 사용자는 지정된 유형의 모든 객체에 대한 이벤트를 수신합니다.

* objCode(필수)

   * **문자열** - 변경 사항을 구독 중인 오브젝트의 objCode입니다. 아래 표에는 objCode에 대해 가능한 값이 나열되어 있습니다.

      <table style="table-layout:auto"> 
      <col> 
      <col> 
      <thead> 
       <tr> 
        <th><p>오브젝트</p></th> 
        <th><p>objCode</p></th> 
       </tr> 
      </thead> 
      <tbody> 
       <tr> 
        <td scope="col">할당</td> 
        <td scope="col"><p>ASSIGN</p></td> 
       </tr> 
       <tr> 
        <td scope="col">회사 </td> 
        <td scope="col"><p>지저분해</p></td> 
       </tr> 
       <tr> 
        <td scope="col">대시보드</td> 
        <td scope="col">PTLTAB</td> 
       </tr> 
       <tr> 
        <td scope="col"><p>문서</p></td> 
        <td scope="col">도쿠 </td> 
       </tr> 
       <tr> 
        <td scope="col"><p>경비</p></td> 
        <td scope="col">확장</td> 
       </tr> 
       <tr> 
        <td scope="col"><p>시간</p></td> 
        <td scope="col">시간</td> 
       </tr> 
       <tr> 
        <td scope="col">문제</td> 
        <td scope="col"><p>OPTASK</p></td> 
       </tr> 
       <tr> 
        <td scope="col">참고</td> 
        <td scope="col">메모</td> 
       </tr> 
       <tr> 
        <td scope="col"><p>포트폴리오</p></td> 
        <td scope="col"><p>포트</p></td> 
       </tr> 
       <tr> 
        <td scope="col"><p>프로그램</p></td> 
        <td scope="col"><p>PRGM</p></td> 
       </tr> 
       <tr> 
        <td scope="col"><p>프로젝트</p></td> 
        <td scope="col"><p>프로젝트</p></td> 
       </tr> 
       <tr> 
        <td scope="col"><p>보고서</p></td> 
        <td scope="col"><p>PTLSEC</p></td> 
       </tr> 
       <tr> 
        <td scope="col"><p>작업</p></td> 
        <td scope="col"><p>작업</p></td> 
       </tr> 
       <tr> 
        <td scope="col"><p>템플릿</p></td> 
        <td scope="col"><p>템플릿</p></td> 
       </tr> 
       <tr> 
        <td scope="col">타임시트</td> 
        <td scope="col">체트</td> 
       </tr> 
       <tr> 
        <td scope="col">사용자</td> 
        <td scope="col">사용자</td> 
       </tr> 
      </tbody> 
     </table>

* eventType(필수)

   * **문자열** - 개체가 구독한 이벤트 유형을 나타내는 값입니다. 사용 가능한 이벤트 유형은 다음과 같습니다.

      * 만들기
      * DELETE 
      * 업데이트

* url(필수)

   * **문자열** - HTTP를 통해 구독 이벤트 페이로드가 전송되는 끝점의 URL입니다.

* authToken(필수)

   * **문자열** - &quot;URL&quot; 필드에 지정된 URL로 인증하는 데 사용되는 OAuth2 전달자 토큰입니다. 

## 이벤트 구독 API 요청 만들기

사용자에게 관리자 액세스 권한이 있는지 확인하고 구독 리소스를 구성한 후에는 이벤트 구독을 만들 수 있습니다.

다음 구문을 사용하여 URL을 생성합니다.

**요청 URL:**


```
POST https://<HOSTNAME>/attask/eventsubscription/api/v1/subscriptions
```

**요청 헤더:**

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th> <p>헤더 이름</p> </th> 
   <th> <p>헤더 값</p> </th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td> <p>Content-type</p> </td> 
   <td> <p>application/json</p> </td> 
  </tr> 
  <tr> 
   <td> <p>sessionID</p> </td> 
   <td> <p>sessionID 값</p> </td> 
  </tr> 
 </tbody> 
</table>

**요청 본문 예:**

<!-- [Copy](javascript:void(0);) -->

```
{
                "objCode": "PROJ",
                "eventType": "UPDATE",
                "url": "http://requestb.in/ua5hi2ua",
                "authToken": "EauthTokenWorkfrontRocks1234_"
            }
```

| 응답 코드 | 설명 |
|---|---|
| 201(생성됨) | 이벤트 구독이 정상적으로 생성되었습니다. |
| 400(잘못된 요청) | 구독 리소스의 URL 필드가 유효하지 않은 것으로 간주되었습니다. |
| 401(승인되지 않음) | 입력한 sessionID가 비어 있거나 유효하지 않은 것으로 간주되었습니다. |
| 403(금지됨) | 제공된 sessionID와 일치하는 사용자에게 관리자 액세스 권한이 없습니다. |

구독 리소스를 요청 본문으로 전달하면(&quot;application/json&quot; 콘텐츠 유형이 있음) 지정된 개체에 대해 이벤트 구독이 생성됩니다. 응답 코드 201(생성됨)은 구독이 생성되었음을 나타냅니다. 201 이외의 응답 코드는 구독이 **아님** 생성됨.

>[!NOTE]
>
> &quot;위치&quot; 응답 헤더에는 새로 만든 이벤트 구독의 URI가 포함되어 있습니다.

**응답 헤더 예:**

| 응답 헤더 | 예 |
|---|---|
| Content-Length | `→0` |
| 일자 | `→Wed, 05 Apr 2017 21:23:33 GMT` |
| 위치 | `→https://<HOSTNAME>/attask/eventsubscription/api/v1/subscriptions/750a636c-5628-48f5-ba26-26b7ce537ac2` |
| 서버 | `→Apache-Coyote/1.1` |

## 이벤트 구독 쿼리

Workfront의 HTTP를 쿼리할 때 GET 메서드를 사용합니다. 이벤트 구독을 쿼리하는 방법에는 구독 ID로 쿼리(아래 참조) 또는 모든 이벤트 구독을 쿼리하는 두 가지가 있습니다.

### 모든 이벤트 구독 쿼리

고객에 대한 모든 이벤트 구독을 쿼리하거나 다음을 사용하여 응답을 관리할 수 있습니다. 다음 옵션을 사용하여 응답을 관리할 수도 있습니다.

* **페이지**: 반환할 페이지 수를 지정하는 쿼리 매개 변수 옵션입니다. 기본값은 1입니다.
* **제한**: 페이지당 반환할 결과 수를 지정하는 쿼리 매개 변수 옵션입니다. 기본값은 100(최대 1,000)입니다.

특정 고객에 대한 모든 이벤트 구독을 나열하기 위한 요청 구문은 다음과 같습니다.

**요청 URL:**

<!-- [Copy](javascript:void(0);) -->

```
GET https://<HOSTNAME>/attask/eventsubscription/api/v1/subscriptions
```

**요청 헤더:**

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th> <p>헤더 이름</p> </th> 
   <th> <p>헤더 값</p> </th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td> <p>sessionID</p> </td> 
   <td> <p>sessionID 값</p> </td> 
  </tr> 
 </tbody> 
</table>

**응답 코드:**

| 응답 코드 | 설명 |
|---|---|
| 200(확인) | 제공된 sessionID와 일치하는 고객에 대해 발견된 모든 이벤트 구독과 함께 요청이 반환되었습니다. |
| 401(승인되지 않음) | 입력한 sessionID가 비어 있습니다. |
| 403(금지됨) | 제공된 sessionID와 일치하는 사용자에게 관리자 액세스 권한이 없습니다. |


**응답 헤더 예:**

| 응답 헤더 | 예 |
|---|---|
| Content-Type | `→application/json;charset=UTF-8` |
| 일자 | `→Wed, 05 Apr 2017 21:29:32 GMT` |
| 서버 | `→Apache-Coyote/1.1` |
| 전송 인코딩 | `→chunked` |


**응답 본문 예:**

<!-- [Copy](javascript:void(0);) -->

```
                {
                "subscriptions":                
                [
                {
                "id": "37c4bcf5-e0b5-4256-aba3-a51cba7bf997",
                "customerId": "504f9640000013401be513579fbebffa",
                "objId": "ObjId1234",
                "objCode": "TASK",
                "url": "http://test.test.net/test/1234",
                "eventType": "UPDATE",
                "authToken": "auth_token"
                },
                {
                "id": "750a636c-5628-48f5-ba26-26b7ce537ac2",
                "customerId": "504f9640000013401be513579fbebffa",
                "objId": null,
                "objCode": "PROJ",
                "url": "http://requestb.in/ua5hi2ua",
                "eventType": "UPDATE",
                "authToken": "authTokenWorkfrontRocks1234_"
                }
                ],
                "meta":
                {
                "page": 1,
                "page_count": 2,
                "limit": 100,
                "total_count": 150
                }
                }            
```

위치

* **페이지** 및 **제한** 요청에 제공된 값이거나 제공된 값이 없는 경우 기본값입니다
* **page_count** 쿼리할 수 있는 총 페이지 수입니다.
* **total_count** 는 쿼리와 일치하는 총 구독 수입니다.

### 이벤트 구독 ID로 쿼리

이벤트 구독의 ID로 이벤트 구독을 쿼리할 수 있습니다. 이벤트 구독을 나열하기 위한 요청 구문은 다음과 같습니다.

**요청 URL:**

<!-- [Copy](javascript:void(0);) -->

```
GET https://<HOSTNAME>/attask/eventsubscription/api/v1/subscriptions/<SUBSCRIPTION ID>
```

**요청 헤더:**

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th> <p>헤더 이름</p> </th> 
   <th> <p>헤더 값</p> </th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td> <p>sessionID</p> </td> 
   <td> <p>sessionID 값</p> </td> 
  </tr> 
 </tbody> 
</table>

**응답 코드:**

| 응답 코드 | 설명 |
|---|---|
| 200(확인) | 제공된 구독 ID와 일치하는 이벤트 구독과 함께 요청이 반환되었습니다. |
| 401(승인되지 않음) | 입력한 sessionID가 비어 있습니다. |
| 403(금지됨) | 제공된 sessionID와 일치하는 사용자에게 관리자 액세스 권한이 없습니다. |


**응답 본문 예:**

<!-- [Copy](javascript:void(0);) -->

```
{
                "id": "750a636c-5628-48f5-ba26-26b7ce537ac2",
                "customerId": "504f9640000013401be513579fbebffa",
                "objId": null,
                "objCode": "PROJ",
                "url": "http://requestb.in/ua5hi2ua",
                "eventType": "UPDATE",
                "authToken": "authTokenWorkfrontRocks1234_"
                }
```

## 이벤트 구독 필터링

이벤트 구독 필터링을 사용하여 관련 메시지만 받도록 할 수 있습니다. 구독에 대한 필터를 만들면 엔드포인트에서 사용해야 하는 메시지 수가 상당히 줄어들 수 있습니다.

예: **업데이트 - 작업** 이벤트 구독은 다음 경우에만 트리거되도록 설정할 수 있습니다. **newState** 이벤트 페이로드의 **taskStatus** 다음으로: **현재**.

>[!IMPORTANT]
다음 속성은 이벤트 구독 필터링에 적용됩니다

* 필터 필드에 비어 있지 않은 값이 있는 경우 **newState** 필터 키 및 값이 포함된 은 구독한 URL로 전송됩니다.
* 에 포함된 사용자 지정 데이터로 필터링할 수 있습니다. **newState** 및/또는 **oldState**/ 오브젝트
* 필터는 특정 값과 동일한지 여부에만 평가됩니다
* 필터 구문이 올바르지 않거나 **newState** 페이로드의 경우 오류가 발생했음을 나타내는 유효성 검사 메시지가 반환되지 않습니다
* 현재 존재하는 구독에서는 필터를 업데이트할 수 없습니다. 새 구독은 새 필터 매개 변수로 만들어야 합니다.
* 여러 필터를 단일 구독에 적용할 수 있으며 모든 필터 조건이 충족된 경우에만 구독이 전달됩니다.
* 단일 구독에 여러 필터를 적용하는 것은 를 사용하는 것과 동일한 방법입니다. **및** 논리 연산자.
* 각 이벤트 구독 간에 하나 이상의 이벤트 구독 필드 매개 변수가 다른 한 단일 오브젝트에 여러 이벤트 구독을 적용할 수 있습니다.
* 여러 이벤트 구독이 단일 개체에 할당되면 해당 개체와 연결된 모든 이벤트 구독이 단일 끝점에 반환될 수 있습니다. 이 방법은 논리 연산자에 대한 동등한 대용으로 사용할 수 있습니다 **또는** 필터 매개 변수를 사용하여 설정할 수 없습니다.

### 비교 연산자 사용

필터 필드와 함께 비교 필드를 지정할 수 있습니다. 비교 결과를 필터링하려면 이 필드에 비교 연산자를 사용하십시오. 예를 들어 작업 상태가 현재와 같지 않은 경우에만 페이로드를 전송하는 UPDATE - TASK 가입을 생성할 수 있습니다. 다음 비교 연산자를 사용할 수 있습니다.

#### eq: 같음

이 필터를 사용하면 발생한 변경 사항이 일치하는 경우 메시지를 전달할 수 있습니다. `fieldValue` 을 정확히 필터에서 클릭합니다. 다음 `fieldValue` 값은 대/소문자를 구분합니다.

```
{
    "objCode": "TASK",
    "eventType": "UPDATE",
    "authToken": "token",
    "url": "https://domain-for-subscription.com/API/endpoint/UpdatedTasks",
    "filters": [
        {
            "fieldName": "name",
            "fieldValue": "again",
            "comparison": "eq"
        }
    ]
}
```

#### ne: 같지 않음

이 필터를 사용하면 발생한 변경 사항이 일치하지 않는 경우 메시지를 보낼 수 있습니다. `fieldValue` 을 정확히 필터에서 클릭합니다. 다음 `fieldValue` 값은 대/소문자를 구분합니다.

```
{
    "objCode": "TASK",
    "eventType": "UPDATE",
    "authToken": "token",
    "url": "https://domain-for-subscription.com/API/endpoint/UpdatedTasks",
    "filters": [
        {
            "fieldName": "name",
            "fieldValue": "again",
            "comparison": "ne"
        }
    ]
}
```

#### gt: 보다 큼

이 필터를 사용하면 지정된 의 업데이트가 있을 경우 메시지를 보낼 수 있습니다. `fieldName` 이(가) 의 값보다 큽니다. `fieldValue`.

```
{
    "objCode": "TASK",
    "eventType": "UPDATE",
    "authToken": "token",
    "url": "https://domain-for-subscription.com/API/endpoint/UpdatedTasks",
    "filters": [
        {
            "fieldName": "plannedCompletionDate",
            "fieldValue": "2022-12-11T16:00:00.000-0800",
            "comparison": "gt"
        }
    ]
}
```

#### gte: 보다 크거나 같음

이 필터를 사용하면 지정된 의 업데이트가 있을 경우 메시지를 보낼 수 있습니다. `fieldName` 다음 값보다 크거나 같음: `fieldValue`.

```
{
    "objCode": "TASK",
    "eventType": "UPDATE",
    "authToken": "token",
    "url": "https://domain-for-subscription.com/API/endpoint/UpdatedTasks",
    "filters": [
        {
            "fieldName": "plannedCompletionDate",
            "fieldValue": "2022-12-11T16:00:00.000-0800",
            "comparison": "gte"
        }
    ]
}
```

#### lt: 보다 작음

이 필터를 사용하면 지정된 의 업데이트가 있을 경우 메시지를 보낼 수 있습니다. `fieldName` 다음 값보다 작음: `fieldValue`.

```
{
    "objCode": "TASK",
    "eventType": "UPDATE",
    "authToken": "token",
    "url": "https://domain-for-subscription.com/API/endpoint/UpdatedTasks",
    "filters": [
        {
            "fieldName": "plannedCompletionDate",
            "fieldValue": "2022-12-18T16:00:00.000-0800",
            "comparison": "lt"
        }
    ]
}
```

#### lte: 보다 작거나 같음

이 필터를 사용하면 지정된 의 업데이트가 있을 경우 메시지를 보낼 수 있습니다. `fieldName` 다음 값보다 작거나 같음: `fieldValue`.

```
{
    "objCode": "TASK",
    "eventType": "UPDATE",
    "authToken": "token",
    "url": "https://domain-for-subscription.com/API/endpoint/UpdatedTasks",
    "filters": [
        {
            "fieldName": "plannedCompletionDate",
            "fieldValue": "2022-12-18T16:00:00.000-0800",
            "comparison": "lte"
        }
    ]
}
```

#### 포함

이 필터를 사용하면 발생한 변경 사항에 `fieldValue` 필터에서. 다음 `fieldValue` 값은 대/소문자를 구분합니다.

```
{
    "objCode": "TASK",
    "eventType": "UPDATE",
    "authToken": "token",
    "url": "https://domain-for-subscription.com/API/endpoint/UpdatedTasks",
    "filters": [
        {
            "fieldName": "name",
            "fieldValue": "again",
            "comparison": "contains"
        }
    ]
}
```

#### 변경

이 필터는 지정된 필드(`fieldName`)의 값은 oldstate와 newstate에서 다릅니다. 지정된 필드 이외의 다른 필드 업데이트(`fieldName`)은 해당 변경 사항을 반환하지 않습니다.

>[!NOTE]
`fieldValue` 아래의 필터 배열에서는 영향을 주지 않습니다.

```
{
    "objCode": "TASK",
    "eventType": "UPDATE",
    "authToken": "token",
    "url": "https://domain-for-subscription.com/API/endpoint/UpdatedTasks",
    "filters": [
        {
            "fieldName": "name",
            "fieldValue": "",
            "comparison": "changed"
        }
    ]
}
```

#### 상태

이 커넥터를 사용하면 필터가 생성 또는 업데이트된 객체의 새 상태 또는 이전 상태에 적용됩니다. 이 기능은 어떤 항목에서 다른 항목으로 변경된 위치를 알고 싶을 때 유용합니다.
`oldState` 만들 수 없음 `eventTypes`.

>[!NOTE]
지정된 필터가 있는 아래 구독은 작업 이름에 포함된 메시지만 반환합니다. `again` 다음에 있음 `oldState`, 작업에 대한 업데이트가 수행되기 전의 작업.
이 메서드의 사용 사례는 사물 간에 변경된 objCode 메시지를 찾는 것입니다. 예를 들어 &quot;Research Some name&quot;에서 &quot;Research TeamName Some name&quot;으로 변경된 모든 작업을 찾으려면

```
{
    "objCode": "TASK",
    "eventType": "UPDATE",
    "authToken": "token",
    "url": "https://domain-for-subscription.com/API/endpoint/UpdatedTasks",
    "filters": [
        {
            "fieldName": "name",
            "fieldValue": "again",
            "comparison": "contains",
            "state": "oldState"
        }
    ]
}
```

### 커넥터 필드 사용

다음 `filterConnector` 구독 페이로드의 필드에서 필터를 적용하는 방법을 선택할 수 있습니다. 기본값은 &quot;AND&quot;이며, 여기서 필터는 모두 다음과 같아야 합니다. `true` 구독 메시지를 보낼 수 있습니다. &quot;OR&quot;을 지정하면 구독 메시지가 표시되기 위해 하나의 필터만 일치해야 합니다.

```
{
    "objCode": "TASK",
    "eventType": "UPDATE",
    "authToken": "token",
    "url": "https://domain-for-subscription.com/API/endpoint/UpdatedTasks",
    "filters": [
        {
            "fieldName": "name",
            "fieldValue": "again",
            "comparison": "contains"
        },
        {
            "fieldName": "name",
            "fieldValue": "also",
            "comparison": "contains"
        }
    ],
    "filterConnector": "AND"
}
```

## 이벤트 구독 삭제

Workfront의 HTTP를 삭제할 때 DELETE 메서드를 사용합니다. 구독 ID로 단일 이벤트 구독을 삭제하는 요청 구문은 다음과 같습니다.

**요청 URL:**

<!-- [Copy](javascript:void(0);) -->

```
DELETE https://<HOSTNAME>/attask/eventsubscription/api/v1/subscriptions/<SUBSCRIPTION ID>
```

**요청 헤더:**

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th> <p>헤더 이름</p> </th> 
   <th> <p>헤더 값</p> </th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td> <p>sessionID</p> </td> 
   <td> <p> sessionID 값 </p> </td> 
  </tr> 
 </tbody> 
</table>

**응답 코드:**

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th> <p>응답 코드</p> </th> 
   <th> 설명</th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td>200(콘텐츠 없음)</td> 
   <td>서버에서 제공된 subscriptionID와 일치하는 이벤트 구독을 제거했습니다.</td> 
  </tr> 
  <tr> 
   <td>401(승인되지 않음)</td> 
   <td>입력한 sessionID가 비어 있습니다.</td> 
  </tr> 
  <tr> 
   <td>403(금지됨)</td> 
   <td>제공된 sessionID와 일치하는 사용자에게 관리자 액세스 권한이 없습니다.</td> 
  </tr> 
  <tr> 
   <td>404(찾을 수 없음)</td> 
   <td>서버에서 삭제하도록 제공된 subscriptionID와 일치하는 이벤트 구독을 찾을 수 없습니다.</td> 
  </tr> 
 </tbody> 
</table>

**응답 헤더 예:**

| 응답 헤더 | 예 |
|---|---|
| 일자 | `→Wed, 05 Apr 2017 21:33:41 GMT` |
| 서버 | `→Apache-Coyote/1.1` |


**응답 본문 예:** 해당 사항 없음

## 이벤트 페이로드의 예

사용자가 받는 페이로드는 오브젝트 유형에 따라 다르지만, 이러한 다양한 페이로드가 전달되는 일관된 형식이 있습니다.

예를 들어 다음 속성은 모든 이벤트 페이로드에서 일관되게 유지됩니다.

* eventType
* subscriptionId
* oldState
* newState
* eventTime

형식에서는 일관되지만 속성에 포함된 값은 개체 및 개체 유형마다 다릅니다.

UPDATE 이벤트 및 CREATE 이벤트에 대한 페이로드 샘플은 아래에 나와 있습니다. UPDATE 예제에서 oldState 및 newState 개체는 동일하지만, CREATE 예제에서 oldState 개체는 비어 있습니다(NULL이 아님).

다음은 UPDATE 이벤트에 대한 예제 페이로드입니다.

<!-- [Copy](javascript:void(0);) -->

```
{
                  "eventType": "UPDATE",
                   "subscriptionId": "8a0d839d5ef32c9a015ef336a5ed0002",
                   "eventTime": {
                       "nano": 998000000,
                       "epochSecond": 1507319336
                   },
                   "newState": {
                "ID": "59d7ddf7000002322d791eb08bafddfb", 
                       "name": "EventSub Test updated",
                       "objCode": "PROJ",
                       "entryDate": "2017-10-06T13:48:07.776-0600",
                       "accessorIDs": [
                           "544820df0000142362741fc0c368de19"
                       ],
                       "lastUpdateDate": "2017-10-06T13:48:56.980-0600",
                       "groupID": "544820df0000140f6a9c1faa7cacadd3",
                       "sponsorID": null,
                       "description": null,
                       "plannedCompletionDate": "2017-10-06T09:00:00.000-0600",
                       "enteredByID": "544820df0000142362741fc0c368de19",
                       "ownerID": "544820df0000142362741fc0c368de19",
                       "templateID": null,
                       "priority": 0,
                       "companyID": null,
                       "portfolioID": null,
                       "referenceNumber": 1894,
                       "lastUpdatedByID": "544820df0000142362741fc0c368de19",
                       "customerID": "544820df0000135b7719dcca654391f6",
                       "currency": null,       "categoryID": null,
                      "status": "CUR",
                      "parameterValues": {}
                   },
                   "oldState": {
                       "ID": "59d7ddf7000002322d791eb08bafddfb",
                       "name": "EventSub Test 180fd595-63fb-4fa9-bd47-58bf6e53d964",
                       "objCode": "PROJ",
                       "entryDate": "2017-10-06T13:48:07.776-0600",
                       "accessorIDs": [
                           "544820df0000142362741fc0c368de19"
                       ],
                       "lastUpdateDate": "2017-10-06T13:48:07.792-0600",
                       "groupID": "544820df0000140f6a9c1faa7cacadd3",
                       "sponsorID": null,
                       "description": null,
                       "plannedCompletionDate": "2017-10-06T09:00:00.000-0600",
                       "enteredByID": "544820df0000142362741fc0c368de19",
                       "ownerID": "544820df0000142362741fc0c368de19",
                       "templateID": null,
                       "priority": 0,
                       "companyID": null,<
                       "portfolioID": null,
                       "referenceNumber": 1894,
                       "lastUpdatedByID": "544820df0000142362741fc0c368de19",
                       "customerID": "544820df0000135b7719dcca654391f6",
                       "currency": null,
                       "categoryID": null,
                       "status": "CUR",
                       "parameterValues": {}
                   }
                }
```

다음은 CREATE 이벤트에 대한 예제 페이로드입니다.

<!-- [Copy](javascript:void(0);) -->

```
{
                "eventType": "CREATE",
                "subscriptionId": "4028e3815ebf03a7015ebfa53b6d0002",
                "eventTime": {
                "nano": 232000000,
                "epochSecond": 1506453831
                },
                "newState": {
                "ID": "59caa946000000e07b0afc3383230c67",
                "name": "EventSub Test fe16d470-0a40-4290-92f4-6a0389fb536c",
                "objCode": "PROJ",
                "entryDate": "2017-09-26T13:23:50.746-0600",
                "accessorIDs": ["544820df0000142362741fc0c368de19"],
                "lastUpdateDate": "2017-09-26T13:23:50.927-0600",
                "groupID": "544820df0000140f6a9c1faa7cacadd3",
                "sponsorID": null,
                "description": null,
                "plannedCompletionDate": "2017-09-26T09:00:00.000-0600",
                "enteredByID": "544820df0000142362741fc0c368de19",
                "ownerID": "544820df0000142362741fc0c368de19",
                "templateID": null,
                "priority": 0,
                "companyID": null,
                "portfolioID": null,
                "referenceNumber": 1750,
                "lastUpdatedByID": "544820df0000142362741fc0c368de19",
                "customerID": "544820df0000135b7719dcca654391f6",
                "currency": null,
                "categoryID": null,
                "status": "CUR",
                "parameterValues": {}
                },
                "oldState": {}
            }
```

## Base 64 인코딩

이벤트 구독에 포함된 특수 문자와 네트워크 설정이 충돌하여 이벤트 구독이 거부되는 경우 Base64 인코딩을 사용하여 이벤트 구독을 전달할 수 있습니다. Base64는 임의의 데이터를 ASCII 문자열 형식으로 변환할 수 있는 인코딩 체계 세트입니다. Base64는 보안 암호화의 한 형태가 아니라는 점에 유의해야 합니다.

### Base 64 인코딩 필드

Base64Encoding 필드는 이벤트 구독 페이로드의 Base64 인코딩을 활성화하는 데 사용되는 선택적 필드입니다. 기본값은 false이고 가능한 값은 true, false 및 &quot; &quot;(공백)입니다.

### base64Encoding 필드를 사용하는 요청의 예

true로 설정된 base64Encoding 필드를 사용하여 요청한 경우 **newState** 및 **oldState** 페이로드의 개체는 기본 64개의 인코딩 문자열로 전달됩니다. base64Encoding 필드가 false로 설정되어 있거나, 비어 있거나, 요청에 포함되지 않은 경우, 반환된 페이로드는 base64에서 인코딩되지 않습니다.

다음은 base64Encoding 필드를 사용하는 요청의 예입니다.

<!-- [Copy](javascript:void(0);) -->

```
{
                "objCode": "PROJ",
                "eventType": "UPDATE",
                "url": "http://requestb.in/ua5hi2ua"",
                "authToken": "EauthTokenWorkfrontRocks1234_",
                "base64Encoding": "true"
            }
```

### Base 64 인코딩의 응답 페이로드 예

<!-- [Copy](javascript:void(0);) -->

```
                {
                "eventType": "UPDATE",
                "subscriptionId": "8a0d839d5ef32c9a015ef336a5ed0002",
                "eventTime": {
                "nano": 998000000,
                "epochSecond": 1507319336
                },
                "newState": "ewogICAgICAgIklEIjogIjU5ZDdkZGY3MDAwMDAyMzIyZDc5MWViMDhiYWZkZGZiIiwgCiAgICAgICAibmFtZSI6ICJFdmVudFN1YiBUZXN0IHVwZGF0ZWQiLAogICAgICAgIm9iakNvZGUiOiAiUFJPSiIsCiAgICAgICAiZW50cnlEYXRlIjogIjIwMTctMTAtMDZUMTM6NDg6MDcuNzc2LTA2MDAiLAogICAgICAgImFjY2Vzc29ySURzIjogWwogICAgICAgICAgICI1NDQ4MjBkZjAwMDAxNDIzNjI3NDFmYzBjMzY4ZGUxOSIKICAgICAgIF0sCiAgICAgICAibGFzdFVwZGF0ZURhdGUiOiAiMjAxNy0xMC0wNlQxMzo0ODo1Ni45ODAtMDYwMCIsCiAgICAgICAiZ3JvdXBJRCI6ICI1NDQ4MjBkZjAwMDAxNDBmNmE5YzFmYWE3Y2FjYWRkMyIsCiAgICAgICAic3BvbnNvcklEIjogbnVsbCwKICAgICAgICJkZXNjcmlwdGlvbiI6IG51bGwsCiAgICAgICAicGxhbm5lZENvbXBsZXRpb25EYXRlIjogIjIwMTctMTAtMDZUMDk6MDA6MDAuMDAwLTA2MDAiLAogICAgICAgImVudGVyZWRCeUlEIjogIjU0NDgyMGRmMDAwMDE0MjM2Mjc0MWZjMGMzNjhkZTE5IiwKICAgICAgICJvd25lcklEIjogIjU0NDgyMGRmMDAwMDE0MjM2Mjc0MWZjMGMzNjhkZTE5IiwKICAgICAgICJ0ZW1wbGF0ZUlEIjogbnVsbCwKICAgICAgICJwcmlvcml0eSI6IDAsCiAgICAgICAiY29tcGFueUlEIjogbnVsbCwKICAgICAgICJwb3J0Zm9saW9JRCI6IG51bGwsCiAgICAgICAicmVmZXJlbmNlTnVtYmVyIjogMTg5NCwKICAgICAgICJsYXN0VXBkYXRlZEJ5SUQiOiAiNTQ0ODIwZGYwMDAwMTQyMzYyNzQxZmMwYzM2OGRlMTkiLAogICAgICAgImN1c3RvbWVySUQiOiAiNTQ0ODIwZGYwMDAwMTM1Yjc3MTlkY2NhNjU0MzkxZjYiLAogICAgICAgImN1cnJlbmN5IjogbnVsbCwKICAgICAgICJjYXRlZ29yeUlEIjogbnVsbCwKICAgICAgICJzdGF0dXMiOiAiQ1VSIiwKICAgICAgICJwYXJhbWV0ZXJWYWx1ZXMiOiB7fQogICAgfQ==",
                "oldState": "ewogICAgICAgICJJRCI6ICI1OWQ3ZGRmNzAwMDAwMjMyMmQ3OTFlYjA4YmFmZGRmYiIsCiAgICAgICAgIm5hbWUiOiAiRXZlbnRTdWIgVGVzdCAxODBmZDU5NS02M2ZiLTRmYTktYmQ0Ny01OGJmNmU1M2Q5NjQiLAogICAgICAgICJvYmpDb2RlIjogIlBST0oiLAogICAgICAgICJlbnRyeURhdGUiOiAiMjAxNy0xMC0wNlQxMzo0ODowNy43NzYtMDYwMCIsCiAgICAgICAgImFjY2Vzc29ySURzIjogWwogICAgICAgICAgICAiNTQ0ODIwZGYwMDAwMTQyMzYyNzQxZmMwYzM2OGRlMTkiCiAgICAgICAgXSwKICAgICAgICAibGFzdFVwZGF0ZURhdGUiOiAiMjAxNy0xMC0wNlQxMzo0ODowNy43OTItMDYwMCIsCiAgICAgICAgImdyb3VwSUQiOiAiNTQ0ODIwZGYwMDAwMTQwZjZhOWMxZmFhN2NhY2FkZDMiLAogICAgICAgICJzcG9uc29ySUQiOiBudWxsLAogICAgICAgICJkZXNjcmlwdGlvbiI6IG51bGwsCiAgICAgICAgInBsYW5uZWRDb21wbGV0aW9uRGF0ZSI6ICIyMDE3LTEwLTA2VDA5OjAwOjAwLjAwMC0wNjAwIiwKICAgICAgICAiZW50ZXJlZEJ5SUQiOiAiNTQ0ODIwZGYwMDAwMTQyMzYyNzQxZmMwYzM2OGRlMTkiLAogICAgICAgICJvd25lcklEIjogIjU0NDgyMGRmMDAwMDE0MjM2Mjc0MWZjMGMzNjhkZTE5IiwKICAgICAgICAidGVtcGxhdGVJRCI6IG51bGwsCiAgICAgICAgInByaW9yaXR5IjogMCwKICAgICAgICAiY29tcGFueUlEIjogbnVsbCw8CiAgICAgICAgInBvcnRmb2xpb0lEIjogbnVsbCwKICAgICAgICAicmVmZXJlbmNlTnVtYmVyIjogMTg5NCwKICAgICAgICAibGFzdFVwZGF0ZWRCeUlEIjogIjU0NDgyMGRmMDAwMDE0MjM2Mjc0MWZjMGMzNjhkZTE5IiwKICAgICAgICAiY3VzdG9tZXJJRCI6ICI1NDQ4MjBkZjAwMDAxMzViNzcxOWRjY2E2NTQzOTFmNiIsCiAgICAgICAgImN1cnJlbmN5IjogbnVsbCwKICAgICAgICAiY2F0ZWdvcnlJRCI6IG51bGwsCiAgICAgICAgInN0YXR1cyI6ICJDVVIiLAogICAgICAgICJwYXJhbWV0ZXJWYWx1ZXMiOiB7fQogICAgfQ=="
                }
 
```

## 모든 이벤트 구독을 쿼리하기 위해 더 이상 사용되지 않는 메서드

다음 API 끝점은 더 이상 사용되지 않으며 새 구현에 사용되어서는 안 됩니다. 또한 이전 구현을 의 메서드로 전환하는 것이 좋습니다 **이벤트 구독 쿼리** 섹션에 설명되어 있습니다.

sessionID 값으로 지정된 대로 고객에 대한 모든 이벤트 구독을 쿼리할 수 있습니다. 특정 고객에 대한 모든 이벤트 구독을 나열하기 위한 요청 구문은 다음 URL입니다.

<!-- [Copy](javascript:void(0);) -->

```
GET https://<HOSTNAME>/attask/eventsubscription/api/v1/subscriptions/list
```

**요청 헤더:**

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th> <p>헤더 이름</p> </th> 
   <th> <p>헤더 값</p> </th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td> <p>sessionID</p> </td> 
   <td> <p> sessionID 값 </p> </td> 
  </tr> 
 </tbody> 
</table>

**응답 코드:**

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th> <p>응답 코드</p> </th> 
   <th> 설명</th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td>200(콘텐츠 없음)</td> 
   <td>요청에 의해 사용자에 대해 찾은 모든 이벤트 구독이 반환되었습니다.</td> 
  </tr> 
  <tr> 
   <td>401(승인되지 않음)</td> 
   <td>입력한 sessionID가 비어 있습니다.</td> 
  </tr> 
  <tr> 
   <td>403(금지됨)</td> 
   <td>제공된 sessionID와 일치하는 사용자에게 관리자 액세스 권한이 없습니다.</td> 
  </tr> 
 </tbody> 
</table>

 

### 응답 본문 예

<!-- [Copy](javascript:void(0);) -->

```
                [
                {
                "id": "37c4bcf5-e0b5-4256-aba3-a51cba7bf997",
                "customer_id": "504f9640000013401be513579fbebffa",
                "obj_id": "ObjId1234",
                "obj_code": "TASK",
                "url": "http://test.test.net/test/1234",
                "event_type": "UPDATE",
                "auth_token": "auth_token"
                },
                {
                "id": "750a636c-5628-48f5-ba26-26b7ce537ac2",
                "customer_d": "504f9640000013401be513579fbebffa",
                "obj_id": null,
                "obj_code": "PROJ",
                "url": "http://requestb.in/ua5hi2ua",
                "event_type": "UPDATE",
                "auth_token": "authTokenWorkfrontRocks1234_"
                }                
                ]
```
