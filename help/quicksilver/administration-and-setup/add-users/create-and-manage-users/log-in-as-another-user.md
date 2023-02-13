---
title: 다른 사용자로 로그인
user-type: administrator
product-area: system-administration;user-management
navigation-topic: create-and-manage-users
description: Adobe Workfront 관리자로서 다른 사용자를 대신하여 Workfront에 액세스해야 하는 경우가 있습니다.
author: Caroline
feature: System Setup and Administration
role: Admin
exl-id: 2f8dd132-1086-4980-9b56-993a68231e96
source-git-commit: 7fa4791e19a84d7215e341e8bbde8dd4d4d8ccc6
workflow-type: tm+mt
source-wordcount: '809'
ht-degree: 0%

---

# 다른 사용자로 로그인

<!--
**DON'T DELETE, DRAFT OR HIDE THIS ARTICLE. IT IS LINKED TO THE PRODUCT, THROUGH THE CONTEXT SENSITIVE HELP LINKS. Also linked to other articles: Creating and Managing Groups, etc.</p>
-->

>[!IMPORTANT]
>
>이 페이지에서 설명하는 절차는 Adobe Admin Console에 아직 온보딩되지 않은 조직에만 적용됩니다. 조직이 Adobe Admin Console에 온보딩된 경우 이 작업을 사용할 수 없습니다.
>
>조직이 Adobe Admin Console에 온보딩되었는지 여부에 따라 다른 절차 목록은 [플랫폼 기반의 관리 차이점(Adobe Workfront/Adobe Business Platform)](../../../administration-and-setup/get-started-wf-administration/actions-in-admin-console.md).

Adobe Workfront 관리자로서 다른 사용자를 대신하여 Workfront에 액세스해야 하는 경우가 있습니다.

또는 그룹 관리자로서 관리하는 그룹의 구성원인 사용자를 대신하여 Workfront에 액세스해야 할 수 있습니다.

예를 들어 휴가 중인 사용자가 특정 작업을 수행할 때까지 작업을 진행할 수 없는 경우 해당 사용자로 로그인하여 대신 작업을 수행할 수 있습니다.

<!--
<note type="note">
Some users, such as executives, need to be able to control which administrators can log in to their accounts, and for how long. Working with your organization, Workfront configures settings that allow this control for these users. When a Workfront administrator or group administrator (associated with one of the user's groups) tries to log in as one of these users, an on-screen message prompts the administrator to contact the user for access. From the user profile area, the user can then grant access to the administrator and specify an expiration time for it. For more information on how the user does this, see
<a href="../../../workfront-basics/manage-your-account-and-profile/configuring-your-user-profile/configure-my-settings.md#access" class="MCXref xref">Access</a> in
<a href="../../../workfront-basics/manage-your-account-and-profile/configuring-your-user-profile/configure-my-settings.md" class="MCXref xref">Configure My Settings</a>.
<span class="PinkDraftNote">[Add a note about this being only for the Enterprise package if they decide to do it that way]</span>
</note>
-->

>[!NOTE]
>
>문서 통합은 개인 개인 파일에 연결할 수 있으므로 관리자는 다른 사용자로 로그인하는 동안 문서 통합에 액세스할 수 없습니다.
>
>문서 통합에 대한 자세한 내용은 [문서 통합 구성](../../../administration-and-setup/configure-integrations/configure-document-integrations.md)

## 액세스 요구 사항

이 문서의 절차를 수행하려면 다음 사항이 있어야 합니다.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront 플랜</td> 
   <td>모든</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront 라이선스</td> 
   <td>플랜</td> 
  </tr> 
  <tr> 
   <td role="rowheader">액세스 수준 구성</td> 
   <td> <p>시스템 관리자 액세스 수준을 사용하면 다른 사용자로 로그인할 수 있습니다. 이 액세스 수준에 대한 자세한 내용은 <a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-a-user-full-administrative-access.md" class="MCXref xref">사용자에게 전체 관리자 액세스 권한 부여</a>. </p> <p>계획자 액세스 레벨을 사용하면 <b>사용자</b> 액세스 수준에서 설정은 <b>편집</b> 액세스, 사용 <b>만들기</b> 둘 중 적어도 하나 <b>사용자 관리자</b> 옵션 사용 <b>설정 세부 조정</b> <img src="assets/gear-icon-in-access-levels.png">. </p> 
   <p><b>참고</b>: 이 두 옵션 중 사용자가 <b>관리자(그룹 사용자)</b> 이 활성화되어 있으면 사용자가 구성원인 그룹의 그룹 관리자여야 합니다.</p> 
   <p>에 대한 자세한 정보 <b>사용자</b> 액세스 수준에서 설정하는 방법은 <a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-other-users.md" class="MCXref xref">사용자에게 액세스 권한 부여</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

## 다른 사용자로 로그인 및 작업 수행

1. Workfront 관리자 또는 그룹 관리자로 Workfront에 로그인합니다.

   >[!NOTE]
   >
   >* 그룹 관리자라면 관리하는 그룹의 사용자만 로그인할 수 있습니다. 또한 액세스 수준에서 사용자 관리자(그룹 사용자) 권한을 활성화해야 합니다.
   >   
   >  ![](assets/group-admin-user.png)
   >   
   >  이 설정은 기본적으로 비활성화됩니다. 자세한 내용은 [사용자 정의 액세스 수준 만들기 또는 수정](../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md).
   >   
   >* Workfront 관리자의 암호를 재설정할 수 없습니다.


1. 을(를) 클릭합니다. **기본 메뉴** 아이콘 ![](assets/main-menu-icon.png) Adobe Workfront의 오른쪽 위 모서리에서 을(를) 클릭하고 **설정** ![](assets/gear-icon-settings.png).

1. 왼쪽 패널에서 **다른 이름으로 로그인**.

1. 에서 **사용자** 상자 **다른 이름으로 로그인** 탭에서 사용자 이름을 입력하고 드롭다운 목록에 표시될 때 해당 이름을 클릭합니다.

   사용자에게 Workfront에 정의된 액세스 수준이 있어야 합니다. 로그인할 권한이 없는 사용자는 Workfront 시스템에 로그인할 수 없습니다.

   >[!NOTE]
   >
   >그룹 관리자는 관리하는 그룹의 구성원인 사용자만 로그인할 수 있습니다. Workfront 관리자로 로그인할 수 없습니다.

1. 클릭 **로그인합니다.**

   <!--
   <p data-mc-conditions="QuicksilverOrClassic.Draft mode">Might come in a future story:</p>
   -->

   <!--
   <p data-mc-conditions="QuicksilverOrClassic.Draft mode">click an Access period and then click Request to ask the user for access to log as him or her for the specified period of time. Continue these steps after the user grants access. Specify somewhere here that this is only for the Enterprise package if they decide on that</p>
   -->

   <!--
   <p data-mc-conditions="QuicksilverOrClassic.Draft mode">Or </p>
   -->

   <!--
   <p data-mc-conditions="QuicksilverOrClassic.Draft mode">If a prompt appears indicating that the user has restricted access to their account, contact the user to request access.</p>
   -->

   <!--
   <p data-mc-conditions="QuicksilverOrClassic.Draft mode">The user can then can grant you "Log in as" access in their user profile. They can also specify an expiration date and time for the access period. </p>
   -->

   <!--
   This triggers an email to let you know that you have access to log in as the user, depending on how your event notifications are enabled. For more information, see <a href="../../../workfront-basics/using-notifications/event-notifications.md" class="MCXref xref">Event notifications</a>.
   </div>
   -->

   다른 사용자로 로그인한 경우 화면 상단에 알림을 표시하여 이 사항을 나타냅니다.

1. 사용자로 필요한 작업을 수행한 후 **로그아웃합니다.**

## 관리자가 다른 사용자로 로그인하는 동안 활동 추적 및 감사

Workfront에서는 관리자가 다른 사용자로 로그인하는 동안 발생하는 활동 추적 및 감사 메커니즘을 제공합니다.

다른 사용자로 로그인하면 시스템 또는 그룹 관리자가 해당 사용자로 로그인하는 날짜까지 해당 사용자에 대한 마지막 로그인 날짜가 수정됩니다.

* [항목에 대한 표시기 보기](#view-indicators-on-items)
* [감사 정보 보기](#view-audit-information)

### 항목에 대한 표시기 보기 {#view-indicators-on-items}

Workfront에 다른 사용자로 로그인하여 작업을 수행하는 경우 Workfront은 사용자가 로그인한 사용자를 대신하여 수행한 작업이 수행됨을 명확하게 나타냅니다.

예를 들어, 다른 사용자로 로그인한 동안 항목에 대해 주석을 다는 경우 문은 사용자를 대신하여 댓글 작업을 수행했음을 나타냅니다.

### 감사 정보 보기 {#view-audit-information}

1. Workfront 관리자 또는 그룹 관리자로 Workfront에 로그인합니다.
1. 을(를) 클릭합니다. **기본 메뉴** 아이콘 ![](assets/main-menu-icon.png) Adobe Workfront의 오른쪽 위 모서리에서 을(를) 클릭하고 **설정** ![](assets/gear-icon-settings.png).

1. 클릭 **다른 이름으로 로그인,** 그런 다음 **액세스 로그** 탭.

   시스템 또는 그룹 관리자가 다른 사용자로 Workfront에 로그인할 때마다 이벤트가 감사 추적에 기록됩니다. 또한 관리자가 다른 사용자로 로그인하는 동안 발생한 모든 감사 작업은 감사 추적에 기록됩니다.

1. (선택 사항) 다음 방법으로 감사 추적에 표시되는 결과를 필터링할 수 있습니다.

   * 로그인한 사용자별
   * 으로 로그인한 사용자
   * 날짜별
