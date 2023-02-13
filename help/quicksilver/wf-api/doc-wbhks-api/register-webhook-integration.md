---
content-type: api
product-area: documents
navigation-topic: documents-webhooks-api
title: Webhook 통합 등록
description: Webhook 통합 등록
author: John
feature: Workfront API
exl-id: 9a4f8dbe-967f-4a41-a42c-8e3acb604972
source-git-commit: 5cb65c3a0c3ffd374c4002867c9c48985378e03c
workflow-type: tm+mt
source-wordcount: '346'
ht-degree: 11%

---


# Webhook 통합 등록

Adobe Workfront 관리자는 Workfront 내의 설정 > 문서 > 사용자 지정 통합으로 이동하여 회사를 위한 사용자 지정 웹 후크 통합을 추가할 수 있습니다. 관리자는 설정 내의 사용자 지정 통합 페이지에서 기존 문서 Webhook 통합 목록을 볼 수 있습니다. 이 페이지에서 통합을 추가, 편집, 활성화 및 비활성화할 수 있습니다.

통합을 추가하려면 를 클릭합니다 **사용자 지정 통합 추가**.

![](assets/webhooks-integration-350x230.png)

![](assets/webhooks-integration-2-350x220.png)

## 사용 가능한 필드

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
   <td>이 통합의 이름.</td> 
  </tr> 
  <tr> 
   <td>기본 API URL</td> 
   <td> <p>콜백 API의 위치입니다. 외부 시스템을 호출할 때 Workfront은 단순히 끝점 이름을 이 주소에 추가합니다. 예를 들어, 관리자가 기본 API URL인 "https://www.mycompany.com/api/v1"을 입력하면 Workfront은 다음 URL을 사용하여 문서의 메타데이터를 가져옵니다. https://www.mycompany.com/api/v1/metadata?id=1234</p> </td> 
  </tr> 
  <tr> 
   <td>요청 매개 변수</td> 
   <td> <p>모든 API 호출의 querystring에 추가할 선택 값. 예, access_type=offline. </p> </td> 
  </tr> 
  <tr> 
   <td>인증 유형</td> 
   <td>OAuth2 또는 ApiKey</td> 
  </tr> 
  <tr> 
   <td>인증 URL</td> 
   <td> <p>(OAuth2만 해당) 사용자 인증에 사용되는 전체 URL입니다. Workfront은 OAuth 프로비저닝 프로세스의 일부로 이 주소로 사용자를 이동합니다. 참고: Workfront이 쿼리 문자열에 "상태" 매개 변수를 추가합니다. 공급자가 Workfront 리디렉션 URI에 추가하여 이 정보를 Workfront에 다시 전달해야 합니다.</p> </td> 
  </tr> 
  <tr> 
   <td>토큰 엔드포인트 URL</td> 
   <td> <p>(OAuth2만 해당) OAuth2 토큰을 검색하는 데 사용되는 전체 API URL입니다. 웹 후크 공급자 또는 외부 문서 공급자가 호스팅합니다</p> </td> 
  </tr> 
  <tr> 
   <td>클라이언트 ID</td> 
   <td>(OAuth2만 해당) 이 통합을 위한 OAuth2 클라이언트 ID입니다</td> 
  </tr> 
  <tr> 
   <td>클라이언트 암호</td> 
   <td> <p>(OAuth2만 해당) 이 통합을 위한 OAuth2 클라이언트 암호</p> </td> 
  </tr> 
  <tr> 
   <td>Workfront 리디렉션 URI</td> 
   <td>(OAuth2만 해당) 읽기 전용 필드이며, Workfront에 의해 생성됩니다. 이 값은 외부 문서 공급자에 이 통합을 등록하는 데 사용됩니다. 참고: 인증 URL에 대해 위에 설명된 대로, 공급자는 리디렉션을 수행할 때 "state" 매개 변수와 그 값을 querystring에 추가해야 합니다.</td> 
  </tr> 
  <tr> 
   <td>API 키</td> 
   <td> <p>(ApiKey만 해당) 웹 후크 공급자에 인증된 API 호출을 수행하는 데 사용됩니다. 웹 후크 공급자가 발급한 API 키입니다.</p> </td> 
  </tr> 
 </tbody> 
</table>
