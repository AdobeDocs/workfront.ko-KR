---
user-type: administrator
product-area: system-administration;projects
navigation-topic: configure-system-defaults
title: 시스템의 모든 그룹에 대한 프로젝트 환경 설정 잠금 또는 잠금 해제
description: 조직의 그룹은 고유한 워크플로우에 대해 다르게 구성된 프로젝트 환경 설정이 필요할 수 있습니다. 조직 전체에서 모든 그룹에 대한 환경 설정을 잠금 해제하여 그룹 스스로 구성할 수 있습니다.
author: Lisa
feature: System Setup and Administration
role: Admin
exl-id: f5a94eaf-ebb8-424b-80ff-ba40cc985a6e
source-git-commit: 612243e928c6053d9b02715d9fcfef4dae25cb7a
workflow-type: tm+mt
source-wordcount: '532'
ht-degree: 0%

---

# 시스템의 모든 그룹에 대한 프로젝트 환경 설정 잠금 또는 잠금 해제

조직의 그룹은 고유한 워크플로우에 대해 다르게 구성된 프로젝트 환경 설정이 필요할 수 있습니다. 조직 전체에서 모든 그룹에 대한 환경 설정을 잠금 해제하여 그룹 스스로 구성할 수 있습니다.

기본 설정이 잠금 해제되고 그룹 관리자가 기본 설정을 수정하면 그룹과 관련된 프로젝트가 시스템 수준 설정이 아닌 그룹 수준 설정에서 해당 기본 설정에 대한 구성을 가져옵니다.

## 액세스 요구 사항

+++ 을 확장하여 이 문서의 기능에 대한 액세스 요구 사항을 봅니다.

이 문서의 단계를 수행하려면 다음 액세스 권한이 있어야 합니다.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] 플랜</td> 
   <td>임의</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] 라이센스</td> 
   <td><p>새로운 기능: [!UICONTROL Standard]</p>
   또는
   <p>현재: [!UICONTROL Plan]</p>
   </td> 
  </tr>
  <tr> 
   <td role="rowheader">액세스 수준 구성</td>
   <td>[!UICONTROL 시스템 관리자]</td> 
  </tr> 
 </tbody> 
</table>

이 표의 정보에 대한 자세한 내용은 [Workfront 설명서의 액세스 요구 사항](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)을 참조하십시오.

+++

## 잠금 및 잠금 해제된 환경 설정 정보

시스템 수준에서 구성한 프로젝트, 작업 또는 문제 환경 설정을 잠그면 모든 사람이 해당 환경 설정에 대해 동일한 설정을 사용할 수 있습니다. 잠근 환경 설정을 다시 구성할 수는 있지만 그룹 관리자는 해당 그룹에 대해 환경 설정을 다시 구성할 수는 없습니다.

반대로 프로젝트, 작업 또는 문제 환경 설정을 잠금 해제하면 그룹 관리자가 해당 항목을 사용하여 그룹이 작동하는 방식을 보다 유연하게 관리할 수 있습니다. 환경 설정이 잠금 해제되면 그룹 관리자는 해당 그룹에 대해 환경 설정을 다시 구성할 수 있습니다.

필드에 잠금/잠금 해제 토글이 없으면 그룹 관리자가 그룹 수준에서 설정을 구성할 수 있도록 잠금 해제할 수 없습니다. 구성은 시스템 수준에서만 사용할 수 있습니다.

시스템 수준 프로젝트, 작업 또는 문제 환경 설정을 잠그거나 잠금 해제하는 방법에 대한 지침은 [시스템 전체 작업 및 문제 환경 설정 구성](../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-task-issue-preferences.md)을 참조하십시오.

>[!NOTE]
>
>[!DNL Workfront] 관리자가 시스템 수준에서 환경 설정을 잠금 해제하면 모든 그룹 관리자가 이를 구성한 다음 잠가 그룹의 모든 사용자와 아래의 하위 그룹이 동일한 구성을 사용하도록 할 수 있습니다. 이는 [!DNL Workfront] 관리자가 시스템 내의 모든 사용자에 대한 환경 설정을 구성하고 잠그는 기능과 비슷합니다. 자세한 내용은 [그룹에 대한 프로젝트 환경 설정 구성](../../../administration-and-setup/manage-groups/create-and-manage-groups/configure-project-preferences-group.md) 및 [하위 그룹에 대한 프로젝트, 작업 또는 문제 환경 설정 잠금 또는 잠금 해제](../../../administration-and-setup/manage-groups/create-and-manage-groups/lock-or-unlock-a-group-preference.md)를 참조하십시오.

## 그룹이 구성할 수 있도록 프로젝트 환경 설정 잠금 해제

{{step-1-to-setup}}

1. **[!UICONTROL 프로젝트 환경 설정]**&#x200B;을 클릭한 다음 **[!UICONTROL 프로젝트]**&#x200B;을 클릭합니다.

1. 다음 중 하나를 수행합니다.

   * 그룹 관리자가 그룹의 환경 설정을 구성할 수 있도록 하려면 ![잠금 해제 토글](assets/unlock-toggle-button.png)을 잠금 해제하세요.
   * 모든 그룹이 환경 설정에 대한 구성을 사용하도록 하려면 구성 설정이 잠겨 있는지(기본값) 확인합니다.

     >[!IMPORTANT]
     >
     >모든 요구 사항이 잠긴 기본 설정을 구성하는 방식으로 처리되도록 시스템 전체에서 그룹 관리자 및 사용자와 통신하는 것이 좋습니다. 이 구성을 잠그면 시스템의 모든 그룹에서 해당 구성을 상속합니다. 또한 환경 설정이 일정 기간 동안 잠금 해제된 경우 구성은 그룹 관리자가 수행했을 수 있는 설정을 대체합니다.

1. **[!UICONTROL 저장]**&#x200B;을 클릭합니다.
