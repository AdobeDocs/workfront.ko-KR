---
content-type: overview
product-area: reporting
navigation-topic: calculate-custom-data-reports
title: 계산된 사용자 정의 필드와 계산된 열 비교
description: Adobe Workfront의 여러 필드를 집계하여 해당 집계 값을 새 필드에 표시하려면 사용자 정의 양식에서 계산된 사용자 정의 필드를 만들거나 보기에서 계산된 열을 만들 수 있습니다.
author: Jenny
feature: Reports and Dashboards
exl-id: 17ac554d-0c90-4592-946e-a89f1784571d
source-git-commit: ce986a912c2ee231b9dc2e1c7a3e9587b20aa0ba
workflow-type: tm+mt
source-wordcount: '844'
ht-degree: 0%

---

# 계산된 사용자 정의 필드와 계산된 열 비교

Adobe Workfront의 여러 필드를 집계하고 해당 집계 값을 새 필드에 표시하려면 다음을 만들 수 있습니다.

* 사용자 정의 양식의 계산된 사용자 정의 필드\
  사용자 지정 양식에 계산된 사용자 지정 필드를 추가하는 방법에 대한 자세한 내용은 [양식에 계산된 필드 추가](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/form-designer/design-a-form/add-a-calculated-field.md)를 참조하십시오.

* 보기의 계산된 열\
  보기에서 계산을 사용하는 방법에 대한 자세한 내용은 문서 [텍스트 모드의 일반적인 사용 개요](../../../reports-and-dashboards/reports/text-mode/understand-common-uses-text-mode.md#use-text-mode-in-views)의 [보기에서 텍스트 모드 사용](../../../reports-and-dashboards/reports/text-mode/understand-common-uses-text-mode.md) 섹션을 참조하십시오.

텍스트 모드를 사용하여 계산된 필드와 계산된 열을 모두 작성하지만 작성하기 위한 구문은 다릅니다. 계산된 필드 및 계산된 열을 작성하는 방법에 대해 알아보려면 위에 나열된 문서를 참조하십시오. 계산된 사용자 지정 필드 및 열과 같은 계산된 데이터 식에 사용되는 다른 구문에 대한 자세한 내용은 이 문서의 [계산된 사용자 지정 필드와 계산된 사용자 지정 열의 구문](/help/quicksilver/reports-and-dashboards/reports/calc-cstm-data-reports/calculated-custom-fields-calculated-columns.md#syntax-of-calculated-custom-fields-vs-calculated-custom-columns) 섹션을 참조하십시오.

계산된 열과 계산된 필드 모두에서 동일한 계산을 사용할 수 있습니다. 그러나 이러한 계산을 위해 목적이 무엇인지에 따라 하나를 구축하는 것을 다른 하나와 비교하는 것을 고려할 수 있습니다.

## 계산된 사용자 정의 필드와 계산된 사용자 정의 열의 구문

사용하는 함수는 동일하지만 계산된 사용자 정의 필드에 표현식을 작성하는 구문은 계산된 사용자 정의 열을 작성하는 구문과 다를 수 있습니다.

For example:

* 사용자 정의 필드의 작업에 대한 사용자 정의 양식에서 다음을 사용하여 사용자 정의 양식이 첨부된 작업의 상위 프로젝트 이름을 생성합니다.

  `{project}.{name}`

* 보고서의 사용자 정의 열에서 다음을 사용하여 작업 보고서에 프로젝트 이름 사용자 정의 열을 추가합니다.

  `valuefield=project:name`

  또는

  `valueexpression={project}.{name}`

  >[!TIP]
  >
  >계산된 표현식이 사용되는 모든 텍스트 모드 보고 요소(보기, 필터, 그룹화 및 프롬프트)에는 동일한 구문이 적용됩니다.

두 구문 간의 차이점은 다음과 같습니다.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td><strong>계산된 사용자 정의 필드</strong></td>
   <td><strong>계산된 사용자 지정 보고 요소</strong></td> 
  </tr> 
  <tr> 
   <td> <p>Workfront 인터페이스에 표시되는 필드의 이름을 사용합니다.</p> <p class="example" data-mc-autonum="<b>Example: </b>"><span class="autonumber"><span><b>예: </b></span></span>계산된 사용자 지정 필드에 사용되는 필드 이름의 예: <code>Planned Completion Date</code>.</p> </td> 
   <td> <p>Workfront 데이터베이스에 나타나는 개체 또는 필드의 이름을 사용합니다. 오브젝트 및 필드의 이름이 컴파운드 이름인 경우 소문자 또는 카멜 문자로 입력됩니다. </p> <p>데이터베이스에 나타나는 모든 Workfront 개체 및 필드의 인벤토리는 <a href="../../../wf-api/general/api-explorer.md" class="MCXref xref">API 탐색기</a>를 참조하십시오. </p> <p class="example" data-mc-autonum="<b>Example: </b>"><span class="autonumber"><span><b>예: </b></span></span>계산된 사용자 지정 보고 요소에 사용되는 필드 이름의 예: <code>plannedCompletionDate</code>.</p> </td> 
  </tr> 
  <tr> 
   <td>필드 이름을 괄호 또는 중괄호로 묶습니다.</td> 
   <td> <p>필드 이름을 <code>valuefield </code> 줄에서 사용할 때는 대괄호 또는 괄호로 묶지 마십시오.</p> <p>필드 이름을 <code>valueexpression</code> 줄에서 사용할 때는 중괄호로 묶습니다.</p> </td> 
  </tr> 
  <tr> 
   <td>필드를 마침표로 구분합니다.</td> 
   <td> <p>필드를 <code>valuefield</code> 줄에서 사용할 때 콜론으로 구분합니다.</p> <p>필드를 <code>valueexpression</code>줄에 사용할 때는 필드를 마침표로 구분하십시오.</p> </td> 
  </tr> 
 </tbody> 
</table>

계산된 사용자 지정 열에서 사용해야 하는 구문에 대한 자세한 내용은 [텍스트 모드 개요](../../../reports-and-dashboards/reports/text-mode/understand-text-mode.md)를 참조하십시오.

## 계산된 사용자 정의 필드를 사용해야 하는 경우

* 보고서에서 집계된 결과를 그룹화하거나 이 정보를 차트에 표시하려는 경우
* 필드에서 계산되는 집계 이상의 데이터를 집계하려는 경우
* 데이터가 업데이트되지 않고 시간이 지남에 따라 변경될 수 있으므로 데이터의 적시성에 대해 걱정하지 않는 경우

## 계산된 사용자 정의 필드의 업데이트를 트리거하는 작업

* 개체의 기본 페이지에서 기타 아이콘 ![기타 아이콘](assets/more-icon.png)을 클릭한 다음 **표현식 다시 계산**&#x200B;을 클릭합니다.

* **사용자 지정 식 다시 계산**&#x200B;을 사용하도록 설정한 경우 여러 개체를 일괄 편집하고 있습니다.
* 개체 목록의 기타 메뉴에서 **식 다시 계산**&#x200B;을 클릭할 때 여러 개체를 일괄 편집하는 중입니다.
* 계산된 사용자 정의 필드에 대해 **이전 계산 업데이트**&#x200B;를 사용할 수 있는 경우 사용자 정의 양식을 편집합니다.

자세한 내용은 [사용자 정의 양식 필드에서 정보 편집](/help/quicksilver/workfront-basics/work-with-custom-forms/edit-custom-forms.md)을 참조하십시오.

## 보기에서 계산된 열을 사용해야 하는 경우

* 보고서에서 실시간 데이터를 사용할 수 있게 하려는 경우.

  보고서가 실행되거나 보기가 적용될 때 계산이 이루어지기 때문에 계산된 보기는 항상 새로 고쳐집니다.

* 집계된 결과로 그룹화하거나 차트에서 이 정보를 사용할 계획이 없는 경우
* 열에서 계산되는 집계 이상의 데이터를 집계할 계획이 없는 경우(데이터는 한 번만 집계될 수 있음)
* $$TODAY 또는 $$NOW 와일드카드를 사용하여 현재 날짜에 대한 참조를 계산에 포함하려는 경우.

  >[!TIP]
  >
  >이 참조는 첨부된 개체를 편집할 때만 다시 계산되므로 계산된 사용자 지정 필드에서는 이 참조를 사용하지 마십시오. 이런 종류의 계산은 구식이 된다.

## 계산된 사용자 정의 필드 및 열의 예

계산된 사용자 지정 필드의 예는 [보고서의 계산된 사용자 지정 데이터](../../../reports-and-dashboards/reports/calc-cstm-data-reports/calculated-custom-data-reports.md)를 참조하십시오.

보기에서 계산된 사용자 정의 열의 예는 다음 문서를 참조하십시오.

* [텍스트 모드의 일반적인 사용 개요](../../../reports-and-dashboards/reports/text-mode/understand-common-uses-text-mode.md)
* [사용자 정의 보기, 필터링 및 그룹화 샘플: 문서 인덱스](../../../reports-and-dashboards/reports/custom-view-filter-grouping-samples/custom-view-filter-grouping-samples.md)
