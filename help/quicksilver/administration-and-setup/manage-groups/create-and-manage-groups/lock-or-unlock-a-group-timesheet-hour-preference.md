---
user-type: administrator
product-area: system-administration;user-management;setup
navigation-topic: create-and-manage-groups
title: 그룹 타임시트 및 시간 환경 설정 잠금 또는 잠금 해제
description: 그룹 관리자인 경우 Workfront 관리자가 시스템 수준에서 그룹을 잠금 해제한 후 그룹에 대한 타임시트 및 시간 기본 설정을 구성한 다음 잠글 수 있습니다.
author: Caroline
feature: System Setup and Administration, People Teams and Groups
role: Admin
exl-id: 5b36106f-d521-4cc1-9f1f-647415c282b4
source-git-commit: f2f825280204b56d2dc85efc7a315a4377e551c7
workflow-type: tm+mt
source-wordcount: '629'
ht-degree: 0%

---

# 그룹 타임시트 및 시간 환경 설정 잠금 또는 잠금 해제

그룹 관리자인 경우 Workfront 관리자가 시스템 수준에서 그룹을 잠금 해제한 후 그룹에 대한 타임시트 및 시간 기본 설정을 구성한 다음 잠글 수 있습니다.

Adobe Workfront 환경 설정을 잠그면 그룹과 하위 그룹의 모든 사용자가 해당 환경 설정에 대해 동일한 설정을 사용할 수 있습니다. 잠근 환경 설정을 다시 구성할 수는 있지만 그룹 관리자는 하위 그룹을 더 낮게 만들 수는 없습니다.

반대로 그룹 수준에서 환경 설정을 잠금 해제하면 하위 그룹 관리자가 해당 항목을 사용하여 그룹이 작동하는 방식을 보다 유연하게 관리할 수 있습니다. 환경 설정이 잠금 해제되면 그룹 관리자는 해당 하위 그룹에 대해 환경 설정을 다시 구성할 수 있습니다.

이는 Workfront 관리자가 시스템의 모든 사용자에 대한 환경 설정을 잠그거나 잠금 해제해야 하는 기능과 병행됩니다.

Workfront 관리자가 시스템의 모든 그룹에 대한 타임시트 및 시간 환경 설정을 잠그거나 잠금 해제할 수 있는 방법에 대한 자세한 내용은 [타임시트 및 시간 환경 설정 구성](../../../administration-and-setup/set-up-workfront/configure-timesheets-schedules/timesheet-and-hour-preferences.md)을 참조하십시오.

그룹의 타임시트 및 시간 환경 설정을 구성하는 방법에 대한 자세한 내용은 [그룹의 타임시트 및 시간 환경 설정 구성](../../../administration-and-setup/manage-groups/create-and-manage-groups/configure-timesheet-hour-preferences-group.md)을 참조하십시오.

<!--
Unlike other Lock/Unlock articles that start just like this one, we need the steps here. In other areas, the lock/unlock step is part of the article about setting preferences or creating statuses.</p>
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

## 그룹 타임시트 및 시간 환경 설정 잠금 또는 잠금 해제

>[!TIP]
>
>Workfront 관리자인 경우 설정 > 타임시트 및 시간 > 환경 설정으로 이동한 다음 페이지 상단에 있는 상자에서 그룹 이름을 검색하여 1-4단계를 건너뛸 수 있습니다.

1. Adobe Workfront 오른쪽 상단의 **기본 메뉴** 아이콘 ![](assets/main-menu-icon.png)을(를) 클릭한 다음 **설정** ![](assets/gear-icon-settings.png)을(를) 클릭합니다.

1. 왼쪽 패널에서 **그룹**&#x200B;을 클릭합니다.
1. 타임시트 및 시간 환경 설정을 잠그거나 잠금 해제할 그룹의 이름을 클릭합니다.
1. 왼쪽 패널에서 **타임시트 및 시간 환경 설정**&#x200B;을 클릭합니다.

1. 표시되는 페이지에서 다음 중 하나를 수행합니다.

   * 그룹 아래의 그룹 관리자가 해당 그룹에 대한 환경 설정을 구성할 수 있도록 하려면 ![](assets/unlock-toggle-button.png) 잠금을 해제하세요.
   * 아래의 모든 그룹이 환경 설정에 대한 구성을 사용하도록 하려면 ![](assets/lock-toggle-button.png)이(가) 잠겨 있는지 확인하십시오(기본값).

     >[!IMPORTANT]
     >
     >잠긴 기본 설정을 구성하는 방식으로 모든 요구 사항을 처리할 수 있도록 아래 그룹의 관리자 및 사용자와 통신하는 것이 중요합니다. 이 구성을 잠그면 아래 하위 그룹에서 해당 구성을 상속합니다. 또한 환경 설정이 일정 기간 동안 잠금 해제된 경우 구성은 하위 그룹의 그룹 관리자가 수행한 작업을 대체합니다.

1. **저장**&#x200B;을 클릭합니다.
