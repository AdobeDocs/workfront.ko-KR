---
user-type: administrator
product-area: system-administration
navigation-topic: create-and-manage-custom-forms
title: 기존 양식 빌더를 사용하여 사용자 정의 양식에 사용자 정의 필드 및 위젯 배치
description: 사용자 정의 양식에서 사용자 정의 필드 및 위젯의 위치를 변경할 수 있습니다.
author: Lisa
feature: System Setup and Administration, Custom Forms
role: Admin
exl-id: f96425e3-8e20-43ac-8340-915538ae5886
source-git-commit: d32f274390f6ffc5fdd01c2c9b4b2abd99d7cb10
workflow-type: tm+mt
source-wordcount: '449'
ht-degree: 0%

---

# 기존 양식 빌더를 사용하여 사용자 정의 양식에 사용자 정의 필드 및 위젯 배치

{{form-designer-default}}

사용자 정의 양식에서 사용자 정의 필드 및 위젯의 위치를 변경할 수 있습니다.

사용자 정의 양식의 사용자 정의 필드 및 위젯에 대한 자세한 내용은 [사용자 정의 양식에 사용자 정의 필드 추가](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/add-a-custom-field-to-a-custom-form.md) 및 [사용자 정의 양식의 에셋 위젯 추가 또는 편집](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/add-widget-or-edit-its-properties-in-a-custom-form.md)을 참조하십시오.

## 액세스 요구 사항

이 문서의 단계를 수행하려면 다음이 있어야 합니다.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr data-mc-conditions=""> 
   <td role="rowheader"> <p>Adobe Workfront 플랜*</p> </td> 
   <td>임의</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront 라이센스*</td> 
   <td>플랜</td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader">액세스 수준 구성*</td> 
   <td> <p>사용자 정의 양식에 대한 관리 액세스</p> <p>Workfront 관리자가 이 액세스 권한을 부여하는 방법에 대한 자세한 내용은 <a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-users-admin-access-certain-areas.md" class="MCXref xref">특정 영역에 대한 관리자 액세스 권한 부여</a>를 참조하십시오.</p> </td> 
  </tr>  
 </tbody> 
</table>

&#42;플랜, 라이선스 유형 또는 액세스 수준 구성을 알아보려면 Workfront 관리자에게 문의하세요.

## 사용자 정의 양식에 사용자 정의 필드 및 위젯 배치

1. [기존 양식 빌더로 사용자 정의 양식 만들기 또는 편집](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/create-or-edit-a-custom-form.md)에 설명된 대로 사용자 정의 양식을 만들거나 편집하십시오.
1. [기존 양식 빌더를 사용하여 사용자 정의 양식에 사용자 정의 필드 추가](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/add-a-custom-field-to-a-custom-form.md) 및 [기존 양식 빌더를 사용하여 사용자 정의 양식에 에셋 위젯을 추가 또는 편집](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/add-widget-or-edit-its-properties-in-a-custom-form.md)에 설명된 대로 양식에 사용자 정의 필드 및 위젯을 추가합니다.

1. (선택 사항) 사용자 정의 필드 및 위젯을 동일한 행에 배치하려면 한 줄을 서로 다른 행 옆에 드래그하여 그 사이에 선이 표시되도록 합니다.

<!--
Courtney, this is a story that got postponed after I did the work. Slated for some time in 22.4 (https://hub.workfront.adobe.com/task/6220d425000140d7f7d3ea68cc9529c8/documents)
   You can drag multiple items. Press the following keys while you select the items, then drag the items together to the new row:
   * Mac: Command+Shift [Courtney, double-check these commands]
   * Windows: Ctrl+Shift

   When you drop the custom field or widget, a gray box displays around the two items to indicate that they share a row.
-->

>[!NOTE]
>
>* 오른쪽 아래 모서리에 있는 **미리 보기** 단추를 사용하여 사용자 정의 필드 및 위젯이 양식에 표시되는 방식을 파악할 수 있습니다.
>* 설명 텍스트 필드는 행을 공유할 수 없습니다.
>* 사용자 정의 필드 및 위젯은 사용자가 볼 때 사용할 수 있는 화면 공간의 크기에 따라 양식에서 항상 동일한 방식으로 표시되지 않을 수 있습니다. 예를 들어, 수평 공간이 제한되는 경우 필드 행의 세 번째 필드는 다음 필드 행으로 래핑될 수 있다.

1. (선택 사항) 사용자 정의 필드 또는 위젯을 다른 필드 위 또는 아래에 배치하려면 항목 사이에 가로 파란색 선이 나타날 때까지 위 또는 아래로 드래그합니다.
1. **적용**&#x200B;을 클릭합니다.
1. 다른 방법으로 사용자 정의 양식을 계속 작성하려면 다음 문서 중 하나를 계속 진행하십시오.

   * [기존 양식 빌더를 사용하여 사용자 정의 양식에 사용자 정의 필드를 추가](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/add-a-custom-field-to-a-custom-form.md#add2)
   * [기존 양식 빌더를 사용하여 사용자 지정 양식에 자산 위젯을 추가하거나 편집합니다](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/add-widget-or-edit-its-properties-in-a-custom-form.md)
   * [기존 양식 빌더를 사용하여 사용자 정의 양식에 계산된 데이터를 추가](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/add-calculated-data-to-custom-form.md)
   * [기존 양식 빌더를 사용하여 사용자 지정 양식에 섹션 나누기를 추가합니다](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/add-a-section-break-to-a-custom-form.md)
   * [기존 양식 빌더를 사용하여 표시 논리를 추가하고 건너뛰기 논리를 사용자 지정 양식에 추가](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/display-or-skip-logic-custom-form.md)
   * [기존 양식 빌더로 사용자 정의 양식 미리 보기 및 완료](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/preview-and-complete-a-custom-form.md)
