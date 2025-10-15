---
product-area: reporting
navigation-topic: text-mode-reporting
title: 텍스트 모드를 사용하여 보기 편집
description: 텍스트 모드를 사용하여 목록이나 보고서의 보기를 편집하여 표준 인터페이스에서 사용할 수 없는 필드에 액세스하고 보다 복잡한 보기를 만들 수 있습니다.
author: Nolan
feature: Reports and Dashboards
exl-id: b99a2d14-a226-4075-9b1b-ac9426fd41b8
source-git-commit: aa8275f252dd51f5a14d7aa931423aa4afb4ba8f
workflow-type: tm+mt
source-wordcount: '461'
ht-degree: 3%

---

# 텍스트 모드를 사용하여 보기 편집

<!-- Audited: 1/2025 -->

텍스트 모드를 사용하여 목록이나 보고서의 보기를 편집하여 표준 인터페이스에서 사용할 수 없는 필드에 액세스하고 보다 복잡한 보기를 만들 수 있습니다.

## 액세스 요구 사항

+++ 을 확장하여 이 문서의 기능에 대한 액세스 요구 사항을 봅니다.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront 패키지</td> 
   <td> <p>임의</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront 라이선스</td> 
   <td> 
     <p>표준</p>
     <p>플랜</p>
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader">액세스 수준 구성</td> 
   <td> <p>필터, 보기, 그룹화에 대한 액세스 편집</p> <p>보고서, 대시보드, 캘린더에 대한 액세스 권한을 편집하여 보고서의 보고 요소를 편집합니다.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">개체 권한</td> 
   <td> <p>보고서의 보기를 편집할 수 있도록 보고서에 대한 권한 관리</p> <p>보기에 대한 편집 권한 관리</p> </td> 
  </tr>
 </tbody> 
</table>

이 표의 정보에 대한 자세한 내용은 [Workfront 설명서의 액세스 요구 사항](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)을 참조하십시오.

+++

## 전제 조건

보고서나 목록에서 텍스트 모드 사용을 시작하기 전에 항상 Workfront 텍스트 모드 구문을 잘 알고 있는지 확인하십시오.

자세한 내용은 다음 문서를 참조하십시오.

* [텍스트 모드 개요](../../../reports-and-dashboards/reports/text-mode/understand-text-mode.md)
* [텍스트 모드 구문 개요](../../../reports-and-dashboards/reports/text-mode/text-mode-syntax-overview.md)
* [사용자 정의 보기, 필터링 및 그룹화 샘플: 문서 인덱스](../../../reports-and-dashboards/reports/custom-view-filter-grouping-samples/custom-view-filter-grouping-samples.md)

## 보기에서 텍스트 모드 편집

텍스트 모드를 사용하여 뷰를 편집하는 것은 보고서와 목록에 대해 동일합니다. 보고서 또는 목록에서 보기에 액세스하는 방법은 다릅니다.

>[!TIP]
>
>표준 모드에서 가능한 한 많은 보기를 작성한 다음 텍스트 모드로 변환하여 편집하는 것이 좋습니다.

뷰 빌드에 대한 자세한 내용은 [Adobe Workfront의 뷰 개요](../../../reports-and-dashboards/reports/reporting-elements/views-overview.md)를 참조하십시오.

보고서 만들기에 대한 자세한 내용은 [사용자 지정 보고서 만들기](../../../reports-and-dashboards/reports/creating-and-managing-reports/create-custom-report.md)를 참조하십시오.

1. 다음 중 하나를 수행하십시오.

   1. 보고서에서 보기에 액세스하려면 보고서로 이동한 다음 **보고서 작업** > **편집** > **열(보기)** 탭을 클릭합니다.
   1. 목록에서 보기에 액세스하려면 목록으로 이동한 후 **보기** 드롭다운 메뉴에서 수정할 보기를 마우스로 가리키고 **편집** 아이콘 ![편집 아이콘](assets/edit-icon.png)을 클릭합니다.

      뷰 빌더 가 열립니다.

1. 보기에서 열을 선택합니다.

   또는

   Report Builder의 **열(보기)** 탭을 선택한 다음 열을 선택합니다.

   >[!TIP]
   >
   >텍스트 모드를 사용하여 뷰를 편집하려면 한 번에 한 열씩 편집해야 합니다.

1. 빌더의 오른쪽 상단에 있는 **텍스트 모드로 전환**&#x200B;을 클릭한 다음 **텍스트 모드 편집**&#x200B;을 클릭합니다.

   >[!NOTE]
   >
   >텍스트 모드에서 열을 편집하면 Workfront에서 `textmode=true` 코드 행을 열에 추가합니다. 텍스트 모드에서 열이 수정되었음을 나타냅니다.

   다음 표에서는 텍스트 모드 보기의 주요 행에 대해 설명합니다.

   <!--
   <p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: make this a snippet and add it to the grouping article too)</p>
   -->

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <thead> 
     <tr> 
      <th>샘플 라인</th> 
      <th>설명</th> 
     </tr> 
    </thead> 
    <tbody> 
     <tr> 
      <td> <p><ol><tr><tr><ol><tr><tr><tr><tr><tr><tr><tr><tr><tr><tr><div class="example" data-mc-autonum="<b>Example: </b>"><code><strong>valuefield</strong>=&lt;/cod></p> </td> 
      <td> <p>This is the name of the object or of the field as it appears in the database. For more information about how objects and fields appear in the database, see <a href="../../../wf-api/general/api-explorer.md" class="MCXref xref">API Explorer</a>.</p> <p>The following scenarios exist:</p> 
        
        <li value="1"> <p> If the name of the field you display is a phrase instead of a single noun, you must use camel case syntax for the <code>valuefield</code>. For example, for the Planned Start Date of a task the code is: </p> <p class="example" data-mc-autonum="<b>Example: </b>"><span class="autonumber"><span><b>Example: </b></span></span><code>valuefield=plannedStartDate</code> </p> </li> 
        <li value="2"> <p>If you want to display a custom field, the <code>valuefield</code> value is the actual name of the field, as you see it in the interface. For example, for a custom field named "More information", the code is:</p> <p class="example" data-mc-autonum="<b>Example: </b>"><span class="autonumber"><span><b>Example: </b></span></span><code>valuefield=More information</code> </p> </li> 
        <li value="3"> <p>If you want to display objects that are related to other objects in a view using the <code>valuefield</code> line of code the object names and attributes are separated by colons. </p> <p>For example, a column in a task view that would display the name of the Portfolio Owner has the following value for the valuefield line:</p> <p class="example" data-mc-autonum="<b>Example: </b>"><span class="autonumber"><span><b>Example: </b></span></span><code>valuefield=project:portfolio:owner:name</code> </p> <p>This indicates that from the object of the report (task), you can access the next related object (project), from there, you can access the following related object from project (portfolio), then the portfolio owner (owner) and then their name (name). </p> </li> 
       </ol> <p>For information about how objects connect to one another, see the section <a href="../../../workfront-basics/navigate-workfront/workfront-navigation/understand-objects.md#understanding-interdependency-and-hierarchy-of-objects" class="MCXref xref">Interdependency and hierarchy of objects</a> in <a href="../../../workfront-basics/navigate-workfront/workfront-navigation/understand-objects.md" class="MCXref xref">Understand objects in Adobe Workfront</a>.</p> <p>Note: If you choose a field in text mode that is not valid in the standard interface, you are not able to switch back to the standard interface within the column.</p> </td> 
     </tr> 
      
      <td><code><strong>valueformat=</strong></code> </td> 
      <td> <p>This line represents the format used to display the <code>valuefield</code>. The <code>valueformat</code> identifies whether an object or field displays as text, number, percentage, or date.</p> <p>We recommend using <code>HTML</code> for your <code>valueformat</code>, especially when using <code>valueexpression</code>, to ensure the most accurate display of your information. </p> <p>For information about additional values for this line, see <a href="../../../reports-and-dashboards/reports/text-mode/use-conditional-formatting-text-mode.md" class="MCXref xref">Use conditional formatting in Text Mode</a>.</p> </td> 
     </tr> 
      
      <td> <p><code><strong>valueexpression=</strong></code> </p> </td> 
      <td> <p>You can add this line to replace <code>valuefield</code>, if you want to display a calculated field in the column.</p> <p>You must enclose the <code>valuefield</code> of the objects in curly brackets every time you use it in a <code>valueexpression</code>.</p> <p>The following scenarios exist: </p> 
        
        <li value="1"> <p>If you want to display a field in a column in upper case, you would use:</p> <p class="example" data-mc-autonum="<b>Example: </b>"><span class="autonumber"><span><b>Example: </b></span></span><code>valueexpression=UPPER({valuefield})</code> </p> <p>The <code>valuefield</code> of the object is spelled as it appears in the API Explorer. </p> </li> 
        <li value="2">If you want to add multiple <code>valuefields</code> by stringing them together, you must separate them by a period.</li> 
        <li value="3"> <p>For example, if you want to display the name of the Primary Assignee of a task using <code>valueexpression</code>, you would use:</p> <p class="example" data-mc-autonum="<b>Example: </b>"><span class="autonumber"><span><b>Example: </b></span></span><code>valueexpreesion={assignedTo}.{name}</code> </p> </li> 
        <li value="4"> <p>If you want to use a custom field in a <code>valueexpression</code> line you must precede the name of the field by <code>DE:</code> to indicate that it is a custom field. The name of the field is spelled as it appears in the interface. </p> <p>Important: When you use a custom field that is placed in a custom form section that has restricted permissions for some users, the calculation of the valueexpression is blank when those users view this calculation in a report. For information about adjusting permissions on custom form sections, see <span help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/form-designer/design-a-form/design-a-form.md"><a href="/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/form-designer/design-a-form/design-a-form.md">Create a custom form</a></span>.</p> <p>For example, if you have a custom field labeled "Developer Name" and you want to display this field in upper case in a column, you can use the following <code>valueexpression</code> to indicate this:</p> <p class="example" data-mc-autonum="<b>Example: </b>"><span class="autonumber"><span><b>Example: </b></span></span><code>valueexpression=UPPER({DE:Developer Name}</code>) </p> <p>When referencing a Typeahead type custom field, use the following expression to reference the name of the object selected in a field labeled "Developer Name":</p> <p><code>valueexpression=UPPER({DE:Developer Name:name})</code> </p> </li> 
       </ol> </td> 
     </tr> 
      
      <td> <p><code><strong>descriptionkey=</strong></code> / <code><strong>description=</strong></code> </p> </td> 
      <td> <p>This line defines the text of a tool tip as you mouse over the name of the column. In this case it is using a key to translate the name value in the description text. If you want to modify the description, change this line to read: </p> <p class="example" data-mc-autonum="<b>Example: </b>"><span class="autonumber"><span><b>Example: </b></span></span><code>description=Your Value</code>.</p> </td> 
     </tr> 
      
      <td><code><strong>namekey=</code> / <code><strong>name=</strong></code> </td> 
      <td> <p>This line defines the column label. In this case it is using the abbreviated value based on the key.</p> <p>If you want to modify the column name you can change this value to: </p> <p class="example" data-mc-autonum="<b>Example: </b>"><span class="autonumber"><span><b>Example: </b></span></span><code>name=Your Value</code> </p> <p><code>Name</code> allows you to enter any text for the column name, while<code>namekey</code> requires you enter a key that is used to translate the name of a column.</p> <p>To change the column name you can also add the <code>displayname </code>line, if one is not present.</p> </td> 
     </tr> 
      
      <td><code><strong>displayname =</strong></code> </td> 
      <td> <p>You can add the following line to change the name of a column, which suspends the <code>namekey/name</code> value:</p> <p class="example" data-mc-autonum="<b>Example: </b>"><span class="autonumber"><span><b>Example: </b></span></span><code>displayname=Your Value</code> </p> </td> 
     </tr> 
      
      <td><code><strong>querysort=</strong> </code></td> 
      <td>This line defines how the results are sorted when the column header is clicked. If it is not present then the column cannot be sorted after the report is run.</td> 
     </tr> 
      
      <td><code><strong>width=</strong></code> </td> 
      <td> <p>This line represents the number of pixels that are used for the column. If the line is omitted or set to 0 (zero) then the column does not appear in the view.</p> <p>When you modify this field manually in text mode, you must also add the <code>usewidths=true</code> value to your column.</p> </td> 
     </tr> 
      
      <td><code><strong>usewidths=true</strong></code> </td> 
      <td> <p>You must use this line in addition to the <code>width=</code> line when customizing the width of a column. </p> </td> 
     </tr> 
      
      <td><code><strong>makeFieldEditable=</strong></code> </td> 
      <td> <p>This line defines whether the value displayed in a column is inline editable or not. If this line equals <strong>true</strong>, the value in the column is inline editable. If this line equals <code>false</code>, the value in the column is not inline editable.</p> </td> 
     </tr> 
      
      <td><code><strong>link.valuefield=</strong> </code></td> 
      <td> <p>Insert this line only when you want the value displayed in a column to link to the object associated with it. The link opens the details page of the object. This value should match the <code>valuefield=</code> line. When you insert this, you must also add the <code>link.valueformat=</code> line. </p> <p> For example, you can insert <code>link.valuefield=priority</code> in an issue view, and the Priority of the issue displays as a link. Clicking this link opens the Issue page.</p> </td> 
     </tr> 
      
      <td><code><strong>link.valueformat=</strong> </code></td> 
      <td> <p>Insert this line only when you have inserted the <code>link.valuefield</code> line to add a link to the value in a column. The link opens the details page of the object. This value should match the <code>valueformat=</code> line and indicates the format used to display the <code>valuefield</code>. </p> <p>Important: When viewing the text mode in a built-in column that also includes a link, you notice a number of lines referring to the link. Some of those lines might no longer be supported or are unnecessary when you create your own custom column in text mode and add the link statements to it. The lines that are mandatory when adding a linked value are<code> link.valuefield</code> and <code>link.valueformat</code>. </p> </td> 
     </tr> 
      
      <td><code><strong>aggregator.function=</strong></code> </td> 
      <td> <p>This refers to how the values of each column are summarized. There are multiple lines that start with <code>aggregator.</code> and they all refer to the aggregator that summarizes the results of the column. </p> <p>As a general rule, the <code>aggregator.</code> lines match those of the column object. </p> 
       
        <span class="autonumber"><span><b>Example: </b></span></span> 
        <p>The Planned&nbsp;Hours column in a task report summarized by Sum may look like the following: </p>

   <div>
         <code>textmode=true</code>
         <code>valuefield=workRequired</code>
         <code>valueformat=compound</code>
         <code>aggregator.function=SUM</code>
         <code>aggregator.valuefield=workRequired</code>
         <code>aggregator.displayformat=minutesAsHoursString</code>
         <code>aggregator.valueformat=compound</code>
         <code>namekey=workRequired</code>
         <code>shortview=false</code> 
        </div> 
       </div>

   <div>
      <code>aggregator. </code>줄에 <code>valuefield </code> 또는 <code>valueexpression</code>이(가) 포함될 수 있습니다.
       </div> </td> 
     </tr> 
    </tbody> 
   </table>

1. 변경 내용을 저장하고 보기를 계속 편집하려면 **적용**&#x200B;을 클릭합니다.
1. 보고서를 저장하려면 **저장 + 닫기**&#x200B;를 클릭하십시오.

   또는

   **보기 저장**&#x200B;을 클릭하여 목록에 보기를 저장합니다.
