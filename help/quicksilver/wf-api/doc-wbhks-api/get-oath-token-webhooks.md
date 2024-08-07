---
content-type: api
product-area: documents
navigation-topic: documents-webhooks-api
title: OAuth2 토큰 가져오기
description: OAuth2 토큰 가져오기
author: Becky
feature: Workfront API
role: Developer
exl-id: f3a2630d-d34e-4d36-b2bb-707ba0d3258e
source-git-commit: 14ff8da8137493e805e683e5426ea933f56f8eb8
workflow-type: tm+mt
source-wordcount: '253'
ht-degree: 3%

---


# OAuth2 토큰 가져오기

## OAuth2 토큰 가져오기

인증된 사용자에 대한 OAuth2 새로 고침 토큰 및 액세스 토큰을 반환합니다. 사용자가 문서 공급자를 프로비저닝할 때 한 번 호출됩니다. 업데이트된 액세스 토큰을 얻기 위한 후속 호출이 수행됩니다.

**URL**

POST /any/url

URL은 구성이 가능하며 사용자 지정 통합 설정 페이지의 토큰 끝점 URL 값에 해당합니다.

### 쿼리 매개변수

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
   <td><p>값에는 "authorization_code" 또는 "refresh_token"이 포함됩니다. 지정된 값은 두 매개 변수 중 코드 또는 refresh_token 중 어느 매개 변수가 이 API 호출에 전달될지 나타냅니다.</p></td>
  </tr>
  <tr>
   <td>코드</td>
   <td>종속</td>
   <td><p>사용자가 "부여" 버튼을 클릭한 직후 Adobe Workfront으로 전송된 인증 코드입니다. 권한 부여 유형이 "authorization_code"인 경우에만 필요합니다. 인증 코드는 수명이 짧아야 하며 일반적으로 10분 이내에 만료됩니다.</p></td>
  </tr>
  <tr>
   <td>refresh_token</td>
   <td>종속</td>
   <td><p>이전 access_token이 만료된 경우 새 access_token을 검색하기 위해 후속 호출을 할 때만 필요합니다. 이 값을 보낼 때 grant_type 매개 변수를 "refresh_token"으로 설정합니다.</p></td>
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

 

## 응답

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
   <td><p>사용자 대신 승인된 API 호출을 수행하는 데 사용되는 토큰입니다. 승인되지 않은 API 호출을 방지하기 위해 만료되어야 합니다.</p></td>
  </tr>
  <tr>
   <td>refresh_token </td>
   <td>문자열</td>
   <td><p>이 API 메서드를 호출하여 새 access_token을 검색하는 데 사용되는 장기 토큰입니다.</p></td>
  </tr>
  <tr>
   <td>expires_in </td>
   <td>길게</td>
   <td><p>(선택 사항) access_token이 만료되기 전 시간(초)으로, 일반적으로 3,600입니다.</p></td>
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

## 응답

```
{
access_token:"ad8af5ad5ads759",
refresh_token:"9a0h5d87d808ads",
expires_id:3600
}
```
