---
user-type: administrator
product-area: system-administration;user-management
navigation-topic: organization-setup
title: 작업 역할 삭제
description: 조직에서 더 이상 사용하지 않는 작업 역할을 삭제할 수 있습니다. 작업 역할이 과거에 작업 항목과 연결된 경우에는 삭제하지 않는 것이 좋습니다. 작업 할당에 대한 모든 내역 정보를 유지하려면 더 이상 사용되지 않는 역할을 삭제하는 대신 비활성화하는 것이 좋습니다. 역할 비활성화에 대한 자세한 내용은 작업 역할 비활성화를 참조하십시오.
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

조직에서 더 이상 사용하지 않는 작업 역할을 삭제할 수 있습니다. 작업 역할이 과거에 작업 항목과 연결된 경우에는 삭제하지 않는 것이 좋습니다.

작업 할당에 대한 모든 내역 정보를 유지하려면 더 이상 사용되지 않는 역할을 삭제하는 대신 비활성화하는 것이 좋습니다. 역할 비활성화에 대한 자세한 내용은 [작업 역할 비활성화](../../../administration-and-setup/set-up-workfront/organizational-setup/deactivate-job-roles.md)를 참조하십시오.

## 액세스 요구 사항

다음 항목이 있어야 합니다.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] 플랜*</td> 
   <td> <p>임의 </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] 라이센스*</td> 
   <td>[!UICONTROL 계획]</td> 
  </tr> 
  <tr> 
   <td role="rowheader">액세스 수준 구성*</td> 
   <td> <p>작업 역할에 대한 관리 액세스</p> <p><b>참고</b>: 아직 액세스 권한이 없는 경우 [!DNL Workfront] 관리자에게 액세스 수준에 추가 제한을 설정했는지 문의하세요. [!DNL Workfront] 관리자가 액세스 수준을 수정하는 방법에 대한 자세한 내용은 <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">사용자 지정 액세스 수준 만들기 또는 수정</a>을 참조하십시오.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;플랜, 라이선스 유형 또는 액세스 권한을 확인하려면 [!DNL Workfront] 관리자에게 문의하세요.

## 작업 역할 삭제

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: this moved from create and manage job roles)</p>
-->

1. [!DNL Adobe Workfront]의 오른쪽 위 모서리에 있는 **[!UICONTROL 기본 메뉴]** 아이콘 ![](assets/main-menu-icon.png)을 클릭한 다음 **[!UICONTROL 설정]** ![](assets/gear-icon-settings.png)을 클릭합니다.

1. **[!UICONTROL 작업 역할].**&#x200B;을 클릭합니다.
1. 삭제할 작업 역할을 선택한 다음 **[!UICONTROL 삭제].**&#x200B;를 클릭합니다
1. 작업 역할에 할당된 개체(사용자, 작업, 문제)가 있는 경우 다음 중 하나를 수행합니다.

   * **작업 역할을 다른 작업 역할로 바꾸기:** 드롭다운 목록에서 새 작업 역할을 선택합니다.

     삭제된 작업 역할과 연결된 현재 및 과거 리소스 할당은 선택한 작업 역할로 전송됩니다.

     작업 역할이 한 개만 할당된 사용자는 선택한 작업 역할에 재할당되고, 보조 작업 역할이 할당된 사용자는 선택한 작업 역할에 재할당되지 않습니다.

   * **작업 역할과 해당 리소스 할당을 삭제합니다.** 드롭다운 목록에서 **[!UICONTROL 없음]**&#x200B;을 선택합니다.

     >[!IMPORTANT]
     >
     >작업 역할을 삭제하면 모든 프로젝트에 대해 해당 작업 역할과 관련된 현재 및 과거 리소스 할당이 모두 삭제됩니다.

     예를 &#x200B; 들어 작업 또는 문제가 해당 작업 역할에만 할당된 경우 작업 역할이 삭제된 후에는 작업 또는 문제가 할당 해제됩니다.

1. **[!UICONTROL 예, 삭제]**&#x200B;를 클릭합니다.
