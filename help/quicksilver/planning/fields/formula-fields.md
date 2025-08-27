---
title: 공식 필드 개요
description: Adobe Workfront Planning에서 함수 및 기존 필드를 사용하여 새 사용자 정의 값을 계산하는 공식 필드를 생성할 수 있습니다.
feature: Workfront Planning
role: User, Admin
author: Alina
recommendations: noDisplay, noCatalog
exl-id: 5027d611-916e-492d-9a44-841bdde11c94
source-git-commit: 7288c6fb0f5d45758e0a82b8d1283e1f43ae94e6
workflow-type: tm+mt
source-wordcount: '684'
ht-degree: 7%

---

# 공식 필드 개요

<!--<span class="preview">The highlighted information on this page refers to functionality not yet generally available. It is available only in the Preview environment for all customers. After the monthly releases to Production, the same features are also available in the Production environment for customers who enabled fast releases. </span>   

<span class="preview">For information about fast releases, see [Enable or disable fast releases for your organization](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/enable-fast-release-process.md). </span>-->

{{planning-important-intro}}

기존 필드를 참조하고 수식 유형 필드에서 연결하여 Adobe Workfront Planning에서 사용자 정의 필드를 만들 수 있습니다.

공식 필드는 레코드 유형의 다른 필드에 있는 기존 값과 기존 값을 계산하는 방법을 나타내는 함수를 사용하여 새 값을 생성합니다.

자세한 내용은 문서 [필드 만들기](/help/quicksilver/planning/fields/create-fields.md)의 &quot;수식&quot; 섹션을 참조하십시오.

## 액세스 요구 사항

+++ 를 확장하여 액세스 요구 사항을 확인합니다. 

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
   <ul><li><p> Adobe Workfront</p></li> 
   <li><p> Adobe Workfront 계획<p></li></ul></td> 
  </tr>   
<tr> 
   <td role="rowheader"><p>Adobe Workfront 플랜*</p></td> 
   <td> 
<p>다음 Workfront 플랜 중 하나:</p> 
<ul><li>선택</li> 
<li>Prime</li> 
<li>Ultimate</li></ul> 
<p>Workfront Planning은 기존 Workfront 플랜에 사용할 수 없습니다.</p> 
   </td> 
<tr> 
   <td role="rowheader"><p>Adobe Workfront 계획 패키지*</p></td> 
   <td> 
<p>임의 </p> 
<p>각 Workfront Planning 계획에 포함된 사항에 대한 자세한 내용은 Workfront 계정 관리자에게 문의하십시오. </p> 
   </td> 
 <tr> 
   <td role="rowheader"><p>Adobe Workfront 플랫폼</p></td> 
   <td> 
<p>Workfront Planning에 액세스하려면 조직의 Workfront 인스턴스가 Adobe 통합 경험에 온보딩되어야 합니다.</p> 
<p>자세한 내용은 <a href="/help/quicksilver/workfront-basics/navigate-workfront/workfront-navigation/adobe-unified-experience.md">Workfront용 Adobe 통합 환경</a>을 참조하십시오. </p> 
   </td> 
   </tr> 
  </tr> 
  <tr> 
   <td role="rowheader"><p>Adobe Workfront 라이센스*</p></td> 
   <td><p> 표준</p>
   <p>기존 Workfront 라이선스에는 Workfront Planning을 사용할 수 없습니다.</p> 
  </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><p>액세스 수준 구성</p></td> 
   <td> <p>Adobe Workfront Planning에 대한 액세스 수준 제어가 없습니다.</p>   
</td> 
  </tr> 
<tr> 
   <td role="rowheader"><p>개체 권한</p></td> 
   <td>   <p>작업 영역 및 레코드 종류 </a>에 대한 권한을 관리합니다. </p>  
   <p>시스템 관리자는 만들지 않은 작업 영역을 포함하여 모든 작업 영역에 대한 권한을 가집니다</p> </td> 
  </tr>

</tbody> 
</table>

*Workfront 액세스 요구 사항에 대한 자세한 내용은 Workfront 설명서의 [액세스 요구 사항](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)을 참조하십시오.

+++   

## 공식 필드에 대한 고려 사항

* 공식 필드는 동일한 레코드 유형에 속하는 필드를 참조합니다.
* 다른 레코드 종류를 수식 필드를 만드는 레코드 종류에 연결하는 경우에만 다른 레코드 종류의 필드를 참조할 수 있습니다.
* 수식에서 연결된 레코드 종류 또는 조회 필드를 참조하는 것은 연결된 레코드 종류에 대한 사용 권한에 따라 다릅니다. 레코드 종류를 볼 수 있는 권한이 없으면 수식에서 해당 필드를 참조할 수 없습니다.
* 수식 필드를 저장한 후에는 수식 필드의 필드 유형을 변경할 수 없습니다.
* 배합표 필드를 저장한 후 배합표 필드의 계산을 갱신할 수 있으며, 계산 결과는 동일한 유형의 모든 레코드에 대해 자동으로 갱신됩니다.
* 수식에서 참조하는 필드가 Workfront Planning 인터페이스에 표시되는 대로 추가해야 합니다.
* 레코드 유형의 표 보기 또는 레코드 세부 정보 페이지에 표시되는 필드만 참조할 수 있습니다.
* 다음 형식 옵션 중에서 선택하여 공식 계산 값에 대한 형식을 정의할 수 있습니다.

   * 텍스트
   * 숫자
   * 비율
   * 통화
   * 태그
   * Date

  자세한 내용은 문서 [필드 만들기](/help/quicksilver/planning/fields/create-fields.md)의 &quot;수식&quot; 섹션을 참조하십시오.
* 새 수식에서 수식 필드를 참조할 수 있습니다. 공식 필드에서 참조되는 필드에서 값이 업데이트되면 해당 필드를 참조하는 모든 후속 필드 또는 해당 필드가 포함된 공식 필드가 자동으로 업데이트됩니다.


<!--

<div class="preview">

## Limitations of formula fields

* You can add a maximum of 20 formula fields for one record type. 

   Formula lookup fields added from connected record types do not count against this limit. 

* The formula expression cannot exceed 50,000 characters. 

* Formula fields might display as `#ERROR!` in the following cases:
   * When a field used in a formula is deleted.
   * When a field used in an aggregated lookup field displays as `#ERROR!`. 
   
      For example, if you display a lookup field that contains aggregated lookup formula fields and one of the referenced formula fields  displays as `#ERROR!`. 
   *  When a formula value cannot be displayed in the selected format. 
   
      For example, if I select Number for the Format of a formula field, and the fields used in the formula are text fields that display only non-numeric text values, the formula result will display as `#ERROR!`, because it cannot parse the text into a number.
 
 </div>
 
 -->

## 지원되는 공식

Adobe Workfront Planning 공식 필드는 Workfront 계산된 필드의 대부분의 표현식을 지원합니다.

>[!NOTE]
>
>다음 Workfront 표현식은 Workfront Planning 공식 필드에서 지원되지 않습니다.
>
><!--* SORTASCARRAY-->
><!--* SORTDESCARRAY-->
>* ADDHOUR
>* 전환
>* 형식

<!--remove the ones commented out when we go live to Preview and Prod, if they truly are added to Planning-->

Workfront 식의 전체 목록을 보려면 [계산된 데이터 식의 개요](/help/quicksilver/reports-and-dashboards/reports/calc-cstm-data-reports/calculated-data-expressions.md)를 참조하십시오.

또한 Workfront Planning 공식 필드에 대해 다음 표현식을 지원합니다. 다음 표현식은 Workfront 표현식에 지원되지 않습니다.

<!--take these three out when they also come to WF and Lisa has added them to the WF expression article linked above-->

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
   <td><strong>JSONELEMENT</strong> </td> 
   <td> <p>제공된 JSONPath로 JSON의 데이터를 반환합니다. JSONPath가 JSON에 존재하지 않으면 빈 결과가 반환됩니다. </p> <p>표현식의 형식은 다음과 같습니다.
      <code>JSONELEMENT(JSONString, JSONPathString) </code>
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
