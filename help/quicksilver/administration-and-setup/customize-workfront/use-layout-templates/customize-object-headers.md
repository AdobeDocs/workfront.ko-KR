---
title: 레이아웃 템플릿을 사용하여 개체 머리글 사용자 지정
user-type: administrator
product-area: system-administration;templates;setup
navigation-topic: layout-templates
description: Adobe Workfront 관리자 또는 그룹 관리자 는 레이아웃 템플릿을 사용하여 사용자가 오브젝트의 페이지를 열 때 오브젝트 헤더에 표시되는 필드를 구성할 수 있습니다.
author: Alina
feature: System Setup and Administration
role: Admin
exl-id: cbeaa0d7-a61a-4806-a871-96663d9ce124
source-git-commit: d2ca099e78d5adb707a0a5a53ccb2e6dd06698f8
workflow-type: tm+mt
source-wordcount: '531'
ht-degree: 0%

---

# 레이아웃 템플릿을 사용하여 개체 머리글 사용자 지정

Adobe Workfront 관리자 또는 그룹 관리자는 레이아웃 템플릿을 사용하여 사용자가 오브젝트의 페이지를 열 때 오브젝트 헤더에 표시되는 필드를 구성할 수 있습니다.

>[!IMPORTANT]
>
>현재 프로젝트, 작업 및 문제에 대해 개체 헤더 맞춤화를 사용할 수 있습니다.

![개체 헤더 필드](assets/object-header-fields.png)

레이아웃 템플릿 만들기에 대한 자세한 내용은 [레이아웃 템플릿 만들기 및 관리](../use-layout-templates/create-and-manage-layout-templates.md)를 참조하십시오.

그룹의 레이아웃 템플릿에 대한 자세한 내용은 [그룹의 레이아웃 템플릿 만들기 및 수정](../../../administration-and-setup/manage-groups/work-with-group-objects/create-and-modify-a-groups-layout-templates.md)을 참조하십시오.

레이아웃 템플릿을 구성한 후에는 다른 사용자가 변경 내용을 볼 수 있도록 사용자에게 할당해야 합니다. 사용자에게 레이아웃 템플릿을 할당하는 방법에 대한 자세한 내용은 [레이아웃 템플릿에 사용자 할당](../use-layout-templates/assign-users-to-layout-template.md)을 참조하십시오.

## 액세스 요구 사항

+++ 을 확장하여 이 문서의 기능에 대한 액세스 요구 사항을 봅니다.

이 문서의 단계를 수행하려면 다음 액세스 권한이 있어야 합니다.


<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront 플랜</td> 
   <td>임의</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront 라이센스*</td> 
   <td><p>새로운 기능: 표준</p>
  <p> 현재: 플랜</p>
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader">액세스 수준 구성</td> 
   <td> <p>시스템 수준에서 이러한 단계를 수행하려면 시스템 관리자 액세스 수준이 필요합니다.
그룹에 대해 이러한 작업을 수행하려면 해당 그룹의 관리자여야 합니다.</p> </td> 
  </tr> 
 </tbody> 
</table>

*자세한 내용은 [Workfront 설명서의 액세스 요구 사항](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)을 참조하십시오.

+++

## 개체 헤더 사용자 지정

1. [레이아웃 템플릿 만들기 및 관리](../../customize-workfront/use-layout-templates/create-and-manage-layout-templates.md)에 설명된 대로 레이아웃 템플릿 작업을 시작합니다.
1. **사용자에게 표시되는 항목 사용자 지정** 드롭다운 메뉴에서 **프로젝트**, **작업** 또는 **문제**&#x200B;를 선택합니다.

   <!--when this will be possible for more than 3 objects, at production, make this more general: update the sentence above to say "select an object you want to customize in the Customize what users see drop-down menu). -->

1. [!UICONTROL 헤더 필드] 섹션에서 표시된 필드 위로 마우스를 가져간 후 다음 중 하나를 수행합니다.
   * 필드를 제거하려면 **x** 아이콘을 클릭하십시오.

     또는

   * **grab** 아이콘을 길게 클릭하여 필드를 새 위치로 끌어서 놓습니다.

   <!--(NOTE: make sure the default names of these fields have not changed; otherwise, update screen shot)-->

   ![개체 머리글 필드 숨기기 및 이동 아이콘](assets/object-header-field-x-and-grab-icons-in-lt.png)

1. 오브젝트의 헤더에는 최대 5개의 필드가 있을 수 있습니다.
이미 5개의 필드를 선택한 경우 새 필드를 추가하기 전에 필드를 제거해야 합니다.
1. **필드 추가** 상자에서 추가하려는 편집할 수 없는 Workfront 필드의 이름을 입력한 다음 목록에 표시될 때 선택합니다. 필드는 필드 추가 상자의 바로 오른쪽에 추가되며, 개체 헤더의 왼쪽 위 모서리에 첫 번째 필드로 표시됩니다.

   >[!TIP]
   >
   >* 객체의 세부내용(Details) 섹션의 개요 영역에 표시되고 편집할 수 없는 필드만 추가할 수 있습니다. 편집할 수 없는 필드는 사용자가 수동으로 편집할 수 없는 필드입니다. 이 숫자들은 Workfront에 의해 자동으로 계산됩니다.
   >
   >* 이미 기본 머리글의 일부인 편집 가능한 필드(예: 프로젝트 소유자, 상태, 완료율, 할당)를 추가할 수 있습니다.
   >
   >* 문제의 헤더에 &quot;해결된 사람&quot; 필드를 추가할 때 문제와 연결된 해결 개체가 있으면 필드가 &quot;해결 중 문제, 작업 또는 프로젝트&quot;로 변경됩니다.


   ![헤더에 필드 추가](assets/add-field-to-header-in-lt-list.png)


1. (선택 사항) 다른 순서로 추가된 필드를 끌어다 놓습니다.

1. 레이아웃 템플릿을 계속 사용자 지정합니다.

   또는

   사용자 지정을 마쳤으면 **저장**&#x200B;을 클릭합니다.

   >[!TIP]
   >
   >언제든지 저장 을 클릭하여 진행 상황을 저장한 다음 나중에 템플릿을 계속 수정할 수 있습니다.
