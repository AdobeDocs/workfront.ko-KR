---
user-type: administrator
product-area: system-administration
navigation-topic: create-custom-status-and-priority-labels
title: 사용자 지정 상태 삭제
description: 사용자 지정 시스템 상태가 더 이상 조직에 유용하지 않을 경우 삭제할 수 있습니다.
author: Caroline
feature: System Setup and Administration
role: Admin
exl-id: 73c4eb87-94f6-47bf-b447-eb02a703f7ef
source-git-commit: f2f825280204b56d2dc85efc7a315a4377e551c7
workflow-type: tm+mt
source-wordcount: '486'
ht-degree: 1%

---

# 사용자 지정 상태 삭제

사용자 지정 시스템 상태가 더 이상 조직에 유용하지 않을 경우 삭제할 수 있습니다.

상태가 잠기는지 잠금 해제되었는지에 따라 시스템의 모든 그룹에 대해 상태가 삭제되었는지 여부가 결정됩니다.

* 현재 잠긴 시스템 상태를 삭제하면 그룹의 이름이 변경되었는지 여부에 관계없이 시스템의 모든 그룹에 대해 상태가 제거됩니다.
* 반대로 현재 잠금이 해제된 시스템 상태를 삭제하면 시스템의 모든 그룹에 대해 상태가 유지됩니다.


>[!NOTE]
>
>다음 항목은 삭제할 수 없습니다.
>
>* 시스템 승인 프로세스에 사용되는 잠김 또는 잠금 해제된 시스템 상태로서 시스템에 있는 하나 이상의 객체에 대한 현재 승인 대기 중입니다.
>
>  그러나 현재 승인 보류 중인 단일 사용 또는 그룹 수준 승인 프로세스에서 사용되는 잠금 해제된 시스템 상태를 삭제할 수 있습니다.
>
>  보고서를 실행하여 객체를 찾고 보류 중인 승인을 확인한 다음 상태를 다시 삭제해 볼 수 있습니다. 자세한 내용은 [특정 상태를 사용하여 대기 중인 승인 프로세스를 사용하여 객체 나열](../../../administration-and-setup/customize-workfront/creating-custom-status-and-priority-labels/list-objects-pending-approval-certain-status.md).
>
>* 시스템에 있는 하나 이상의 객체에 대한 현재 승인 보류 중인 승인 프로세스에 사용되는 상태입니다.


그룹 상태 삭제에 대한 지침은 [그룹 상태 삭제](../../../administration-and-setup/manage-groups/manage-group-statuses/delete-a-group-status.md).

## 액세스 요구 사항

이 문서의 절차를 수행하려면 다음 액세스 권한이 있어야 합니다.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront 플랜</td> 
   <td>모든</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront 라이선스</td> 
   <td>플랜</td> 
  </tr> 
  <tr> 
   <td role="rowheader">액세스 수준 구성</td> 
   <td> <p>Workfront 관리자여야 합니다.</p> <p><b>참고</b>: 여전히 액세스 권한이 없는 경우 Workfront 관리자에게 액세스 수준에서 추가 제한 사항을 설정하는지 문의하십시오. Workfront 관리자가 액세스 수준을 수정하는 방법에 대한 자세한 내용은 <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">사용자 정의 액세스 수준 만들기 또는 수정</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

## 사용자 지정 시스템 상태 삭제

1. 을(를) 클릭합니다. **기본 메뉴** 아이콘 ![](assets/main-menu-icon.png) Adobe Workfront의 오른쪽 위 모서리에서 을(를) 클릭하고 **설정** ![](assets/gear-icon-settings.png).

1. 왼쪽 패널에서 **프로젝트 환경 설정** > **상태**.

1. 전체 시스템(개별 그룹에 대해 포함)에서 상태를 삭제하려면 상태 위에 마우스를 놓고 **편집**, 그런 다음 **모든 그룹에 대한 잠금** 이 선택되어 있습니다. **저장**&#x200B;을 클릭합니다.

   또는

   시스템 상태를 삭제하지만 개별 그룹에 대해 해당 상태를 유지하려면 마우스를 상태 위에 올린 후 **편집**, 그런 다음 **모든 그룹에 대한 잠금** 이 선택되어 있지 않습니다. **저장**&#x200B;을 클릭합니다.

1. 삭제할 상태를 마우스로 가리킨 다음 **삭제**.
1. 표시되는 메시지에서 **삭제 상태**.
1. 에서 **삭제 상태** 표시되는 상자에서, 필드의 상태를 **현재 이 상태의 모든 프로젝트를 로 설정합니다.**.

   삭제 중인 상태를 사용한 프로젝트는 선택한 상태로 설정됩니다.

   삭제 중인 상태와 동일한 상태에 해당하는 경우에만 드롭다운 목록에서 상태를 사용할 수 있습니다.

   예를 들어, 현재 상태 와 같은 상태를 삭제하는 경우 현재 상태 와 같은 상태만 선택할 수 있습니다.

1. 클릭 **삭제 상태**.
