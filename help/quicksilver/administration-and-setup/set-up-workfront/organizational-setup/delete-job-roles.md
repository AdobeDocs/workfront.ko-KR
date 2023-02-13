---
user-type: administrator
product-area: system-administration;user-management
navigation-topic: organization-setup
title: 작업 역할 삭제
description: 조직에서 더 이상 사용하지 않는 작업 역할을 삭제할 수 있습니다. 작업 역할이 이전에 작업 항목과 연결된 경우에는 삭제하지 않는 것이 좋습니다. 작업 배정에 대한 모든 기록 정보를 보관하려면 역할을 삭제할 때 삭제하지 않고 비활성화하는 것이 좋습니다. 역할 비활성화에 대한 자세한 내용은 작업 역할 비활성화를 참조하십시오.
author: Caroline
feature: System Setup and Administration
role: Admin
exl-id: b0e81d76-5227-4fda-9a58-68fbce3f5b94
source-git-commit: b6f6964bb80f172849434c669df2b0ecd735a590
workflow-type: tm+mt
source-wordcount: '398'
ht-degree: 0%

---

# 작업 역할 삭제

조직에서 더 이상 사용하지 않는 작업 역할을 삭제할 수 있습니다. 작업 역할이 이전에 작업 항목과 연결된 경우에는 삭제하지 않는 것이 좋습니다.

작업 배정에 대한 모든 기록 정보를 보관하려면 역할을 삭제할 때 삭제하지 않고 비활성화하는 것이 좋습니다. 역할 비활성화에 대한 자세한 내용은 [작업 역할 비활성화](../../../administration-and-setup/set-up-workfront/organizational-setup/deactivate-job-roles.md).

## 액세스 요구 사항

다음 항목이 있어야 합니다.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] 플랜*</td> 
   <td> <p>모든 </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] 라이센스*</td> 
   <td>[!UICONTROL 계획]</td> 
  </tr> 
  <tr> 
   <td role="rowheader">액세스 수준 구성*</td> 
   <td> <p>작업 역할에 대한 관리자 액세스</p> <p><b>참고</b>: 여전히 액세스할 수 없는 경우 [!DNL Workfront] 관리자가 액세스 수준에서 추가 제한을 설정한 경우 자세한 내용은 [!DNL Workfront] 관리자는 액세스 수준을 수정할 수 있습니다. <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">사용자 정의 액세스 수준 만들기 또는 수정</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;어떤 계획, 라이센스 유형 또는 액세스 권한을 보유하고 있는지 확인하려면 [!DNL Workfront] 관리자

## 작업 역할 삭제

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: this moved from create and manage job roles)</p>
-->

1. 을(를) 클릭합니다. **[!UICONTROL 기본 메뉴]** 아이콘 ![](assets/main-menu-icon.png) 의 오른쪽 위 모서리에서 [!DNL Adobe Workfront]를 클릭한 다음 **[!UICONTROL 설정]** ![](assets/gear-icon-settings.png).

1. 클릭 **[!UICONTROL 작업 역할].**
1. 삭제할 작업 역할을 선택한 다음 **[!UICONTROL 삭제].**
1. 작업 역할에 할당된 객체(사용자, 작업, 문제)가 있는 경우 다음 중 하나를 수행합니다.

   * **작업 역할을 다른 작업 역할로 바꿉니다.** 드롭다운 목록에서 새 작업 역할을 선택합니다.

      삭제된 작업 역할과 연관된 현재 및 과거 리소스 할당이 선택한 작업 역할로 전송됩니다.

      한 개의 작업 역할만 할당된 사용자는 선택한 작업 역할에 재할당됩니다. 보조 작업 역할이 할당된 사용자는 선택한 작업 역할에 재할당되지 않습니다.

   * **작업 역할 및 해당 리소스 할당을 삭제합니다.** 선택 **[!UICONTROL 없음]** 드롭다운 목록에서 을 선택합니다.

      >[!IMPORTANT]
      >
      >작업 역할을 삭제하면 모든 프로젝트에 대해 해당 작업 역할과 관련된 현재 및 과거 리소스 할당이 모두 삭제됩니다.

      예&#x200B;을 들어 해당 작업 역할에만 작업 또는 문제가 할당되면 작업 역할이 삭제된 후 작업 또는 문제가 할당되지 않습니다.

1. 클릭  **[!UICONTROL 예, 삭제합니다.]**.
