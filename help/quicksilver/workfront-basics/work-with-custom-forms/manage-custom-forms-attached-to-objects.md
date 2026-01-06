---
product-area: projects;user-management
navigation-topic: work-with-custom-forms
title: 오브젝트에 첨부된 사용자 정의 양식 관리
description: 한 오브젝트에 첨부된 사용자 정의 양식의 표시 순서를 업데이트하거나 제거하거나 여러 오브젝트에 사용자 정의 양식이 표시되는 방식을 벌크 편집할 수 있습니다.
author: Alina
feature: Get Started with Workfront
exl-id: e5570a09-32cb-43e3-9c1d-4421db42fa24
source-git-commit: dbc4404501e20b3f1905a5eebd13734a65db27ae
workflow-type: tm+mt
source-wordcount: '1054'
ht-degree: 2%

---

# 오브젝트에 첨부된 사용자 정의 양식 관리

<!--<span class="preview">The highlighted information on this page refers to functionality not yet generally available. It is available for all customers in the Preview environment and for a select group of customers in the Production environment.</span>-->

한 오브젝트에 첨부된 사용자 정의 양식의 표시 순서를 업데이트하거나 제거하거나 여러 오브젝트에 사용자 정의 양식이 표시되는 방식을 벌크 편집할 수 있습니다.

## 액세스 요구 사항

+++ 이 문서의 기능에 대한 액세스 요구 사항을 보려면 확장하십시오.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront 패키지</td> 
   <td> <p>임의 </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront 라이선스</td> 
   <td><p>기여자 이상</p> 
   <p>요청 이상</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">액세스 수준 구성</td> 
   <td> <p>사용자 정의 양식을 관리하는 객체에 대한 액세스 편집</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">개체 권한</td> 
   <td> <p>사용자 정의 양식을 관리하는 오브젝트에 권한 이상 부여</p>  </td> 
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
   <td role="rowheader">Adobe Workfront plan</td> 
   <td> <p>Any </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront license</td> 
   <td> <p>Request or higher</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Access level configurations</td> 
   <td> <p>Edit access to the objects for which you manage custom forms</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Object permissions</td> 
   <td> <p>Contribute permissions or higher to the objects for which you manage custom forms</p>  </td> 
  </tr> 
 </tbody> 
</table>-->

## 전제 조건

* Workfront 관리자 또는 사용자 정의 양식에 대한 관리 액세스 권한이 있는 계획 사용자는 사용자 환경에서 사용자 정의 양식을 만들어야 합니다. 자세한 내용은 [사용자 정의 양식 만들기](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/form-designer/design-a-form/design-a-form.md)를 참조하십시오.
* 오브젝트에 사용자 정의 양식을 첨부해야 합니다.

  개체에 사용자 정의 양식을 적용하는 방법에 대한 자세한 내용은 [개체에 사용자 정의 양식 추가](../../workfront-basics/work-with-custom-forms/add-a-custom-form-to-an-object.md)를 참조하십시오.

## 오브젝트에 첨부된 여러 사용자 정의 양식 순서 바꾸기 {#reorder-multiple-custom-forms-attached-to-an-object}

1. 추가된 사용자 정의 양식의 순서를 변경할 객체로 이동한 다음 객체 편집을 시작합니다.

   **예:** 예를 들어 프로젝트의 사용자 정의 양식을 관리하려면 프로젝트로 이동하여 **자세히** 메뉴 ![](assets/more-icon.png)을(를) 클릭한 다음 **편집** 을 클릭합니다.

1. 프로젝트, 작업 및 문제에 대한 **사용자 지정 Forms** 섹션에서 사용자 지정 양식 이름 옆에 있는 ![](assets/move-icon---dots.png) 아이콘을 클릭합니다. 다른 모든 개체에 대해 **Forms 관리**&#x200B;를 클릭합니다. 이 옵션은 객체에 하나 이상의 사용자 정의 양식이 첨부된 경우에만 표시됩니다.
1. ![](assets/move-icon---dots.png) 양식을 목록의 새 위치로 끕니다.
1. 프로젝트, 작업 및 문제 사용자 정의 양식의 경우 **저장**&#x200B;을 클릭하세요.

   다른 모든 개체에 대해 **관리 완료** > **변경 내용 저장**&#x200B;을 클릭합니다.

## 오브젝트에서 사용자 정의 양식 제거 {#remove-a-custom-form-from-an-object}

>[!IMPORTANT]
>
>객체에서 사용자 정의 양식을 제거하면 양식의 사용자 정의 필드에 캡처된 모든 정보가 손실되어 복구할 수 없습니다.

1. 사용자 정의 양식을 제거할 개체로 이동한 다음, 개체의 왼쪽 패널에서 **세부 정보** 섹션을 클릭합니다.

   예를 들어 프로젝트로 이동하여 **프로젝트 세부 정보** 섹션을 클릭합니다.

1. 개체 페이지의 오른쪽 상단에 있는 **편집** 아이콘 ![편집 아이콘](assets/edit-icon.png)을 클릭한 다음 **모두 편집**&#x200B;을 클릭합니다.
1. 사용자 정의 양식 이름의 오른쪽에 있는 **삭제** 아이콘 ![](assets/delete-icon.png)을(를) 클릭한 다음 **삭제**&#x200B;를 클릭하여 양식을 확인하고 개체에서 제거하거나 **취소**&#x200B;를 클릭하여 제거하지 마십시오.
1. **변경 내용 저장** 을 클릭합니다.

## 동일한 사용자 정의 필드를 포함하는 여러 사용자 정의 양식 관리

동일한 오브젝트에 첨부된 여러 사용자 정의 양식에 동일한 필드가 표시될 수 있습니다. 이 경우 다음 사항을 고려하십시오.

* 필드의 값은 모든 양식에서 동일합니다.

  동일한 오브젝트에 첨부된 다른 양식의 동일한 필드에 대해 다른 값을 가질 수 없습니다.

* 서로 다른 두 객체에 동일한 계산된 필드가 있는 경우, 오류를 방지하기 위해 계산이 동일해야 합니다. 여러 양식을 포함한 사용자 정의 양식에 계산된 필드를 추가하는 방법에 대한 자세한 내용은 [양식에 계산된 필드 추가](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/form-designer/design-a-form/add-a-calculated-field.md)를 참조하십시오.

## 오브젝트를 벌크 편집할 때 여러 사용자 정의 양식 관리

<!--
drafted for bulk-editing projects. When it releases to Prod for projects, take "in the preview environment" and the yellow tags out. Add additional objects here in the same way when they become available:-->

>[!NOTE]
>
>사용자 정의 양식을 객체로 관리하는 것은 프로젝트를 제외한 모든 객체에 대해 동일합니다.
>
>프로젝트에 사용자 정의 양식을 대량으로 추가하는 방법에 대한 자세한 내용은 문서 [프로젝트 편집](../../manage-work/projects/manage-projects/edit-projects.md)을 참조하십시오.

여러 사용자 정의 양식이 적용된 오브젝트를 벌크 편집할 때 해당 오브젝트에 사용자 정의 양식이 표시되는 방식을 편집하고 사용자 정의 양식 간의 공통 필드를 편집할 수 있습니다.

선택한 모든 개체에 첨부된 사용자 정의 양식만 벌크 편집에서 편집할 수 있습니다.

개체를 일괄 편집할 때 여러 사용자 정의 양식을 편집하려면 다음을 수행하십시오.

1. 목록 개체에서 사용자 정의 양식이 첨부된 개체를 선택한 다음 **편집** 아이콘 ![](assets/edit-icon.png)을(를) 클릭합니다.
1. **사용자 지정 Forms**&#x200B;을 클릭합니다.

   선택한 모든 개체에 첨부된 사용자 정의 양식만 편집할 수 있습니다.

   일부 객체에만 첨부된 사용자 정의 양식은 표시되지 않습니다.

1. 사용자 정의 양식의 필드 편집을 시작합니다.

   필드를 편집할 때 필드가 편집되었음을 나타내는 시각적 표시기가 필드에 표시됩니다.

   필드가 두 개 이상의 사용자 정의 양식에 포함된 경우, 양식 중 하나에서 필드를 업데이트할 때 해당 필드의 모든 값이 각 양식에서 업데이트됩니다.

1. **선택** 드롭다운 메뉴를 클릭하고 선택한 모든 개체에 추가할 다른 양식을 선택하십시오.

   추가 양식을 적용할 때는 다음 사항을 고려하십시오.

   * 오브젝트에는 최대 10개의 사용자 정의 양식이 포함될 수 있습니다.
   * 편집 중인 오브젝트에 양식이 아직 적용되지 않은 경우에만 양식을 적용할 수 있습니다. 개체 중 하나에 이미 첨부된 양식은 드롭다운 메뉴에 나타나지 않습니다.
   * 추가 양식을 적용하면 양식에 다른 양식과 공통되는 모든 필드가 **공통 필드** 섹션에 표시되고 편집할 수 있습니다.

1. (선택 사항) 모든 오브젝트에 사용자 정의 양식을 추가했지만 아직 오브젝트를 저장하지 않은 경우 사용자 정의 양식이 오브젝트에 표시되는 순서를 변경할 수 있습니다.

   양식 순서 변경에 대한 자세한 내용은 이 문서에서 [개체에 첨부된 여러 사용자 정의 양식 순서 바꾸기](#reorder-multiple-custom-forms-attached-to-an-object)를 참조하십시오.

1. 개체에서 사용자 정의 양식을 제거하려면 **양식 제거**&#x200B;를 클릭하십시오.

   개체에서 사용자 정의 양식을 제거하는 방법에 대한 자세한 내용은 [개체에서 사용자 정의 양식 제거](#remove-a-custom-form-from-an-object)를 참조하십시오.

   여러 개체에서 양식을 대량으로 제거할 때에는 다음 사항을 고려하십시오.

   * 양식을 변경한 경우 이를 제거하면 변경 사항이 손실되어 복구할 수 없습니다.
   * 양식을 제거한 후 해당 양식의 **공통 필드** 섹션에 있는 모든 필드가 이 섹션에서 제거되며 더 이상 여기에서 편집할 수 없습니다.

1. **양식 복원**&#x200B;을 클릭하여 양식을 개체를 편집하기 전의 상태로 복원합니다.
1. (선택 사항) 한 번에 하나의 양식을 축소하려면 양식 이름 옆에 있는 축소 화살표를 클릭합니다.

   또는

   동시에 모든 양식을 축소하려면 **Forms 축소**&#x200B;를 클릭하십시오.

1. (선택 사항) 양식 이름 옆에 있는 확장 화살표를 클릭하여 한 번에 하나의 양식을 확장합니다.

   또는

   모든 양식을 동시에 확장하려면 **Forms 확장**&#x200B;을 클릭하십시오.

1. **변경 내용 저장**&#x200B;을 클릭합니다.
