---
user-type: administrator
content-type: tips-tricks-troubleshooting
product-area: system-administration
navigation-topic: tips-tricks-troubleshooting-setup-admin
title: "오류 메시지: 약간의 문제가 있습니다. 해당 필드는 다중 양식 구성에서 사용됩니다."
description: 사용자 정의 양식의 계산된 사용자 정의 필드에서 계산을 변경할 때 필드가 다중 양식 구성에서 사용된다는 오류 메시지가 표시되면 필드를 사용할 계산이 포함된 새 필드로 바꿔야 합니다.
author: Lisa
feature: System Setup and Administration
role: Admin
exl-id: 43668525-5572-4d82-8eed-0e320249f296
source-git-commit: c389b4829f16bf82a5851a597f5dd358d9c96999
workflow-type: tm+mt
source-wordcount: '1239'
ht-degree: 0%

---

# 오류 메시지: 약간의 문제가 있습니다. 해당 필드는 다중 양식 구성에서 사용됩니다

## 문제

사용자 지정 양식의 계산된 사용자 지정 필드에서 계산을 변경하면 [!DNL Adobe Workfront]에 다음 경고가 표시될 수 있습니다.

약간의 문제가 발생했습니다.

[필드]이(가) 다중 형식 구성에 사용되었습니다. 이 수식을 변경하려면 이 필드를 제거하고 원하는 계산이 포함된 새 필드로 바꿔야 합니다.

## 원인

변경하려는 계산된 사용자 정의 필드가 포함된 사용자 정의 양식이 [!DNL Workfront] 인스턴스의 단일 개체에 연결되어 있습니다.

**예:** 사용자 정의 양식 A와 B가 모두 같은 작업에 연결되어 있습니다. 두 양식에 Profit이라는 계산된 사용자 정의 필드가 포함되어 있습니다. 사용자 정의 양식 A의 이익 필드에서 계산을 편집하려고 하면 오류가 발생합니다.

한 양식의 사용자 정의 필드에 대한 계산은 다른 양식의 동일한 필드에 있는 공식과 충돌하므로 변경할 수 없습니다.
이 충돌을 해결하려면 계산된 사용자 정의 필드가 동일한 여러 양식이 첨부된 개체를 찾은 후 다음 중 하나를 수행해야 합니다.

* 개체에서 양식 중 하나를 제거합니다.
* 필요에 따라 계산을 변경하되 객체에 첨부된 모든 사용자 정의 양식에서 계산을 변경합니다.
* 오브젝트에 첨부된 모든 사용자 정의 양식에서 필요한 계산이 포함된 새 계산된 사용자 정의 필드를 추가하고 이전 계산된 사용자 정의 필드를 더 이상 사용하지 않는 것으로 표시합니다.

이 문서에서는 객체를 찾은 다음 이 세 가지 방법 중 하나로 문제를 해결하는 방법에 대해 설명합니다.

## 사용자 정의 양식이 첨부된 오브젝트 찾기 {#find-the-object-where-the-custom-forms-are-attached}

{{step-1-to-setup}}

1. **[!UICONTROL 사용자 지정 Forms]** > **[!UICONTROL 필드]**&#x200B;를 클릭합니다.
1. **[!UICONTROL 필드 목록]** 보기를 적용하여 수정하려는 계산된 필드를 찾고 이 필드가 사용되는 모든 사용자 정의 양식(예: 양식 1, 양식 2, 양식 3) 을 메모하십시오.
1. **[!UICONTROL Forms]**&#x200B;을 클릭한 다음 **[!UICONTROL 양식 목록]** 보기를 적용합니다.
1. **[!UICONTROL 필터]** 드롭다운 목록을 클릭한 다음 **[!UICONTROL 새 필터]**&#x200B;을 클릭합니다.

1. **[!UICONTROL 필터 규칙 추가]**&#x200B;를 클릭한 다음 &quot;사용자 정의 양식 이름&quot;을 입력하고 목록에 표시될 때 이 값을 선택합니다.
1. 필터 수정자에 대해 **[!UICONTROL 같음]**&#x200B;을 선택하고 1단계에서 메모한 각 양식의 이름을 입력한 다음 표시될 때 선택합니다.

   **예:** 사용자 지정 양식 이름이 양식 1, 양식 2, 양식 3과 같습니다.

1. **[!UICONTROL 필터 저장]**&#x200B;을 클릭한 다음 새 필터의 이름을 지정하고 **[!UICONTROL 필터 저장]**&#x200B;을 클릭합니다.

1. 양식 목록에서 **[!UICONTROL Type]** 열에 표시되는 필터의 개체 유형(예: 작업 또는 문제)을 메모하십시오.
1. 1단계에서 찾은 각 사용자 정의 양식에서 단일 기본값이 Yes인 새 Checkbox 사용자 정의 필드를 만듭니다.

   **예:** 양식 1의 필드 1 = 예, 양식 2의 필드 2 = 예, 양식 3의 필드 3 = 예. 즉, &quot;계산된 사용자 정의 필드가 양식 1에 있음&quot; 또는 &quot;계산된 사용자 정의 필드가 양식 2에 있음&quot;이 됩니다.

1. 화면 오른쪽 상단의 **[!UICONTROL 검색 아이콘]** ![](assets/search-icon.png)에서 **[!UICONTROL 고급 검색]**&#x200B;을 클릭합니다.
1. 사용자 정의 양식의 개체(문제 등)를 클릭하고 **[!UICONTROL 결과 필터링]**&#x200B;을 클릭한 다음 **[!UICONTROL 필터 추가]**&#x200B;를 클릭합니다.
1. **[!UICONTROL 필드 이름을 입력하십시오]** 필드에 확인란 필드의 이름을 입력하십시오. 목록에 표시될 때 이 필드를 선택한 다음, **[!UICONTROL 같음]**&#x200B;을 선택하고 다음 상자에 **[!UICONTROL 예]**(따옴표 제외)를 입력하십시오.

   **예:** 필드 1은 같습니다(대/소문자 구분). 예.

1. **[!UICONTROL 필터 추가]**&#x200B;를 클릭하고 모든 확인란 필드를 고급 검색에 추가하십시오.

   가능한 모든 조합을 찾아라.

   **예:** 아래 나열된 대로 찾은 조합으로 여러 필터를 빌드합니다. 동일한 계산된 필드를 포함하는 사용자 정의 양식이 여러 개 첨부된 개체를 찾아야 합니다. 다음과 같은 시나리오를 찾을 수 있습니다.

   * 필드 1= 예 + 필드 2 = 예 + 필드 3 = 예(예: 오브젝트 없음)
   * 필드 1= 예 + 필드 2 = 예(예: 오브젝트 없음)
   * 필드 1= 예 + 필드 3 = 예(예: 두 개의 객체)

   즉, 해당 확인란 필드(필드 1과 필드 3)가 이 개체에 있으므로 계산된 필드가 양식 1과 양식 3 모두에 있습니다.

   필드 2 = 예 + 필드 3 = 예(예: 개체 없음)

1. 이 문서의 다음 섹션 중 하나를 계속 진행하십시오.

   * [오브젝트에서 사용자 정의 양식 중 하나를 제거하고 계산을 편집합니다](#remove-one-of-the-custom-forms-from-the-object-and-edit-the-calculation-there)
   * [첨부된 모든 사용자 정의 양식에서 계산에 동일한 편집을 수행합니다](#make-identical-edits-in-the-calculation-in-all-of-the-attached-custom-forms)
   * [첨부된 사용자 정의 양식 중 하나 또는 모두에 편집된 계산이 포함된 새 계산된 필드를 추가합니다](#add-a-new-calculated-field-containing-the-edited-calculation-to-one-or-all-of-the-attached-custom-forms)

## 오브젝트에서 사용자 정의 양식 중 하나를 제거하고 계산을 편집합니다 {#remove-one-of-the-custom-forms-from-the-object-and-edit-the-calculation-there}

1. 이 문서에서 [사용자 정의 양식이 첨부된 개체 찾기](#find-the-object-where-the-custom-forms-are-attached)에 설명된 대로 사용자 정의 양식이 첨부된 개체를 찾은 다음 개체를 엽니다.
1. 개체에서 사용자 정의 양식 중 하나를 제거한 다음 개체를 저장합니다.

   >[!NOTE]
   >
   >개체에서 제거한 양식에서 필드를 추가하려면 개체에 첨부된 상태로 남아 있는 사용자 정의 양식을 편집해야 할 수 있습니다. 이렇게 하면 개체에 대한 사용자 지정 데이터 정보를 보존할 수 있습니다.

1. 제거한 사용자 정의 양식에서 원래 업데이트하려는 사용자 정의 필드의 계산을 편집한 다음 **[!UICONTROL 저장]**&#x200B;을 클릭합니다.

   이번에는 [!DNL Workfront]에 충돌이 발생하지 않아야 합니다.

1. (선택 사항) 사용자 정의 양식에서 확인란 필드를 제거하거나 [!DNL Workfront]에서 삭제하십시오.

## 첨부된 모든 사용자 정의 양식에서 계산에 동일한 편집을 수행합니다 {#make-identical-edits-in-the-calculation-in-all-of-the-attached-custom-forms}

>[!IMPORTANT]
>
>이 단계를 수행하면 사용자 정의 양식이 이미 첨부된 오브젝트에서 데이터가 손실됩니다. 그러나 계산 필드가 계산 필드가 아닌 정적 필드를 참조하는 경우 개체의 [!UICONTROL 사용자 지정 표현식 다시 계산] 옵션을 사용하여 손실된 데이터를 복원할 수 있습니다

1. 이 문서에서 [사용자 정의 양식이 첨부된 개체 찾기](#find-the-object-where-the-custom-forms-are-attached)에 설명된 대로 사용자 정의 양식이 첨부된 개체를 찾습니다.
1. 오브젝트에 첨부된 모든 사용자 정의 양식에서 필드를 제거한 다음 양식을 저장합니다.

1. 새 계산이 포함된 사용자 정의 필드를 사용자 정의 양식에 다시 추가합니다.

   >[!IMPORTANT]
   >
   >첨부된 모든 사용자 정의 양식에서 계산이 동일해야 합니다.

1. (선택 사항) 양식에서 확인란 필드를 제거하거나 [!DNL Workfront]에서 삭제하십시오.

## 첨부된 사용자 정의 양식 중 하나 또는 모두에 편집된 계산이 포함된 새 계산된 필드를 추가합니다 {#add-a-new-calculated-field-containing-the-edited-calculation-to-one-or-all-of-the-attached-custom-forms}

기존 계산된 사용자 정의 필드의 데이터가 손실되지 않도록 하거나, 찾은 오브젝트에 첨부된 사용자 정의 양식 중 하나에서만 편집된 계산을 수행해야 하는 경우:

1. 이 문서에서 [사용자 정의 양식이 첨부된 개체 찾기](#find-the-object-where-the-custom-forms-are-attached)에 설명된 대로 사용자 정의 양식이 첨부된 개체를 찾습니다.
1. 필요한 계산이 포함된 새 계산된 사용자 정의 필드를 하나 또는 모든 양식에 추가합니다.
1. 이전에 계산된 사용자 지정 필드 **사용되지 않음**&#x200B;의 이름을 바꾸십시오.

   오브젝트에 첨부된 모든 양식에서 이 이전 계산된 사용자 정의 양식은 이전 데이터를 보존하지만 사용자는 사용을 중단합니다.

   >[!IMPORTANT]
   >
   >이전 필드는 다른 계산된 사용자 지정 필드에서 참조될 수 있으므로 이름을 변경한 후 해당 계산을 업데이트해야 합니다.

1. (선택 사항) 양식에서 확인란 필드를 제거하거나 Workfront에서 삭제합니다.

<!--
<blockquote data-mc-conditions="QuicksilverOrClassic.Draft mode">
<h2>Problem</h2>
<p>You get the following error while editing a calculated Custom Field on a custom form: </p>
<p><em>"<Name of custom field> field is used in a multi-form configuration, if you would like to change this formula you will need to remove this field and replace it with a new one containing the desired calculation."</em> </p>
<h2>Cause</h2>
<p>The error occurs because the following setup exists: currently you have at least one object in your system that has multiple custom forms attached. The calculated field you are editing exists on multiple forms attached to these objects.</p>
<p>You cannot have the same calculated field with different calculations on the same object. For this reason, the system does not allow you to make a change which will result in calculations being different.</p>
<p><a href="../../Resources/Images/Admin and setup/Tips, Tricks, and Troubleshooting/Calculated_field_error.png" class="MCXref xref" xrefformat="{para}"><img src="assets/calculated-field-error.png" alt="" width="542" height="272"></a> </p>
<p>For example, you have a task with custom forms A and B attached to it. Both forms contain the same calculated field, Field 1. You encounter this error when you try to edit the calculation for Field 1 on custom form A. </p>
<h2>Solution</h2>
<p>Remove the field from the custom form and replace it with a new one containing the desired calculation.  </p>
<p>To understand what custom forms are attached to objects, you can build a report for those objects and reference the Category Name field in the view of the report.<br>For more information about referencing custom forms in reports, see the "Referencing Custom Forms in a Report View (Column)" section in <a href="../../reports-and-dashboards/reports/creating-and-managing-reports/reference-custom-form-report.md" class="MCXref xref" xrefformat="{para}">Reference a custom form in a report</a>.</p>
<p>To understand what custom form contains a Custom Field, see the "Accessing Custom Forms and Fields" section in <a href="../../administration-and-setup/customize-workfront/create-manage-custom-forms/custom-forms-overview.md" class="MCXref xref" xrefformat="{para}">Custom forms overview</a>.</p>
</blockquote>
-->
