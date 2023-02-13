---
content-type: reference
product-area: reporting
navigation-topic: custom-view-filter-and-grouping-samples
title: 다중 선택 사용자 지정 필드로 보고서 그룹화
description: Adobe Workfront 보고서의 다중 선택 사용자 지정 필드에 있는 값별로 그룹화할 수 있습니다. 다중 선택 사용자 지정 필드의 예는 EDIT ME입니다.
author: Lisa and Nolan
feature: Reports and Dashboards
exl-id: 530dff59-0d4c-490e-b464-1d3bb1d0f36f
source-git-commit: 54f4c136cfaaaaaa90a4fc64d3ffd06816cff9cb
workflow-type: tm+mt
source-wordcount: '468'
ht-degree: 0%

---

# 다중 선택 사용자 지정 필드로 보고서 그룹화

Adobe Workfront 보고서의 다중 선택 사용자 지정 필드에 있는 값별로 그룹화할 수 있습니다. 다중 선택 사용자 지정 필드의 예는 다음과 같습니다.

* 확인란
* 다중 선택 드롭다운 메뉴

텍스트 모드를 사용해야만 이 유형의 필드별로 그룹화할 수 있습니다. 텍스트 모드 사용에 대한 자세한 내용은 문서를 참조하십시오 [텍스트 모드 개요](../../../reports-and-dashboards/reports/text-mode/understand-text-mode.md).

>[!NOTE]
>
>다중 선택 사용자 지정 필드로 보고서를 차트할 수 없습니다. 다중 선택 사용자 지정 필드를 참조하는 추가 계산된 필드를 만들어 다중 선택 사용자 지정 필드의 값으로 보고서를 차트화해야 합니다. 자세한 내용은 [다중 선택 사용자 지정 필드로 보고서 차트 지정](../../../reports-and-dashboards/reports/custom-view-filter-grouping-samples/chart-report-by-multi-select-custom-field.md).

## 액세스 요구 사항

이 문서의 절차를 수행하려면 다음 액세스 권한이 있어야 합니다.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront 플랜*</td> 
   <td> <p>모든</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront 라이선스*</td> 
   <td> <p>플랜 </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">액세스 수준 구성*</td> 
   <td> <p>보고서, 대시보드, 달력에 대한 액세스 편집</p> <p>필터, 보기, 그룹화에 대한 액세스 편집</p> <p>참고: 여전히 액세스 권한이 없는 경우 Workfront 관리자에게 액세스 수준에서 추가 제한 사항을 설정하는지 문의하십시오. Workfront 관리자가 액세스 수준을 수정하는 방법에 대한 자세한 내용은 <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">사용자 정의 액세스 수준 만들기 또는 수정</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">개체 권한</td> 
   <td> <p>보고서에 대한 권한 관리</p> <p>추가 액세스 요청에 대한 자세한 내용은 <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">개체에 대한 액세스 요청 </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;어떤 계획, 라이선스 유형 또는 액세스 권한을 보유하고 있는지 알아보려면 Workfront 관리자에게 문의하십시오.

## 사용자 지정 필드를 여러 개 선택하여 보고서를 그룹화합니다

다중 선택 사용자 지정 필드로 그룹화하려면 다음 전제 조건이 있어야 합니다.

* 사용자 지정 양식에서 다중 선택 사용자 지정 필드를 작성합니다.\
   사용자 지정 양식 작성 및 사용자 지정 필드 추가에 대한 자세한 내용은 문서를 참조하십시오 [사용자 지정 양식 만들기 또는 편집](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/create-or-edit-a-custom-form.md).

* 개체에 사용자 지정 양식을 첨부합니다.
* 다중 선택 사용자 지정 필드를 각 개체의 값으로 채웁니다. 

보고서에서 다중 선택 사용자 지정 필드를 기준으로 그룹화하려면,

1. 다중 선택 사용자 지정 필드에 대한 그룹을 추가할 보고서를 만들거나 기존 보고서를 편집합니다.\
   보고서 만들기에 대한 내용은 문서를 참조하십시오 [사용자 지정 보고서 만들기](../../../reports-and-dashboards/reports/creating-and-managing-reports/create-custom-report.md).

1. 을(를) 선택합니다 **그룹화** 탭.
1. 클릭 **텍스트 모드로 전환**.

1. 에서 텍스트를 선택합니다 **보고서 그룹화** 상자를 열고 다음 코드로 바꿉니다.

   <pre>group.0.displayname=Multi-select Custom Field Name<br>group.0.valueexpression={DE:Multi-select Custom Field Name}<br>group.0.valueformat=HTML<br>textmode=true</pre>

1. Workfront에 표시되는 다중 선택 사용자 지정 필드의 실제 이름으로 &quot;Multi-select Custom Field Name&quot;을 대체합니다.  
1. 클릭 **저장 후 닫기**.\
   보고서의 객체는 다중 선택 사용자 지정 필드의 값으로 그룹화됩니다.\
   보고서 그룹의 이름은 다중 선택 사용자 지정 필드의 이름 뒤에 필드에서 선택한 값이 옵니다. 

<!--
<div data-mc-conditions="QuicksilverOrClassic.Draft mode">
<h2>Chart a report by multi-select Custom Fields</h2>
<p>(NOTE: this moved to its own article, linked in the Note above!)</p>
<p>You cannot build a chart in a report by referencing a multi-select custom field. Instead, you can create a calculated field that records the values of the multi-select custom field on a given object and group by the calculated field.&nbsp;</p>
<ul>
<li><a href="#build-a-calculated-custom-field-that-references-a-multi-select-custom-field" class="MCXref xref">Build a calculated custom field that references a multi-select custom field</a> </li>
<li><a href="#build-a-chart-that-references-a-calculated-custom-field" class="MCXref xref">Build a chart that references a calculated custom field</a> </li>
</ul>
<p><strong>Build a calculated custom field that references a multi-select custom field</strong></p>
<p>To be able to build a calculated field that references a multi-select custom field, you must have the following prerequisites:</p>
<ul>
<li>Build the multi-select custom field in a custom form.<br>For information about building custom forms and adding custom fields to them, see the article <a href="../../../administration-and-setup/customize-workfront/create-manage-custom-forms/create-or-edit-a-custom-form.md" class="MCXref xref">Create or edit a custom form</a>.</li>
<li>Attach the custom form to objects.</li>
<li>Populate the multi-select custom field with a value on each object.</li>
</ul>
<p>To build the calculated custom field that references the multi-select custom field:</p>
<ol>
<li value="1">Create a custom form, or edit an existing one.<br>For information about creating custom forms, see the article <a href="../../../administration-and-setup/customize-workfront/create-manage-custom-forms/create-or-edit-a-custom-form.md" class="MCXref xref">Create or edit a custom form</a>.</li>
<li value="2">Click<strong>Add a Field</strong>, then <strong>Calculated</strong> to add the multi-select custom field to the form.</li>
<li value="3">In the <strong>Label</strong> box, name the new calculated field to indicate that it references the multi-select custom field.<br>For example: "Calculated Multi-select Field."</li>
<li value="4"> <p>In the <strong>Calculation</strong> box, enter the following code:</p><pre>{DE:Multi-select Custom Field}</pre> <p> <img src="assets/calculated-multi-select-custom-field-350x201.png" style="width: 350;height: 201;"> <br> </p> </li>
<li value="5">Replace "Multi-select Custom Field" with the actual name of your multi-select custom field, as it appears in Workfront.</li>
<li value="6"> <p>(Optional) If the multi-select custom field is already on this form and if this form is already attached to objects, enable the <strong>Update previous calculations</strong>&nbsp;option.</p> <p>This ensures that the new field is automatically populated with the value from the multi-select custom field as it is added to the forms attached to the objects already.</p> </li>
<li value="7">Click <strong>Done</strong>.</li>
<li value="8">Click <strong>Save +Close</strong>.</li>
</ol>
<p><strong>Build a chart that references a calculated custom field</strong></p>
<ol>
<li value="1"> Go to the report where you want to add the chart for the calculated field that references the multi-select custom field. </li>
<li value="2"> (Optional) To ensure that all the calculated fields that you want to chart by are populated with values, select all the objects in your report, then click <strong>Edit</strong>. </li>
<li value="3"> <p> (Optional and conditional) Enable the <strong>Recalculate Custom Expressions</strong> field, then click <strong>Save Changes</strong>.</p> <p> <img src="assets/recalculate-custom-expressions-350x259.png" style="width: 350;height: 259;"> <br> </p> </li>
<li value="4"> Click <strong>Report Actions</strong>, then <strong>Edit</strong>. </li>
<li value="5">Select the <strong>Groupings</strong> tab, then click <strong>Add Grouping</strong>. </li>
<li value="6">Add the<strong>Calculated Multi-select Field</strong> you created as your grouping. </li>
<li value="7"> <p>Select the <strong>Chart</strong> tab, and add a chart to your report.</p> <p>For information about adding a chart to a report, see the section <a href="../../../reports-and-dashboards/reports/creating-and-managing-reports/create-custom-report.md#add-a-chart" class="MCXref xref">Add a chart to a report</a> in the article <a href="../../../reports-and-dashboards/reports/creating-and-managing-reports/create-custom-report.md" class="MCXref xref">Create a custom report</a>. </p> </li>
<li value="8">Select the <strong>Calculated Multi-select Field</strong> as one of the fields to display in the chart. </li>
<li value="9"> <p>Click <strong>Save + Close</strong>.</p> <p>The report displays the results grouped by the Calculated Multi-select Field in a chart. </p> </li>
</ol>
</div>
-->
