---
user-type: administrator
product-area: system-administration
keywords: 수정,이메일,알림,설정,일괄,일괄 편집,구성,다중,사용자
navigation-topic: emails-administration
title: 사용자 프로필의 이메일 알림 설정 수정
description: Adobe Workfront 관리자이거나 다른 사용자의 설정을 편집할 수 있는 플래너 액세스 수준이 있는 경우 한 번에 여러 사용자에 대한 알림 설정을 구성할 수 있습니다. 여기에는 Adobe Workfront 알림에 설명된 대로 이벤트 발생 시 또는 일별 다이제스트 이메일 하나로 알림을 수신하는지 여부를 지정하는 작업이 포함됩니다. 사용자 편집에 필요한 액세스 수준에 대한 자세한 내용은 사용자에게 액세스 권한 부여를 참조하십시오.
author: Lisa, Caroline
feature: System Setup and Administration
role: Admin
exl-id: 658f97cd-0500-421d-9c89-26041ca59655
source-git-commit: 4331917d133c52cf727f148b75a213853c1e5679
workflow-type: tm+mt
source-wordcount: '538'
ht-degree: 0%

---

# 사용자 프로필의 이메일 알림 설정 수정

Adobe Workfront 관리자이거나 다른 사용자의 설정을 편집할 수 있는 플래너 액세스 수준이 있는 경우 한 번에 여러 사용자에 대한 알림 설정을 구성할 수 있습니다. 여기에는 이벤트 발생에 따라 사용자가에서 설명한 대로 알림을 수신하는지 또는 일별 요약 이메일 하나에서 알림을 수신하는지 여부도 포함됩니다 [Adobe Workfront 알림](../../../workfront-basics/using-notifications/wf-notifications.md). 사용자 편집에 필요한 액세스 수준에 대한 자세한 내용은 [사용자에게 액세스 권한 부여](../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-other-users.md).

알림 설정을 대량으로 구성할 때 선택한 사용자가 공통으로 가지는 설정만 변경할 수 있습니다.

자신의 프로필을 포함하여 한 번에 한 명의 사용자에 대한 이메일 알림을 구성할 수도 있습니다. 자세한 내용은 [자체 이벤트 알림 활성화 또는 비활성화](../../../workfront-basics/using-notifications/activate-or-deactivate-your-own-event-notifications.md).

## 액세스 요구 사항

이 문서의 단계를 수행하려면 다음 액세스 권한이 있어야 합니다.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront 플랜*</td> 
   <td>모든</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront 라이센스*</td> 
   <td>플랜</td> 
  </tr> 
 </tbody> 
</table>

&#42;보유 중인 플랜 또는 라이선스 유형을 확인하려면 Workfront 관리자에게 문의하십시오.

## 여러 사용자의 이메일 알림 설정을 일괄적으로 수정

1. 다음을 클릭합니다. **메인 메뉴** 아이콘 ![](assets/main-menu-icon.png) Adobe Workfront의 오른쪽 상단에서 을(를) 클릭한 다음 **사용자** ![](assets/users-icon-in-main-menu.png). 사용자를 선택한 다음 **편집**.
1. 다음에서 **사용자 편집** 나타나는 상자에서 **알림**.

1. 범주를 확장하여 해당 범주와 관련된 알림 설정을 봅니다.

   알림이 선택된 다른 사용자의 알림과 일치하지 않는 사용자를 한 명 이상 선택한 경우 해당 알림의 범주 확인란에 가로줄이 표시됩니다 ![](assets/straight-line-instead-of-checkmark.jpg) 확인 표시 대신 사용할 수 있습니다.

1. 사용자가 매일 또는 즉시 수신할 알림을 클릭하거나 수신을 중지할 알림을 지우십시오.

   의 경우 **커뮤니케이션** 범주, 인스턴트 게재에 대해서만 개별 알림을 선택할 수 있습니다. 일별 요약으로 게재할 알림을 모두 선택해야 합니다.

   알림 설정을 수정할 때 레이블은 **편집됨** 은 해당 알림 설정에 대해 표시되어 해당 알림 설정이 수정되었음을 알려줍니다.

1. 일별 요약으로 보낼 알림을 선택한 경우, 요약의 맨 위에서 요약이 전달될 시간을 선택합니다. **알림** 의 섹션 **다음 이후 이메일 일일 요약:** 메뉴 아래의 제품에서 사용할 수 있습니다.

   배달 시간을 선택한 후 **다음 이후 이메일 일일 요약:** 상자가 표시되어 게재 시간이 편집되었음을 나타냅니다.

   일별 요약에는 선택한 시간보다 24시간 전에 알림 기준을 충족하는 이벤트가 포함됩니다. 사용자는 각 알림 유형에 대해 일별 요약 이메일을 1개씩 수신합니다.

   시스템에서 게재를 위해 큐에 올라가 있는 이메일 수에 따라, 선택한 시간 후에 일별 요약이 도착할 수 있습니다. 나열된 시간은 브라우저 설정에 지정된 현지 시간입니다.
