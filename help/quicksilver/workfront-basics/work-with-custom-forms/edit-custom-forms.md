---
product-area: projects;user-management
keywords: 편집,양식,리치,텍스트,특수,서식,필드,사용자 지정,정보,사용자 지정,개체
navigation-topic: work-with-custom-forms
title: 사용자 정의 양식 필드의 정보 편집
description: 양식을 오브젝트에 첨부한 후 사용자 정의 양식에 대한 정보를 편집할 수 있습니다. 오브젝트에 사용자 정의 양식을 추가하는 방법에 대한 자세한 내용은 오브젝트에 사용자 정의 양식 추가를 참조하십시오.
author: Alina
feature: Get Started with Workfront
exl-id: c2b6afde-91a8-4e17-8e1a-3428b48e500a
source-git-commit: 456310e460bae44183de390efc4be919fda3f36d
workflow-type: tm+mt
source-wordcount: '1034'
ht-degree: 0%

---

# 사용자 정의 양식 필드의 정보 편집

양식을 오브젝트에 첨부한 후 사용자 정의 양식에 대한 정보를 편집할 수 있습니다. 개체에 사용자 정의 양식을 추가하는 방법에 대한 자세한 내용은 [개체에 사용자 정의 양식 추가](../../workfront-basics/work-with-custom-forms/add-a-custom-form-to-an-object.md)를 참조하십시오.

## 액세스 요구 사항

다음 항목이 있어야 합니다.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <p>Adobe Workfront 플랜*</p> </td> 
   <td>팀 이상</td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>Adobe Workfront 라이센스*</p> </td> 
   <td> <p>요청 이상</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader">액세스 수준*</td> 
   <td> <p>사용자 정의 양식을 편집할 객체에 대한 액세스 편집</p> <p>참고: 여전히 액세스 권한이 없는 경우 Workfront 관리자에게 액세스 수준에서 추가 제한을 설정하는지 문의하십시오. Workfront 관리자가 액세스 수준을 변경하는 방법에 대한 자세한 내용은 <a href="../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">사용자 지정 액세스 수준 만들기 또는 수정</a>을 참조하십시오.</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader"> <p>개체 권한</p> </td> 
   <td> 
    <ul> 
     <li> <p>사용자 정의 양식을 편집할 객체에 대한 Contribute 이상의 권한</p> </li> 
     <li>편집할 필드에 대한 권한을 봅니다. 사용자 정의 필드에 대한 공유 권한에 대한 자세한 내용은 <a href="../../administration-and-setup/customize-workfront/create-manage-custom-forms/configure-sharing-for-a-custom-field.md" class="MCXref xref">사용자 정의 필드 및 위젯에 대한 공유 구성</a>을 참조하십시오.</li> 
     <li> <p>편집할 필드가 있는 양식의 섹션에 대한 권한 편집</p> </li> 
    </ul> <p>개체에 대한 추가 액세스 요청에 대한 자세한 내용은 <a href="../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">개체에 대한 액세스 요청 </a>을(를) 참조하십시오.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;보유 중인 플랜, 라이선스 유형 또는 액세스 권한을 확인하려면 Workfront 관리자에게 문의하십시오.

## 전제 조건

* Workfront 관리자 또는 사용자 정의 양식에 대한 관리 액세스 권한이 있는 계획 사용자는 사용자 환경에서 사용자 정의 양식을 만들어야 합니다. 자세한 내용은 [사용자 정의 양식 만들기 또는 편집](../../administration-and-setup/customize-workfront/create-manage-custom-forms/create-or-edit-a-custom-form.md)을 참조하세요.
* 오브젝트에 사용자 정의 양식을 첨부해야 합니다.

  개체에 사용자 정의 양식을 적용하는 방법에 대한 자세한 내용은 [개체에 사용자 정의 양식 추가](../../workfront-basics/work-with-custom-forms/add-a-custom-form-to-an-object.md)를 참조하십시오.

## 사용자 정의 양식의 정보 편집

오브젝트에 첨부된 사용자 정의 양식에 대한 정보를 편집하는 것은 모든 오브젝트에 대해 동일합니다. 사용자 정의 양식을 사용할 수 있는 개체에 대한 자세한 내용은 [사용자 정의 양식 개요](../../administration-and-setup/customize-workfront/create-manage-custom-forms/custom-forms-overview.md)를 참조하십시오.

1. 사용자 정의 양식의 정보를 편집할 객체로 이동합니다.
1. 왼쪽 패널에서 **`<Object type>`세부 정보**&#x200B;을(를) 클릭합니다.

   예를 들어 프로젝트 사용자 정의 양식의 정보를 편집할 때 **프로젝트 세부 정보**&#x200B;를 클릭합니다.

1. 사용자 정의 양식으로 스크롤합니다. 오브젝트에 사용자 정의 양식이 첨부되어 있는 경우 양식 이름이 세부 정보 섹션에 영역으로 표시됩니다.
1. 필요한 경우 사용자 정의 양식 이름 왼쪽에 있는 ![](assets/expand-arrow-right.png) 화살표를 클릭하여 확장합니다.
1. 페이지의 오른쪽 상단 모서리에서 편집 아이콘 ![](assets/edit-icon.png)을(를) 클릭합니다.
1. 액세스 권한이 있는 모든 필드에 정보를 입력하십시오.

   ![](assets/click-in-field-to-edit-info-350x132.png)

   또는

   양식에 정보를 입력하지 않은 경우 액세스 권한이 있는 모든 필드에 대해 **추가+**&#x200B;를 클릭하고 정보 입력을 시작합니다.

   ![](assets/plus-add-to-edit-info-350x180.png)

   여러 사용자 정의 양식이 오브젝트에 첨부된 경우 모든 양식에 대해 이 작업을 수행할 수 있습니다.

   작업 중인 필드 유형에 따라 다음 사항을 고려하십시오.

   * 라디오 단추 필드에 대해 하나의 옵션만 선택할 수 있습니다.
   * 양식 작성자가 필드를 구성한 방식에 따라 확인란 필드에서 옵션을 하나 이상 선택할 수 있습니다.
   * 양식 작성자가 필드를 구성한 방식에 따라 다중 선택 드롭다운 필드에서 하나 또는 여러 옵션을 선택할 수 있습니다.
   * 양식을 만든 사용자가 텍스트 필드를 서식 필드 유형이 있는 텍스트 필드로 설정한 경우에만 텍스트 필드에 서식을 지정(굵게, 기울임꼴 또는 밑줄)할 수 있습니다. 한 줄 텍스트 필드와 단락 텍스트 필드의 서식을 지정할 수 없습니다.
   * 필드를 만들 때 양식을 만든 사용자가 포함시킨 경우에만 날짜 필드 유형에서 하루 중 시간을 업데이트할 수 있습니다.

   모든 필드 형식에 대한 자세한 내용은 [사용자 지정 양식 만들기 또는 편집](../../administration-and-setup/customize-workfront/create-manage-custom-forms/create-or-edit-a-custom-form.md)을 참조하세요.

1. **변경 내용 저장**&#x200B;을 클릭합니다.

   >[!IMPORTANT]
   >
   >양식을 저장하려면 먼저 양식의 모든 필수 필드를 작성해야 합니다. 필수 필드의 이름 뒤에 별표가 붙습니다.
   >
   >![](assets/nwe-required-custom-field.png)

   다른 사용자가 오브젝트의 계산된 사용자 정의 필드에서 참조하는 다른 오브젝트의 데이터를 변경할 때 변경 사항이 오브젝트에 자동으로 반영되지 않습니다. 개체의 모든 계산된 사용자 지정 필드를 수동으로 업데이트하는 방법에 대한 자세한 내용은 이 문서에서 [개체에 대한 모든 계산된 사용자 지정 필드 다시 계산](#recalculate-all-calculated-custom-fields-for-an-object)을 참조하십시오.

   페이지의 종속 필드가 수정되면 사용자 정의 양식의 계산된 필드가 실시간으로 동적으로 다시 계산됩니다. 양식을 저장하지 않고 새 계산된 필드 값을 볼 수 있지만 변경 사항을 저장할 때까지 실제로 양식 및 개체에 적용되지 않습니다. 이는 기본 양식의 계산된 필드와 사용자 정의 양식에 적용됩니다.

   목록의 다른 오브젝트와 함께 오브젝트를 일괄 편집할 때 오브젝트에 대한 모든 계산된 사용자 정의 필드를 수동으로 업데이트할 수도 있습니다. 자세한 내용은 이 문서에서 [개체를 편집할 때 목록의 여러 개체에 대해 계산된 사용자 지정 필드 모두 다시 계산](#recalculate-all-calculated-custom-fields-for-multiple-objects-in-a-list-when-editing-the-objects)을 참조하십시오.

## 오브젝트에 대해 계산된 모든 사용자 정의 필드 다시 계산  {#recalculate-all-calculated-custom-fields-for-an-object}

1. 사용자 정의 필드를 다시 계산하려는 오브젝트의 기본 페이지로 이동합니다.
1. 개체 이름의 오른쪽에 있는 **자세히** 메뉴 ![](assets/more-icon.png)을(를) 클릭한 다음 **표현식 다시 계산**&#x200B;을 클릭합니다.

   이렇게 하면 오브젝트 양식의 모든 사용자 정의 필드가 다시 계산됩니다.

## 객체를 편집할 때 목록의 여러 객체에 대해 계산된 모든 사용자 정의 필드 다시 계산 {#recalculate-all-calculated-custom-fields-for-multiple-objects-in-a-list-when-editing-the-objects}

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: this will need to be edited when the bulk edit for objects update in NW)</p>
-->

목록 또는 보고서에서 여러 객체의 사용자 정의 필드를 일괄적으로 편집하여 수동으로 다시 계산할 수 있습니다.

1. 계산된 필드가 있는 사용자 정의 양식이 포함된 개체 목록으로 이동합니다.
1. 계산된 사용자 정의 필드를 업데이트할 오브젝트를 선택합니다.
1. **편집 아이콘**&#x200B;을 클릭합니다.
1. 왼쪽 메뉴에서 **사용자 지정 Forms**&#x200B;을 클릭한 다음 **사용자 지정 표현식 다시 계산**&#x200B;을 선택합니다.
1. **저장** **변경 내용**&#x200B;을 클릭합니다.

   Workfront은 선택한 모든 객체에 대한 모든 사용자 정의 필드를 계산합니다.

>[!TIP]
>
>프로젝트의 복잡성에 따라 최적의 성능을 보장하기 위해 계산된 사용자 정의 필드를 일괄로 다시 계산할 때 많은 수의 프로젝트를 선택하지 않는 것이 좋습니다. 프로젝트를 너무 복잡하게 만들 수 있는 몇 가지 사항은 여러 종속성 또는 할당이거나 사용자 정의 필드의 수가 많을 수 있습니다.
>
>프로젝트 목록에서 사용자 정의 표현식을 일괄적으로 재계산하려면
>
>1. 프로젝트 목록 또는 보고서로 이동하고 하나 또는 여러 프로젝트를 선택합니다.
>1. **자세히** 메뉴 ![](assets/more-icon.png)을(를) 클릭한 다음 **사용자 지정 표현식 다시 계산**&#x200B;을 클릭합니다.
>
>![](assets/recalculate-expressions-timeline-finances-drop-down-in-project-list-nwe.png)
>
>Workfront은 선택한 모든 프로젝트에 대해 모든 사용자 지정 필드를 계산합니다.
