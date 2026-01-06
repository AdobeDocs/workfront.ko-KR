---
content-type: api
navigation-topic: general-api
title: API 기본 사항
description: API 기본 사항
author: Becky
feature: Workfront API
role: Developer
exl-id: d8c27915-8e1b-4804-9ef8-3a2efd57caac
source-git-commit: 319c45bc6617269f358af1e7b5f6132a8694710b
workflow-type: tm+mt
source-wordcount: '4396'
ht-degree: 0%

---


# API 기본 사항

Adobe Workfront API의 목표는 HTTP를 통해 작동하는 REST 풀 아키텍처를 도입하여 Workfront과의 통합 빌드를 간소화하는 것입니다. 이 문서에서는 사용자가 REST 및 JSON 응답에 익숙하다고 가정하고 Workfront API로 취한 접근 방식을 설명합니다.

Workfront 스키마에 익숙하면 통합 목적으로 Workfront에서 데이터를 가져오는 데 활용할 수 있는 데이터베이스 관계를 이해하는 데 도움이 됩니다.

## 제한 및 지침

일관된 Workfront 온디맨드 시스템 성능을 보장하기 위해 Workfront API는 동시 API 스레드를 제한합니다. 이 가드레일은 API 호출 남용으로 인해 발생하는 시스템 문제를 방지합니다. 샌드박스 환경에는 동일한 동시 API 스레드 제한이 있으므로 고객 및 파트너가 프로덕션에 코드를 릴리스하기 전에 API 호출을 정확하게 테스트할 수 있습니다.

프로덕션, 미리보기 및 테스트 드라이브 환경의 경우 최종 사용자 요청은 Workfront CDN(Akamai)을 통해 라우팅되므로 최대 URI 길이가 8892바이트입니다. 이 제한은 CDN을 통해 라우팅되는 URI에만 적용됩니다.

### 면책 조항

API의 모든 사용은 프로덕션 환경에서 실행하기 전에 Workfront Beta 환경에서 테스트해야 합니다. Workfront이 온디맨드 소프트웨어에 부담을 준다고 합리적으로 생각하는 프로세스에 고객이 API를 사용하는 경우(즉, 프로세스가 다른 고객을 위해 소프트웨어 성능에 심각한 부정적인 영향을 미치는 경우), Workfront은 고객에게 해당 프로세스를 중단하도록 요청할 권리를 보유합니다. 고객이 이를 준수하지 않고 문제가 지속되는 경우 Workfront은 프로세스를 종료할 수 있는 권한을 보유합니다.

## WORKFRONT API URL

Workfront API를 호출하는 데 사용할 URL에 대한 자세한 내용은 [Adobe Workfront API 호출에 대한 도메인 형식](/help/quicksilver/wf-api/tips-tricks-and-troubleshooting/locate-domain-for-api.md)을 참조하십시오.

## REST 기본 사항

이 섹션에서는 다음 REST 원칙에 대해 Workfront REST API와 상호 작용하는 방법에 대한 높은 수준의 소개를 제공합니다.

### 개체 URI

시스템의 각 객체에는 객체 유형과 ID로 구성된 고유한 URI가 제공됩니다. 다음 예는 세 개의 고유 개체를 설명하는 URI를 보여 줍니다.

```
/attask/api/v15.0/project/4c78821c0000d6fa8d5e52f07a1d54d0
/attask/api/v15.0/task/4c78821c0000d6fa8d5e52f07a1d54d1
/attask/api/v15.0/issue/4c78821c0000d6fa8d5e52f07a1d54d2
```

개체 유형은 대소문자를 구분하지 않으며 축약된 ObjCode(예: proj) 또는 대체 개체 이름(프로젝트)일 수 있습니다.

개체 목록, 유효한 ObjCodes 및 개체 필드는  [API 탐색기](../../wf-api/general/api-explorer.md).

>[!NOTE]
>
>Workfront API의 컨텍스트에서 사용자 정의 양식은 `Category` 개체이고 사용자 정의 필드는 `Parameter` 개체입니다.

### 작업

개체는 고유한 URI에 HTTP 요청을 전송하여 조작됩니다. 수행할 작업은 HTTP 메서드에서 지정합니다.

표준 HTTP 메서드는 다음 작업에 해당합니다.

* **GET** - ID별로 개체를 검색하고, 쿼리로 모든 개체를 검색하고, 보고서를 실행하거나, 명명된 쿼리를 실행합니다.
* **POST** - 새 개체를 삽입합니다.
* **PUT** - 기존 개체를 편집합니다.
* **DELETE** - 개체를 삭제합니다.

클라이언트 결함이나 프로토콜 길이 제한을 해결하기 위해 메서드 매개 변수를 사용하여 HTTP 동작을 재정의할 수 있습니다. 예를 들어, 다음 URI를 게시하여 GET 작업을 구현할 수 있습니다.
<pre>GET /attask/api/v15.0/project?id=4c78...54d0&amp;method=get<br>GET /attask/api/v15.0/project/4c78...54d0?method=get</pre>

### 응답

각 요청에는 JSON 형식의 응답이 제공됩니다. 요청에 성공한 경우 응답에 데이터 속성이 있거나 문제가 발생한 경우 오류 속성이 있습니다. 예: 요청

```
GET /attask/api/v15.0/proj/4c7c08b20000002de5ca1ebc19edf2d5
```

다음과 유사한 JSON 응답을 반환합니다.


<pre>{<br>    "data": [<br>        {<br>            "percentComplete": 0,<br>            "status": "CUR",<br>            "우선 순위": 2,<br>            "name": "새 프로젝트",<br>            "ID": "4c7c08b20000002de5ca1ebc19edf2d5" <br>        } <br>    ] <br>}</pre>

>[!NOTE]
>
>브라우저의 주소 표시줄을 통해 GET 요청을 실행할 때 sessionID를 요청의 일부로 포함할 필요가 없습니다.

PUT, POST 및 DELETE 요청 주위에 특수 보안이 추가되었습니다. 데이터베이스에 쓰거나 데이터베이스에서 삭제하는 요청은 **sessionID=abc123**&#x200B;이(가) URI에 포함된 경우에만 실행할 수 있습니다. 다음 예제는 DELETE 요청을 검색하는 방법을 보여 줍니다.
<pre>GET /attask/api/v15.0/project?id=4c78...54d0&amp;method=delete&amp;sessionID=abc123<br>GET /attask/api/v15.0/project/4c78...54d0?method=delete&amp;sessionID=abc123</pre>

### 인증

API는 각 요청을 인증하여 클라이언트가 요청된 개체를 보거나 수정할 수 있는 액세스 권한을 보유하는지 확인합니다.

인증은 다음 방법 중 하나를 사용하여 제공할 수 있는 세션 ID를 전달하여 수행됩니다.

#### 요청 헤더 인증

기본 인증 방법은 세션 토큰이 포함된 SessionID라는 요청 헤더를 전달하는 것입니다. 이를 통해 [CSRF(크로스 사이트 요청 위조)](https://en.wikipedia.org/wiki/Cross-site_request_forgery) 공격으로부터 안전하며 캐싱을 위해 URI를 방해하지 않는 이점이 있습니다.

다음은 요청 헤더의 예입니다.

```
GET /attask/api/v15.0/project/search
SessionID: abc1234
```

#### 쿠키 기반 인증

API는 웹 UI에서 시스템에 사용하는 것과 동일한 쿠키 기반 인증을 사용합니다. 클라이언트가 웹 UI를 사용하여 Workfront에 로그인하는 경우 동일한 브라우저 내에서 수행된 모든 AJAX 호출은 동일한 인증을 사용합니다.

>[!NOTE]
>
>CSRF(Cross Site Request Forgery) 공격으로부터 보호하기 위해 이 인증 방법은 읽기 전용 작업에만 사용할 수 있습니다.

## 로그인

>[!IMPORTANT]
>
>Workfront에서는 더 이상 `/login` 끝점 또는 API 키를 사용하지 않는 것이 좋습니다. 대신 다음 인증 방법 중 하나를 사용하십시오.
>
>* JWT를 사용한 서버 인증
>* OAuth2를 통한 사용자 인증
>
>이러한 인증 방법 설정에 대한 지침은 [Workfront 통합을 위한 OAuth2 애플리케이션 만들기](../../administration-and-setup/configure-integrations/create-oauth-application.md)를 참조하십시오.
>
>Workfront에서 서버 인증을 사용하는 방법에 대한 지침은 [JWT 흐름을 사용하여 조직의 사용자 지정 OAuth 2 애플리케이션 구성 및 사용](../../wf-api/api/oauth-app-jwt-flow.md)을 참조하십시오.
>
>Workfront에서 사용자 인증을 사용하는 방법에 대한 지침은 [인증 코드 흐름을 사용하여 조직의 사용자 지정 OAuth 2 애플리케이션 구성 및 사용](../../wf-api/api/oauth-app-code-token-flow.md)을 참조하십시오.

>[!NOTE]
>
>이 섹션에 설명된 절차는 Adobe 비즈니스 플랫폼에 아직 온보딩되지 않은 조직에만 적용됩니다. 조직이 Workfront Business Platform에 온보딩된 경우 Workfront API를 통해 Adobe에 로그인할 수 없습니다.
>
>조직이 Adobe Business Platform에 온보딩되었는지 여부에 따라 달라지는 절차 목록은 [플랫폼 기반 관리 차이점(Adobe Workfront/Adobe Business Platform)](../../administration-and-setup/get-started-wf-administration/actions-in-admin-console.md)을 참조하십시오.

유효한 사용자 이름과 암호를 사용하여 다음 요청을 사용하여 세션 ID를 얻을 수 있습니다.

```
POST /attask/api/v15.0/login?username=admin&password=user
```

이렇게 하면 쿠키를 설정하여 이후 요청을 인증하고 새로 만든 sessionID, 로그인한 사용자의 userID 및 기타 세션 속성으로 JSON 응답을 반환합니다.

>[!NOTE]
>
>지정된 API 사용자 및 관리자가 있는 경우 Workfront에서는 API 키를 사용하여 로그인할 것을 권장합니다.

**API 키 생성**

다음 예와 같이 시스템에 해당 사용자로 로그인할 때 API 키를 생성할 수 있습니다.


```
PUT /attask/api/v15.0/user?action=generateApiKey&username= username&password=password&method=put
```

**이전에 생성한 API 키 검색**

getApiKey를 실행하여 특정 사용자에 대해 이전에 생성된 API 키를 검색할 수도 있습니다.


```
PUT /attask/api/v15.0/user?action=getApiKey&username=user@email.com&password=userspassword&method=put
```

그런 다음 sessionID 또는 사용자 이름과 암호 대신 이 값을 사용하여 &quot;apiKey&quot;를 요청 매개 변수로 추가하여 모든 API 호출을 인증할 수 있습니다. 이는 보안 관점에서 볼 때 유용합니다.

다음 요청은 apiKey를 사용하여 프로젝트에서 데이터를 검색하는 예제입니다.

```
GET /attask/api/v15.0/project/abc123xxxxx?apiKey=123abcxxxxxxxxx
```

**API 키 무효화**

apiKey 값이 손상된 경우 다음 예와 같이 현재 API 키를 무효화하는 &quot;clearApiKey&quot;를 실행할 수 있습니다.

```
GET /attask/api/v15.0/user?action=clearApiKey&username=user@email.com&password=userspassword&method=put
```

삭제하면 getApiKey를 다시 실행하여 새 API 키를 생성할 수 있습니다.

### 로그아웃

세션이 완료되면 다음 요청을 사용하여 사용자를 로그아웃시켜 sessionID에 대한 추가 액세스를 방지할 수 있습니다.

```
GET /attask/api/v15.0/logout?sessionID=abc1234
```

로그아웃할 sessionID는 쿠키, 요청 헤더 또는 요청 매개 변수로 지정할 수 있습니다.

사용자를 로그아웃하려면 다음 작업을 수행하십시오.

1. 로그인 화면으로 이동하지만 로그인하지 않습니다.
1. URL을 /attask/api/v15.0/project/search로 변경합니다.\
   페이지를 찾을 수 없습니다.
1. *search* 단어를 login?username=admin&amp;password=user로 바꾸고 *admin* 및 *user에 사용자 이름과 암호를 대입합니다.\
   *이 세션은 브라우저에 쿠키로 저장되며 후속 GET 요청마다 다시 기술할 필요가 없습니다.

1. URL을 **/attask/api/v15.0/project/search**(으)로 다시 변경합니다.
1. 제공된 응답에 주목합니다.

PUT, POST 및 DELETE 요청을 수행할 때 로그인 후 제공된 sessionID를 항상 포함해야 합니다.

## GET 동작

HTTP GET 메서드를 사용하여 개체 또는 여러 개체를 검색하고 보고서를 실행합니다.

### 개체 검색 중

수정자 및 필터를 사용하여 객체 검색을 향상시킬 수 있습니다.

#### 개체 ID를 사용하여 개체 검색

객체의 ID를 알고 있는 경우 고유한 URI에 액세스하여 객체를 검색할 수 있습니다. 예: 요청

```
GET /attask/api/v15.0/project/4c78821c0000d6fa8d5e52f07a1d54d0
```

다음과 유사한 응답을 반환합니다.

<pre>{<br>    "percentComplete": 0,<br>    "status": "CUR",<br>    "우선 순위": 2,<br>    "name": "새 프로젝트",<br>    "ID": "4c7c08b20000002de5ca1ebc19edf2d5" <br>}</pre>


다음 예와 같이 id 요청 매개 변수를 지정하고 쉼표로 구분된 ID 목록을 제공하여 동일한 요청에서 여러 개체를 검색할 수 있습니다.


```
GET /attask/api/v15.0/project?id=4c78...54d0,4c78...54d1
```

/attask/api/v15.0/project?id=... 요청이 `/attask/api/v15.0/project/...` 요청과 동일합니다.

#### URI를 사용하여 개체 검색

ID 이외의 기준으로 개체를 검색하려면 URI를 검색하면 됩니다.

예를 들어 다음 요청을 사용하여 시스템의 모든 프로젝트 목록을 반환할 수 있습니다.

```
GET /attask/api/v15.0/project/search
```

요청 매개 변수를 이름-값 쌍으로 사용하여 필터를 지정할 수 있습니다. 예를 들어 다음 예제는 모든 현재 프로젝트를 찾는 요청을 보여 줍니다.

```
GET /attask/api/v15.0/project/search?status=CUR
```

다음 요청은 아직 완료되지 않았고 John이라는 사용자에게 할당된 모든 작업을 찾습니다.

```
GET /attask/api/v15.0/task/search?percentComplete=100
&percentComplete_Mod=lt &assignedTo:firstName=John
```

#### 검색 수정자 사용

다음 표에는 Workfront API와 함께 사용할 수 있는 몇 가지 수정자가 나와 있습니다.

| **한정자** | **설명** | **예** |
| --- | --- | --- |
| eq | 종료됨 상태의 결과를 반환합니다. | <pre>...status=cls&amp;status_Mod=eq...</pre> |
| ne | 닫힘 상태가 아닌 결과를 반환합니다. | <pre>...status=cls&amp;status_Mod=ne...</pre> |
| gte | 완료율이 50보다 크거나 같은 결과 반환 | <pre>...percentComplete=50&amp;percentComplete_Mod=gte...</pre> |
| lte | 완료율이 50보다 작거나 같은 결과 반환 | <pre>...percentComplete=50&amp;percentComplete_Mod=lte...</pre> |
| isnull | 설명이 Null인 결과를 반환합니다. | <pre>...description_Mod=isnull..</pre> |
| null 아님 | 설명이 Null이 아닌 결과를 반환합니다. | <pre>...description_Mod=notnull...</pre> |
| 포함 | 이름에 &quot;Workfront&quot;가 포함된 결과를 반환합니다. | <pre>...name=Workfront&amp;name_Mod=포함...</pre> |
| 사이 | 지난 7일 내에 입력 일자가 있는 결과를 반환합니다. | <pre>...entryDate=$$TODAY-7d&amp;entryDate_Range=$$TODAY&amp;entryDate_Mod=between...</pre> |

{style="table-layout:auto"}

>[!NOTE]
>
>검색 요청은 대소문자를 구분합니다. 오류가 표시되면 다음을 확인하십시오.  **_Mod** 및 **_Range**&#x200B;의 대소문자가 잘못되었습니다.

#### OR 문 사용

&quot;OR&quot;을 포함하는 매개 변수와 필터 또는 일련의 필터 수준을 나타내는 숫자를 추가하여 검색을 강화할 수 있습니다.

OR 문은 OR 문의 필터링 기준을 충족하는 API 호출의 레코드만 반환합니다. 필터가 OR 문 수준 간에 암시되어 있지 않습니다.

예를 들어 을 필터링하려면 다음을 수행합니다

* 이름에 &quot;Planning&quot; OR이 포함된 작업
* 포트폴리오의 작업 이름이 &quot;FixedAssets&quot;이고 이름이 &quot;Steve&quot; OR인 사용자에게 할당된 작업
* &quot;최종 작업&quot;이라는 상위 작업이 있는 작업

그런 다음 여러 OR 문과 함께 다음 API 호출을 사용합니다.
<pre>GET /attask/api/v15.0/task/search?name=Planning<br>&amp;name_Mod=contains<br>&amp;OR:1:portfolio:name=FixedAssets<br>&amp;OR:1:portfolio:name_Mod=eq<br>&amp;OR:1:assignedTo:name=Steve<br>&amp;OR:1:assignedTo:name_Mod=cootains<br>&amp;OR:2:parent:name=Final Task<br>&amp;OR:2:parent:name_Mod=eq
</pre>

#### 필터 매개 변수 사용

검색 필터에 URL 매개 변수를 사용할 때 발생할 수 있는 잠재적인 위험 중 하나는 Workfront이 다른 인증 방법(예: 사용자 이름, 암호, apiKey, 쿠키)을 확인하기 전에 특정 매개 변수를 구문 분석한다는 것입니다. 이런 경우 매개 변수는 호출에서 필터로 사용되지 않습니다. 

이 문제를 방지하기 위해 JSON 형식을 사용하여 필터 매개 변수에 이러한 값을 배치할 수 있습니다. 예를 들어 사용자 이름을 필터링하려면 다음을 사용하지 않고 testuser를 필터링합니다 
<pre>/attask/api/v15.0/user/search?username=testuser@workfront.com</pre>다음 예제와 같이 URL 매개 변수를 필터에 전달합니다.
<pre>/attask/api/v15.0/user/search?filters={"username":"testuser@workfront.com"}</pre>

#### 맵 요청 매개 변수 사용

기본적으로 검색에서 반환되는 데이터는 JSON 배열입니다. 사용 사례에 따라 결과를 ID로 인덱싱된 JSON 개체로 가져오는 것이 더 효율적일 수 있습니다. 이 작업은 맵 요청 매개 변수를 사용하여 수행할 수 있습니다. 예: 요청 
<pre>/attask/api/v15.0/task/search?map=true</pre>는 다음과 유사한 ID로 인덱싱된 응답을 반환합니다.
<pre>{<br>    "data": {<br>        "4c9a97db0000000f13ee444b9aead9b": {<br>            "percentComplete": 0,<br>            "status": "NEW",<br>            "name": "첫 번째 작업",<br>            "ID": "4c9a97db0000000f13ee4446b9aead9b",<br>            "taskNumber": 1 <br>        },<br>        "4ca28ba600002024cd49e75bd43cf601": {<br>            "percentComplete": 0,<br>            "status": "INP:A",<br>            "name": "두 번째 작업",<br>            "ID": "4ca28ba600002024cd49e75bd43cf601",<br>            "taskNumber": 2 <br>        } <br>    } <br>}</pre>

#### 필드 요청 매개 변수 사용

기본적으로 개체를 검색하면 가장 일반적으로 사용되는 필드의 하위 집합만 반환됩니다.

필드 요청 매개 변수를 사용하여 쉼표로 구분된 특정 필드 목록이 반환되도록 지정할 수 있습니다. 예: 요청
<pre>/attask/api/v15.0/task/search?fields=plannedStartDate,priority</pre>다음과 유사한 응답을 반환합니다.
<pre>{<br>    "우선 순위": 2,<br>    "name": "첫 번째 작업",<br>    "ID": "4c7c08fa0000002ff924e298ee148df4",<br>    "plannedStartDate": "2010-08-30T09:00:00:000-0600" <br>}</pre>

>[!NOTE]
>
>이 필드 이름은 대소문자를 구분합니다.

가능한 필드 참조 목록을 보려면  [API 탐색기](../../wf-api/general/api-explorer.md)

#### 중첩된 오브젝트 검색

중첩된 객체를 검색할 수 있습니다. 기본적으로 중첩된 개체는 이름과 ID만 사용하여 반환됩니다. 예를 들어 소유자와 함께 모든 문제를 가져오려면 다음 요청을 사용하십시오.
<pre>/attask/api/v15.0/issue/search?fields=owner</pre>추가 정보가 필요한 경우 콜론 구문을 사용하여 중첩된 필드를 요청할 수 있습니다. 예를 들어 다음 요청은 소유자 이름, ID, 제목 및 전화 번호와 함께 모든 문제를 검색합니다
<pre>/attask/api/v15.0/issue/search?fields=owner:title,owner:phoneNumber</pre>및 는 다음을 반환합니다. 
<pre>&lbrace;<br>    "name": "중요한 문제",<br>    "ID": "4c78285f00000908ea8cfd66e084939f",<br>    "소유자": {<br>        "title": "Operations Specialist",<br>        "phoneNumber": "555-1234",<br>        "name": "Admin User",<br>        "ID": "4c76ed7a0000054c172b2c2d9f7f81c3" <br>    } <br></pre>

#### 중첩된 컬렉션 검색

중첩된 개체 컬렉션을 검색할 수 있습니다. 예를 들어 모든 작업이 포함된 프로젝트를 가져오려면 다음 요청을 사용하십시오.
<pre>/attask/api/v15.0/project/search?fields=tasks</pre>다음 요청은 작업 할당을 받습니다.
<pre>/attask/api/v15.0/task/search?fields=assignments</pre>

#### 여러 중첩 필드 검색

기본적으로 각 작업의 이름과 ID만 반환되지만 콜론 구문을 사용하여 중첩된 필드를 추가로 지정할 수 있습니다. 관련 개체 또는 컬렉션에 사용할 수 있는 모든 필드를 보려면 개체/컬렉션 참조에 콜론과 별표를 추가하면 됩니다.
<pre>/attask/api/v15.0/task/search?fields=assignments:*</pre>

#### 사용자 정의 데이터 검색

접두사 &quot;DE:&quot;를 사용하여 사용자 지정 데이터 필드를 검색할 수 있습니다. 예를 들어 &quot;CustomText&quot;라는 매개 변수를 사용하여 프로젝트를 요청하려면 다음 요청을 사용합니다.
<pre>/attask/api/v15.0/project/search?fields=DE:CustomText</pre>반환
<pre>{<br>    "name": "사용자 지정 데이터 프로젝트",<br>    "ID": "4c9a954f0000001afad0687d7b1b4e43",<br>    "DE:CustomText": "작업 b" <br>}</pre>parameterValues 필드를 요청하여 개체에 대한 모든 사용자 지정 데이터를 검색할 수도 있습니다. 예를 들어, 
<pre>/attask/api/v15.0/project/search?fields=매개 변수 값</pre>는 유사한 데이터를 다음과 반환합니다.
<pre>{<br>    "name": "사용자 지정 데이터 프로젝트",<br>    "ID": "4c9a954f0000001afad0687d7b1b4e43",<br>    parameterValues: { <br>        "DE:CustomText": "작업 b", <br>        "DE:CustomNumber": 1.4, <br>        "DE:CustomCheckBoxes": ["first", "second", "third"] <br>    } <br>}</pre>

#### 명명된 쿼리 사용

일부 객체 유형에는 일반적으로 실행되며 객체 유형 URI의 끝에 쿼리 이름을 추가하여 사용할 수 있는 이름이 지정된 검색어가 있습니다. 예를 들어 다음 요청은 사용자가 현재 할당된 작업 항목(작업 및 문제)을 검색합니다.
<pre>/attask/api/v15.0/work/myWork</pre>명명된 쿼리는 필드 매개 변수를 요청하여 추가 필드를 검색할 수 있도록 지원합니다. 일부 명명된 쿼리는 추가 필터도 수락합니다. 객체에서 허용되는 명명된 쿼리 목록은 의 객체에 대한 작업 탭을 참조하십시오  [API 탐색기](https://developer.adobe.com/workfront/api-explorer/)

#### `Count` 사용 중

`count`을(를) 사용하여 쿼리와 일치하는 결과 수를 반환할 수 있습니다. 이 기능은 결과에 데이터가 필요하지 않을 때 유용합니다. 카운트만 반환하면 서버는 요청을 보다 빠르게 처리하고 대역폭을 절약할 수 있습니다. 예: 요청
<pre>GET /attask/api/v15.0/project/count?status=CUR</pre>결과 수를 다음 형식으로 반환합니다.
<pre>{<br>    "count": 3 <br>}</pre>카운트를 반환하면 전체 개체가 반환되는 경우보다 훨씬 작은 데이터 전송이 수행됩니다. 구문은 검색 명령과 동일합니다.

### 보고서 요청

하나 이상의 그룹화를 사용하여 일부 필드의 집계만 원하는 보고서 요청을 수행할 수 있습니다. 다음 예에 표시된 대로 보고서 구문은 SOAP API의 구문과 동일합니다.
<pre>GET /attask/api/v15.0/hour/report?project:name_1_GroupBy=true&amp;hours_AggFunc=sum</pre>다음 결과를 반환합니다
<pre>&lbrace;<br>    "첫 번째 프로젝트": { <br>        "sum_hours": 15 <br>    }, <br>     "두 번째 프로젝트": { <br>        "sum_hours": 30 <br>    } <br></pre>$$ROLLUP=true 매개 변수를 추가하면 각 그룹화 수준의 합계가 포함됩니다.
<pre>&lbrace;<br>    "첫 번째 프로젝트": { <br>        "sum_hours": 15 <br>    }, <br>    "두 번째 프로젝트": { <br>        "sum_hours": 30 <br>    }, <br>    "$$ROLLUP": { <br>        "sum_hours": 45 <br>    } <br></pre>

### API에서 쿼리 결과 정렬

다음 내용을 API 호출에 추가하면 필드를 기준으로 결과를 정렬할 수 있습니다.

&amp;entryDate_Sort=asc

예를 들어 작업 계획 시작 날짜별로 정렬하려면 entryDate를 제거하고 plannedCompletionDate로 바꿉니다.

Workfront의 대부분의 필드에 적용됩니다.

### 쿼리 제한 고려

객체를 질의할 때는 관련 객체의 관계 및 검색 제한에 대해 특별히 고려해야 합니다. 예를 들어 다음 표에 표시된 것처럼 프로젝트에 대한 쿼리는 2,000개 이하의 프로젝트를 반환할 수 있습니다. 이 2,000개의 프로젝트는 &quot;기본 오브젝트&quot;로 간주됩니다. 프로젝트에서 작업 필드를 쿼리하면 컬렉션인 작업 필드가 기본 개체 프로젝트의 보조 개체가 됩니다. 작업 필드에 대한 쿼리에는 프로젝트에 대한 수천 개의 작업이 포함될 수 있습니다. 총 반환되는 오브젝트(프로젝트 및 작업)의 수는 최대 50,000개를 초과할 수 없습니다.

최적의 성능을 보장하기 위해 다음 표에는 검색 요청에 대한 제한 사항이 나와 있습니다. 

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
   <td>10</td> 
   <td> 쿼리 필터에 제한이 지정되지 않은 경우(예: $$LIMIT) 결과에는 100개 이하의 기본 개체가 포함될 수 있습니다. <br>이 제한을 재정의하는 방법에 대한 지침은 <a href="#using-paginated-responses" class="MCXref xref">페이지 매김된 응답 사용</a>을 참조하세요. </td> 
  </tr> 
  <tr> 
   <td>최대 결과 수</td> 
   <td>2,000</td> 
   <td>쿼리 필터(즉, $$LIMIT)는 2000개 이하의 결과를 반환할 수 있습니다. 자세한 내용은 "페이지 매김된 응답"을 참조하십시오.</td> 
  </tr> 
  <tr> 
   <td>최대 필드 깊이</td> 
   <td>4</td> 
   <td>표시할 필드를 식별할 때 쿼리되는 오브젝트에서 4개 수준 이상 벗어날 수 없습니다.</td> 
  </tr> 
  <tr> 
   <td>최대 오브젝트 수</td> 
   <td>50,000</td> 
   <td>결과 집합에는 기본 및 보조 개체50000 포함될 수 없습니다.</td> 
  </tr> 
  <tr> 
   <td>최대 필드 수</td> 
   <td nowrap>1,000,000</td> 
   <td>결과 집합이 50000 개보다 작으면 결과에 최대 1,000,000개의 필드가 포함될 수 있습니다.</td> 
  </tr> 
  <tr> 
   <td>최대 배치 생성/업데이트 수</td> 
   <td>100</td> 
   <td>최대 배치 생성 또는 업데이트 제한은 100입니다.</td> 
  </tr> 
 </tbody> 
</table>

### 페이지 매김된 응답 사용 {#using-paginated-responses}

기본 결과 수 쿼리 제한을 무시하고 200개의 결과를 허용하려면 다음 예제와 같이 쿼리에 `$$LIMIT=200` 필터를 포함할 수 있습니다.
<pre>GET /attask/api/v15.0/project/search?$$LIMIT=200</pre>

시스템의 다른 테넌트에 대한 신뢰성과 성능을 보장하기 위해 쿼리당 허용되는 최대 결과 제한은 2000개입니다. 더 큰 제한을 지정하려고 하면 `IllegalArgumentException` 오류 메시지가 표시됩니다. 

따라서 큰 데이터 세트에 대해 페이지 번호를 매긴 응답을 사용하는 것이 좋습니다. 반환해야 하는 첫 번째 결과를 지정하려면 `$$FIRST` 필터를 추가합니다. 예를 들어 다음 요청은 쿼리에 대한 결과 201-250을 반환합니다.
<pre>GET /attask/api/v15.0/project/search?$$FIRST=200&amp;$$LIMIT=50</pre>

위의 예에서 `$$FIRST=200`은(는) 201번째 결과를 반환합니다. `$$FIRST=0`이(가) 첫 번째 결과를 반환합니다. $$FIRST 값을 결과를 반환하기 전에 건너뛸 결과 수로 간주하는 것이 도움이 될 수 있습니다.

결과에 페이지가 올바르게 매겨졌는지 확인하려면 정렬 매개 변수를 사용하십시오. 이렇게 하면 결과를 같은 순서로 반환할 수 있으므로 페이지 매김이 반복되거나 결과를 건너뛰지 않습니다. 예를 들어 개체 ID를 사용하여 정렬하려면 `ID_Sort=asc`을(를) 사용합니다.

### 액세스 규칙 만들기

액세스 규칙을 만들어 객체에 액세스할 수 있는 사용자를 결정할 수 있습니다. 다음은 설정할 수 있는 액세스 규칙의 예입니다.

ID가 &quot;abc123&quot;인 사용자와만 공유되도록 프로젝트를 설정하려면 다음 요청을 사용하십시오.
<pre>GET /attask/api/v15.0/project/123abcxxxxxxxxxxxxxxxxxxxx?method=put &amp;updates={ accessRules: [ {accessorID: 'abc123', accessorObjCode: 'USER', coreAction: 'VIEW'} ] }</pre>또는 새 사람과만 공유하고 기존 권한을 그대로 유지하려면 다음을 수행합니다.
<pre>GET /attask/api/v15.0/project/123abcxxxxxxxxxxxxxxxxxxxxxx/share?method=put&amp;accessorID=abc123&amp;accessorObjCode=USER&amp;coreAction=VIEW</pre>기존 액세스 규칙을 검색하려면 다음과 같이 하십시오.
<pre>GET /attask/api/v15.0/project/123abcxxxxxxxxxxxxxxxxxxxxxxxx?fields=accessRules:*</pre>

## POST 동작

POST는 새 개체를 삽입합니다. 이 구문은 PUT과 동일하지만 몇 가지 예외가 있습니다. 새 개체는 아직 존재하지 않으므로 ID를 가지고 있지 않습니다. 이러한 이유로 URI에는 ID가 포함되지 않습니다.

### 개체 만들기

다음은 새 프로젝트 만들기 요청의 예입니다.
<pre>POST /attask/api/v15.0/project?name=새 프로젝트</pre>응답에는 새 ID 및 지정된 다른 필드와 함께 새로 생성된 프로젝트가 포함됩니다.

### 객체 복사

일부 객체는 복사가 지원됩니다. 이러한 객체 유형의 경우 copySourceID 매개 변수와 함께 게시하여 새 객체를 만들 수 있습니다. 예를 들어 다음 요청은 주어진 프로젝트를 복사하고 새 이름을 지정합니다.

```
POST /attask/api/v15.0/project?copySourceID=4c7...&name=Copied Project
```

### 문서 업로드

다음 API URL을 통해 문서를 업로드할 수 있습니다.
<pre>POST /attask/api/v15.0/upload</pre>API에서는 콘텐츠 유형이 다중 부분/양식 데이터여야 합니다. 파일의 매개 변수 이름은 uploadedFile이어야 합니다. 서버가 다음 JSON 데이터를 반환합니다.
<pre>{<br>    "handle": "4c7c08fa0000002ff924e298ee148df4"<br>}</pre>Workfront 문서를 만들 때 핸들을 사용하여 다음 URL에 게시할 수 있습니다.
<pre>POST /attask/api/v15.0/document?updates=&lbrace;<br>    이름: aFileName,<br>    핸들: abc...123, (파일 업로드의 핸들)<br>    docObjCode: PROJ, (또는 TASK, OPTASK 등)<br>    objID: abc...123,<br>    현재 버전:{version:v1.0,fileName:aFileName}<br></pre>

## PUT 동작

PUT은 기존 개체를 업데이트하는 데 사용됩니다.

PUT에 대한 응답은 GET과 동일합니다. 두 경우 모두 업데이트 후 서버가 개체의 새 상태를 반환합니다. GET 요청에 대한 응답을 변경하는 데 사용되는 모든 규칙은 반환할 추가 필드, 사용자 지정 데이터 지정 등과 같이 PUT에서도 작동합니다.

### 개체 편집

오브젝트에 대한 업데이트는 항상 오브젝트의 고유 URI를 사용하여 ID로 수행됩니다. 업데이트할 필드가 요청 매개 변수로 지정됩니다. 예를 들어 프로젝트 이름을 변경하려면 다음과 유사한 요청을 보낼 수 있습니다.
<pre>PUT /attask/api/v15.0/project/4c7...?name=새 프로젝트 이름 <br>PUT /attask/api/v15.0/project?id=4c7...&amp;name=새 프로젝트 이름</pre>업데이트에는 ID가 필요하므로 개체가 서버에 없으면 이 작업은 삽입되지 않고 실패합니다.

### JSON 편집 지정

다음 예에 표시된 것처럼 업데이트 요청 매개 변수 를 사용하여 JSON 구문을 사용하여 업데이트할 필드를 지정할 수 있습니다.
<pre>PUT /attask/api/v15.0/project/4c7...?업데이트= <br>{<br>     이름: "새 프로젝트 이름", <br>     상태: "현재", <br>     ... <br>}</pre>

### 중첩 업데이트 만들기

일부 객체에는 업데이트할 수 있는 개인 소유 컬렉션이 있습니다. 예를 들어 다음 예에서는 주어진 작업에 대한 기존 할당을 덮어쓰는 방법을 보여 줍니다.
<pre>PUT /attask/api/v15.0/task/4c7...?업데이트= <br>{<br>    할당: [ <br>        { <br>            assignedToID: "2222...54d0, <br>            assignmentPercent: 50.0 <br>        },{ <br>            roleID: "1111...54d0"<br>        } <br>    ] <br>}</pre>

>[!NOTE]
>
>최상위 수준에 대한 업데이트는 스파스(sparse)이지만 컬렉션이나 중첩된 객체에 대한 업데이트는 기존 컬렉션을 완전히 대체합니다. 오브젝트에 영향을 주지 않고 작업에 대한 단일 할당을 편집하려면 작업이 아닌 할당에 PUT을 사용하십시오.

다음 예제에서는 프로젝트를 공용 헬프 데스크 대기열로 만듭니다. 기존 대기열 속성이 대체됩니다.
<pre>PUT /attask/api/v15.0/project/4c7...?업데이트= <br>&lbrace; <br>    queueDef: { <br>        isPublic: 1 <br>    } <br></pre>

### 작업 요청 매개 변수 사용

일부 오브젝트는 간단한 편집 외에 수행할 수 있는 추가 작업을 지원합니다. 작업 요청 매개 변수를 사용하여 이러한 작업을 지정할 수 있습니다. 예를 들어 다음 요청은 주어진 프로젝트에 대한 타임라인을 다시 계산합니다.
<pre>PUT /attask/api/v15.0/project/4c7...?action=calculateTimeline<br><br>or<br><br>PUT /attask/api/v15.0/project/4c7.../calculateTimeline </pre>

### 객체 이동

다음은 한 프로젝트에서 다른 프로젝트로 작업을 이동하는 구문을 보여 줍니다.
<pre>PUT /attask/api/v15.0/task/4c7.../move?projectID=5d8...</pre>각 작업 유형에 대한 예는 여기에 제공됩니다(??).
<pre>PUT /attask/api/v15.0/project/1234/approveApproval<br><br>PUT /attask/api/v15.0/project/1234/calculateFinance<br><br>PUT /attask/api/v15.0/project/1234/calculateTimeline<br><br>PUT /attask/api/v15.0/project/1234/calculateDataExtension<br><br>PUT /attask/api/v15.0/project/1234/recallApproval<br><br>PUT /attask/api/v15.0/project/134/rejectApproval<br><br>PUT&rbrace;5 /attask/api/v15.0/task/1234/move<br><br>PUT /attask/api/v15.0/workitem/1234/markViewed</pre>이동 작업만 수행하면 작업 항목을 이동할 프로젝트를 지정하는 추가 속성을 식별할 수 있습니다.

다음은 각 작업 유형의 예입니다. 
<pre>PUT /attask/api/v15.0/project/1234?method=put&amp;updates={accessRules:[{accessorID: 'abc123', accessorObjCode: 'USER', coreAction: 'VIEW'}]}</pre>

### 개체 공유

다음 예제에서는 팀과 프로젝트를 공유하는 구문을 보여 줍니다.
<pre>PUT /attask/api/v15.0/project/123abcxxxxxxxxxxxxxxxxxxxxxx/share?accessorID=123abcxxxxxxxxxxxxxxxxxxxxxxxxxxxxxx&amp;accessorObjCode=TEAMOB</pre>객체를 편집할 때 다음 예와 유사한 업데이트를 전송하여 PUT을 수행하여 객체에 대한 모든 액세스 규칙을 바꿀 수 있습니다.
<pre>PUT /attask/api/v15.0/project/123abcxxxxxxxxxxxxxxxxxxxxxx?method=PUT&amp;updates={accessRules:[{accessorID:'123abcxxxxxxxxxxxxxxxxxxxxxxxxxxxxxx',accessorObjCode:'TEAMOB',coreAction:'VIEW'}]}</pre>다음 예제는 한 프로젝트에서 다른 프로젝트로 작업을 이동하는 구문을 보여 줍니다.
<pre>PUT /attask/api/v15.0/task/4c7.../move?projectID=5d8...</pre>

## DELETE 동작

DELETE은 개체를 제거합니다. 모든 경우에, URI는 서버가 지정된 데이터 및 그 의존자들을 제거하게 하는 매개 변수 force=true를 포함할 수 있다. 다음 예제에서는 URI에서 HTTP DELETE 메서드를 실행하여 작업이 삭제됩니다.
<pre>DELETE /attask/api/v15.0/task/4c78821c0000d6fa8d5e52f07a1d54d0 <br>DELETE /attask/api/v15.0/task?id=4c78821c0000d6fa8d5e52f07a1d54d0 <br>DELETE /attask/api/v15.0/task/4c788210000d6fa8d5e52f07a1d54d0?force=true <br>DELETE /attask/api/v15.0/task?id=4c78821c0000d6fa8d5e52f07a1d54d0?force=true</pre>

## 벌크 업데이트

벌크 업데이트 문은 단일 API 호출 내에서 여러 개체를 동시에 업데이트합니다. 벌크 만들기 API 호출은 다음 예에 표시된 대로 일반 업데이트 호출과 유사하게 빌드됩니다.
<pre>PUT /attask/api/v15.0/proj?updates=[{"name":"Test_Project_1"},{"name":"Test_Project_2"}]&amp;method=POST&amp;apiKey=123ab-cxxxxxxxxxxxxxxxxxxxxxxxxxxxxxx</pre>또는 <pre>푸시 /attask/api/v15.0/proj?updates=[{"name":"Test_Project_1"},{"name":"Test_Project_2"}]&amp;method=POST&amp;apiKey=123ab-cxxxxxxxxxxxxxxxxxxxxxxxxxxxxxx</pre>그러면 다음과 유사한 결과가 발생합니다.
<pre>데이터: [{<br>}    ID: "53ff8d3d003b438b57a8a784df38f6b3",<br>    이름: "Test_Project_1",<br>    objCode: "PROJ",<br>    percentComplete: 0,<br>    plannedCompletionDate: "2014-08-28T11:00:00:000-0400",<br>    plannedStartDate: "2014-08-28T11:00:00:000-0400",<br>    우선 순위: 0,<br>    projectedCompletionDate: "2014-08-28T16:12:00:000-0400",<br>    상태: "현재"<br>,<br>&lbrace;<br>    ID: "53ff8d49003b43a2562aa34eea3b6b10",<br>    이름: "Test_Project_2",<br>    objCode: "PROJ",<br>    percentComplete: 0usi,<br>    plannedCompletionDate: "2014-08-28T11:00:00:000-0400",<br>    plannedStartDate: "2014-08-28T11:00:00:000-0400",<br>    우선 순위: 0,<br>    projectedCompletionDate: "2014-08-28T16:12:00:000-0400",<br>    상태: "현재"<br>]</pre>다음과 유사한 대량 업데이트를 수행할 수도 있습니다.
<pre>PUT /attask/api/v15.0/proj?Umethod=PUT&amp;updates=[{"ID":"123abcxxxxxxxxxxxxxxxxxxxxxxxxxx","name":"Test_Project_1_ Edit"},{"ID":"123abcxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxx","name":"Test_Project_2_Edit"}]&amp;apiKey=123abcxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxx</pre>그러면 다음과 유사한 결과가 발생합니다.
<pre>데이터: [ &lbrace;<br>     ID: "53ff8e15003b461d4560f7f65a440078",<br>     이름: "Test_Project_1_Edit",<br>     objCode: "PROJ",<br>     percentComplete: 0,<br>     plannedCompletionDate: "2014-08-28T11:00:00:000-0400",<br>     plannedStartDate: "2014-08-28T11:00:00:000-0400",<br>     우선 순위: 0,<br>     projectedCompletionDate: "2014-08-28T16:16:00:000-0400",<br>     상태: "현재"<br>,<br>&lbrace;<br>    ID: "53ff8e19003b46238a58d303608de502",<br>    이름: "Test_Project_2_Edit",<br>    objCode: "PROJ",<br>    percentComplete: 0,<br>    plannedCompletionDate: "2014-08-28T11:00:00:000-0400",<br>    plannedStartDate: "2014-08-28T11:00:00:000-0400",<br>    우선 순위: 0,<br>    projectedCompletionDate: "2014-08-28T16:16:00:000-0400",<br>    상태: "현재"<br>]</pre>모든 작업이 동일한 트랜잭션에서 발생하도록 하려면 일괄 처리 API 호출에 "atomic=true"를 요청 매개 변수로 추가하십시오. 이렇게 하면 작업 중 하나라도 실패하면 모든 작업이 롤백됩니다.

>[!NOTE]
>
>원자 일괄 처리 작업은 &quot;success: true&quot; 또는 오류만 반환할 수 있습니다.

