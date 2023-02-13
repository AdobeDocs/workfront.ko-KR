---
user-type: administrator
product-area: system-administration
keywords: 수정,전자 메일,알림,설정,벌크,대량 편집,구성,다중,사용자
navigation-topic: emails-administration
title: 사용자 프로필에서 전자 메일 알림 설정 수정
description: Adobe Workfront 관리자이거나 다른 사용자의 설정을 편집할 수 있는 계획자 액세스 레벨이 있는 경우에는 한 번에 여러 사용자에 대한 통지 설정을 구성할 수 있습니다. 여기에는 Adobe Workfront 알림에 설명된 대로 사용자가 이벤트를 수신하는지 또는 일별 다이제스트 이메일을 수신하는지 여부를 지정할 수 있습니다. 사용자를 편집하는 데 필요한 액세스 수준에 대한 자세한 내용은 사용자에게 액세스 권한 부여 를 참조하십시오.
author: Lisa, Caroline
feature: System Setup and Administration
role: Admin
exl-id: 658f97cd-0500-421d-9c89-26041ca59655
source-git-commit: 730932f6c8d4658273dd943e464a038828d288e9
workflow-type: tm+mt
source-wordcount: '534'
ht-degree: 0%

---

# 사용자 프로필에서 전자 메일 알림 설정 수정

Adobe Workfront 관리자이거나 다른 사용자의 설정을 편집할 수 있는 계획자 액세스 레벨이 있는 경우에는 한 번에 여러 사용자에 대한 통지 설정을 구성할 수 있습니다. 여기에는 다음에 설명된 대로 사용자가 이벤트 발생으로 알림을 수신하는지, 또는 일별 다이제스트 이메일에서 알림을 수신하는지 여부를 지정할 수 있습니다. [Adobe Workfront 알림](../../../workfront-basics/using-notifications/wf-notifications.md). 사용자를 편집하는 데 필요한 액세스 수준에 대한 자세한 내용은 [사용자에게 액세스 권한 부여](../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-other-users.md).

알림 설정을 일괄적으로 구성할 때는 선택한 사용자가 가지는 공통 설정만 변경할 수 있습니다.

한 번에 한 사용자에 대한 이메일 알림을 구성할 수도 있습니다. 자세한 내용은 [고유한 이벤트 알림 활성화 또는 비활성화](../../../workfront-basics/using-notifications/activate-or-deactivate-your-own-event-notifications.md).

## 액세스 요구 사항

이 문서의 절차를 수행하려면 다음 액세스 권한이 있어야 합니다.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront 플랜*</td> 
   <td>모든</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront 라이선스*</td> 
   <td>플랜</td> 
  </tr> 
 </tbody> 
</table>

&#42;보유하고 있는 플랜 또는 라이선스 유형을 확인하려면 Workfront 관리자에게 문의하십시오.

## 여러 사용자의 이메일 알림 설정을 일괄적으로 수정합니다

1. 을(를) 클릭합니다. **기본 메뉴** 아이콘 ![](assets/main-menu-icon.png) Adobe Workfront의 오른쪽 위 모서리에서 을(를) 클릭하고 **사용자** ![](assets/users-icon-in-main-menu.png). 사용자를 선택한 다음 를 클릭합니다 **편집**.
1. 에서 **개인 편집** 표시되는 상자를 클릭합니다. **알림 을 참조하십시오**.

1. 카테고리를 확장하여 해당 카테고리와 관련된 알림 설정을 봅니다.

   알림이 선택된 다른 사용자의 알림과 일치하지 않는 사용자를 한 명 이상 선택한 경우 해당 알림의 카테고리 확인란에 가로줄이 포함됩니다 ![](assets/straight-line-instead-of-checkmark.jpg) 확인 표시 대신

1. 사용자가 매일 또는 즉시 받을 알림을 클릭하거나, 사용자가 수신하지 못하도록 할 알림을 지웁니다.

   대상 **통신** 카테고리에서는 인스턴트 게재에만 사용할 개별 알림을 선택할 수 있습니다. 일별 다이제스트에 전달할 모든 알림을 선택해야 합니다.

   알림 설정을 수정할 때 레이블은 **편집됨** 알림 설정이 수정되었음을 알리는 해당 알림 설정에 대해 나타납니다.

1. 일별 다이제스트로 전송할 알림을 선택한 경우, 다이제스트를 일별 다이제스트 맨 위에서 전달할 시간을 선택합니다 **알림 을 참조하십시오** 의 섹션 **Email Daily Digest after** 메뉴 아래의 제품에서 사용할 수 있습니다.

   배달 시간을 선택한 후 **Email Daily Digest after** 상자는 게재 시간을 편집했음을 나타내는 주황색 프레임과 함께 표시됩니다.

   일별 다이제스트는 선택한 시간 24시간 전에 알림의 기준을 충족하는 이벤트를 포함합니다. 사용자는 각 알림 유형에 대해 일별 다이제스트 이메일 하나를 받습니다.

   일별 다이제스트는 시스템에서 전달을 위해 대기하는 이메일 수에 따라 사용자가 선택하는 시간 이후에 도착할 수 있습니다. 나열된 시간은 브라우저 설정에 지정된 현지 시간입니다.
