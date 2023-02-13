---
title: 레이아웃 템플릿을 사용하여 개체 머리글 사용자 지정
user-type: administrator
product-area: system-administration;templates;setup
navigation-topic: layout-templates
description: Adobe Workfront 관리자 또는 그룹 관리자 는 레이아웃 템플릿을 사용하여 사용자가 개체의 페이지를 열 때 개체 헤더에서 볼 수 있는 필드를 구성할 수 있습니다.
author: Caroline
feature: System Setup and Administration
role: Admin
exl-id: cbeaa0d7-a61a-4806-a871-96663d9ce124
source-git-commit: a1ffec0d8a50ff7f025ff23370afa746cf0d6d3f
workflow-type: tm+mt
source-wordcount: '464'
ht-degree: 0%

---

# 레이아웃 템플릿을 사용하여 개체 머리글 사용자 지정

Adobe Workfront 관리자나 그룹 관리자는 레이아웃 템플릿을 사용하여 사용자가 객체의 페이지를 열 때 객체 헤더에서 볼 수 있는 필드를 구성할 수 있습니다.

>[!IMPORTANT]
>
>객체 헤더 사용자 지정은 현재 프로젝트, 작업 및 문제에 사용할 수 있습니다.


그룹의 레이아웃 템플릿에 대한 자세한 내용은 [그룹의 레이아웃 템플릿 만들기 및 수정](../../manage-groups/work-with-group-objects/create-and-modify-a-groups-layout-templates.md).

![](assets/object-header-fields.png)

## 액세스 요구 사항

이 문서의 절차를 수행하려면 다음 액세스 권한이 있어야 합니다.


<table>
  <tr>
   <td><strong>Adobe Workfront 플랜</strong>
   </td>
   <td>모든
   </td>
  </tr>
  <tr>
   <td><strong>Adobe Workfront 라이선스</strong>
   </td>
   <td>플랜
   </td>
  </tr>
  <tr>
   <td><strong>액세스 수준 구성</strong>
   </td>
   <td>Workfront 또는 그룹 관리자여야 합니다.
<p>
   </td>
  </tr>
</table>

여전히 액세스 권한이 없는 경우 Workfront 관리자에게 액세스 수준에서 추가 제한 사항을 설정하는지 문의하십시오. Workfront 관리자가 액세스 수준을 수정하는 방법에 대한 자세한 내용은 [사용자 정의 액세스 수준 만들기 또는 수정](../../add-users/configure-and-grant-access/create-modify-access-levels.md).

## 개체 헤더 사용자 지정

1. 에 설명된 대로 레이아웃 템플릿 작업을 시작합니다. [레이아웃 템플릿 만들기 및 관리](../../customize-workfront/use-layout-templates/create-and-manage-layout-templates.md).
1. 에서 **사용자에게 표시되는 항목 사용자 지정** 드롭다운 메뉴에서 **프로젝트**, **작업** 또는 **문제**.

   <!--when this will be possible for more than 3 objects, at production, make this more general: update the sentence above to say "select an object you want to customize in the Customize what users see drop-down menu). -->

1. 에서 [!UICONTROL 헤더 필드] 섹션을 마우스로 표시된 필드 위에 마우스를 놓고 다음 중 하나를 수행합니다.
   * 을(를) 클릭합니다. **x** 아이콘을 사용하여 필드를 제거합니다

      또는

   * 을(를) 클릭하고 **잡아서** 아이콘을 클릭하여 필드를 새 위치에 끌어 놓습니다.

   <!--(NOTE: make sure the default names of these fields have not changed; otherwise, update screen shot)-->

   ![](assets/object-header-field-x-and-grab-icons-in-lt.png)

1. 개체 헤더에 최대 5개의 필드를 포함할 수 있습니다.
이미 5개의 필드를 선택한 경우 새 필드를 추가하려면 먼저 필드를 제거해야 합니다.
1. 에서 **필드 추가** 상자에서 추가할 편집할 수 없는 Workfront 필드의 이름을 입력한 다음 목록에 표시될 때 선택합니다. 필드가 추가 필드 상자의 바로 오른쪽에 추가되고 객체 헤더의 왼쪽 위 모서리에 첫 번째 필드로 표시됩니다.

   >[!TIP]
   >
   >* 객체의 세부 정보 섹션의 개요 영역에 표시되고 편집할 수 없는 필드만 추가할 수 있습니다. 편집할 수 없는 필드는 사용자가 수동으로 편집할 수 없는 필드입니다. 이러한 데이터는 Workfront에 의해 자동으로 계산됩니다.
   >
   >* 이미 기본 헤더의 일부인 편집 가능한 필드(예: 프로젝트 소유자, 상태, 완료%, 지정)를 추가할 수 있습니다.
   >
   >* 문제 헤더에 &quot;해결된 사람&quot; 필드를 추가하면 문제와 연관된 해결 개체가 있으면 필드가 &quot;문제 해결, 작업 또는 프로젝트&quot;로 변경됩니다.



   ![](assets/add-field-to-header-in-lt-list.png)


1. (선택 사항) 추가된 필드를 다른 순서로 드래그하여 놓습니다.

1. 레이아웃 템플릿을 계속 사용자 지정합니다.

   또는

   사용자 지정을 완료한 경우 을 누릅니다 **저장**.

   >[!TIP]
   >
   >언제든지 저장 을 클릭하여 진행 상태를 저장한 다음 나중에 계속 템플릿을 수정할 수 있습니다.
