---
content-type: overview
product-area: reporting
navigation-topic: calculate-custom-data-reports
title: 계산된 사용자 지정 필드와 계산된 열
description: Adobe Workfront에서 여러 필드를 집계하고 해당 합계 값을 새 필드에 표시하려면 다음 - EDIT ME를 수행할 수 있습니다.
author: Nolan
feature: Reports and Dashboards
exl-id: 17ac554d-0c90-4592-946e-a89f1784571d
source-git-commit: 54f4c136cfaaaaaa90a4fc64d3ffd06816cff9cb
workflow-type: tm+mt
source-wordcount: '815'
ht-degree: 0%

---

# 계산된 사용자 지정 필드와 계산된 열

Adobe Workfront에서 여러 필드를 집계하고 해당 합계 값을 새 필드에 표시하려면 다음을 수행할 수 있습니다.

* 사용자 지정 양식의 계산된 사용자 지정 필드\
   사용자 지정 양식에 계산된 사용자 지정 필드를 추가하는 방법에 대한 자세한 내용은 섹션을 참조하십시오 [사용자 지정 양식에 계산된 필드 추가](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/add-calculated-data-to-custom-form.md#creating-calculated-custom-fields) 기사 [사용자 지정 양식에 계산된 데이터 추가](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/add-calculated-data-to-custom-form.md).

* 보기의 계산된 열\
   보기에서 계산을 사용하는 방법에 대한 자세한 내용은 섹션을 참조하십시오 [보기에서 텍스트 모드 사용](../../../reports-and-dashboards/reports/text-mode/understand-common-uses-text-mode.md#using-text-mode-in-views) 기사 [텍스트 모드에 대한 일반적인 사용 개요](../../../reports-and-dashboards/reports/text-mode/understand-common-uses-text-mode.md).

텍스트 모드를 사용하여 계산된 필드와 계산된 열을 모두 작성하지만, 이를 작성하는 구문은 다릅니다. 계산된 필드 및 계산된 열을 작성하는 방법에 대해 알아보려면 위에 나열된 문서를 참조하십시오. 계산된 사용자 지정 필드 및 열과 같은 계산된 데이터 표현식에서 사용되는 다양한 구문에 대한 자세한 내용은 섹션을 참조하십시오 [계산된 사용자 지정 필드의 구문과 계산된 사용자 지정 열 구문](#syntax-of-calculated-custom-fields-vs-calculated-custom-columns-syntax) 참조하십시오.

계산된 열과 계산된 필드 모두에서 동일한 계산을 사용할 수 있습니다. 그러나 이러한 계산의 목적에 따라 한 계산 이외에 다른 계산 하나를 작성하는 것을 고려할 수 있습니다.

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
   <td>계산된 사용자 지정 필드</td> 
   <td>계산된 사용자 지정 보고 요소</td> 
  </tr> 
  <tr> 
   <td> <p>Workfront 인터페이스에 표시되는 필드의 이름을 사용합니다.</p> <p class="example" data-mc-autonum="<b>Example: </b>"><span class="autonumber"><span><b>예: </b></span></span>계산된 사용자 지정 필드에 사용되는 필드 이름의 예: <code>Planned Completion Date</code>.</p> </td> 
   <td> <p>Workfront 데이터베이스에 표시되는 개체 또는 필드의 이름을 사용합니다. 개체 및 필드의 이름이 조합 이름인 경우 그 이름은 소문자나 카멜 대소문자를 쓴다. </p> <p>데이터베이스에 표시되는 모든 Workfront 개체 및 필드의 인벤토리에 대해서는 <a href="../../../wf-api/general/api-explorer.md" class="MCXref xref">API 탐색기</a>. </p> <p class="example" data-mc-autonum="<b>Example: </b>"><span class="autonumber"><span><b>예: </b></span></span>계산된 사용자 지정 보고 요소에 사용되는 필드 이름의 예: <code>plannedCompletionDate</code>.</p> </td> 
  </tr> 
  <tr> 
   <td>필드 이름을 괄호 또는 중괄호로 묶습니다</td> 
   <td> <p>괄호로 필드 이름을 묶지 마십시오 <code>valuefield </code>줄.</p> <p>필드 이름을 중괄호로 묶습니다 <code>valueexpression</code> 줄.</p> </td> 
  </tr> 
  <tr> 
   <td>마침표로 필드를 구분합니다</td> 
   <td> <p>에서 필드를 사용할 때 콜론으로 필드를 구분합니다 <code>valuefield </code>라인</p> <p>에서 필드를 사용할 때 마침표로 필드를 구분합니다 <code>valueexpression </code>줄. </p> </td> 
  </tr> 
 </tbody> 
</table>

계산된 사용자 지정 열에서 사용해야 하는 구문에 대한 자세한 내용은 [텍스트 모드 개요](../../../reports-and-dashboards/reports/text-mode/understand-text-mode.md).

## 계산된 사용자 지정 필드를 사용해야 하는 경우

* 집계된 결과를 보고서에 그룹화하거나 이 정보를 차트에 표시하려면
* 필드에서 계산된 집계 이상의 데이터를 집계하려는 경우
* 데이터가 업데이트되지 않고 시간이 지남에 따라 변경될 수 있으므로 데이터의 적시성이 걱정되지 않는 경우

## 계산된 사용자 지정 필드의 업데이트를 트리거하는 작업

* 개체의 기본 페이지에서 자세히 아이콘을 클릭합니다. ![](assets/more-icon.png)를 클릭한 다음 **표현식 다시 계산**

* 여러 개체 벌크 편집 **사용자 지정 표현식 다시 계산** 이 활성화되어 있습니다.
* 다음 경우에 사용자 지정 양식 편집 **이전 계산 업데이트** 이 계산된 사용자 지정 필드에 대해 활성화되어 있습니다

## 보기에서 계산된 열을 사용해야 하는 경우

* 보고서에서 실시간 데이터를 사용할 수 있도록 하려면.

   계산된 보기는 보고서가 실행되거나 보기가 적용될 때 계산되므로 항상 새로 고침됩니다.

* 집계된 결과별로 그룹화할 계획이 없거나 차트에 이 정보를 사용할 계획이 없는 경우
* 열에서 계산된 합계 이외의 데이터를 집계하지 않을 경우(데이터는 한 번만 집계할 수 있음).
* $$TODAY 또는 $$NOW 와일드카드를 사용하여 현재 날짜에 대한 참조를 계산하려는 경우.

   >[!TIP]
   >
   >첨부된 개체를 편집할 때만 다시 계산되므로 계산된 사용자 지정 필드에서 이 참조를 사용하지 마십시오. 이런 계산은 시대에 뒤떨어진 것이다.

## 계산된 사용자 지정 필드 및 열의 예

계산된 사용자 지정 필드의 예는 를 참조하십시오. [보고서에서 계산된 사용자 지정 데이터](../../../reports-and-dashboards/reports/calc-cstm-data-reports/calculated-custom-data-reports.md).

보기의 계산된 사용자 지정 열에 대한 예는 다음 문서를 참조하십시오.

* [텍스트 모드에 대한 일반적인 사용 개요](../../../reports-and-dashboards/reports/text-mode/understand-common-uses-text-mode.md)
* [사용자 정의 보기, 필터 및 그룹화 샘플](../../../reports-and-dashboards/reports/custom-view-filter-grouping-samples/custom-view-filter-grouping-samples.md)
