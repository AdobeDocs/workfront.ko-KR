---
user-type: administrator
product-area: system-administration
navigation-topic: create-and-manage-custom-forms
title: 시스템에서 사용자 지정 필드 또는 위젯 삭제
description: 시스템 성능을 향상시키고 사용자가 양식을 쉽게 사용할 수 있도록 하기 위해 더 이상 사용하지 않을 때 시스템에서 사용자 지정 필드 및 위젯을 제거할 수 있습니다.
author: Caroline
feature: System Setup and Administration
role: Admin
exl-id: c22a7ced-da81-40b5-bb4d-69d59b855add
source-git-commit: f2f825280204b56d2dc85efc7a315a4377e551c7
workflow-type: tm+mt
source-wordcount: '576'
ht-degree: 0%

---

# 시스템에서 사용자 지정 필드 또는 위젯 삭제

시스템 성능을 향상시키고 사용자가 양식을 쉽게 사용할 수 있도록 하기 위해 더 이상 사용하지 않을 때 시스템에서 사용자 지정 필드 및 위젯을 제거할 수 있습니다.

>[!CAUTION]
>
>사용자 지정 필드를 삭제하면 사용자가 객체에 첨부된 사용자 지정 양식을 작성할 때 필드에 입력한 모든 사용자 지정 데이터도 삭제됩니다. 삭제된 데이터는 복구할 수 없습니다.
>
>삭제하려는 사용자 지정 필드를 사용하는 모든 사용자 지정 양식 및 보고서를 볼 수 있으므로 어떤 영향을 받을 수 있는지 평가할 수 있습니다. 자세한 내용은 [특정 사용자 지정 필드 또는 위젯을 사용하는 모든 사용자 지정 양식 보기](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/view-all-custom-forms-that-use-a-particular-custom-field.md) 및 [특정 사용자 지정 필드 또는 위젯을 사용하는 모든 보고서 보기](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/view-all-reports-that-use-a-particular-custom-field.md).
>
>또는 더 이상 사용되지 않는 필드의 데이터를 손실하지 않는 데 사용할 수 있는 해결 방법은 를 참조하십시오 [사용자가 입력한 데이터를 손실하지 않고 사용자 지정 필드를 제거합니다](#remove-a-custom-field-without-losing-data-that-users-have-entered) 참조하십시오.

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

## 시스템에서 사용자 지정 필드 또는 위젯 삭제

1. 을(를) 클릭합니다. **기본 메뉴** 아이콘 ![](assets/main-menu-icon.png) Adobe Workfront의 오른쪽 위 모서리에서 을(를) 클릭하고 **설정** ![](assets/gear-icon-settings.png).

1. 클릭 **사용자 지정 Forms.**
1. 을(를) 클릭합니다. **필드** 탭.
1. 사용자 지정 필드 또는 위젯을 선택한 다음 **삭제**.
1. 항목을 영구적으로 삭제하고 (사용자 지정 필드의 경우) 연결된 개체의 모든 관련 데이터를 삭제하려면 **예, 삭제합니다.**.

## 사용자가 입력한 데이터를 손실하지 않고 사용자 지정 필드를 제거합니다 {#remove-a-custom-field-without-losing-data-that-users-have-entered}

>[!CAUTION]
>
>필드 및 위젯이 500개를 초과하는 사용자 지정 양식에서 사용자 지정 필드를 제거하는 작업은 취소할 수 없습니다. 필드를 제거하는 경우 양식에 필드 및 위젯이 500개 미만이어야 필드를 다시 추가할 수 있습니다.

1. 원래 사용자 지정 양식에서 제거할 사용자 지정 필드를 결정하되, 이 시점에서는 제거하지 마십시오.
1. 에 설명된 대로 새 사용자 지정 양식을 만듭니다. [사용자 지정 양식 만들기 또는 편집](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/create-or-edit-a-custom-form.md).

   1. 에 설명된 대로 원본 사용자 지정 양식에서 제거할 새 양식에 사용자 지정 필드를 추가합니다 [사용자 지정 양식에서 사용자 지정 필드 또는 위젯 재사용](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/reuse-an-existing-field.md).
   1. 새 사용자 지정 양식을 저장합니다.

1. 다음에 설명된 대로 사용자 지정 양식에 대한 액세스를 관리자 액세스 권한이 있는 사용자만 제한할 수 있습니다. [사용자 지정 양식 공유](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/share-access-to-a-custom-form.md).
1. 에 설명된 대로 원본 사용자 지정 양식이 이미 적용된 개체에 새 사용자 지정 양식을 적용합니다. [개체에 사용자 지정 양식 추가](../../../workfront-basics/work-with-custom-forms/add-a-custom-form-to-an-object.md).

   이러한 개체에 새 사용자 지정 양식을 적용하면 이전 보고 데이터가 영향을 받지 않습니다.

1. 원래 사용자 지정 양식을 수정하고 새 양식(2단계)에 추가한 사용자 지정 필드를 제거합니다.

   이제 원래 사용자 지정 양식에서 제거한 필드를 만든 새 사용자 지정 양식에서만 사용할 수 있습니다. 사용자는 개체에서 사용자 지정 양식을 볼 수 있지만 관리 액세스 권한이 없는 사용자는 사용자 지정 양식을 수정할 수 없습니다.
