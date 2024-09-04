---
title: 작업 공간 공유
description: Adobe Workfront Planning에서 작업할 때 공동 작업을 보장하기 위해 다른 사용자와 작업 영역을 공유할 수 있습니다.
author: Alina
feature: Workfront Planning
role: User, Admin
recommendations: noDisplay, noCatalog
source-git-commit: bd202821687453288c96147933331c8a7a6b3acb
workflow-type: tm+mt
source-wordcount: '723'
ht-degree: 2%

---


# 작업 공간 공유

{{planning-important-intro}}

Adobe Workfront Planning에서 작업할 때 공동 작업을 보장하기 위해 다른 사용자와 작업 영역을 공유할 수 있습니다.

<!--
This article describes how you can share a view with others. For information about requesting, granting, or denying permissions to a view, see [Request permissions to a view or a workspace](/help/quicksilver/planning/access/request-permissions.md). -->

>[!NOTE]
>
>작업 영역에 권한을 부여해도 다른 사용자에게 레코드 유형 페이지의 보기에 대한 권한이 부여되지 않습니다. 다른 사용자와 공유하려면 레코드 유형 페이지에서 개별 보기에 대한 권한을 부여해야 합니다. 자세한 내용은 [보기 공유](/help/quicksilver/planning/access/share-views.md)를 참조하십시오.


## 액세스 요구 사항

+++ 를 확장하여 Workfront Planning에 대한 액세스 요구 사항을 봅니다.

Workfront Planning에 액세스하려면 다음 항목이 있어야 합니다.

<table style="table-layout:auto"> 
<col> 
</col> 
<col> 
</col> 
<tbody> 
    <tr> 
<tr> 
<td> 
   <p> 제품</p> </td> 
   <td> 
   <ul><li><p> Adobe Workfront</p></li> 
   <li><p> Adobe Workfront 계획<p></li></ul></td> 
  </tr>   
<tr> 
   <td role="rowheader"><p>Adobe Workfront 플랜*</p></td> 
   <td> 
<p>다음 Workfront 플랜 중 하나:</p> 
<ul><li>선택</li> 
<li>Prime</li> 
<li>Ultimate</li></ul> 
<p>Workfront Planning은 기존 Workfront 플랜에 사용할 수 없습니다.</p> 
   </td> 
<tr> 
   <td role="rowheader"><p>Adobe Workfront 계획 계획*</p></td> 
   <td> 
<p>임의 </p> 
<p>각 Workfront Planning 계획에 포함된 사항에 대한 자세한 내용은 Workfront 계정 관리자에게 문의하십시오. </p> 
   </td> 
 <tr> 
   <td role="rowheader"><p>Adobe Workfront 플랫폼</p></td> 
   <td> 
<p>Workfront Planning의 모든 기능에 액세스할 수 있으려면 조직의 Workfront 인스턴스가 통합 경험 Adobe에 온보딩되어야 합니다.</p>
<p>사용자가 권한 요청에서 작업 영역에 권한을 요청하고 부여할 수 있으려면 조직이 Adobe 통합 경험에 온보딩되어야 합니다. </p> 
<p>자세한 내용은 <a href="/help/quicksilver/workfront-basics/navigate-workfront/workfront-navigation/adobe-unified-experience.md">Workfront용 통합 경험 Adobe</a>를 참조하십시오. </p> 
   </td> 
   </tr> 
  </tr> 
  <tr> 
   <td role="rowheader"><p>Adobe Workfront 라이센스*</p></td> 
   <td><p> 표준 </p>
   <p>기존 Workfront 라이선스에는 Workfront Planning을 사용할 수 없습니다.</p> 
  </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><p>액세스 수준 구성</p></td> 
   <td> <p>Adobe Workfront Planning에 대한 액세스 수준 제어가 없습니다.</p>   
</td> 
  </tr> 
<tr> 
   <td role="rowheader"><p>개체 권한</p></td> 
   <td>  <p>작업 공간에 대한 권한 관리</p>  </td> 
  </tr> 
<tr> 
   <td role="rowheader"><p>레이아웃 템플릿</p></td> 
   <td> <p>Workfront 관리자를 포함한 모든 사용자에게 메인 메뉴의 계획 영역을 포함하는 레이아웃 템플릿을 할당해야 합니다. </p> </td> 
  </tr> 
</tbody> 
</table>

*Workfront 액세스 요구 사항에 대한 자세한 내용은 Workfront 설명서의 [액세스 요구 사항](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)을 참조하십시오.

+++

<!--

OLD: 
 
<table style="table-layout:auto">
 <col>
 </col>
 <col>
 </col>
 <tbody>
    <tr>
<tr>
<td>
   <p> Product</p> </td>
   <td>
   <p> Adobe Workfront</p> </td>
  </tr>  
 <td role="rowheader"><p>Adobe Workfront agreement</p></td>
   <td>
<p>Your organization must be enrolled in the early access stage for Workfront Planning </p>
   </td>
  </tr>
  <tr>
   <td role="rowheader"><p>Adobe Workfront plan</p></td>
   <td>
<p>Any</p>
   </td>
  </tr>
  <tr>
   <td role="rowheader"><p>Adobe Workfront license*</p></td>
   <td>
   <p>New: Standard</p>
   Or
   <p>Current: Plan </p> 
  </td>
  </tr>
  
  <tr>
   <td role="rowheader"><p>Access level configurations</p></td>
   <td> There are no access controls for Adobe Workfront Planning</p>  
</td>
  </tr>

  <tr>
   <td role="rowheader"><p>Permissions</p></td>
   <td> <p>Manage permissions to a workspace</p>  
</td>
  </tr>

<tr>
   <td role="rowheader"><p>Layout template</p></td>
   <td> <p>All users, including Workfront administrators,  must be assigned a layout template that includes the Planning area in the Main Menu. </p> <p>For information, see <a href="/help/quicksilver/planning/access/access-overview.md">Access overview</a>. </p> 
</td>
  </tr>
 </tbody>
</table>

*For information, see [Access requirements in Workfront documentation](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).-->



## 작업 공간에 대한 권한 공유

다음 사용자는 다른 사용자와 작업 영역을 공유할 수 있습니다.

* 시스템 관리자는 작성하지 않은 작업 영역을 포함하여 모든 작업 영역을 공유할 수 있습니다.
* 다른 모든 사용자는 관리 권한이 있는 작업 영역만 공유할 수 있습니다.

다른 사용자와 작업 공간을 공유하려면 다음을 수행하십시오.

{{step1-to-planning}}

1. 공유할 작업 영역을 연 다음 화면 오른쪽 상단의 **공유**&#x200B;를 클릭합니다.

   ![](assets/share-button-on-workspace-top-right.png)

1. **작업 공간 액세스 권한 부여** 필드에서 사용자 또는 그룹의 이름을 입력한 다음 목록에 표시될 때 클릭합니다.

   ![](assets/sharing-ui-with-groups.png)

1. 드롭다운 메뉴에서 다음 권한 수준 중 하나를 선택합니다.
   * 보기
   * 참여
   * 관리

     권한 수준 및 사용자가 각 수준에 대해 수행할 수 있는 작업에 대한 자세한 내용은 [Adobe Workfront Planning의 권한 공유 개요](/help/quicksilver/planning/access/sharing-permissions-overview.md)를 참조하십시오.
1. 작업 영역에 대한 링크를 클립보드에 복사하려면 **링크 복사**&#x200B;를 클릭하십시오.
1. 복사한 링크를 다른 사용자와 공유합니다. 링크를 받은 사용자가 활성 사용자여야 하며 작업 영역에 액세스할 수 있도록 Workfront에 로그인해야 합니다.
1. **저장**&#x200B;을 클릭합니다.

## 권한 요청에서 작업 영역에 대한 권한 부여

권한이 없는 작업 영역 링크에 액세스하는 사용자는 작업 영역에 대한 권한을 요청할 수 있습니다. 작업 영역에 대한 관리 권한이 있는 모든 사용자는 권한 요청을 받고 권한을 부여하거나 거부할 수 있습니다.

1. (조건부) 작업 공간의 관리자인 경우 다른 사용자로부터 다음 영역의 보기에 대한 액세스 요청을 받을 수 있습니다.

   * 인앱 알림
     ![](assets/in-app-notification-for-access-request.png)
   * 이메일 알림
     ![](assets/email-notification-for-access-request.png)
1. (조건부) Workfront의 알림 영역에서 인앱 알림을 클릭합니다
또는
전자 메일 알림에서 **모든 알림 보기**&#x200B;를 클릭한 다음 목록에서 알림을 클릭합니다.

   **액세스 요청 보류 중** 상자가 표시됩니다.

   ![](assets/notifications-list-approval-box.png)

1. (선택 사항) 권한을 승인하려는 사용자의 경우 드롭다운 메뉴에서 사용자 이름 오른쪽에 있는 다음 옵션 중 하나를 선택합니다.
   * **보기**
   * **Contribute**
   * **관리**
1. 권한을 승인하거나 거부할 사용자를 선택한 다음 **모두 승인** 또는 **모두 거부**&#x200B;를 클릭합니다.
1. **보류 중인 액세스 요청**&#x200B;의 왼쪽에 있는 왼쪽 화살표를 클릭한 다음 **저장**&#x200B;을 클릭합니다.

   요청을 승인하면 작업 영역의 공유 상자에 사용자가 추가됩니다. 권한을 요청하는 사용자는 요청이 승인되었다는 이메일 확인을 받게 됩니다. <!--will they also get an in-app notification??-->


## 작업 공간에 대한 권한 제거


{{step1-to-planning}}

1. 권한을 제거할 작업 영역을 연 다음 화면 오른쪽 상단의 **공유**&#x200B;를 클릭합니다.
1. 사용자 또는 그룹 이름 오른쪽에 있는 드롭다운 메뉴를 클릭한 다음 **제거**&#x200B;를 클릭합니다.
1. **저장**&#x200B;을 클릭합니다.

   제거된 그룹에 속한 사용자나 사용자는 더 이상 작업공간이나 해당 객체에 액세스할 수 없습니다.