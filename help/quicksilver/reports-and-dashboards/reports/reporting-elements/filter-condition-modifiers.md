---
product-area: reporting
navigation-topic: reporting-elements
title: Filter and condition modifiers
description: The filter and condition modifiers allow you to build filters and establish conditions for formatting your report results.
author: Courtney
feature: Reports and Dashboards
exl-id: 13e9d926-8a89-490e-aa7a-e6e8baf2a36b
source-git-commit: 6a6d3d47ed5741e3202c44b7240a2e67b687ea95
workflow-type: tm+mt
source-wordcount: '1593'
ht-degree: 0%

---

# Filter and condition modifiers

<!-- Audited: 11/2024 -->

<!--(NOTE: Alina: This is temporary - Lilit is fixing this in a future story: NOTE If the field you are filtering for has multiple options, this filters out the results that contain only the choice you specify. If the field contains additional options including the one specified, those results are not filtered from the report. See this document and search for "not equal" for the link to the req doc: https://docs.google.com/document/d/1WA0zZ_wws-2qb908i53BFQ8zDwL3nPJHyIybtJvvnqU/edit)-->

The filter and condition modifiers allow you to build filters and establish conditions for formatting your report results.

For more information about building filters, see the article [Filters overview](../../../reports-and-dashboards/reports/reporting-elements/filters-overview.md).

보기에서 조건부 서식 사용에 대한 자세한 내용은 [보기에서 조건부 서식 사용](../../../reports-and-dashboards/reports/reporting-elements/use-conditional-formatting-views.md) 문서를 참조하십시오.

## 필터 및 조건 수정자

일부 수정자는 내장되어 있으므로 필터 명령문이나 조건부 서식 명령문 내의 드롭다운 메뉴에서 선택할 수 있습니다. 다른 수정자는 텍스트 모드 필터에서만 사용할 수 있습니다.

텍스트 모드 이해에 대한 자세한 내용은 [텍스트 모드 개요](../../../reports-and-dashboards/reports/text-mode/understand-text-mode.md)를 참조하십시오.

기본 제공 시간 프레임 한정자 목록을 보려면 문서 [시간대별 보고서 필터링](/help/quicksilver/reports-and-dashboards/reports/creating-and-managing-reports/filter-reports-time-frames.md)을 참조하십시오.

You can use the following condition modifiers in filters and conditional formatting statements:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th> <p><strong>Built-in Modifier</strong> </p> </th> 
   <th> <p><strong>Text Mode Modifier</strong> </p> </th> 
   <th> <p><strong>설명</strong> </p> </th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr valign="top"> 
   <td> <p><strong>Is Blank</strong> </p> </td> 
   <td> <p><strong>blank</strong> </p> </td> 
   <td> <p>The field exists for the object but the field does not currently have a value.</p> </td> 
  </tr> 
  <tr valign="top"> 
   <td> <p><strong>Is Not Blank</strong> </p> </td> 
   <td> <p><strong>notblank</strong> </p> </td> 
   <td> <p>The field you are filtering for exists and has been given a value.</p> </td> 
  </tr> 
  <tr valign="top"> 
   <td> <p> </p> </td> 
   <td> <p><strong>null</strong> </p> </td> 
   <td> <p>필드가 비어 있거나 존재하지 않습니다. 예를 들어, 상위 작업 ID가 없는 항목을 찾을 수 있습니다. 즉, 독립형 작업만 볼 수 있습니다. ID가 없는 작업(이 경우 상위 작업)이 없으므로 "상위 작업 ID"의 한정자는 <strong>null</strong>이 됩니다. </p> <p>이 수정자는 텍스트 모드 필터에서만 사용할 수 있습니다. 필터의 텍스트 모드에 대한 자세한 내용은 <a href="../../../reports-and-dashboards/reports/text-mode/edit-text-mode-in-filter.md" class="MCXref xref">텍스트 모드를 사용하여 필터 편집</a>을 참조하세요.</p> </td> 
  </tr> 
  <tr valign="top"> 
   <td> <p> </p> </td> 
   <td> <p><strong>notnull</strong> </p> </td> 
   <td> <p>필터링하려는 필드가 존재하며 null 이외의 값을 포함합니다.</p> <p>이 수정자는 텍스트 모드 필터에서만 사용할 수 있습니다. 필터의 텍스트 모드에 대한 자세한 내용은 <a href="../../../reports-and-dashboards/reports/text-mode/edit-text-mode-in-filter.md" class="MCXref xref">텍스트 모드를 사용하여 필터 편집</a>을 참조하세요.</p> </td> 
  </tr> 
  <tr valign="top"> 
   <td> <p><strong>포함</strong> </p> </td> 
   <td> <p><strong>선명</strong> </p> </td> 
   <td> <p><i>포함</i>의 <strong>대/소문자를 구분하지 않는</strong> 버전입니다. 예: <code>cicontains inf</code>은(는) <code>Inf</code> 또는 <code>inf</code>을(를) 포함하는 모든 값을 캡처합니다.</p> <p> <p>Note: Adobe Workfront searches for the exact word or phrase that you are specifying for each filter statement. For example, if you are searching for any project that contains the phrase <code>new project</code> in the name, Workfront does not display projects that have just <code>new</code> or just <code>project</code>, or <code>new main project</code> in the name. The filter finds only projects with the exact phrase <code>new project</code> in the name.</p> </p> </td> 
  </tr> 
  <tr valign="top"> 
   <td> <p><strong>포함하지 않음</strong> </p> </td> 
   <td> <p><strong>cinotcontains</strong> </p> </td> 
   <td> <p><i>포함 안 함</i>의 <strong>대/소문자를 구분하지 않는</strong> 버전입니다.</p><p>이 수정자는 지정된 값이 없는 항목을 필터링합니다.</p> <p>예를 들어 <code>does not contain inf</code>은(는) 이름에 <code>Inf</code> 또는 <code>inf</code>이(가) 없는 모든 항목을 캡처합니다.</p> <p>Note: When applied to fields that contain multiple values (such as a collection of notes within a project), the filter determines exclusion as follows:
<ul>
    <li>If all items in a collection contain the specified text, the entire record is excluded from the results.</li>
    <li>If at least one item in the collection does not contain the specified text, the record remains in the results.</li>
</ul>
 </p> </td> 
  </tr> 
  <tr valign="top"> 
   <td> </td> 
   <td> <p><strong>포함</strong> </p> </td> 
   <td> <p> Searches for the specified <i>case sensitive</i> text throughout an entire text string.</p> <p>For example, using <code>contains Inf</code> captures anything with <code>Inf</code> in it, such as the word <code>Infinity.</code></p> <p>This modifier can only be used in text mode filters.For more information about text mode in filters, see <a href="../../../reports-and-dashboards/reports/text-mode/edit-text-mode-in-filter.md" class="MCXref xref">Edit a filter using text mode</a>.</p> </td> 
  <tr valign="top"> 
   <td> <p> </p> </td> 
   <td> <p><strong>notcontains</strong> </p> </td> 
   <td> <p>지정된 <i>대/소문자 구분</i> 값이 없는 항목을 필터링합니다.</p> <p>For example, <code>notcontains inf</code> captures anything without <code>inf</code>, but it displays values that contain <code>Inf</code>.</p> <p>This modifier can only be used in text mode filters. For more information about text mode in filters, see <a href="../../../reports-and-dashboards/reports/text-mode/edit-text-mode-in-filter.md" class="MCXref xref">Edit a filter using text mode</a>.</p> </td> 
  </tr> 
  </tr> 
  <tr valign="top"> 
   <td> <p> </p> </td> 
   <td> <p><strong>cieq</strong> </p> </td> 
   <td> <p>This is the <i>case insensitive</i> option of <strong>eq</strong>. It only returns an exact match of the searched value.</p> <p>예를 들어, 특정 이름의 작업을 검색할 때 <code>task name cieq test</code>은(는) 이름이 <code>Test</code>, <code>TEST</code> 또는 <code>Test</code>인 작업을 찾지만 해당 이름의 작업은 찾지 않습니다 <code>test 123.</code></p> <p>상태를 검색할 때 <strong>cieq</strong> 한정자는 지원되지 않습니다. 상태를 검색하려면 대/소문자 구분 한정자 <strong>eq</strong>을(를) 사용해야 합니다.</p> <p>This modifier can only be used in text mode filters. 필터의 텍스트 모드에 대한 자세한 내용은 <a href="../../../reports-and-dashboards/reports/text-mode/edit-text-mode-in-filter.md" class="MCXref xref">텍스트 모드를 사용하여 필터 편집</a>을 참조하세요.</p> </td>
  </tr> 
  <tr valign="top"> 
   <td> </td> 
   <td><strong>cine</strong> </td> 
   <td> <p>This is the <i>case insensitive</i> option of <strong>ne</strong>, and it is the opposite of the <b>cieq</b> modifier. It only returns results that are not an exact match of the searched value, not taking in account the case of the value.</p> <p>For example, <b>cine</b> returns any values that do not equal either "current" or "Current". </p> <p>This modifier can only be used in text mode filters. For more information about text mode in filters, see <a href="../../../reports-and-dashboards/reports/text-mode/edit-text-mode-in-filter.md" class="MCXref xref">Edit a filter using text mode</a>.</p> </td> 
  </tr>   <tr valign="top"> 
   <td> </td> 
   <td> <p><strong>eq</strong> </p> </td> 
   <td> <p>이 한정자는 검색된 값과 정확히 일치하는 <i>대/소문자 구분</i>만 반환합니다.</p> <p>예를 들어, 전체 프로젝트를 검색할 때 <code>eq CPL</code>은(는) 전체 상태의 모든 프로젝트를 반환합니다. 프로젝트를 완료하고 동시에 최신 상태로 유지할 수 없으므로 <code>eq CPL, CUR</code>에서 결과를 반환하지 않습니다.</p> <p>이 수정자는 텍스트 모드 필터에서만 사용할 수 있습니다. 필터의 텍스트 모드에 대한 자세한 내용은 <a href="../../../reports-and-dashboards/reports/text-mode/edit-text-mode-in-filter.md" class="MCXref xref">텍스트 모드를 사용하여 필터 편집</a>을 참조하세요.</p> </td> 
  </tr> 
  <tr valign="top"> 
   <td> </td> 
   <td><strong>ne</strong> </td> 
   <td> <p>This is the <i>case sensitive</i> opposite of <strong>eq</strong>. It returns only results that are not an exact match of the searched value, and it also matches the case of the value.</p> <p>For example, <b>ne</b> returns any values that do not equal "Current", but it does not return any values that do not equal "current". </p> <p>This modifier can only be used in text mode filters. For more information about text mode in filters, see <a href="../../../reports-and-dashboards/reports/text-mode/edit-text-mode-in-filter.md" class="MCXref xref">Edit a filter using text mode</a>.<br></p> </td> 
  </tr> 
  <tr valign="top"> 
   <td> <p> </p> </td> 
   <td> <p><strong>ciin</strong> </p> </td> 
   <td> <p> This is the <i>case insensitive</i> version of <strong>in</strong>.</p> <p>This modifier can only be used in text mode filters. For more information about text mode in filters, see <a href="../../../reports-and-dashboards/reports/text-mode/edit-text-mode-in-filter.md" class="MCXref xref">Edit a filter using text mode</a>.</p> </td> 
  </tr> 
  <tr valign="top"> 
   <td> <p> </p> </td> 
   <td> <p><strong>cinotin</strong> </p> </td> 
   <td> <p>This is the <i>case insensitive</i> version of <strong>notin</strong>.</p> <p>This modifier can only be used in text mode filters. 필터의 텍스트 모드에 대한 자세한 내용은 <a href="../../../reports-and-dashboards/reports/text-mode/edit-text-mode-in-filter.md" class="MCXref xref">텍스트 모드를 사용하여 필터 편집</a>을 참조하세요.</p> </td> 
  </tr> 
  <tr valign="top"> 
   <td> <p> </p> <p> </p> <p> </p> <p><strong>같음</strong> </p> </td> 
   <td> <p><strong>in</strong> </p> </td> 
   <td> <p>이 한정자를 사용하면 쉼표로 구분된 <i>대/소문자 구분</i> 변수 목록을 만들어 필터에서 평가된 단일 특성과 비교할 수 있습니다. 전체 목록이 OR 문으로 처리되고 하나 이상의 변수 기준에 맞는 결과를 반환합니다.</p> <p>예를 들어, 프로젝트를 검색할 때 <code>in CUR, PLN, CPL</code>을(를) 사용하면 현재, 계획 또는 완료 상태인 모든 프로젝트가 반환됩니다.</p> <p>기본 제공 한정자 <strong>Equal</strong>은(는) <strong>in</strong>의 텍스트 모드 한정자에 해당합니다. 즉, 필드에 대해 여러 값을 사용하여 [같음]을 선택할 수 있습니다.</p> <p>예를 들어, 프로젝트 보고서에서 "Status equals Current, Planning, Dead"를 선택할 수 있으며 이러한 상태의 프로젝트를 볼 수 있습니다.</p> </td> 
  </tr> 
  <tr valign="top"> 
   <td> <p><strong>같지 않음</strong> </p> </td> 
   <td> <p><strong>알림</strong> </p> </td> 
   <td> <p><i>in</i>과(와) 반대되는 <strong>대/소문자 구분</strong>입니다. 지정된 목록에 없는 결과만 반환합니다.</p> <p>This modifier can only be used in text mode filters. For more information about text mode in filters, see <a href="../../../reports-and-dashboards/reports/text-mode/edit-text-mode-in-filter.md" class="MCXref xref">Edit a filter using text mode</a>.</p> <p>Note: <span>If the field you are filtering for has multiple options, this filters out the results that contain both the choice you specify, as well as the choice you specify and any additional choices.</span> </p> </td> 
  </tr>
  <tr valign="top"> 
   <td> <p> </p> </td> 
   <td> <p><strong>like</strong> </p> </td> 
   <td> <p>이 한정자는 <i>포함</i>과 유사한 방식으로 <strong>대/소문자 구분</strong> 텍스트 문자열의 일부를 검색합니다. 그러나 <strong>좋아요</strong>를 사용하면 와일드카드 문자를 삽입하여 텍스트를 분리할 수 있습니다.</p> <p>예를 들어, 메모를 검색할 때 <code>like %Current% %Dead%</code>을(를) 사용하면 "Current to Dead" 구문이 포함된 모든 메모를 반환합니다. "Dead to Current"가 포함된 노트는 포함되지 않습니다. 각 값은 나열된 순서대로 검색됩니다. % 는 텍스트의 문자 또는 세그먼트를 바꾸는 와일드 카드를 나타냅니다. "Project" 및 "Projects"를 모두 반환하는 <code>like Project_</code>과 같이 단일 와일드카드 문자에 밑줄을 사용할 수도 있습니다. 필터링에 <strong>like</strong> 또는 <strong>like</strong> 한정자를 사용하려면 사용자 지정 데이터 필드 이름, 매개 변수 옵션 값 또는 기타 개체 이름에 % 또는 _ 문자를 사용하지 않는 것이 좋습니다.</p><p>이 수정자는 텍스트 모드 필터에서만 사용할 수 있습니다. 필터의 텍스트 모드에 대한 자세한 내용은 <a href="../../../reports-and-dashboards/reports/text-mode/edit-text-mode-in-filter.md" class="MCXref xref">텍스트 모드를 사용하여 필터 편집</a>을 참조하세요.</p> </td> 
  </tr>  
  <tr valign="top"> 
   <td> <p> </p> </td> 
   <td> <p><strong>섬모</strong> </p> </td> 
   <td> <p><i>좋아요</i>의 <strong>대/소문자를 구분하지 않는</strong> 버전입니다. 예: <code>cilike %Current% %Dead%</code>은(는) <code>Current to Dead</code> 또는 <code>current to dead</code>을(를) 포함하는 모든 메모를 반환합니다.</p> <p>이 수정자는 텍스트 모드 필터에서만 사용할 수 있습니다. 필터의 텍스트 모드에 대한 자세한 내용은 <a href="../../../reports-and-dashboards/reports/text-mode/edit-text-mode-in-filter.md" class="MCXref xref">텍스트 모드를 사용하여 필터 편집</a>을 참조하세요.</p> </td> 
  </tr> 
  <tr valign="top"> 
   <td><strong>존재하지 않음</strong> </td> 
   <td><strong>NOTEXISTS</strong> </td> 
   <td> <p>This modifier is used only with complex filters in an EXISTS statement. These filters refer only to the following objects: </p> 
    <ul> 
     <li>Objects that span multiple levels in the object hierarchy </li> 
     <li>Objects that are missing </li> 
    </ul> <p>For information about creating complex filters using EXISTS statements see the article <a href="../../../reports-and-dashboards/reports/text-mode/create-complex-text-mode-filters-using-exists-statements.md">Create Complex Text-Mode Filters Using EXISTS Statements</a>. This is the only modifier used in EXISTS statements.</p> </td> 
  </tr> 
  <tr valign="top"> 
   <td> <p><strong>보다 큼</strong> </p> </td> 
   <td> <p><strong>gt</strong> </p> </td> 
   <td> <p>입력한 값을 제외한 입력한 값보다 큰 값을 갖는 모든 결과가 검색됩니다.</p> </td> 
  </tr> 
  <tr valign="top"> 
   <td> <p><strong>보다 작음</strong> </p> </td> 
   <td> <p><strong>lt</strong> </p> </td> 
   <td> <p>This searches for all results with a value less than what is entered, not including the entered value.</p> </td> 
  </tr> 
  <tr valign="top"> 
   <td> <p><strong>Greater Than Equal</strong> </p> </td> 
   <td> <p><strong>gte</strong> </p> </td> 
   <td> <p>This searches for all results with values greater than or equal to the entered value.</p> </td> 
  </tr> 
  <tr valign="top"> 
   <td> <p><strong>Less Than Equal</strong> </p> </td> 
   <td> <p><strong>lte</strong> </p> </td> 
   <td> <p>This searches for all results with a value less than or equal to the entered value.</p> </td> 
  </tr> 
  <tr valign="top"> 
   <td> <p><strong>사이</strong> </p> </td> 
   <td> <p><strong>사이</strong> </p> </td> 
   <td> <p>두 개의 필수 필드 값을 제공하고 입력한 값을 포함하여 두 필드의 범위 내에 있는 모든 결과를 검색합니다.</p> </td> 
  </tr> 
  <tr valign="top"> 
   <td> <p> </p> </td> 
   <td> <p><strong>사이 아님</strong> </p> </td> 
   <td> <p><strong>between</strong>의 역입니다. 두 개의 필수 값 필드를 제공하고 입력한 값을 포함한 두 필드 범위 밖의 모든 결과를 검색합니다.</p> <p>This modifier can only be used in text mode filters. For more information about text mode in filters, see <a href="../../../reports-and-dashboards/reports/text-mode/edit-text-mode-in-filter.md" class="MCXref xref">Edit a filter using text mode</a>.</p> </td> 
  </tr>

</tbody> 
</table>
