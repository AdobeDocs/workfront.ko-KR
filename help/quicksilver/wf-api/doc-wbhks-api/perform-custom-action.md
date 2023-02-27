---
content-type: api
product-area: documents
navigation-topic: documents-webhooks-api
title: 사용자 지정 작업 수행
description: 사용자 지정 작업 수행
author: Becky
feature: Workfront API
exl-id: a18b6b97-ee1e-4ad2-a4e1-00a644a0f4f2
source-git-commit: f050c8b95145552c9ed67b549608c16115000606
workflow-type: tm+mt
source-wordcount: '191'
ht-degree: 3%

---


# 사용자 지정 작업 수행(아직 구현되지 않음)

이 종단점을 사용하면 Adobe Workfront 사용자(또는 자동화된 워크플로우 이벤트)가 외부 시스템에서 작업을 수행할 수 있습니다. /customAction 종단점은 &quot;name&quot; 매개 변수를 허용하므로 웹 후크 공급자가 여러 사용자 지정 작업을 구현할 수 있습니다.

웹 후크 공급자는 customActions 아래에 있는 /serviceInfo 응답에 있는 작업을 포함하여 사용자 지정 작업을 Workfront에 등록합니다. Workfront은 설정 > 문서 > 사용자 지정 통합에서 웹 후크 공급자를 설정하거나 새로 고칠 때 이 목록을 로드합니다.

사용자는 &quot;문서 작업&quot; 아래에서 섹션을 선택하여 사용자 지정 작업을 트리거할 수 있습니다

**URL**

GET /customAction

## 쿼리 매개 변수

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
   <td> <p>이름</p> </td> 
   <td> <p>수행할 작업 유형을 지정하는 식별자입니다. 이 값은 /serviceInfo 종단점에 의해 반환되는 customAction 값 중 하나에 해당합니다.</p> </td> 
  </tr> 
  <tr> 
   <td>documentId </td> 
   <td>작업이 수행되는 작업 영역 문서 ID입니다.</td> 
  </tr> 
  <tr> 
   <td>documentVersionId </td> 
   <td> 작업이 수행되는 workfront 문서 버전 ID입니다.</td> 
  </tr> 
 </tbody> 
</table>

 

## 응답

아래 오류 처리 섹션에 지정된 대로 성공 또는 실패를 나타내는 JSON 문자열입니다. 실패 시(즉, 상태 = &quot;실패&quot;) Workfront에 제공된 오류 메시지가 사용자에게 표시됩니다.

**예:**

```
https://sample.com/webhooks/customName?name=archive&documentId=5502082c003a4f30 ddec2fb2b739cb7c&documentVersionId=54b598a700e2342d6971597a5df1a8d3
```

응답

```
{
status: “success”
}
```
