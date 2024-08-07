---
content-type: api
product-area: documents
navigation-topic: documents-webhooks-api
title: 파일 또는 폴더에 대한 메타데이터 가져오기
description: 파일 또는 폴더에 대한 메타데이터 가져오기
author: Becky
feature: Workfront API
role: Developer
exl-id: 7b594df5-c87f-45d4-b84a-cae17171e906
source-git-commit: 14ff8da8137493e805e683e5426ea933f56f8eb8
workflow-type: tm+mt
source-wordcount: '268'
ht-degree: 2%

---


# 파일 또는 폴더에 대한 메타데이터 가져오기

지정된 파일 또는 폴더에 대한 메타데이터를 반환합니다.

**URL**

GET /metadata?id=[문서 또는 폴더 ID]

## 쿼리 매개변수

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
   <td>웹후크 공급자가 참조하는 파일 또는 폴더의 ID입니다. Adobe Workfront의 문서 ID와 다릅니다. 루트 디렉토리의 메타데이터를 가져오려면 값 '/'를 사용합니다.
   <p>참고: ID의 최대 길이는 255자입니다.</p></td> 
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
   <th>이름 </th> 
   <th>유형 </th> 
   <th>설명</th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td>제목 </td> 
   <td>문자열 </td> 
   <td>문서 또는 폴더의 이름</td> 
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
   <td>파일의 MIME 유형입니다. (선택 사항)</td> 
  </tr> 
  <tr> 
   <td>날짜 수정</td> 
   <td>문자열 </td> 
   <td>이 파일이 마지막으로 수정된 시간(형식이 지정된 RFC 3339 타임스탬프)</td> 
  </tr> 
  <tr> 
   <td>크기</td> 
   <td>길이</td> 
   <td> 파일 크기(바이트)입니다. (선택 사항)</td> 
  </tr> 
  <tr> 
   <td>읽기 전용</td> 
   <td>부울</td> 
   <td> 이 파일 또는 폴더가 인증된 사용자에게 읽기 전용인지 여부를 나타냅니다.(선택 사항) </td> 
  </tr> 
 </tbody> 
</table>

**예:** https://www.acme.com/api/metadata?id=12345
<pre>{<br>title:"내 문서",<br>종류:"파일"<br>id":"12345",<br>viewLink:"https://www.acme.com/viewDocument?id=12345",<br>downloadLink:"https://www.acme.com/downloadDocument?id=12345",<br>mimeType:"image/png",<br>dateModified:"20140605T17:39:45.251Z",<br>크기: "32554694"<br>}</pre>

>[!NOTE]
>
>오류 처리는 모든 API 호출에서 일관되어야 합니다. 자세한 내용은 아래의 &quot;오류 처리&quot; 섹션을 참조하십시오.
