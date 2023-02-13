---
product-area: projects;user-management
navigation-topic: work-with-custom-forms
title: 개체에 첨부된 사용자 지정 양식 관리
description: 한 개체에 첨부된 사용자 지정 양식이 표시되는 순서를 업데이트하거나, 제거하거나, 여러 개체에 사용자 지정 양식이 표시되는 방식을 대량 편집할 수 있습니다.
author: Alina
feature: Get Started with Workfront
exl-id: e5570a09-32cb-43e3-9c1d-4421db42fa24
source-git-commit: 6580fec18982215dbc2535d5f2ab159fc32ac3f5
workflow-type: tm+mt
source-wordcount: '1080'
ht-degree: 0%

---

# 개체에 첨부된 사용자 지정 양식 관리

한 개체에 첨부된 사용자 지정 양식이 표시되는 순서를 업데이트하거나, 제거하거나, 여러 개체에 사용자 지정 양식이 표시되는 방식을 대량 편집할 수 있습니다.

## 액세스 요구 사항

이 문서에 설명된 작업을 수행하려면 다음 액세스 권한이 있어야 합니다.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront 플랜*</td> 
   <td> <p>모든 </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront 라이선스*</td> 
   <td> <p>요청 이상</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">액세스 수준 구성*</td> 
   <td> <p>사용자 지정 양식을 관리하는 개체에 대한 액세스 편집</p> <p>참고: 여전히 액세스 권한이 없는 경우 Workfront 관리자에게 액세스 수준에서 추가 제한 사항을 설정하는지 문의하십시오. Workfront 관리자가 액세스 수준을 수정하는 방법에 대한 자세한 내용은 <a href="../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">사용자 정의 액세스 수준 만들기 또는 수정</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">개체 권한</td> 
   <td> <p>사용자 지정 양식을 관리하는 개체에 대한 사용 권한 이상을 제공합니다</p> <p>추가 액세스 요청에 대한 자세한 내용은 <a href="../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">개체에 대한 액세스 요청 </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;어떤 계획, 라이선스 유형 또는 액세스 권한을 보유하고 있는지 알아보려면 Workfront 관리자에게 문의하십시오.

## 전제 조건

* Workfront 관리자나 사용자 지정 양식에 대한 관리자 액세스 권한이 있는 계획 사용자는 해당 환경에서 사용자 지정 양식을 만들어야 합니다. 자세한 내용은 [사용자 지정 양식 만들기 또는 편집](../../administration-and-setup/customize-workfront/create-manage-custom-forms/create-or-edit-a-custom-form.md).
* 개체에 사용자 지정 양식이 연결되어 있어야 합니다.

   개체에 사용자 지정 양식을 적용하는 방법에 대한 자세한 내용은 [개체에 사용자 지정 양식 추가](../../workfront-basics/work-with-custom-forms/add-a-custom-form-to-an-object.md).

## 개체에 첨부된 여러 사용자 지정 양식 재정렬 {#reorder-multiple-custom-forms-attached-to-an-object}

1. 추가된 사용자 지정 양식의 순서를 변경할 개체로 이동한 다음 개체 편집을 시작합니다.

   **예:** 예를 들어 프로젝트의 사용자 지정 양식을 관리하려면 프로젝트로 이동하여 **자세히** 메뉴 ![](assets/more-icon.png)를 클릭한 다음 **편집** .

1. 에서 **사용자 지정 Forms** 프로젝트, 작업 및 문제에 대한 섹션에서 ![](assets/move-icon---dots.png) 사용자 지정 양식 이름 옆에 있는 아이콘을 클릭합니다. 다른 모든 객체의 경우 **Forms 관리**. 이 옵션은 개체에 하나 이상의 사용자 지정 양식이 첨부된 경우에만 표시됩니다.
1. 양식 드래그 ![](assets/move-icon---dots.png) 새 위치를 클릭합니다.
1. 프로젝트, 작업 및 문제 사용자 지정 양식의 경우 **저장**.

   다른 모든 객체의 경우 **난 이제 다 관리해** > **변경 내용 저장**.

## 개체에서 사용자 지정 양식 제거 {#remove-a-custom-form-from-an-object}

>[!IMPORTANT]
>
>개체에서 사용자 지정 양식을 제거하면 양식의 사용자 지정 필드에 캡처된 모든 정보가 손실되어 복구할 수 없습니다.

1. 사용자 지정 양식을 제거할 개체로 이동하고 개체 편집을 시작합니다.

   예를 들어 프로젝트로 이동하여 **자세히** 메뉴 ![](assets/more-icon.png)를 클릭한 다음 **편집** .

1. 클릭 **사용자 지정 Forms**.
1. 프로젝트, 작업 및 문제 사용자 지정 양식의 경우 **X** 폼의 오른쪽에 있는 아이콘을 사용하여 개체에서 제거할 수 있습니다.

   다른 모든 객체의 경우 **Forms 관리**&#x200B;를 클릭한 다음 **X** 폼의 오른쪽에 있는 아이콘을 사용하여 개체에서 제거할 수 있습니다.

1. **저장**&#x200B;을 클릭합니다 .

## 동일한 사용자 지정 필드를 포함하는 여러 사용자 지정 양식을 관리합니다

동일한 개체에 첨부된 여러 사용자 지정 양식에 동일한 필드가 표시될 수 있습니다. 이 경우 다음 사항을 고려하십시오.

* 필드의 값은 모든 양식에서 동일합니다.

   같은 객체에 첨부된 다른 양식에서 동일한 필드에 대해 다른 값을 가질 수 없습니다.

* 두 개의 서로 다른 개체에 동일한 계산된 필드가 있는 경우 해당 계산은 오류를 방지하기 위해 동일해야 합니다. 여러 양식을 포함하는 사용자 지정 양식에 계산된 필드를 추가하는 방법에 대한 내용은 [사용자 지정 양식에 계산된 데이터 추가](../../administration-and-setup/customize-workfront/create-manage-custom-forms/add-calculated-data-to-custom-form.md) .

## 개체를 벌크 편집할 때 여러 사용자 지정 양식 편집

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: this section will need to be edited when the bulk Edit box is released to NWE; add some screen shots for NWE) </p>
-->

여러 사용자 정의 양식이 적용된 개체를 벌크 편집하는 경우 사용자 정의 양식이 해당 개체에 표시되는 방식을 편집하고 사용자 정의 양식 간의 공통 필드를 편집할 수 있습니다.

선택한 모든 개체에 첨부된 사용자 지정 양식만 벌크 편집에서 편집할 수 있습니다.

개체를 벌크로 편집할 때 여러 사용자 지정 양식을 편집하려면 다음을 수행하십시오.

1. 목록 개체에서 사용자 지정 양식이 첨부된 개체를 선택한 다음 **편집** 아이콘 ![](assets/edit-icon.png).
1. 클릭 **사용자 지정 Forms**.

   선택한 모든 객체에 첨부된 사용자 정의 양식만 편집할 수 있습니다.

   일부 개체에만 첨부된 사용자 지정 양식이 표시되지 않습니다.

1. 사용자 지정 양식에서 필드 편집을 시작합니다.

   필드를 편집하면 필드에 필드가 편집되었음을 나타내는 시각적 표시기가 표시됩니다.

   필드가 두 개 이상의 사용자 지정 양식에 포함되어 있는 경우, 양식 중 하나에서 필드를 업데이트할 때 이러한 필드의 값이 모두 각 양식에서 업데이트됩니다.

1. 을(를) 클릭합니다. **선택** 드롭다운 메뉴를 클릭하고 선택한 모든 객체에 추가할 양식을 추가로 선택합니다.

   추가 양식을 적용할 때 다음 사항을 고려하십시오.

   * 개체에는 최대 10개의 사용자 지정 양식이 있을 수 있습니다.
   * 양식이 편집 중인 개체에 아직 적용되지 않은 경우에만 양식을 적용할 수 있습니다. 객체 중 하나에 이미 첨부된 양식은 드롭다운 메뉴에 나타나지 않습니다.
   * 추가 양식을 적용하면 양식에 다른 양식과 공통된 필드가 **공통 필드** 섹션을 편집하고 편집할 수 있습니다.

1. (선택 사항) 모든 객체에 사용자 정의 양식을 추가했지만 아직 객체를 저장하지 않은 경우 객체에 사용자 정의 양식이 표시되는 순서를 변경할 수 있습니다.

   양식 순서 변경에 대한 자세한 내용은 [개체에 첨부된 여러 사용자 지정 양식 재정렬](#reorder-multiple-custom-forms-attached-to-an-object) 참조하십시오.

1. 클릭 **양식 제거** 개체에서 사용자 지정 양식을 제거하려면

   개체에서 사용자 지정 양식을 제거하는 방법에 대한 자세한 내용은 [개체에서 사용자 지정 양식 제거](#remove-a-custom-form-from-an-object).

   여러 개체에서 양식을 일괄적으로 제거할 때는 다음 사항을 고려하십시오.

   * 양식을 변경한 경우 양식을 제거하면 변경 사항이 손실되어 복구할 수 없습니다.
   * 양식을 제거한 후에는 **공통 필드** 섹션은 이 섹션에서 제거되며 더 이상 여기에서 편집할 수 없습니다.

1. 클릭 **양식 복원** 양식을 객체를 편집하기 전의 상태로 복원하려면
1. (선택 사항) 한 번에 한 폼을 축소하려면 양식 이름 옆에 있는 축소 화살표를 클릭합니다.

   또는

   클릭 **Forms 축소** 모든 양식을 동시에 축소합니다.

1. (선택 사항) 한 번에 한 양식을 확장하려면 양식 이름 옆에 있는 확장 화살표를 클릭합니다.

   또는

   클릭 **Forms 확장** 모든 양식을 동시에 확장하려면 다음을 수행하십시오. 

1. 클릭 **변경 내용 저장**.
