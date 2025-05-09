---
content-type: api
product-area: documents
navigation-topic: documents-webhooks-api
title: 서비스에 대한 정보 가져오기
description: 서비스에 대한 정보 가져오기
author: Becky
feature: Workfront API
role: Developer
exl-id: a3a423ff-29a6-466e-a568-f64e02dcb484
source-git-commit: b18a7835c6de131c125b77c6688057638c62fa4a
workflow-type: tm+mt
source-wordcount: '266'
ht-degree: 2%

---


# 서비스에 대한 정보 가져오기(아직 구현되지 않음)

>[!NOTE]
>
>이 기능의 릴리스 날짜는 아직 결정되지 않았습니다.

기능 등 서비스에 대한 정보를 반환합니다. Adobe Workfront은 이 정보를 사용하여 Workfront의 사용자 인터페이스를 사용자 정의합니다. 예를 들어 Webhook 구현에 일부 사용자 지정 작업이 포함된 경우 JSON은 해당 작업을 JSON에 나열해야 합니다. 그러면 사용자는 Workfront에서 이러한 작업을 호출할 수 있습니다.

**URL**

GET /serviceInfo

## 쿼리 매개변수

없음. 또한 이 끝점에 대한 호출에는 인증이 필요하지 않습니다.

## 응답

이 서비스에 대한 정보가 포함된 JSON

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
   <td>  <p>이 웹후크에서 구현한 사용자 지정 작업이 포함된 목록입니다. 각 목록 항목에는 이름과 표시 이름이 포함됩니다. Workfront의 "문서 작업" 드롭다운에 표시 이름이 표시됩니다. 드롭다운에서 항목을 클릭하면 /customAction 끝점을 호출하여 웹 후크에서 작업을 호출합니다.</p></td> 
  </tr> 
 </tbody> 
</table>

**예:** `https://www.acme.com/api/serviceInfo`

반환

```
{
webhook version: "1.2", version: "1.0", publisher: "Acme, LLC", availableEndpoints: ["files", "metadata", "search", "download"
"thumbnail", "uploadInit", "upload" ], customActions [
{
name: "archive", displayName: "Archive" 
}, 
{name: "doSomethingElse", displayName: "Do Something" }, 
] 
}
```
