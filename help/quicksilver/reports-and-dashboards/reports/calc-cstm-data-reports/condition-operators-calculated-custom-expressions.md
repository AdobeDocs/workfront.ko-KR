---
content-type: reference
product-area: reporting
navigation-topic: calculate-custom-data-reports
title: 계산된 사용자 정의 표현식의 조건 연산자
description: 텍스트 모드를 사용할 때 Adobe Workfront에서 계산된 사용자 지정 데이터를 작성할 때 조건 연산자 또는 수정자를 사용할 수 있습니다.
author: Nolan
feature: Reports and Dashboards
exl-id: ce98ca39-cb86-4ef7-b75c-29ceb916e885
source-git-commit: e10fd7a3237d38ece8a5213990306ce511bd2412
workflow-type: tm+mt
source-wordcount: '731'
ht-degree: 1%

---

# 계산된 사용자 정의 필드의 조건 연산자

<!-- Audited: 2/2024 -->

텍스트 모드를 사용할 때 Adobe Workfront에서 계산된 사용자 지정 데이터를 작성할 때 조건 연산자 또는 수정자를 사용할 수 있습니다. Workfront에서 텍스트 모드를 사용하는 방법에 대한 자세한 내용은 [텍스트 모드 개요](../../../reports-and-dashboards/reports/text-mode/understand-text-mode.md)를 참조하십시오.

조건 연산자 또는 수정자는 문에서 기존 Workfront 필드를 연결하고 새 필드를 생성하여 조건문을 작성하는 데 도움이 됩니다. 조건 연산자의 가장 일반적인 사용은 &quot;IF&quot; 문의 조건을 작성하는 것입니다.

Workfront에서 &quot;IF&quot; 문을 사용하여 보고 및 사용자 지정 데이터 목적 모두에 대해 데이터 필드를 비교하고, 형식을 지정하며, 함께 문자열을 지정할 수 있습니다.

다음 Workfront 요소에 대해 &quot;IF&quot; 문을 작성할 수 있습니다.

* 보기
* 그룹화
* 계산된 사용자 정의 필드
* 비즈니스 규칙

&quot;IF&quot; 문 작성에 대한 자세한 내용은 [&quot;IF&quot; 문 개요](../../../reports-and-dashboards/reports/calc-cstm-data-reports/if-statements-overview.md)를 참조하십시오.

이 안내서의 예는 계산된 사용자 정의 필드에서 조건 연산자를 사용하는 방법을 보여 줍니다. 보고서의 계산된 사용자 정의 필드에 대한 올바른 구문을 따를 때 계산된 사용자 정의 열 또는 그룹화에서도 사용할 수 있습니다.

보고서의 계산된 사용자 지정 필드와 계산된 사용자 지정 데이터 간의 구문 차이에 대한 자세한 내용은 [계산된 사용자 지정 필드와 계산된 열](../../../reports-and-dashboards/reports/calc-cstm-data-reports/calculated-custom-fields-calculated-columns.md)을 참조하십시오.

비즈니스 규칙에 대한 자세한 내용은 [비즈니스 규칙 만들기 및 편집](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/business-rules.md)을 참조하세요.

계산된 사용자 정의 표현식에서 참조할 필드를 찾으려면 API 탐색기 를 참조하십시오. API 탐색기에 대한 자세한 내용은 [API 탐색기](../../../wf-api/general/api-explorer.md)를 참조하십시오.

Workfront에서 다음 조건 수정자를 사용할 수 있습니다.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th>조건 연산자</th> 
   <th>조건 연산자 구문</th> 
   <th>조건 연산자 정의</th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td>Equal</td> 
   <td>= </td> 
   <td> <p>이 연산자를 사용하여 명령문의 첫 번째 필드가 두 번째 필드와 같을 때 조건이 충족되었음을 나타냅니다.</p> <p>예를 들어 계산된 사용자 정의 필드에서 다음 문을 사용하여 계획된 완료 일자와 작업의 예상 완료 일자를 비교하는 "IF" 문을 작성할 수 있습니다. </p><p><code>IF({projectedCompletionDate}={plannedCompletionDate},"On Track","Off Track")</code></p> </td> 
  </tr> 
  <tr> 
   <td>보다 큼 </td> 
   <td>&gt; </td> 
   <td>이 연산자를 사용하여 명령문의 첫 번째 필드가 두 번째 필드보다 클 때 조건이 충족되었음을 나타냅니다. <p>예를 들어 계산된 사용자 정의 필드에서 다음 문을 사용하여 계획된 완료 일자와 작업의 예상 완료 일자를 비교하는 "IF" 문을 작성할 수 있습니다. </p><p><code>IF({projectedCompletionDate}&gt;{plannedCompletionDate},"Late","")</code></p></td> 
  </tr> 
  <tr> 
   <td>크거나 같음 </td> 
   <td>&gt;= </td> 
   <td>이 연산자를 사용하여 명령문의 첫 번째 필드가 두 번째 필드보다 크거나 같을 때 조건이 충족되었음을 나타냅니다. <p>예를 들어 계산된 사용자 정의 필드에서 다음 문을 사용하여 계획된 완료 일자와 작업의 예상 완료 일자를 비교하는 "IF" 문을 작성할 수 있습니다. </p><p><code>IF({projectedCompletionDate}&gt;={plannedCompletionDate},"Late","Early")</code></p></td> 
  </tr> 
  <tr> 
   <td>보다 작음 </td> 
   <td>&lt; </td> 
   <td>이 연산자를 사용하여 다음과 같은 경우 조건이 충족되었음을 나타냅니다.  명령문의 첫 번째 필드가 두 번째 필드보다 작습니다. <p>예를 들어 계산된 사용자 정의 필드에서 다음 문을 사용하여 계획된 완료 일자와 작업의 예상 완료 일자를 비교하는 "IF" 문을 작성할 수 있습니다. </p><p><code>IF({projectedCompletionDate}&lt;{plannedCompletionDate},"Early","")</code></p></td> 
  </tr> 
  <tr> 
   <td>작거나 같음 </td> 
   <td>&lt;= </td> 
   <td>이 연산자를 사용하여 다음과 같은 경우 조건이 충족되었음을 나타냅니다.  명령문의 첫 번째 필드가 두 번째 필드보다 작거나 같습니다. <p>예를 들어 계산된 사용자 정의 필드에서 다음 문을 사용하여 계획된 완료 일자와 작업의 예상 완료 일자를 비교하는 "IF" 문을 작성할 수 있습니다. </p><p><code>IF({projectedCompletionDate}&lt;={plannedCompletionDate},"Early","Late")</code></p></td> 
  </tr> 
  <tr> 
   <td>다음이 아님 </td> 
   <td>! </td> 
   <td> <p>위의 연산자 앞에 이 연산자를 추가하여 연산자를 무효화합니다. </p> <p>For example: </p> 
    <ul> 
     <li>같음: = </li> 
     <li>같지 않음: != </li> 
    </ul> <p>다음 데이터 표현식 앞에 이 연산자를 추가하면 표현식에 음수 문이 추가됩니다. </p> 
    <ul> 
     <li>포함 </li> 
     <li>안에 있음 </li> 
     <li>IFIN </li> 
     <li>ISBLANK </li> 
    </ul> <p>이러한 데이터 식에 대한 정보와 전체 목록은 <a href="../../../reports-and-dashboards/reports/calc-cstm-data-reports/calculated-data-expressions.md" class="MCXref xref">계산된 데이터 식의 개요</a>를 참조하십시오. </p> </td> 
  </tr> 
  <tr> 
   <td>또는 </td> 
   <td>|| </td> 
   <td> <p>이 연산자를 사용하여 표현식이 실행될 때 조건이 충족됨을 나타냅니다.  문의 첫 번째 또는 두 번째 값을 찾습니다. </p> <p>예를 들어 계산된 사용자 정의 필드에서 다음 문을 사용하여 현재 또는 계획 상태의 프로젝트를 "활성"으로 표시하는 "IF" 문을 작성합니다. </p><p><code>IF({status}="PLN"||{status}="CUR","Active","Not Active")</code></p> </td> 
  </tr> 
  <tr> 
   <td> 및 </td> 
   <td>&amp;&amp; </td> 
   <td> <p>이 연산자를 사용하여 표현식이 실행될 때 조건이 충족됨을 나타냅니다.  두 가지 조건을 동시에 충족하는 항목을 찾습니다. </p> <p>예를 들어 계산된 사용자 정의 필드에서 다음 문을 사용하여 현재 상태에 있고 위험 상태인 프로젝트를 찾아서 "조정 필요"로 표시하는 "IF" 문을 작성합니다. </p><p><code>IF({status}="CUR"&&{condition}="AR","Mediation Needed","")</code></p> </td> 
  </tr> 
 </tbody> 
</table>
