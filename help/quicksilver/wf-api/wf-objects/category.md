---
content-type: api
navigation-topic: workfront-objects
title: 카테고리
description: Category 객체에 사용 가능한 필드 테이블로서, 설명 및 값 유형이 포함되어 있습니다.
author: Becky
feature: Workfront API
role: Developer
exl-id: 24c900ee-a8f1-458e-a18b-c098c6314e0c
source-git-commit: 8c72a44c49d137c6c73f7c213cb411e45f5a6e24
workflow-type: tm+mt
source-wordcount: '270'
ht-degree: 28%

---


# 카테고리

<!-- Audited: 5/2025 -->

<!--Fieldsclass: "java.lang.IllegalArgumentException",  
message: "APIModel INTERNAL does not support field projectid (OpTask)"-->

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
   <td data-sheets-value="{&quot;1&quot;:2,&quot;2&quot;:&quot;Identifying GUID&quot;}">식별 GUID</td> 
   <td> </td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td data-sheets-value="{&quot;1&quot;:2,&quot;2&quot;:&quot;accessorIDs&quot;}"><strong>접근자 ID</strong> </td> 
   <td data-sheets-value="{&quot;1&quot;:2,&quot;2&quot;:&quot;acessorIDs&quot;}">accessorIDs</td> 
   <td data-sheets-value="{&quot;1&quot;:2,&quot;2&quot;:&quot;String Array&quot;}">문자열 배열</td> 
   <td data-sheets-value="{&quot;1&quot;:2,&quot;2&quot;:&quot;List of People/Team IDs that can access this object&quot;}">이 오브젝트에 액세스할 수 있는 사람/팀 ID 목록</td> 
   <td> </td> 
   <td> <p><span class="dtRead">읽기 전용</span> </p> <p><span class="dtLazy">지연 읽기</span> </p> <p><span class="dtDyn">동적</span> </p> <p><span class="dtGrp">그룹화할 수 없음</span> </p> </td> 
  </tr> 
  <tr> 
   <td data-sheets-value="{&quot;1&quot;:2,&quot;2&quot;:&quot;catObjCode&quot;}"><strong>catObjCode</strong> </td> 
   <td data-sheets-value="{&quot;1&quot;:2,&quot;2&quot;:&quot;Type&quot;}">유형</td> 
   <td data-sheets-value="{&quot;1&quot;:2,&quot;2&quot;:&quot;String&quot;}">문자열</td> 
   <td data-sheets-value="{&quot;1&quot;:2,&quot;2&quot;:&quot;Type of Object the Custom form is related to&quot;}">사용자 정의 양식과 관련된 오브젝트의 유형</td> 
   <td data-sheets-value="{&quot;1&quot;:2,&quot;2&quot;:&quot;[{\&quot;label\&quot;:\&quot;Company\&quot;,\&quot;value\&quot;:\&quot;CMPY\&quot;},{\&quot;label\&quot;:\&quot;Task\&quot;,\&quot;value\&quot;:\&quot;TASK\&quot;},{\&quot;label\&quot;:\&quot;Project\&quot;,\&quot;value\&quot;:\&quot;PROJ\&quot;},{\&quot;label\&quot;:\&quot;Portfolio\&quot;,\&quot;value\&quot;:\&quot;PORT\&quot;},{\&quot;label\&quot;:\&quot;Program\&quot;,\&quot;value\&quot;:\&quot;PRGM\&quot;},{\&quot;label\&quot;:\&quot;User\&quot;,\&quot;value\&quot;:\&quot;USER\&quot;},{\&quot;label\&quot;:\&quot;Document\&quot;,\&quot;value\&quot;:\&quot;DOCU\&quot;},{\&quot;label\&quot;:\&quot;Issue\&quot;,\&quot;value\&quot;:\&quot;OPTASK\&quot;},{\&quot;label\&quot;:\&quot;Expense\&quot;,\&quot;value\&quot;:\&quot;EXPNS\&quot;},{\&quot;label\&quot;:\&quot;Iteration\&quot;,\&quot;value\&quot;:\&quot;ITRN\&quot;}]&quot;}"><code>[{"label":"Company","value":"CMPY"},{"label":"Task","value":"TASK"},{"label":"Project","value":"PROJ"},{"label":"Portfolio","value":"PORT"},{"label":"Program","value":"PRGM"},{"label":"User","value":"USER"},{"label":"Document","value":"DOCU"},{"label":"Issue","value":"OPTASK"},{"label":"Expense","value":"EXPNS"},{"label":"Iteration","value":"ITRN"}]</code> </td> 
   <td> <p><span class="dtEdit">편집 가능</span> </p> <p><span class="dtReq">필수</span> </p> </td> 
  </tr> 
  <tr> 
   <td data-sheets-value="{&quot;1&quot;:2,&quot;2&quot;:&quot;customerID&quot;}"><strong>customerID</strong> </td> 
   <td data-sheets-value="{&quot;1&quot;:2,&quot;2&quot;:&quot;Customer ID&quot;}">고객 ID</td> 
   <td data-sheets-value="{&quot;1&quot;:2,&quot;2&quot;:&quot;String&quot;}">문자열</td> 
   <td data-sheets-value="{&quot;1&quot;:2,&quot;2&quot;:&quot;ID of the Customer&quot;}">고객 ID</td> 
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
   <td data-sheets-value="{&quot;1&quot;:2,&quot;2&quot;:&quot;ID of the User that added the Custom Form&quot;}">사용자 정의 양식을 추가한 사용자의 ID</td> 
   <td> </td> 
   <td> <p><span class="dtGrp">그룹화할 수 없음</span> </p> </td> 
  </tr> 
  <tr> 
   <td data-sheets-value="{&quot;1&quot;:2,&quot;2&quot;:&quot;extRefID&quot;}"><strong>extRefID</strong> </td> 
   <td data-sheets-value="{&quot;1&quot;:2,&quot;2&quot;:&quot;External Reference ID&quot;}">외부 참조 ID</td> 
   <td data-sheets-value="{&quot;1&quot;:2,&quot;2&quot;:&quot;String&quot;}">문자열</td> 
   <td data-sheets-value="{&quot;1&quot;:2,&quot;2&quot;:&quot;User Editable Field inteded to be used a link to an external object&quot;}">외부 오브젝트에 대한 링크를 사용하기 위한 사용자 편집 가능 필드</td> 
   <td> </td> 
   <td> <p><span class="dtEdit">편집 가능</span> </p> </td> 
  </tr> 
  <tr> 
   <td data-sheets-value="{&quot;1&quot;:2,&quot;2&quot;:&quot;groupID&quot;}"><strong>groupID</strong> </td> 
   <td data-sheets-value="{&quot;1&quot;:2,&quot;2&quot;:&quot;Group ID&quot;}">그룹 ID</td> 
   <td data-sheets-value="{&quot;1&quot;:2,&quot;2&quot;:&quot;String&quot;}">문자열</td> 
   <td data-sheets-value="{&quot;1&quot;:2,&quot;2&quot;:&quot;ID of the first group with access to the custom form&quot;}">사용자 정의 양식에 대한 액세스 권한이 있는 첫 번째 그룹의 ID</td> 
   <td> </td> 
   <td> <p><span class="dtEdit">편집 가능</span> </p> <p><span class="dtGrp">그룹화할 수 없음</span> </p> </td> 
  </tr> 
  <tr> 
   <td data-sheets-value="{&quot;1&quot;:2,&quot;2&quot;:&quot;hasCalculatedFields&quot;}"><strong>hasCalculatedFields</strong> </td> 
   <td data-sheets-value="{&quot;1&quot;:2,&quot;2&quot;:&quot;Has Calculated Fields&quot;}">계산 필드 있음</td> 
   <td data-sheets-value="{&quot;1&quot;:2,&quot;2&quot;:&quot;Boolean&quot;}">부울</td> 
   <td data-sheets-value="{&quot;1&quot;:2,&quot;2&quot;:&quot;Does the form have calculated fields associated with it?&quot;}">양식에 그것과 연결된 계산된 필드가 있습니까?</td> 
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

| 이름 | 레이블 | 유형 | 개체 코드 입력 |
|---|---|---|---|
| 고객 | 고객 | 고객 | CUST |
| 작성자 | 입력한 사람 | 사용자 | 사용자 |
| 그룹 | 그룹 | 그룹 | 그룹 |
| 마지막으로 업데이트한 사람 | lastUpdatedBy | 사용자 | 사용자 |


## 컬렉션

| 이름 | 레이블 | 유형 | 개체 코드 입력 |
|---|---|---|---|
| 액세스 규칙 | accessRules | 액세스 규칙 | ACSRUL |
| 범주 액세스 규칙 | 범주 액세스 규칙 | 범주 액세스 규칙 | 카타르 |
| 범주 캐스케이드 규칙 | categoryCascadeRules | 카탈로그 캐스케이드 규칙 | CTCSRL |
| 범주 매개변수 | 범주 매개변수 | 범주 매개변수 | CTGYA |
| 기타 그룹 | 기타 그룹 | 그룹 | 그룹 |


## 액션

| 레이블 | 이름 | 인수 |
|---|---|---|
| 범주 할당 | assignCategors | `[{name: "objID",type: "string"},{name: "objCode",type: "string"},{name: "categoryIDs",type: "string[]"}]` |
| 범주 할당 | 할당 범주 | `[{name: "objID",type: "string"},name: "objCode",type: "string"},{name: "categoryID",type: "string"}]` |
| 범주 할당 해제 | unassignCategories | `[{name: "objID",type: "string"},{name: "objCode",type: "string"},{name: "categoryIDs",type: "string[]"}]` |
| 범주 할당 해제 | unassign범주 | `[{name: "objID",type: "string"},name: "objCode",type: "string"},{name: "categoryID",type: "string"}]` |
