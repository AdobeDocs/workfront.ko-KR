---
user-type: administrator
product-area: system-administration
navigation-topic: create-and-manage-custom-forms
title: 시스템에서 사용자 정의 필드 또는 위젯 삭제
description: 시스템 성능을 개선하고 양식을 사용자가 쉽게 사용할 수 있도록 하기 위해 더 이상 사용되지 않는 사용자 정의 필드 및 위젯을 시스템에서 제거할 수 있습니다.
author: Lisa
feature: System Setup and Administration, Custom Forms
role: Admin
exl-id: c22a7ced-da81-40b5-bb4d-69d59b855add
source-git-commit: 8dac7959919014d7bfbbbd39d193d026ca31c4b2
workflow-type: tm+mt
source-wordcount: '581'
ht-degree: 0%

---

# 시스템에서 사용자 정의 필드 또는 위젯 삭제

시스템 성능을 개선하고 양식을 사용자가 쉽게 사용할 수 있도록 하기 위해 더 이상 사용되지 않는 사용자 정의 필드 및 위젯을 시스템에서 제거할 수 있습니다.

>[!CAUTION]
>
>사용자 정의 필드를 삭제하면 오브젝트에 첨부된 사용자 정의 양식을 작성할 때 사용자가 필드에 입력한 모든 사용자 정의 데이터도 삭제됩니다. 삭제된 데이터는 복구할 수 없습니다. 또한 사용자 정의 양식을 사용하는 사람에게 삭제된 것을 경고하기 위한 알림 시스템이 없습니다.
>
>삭제하려는 사용자 정의 필드를 사용하는 모든 사용자 정의 양식 및 보고서를 보고 영향을 평가할 수 있습니다. 자세한 내용은 [특정 사용자 정의 필드 또는 위젯을 사용하는 모든 사용자 정의 양식 보기](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/view-all-custom-forms-that-use-a-particular-custom-field.md) 및 [특정 사용자 정의 필드 또는 위젯을 사용하는 모든 보고서 보기](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/view-all-reports-that-use-a-particular-custom-field.md)를 참조하십시오.
>
>또는 더 이상 사용되지 않는 필드의 데이터가 손실되지 않도록 하는 데 사용할 수 있는 해결 방법은 이 문서에서 [사용자가 입력한 데이터를 손실하지 않고 사용자 정의 필드 제거](#remove-a-custom-field-without-losing-data-that-users-have-entered)를 참조하십시오.

## 액세스 요구 사항

+++ 을 확장하여 이 문서의 기능에 대한 액세스 요구 사항을 봅니다.

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
   <td>
   <p>새로운 기능: 표준</p>
   <p>또는</p>
   <p>현재: 플랜</p></td>
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader">액세스 수준 구성</td> 
   <td> <p>사용자 정의 양식에 대한 관리 액세스</p> </td> 
  </tr> 
 </tbody> 
</table>

이 표의 정보에 대한 자세한 내용은 [Workfront 설명서의 액세스 요구 사항](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)을 참조하십시오.

+++

## 시스템에서 사용자 정의 필드 또는 위젯 삭제

{{step-1-to-setup}}

1. **사용자 지정 Forms을 클릭합니다.**
1. 필드 영역을 열려면 **필드**&#x200B;를 클릭하세요.
1. 사용자 지정 필드 또는 위젯을 선택한 다음 **삭제**&#x200B;를 클릭합니다.
1. 항목을 영구적으로 삭제하려면(사용자 지정 필드의 경우) 항목이 첨부된 개체에 연결된 모든 데이터를 클릭합니다. **예, 삭제**&#x200B;를 클릭합니다.

## 사용자가 입력한 데이터를 손실하지 않고 사용자 정의 필드 제거 {#remove-a-custom-field-without-losing-data-that-users-have-entered}

>[!CAUTION]
>
>500개가 넘는 필드 및 위젯이 있는 사용자 정의 양식에서 사용자 정의 필드를 제거하는 작업은 실행 취소할 수 없습니다. 필드를 제거하면 양식에 500개 이하의 필드 및 위젯이 포함될 때까지 필드를 다시 추가할 수 없습니다.

1. 원래 사용자 정의 양식에서 제거할 사용자 정의 필드를 결정하되 지금은 제거하지 마십시오.
1. 새 사용자 정의 양식 만들기:

   1. 원래 사용자 정의 양식에서 제거할 새 양식에 사용자 정의 필드를 추가합니다.

      자세한 내용은 [양식 디자이너를 사용한 양식 디자인](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/form-designer/design-a-form/design-a-form.md)에서 [사용자 정의 양식에 새 필드 또는 기존 필드 추가](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/form-designer/design-a-form/design-a-form.md#add-new-or-existing-fields-to-your-custom-form) 섹션을 참조하십시오.

   1. 새 사용자 정의 양식을 저장합니다.

1. [사용자 정의 양식 공유](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/share-access-to-a-custom-form.md)에 설명된 대로 관리 액세스 권한이 있는 사용자만 사용자 정의 양식에 액세스하도록 제한합니다.
1. [개체에 사용자 정의 양식 추가](../../../workfront-basics/work-with-custom-forms/add-a-custom-form-to-an-object.md)에 설명된 대로 원본 사용자 정의 양식이 이미 적용된 개체에 새 사용자 정의 양식을 적용하십시오.

   이러한 오브젝트에 새 사용자 정의 양식을 적용하면 이전 보고 데이터에 영향을 주지 않습니다.

1. 원래 사용자 정의 양식을 수정하고 2단계에서 새 양식에 추가한 사용자 정의 필드를 제거합니다.

   원래 사용자 정의 양식에서 제거한 필드는 이제 새로 만든 사용자 정의 양식에서만 사용할 수 있습니다. 사용자는 오브젝트에 대한 사용자 정의 양식을 볼 수 있지만, 관리 액세스 권한이 없는 사용자는 사용자 정의 양식을 수정할 수 없습니다.
