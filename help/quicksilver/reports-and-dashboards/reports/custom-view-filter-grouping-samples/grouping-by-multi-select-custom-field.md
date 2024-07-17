---
content-type: reference
product-area: reporting
navigation-topic: custom-view-filter-and-grouping-samples
title: 다중 선택 사용자 정의 필드로 보고서 그룹화
description: 텍스트 모드를 사용해야만 Adobe Workfront 보고서의 다중 선택 사용자 지정 필드에 있는 값별로 그룹화할 수 있습니다.
author: Lisa and Nolan
feature: Reports and Dashboards
exl-id: 530dff59-0d4c-490e-b464-1d3bb1d0f36f
source-git-commit: b0447fd2ea9419fabcc21a1131910485c18b75d0
workflow-type: tm+mt
source-wordcount: '543'
ht-degree: 0%

---

# 다중 선택 사용자 정의 필드로 보고서 그룹화

텍스트 모드를 사용해야만 Adobe Workfront 보고서의 다중 선택 사용자 지정 필드에 있는 값별로 그룹화할 수 있습니다.

다중 선택 사용자 정의 필드의 예는 다음과 같습니다.

* 확인란
* 드롭다운 메뉴 다중 선택

텍스트 모드 사용에 대한 자세한 내용은 문서 [텍스트 모드 개요](../../../reports-and-dashboards/reports/text-mode/understand-text-mode.md)를 참조하십시오.

## 다중 선택 사용자 정의 필드로 그룹화할 때의 고려 사항

* 텍스트 모드 그룹화를 사용하는 보고서는 차트로 작성할 수 없습니다. 다중 선택 사용자 정의 필드를 참조하는 추가 계산된 필드를 만들어 다중 선택 사용자 정의 필드의 값으로 보고서를 차트로 작성해야 합니다.

  자세한 내용은 [다중 선택 사용자 지정 필드로 보고서 차트 만들기](../../../reports-and-dashboards/reports/custom-view-filter-grouping-samples/chart-report-by-multi-select-custom-field.md)를 참조하세요.
* 선택한 항목이 있는 항목은 한 번만 카운트됩니다.

  예를 들어, 선택 항목 1과 선택 항목 2를 옵션으로 사용하는 확인란 사용자 정의 필드가 있고, 양식을 작업에 첨부하는 경우, 선택 항목 1과 선택 항목 2가 모두 선택된 작업은 선택 항목 1 또는 선택 항목 2만 선택된 작업과 별도로 그룹화됩니다.


## 액세스 요구 사항

이 문서의 단계를 수행하려면 다음 액세스 권한이 있어야 합니다.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront 플랜*</td> 
   <td> <p>임의</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront 라이센스*</td> 
   <td> <p>그룹화 수정 요청 </p>
   <p>보고서 수정 계획</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">액세스 수준 구성*</td> 
   <td> <p>보고서, 대시보드, 캘린더에 대한 액세스 권한을 편집하여 보고서 수정</p> <p>필터, 보기, 그룹화에 대한 액세스 권한을 편집하여 그룹화 수정</p> <p><b>메모</b>

여전히 액세스 권한이 없는 경우 Workfront 관리자에게 액세스 수준에 추가 제한을 설정하는지 문의하십시오. Workfront 관리자가 액세스 수준을 수정하는 방법에 대한 자세한 내용은 <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">사용자 지정 액세스 수준 만들기 또는 수정</a>을 참조하십시오.</p> </td>
</tr>  
  <tr> 
   <td role="rowheader">개체 권한</td> 
   <td> <p>보고서에 대한 권한 관리</p> <p>추가 액세스 요청에 대한 자세한 내용은 <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">개체 </a>에 대한 액세스 요청 을 참조하십시오.</p> </td> 
  </tr> 
 </tbody> 
</table>

*보유 중인 플랜, 라이선스 유형 또는 액세스 권한을 확인하려면 Workfront 관리자에게 문의하십시오.

## 다중 선택 사용자 정의 필드로 보고서 그룹화

다중 선택 사용자 지정 필드로 그룹화하려면 다음 사전 요구 사항이 있어야 합니다.

* 다중 선택 사용자 정의 필드를 사용자 정의 양식에서 작성합니다.\
  사용자 정의 양식을 작성하고 사용자 정의 필드를 추가하는 방법에 대한 자세한 내용은 문서 [사용자 정의 양식 만들기 또는 편집](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/create-or-edit-a-custom-form.md)을 참조하십시오.

* 사용자 정의 양식을 오브젝트에 첨부합니다.
* 다중 선택 사용자 정의 필드를 각 오브젝트의 값으로 채웁니다. 

보고서에서 다중 선택 사용자 정의 필드로 그룹화하려면 다음을 수행합니다.

1. 다중 선택 사용자 정의 필드에 대한 그룹화를 추가할 보고서를 만들거나 기존 보고서를 편집합니다.\
   보고서 만들기에 대한 자세한 내용은 문서 [사용자 지정 보고서 만들기](../../../reports-and-dashboards/reports/creating-and-managing-reports/create-custom-report.md)를 참조하세요.

1. **그룹화** 탭을 선택합니다.
1. **텍스트 모드로 전환**&#x200B;을 클릭합니다.

1. **보고서 그룹화** 상자에서 텍스트를 선택하고 다음 코드로 바꿉니다.

   <pre>
   group.0.displayname=다중 선택 사용자 지정 필드 이름
   group.0.valueexpression={DE:Multi-select Custom Field Name}
   group.0.valueformat=HTML
   group.0.textmode=true
   </pre>

1. 다중 선택 사용자 정의 필드 이름 은 Workfront에 표시되는 대로 다중 선택 사용자 정의 필드의 실제 이름으로 바꿉니다.
1. **저장 후 닫기**&#x200B;를 클릭합니다.

   보고서의 개체는 다중 선택 사용자 지정 필드의 값으로 그룹화됩니다.

   ![](assets/grouping-by-multi-select-field-text-mode-ui-example.png)

   보고서의 그룹화 이름은 다중 선택 사용자 정의 필드 이름 뒤에 필드에서 선택한 값이 옵니다.

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
