---
product-area: reporting
navigation-topic: reporting-elements
title: 필터 및 조건 수정자
description: 필터 및 조건 수정자를 사용하여 필터를 빌드하고 보고서 결과 서식을 위한 조건을 설정할 수 있습니다.
author: Lisa
feature: Reports and Dashboards
exl-id: 13e9d926-8a89-490e-aa7a-e6e8baf2a36b
source-git-commit: 442e0b8fde9e4acaa2686ccd292fb003f72be623
workflow-type: tm+mt
source-wordcount: '1556'
ht-degree: 1%

---

# 필터 및 조건 수정자

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: Alina: This is temporary - Lilit is fixing this in a future story: NOTE If the field you are filtering for has multiple options, this filters out the results that contain only the choice you specify. If the field contains additional options including the one specified, those results are not filtered from the report. See this document and search for "not equal" for the link to the req doc: https://docs.google.com/document/d/1WA0zZ_wws-2qb908i53BFQ8zDwL3nPJHyIybtJvvnqU/edit) </p>
-->

필터 및 조건 수정자를 사용하여 필터를 빌드하고 보고서 결과 서식을 위한 조건을 설정할 수 있습니다.

필터 만들기에 대한 자세한 내용은 문서를 참조하십시오 [Adobe Workfront의 필터 개요](../../../reports-and-dashboards/reports/reporting-elements/filters-overview.md).

보기에서 조건부 서식을 사용하는 방법에 대한 자세한 내용은 문서를 참조하십시오 [보기에서 조건부 서식 사용](../../../reports-and-dashboards/reports/reporting-elements/use-conditional-formatting-views.md).

## 필터 및 조건 수정자

기본 제공 기간 수정자 목록을 보려면 문서를 참조하십시오 [기간별로 보고서 필터링](../../../reports-and-dashboards/reports/creating-and-managing-reports/filter-reports-time-frames.md).

일부 수정자는 기본적으로 제공되며 필터 또는 조건문 내의 드롭다운 메뉴에서 선택할 수 있습니다. 기타 수정자는 텍스트 모드 필터에서만 사용할 수 있습니다. 텍스트 모드 이해에 대한 자세한 내용은 [텍스트 모드 개요](../../../reports-and-dashboards/reports/text-mode/understand-text-mode.md).

필터 및 조건부 서식 명령문에서 다음 조건 한정자를 사용할 수 있습니다.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th> <p><strong>기본 제공 수정자</strong> </p> </th> 
   <th> <p><strong>텍스트 모드 수정자</strong> </p> </th> 
   <th> <p><strong>설명</strong> </p> </th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr valign="top"> 
   <td> <p><strong>비어 있음</strong> </p> </td> 
   <td> <p><strong>공백</strong> </p> </td> 
   <td> <p>객체에 대한 필드가 있지만 필드에 값이 아직 지정되지 않았습니다.</p> </td> 
  </tr> 
  <tr valign="top"> 
   <td> <p><strong>비어 있지 않음</strong> </p> </td> 
   <td> <p><strong>비어 있지 않음</strong> </p> </td> 
   <td> <p>필터링하는 필드가 존재하며 값이 제공되었습니다.</p> </td> 
  </tr> 
  <tr valign="top"> 
   <td> <p> </p> </td> 
   <td> <p><strong>null</strong> </p> </td> 
   <td> <p>필드가 비어 있거나 존재하지 않습니다. 예를 들어 상위 작업 ID가 없는 항목을 찾습니다. 이는 독립형 작업만 표시하려는 것을 의미합니다. "상위 작업 ID"의 한정자는 다음과 같습니다 <strong>null</strong>ID가 없는 작업(이 경우 상위)이 존재하지 않으므로 </p> <p>이 수정자는 텍스트 모드 필터에서만 사용할 수 있습니다. 필터의 텍스트 모드에 대한 자세한 내용은 <a href="../../../reports-and-dashboards/reports/text-mode/edit-text-mode-in-filter.md" class="MCXref xref">텍스트 모드를 사용하여 필터 편집</a>.</p> </td> 
  </tr> 
  <tr valign="top"> 
   <td> <p> </p> </td> 
   <td> <p><strong>null</strong> </p> </td> 
   <td> <p>필터링하는 필드가 존재하며 null 이외의 값을 포함합니다.</p> <p>이 수정자는 텍스트 모드 필터에서만 사용할 수 있습니다. 필터의 텍스트 모드에 대한 자세한 내용은 <a href="../../../reports-and-dashboards/reports/text-mode/edit-text-mode-in-filter.md" class="MCXref xref">텍스트 모드를 사용하여 필터 편집</a>.</p> </td> 
  </tr> 
  <tr valign="top"> 
   <td> <p><strong>포함:</strong> </p> </td> 
   <td> <p><strong>ciconcontains</strong> </p> </td> 
   <td> <p>(대/소문자 구분 안 함) 대/소문자를 구분하지 않는 버전 <strong>다음 포함</strong>. 예: "ciconcontains inf"는 "Inf" 또는 "inf"를 포함하는 모든 값을 캡처합니다.</p> <p> <p>참고: Adobe Workfront은 각 필터 문에 대해 지정하는 정확한 단어 또는 구를 검색합니다. 예를 들어 이름에 "새 프로젝트" 구문을 포함하는 프로젝트를 검색하는 경우 Workfront에 이름에 "신규", "프로젝트" 또는 "새 기본 프로젝트"만 있는 프로젝트가 표시되지 않습니다. 이 필터는 이름에 "새 프로젝트" 구문을 정확히 사용하는 프로젝트만 찾습니다.</p> </p> </td> 
  </tr> 
  <tr valign="top"> 
   <td> <p> </p> </td> 
   <td> <p><strong>cieq</strong> </p> </td> 
   <td> <p>(대/소문자 구분 안 함) 다음 중 대/소문자를 구분하지 않는 옵션입니다. <strong>eq</strong>. 검색된 값의 정확한 일치만 반환합니다.</p> <p>예를 들어, 특정 이름으로 작업을 검색할 때 "작업 이름 cieq test"는 이름이 "Test", "TEST" 또는 "Test"인 작업을 찾지만 이름이 "test 123"인 작업은 찾지 못합니다.</p> <p>이 수정자는 텍스트 모드 필터에서만 사용할 수 있습니다. 필터의 텍스트 모드에 대한 자세한 내용은 <a href="../../../reports-and-dashboards/reports/text-mode/edit-text-mode-in-filter.md" class="MCXref xref">텍스트 모드를 사용하여 필터 편집</a>.</p> </td> 
  </tr> 
  <tr valign="top"> 
   <td> <p> </p> </td> 
   <td> <p><strong>ciin</strong> </p> </td> 
   <td> <p>(대/소문자 구분 안 함) 대/소문자를 구분하지 않는 버전 <strong>in</strong>.</p> <p>이 수정자는 텍스트 모드 필터에서만 사용할 수 있습니다. 필터의 텍스트 모드에 대한 자세한 내용은 <a href="../../../reports-and-dashboards/reports/text-mode/edit-text-mode-in-filter.md" class="MCXref xref">텍스트 모드를 사용하여 필터 편집</a>.</p> </td> 
  </tr> 
  <tr valign="top"> 
   <td> <p> </p> </td> 
   <td> <p><strong>칠리크</strong> </p> </td> 
   <td> <p>대/소문자를 구분하지 않는 버전의 <strong>좋아요</strong>. 예: "Coilike %Current% %Dead%"는 "Current to Dead" 또는 "Current to Dead" 항목이 포함된 메모를 반환합니다."</p> <p>이 수정자는 텍스트 모드 필터에서만 사용할 수 있습니다. 필터의 텍스트 모드에 대한 자세한 내용은 <a href="../../../reports-and-dashboards/reports/text-mode/edit-text-mode-in-filter.md" class="MCXref xref">텍스트 모드를 사용하여 필터 편집</a>.</p> </td> 
  </tr> 
  <tr valign="top"> 
   <td> <p> </p> </td> 
   <td> <p><strong>시노틴</strong> </p> </td> 
   <td> <p>(대/소문자 구분 안 함) 대/소문자를 구분하지 않는 버전 <strong>알림</strong>.</p> <p>이 수정자는 텍스트 모드 필터에서만 사용할 수 있습니다. 텍스트 모드를 사용하여 필터를 만드는 방법에 대한 자세한 내용은 <a href="../../../reports-and-dashboards/reports/text-mode/edit-text-mode-in-filter.md" class="MCXref xref">텍스트 모드를 사용하여 필터 편집</a>.</p> </td> 
  </tr> 
  <tr valign="top"> 
   <td> </td> 
   <td> <p><strong>다음 포함</strong> </p> </td> 
   <td> <p>(대/소문자 구분) 전체 텍스트 문자열에서 지정된 텍스트를 검색합니다.</p> <p>예를 들어 "Contains Inf"를 사용하면 "Infinity"라는 단어처럼 "Inf"가 포함된 모든 것을 캡처합니다.</p> <p>이 한정자는 텍스트 모드 필터에서만 사용할 수 있습니다.필터의 텍스트 모드에 대한 자세한 내용은 <a href="../../../reports-and-dashboards/reports/text-mode/edit-text-mode-in-filter.md" class="MCXref xref">텍스트 모드를 사용하여 필터 편집</a>.</p> </td> 
  </tr> 
  <tr valign="top"> 
   <td> <p><strong>포함하지 않음</strong> </p> </td> 
   <td> <p><strong>cinotcontains</strong> </p> </td> 
   <td> <p>(대/소문자 구분 안 함) 지정된 값이 없는 항목을 필터링합니다.</p> <p>예를 들어 "inf 포함하지 않음"은 이름에 "Inf" 또는 "inf"가 없는 모든 내용을 캡처합니다.</p> <p>참고: <span>필터링할 필드에 여러 옵션이 있는 경우, 이 옵션은 지정한 선택과 추가 선택 사항을 모두 포함하는 결과를 필터링합니다.</span> </p> </td> 
  </tr> 
  <tr valign="top"> 
   <td><strong>존재하지 않음</strong> </td> 
   <td><strong>존재하지 않음</strong> </td> 
   <td> <p>이 수정자는 EXISTS 문의 복잡한 필터와만 사용합니다. 이러한 필터는 다음 개체만 참조합니다. </p> 
    <ul> 
     <li>객체 계층 구조에서 여러 수준에 걸쳐 있는 객체 </li> 
     <li>누락된 객체 </li> 
    </ul> <p>EXISTS 문을 사용하여 복잡한 필터를 만드는 방법에 대한 자세한 내용은 문서를 참조하십시오 <a href="../../../reports-and-dashboards/reports/text-mode/create-complex-text-mode-filters-using-exists-statements.md">EXISTS 문을 사용하여 복잡한 텍스트 모드 필터 만들기</a>. EXISTS 문에 사용되는 유일한 수정자입니다.</p> </td> 
  </tr> 
  <tr valign="top"> 
   <td> <p> </p> <p> </p> <p> </p> <p><strong>같음</strong> </p> </td> 
   <td> <p><strong>안에 있음</strong> </p> </td> 
   <td> <p>(대/소문자 구분) 이 수정자를 사용하면 쉼표로 구분된 변수 목록을 만들어 필터에서 평가된 단일 속성과 비교할 수 있습니다. 전체 목록은 OR 문으로 처리되고 하나 이상의 변수의 기준을 충족하는 결과를 반환합니다.</p> <p>예를 들어, 프로젝트를 검색할 때 "CUR에서, PLN, CPL"을 사용하면 Current, OR Planning 또는 Complete 상태에 있는 모든 프로젝트를 반환합니다.</p> <p>기본 제공 수정자 <strong>Equal</strong> 의 텍스트 모드 수정자에 해당합니다. <strong>in</strong>. 즉, 필드에 대해 여러 값과 같음 을 선택할 수 있습니다.</p> <p>예를 들어 프로젝트 보고서에서 "상태가 현재, 계획, 데드"를 선택하고 이러한 상태의 프로젝트를 볼 수 있습니다.</p> </td> 
  </tr> 
  <tr valign="top"> 
   <td> </td> 
   <td> <p><strong>eq</strong> </p> </td> 
   <td> <p>(대/소문자 구분) 검색한 값과 정확히 일치하는 항목만 반환합니다.</p> <p>예를 들어 전체 프로젝트를 검색할 때 "eq CPL"은 완료 상태의 모든 프로젝트를 반환합니다. 프로젝트가 완료되어 현재 상태가 될 수 없으므로 "eq CPL, CUR"에서 결과를 반환하지 않습니다.</p> <p>이 수정자는 텍스트 모드 필터에서만 사용할 수 있습니다. 텍스트 모드를 사용하여 필터를 만드는 방법에 대한 자세한 내용은 <a href="../../../reports-and-dashboards/reports/text-mode/edit-text-mode-in-filter.md" class="MCXref xref">텍스트 모드를 사용하여 필터 편집</a>.</p> </td> 
  </tr> 
  <tr valign="top"> 
   <td> <p><strong>다음보다 큼:</strong> </p> </td> 
   <td> <p><strong>gt</strong> </p> </td> 
   <td> <p>입력한 값을 포함하지 않고 입력한 값보다 큰 값을 가진 모든 결과를 검색합니다.</p> </td> 
  </tr> 
  <tr valign="top"> 
   <td> <p> </p> </td> 
   <td> <p><strong>좋아요</strong> </p> </td> 
   <td> <p>(대/소문자 구분) 와 유사한 방식으로 텍스트 문자열의 부분을 검색합니다 <strong>다음 포함</strong>. 하지만, <strong>좋아요</strong> 은 텍스트를 분류할 와일드카드 문자를 삽입할 수 있는 기능을 제공합니다.</p> <p>예를 들어 메모를 검색할 때 "like %Current% %Dead%"를 사용하면 "Current to Dead" 구문을 포함하는 모든 메모가 반환됩니다. 여기에는 "Dead to Current"가 포함된 노트가 포함되지 않습니다. 각 값은 나열된 순서로 검색됩니다. % 는 문자 또는 텍스트 세그먼트를 바꾸기 위한 와일드카드 를 나타냅니다.</p> <p>이 수정자는 텍스트 모드 필터에서만 사용할 수 있습니다. 필터의 텍스트 모드에 대한 자세한 내용은 <a href="../../../reports-and-dashboards/reports/text-mode/edit-text-mode-in-filter.md" class="MCXref xref">텍스트 모드를 사용하여 필터 편집</a>.</p> </td> 
  </tr> 
  <tr valign="top"> 
   <td> <p><strong>다음보다 작음:</strong> </p> </td> 
   <td> <p><strong>lt</strong> </p> </td> 
   <td> <p>입력한 값을 포함하지 않고 입력한 값보다 작은 값을 가진 모든 결과를 검색합니다.</p> </td> 
  </tr> 
  <tr valign="top"> 
   <td> <p><strong>크거나 같음</strong> </p> </td> 
   <td> <p><strong>gte</strong> </p> </td> 
   <td> <p>입력한 값보다 크거나 같은 값이 있는 모든 결과를 검색합니다.</p> </td> 
  </tr> 
  <tr valign="top"> 
   <td> <p><strong>동일값 미만</strong> </p> </td> 
   <td> <p><strong>lte</strong> </p> </td> 
   <td> <p>입력한 값보다 작거나 같은 값이 있는 모든 결과를 검색합니다.</p> </td> 
  </tr> 
  <tr valign="top"> 
   <td> <p><strong>사이</strong> </p> </td> 
   <td> <p><strong>사이</strong> </p> </td> 
   <td> <p>두 개의 필수 필드 값을 제공하고 입력한 값을 포함하여 두 필드 범위 내의 모든 결과를 검색합니다.</p> </td> 
  </tr> 
  <tr valign="top"> 
   <td> <p> </p> </td> 
   <td> <p><strong>다음 포함</strong> </p> </td> 
   <td> <p>(대/소문자 구분) 지정된 값이 없는 항목을 필터링합니다.</p> <p>예를 들어 "nocontains inf"는 "inf"가 없는 모든 항목을 캡처하지만 "Inf"가 포함된 값을 표시합니다.</p> <p>이 수정자는 텍스트 모드 필터에서만 사용할 수 있습니다. 필터의 텍스트 모드에 대한 자세한 내용은 <a href="../../../reports-and-dashboards/reports/text-mode/edit-text-mode-in-filter.md" class="MCXref xref">텍스트 모드를 사용하여 필터 편집</a>.</p> </td> 
  </tr> 
  <tr valign="top"> 
   <td> <p> </p> </td> 
   <td> <p><strong>다음 사이</strong> </p> </td> 
   <td> <p>의 역수입니다 <strong>사이</strong>. 두 개의 필수 값 필드를 제공하고 입력한 값을 포함하여 두 필드 범위를 벗어나는 모든 결과를 검색합니다.</p> <p>이 수정자는 텍스트 모드 필터에서만 사용할 수 있습니다. 필터의 텍스트 모드에 대한 자세한 내용은 <a href="../../../reports-and-dashboards/reports/text-mode/edit-text-mode-in-filter.md" class="MCXref xref">텍스트 모드를 사용하여 필터 편집</a>.</p> </td> 
  </tr> 
  <tr valign="top"> 
   <td> <p><strong>같지 않음</strong> </p> </td> 
   <td> <p><strong>알림</strong> </p> </td> 
   <td> <p>(대/소문자 구분) 반대입니다 <strong>in</strong>. 지정된 목록에 없는 결과만 반환합니다.</p> <p>이 수정자는 텍스트 모드 필터에서만 사용할 수 있습니다. 필터의 텍스트 모드에 대한 자세한 내용은 <a href="../../../reports-and-dashboards/reports/text-mode/edit-text-mode-in-filter.md" class="MCXref xref">텍스트 모드를 사용하여 필터 편집</a>.</p> <p>참고: <span>필터링할 필드에 여러 옵션이 있는 경우, 이 옵션은 지정한 선택과 추가 선택 사항을 모두 포함하는 결과를 필터링합니다.</span> </p> </td> 
  </tr> 
  <tr valign="top"> 
   <td> </td> 
   <td><strong>ne</strong> </td> 
   <td> <p>(대/소문자 구분) 반대입니다 <strong>eq</strong>. 검색된 값과 정확히 일치하지 않는 결과만 반환하고 값의 대문자도 일치합니다.</p> <p>예, <b>ne</b> "Current"와 같지 않은 값을 반환하지만 "current"와 같지 않은 값은 반환되지 않습니다. </p> <p>이 수정자는 텍스트 모드 필터에서만 사용할 수 있습니다. 필터의 텍스트 모드에 대한 자세한 내용은 <a href="../../../reports-and-dashboards/reports/text-mode/edit-text-mode-in-filter.md" class="MCXref xref">텍스트 모드를 사용하여 필터 편집</a>.<br></p> </td> 
  </tr> 
  <tr valign="top"> 
   <td> </td> 
   <td><strong>cine</strong> </td> 
   <td> <p>(대/소문자 구분 안 함) 다음 중 대/소문자를 구분하지 않는 옵션입니다. <strong>ne</strong> 그리고 그것은 그 반대입니다 <b>cieq</b> 수정자. 값의 대소문자를 고려하지 않고 검색된 값의 정확한 일치가 아닌 결과만 반환합니다.</p> <p>예, <b>cine</b> "current" 또는 "Current"와 같지 않은 값을 반환합니다. </p> <p>이 수정자는 텍스트 모드 필터에서만 사용할 수 있습니다. 필터의 텍스트 모드에 대한 자세한 내용은 <a href="../../../reports-and-dashboards/reports/text-mode/edit-text-mode-in-filter.md" class="MCXref xref">텍스트 모드를 사용하여 필터 편집</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>
