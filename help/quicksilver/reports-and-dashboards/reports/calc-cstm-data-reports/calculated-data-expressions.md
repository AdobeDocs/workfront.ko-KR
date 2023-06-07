---
content-type: reference
product-area: reporting
navigation-topic: calculate-custom-data-reports
title: 계산된 데이터 표현식
description: 데이터 표현식을 사용하여 Adobe Workfront에서 계산된 사용자 정의 데이터 필드를 정의할 수 있습니다. 새 필드를 생성하는 문에서 기존 Workfront 필드를 연결합니다.
author: Nolan
feature: Reports and Dashboards
exl-id: cfb3ace9-76c3-4006-878f-e2ad25ffa03b
source-git-commit: 18f26f976a47af003817f2f82f8550bdfbc0ab90
workflow-type: tm+mt
source-wordcount: '2368'
ht-degree: 7%

---

# 계산된 데이터 표현식

데이터 표현식을 사용하여 Adobe Workfront에서 계산된 사용자 정의 데이터 필드를 정의할 수 있습니다. 새 필드를 생성하는 문에서 기존 Workfront 필드를 연결합니다.

다음에서 계산된 데이터 표현식을 사용할 수 있습니다.

* 사용자 정의 양식

   Workfront의 사용자 정의 양식에서 계산된 사용자 정의 데이터 필드를 만드는 방법에 대한 자세한 내용은 [사용자 정의 양식에 계산된 데이터 추가](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/add-calculated-data-to-custom-form.md).

* 텍스트 모드를 사용할 때 보고서 또는 목록의 계산된 사용자 지정 열

   보고서 및 보기에서 텍스트 모드를 사용하는 방법에 대한 자세한 내용은 [텍스트 모드 개요](../../../reports-and-dashboards/reports/text-mode/understand-text-mode.md).

## 계산된 사용자 정의 필드와 계산된 사용자 정의 열의 구문

사용하는 함수는 동일하지만 계산된 사용자 정의 필드에 표현식을 작성하는 구문은 계산된 사용자 정의 열을 작성하는 구문과 다를 수 있습니다.

For example:

* 사용자 정의 필드의 작업에 대한 사용자 정의 양식에서 다음을 사용하여 사용자 정의 양식이 첨부된 작업의 상위 프로젝트 이름을 생성합니다.

   ```
   {project}.{name}
   ```

* 보고서의 사용자 정의 열에서 다음을 사용하여 작업 보고서에 프로젝트 이름 사용자 정의 열을 추가합니다.

   ```
   valuefield=project:name
   ```

   또는

   ```
   valueexpression={project}.{name}
   ```

   >[!TIP]
   >
   >계산된 표현식이 사용되는 모든 텍스트 모드 보고 요소(보기, 필터, 그룹화, 프롬프트)에도 동일한 구문이 적용됩니다.

두 구문 간의 차이점은 다음과 같습니다.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td><strong>계산된 사용자 정의 필드</strong></td> 
   <td><strong>계산된 사용자 지정 보고 요소</strong></td> 
  </tr> 
   <td>필드 이름은 중괄호로 묶습니다.</td> 
   <td>에서 필드 이름을 사용할 때 대괄호나 괄호로 묶지 마십시오. <code>valuefield </code>줄. <p>필드 이름을 사용할 때 중괄호로 묶습니다. <code>valueexpression</code> 줄.</p> </td> 
  </tr> 
  <tr> 
   <td>필드를 마침표로 구분합니다.</td> 
   <td> <p>에서 필드를 사용할 때 콜론으로 구분합니다. <code>valuefield </code>line</p> <p>에서 사용할 때 필드를 마침표로 구분합니다. <code>valueexpression </code>줄. </p> </td> 
  </tr> 
 </tbody> 
</table>

계산된 사용자 지정 열에서 사용해야 하는 구문에 대한 자세한 내용은 [텍스트 모드 개요](../../../reports-and-dashboards/reports/text-mode/understand-text-mode.md).

## 사용할 수 있는 데이터 표현식

아래 목록은 Workfront에서 세 가지 유형의 계산된 사용자 정의 필드 중 하나를 작성할 때 사용할 수 있는 표현식을 정의합니다.

* [계산된 날짜 및 시간 사용자 정의 필드](#date-time-calculated-custom-fields)
* [계산된 수학 사용자 정의 필드](#mathematical-calculated-custom-fields)
* [계산된 사용자 정의 필드 텍스트](#text-calculated-custom-fields)

### 계산된 날짜 및 시간 사용자 정의 필드 {#date-time-calculated-custom-fields}

>[!NOTE]
>
>시간 부분을 포함하지 않거나 날짜 와일드카드 $$TODAY 또는 $$NOW를 사용하는 날짜 및 시간 계산을 만드는 경우, 시스템은 현지 시간대가 아닌 UTC(협정 세계시) 시간대에 따라 날짜를 사용합니다. 이로 인해 예상치 못한 날짜 결과가 발생할 수 있습니다.

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
   <td> <p>이 표현식은 날짜에 일수를 추가합니다. 숫자 값은 부분적인 일을 포함할 수 있습니다(예: 1.5는 날짜에 1일 반일을 추가합니다).</p> <p>표현식의 형식은 다음과 같습니다.</p><pre>ADDDAYS(일자, 숫자)</pre> </td> 
  </tr> 
  <tr> 
   <td><strong>ADDWEEKDAYS</strong> </td> 
   <td> <p>이 표현식은 날짜에 평일 수를 추가합니다. 이 표현식은 날짜에 정수 값만 추가하여 내림합니다. </p> <p>표현식의 형식은 다음과 같습니다.</p><pre>ADDWEEKDAYS(date, number)</pre> </td> 
  </tr> 
  <tr> 
   <td><strong>ADDMONTHS</strong> </td> 
   <td> <p>이 표현식은 날짜에 개월 수를 추가하고 형식은 다음과 같습니다.</p><pre>ADDMONTHS(date, number)</pre> </td> 
  </tr> 
  <tr> 
   <td><strong>ADDYEARS</strong> </td> 
   <td> <p>이 표현식은 날짜에 연도 수를 추가하고 형식은 다음과 같습니다.</p><pre>ADDYEARS(일자, 숫자)</pre> </td> 
  </tr> 
  <tr> 
   <td><strong>CLEARTIME</strong> </td> 
   <td> <p>이 표현식은 날짜의 시간 부분을 지우고 형식을 다음과 같이 지정합니다. 이 예에서 날짜는 작업 객체의 입력 날짜입니다.</p><pre>CLEARTIME({entryDate})</pre> </td> 
  </tr> 
  <tr> 
   <td><strong>날짜</strong> </td> 
   <td> <p>이 표현식은 문자열을 날짜로 전환하며 형식은 다음과 같습니다.</p><pre>DATE(문자열)</pre> </td> 
  </tr> 
  <tr> 
   <td><strong>DATEDIFF</strong> </td> 
   <td> <p>이 표현식은 선택한 기간의 시작 날짜와 종료 날짜 및 해당 날짜의 타임스탬프를 고려하여 두 날짜 사이의 일 수를 반환합니다. 예를 들어 시작 일자의 시작 시간이 오후 3시인 경우 시작 일은 전일로 계산되지 않습니다.</p> <p>표현식의 형식은 다음과 같습니다.</p><pre>DATEDIFF(date1, date2)</pre> </td> 
  </tr> 
  <tr> 
   <td><strong>DAYOFMONTH</strong> </td> 
   <td> <p>이 표현식은 1과 31 사이의 숫자로 날짜의 월 중 일을 반환합니다.</p> <p>표현식의 형식은 다음과 같습니다. 이 예에서 날짜는 작업 객체의 입력 날짜입니다.</p><pre>DAYOFMONTH({entryDate})</pre> </td> 
  </tr> 
  <tr> 
   <td><strong>DAYOFWEEK</strong> </td> 
   <td> <p>이 표현식은 1(일요일)과 7(토요일) 사이의 숫자로 날짜의 요일을 반환합니다.</p> <p>표현식의 형식은 다음과 같습니다. 이 예에서 날짜는 작업 객체의 입력 날짜입니다.</p><pre>DAYOFWEEK({entryDate})</pre> </td> 
  </tr> 
  <tr> 
   <td><strong>DAYSINMONTH</strong> </td> 
   <td> <p>이 표현식은 날짜의 월간 총 일수를 숫자로 반환하며 형식은 다음과 같습니다. 이 예에서 날짜는 작업 객체의 입력 날짜입니다.</p><pre>DAYSINMONTH({entryDate})</pre> </td> 
  </tr> 
  <tr> 
   <td><strong>DAYSINSPLITWEEK</strong> </td> 
   <td> <p>이 표현식은 날짜와 주의 끝 또는 월의 끝 중 먼저 도래하는 날짜 사이의 총 평일을 반환합니다. 이 예에서 날짜는 작업 객체의 입력 날짜입니다.</p> <p>표현식의 형식은 다음과 같습니다.</p><pre>DAYSINSPLITWEEK({entryDate})</pre> </td> 
  </tr> 
  <tr> 
   <td><strong>DAYSINYEAR</strong> </td> 
   <td> <p>이 표현식은 날짜의 연중 총 일수를 숫자로 반환하며 형식은 다음과 같습니다. 이 예에서 날짜는 작업 객체의 입력 날짜입니다.</p><pre>DAYSINYEAR({entryDate})</pre> </td> 
  </tr> 
  <tr> 
   <td><strong>DMAX</strong> </td> 
   <td> <p>이 표현식은 목록의 최신 날짜를 반환하며 형식은 다음과 같습니다.</p><pre>DMAX(date1, date2, ...)</pre> </td> 
  </tr> 
  <tr> 
   <td><strong>DMIN</strong> </td> 
   <td> <p>이 표현식은 목록에서 가장 빠른 날짜를 반환하며 형식은 다음과 같습니다.</p><pre>DMIN(date1, date2, ...)</pre> </td> 
  </tr> 
  <tr> 
   <td><strong>시간</strong> </td> 
   <td> <p>이 표현식은 날짜의 시간을 0과 23 사이의 숫자로 반환합니다.</p> <p>표현식의 형식은 다음과 같습니다. 이 예에서 날짜는 작업 객체의 입력 날짜입니다.</p><pre>HOUR({entryDate})</pre> </td> 
  </tr> 
  <tr> 
   <td><strong>분</strong> </td> 
   <td> <p>이 표현식은 다음과 같이 형식이 지정된 0과 60 사이의 숫자로 날짜의 분을 반환합니다. 이 예에서 날짜는 작업 객체의 입력 날짜입니다.</p><pre>MINUTE({entryDate})</pre> </td> 
  </tr> 
  <tr> 
   <td><strong>개월</strong> </td> 
   <td> <p>이 표현식은 다음과 같이 형식이 지정된 1과 12 사이의 숫자로 날짜 월을 반환합니다. 이 예에서 날짜는 작업 객체의 입력 날짜입니다.</p><pre>MONTH({entryDate})</pre> </td> 
  </tr> 
  <tr> 
   <td><strong>초</strong> </td> 
   <td> <p>이 표현식은 다음과 같이 형식이 지정된 0과 60 사이의 숫자로 날짜의 초를 반환합니다. 이 예에서 날짜는 작업 객체의 입력 날짜입니다.</p><pre>SECOND({entryDate})</pre> </td> 
  </tr> 
  <tr> 
   <td><strong>WEEKDAYDIFF</strong> </td> 
   <td> <p>이 표현식은 선택한 기간의 시작 날짜와 종료 날짜, 해당 날짜의 타임스탬프를 고려하여 두 날짜 사이의 평일 수를 반환합니다. 예를 들어 시작 일자의 시작 시간이 오후 3시인 경우 시작 일은 전일로 계산되지 않습니다.</p> <p>표현식의 형식은 다음과 같습니다.</p><pre>WEEKDAYDIFF(date2, date1)</pre> </td> 
  </tr> 
  <tr> 
   <td><strong>WORKMINUTESDIFF</strong> </td> 
   <td> <p>이 표현식은 기본 일정에 따라 날짜 사이의 예약된 시간(분)을 반환합니다.</p> <p>표현식의 형식은 다음과 같습니다.</p><pre>WORKMINUTESDIFF(date1, date2)</pre> </td> 
  </tr> 
  <tr> 
   <td><strong>년</strong> </td> 
   <td> <p>이 표현식은 다음과 같은 형식의 4자리 숫자로 날짜의 연도를 반환합니다. 이 예에서 날짜는 작업 객체의 입력 날짜입니다.</p><pre>YEAR({entryDate})</pre> </td> 
  </tr> 
 </tbody> 
</table>

### 계산된 수학 사용자 정의 필드 {#mathematical-calculated-custom-fields}

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
   <td><strong>ABS</strong> </td> 
   <td>이 식은 숫자의 절대값을 반환하며 형식은 다음과 같습니다. 이 예제에서는 사용자 정의 양식이 첨부된 오브젝트 아래에 있는 오브젝트의 수를 사용합니다.<pre>ABS({numberOfChildren})</pre></td> 
  </tr> 
  <tr> 
   <td><strong>평균</strong> </td> 
   <td>이 표현식은 숫자의 평균을 반환하며 형식은 다음과 같습니다.<pre>AVERAGE(number1, number2, ...)</pre></td> 
  </tr> 
  <tr> 
   <td><strong>CEIL</strong> </td> 
   <td>이 표현식은 숫자를 가장 가까운 정수로 반올림하며 형식은 다음과 같습니다. 이 예제에서는 사용자 정의 양식이 첨부된 오브젝트 아래에 있는 오브젝트의 수를 사용합니다.<pre>CEIL({numberOfChildren})</pre></td> 
  </tr> 
  <tr> 
   <td><strong>DIV</strong> </td> 
   <td>이 표현식은 모든 숫자를 제공된 순서대로 나누며 형식은 다음과 같습니다.<pre>DIV(number1, number2, ...)</pre></td> 
  </tr> 
  <tr> 
   <td><strong>FLOOR</strong> </td> 
   <td>이 표현식은 숫자를 가장 가까운 정수로 내림하고 형식을 다음과 같이 지정합니다. 이 예제에서는 사용자 정의 양식이 첨부된 오브젝트 아래에 있는 오브젝트의 수를 사용합니다.<pre>FLOOR({numberOfChildren})</pre></td> 
  </tr> 
  <tr> 
   <td><strong>LN</strong> </td> 
   <td>이 표현식은 숫자의 자연 로그 값을 반환하며 형식은 다음과 같습니다.<pre>LN({numberOfChildren})</pre></td> 
  </tr> 
  <tr> 
   <td><strong>LOG</strong> </td> 
   <td>이 표현식은 기본 number1에 대한 number2의 로그 값을 반환하며 형식은 다음과 같습니다.<pre>LOG(number1, number2)</pre></td> 
  </tr> 
  <tr> 
   <td><strong>최대</strong> </td> 
   <td>이 표현식은 목록에서 가장 큰 항목을 반환하며 형식은 다음과 같습니다.<pre>MAX(item1, item2, ...)</pre></td> 
  </tr> 
  <tr> 
   <td><strong>최소</strong> </td> 
   <td>이 표현식은 목록에서 가장 작은 항목을 반환하며 형식은 다음과 같습니다.<pre>MIN(item1, item2, ...)</pre></td> 
  </tr> 
  <tr> 
   <td><strong>NUMBER</strong> </td> 
   <td>이 표현식은 문자열을 숫자로 전환하고 형식을 다음과 같이 지정합니다.<pre>NUMBER(string)</pre></td> 
  </tr> 
  <tr> 
   <td><strong>POWER</strong> </td> 
   <td>이 표현식은 제곱한 숫자를 반환하며 형식은 다음과 같습니다.<pre>POWER(number, power)</pre></td> 
  </tr> 
  <tr> 
   <td><strong>PROD</strong> </td> 
   <td>이 표현식은 모든 숫자를 곱하고 형식을 다음과 같이 지정합니다.<pre>PROD(number1, number2, ....)</pre>
   <b>메모</b>

시간이 포함된 필드에 곱할 때 선택한 필드의 시간이 데이터베이스에 분, 시간 또는 초 단위로 저장되는지 여부를 이해해야 합니다. 시간이 분 또는 초 단위로 저장되지만 Workfront 인터페이스에 시간 단위로 표시되는 경우 이 계산을 사용하여 표현식을 작성할 때 분 또는 초에서 시간으로 변환해야 할 수 있습니다.
</td> 
  </tr> 
  <tr> 
   <td><strong>ROUND</strong> </td> 
   <td>이 표현식은 지정한 정밀도 소수점으로 숫자를 반올림하며 형식은 다음과 같습니다.<p>ROUND(숫자, 정밀도)</p></td> 
  </tr> 
  <tr> 
   <td><strong>SORTASCNUM</strong> </td> 
   <td> <p> 이 표현식은 숫자를 오름차순으로 정렬하며 형식은 다음과 같습니다.</p><pre>SORTASCNUM(number1, number2, ...)</pre> </td> 
  </tr> 
  <tr> 
   <td><strong>SORTDESCNUM</strong> </td> 
   <td>이 표현식은 숫자를 내림차순으로 정렬하며 형식은 다음과 같습니다.<pre>SORTDESCNUM(number1, number2, ...)</pre></td> 
  </tr> 
  <tr> 
   <td><strong>SQRT</strong> </td> 
   <td> <p>이 표현식은 숫자의 제곱근을 반환하며 형식은 다음과 같습니다. 이 예제에서는 사용자 정의 양식이 첨부된 오브젝트 아래에 있는 오브젝트의 수를 사용합니다.</p><pre>SQRT({numberOfChildren})</pre> </td> 
  </tr> 
  <tr> 
   <td><strong>SUB</strong> </td> 
   <td>이 표현식은 제공된 순서대로 모든 숫자를 뺍니다. 형식은 다음과 같습니다.<pre>SUB(number1, number2, ...)</pre></td> 
  </tr> 
  <tr> 
   <td><strong>합계</strong> </td> 
   <td>이 표현식은 모든 숫자를 추가하고 형식은 다음과 같습니다.<pre>SUM(number1, number2, ...)</pre></td> 
  </tr> 
 </tbody> 
</table>

### 계산된 사용자 정의 필드 텍스트 {#text-calculated-custom-fields}

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
   <td><strong>사례</strong> </td> 
   <td> <p>이 표현식은 색인 번호를 기반으로 목록에서 값을 선택하는 데 다른 표현식과 함께 사용됩니다. 색인 번호는 숫자 값(일반적으로 알려진 범위)을 반환하는 필드 또는 함수입니다.</p> <p>표현식의 형식은 다음과 같습니다.</p><pre>CASE(indexNumber, value1, value2, ...)</pre> <p>예를 들어, 다음 표현식은 계산된 열에서 1=일요일, 2=월요일 등 요일의 이름을 반환합니다.</p><pre>CASE(DAYOFWEEK({entryDate}),"Sunday","Monday","Tuesday","Wednesday","Thursday","Friday","Saturday")</pre> <p>이 표현식은 DAYOFWEEK, DAYOFMONTH 및 MONTH와 같이 숫자를 반환하는 다른 표현식에 가장 적합합니다.</p> </td> 
  </tr> 
  <tr> 
   <td><strong>CONCAT</strong> </td> 
   <td> <p>이 표현식은 문자열을 연결하고 형식을 다음과 같이 지정합니다.</p><pre>CONCAT(string1,"separator", string2)</pre> <p>다음은 포함할 수 있는 구분 기호의 예입니다.</p> 
    <ul> 
     <li>공백: " "</li> 
     <li>대시: "-"</li> 
     <li>슬래시: "/"</li> 
     <li>쉼표: ","</li> 
     <li>단어: "or", "and"</li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td><strong>이(가) </strong>을(를) 포함 </td> 
   <td>이 식은 findText 문자열이 withinText 문자열 내에 있고 형식이 다음과 같이 지정된 경우 true를 반환합니다.<pre>포함(findText, withinText)</pre></td> 
  </tr> 
  <tr> 
   <td><strong>ENCODEURL</strong> </td> 
   <td>이 표현식은 문자열의 모든 특수 문자를 이스케이프하므로 URL 인수에 포함될 수 있습니다.<p>표현식의 형식은 다음과 같습니다.</p><pre>ENCODEURL(문자열)</pre></td> 
  </tr> 
  <tr> 
   <td><strong>IF</strong> </td> 
   <td> <p>이 표현식은 사용자가 지정하는 조건을 평가하고 true인 경우 trueExpression의 값을 반환하며, false인 경우 falseExpression의 값을 반환합니다.</p> <p>표현식의 형식은 다음과 같습니다.</p><pre>IF(condition, trueExpression, falseExpression)</pre> <p>예를 들어 두 개의 서로 다른 날짜 필드와 True/False 결과를 데이터 문자열로 비교할 수 있습니다.</p><pre>IF({projectedCompletionDate}&gt;{plannedCompletionDate},"Off Track","On Track")</pre> <p>일상 대화에서 이 문은 "내 객체의 예상 완료 일자가 동일한 객체의 계획된 완료 일자보다 '큼'인 경우 이 필드에 '트랙외'라는 단어를 표시하고 그렇지 않은 경우 '트랙내'라는 단어를 표시합니다."를 의미합니다.</p> <p>true 또는 false 표현식에 레이블을 지정하지 않으려면 다음과 같이 문에 빈 레이블을 삽입해야 합니다.</p><pre>IF({projectedCompletionDate}&gt;{plannedCompletionDate},","트랙에")</pre> <p>또는</p><pre>IF({projectedCompletionDate}&gt;{plannedCompletionDate},"Off Track",")</pre> <p>"IF" 문 작성에 대한 자세한 내용은 <a href="../../../reports-and-dashboards/reports/calc-cstm-data-reports/if-statements-overview.md" class="MCXref xref">"IF" 문 개요</a>.</p> </td> 
  </tr> 
  <tr> 
   <td><strong>IFIN</strong> </td> 
   <td> <p>이 표현식을 사용하면 가능한 값의 문자열에서 특정 값을 찾을 수 있습니다. 찾고 있는 값이 제공된 값 중 하나와 같으면 표현식은 trueExpression을 반환하고 그렇지 않으면 falseExpression을 반환합니다.</p> <p>표현식의 형식은 다음과 같습니다.</p><pre>IFIN(value, value1, value2,..., trueExpression, falseExpression)</pre> <p>예를 들어 특정 프로젝트 소유자를 찾아 프로젝트 보기에서 해당 프로젝트를 지정된 태그로 표시할 수 있습니다. <br><code>IFIN({owner}.{name},"Jennifer Campbell","Rick Kuvec","Marketing Team","Other Teams")</code></p> <p> 일상 연설에서 이 문장은 "프로젝트 소유자가 Jennifer Campbell 또는 Rick Kuvec인 경우 이 프로젝트를 '마케팅 팀'으로 표시하고, 그렇지 않은 경우 '기타 팀'으로 표시합니다."를 의미합니다.</p> <p> true 또는 false 표현식에 레이블을 지정하지 않으려면 다음과 같이 문에 빈 레이블을 삽입해야 합니다. </p> <p><code>IFIN({owner}.{name},"Jennifer Campbell","Rick Kuvec","","Other Teams")</code></p> <p>또는 </p> <p><code>IFIN({owner}.{name},"Jennifer Campbell","Rick Kuvec","Marketing Team",""</code> </p> </td> 
  </tr> 
  <tr> 
   <td></strong>의 <strong> </strong></td> 
   <td> <p>이 표현식은 값이 제공된 값 중 하나와 같으면 true를 반환하고, 그렇지 않으면 false를 반환합니다.</p> <p>표현식의 형식은 다음과 같습니다.</p><pre>IN(value, value1[, value2...])</pre> </td> 
  </tr> 
  <tr> 
   <td><strong>ISBLANK</strong> </td> 
   <td> <p>이 표현식은 값이 null이거나 비어 있으면 true를 반환하고 그렇지 않으면 false를 반환합니다.</p> <p>표현식의 형식은 다음과 같습니다.</p><pre>ISBLANK(value)</pre> </td> 
  </tr> 
  <tr> 
   <td><strong>LEFT</strong> </td> 
   <td> <p>이 표현식은 문자열의 왼쪽에서 지정된 문자 수를 반환하며 형식은 다음과 같습니다.</p><pre>LEFT(string, length)</pre> </td> 
  </tr> 
  <tr> 
   <td><strong>LEN</strong> </td> 
   <td> <p>이 표현식은 문자열의 길이를 반환하며 형식은 다음과 같습니다.</p><pre>LEN(string)</pre> </td> 
  </tr> 
  <tr> 
   <td><strong>더 낮음</strong> </td> 
   <td>이 표현식은 문자열을 소문자로 반환하며 형식은 다음과 같습니다.<pre>LOWER(문자열)</pre></td> 
  </tr> 
  <tr> 
   <td><strong>바꾸기</strong> </td> 
   <td> <p>이 표현식은 string2의 모든 발생 횟수를 string1의 string3으로 바꿉니다.</p> <p>표현식의 형식은 다음과 같습니다.</p><pre>REPLACE(string1, string2, string3)</pre> </td> 
  </tr> 
  <tr> 
   <td><strong>RIGHT</strong> </td> 
   <td> <p>이 표현식은 문자열의 오른쪽에서 지정된 문자 수를 반환하며 형식은 다음과 같습니다.</p><pre>오른쪽(문자열, 길이)</pre> </td> 
  </tr> 
  <tr> 
   <td><strong>검색</strong> </td> 
   <td> <p>이 식은 지정된 시작 위치에서 시작하는 문자열 withinText에서 findText의 첫 번째 발생 횟수 인덱스를 반환하거나 텍스트를 찾을 수 없는 경우 -1을 반환합니다.</p> <p>표현식의 형식은 다음과 같습니다.</p><pre>SEARCH(findText, withinText, start)</pre> </td> 
  </tr> 
  <tr> 
   <td><strong>문자열</strong> </td> 
   <td> <p>이 표현식은 숫자를 문자열로 변환하고 형식은 다음과 같습니다.</p><pre>STRING(number)</pre> </td> 
  </tr> 
  <tr> 
   <td><strong>SORTASCSTRING</strong> </td> 
   <td> <p>이 식은 문자열 목록을 오름차순으로 정렬하며 형식은 다음과 같습니다.</p><pre>SORTASCSTRING(string1, string2, ...)</pre> </td> 
  </tr> 
  <tr> 
   <td><strong>SORTDESCSTRING</strong> </td> 
   <td> <p> 이 표현식은 문자열 목록을 내림차순으로 정렬하며 형식은 다음과 같습니다.</p><pre>SORTDESCSTRING(string1, string2, ...)</pre> </td> 
  </tr> 
  <tr> 
   <td><strong>SUBSTR</strong> </td> 
   <td> <p>이 표현식은 지정된 시작 및 끝 인덱스를 기반으로 문자열의 문자를 반환하며 형식은 다음과 같습니다.</p><pre>SUBSTR({string}, 시작 위치 수, 끝 위치 수)</pre> </td> 
  </tr> 
  <tr> 
   <td><strong>트리밍</strong> </td> 
   <td> <p>이 표현식은 문자열의 시작과 끝에서 공백을 제거하고 형식은 다음과 같습니다.</p><pre>TRIM(문자열)</pre> </td> 
  </tr> 
  <tr> 
   <td><strong>UPPER</strong> </td> 
   <td> <p>이 표현식은 문자열을 대문자로 반환하며 형식은 다음과 같습니다.</p><pre>UPPER(string)</pre> </td> 
  </tr> 
 </tbody> 
</table>
