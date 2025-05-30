---
content-type: api
product-area: documents
navigation-topic: documents-webhooks-api
title: 문서 웹후크 API
description: Adobe Workfront Document Webhooks는 Workfront이 외부 문서 공급자에 대해 승인된 API 호출을 수행하는 API 엔드포인트 세트를 정의합니다. 이를 통해 모든 문서 스토리지 공급자에 대한 미들웨어 플러그인을 생성할 수 있습니다.
author: Becky
feature: Workfront API
role: Developer
exl-id: 7ac2c6c8-1cb8-49df-8d63-a6b47ad02a13
source-git-commit: 48de4553478fc42d88d81ea953440337f6684e50
workflow-type: tm+mt
source-wordcount: '3649'
ht-degree: 2%

---


# 문서 웹후크 API

<!-- Audited: 5/2025 -->

Adobe Workfront Document Webhooks는 Workfront이 외부 문서 공급자에 대해 승인된 API 호출을 수행하는 API 엔드포인트 세트를 정의합니다. 이를 통해 모든 문서 스토리지 공급자에 대한 미들웨어 플러그인을 생성할 수 있습니다.

Webhook 기반 통합을 위한 사용자 경험은 Google Drive, Box 및 Dropbox과 같은 기존 문서 통합의 사용자 경험과 유사합니다. 예를 들어 Workfront 사용자는 다음 작업을 수행할 수 있습니다.

* 외부 문서 공급자의 폴더 구조 탐색
* 파일 검색
* Workfront에 파일 연결
* 외부 문서 공급자에 파일 업로드
* 문서의 축소판 보기

## 참조 구현

새 웹후크 구현의 개발을 바로 시작할 수 있도록 Workfront에서는 참조 구현을 제공합니다. 이에 대한 코드는 [https://github.com/Workfront/webhooks-app](https://github.com/Workfront/webhooks-app)에서 찾을 수 있습니다. 이 구현은 Java 기반이며 Workfront에서 네트워크 파일 시스템의 문서를 연결할 수 있도록 해 줍니다.

## Webhook 통합 등록

Workfront 관리자는 Workfront 내의 설정 > 문서 > 사용자 정의 통합으로 이동하여 회사에 대해 사용자 정의 웹후크 통합을 추가할 수 있습니다. 관리자는 설정 내의 사용자 정의 통합 페이지에서 기존 문서 Webhook 통합 목록을 볼 수 있습니다. 이 페이지에서 통합을 추가, 편집, 활성화 및 비활성화할 수 있습니다. 통합을 추가하려면 통합 추가 버튼을 클릭합니다.

### 사용 가능한 필드

통합을 추가할 때 관리자는 다음 필드에 값을 입력합니다.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th>필드 이름</th> 
   <th>설명</th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td>이름</td> 
   <td>이 통합의 이름입니다.</td> 
  </tr> 
  <tr> 
   <td>기본 API URL</td> 
   <td> <p>콜백 API의 위치입니다. 외부 시스템을 호출할 때 Workfront이 끝점 이름을 이 주소에 추가합니다. 예를 들어 관리자가 기본 API URL " https://www.mycompany.com/api/v1 "을 입력한 경우, Workfront은 다음 URL을 사용하여 문서의 메타데이터를 가져옵니다. https://www.mycompany.com/api/v1/metadata?id=1234</p> </td> 
  </tr> 
  <tr> 
   <td>요청 매개 변수</td> 
   <td> <p>모든 API 호출의 querystring에 추가할 선택 값. 예, access_type=offline.</p> </td> 
  </tr> 
  <tr> 
   <td>인증 유형</td> 
   <td>OAuth2 또는 ApiKey.</td> 
  </tr> 
  <tr> 
   <td>인증 URL</td> 
   <td> <p>(OAuth2만 해당) 사용자 인증에 사용되는 전체 URL입니다. Workfront은 OAuth 프로비저닝 프로세스의 일부로 사용자를 이 주소로 탐색합니다. <br><br>참고: Workfront에서 쿼리 문자열에 "state" 매개 변수를 추가합니다. 공급자는 Workfront 리디렉션 URI에 이 ID를 추가하여 Workfront에 다시 전달해야 합니다.</p> </td> 
  </tr> 
  <tr> 
   <td>토큰 엔드포인트 URL</td> 
   <td> <p>(OAuth2만 해당) OAuth2 토큰을 검색하는 데 사용되는 전체 API URL입니다. 웹후크 공급자 또는 외부 문서 공급자에 의해 호스팅됩니다.</p> </td> 
  </tr> 
  <tr> 
   <td>클라이언트 ID</td> 
   <td>(OAuth2만 해당) 이 통합을 위한 OAuth2 클라이언트 ID입니다.</td> 
  </tr> 
  <tr> 
   <td>클라이언트 암호</td> 
   <td> <p>(OAuth2만 해당) 이 통합을 위한 OAuth2 클라이언트 암호입니다.</p> </td> 
  </tr> 
  <tr> 
   <td>Workfront 리디렉션 URI</td> 
   <td> <p>(OAuth2 전용) 읽기 전용 필드이며 Workfront에서 생성합니다. 이 값은 외부 문서 공급자에 이 통합을 등록하는 데 사용됩니다. <br><br>참고: 인증 URL에 대해 위에서 설명한 대로 리디렉션을 수행할 때 공급자는 "state" 매개 변수와 그 값을 쿼리 문자열에 추가해야 합니다.</p></td> 
  </tr> 
  <tr> 
   <td>API 키</td> 
   <td>  <p>(ApiKey만 해당) Webhook 공급자에 대해 승인된 API 호출을 수행하는 데 사용됩니다. API 키는 Webhook 공급자가 발행합니다.</p></td> 
  </tr> 
 </tbody> 
</table>

 

## 인증

Workfront document webhooks는 OAuth2와 ApiKey라는 두 가지 서로 다른 인증 형식을 지원합니다. 두 경우 모두, Workfront은 API 호출을 수행할 때 헤더에 인증 토큰을 전달합니다.

### OAuth2

OAuth2를 통해 Workfront은 사용자를 대신하여 웹후크 공급자에 대해 승인된 API 호출을 수행할 수 있습니다. 이렇게 하기 전에 사용자는 외부 문서 공급자 계정을 Workfront에 연결하고 Workfront에 대신하여 행동할 수 있는 액세스 권한을 부여해야 합니다. 이 핸드셰이킹 프로세스는 각 사용자에 대해 한 번만 수행됩니다. 작동 방식은 다음과 같습니다.

1. 사용자가 Webhook 통합을 해당 계정에 연결하기 시작합니다. 현재 이 작업은 문서 추가 드롭다운 > 서비스 추가 > 사용자 정의 통합 이름을 클릭하여 수행합니다.
1. Workfront은 사용자를 인증 URL로 안내합니다. 인증 URL은 사용자가 외부 문서 공급자에 로그인하라는 메시지를 표시할 수 있습니다. 이 페이지는 웹후크 공급자 또는 외부 문서 관리 시스템에 의해 호스팅됩니다. 이렇게 하면 Workfront이 인증 URL에 &quot;state&quot; 매개 변수를 추가합니다. 아래 단계에서 동일한 값을 Workfront 반환 URI에 추가하여 이 값을 Workfront에 다시 전달해야 합니다.
1. 외부 시스템에 로그인한 후(또는 사용자가 이미 로그인한 경우) 인증 페이지로 이동합니다. 이 페이지는 Workfront이 사용자를 대신하여 일련의 작업을 수행하기 위해 액세스 권한을 요청하고 있음을 설명합니다.
1. 사용자가 허용 단추를 클릭하면 브라우저가 Workfront 리디렉션 URI 로 리디렉션되고 쿼리 문자열에 &quot;code=`<code>`&quot;이(가) 추가됩니다. OAuth2 사양에 따라 이 토큰은 수명이 짧습니다. 쿼리 문자열에는 &quot;state=`<sent_by_workfront>`&quot;도 있어야 합니다.
1. Workfront은 이 요청을 처리하고 인증 코드를 사용하여 토큰 끝점 URL에 대한 API를 호출합니다.
1. 토큰 끝점 URL은 새로 고침 토큰 및 액세스 토큰을 반환합니다.
1. Workfront은 이러한 토큰을 저장하고 이 사용자를 위한 webhook 통합을 완전히 프로비저닝합니다.
1. 이 시점부터 Workfront은 웹후크 공급자에 대해 승인된 API 호출을 수행할 수 있습니다. 이러한 호출을 수행하면 Workfront은 아래와 같이 HTTP 요청 헤더에 액세스 토큰을 전송합니다.

   ```
   -------------------------------  
   Authorization: Bearer [access_token] ­­­­­­­­­­­­­­­­­­­­­­­­­­  
   -------------------------------
   ```

1. 액세스 토큰이 만료된 경우, Workfront은 토큰 끝점 URL을 호출하여 새 액세스 토큰을 검색한 다음, 새 액세스 토큰으로 승인된 API 호출을 다시 시도합니다.

### API 키

ApiKey를 사용하여 웹후크 공급자에 대해 승인된 API 호출을 수행하는 것은 OAuth2보다 훨씬 간단합니다. API를 호출할 때 Workfront은 HTTP 요청 헤더에 ApiKey 및 Workfront 사용자 이름을 전달하기만 하면 됩니다.

```
-------------------------------

apiKey: 12345

username: johndoe@foo.com

-------------------------------
```

Webhook 공급자는 사용자 이름을 사용하여 사용자별 권한을 적용할 수 있습니다. 이 기능은 두 시스템이 SSO(Single Sign-On)를 사용하여 LDAP에 연결할 때 가장 적합합니다.

### 요청 헤더 추가(선택 사항)

인증에 OAuth2 토큰 또는 ApiKey를 사용하는 것 외에도 Workfront은 모든 API 호출에 대해 사전 정의된 헤더 집합을 Webhook 공급자로 전송할 수 있습니다. Workfront 관리자는 위의 섹션에 설명된 대로 Webook 통합을 등록하거나 편집할 때 이 설정을 수행할 수 있습니다.

예를 들어 기본 인증에 사용할 수 있습니다. 이를 위해 Workfront 관리자는 사용자 정의 통합 대화 상자에 다음 요청 헤더 정보를 추가합니다.

   인증 기본 QWxhZGRpbjpvcGVuIHNlc2FtZQ==

여기서 QWxhZGRpbjpvcGVuIHNlc2FtZQ==는 &quot;username:password&quot;의 base-64 인코딩 문자열입니다. 기본 인증을 참조하십시오. 이 기능이 추가되면 Workfront은 다른 요청 헤더 외에 HTTP 요청 헤더에서도 이 기능을 전달합니다.

```
­­­­­­­­­­­­­­­­­­­­­­­­­­-------------------------------

apiKey: 12345

username: johndoe@foo.com

Authorization: Basic QWxhZGRpbjpvcGVuIHNlc2FtZQ== ­­­­­­­­­­­­­­­­­­­­­­­­­­

-------------------------------
```

## API 사양

다음은 문서 웹후크가 작동하기 위해 웹후크 공급자가 구현해야 하는 API 목록입니다.

### OAuth2 토큰 가져오기(OAuth2 인증만 필요)

인증된 사용자에 대한 OAuth2 새로 고침 토큰 및 액세스 토큰을 반환합니다. 사용자가 문서 공급자를 프로비저닝할 때 한 번 호출됩니다. 업데이트된 액세스 토큰을 얻기 위한 후속 호출이 수행됩니다.

HTTP 요청 POST /any/url

URL은 구성이 가능하며 사용자 지정 통합 설정 페이지의 토큰 끝점 URL 값에 해당합니다.

**쿼리 매개 변수**

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th>이름</th> 
   <th>필수</th> 
   <th>설명</th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td>grant_type</td> 
   <td>예</td> 
   <td> <p>값에는 "authorization_code" 또는 "refresh_token"이 포함됩니다. 지정된 값은 두 매개 변수 중 코드 또는 refresh_token 중 어느 매개 변수가 이 API 호출에 전달될지 나타냅니다.</p> </td> 
  </tr> 
  <tr> 
   <td>코드</td> 
   <td>종속</td> 
   <td> <p>사용자가 부여 단추를 클릭한 직후 Workfront으로 전송된 인증 코드입니다. 권한 부여 유형이 "authorization_code"인 경우에만 필요합니다. 인증 코드는 수명이 짧아야 하며 일반적으로 10분 이내에 만료됩니다.</p> </td> 
  </tr> 
  <tr> 
   <td>refresh_token</td> 
   <td>종속</td> 
   <td> <p>이전 access_token이 만료된 경우 새 access_token을 검색하기 위해 후속 호출을 할 때만 필요합니다. 이 값을 보낼 때 grant_type 매개 변수를 "refresh_token"으로 설정합니다.</p> </td> 
  </tr> 
  <tr> 
   <td>client_id</td> 
   <td>예</td> 
   <td>이 사용자 정의 통합을 위해 Workfront에 구성된 클라이언트 ID입니다.</td> 
  </tr> 
  <tr> 
   <td>클라이언트 암호</td> 
   <td>예</td> 
   <td> 이 사용자 정의 통합을 위해 Workfront에 구성된 클라이언트 암호.</td> 
  </tr> 
 </tbody> 
</table>

 

**응답**

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th>이름</th> 
   <th>유형 </th> 
   <th>설명</th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td>access_token </td> 
   <td>문자열</td> 
   <td> <p>사용자 대신 승인된 API 호출을 수행하는 데 사용되는 토큰입니다. 승인되지 않은 API 호출을 방지하기 위해 만료되어야 합니다.</p> </td> 
  </tr> 
  <tr> 
   <td>refresh_token </td> 
   <td>문자열</td> 
   <td> <p>이 API 메서드를 호출하여 새 access_token을 검색하는 데 사용되는 장기 토큰입니다.</p> </td> 
  </tr> 
  <tr> 
   <td>expires_in </td> 
   <td>길게</td> 
   <td>  <p>(선택 사항) access_token이 만료되기 전 시간(초)으로, 일반적으로 3,600입니다.</p></td> 
  </tr> 
 </tbody> 
</table>

 

**예**

```
POST /oauth2/token
grant_type=authorization_code
code=d9ac7asdf6asdf579d7a8
client_id=123456
client_secret=6asdf7a7a9a4af
```


**응답**

```
{
"access_token":"ad8af5ad5ads759", 
"refresh_token":"9a0h5d87d808ads", 
"expires_id":"3600" 
}
```

### 파일 또는 폴더에 대한 메타데이터 가져오기

지정된 파일 또는 폴더에 대한 메타데이터를 반환합니다.

**URL**

GET /metadata?id=[문서 또는 폴더 ID]

**쿼리 매개 변수**

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th>이름 </th> 
   <th>설명</th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td>id</td> 
   <td>  <p>웹후크 공급자가 참조하는 파일 또는 폴더의 ID. Workfront의 문서 ID와 다릅니다. 루트 디렉토리의 메타데이터를 가져오려면 값 '/'를 사용합니다.</p><p>참고: ID의 최대 길이는 255자입니다.</p></td> 
  </tr> 
 </tbody> 
</table>

 

**응답**

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th>이름 </th> 
   <th>유형 </th> 
   <th>설명</th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td>제목 </td> 
   <td>문자열 </td> 
   <td>문서 또는 폴더의 이름입니다.</td> 
  </tr> 
  <tr> 
   <td>종류 </td> 
   <td>문자열 </td> 
   <td>이 항목이 파일 또는 폴더('file' 또는 'folder')인지 지정합니다.</td> 
  </tr> 
  <tr> 
   <td>id</td> 
   <td>문자열 </td> 
   <td>파일 또는 폴더의 ID입니다.</td> 
  </tr> 
  <tr> 
   <td>viewLink</td> 
   <td>문자열 </td> 
   <td> <p>사용자가 브라우저 창에서 문서를 보는 데 사용하는 URL 경로입니다. URL은 문서 공급자나 기본 외부 스토리지 공급자에 의해 호스팅될 수 있습니다.</p> </td> 
  </tr> 
  <tr> 
   <td>downloadLink</td> 
   <td>문자열 </td> 
   <td> <p>사용자가 브라우저 창에서 문서를 다운로드하는 데 사용하는 URL 경로입니다. URL은 문서 공급자나 기본 외부 스토리지 공급자에 의해 호스팅될 수 있습니다.</p> </td> 
  </tr> 
  <tr> 
   <td>mimeType</td> 
   <td>문자열 </td> 
   <td>(선택 사항) 파일의 MIME 유형입니다.</td> 
  </tr> 
  <tr> 
   <td>날짜 수정</td> 
   <td>문자열 </td> 
   <td>이 파일이 마지막으로 수정된 시간(형식이 지정된 RFC 3339 타임스탬프).</td> 
  </tr> 
  <tr> 
   <td>크기</td> 
   <td>길이</td> 
   <td>(선택 사항) 파일 크기(바이트)입니다.</td> 
  </tr> 
  <tr> 
   <td>읽기 전용</td> 
   <td>부울</td> 
   <td><p> (선택 사항) 이 파일 또는 폴더가 인증된 사용자에게 읽기 전용인지 여부를 나타냅니다.</p><p> </p></td> 
  </tr> 
 </tbody> 
</table>

**예:** `https://www.acme.com/api/metadata?id=12345`

**응답**

```
{
"title":"My Document", 
"kind":"file"
"id":"12345", 
"viewLink":"https://www.acme.com/viewDocument?id=12345", 
"downloadLink":"https://www.acme.com/downloadDocument?id=12345",
"mimeType":"image/png",
"dateModified":"2014­06­05T17:39:45.251Z",
"size": "32554694"
}
```

>[!NOTE]
>
>오류 처리는 모든 API 호출에서 일관되어야 합니다. 자세한 내용은 아래의 오류 처리 섹션을 참조하십시오.

### 폴더의 항목 목록 가져오기

지정된 폴더의 파일 및 폴더에 대한 메타데이터를 반환합니다.

**URL**

GET /files

**쿼리 매개 변수**

| 이름  | 설명 |
|---|---|
| parentId  | 폴더 ID입니다. 루트 디렉토리의 메타데이터를 가져오려면 값 &#39;/&#39;를 사용합니다. |

{style="table-layout:auto"}

Document Webhooks API는 현재 페이지 매김을 지원하지 않습니다.

**응답**

파일 및 폴더 목록이 포함된 JSON. 각 항목에 대한 메타데이터는 /metadata 끝점에서 반환된 메타데이터와 동일합니다.

**예:** `https://www.acme.com/api/files?parentId=123456`

**응답**

```
[
{
"title":"Folder A",
"kind":"folder",
"id":"2lj23lkj",
"viewLink":"https://www.acme.com/viewDocument?id=2lj23lkj",
"downloadLink":"https://www.acme.com/downloadDocument?id=2lj23lkj",
"mimeType":"",
"dateModified":"2014­06­05T17:39:45.251Z",
"size":"" 
},
{
"title":"My Document",
"kind":"file",
"id":"da8cj234"
"viewLink":"https://www.acme.com/viewDocument?id=da8cj234",
"downloadLink":"https://www.acme.com/downloadDocument?id=da8cj234",
"mimeType":"image/png",
"dateModified":"2014­06­05T17:39:45.251Z",
"size":"32554694"
},
]
```

### 검색

검색에서 반환된 파일 및 폴더에 대한 메타데이터를 반환합니다. 전체 텍스트 검색이나 일반 데이터베이스 쿼리로 구현할 수 있습니다. Workfront은 사용자가 외부 파일 브라우저에서 검색을 수행할 때 /search 끝점을 호출합니다.

**URL**

GET /search

**쿼리 매개 변수**

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th>이름 </th> 
   <th>설명</th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td>쿼리</td> 
   <td>검색어 또는 구.</td> 
  </tr> 
  <tr> 
   <td>parentId</td> 
   <td> <p>(선택 사항) 검색이 실행되는 폴더 ID입니다. <br><br>참고: Workfront의 향후 기능을 위한 자리 표시자입니다. 현재 Workfront은 이 매개 변수를 전달하지 않습니다. </p> </td> 
  </tr> 
  </tbody> 
</table>

Document Webhooks API는 현재 페이지 매김을 지원하지 않습니다.

 

**응답**

쿼리와 일치하는 파일 및 폴더에 대한 메타데이터 목록이 포함된 JSON입니다. &quot;일치&quot;를 구성하는 것은 웹후크 공급자에 의해 결정됩니다. 가장 좋은 방법은 전체 텍스트 또는 파일 이름 기반 검색을 수행하는 것입니다.

**예:** `https://www.acme.com/api/search?query=test-query`

**응답**

```
[
{ File/Folder Metadata },
{ File/Folder Metadata }
]
```

### 문서 콘텐츠 가져오기

문서에 대한 원시 바이트를 반환합니다.

**URL**

GET /download

**쿼리 매개 변수**

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th>이름 </th> 
   <th>설명</th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td> <p>id</p> </td> 
   <td> 문서 ID.</td> 
  </tr> 
 </tbody> 
</table>

 

**응답**

문서의 원시 바이트입니다.

**예:** `https://www.acme.com/api/download?id=123456`

### 문서에 대한 썸네일 가져오기

문서에 대한 원시 썸네일 바이트를 반환합니다.

**URL**

GET /thumbnail

**쿼리 매개 변수**

| 이름  | 설명 |
|---|---|
| id  | 문서 ID. |
| 크기  | 썸네일의 너비입니다. |

{style="table-layout:auto"}

 

**응답**

원시 썸네일 바이트.

**예:** `https://www.acme.com/api/thumbnail?id=123456`

### 파일 업로드 - 2부 중 1부

문서 스토리지 공급자에 파일을 업로드하는 것은 2개의 개별 API 엔드포인트가 필요한 2단계 프로세스입니다. Workfront은 /uploadInit 를 호출하여 업로드 프로세스를 시작합니다. 이 끝점은 문서 ID를 반환하며, 문서 바이트를 업로드할 때 /upload에 전달됩니다. 기본 문서 스토리지 시스템에 따라 길이가 0인 문서를 만든 다음 나중에 문서 내용을 업데이트해야 할 수 있습니다.

이 사양의 버전 1.1에 추가된 문서 ID 및 문서 버전 ID를 사용하여 Workfront에서 추가 정보를 검색할 수 있습니다. 예를 들어 문서 관리 시스템에서 문서에 대한 추가 정보를 원하는 경우 웹후크 구현 코드는 문서 ID를 사용하여 Workfront의 RESTful API를 사용하여 해당 정보를 검색할 수 있습니다. 이 정보는 문서와 포함된 작업, 문제 또는 프로젝트의 사용자 정의 데이터 필드에서 가져오는 것이 좋습니다.

**URL**

POST /uploadInit

**쿼리 매개 변수**

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th>이름 </th> 
   <th>설명</th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td>parentId </td> 
   <td>웹후크 공급자가 참조하는 상위 폴더 ID입니다.</td> 
  </tr> 
  <tr> 
   <td>파일 이름 </td> 
   <td>문서의 이름입니다.</td> 
  </tr> 
  <tr> 
   <td>documentId</td> 
   <td> <p>Workfront 문서 ID(버전 1.1에 추가됨)입니다.</p> <p> </p> </td> 
  </tr> 
  <tr> 
   <td>documentVersionId </td> 
   <td>Workfront 문서 버전 ID(버전 1.1에 추가됨)입니다.</td> 
  </tr> 
 </tbody> 
</table>

 

**응답**

/metadata 끝점에 정의된 파일의 메타데이터입니다.

**예:** `https://www.acme.com/api/uploadInit?parentId=12345&filename=new-file.png&docu mentId=511ea6e000023edb38d2effb2f4e6e3b&documentVersionId=511ea6e000023edb38d2e ffb2f4e6e3b`

**응답**

`[file_metadata]`에 문서 공급자가 사용하는 새 문서 ID가 포함되어 있습니다.

### 파일 업로드 - 2부

문서의 바이트를 웹후크 공급자에 업로드합니다.

**URL**

PUT /upload

**쿼리 매개 변수**

| 이름  | 설명 |
|---|---|
| id  |  방금 만든 문서 ID입니다. |


 

**요청 본문**

문서에 대한 원시 콘텐츠 바이트입니다.

**응답**

```
{
"result": "success"
}
```

또는

```
{
"result": "fail"
}
```

**예:** `https://www.acme.com/api/upload?id=1234` *[업데이트 스트림에 포함된 문서 바이트]*

**응답**

```
{
"result":"success"
}
```

### 서비스에 대한 정보 가져오기 

(릴리스 날짜 - TBD) 기능 등 서비스에 대한 정보를 반환합니다. Workfront은 이 정보를 사용하여 Workfront의 사용자 인터페이스를 사용자 정의합니다. 예를 들어 Webhook 구현에 일부 사용자 지정 작업이 포함된 경우 JSON은 해당 작업을 JSON에 나열해야 합니다. 그러면 사용자는 Workfront에서 이러한 작업을 호출할 수 있습니다.

**URL**

GET /serviceInfo

쿼리 매개변수

없음. 또한 이 끝점에 대한 호출에는 인증이 필요하지 않습니다.

**응답**

이 서비스에 대한 정보가 포함된 JSON.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th>이름</th> 
   <th>유형 </th> 
   <th>설명</th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td>webhookVersion </td> 
   <td>문자열 </td> 
   <td>이 서비스에서 구현한 웹후크 버전. 이 사양의 맨 위에 나열된 버전 번호입니다.</td> 
  </tr> 
  <tr> 
   <td>버전 </td> 
   <td>문자열 </td> 
   <td>이 서비스의 내부 버전 번호입니다. 이 번호는 웹후크 서비스 공급업체에 의해 결정되며 정보 제공 용도로만 사용됩니다.<br><br></td> 
  </tr> 
  <tr> 
   <td>게시자 </td> 
   <td>문자열 </td> 
   <td>Webhook 구현을 제공하는 회사의 이름입니다.</td> 
  </tr> 
  <tr> 
   <td>availableEndpoints</td> 
   <td>문자열 </td> 
   <td>이 서비스에서 구현한 API 끝점이 포함된 목록입니다. 이 확장은 Workfront의 사용자 인터페이스가 webhook 공급자가 제공하는 기능을 반영하도록 하는 데 사용할 수 있습니다. 목록의 각 항목에는 끝점의 이름이 포함되어야 합니다(예: "search").</td> 
  </tr> 
  <tr> 
   <td>사용자 지정 작업 </td> 
   <td>문자열</td> 
   <td>  <p>이 웹후크에서 구현한 사용자 지정 작업이 포함된 목록입니다. 각 목록 항목에는 이름과 표시 이름이 포함됩니다. 표시 이름이 Workfront의 문서 작업 드롭다운에 나타납니다. 드롭다운에서 항목을 클릭하면 /customAction 끝점을 호출하여 웹 후크에서 작업을 호출합니다.</p></td> 
  </tr> 
 </tbody> 
</table>

**예:** https://www.acme.com/api/serviceInfo

**반환**

```
{
"webhook version": "1.2", "version": "1.0", "publisher": "Acme, LLC", "availableEndpoints": ["files", "metadata", "search", "download"

"thumbnail", "uploadInit", "upload" ], "customActions" [
{
"name": "archive", "displayName": "Archive" }, {

"name": "doSomethingElse", "displayName": "Do Something" }, ] }
```

### 폴더 만들기

(버전 1.2에 추가됨) 특정 디렉터리에 폴더를 만듭니다.
URL

POST /createFolder

**쿼리 매개 변수**

| 이름  | 설명 |
|---|---|
| parentId  | 폴더를 만들 폴더 ID입니다. |
| 이름  | 새 폴더의 이름입니다. |

{style="table-layout:auto"}

 

**응답**

/metadata 끝점에 정의된 대로 새로 생성된 폴더의 메타데이터입니다.

**예:** `POST https://www.acme.com/api/createFolder`

```
-------------------------------

parentId=1234

name=New Folder ­­­­­­­­­­­­­­­­­­­­­­­­­­­­­­­­­­­­

-------------------------------
```

반환

```
{"title":"New Folder", 
 "kind":"folder""id":"5678",
 "viewLink":"",
 "downloadLink":"",
 "mimeType":"",
 "dateModified":"2014­06­05T17:39:45.251Z" 
 "size": "" 
 }
```

### 문서 또는 폴더 삭제

(릴리스 날짜 - TBD) 외부 시스템에서 해당 ID가 있는 문서 또는 폴더를 삭제합니다. 폴더를 삭제하면 해당 컨텐츠도 삭제됩니다.

URL

PUT /delete

**쿼리 매개 변수**

| 이름  | 설명 |
|---|---|
| documentId  | 삭제할 문서 ID입니다. |
| folderId  | 삭제할 폴더 ID입니다. |

{style="table-layout:auto"}

응답 아래 오류 처리 섹션에 지정된 대로 성공 또는 실패를 나타내는 JSON 문자열입니다.

**예:** PUT https://www.acme.com/api/delete id=1234

반환

```
{
"status": "success" 
}
```

반환

```
{
"status": "failure", "error": "File not found"
}
```


### 문서 또는 폴더 이름 바꾸기

(릴리스 날짜 - TBD) 외부 시스템에서 특정 ID로 문서 또는 폴더의 이름을 바꿉니다.

URL

PUT /rename

**쿼리 매개 변수**

| 이름  | 설명 |
|---|---|
| id | 이름을 바꿀 문서 또는 폴더 ID입니다. |
| 이름  | 문서 또는 폴더의 새 이름입니다. |

{style="table-layout:auto"}

 

응답

아래 오류 처리 섹션에 지정된 대로 성공 또는 실패를 나타내는 JSON 문자열입니다.

**예:**

`PUT https://www.acme.com/api/rename`

```
-------------------------------

id=1234

name=Folder B ­­­­­­­­­­­­­­­­­­­­­­­­­­­­­­­­­­­­

-------------------------------
```

```
{
"status": "success" 
}returns
{
"status": "failure", error: "Folder cannot be renamed because a folder with that name already exists." 
}
```

### 사용자 지정 작업 수행

(릴리스 날짜 - TBD) 이 끝점을 사용하면 Workfront 사용자(또는 자동화된 워크플로 이벤트)가 외부 시스템에서 작업을 수행할 수 있습니다. /customAction 끝점이 &quot;name&quot; 매개 변수를 허용하므로 웹후크 공급자가 여러 사용자 지정 작업을 구현할 수 있습니다.

웹후크 공급자는 customActions 아래의 /serviceInfo 응답에 작업을 포함하여 사용자 지정 작업을 Workfront에 등록합니다. Workfront은 설정 > 문서 > 사용자 정의 통합에서 웹후크 공급자를 설정하거나 새로 고칠 때 이 목록을 로드합니다.\
![사용자 지정 작업 수행](assets/mceclip0-350x262.png)

사용자는 문서 작업 아래에서 섹션을 선택하여 사용자 지정 작업을 트리거할 수 있습니다.\
![사용자 지정 작업 트리거](assets/mceclip1-350x95.png)

**URL**

GET /customAction

**쿼리 매개 변수**

<table style="table-layout:auto">
 <col>
 <col>
 <thead>
  <tr>
   <th>이름 </th>
   <th>설명</th>
  </tr>
 </thead>
 <tbody>
  <tr>
   <td><p>이름</p></td>
   <td><p>수행할 작업 유형을 지정하는 식별자입니다. 이 값은 /serviceInfo 끝점에서 반환된 나열된 customAction 값 중 하나에 해당합니다.</p></td>
  </tr>
  <tr>
   <td>documentId </td>
   <td>작업이 수행되는 Workfront 문서 ID입니다.</td>
  </tr>
  <tr>
   <td>documentVersionId </td>
   <td>작업이 수행되는 Workfront 문서 버전 ID입니다.</td>
  </tr>
 </tbody>
</table>

 

**응답**

아래 오류 처리 섹션에 지정된 대로 성공 또는 실패를 나타내는 JSON 문자열입니다. 실패 시(예: 상태 = &quot;failure&quot;) Workfront은 사용자에게 제공된 오류 메시지를 표시합니다.

**예:** https://sample.com/webhooks/customName?name=archive&amp;documentId=5502082c003a4f30 ddec2fb2b739cb7c&amp;documentVersionId=54b598a700e2342d6971597a5df1a8d3

응답

```
{
"status": "success" 
}
```


## 오류 처리

API 요청을 처리할 때 문제가 발생할 수 있습니다. 이 작업은 모든 API 종단점에서 일관된 방식으로 처리되어야 합니다. 오류가 발생하면 웹후크 공급자는 다음 작업을 수행합니다.

* 응답 헤더에 오류 코드를 포함합니다. 오류 코드는 다음과 같습니다.

   * 403 - 사용할 수 없음. 요청 토큰이 누락되었거나 잘못되었거나 토큰과 연결된 자격 증명에 지정된 리소스에 대한 액세스 권한이 없음을 나타냅니다. OAuth 기반 웹후크 공급자의 경우 Workfront은 새 액세스 토큰 검색을 시도합니다.
   * 404 - 찾을 수 없음. 지정한 파일 또는 폴더가 없음을 나타냅니다.
   * 500 - 내부 서버 오류. 기타 모든 유형의 오류.

* 다음 형식을 사용하여 응답 본문의 오류를 설명합니다.


```
{
"status": "error"
"error": "Sample error message" 
}
```


## 테스트

문서 Webhook 구현이 올바르게 작동하는지 확인하려면 다음 테스트를 실행합니다. Workfront 웹 인터페이스를 거치고 Webhook 구현의 끝점을 간접적으로 히트하는 수동 테스트입니다.

### 전제 조건

이러한 테스트를 실행하려면 다음이 필요합니다.

* ADM(Advanced Document Management)이 활성화된 Workfront 계정
* 시스템 관리자 권한이 있는 이 계정의 Workfront 사용자입니다.
* Workfront에 액세스할 수 있는 HTTP 끝점을 제공하는 문서 Webhook 인스턴스.

또한 이러한 테스트에서는 설정 > 문서 > 사용자 정의 통합 아래의 Workfront에서 문서 Webhook 인스턴스를 이미 등록했다고 가정합니다.

### 테스트 1: 사용자를 위한 Document Webhook 서비스 제공

OAuth 기반 웹후크 공급자에 대한 인증 URL 및 토큰 끝점 URL을 테스트합니다.

1. Workfront에서 상단 탐색 막대에 있는 문서 링크를 클릭하여 기본 문서 페이지로 이동합니다.
1. Add Documents 드롭다운을 클릭하고 Add Service 아래에서 Document Webhook 서비스를 선택합니다.
1. (OAuth 서비스만 해당) 이전 단계를 완료한 후 서비스의 OAuth2 인증 페이지 로드가 팝업 창에 표시됩니다. (참고: 먼저 서비스에 로그인하라는 메시지가 표시될 수 있습니다.) 인증 페이지에서 [신뢰] 또는 [허용] 단추를 클릭하여 Workfront에 사용자 계정에 대한 액세스 권한을 부여합니다.
1. 서비스가 문서 추가 드롭다운에 추가되었는지 확인합니다. 처음에 표시되지 않으면 브라우저를 새로 고침해 보십시오.

### 테스트 2: Workfront에 문서 연결 /files, /metadata

1. Workfront에서 상단 탐색 막대에 있는 문서 링크를 클릭하여 기본 문서 페이지로 이동합니다.
1. 문서 추가에서 Document Webhook 서비스를 선택합니다.
1. 모달에서 폴더 구조를 탐색합니다.
1. 폴더 구조를 제대로 탐색할 수 있는지 확인합니다.
1. 문서를 선택하여 Workfront에 연결합니다.

### 테스트 3: 컨텐츠 관리 시스템의 문서로 이동합니다.

/metadata(특히 viewLink) 끝점을 테스트합니다.

1. Workfront에 문서를 연결합니다.
1. 문서를 선택하고 열기 링크를 클릭합니다.
1. 문서가 새 탭에서 열리는지 확인합니다.

### 테스트 4: 콘텐츠 관리 시스템의 문서(로그인 포함)로 이동합니다.

/metadata(특히 viewLink) 끝점을 테스트합니다.

1. 컨텐츠 관리 시스템에서 로그아웃되었는지 확인합니다.
1. Workfront에 문서를 연결합니다.
1. 문서를 선택하고 열기 링크를 클릭합니다.
1. 컨텐츠 관리 시스템의 로그인 화면이 새 탭에 로드되는지 확인합니다.
1. 로그인하고 문서에 연결되었는지 확인합니다.

### 테스트 5: 컨텐츠 관리 시스템에서 문서 다운로드

/metadata(특히 downloadLink) 끝점을 테스트합니다.

1. Workfront에 문서를 연결합니다.
1. 문서를 선택하고 다운로드 링크를 클릭합니다.
1. 다운로드가 시작되는지 확인합니다.

### 테스트 6: 콘텐츠 검색

다음 끝점을 테스트합니다. /search

1. Workfront에서 상단 탐색 막대에 있는 문서 링크를 클릭하여 기본 문서 페이지로 이동합니다.
1. 문서 추가에서 Document Webhook 서비스를 선택합니다.
1. 모달에서 검색을 수행합니다.
1. 검색 결과가 올바른지 확인합니다.

### 테스트 7: Workfront에서 컨텐츠 관리 시스템으로 문서 보내기

/files, /uploadInit, /upload 끝점을 테스트합니다.

1. Workfront에서 상단 탐색 막대에 있는 문서 링크를 클릭하여 기본 문서 페이지로 이동합니다.
1. 컴퓨터에서 Workfront으로 문서를 업로드합니다.
1. 문서 세부 정보 페이지로 이동합니다.
1. Document Actions 드롭다운에서 Send To...에 있는 Document Webhook 서비스를 선택합니다.
1. 원하는 대상 폴더로 이동하고 저장 버튼을 클릭합니다.
1. 문서가 컨텐츠 관리 시스템의 올바른 위치에 업로드되었는지 확인합니다.

### 테스트 8: Workfront에서 썸네일 보기

다음 끝점을 테스트합니다. /thumbnail

1. Workfront에 문서를 연결합니다.
1. 목록에서 문서를 선택합니다.
1. 축소판이 오른쪽 패널에 표시되는지 확인합니다.

### 테스트 9: 컨텐츠 바이트 가져오기

다음 끝점을 테스트합니다. /download

1. Workfront에 문서를 연결합니다.
1. 문서 세부 정보 페이지로 이동합니다.
1. [문서 작업] > [전송 대상...] > [Workfront]를 선택하여 Workfront으로 문서를 전송합니다. 이렇게 하면 Workfront에 새 문서 버전이 만들어집니다.
1. 다운로드 링크를 클릭하여 Workfront에서 문서를 다운로드합니다.

### 테스트 10: 액세스 토큰 새로 고침(OAuth2 웹후크 공급자만 해당)

다음 끝점을 테스트합니다. 토큰 끝점 URL

1. 사용자를 위한 Document Webhook 서비스 제공.
1. 사용자의 액세스 토큰이 시간 초과될 때까지 기다리거나 외부 시스템에서 수동으로 무효화하여 무효화합니다.
1. Workfront에서 액세스 토큰을 새로 고칩니다. 예를 들어 문서를 Workfront에 연결하여 이 작업을 수행할 수 있습니다. 문서로 이동하여 연결할 수 있으면 액세스 토큰이 성공적으로 새로 고쳐졌다는 것을 알 수 있습니다.

>[!NOTE]
>
>현재 연결된 문서에는 전송 대상...을 사용할 수 없습니다. Workfront에서 추가합니다. Postman과 같은 REST 클라이언트를 사용하여 수동으로 끝점을 눌러 /download 끝점을 테스트할 수 있습니다. 또는 디지털 증명을 생성하여 /download 끝점을 테스트할 수 있습니다. 디지털 증명을 활성화하려면 Workfront에 문의하십시오.

## 버전

* 버전 1.0(릴리스 날짜 - 2015년 5월)

   * 초기 사양

* 버전 1.1(릴리스 날짜 - 2015년 6월)

   * 업데이트된 /uploadInit - 추가된 documentId 및 documentVersionId

* 버전 1.2(릴리스 날짜 - 2015년 10월)

   * /createFolder 추가됨

