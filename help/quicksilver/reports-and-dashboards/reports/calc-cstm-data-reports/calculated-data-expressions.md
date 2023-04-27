---
content-type: reference
product-area: reporting
navigation-topic: calculate-custom-data-reports
title: 계산된 데이터 표현식
description: 데이터 표현식을 사용하여 Adobe Workfront에서 계산된 사용자 지정 데이터 필드를 정의할 수 있습니다. 새 필드를 생성하는 문에서 기존 Workfront 필드를 연결합니다.
author: Nolan
feature: Reports and Dashboards
exl-id: cfb3ace9-76c3-4006-878f-e2ad25ffa03b
source-git-commit: 1e91514f86a307ffa71cde650b35a2e3b8f0fa88
workflow-type: tm+mt
source-wordcount: '2302'
ht-degree: 7%

---

# 계산된 데이터 표현식

데이터 표현식을 사용하여 Adobe Workfront에서 계산된 사용자 지정 데이터 필드를 정의할 수 있습니다. 새 필드를 생성하는 문에서 기존 Workfront 필드를 연결합니다.

다음에서 계산된 데이터 표현식을 사용할 수 있습니다.

* 사용자 지정 양식

   Workfront에서 사용자 지정 양식에서 계산된 사용자 지정 데이터 필드를 만드는 방법에 대한 자세한 내용은 다음을 참조하십시오 [사용자 지정 양식에 계산된 데이터 추가](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/add-calculated-data-to-custom-form.md).

* 텍스트 모드를 사용하는 경우 보고서나 목록의 계산된 사용자 지정 열

   보고서 및 보기에서 텍스트 모드를 사용하는 방법에 대한 자세한 내용은 [텍스트 모드 개요](../../../reports-and-dashboards/reports/text-mode/understand-text-mode.md).

## 계산된 사용자 지정 필드의 구문과 계산된 사용자 지정 열 구문

사용하는 함수는 동일하지만 계산된 사용자 지정 필드에서 표현식을 작성하는 구문은 계산된 사용자 지정 열을 작성하는 구문과 다를 수 있습니다.

For example:

* 사용자 지정 필드의 사용자 지정 양식에서 사용자 지정 양식이 첨부된 작업의 상위 프로젝트의 이름을 생성하는 데 다음을 사용합니다.

   ```
   {project}.{name}
   ```

* 보고서의 사용자 지정 열에서 다음을 사용하여 작업 보고서에 프로젝트 이름 사용자 지정 열을 추가합니다.

   ```
   valuefield=project:name
   ```

   또는

   ```
   valueexpression={project}.{name}
   ```

   >[!TIP]
   >
   >계산된 표현식이 사용되는 모든 텍스트 모드 보고 요소에 동일한 구문이 적용됩니다. 보기, 필터, 그룹화, 프롬프트.

두 구문 간의 차이점은 다음과 같습니다.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td><strong>계산된 사용자 지정 필드</strong></td> 
   <td><strong>계산된 사용자 지정 보고 요소</strong></td> 
  </tr> 
   <td>필드 이름을 중괄호로 묶습니다.</td> 
   <td>괄호로 필드 이름을 묶지 마십시오 <code>valuefield </code>줄. <p>필드 이름을 중괄호로 묶습니다 <code>valueexpression</code> 줄.</p> </td> 
  </tr> 
  <tr> 
   <td>필드를 마침표로 구분합니다.</td> 
   <td> <p>에서 필드를 사용할 때 콜론으로 필드를 구분합니다 <code>valuefield </code>라인</p> <p>에서 필드를 사용할 때 마침표로 필드를 구분합니다 <code>valueexpression </code>줄. </p> </td> 
  </tr> 
 </tbody> 
</table>

계산된 사용자 지정 열에서 사용해야 하는 구문에 대한 자세한 내용은 [텍스트 모드 개요](../../../reports-and-dashboards/reports/text-mode/understand-text-mode.md).

## 사용할 수 있는 데이터 표현식

아래 목록은 Workfront에서 세 가지 서로 다른 유형의 계산된 사용자 지정 필드 중 하나를 작성할 때 사용할 수 있는 표현식을 정의합니다.

* [날짜 및 시간 계산된 사용자 지정 필드](#date-time-calculated-custom-fields)
* [수학 계산 사용자 지정 필드](#mathematical-calculated-custom-fields)
* [텍스트 계산된 사용자 지정 필드](#text-calculated-custom-fields)

### 날짜 및 시간 계산된 사용자 지정 필드 {#date-time-calculated-custom-fields}

>[!NOTE]
>
>시간부가 포함되지 않은 날짜 및 시간 계산을 생성하거나 날짜 와일드카드 $$TODAY 또는 $$NOW 를 사용하는 경우, 시스템은 현지 시간대가 아닌 UTC(Coordinated Universal Time) 영역에 따라 날짜를 사용합니다. 이로 인해 예기치 않은 날짜 결과가 발생할 수 있습니다.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th>표현식</th> 
   <th>설명 및 예</th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td><strong>ADDDAYS</strong> </td> 
   <td> <p>이 표현식은 날짜에 일 수를 추가합니다. 숫자 값에는 일부 일이 포함될 수 있습니다(예: 1.5는 날짜에 1일 반 추가).</p> <p>표현식의 형식은 다음과 같습니다.</p><pre>ADDDAYS(일자, 숫자)</pre> </td> 
  </tr> 
  <tr> 
   <td><strong>ADDWEEKDAYS</strong> </td> 
   <td> <p>이 표현식은 날짜에 평일 수를 추가합니다. 이 표현식은 날짜에 전체 정수 값만 추가하고 반올림합니다. </p> <p>표현식의 형식은 다음과 같습니다.</p><pre>ADDWEEKDAYS(date, number)</pre> </td> 
  </tr> 
  <tr> 
   <td><strong>ADDMONTHS</strong> </td> 
   <td> <p>이 표현식은 날짜에 개월 수를 추가하고 형식을 다음과 같이 지정합니다.</p><pre>ADDMONTHS(date, number)</pre> </td> 
  </tr> 
  <tr> 
   <td><strong>ADDYEARS</strong> </td> 
   <td> <p>이 표현식은 날짜에 연도 수를 추가하고 형식을 다음과 같이 지정합니다.</p><pre>ADDYEARS(일자, 숫자)</pre> </td> 
  </tr> 
  <tr> 
   <td><strong>CLEARTIME</strong> </td> 
   <td> <p>이 표현식은 날짜의 시간 부분을 지우고 다음과 같이 형식을 지정합니다. 이 예에서 날짜는 작업 객체의 시작 날짜입니다.</p><pre>CLEARTIME({entryDate})</pre> </td> 
  </tr> 
  <tr> 
   <td><strong>날짜</strong> </td> 
   <td> <p>이 표현식은 문자열을 날짜로 변환하며 다음과 같이 형식을 지정합니다.</p><pre>DATE(문자열)</pre> </td> 
  </tr> 
  <tr> 
   <td><strong>DATEDIFF</strong> </td> 
   <td> <p>이 표현식은 선택한 기간의 시작일과 종료일 및 해당 날짜의 타임스탬프를 고려하여 두 날짜 사이의 일 수를 반환합니다. 예를 들어 시작 날짜의 시작 시간이 오후 3시이면 시작 날짜는 전체 날짜로 계산되지 않습니다.</p> <p>표현식의 형식은 다음과 같습니다.</p><pre>DATEDIFF(date1, date2)</pre> </td> 
  </tr> 
  <tr> 
   <td><strong>DAYOFMONTH</strong> </td> 
   <td> <p>이 표현식은 1에서 31 사이의 숫자로 날짜에 대한 월의 일을 반환합니다.</p> <p>표현식의 형식은 다음과 같습니다. 이 예에서 날짜는 작업 객체의 시작 날짜입니다.</p><pre>DAYOFMONTH({entryDate})</pre> </td> 
  </tr> 
  <tr> 
   <td><strong>DAYOFWEEK</strong> </td> 
   <td> <p>이 표현식은 1(일요일)과 7(토요일) 사이의 날짜의 요일을 숫자로 반환합니다.</p> <p>표현식의 형식은 다음과 같습니다. 이 예에서 날짜는 작업 객체의 시작 날짜입니다.</p><pre>DAYOFWEEK({entryDate})</pre> </td> 
  </tr> 
  <tr> 
   <td><strong>DAYSINMONTH</strong> </td> 
   <td> <p>이 표현식은 날짜 월의 총 일 수를 숫자로 반환하며 다음과 같이 형식이 지정됩니다. 이 예에서 날짜는 작업 객체의 시작 날짜입니다.</p><pre>DAYSINMONTH({entryDate})</pre> </td> 
  </tr> 
  <tr> 
   <td><strong>DAYSINSPLITWEEK</strong> </td> 
   <td> <p>이 표현식은 날짜와 요일 사이 또는 그 달의 말일(둘 중 먼저 오는 일) 사이의 총 주일을 반환합니다. 이 예에서 날짜는 작업 객체의 시작 날짜입니다.</p> <p>표현식의 형식은 다음과 같습니다.</p><pre>DAYSINSPLITWEEK({entryDate})</pre> </td> 
  </tr> 
  <tr> 
   <td><strong>DAYSINYEAR</strong> </td> 
   <td> <p>이 표현식은 날짜의 연 총 일 수를 숫자로 반환하며 다음과 같이 형식이 지정됩니다. 이 예에서 날짜는 작업 객체의 시작 날짜입니다.</p><pre>DAYSINYEAR({entryDate})</pre> </td> 
  </tr> 
  <tr> 
   <td><strong>DMAX</strong> </td> 
   <td> <p>이 표현식은 목록에서 최신 날짜를 반환하고 형식을 다음과 같이 지정합니다.</p><pre>DMAX(date1, date2, ...)</pre> </td> 
  </tr> 
  <tr> 
   <td><strong>DMIN</strong> </td> 
   <td> <p>이 표현식은 목록에서 가장 이른 날짜를 반환하며 다음과 같이 형식을 지정합니다.</p><pre>DMIN(date1, date2, ...)</pre> </td> 
  </tr> 
  <tr> 
   <td><strong>시간</strong> </td> 
   <td> <p>이 표현식은 날짜의 시간을 0에서 23 사이의 숫자로 반환합니다.</p> <p>표현식의 형식은 다음과 같습니다. 이 예에서 날짜는 작업 객체의 시작 날짜입니다.</p><pre>HOUR({entryDate})</pre> </td> 
  </tr> 
  <tr> 
   <td><strong>분</strong> </td> 
   <td> <p>이 표현식은 다음과 같이 형식이 지정된 0에서 60 사이의 숫자로 날짜의 분을 반환합니다. 이 예에서 날짜는 작업 객체의 시작 날짜입니다.</p><pre>MINUTE({entryDate})</pre> </td> 
  </tr> 
  <tr> 
   <td><strong>개월</strong> </td> 
   <td> <p>이 표현식은 다음과 같이 형식이 지정된 날짜 월을 1에서 12 사이의 숫자로 반환합니다. 이 예에서 날짜는 작업 객체의 시작 날짜입니다.</p><pre>MONTH({entryDate})</pre> </td> 
  </tr> 
  <tr> 
   <td><strong>초</strong> </td> 
   <td> <p>이 표현식은 날짜의 두 번째 숫자를 0에서 60 사이의 숫자로 다음과 같이 반환합니다. 이 예에서 날짜는 작업 객체의 시작 날짜입니다.</p><pre>SECOND({entryDate})</pre> </td> 
  </tr> 
  <tr> 
   <td><strong>WEEKDAYDIFF</strong> </td> 
   <td> <p>이 표현식은 선택한 기간의 시작일과 종료일 및 해당 날짜의 타임스탬프를 고려하여 두 날짜 사이의 평일 수를 반환합니다. 예를 들어 시작 날짜의 시작 시간이 오후 3시이면 시작 날짜는 전체 날짜로 계산되지 않습니다.</p> <p>표현식의 형식은 다음과 같습니다.</p><pre>WEEKDAYDIFF(date2, date1)</pre> </td> 
  </tr> 
  <tr> 
   <td><strong>WORKMINUTESDIFF</strong> </td> 
   <td> <p>이 표현식은 기본 예약에 따라 날짜 사이의 예약된 시간(분)을 반환합니다.</p> <p>표현식의 형식은 다음과 같습니다.</p><pre>WORKMINUTESDIFF(date1, date2)</pre> </td> 
  </tr> 
  <tr> 
   <td><strong>년</strong> </td> 
   <td> <p>이 표현식은 날짜 연도를 다음과 같이 형식이 지정된 4자리 숫자로 반환합니다. 이 예에서 날짜는 작업 객체의 시작 날짜입니다.</p><pre>YEAR({entryDate})</pre> </td> 
  </tr> 
 </tbody> 
</table>

### 수학 계산 사용자 지정 필드 {#mathematical-calculated-custom-fields}

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
   <td>이 표현식은 숫자의 절대값을 반환하며 다음과 같이 형식이 지정됩니다. 이 예제에서는 사용자 지정 양식이 첨부된 개체 아래에 있는 개체 수를 사용합니다.<pre>ABS({numberOfChildren})</pre></td> 
  </tr> 
  <tr> 
   <td><strong>평균</strong> </td> 
   <td>이 표현식은 평균 숫자 값을 반환하며 다음과 같이 형식이 지정됩니다.<pre>AVERAGE(number1, number2, ...)</pre></td> 
  </tr> 
  <tr> 
   <td><strong>CEIL</strong> </td> 
   <td>이 표현식은 숫자를 가장 가까운 정수로 반올림하며 다음과 같이 형식을 지정합니다. 이 예제에서는 사용자 지정 양식이 첨부된 개체 아래에 있는 개체 수를 사용합니다.<pre>CEIL({numberOfChildren})</pre></td> 
  </tr> 
  <tr> 
   <td><strong>DIV</strong> </td> 
   <td>이 표현식은 제공된 순서대로 모든 숫자를 나눕니다.<pre>DIV(number1, number2, ...)</pre></td> 
  </tr> 
  <tr> 
   <td><strong>FLOOR</strong> </td> 
   <td>이 표현식은 숫자를 가장 가까운 정수로 반올림하고 다음과 같이 형식을 지정합니다. 이 예제에서는 사용자 지정 양식이 첨부된 개체 아래에 있는 개체 수를 사용합니다.<pre>FLOOR({numberOfChildren})</pre></td> 
  </tr> 
  <tr> 
   <td><strong>LN</strong> </td> 
   <td>이 표현식은 숫자의 자연 로그 값을 반환하며 다음과 같이 형식을 지정합니다.<pre>LN({numberOfChildren})</pre></td> 
  </tr> 
  <tr> 
   <td><strong>LOG</strong> </td> 
   <td>이 표현식은 number2의 로그 값을 base number1에 반환하며 다음과 같이 형식이 지정됩니다.<pre>LOG(number1, number2)</pre></td> 
  </tr> 
  <tr> 
   <td><strong>최대</strong> </td> 
   <td>이 표현식은 목록에서 가장 큰 항목을 반환하며 다음과 같이 형식을 지정합니다.<pre>MAX(item1, item2, ...)</pre></td> 
  </tr> 
  <tr> 
   <td><strong>최소</strong> </td> 
   <td>이 표현식은 목록에서 가장 작은 항목을 반환하며 다음과 같이 형식을 지정합니다.<pre>MIN(item1, item2, ...)</pre></td> 
  </tr> 
  <tr> 
   <td><strong>NUMBER</strong> </td> 
   <td>이 표현식은 문자열을 숫자로 변환하며 다음과 같이 형식을 지정합니다.<pre>NUMBER(string)</pre></td> 
  </tr> 
  <tr> 
   <td><strong>POWER</strong> </td> 
   <td>이 표현식은 전원으로 증가하는 숫자를 반환하며 다음과 같이 형식을 지정합니다.<pre>POWER(number, power)</pre></td> 
  </tr> 
  <tr> 
   <td><strong>PROD</strong> </td> 
   <td>이 표현식은 모든 숫자를 곱하고 형식을 다음과 같이 지정합니다.<pre>PROD(number1, number2, ....)</pre></td> 
  </tr> 
  <tr> 
   <td><strong>ROUND</strong> </td> 
   <td>이 표현식은 숫자를 지정된 소수점 자릿수로 반올림하며 다음과 같이 형식을 지정합니다.<p>ROUND(숫자, 정밀도)</p></td> 
  </tr> 
  <tr> 
   <td><strong>SORTASCNUM</strong> </td> 
   <td> <p> 이 표현식은 숫자가 오름차순으로 정렬되며, 형식은 다음과 같습니다.</p><pre>SORTASCNUM(number1, number2, ...)</pre> </td> 
  </tr> 
  <tr> 
   <td><strong>SORTDESCNUM</strong> </td> 
   <td>이 표현식은 숫자를 내림차순으로 정렬하며 다음과 같이 형식을 지정합니다.<pre>SORTDESCNUM(number1, number2, ...)</pre></td> 
  </tr> 
  <tr> 
   <td><strong>SQRT</strong> </td> 
   <td> <p>이 표현식은 숫자의 제곱근을 반환하며 다음과 같이 형식이 지정됩니다. 이 예제에서는 사용자 지정 양식이 첨부된 개체 아래에 있는 개체 수를 사용합니다.</p><pre>SQRT({numberOfChildren})</pre> </td> 
  </tr> 
  <tr> 
   <td><strong>SUB</strong> </td> 
   <td>이 표현식은 제공된 순서대로 모든 숫자를 빼고 다음 형식으로 지정합니다.<pre>SUB(number1, number2, ...)</pre></td> 
  </tr> 
  <tr> 
   <td><strong>SUM</strong> </td> 
   <td>이 표현식은 모든 숫자를 추가하고 형식을 다음과 같이 지정합니다.<pre>SUM(number1, number2, ...)</pre></td> 
  </tr> 
 </tbody> 
</table>

### 텍스트 계산된 사용자 지정 필드 {#text-calculated-custom-fields}

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
   <td> <p>이 표현식은 인덱스 번호를 기준으로 목록에서 값을 선택하는 다른 표현식과 함께 사용됩니다. 인덱스 번호는 숫자 값(일반적으로 알려진 범위)을 반환하는 필드 또는 함수입니다.</p> <p>표현식의 형식은 다음과 같습니다.</p><pre>CASE(indexNumber, value1, value2, ...)</pre> <p>예를 들어 다음 표현식은 계산된 열에서 요일 이름(1=Sunday, 2=Monday 등)을 반환합니다.</p><pre>CASE(DAYOFWEEK({entryDate}),"일요일","월요일","화요일","수요일","목요일","금요일","토요일")</pre> <p>이 표현식은 DAYOFWEEK, DAYOFMONTH 및 MONTH와 같이 숫자를 반환하는 다른 표현식에서 가장 잘 작동합니다.</p> </td> 
  </tr> 
  <tr> 
   <td><strong>CONCAT</strong> </td> 
   <td> <p>이 표현식은 문자열을 연결하며 다음과 같이 형식을 지정합니다.</p><pre>CONCAT(string1,"separator", string2)</pre> <p>다음은 포함할 수 있는 구분자의 예입니다.</p> 
    <ul> 
     <li>공백: "</li> 
     <li>대시: "-"</li> 
     <li>슬래시: "/"</li> 
     <li>쉼표: ","</li> 
     <li>단어: "or", "and"</li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td><strong>이(가) </strong>을(를) 포함 </td> 
   <td>이 표현식은 findText 문자열이 withinText 문자열 내에 있고 다음과 같은 형식의 경우 true를 반환합니다.<pre>포함(findText, withinText)</pre></td> 
  </tr> 
  <tr> 
   <td><strong>ENCODEURL</strong> </td> 
   <td>이 표현식은 문자열의 모든 특수 문자를 이스케이프하므로 URL 인수에 포함할 수 있습니다.<p>표현식의 형식은 다음과 같습니다.</p><pre>ENCODEURL(문자열)</pre></td> 
  </tr> 
  <tr> 
   <td><strong>IF</strong> </td> 
   <td> <p>이 표현식은 지정한 조건을 평가하고 true일 경우 trueExpression의 값을 반환하며, false일 경우 falseExpression의 값을 반환합니다.</p> <p>표현식의 형식은 다음과 같습니다.</p><pre>IF(condition, trueExpression, falseExpression)</pre> <p>예를 들어 다음 두 개의 서로 다른 날짜 필드 뒤에 True/False 결과를 데이터 문자열로 비교할 수 있습니다.</p><pre>IF({projectedCompletionDate}&gt;{계획된CompletionDate},"추적 해제","추적 중")</pre> <p>이 성명은 일상 연설에서 다음을 의미합니다. "내 객체의 예상 완료 날짜가 내 객체의 계획 완료 날짜보다 큼"이면 이 필드에 'Off Track'이라는 단어를 표시합니다. 그렇지 않으면 'On Track'이라는 단어를 표시합니다.</p> <p>true 또는 false 표현식에 레이블을 지정하지 않으려면 다음과 같이 문에 빈 레이블을 삽입해야 합니다.</p><pre>IF({projectedCompletionDate}&gt;{계획된CompletionDate},"","추적")</pre> <p>또는</p><pre>IF({projectedCompletionDate}&gt;{계획된CompletionDate},"추적 해제","")</pre> <p>"IF" 문 빌드에 대한 자세한 내용은 <a href="../../../reports-and-dashboards/reports/calc-cstm-data-reports/if-statements-overview.md" class="MCXref xref">"IF" 문 개요</a>.</p> </td> 
  </tr> 
  <tr> 
   <td><strong>IFIN</strong> </td> 
   <td> <p>이 표현식을 사용하면 가능한 값 문자열에서 특정 값을 찾을 수 있습니다. 찾고 있는 값이 제공된 값 중 하나와 같으면 표현식이 trueExpression;을 반환합니다. 그렇지 않으면 falseExpression을 반환합니다.</p> <p>표현식의 형식은 다음과 같습니다.</p><pre>IFIN(값, 값1, 값2,.., trueExpression, falseExpression)</pre> <p>예를 들어 특정 프로젝트 소유자를 찾아 프로젝트 보기에서 지정된 태그로 해당 프로젝트를 표시할 수 있습니다. <br><code>IFIN({owner}.{name},"Jennifer Campbell","Rick Kuvec","Marketing Team","Other Teams")</code></p> <p> 이 성명은 일상 연설에서 다음을 의미합니다. 만약 프로젝트 소유자가 제니퍼 캠벨이나 릭 쿠벡이라면, 이 프로젝트를 '마케팅 팀'으로 표시하세요; 그렇지 않으면 '기타 팀'으로 표시합니다."</p> <p> true 또는 false 표현식에 레이블을 지정하지 않으려면 다음과 같이 문에 빈 레이블을 삽입해야 합니다. </p> <p><code>IFIN({owner}.{name},"Jennifer Campbell","Rick Kuvec","","Other Teams")</code></p> <p>또는 </p> <p><code>IFIN({owner}.{name},"Jennifer Campbell","Rick Kuvec","Marketing Team",""</code> </p> </td> 
  </tr> 
  <tr> 
   <td></strong>의 <strong> </strong></td> 
   <td> <p>값이 제공된 값 중 하나와 같은 경우 이 표현식은 true를 반환합니다. 그렇지 않으면 표현식이 false를 반환합니다.</p> <p>표현식의 형식은 다음과 같습니다.</p><pre>IN(value, value1[, value2...])</pre> </td> 
  </tr> 
  <tr> 
   <td><strong>ISBLANK</strong> </td> 
   <td> <p>값이 null이거나 비어 있으면 이 표현식은 true를 반환합니다. 그렇지 않으면 표현식이 false를 반환합니다.</p> <p>표현식의 형식은 다음과 같습니다.</p><pre>ISBLANK(value)</pre> </td> 
  </tr> 
  <tr> 
   <td><strong>LEFT</strong> </td> 
   <td> <p>이 표현식은 문자열 왼쪽에서 지정된 수의 문자를 반환하며 다음과 같이 형식을 지정합니다.</p><pre>LEFT(string, length)</pre> </td> 
  </tr> 
  <tr> 
   <td><strong>LEN</strong> </td> 
   <td> <p>이 표현식은 문자열 길이를 반환하며 다음과 같이 형식을 지정합니다.</p><pre>LEN(string)</pre> </td> 
  </tr> 
  <tr> 
   <td><strong>더 낮음</strong> </td> 
   <td>이 표현식은 문자열을 소문자로 반환하며 다음과 같이 형식을 지정합니다.<pre>LOWER(문자열)</pre></td> 
  </tr> 
  <tr> 
   <td><strong>바꾸기</strong> </td> 
   <td> <p>이 표현식은 string1에서 string2의 모든 항목을 string3으로 바꿉니다.</p> <p>표현식의 형식은 다음과 같습니다.</p><pre>REPLACE(string1, string2, string3)</pre> </td> 
  </tr> 
  <tr> 
   <td><strong>RIGHT</strong> </td> 
   <td> <p>이 표현식은 문자열 오른쪽에서 지정된 수의 문자를 반환하며 다음과 같이 형식이 지정됩니다.</p><pre>오른쪽(문자열, 길이)</pre> </td> 
  </tr> 
  <tr> 
   <td><strong>검색</strong> </td> 
   <td> <p>이 표현식은 지정된 시작 위치에서 시작하여 Text 내의 문자열에 있는 findText의 첫 번째 발생 인덱스를 반환하거나 텍스트를 찾을 수 없으면 -1을 반환합니다.</p> <p>표현식의 형식은 다음과 같습니다.</p><pre>SEARCH(findText, withinText, start)</pre> </td> 
  </tr> 
  <tr> 
   <td><strong>문자열</strong> </td> 
   <td> <p>이 표현식은 숫자를 문자열로 변환하고 형식을 다음과 같이 지정합니다.</p><pre>STRING(숫자)</pre> </td> 
  </tr> 
  <tr> 
   <td><strong>SORTASCSTRING</strong> </td> 
   <td> <p>이 표현식은 문자열 목록을 오름차순으로 정렬하며 형식은 다음과 같습니다.</p><pre>SORTASCSTRING(string1, string2, ...)</pre> </td> 
  </tr> 
  <tr> 
   <td><strong>SORTDESCSTRING</strong> </td> 
   <td> <p> 이 표현식은 문자열 목록을 내림차순으로 정렬하며 형식을 다음과 같이 지정합니다.</p><pre>SORTDESCSTRING(string1, string2, ...)</pre> </td> 
  </tr> 
  <tr> 
   <td><strong>SUBSTR</strong> </td> 
   <td> <p>이 표현식은 지정된 시작 및 종료 인덱스를 기반으로 문자열의 문자를 반환하며 다음과 같이 형식을 지정합니다.</p><pre>SUBSTR({string}, 시작 위치 수, 종료 위치 수)</pre> </td> 
  </tr> 
  <tr> 
   <td><strong>트리밍</strong> </td> 
   <td> <p>이 표현식은 문자열의 시작과 끝에서 공백을 제거하고 다음과 같이 형식을 지정합니다.</p><pre>TRIM(문자열)</pre> </td> 
  </tr> 
  <tr> 
   <td><strong>UPPER</strong> </td> 
   <td> <p>이 표현식은 대소문자를 구분하는 문자열을 반환하며 다음과 같이 형식을 지정합니다.</p><pre>UPPER(string)</pre> </td> 
  </tr> 
 </tbody> 
</table>
