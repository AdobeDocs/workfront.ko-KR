---
user-type: administrator
product-area: system-administration
navigation-topic: emails-administration
title: 모든 그룹에 대한 이벤트 알림 구성 잠금 해제 또는 잠금
description: Adobe Workfront 관리자인 경우 그룹 관리자가 관리하는 최상위 그룹에 대한 이벤트 알림을 구성할 수 있는 기능을 잠금 해제하거나 다시 잠글 수 있습니다. 이벤트 알림의 구성은 활성화 또는 비활성화로 구성됩니다.
author: Lisa, Nolan
feature: System Setup and Administration
role: Admin
exl-id: 056d76c1-7e9b-49b9-974a-75765e53b7fd
source-git-commit: ab774e937a15aaa04704e872579df880a9b80aaf
workflow-type: tm+mt
source-wordcount: '544'
ht-degree: 0%

---

# 모든 그룹에 대한 이벤트 알림 구성 잠금 해제 또는 잠금

Adobe Workfront 관리자인 경우 그룹 관리자가 관리하는 최상위 그룹에 대한 이벤트 알림을 구성할 수 있는 기능을 잠금 해제하거나 다시 잠글 수 있습니다. 이벤트 알림의 구성은 활성화 또는 비활성화로 구성됩니다.

관리하는 그룹 위에 그룹이 있는 경우 해당 관리자는 해당 그룹에 대해 이 작업을 수행할 수도 있습니다. Workfront 관리자(모든 그룹)의 경우도 마찬가지입니다.

관리자가 그룹에 대한 이벤트 알림을 구성할 때 이 구성은 해당 그룹 또는 하위 그룹 중 하나가 홈 그룹인 사용자에게 영향을 줍니다. 이러한 사용자는 사용자 프로필에서 시스템 전체에서 활성화된 이벤트 알림 대신 홈 그룹에 대해 활성화된 이벤트 알림을 보게 됩니다. 자세한 내용은 [그룹에 대한 이벤트 알림 보기 및 구성](../../../administration-and-setup/manage-groups/create-and-manage-groups/view-and-configure-event-notifications-group.md)을 참조하세요.

>[!NOTE]
>
>* Workfront 관리자는 Adobe Workfront Classic과 새 Adobe Workfront 경험 모두에서 이벤트 알림에 대한 구성을 잠금 해제하고 다시 잠글 수 있습니다. 하지만 그룹 관리자는 새 Adobe Workfront 경험에서만 그룹에 대한 이벤트 알림을 구성할 수 있습니다. Adobe Workfront Classic을 사용하는 그룹 관리자는 새로운 Adobe Workfront 환경으로 전환하여 그룹에 대해 잠금 해제된 이벤트 알림을 구성한 다음 Adobe Workfront Classic으로 다시 전환하여 변경 사항을 확인할 수 있습니다.
>* 하위 그룹은 그룹 위의 최상위 그룹에서 그룹 수준 이벤트 알림 구성을 상속합니다.
>

## 액세스 요구 사항

+++ 을 확장하여 이 문서의 기능에 대한 액세스 요구 사항을 봅니다.

이 문서의 단계를 수행하려면 다음 액세스 권한이 있어야 합니다.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront 플랜</td> 
   <td>임의</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront 라이선스</td> 
   <td>플랜</td> 
  </tr> 
  <tr> 
   <td role="rowheader">액세스 수준 구성</td> 
   <td> <p>시스템 관리자</p> </td> 
  </tr> 
 </tbody> 
</table>

+++

## 이벤트 알림 구성 기능 잠금 해제 또는 재잠금

>[!IMPORTANT]
>
>알림을 다시 잠그면 시스템의 모든 그룹은 사용자가 설정한 대로 알림을 상속합니다. 이는 그룹 관리자가 그룹에 대해 수행한 모든 변경 사항을 무시하므로 먼저 그룹과 협의하는 것이 좋습니다.

{{step-1-to-setup}}

1. **전자 메일** > **알림**&#x200B;을 클릭합니다.

1. **이벤트 알림** 탭이 열려 있는지 확인하십시오.
1. 알림 오른쪽에 있는 아이콘을 클릭하여 잠긴 ![잠금 아이콘](assets/lock-toggle-button.png) 또는 잠금 해제된 ![잠금 해제 아이콘](assets/unlock-toggle-button.png) 위치로 전환하십시오.

   또는

   여러 알림을 한 번에 잠금 해제하거나 잠그려면 해당 알림을 선택한 다음 목록 위의 도구 모음에 표시되는 ![잠금 해제 아이콘](assets/unlock-icon-toolbar.png) 또는 ![잠금 아이콘](assets/lock-icon-locked-qs.png) 잠금 버튼을 클릭합니다.

1. **저장**&#x200B;을 클릭합니다.
1. (선택 사항) 이 작업을 그룹 관리자에게 맡기는 대신 최상위 그룹에 대한 이벤트 알림을 구성하려면 다음 중 하나를 수행할 수 있습니다.

   * 알림 목록 위의 검색 상자에서 **시스템 이벤트 알림**&#x200B;을 삭제하고, 알림을 나열할 최상위 그룹의 이름을 검색하여 선택한 다음 표시되는 목록에서 잠금 해제된 알림을 활성화하거나 비활성화합니다.
   * 왼쪽 메뉴에서 **그룹**&#x200B;을 클릭한 다음 최상위 그룹의 이름을 클릭합니다. [그룹에 대한 이벤트 알림 보기 및 구성](../../../administration-and-setup/manage-groups/create-and-manage-groups/view-and-configure-event-notifications-group.md)에 설명된 대로 왼쪽 패널에서 **이벤트 알림**&#x200B;을 클릭한 다음 잠금 해제된 이벤트 알림을 구성하십시오.
