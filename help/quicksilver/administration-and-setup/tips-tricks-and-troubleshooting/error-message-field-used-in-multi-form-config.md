---
user-type: administrator
content-type: tips-tricks-troubleshooting
product-area: system-administration
navigation-topic: tips-tricks-troubleshooting-setup-admin
title: '''오류 메시지: 약간의 문제가 있습니다. 이 필드는 다중 양식 구성에서 사용됩니다.'
description: 사용자 지정 양식의 계산된 사용자 지정 필드에서 계산을 변경하고 오류 메시지에 이 필드가 다중 양식 구성에서 사용된다는 메시지가 표시되면 해당 필드를 사용할 계산을 포함하는 새 필드로 바꿔야 합니다.
author: Caroline
feature: System Setup and Administration
role: Admin
exl-id: 43668525-5572-4d82-8eed-0e320249f296
source-git-commit: c2bf6441e4ac8520a56d4005b3e87c48370dc065
workflow-type: tm+mt
source-wordcount: '1222'
ht-degree: 0%

---

# 오류 메시지: 약간의 문제가 있습니다. 이 필드는 다중 양식 구성에 사용됩니다

## 문제

사용자 지정 양식의 계산된 사용자 지정 필드에서 계산을 변경하면 [!DNL Adobe Workfront] 다음 경고가 표시될 수 있습니다.

약간의 문제가 발생했습니다.

[필드] 다중 양식 구성에 사용됩니다. 이 수식을 변경하려면 이 필드를 제거하고 원하는 계산을 포함하는 새 수식으로 바꾸어야 합니다.

## 원인

변경하려는 계산된 사용자 지정 필드가 포함된 두 개 이상의 사용자 지정 양식이 [!DNL Workfront] 인스턴스.

**예:** 사용자 지정 양식 A와 B는 모두 동일한 작업에 연결됩니다. 두 양식에는 Profit이라는 계산된 사용자 지정 필드가 포함되어 있습니다. 사용자 지정 양식 A의 이익 필드에서 계산을 편집하려고 할 때 오류가 발생합니다.

한 양식의 사용자 지정 필드에 대한 계산은 다른 양식의 동일한 필드에 있는 수식과 충돌하므로 변경할 수 없습니다.
이 충돌을 해결하려면 동일한 계산된 사용자 지정 필드가 있는 여러 양식이 첨부된 개체를 찾은 다음 다음 중 하나를 수행해야 합니다.

* 개체에서 양식 중 하나를 제거합니다.
* 필요에 따라 계산을 변경하지만 객체에 첨부된 모든 사용자 지정 양식에서 변경합니다.
* 객체에 첨부된 모든 사용자 지정 양식에서 필요한 계산을 포함하는 새 계산된 사용자 지정 필드를 추가하고 기존의 계산된 사용자 지정 필드를 더 이상 사용하지 않는 것으로 표시합니다.

이 문서에서는 개체를 찾은 다음 이 세 가지 방법 중 하나로 문제를 해결하는 방법을 설명합니다.

## 사용자 지정 양식이 첨부된 개체를 찾습니다 {#find-the-object-where-the-custom-forms-are-attached}

1. 을(를) 클릭합니다. **[!UICONTROL 기본 메뉴]** 아이콘 ![](assets/main-menu-icon.png) 의 오른쪽 위 모서리에서 [!DNL Adobe Workfront]를 클릭한 다음 **[!UICONTROL 사용자]** ![](assets/users-icon-in-main-menu.png).

1. 클릭 **[!UICONTROL 사용자 지정 Forms]** > **[!UICONTROL 필드]**.
1. 적용 **[!UICONTROL 필드 목록]** 보려는 계산된 필드를 찾고 양식 1, 양식 2, 양식 3 등 이 필드를 사용하는 모든 사용자 지정 양식을 기록해 둡니다.
1. 클릭 **[!UICONTROL Forms]**&#x200B;를 적용한 후 **[!UICONTROL 양식 목록]** 보기.
1. 을(를) 클릭합니다. **[!UICONTROL 필터]** 드롭다운 목록을 클릭한 다음 **[!UICONTROL 새 필터]**.

1. 클릭 **[!UICONTROL 필터 규칙 추가]**&#x200B;을 입력한 다음 &quot;사용자 지정 양식 이름&quot; 입력을 시작하고 목록에 이 값이 표시되면 이 값을 선택합니다.
1. 선택 **[!UICONTROL Equal]** 필터 수정자의 경우, 1단계에서 메모한 각 양식의 이름을 입력을 시작한 다음 표시될 때 선택합니다.

   **예:** 사용자 지정 양식 이름은 양식 1, 양식 2, 양식 3입니다.

1. 클릭 **[!UICONTROL 필터 저장]**&#x200B;를 클릭한 다음 새 필터의 이름을 지정하고 **[!UICONTROL 필터 저장]**.

1. 양식 목록에서, **[!UICONTROL 유형]** 열.
1. 1단계에서 찾은 각 사용자 지정 양식에서 단일 기본값이 Yes인 새 확인란 사용자 지정 필드를 만듭니다.

   **예:** 양식 1의 필드 1 = 예, 양식 2의 필드 2 = 예, 양식 3의 필드 3 = 예. 이는 &quot;계산된 사용자 지정 필드가 양식 1에 있음&quot; 또는 &quot;계산된 사용자 지정 필드가 양식 2에 있음&quot; 등을 의미합니다.

1. 에서 **[!UICONTROL 검색 아이콘]** ![](assets/search-icon.png) 화면의 오른쪽 상단 모서리에서 을(를) 클릭합니다. **[!UICONTROL 고급 검색]**.
1. 사용자 지정 양식 개체(예: 문제)를 클릭하고 **[!UICONTROL 결과 필터링]**&#x200B;를 클릭한 다음 **[!UICONTROL 필터 추가]**.
1. 에 확인란 필드 이름을 입력합니다. **[!UICONTROL 필드 이름 입력 시작]** 필드를 선택하고 목록에 표시될 때 선택한 다음 **[!UICONTROL Equal]** 및 유형 **[!UICONTROL 예]** (큰따옴표 없이)를 클릭하여 입력할 수 있습니다.

   **예:** 필드 1 같음(대/소문자 구분) 예.

1. 클릭 **[!UICONTROL 필터 추가]** 고급 검색에 모든 확인란 필드를 추가합니다.

   가능한 모든 조합을 찾습니다.

   **예:** 아래 나열된 대로 찾은 조합으로 여러 필터를 빌드합니다. 동일한 계산된 필드를 포함하는 여러 사용자 지정 양식이 있는 개체를 찾아야 합니다. 다음 시나리오를 찾을 수 있습니다.

   * 필드 1= 예 + 필드 2 = 예 + 필드 3 = 예(예: 객체 없음)
   * 필드 1 = 예 + 필드 2 = 예(예: 객체 없음)
   * 필드 1 = 예 + 필드 3 = 예(예: 두 개의 객체)

   즉, 해당 확인란 필드(필드 1 및 필드 3)가 이러한 개체에 존재하므로 계산된 필드가 양식 1과 양식 3 모두에 존재합니다.

   필드 2 = 예 + 필드 3 = 예(예: 객체 없음)

1. 이 문서에서 다음 섹션 중 하나를 계속 진행합니다.

   * [개체에서 사용자 지정 양식 중 하나를 제거하고 거기에서 계산을 편집합니다](#remove-one-of-the-custom-forms-from-the-object-and-edit-the-calculation-there)
   * [첨부된 모든 사용자 지정 양식에서 계산에서 동일한 편집 작업을 수행합니다](#make-identical-edits-in-the-calculation-in-all-of-the-attached-custom-forms)
   * [편집된 계산이 포함된 새 계산된 필드를 첨부된 사용자 지정 양식 중 하나 또는 모두에 추가합니다](#add-a-new-calculated-field-containing-the-edited-calculation-to-one-or-all-of-the-attached-custom-forms)

## 개체에서 사용자 지정 양식 중 하나를 제거하고 거기에서 계산을 편집합니다 {#remove-one-of-the-custom-forms-from-the-object-and-edit-the-calculation-there}

1. 다음에 설명된 대로 사용자 지정 양식이 첨부된 개체를 찾습니다. [사용자 지정 양식이 첨부된 개체를 찾습니다](#find-the-object-where-the-custom-forms-are-attached) 이 문서에서 개체를 엽니다.
1. 개체에서 사용자 지정 양식 중 하나를 제거한 다음 개체를 저장합니다.

   >[!NOTE]
   >
   >개체에서 제거한 양식에서 필드를 추가하려면 개체에 첨부된 사용자 지정 양식을 편집해야 할 수 있습니다. 이렇게 하면 개체의 사용자 지정 데이터 정보를 유지할 수 있습니다.

1. 제거한 사용자 지정 양식에서 원래 업데이트하려는 사용자 지정 필드의 계산을 편집한 다음 를 클릭합니다 **[!UICONTROL 저장]**.

   이번에는 [!DNL Workfront] 충돌이 있어서는 안 된다.

1. (선택 사항) 사용자 지정 양식에서 확인란 필드를 제거하거나 [!DNL Workfront].

## 첨부된 모든 사용자 지정 양식에서 계산에서 동일한 편집 작업을 수행합니다 {#make-identical-edits-in-the-calculation-in-all-of-the-attached-custom-forms}

>[!IMPORTANT]
>
>이 단계를 수행하면 사용자 지정 양식이 이미 첨부된 개체에서 데이터가 손실됩니다. 그러나 계산된 필드가 계산된 필드가 아닌 정적 필드를 참조하는 경우 [!UICONTROL 사용자 지정 표현식 다시 계산] 개체의 옵션을 사용하여 손실된 데이터를 복원합니다.

1. 다음에 설명된 대로 사용자 지정 양식이 첨부된 개체를 찾습니다. [사용자 지정 양식이 첨부된 개체를 찾습니다](#find-the-object-where-the-custom-forms-are-attached) 참조하십시오.
1. 객체에 첨부된 모든 사용자 지정 양식에서 필드를 제거한 다음 양식을 저장합니다.

1. 새 계산이 포함된 사용자 지정 필드를 다시 사용자 지정 양식에 추가합니다.

   >[!IMPORTANT]
   >
   >계산은 첨부된 모든 사용자 지정 양식에서 동일해야 합니다.

1. (선택 사항) 양식에서 확인란 필드를 제거하거나 [!DNL Workfront].

## 편집된 계산이 포함된 새 계산된 필드를 첨부된 사용자 지정 양식 중 하나 또는 모두에 추가합니다 {#add-a-new-calculated-field-containing-the-edited-calculation-to-one-or-all-of-the-attached-custom-forms}

기존의 계산된 사용자 지정 필드에서 데이터가 손실되지 않도록 하거나 찾은 개체에 첨부된 사용자 지정 양식 중 하나에서만 편집된 계산을 수행해야 하는 경우:

1. 다음에 설명된 대로 사용자 지정 양식이 첨부된 개체를 찾습니다. [사용자 지정 양식이 첨부된 개체를 찾습니다](#find-the-object-where-the-custom-forms-are-attached) 참조하십시오.
1. 하나 또는 모든 양식에 필요한 계산을 포함하는 계산된 새 사용자 지정 필드를 추가합니다.
1. 이전에 계산된 사용자 지정 필드의 이름을 변경합니다 **사용되지 않음**.

   객체에 첨부된 모든 양식에서 이 오래된 계산된 사용자 지정 양식은 이전 데이터를 보존하지만 사용자가 해당 데이터 사용을 중지합니다.

   >[!IMPORTANT]
   >
   >이전 필드는 다른 계산된 사용자 지정 필드에서 참조될 수 있으므로 이름을 변경한 후 이러한 계산을 업데이트해야 합니다.

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
<p>For more information about creating a custom form and adding or removing fields from it, see <a href="../../administration-and-setup/customize-workfront/create-manage-custom-forms/create-or-edit-a-custom-form.md" class="MCXref xref" xrefformat="{para}">Create or edit a custom form</a>.</p>
</blockquote>
-->
