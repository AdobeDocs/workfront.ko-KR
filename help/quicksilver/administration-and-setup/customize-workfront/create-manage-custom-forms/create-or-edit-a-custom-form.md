---
title: 기존 양식 빌더로 사용자 정의 양식 만들기 또는 편집
user-type: administrator
product-area: system-administration
navigation-topic: create-and-manage-custom-forms
description: 새 사용자 정의 양식을 만들거나 편집할 수 있습니다.
author: Lisa
feature: System Setup and Administration, Custom Forms
role: Admin
exl-id: 5712e82d-bd1d-4d8a-9a2a-1e19b562b9d1
source-git-commit: ccb2b6bb9fa63d29523ff396490f9580ad130bdd
workflow-type: tm+mt
source-wordcount: '956'
ht-degree: 0%

---

# 기존 양식 빌더로 사용자 정의 양식 만들기 또는 편집

<!--Audited: 01/2024-->

<span class="preview">이 페이지에서 강조 표시된 정보는 아직 일반적으로 사용할 수 없는 기능을 참조합니다. 모든 고객의 미리보기 환경 또는 빠른 릴리스를 활성화한 고객의 프로덕션 환경에서만 사용할 수 있습니다.</span>

<span class="preview">빠른 릴리스에 대한 자세한 내용은 [조직의 빠른 릴리스 활성화 또는 비활성화](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/enable-fast-release-process.md).</span>

<span class="preview">현재 릴리스에 대한 자세한 내용은 [2024년 2분기 릴리스 개요](/help/quicksilver/product-announcements/product-releases/24-q2-release-activity/24-q2-release-overview.md).</span>

새 사용자 정의 양식을 만들거나 편집할 수 있습니다. 두 작업은 이 문서에 설명되어 있습니다.

기존 양식에서 새 사용자 정의 양식을 만드는 방법에 대한 자세한 내용은 [기존 양식 빌더로 새 양식을 만들려면 사용자 정의 양식을 복사하십시오.](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/copy-custom-form-to-create-a-new-one.md).

이 문서에서는 기존 양식 빌더를 사용하여 사용자 정의 양식을 만드는 방법을 설명합니다. 양식 디자이너를 사용하여 사용자 정의 양식을 만드는 방법에 대한 자세한 내용은 [양식 디자이너를 사용하여 양식 디자인](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/form-designer/design-a-form/design-a-form.md).

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
   <td><p>새로운 기능: 표준</p>
   <p>또는</p>
   <p>현재: 플랜</p></td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader">액세스 수준 구성</td> 
   <td> <p>사용자 정의 양식에 대한 관리 액세스</p> </td> 
  </tr>  
 </tbody> 
</table>

이 표의 정보에 대한 자세한 내용은 [Workfront 설명서의 액세스 요구 사항](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

## 사용자 정의 양식 만들기 시작

{{step-1-to-setup}}

1. 클릭 **사용자 지정 Forms** 왼쪽 패널에서

   사용자 정의 양식이 목록에 표시됩니다. 조직에 대해 만들어진 모든 사용자 정의 양식 및 사용자 정의 필드를 검토할 수 있습니다. 각 양식을 작성한 사용자, 양식 작성과 연관된 객체 및 양식 작성의 활성 여부도 확인할 수 있습니다.

1. 클릭 **새 사용자 정의 양식.**
1. 사용자 정의 양식과 연결할 개체 유형을 하나 이상 선택한 다음 를 클릭합니다 **계속**.

   ![](assets/choose-object-type.jpg)

1. 다음에서 **양식 설정** 탭이 열리면 a를 입력합니다. **양식 제목** 및 선택 사항 **설명** 사용자 정의 양식에 사용됩니다.

1. (선택 사항) 더 많은 오브젝트에 첨부할 수 있도록 양식에 더 많은 오브젝트 유형을 추가하려면 **플러스** 다음 이후 서명 **오브젝트 유형**&#x200B;을 클릭한 다음 표시되는 메뉴에서 원하는 오브젝트 유형을 선택합니다.

   이 단계를 반복하여 원하는 만큼 객체 유형을 추가할 수 있습니다.

1. (선택 사항) **X** 양식에서 삭제할 객체 유형을 입력합니다.

   이미 저장한 사용자 정의 양식에서 개체 유형을 삭제하는 방법에 대한 자세한 내용은 [사용자 정의 양식의 오브젝트 유형 삭제](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/delete-object-type-on-a-custom-form.md).

1. 클릭 **완료** 화면의 왼쪽 아래에 있습니다.

   >[!TIP]
   >
   >다음을 클릭할 수 있습니다. **적용** 언제든지 사용자 정의 양식을 만들어 변경 사항을 저장하고 양식을 열어 둡니다.

1. 양식에 새 사용자 정의 필드를 추가하려면 을(를) 계속합니다. [사용자 정의 양식에 사용자 정의 필드 추가](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/add-a-custom-field-to-a-custom-form.md) 또는 [사용자 정의 양식에서 사용자 정의 필드 또는 위젯 재사용](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/reuse-an-existing-field.md).

   또는

   다른 방법으로 사용자 정의 양식을 계속 작성하려면 다음 문서 중 하나를 계속 진행하십시오.

   * [사용자 정의 양식에서 에셋 위젯 추가 또는 편집](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/add-widget-or-edit-its-properties-in-a-custom-form.md)
   * [사용자 정의 양식에 사용자 정의 필드 및 위젯 배치](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/position-fields-in-a-custom-form.md)
   * [사용자 정의 양식에 섹션 구분 추가](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/add-a-section-break-to-a-custom-form.md)
   * [사용자 정의 양식에 계산된 데이터 추가](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/add-calculated-data-to-custom-form.md)
   * [사용자 정의 양식에서 기존의 계산된 사용자 정의 필드 재사용](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/use-existing-calc-field-new-custom-form.md)
   * [사용자 정의 양식에 표시 논리 및 건너뛰기 논리 추가](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/display-or-skip-logic-custom-form.md)

## 사용자 정의 양식 편집 시작

사용자 정의 양식이 만들어진 후 언제든지 편집할 수 있습니다.

>[!CAUTION]
>
>사용자가 사용자 정의 양식에서 해당 필드에 입력한 데이터를 손실하지 않고 필드를 제거하는 방법에 대한 자세한 내용은 섹션을 참조하십시오 [사용자가 입력한 데이터를 손실하지 않고 사용자 정의 필드 제거](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/delete-a-custom-field.md#remove) 이 문서에서 [시스템에서 사용자 정의 필드 또는 위젯 삭제](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/delete-a-custom-field.md).
>
>일반적으로 이미 사용 중인 사용자 정의 양식을 편집하는 횟수를 최소화하는 것이 좋습니다. 사용자 정의 양식을 사용하는 사람에게 변경 사항을 알리는 알림 시스템이 없습니다.

{{step-1-to-setup}}

1. 클릭 **사용자 지정 Forms** 왼쪽 패널에서

   사용자 정의 양식이 목록에 표시됩니다. 조직에 대해 만들어진 모든 사용자 정의 양식 및 사용자 정의 필드를 검토할 수 있습니다. 각 양식을 작성한 사용자, 양식 작성과 연관된 객체 및 양식 작성의 활성 여부도 확인할 수 있습니다.

1. 편집할 사용자 정의 양식을 선택한 다음 **편집** <span class="preview">또는 ![편집 아이콘](assets/edit-icon.png).</span>
1. (선택 사항) 사용자 정의 양식의 제목과 설명을 변경하려면 **양식 설정** 탭을 클릭한 다음 a를 입력합니다 **양식 제목** 및 **설명**.

1. (선택 사항) 더 많은 오브젝트에 첨부할 수 있도록 양식에 더 많은 오브젝트 유형을 추가하려면 다음 더하기 기호 + 를 클릭합니다 **오브젝트 유형**&#x200B;을 클릭한 다음 표시되는 메뉴에서 원하는 유형을 선택합니다.

   ![](assets/add-object-type-existing-form.png)

   이 단계를 반복하여 원하는 만큼 객체 유형을 추가할 수 있습니다.

   객체 유형의 X를 클릭하여 양식에서 삭제할 수도 있습니다. 이미 저장한 사용자 정의 양식에서 오브젝트 유형을 삭제하려는 경우 주의해서 이 작업을 수행해야 합니다. 자세한 내용은 [사용자 정의 양식의 오브젝트 유형 삭제](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/delete-object-type-on-a-custom-form.md).

1. 클릭 **완료**.

   >[!TIP]
   >
   >다음을 클릭할 수 있습니다. **적용** 언제든지 사용자 정의 양식을 만들어 변경 사항을 저장하고 양식을 열어 둡니다.

1. 양식에 새 사용자 정의 필드를 추가하려면 을(를) 계속합니다. [사용자 정의 양식에 사용자 정의 필드 추가](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/add-a-custom-field-to-a-custom-form.md) 또는 [사용자 정의 양식에서 사용자 정의 필드 또는 위젯 재사용](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/reuse-an-existing-field.md).

   또는

   다른 방법으로 사용자 정의 양식을 계속 작성하려면 다음 문서 중 하나를 계속 진행하십시오.

   * [사용자 정의 양식에서 에셋 위젯 추가 또는 편집](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/add-widget-or-edit-its-properties-in-a-custom-form.md)
   * [사용자 정의 양식에 사용자 정의 필드 및 위젯 배치](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/position-fields-in-a-custom-form.md)
   * [사용자 정의 양식에 섹션 구분 추가](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/add-a-section-break-to-a-custom-form.md)
   * [사용자 정의 양식에 계산된 데이터 추가](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/add-calculated-data-to-custom-form.md)
   * [사용자 정의 양식에서 기존의 계산된 사용자 정의 필드 재사용](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/use-existing-calc-field-new-custom-form.md)
   * [사용자 정의 양식에 표시 논리 및 건너뛰기 논리 추가](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/display-or-skip-logic-custom-form.md)
