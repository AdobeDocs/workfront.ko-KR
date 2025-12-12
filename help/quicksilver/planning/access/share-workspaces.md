---
title: 작업 공간 공유
description: Adobe Workfront Planning에서 작업할 때 공동 작업을 보장하기 위해 다른 사용자와 작업 영역을 공유할 수 있습니다.
author: Alina
feature: Workfront Planning
role: User, Admin
recommendations: noDisplay, noCatalog
exl-id: 475a519d-d3bd-4461-8099-0e296d556d34
source-git-commit: 5404cec0cb02d363154a3696b63aaedaafc82688
workflow-type: tm+mt
source-wordcount: '789'
ht-degree: 3%

---

# 작업 공간 공유

<!--<span class="preview">The highlighted information on this page refers to functionality not yet generally available. It is available only in the Preview environment for all customers. After the monthly releases to Production, the same features are also available in the Production environment for customers who enabled fast releases. </span>   

<span class="preview">For information about fast releases, see [Enable or disable fast releases for your organization](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/enable-fast-release-process.md). </span>-->

{{planning-important-intro}}

Adobe Workfront Planning에서 작업할 때 공동 작업을 보장하기 위해 다른 사용자와 작업 영역을 공유할 수 있습니다.

<!--
This article describes how you can share a view with others. For information about requesting, granting, or denying permissions to a view, see [Request permissions to a view or a workspace](/help/quicksilver/planning/access/request-permissions.md). -->

>[!NOTE]
>
>작업 영역에 권한을 부여해도 다른 사용자에게 레코드 유형 페이지의 보기에 대한 권한이 부여되지 않습니다. 다른 사용자와 공유하려면 레코드 유형 페이지에서 개별 보기에 대한 권한을 부여해야 합니다. 자세한 내용은 [보기 공유](/help/quicksilver/planning/access/share-views.md)를 참조하십시오.


## 액세스 요구 사항

+++ 이 문서의 기능에 대한 액세스 요구 사항을 보려면 확장하십시오. 

<!--at GA, check that the Workfront plans article linked below has Planning info-->

<table style="table-layout:auto"> 
<col> 
</col> 
<col> 
</col> 
<tbody> 
<tr> 
   <td role="rowheader"><p>Adobe Workfront 패키지</p></td> 
   <td> 
<p>모든 Workfront 및 Planning 패키지</p> 
또는
<p>모든 워크플로우 및 계획 패키지</p> 
 </tr>
<tr> 
   <td role="rowheader"><p>Adobe Workfront 라이선스</p></td> 
   <td><p>표준</p> 
  </td> 
  </tr>

<td role="rowheader"><p>개체 권한</p></td> 
   <td>  <p>작업 공간에 대한 권한 관리</p>  </td> 
  </tr>

</tbody> 
</table>

Workfront 액세스 요구 사항에 대한 자세한 내용은 Workfront 설명서의 [액세스 요구 사항](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)을 참조하십시오.

+++

<!--Old:
<table style="table-layout:auto"> 
<col> 
</col> 
<col> 
</col> 
<tbody> 
    <tr> 
<tr> 
<td> 
   <p> Products</p> </td> 
   <td> 
   <ul><li><p> Adobe Workfront</p></li> 
   <li><p> Adobe Workfront Planning<p></li></ul></td> 
  </tr>   
<tr> 
   <td role="rowheader"><p>Adobe Workfront plan*</p></td> 
   <td> 
<p>Any of the following Workfront plans:</p> 
<ul><li>Select</li> 
<li>Prime</li> 
<li>Ultimate</li></ul> 
<p>Workfront Planning is not available for legacy Workfront plans</p> 
   </td> 
<tr> 
   <td role="rowheader"><p>Adobe Workfront Planning package*</p></td> 
   <td> 
<p>Any </p> 
<p>For more information about what is included in each Workfront Planning plan, contact your Workfront account manager. </p> 
   </td> 
 <tr> 
   <td role="rowheader"><p>Adobe Workfront platform</p></td> 
   <td> 
<p>Your organization's instance of Workfront must be onboarded to the Adobe Unified Experience to be able to access Workfront Planning.</p>
<p>Your organization must be onboarded to the Adobe Unified Experience for users to be able to request and grant permissions to a workspace from a permission request. </p> 
<p>Users must be added to the Adobe Admin Console in order to gain permissions to Workfront Planning workspaces.</p>
<p>For more information, see <a href="/help/quicksilver/workfront-basics/navigate-workfront/workfront-navigation/adobe-unified-experience.md">Adobe Unified Experience for Workfront</a>. </p> 
   </td> 
   </tr> 
  </tr> 
  <tr> 
   <td role="rowheader"><p>Adobe Workfront license*</p></td> 
   <td><p> Standard </p>
   <p>Workfront Planning is not available for legacy Workfront licenses</p> 
  </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><p>Access level configuration</p></td> 
   <td> <p>There are no access level controls for Adobe Workfront Planning</p>   
</td> 
  </tr> 
<tr> 
   <td role="rowheader"><p>Object permissions</p></td> 
   <td>  <p>Manage permissions to a workspace</p>  </td> 
  </tr> 

</tbody> 
</table> -->

## 작업 공간 공유에 대한 고려 사항

* Workfront Planning에서 개체 공유에 대한 일반적인 내용은 [Adobe Workfront Planning의 공유 권한 개요](/help/quicksilver/planning/access/sharing-permissions-overview.md)를 참조하십시오.
* 조직 내에서 사용자, 팀, 역할, 그룹 또는 회사와 작업 공간을 공유할 수 있습니다.
* 팀, 그룹, 회사 및 작업 역할 외에도 Adobe Admin Console에 추가된 사용자와만 공유할 수 있습니다.
* 조직 외부의 사용자와 작업 공간을 공유할 수 없습니다.
* 작업 영역을 공유하면 작업 영역과 연관된 모든 레코드 유형, 레코드 및 필드도 공유됩니다.
* 작업 영역을 공유하면 보기가 공유되지 않습니다. 별도로 보기를 공유해야 합니다.
* Workspace 권한은 레코드 유형에 상속된 권한으로 표시됩니다.

## 작업 공간에 대한 권한 공유

다음 사용자는 다른 사용자와 작업 영역을 공유할 수 있습니다.

* 시스템 관리자는 작성하지 않은 작업 영역을 포함하여 모든 작업 영역을 공유할 수 있습니다.
* 다른 모든 사용자는 관리 권한이 있는 작업 영역만 공유할 수 있습니다.

다른 사용자와 작업 공간을 공유하려면 다음을 수행하십시오.

{{step1-to-planning}}

1. 공유할 작업 영역을 연 다음 화면 오른쪽 상단의 **공유**&#x200B;를 클릭합니다.

   작업 영역 오른쪽 상단의 ![공유 단추](assets/share-button-on-workspace-top-right.png)

1. **이 작업 영역에 대한 액세스 권한 부여** 필드에서 사용자, 그룹, 팀, 회사 또는 작업 역할의 이름을 입력한 다음 목록에 표시될 때 클릭합니다.

   ![그룹과 UI 공유](assets/sharing-ui-with-groups.png)

   >[!NOTE]
   >
   >   팀, 그룹, 회사 및 작업 역할 외에도 Adobe Admin Console에 추가된 사용자와만 공유할 수 있습니다. Workfront 전용 사용자는 추가할 수 없습니다. 자세한 내용은 [Adobe Admin Console에서 사용자 관리](/help/quicksilver/administration-and-setup/add-users/create-and-manage-users/admin-console.md)를 참조하십시오.


1. 드롭다운 메뉴에서 다음 권한 수준 중 하나를 선택합니다.
   * 보기
   * 참여
   * 관리

     권한 수준 및 사용자가 각 수준에 대해 수행할 수 있는 작업에 대한 자세한 내용은 [Adobe Workfront Planning의 권한 공유 개요](/help/quicksilver/planning/access/sharing-permissions-overview.md)를 참조하십시오.
1. 작업 영역에 대한 링크를 클립보드에 복사하려면 **링크 복사**&#x200B;를 클릭하십시오.
1. 복사한 링크를 다른 사용자와 공유합니다. 링크를 받은 사용자가 활성 사용자여야 하며 작업 영역에 액세스할 수 있도록 Workfront에 로그인해야 합니다.
1. **저장**&#x200B;을 클릭합니다.

   사용자가 작업 영역을 공유한 사용자는 해당 작업 영역에 대한 권한 보유에 대한 인앱과 이메일 알림을 모두 수신하게 됩니다.

## 권한 요청에서 작업 영역에 대한 권한 부여

권한이 없는 작업 영역 링크에 액세스하는 사용자는 작업 영역에 대한 권한을 요청할 수 있습니다. 작업 영역에 대한 관리 권한이 있는 모든 사용자는 권한 요청을 받고 권한을 부여하거나 거부할 수 있습니다.

1. (조건부) 작업 공간의 관리자인 경우 다른 사용자로부터 다음 영역의 보기에 대한 액세스 요청을 받을 수 있습니다.

   * 인앱 알림
     ![액세스 요청에 대한 인앱 알림](assets/in-app-notification-for-access-request.png)
   * 이메일 알림
     ![액세스 요청에 대한 전자 메일 알림](assets/email-notification-for-access-request.png)
1. (조건부) Workfront의 알림 영역에서 인앱 알림을 클릭합니다
또는
전자 메일 알림에서 **모든 알림 보기**&#x200B;를 클릭한 다음 목록에서 알림을 클릭합니다.

   **액세스 요청 보류 중** 상자가 표시됩니다.

   ![알림 목록 승인 상자](assets/notifications-list-approval-box.png)

1. (선택 사항) 권한을 승인하려는 사용자의 경우 드롭다운 메뉴에서 사용자 이름 오른쪽에 있는 다음 옵션 중 하나를 선택합니다.
   * **보기**
   * **참여**
   * **관리**
1. 권한을 승인하거나 거부할 사용자를 선택한 다음 **모두 승인** 또는 **모두 거부**&#x200B;를 클릭합니다.
1. **보류 중인 액세스 요청**&#x200B;의 왼쪽에 있는 왼쪽 화살표를 클릭한 다음 **저장**&#x200B;을 클릭합니다.

   요청을 승인하면 작업 영역의 공유 상자에 사용자가 추가됩니다. 권한을 요청하는 사용자는 요청이 승인되었다는 이메일 확인을 받게 됩니다. <!--will they also get an in-app notification??-->


## 작업 공간에 대한 권한 제거


{{step1-to-planning}}

1. 권한을 제거할 작업 영역을 연 다음 화면 오른쪽 상단의 **공유**&#x200B;를 클릭합니다.
1. 작업 영역을 공유하는 엔터티의 이름 오른쪽에 있는 드롭다운 메뉴를 클릭한 다음 **제거**&#x200B;를 클릭합니다.
1. **저장**&#x200B;을 클릭합니다.

   제거된 사용자는 더 이상 작업공간이나 해당 객체에 액세스할 수 없습니다.

   작업 영역 액세스에서 제거된 사용자에게 더 이상 이러한 권한이 없다는 알림이 없습니다.