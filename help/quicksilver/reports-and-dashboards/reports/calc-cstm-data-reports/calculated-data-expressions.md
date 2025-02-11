---
content-type: reference
product-area: reporting
navigation-topic: calculate-custom-data-reports
title: 계산된 데이터 표현식 개요
description: 데이터 표현식을 사용하여 Adobe Workfront에서 계산된 사용자 정의 데이터 필드를 정의할 수 있습니다. 계산된 표현식은 새 필드를 생성하는 문에서 기존 Workfront 필드를 연결합니다.
author: Nolan
feature: Reports and Dashboards
exl-id: cfb3ace9-76c3-4006-878f-e2ad25ffa03b
source-git-commit: e66d4223b13bcd4813156f147769e7ee99c3f8ef
workflow-type: tm+mt
source-wordcount: '2425'
ht-degree: 2%

---

# 계산된 데이터 표현식 개요

<!--Audited: 12/2023-->

데이터 표현식을 사용하여 Adobe Workfront에서 계산된 사용자 정의 필드를 정의할 수 있습니다. 계산된 표현식은 새 필드를 생성하는 문에서 기존 Workfront 필드를 연결합니다.

다음에서 계산된 데이터 표현식을 사용할 수 있습니다.

* 사용자 정의 양식의 계산된 사용자 정의 필드

  Workfront의 사용자 정의 양식에서 계산된 사용자 정의 필드를 만드는 방법에 대한 자세한 내용은 [양식에 계산된 필드 추가](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/form-designer/design-a-form/add-a-calculated-field.md)를 참조하십시오.

* 텍스트 모드를 사용할 때 보고서 또는 목록의 계산된 사용자 지정 열

  보고서 및 보기에서 텍스트 모드를 사용하는 방법에 대한 자세한 내용은 [텍스트 모드 개요](../../../reports-and-dashboards/reports/text-mode/understand-text-mode.md)를 참조하십시오.

## 계산된 사용자 정의 필드와 계산된 사용자 정의 열의 구문

사용하는 함수는 동일하지만 계산된 사용자 정의 필드에 표현식을 작성하는 구문은 계산된 사용자 정의 열을 작성하는 구문과 다를 수 있습니다.

두 구문 간의 차이점은 다음과 같습니다.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td><strong>계산된 사용자 정의 필드</strong></td> 
   <td><strong>계산된 사용자 지정 보고 요소</strong></td> 
  </tr> 
   <td>필드 이름을 중괄호로 묶습니다.</td> 
   <td>에서 필드 이름을 사용할 때 대괄호나 괄호로 묶지 마십시오. <p><code>valuefield </code></p>줄. <p>필드 이름을 사용할 때 중괄호로 묶습니다. <p><code>valueexpression</code></p> 줄.</p> </td> 
  </tr> 
  <tr> 
   <td>필드를 마침표로 구분합니다.</td> 
   <td> <p>에서 필드를 사용할 때 콜론으로 구분합니다. <p><code>valuefield </code></p>line</p> <p>에서 사용할 때 필드를 마침표로 구분합니다. <p><code>valueexpression </code></p>줄. </p> </td> 
  </tr> 
 </tbody> 
</table>

For example:

* 사용자 정의 필드의 작업에 대한 사용자 정의 양식에서 다음을 사용하여 사용자 정의 양식이 첨부된 작업의 상위 프로젝트 이름을 생성합니다.


  ` {project}.{name}`


* 보고서의 사용자 정의 열에서 다음을 사용하여 작업 보고서에 프로젝트 이름 사용자 정의 열을 추가합니다.


  `valuefield=project:name`


  또는

  `valueexpression={project}.{name}`


  >[!TIP]
  >
  >계산된 표현식이 사용되는 모든 텍스트 모드 보고 요소(보기, 필터, 그룹화, 프롬프트)에도 동일한 구문이 적용됩니다.

계산된 사용자 지정 열에서 사용해야 하는 구문에 대한 자세한 내용은 [텍스트 모드 개요](../../../reports-and-dashboards/reports/text-mode/understand-text-mode.md)를 참조하십시오.

## 사용할 수 있는 데이터 표현식

아래 목록은 Workfront에서 세 가지 유형의 계산된 사용자 정의 필드 중 하나를 작성할 때 사용할 수 있는 표현식을 정의합니다.

* [계산된 사용자 정의 필드 날짜 및 시간](#date-time-calculated-custom-fields)
* [계산된 사용자 정의 필드](#mathematical-calculated-custom-fields)
* [계산된 사용자 정의 필드 텍스트](#text-calculated-custom-fields)

아래 나열된 표현식을 사용하여 계산된 사용자 정의 열을 작성할 수 있습니다. 그러나 이 문서의 [계산된 사용자 정의 필드와 계산된 사용자 정의 열의 구문](#syntax-of-calculated-custom-fields-vs-calculated-custom-columns) 섹션에 설명된 대로 계산된 사용자 정의 열에 올바른 구문을 사용해야 합니다.

### 계산된 날짜 및 시간 사용자 정의 필드 {#date-time-calculated-custom-fields}

>[!NOTE]
>
>시간 부분을 포함하지 않거나 날짜 와일드카드 $$TODAY 또는 $$NOW를 사용하는 날짜 및 시간 계산을 만드는 경우, 시스템은 현지 시간대가 아닌 UTC(협정 세계시) 시간대에 따라 날짜를 사용합니다. 이로 인해 예상치 못한 날짜 결과가 발생할 수 있습니다.

다음 표현식을 사용하여 날짜 또는 시간 계산된 사용자 정의 필드를 만들 수 있습니다.

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
   <td><strong>ADDDAYS</strong> </td> 
   <td> <p>날짜에 일수를 추가합니다. 숫자 값은 부분 일을 포함할 수 있습니다. 예를 들어 1.5는 날짜에 1일 반일을 추가합니다.</p> <p>표현식의 형식은 다음과 같습니다.</p>

<p><code>ADDDAYS(date, number)</code></p> </td> 
  </tr> 
  <tr> 
   <td><strong>ADDWEEKDAYS</strong> </td> 
   <td> <p>날짜에 평일 수를 추가합니다. 이 표현식은 날짜에 정수 값만 추가하여 내림합니다. </p> <p>표현식의 형식은 다음과 같습니다.</p>

<p><code>ADDWEEKDAYS(date, number)</code></p> </td> 
  </tr> 
  <tr> 
   <td><strong>ADDMONTHS</strong> </td> 
   <td> <p>날짜에 개월 수를 추가하고 형식은 다음과 같습니다.

</p><p><code>ADDMONTHS(date, number)</code></p> </td> 
  </tr> 
  <tr> 
   <td><strong>ADDYEARS</strong> </td> 
   <td> <p>날짜에 연도 수를 추가하고 형식은 다음과 같습니다.</p>

<p><code>ADDYEARS(date, number)</code></p> </td> 
  </tr> 
  <tr> 
   <td><strong>ADDHOURS</strong> </td> 
   <td> <p>날짜에 시간(시) 수를 추가하고 형식은 다음과 같습니다.</p>

<p><code>ADDHOUR(date, number)</code></p>
   <p>참고: 이 표현식은 Workfront Planning에서 지원되지 않습니다.</p></td> 
  </tr>
  <tr> 
   <td><strong>CLEARTIME</strong> </td> 
   <td> <p>날짜의 시간 부분을 지우고 형식을 다음과 같이 지정합니다. 이 예에서 날짜는 작업 객체의 입력 날짜입니다.</p>

<p><code>CLEARTIME({entryDate})</code></p> </td> 
  </tr> 
  <tr> 
   <td><strong>날짜</strong> </td> 
   <td> <p>문자열을 날짜로 전환하고 형식을 다음과 같이 지정합니다.</p>

<p><code>DATE(string)</code></p> </td> 
  </tr> 
  <tr> 
   <td><strong>DATEDIFF</strong> </td> 
   <td> <p>선택한 기간의 시작 및 종료 일수와 해당 날짜의 타임스탬프를 고려하여 두 날짜 사이의 일 수를 반환합니다. 예를 들어 시작 일자의 시작 시간이 오후 3시인 경우 시작 일은 전일로 계산되지 않습니다.</p> <p>표현식의 형식은 다음과 같습니다.</p>

<p><code>DATEDIFF(date1, date2)</code></p> </td> 
  </tr> 
  <tr> 
   <td><strong>DAYOFMONTH</strong> </td> 
   <td> <p>1과 31 사이의 날짜에 대한 월 중 일을 숫자로 반환합니다.</p> <p>표현식의 형식은 다음과 같습니다. 이 예에서 날짜는 작업 객체의 입력 날짜입니다.</p>

<p><code>DAYOFMONTH({entryDate})</code></p> </td> 
  </tr> 
  <tr> 
   <td><strong>DAYOFWEEK</strong> </td> 
   <td> <p>1(일요일)과 7(토요일) 사이의 날짜에 대한 요일을 숫자로 반환합니다.</p> <p>표현식의 형식은 다음과 같습니다. 이 예에서 날짜는 작업 객체의 입력 날짜입니다.</p>

<p><code>DAYOFWEEK({entryDate})</code></p> </td> 
  </tr> 
  <tr> 
   <td><strong>DAYSINMONTH</strong> </td> 
   <td> <p>날짜의 월간 총 일수를 숫자로 반환하며 형식은 다음과 같습니다. 이 예에서 날짜는 작업 객체의 입력 날짜입니다.</p>

<p><code>DAYSINMONTH({entryDate})</code></p> </td> 
  </tr> 
  <tr> 
   <td><strong>DAYSINSPLITWEEK</strong> </td> 
   <td> <p>일자와 주의 끝 또는 월의 끝 중 먼저 도래하는 일자 사이의 총 평일 반환 이 예에서 날짜는 작업 객체의 입력 날짜입니다.</p> <p>표현식의 형식은 다음과 같습니다.</p>

<p><code>DAYSINSPLITWEEK({entryDate})</code></p> </td> 
  </tr> 
  <tr> 
   <td><strong>DAYSINYEAR</strong> </td> 
   <td> <p>날짜의 연중 총 일수를 숫자로 반환하며 형식은 다음과 같습니다. 이 예에서 날짜는 작업 객체의 입력 날짜입니다.</p>

<p><code>DAYSINYEAR({entryDate})</code></p> </td> 
  </tr> 
  <tr> 
   <td><strong>DMAX</strong> </td> 
   <td> <p>목록에서 가장 늦은 날짜를 반환하며 형식은 다음과 같습니다.</p>

<p><code>DMAX(date1, date2, ...)</code></p> </td> 
  </tr> 
  <tr> 
   <td><strong>관리자</strong> </td> 
   <td> <p>목록에서 가장 빠른 날짜를 반환하며 형식은 다음과 같습니다.</p>

<p><code>DMIN(date1, date2, ...)</code></p> </td> 
  </tr> 
  <tr> 
   <td><strong>시간</strong> </td> 
   <td> <p>날짜의 시간을 0에서 23 사이의 숫자로 반환합니다.</p> <p>표현식의 형식은 다음과 같습니다. 이 예에서 날짜는 작업 객체의 입력 날짜입니다.</p>

<p><code>HOUR({entryDate})</code></p> </td> 
  </tr> 
  <tr> 
   <td><strong>분</strong> </td> 
   <td> <p>날짜의 분을 0에서 60 사이의 숫자로 반환합니다(다음 형식). 이 예에서 날짜는 작업 객체의 입력 날짜입니다.</p>

<p><code>MINUTE({entryDate})</code></p> </td> 
  </tr> 
  <tr> 
   <td><strong>개월</strong> </td> 
   <td> <p>날짜의 월을 1에서 12 사이의 숫자로 반환합니다(다음 형식). 이 예에서 날짜는 작업 객체의 입력 날짜입니다.</p>

<p><code>MONTH({entryDate})</code></p> </td> 
  </tr> 
  <tr> 
   <td><strong>초</strong> </td> 
   <td> <p>날짜의 초를 0에서 60 사이의 숫자로 반환합니다(형식은 다음과 같음). 이 예에서 날짜는 작업 객체의 입력 날짜입니다.</p>

<p><code>SECOND({entryDate})</code></p> </td> 
  </tr> 
  <tr> 
   <td><strong>WEEKDAYDIFF</strong> </td> 
   <td> <p>선택한 기간의 시작 날짜와 종료 날짜 및 해당 날짜의 타임스탬프를 고려하여 두 날짜 사이의 평일 수를 반환합니다. 예를 들어 시작 일자의 시작 시간이 오후 3시인 경우 시작 일은 전일로 계산되지 않습니다.</p> <p>표현식의 형식은 다음과 같습니다.</p>

<p><code>WEEKDAYDIFF(date2, date1)</code></p> </td> 
  </tr> 
  <tr> 
   <td><strong>WORKMINUTESDIFF</strong> </td> 
   <td> <p>기본 일정에 따라 날짜 사이의 예약된 시간(분)을 반환합니다.</p> <p>표현식의 형식은 다음과 같습니다.</p>

<p><code>WORKMINUTESDIFF(date1, date2)</code></p> </td> 
  </tr> 
  <tr> 
   <td><strong>년</strong> </td> 
   <td> <p>날짜의 연도를 다음과 같은 형식의 4자리 숫자로 반환합니다. 이 예에서 날짜는 작업 객체의 입력 날짜입니다.</p>

<p><code>YEAR({entryDate})</code></p> </td> 
  </tr> 
 </tbody> 
</table>

### 계산된 수학 사용자 정의 필드 {#mathematical-calculated-custom-fields}

다음 수학 표현식 중 일부를 사용하는 계산된 사용자 정의 필드를 생성할 수 있습니다.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th>표현식</th> 
   <th>설명</th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td><strong>절대</strong> </td> 
   <td>숫자의 절대값을 반환하며 형식은 다음과 같습니다. 이 예제에서는 사용자 정의 양식이 첨부된 오브젝트 아래에 있는 오브젝트의 수를 사용합니다.

<p><code>ABS({numberOfChildren})</code></p></td> 
  </tr> 
  <tr> 
   <td><strong>평균</strong> </td> 
   <td>숫자의 평균을 반환하며 형식은 다음과 같습니다.

<p><code>AVERAGE(number1, number2, ...)</code></p></td> 
  </tr> 
  <tr> 
   <td><strong>CEIL</strong> </td> 
   <td>숫자를 가장 가까운 정수로 반올림하고 형식을 다음과 같이 지정합니다. 이 예제에서는 사용자 정의 양식이 첨부된 오브젝트 아래에 있는 오브젝트의 수를 사용합니다.

<p><code>CEIL({numberOfChildren})</code></p></td> 
  </tr> 
  <tr> 
   <td><strong>DIV</strong> </td> 
   <td>제공된 순서대로 모든 숫자를 나눕니다. 형식은 다음과 같습니다.

<p><code>DIV(number1, number2, ...)</code></p></td> 
  </tr> 
  <tr> 
   <td><strong>층</strong> </td> 
   <td>숫자를 가장 가까운 정수로 내림하고 형식을 다음과 같이 지정합니다. 이 예제에서는 사용자 정의 양식이 첨부된 오브젝트 아래에 있는 오브젝트의 수를 사용합니다.

<p><code>FLOOR({numberOfChildren})</code></p></td> 
  </tr> 
  <tr> 
   <td><strong>LN</strong> </td> 
   <td>숫자의 자연 로그 값을 반환하며 형식은 다음과 같습니다.

<p><code>LN({numberOfChildren})</code></p></td> 
  </tr> 
  <tr> 
   <td><strong>로그</strong> </td> 
   <td>기본 number1에 대한 number2의 로그 값을 반환하며 형식은 다음과 같습니다.

<p><code>LOG(number1, number2)</code></p></td> 
  </tr> 
  <tr> 
   <td><strong>MAX</strong> </td> 
   <td>목록에서 가장 큰 항목을 반환하고 형식을 다음과 같이 지정합니다.

<p><code>MAX(item1, item2, ...)</code></p></td> 
  </tr> 
  <tr> 
   <td><strong>분</strong> </td> 
   <td>목록에서 가장 작은 항목을 반환하고 형식을 다음과 같이 지정합니다.

<p><code>MIN(item1, item2, ...)</code></p></td> 
  </tr> 
  <tr> 
   <td><strong>숫자</strong> </td> 
   <td>문자열을 숫자로 전환하고 형식을 다음과 같이 지정합니다.<p><code>NUMBER(string)</code></p></td> 
  </tr> 
  <tr> 
   <td><strong>전원</strong> </td> 
   <td>제곱한 숫자를 반환하며 형식은 다음과 같습니다.

<p><code>POWER(number, power)</code></p></td> 
  </tr> 
  <tr> 
   <td><strong>PROD</strong> </td> 
   <td>모든 숫자를 곱하고 형식을 다음과 같이 지정합니다.

<p><code>PROD(number1, number2, ....)</code></p>
   <p><b>메모</b></p>

<p>시간이 포함된 필드에 곱할 때 데이터베이스가 시간을 선택한 필드에 분, 시간 또는 초 단위로 저장하는지 여부를 이해해야 합니다. 시간이 분 또는 초 단위로 저장되지만 Workfront 인터페이스에 시간 단위로 표시되는 경우 이 계산을 사용하여 표현식을 작성할 때 분 또는 초에서 시간으로 변환해야 할 수 있습니다. </p>
   </td> 
  </tr> 
  <tr> 
   <td><strong>라운드</strong> </td> 
   <td>지정한 정밀도 소수점으로 숫자를 반올림하고 형식을 다음과 같이 지정합니다.

<p><code>ROUND(number, precision)</code></p></td> 
  </tr> 
  <tr> 
   <td><strong>SORTASCNUM</strong> </td> 
   <td> <p> 숫자를 오름차순으로 정렬하고 형식은 다음과 같습니다.</p>

<p><code>SORTASCNUM(number1,number2, ...)</code></p> </td> 
  </tr> 
  <tr> 
   <td><strong>SORTDESCNUM</strong> </td> 
   <td>내림차순으로 숫자를 정렬하고 형식을 다음과 같이 지정합니다.

<p><code>SORTDESCNUM(number1, number2, ...)</code></p></td> 
  </tr> 
  <tr> 
   <td><strong>SQRT</strong> </td> 
   <td> <p>숫자의 제곱근을 반환하고 형식을 다음과 같이 지정합니다. 이 예제에서는 사용자 정의 양식이 첨부된 오브젝트 아래에 있는 오브젝트의 수를 사용합니다.</p>

<p><code>SQRT({numberOfChildren})</code></p> </td> 
  </tr> 
  <tr> 
   <td><strong>하위</strong> </td> 
   <td>제공된 순서대로 모든 숫자를 뺍니다. 형식은 다음과 같습니다.

<p><code>SUB(number1, number2, ...)</code></p></td> 
  </tr> 
  <tr> 
   <td><strong>합계</strong> </td> 
   <td>모든 숫자를 추가하고 형식은 다음과 같습니다.

<p><code>SUM(number1, number2, ...)</code></p></td> 
  </tr> 
 </tbody> 
</table>

### 계산된 사용자 정의 필드 텍스트 {#text-calculated-custom-fields}

다음 표현식을 사용하여 텍스트 형식의 값을 표시하는 계산된 사용자 지정 필드를 만들 수 있습니다.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th>표현식</th> 
   <th>설명</th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td><strong>배열</strong> </td> 
   <td> <p>문자열을 배열로 변환합니다. 구분 기호는 모든 문자열이 될 수 있습니다.</p> 
   <p>표현식의 형식은 다음과 같습니다.</p>
   <p><code>ARRAY(string1, "delimiter")</code></p> 
   </td> 
  </tr>
  <tr> 
   <td><strong>ARRAYLENGTH</strong> </td> 
   <td> <p>배열에 있는 요소의 수를 반환하며 형식은 다음과 같습니다.</p>
   <p><code>ARRAYLENGTH(array)</code></p> 
   </td> 
  </tr>
  <tr> 
   <td><strong>ARRAYELEMENT</strong> </td> 
   <td> <p>배열에서 지정된 번호에 있는 요소를 반환합니다. 색인이 범위를 벗어나면 비어 있는 값을 반환합니다.</p> 
   <p>표현식의 형식은 다음과 같습니다.</p>
   <p><code>ARRAYELEMENT(array, number)</code></p> 
   </td> 
  </tr>
  <tr> 
   <td><strong>SORTASCARRAY</strong> </td> 
   <td> <p>배열 요소의 순서를 오름차순으로 정렬하고 첫 번째 요소의 유형으로 변환합니다.</p>
   <p>표현식의 형식은 다음과 같습니다.</p>
   <p><code>SORTASCARRAY(array)</code></p>
   <p>예를 들어 ["-12.6", -13.0]은 ["-12.6", "-13"]이 됩니다.</p>
   <p>참고: 이 표현식은 Workfront Planning에서 지원되지 않습니다.</p></td> 
  </tr>
  <tr> 
   <td><strong>SORTDESCARRAY</strong> </td> 
   <td> <p>배열 요소의 순서를 내림차순으로 지정하고 첫 번째 요소의 유형으로 변환합니다.</p>
   <p>표현식의 형식은 다음과 같습니다.</p>
   <p><code>SORTDESCARRAY(array)</code></p>
   <p>예를 들어 ["-12.6", -13.0]은 ["-13", "-12.6"]이 됩니다.</p>
   <p>참고: 이 표현식은 Workfront Planning에서 지원되지 않습니다.</p></td> 
  </tr>
  <tr>   
   <td><strong>사례</strong> </td> 
   <td> <p>색인 번호를 기반으로 목록에서 값을 선택하는 데 다른 표현식과 함께 사용됩니다. </p>
   <p>색인 번호는 숫자 값(일반적으로 알려진 범위)을 반환하는 필드 또는 함수입니다.</p> 
   <p>표현식의 형식은 다음과 같습니다.</p>
   <p><code>CASE(indexNumber, value1, value2, ...)</code></p>

<p>예를 들어, 다음 표현식은 계산된 열에서 1=일요일, 2=월요일 등 요일의 이름을 반환합니다.</p>

<p><code>CASE(DAYOFWEEK({entryDate}),"Sunday","Monday","Tuesday","Wednesday","Thursday","Friday","Saturday")</code></p>

<p>DAYOFWEEK, DAYOFMONTH 및 MONTH와 같이 숫자를 반환하는 다른 표현식에 가장 적합합니다.</p> </td> 
  </tr> 
  <tr> 
   <td><strong>CONCAT</strong> </td> 
   <td> <p>문자열을 연결하고 형식을 다음과 같이 지정합니다.</p><p><code>CONCAT(string1,"separator", string2)</code></p> <p>다음은 포함할 수 있는 구분 기호의 예입니다.</p> 
    <ul> 
     <li>공백: " "</li> 
     <li>대시: "-"</li> 
     <li>슬래시: "/"</li> 
     <li>쉼표: ","</li> 
     <li>단어: "or", "and"</li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td><strong>포함</strong> </td> 
   <td>findText 문자열이 withinText 문자열 내에 있고 형식이 다음과 같이 지정된 경우 true를 반환합니다.

<p><code>CONTAINS(findText, withinText)</code></p></td> 
  </tr> 
  <tr> 
   <td><strong>ENCODEURL</strong> </td> 
   <td>URL 인수에 포함될 수 있도록 문자열의 모든 특수 문자를 이스케이프합니다.<p>표현식의 형식은 다음과 같습니다.</p>

<p><code>ENCODEURL(string)</code></p></td> 
  </tr> 
  <tr> 
   <td><strong>형식</strong> </td> 
   <td><p>서식 있는 텍스트를 반환합니다. 색상 옵션은 $$POSITIVE, $$INFORMATIVE, $$NEGATIVE, $$NOTICE이고, 기타 서식 옵션은 $$BOLD, $$ITALIC, $$UNDERLINE입니다. 최대 3개의 다른 서식 옵션과 함께 기능당 하나의 색상 옵션만 사용할 수 있습니다. 색상 옵션을 지정하지 않으면 시스템의 기본 색상이 적용됩니다.</p>
   <p>표현식의 형식은 다음과 같습니다.</p>
   <p><code>FORMAT($$POSITIVE, $$BOLD, $$ITALIC)</code></p>
   <p>참고: 이 표현식은 Workfront Planning에서 지원되지 않습니다.</p></td> 
  </tr>   
  <tr> 
   <td><strong>IF</strong> </td> 
   <td> <p>지정한 조건을 평가하고 true인 경우 trueExpression의 값을 반환하며, false인 경우 falseExpression의 값을 반환합니다.</p>

<p>표현식의 형식은 다음과 같습니다.</p>

<p><code>IF(condition, trueExpression, falseExpression)</code></p>

<p>예를 들어 두 개의 서로 다른 날짜 필드와 True/False 결과를 데이터 문자열로 비교할 수 있습니다.</p>

<p><code>IF({projectedCompletionDate}&gt;{plannedCompletionDate},"Off Track","On Track")</code></p>

<p>일상 대화에서 이 문은 "내 객체의 예상 완료 일자가 동일한 객체의 계획된 완료 일자보다 '큼'인 경우 이 필드에 '트랙외'라는 단어를 표시하고 그렇지 않은 경우 '트랙내'라는 단어를 표시합니다."를 의미합니다.</p>

<p>true 또는 false 표현식에 레이블을 지정하지 않으려면 다음과 같이 문에 빈 레이블을 삽입해야 합니다.</p>

<p><code>IF({projectedCompletionDate}&gt;{plannedCompletionDate},"","On Track")</code></p> 
   <p>또는</p>

<p><code>IF({projectedCompletionDate}&gt;{plannedCompletionDate},"Off Track","")</code></p>

<p>"IF" 문 작성에 대한 자세한 내용은 <a href="../../../reports-and-dashboards/reports/calc-cstm-data-reports/if-statements-overview.md" class="MCXref xref">"IF" 문 개요</a>를 참조하십시오.</p> </td> 
  </tr> 
  <tr> 
   <td><strong>IFIN</strong> </td> 
   <td> <p>가능한 값의 문자열에서 특정 값을 찾을 수 있습니다. 찾고 있는 값이 제공된 값 중 하나와 같으면 표현식은 trueExpression을 반환하고 그렇지 않으면 falseExpression을 반환합니다.</p> 
   <p>표현식의 형식은 다음과 같습니다.</p>

<p><code>IFIN(value, value1, value2,..., trueExpression, falseExpression)</code></p>

<p>예를 들어 특정 프로젝트 소유자를 찾아 프로젝트 보기에서 해당 프로젝트를 지정된 태그로 표시할 수 있습니다. <br><p><code>IFIN({owner}.{name},"Jennifer Campbell","Rick Kuvec","Marketing Team","Other Teams")
   </code></p>
    <p> 일상 연설에서 이 문장은 "프로젝트 소유자가 Jennifer Campbell 또는 Rick Kuvec인 경우 이 프로젝트를 '마케팅 팀'으로 표시하고, 그렇지 않은 경우 '기타 팀'으로 표시합니다."를 의미합니다.</p> 
    <p> true 또는 false 표현식에 레이블을 지정하지 않으려면 다음과 같이 문에 빈 레이블을 삽입해야 합니다. </p> 
    <p><code>IFIN({owner}.{name},"Jennifer Campbell","Rick Kuvec","","Other Teams")</code></p> 
    <p>또는 </p> 
    <p><code>IFIN({owner}.{name},"Jennifer Campbell","Rick Kuvec","Marketing Team","")</code></p> </p> </td> 
  </tr> 
  <tr> 
   <td><strong>IN</strong> </td> 
   <td> <p>값이 제공된 값 중 하나와 같으면 true를 반환하고, 그렇지 않으면 표현식에서 false를 반환합니다.</p> <p>표현식의 형식은 다음과 같습니다.

</p><p><code>IN(value, value1[, value2...])</code></p> </td> 
  </tr> 
  <tr> 
   <td><strong>ISBLANK</strong> </td> 
   <td> <p>값이 null이거나 비어 있으면 true를 반환합니다. 그렇지 않으면 표현식이 false를 반환합니다.</p> <p>표현식의 형식은 다음과 같습니다.

</p><p><code>ISBLANK(value)</code></p> </td> 
  </tr> 
  <tr> 
   <td><strong>왼쪽</strong> </td> 
   <td> <p>문자열의 왼쪽에서 지정된 문자 수를 반환하며 형식은 다음과 같습니다.</p>

<p><code>LEFT(string, length)</code></p> </td> 
  </tr> 
  <tr> 
   <td><strong>LEN</strong> </td> 
   <td> <p>문자열의 길이를 반환하고 형식을 다음과 같이 지정합니다.</p>

<p><code>LEN(string)</code></p> </td> 
  </tr> 
  <tr> 
   <td><strong>LOWER</strong> </td> 
   <td>문자열을 소문자로 반환하고 형식은 다음과 같이 지정합니다.

<p><code>LOWER(string)</code></p></td> 
  </tr> 
  <tr> 
   <td><strong>바꾸기</strong> </td> 
   <td> <p>string2의 모든 발생 횟수를 string1의 string3으로 바꿉니다.</p> <p>표현식의 형식은 다음과 같습니다.</p>

<p><code>REPLACE(string1, string2, string3)</code></p> </td> 
  </tr> 
  <tr> 
   <td><strong>오른쪽</strong> </td> 
   <td> <p>문자열 오른쪽에서 지정된 문자 수를 반환하며 형식은 다음과 같습니다.</p>

<p><code>RIGHT(string, length)</code></p> </td> 
  </tr> 
  <tr> 
   <td><strong>검색</strong> </td> 
   <td> <p>지정된 시작 위치에서 시작하는 문자열 withinText에서 findText의 첫 번째 발생 횟수 인덱스를 반환하거나 텍스트를 찾을 수 없는 경우 -1을 반환합니다.</p> <p>표현식의 형식은 다음과 같습니다.</p>

<p><code>SEARCH(findText, withinText, start)</code></p> </td> 
  </tr> 
  <tr> 
   <td><strong>문자열</strong> </td> 
   <td> <p>숫자를 문자열로 변환하고 형식을 다음과 같이 지정합니다.</p>

<p><code>STRING(number)</code></p> </td> 
  </tr>
  <tr> 
   <td><strong>SORTASCSTRING</strong> </td> 
   <td> <p>문자열 목록을 오름차순으로 정렬하고 형식을 다음과 같이 지정합니다.</p>
   <p><code>SORTASCSTRING(string1, string2, ...)</code></p> </td> 
  </tr>
  <tr> 
   <td><strong>SORTDESCSTRING</strong> </td> 
   <td> <p> 문자열 목록을 내림차순으로 정렬하고 형식을 다음과 같이 지정합니다.</p>
   <p><code>SORTDESCSTRING(string1, string2, ...)</code></p> </td> 
  </tr> 
  <tr> 
   <td><strong>하위 문자열</strong> </td> 
   <td> <p>지정된 시작 및 끝 인덱스를 기반으로 문자열의 문자를 반환하고 형식은 다음과 같습니다.</p>

<p><code>SUBSTR({string}, number of start position, number of end position)</code></p> </td> 
  </tr> 
  <tr> 
   <td><strong>전환</strong> </td> 
   <td> <p>표현식을 값의 목록과 비교하고, 일치하는 첫 번째 값에 해당하는 결과를 반환합니다.</p>
   <p>표현식의 형식은 다음과 같습니다.</p>
   <p><code>SWITCH(expression, value1, result1, [value2, result2], ...)</code></p>
   <p>이 표현식은 Workfront Planning에서 지원되지 않습니다.</p></td> 
  </tr>   
  <tr> 
   <td><strong>트리밍</strong> </td> 
   <td> <p>문자열의 시작과 끝에서 공백을 제거하고 형식을 다음과 같이 지정합니다.</p>

<p><code>TRIM(string)</code></p> </td> 
  </tr> 
  <tr> 
   <td><strong>UPPER</strong> </td> 
   <td> <p>문자열을 대문자로 반환하고 형식을 다음과 같이 지정합니다.</p>

<p><code>UPPER(string)</code></p> </td> 
  </tr> 
 </tbody> 
</table>
