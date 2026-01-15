---
product-area: projects;user-management
keywords: 편집,양식,리치,텍스트,특수,서식,필드,사용자 지정,정보,사용자 지정,개체
navigation-topic: work-with-custom-forms
title: 사용자 정의 양식 필드의 정보 편집
description: 양식을 오브젝트에 첨부한 후 사용자 정의 양식에 대한 정보를 편집할 수 있습니다. 오브젝트에 사용자 정의 양식을 추가하는 방법에 대한 자세한 내용은 오브젝트에 사용자 정의 양식 추가를 참조하십시오.
author: Alina
feature: Get Started with Workfront
exl-id: c2b6afde-91a8-4e17-8e1a-3428b48e500a
source-git-commit: 6dce5e15a41587cd9febf82ffc0a62d3b7e121d1
workflow-type: tm+mt
source-wordcount: '1207'
ht-degree: 3%

---

# 사용자 정의 양식 필드의 정보 편집

<!--Audited: 10/2025-->

양식을 오브젝트에 첨부한 후 사용자 정의 양식에 대한 정보를 편집할 수 있습니다. 개체에 사용자 정의 양식을 추가하는 방법에 대한 자세한 내용은 [개체에 사용자 정의 양식 추가](../../workfront-basics/work-with-custom-forms/add-a-custom-form-to-an-object.md)를 참조하십시오.

## 액세스 요구 사항

+++ 이 문서의 기능에 대한 액세스 요구 사항을 보려면 확장하십시오.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <p>Adobe Workfront 패키지</p> </td> 
   <td>임의</td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>Adobe Workfront 라이선스</p> </td> 
   <td> <p>기여자 이상</p> 
   <p>요청 이상</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader">액세스 수준 구성</td> 
   <td> <p>사용자 정의 양식을 편집할 객체에 대한 액세스 편집</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader"> <p>개체 권한</p> </td> 
   <td> 
    <ul> 
     <li> <p>사용자 정의 양식을 편집할 오브젝트에 대한 기여 이상의 권한</p> </li> 
     <li><p>편집할 필드에 대한 권한을 봅니다.</p></li> 
     <li><p>편집할 필드가 있는 양식의 섹션에 대한 권한 편집</p></li> 
    </ul></td> 
  </tr> 
 </tbody> 
</table>

자세한 내용은 [Workfront 설명서의 액세스 요구 사항](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)을 참조하십시오.

+++

<!--Old:
<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <p>Adobe Workfront plan*</p> </td> 
   <td>Team or higher</td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>Adobe Workfront licenses*</p> </td> 
   <td> <p>Request or higher</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader">Access level*</td> 
   <td> <p>Edit access to the object for which you want to edit the custom form</p> <p>Note: If you still don't have access, ask your Workfront administrator if they set additional restrictions in your access level. For information on how a Workfront administrator can change your access level, see <a href="../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Create or modify custom access levels</a>.</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader"> <p>Object permissions</p> </td> 
   <td> 
    <ul> 
     <li> <p>Contribute or higher permissions on the object for which you want to edit the custom form</p> </li> 
     <li>View permissions on the fields you want to edit. For information about sharing permissions for custom fields, see <a href="/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/form-designer/manage-a-form/share-custom-fields.md" class="MCXref xref">Configure sharing for custom fields and widgets</a>.</li> 
     <li> <p>Edit permissions for the sections on the form where the fields you want to edit are located</p> </li> 
    </ul> <p>For information on requesting additional access for objects, see <a href="../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Request access to objects </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>-->

## 전제 조건

* Workfront 관리자 또는 사용자 정의 양식에 대한 관리 액세스 권한이 있는 계획 사용자는 사용자 환경에서 사용자 정의 양식을 만들어야 합니다. 자세한 내용은 [사용자 정의 양식 만들기](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/form-designer/design-a-form/design-a-form.md)를 참조하십시오.
* 오브젝트에 사용자 정의 양식을 첨부해야 합니다.

  개체에 사용자 정의 양식을 적용하는 방법에 대한 자세한 내용은 [개체에 사용자 정의 양식 추가](../../workfront-basics/work-with-custom-forms/add-a-custom-form-to-an-object.md)를 참조하십시오.

## 사용자 정의 양식의 정보 편집

오브젝트에 첨부된 사용자 정의 양식에 대한 정보를 편집하는 것은 대부분의 오브젝트에서 유사합니다.

사용자 정의 양식을 사용할 수 있는 개체에 대한 자세한 내용은 [사용자 정의 양식 개요](../../administration-and-setup/customize-workfront/create-manage-custom-forms/custom-forms-overview.md)를 참조하십시오.

1. 이터레이션 목록을 제외하고 사용자 정의 양식에 대한 정보를 편집할 객체 목록으로 이동합니다.
1. 목록에서 하나 이상의 개체를 선택한 다음 목록 맨 위에 있는 **편집** 아이콘 ![편집 아이콘](assets/edit-icon.png)을 클릭합니다.
1. **편집 &lt; 개체 >** 상자 안의 왼쪽 패널에서 **사용자 지정 Forms**&#x200B;을 클릭합니다.

   개체에 사용자 지정 양식이 첨부된 경우 양식 이름이 **사용자 지정 Forms** 섹션에 영역으로 표시됩니다.
1. 액세스 권한이 있는 모든 필드에 정보를 입력하십시오.

   ![청구 기록에 사용자 정의 양식이 있는 편집 상자](assets/edit-box-with-custom-forms-on-billing-record.png)

   여러 사용자 정의 양식이 오브젝트에 첨부된 경우 모든 양식에 대해 이 작업을 수행합니다.

   작업 중인 필드 유형에 따라 다음 사항을 고려하십시오.

   * 라디오 단추 필드에 대해 하나의 옵션만 선택할 수 있습니다.
   * 양식 작성자가 필드를 구성한 방식에 따라 확인란 필드에서 옵션을 하나 이상 선택할 수 있습니다.
   * 양식 작성자가 필드를 구성한 방식에 따라 다중 선택 드롭다운 필드에서 하나 또는 여러 옵션을 선택할 수 있습니다.
   * 양식을 만든 사용자가 텍스트 필드를 서식 필드 유형이 있는 텍스트 필드로 설정한 경우에만 텍스트 필드에 서식을 지정(굵게, 기울임꼴 또는 밑줄)할 수 있습니다. 한 줄 텍스트 필드와 단락 텍스트 필드의 서식을 지정할 수 없습니다.
   * 필드를 만들 때 양식을 만든 사용자가 포함시킨 경우에만 날짜 필드 유형에서 하루 중 시간을 업데이트할 수 있습니다.

   >[!NOTE]
   >
   >여러 항목을 선택할 수 있는 필드에는 선택할 수 있는 옵션 수가 제한될 수 있습니다. 확인란 및 다중 선택 드롭다운은 5000개 선택으로 제한됩니다.

   모든 필드 형식에 대한 자세한 내용은 [사용자 지정 양식 만들기](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/form-designer/design-a-form/design-a-form.md)를 참조하십시오.

1. **저장**&#x200B;을 클릭합니다.

   >[!IMPORTANT]
   >
   >양식을 저장하려면 먼저 양식의 모든 필수 필드를 작성해야 합니다. 필수 필드의 이름 뒤에 별표가 붙습니다.
   >
   >![](assets/nwe-required-custom-field.png)

   다른 사용자가 오브젝트의 계산된 사용자 정의 필드에서 참조하는 다른 오브젝트의 데이터를 변경할 때 변경 사항이 오브젝트에 자동으로 반영되지 않습니다. 개체의 모든 계산된 사용자 지정 필드를 수동으로 업데이트하는 방법에 대한 자세한 내용은 이 문서에서 [개체에 대한 모든 계산된 사용자 지정 필드 다시 계산](#recalculate-all-calculated-custom-fields-for-an-object)을 참조하십시오.

   페이지의 종속 필드가 수정되면 사용자 정의 양식의 계산된 필드가 실시간으로 동적으로 다시 계산됩니다. 양식을 저장하지 않고 새 계산된 필드 값을 볼 수 있지만 변경 사항을 저장할 때까지 실제로 양식 및 개체에 적용되지 않습니다. 이는 기본 양식의 계산된 필드와 사용자 정의 양식에 적용됩니다.

   목록의 다른 오브젝트와 함께 오브젝트를 일괄 편집할 때 오브젝트에 대한 모든 계산된 사용자 정의 필드를 수동으로 업데이트할 수도 있습니다. 자세한 내용은 이 문서에서 [개체를 편집할 때 목록의 여러 개체에 대해 계산된 사용자 지정 필드 모두 다시 계산](#recalculate-all-calculated-custom-fields-for-multiple-objects-in-a-list-when-editing-the-objects)을 참조하십시오.

1. (조건부) 반복 사용자 정의 양식에 대한 사용자 정의 필드를 업데이트하려면 다음 작업을 수행하십시오.

   1. 반복으로 이동합니다.
   1. 왼쪽 패널에서 **사용자 지정 Forms**&#x200B;을 클릭합니다.
   1. 사용자 정의 양식을 추가하려면 페이지의 오른쪽 상단에 있는 **사용자 정의 양식 추가** 필드에 양식 이름을 입력하십시오

      또는

      첨부된 양식의 필드 편집을 시작하려면 동일한 영역에서 **편집** 아이콘을 클릭하십시오.

      ![반복 사용자 정의 양식 편집](assets/edit-iteration-custom-form.png)

   1. **변경 내용 저장**&#x200B;을 클릭합니다.

## 오브젝트에 대한 사용자 정의 필드 다시 계산

사용자 정의 양식에 발생할 수 있는 변경 사항이나 사용자 정의 필드에서 참조되는 필드에 발생하는 변경 사항에 따라 정기적으로 계산된 사용자 정의 필드의 값이 오래된 것일 수 있습니다. 이 경우 사용자 정의 필드를 다시 계산하거나 객체에 대한 사용자 정의 표현식을 다시 계산해야 할 수 있습니다.

다음 섹션에서는 사용자 정의 양식이 있는 객체에 대한 사용자 정의 표현식을 다시 계산하는 방법을 설명합니다.

>[!NOTE]
>
>그룹에 대한 사용자 정의 표현식을 다시 계산할 수 없습니다.

### 오브젝트의 페이지에서 계산된 모든 사용자 정의 필드 다시 계산

>[!IMPORTANT]
>
>이 섹션의 단계를 따르려면 계산된 필드가 오브젝트에 첨부된 사용자 정의 양식이 있어야 합니다.

1. 사용자 정의 필드를 다시 계산하려는 다음 개체 중 하나의 기본 페이지로 이동합니다.

   * 프로젝트
   * 작업
   * 문제
   * 포트폴리오
   * 프로그램
   * 문서

1. 개체 이름의 오른쪽에 있는 **자세히** 메뉴 ![](assets/more-icon.png)을(를) 클릭한 다음 **표현식 다시 계산**&#x200B;을 클릭합니다.

   이렇게 하면 오브젝트 양식의 모든 사용자 정의 필드가 다시 계산됩니다.

### 객체를 편집할 때 목록의 여러 객체에 대해 계산된 모든 사용자 정의 필드 다시 계산 {#recalculate-all-calculated-custom-fields-for-multiple-objects-in-a-list-when-editing-the-objects}

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: this will need to be edited when the bulk edit for objects update in NW)</p>
-->

사용자 정의 표현식을 다시 계산하려는 객체에 따라 다음 영역에서 다시 계산할 수 있습니다.

* 개체 목록의 맨 위에 있는 기타 메뉴에서
* 편집 상자에서 여러 객체를 일괄적으로 선택하고 편집할 때

목록 또는 보고서에서 여러 객체의 사용자 정의 필드를 일괄적으로 편집하여 수동으로 다시 계산하려면 다음을 수행합니다.

1. 계산된 필드가 있는 사용자 정의 양식을 포함하는 객체에 대한 다음 객체 유형 목록으로 이동합니다.

   * 사용자
   * 회사
   * 청구 기록

1. 계산된 사용자 정의 필드를 업데이트할 오브젝트를 선택합니다.
1. **편집 아이콘**&#x200B;을 클릭합니다.
1. 왼쪽 메뉴에서 **사용자 지정 Forms**&#x200B;을 클릭한 다음 **사용자 지정 표현식 다시 계산**&#x200B;을 선택합니다.
1. **저장** 또는 **변경 내용 저장**&#x200B;을 클릭합니다.

   Workfront은 선택한 모든 객체에 대한 모든 사용자 정의 필드를 계산합니다.

객체 목록에서 사용자 정의 표현식을 다시 계산하려면 다음과 같이 하십시오.

1. 프로젝트 목록 또는 보고서로 이동하고 다음 객체 유형 중 하나 또는 일부를 선택합니다.

   * 프로젝트
   * 작업
   * 문제
   * 포트폴리오
   * 프로그램
   * 경비
1. **자세히** 메뉴 ![](assets/more-icon.png)을(를) 클릭한 다음 **사용자 지정 표현식 다시 계산**&#x200B;을 클릭합니다.

![](assets/recalculate-expressions-timeline-finances-drop-down-in-project-list-nwe.png)

Workfront은 선택한 모든 프로젝트에 대해 모든 사용자 정의 필드를 즉시 계산합니다.
모든 객체 목록에 이 기능이 있는 것은 아닙니다.

>[!NOTE]
>
>여러 프로젝트에 대한 표현식을 다시 계산할 때 복잡성에 따라 최적의 성능을 보장하기 위해 너무 많은 프로젝트를 선택하지 않는 것이 좋습니다.
>
>프로젝트를 너무 복잡하게 만들 수 있는 몇 가지 사항은 여러 종속성 또는 할당이거나 사용자 정의 필드의 수가 많을 수 있습니다.

