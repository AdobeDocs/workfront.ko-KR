---
user-type: administrator
product-area: system-administration;user-management;setup
navigation-topic: create-and-manage-groups
title: 하위 그룹에 대한 프로젝트, 작업 또는 문제 환경 설정 잠금 또는 잠금 해제
description: Workfront 관리자가 시스템 수준에서 잠금을 해제한 경우 그룹 관리자는 프로젝트, 작업 또는 문제 환경 설정을 구성한 다음 잠글 수 있습니다.
author: Caroline
feature: System Setup and Administration, People Teams and Groups
role: Admin
exl-id: 05c32b6f-52e1-46a7-9011-633713422f3d
source-git-commit: 02191d80ea58f80de2e7be2ff55f43663e415e31
workflow-type: tm+mt
source-wordcount: '600'
ht-degree: 0%

---

# 하위 그룹에 대한 프로젝트, 작업 또는 문제 환경 설정 잠금 또는 잠금 해제

Workfront 관리자가 시스템 수준에서 잠금을 해제한 경우 그룹 관리자는 프로젝트, 작업 또는 문제 환경 설정을 구성한 다음 잠글 수 있습니다.

수준에서 구성한 프로젝트, 작업 또는 문제 환경 설정을 잠그면 그룹 및 해당 하위 그룹의 모든 사용자가 해당 환경 설정에 대해 동일한 설정을 사용할 수 있습니다. 그룹에 대해 잠근 환경 설정을 다시 구성할 수는 있지만 그룹 관리자는 그룹에 대해 기본 설정을 다시 구성할 수는 없습니다.

반대로 프로젝트, 작업 또는 문제 환경 설정을 잠금 해제하면 그룹 관리자가 해당 항목을 사용하여 그룹이 작동하는 방식을 보다 유연하게 관리할 수 있습니다. 환경 설정이 잠금 해제되면 그룹 관리자는 해당 하위 그룹에 대해 환경 설정을 다시 구성할 수 있습니다.

이는 Workfront 관리자가 시스템의 모든 사용자에 대한 환경 설정을 잠그거나 잠금 해제해야 하는 기능과 병행됩니다.

Workfront 관리자가 시스템의 모든 그룹에 대한 환경 설정을 잠그거나 잠금 해제할 수 있는 방법에 대한 자세한 내용은 [시스템의 모든 그룹에 대한 프로젝트 환경 설정 잠금 또는 잠금 해제](../../../administration-and-setup/set-up-workfront/configure-system-defaults/lock-or-unlock-project-preferences-for-groups-system.md)을 참조하십시오.

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">Unlike other Lock/Unlock articles that start just like this one, we need the steps here. In other areas, the lock/unlock step is part of the article about setting preferences or creating statuses.</p>
-->

>[!NOTE]
>
>* 그룹에 대해 잠금 해제된 환경 설정을 구성해도 그룹 아래의 하위 그룹에 대한 환경 설정에는 영향을 주지 않습니다.
>
>  그러나 새 하위 그룹이 생성되면 환경 설정 및 바로 위에 있는 그룹의 잠김 또는 잠금 해제 상태를 상속합니다.
>
>* 잠긴 기본 설정이 있는 그룹 아래로 그룹을 이동하면 이동된 그룹은 해당 기본 설정을 상속하며 이동된 그룹에 대해 잠깁니다.
>* 잠금 해제된 환경 설정이 있는 그룹으로 그룹을 이동하면 이동된 그룹은 해당 환경 설정의 영향을 받지 않습니다.
>
>  이동 시 이동된 그룹의 기본 설정이 잠겨 있으면 잠긴 상태로 유지되지만 상위 그룹에 대해 잠금 해제되어 있으므로 그룹 관리자가 지금 잠금 해제할 수 있습니다.
>

## 액세스 요구 사항

이 문서의 단계를 수행하려면 다음이 있어야 합니다.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Workfront 플랜*</td> 
   <td>임의</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront 라이센스*</td> 
   <td> <p>플랜 </p> <p>그룹의 그룹 관리자 또는 Workfront 관리자여야 합니다. 자세한 내용은 <a href="../../../administration-and-setup/manage-groups/group-roles/group-administrators.md" class="MCXref xref">그룹 관리자</a> 및 <a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-a-user-full-administrative-access.md" class="MCXref xref">사용자에게 전체 관리 액세스 권한 부여</a>를 참조하십시오.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;보유 중인 플랜 또는 라이선스 유형을 확인해야 하는 경우 Workfront 관리자에게 문의하십시오.

## 그룹 프로젝트, 작업 또는 문제 환경 설정 잠금 또는 잠금 해제

1. Adobe Workfront 오른쪽 상단의 **기본 메뉴** 아이콘 ![](assets/main-menu-icon.png)을(를) 클릭한 다음 **설정** ![](assets/gear-icon-settings.png)을(를) 클릭합니다.

1. 왼쪽 패널에서 **그룹**&#x200B;을 클릭합니다.
1. 프로젝트 환경 설정을 잠그거나 잠금 해제할 그룹의 이름을 클릭합니다.
1. 왼쪽 패널에서 **프로젝트 환경 설정** 또는 **작업 및 문제 환경 설정**&#x200B;을 클릭합니다.

1. 표시되는 페이지에서 시스템 수준에서 잠금 해제된 환경 설정 또는 그룹 위의 그룹에 대해 다음 중 하나를 수행합니다.

   * 그룹 아래의 그룹 관리자가 해당 그룹에 대한 환경 설정을 구성할 수 있도록 하려면 ![](assets/unlock-toggle-button.png) 잠금을 해제하세요.
   * 아래의 모든 그룹이 환경 설정에 대한 구성을 사용하도록 하려면 ![](assets/lock-toggle-button.png)이(가) 잠겨 있는지 확인하십시오.

     >[!IMPORTANT]
     >
     >잠긴 기본 설정을 구성하는 방식으로 모든 요구 사항을 처리할 수 있도록 아래 그룹의 관리자 및 사용자와 통신하는 것이 중요합니다. 이 구성을 잠그면 아래 하위 그룹에서 해당 구성을 상속합니다. 또한 환경 설정이 일정 기간 동안 잠금 해제된 경우 구성은 하위 그룹의 그룹 관리자가 수행한 작업을 대체합니다.

1. **저장**&#x200B;을 클릭합니다.
