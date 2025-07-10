---
user-type: administrator
product-area: system-administration;user-management
keywords: 관리,하위 그룹,편집
navigation-topic: create-and-manage-subgroups
title: 하위 그룹 관리
description: 하위 그룹의 그룹 관리자는 하위 그룹을 생성, 이동, 보기, 편집, 복사, 이름 변경, 내보내기 및 삭제할 수 있습니다. 상위 그룹에서 하위 그룹을 제거하여 최상위 그룹으로 만들 수도 있습니다.
author: Lisa
feature: System Setup and Administration, People Teams and Groups
role: Admin
exl-id: 5186d266-fa9f-445d-9dcc-bc07eb147b60
source-git-commit: 6c3f5ee43040f81dac734c5e0b4def9021a0d737
workflow-type: tm+mt
source-wordcount: '1409'
ht-degree: 0%

---

# 하위 그룹 관리

하위 그룹의 그룹 관리자는 하위 그룹을 작성, 이동, 보기, 편집, 복사, 이름 변경, 내보내기 및 삭제할 수 있습니다.

상위 그룹에서 하위 그룹을 제거하여 최상위 그룹으로 만들 수도 있습니다.

그룹 위에 그룹이 있는 경우 해당 관리자는 그룹을 위해 이러한 작업을 수행할 수도 있습니다. Workfront 관리자(모든 그룹)의 경우도 마찬가지입니다.

하위 그룹에 대한 자세한 내용은 [하위 그룹 개요](../../../administration-and-setup/manage-groups/groups-overview/subgroups.md)를 참조하세요.

>[!TIP]
>
>하위 그룹을 포함하는 그룹을 관리할 때 전체 그룹과 모든 하위 그룹에 대한 데이터를 식별하고 필터링할 수 있는 것이 유용합니다. 이 작업은 보고서나 목록의 최상위 ID 필드를 사용하여 수행할 수 있습니다.
>
>예를 들어 대규모 마케팅 부서를 관리하고 전체 부서가 작업 중인 모든 프로젝트 목록을 원한다고 가정해 보겠습니다.
>
>Workfront에서 이 마케팅 부서는 Marketing이라는 그룹으로 표시되며, 3개의 하위 그룹인 Field Marketing, Product Marketing 및 Digital Marketing을 포함합니다. 전체 마케팅 부서(4개 그룹 모두)에 속하는 프로젝트를 나열하려면 다음 필터 규칙을 사용하여 프로젝트 영역에 대한 필터를 만들 수 있습니다.
>
>`Group: Top Parent ID > Equal > Marketing`
>
>최상위 이름 필드를 사용하여 최상위 그룹과 연관된 데이터를 식별할 수도 있지만 필터나 그룹화가 아닌 보기에서만 가능합니다.

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
  <tr> 
   <td role="rowheader">Adobe Workfront 라이선스</td> 
   <td><p>새로운 기능: 표준</p>
       <p>또는</p>
       <p>현재: 플랜</p></td>
  </tr> 
  </tr> 
  <tr> 
   <td role="rowheader">액세스 수준 구성</td> 
   <td>그룹의 그룹 관리자 또는 시스템 관리자여야 합니다.</td>
  </tr> 
 </tbody> 
</table>

이 표의 정보에 대한 자세한 내용은 [Workfront 설명서의 액세스 요구 사항](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)을 참조하십시오.

+++

## 하위 그룹 만들기

{{step-1-to-setup}}

1. 왼쪽 패널에서 **그룹** ![그룹](assets/groups-icon.png)을 클릭합니다.

   표시되는 목록에서 관리하는 그룹과 포함된 하위 그룹을 볼 수 있습니다. Adobe Workfront 관리자는 모든 그룹을 볼 수 있습니다.

1. 하위 그룹을 추가하려는 그룹의 이름을 클릭합니다.
1. 왼쪽 메뉴에서 **하위 그룹**&#x200B;을 클릭합니다.
1. 보고 있는 그룹에서 한 수준 아래에 새 하위 그룹을 만들려면 **하위 그룹 추가**&#x200B;를 클릭하세요.

   또는 목록의 다른 하위 그룹 아래에 새 하위 그룹을 만들려면 해당 하위 그룹을 선택한 다음 **하위 그룹 추가**&#x200B;를 클릭합니다.

   하위 그룹을 구성하는 데 사용할 수 있는 옵션에 대한 자세한 내용은 [하위 그룹 만들기](/help/quicksilver/administration-and-setup/manage-groups/create-and-manage-subgroups/create-a-subgroup.md)를 참조하십시오.

   그룹 계층은 15개 수준을 초과할 수 없지만, 단일 수준에는 병렬 그룹의 수가 무제한으로 포함될 수 있습니다.

## 하위 그룹 이동

기존 하위 그룹을 관리하는 다른 그룹으로 이동할 수 있습니다.

그룹 계층은 15개 수준을 초과할 수 없지만, 단일 수준에는 병렬 그룹의 수가 무제한으로 포함될 수 있습니다.

{{step-1-to-setup}}

1. 왼쪽 패널에서 **그룹** ![그룹](assets/groups-icon.png)을 클릭합니다.

   표시되는 목록에서 관리하는 그룹과 포함된 하위 그룹을 볼 수 있습니다. Adobe Workfront 관리자는 모든 그룹을 볼 수 있습니다.

1. 대상 그룹의 이름을 클릭합니다(이후 단계에서 이동할 하위 그룹을 지정합니다).
1. 왼쪽 메뉴에서 **하위 그룹**&#x200B;을 클릭합니다.
1. (선택 사항) 하위 그룹을 선택하여 대상 그룹으로 지정합니다.

   이 단계를 건너뛸 경우 3단계에서 선택한 그룹이 대상 그룹입니다.

1. **하위 그룹 추가 > 기존 그룹**&#x200B;을 클릭합니다.
1. 표시되는 **기존 그룹** 상자에서 이동할 하위 그룹의 이름을 입력하세요.

   표시되는 결과에 대상 그룹 위의 그룹이 포함되지 않습니다.

   마우스로 가리키고 그 옆에 표시되는 정보 아이콘 ![정보 아이콘](assets/info-icon.png)을 클릭하여 올바른 그룹을 선택했는지 확인할 수 있습니다. 그룹 및 해당 관리자의 상위 그룹 계층과 같은 그룹에 대한 정보를 나열하는 도구 설명이 표시됩니다.

1. 목록에서 이동할 하위 그룹의 이름을 선택합니다.
1. 대상 그룹으로 이동할 다른 모든 하위 그룹에 대해 7-8단계를 반복합니다.
1. **저장**&#x200B;을 클릭합니다.

## 하위 그룹 편집

{{step-1-to-setup}}

1. 왼쪽 패널에서 **그룹** ![그룹](assets/groups-icon.png)을 클릭합니다.

   표시되는 목록에서 관리하는 그룹과 포함된 하위 그룹을 볼 수 있습니다. Adobe Workfront 관리자는 모든 그룹을 볼 수 있습니다.

1. 편집할 하위 그룹이 포함된 그룹의 이름을 클릭합니다.
1. 왼쪽 메뉴에서 **하위 그룹**&#x200B;을 클릭합니다.
1. 편집할 하위 그룹을 선택한 다음 **편집** 아이콘 ![편집 아이콘](assets/edit-icon.png)을 클릭합니다.

   하위 그룹을 구성하는 데 사용할 수 있는 옵션에 대한 자세한 내용은 [하위 그룹 만들기](/help/quicksilver/administration-and-setup/manage-groups/create-and-manage-subgroups/create-a-subgroup.md)를 참조하십시오.

## 하위 그룹 복사

>[!NOTE]
>
>시스템 관리자만 하위 그룹을 복사할 수 있습니다.

하위 그룹을 복사하면 상위 그룹이 됩니다. 모든 그룹 멤버와 하위 그룹이 함께 복사됩니다. 그룹의 구성원은 원래 그룹에서 수행한 모든 임무를 유지합니다.

하위 그룹을 복사할 때에는 다음 사항을 고려하십시오.

* 복사하는 하위 그룹에 고유한 하위 그룹이 있는 경우 해당 하위 그룹이 복사본에 포함되며 해당 이름의 형식은 다음과 같습니다.

  `Original subgroup name (Copy)`

* 공개 그룹에 속한 모든 하위 그룹도 공개이므로 그룹 내외에서 사용자를 편집할 수 있는 액세스 권한이 있는 모든 사용자는 하위 그룹에 사용자를 추가할 수 있습니다.

하위 그룹을 복사하려면

{{step-1-to-setup}}

1. 왼쪽 패널에서 **그룹** ![그룹](assets/groups-icon.png)을 클릭합니다.

   표시되는 목록에서 관리하는 그룹과 포함된 하위 그룹을 볼 수 있습니다. Adobe Workfront 관리자는 모든 그룹을 볼 수 있습니다.

1. 복사할 하위 그룹이 포함된 그룹의 이름을 클릭합니다.
1. 왼쪽 메뉴에서 **하위 그룹**&#x200B;을 클릭합니다.
1. 하위 그룹을 선택한 다음 **복사** 아이콘 ![복사 아이콘](assets/copy-icon.png)을 클릭하여 선택한 그룹을 기반으로 새 최상위 그룹을 만듭니다.
1. 새 그룹의 설정을 구성합니다.

   이러한 설정에 대한 도움말은 문서 [그룹 만들기](/help/quicksilver/administration-and-setup/manage-groups/create-and-manage-groups/create-a-group.md#create-a-top-level-group-by-copying-an-existing-group-or-subgroup)에서 [기존 그룹 또는 하위 그룹을 복사하여 최상위 그룹 만들기](/help/quicksilver/administration-and-setup/manage-groups/create-and-manage-groups/create-a-group.md)를 참조하십시오.

1. **그룹 만들기**&#x200B;를 클릭합니다.

## 하위 그룹 내보내기

{{step-1-to-setup}}

1. 왼쪽 패널에서 **그룹** ![그룹](assets/groups-icon.png)을 클릭합니다.

   표시되는 목록에서 관리하는 그룹과 포함된 하위 그룹을 볼 수 있습니다. Adobe Workfront 관리자는 모든 그룹을 볼 수 있습니다.

1. 내보낼 하위 그룹이 포함된 그룹의 이름을 클릭합니다.
1. 왼쪽 메뉴에서 **하위 그룹**&#x200B;을 클릭합니다.
1. 내보낼 하위 그룹 또는 하위 그룹을 선택합니다.
1. **내보내기** 아이콘 ![내보내기 아이콘](assets/export.png)을 클릭한 다음 원하는 파일 형식을 선택합니다.

## 상위 그룹에서 하위 그룹을 제거하고 최상위 그룹으로 만들기

상위 그룹에서 하위 그룹을 제거하여 최상위 그룹으로 만들 수 있습니다.

>[!TIP]
>
>하위 그룹이 있는 그룹을 비활성화하면 해당 하위 그룹도 비활성화됩니다. 이들 중 하나를 활성화하려면 다음 지침을 사용하여 상위 그룹에서 제거한 다음 다시 활성화할 수 있습니다.
>&#x200B;>그룹 비활성화 및 다시 활성화에 대한 지침은 [그룹 비활성화 또는 다시 활성화](/help/quicksilver/administration-and-setup/manage-groups/create-and-manage-groups/deactivate-or-reactivate-a-group.md)를 참조하십시오.

{{step-1-to-setup}}

1. 왼쪽 패널에서 **그룹** ![그룹](assets/groups-icon.png)을 클릭합니다.
1. 최상위 그룹을 만들 하위 그룹의 상위 그룹을 선택한 다음 **편집** 아이콘 ![편집 아이콘](assets/edit-icon.png)을 클릭합니다.
1. 표시되는 **그룹 편집** 상자에서 **검색** 필드(**그룹 구성원 및 그룹 관리자** 아래)에 최상위 그룹을 만들 하위 그룹의 이름을 입력한 다음 표시될 때 이름 오른쪽에 있는 X를 클릭합니다.
1. **저장**&#x200B;을 클릭합니다.

## 하위 그룹 삭제

>[!IMPORTANT]
>
>그룹 또는 하위 그룹을 삭제할 때 현재 할당된 사용자, 작업 항목 및 모든 하위 그룹을 보존해야 합니다. 이러한 항목이 보존되어 있는지 확인하기 위해 프롬프트에서 그룹의 개체를 다른 그룹에 재할당해야 합니다.

{{step-1-to-setup}}

1. 왼쪽 패널에서 **그룹** ![그룹](assets/groups-icon.png)을 클릭합니다.

   표시되는 목록에서 관리하는 그룹과 포함된 하위 그룹을 볼 수 있습니다. Adobe Workfront 관리자는 모든 그룹을 볼 수 있습니다.

1. 삭제할 하위 그룹을 포함하는 그룹의 이름을 클릭합니다.
1. 왼쪽 메뉴에서 **하위 그룹**&#x200B;을 클릭합니다.
1. 하위 그룹을 선택한 다음 **삭제** 아이콘 ![삭제 아이콘](assets/delete.png)을 클릭합니다.

   표시되는 **그룹 삭제** 상자에서 입력을 시작한 다음 삭제할 그룹의 구성원, 작업 항목 및 하위 그룹을 이동할 그룹 이름을 선택합니다.

1. **삭제**&#x200B;를 클릭합니다.

## 그룹의 하위 그룹 구성원 보기 및 관리

관리하는 그룹의 기본 페이지를 볼 때 그룹의 하위 그룹에 있는 모든 사용자를 보고 관리할 수 있습니다. 지침은 [하위 그룹 구성원 보기 및 관리](../../../administration-and-setup/manage-groups/create-and-manage-subgroups/view-and-manage-subgroup-members.md)를 참조하세요.

