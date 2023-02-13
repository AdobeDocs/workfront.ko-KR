---
user-type: administrator
product-area: system-administration;user-management
navigation-topic: manage-group-statuses
title: 그룹 상태 삭제
description: 그룹 관리자는 관리 그룹이 시스템 수준에서 필수 또는 잠긴 상태로 구성되지 않았거나 계층의 상위 그룹에 대해 상태를 삭제할 수 있습니다.
author: Caroline
feature: System Setup and Administration, People Teams and Groups
role: Admin
exl-id: bfce0325-fe6e-459f-96ca-9a5c94c61ed3
source-git-commit: f2f825280204b56d2dc85efc7a315a4377e551c7
workflow-type: tm+mt
source-wordcount: '572'
ht-degree: 0%

---

# 그룹 상태 삭제

그룹 관리자는 관리 그룹이 시스템 수준에서 필수 또는 잠긴 상태로 구성되지 않았거나 계층의 상위 그룹에 대해 상태를 삭제할 수 있습니다.

관리하는 그룹 위에 그룹이 있으면 해당 관리자가 사용자 그룹을 위해 이 작업을 수행할 수도 있습니다. Workfront 관리자(모든 그룹의 경우)도 마찬가지입니다.

>[!NOTE]
>
>다음 항목은 삭제할 수 없습니다.
>
>* 기본 제공 상태 계획, 현재 및 완료 이름을 업데이트하고 색상을 편집하고 잠그거나 잠금 해제할 수 있지만 삭제할 수 없습니다.
>* 그룹 또는 해당 하위 그룹 중 하나에 연결된 하나 이상의 객체에 대한 승인 보류 중인 상태입니다.


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

## 그룹 상태 삭제

1. 을(를) 클릭합니다. **기본 메뉴** 아이콘 ![](assets/main-menu-icon.png) Adobe Workfront의 오른쪽 위 모서리에서 을(를) 클릭하고 **설정** ![](assets/gear-icon-settings.png).

1. 왼쪽 패널에서 **그룹**.
1. 최상위 수준 그룹의 이름을 클릭합니다.
1. 왼쪽 패널에서 **상태**.
1. 표시되는 상태 목록에서 삭제할 상태를 마우스로 가리킨 다음 을 클릭합니다 **삭제** 그것이 맨 오른쪽에 보일 때.

   ![](assets/hover-click-delete.jpg)

1. 표시되는 상자에서 삭제 중인 상태를 사용한 객체(프로젝트, 작업, 문제 및 승인 프로세스)의 교체 상태를 지정할 상태를 선택합니다.

   삭제 중인 상태와 동일한 상태만 사용할 수 있습니다. 예를 들어, 현재 상태와 동일한 상태를 삭제하는 경우 현재 상태와 동일한 상태만 볼 수 있습니다.

   또한 표시되는 상태는 삭제 중인 상태가 잠금 해제되었는지 아니면 잠겼는지에 따라 달라집니다.

   * **잠금이 해제된 경우**: 숨기지 않은 잠금 및 잠금 해제된 상태를 사용할 수 있습니다.

      하위 그룹에 대해 생성된 상태와 함께 시스템 수준 및 상위 수준 그룹에서 상속된 상태가 포함됩니다.

   * **잠겨있다면**: 다음 중 하나가 true입니다.

      * 잠겨있고 숨기지 않은 다른 상태가 있는 경우 이러한 상태만 사용할 수 있습니다.
      * 잠기지 않은 잠금이 없는 상태가 없는 경우 숨겨진 상태이거나 잠금 해제된 경우에도 기본 Workfront 상태를 사용할 수 있습니다.

         기본 Workfront 상태에 대한 자세한 내용은 [시스템 프로젝트 상태 목록에 액세스합니다](../../../administration-and-setup/customize-workfront/creating-custom-status-and-priority-labels/project-statuses.md), [시스템 작업 상태 목록에 액세스합니다](../../../administration-and-setup/customize-workfront/creating-custom-status-and-priority-labels/task-statuses.md), 및에서 4개의 필요한 문제 상태에 대한 정보 [시스템 문제 상태 목록에 액세스합니다](../../../administration-and-setup/customize-workfront/creating-custom-status-and-priority-labels/issue-statuses.md).

1. 클릭 **삭제 상태**.

   삭제된 상태가 그룹의 해당 유형의 기본 상태이면 교체 상태가 적용됩니다.

   삭제된 상태가 프로젝트 기본 설정에서 기본 프로젝트 상태로 설정된 경우 이제 기본 설정이 교체 상태로 설정됩니다.

## 그룹이 삭제될 때

그룹이 삭제되어 다른 그룹으로 대체되면 삭제된 그룹이 가지는 모든 고유 상태가 교체 그룹의 상태에 추가됩니다. 자세한 내용은 [이동 또는 삭제된 그룹의 사용자 지정 상태](../../../administration-and-setup/manage-groups/manage-group-statuses/custom-statuses-in-group-moved-or-deleted.md).
