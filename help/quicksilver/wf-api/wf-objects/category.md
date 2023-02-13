---
content-type: api
navigation-topic: workfront-objects
title: APIModel INTERNAL이 필드 자동화(OpTask)Category를 지원하지 않는 경우
description: APIModel INTERNAL이 필드 자동화를 지원하지 않는 경우(OpTask)
author: John
feature: Workfront API
exl-id: 24c900ee-a8f1-458e-a18b-c098c6314e0c
source-git-commit: a939e14cbd6936bdd0c46c1ed641acdda497b8fc
workflow-type: tm+mt
source-wordcount: '376'
ht-degree: 22%

---


# 범주

Fieldsclass: &quot;java.lang.IllegalArgumentException&quot;,\
메시지: &quot;APIModel INTERNAL이 필드 자동화를 지원하지 않습니다(OpTask).&quot;

<table style="table-layout:auto"> 
 <col width="100"> 
 <col width="100"> 
 <col width="100"> 
 <col width="240"> 
 <col width="200"> 
 <col width="100"> 
 <thead> 
  <tr> 
   <th>이름</th> 
   <th>레이블</th> 
   <th>유형</th> 
   <th>설명</th> 
   <th>가능한 값</th> 
   <th>플래그</th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td data-sheets-value="{&quot;1&quot;:2,&quot;2&quot;:&quot;ID&quot;}"><strong>ID</strong> </td> 
   <td data-sheets-value="{&quot;1&quot;:2,&quot;2&quot;:&quot;ID&quot;}">ID</td> 
   <td data-sheets-value="{&quot;1&quot;:2,&quot;2&quot;:&quot;String&quot;}">문자열</td> 
   <td data-sheets-value="{&quot;1&quot;:2,&quot;2&quot;:&quot;Identifying GUID&quot;}">GUID 식별</td> 
   <td> </td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td data-sheets-value="{&quot;1&quot;:2,&quot;2&quot;:&quot;accessorIDs&quot;}"><strong>accessorIDs</strong> </td> 
   <td data-sheets-value="{&quot;1&quot;:2,&quot;2&quot;:&quot;acessorIDs&quot;}">acessorIDs</td> 
   <td data-sheets-value="{&quot;1&quot;:2,&quot;2&quot;:&quot;String Array&quot;}">문자열 배열</td> 
   <td data-sheets-value="{&quot;1&quot;:2,&quot;2&quot;:&quot;List of People/Team IDs that can access this object&quot;}">이 개체에 액세스할 수 있는 사람/팀 ID 목록</td> 
   <td> </td> 
   <td> <p><span class="dtRead">읽기 전용</span> </p> <p><span class="dtLazy">게으른 읽기</span> </p> <p><span class="dtDyn">동적</span> </p> <p><span class="dtGrp">그룹화할 수 없음</span> </p> </td> 
  </tr> 
  <tr> 
   <td data-sheets-value="{&quot;1&quot;:2,&quot;2&quot;:&quot;catObjCode&quot;}"><strong>catObjCode</strong> </td> 
   <td data-sheets-value="{&quot;1&quot;:2,&quot;2&quot;:&quot;Type&quot;}">유형</td> 
   <td data-sheets-value="{&quot;1&quot;:2,&quot;2&quot;:&quot;String&quot;}">문자열</td> 
   <td data-sheets-value="{&quot;1&quot;:2,&quot;2&quot;:&quot;Type of Object the Custom form is related to&quot;}">사용자 지정 양식이 관련된 개체의 유형입니다</td> 
   <td data-sheets-value="{&quot;1&quot;:2,&quot;2&quot;:&quot;[{\&quot;label\&quot;:\&quot;Company\&quot;,\&quot;value\&quot;:\&quot;CMPY\&quot;},{\&quot;label\&quot;:\&quot;Task\&quot;,\&quot;value\&quot;:\&quot;TASK\&quot;},{\&quot;label\&quot;:\&quot;Project\&quot;,\&quot;value\&quot;:\&quot;PROJ\&quot;},{\&quot;label\&quot;:\&quot;Portfolio\&quot;,\&quot;value\&quot;:\&quot;PORT\&quot;},{\&quot;label\&quot;:\&quot;Program\&quot;,\&quot;value\&quot;:\&quot;PRGM\&quot;},{\&quot;label\&quot;:\&quot;User\&quot;,\&quot;value\&quot;:\&quot;USER\&quot;},{\&quot;label\&quot;:\&quot;Document\&quot;,\&quot;value\&quot;:\&quot;DOCU\&quot;},{\&quot;label\&quot;:\&quot;Issue\&quot;,\&quot;value\&quot;:\&quot;OPTASK\&quot;},{\&quot;label\&quot;:\&quot;Expense\&quot;,\&quot;value\&quot;:\&quot;EXPNS\&quot;},{\&quot;label\&quot;:\&quot;Iteration\&quot;,\&quot;value\&quot;:\&quot;ITRN\&quot;}]&quot;}"><code>[{"label":"Company","value":"CMPY"},{"label":"Task","value":"TASK"},{"label":"Project","value":"PROJ"},{"label":"Portfolio","value":"PORT"},{"label":"Program","value":"PRGM"},{"label":"User","value":"USER"},{"label":"Document","value":"DOCU"},{"label":"Issue","value":"OPTASK"},{"label":"Expense","value":"EXPNS"},{"label":"Iteration","value":"ITRN"}]</code> </td> 
   <td> <p><span class="dtEdit">편집 가능</span> </p> <p><span class="dtReq">필수</span> </p> </td> 
  </tr> 
  <tr> 
   <td data-sheets-value="{&quot;1&quot;:2,&quot;2&quot;:&quot;customerID&quot;}"><strong>customerID</strong> </td> 
   <td data-sheets-value="{&quot;1&quot;:2,&quot;2&quot;:&quot;Customer ID&quot;}">고객 ID</td> 
   <td data-sheets-value="{&quot;1&quot;:2,&quot;2&quot;:&quot;String&quot;}">문자열</td> 
   <td data-sheets-value="{&quot;1&quot;:2,&quot;2&quot;:&quot;ID of the Customer&quot;}">고객의 ID</td> 
   <td> </td> 
   <td> <p><span class="dtGrp">그룹화할 수 없음</span> </p> </td> 
  </tr> 
  <tr> 
   <td data-sheets-value="{&quot;1&quot;:2,&quot;2&quot;:&quot;description&quot;}"><strong>설명</strong> </td> 
   <td data-sheets-value="{&quot;1&quot;:2,&quot;2&quot;:&quot;Description&quot;}">설명</td> 
   <td data-sheets-value="{&quot;1&quot;:2,&quot;2&quot;:&quot;String&quot;}">문자열</td> 
   <td data-sheets-value="{&quot;1&quot;:2,&quot;2&quot;:&quot;Description&quot;}">설명</td> 
   <td> </td> 
   <td> <p><span class="dtEdit">편집 가능</span> </p> </td> 
  </tr> 
  <tr> 
   <td data-sheets-value="{&quot;1&quot;:2,&quot;2&quot;:&quot;enteredByID&quot;}"><strong>enteredByID</strong> </td> 
   <td data-sheets-value="{&quot;1&quot;:2,&quot;2&quot;:&quot;Entered By ID&quot;}">작성자 ID</td> 
   <td data-sheets-value="{&quot;1&quot;:2,&quot;2&quot;:&quot;String&quot;}">문자열</td> 
   <td data-sheets-value="{&quot;1&quot;:2,&quot;2&quot;:&quot;ID of the User that added the Custom Form&quot;}">사용자 지정 양식을 추가한 사용자의 ID</td> 
   <td> </td> 
   <td> <p><span class="dtGrp">그룹화할 수 없음</span> </p> </td> 
  </tr> 
  <tr> 
   <td data-sheets-value="{&quot;1&quot;:2,&quot;2&quot;:&quot;extRefID&quot;}"><strong>extRefID</strong> </td> 
   <td data-sheets-value="{&quot;1&quot;:2,&quot;2&quot;:&quot;External Reference ID&quot;}">외부 참조 ID</td> 
   <td data-sheets-value="{&quot;1&quot;:2,&quot;2&quot;:&quot;String&quot;}">문자열</td> 
   <td data-sheets-value="{&quot;1&quot;:2,&quot;2&quot;:&quot;User Editable Field inteded to be used a link to an external object&quot;}">외부 객체에 대한 링크를 사용할 사용자 편집 가능 필드</td> 
   <td> </td> 
   <td> <p><span class="dtEdit">편집 가능</span> </p> </td> 
  </tr> 
  <tr> 
   <td data-sheets-value="{&quot;1&quot;:2,&quot;2&quot;:&quot;groupID&quot;}"><strong>groupID</strong> </td> 
   <td data-sheets-value="{&quot;1&quot;:2,&quot;2&quot;:&quot;Group ID&quot;}">그룹 ID</td> 
   <td data-sheets-value="{&quot;1&quot;:2,&quot;2&quot;:&quot;String&quot;}">문자열</td> 
   <td data-sheets-value="{&quot;1&quot;:2,&quot;2&quot;:&quot;ID of the first group with access to the custom form&quot;}">사용자 지정 양식에 액세스할 수 있는 첫 번째 그룹의 ID</td> 
   <td> </td> 
   <td> <p><span class="dtEdit">편집 가능</span> </p> <p><span class="dtGrp">그룹화할 수 없음</span> </p> </td> 
  </tr> 
  <tr> 
   <td data-sheets-value="{&quot;1&quot;:2,&quot;2&quot;:&quot;hasCalculatedFields&quot;}"><strong>hasCalculatedFields</strong> </td> 
   <td data-sheets-value="{&quot;1&quot;:2,&quot;2&quot;:&quot;Has Calculated Fields&quot;}">계산 필드 있음</td> 
   <td data-sheets-value="{&quot;1&quot;:2,&quot;2&quot;:&quot;Boolean&quot;}">부울</td> 
   <td data-sheets-value="{&quot;1&quot;:2,&quot;2&quot;:&quot;Does the form have calculated fields associated with it?&quot;}">양식에 계산된 필드가 연결되어 있습니까?</td> 
   <td> </td> 
   <td> <p><span class="dtGrp">그룹화할 수 없음</span> </p> </td> 
  </tr> 
  <tr> 
   <td data-sheets-value="{&quot;1&quot;:2,&quot;2&quot;:&quot;lastUpdateDate&quot;}"><strong>lastUpdateDate</strong> </td> 
   <td data-sheets-value="{&quot;1&quot;:2,&quot;2&quot;:&quot;Last Update Date&quot;}">마지막 업데이트 날짜</td> 
   <td data-sheets-value="{&quot;1&quot;:2,&quot;2&quot;:&quot;Date/Time&quot;}">일자/시간</td> 
   <td data-sheets-value="{&quot;1&quot;:2,&quot;2&quot;:&quot;Date of when the object was last modified&quot;}">개체를 마지막으로 수정한 날짜</td> 
   <td> </td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td data-sheets-value="{&quot;1&quot;:2,&quot;2&quot;:&quot;lastUpdatedByID&quot;}"><strong>lastUpdatedByID</strong> </td> 
   <td data-sheets-value="{&quot;1&quot;:2,&quot;2&quot;:&quot;Last Updated By ID&quot;}">마지막으로 업데이트한 사람 ID</td> 
   <td data-sheets-value="{&quot;1&quot;:2,&quot;2&quot;:&quot;String&quot;}">문자열</td> 
   <td data-sheets-value="{&quot;1&quot;:2,&quot;2&quot;:&quot;ID of the last user to Update the object&quot;}">개체를 업데이트할 마지막 사용자의 ID</td> 
   <td> </td> 
   <td> <p><span class="dtGrp">그룹화할 수 없음</span> </p> </td> 
  </tr> 
  <tr> 
   <td data-sheets-value="{&quot;1&quot;:2,&quot;2&quot;:&quot;name&quot;}"><strong>이름</strong> </td> 
   <td data-sheets-value="{&quot;1&quot;:2,&quot;2&quot;:&quot;Name&quot;}">이름</td> 
   <td data-sheets-value="{&quot;1&quot;:2,&quot;2&quot;:&quot;String&quot;}">문자열</td> 
   <td data-sheets-value="{&quot;1&quot;:2,&quot;2&quot;:&quot;Name of the Object&quot;}">개체 이름</td> 
   <td> </td> 
   <td> <p><span class="dtEdit">편집 가능</span> </p> <p><span class="dtReq">필수</span> </p> </td> 
  </tr> 
 </tbody> 
</table>

## 참조

| 이름 | 레이블 | 유형 | 유형 개체 코드 | URL |
|---|---|---|---|---|
| 고객 | 고객 | 고객 | CUST | [https://support.workfront.com/hc/en-us/articles/226425467](https://support.workfront.com/hc/en-us/articles/226425467) |
| 입력한 사람 | enteredBy | 사용자 | 사용자 | [https://support.workfront.com/hc/en-us/articles/226425467](https://support.workfront.com/hc/en-us/articles/226425467) |
| 그룹 | 그룹 | 그룹 | 그룹 | [https://support.workfront.com/hc/en-us/articles/226425467](https://support.workfront.com/hc/en-us/articles/226425467) |
| 마지막으로 업데이트한 사람 | lastUpdatedBy | 사용자 | 사용자 | [https://support.workfront.com/hc/en-us/articles/226425467](https://support.workfront.com/hc/en-us/articles/226425467) |


## 컬렉션

| 이름 | 레이블 | 유형 | 유형 개체 코드 | URL |
|---|---|---|---|---|
| 액세스 규칙 | accessRules | 액세스 규칙 | ACSURL | [https://support.workfront.com/hc/en-us/articles/226425467](https://support.workfront.com/hc/en-us/articles/226425467) |
| 카테고리 액세스 규칙 | categoryAccessRules | 카테고리 액세스 규칙 | CATACR | [https://support.workfront.com/hc/en-us/articles/226425467](https://support.workfront.com/hc/en-us/articles/226425467) |
| 카테고리 캐스케이드 규칙 | categoryCascadeRules | 카테고리 캐스케이드 규칙 | CTCSRL | [https://support.workfront.com/hc/en-us/articles/226425467](https://support.workfront.com/hc/en-us/articles/226425467) |
| 범주 매개변수 | categoryParameters | 범주 매개변수 | CTGYPA | [https://support.workfront.com/hc/en-us/articles/226425467](https://support.workfront.com/hc/en-us/articles/226425467) |
| 기타 그룹 | otherGroups | 그룹 | 그룹 | [https://support.workfront.com/hc/en-us/articles/226425467](https://support.workfront.com/hc/en-us/articles/226425467) |


## 액션

| 레이블 | 이름 | 인수 |
|---|---|---|
| 카테고리 할당 | assignCategories | `[{name: "objID",type: "string"},{name: "objCode",type: "string"},{name: "categoryIDs",type: "string[]"}]` |
| 범주 지정 | assignCategory | `[{name: "objID",type: "string"},name: "objCode",type: "string"},{name: "categoryID",type: "string"}]` |
| 범주 할당 취소 | unassignCategories | `[{name: "objID",type: "string"},{name: "objCode",type: "string"},{name: "categoryIDs",type: "string[]"}]` |
| 범주 할당 취소 | unassignCategory | `[{name: "objID",type: "string"},name: "objCode",type: "string"},{name: "categoryID",type: "string"}]` |
