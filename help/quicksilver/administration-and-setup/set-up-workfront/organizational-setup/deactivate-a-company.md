---
user-type: administrator
product-area: system-administration;user-management
navigation-topic: organization-setup
title: 회사 비활성화 또는 재활성화
description: 관련된 모든 내역 데이터를 유지하면서 더 이상 사용하지 않는 회사를 비활성화할 수 있습니다. 이미 사용 중인 회사를 시스템 어딘가에서 비활성화하면 항상 그랬던 것처럼 계속 작동합니다. 제거되거나 차단되지 않습니다.
author: Caroline
feature: System Setup and Administration
role: Admin
exl-id: 479dfb9d-0e47-4790-a33a-336b415fbf6e
source-git-commit: b6f6964bb80f172849434c669df2b0ecd735a590
workflow-type: tm+mt
source-wordcount: '410'
ht-degree: 0%

---

# 회사 비활성화 또는 재활성화

관련된 모든 내역 데이터를 유지하면서 더 이상 사용하지 않는 회사를 비활성화할 수 있습니다. 이미 사용 중인 회사를 시스템 어딘가에서 비활성화하면 항상 그랬던 것처럼 계속 작동합니다. 제거되거나 차단되지 않습니다.

## 액세스 요구 사항

[!DNL Workfront]에서 회사를 관리하려면 다음 항목이 있어야 합니다.

<table style="table-layout:auto"> 
 <col data-mc-conditions=""> 
 <col data-mc-conditions=""> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <p>[!DNL Workfront] 플랜*</p> </td> 
   <td>[!UICONTROL Team] 이상</td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!DNL Adobe Workfront] 라이센스*</p> </td> 
   <td>[!UICONTROL 계획]</td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader"><strong>액세스 수준 구성*</strong> </td> 
   <td> <p>다음 중 하나:</p> 
    <ul> 
     <li> <p>시스템에서 회사를 편집할 수 있는 [!UICONTROL 시스템 관리자] 액세스 수준입니다. 자세한 내용은 <a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-a-user-full-administrative-access.md" class="MCXref xref">사용자에게 전체 관리 액세스 권한 부여</a>를 참조하십시오. </p> </li> 
     <li> <p>회사 관리에 대한 관리 액세스 권한으로, 시스템에서 모든 회사를 편집할 수 있습니다. 자세한 내용은 <a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-users-admin-access-certain-areas.md" class="MCXref xref">특정 영역에 대한 관리자 액세스 권한 부여</a>를 참조하십시오.</p> </li> 
    </ul> <p><b>참고</b>:  
     <ul> 
      <li> <p>그룹 관리자로 할당된 모든 그룹과 연결된 회사를 관리할 수도 있습니다.</p> </li> 
      <li> <p>[!DNL Workfront] 시스템에 사용자를 추가하고 제거하려면 다음 중 하나가 있어야 합니다.</p> 
       <ul> 
        <li> <p>[!UICONTROL 시스템 관리자] 액세스 수준입니다. 자세한 내용은 <a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-a-user-full-administrative-access.md" class="MCXref xref">사용자에게 전체 관리 액세스 권한 부여</a>를 참조하십시오. </p> </li> 
        <li> <p>액세스 수준에서 [!UICONTROL 사용자] 설정에 대해 [!UICONTROL 편집]을 선택해야 합니다. 또한 [!UICONTROL 사용자] 설정의 경우 [!UICONTROL 설정 미세 조정] <img src="assets/gear-icon-in-access-levels.png">에서 [!UICONTROL 만들기] 옵션과 두 [!UICONTROL 사용자 관리] 옵션 중 하나 이상을 활성화해야 합니다. </p> <p> <img src="assets/access-req-users.png" style="width: 350;height: 101;"> </p> <p>[!UICONTROL 사용자 관리자(그룹 사용자)] 옵션을 사용하는 경우 사용자가 멤버인 그룹의 그룹 관리자여야 합니다.</p> </li> 
       </ul> <p>액세스 수준의 사용자 설정에 대한 자세한 내용은 <a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-other-users.md" class="MCXref xref">사용자에게 액세스 권한 부여</a>를 참조하십시오.</p> </li> 
     </ul> </p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;플랜, 라이선스 유형 또는 액세스 수준 구성을 확인하려면 [!DNL Workfront] 관리자에게 문의하세요.

## 회사 비활성화 또는 재활성화

1. [!DNL Adobe] Workfront의 오른쪽 위 모서리에 있는 **[!UICONTROL 기본 메뉴]** 아이콘 ![](assets/main-menu-icon.png)을(를) 클릭한 다음 **[!UICONTROL 설정]** ![](assets/gear-icon-settings.png)을(를) 클릭합니다.

1. 왼쪽 패널에서 **[!UICONTROL 회사]** ![](assets/companies-icon-left-panel.png)를 클릭합니다.

1. 비활성화하거나 다시 활성화할 회사를 하나 이상 선택하십시오.
1. **[!UICONTROL 편집]**&#x200B;을 클릭합니다.
1. 단일 회사의 경우 **[!UICONTROL 활성 상태임]** 옵션을 비활성화하여 비활성화하거나 옵션을 활성화하여 활성화하십시오.

   또는

   여러 회사의 경우 **[!UICONTROL 활성 상태임]** 드롭다운 메뉴에서 **[!UICONTROL 아니요]**&#x200B;를 선택하여 비활성화하거나 **[!UICONTROL 예]**&#x200B;를 선택하여 활성화하십시오.

1. **[!UICONTROL 변경 내용 저장]**&#x200B;을 클릭합니다.
