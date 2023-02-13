---
product-area: user-management
navigation-topic: grant-and-request-access-to-objects
title: 홈 영역의 객체에 대한 액세스 권한 부여
description: 사용자는 Adobe Workfront 내의 개체에 대한 액세스를 요청할 수 있습니다. 액세스 요청에 대한 자세한 내용은 개체에 대한 액세스 요청 을 참조하십시오.
author: Alina
feature: Get Started with Workfront
exl-id: e0a69ed5-57c3-47ac-bb7a-65495f93b3e3
source-git-commit: dd7f61fcd92a43303be356dd3209ec6da6a063dd
workflow-type: tm+mt
source-wordcount: '466'
ht-degree: 0%

---

# 홈 영역의 객체에 대한 액세스 권한 부여

사용자는 Adobe Workfront 내의 개체에 대한 액세스를 요청할 수 있습니다. 액세스 요청에 대한 자세한 내용은  [개체에 대한 액세스 요청](../../workfront-basics/grant-and-request-access-to-objects/request-access.md).

객체의 소유자인 경우 홈 영역에서 항목에 대한 액세스를 부여하거나 거부할 수 있습니다.

## 액세스 요구 사항

<!--drafted for P&P:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront plan*</td> 
   <td> <p>Any</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront license*</td> 
   <td> <p>Current license: Standard</p> 
   Or
   <p>Legacy license: Work or higher</p>
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Access level configurations*</td> 
   <td> <p>View access or higher to projects, tasks, issues, or documents</p> <p><b>NOTE</b>
   
   If you still don't have access, ask your Workfront administrator if they set additional restrictions in your access level. For information on how a Workfront administrator can modify your access level, see <a href="../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Create or modify custom access levels</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Object permissions</td> 
   <td> <p>View permissions or higher to projects, tasks, issues, or documents</p> <p>For information on requesting additional access, see <a href="../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Request access to objects </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

-->

이 문서의 절차를 수행하려면 다음 액세스 권한이 있어야 합니다.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront 플랜*</td> 
   <td> <p>모든</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront 라이선스*</td> 
   <td> <p>작업 이상</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">액세스 수준 구성*</td> 
   <td> <p>프로젝트, 작업, 문제 또는 문서에 대한 액세스 이상의 보기</p> <p><b>메모</b>

여전히 액세스 권한이 없는 경우 Workfront 관리자에게 액세스 수준에서 추가 제한 사항을 설정하는지 문의하십시오. Workfront 관리자가 액세스 수준을 수정하는 방법에 대한 자세한 내용은 <a href="../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">사용자 정의 액세스 수준 만들기 또는 수정</a>.</p> </td>
</tr> 
  <tr> 
   <td role="rowheader">개체 권한</td> 
   <td> <p>프로젝트, 작업, 문제 또는 문서에 대한 권한 보기</p> <p>추가 액세스 요청에 대한 자세한 내용은 <a href="../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">개체에 대한 액세스 요청 </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;어떤 계획, 라이선스 유형 또는 액세스 권한을 보유하고 있는지 알아보려면 Workfront 관리자에게 문의하십시오.

## 홈 영역의 객체에 대한 액세스 권한 부여

1. 을(를) 클릭합니다. **홈** 아이콘 ![](assets/home-icon-30x29.png) Adobe Workfront의 왼쪽 위 모서리에서

   >[!NOTE]
   >
   >Workfront 관리자는 사용자 환경에서 홈 아이콘을 다음과 같이 변경할 수 있습니다.
   >
   >* 조직을 보여주기 위해 사용자 지정된 이미지로 바꿉니다. 이 경우 이 문서에 표시된 아이콘의 모양이 다릅니다.
   >* 연결된 페이지를 다른 페이지로 바꿉니다. 이 경우 **기본 메뉴** ![](assets/main-menu-icon.png) 페이지의 오른쪽 위 모서리에서 을(를) 클릭하고 **홈**.


1. 에서 **작업 목록**&#x200B;을 클릭하고, 관리할 액세스 요청을 선택합니다.\
   ![Screen_Shot_2018-07-02_at_11.35.29_AM.png](assets/screen-shot-2018-07-02-at-11.35.29-am-350x242.png)

1. 오른쪽 상단 모서리에서 액세스 권한 부여 단추를 클릭합니다.\
   요청한 액세스 유형에 따라 단추 이름이 변경됩니다. 예를 들어 요청자가 보기 액세스를 요청하는 경우 버튼은 **보기 액세스 권한 부여**.\
   ![Grant_Access_2.png](assets/grant-access-2-350x98.png)

1. (선택 사항) 요청된 액세스 수준을 다르게 설정하려면 액세스 권한 부여 단추 옆에 있는 화살표를 클릭하고 새 액세스 권한을 선택합니다.\
   액세스 권한이 부여되었음을 확인하는 메시지가 나타납니다.\
   또는\
   클릭 **무시** 액세스를 거부하려면\
   액세스가 무시되었음을 확인하는 메시지가 나타납니다.

## 요청에 대한 이메일 알림 구성

액세스 요청에 대한 이메일 알림을 수신하는지 여부를 구성할 수 있습니다. Workfront 관리자는 [시스템의 모든 사용자에 대한 이벤트 알림을 구성합니다](../../administration-and-setup/manage-workfront/emails/configure-event-notifications-for-everyone-in-the-system.md)).

1. 을(를) 클릭합니다. **기본 메뉴** 아이콘 ![](assets/main-menu-icon.png) Adobe Workfront의 오른쪽 위 모서리에서 을(를) 클릭하고 **설정** ![](assets/gear-icon-settings.png).

1. 클릭 **기본 설정**&#x200B;또는 환경 설정 섹션으로 스크롤합니다.
1. 에서 **다음의 경우에 이메일 보내기** 드롭다운 목록, 선택 또는 선택 취소 **누군가 내게 액세스를 요청합니다**&#x200B;다른 사용자가 자신에 대한 액세스를 요청할 때 이메일 알림을 수신할지 여부에 따라 다릅니다.

1. 클릭 **변경 내용 저장**.
