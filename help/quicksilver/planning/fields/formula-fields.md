---
title: 공식 필드 개요
description: Adobe Workfront Planning에서 함수 및 기존 필드를 사용하여 새 사용자 정의 값을 계산하는 공식 필드를 생성할 수 있습니다.
hidefromtoc: true
hide: true
recommendations: noDisplay, noCatalog
exl-id: 5027d611-916e-492d-9a44-841bdde11c94
source-git-commit: 7580c7638c9e4d0f9aa53d208d9773fa1524ab54
workflow-type: tm+mt
source-wordcount: '424'
ht-degree: 8%

---

# 공식 필드 개요

<!--update the metadata with real information when making this available in TOC and in the left nav - below-->

<!--this article is linked to the UI in the formula box, "Learn more..."-->

<!---
title: Formula fields overview
description: In Adobe Workfront Planning, you can create formula fields that use functions and existing  fields to calculate a new custom value. 
hidefromtoc: yes
hide: yes
author: Alina
feature: (*******************WE NEED A NEW ONE*******************)
role: User, Administrator (************is this right???************)
recommendations: noDisplay, noCatalog
--->

<!--when we release permissions to RECORDS and we release referring lookup fields in a formula field, update considerations to say that lookup fields from linked records depends on the permissions to the record; if they have no permissions to view a linked record, they won't be able to use that records's lookup fields in a formula-->

{{planning-important-intro}}

기존 필드를 참조하고 수식 유형 필드에서 연결하여 Adobe Workfront Planning에서 사용자 정의 필드를 만들 수 있습니다.

공식 필드는 레코드 유형의 다른 필드에 있는 기존 값과 기존 값을 계산하는 방법을 나타내는 함수를 사용하여 새 값을 생성합니다.

자세한 내용은 문서 [필드 만들기](/help/quicksilver/planning/fields/create-fields.md)의 &quot;수식&quot; 섹션을 참조하십시오.

## 액세스 요구 사항

이 문서의 단계를 수행하려면 다음 액세스 권한이 있어야 합니다.

<table style="table-layout:auto">
 <col>
 </col>
 <col>
 </col>
 <tbody>
    <tr>
<tr>
<td>
   <p> 제품</p> </td>
   <td>
   <p> Adobe Workfront</p> </td>
  </tr>  
 <td role="rowheader"><p>Adobe Workfront 계약</p></td>
   <td>
<p>Workfront Planning의 조기 액세스 단계에 조직을 등록해야 합니다. </p>
   </td>
  </tr>
  <tr>
   <td role="rowheader"><p>Adobe Workfront 플랜</p></td>
   <td>
<p>임의</p>
   </td>
  </tr>
  <tr>
   <td role="rowheader"><p>Adobe Workfront 라이선스</p></td>
   <td>
   <p>임의</p> 
  </td>
  </tr>

<tr>
   <td role="rowheader"><p>액세스 수준 구성</p></td>
   <td> <p>Workfront 계획에 대한 액세스 제어가 없습니다.</p>  
</td>
  </tr>
<tr>
   <td role="rowheader"><p>권한</p></td>
   <td> <p>작업 영역</a>에 대한 권한 관리 </p>  
   <p>시스템 관리자는 만들지 않은 작업 영역을 포함하여 모든 작업 영역에 대한 권한을 가집니다</p>
</td>
  </tr>
<tr>
   <td role="rowheader"><p>레이아웃 템플릿</p></td>
   <td> <p>Workfront 또는 그룹 관리자는 레이아웃 템플릿에 계획 영역을 추가해야 합니다. 자세한 내용은 <a href="/help/quicksilver/planning/access/access-overview.md">액세스 개요</a>를 참조하십시오. </p>  
</td>
  </tr>

</tbody>
</table>

<!-- Notes to add for the table: for the "Workfront plans" row: the above is only for closed beta; when going to GA - activate the following plans:    
<p>Current plan: Prime and Ultimate</p>
<p>Legacy plan: Enterprise</p>-->


## 공식 필드에 대한 고려 사항

* 공식 필드는 동일한 레코드 유형에 속하는 필드를 참조합니다. 공식 필드를 만들 때 다른 레코드 유형의 필드를 참조할 수 없습니다. <!--is this still accurate??-->
* 수식 필드를 저장한 후에는 수식 필드의 필드 유형을 변경할 수 없습니다.
* 배합표 필드를 저장한 후 배합표 필드의 계산을 갱신할 수 있으며, 계산 결과는 동일한 유형의 모든 레코드에 대해 자동으로 갱신됩니다.
* 수식에서 참조하는 필드가 Workfront Planning 인터페이스에 표시되는 대로 추가해야 합니다.

## 지원되는 공식

Adobe Workfront Planning 공식 필드는 Workfront 계산된 필드의 모든 표현식을 지원합니다. 자세한 내용은 [계산된 데이터 식의 개요](/help/quicksilver/reports-and-dashboards/reports/calc-cstm-data-reports/calculated-data-expressions.md)를 참조하십시오.

또한 Workfront Planning 공식 필드에 대해 다음 표현식을 지원합니다.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th>표현식</th> 
   <th>설명 및 예제</th> 
  </tr> 
 </thead> 
 <tbody>

<tr> 
   <td><strong>ARRAYJOIN</strong> </td> 
   <td> <p>구분 기호로 연결된 문자열을 반환합니다.</p> <p>표현식의 형식은 다음과 같습니다.

<code>ARRAYJOIN(구분 기호,배열)</code>
</p>
   </td></tr>

<tr> 
   <td><strong>ARRAYUNIQUE</strong> </td> 
   <td> <p>고유한 값이 있는 배열을 반환합니다.</p> <p>표현식의 형식은 다음과 같습니다.

<code>ARRAYUNIQUE(배열)</code>
</p>
   </td></tr>
     <tr> 
   <td><strong>ID</strong> </td> 
   <td> <p>레코드의 ID를 반환합니다. 각 레코드에는 고유한 ID가 있습니다.</p> <p>표현식의 형식은 다음과 같습니다.

<code>{ID}</code>
</p>
   </td></tr>

<tr> 
   <td><strong>SETTIMEZONE</strong> </td> 
   <td> <p>날짜 및 시간의 시간대를 특정 시간대로 설정합니다.</p> <p>표현식의 형식은 다음과 같습니다.

<code>SETTIMEZONE(date,&#39;America/Los_Angeles&#39;)</code>
</p>
   </td></tr>

<tr> 
   <td><strong>WEEKOFYEAR</strong> </td> 
   <td> <p>1년의 주 수를 반환합니다. 선택적으로 주가 시작되는 요일을 지정할 수 있습니다(일요일은 1, 월요일은 2 사용). 생략하면 기본적으로 주가 일요일에 시작됩니다.</p> <p>표현식의 형식은 다음과 같습니다.

<code>WEEKOFYEAR(date,2)</code>
또는
<code>WEEKOFYEAR(일자)</code>
</p>
   </td></tr>

</table>
