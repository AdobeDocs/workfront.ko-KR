---
content-type: api
product-area: documents
navigation-topic: documents-webhooks-api
title: 문서 웹후크 인증
description: 문서 웹후크 인증
author: Becky
feature: Workfront API
role: Developer
exl-id: 2303c202-27c7-4922-a613-e9824910504c
source-git-commit: 14ff8da8137493e805e683e5426ea933f56f8eb8
workflow-type: tm+mt
source-wordcount: '438'
ht-degree: 0%

---

# 문서 웹후크 인증

## 인증

Adobe Workfront document webhooks는 OAuth2와 ApiKey라는 두 가지 서로 다른 인증 형식을 지원합니다. 두 경우 모두, Workfront은 API 호출을 수행할 때 헤더에 인증 토큰을 전달합니다.

### OAuth2

OAuth2를 통해 Workfront은 사용자를 대신하여 웹후크 공급자에 대해 승인된 API 호출을 수행할 수 있습니다. 이 작업을 수행하기 전에 사용자는 외부 문서 공급자 계정을 Workfront에 연결하고 Workfront에 권한을 부여해야 합니다

를 대신하여 행동할 수 있는 액세스 권한. 이 핸드셰이킹 프로세스는 각 사용자에 대해 한 번만 수행됩니다. 작동 방식은 다음과 같습니다.

1. 사용자가 Webhook 통합을 해당 계정에 연결하기 시작합니다. 현재 이 작업은 &quot;문서 추가&quot; 드롭다운 > &quot;서비스 추가&quot; > 사용자 정의 통합 이름을 클릭하여 수행됩니다.
1. Workfront은 사용자에게 인증 URL을 탐색합니다. 이 URL은 사용자가 외부 문서 공급자에 로그인하라는 메시지를 표시할 수 있습니다. 이 페이지는 웹후크 공급자 또는 외부 문서 관리 시스템에 의해 호스팅됩니다. 이렇게 하면 Workfront이 인증 URL에 &quot;state&quot; 매개 변수를 추가합니다. 아래 단계에서 동일한 값을 Workfront 반환 URI에 추가하여 이 값을 Workfront에 다시 전달해야 합니다.
1. 외부 시스템에 로그인한 후(또는 사용자가 이미 로그인한 경우) 사용자는 &quot;인증&quot; 페이지로 이동됩니다. 이 페이지는 Workfront이 사용자를 대신하여 일련의 작업을 수행하기 위해 액세스 권한을 요청하고 있음을 설명합니다.
1. 사용자가 &quot;허용&quot; 단추를 클릭하면 브라우저가 Workfront 리디렉션 URI 로 리디렉션되고 쿼리 문자열에 &quot;code=`<code>`&quot;이(가) 추가됩니다. OAuth2 사양에 따라 이 토큰은 수명이 짧습니다. 쿼리 문자열에는 &quot;state=`<sent_by_workfront>`&quot;도 있어야 합니다.
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

<!--
<div data-mc-conditions="QuicksilverOrClassic.Draft mode">
<h3>Adding Request Headers (optional)</h3>
<p>In addition to using either OAuth2 tokens or an ApiKey for authentication, Workfront can send a predefined set of headers to the webhook provider for every API call. A Workfront admin can setup set this up when&nbsp;registering or editing a Webook Integration, as described in the section above. See Registering a Webhook Integration.</p>
<p>For example, this can be used for Basic Authentication. To do this, the Workfront administrator would add the following Request Header information in the Custom Integration dialog:</p>
<p>&nbsp; &nbsp; &nbsp;Authorization Basic QWxhZGRpbjpvcGVuIHNlc2FtZQ==</p>
<p>where QWxhZGRpbjpvcGVuIHNlc2FtZQ== is a base-64 encoded string of "username:password". See Basic Authentication . Provided that this added, Workfront will pass this in the HTTP request header, in addition to other request headers:&nbsp;</p>
<p>-------------------------------</p>
<p>apiKey: 12345</p>
<p>username: johndoe@foo.com</p>
<p>Authorization: Basic QWxhZGRpbjpvcGVuIHNlc2FtZQ== ­­­­­­­­­­­­­­­­­­­­­­­­­­</p>
<p>-------------------------------</p>
</div>
-->
