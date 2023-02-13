---
user-type: administrator
product-area: system-administration;projects
navigation-topic: configure-system-defaults
title: 시스템의 모든 그룹에 대한 프로젝트 환경 설정 잠금 또는 잠금 해제
description: 조직의 그룹은 고유한 워크플로우에 대해 다르게 구성된 프로젝트 환경 설정이 필요할 수 있습니다. 조직 전체에서 모든 그룹에 대한 기본 설정을 잠금 해제하여 자신이 직접 구성할 수 있습니다.
author: Caroline
feature: System Setup and Administration
role: Admin
exl-id: f5a94eaf-ebb8-424b-80ff-ba40cc985a6e
source-git-commit: 2fd772ffc667c4f32c6a7b0de9c87676ee6dd65b
workflow-type: tm+mt
source-wordcount: '518'
ht-degree: 0%

---

# 시스템의 모든 그룹에 대한 프로젝트 환경 설정 잠금 또는 잠금 해제

조직의 그룹은 고유한 워크플로우에 대해 다르게 구성된 프로젝트 환경 설정이 필요할 수 있습니다. 조직 전체에서 모든 그룹에 대한 기본 설정을 잠금 해제하여 자신이 직접 구성할 수 있습니다.

기본 설정이 잠금 해제되어 그룹 관리자가 이를 수정하는 경우, 그룹과 연관된 프로젝트는 시스템 수준 설정이 아닌 그룹 수준 설정에서 해당 기본 설정에 대한 구성을 획득합니다.

## 액세스 요구 사항

이 문서의 절차를 수행하려면 다음 액세스 권한이 있어야 합니다.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] 플랜</td> 
   <td>모든</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] 라이선스</td> 
   <td>[!UICONTROL 계획]</td> 
  </tr> 
  <tr> 
   <td role="rowheader">액세스 수준 구성</td> 
   <td> <p>넌 [!DNL Workfront] 관리자</p> <p><b>참고</b>: 여전히 액세스할 수 없는 경우 [!DNL Workfront] 관리자가 액세스 수준에서 추가 제한을 설정한 경우 자세한 내용은 [!DNL Workfront] 관리자는 액세스 수준을 수정할 수 있습니다. <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">사용자 정의 액세스 수준 만들기 또는 수정</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

## 잠김 및 잠금 해제된 기본 설정 정보

시스템 수준에서 구성한 프로젝트, 작업 또는 문제 환경 설정을 잠그면 모든 사용자가 해당 기본 설정에 대해 동일한 설정을 사용할 수 있습니다. 잠그는 기본 설정을 다시 구성할 수는 있지만 그룹 관리자는 그룹 설정을 다시 구성할 수 없습니다.

반대로 프로젝트, 작업 또는 문제 환경 설정을 해제하면 그룹 관리자가 그룹 내에서 해당 항목이 작동하는 방식을 보다 유연하게 관리할 수 있습니다. 기본 설정 잠금이 해제되면 그룹 관리자는 그룹 그룹에 대해 다시 구성할 수 있습니다.

시스템 수준 프로젝트, 작업 또는 문제 환경 설정을 잠금 또는 잠금 해제하는 방법에 대한 지침은 [시스템 전체 작업 및 문제 환경 설정 구성](../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-task-issue-preferences.md).

>[!NOTE]
>
>후 [!DNL Workfront] 관리자는 시스템 수준에서 기본 설정을 잠금 해제하면 모든 그룹 관리자가 해당 설정을 구성한 다음 잠근 후 해당 그룹의 모든 사람과 아래 하위 그룹이 동일한 구성을 사용하도록 할 수 있습니다. 이것은 [!DNL Workfront] 관리자는 시스템의 모든 사용자에 대한 환경 설정을 구성하고 잠그어야 합니다. 자세한 내용은 [그룹에 대한 프로젝트 환경 설정 구성](../../../administration-and-setup/manage-groups/create-and-manage-groups/configure-project-preferences-group.md) 및 [하위 그룹에 대한 프로젝트, 작업 또는 문제 환경 설정 잠금 또는 잠금 해제](../../../administration-and-setup/manage-groups/create-and-manage-groups/lock-or-unlock-a-group-preference.md).

## 그룹이 프로젝트 기본 설정을 구성할 수 있도록 프로젝트 기본 설정의 잠금을 해제합니다

1. 을(를) 클릭합니다. **[!UICONTROL 기본 메뉴]** 아이콘 ![](assets/main-menu-icon.png) 의 오른쪽 위 모서리에서 [!DNL Adobe Workfront]를 클릭한 다음 **[!UICONTROL 설정]** ![](assets/gear-icon-settings.png).

1. 클릭 **[!UICONTROL 프로젝트 환경 설정]**&#x200B;를 클릭한 다음 **[!UICONTROL 프로젝트]**.

1. 다음 중 하나를 수행합니다.

   * 그룹 관리자가 해당 그룹에 대한 환경 설정을 구성할 수 있도록 하려면 그룹 잠금을 해제하십시오 ![](assets/unlock-toggle-button.png).
   * 모든 그룹이 기본 설정에 대한 구성을 사용하려면 구성이 잠겼는지 확인합니다(기본값).

      >[!IMPORTANT]
      >
      >잠긴 기본 설정을 구성하는 방식으로 모든 요구 사항을 처리하도록 시스템 전체에서 관리자 및 그룹의 사용자와 통신하는 것이 좋습니다. 잠글 때 시스템의 모든 그룹에 의해 구성이 상속됩니다. 그리고 특정 기간 동안 기본 설정 잠금이 해제되어 있으면 해당 그룹 관리자가 만들 수 있는 구성 대신

1. **[!UICONTROL 저장]**&#x200B;을 클릭합니다.
