---
user-type: administrator
product-area: system-administration;user-management;setup
navigation-topic: create-and-manage-groups
title: 하위 그룹에 대한 프로젝트, 작업 또는 문제 환경 설정 잠금 또는 잠금 해제
description: Workfront 관리자가 시스템 수준에서 잠금을 해제한 경우 그룹 관리자는 프로젝트, 작업 또는 문제 환경 설정을 구성한 다음 잠글 수 있습니다.
author: Lisa
feature: System Setup and Administration, People Teams and Groups
role: Admin
exl-id: 05c32b6f-52e1-46a7-9011-633713422f3d
source-git-commit: a42a167447d2f11b5502e4a0953b5e7eec2e67b1
workflow-type: tm+mt
source-wordcount: '571'
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

## 액세스 요구 사항

+++ 을 확장하여 이 문서의 기능에 대한 액세스 요구 사항을 봅니다.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>Adobe Workfront 패키지</td> 
   <td><p>임의</p></td> 
  </tr> 
  <tr> 
   <td>Adobe Workfront 라이선스</td> 
   <td><p>표준</p>
       <p>플랜</p></td>
  </tr>
  <tr> 
   <td>액세스 수준 구성</td> 
   <td>그룹의 그룹 관리자 또는 시스템 관리자여야 합니다.</td>
  </tr>
 </tbody> 
</table>

자세한 내용은 [Workfront 설명서의 액세스 요구 사항](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)을 참조하십시오.

+++

## 그룹 프로젝트, 작업 또는 문제 환경 설정 잠금 또는 잠금 해제

{{step-1-to-setup}}

1. 왼쪽 패널에서 **그룹**&#x200B;을 클릭합니다.
1. 프로젝트 환경 설정을 잠그거나 잠금 해제할 그룹의 이름을 클릭합니다.
1. 왼쪽 패널에서 **프로젝트 환경 설정** 또는 **작업 및 문제 환경 설정**&#x200B;을 클릭합니다.

1. 표시되는 페이지에서 시스템 수준에서 잠금 해제된 환경 설정 또는 그룹 위의 그룹에 대해 다음 중 하나를 수행합니다.

   * 그룹 아래의 그룹 관리자가 그룹의 환경 설정을 구성할 수 있도록 하려면 ![잠금 해제 토글](assets/unlock-toggle-button.png)을 잠금 해제하세요.
   * 아래의 모든 그룹이 환경 설정에 대한 구성을 사용하도록 하려면 ![잠금 전환](assets/lock-toggle-button.png)이 잠겨 있는지 확인하세요.

     >[!IMPORTANT]
     >
     >잠긴 기본 설정을 구성하는 방식으로 모든 요구 사항을 처리할 수 있도록 아래 그룹의 관리자 및 사용자와 통신하는 것이 중요합니다. 이 구성을 잠그면 아래 하위 그룹에서 해당 구성을 상속합니다. 또한 환경 설정이 일정 기간 동안 잠금 해제된 경우 구성은 하위 그룹의 그룹 관리자가 수행한 작업을 대체합니다.

1. **저장**&#x200B;을 클릭합니다.
