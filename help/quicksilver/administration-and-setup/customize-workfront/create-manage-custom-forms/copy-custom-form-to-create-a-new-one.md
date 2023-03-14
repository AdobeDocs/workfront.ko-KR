---
user-type: administrator
product-area: system-administration
keywords: create,custom,form,copy,base,another
navigation-topic: create-and-manage-custom-forms
title: 사용자 지정 양식을 복사하여 기존 빌더로 새 양식 만들기
description: 기존 사용자 지정 양식을 기반으로 하는 새 사용자 지정 양식을 만들 수 있습니다.
author: Caroline
feature: System Setup and Administration
role: Admin
exl-id: 946a726e-af88-413c-abe3-55fbc7486380
source-git-commit: ''
workflow-type: tm+mt
source-wordcount: '464'
ht-degree: 0%

---

# 사용자 지정 양식을 복사하여 기존 빌더로 새 양식 만들기

기존 사용자 지정 양식을 기반으로 하는 새 사용자 지정 양식을 만들 수 있습니다.

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

## 사용자 지정 양식을 복사하여 새 양식 만들기

1. 을(를) 클릭합니다. **기본 메뉴** 아이콘 ![](assets/main-menu-icon.png) Adobe Workfront의 오른쪽 위 모서리에서 을(를) 클릭하고 **설정** ![](assets/gear-icon-settings.png).

1. 클릭 **사용자 지정 Forms.**
1. 새 사용자 지정 양식의 기반으로 사용할 사용자 지정 양식을 선택한 다음 **복사**.
1. 에서 **사용자 지정 양식 복사** 표시되는 상자에 다음 정보를 입력합니다.

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">양식 이름</td> 
      <td>복사한 양식의 이름을 입력합니다.</td> 
     </tr> 
     <tr> 
      <td role="rowheader"> <p role="rowheader">양식 유형 </p> </td> 
      <td> <p>에서 <b>양식 유형</b> 상자에서 사용자 지정 양식을 사용할 개체 유형을 선택하고 제거할 형식 옆의 X를 클릭합니다. 이미 양식과 연결된 유형은 목록에서 비활성화됩니다.</p> 
      <p><img src="assets/copy-form-obj-types.png"></p> 
      <p>양식은 하나 이상의 개체 형식과 연결되어야 합니다.</p> 
      </td> 
     </tr> 
    </tbody> 
   </table>

1. 클릭 **양식 복사**.

   원래 양식에서 계산된 필드가 새 양식에 추가하는 개체 유형과 호환되지 않는 필드를 참조하는 경우 해당 필드의 계산을 변경하라는 메시지가 표시됩니다.

   마찬가지로, 원본 양식의 구역 나누기에 대한 액세스 옵션이 새 양식에 추가한 개체 유형과 호환되지 않으면 옵션을 조정하라는 메시지가 표시됩니다.

1. 방금 복사한 양식을 선택하고 **편집**.
1. 다음 문서에 설명된 대로 양식을 변경합니다.

   * [사용자 지정 양식을 복사하여 기존 양식 빌더로 새 양식 만들기](#Add2)
   * [기존 양식 빌더를 사용하여 계산된 데이터를 사용자 지정 양식에 추가합니다](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/add-calculated-data-to-custom-form.md)
   * [기존 양식 빌더를 사용하여 사용자 지정 양식에 사용자 지정 필드 및 위젯을 배치합니다](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/position-fields-in-a-custom-form.md)
   * [기존 양식 빌더를 사용하여 사용자 지정 양식에서 자산 위젯을 추가하거나 편집합니다](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/add-widget-or-edit-its-properties-in-a-custom-form.md)
   * [기존 양식 빌더를 사용하여 사용자 지정 양식에서 기존의 계산된 사용자 지정 필드를 다시 사용하십시오](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/use-existing-calc-field-new-custom-form.md)
   * [표시 논리를 추가하고 기존 양식 빌더를 사용하여 사용자 지정 양식에 논리를 건너뜁니다](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/display-or-skip-logic-custom-form.md)
   * [기존 양식 빌더로 사용자 지정 양식 미리 보기 및 완료](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/preview-and-complete-a-custom-form.md)

1. (선택 사항) **저장+닫기**&#x200B;에 설명된 대로 양식을 사용할 개체에 첨부합니다. [개체에 사용자 지정 양식 추가](../../../workfront-basics/work-with-custom-forms/add-a-custom-form-to-an-object.md).
