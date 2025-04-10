---
product-area: reporting
navigation-topic: reporting-elements
title: 필터 및 조건 수정자
description: 필터 및 조건 수정자를 사용하여 필터를 작성하고 보고서 결과를 서식 지정하는 조건을 설정할 수 있습니다.
author: Nolan
feature: Reports and Dashboards
exl-id: 13e9d926-8a89-490e-aa7a-e6e8baf2a36b
source-git-commit: b2b17c34fe4887e291e69facf76f5071bca43b06
workflow-type: tm+mt
source-wordcount: '1565'
ht-degree: 0%

---

# 필터 및 조건 수정자

<!-- Audited: 11/2024 -->

<!--(NOTE: Alina: This is temporary - Lilit is fixing this in a future story: NOTE If the field you are filtering for has multiple options, this filters out the results that contain only the choice you specify. If the field contains additional options including the one specified, those results are not filtered from the report. See this document and search for "not equal" for the link to the req doc: https://docs.google.com/document/d/1WA0zZ_wws-2qb908i53BFQ8zDwL3nPJHyIybtJvvnqU/edit)-->

필터 및 조건 수정자를 사용하여 필터를 작성하고 보고서 결과를 서식 지정하는 조건을 설정할 수 있습니다.

필터 빌드에 대한 자세한 내용은 문서 [필터 개요](../../../reports-and-dashboards/reports/reporting-elements/filters-overview.md)를 참조하십시오.

보기에서 조건부 서식 사용에 대한 자세한 내용은 문서 [보기에서 조건부 서식 사용](../../../reports-and-dashboards/reports/reporting-elements/use-conditional-formatting-views.md)을 참조하십시오.

## 필터 및 조건 수정자

일부 수정자는 기본 제공되며 필터 또는 조건부 서식 명령문 내의 드롭다운 메뉴에서 선택할 수 있습니다. 다른 수정자는 텍스트 모드 필터에서만 사용할 수 있습니다.

텍스트 모드를 이해하는 방법에 대한 자세한 내용은 [텍스트 모드 개요](../../../reports-and-dashboards/reports/text-mode/understand-text-mode.md)를 참조하십시오.

기본 제공 시간 간격 수정자 목록을 보려면 문서 [시간대별 보고서 필터링](/help/quicksilver/reports-and-dashboards/reports/creating-and-managing-reports/filter-reports-time-frames.md)을 참조하십시오.

필터 및 조건부 서식 명령문에서 다음 조건 수정자를 사용할 수 있습니다.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th> <p><strong>기본 제공 한정자</strong> </p> </th> 
   <th> <p><strong>텍스트 모드 수정자</strong> </p> </th> 
   <th> <p><strong>설명</strong> </p> </th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr valign="top"> 
   <td> <p><strong>비어 있음</strong> </p> </td> 
   <td> <p><strong>blank</strong> </p> </td> 
   <td> <p>오브젝트에 대한 필드가 있지만 필드에 현재 값이 없습니다.</p> </td> 
  </tr> 
  <tr valign="top"> 
   <td> <p><strong>비어 있지 않음</strong> </p> </td> 
   <td> <p><strong>notblank</strong> </p> </td> 
   <td> <p>필터링 중인 필드가 존재하며 해당 필드에 값이 지정되었습니다.</p> </td> 
  </tr> 
  <tr valign="top"> 
   <td> <p> </p> </td> 
   <td> <p><strong>null</strong> </p> </td> 
   <td> <p>필드가 비어 있거나 존재하지 않습니다. 예를 들어 상위 작업 ID가 없는 항목을 찾으려고 합니다. 즉, 독립 실행형 작업만 표시하려고 합니다. ID(이 경우 상위)가 없는 작업이 없으므로 "상위 작업 ID"의 한정자는 <strong>null</strong>이 됩니다. </p> <p>이 수정자는 텍스트 모드 필터에서만 사용할 수 있습니다. 필터의 텍스트 모드에 대한 자세한 내용은 <a href="../../../reports-and-dashboards/reports/text-mode/edit-text-mode-in-filter.md" class="MCXref xref">텍스트 모드를 사용하여 필터 편집</a>을 참조하십시오.</p> </td> 
  </tr> 
  <tr valign="top"> 
   <td> <p> </p> </td> 
   <td> <p><strong>notnull</strong> </p> </td> 
   <td> <p>필터링하려는 필드가 존재하며 null 이외의 값을 포함합니다.</p> <p>이 수정자는 텍스트 모드 필터에서만 사용할 수 있습니다. 필터의 텍스트 모드에 대한 자세한 내용은 <a href="../../../reports-and-dashboards/reports/text-mode/edit-text-mode-in-filter.md" class="MCXref xref">텍스트 모드를 사용하여 필터 편집</a>을 참조하십시오.</p> </td> 
  </tr> 
  <tr valign="top"> 
   <td> <p><strong>포함</strong> </p> </td> 
   <td> <p><strong>범위</strong> </p> </td> 
   <td> <p><strong>포함</strong>의 <i>대/소문자를 구분하지 않음</i> 버전입니다. 예를 들어 <code>cicontains inf</code>은(는) <code>Inf</code> 또는 <code>inf</code>을(를) 포함하는 모든 값을 캡처합니다.</p> <p> <p>참고: Adobe Workfront은 각 필터 문에 대해 지정하는 정확한 단어 또는 구를 검색합니다. 예를 들어, 이름에 <code>new project</code> 구문이 포함된 프로젝트를 검색하는 경우 Workfront은 이름에 <code>new</code>, <code>project</code> 또는 <code>new main project</code>만 있는 프로젝트를 표시하지 않습니다. 필터에서 이름에 정확한 구 <code>new project</code>이(가) 있는 프로젝트만 찾습니다.</p> </p> </td> 
  </tr> 
  <tr valign="top"> 
   <td> <p><strong>다음을 포함하지 않음</strong> </p> </td> 
   <td> <p><strong>cinotcontains</strong> </p> </td> 
   <td> <p><strong>notcontains</strong>의 <i>대/소문자를 구분하지 않습니다</i> 버전입니다.</p><p>이 수정자는 지정된 값이 누락된 항목을 필터링합니다.</p> <p>예를 들어 <code>does not contain inf</code>은(는) 이름에 <code>Inf</code> 또는 <code>inf</code>이(가) 없는 모든 항목을 캡처합니다.</p> <p>참고: <span>필터링하려는 필드에 여러 옵션이 있는 경우, 이 옵션은 지정한 선택과 지정한 선택 및 추가 선택 항목이 모두 포함된 결과를 필터링합니다.</span> </p> </td> 
  </tr> 
  <tr valign="top"> 
   <td> </td> 
   <td> <p><strong>포함</strong> </p> </td> 
   <td> <p> 전체 텍스트 문자열에서 지정된 <i>대/소문자 구분</i> 텍스트를 검색합니다.</p> <p>예를 들어 <code>contains Inf</code>을(를) 사용하면 단어와 같이 <code>Inf</code>이(가) 포함된 모든 항목을 캡처합니다 <code>Infinity.</code></p> <p>이 수정자는 텍스트 모드 필터에서만 사용할 수 있습니다. 필터의 텍스트 모드에 대한 자세한 내용은 <a href="../../../reports-and-dashboards/reports/text-mode/edit-text-mode-in-filter.md" class="MCXref xref">텍스트 모드를 사용하여 필터 편집</a>을 참조하세요.</p> </td> 
  <tr valign="top"> 
   <td> <p> </p> </td> 
   <td> <p><strong>notcontains</strong> </p> </td> 
   <td> <p>지정한 <i>대/소문자 구분</i> 값이 없는 항목을 필터링합니다.</p> <p>예를 들어 <code>notcontains inf</code>은(는) <code>inf</code>이(가) 없는 모든 항목을 캡처하지만 <code>Inf</code>이(가) 포함된 값을 표시합니다.</p> <p>이 수정자는 텍스트 모드 필터에서만 사용할 수 있습니다. 필터의 텍스트 모드에 대한 자세한 내용은 <a href="../../../reports-and-dashboards/reports/text-mode/edit-text-mode-in-filter.md" class="MCXref xref">텍스트 모드를 사용하여 필터 편집</a>을 참조하십시오.</p> </td> 
  </tr> 
  </tr> 
  <tr valign="top"> 
   <td> <p> </p> </td> 
   <td> <p><strong>cieq</strong> </p> </td> 
   <td> <p><strong>eq</strong>의 <i>대/소문자를 구분하지 않는</i> 옵션입니다. 검색된 값과 정확히 일치하는 값만 반환합니다.</p> <p>예를 들어, 특정 이름의 작업을 검색할 때 <code>task name cieq test</code>은(는) 이름이 <code>Test</code>, <code>TEST</code> 또는 <code>Test</code>인 작업을 찾지만 해당 이름의 작업은 찾지 않습니다 <code>test 123.</code></p> <p>상태를 검색할 때 <strong>cieq</strong> 한정자는 지원되지 않습니다. 상태를 검색하려면 대/소문자를 구분하는 한정자 <strong>eq</strong>을(를) 사용해야 합니다.</p> <p>이 수정자는 텍스트 모드 필터에서만 사용할 수 있습니다. 필터의 텍스트 모드에 대한 자세한 내용은 <a href="../../../reports-and-dashboards/reports/text-mode/edit-text-mode-in-filter.md" class="MCXref xref">텍스트 모드를 사용하여 필터 편집</a>을 참조하십시오.</p> </td>
  </tr> 
  <tr valign="top"> 
   <td> </td> 
   <td><strong>cine</strong> </td> 
   <td> <p><strong>ne</strong>의 <i>대/소문자를 구분하지 않는</i> 옵션이며 <b>cieq</b> 수정자와 반대입니다. 값의 대/소문자를 구분하지 않고 검색된 값의 정확한 일치 결과가 아닌 결과만 반환합니다.</p> <p>예를 들어 <b>cine</b>은(는) "current" 또는 "Current"와 같지 않은 값을 반환합니다. </p> <p>이 수정자는 텍스트 모드 필터에서만 사용할 수 있습니다. 필터의 텍스트 모드에 대한 자세한 내용은 <a href="../../../reports-and-dashboards/reports/text-mode/edit-text-mode-in-filter.md" class="MCXref xref">텍스트 모드를 사용하여 필터 편집</a>을 참조하십시오.</p> </td> 
  </tr>   <tr valign="top"> 
   <td> </td> 
   <td> <p><strong>eq</strong> </p> </td> 
   <td> <p>이 한정자는 검색된 값과 정확히 일치하는 <i>대/소문자를 구분하는</i>만 반환합니다.</p> <p>예를 들어 전체 프로젝트를 검색할 때 <code>eq CPL</code>은(는) 완료 상태의 모든 프로젝트를 반환합니다. 프로젝트를 완료하고 동시에 현재 상태로 만들 수 없으므로 <code>eq CPL, CUR</code>에서 결과를 반환하지 않습니다.</p> <p>이 수정자는 텍스트 모드 필터에서만 사용할 수 있습니다. 필터의 텍스트 모드에 대한 자세한 내용은 <a href="../../../reports-and-dashboards/reports/text-mode/edit-text-mode-in-filter.md" class="MCXref xref">텍스트 모드를 사용하여 필터 편집</a>을 참조하십시오.</p> </td> 
  </tr> 
  <tr valign="top"> 
   <td> </td> 
   <td><strong>새</strong> </td> 
   <td> <p><strong>eq</strong>과(와) 반대의 <i>대/소문자 구분</i>입니다. 검색된 값과 정확히 일치하지 않는 결과만 반환하며 값의 대/소문자도 일치합니다.</p> <p>예를 들어 <b>ne</b>은(는) "Current"와 같지 않은 값은 반환하지만 "current"와 같지 않은 값은 반환하지 않습니다. </p> <p>이 수정자는 텍스트 모드 필터에서만 사용할 수 있습니다. 필터의 텍스트 모드에 대한 자세한 내용은 <a href="../../../reports-and-dashboards/reports/text-mode/edit-text-mode-in-filter.md" class="MCXref xref">텍스트 모드를 사용하여 필터 편집</a>을 참조하십시오.<br></p> </td> 
  </tr> 
  <tr valign="top"> 
   <td> <p> </p> </td> 
   <td> <p><strong>로그인</strong> </p> </td> 
   <td> <p> <strong>in</strong>의 <i>대/소문자를 구분하지 않는</i> 버전입니다.</p> <p>이 수정자는 텍스트 모드 필터에서만 사용할 수 있습니다. 필터의 텍스트 모드에 대한 자세한 내용은 <a href="../../../reports-and-dashboards/reports/text-mode/edit-text-mode-in-filter.md" class="MCXref xref">텍스트 모드를 사용하여 필터 편집</a>을 참조하십시오.</p> </td> 
  </tr> 
  <tr valign="top"> 
   <td> <p> </p> </td> 
   <td> <p><strong>cinotin</strong> </p> </td> 
   <td> <p><strong>알림</strong>의 <i>대/소문자를 구분하지 않는</i> 버전입니다.</p> <p>이 수정자는 텍스트 모드 필터에서만 사용할 수 있습니다. 필터의 텍스트 모드에 대한 자세한 내용은 <a href="../../../reports-and-dashboards/reports/text-mode/edit-text-mode-in-filter.md" class="MCXref xref">텍스트 모드를 사용하여 필터 편집</a>을 참조하십시오.</p> </td> 
  </tr> 
  <tr valign="top"> 
   <td> <p> </p> <p> </p> <p> </p> <p><strong>같음</strong> </p> </td> 
   <td> <p><strong>in</strong> </p> </td> 
   <td> <p>이 수정자를 사용하면 필터에서 평가된 단일 특성과 비교할 <i>대/소문자 구분</i> 변수의 쉼표로 구분된 목록을 만들 수 있습니다. 전체 목록은 OR 문으로 처리되며, 하나 이상의 변수 기준을 충족하는 결과를 반환합니다.</p> <p>예를 들어 프로젝트를 검색할 때 <code>in CUR, PLN, CPL</code>을(를) 사용하면 현재, OR 계획 또는 완료 상태의 모든 프로젝트가 반환됩니다.</p> <p>기본 제공 한정자 <strong>Equal</strong>은(는) <strong>in</strong>의 텍스트 모드 한정자에 해당합니다. 즉, 필드에 대해 여러 값을 사용하여 [같음]을 선택할 수 있습니다.</p> <p>예를 들어 프로젝트 보고서에서 "상태가 현재, 계획, 중단"을 선택할 수 있으며 이러한 상태 중 하나로 프로젝트를 볼 수 있습니다.</p> </td> 
  </tr> 
  <tr valign="top"> 
   <td> <p><strong>같지 않음</strong> </p> </td> 
   <td> <p><strong>알림</strong> </p> </td> 
   <td> <p><strong>in</strong>의 반대인 <i>대/소문자를 구분하는</i>입니다. 지정된 목록에 없는 결과만 반환합니다.</p> <p>이 수정자는 텍스트 모드 필터에서만 사용할 수 있습니다. 필터의 텍스트 모드에 대한 자세한 내용은 <a href="../../../reports-and-dashboards/reports/text-mode/edit-text-mode-in-filter.md" class="MCXref xref">텍스트 모드를 사용하여 필터 편집</a>을 참조하십시오.</p> <p>참고: <span>필터링하려는 필드에 여러 옵션이 있는 경우, 이 옵션은 지정한 선택과 지정한 선택 및 추가 선택 항목이 모두 포함된 결과를 필터링합니다.</span> </p> </td> 
  </tr>
  <tr valign="top"> 
   <td> <p> </p> </td> 
   <td> <p><strong>좋아요</strong> </p> </td> 
   <td> <p>이 한정자는 <strong>포함</strong>과 유사한 방식으로 <i>대/소문자를 구분하는</i> 텍스트 문자열의 일부를 검색합니다. 그러나 <strong>like</strong>에서는 와일드카드 문자를 삽입하여 텍스트를 구분하는 기능을 제공합니다.</p> <p>예를 들어 메모를 검색할 때 <code>like %Current% %Dead%</code>을(를) 사용하면 "Current to Dead" 구문을 포함하는 메모가 반환됩니다. "Dead to Current"가 포함된 노트는 포함되지 않습니다. 각 값은 나열된 순서대로 검색됩니다. %는 텍스트의 문자 또는 세그먼트를 바꿀 와일드카드를 나타냅니다. "Project"와 "Projects"를 모두 반환하는 <code>like Project_</code>에서와 같이 단일 와일드카드 문자에도 밑줄을 사용할 수 있습니다. 필터링에 <strong>like</strong> 또는 <strong>like</strong> 한정자를 사용하려는 경우 사용자 지정 데이터 필드 이름, 매개 변수 옵션 값 또는 기타 개체 이름에 % 또는 _ 문자를 사용하지 않는 것이 좋습니다.</p><p>이 수정자는 텍스트 모드 필터에서만 사용할 수 있습니다. 필터의 텍스트 모드에 대한 자세한 내용은 <a href="../../../reports-and-dashboards/reports/text-mode/edit-text-mode-in-filter.md" class="MCXref xref">텍스트 모드를 사용하여 필터 편집</a>을 참조하십시오.</p> </td> 
  </tr>  
  <tr valign="top"> 
   <td> <p> </p> </td> 
   <td> <p><strong>기능</strong> </p> </td> 
   <td> <p><strong>like</strong>의 <i>대/소문자를 구분하지 않습니다</i> 버전입니다. 예를 들어 <code>cilike %Current% %Dead%</code>은(는) <code>Current to Dead</code> 또는 <code>current to dead</code>이(가) 포함된 메모를 반환합니다.</p> <p>이 수정자는 텍스트 모드 필터에서만 사용할 수 있습니다. 필터의 텍스트 모드에 대한 자세한 내용은 <a href="../../../reports-and-dashboards/reports/text-mode/edit-text-mode-in-filter.md" class="MCXref xref">텍스트 모드를 사용하여 필터 편집</a>을 참조하십시오.</p> </td> 
  </tr> 
  <tr valign="top"> 
   <td><strong>존재하지 않음</strong> </td> 
   <td><strong>NOTEXISTS</strong> </td> 
   <td> <p>이 수정자는 EXISTS 문의 복잡한 필터에만 사용됩니다. 이 필터는 다음 개체만 참조합니다. </p> 
    <ul> 
     <li>객체 계층의 여러 레벨에 걸쳐 있는 객체 </li> 
     <li>누락된 오브젝트 </li> 
    </ul> <p>EXISTS 문을 사용하여 복합 필터를 만드는 방법에 대한 자세한 내용은 문서 <a href="../../../reports-and-dashboards/reports/text-mode/create-complex-text-mode-filters-using-exists-statements.md">EXISTS 문을 사용하여 복합 텍스트 모드 필터 만들기</a>를 참조하십시오. EXISTS 문에 사용되는 유일한 수정자입니다.</p> </td> 
  </tr> 
  <tr valign="top"> 
   <td> <p><strong>보다 큼</strong> </p> </td> 
   <td> <p><strong>gt</strong> </p> </td> 
   <td> <p>입력한 값이 포함되지 않고 입력한 값보다 큰 값이 있는 모든 결과가 검색됩니다.</p> </td> 
  </tr> 
  <tr valign="top"> 
   <td> <p><strong>보다 작음</strong> </p> </td> 
   <td> <p><strong>lt</strong> </p> </td> 
   <td> <p>입력한 값이 포함되지 않고 입력한 값보다 작은 값이 있는 모든 결과를 검색합니다.</p> </td> 
  </tr> 
  <tr valign="top"> 
   <td> <p><strong>같음</strong> </p> </td> 
   <td> <p><strong>gte</strong> </p> </td> 
   <td> <p>입력한 값보다 크거나 같은 값이 있는 모든 결과를 검색합니다.</p> </td> 
  </tr> 
  <tr valign="top"> 
   <td> <p><strong>같음</strong> </p> </td> 
   <td> <p><strong>lte</strong> </p> </td> 
   <td> <p>입력한 값보다 작거나 같은 값이 있는 모든 결과를 검색합니다.</p> </td> 
  </tr> 
  <tr valign="top"> 
   <td> <p><strong>사이</strong> </p> </td> 
   <td> <p><strong>사이</strong> </p> </td> 
   <td> <p>두 개의 필수 필드 값을 제공하고 입력한 값을 포함하여 두 필드의 범위 내에 있는 모든 결과를 검색합니다.</p> </td> 
  </tr> 
  <tr valign="top"> 
   <td> <p> </p> </td> 
   <td> <p><strong>notbetween</strong> </p> </td> 
   <td> <p><strong>between</strong>의 역버전입니다. 두 개의 필수 값 필드를 제공하고, 입력한 값을 포함하여 두 필드의 범위를 벗어나는 모든 결과를 검색합니다.</p> <p>이 수정자는 텍스트 모드 필터에서만 사용할 수 있습니다. 필터의 텍스트 모드에 대한 자세한 내용은 <a href="../../../reports-and-dashboards/reports/text-mode/edit-text-mode-in-filter.md" class="MCXref xref">텍스트 모드를 사용하여 필터 편집</a>을 참조하십시오.</p> </td> 
  </tr>

</tbody> 
</table>
