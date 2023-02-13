---
user-type: administrator
product-area: system-administration
navigation-topic: create-and-manage-custom-forms
title: 사용자 지정 양식에서 사용자 지정 필드 또는 자산 위젯 재사용
description: 사용자 지정 양식을 만들거나 편집할 때 다른 사용자 지정 양식에 이미 추가된 사용자 지정 필드 또는 위젯을 추가할 수 있습니다.
author: Caroline
feature: System Setup and Administration
role: Admin
exl-id: 2c617909-48cb-4ee1-b0e8-002f2e57b0f0
source-git-commit: 63e332ff99d5c9d23f39d7e771c5eb924f1ffca3
workflow-type: tm+mt
source-wordcount: '386'
ht-degree: 0%

---

# 사용자 지정 양식에서 사용자 지정 필드 또는 자산 위젯 재사용

사용자 지정 양식을 만들거나 편집할 때 다른 사용자 지정 양식에 이미 추가된 사용자 지정 필드 또는 자산 위젯을 추가할 수 있습니다.

사용자 지정 양식에서 기존의 계산된 사용자 지정 필드를 다시 사용할 수도 있습니다. 자세한 내용은 [사용자 지정 양식에서 기존의 계산된 사용자 지정 필드 재사용](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/use-existing-calc-field-new-custom-form.md).

사용자 지정 양식의 사용자 지정 필드 및 자산 위젯에 대한 자세한 내용은 [사용자 지정 양식에 사용자 지정 필드 추가](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/add-a-custom-field-to-a-custom-form.md) 및 [사용자 지정 양식에서 자산 위젯 추가 또는 편집](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/add-widget-or-edit-its-properties-in-a-custom-form.md).

## 액세스 요구 사항

이 문서의 절차를 수행하려면 다음 사항이 있어야 합니다.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr data-mc-conditions=""> 
   <td role="rowheader"> <p>Adobe Workfront 플랜*</p> </td> 
   <td>모든</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront 라이선스*</td> 
   <td>플랜</td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader">액세스 수준 구성*</td> 
   <td> <p>사용자 정의 양식에 대한 관리 액세스</p> <p>Workfront 관리자가 이 액세스 권한을 부여하는 방법에 대한 자세한 내용은 <a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-users-admin-access-certain-areas.md" class="MCXref xref">특정 영역에 대한 관리자 액세스 권한 부여</a>.</p> </td> 
  </tr>  
 </tbody> 
</table>

&#42;보유한 계획, 라이선스 유형 또는 액세스 수준 구성을 알아보려면 Workfront 관리자에게 문의하십시오.

## 다른 사용자 지정 양식에 이미 사용된 사용자 지정 필드 또는 위젯을 다시 사용합니다

1. 에 설명된 대로 사용자 지정 양식 만들기 또는 편집을 시작합니다. [사용자 지정 양식 만들기 또는 편집](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/create-or-edit-a-custom-form.md).
1. 사용 **필드 추가** 선택한 경우 **필드 라이브러리**.

1. 원하는 사용자 지정 양식으로 필드나 위젯을 여기에 드래그합니다.
1. (선택 사항) 다른 필드나 위젯을 추가하려면 이전 두 단계를 반복합니다.

   >[!NOTE]
   >
   >단일 사용자 지정 양식에 최대 500개의 필드와 위젯을 추가할 수 있습니다. 그러나 양식에 100개 이상이 있을 경우 그 복잡성에 따라 성능이 저하될 수 있습니다.
   >
   >
   >복잡한 양식의 예로는 계단식 매개 변수가 있는 양식, 계산된 사용자 지정 데이터 필드 및 단일 필드에 여러 값 옵션이 있습니다.

1. 사용자 지정 양식을 다른 방식으로 계속 빌드하려면 다음 문서 중 하나를 계속 진행합니다.

   * [사용자 지정 양식에 사용자 지정 필드 추가](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/add-a-custom-field-to-a-custom-form.md#add2)
   * [사용자 지정 양식에 섹션 브레이크 추가](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/add-a-section-break-to-a-custom-form.md)
   * [사용자 지정 양식에서 자산 위젯 추가 또는 편집](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/add-widget-or-edit-its-properties-in-a-custom-form.md)
   * [사용자 지정 양식에 계산된 데이터 추가](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/add-calculated-data-to-custom-form.md)
   * [사용자 지정 양식에 사용자 지정 필드 및 위젯을 배치합니다](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/position-fields-in-a-custom-form.md)
   * [표시 논리를 추가하고 논리를 사용자 지정 양식에 건너뜁니다](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/display-or-skip-logic-custom-form.md)
   * [사용자 지정 양식 미리 보기 및 완료](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/preview-and-complete-a-custom-form.md)
