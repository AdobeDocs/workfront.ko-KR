---
product-area: projects;user-management
keywords: 편집,양식,서식,텍스트,특수,형식,필드,사용자 지정,정보,사용자 지정,개체
navigation-topic: work-with-custom-forms
title: 사용자 지정 양식 필드에서 정보 편집
description: 양식이 개체에 첨부된 후에 사용자 지정 양식에 대한 정보를 편집할 수 있습니다. 개체에 사용자 지정 양식을 추가하는 방법에 대한 자세한 내용은 개체에 사용자 지정 양식 추가 를 참조하십시오.
author: Alina
feature: Get Started with Workfront
exl-id: c2b6afde-91a8-4e17-8e1a-3428b48e500a
source-git-commit: 6580fec18982215dbc2535d5f2ab159fc32ac3f5
workflow-type: tm+mt
source-wordcount: '982'
ht-degree: 0%

---

# 사용자 지정 양식 필드에서 정보 편집

양식이 개체에 첨부된 후에 사용자 지정 양식에 대한 정보를 편집할 수 있습니다. 개체에 사용자 지정 양식 추가에 대한 자세한 내용은 [개체에 사용자 지정 양식 추가](../../workfront-basics/work-with-custom-forms/add-a-custom-form-to-an-object.md).

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
   <td role="rowheader"> <p>Adobe Workfront 라이선스*</p> </td> 
   <td> <p>요청 이상</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader">액세스 수준*</td> 
   <td> <p>사용자 지정 양식을 편집할 개체에 대한 액세스 편집</p> <p>참고: 여전히 액세스 권한이 없는 경우 Workfront 관리자에게 액세스 수준에서 추가 제한 사항을 설정하는지 문의하십시오. Workfront 관리자가 액세스 수준을 변경하는 방법에 대한 자세한 내용은 <a href="../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">사용자 정의 액세스 수준 만들기 또는 수정</a>.</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader"> <p>개체 권한</p> </td> 
   <td> 
    <ul> 
     <li> <p>사용자 지정 양식을 편집할 개체에 대한 Contribute 이상의 권한</p> </li> 
     <li>편집할 필드에 대한 권한을 봅니다. 사용자 지정 필드에 대한 권한 공유에 대한 자세한 내용은 <a href="../../administration-and-setup/customize-workfront/create-manage-custom-forms/configure-sharing-for-a-custom-field.md" class="MCXref xref">사용자 지정 필드 및 위젯에 대한 공유 구성</a>.</li> 
     <li> <p>편집할 필드가 있는 양식의 섹션에 대한 권한 편집</p> </li> 
    </ul> <p>객체에 대한 추가 액세스 요청에 대한 내용은 <a href="../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">개체에 대한 액세스 요청 </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;어떤 계획, 라이선스 유형 또는 액세스 권한을 보유하고 있는지 알아보려면 Workfront 관리자에게 문의하십시오.

## 전제 조건

* Workfront 관리자나 사용자 지정 양식에 대한 관리자 액세스 권한이 있는 계획 사용자는 해당 환경에서 사용자 지정 양식을 만들어야 합니다. 자세한 내용은 [사용자 지정 양식 만들기 또는 편집](../../administration-and-setup/customize-workfront/create-manage-custom-forms/create-or-edit-a-custom-form.md).
* 개체에 사용자 지정 양식이 연결되어 있어야 합니다.

   개체에 사용자 지정 양식을 적용하는 방법에 대한 자세한 내용은 [개체에 사용자 지정 양식 추가](../../workfront-basics/work-with-custom-forms/add-a-custom-form-to-an-object.md).

## 사용자 지정 양식에서 정보 편집

개체에 첨부된 사용자 지정 양식에 대한 정보 편집은 모든 개체에 대해 동일합니다. 사용자 지정 양식을 가질 수 있는 객체에 대한 자세한 내용은 [사용자 지정 양식 개요](../../administration-and-setup/customize-workfront/create-manage-custom-forms/custom-forms-overview.md).

1. 사용자 지정 양식의 정보를 편집할 개체로 이동합니다.
1. 클릭 **`<Object type>`세부 사항** 왼쪽 패널에 표시됩니다.

   예를 들어 프로젝트 사용자 지정 양식에 대한 정보를 편집할 때 **프로젝트 세부 사항**.

1. 사용자 지정 양식으로 스크롤합니다. 객체에 첨부된 사용자 지정 양식이 있으면 양식의 이름이 세부 정보 섹션에 영역으로 표시됩니다.
1. 필요한 경우 화살표를 클릭합니다 ![](assets/expand-arrow-right.png) 사용자 지정 양식 이름의 왼쪽에 추가하여 확장하십시오.
1. 페이지의 오른쪽 위 모서리 근처에 있는 편집 아이콘을 클릭합니다 ![](assets/edit-icon.png).
1. 액세스 권한이 있는 필드에 정보를 입력합니다.

   ![](assets/click-in-field-to-edit-info-350x132.png)

   또는

   양식에 아직 정보를 입력하지 않은 경우 **추가+** 모든 필드에 대해 액세스 권한이 있고 정보 입력을 시작합니다.

   ![](assets/plus-add-to-edit-info-350x180.png)

   여러 사용자 지정 양식이 개체에 첨부된 경우 모든 양식에 대해 이 작업을 수행할 수 있습니다.

   작업 중인 필드 유형에 따라 다음 사항을 고려하십시오.

   * 라디오 단추 필드에 대해 옵션을 하나만 선택할 수 있습니다.
   * 양식 작성자가 필드를 구성한 방법에 따라 확인란 필드에서 하나 이상의 옵션을 선택할 수 있습니다.
   * 양식 작성자가 필드를 구성한 방법에 따라 다중 선택 드롭다운 필드에서 하나 이상의 옵션을 선택할 수 있습니다.
   * 양식을 만든 사용자가 서식 필드 유형을 사용하는 텍스트 필드로 설정한 경우에만 텍스트 필드(굵게, 기울임체 또는 밑줄)의 서식을 지정할 수 있습니다. 단일 행 텍스트 필드 및 단락 텍스트 필드의 형식은 지정할 수 없습니다.
   * 날짜 필드 유형에서는 양식을 만든 사용자가 필드를 만들 때 포함하는 경우에만 시간을 업데이트할 수 있습니다.

   모든 필드 유형에 대한 자세한 내용은 [사용자 지정 양식 만들기 또는 편집](../../administration-and-setup/customize-workfront/create-manage-custom-forms/create-or-edit-a-custom-form.md).

1. 클릭 **저장** 변경 사항.

   >[!IMPORTANT]
   >
   >
   >
   ><!--   >
   ><p style="color: #ff1493;" data-mc-conditions="QuicksilverOrClassic.Draft mode">This is true in "Edit custom forms" but not in "Add a custom form to an object." This snippet is used in both articles. The whole snippet is conditioned for classic only in "Add" but not in "Edit." Don't remove the NWE conditioning in the snippet because it is needed in "Edit."</p>   >
   >-->   >
   >
   >양식을 저장하려면 먼저 양식의 모든 필수 필드를 완료해야 합니다. 필수 필드의 이름 뒤에는 별표가 표시됩니다.
   ![](assets/nwe-required-custom-field.png)   >

   어떤 사용자가 개체의 계산된 사용자 지정 필드에서 참조하는 다른 개체의 데이터를 변경하면 변경 내용이 개체에 자동으로 반영되지 않습니다. 개체에서 계산된 모든 사용자 지정 필드를 수동으로 업데이트하는 방법에 대한 자세한 내용은 [개체의 계산된 사용자 지정 필드를 모두 다시 계산합니다](#recalculate-all-calculated-custom-fields-for-an-object) 참조하십시오.

   개체의 계산된 사용자 정의 필드를 목록에 있는 다른 개체와 함께 벌크 편집할 때 개체에 대해 수동으로 모두 업데이트할 수도 있습니다. 자세한 내용은 [개체를 편집할 때 목록의 여러 개체에 대해 계산된 사용자 지정 필드를 모두 다시 계산합니다](#recalculate-all-calculated-custom-fields-for-multiple-objects-in-a-list-when-editing-the-objects) 참조하십시오.

## 개체의 계산된 사용자 지정 필드를 모두 다시 계산합니다  {#recalculate-all-calculated-custom-fields-for-an-object}

1. 재계산할 사용자 지정 필드가 있는 개체의 기본 페이지로 이동합니다.
1. 을(를) 클릭합니다. **자세히** 메뉴 ![](assets/more-icon.png) 개체 이름의 오른쪽에 있는 **표현식 다시 계산**.

   이렇게 하면 개체의 양식에서 모든 사용자 지정 필드가 다시 계산됩니다.

## 개체를 편집할 때 목록의 여러 개체에 대해 계산된 사용자 지정 필드를 모두 다시 계산합니다 {#recalculate-all-calculated-custom-fields-for-multiple-objects-in-a-list-when-editing-the-objects}

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: this will need to be edited when the bulk edit for objects update in NW)</p>
-->

목록 또는 보고서에서 여러 객체의 사용자 정의 필드를 일괄적으로 편집하여 수동으로 다시 계산할 수 있습니다.

1. 계산된 필드가 있는 사용자 지정 양식이 포함된 개체 목록으로 이동합니다.
1. 계산된 사용자 지정 필드를 업데이트할 개체를 선택합니다.
1. 을(를) 클릭합니다. **편집 아이콘**.
1. 클릭 **사용자 지정 Forms** 왼쪽 메뉴에서 **사용자 지정 표현식 다시 계산**.
1. 클릭 **저장** **변경 사항**.

   Workfront은 선택한 모든 개체에 대해 모든 사용자 지정 필드를 계산합니다.

>[!TIP]
프로젝트의 복잡성에 따라 계산된 사용자 지정 필드를 일괄 계산하여 최적의 성능을 보장할 때 많은 수의 프로젝트를 선택하지 않는 것이 좋습니다. 프로젝트를 너무 복잡하게 만들 수 있는 몇 가지 사항은 여러 종속성 또는 할당 또는 많은 사용자 지정 필드일 수 있습니다.
프로젝트 목록에서 사용자 지정 표현식을 일괄적으로 재계산하려면
1. 프로젝트 목록 또는 보고서로 이동하고 하나 또는 여러 프로젝트를 선택합니다.
1. 을(를) 클릭합니다. **자세히** 메뉴 ![](assets/more-icon.png)를 클릭한 다음 **사용자 지정 표현식 다시 계산**.
![](assets/recalculate-expressions-timeline-finances-drop-down-in-project-list-nwe.png)
Workfront은 선택한 모든 프로젝트에 대한 모든 사용자 지정 필드를 계산합니다.
