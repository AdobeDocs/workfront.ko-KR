---
content-type: api
navigation-topic: general-api
title: 이벤트 구독 API
description: 이벤트 구독 API
author: Becky
feature: Workfront API
exl-id: c3646a5d-42f4-4af8-9dd0-e84977506b79
source-git-commit: f050c8b95145552c9ed67b549608c16115000606
workflow-type: tm+mt
source-wordcount: '2203'
ht-degree: 3%

---


# 이벤트 구독 API

<!--BOB clean this up-->

<!--
{{highlighted-preview}}
-->

이벤트 구독에서 지원하는 Adobe Workfront 개체에서 작업이 발생하면 원하는 종단점에 대한 응답을 보내도록 Workfront을 구성할 수 있습니다. 즉, 타사 애플리케이션은 Workfront API를 통해 Workfront 상호 작용에서 업데이트 사항이 발생한 직후 업데이트를 받을 수 있습니다. 일반적으로 데이터 변경 사항이 기록되면 5초 이내에 웹 후크 알림을 받을 수 있습니다. 평균적으로, 고객은 기록되는 데이터 변경 후 1초 이내에 웹 후크 알림을 받게 됩니다.  

방화벽을 통해 이벤트 구독 페이로드를 수신하려면 다음 IP 주소를에 추가해야 허용 목록에 추가하다 합니다.

**유럽 고객의 경우:**

* 52.30.133.50
* 52.208.159.124
* 54.220.93.204
* 52.17.130.201
* 34.254.76.122
* 34.252.250.191

**유럽 이외의 지역에 있는 고객의 경우:**

* 54.244.142.219
* 44.241.82.96
* 52.36.154.34
* 34.211.224.9
* 54.218.48.56
* 52.39.217.230

다음 항목은 이벤트 구독 API를 지원합니다.

## 이벤트 구독에서 지원하는 개체

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

이벤트 구독 개체에서 지원하는 필드 목록은 [이벤트 구독 리소스 필드](../../wf-api/api/event-sub-resource-fields.md).

## 이벤트 구독 인증

이벤트 가입을 생성, 쿼리 또는 삭제하려면 Workfront 사용자에게 다음 항목이 필요합니다.

* &quot;시스템 관리자&quot;의 액세스 수준
* apiKey

   >[!NOTE]
   >
   >사용자가 이미 Workfront의 API를 사용하고 있는 경우 사용자에게 이미 apiKey가 있어야 합니다. 다음 HTTP 요청을 통해 apiKey를 검색할 수 있습니다.

**요청 URL:**

```
PUT https://<HOSTNAME>/attask/api/v15.0/USER?action=getApiKey&username=<USERNAME>&password=<PASSWORD>
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
   <td> <p>컨텐츠 유형</p> </td> 
   <td> <p>텍스트/html</p> </td> 
  </tr> 
 </tbody> 
</table>

**응답 코드:**

| 응답 코드 | 설명 |
|---|---|
| 200 (확인) | 요청이 성공적으로 처리되었으며 사용자에 대한 기존 apiKey가 응답 본문에 반환되어야 합니다. |
| 401(허가되지 않음) | 서버는 요청을 승인하지만 요청 apiKey/사용자에게 이 요청을 수행할 수 있는 액세스 권한이 없으므로 요청을 처리할 수 없습니다. |

{style=&quot;table-layout:auto&quot;}

**응답 본문 예:**

```
{
               "data"{
               "result": "rekxqndrw9783j4v79yhdsakl56bu1jn"
               }
      }
```

>[!NOTE]
>
> Workfront API를 처음 사용하는 경우 이 링크를 통해 수행할 수 있는 apiKey를 생성해야 합니다.


```
PUT https://<HOSTNAME>/attask/api/v15.0/USER/generateApiKey?username=<USERNAME>&password=<PASSWORD>
```

## 구독 리소스 구성

구독 리소스에는 다음 필드가 포함되어 있습니다.

* objId(선택 사항)

   * **문자열** - 이벤트가 실행되는 지정된 objCode의 개체 ID입니다. 이 필드를 지정하지 않으면 지정된 유형의 모든 객체에 대한 이벤트를 수신합니다.

* objCode(필수)

   * **문자열** - 변경 내용을 구독하는 개체의 objCode입니다. objCode에 사용할 수 있는 값은 아래 표에 나와 있습니다.

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
        <td scope="col"><p>ASGN</p></td> 
       </tr> 
       <tr> 
        <td scope="col">회사 </td> 
        <td scope="col"><p>CMPY</p></td> 
       </tr> 
       <tr> 
        <td scope="col">대시보드</td> 
        <td scope="col">PTLTAB</td> 
       </tr> 
       <tr> 
        <td scope="col"><p>문서</p></td> 
        <td scope="col">DOCU </td> 
       </tr> 
       <tr> 
        <td scope="col"><p>경비</p></td> 
        <td scope="col">EXPNS</td> 
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
        <td scope="col"><p>PROJ</p></td> 
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
        <td scope="col"><p>TMPL</p></td> 
       </tr> 
       <tr> 
        <td scope="col">타임시트</td> 
        <td scope="col">TSHET</td> 
       </tr> 
       <tr> 
        <td scope="col">사용자</td> 
        <td scope="col">사용자</td> 
       </tr> 
      </tbody> 
     </table>

* eventType(필수)

   * **문자열** - 개체를 구독한 이벤트 유형을 나타내는 값입니다. 사용 가능한 이벤트 유형은 다음과 같습니다.

      * 만들기
      * DELETE 
      * 업데이트

* url(필수)

   * **문자열** - HTTP를 통해 구독 이벤트 페이로드를 전송하는 끝점의 URL입니다.

* authToken(필수)

   * **문자열** - &quot;URL&quot; 필드에 지정된 URL로 인증하는 데 사용되는 OAuth2 베어러 토큰입니다. 

## 이벤트 구독 API 요청 만들기

사용자에게 관리자 액세스 권한이 있고 구독 리소스를 구성한 후 이벤트 구독을 만들 준비가 되었습니다.

다음 구문을 사용하여 URL을 구성합니다.

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
   <td> <p>컨텐츠 유형</p> </td> 
   <td> <p>application/json</p> </td> 
  </tr> 
  <tr> 
   <td> <p>인증</p> </td> 
   <td> <p>apiKey 값</p> </td> 
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
| 201(생성됨) | 이벤트 구독을 만들었습니다. |
| 400(잘못된 요청) | 구독 리소스의 URL 필드가 잘못된 것으로 간주됩니다. |
| 401(허가되지 않음) | 제공된 apiKey가 비어 있거나 잘못된 것으로 간주되었습니다. |
| 403 (금지됨) | 제공된 apiKey와 일치하는 사용자에게는 관리자 액세스 권한이 없습니다. |

구독 리소스를 요청의 본문(콘텐츠 유형은 &quot;application/json&quot;인 경우)으로 전달하면 지정된 개체에 대해 이벤트 구독이 생성됩니다. 응답 코드 201(작성됨)은 구독이 만들어졌음을 나타냅니다. 201 이외의 응답 코드는 구독이 **NOT** 생성되었습니다.

>[!NOTE]
 위치 응답 헤더에는 새로 만든 이벤트 구독의 URI가 포함되어 있습니다.

**응답 헤더 예:**

| 응답 헤더 | 예 |
|---|---|
| Content-Length | `→0` |
| 일자 | `→Wed, 05 Apr 2017 21:23:33 GMT` |
| 위치 | `→https://<HOSTNAME>/attask/eventsubscription/api/v1/subscriptions/750a636c-5628-48f5-ba26-26b7ce537ac2` |
| 서버 | `→Apache-Coyote/1.1` |

## 이벤트 구독 쿼리

Workfront의 HTTP를 쿼리할 때 GET 메서드를 사용하십시오. 이벤트 구독을 쿼리하는 방법에는 두 가지가 있습니다. 구독 ID로 쿼리하거나(아래 참조), 모든 이벤트 가입을 쿼리합니다.

### 모든 이벤트 구독 쿼리

apiKey 값으로 지정한 대로 고객에 대한 모든 이벤트 구독을 쿼리할 수 있습니다. 다음 옵션을 사용하여 응답을 관리할 수도 있습니다.

* **페이지**: 쿼리 매개 변수 옵션을 사용하여 반환할 페이지 수를 지정합니다. 기본값은 1입니다.
* **제한**: 쿼리 매개 변수 선택 사항을 사용하여 페이지당 반환할 결과 수를 지정합니다. 기본값은 100이며, 최대 1000입니다.

특정 고객에 대한 모든 이벤트 가입을 나열하는 요청 구문은 다음과 같습니다.

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
   <td> <p>인증</p> </td> 
   <td> <p>apiKey 값</p> </td> 
  </tr> 
 </tbody> 
</table>

**응답 코드:**

| 응답 코드 | 설명 |
|---|---|
| 200 (확인) | 제공된 apiKey와 일치하는 고객에 대해 검색된 모든 이벤트 구독과 함께 요청이 반환되었습니다. |
| 401(허가되지 않음) | 제공된 apiKey가 비어 있습니다. |
| 403 (금지됨) | 제공된 apiKey와 일치하는 사용자에게는 관리자 액세스 권한이 없습니다. |


**응답 헤더 예:**

| 응답 헤더 | 예 |
|---|---|
| 컨텐츠 유형 | `→application/json;charset=UTF-8` |
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

* **페이지** 및 **제한** 는 요청에 제공된 값이거나 값이 제공되지 않을 경우 기본값입니다
* **page_count** 은 쿼리할 수 있는 총 페이지 수입니다.
* **total_count** 은 쿼리와 일치하는 총 구독 수입니다.

### 이벤트 구독 ID로 쿼리

이벤트 구독의 ID로 이벤트 구독을 쿼리할 수 있습니다. 이벤트 구독을 나열하는 요청 구문은 다음과 같습니다.

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
   <td> <p>인증</p> </td> 
   <td> <p>apiKey 값</p> </td> 
  </tr> 
 </tbody> 
</table>

**응답 코드:**

| 응답 코드 | 설명 |
|---|---|
| 200 (확인) | 제공된 구독 ID와 일치하는 이벤트 구독과 함께 반환된 요청입니다. |
| 401(허가되지 않음) | 제공된 apiKey가 비어 있습니다. |
| 403 (금지됨) | 제공된 apiKey와 일치하는 사용자에게는 관리자 액세스 권한이 없습니다. |


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

이벤트 구독 필터링을 사용하여 관련 메시지만 수신할 수 있습니다. 가입에 대한 필터를 만들면 종단점에서 사용해야 하는 메시지 수가 크게 줄어들 수 있습니다.

예: **업데이트 - 작업** 이벤트 구독은 **newState** 이벤트 페이로드의 값은 **taskStatus** 로서의 **현재**.

>[!IMPORTANT]
다음 속성은 이벤트 구독 필터링에 적용됩니다

* 필터 필드에 비어 있지 않은 값이 있는 경우 **newState** 필터 키 및 값이 포함된 경우 구독한 URL로 전송됩니다
* 에 포함된 사용자 지정 데이터로 필터링할 수 있습니다. **newState** 및/또는 **oldState**&#x200B;개체
* 필터는 특정 값과 같은지 여부에 대해서만 평가됩니다
* 필터 구문이 잘못되었거나 에 포함된 데이터와 일치하지 않는 경우 **newState** 페이로드 중 오류가 발생했음을 나타내는 유효성 검사 메시지가 반환되지 않습니다
* 현재 존재하는 구독에서 필터를 업데이트할 수 없습니다. 새 필터 매개 변수를 사용하여 새 구독을 만들어야 합니다.
* 여러 필터를 단일 구독에 적용할 수 있으며 구독은 모든 필터 조건이 충족된 경우에만 전달됩니다.
* 단일 구독에 여러 필터를 적용하는 것은 **및** 논리 연산자입니다.
* 각 이벤트 구독 간에 하나 이상의 이벤트 구독 필드 매개 변수가 다른 한 단일 개체에 여러 이벤트 구독을 적용할 수 있습니다.
* 여러 이벤트 구독을 단일 개체에 지정하면 해당 개체와 연결된 모든 이벤트 구독을 단일 종단점으로 반환할 수 있습니다. 이 방법은 논리 연산자의 동등한 대용으로 사용할 수 있습니다 **또는** 필터 매개 변수를 사용하여 설정할 수 없습니다.

### 비교 연산자 사용

필터 필드와 함께 비교 필드를 지정할 수 있습니다. 비교 결과를 필터링하려면 이 필드의 비교 연산자를 사용하십시오. 예를 들어 작업 상태가 최신 상태가 아닌 경우에만 페이로드를 전송하는 UPDATE - TASK 가입을 만들 수 있습니다. 다음 비교 연산자를 사용할 수 있습니다.

#### eq: equal

이 필터를 사용하면 발생한 변경 내용이 일치하는 경우 메시지를 보낼 수 있습니다 `fieldValue` 에 있는 것을 의미합니다. 다음 `fieldValue` 값은 대/소문자를 구분합니다.

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

이 필터를 사용하면 발생한 변경 내용이 일치하지 않는 경우 메시지를 보낼 수 있습니다 `fieldValue` 에 있는 것을 의미합니다. 다음 `fieldValue` 값은 대/소문자를 구분합니다.

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

이 필터를 사용하면 지정된 `fieldName` 다음보다 큼 `fieldValue`.

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

#### gte: 크거나 같음

이 필터를 사용하면 지정된 `fieldName` 다음보다 크거나 같음 `fieldValue`.

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

이 필터를 사용하면 지정된 `fieldName` 의 값보다 작습니다. `fieldValue`.

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

#### lte: 작거나 같음

이 필터를 사용하면 지정된 `fieldName` 다음보다 작거나 같음 `fieldValue`.

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

이 필터를 사용하면 발생한 변경 사항에 `fieldValue` 아래에 표시됩니다. 다음 `fieldValue` 값은 대/소문자를 구분합니다

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

이 필터를 사용하면 지정된 필드(`fieldName`)의 값은 이전 상태와 새 상태에서 다릅니다. 지정한 필드 외에 다른 필드를 업데이트하는 중(`fieldName`)은 해당 변경 사항을 반환하지 않습니다.

>[!NOTE]
`fieldValue` 아래의 filters 배열에는 영향을 주지 않습니다.

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

#### state

이 커넥터를 사용하면 필터를 만들거나 업데이트한 개체의 새 상태나 이전 상태에 적용합니다. 이 기능은 어떤 항목에서 다른 항목으로 변경된 위치를 알고 싶을 때 유용합니다.
`oldState` CREATE에서는 사용할 수 없습니다 `eventTypes`.

>[!NOTE]
지정된 필터가 있는 아래 구독은 작업 이름에 포함된 메시지만 반환합니다 `again` on `oldState`: 작업에 대한 업데이트가 수행되기 전이었습니다.
이 경우 한 메시지에서 다른 메시지로 변경된 objCode 메시지를 찾습니다. 예를 들어, &quot;Research Some name&quot;에서 &quot;Research TeamName Some name&quot;으로 변경된 모든 작업을 확인할 수 있습니다

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

다음 `filterConnector` 구독 페이로드 필드를 사용하면 필터를 적용하는 방법을 선택할 수 있습니다. 기본값은 &quot;AND&quot;이며, 여기서 필터는 모두 여야 합니다 `true` 구독 메시지가 수신됩니다. &quot;OR&quot;를 지정하는 경우 구독 메시지가 수신되려면 하나의 필터만 일치해야 합니다.

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

Workfront의 HTTP를 삭제할 때 DELETE 방법을 사용하십시오. 구독 ID별로 단일 이벤트 구독을 삭제하는 요청 구문은 다음과 같습니다.

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
   <td> <p>인증</p> </td> 
   <td> <p> 사용자의 apiKey </p> </td> 
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
   <td>200(컨텐츠 없음)</td> 
   <td>서버가 제공된 subscriptionID와 일치하는 이벤트 구독을 제거했습니다.</td> 
  </tr> 
  <tr> 
   <td>401(허가되지 않음)</td> 
   <td>제공된 apiKey가 비어 있습니다.</td> 
  </tr> 
  <tr> 
   <td>403 (금지됨)</td> 
   <td>제공된 apiKey와 일치하는 사용자에게 관리자 액세스 권한이 없습니다.</td> 
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


**응답 본문 예:** 해당 없음

## 이벤트 페이로드의 예

사용자가 받는 페이로드는 객체 유형에 따라 달라지지만, 이러한 다양한 페이로드가 전달되는 일관된 형식이 있습니다.

예를 들어, 다음 속성은 모든 이벤트 페이로드에서 일관되게 유지됩니다.

* eventType
* subscriptionId
* oldState
* newState
* eventTime

형식에서는 일관적이긴 하지만 속성 내에 포함된 값은 서로 다른 객체와 객체 유형 간에 다릅니다.

UPDATE 이벤트 및 CREATE 이벤트에 대한 페이로드 샘플이 아래에 표시되어 있습니다. 업데이트 예제에서 oldState 및 newState 개체는 동일하지만, CREATE 예제에서 oldState 개체는 비어 있습니다(NULL 아님).

다음은 UPDATE 이벤트의 페이로드 예입니다.

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

다음은 CREATE 이벤트에 대한 페이로드 예입니다.

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

## 기본 64 인코딩

이벤트 구독과 네트워크 설정에 포함된 특수 문자 간의 충돌로 인해 이벤트 구독이 거부되는 경우 Base64 인코딩을 사용하여 이벤트 구독을 전달할 수 있습니다. Base64는 임의의 데이터를 ASCII 문자열 형식으로 변환할 수 있는 인코딩 구성표 세트입니다. Base64는 보안 암호화 형식이 아닙니다.

### 기본 64 인코딩 필드

base64Encoding 필드는 이벤트 구독 페이로드의 Base64 인코딩을 활성화하는 데 사용되는 선택적 필드입니다. 기본값은 false이며, 가능한 값은 다음과 같습니다. true, false 및 &quot; &quot;(비어 있음).

### base64Encoding 필드를 사용하는 요청의 예

base64Encoding 필드를 true로 설정하여 요청을 수행하면 **newState** 및 **oldState** 페이로드의 개체는 기본 64 인코딩 문자열로 전달됩니다. base64Encoding 필드가 false로 설정되어 있거나, 비워 두거나, 요청에 포함되지 않은 경우, 반환된 페이로드가 base 64에서 인코딩되지 않습니다.

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

### 기본 64 인코딩의 응답 페이로드 예

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

## 모든 이벤트 구독을 쿼리하기 위해 사용되지 않는 메서드

다음 API 엔드포인트는 더 이상 사용되지 않으며, 새 구현에 사용해서는 안 됩니다. 이전 구현을 의 메서드로 전환하는 것이 좋습니다 **이벤트 구독 쿼리** 섹션에 자세히 설명되어 있습니다.

apiKey 값으로 지정한 대로 고객에 대한 모든 이벤트 구독을 쿼리할 수 있습니다. 특정 고객에 대한 모든 이벤트 구독을 나열하는 요청 구문은 다음 URL입니다.

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
   <td> <p>인증</p> </td> 
   <td> <p> 사용자의 apiKey </p> </td> 
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
   <td>200(컨텐츠 없음)</td> 
   <td>요청에 따라 사용자에 대한 모든 이벤트 구독이 반환되었습니다.</td> 
  </tr> 
  <tr> 
   <td>401(허가되지 않음)</td> 
   <td>제공된 apiKey가 비어 있습니다.</td> 
  </tr> 
  <tr> 
   <td>403 (금지됨)</td> 
   <td>제공된 apiKey와 일치하는 사용자에게 관리자 액세스 권한이 없습니다.</td> 
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
