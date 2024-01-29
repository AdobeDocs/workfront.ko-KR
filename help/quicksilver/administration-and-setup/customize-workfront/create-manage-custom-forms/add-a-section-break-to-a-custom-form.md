---
user-type: administrator
product-area: system-administration
navigation-topic: create-and-manage-custom-forms
title: 기존 양식 빌더로 사용자 정의 양식에 섹션 구분 추가
description: 사용자 정의 양식의 사용자 정의 필드 및 위젯을 제목이 있는 섹션으로 그룹화할 수 있습니다. 이 기능은 양식을 작성할 사용자에게 구성된 경험을 제공하는 데 유용합니다. 또한 특정 사용자 정의 필드 및 위젯에 대한 액세스를 특정 사용자로 제한해야 하는 경우 섹션에 배치한 다음 해당 사용자에게만 섹션에 대한 액세스 권한을 부여할 수 있습니다.
author: Lisa
feature: System Setup and Administration, Custom Forms
role: Admin
exl-id: 44a52767-60a7-4aaa-b3b8-6b8fb7da7e72
source-git-commit: 56e1ceac4f37d9789f4a3a37ee0e6a7774133bfb
workflow-type: tm+mt
source-wordcount: '1173'
ht-degree: 0%

---

# 기존 양식 빌더로 사용자 정의 양식에 섹션 구분 추가

사용자 정의 양식의 사용자 정의 필드 및 위젯을 제목이 있는 섹션으로 그룹화할 수 있습니다. 이 기능은 양식을 작성할 사용자에게 구성된 경험을 제공하는 데 유용합니다. 또한 특정 사용자 정의 필드 및 위젯에 대한 액세스를 특정 사용자로 제한해야 하는 경우 섹션에 배치한 다음 해당 사용자에게만 섹션에 대한 액세스 권한을 부여할 수 있습니다.

예를 들어 시스템 관리자만 보거나 편집할 수 있어야 하는 중요한 정보를 추적해야 하는 경우 관리자 전용 권한으로 섹션 구분을 만들고 해당 섹션에 중요한 필드를 배치할 수 있습니다.

섹션에 대해 선택하는 액세스 설정은 사용자 정의 양식이 첨부된 Workfront 개체에서 사용자가 갖는 권한에 직접 연결되어 있습니다. 사용자가 해당 개체를 보거나, 기여하거나, 관리할 수 있는 액세스 권한을 가지고 있는지 여부에 따라 섹션을 숨기거나 표시할 수 있습니다. 또는 시스템 관리자 액세스 수준이 있는 사용자만 액세스할 수 있도록 섹션을 관리 전용으로 설정할 수 있습니다.

개체의 사용 권한에 대한 자세한 내용은 [오브젝트에 대한 공유 권한 개요](../../../workfront-basics/grant-and-request-access-to-objects/sharing-permissions-on-objects-overview.md).

사용자 정의 양식의 사용자 정의 필드 및 위젯에 대한 자세한 내용은 [사용자 정의 양식에 사용자 정의 필드 추가](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/add-a-custom-field-to-a-custom-form.md) 및 [사용자 정의 양식에서 에셋 위젯 추가 또는 편집](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/add-widget-or-edit-its-properties-in-a-custom-form.md).

<!--
>[!TIP]
>
>Section breaks that you add to custom forms are saved in your system for re-use. For information about listing them, see [List and edit custom forms and widgets added to custom forms](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/list-edit-share-custom-forms-and-custom-fields.md).
-->

## 액세스 요구 사항

이 문서의 단계를 수행하려면 다음이 있어야 합니다.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr data-mc-conditions=""> 
   <td role="rowheader"> <p>Adobe Workfront 플랜</p> </td> 
   <td>임의</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront 라이선스</td> 
   <td>
   <p>새로운 기능: 표준</p>
   <p>현재: 플랜</p></td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader">액세스 수준 구성</td> 
   <td> <p>사용자 정의 양식에 대한 관리 액세스</p></td> 
  </tr>  
 </tbody> 
</table>

이 표의 정보에 대한 자세한 내용은 [Workfront 설명서의 액세스 요구 사항](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

## 사용자 정의 양식의 섹션에 대한 액세스 만들기 및 구성

1. 에 설명된 대로 사용자 정의 양식을 만들거나 편집하기 시작합니다. [사용자 정의 양식 만들기 또는 편집](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/create-or-edit-a-custom-form.md).
1. 에 설명된 대로 양식에 사용자 정의 필드 및 위젯 추가 [사용자 정의 양식에 사용자 정의 필드 추가](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/add-a-custom-field-to-a-custom-form.md) 및 [사용자 정의 양식에서 에셋 위젯 추가 또는 편집](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/add-widget-or-edit-its-properties-in-a-custom-form.md).

1. 사용자 정의 양식을 만들거나 편집하는 동안 **필드 추가** 탭을 클릭하고 **섹션 구분**.

   ![](assets/click-section-break.jpg)

1. 다음에서 **필드 설정** 탭에서 섹션에 사용할 옵션을 구성합니다.

   <table style="table-layout:auto"> 
    <col> 
    </col> 
    <col> 
    </col> 
    <tbody> 
     <tr> 
      <td role="rowheader">레이블</td> 
      <td> <p>(필수) 섹션 위에 표시할 설명 레이블을 입력합니다. 언제든지 레이블을 변경할 수 있습니다.</p> <p><b>중요 사항</b>: 이 레이블에는 특수 문자를 사용하지 마십시오. 보고서에 올바로 표시되지 않습니다.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">설명</td> 
      <td>섹션의 용도를 사용자에게 설명하려면 텍스트를 입력합니다. 사용자 정의 양식에서 섹션의 레이블 아래에 표시됩니다.</td> 
     </tr> 
     <tr> 
      <td role="rowheader"><p>논리 추가</p></td> 
      <td><p>표시 논리를 사용하여 사용자가 양식을 작성할 때 다중 선택 사용자 정의 필드에서 선택한 항목에 따라 섹션을 양식에 표시할지 여부를 지정합니다.</p><p><strong>참고:</strong> 섹션 구분 아래의 모든 개별 필드에 표시 논리가 적용되어 있고 논리의 결과로 해당 필드가 모두 숨겨져 있는 경우 사용자 정의 양식에서 전체 섹션이 숨겨집니다. 이 문제는 표시 논리가 섹션 구분에 적용되지 않는 경우에도 발생합니다.</p><p>자세한 내용은 <a href="../../../administration-and-setup/customize-workfront/create-manage-custom-forms/display-or-skip-logic-custom-form.md" class="MCXref xref">사용자 정의 양식에 표시 논리 및 건너뛰기 논리 추가</a>.</p></td> 
     </tr> 
     <tr> 
      <td role="rowheader"> <p>액세스 권한 부여</p> </td> 
      <td> <p> 이 섹션을 보고 해당 필드 값을 편집하려면 사용자 정의 양식이 첨부된 오브젝트에서 사용자에게 필요한 권한을 선택하십시오.
       <p>다음 권한은 다음에서 사용할 수 있습니다. <b>오브젝트에 대한 이 액세스 권한이 있는 사용자는 필드 값을 볼 수 있습니다.</b>:</p> 
         <ul>
          <li><strong>보기</strong>: 오브젝트에 대한 권한 보기</li>
          <li><p><b>제한된 편집</b>: (객체가 프로젝트, 작업, 문제 또는 사용자인 경우에만 사용 가능):</p> 
          <p>프로젝트, 작업 또는 문제인 경우 사용자가 오브젝트에 기여할 수 있도록 허용합니다.</p>
          <p>사용자가 프로필을 편집하거나, 사용자의 경우 개체에 대한 프로필 권한을 소유할 수 있습니다.</p></li> 
          <li><b>편집</b>: 오브젝트에 대한 권한 관리 </li> 
          <li><b>관리자만</b>: 시스템 관리자 액세스 수준</li> 
         </ul> </li> 
        <p>다음 권한은 다음에서 사용할 수 있습니다. <b>오브젝트에 대한 이 액세스 권한이 있는 사용자는 필드 값을 편집할 수 있습니다.</b>: </p> 
         <ul> 
          <li> <p><b>제한된 편집</b>: (객체가 프로젝트, 작업, 문제 또는 사용자인 경우에만 사용 가능):</p> 
           <p>객체가 프로젝트, 작업 또는 문제인 경우 이 권한을 사용하여 사용자가 객체에 기여할 수 있습니다</p>
          <p>개체가 사용자인 경우 이 권한을 사용하여 사용자가 프로필을 편집하거나 개체에 대한 프로필 권한을 소유할 수 있습니다.</p> 
          <li><b>편집</b>: 오브젝트에 대한 권한 관리 </li> 
          <li><b>관리자만</b>: 시스템 관리자 액세스 수준</li> 
         </ul> </li> 
       </ul> 
       <p>개체의 사용 권한에 대한 자세한 내용은 <a href="../../../workfront-basics/grant-and-request-access-to-objects/sharing-permissions-on-objects-overview.md" class="MCXref xref">오브젝트에 대한 공유 권한 개요</a>.</p> 
       <p><b>참고</b>:  
       <ul> 
       <li> <p>여기에서 지정한 권한이 없는 사용자는 섹션에서 사용자 정의 필드 및 위젯을 볼 수 없습니다. </p> <p>이는 보고서의 필드 값을 표시하거나 텍스트 모드 보고의 계산된 필드에서 사용하는 경우에도 마찬가지입니다.</p> </li> 
       <li> <p>여러 객체 유형을 양식과 연결하면 다음 단계에서 사용할 수 있는 보기 및 편집 권한이 변경될 수 있습니다. 자세한 내용은 <a href="#how-multiple-object-types-can-affect-section-break-permissions-in-a-custom-form" class="MCXref xref">여러 오브젝트 유형이 사용자 정의 양식의 섹션 구분 권한에 영향을 주는 방법</a> 이 문서에서.</p> </li> 
        </ul> </p> </td> 
     </tr> 
    </tbody> 
   </table>

1. 하나 이상의 사용자 정의 필드 또는 위젯을 새 섹션으로 드래그하거나 추가합니다.

   섹션을 저장하기 전에 필요합니다.

1. 클릭 **완료**.

   >[!TIP]
   >
   >다음을 클릭할 수 있습니다. **적용** 언제든지 사용자 정의 양식을 만들어 변경 사항을 저장하고 양식을 열어 둡니다.

1. 다른 방법으로 사용자 정의 양식을 계속 작성하려면 다음 문서 중 하나를 계속 진행하십시오.

   * [사용자 정의 양식에 사용자 정의 필드 추가](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/add-a-custom-field-to-a-custom-form.md#add2)
   * [사용자 정의 양식에서 에셋 위젯 추가 또는 편집](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/add-widget-or-edit-its-properties-in-a-custom-form.md)
   * [사용자 정의 양식에 계산된 데이터 추가](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/add-calculated-data-to-custom-form.md)
   * [사용자 정의 양식에 사용자 정의 필드 및 위젯 배치](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/position-fields-in-a-custom-form.md)
   * [사용자 정의 양식에 표시 논리 및 건너뛰기 논리 추가](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/display-or-skip-logic-custom-form.md)
   * [사용자 정의 양식 미리 보기 및 완료](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/preview-and-complete-a-custom-form.md)

<!--
DRAFTED IN FLARE:
<h2>Configure access for fields without section breaks</h2>
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">************This section might get added later. Team decided not to implement.</p>
<p>In a custom form, you can also control users' access to custom fields
and image widgets that are not placed inside a defined section.</p>
<ol>
<li value="1">Begin creating or editing a custom form, as described in <a href="../../../administration-and-setup/customize-workfront/create-manage-custom-forms/create-or-edit-a-custom-form.md" class="MCXref xref">Create or edit a custom form</a>.</li>
<li value="2">Add custom fields

and widgets

to the form, as described in <a href="../../../administration-and-setup/customize-workfront/create-manage-custom-forms/add-a-custom-field-to-a-custom-form.md" class="MCXref xref">Add a custom field to a custom form</a>.</li>
<li value="3"> <p>While still creating or editing the custom form, open the <b>Form settings</b> tab.</p> <p>SHOW THIS </p> </li>
<li value="4"> <p>Under <b>Grant access</b>, configure the permissions that users need on an object where the custom form is attached, in order to view and edit values in fields not placed under a section break. </p> <p>If you need information about permissions on objects, see <a href="../../../workfront-basics/grant-and-request-access-to-objects/sharing-permissions-on-objects-overview.md" class="MCXref xref">Overview of sharing permissions on objects</a>.</p> <note type="note">
<ul>
<li> <p>Users without the permissions you specify here can't see the values of the fields
and image widgets that are not placed in a defined section in the custom form. This is also true if you display the values in reports or use them in calculated fields in text mode reporting.</p> </li>
<li> <p>Associating multiple object types with your form can change the viewing and editing permissions that are available in these steps. For more information, see <a href="#how-multiple-object-types-can-affect-section-break-permissions-in-a-custom-form" class="MCXref xref">How multiple object types can affect section break permissions in a custom form</a> in this article.</p> </li>
</ul>
</note>
<table style="table-layout:auto">
<col>
<col>
<tbody>
<tr>
<td role="rowheader"><b>Users with this access to the object can view field values</b> </td>
<td>
<ul>  
<li> <p><b>Limited Edit</b>: (Available only if the object is a project, task, issue, or user):</p>
<ul>
<li> <p>Contribute permission to the object if it's a project, task, or issue</p> </li>
<li> <p>Edit the profile or own the profile permission to the object if it's a user (profile)</p> </li>
</ul> </li>
<li><b>Edit</b>: Manage permissions to the object </li>
<li><b>Admin only</b>: System Administrator access level</li>
</ul> </td>
</tr>
<tr>
<td role="rowheader">Users with this access to the object can edit field values</td>
<td>
<ul>
<li> <p><b>Limited Edit</b>: (Available only if the object is a project, task, issue, or user):</p>
<ul>
<li> <p>Contribute permission to the object if it's a project, task, or issue</p> </li>
<li> <p>Edit the profile or own the profile permission to the object if it's a user (profile)</p> </li>
</ul> </li>
<li><b>Edit</b>: Manage permissions to the object </li>
<li><b>Admin only</b>: System Administrator access level</li>
</ul> </td>
</tr>
</tbody>
</table> </li>
<li value="5"> <p>Click Done.</p> <note type="tip">
You can click
<strong>Apply</strong> at any point while you are creating a custom form to save your changes and keep the form open.
</note> </li>
<li value="6"> <p>If you want to continue building your custom form in other ways, continue on to one of the following articles:</p>
<ul>
<li><a href="../../../administration-and-setup/customize-workfront/create-manage-custom-forms/add-a-custom-field-to-a-custom-form.md#add2" class="MCXref xref">Add a custom field to a custom form</a> </li>
<li><a href="../../../administration-and-setup/customize-workfront/create-manage-custom-forms/add-widget-or-edit-its-properties-in-a-custom-form.md" class="MCXref xref">Add or edit an asset widget in a custom form</a> </li>
<li><a href="../../../administration-and-setup/customize-workfront/create-manage-custom-forms/add-calculated-data-to-custom-form.md" class="MCXref xref">Add calculated data to a custom form</a> </li>
<li><a href="../../../administration-and-setup/customize-workfront/create-manage-custom-forms/position-fields-in-a-custom-form.md" class="MCXref xref">Position custom fields and widgets in a custom form</a> </li>
<li><a href="../../../administration-and-setup/customize-workfront/create-manage-custom-forms/display-or-skip-logic-custom-form.md" class="MCXref xref">Add display logic and skip logic to a custom form</a> </li>
<li><a href="../../../administration-and-setup/customize-workfront/create-manage-custom-forms/preview-and-complete-a-custom-form.md" class="MCXref xref">Preview and complete a custom form</a> </li>
</ul> </li>
</ol>
</div>
-->

## 여러 객체 유형이 섹션 구분 권한에 미치는 영향 {#how-multiple-object-types-can-affect-section-break-permissions-in-a-custom-form}

사용자 정의 양식 섹션 구분에 대한 제한된 편집 권한은 프로젝트, 작업, 문제 및 사용자 객체 유형에 대해서만 사용할 수 있습니다.

제한된 편집 권한으로 구성된 섹션 구분이 있는 사용자 정의 양식에서 다른 객체 유형 중 하나(Portfolio, 프로그램, 문서, 회사, 청구 기록, 반복, 경비 또는 그룹)를 양식에 추가하는 경우 해당 객체 유형 및 양식의 기존 객체 유형 모두와 호환되는 편집 권한으로 전환하라는 메시지가 표시됩니다.

>[!INFO]
>
>**예:** 프로젝트 오브젝트 유형과 연결된 사용자 정의 양식에서 제한된 편집 권한으로 섹션 구분이 구성됩니다.
>
>Portfolio 개체 유형을 양식에 추가하면 양식의 섹션 구분에 대해 제한된 편집 권한 옵션을 더 이상 사용할 수 없습니다.
>
>[편집] 권한으로 전환하라는 메시지가 화면에 표시됩니다. 이 권한은 [제한된 편집]과 가장 유사하며 프로젝트 객체 유형 및 Portfolio 객체 유형과 모두 호환됩니다.
