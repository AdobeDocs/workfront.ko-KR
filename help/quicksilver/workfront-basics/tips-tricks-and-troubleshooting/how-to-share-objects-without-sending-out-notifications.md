---
content-type: tips-tricks-troubleshooting
navigation-topic: tips-tricks-and-troubleshooting-workfront-basics
title: 알림을 생성하지 않고 오브젝트를 공유하는 방법
description: 오브젝트를 공유하고 이 변경 내용에 대한 알림이 전송되지 않도록 하는 방법을 알아봅니다. 이 기능은 개체를 대량으로 공유할 때 특히 유용합니다.
author: Alina
feature: Get Started with Workfront
source-git-commit: b14dd633edec3e9746f7f1412445b74bcd37a676
workflow-type: tm+mt
source-wordcount: '590'
ht-degree: 4%

---


# 알림을 생성하지 않고 오브젝트를 공유하는 방법

<!--Audited: 12/2024-->

Adobe Workfront에서 오브젝트를 공유하면 오브젝트를 공유하는 사람들이 공유에 대한 이메일 알림을 받습니다.

다른 사용자가 개체를 귀하와 공유할 때 이메일 알림을 받는 것은 이러한 변경 사항을 알고 있어야 합니다. 하지만 알림이 너무 많으면 사용자에게 너무 혼란스러울 수 있습니다. 한 번에 많은 개체를 사용자와 공유하려는 경우 알림을 일시적으로 비활성화하면 혼동을 피할 수 있습니다.

사용자는 다음 설정을 동시에 활성화하면 이메일 알림을 받습니다.

* 다음 이벤트 알림 중 하나 또는 둘 다가 시스템 또는 그룹 수준에서 활성화됩니다.

   * 사용자에게 오브젝트 공유
   * 팀에 대한 개체 공유는 시스템 또는 그룹 수준에서 사용할 수 있습니다.
* 다음 이메일 알림 중 하나 또는 둘 다가 사용자의 프로필에서 활성화됩니다.

   * 누군가 나와 오브젝트를 공유합니다.
   * 누군가가 내 팀과 오브젝트를 공유합니다.

여러 명의 사용자와 여러 오브젝트를 공유해야 하지만(일괄) 이 변경 사항에 대한 이메일 알림을 받지 않도록 하려면 다음을 수행하십시오.

## 액세스 요구 사항

+++ 을 확장하여 이 문서의 기능에 대한 액세스 요구 사항을 봅니다.

객체를 공유하려면 다음 항목이 있어야 합니다.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront 플랜</td> 
   <td> <p>임의 </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront 라이센스*</td> 
   <td> <p>새 라이선스: Standard</p> 
   또는
   <p>현재 라이선스: 플랜</p>
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader">액세스 수준 구성</td> 
   <td> <p>공유할 개체에 대한 액세스 이상의 보기</p>
   <p>사용자에 대한 액세스 권한 편집</p>
   <p><b>메모</b></p>
   <p> 시스템 또는 그룹에 대한 이벤트 알림의 상태를 확인하려면 시스템 또는 그룹 관리자여야 합니다</p>
    </td> 
  </tr> 
  <tr> 
   <td role="rowheader">개체 권한</td> 
   <td> <p>공유할 개체에 대한 권한 이상 보기</p></td> 
  </tr> 
 </tbody> 
</table>

*자세한 내용은 [Workfront 설명서의 액세스 요구 사항](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)을 참조하십시오.

+++

## 알림을 생성하지 않고 오브젝트 공유

1. 다음 **이벤트 알림**&#x200B;이 시스템 또는 그룹 수준에서 활성화되어 있는지 확인하십시오.

   * **사용자에게 개체 공유**
   * **팀에 대한 개체 공유를 시스템 또는 그룹 수준에서 사용할 수 있습니다**.

   자세한 내용은 [시스템의 모든 사용자를 위한 이벤트 알림 구성](/help/quicksilver/administration-and-setup/manage-workfront/emails/configure-event-notifications-for-everyone-in-the-system.md)을 참조하십시오.

   이러한 이벤트 알림이 활성화되지 않으면 오브젝트 공유에 대한 알림이 사용자에게 전송되지 않습니다. 하나 또는 둘 다 활성화된 경우 다음 단계를 계속 진행합니다.

{{step-1-to-users}}

1. 목록에서 여러 사용자를 선택한 다음 **알림** > **기타**&#x200B;를 클릭합니다.
1. 시스템 또는 그룹 수준에서 사용할 수 있는 알림에 따라 다음 알림 중 하나 또는 모두를 비활성화합니다.

   * **다른 사용자가 나와 개체를 공유합니다**
   * **다른 사용자가 내 팀과 개체를 공유합니다**

   비활성화하기 전에 선택한 모든 사용자에게 이러한 알림이 선택되어 있는지 확인하십시오. 이렇게 하면 개체를 공유한 후 모든 개체에 대해 일괄적으로 다시 활성화할 수 있습니다.

1. **변경 내용 저장**&#x200B;을 클릭합니다.
1. 공유할 개체 목록으로 이동하여 개체를 선택한 다음 목록 맨 위에 있는 **공유** 아이콘을 클릭합니다.

   개체를 일괄 공유하는 방법에 대한 자세한 내용은 [개체 공유](/help/quicksilver/workfront-basics/grant-and-request-access-to-objects/share-an-object.md)를 참조하십시오.

1. 알림을 비활성화한 사용자 목록으로 돌아가서 동일한 사용자를 선택합니다.
1. 목록에서 동일한 사용자를 선택한 다음 **알림** > **기타**&#x200B;를 클릭합니다.
1. 다음 알림 중 하나 또는 모두를 활성화합니다(시스템 또는 그룹 수준에서 활성화된 알림에 따라).

   * **다른 사용자가 나와 개체를 공유합니다**
   * **다른 사용자가 내 팀과 개체를 공유합니다**

1. **변경 내용 저장**&#x200B;을 클릭합니다.

   객체는 선택한 사용자와 공유되었으며, 이 변경 사항에 대한 이메일 알림을 받은 사용자는 없습니다.






