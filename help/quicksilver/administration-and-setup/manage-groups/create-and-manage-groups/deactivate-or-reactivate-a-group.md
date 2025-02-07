---
user-type: administrator
product-area: system-administration;user-management;setup
navigation-topic: create-and-manage-groups
title: 그룹 비활성화 또는 재활성화
description: 더 이상 사용하지 않는 관리 그룹을 비활성화할 수 있습니다.
author: Lisa
feature: System Setup and Administration, People Teams and Groups
role: Admin
exl-id: 99b81090-8d09-4130-a746-44ed1d76f971
source-git-commit: 85aa6cc865bfc28498cca17e1942c146eeb8e4fc
workflow-type: tm+mt
source-wordcount: '770'
ht-degree: 0%

---

# 그룹 비활성화 또는 재활성화

<!--
If Callisto adds the <b>Is active</b> checkbox to the Details page for groups you view, add that info to Manage groups/Create and manage groups/manage-a-group and to Manage groups/Create and manage groups/view-and-manage-a-groups-details
-->

더 이상 사용하지 않는 관리 그룹을 비활성화할 수 있습니다.

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

## 그룹 비활성화 또는 재활성화

>[!IMPORTANT]
>
>그룹을 비활성화하면 그 아래의 모든 하위 그룹도 비활성화됩니다.
>
>이 중 하나를 다시 활성화해야 하는 경우 다음 중 하나를 수행한 후 다시 활성화할 수 있습니다.
>
>* 상위 그룹에서 제거합니다. 자세한 내용은 문서 [하위 그룹 관리](../../../administration-and-setup/manage-groups/create-and-manage-subgroups/manage-subgroups.md)에서 [상위 그룹에서 하위 그룹을 제거하고 최상위 그룹으로 만들기](../../../administration-and-setup/manage-groups/create-and-manage-subgroups/manage-subgroups.md#make) 섹션을 참조하십시오.
>
>* 활성 그룹으로 이동합니다. 자세한 내용은 문서 [하위 그룹 관리](../../../administration-and-setup/manage-groups/create-and-manage-subgroups/manage-subgroups.md)에서 [하위 그룹을 만들기, 이동, 보기, 편집, 복사, 이름 변경, 내보내기 또는 삭제](../../../administration-and-setup/manage-groups/create-and-manage-subgroups/manage-subgroups.md#create) 섹션을 참조하십시오.

{{step-1-to-setup}}

1. 왼쪽 패널에서 **그룹**&#x200B;을 선택합니다.

   표시되는 목록에서 관리하는 그룹과 포함된 하위 그룹을 볼 수 있습니다. Adobe Workfront 관리자는 모든 그룹을 볼 수 있습니다.

1. 그룹 이름을 클릭하여 해당 페이지를 엽니다.

1. 그룹 이름 옆에 있는 기타 메뉴 ![기타 아이콘](assets/more-icon.png)을 클릭한 다음 **비활성화** 또는 **다시 활성화**&#x200B;를 클릭합니다.

   >[!NOTE]
   >
   >활성화됨 옵션(미리보기의 재활성화 옵션)은 그룹이 비활성화된 그룹의 하위 그룹인 경우 사용할 수 없습니다. 다시 활성화하려면 먼저 위의 중요 참고 사항에 설명된 대로 상위 그룹에서 제거하거나 활성 상태인 그룹으로 이동해야 합니다.

1. (조건부) 그룹을 비활성화하는 경우 표시되는 **그룹 비활성화** 상자에서 **비활성화**&#x200B;를 클릭합니다.

## 비활성 그룹에 대한 고려 사항

이 문서의 [그룹 비활성화 또는 다시 활성화](#View) 섹션에 설명된 활성 상태 옵션을 비활성화하여 비활성화하는 그룹에 대한 다음 사항을 고려하십시오.

* 그룹을 비활성화하면 그 아래의 모든 하위 그룹도 비활성화됩니다. 여기에는 비활성화한 후 추가하는 하위 그룹이 포함됩니다.

  이 상황에서 하위 그룹을 다시 활성화하는 방법에 대한 자세한 내용은 이 문서에서 [비활성 상위 그룹 아래의 하위 그룹 다시 활성화 정보](#about-reactivating-a-subgroup-below-an-inactive-parent-group)를 참조하십시오.

* [설정]의 [그룹] 영역으로 이동하면 [활성]이 기본 필터 ![필터 아이콘](assets/filter-nwepng.png)이므로 목록에 활성 그룹만 표시됩니다. 비활성 그룹을 포함하여 관리하는 모든 그룹을 보려면 모두 필터를 사용할 수 있습니다. 또는 비활성 필터를 사용하여 비활성 필터만 나열합니다.

  목록의 필터에 대한 자세한 내용은 [필터 개요](../../../reports-and-dashboards/reports/reporting-elements/filters-overview.md)를 참조하십시오.

* 그룹을 비활성화해도 다음 사항이 변경되지 않습니다.

   * 객체에 대한 그룹의 연관입니다. 연관된 객체는 변경 없이 이전과 동일하게 계속 작동합니다.

     예를 들어, 비활성화 중인 그룹과 프로젝트가 연결되어 있는 경우 프로젝트는 변경 없이 그룹의 환경 설정 및 상태를 계속 사용합니다.

   * 설정의 그룹 페이지 내에서 승인, 팀 또는 회사와 같은 새 개체를 만들 수 있습니다. 기본적으로 새 객체는 비활성 그룹과 연결되어 있습니다.
   * 필터 및 보고에서 그룹을 찾을 수 있는 관리자 권한.

     설정 영역에서 그룹 설정을 관리할 그룹 유형 미리 필드에서도 찾을 수 있습니다. 여기에는 환경 설정, 이벤트 알림 및 시스템 라이선스 영역이 포함됩니다.

     예를 들어 설정 > 프로젝트 환경 설정 > 프로젝트 로 이동하여 옵션 위의 자동 완성 필드를 지우는 경우 비활성 그룹을 계속 찾아 해당 프로젝트 환경 설정을 구성할 수 있습니다.

## 비활성 상위 그룹 아래의 하위 그룹 다시 활성화 정보 {#about-reactivating-a-subgroup-below-an-inactive-parent-group}

그룹을 비활성화하면 그 아래의 모든 하위 그룹도 비활성화됩니다. 비활성 그룹 아래의 하위 그룹 중 하나를 다시 활성화해야 하는 경우 다음 두 가지 중 하나를 수행할 수 있습니다.

* 활성 그룹 아래로 하위 그룹을 이동합니다. 이 문서의 [그룹 비활성화 또는 다시 활성화](#View) 섹션에 설명된 대로 이동한 그룹에 대해 활성 옵션을 활성화합니다.

  그룹 이동에 대한 지침은 [그룹 이동](../../../administration-and-setup/manage-groups/create-and-manage-groups/move-a-group.md)을 참조하세요.

* 상위 그룹에서 하위 그룹을 제거합니다(하위 그룹을 최상위 그룹으로 만들기). 이 문서의 [그룹 비활성화 또는 다시 활성화](#View) 섹션에 설명된 대로 이동한 그룹에 대해 활성 옵션을 활성화합니다.

  상위 그룹에서 하위 그룹을 제거하는 방법에 대한 지침은 문서 [하위 그룹 관리](../../../administration-and-setup/manage-groups/create-and-manage-subgroups/manage-subgroups.md)에서 [상위 그룹에서 하위 그룹 제거 및 최상위 그룹으로 만들기](../../../administration-and-setup/manage-groups/create-and-manage-subgroups/manage-subgroups.md#make) 섹션을 참조하십시오.
