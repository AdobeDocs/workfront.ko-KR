---
user-type: administrator
product-area: system-administration
keywords: 수정,이메일,알림,설정,일괄,일괄 편집,구성,다중,사용자
navigation-topic: emails-administration
title: 여러 사용자의 이메일 알림 설정 수정
description: 이 문서에서는 Workfront 또는 그룹 관리자가 다른 사용자의 이메일 알림을 업데이트하는 방법에 대한 정보를 제공합니다.
author: Nolan
feature: System Setup and Administration
role: Admin
exl-id: 658f97cd-0500-421d-9c89-26041ca59655
source-git-commit: ab774e937a15aaa04704e872579df880a9b80aaf
workflow-type: tm+mt
source-wordcount: '458'
ht-degree: 0%

---

# 여러 사용자의 이메일 알림 설정 수정

<!-- Audited: 12/2023 -->

Adobe Workfront 관리자이거나 다른 사용자의 설정을 편집할 수 있는 플래너 액세스 수준이 있는 경우 한 번에 여러 사용자에 대한 알림 설정을 구성할 수 있습니다. 여기에는 [Adobe Workfront 알림](../../../workfront-basics/using-notifications/wf-notifications.md)에 설명된 대로 이벤트 발생 시 또는 일일 다이제스트 전자 메일 하나로 알림을 받을지 여부를 지정하는 작업이 포함됩니다. 사용자 편집에 필요한 액세스 수준에 대한 자세한 내용은 [사용자에게 액세스 권한 부여](../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-other-users.md)를 참조하십시오.

자신의 프로필을 포함하여 한 번에 한 명의 사용자에 대한 이메일 알림을 구성할 수도 있습니다. 자세한 내용은 [전자 메일 알림 수정](../../../workfront-basics/using-notifications/activate-or-deactivate-your-own-event-notifications.md)을 참조하세요.


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
   <td> <p>새 플랜: 표준 </p>
 <p>또는</p> 
<p>현재 플랜: 플랜 </p> 
</td> 
  </tr> 
 </tbody> 
</table>

이 표의 정보에 대한 자세한 내용은 [Workfront 설명서의 액세스 요구 사항](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)을 참조하십시오.

+++

## 여러 사용자에 대한 이메일 알림 설정 수정

알림 설정을 대량으로 구성할 때 선택한 사용자가 공통으로 가지는 설정만 변경할 수 있습니다.

알림 설정을 수정하면 해당 알림 설정에 대해 **편집됨** 레이블이 표시되어 해당 알림 설정이 수정되었음을 알 수 있습니다.

여러 사용자에 대한 이메일 알림 설정을 수정하려면:

{{step-1-to-users}}

1. 사용자를 선택한 다음 **편집**&#x200B;을 클릭합니다.
1. 표시되는 **사용자 편집** 상자에서 **알림**&#x200B;을 클릭합니다.

1. 범주를 확장하여 해당 범주와 관련된 알림 설정을 봅니다.

   알림이 선택된 다른 사용자의 알림과 일치하지 않는 사용자를 한 명 이상 선택한 경우 해당 알림의 범주 확인란에 확인 표시 대신 가로줄 ![](assets/straight-line-instead-of-checkmark.jpg)이(가) 포함됩니다.


1. 사용자가 매일 또는 즉시 수신할 알림을 클릭하거나 수신을 중지할 알림을 지우십시오.

   >[!NOTE]
   >
   >   **Communication** 범주의 경우 인스턴트 배달에만 해당하는 개별 알림을 선택할 수 있습니다. 일별 요약으로 게재할 알림을 모두 선택해야 합니다.


1. 일별 요약으로 보낼 알림을 선택한 경우 **일별 요약 전자 메일 보내기** 메뉴에서 **알림** 섹션의 맨 위에 있는 요약으로 배달할 시간을 선택하십시오.

   ![](assets/daily-digest-time.png)

   일별 요약에는 선택한 시간보다 24시간 전에 알림 기준을 충족하는 이벤트가 포함됩니다. 사용자는 각 알림 유형에 대해 일별 요약 이메일을 1개씩 수신합니다.

   시스템에서 게재를 위해 큐에 올라가 있는 이메일 수에 따라, 선택한 시간 후에 일별 요약이 도착할 수 있습니다. 나열된 시간은 브라우저 설정에 지정된 현지 시간입니다.
