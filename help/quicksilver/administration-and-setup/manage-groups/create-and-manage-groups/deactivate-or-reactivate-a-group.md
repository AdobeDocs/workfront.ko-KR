---
user-type: administrator
product-area: system-administration;user-management;setup
navigation-topic: create-and-manage-groups
title: 그룹 비활성화 또는 다시 활성화
description: 더 이상 사용하지 않는 그룹을 비활성화할 수 있습니다.
author: Caroline
feature: System Setup and Administration, People Teams and Groups
role: Admin
exl-id: 99b81090-8d09-4130-a746-44ed1d76f971
source-git-commit: f2f825280204b56d2dc85efc7a315a4377e551c7
workflow-type: tm+mt
source-wordcount: '779'
ht-degree: 0%

---

# 그룹 비활성화 또는 다시 활성화

<!--
If Callisto adds the <b>Is active</b> checkbox to the Details page for groups you view, add that info to Manage groups/Create and manage groups/manage-a-group and to Manage groups/Create and manage groups/view-and-manage-a-groups-details
-->

더 이상 사용하지 않는 그룹을 비활성화할 수 있습니다.

## 액세스 요구 사항

이 문서의 절차를 수행하려면 다음 사항이 있어야 합니다.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Workfront 플랜*</td> 
   <td>모든</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront 라이선스*</td> 
   <td> <p>플랜 </p> <p>그룹의 그룹 관리자 또는 Workfront 관리자여야 합니다. 자세한 내용은 <a href="../../../administration-and-setup/manage-groups/group-roles/group-administrators.md" class="MCXref xref">그룹 관리자</a> 및 <a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-a-user-full-administrative-access.md" class="MCXref xref">사용자에게 전체 관리자 액세스 권한 부여</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;보유하고 있는 플랜 또는 라이선스 유형을 찾아야 하는 경우 Workfront 관리자에게 문의하십시오.

## 그룹 비활성화 또는 다시 활성화

>[!IMPORTANT]
>
>그룹을 비활성화하면 그 아래에 있는 모든 하위 그룹도 비활성화됩니다.
>
>이 중 하나를 다시 활성화해야 하는 경우 다음 중 하나를 수행한 후 다시 활성화할 수 있습니다.
>
>* 상위 그룹에서 제거합니다. 자세한 내용은 섹션을 참조하십시오 [상위 그룹에서 하위 그룹을 제거하고 최상위 그룹으로 만듭니다](../../../administration-and-setup/manage-groups/create-and-manage-subgroups/manage-subgroups.md#make) 기사 [하위 그룹 관리](../../../administration-and-setup/manage-groups/create-and-manage-subgroups/manage-subgroups.md).
>
>* 활성 그룹 아래로 이동합니다. 자세한 내용은 섹션을 참조하십시오 [하위 그룹 만들기, 이동, 보기, 편집, 복사, 이름 변경, 내보내기 또는 삭제](../../../administration-and-setup/manage-groups/create-and-manage-subgroups/manage-subgroups.md#create) 기사 [하위 그룹 관리](../../../administration-and-setup/manage-groups/create-and-manage-subgroups/manage-subgroups.md).
>


1. 을(를) 클릭합니다. **기본 메뉴** 아이콘 ![](assets/main-menu-icon.png) Adobe Workfront의 오른쪽 위 모서리에서 을(를) 클릭하고 **설정** ![](assets/gear-icon-settings.png).

1. 왼쪽 패널에서 을 선택합니다 **그룹**.

   표시되는 목록에서 관리하는 그룹과 해당 그룹의 하위 그룹을 볼 수 있습니다. Adobe Workfront 관리자는 모든 그룹을 볼 수 있습니다.

1. 그룹 이름을 클릭하여 해당 페이지를 엽니다.

1. 자세히 메뉴를 클릭합니다 ![](assets/more-icon.png) 그룹 이름 옆에 있는 **비활성화** 또는 **다시 활성화**.

   >[!NOTE]
   >
   >그룹이 비활성화된 그룹의 하위 그룹인 경우 활성 상태임 옵션(미리 보기에서 다시 활성화 옵션)을 사용할 수 없습니다. 다시 활성화하려면 먼저 위의 중요 노트에 설명된 대로 상위 그룹에서 제거하거나 활성 상태인 그룹에서 이동해야 합니다.

1. (조건부) 그룹을 비활성화하려면 **비활성화** 에서 **그룹 비활성화** 표시되는 상자.

## 비활성 그룹에 대한 고려 사항

섹션에서 설명한 활성 옵션을 비활성화하여 비활성화하는 그룹에 대해 다음 사항을 고려하십시오 [그룹 비활성화 또는 다시 활성화](#View) 참조하십시오.

* 그룹을 비활성화하면 그룹 아래에 있는 모든 하위 그룹도 비활성화됩니다. 여기에는 비활성화한 후 추가하는 하위 그룹이 포함됩니다.

   이 상황에서 하위 그룹을 다시 활성화하는 방법에 대한 내용은 [비활성 상위 그룹 아래의 하위 그룹 재활성화 정보](#about-reactivating-a-subgroup-below-an-inactive-parent-group) 참조하십시오.

* 설정의 그룹 영역으로 이동하면 활성 이 기본 필터이므로 목록에서 활성 그룹만 볼 수 있습니다 ![](assets/filter-nwepng.png) 활성화해줄 수 있습니다. 비활성 그룹을 포함하여 관리하는 모든 그룹을 보려면 모두 필터를 사용할 수 있습니다. 또는 비활성 필터를 사용하여 비활성 필터만 나열합니다.

   목록의 필터에 대한 자세한 내용은 다음을 참조하십시오 [Adobe Workfront의 필터 개요](../../../reports-and-dashboards/reports/reporting-elements/filters-overview.md).

* 그룹을 비활성화해도 다음 내용이 변경되지 않습니다.

   * 객체에 대한 그룹의 연관입니다. 연관된 객체는 변경 없이 이전과 동일하게 계속 작동합니다.

      예를 들어, 비활성화한 그룹과 프로젝트가 연결되어 있으면, 변경 없이 프로젝트의 환경 설정 및 상태가 계속 사용됩니다.

   * 설정의 그룹 페이지 내에서 승인, 팀 또는 회사와 같은 새 개체를 만들 수 있습니다. 기본적으로 새 객체는 비활성 그룹과 연결됩니다.
   * 관리자는 필터 및 보고에서 그룹을 찾을 수 있습니다.

      또한 설정 영역에서 그룹 설정을 관리할 수 있는 그룹 유형 앞에 있는 필드에서 해당 필드를 찾을 수도 있습니다. 여기에는 환경 설정, 이벤트 알림 및 시스템 라이센스 영역이 포함됩니다.

      예를 들어, 설정 > 프로젝트 환경 설정 > 프로젝트로 이동하고 여기에 있는 옵션 위에 있는 미리 보기 필드를 지운 경우 비활성 그룹을 찾아 해당 프로젝트 환경 설정을 구성할 수 있습니다.

## 비활성 상위 그룹 아래의 하위 그룹 재활성화 정보 {#about-reactivating-a-subgroup-below-an-inactive-parent-group}

그룹을 비활성화하면 그룹 아래에 있는 모든 하위 그룹도 비활성화됩니다. 비활성 그룹에서 하위 그룹 중 하나를 다시 활성화해야 하는 경우, 다음 두 가지 중 하나를 수행할 수 있습니다.

* 활성 그룹 아래에서 하위 그룹을 이동합니다. 그런 다음 섹션에 설명된 대로 이동된 그룹에 대해 활성 상태임 옵션을 활성화합니다 [그룹 비활성화 또는 다시 활성화](#View) 참조하십시오.

   그룹 이동에 대한 지침은 [그룹 이동](../../../administration-and-setup/manage-groups/create-and-manage-groups/move-a-group.md).

* 하위 그룹을 상위 그룹에서 제거합니다(하위 그룹을 최상위 그룹으로 지정). 그런 다음 섹션에 설명된 대로 이동된 그룹에 대해 활성 상태임 옵션을 활성화합니다 [그룹 비활성화 또는 다시 활성화](#View) 참조하십시오.

   상위 그룹에서 하위 그룹을 제거하는 방법에 대한 지침은 섹션을 참조하십시오 [상위 그룹에서 하위 그룹을 제거하고 최상위 그룹으로 만듭니다](../../../administration-and-setup/manage-groups/create-and-manage-subgroups/manage-subgroups.md#make) 기사 [하위 그룹 관리](../../../administration-and-setup/manage-groups/create-and-manage-subgroups/manage-subgroups.md).
