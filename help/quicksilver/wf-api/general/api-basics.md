---
content-type: api
navigation-topic: general-api
title: API 기본 사항
description: API 기본 사항
author: John
feature: Workfront API
exl-id: d8c27915-8e1b-4804-9ef8-3a2efd57caac
source-git-commit: c1cec2c08c66c704385cde1abd0c019fd59702da
workflow-type: tm+mt
source-wordcount: '4405'
ht-degree: 0%

---


# API 기본 사항

Adobe Workfront API의 목표는 HTTP를 통해 작동하는 REST ful 아키텍처를 도입하여 Workfront와의 통합 구축을 간소화하는 것입니다. 이 문서에서는 사용자가 REST 및 JSON 응답을 잘 알고 있다고 가정하고 Workfront API에서 적용하는 접근 방식을 설명합니다.

Workfront 스키마에 대한 친숙성은 통합을 위해 Workfront에서 데이터를 가져오는 데 사용할 수 있는 데이터베이스 관계를 이해하는 데 도움이 됩니다.

## 제한 및 지침

일관된 Workfront 온디맨드 시스템 성능을 보장하기 위해 각 고객은 10개의 동시 API 스레드로 제한됩니다. 샌드박스 환경에도 동일한 제한이 있으므로 고객 및 파트너가 코드를 프로덕션에 릴리스하기 전에 API 호출을 정확하게 테스트할 수 있습니다.

프로덕션, 미리 보기 및 테스트 드라이브 환경의 경우 최종 사용자 요청은 Workfront CDN(Akamai)을 통해 라우팅되기 때문에 최대 URI 길이가 8892바이트입니다. 이 제한은 CDN을 통해 라우팅되는 URI에만 적용됩니다.

>[!NOTE]
>
>이 제한은 샌드박스 환경이 CDN을 통해 라우팅되지 않으므로 샌드박스 환경에 적용할 수 없습니다.

### 면책조항

API의 모든 사용은 프로덕션 환경에서 실행하기 전에 Workfront 베타 환경에서 테스트해야 합니다. 고객이 Workfront에서 온디맨드 소프트웨어에 부담이 된다고 합리적으로 생각하는 프로세스에 API를 사용하는 경우(즉, 프로세스가 다른 고객에 대한 소프트웨어 성능에 실질적 부정적인 영향을 미치는 경우) Workfront은 고객이 해당 프로세스를 중단하도록 요청할 수 있는 권한을 갖습니다. 고객이 동의하지 않고 문제가 계속 발생하면 Workfront은 프로세스를 종료할 권한을 갖습니다.

## REST 기본 사항

이 섹션에서는 다음 REST 원칙을 위해 Workfront REST API와 상호 작용하는 방법에 대한 높은 수준의 개요를 제공합니다.

### 개체 URI

시스템의 각 객체에는 객체 유형과 ID로 구성된 고유한 URI가 제공됩니다. 다음 예제에서는 세 가지 고유한 개체를 설명하는 URI를 보여 줍니다.

```
/attask/api/v15.0/project/4c78821c0000d6fa8d5e52f07a1d54d0
/attask/api/v15.0/task/4c78821c0000d6fa8d5e52f07a1d54d1
/attask/api/v15.0/issue/4c78821c0000d6fa8d5e52f07a1d54d2
```

개체 유형은 대/소문자를 구분하지 않으며 약식 ObjCode(예: proj) 또는 대체 개체 이름(프로젝트)일 수 있습니다.

유효한 ObjCodes 목록에 대해서는  [API 탐색기](../../wf-api/general/api-explorer.md).

### 작업

개체는 고유한 URI로 HTTP 요청을 보내어 조작됩니다. 수행할 작업은 HTTP 메서드에서 지정합니다.

표준 HTTP 메서드는 다음 작업에 해당합니다.

* **GET** - ID로 개체를 검색하거나, 쿼리를 통해 모든 개체를 검색하거나, 보고서를 실행하거나, 명명된 쿼리를 실행합니다
* **POST** - 새 개체를 삽입합니다.
* **PUT** - 기존 개체 편집
* **DELETE** - 개체 삭제

클라이언트 부족 또는 프로토콜 길이 제한을 해결하기 위해 메서드 매개 변수를 사용하여 HTTP 동작을 무시할 수 있습니다. 예를 들어 다음 URI를 게시하여 GET 작업을 구현할 수 있습니다.
<pre>GET /attask/api/v15.0/project?id=4c78...54d0&amp;method=get<br>GET /attask/api/v15.0/project/4c78...54d0?method=get</pre>

### 응답

각 요청에는 JSON 형식으로 응답이 제공됩니다. 요청에 성공한 경우 응답에 데이터 속성이 있고 문제가 있는 경우 오류 속성이 있습니다. 예를 들어, 요청

```
GET /attask/api/v15.0/proj/4c7c08b20000002de5ca1ebc19edf2d5
```

는 다음과 유사한 JSON 응답을 반환합니다.


<pre>{<br>    "data": [<br>        {<br>            "percentComplete": 0,<br>            "status": "CUR",<br>            "priority": 2,<br>            "name": "Brand New Project",<br>            "ID": "4c7c08b20000002de5ca1ebc19edf2d5" <br>        } <br>    ] <br>}</pre>

>[!NOTE]
>
>브라우저의 주소 표시줄을 통해 GET 요청을 실행할 때 요청의 일부로 sessionID를 포함할 필요가 없습니다.

PUT, POST 및 DELETE 요청에 대한 특수 보안이 추가되었습니다. 데이터베이스에 쓰거나 데이터베이스에서 삭제하는 모든 요청은 **sessionID=abc123** 는 URI에 포함됩니다. 다음 예는 이 방법이 DELETE 요청을 찾는 방법을 보여줍니다.
<pre>GET /attask/api/v15.0/project?id=4c78...54d0&amp;method=delete&amp;sessionID=abc123<br>GET /attask/api/v15.0/project/4c78..54d0?method=delete&amp;sessionID=abc123</pre>

### 인증

API는 클라이언트가 요청한 개체를 보거나 수정할 수 있는 액세스 권한이 있는지 확인하기 위해 각 요청을 인증합니다.

인증은 다음 방법 중 하나를 사용하여 제공할 수 있는 세션 ID를 전달하여 수행됩니다.

#### 요청 헤더 인증

인증의 기본 방법은 세션 토큰이 포함된 SessionID라는 요청 헤더를 전달하는 것입니다. 이것은 안전하다는 장점이 있다 [CSRF(사이트 간 요청 위조)](http://en.wikipedia.org/wiki/Cross-site_request_forgery) 캐싱을 위해 URI를 간섭하지 않고 공격을 수행합니다.

다음은 요청 헤더의 예입니다.

```
GET /attask/api/v15.0/project/search
SessionID: abc1234
```

#### 요청 매개 변수 인증

다음 예와 같이 sessionID라는 요청 매개 변수를 전달하여 인증할 수 있습니다. 

```
GET /attask/api/v15.0/project/4c78821c0000d6fa8d5e52f07a1d54d0?sessionID=abc1234
```

#### 쿠키 기반 인증

API는 웹 UI에서 시스템에 사용하는 동일한 쿠키 기반 인증을 사용합니다. 여기서, 클라이언트가 웹 UI를 사용하여 Workfront에 로그인하는 경우 동일한 브라우저 내에서 수행된 모든 AJAX 호출은 동일한 인증을 사용합니다.

>[!NOTE]
>
>CSRF(Cross Site Request Forgery) 공격 가능성을 방지하기 위해 이 인증 방법은 읽기 전용 작업에서만 사용할 수 있습니다.

## 로그인

>[!IMPORTANT]
Workfront에서는 더 이상 `/login` endpoint 또는 API 키 대신 다음 인증 방법 중 하나를 사용하십시오.
* JWT를 사용한 서버 인증
* OAuth2를 사용한 사용자 인증
>
이러한 인증 방법 설정에 대한 지침은 [Workfront 통합을 위한 OAuth2 애플리케이션 만들기](../../administration-and-setup/configure-integrations/create-oauth-application.md)
Workfront에서 서버 인증을 사용하는 방법에 대한 지침은 [JWT 흐름을 사용하여 조직의 사용자 지정 OAuth 2 애플리케이션을 구성하고 사용합니다](../../wf-api/api/oauth-app-jwt-flow.md)
Workfront에서 사용자 인증을 사용하는 방법에 대한 지침은 [인증 코드 흐름을 사용하여 조직의 사용자 지정 OAuth 2 애플리케이션을 구성하고 사용합니다](../../wf-api/api/oauth-app-code-token-flow.md)

>[!NOTE]
이 섹션에 설명된 절차는 Adobe 비즈니스 플랫폼에 아직 온보딩되지 않은 조직에만 적용됩니다. 조직이 Adobe 비즈니스 플랫폼에 온보딩된 경우 Workfront API를 통해 Workfront에 로그인할 수 없습니다.
조직에서 Adobe 비즈니스 플랫폼에 온보딩되었는지 여부에 따라 다른 절차 목록은 [플랫폼 기반의 관리 차이점(Adobe Workfront/Adobe Business Platform)](../../administration-and-setup/get-started-wf-administration/actions-in-admin-console.md).

유효한 사용자 이름과 암호를 사용하여 다음 요청을 사용하여 세션 ID를 얻을 수 있습니다.

```
POST /attask/api/v15.0/login?username=admin&password=user
```

이 설정은 향후 요청을 인증하는 쿠키를 설정하고 새로 생성된 sessionID, 로그인한 사용자의 userID 및 기타 세션 속성으로 JSON 응답을 반환합니다.

>[!NOTE]
관리자이기도 한 지정된 API 사용자가 있는 경우 Workfront에서는 API 키를 사용하여 로그인할 것을 권장합니다.

**API 키 생성**

다음 예와 같이 해당 사용자로 시스템에 로그인할 때 API 키를 생성할 수 있습니다.


```
PUT /attask/api/v15.0/user?action=generateApiKey&username= username&password=password&method=put
```

**이전에 생성한 API 키 검색**

getApiKey를 실행하여 특정 사용자에 대해 이전에 생성된 API 키를 검색할 수도 있습니다.


```
PUT /attask/api/v15.0/user?action=getApiKey&username=user@email.com&password=userspassword&method=put
```

그런 다음 이 결과를 사용하여 sessionID 또는 사용자 이름 및 암호 대신 이 값을 사용하는 요청 매개 변수로 &quot;apiKey&quot;를 추가하여 모든 API 호출을 인증할 수 있습니다. 이는 안보적 차원에서 볼 수 있다.

다음 요청은 apiKey를 사용하여 프로젝트에서 데이터를 검색하는 예입니다.

```
GET /attask/api/v15.0/project/abc123xxxxx?apiKey=123abcxxxxxxxxx
```

**API 키 무효화**

apiKey 값이 손상된 경우 다음 예와 같이 현재 API 키를 무효화하는 &quot;clearApiKey&quot;를 실행할 수 있습니다.

```
GET /attask/api/v15.0/user?action=clearApiKey&username=user@email.com&password=userspassword&method=put
```

선택을 취소하면 getApiKey를 다시 실행하여 새 API 키를 생성할 수 있습니다.

### 로그아웃

세션이 완료되면 다음 요청을 사용하여 사용자를 로그아웃하여 sessionID로 더 이상 액세스할 수 없습니다.

```
GET /attask/api/v15.0/logout?sessionID=abc1234
```

로그아웃할 sessionID는 쿠키, 요청 헤더 또는 요청 매개 변수로 지정할 수 있습니다.

사용자를 로그아웃하려면

1. 로그인 화면으로 이동하지만 로그인하지 마십시오.
1. URL을 /attask/api/v15.0/project/search 로 변경합니다.\
   페이지를 찾을 수 없습니다.
1. 단어 바꾸기 *검색* 로그인?username=admin&amp;password=user, 사용자 이름 및 암호 바꾸기 *관리* 및 *사용자\
   *이 세션은 브라우저에 쿠키로 저장되며, 이후 각 GET 요청에서 다시 지정할 필요가 없습니다.

1. URL을 다시 **/attask/api/v15.0/project/search**.
1. 제공된 응답을 확인합니다.

PUT, POST 및 DELETE 요청을 수행할 때는 항상 로그인 후 제공된 sessionID를 포함해야 합니다.

## GET 동작

HTTP GET 메서드를 사용하여 개체나 여러 개체를 검색하고 보고서를 실행합니다.

### 개체 검색

수정자 및 필터를 사용하여 객체에 대한 검색을 향상시킬 수 있습니다.

#### 개체 ID를 사용하여 개체 검색

개체의 ID를 알고 있는 경우 해당 고유 URI에 액세스하여 개체를 검색할 수 있습니다. 예를 들어, 요청

```
GET /attask/api/v15.0/project/4c78821c0000d6fa8d5e52f07a1d54d0
```

다음과 유사한 응답을 반환합니다.

<pre>{<br>    "percentComplete": 0,<br>    "status": "CUR",<br>    "priority": 2,<br>    "name": "Brand New Project",<br>    "ID": "4c7c08b20000002de5ca1ebc19edf2d5" <br>}</pre>


다음 예와 같이 id 요청 매개 변수를 지정하고 쉼표로 구분된 ID 목록을 지정하여 동일한 요청에서 여러 개체를 검색할 수 있습니다.


```
GET /attask/api/v15.0/project?id=4c78...54d0,4c78...54d1
```

/attask/api/v15.0/project?id=.. 요청은 와 동일합니다 `/attask/api/v15.0/project/...` 요청.

#### URI를 사용하여 개체 검색

ID 이외의 기준으로 객체를 검색하려면 URI를 검색할 수 있습니다.

예를 들어 다음 요청을 사용하여 시스템의 모든 프로젝트 목록을 반환할 수 있습니다.

```
GET /attask/api/v15.0/project/search
```

요청 매개 변수를 이름-값 쌍으로 사용하여 필터를 지정할 수 있습니다. 예를 들어 다음 예제는 현재 프로젝트를 모두 찾는 요청을 보여줍니다.

```
GET /attask/api/v15.0/project/search?status=CUR
```

다음 요청은 아직 완료되지 않고 John이라는 사용자에게 할당된 모든 작업을 찾습니다.

```
GET /attask/api/v15.0/task/search?percentComplete=100
&percentComplete_Mod=lt &assignedTo:firstName=John
```

#### 검색 수정자 사용

다음 표에는 Workfront API와 함께 사용할 수 있는 몇 가지 수정자가 나와 있습니다.

| **한정자** | **설명** | **예** |
|---|---|---|
| eq | 닫힌 상태의 결과 반환 | <pre>...status=cls&amp;status_Mod=eq...</pre> |
| ne | 닫힌 상태가 아닌 결과를 반환합니다. | <pre>...status=cls&amp;status_Mod=ne...</pre> |
| gte | 완료율이 50보다 크거나 같은 결과 반환 | <pre>...percentComplete=50&amp;percentComplete_Mod=gte..</pre> |
| lte | 완료율이 50보다 작거나 같은 결과 반환 | <pre>...percentComplete=50&amp;percentComplete_Mod=lte..</pre> |
| isnull | 설명이 Null인 결과 반환 | <pre>...description_Mod=isnull..</pre> |
| null | 설명이 Null이 아닌 결과를 반환합니다. | <pre>...description_Mod=nonull..</pre> |
| 포함 | 이름에 &quot;Workfront&quot;이 포함된 결과를 반환합니다. | <pre>...name=Workfront&amp;name_Mod=contains..</pre> |
| 사이 | 최근 7일 내에 시작 날짜가 있는 결과 반환 | <pre>...entryDate=$$TODAY-7d&amp;entryDate_Range=$$TODAY&amp;entryDate_Mod=between..</pre> |

{style=&quot;table-layout:auto&quot;}

>[!NOTE]
검색 요청은 대/소문자를 구분합니다. 오류가 표시된다면  **_Mod** 및 **범위(_R)** 대문자가 올바르게 되어 있습니다.

#### OR 문 사용

필터 또는 일련의 필터의 수준을 나타내는 숫자와 &quot;OR&quot;를 포함하는 매개 변수를 추가하여 검색을 향상시킬 수 있습니다.

OR 문은 OR 문의 필터링 기준을 충족하는 API 호출의 레코드만 반환합니다. 필터는 OR 문 수준에서 암시되지 않습니다.

예를 들어

* 이름이 &quot;Planning&quot; OR인 작업
* &quot;FixedAssets&quot;라는 포트폴리오의 작업 및 &quot;Steve&quot; OR가 포함된 이름을 가진 사람에게 할당됩니다
* &quot;최종 작업&quot;이라는 상위 작업이 있는 작업

그런 다음 여러 OR 문과 함께 다음 API 호출을 사용하십시오.
<pre>GET /attask/api/v15.0/task/search?name=Planning<br>&amp;name_Mod=contains<br>또는(&amp;O):1:portfolio:name=FixedAssets<br>또는(&amp;O):1:portfolio:name_Mod=eq<br>또는(&amp;O):1:assignedTo:name=Steve<br>또는(&amp;O):1:assignedTo:name_Mod=ciconcontains<br>또는(&amp;O):2:parent:name=Final Task<br>또는(&amp;O):2:parent:name_Mod=eq
</pre>

#### 필터 매개 변수 사용

검색 필터에 URL 매개 변수를 사용할 때 발생할 수 있는 한 가지 문제는 Workfront이 다른 인증 방법(예: 사용자 이름, 암호, apiKey, 쿠키)을 확인하기 전에 특정 매개 변수를 구문 분석한다는 것입니다. 이런 경우 매개 변수는 호출에서 필터로 사용되지 않습니다. 

이 문제를 방지하기 위해 이러한 값을 JSON 형식이 있는 필터 매개 변수에 배치할 수 있습니다. 예를 들어, 사용자 이름 testuser를 사용하지 않고 필터링하려면 
<pre>/attask/api/v15.0/user/search?username=testuser@workfront.com</pre>다음 예와 같이 필터에 URL 매개 변수를 전달합니다.
<pre>/attask/api/v15.0/user/search?filters={"username":"testuser@workfront.com"}</pre>

#### 맵 요청 매개 변수 사용

기본적으로 검색에서 반환된 데이터는 JSON 배열입니다. 사용 사례에 따라 ID로 인덱싱된 JSON 개체로서 결과를 가져오는 것이 더 효율적일 수 있습니다. 이 작업은 맵 요청 매개 변수를 사용하여 수행할 수 있습니다. 예를 들어, 요청 
<pre>/attask/api/v15.0/task/search?map=true</pre>다음과 유사한 ID로 인덱싱된 응답을 반환합니다.
<pre>{<br>    "data": {<br>        "4c9a97db0000000f13ee4446b9aead9b": {<br>            "percentComplete": 0,<br>            "status": "새로운",<br>            "name": "첫 번째 작업",<br>            "ID": "4c9a97db0000000f13ee4446b9aead9b",<br>            "taskNumber": 1 <br>        },<br>        "4ca28ba600002024cd49e75bd43cf601": {<br>            "percentComplete": 0,<br>            "status": "INP:A",<br>            "name": "두 번째 작업",<br>            "ID": "4ca28ba600002024cd49e75bd43cf601",<br>            "taskNumber": 2개 <br>        } <br>    } <br>}</pre>

#### 필드 요청 매개 변수 사용

기본적으로 개체 검색은 가장 일반적으로 사용되는 필드의 하위 집합만 반환합니다.

필드 요청 매개 변수를 사용하여 쉼표로 구분된 특정 필드 목록이 반환되도록 지정할 수 있습니다. 예를 들어, 요청
<pre>/attask/api/v15.0/task/search?fields=planningStartDate,priority</pre>다음과 유사한 응답을 반환합니다.
<pre>{<br>    "priority": 2,<br>    "name": "첫 번째 작업",<br>    "ID": "4c7c08fa0000002ff924e298ee148df4",<br>    "planningStartDate": "2010-08-30T09:00:00:000-0600" <br>}</pre>

>[!NOTE]
이러한 필드 이름은 대/소문자를 구분합니다.

가능한 필드 참조 목록을 보려면  [API 탐색기](../../wf-api/general/api-explorer.md)

#### 중첩된 개체 검색

중첩된 개체를 검색할 수 있습니다. 기본적으로 중첩된 개체는 이름과 ID만 사용하여 반환됩니다. 예를 들어 소유자와 함께 모든 문제를 가져오려면 다음 요청을 사용하십시오.
<pre>/attask/api/v15.0/issue/search?fields=owner</pre>추가 정보가 필요한 경우 콜론 구문을 사용하여 중첩 필드를 요청할 수 있습니다. 예를 들어 다음 요청은 소유자의 이름, ID, 제목 및 전화 번호와 함께 모든 문제를 검색합니다
<pre>/attask/api/v15.0/issue/search?fields=owner:title,owner:phoneNumber</pre>를 반환하고 다음을 반환합니다. 
<pre>{<br>    "name": "중요한 문제"<br>    "ID": "4c78285f00000908ea8cfd66e084939f",<br>    "owner": {<br>        "title": "운영 전문가",<br>        "phoneNumber": "555-1234",<br>        "name": "관리자 사용자",<br>        "ID": "4c76ed7a0000054c172b2c2d9f7f81c3" <br>    } <br>}</pre>

#### 중첩된 컬렉션 검색

중첩된 개체 컬렉션을 검색할 수 있습니다. 예를 들어 모든 작업이 포함된 프로젝트를 가져오려면 다음 요청을 사용하십시오.
<pre>/attask/api/v15.0/project/search?fields=tasks</pre>다음 요청은 태스크 지정을 가져옵니다.
<pre>/attask/api/v15.0/task/search?fields=assignments</pre>

#### 여러 중첩 필드 검색

기본적으로 각 작업의 이름과 ID만 반환되지만 콜론 구문으로 추가 중첩 필드를 지정할 수 있습니다. 관련 개체나 컬렉션에 대해 사용 가능한 모든 필드를 보려면 개체/컬렉션 참조에 콜론 및 별표를 추가하기만 하면 됩니다.
<pre>/attask/api/v15.0/task/search?fields=assignments:*</pre>

#### 사용자 지정 데이터 검색

접두사 &quot;DE:&quot;를 사용하여 사용자 지정 데이터 필드를 검색할 수 있습니다. 예를 들어 &quot;CustomText&quot;라는 매개 변수를 사용하여 프로젝트를 요청하려면 다음 요청을 사용하십시오.
<pre>/attask/api/v15.0/project/search?fields=DE:CustomText</pre>어느 것이 반환되는지
<pre>{<br>    "name": "사용자 지정 데이터 프로젝트",<br>    "ID": "4c9a954f0000001afad0687d7b1b4e43",<br>    "DE:CustomText": "task b" <br>}</pre>parameterValues 필드를 요청하여 개체의 모든 사용자 지정 데이터를 검색할 수도 있습니다. For example, 
<pre>/attask/api/v15.0/project/search?fields=parameterValues</pre>는 다음과 유사한 데이터를 반환합니다.
<pre>{<br>    "name": "사용자 지정 데이터 프로젝트",<br>    "ID": "4c9a954f0000001afad0687d7b1b4e43",<br>    parameterValues: { <br>        "DE:CustomText": "작업 b", <br>        "DE:CustomNumber": 1.4, <br>        "DE:CustomCheckBoxes": ["first", "second", "third"] <br>    } <br>}</pre>

#### 명명된 쿼리 사용

일부 객체 유형에는 일반적으로 실행되는 라는 검색이 있으며 객체 유형 URI 끝에 쿼리 이름을 추가하여 사용할 수 있습니다. 예를 들어 다음 요청은 사용자가 현재 할당된 작업 항목(작업 및 문제)을 검색합니다.
<pre>/atask/api/v15.0/work/myWork</pre>명명된 쿼리는 필드 매개 변수를 요청하여 추가 필드를 검색할 수 있도록 지원합니다. 이름이 지정된 일부 쿼리는 추가 필터도 허용합니다. 개체에 대해 허용되는 명명된 쿼리 목록을 보려면 [API 탐색기](../../wf-api/general/api-explorer.md)에서 개체의 작업 탭을 참조하십시오.

#### 카운트 필터 사용

주어진 검색에서 반환할 결과 수를 지정할 수 있습니다. 이렇게 하면 서버가 요청을 보다 신속하게 처리하고 대역폭을 저장할 수 있습니다. 예를 들어, 요청
<pre>GET /attask/api/v15.0/project/count?status=CUR</pre>다음 형식으로 결과 수를 반환합니다.
<pre>{<br>    "count": 3 <br>}</pre>이 결과는 전체 개체가 전송되는 경우보다 훨씬 더 작은 다운로드입니다. 필터 구문은 검색 명령과 동일합니다.

### 보고서 요청

하나 이상의 그룹화를 사용하여 일부 필드의 합계만 원하는 보고서 요청을 수행할 수 있습니다. 다음 예와 같이 보고서 구문은 SOAP API의 구문과 동일합니다.
<pre>GET /atask/api/v15.0/hour/report?project:name_1_GroupBy=true&amp;hours_AggFunc=sum</pre>다음 결과를 반환합니다.
<pre>{<br>    "첫 번째 프로젝트": { <br>        "sum_hours": 15 <br>    }, <br>     "두 번째 프로젝트": { <br>        "sum_hours": 30 <br>    } <br>}</pre>$$ROLLUP=true 매개 변수를 추가하면 각 그룹화 수준에서 합계가 포함됩니다.
<pre>{<br>    "첫 번째 프로젝트": { <br>        "sum_hours": 15 <br>    }, <br>    "두 번째 프로젝트": { <br>        "sum_hours": 30 <br>    }, <br>    "$$ROLLUP": { <br>        "sum_hours": 45 <br>    } <br>}</pre>

### API에서 쿼리 결과 정렬

API 호출에 다음을 추가한 경우 필드를 기준으로 결과를 정렬할 수 있습니다.

&amp;entryDate_Sort=asc

예를 들어, 작업 계획 시작 날짜별로 정렬하려면 entryDate를 제거하고 planningCompletionDate로 바꿉니다.

Workfront의 대부분의 필드에 대해 작동합니다.

### 쿼리 제한 고려

객체를 쿼리할 때는 관련 객체의 관계 및 검색 제한에 대해 특별히 고려해야 합니다. 예를 들어 다음 표에 표시된 대로 프로젝트에 대한 쿼리는 2,000개 이하의 프로젝트를 반환할 수 있습니다. 이러한 2,000개의 프로젝트는 &quot;기본 객체&quot;로 간주됩니다. 프로젝트의 작업 필드를 쿼리하면 컬렉션인 작업 필드가 기본 객체 프로젝트의 보조 객체가 됩니다. 작업 필드에 대한 쿼리는 프로젝트에 수천 개의 작업을 포함할 수 있습니다. 총 반환되는 개체(프로젝트 및 작업)의 총 수는 최대 50,000개를 초과할 수 없습니다.

최적의 성능을 보장하기 위해 다음 표에는 검색 요청에 적용된 제한 사항이 나와 있습니다. 

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th>쿼리 결과</th> 
   <th>제한 사항</th> 
   <th>설명</th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td width="200">기본 결과 수</td> 
   <td>100</td> 
   <td> 쿼리 필터에 제한이 지정되지 않은 경우(예: $$LIMIT) 결과에 기본 개체가 100개 이하일 수 있습니다. <br>자세한 내용은 <a href="#using-paginated-responses" class="MCXref xref">페이지 매김된 응답 사용</a> 을 참조하십시오. </td> 
  </tr> 
  <tr> 
   <td>최대 결과 수</td> 
   <td>2,000</td> 
   <td>쿼리 필터(즉, $$LIMIT)는 2000개 이하의 결과를 반환할 수 있습니다. 자세한 내용은 "페이지 매김된 응답"을 참조하십시오.</td> 
  </tr> 
  <tr> 
   <td>최대 필드 깊이</td> 
   <td>4</td> 
   <td>표시할 필드를 식별할 때 쿼리되는 개체에서 4개 이상의 수준을 유지할 수 없습니다.</td> 
  </tr> 
  <tr> 
   <td>최대 개체 수</td> 
   <td>50,000</td> 
   <td>결과 집합에는 50000 주 개체와 보조 개체를 포함할 수 없습니다.</td> 
  </tr> 
  <tr> 
   <td>최대 필드 수</td> 
   <td nowrap>1,000,000</td> 
   <td>결과 세트가 50000 개체보다 작으면 결과에 최대 100만 개의 필드가 포함될 수 있습니다.</td> 
  </tr> 
  <tr> 
   <td>일괄 생성/갱신 최대 수</td> 
   <td>100</td> 
   <td>최대 배치 생성 또는 업데이트 제한은 100입니다.</td> 
  </tr> 
 </tbody> 
</table>

### 페이지 매김된 응답 사용 {#using-paginated-responses}

기본 결과 수 쿼리 제한을 무시하고 200개의 결과를 허용하려면 다음 예와 같이 $LIMIT=200 필터를 쿼리에 포함할 수 있습니다.
<pre>GET /attask/api/v15.0/project/search?$$LIMIT=200</pre>시스템의 다른 테넌트에 대한 신뢰성 및 성능을 보장하기 위해 쿼리당 허용되는 최대 결과 제한은 2000개 객체입니다. 더 큰 제한을 지정하려고 하면 IllegalArgumentException 오류 메시지가 발생합니다. 

따라서 큰 데이터 세트에 대해 페이지 매김된 응답 사용을 고려해 보는 것이 좋습니다. 반환할 첫 번째 결과를 지정하려면 $$FIRST 필터를 추가합니다. 예를 들어 다음 요청은 쿼리에 대한 결과 201-250을 반환합니다.
<pre>GET /attask/api/v15.0/project/search?$$FIRST=201&amp;$$LIMIT=50</pre>

### 액세스 규칙 만들기

액세스 규칙을 만들어 객체에 액세스할 수 있는 사용자를 결정할 수 있습니다. 다음은 설정할 수 있는 액세스 규칙의 예입니다.

ID가 &quot;abc123&quot;인 사용자만 프로젝트를 공유하도록 설정하려면 다음 요청을 사용하십시오.
<pre>GET /attask/api/v15.0/project/123abxxxxxxxxxxxxxxxxxxxxxxxx?method=put &amp;updates={ accessRules: [ {accessorID: 'abc123', accessorObjCode: 'USER', coreAction: 'VIEW'} ] }</pre>또는 새 개인와만 공유하고 기존 권한을 그대로 유지하려면 다음을 수행하십시오.
<pre>GET /attask/api/v15.0/project/123abxxxxxxxxxxxxxxxxxxxxxxxx/share?method=put&amp;accessorID=abc123&amp;accessorObjCode=USER&amp;coreAction=VIEW</pre>기존 액세스 규칙을 검색하려면
<pre>GET /attask/api/v15.0/project/123abxxxxxxxxxxxxxxxxxxxxxxxx?fields=accessRules:*</pre>

## POST 동작

POST은 새 개체를 삽입합니다. 구문은 PUT과 동일하지만 몇 가지 예외가 있습니다. 새 개체가 아직 없으므로 ID가 없습니다. 따라서 URI에 ID가 포함되지 않습니다.

### 개체 만들기

다음은 새 프로젝트 만들기 요청의 예입니다.
<pre>POST /attask/api/v15.0/project?name=새 프로젝트</pre>응답에는 새 ID 및 지정된 다른 필드와 함께 새로 만든 프로젝트가 포함되어 있습니다.

### 개체 복사

일부 개체는 복사 작업을 지원합니다. 이러한 개체 유형의 경우 copySourceID 매개 변수를 사용하여 게시하여 새 개체를 만들 수 있습니다. 예를 들어 다음 요청은 지정된 프로젝트를 복사하고 새 이름을 지정합니다.

```
POST /attask/api/v15.0/project?copySourceID=4c7...&name=Copied Project
```

### 문서 업로드

다음 API URL을 통해 문서를 업로드할 수 있습니다.
<pre>POST /attask/api/v15.0/upload</pre>API에는 콘텐츠 유형이 다중 부분/양식 데이터여야 합니다. 파일의 매개 변수 이름은 uploadFile이어야 합니다. 서버는 다음 JSON 데이터를 반환합니다.
<pre>{<br>    "handle": "4c7c08fa0000002ff924e298ee148df4"<br>}</pre>Workfront 문서를 만들 때 핸들을 사용하고 다음 URL에 게시할 수 있습니다.
<pre>POST /atask/api/v15.0/document?updates={<br>    이름: aFileName,<br>    핸들: abc...123, (파일 업로드에서 처리)<br>    docObjCode: PROJ, (또는 작업, OPTASK 등)<br>    objID: abc...123,<br>    currentVersion:{version:v1.0,fileName:aFileName}<br>}</pre>

## PUT 동작

PUT은 기존 개체를 업데이트하는 데 사용됩니다.

PUT에 대한 응답은 GET과 동일합니다. 두 경우 모두 업데이트 후 서버가 객체의 새 상태를 반환합니다. GET 요청에 대한 응답을 변경하는 데 사용되는 모든 규칙은 반환할 추가 필드 지정, 사용자 지정 데이터 등과 같은 PUT에서도 작동합니다.

### 개체 편집

개체 업데이트는 항상 개체의 고유한 URI를 사용하여 ID로 수행됩니다. 업데이트할 필드는 요청 매개 변수로 지정됩니다. 예를 들어 프로젝트 이름을 변경하려면 다음과 유사한 요청을 보낼 수 있습니다.
<pre>PUT /attask/api/v15.0/project/4c7..?name=새 프로젝트 이름 <br>PUT /attask/api/v15.0/project?id=4c7..&amp;name=새 프로젝트 이름</pre>업데이트에 ID가 필요하므로 개체가 서버에 없으면 이 작업이 실패합니다.

### JSON 편집 지정

다음 예와 같이 업데이트 요청 매개 변수를 사용하여 JSON 구문을 사용하여 업데이트할 필드를 지정할 수 있습니다.
<pre>PUT /attask/api/v15.0/project/4c7..?업데이트= <br>{<br>     이름: "새 프로젝트 이름", <br>     상태: "CUR", <br>     ... <br>}</pre>

### 중첩 업데이트 만들기

일부 개체에는 업데이트할 수 있는 개인 소유 컬렉션이 있습니다. 예를 들어 다음 예제에서는 지정된 작업의 기존 할당을 덮어쓰는 방법을 보여 줍니다.
<pre>PUT /attask/api/v15.0/task/4c7..?업데이트= <br>{<br>    지정: [ <br>        { <br>            assignedToID: "2222...54d0, <br>            assignmentPercent: 50.0 <br>        },{ <br>            roleID: "1111...54d0"<br>        } <br>    ] <br>}</pre>

>[!NOTE]
최상위 수준의 업데이트는 희박한 반면, 컬렉션이나 중첩 개체에 대한 업데이트는 기존 컬렉션을 완전히 대체합니다. 객체에 영향을 주지 않고 작업에 대한 단일 할당을 편집하려면 작업 대신 할당에 PUT을 사용합니다.

다음 예에서는 프로젝트를 공용 도움말 데스크 대기열로 만듭니다. 기존 큐 속성이 대체됩니다.
<pre>PUT /attask/api/v15.0/project/4c7..?업데이트= <br>{ <br>    queueDef: { <br>        isPublic: 1 <br>    } <br>}</pre>

### 작업 요청 매개 변수 사용

일부 개체에서는 간단한 편집 이외에 수행할 수 있는 추가 작업을 지원합니다. 작업 요청 매개 변수를 사용하여 이러한 작업을 지정할 수 있습니다. 예를 들어 다음 요청은 지정된 프로젝트의 타임라인을 다시 계산합니다.
<pre>PUT /attask/api/v15.0/project/4c7..?action=calculateTimeline<br><br>또는<br><br>PUT /attask/api/v15.0/project/4c7../calculateTimeline </pre>

### 객체 이동

다음은 한 프로젝트에서 다른 프로젝트로 작업을 이동하는 구문을 보여 줍니다.
<pre>PUT /attask/api/v15.0/task/4c7../move?projectID=5d8..</pre>각 작업 유형의 예는 다음과 같습니다. (??)
<pre>PUT /atask/api/v15.0/project/1234/approveApproval<br><br>PUT /atask/api/v15.0/project/1234/calculateFinance<br><br>PUT /attask/api/v15.0/project/1234/calculateTimeline<br><br>PUT /atask/api/v15.0/project/1234/calculateDataExtension<br><br>PUT /atask/api/v15.0/project/1234/recallApproval<br><br>PUT /atask/api/v15.0/project/1234/rejectApproval<br><br>PUT /attask/api/v15.0/task/1234/move<br><br>PUT /atask/api/v15.0/workitem/1234/markViewed</pre>이동 작업만 작업 항목을 이동할 프로젝트를 지정하려면 추가 속성을 식별해야 합니다.

다음은 각 작업 유형의 예입니다. 
<pre>PUT /attask/api/v15.0/project/1234?method=put&amp;updates={accessRules:[{accessorID: 'abc123', accessorObjCode: 'USER', coreAction: 'VIEW'}]}</pre>

### 개체 공유

다음 예제에서는 팀과 프로젝트를 공유하는 구문을 보여 줍니다.
<pre>PUT /atattask/api/v15.0/project/123abxxxxxxxxxxxxxxxxxxxxxxxxxxxxxx/share?accessorID=123abxxxxxxxxxxxxxxxxxxxxxxxxxx&amp;accesobjCode=TEAMOB</pre>개체를 편집할 때 다음 예제와 유사한 PUT 및 업데이트를 보내어 개체의 모든 액세스 규칙을 바꿀 수 있습니다.
<pre>PUT /attask/api/v15.0/project/123abcxxxxxxxxxxxxxxxxxxxxxxxx?method=PUT&amp;updates={accessRules:[{accessorID:'123abcxxxxxxxxxxxxxxxxxxxxxxxxxx',접근자ObjCode:'TEAMOB',coreAction:'VIEW'}}</pre>다음 예제에서는 작업을 한 프로젝트에서 다른 프로젝트로 이동하는 구문을 보여 줍니다.
<pre>PUT /attask/api/v15.0/task/4c7../move?projectID=5d8..</pre>

## DELETE 동작

DELETE은 개체를 제거합니다. 모든 경우 URI에 매개 변수 force=true가 포함되어 서버가 지정된 데이터와 해당 종속성을 제거할 수 있습니다. 다음 예에서는 URI에서 HTTP DELETE 메서드를 실행하여 작업이 삭제됩니다.
<pre>DELETE /atask/api/v15.0/task/4c78821c000d6fa8d5e52f07a1d54d0 <br>DELETE /atask/api/v15.0/task?id=4c78821c000d6fa8d5e52f07a1d54d0 <br>DELETE /atask/api/v15.0/task/4c78821c000d6fa8d5e52f07a1d54d0?force=true <br>DELETE /atask/api/v15.0/task?id=4c78821c000d6fa8d5e52f07a1d54d0?force=true</pre>

## 벌크 업데이트

벌크 업데이트 문은 단일 API 호출 내에서 동시에 여러 개체를 업데이트합니다. 벌크 만들기 API 호출은 다음 예와 같이 일반 업데이트 호출과 유사하게 빌드됩니다.
<pre>PUT /atask/api/v15.0/proj?updates=[{"name":"Test_Project_1"},{"name":"Test_Project_2"}]&amp;method=POST&amp;apiKey=123ab-ccxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxx</pre>결과 다음과 유사한 결과가 발생합니다.
<pre>데이터: [{<br>    ID: "53ff8d3d003b438b57a8a784df38f6b3",<br>    이름: "Test_Project_1",<br>    objCode: "PROJ",<br>    percentComplete: 0,<br>    planningCompletionDate: "2014-08-28T11:00:00:000-0400",<br>    planningStartDate: "2014-08-28T11:00:00:000-0400",<br>    우선 순위: 0,<br>    projectedCompletionDate: "2014-08-28T16:12:00:000-0400",<br>    상태: "CUR"<br>},<br>{<br>    ID: "53ff8d49003b43a2562aa34eea3b6b10",<br>    이름: "Test_Project_2",<br>    objCode: "PROJ",<br>    percentComplete: 0usi<br>    planningCompletionDate: "2014-08-28T11:00:00:000-0400",<br>    planningStartDate: "2014-08-28T11:00:00:000-0400",<br>    우선 순위: 0,<br>    projectedCompletionDate: "2014-08-28T16:12:00:000-0400",<br>    상태: "CUR"<br>}]</pre>다음과 유사한 벌크 업데이트를 수행할 수도 있습니다.
<pre>PUT /atattask/api/v15.0/proj?Umethod=PUT&amp;updates=[{"ID":"123abcxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxx","name":"Test_Project_1_ Edit"},{"ID":"123abcxxxxxxxxxxxxxxxxxxxxxx","이름":"Test_Project_2_Edit"}]&amp;apiKey=123xxxxxxxxxxxxxxxxxxxxxxxxxxxxxx</pre>결과 다음과 유사한 결과가 발생합니다.
<pre>데이터: [ {<br>     ID: "53ff8e15003b461d4560f7f65a440078",<br>     이름: "Test_Project_1_Edit",<br>     objCode: "PROJ",<br>     percentComplete: 0,<br>     planningCompletionDate: "2014-08-28T11:00:00:000-0400",<br>     planningStartDate: "2014-08-28T11:00:00:000-0400",<br>     우선 순위: 0,<br>     projectedCompletionDate: "2014-08-28T16:16:00:000-0400",<br>     상태: "CUR"<br>},<br>{<br>    ID: "53ff8e19003b46238a58d303608de502",<br>    이름: "Test_Project_2_Edit",<br>    objCode: "PROJ",<br>    percentComplete: 0,<br>    planningCompletionDate: "2014-08-28T11:00:00:000-0400",<br>    planningStartDate: "2014-08-28T11:00:00:000-0400",<br>    우선 순위: 0,<br>    projectedCompletionDate: "2014-08-28T16:16:00:000-0400",<br>    상태: "CUR"<br>}]</pre>모든 작업이 동일한 트랜잭션에서 수행되도록 하려면 배치 API 호출에 "atomic=true"를 요청 매개 변수로 추가합니다. 이렇게 하면 작업이 실패할 경우 모든 작업이 롤백됩니다.

>[!NOTE]
원자 배치 작업은 &quot;성공&quot;만 반환할 수 있습니다. true 또는 오류가 표시됩니다.
