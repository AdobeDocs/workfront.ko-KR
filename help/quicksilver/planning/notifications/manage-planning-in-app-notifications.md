---
title: Adobe Workfront Planning 인앱 알림 관리
description: 누군가 레코드 댓글에서 귀하 또는 귀하의 팀을 태그하면 해당 태그에 대한 이메일 알림 받게 됩니다.
feature: Workfront Planning
role: User, Admin
author: Alina
recommendations: noDisplay, noCatalog
exl-id: a6eb8c7c-a34d-4c84-a45c-7e7f050a4302
source-git-commit: 298c542afea902d9fc14ef6a4470c0bc1d9bd33c
workflow-type: tm+mt
source-wordcount: '444'
ht-degree: 1%

---


# Adobe Systems Workfront Planning 인앱 알림 관리

{{planning-important-intro}}

다음 시나리오가 있는 경우 Workfront Planning에서 인앱 알림을 받을 수 있습니다.

* 누군가 레코드 댓글에서 귀하 또는 귀하의 팀을 태그합니다.

  레코드 댓글에 다른 사용자를 태그 지정하는 방법에 대한 자세한 내용은 [레코드 댓글 관리](/help/quicksilver/planning/records/manage-record-comments.md)를 참조하십시오.
* 누군가 보기 또는 작업 영역에 액세스할 수 있는 권한을 요청합니다.
* 누군가 보기 또는 작업 영역 <!--Isk confirmed there is no notification for denying permissions - did not test-->에 대한 액세스 권한이 부여되었음을 확인합니다.

## 액세스 요구 사항

+++ 를 확장하여 액세스 요구 사항을 확인합니다.

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
   <td role="rowheader"><p>Adobe Systems Workfront 플랜*</p></td> 
   <td> 
<p>다음 Workfront 플랜 중 하나:</p> 
<ul><li>선택</li> 
<li>Prime</li> 
<li>Ultimate</li></ul> 
<p>Workfront Planning은 기존 Workfront 플랜에 사용할 수 없습니다.</p> 
   </td> 
<tr> 
   <td role="rowheader"><p>Adobe Workfront 계획 패키지*</p></td> 
   <td> 
<p>임의 </p> 
<p>각 Workfront Planning 계획에 포함된 사항에 대한 자세한 내용은 Workfront 계정 관리자에게 문의하십시오. </p> 
   </td> 
 <tr> 
   <td role="rowheader"><p>Adobe Workfront 플랫폼</p></td> 
   <td> 
<p>조직의 Workfront 인스턴스 Adobe Systems 통합 환경에 온보딩해야 합니다.</p> 
<p>조직의 사용자는 조직이 Adobe Systems 통합 경험에 온보딩된 경우에만 Workfront Planning에서 알림을 받습니다. </p>
<p>자세한 내용은 Adobe Systems Unified Experience for Workfront<a href="/help/quicksilver/workfront-basics/navigate-workfront/workfront-navigation/adobe-unified-experience.md">를 참조하십시오</a>. </p> 
   </td> 
   </tr> 
  </tr> 
  <tr> 
   <td role="rowheader"><p>Adobe Systems Workfront 라이선스*</p></td> 
   <td><p> 표준, 라이트 또는 기여자</p>
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
   <td>   <p>작업 영역 </a>에 대한 이상의 권한 보기 </p>  
   <p>시스템 관리자는 자신이 생성하지 않은 작업 영역을 포함하여 모든 작업 공간에 대한 권한을 갖습니다</p>  </td> 
  </tr> 
<tr>
   <td role="rowheader"><p>레이아웃 템플릿</p></td>
   <td> Light 또는 Contributor 라이센스가 있는 사용자에게는 Planning이 포함된 레이아웃 템플릿 정보가 지정되어야 합니다.
   <p>표준 사용자 및 시스템 관리자는 기본적으로 계획 영역을 사용하도록 설정되어 있습니다.</p></div></li></ul>
</td>
  </tr>
</tbody> 
</table>

*Workfront 액세스 요구 사항에 대한 자세한 내용은 Workfront 설명서[의 액세스 요구 사항을 참조하십시오](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++


<!--
OLD:

+++ Expand to view access requirements. 

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
   <p> Adobe Workfront</p> 
   <p>In order to receive notifications from Workfront Planning, your organization's instance of Workfront must be onboarded to the Adobe Unified Experience. For information, see <a href="/help/quicksilver/workfront-basics/navigate-workfront/workfront-navigation/adobe-unified-experience.md">Adobe Unified Experience for Workfront</a>.</p></td>
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
   <td role="rowheader"><p>Adobe Workfront license</p></td>
   <td>
   <p>Any</p> 
  </td>
  </tr>
  
  <tr>
   <td role="rowheader"><p>Access level configuration</p></td>
   <td> <p>There are no access level controls in Workfront Planning. </p>  
</td>
  </tr>
<tr>
   <td role="rowheader"><p>Permissions</p></td>
   <td> <p>View or higher permissions to a workspace</a> </p>  
   <p>System Administrators have permissions to all workspaces, including the ones they did not create</p>
</td>
  </tr>

<tr>
   <td role="rowheader"><p>Layout template</p></td>
   <td> <p>Your Workfront or group administrator must add the Planning area in your layout template. For information, see <a href="/help/quicksilver/planning/access/access-overview.md">Access overview</a>. </p>  
</td>
  </tr>
 </tbody>
</table>

+++
-->

## 다른 사용자가 귀하를 댓글에 태그 지정할 때 인앱 알림 관리

1. (조건부) 누군가 귀하 또는 귀하의 팀에 레코드에 대한 댓글에 태그를 지정한 후 Adobe Experience Cloud의 인앱 **알림** 아이콘 ![Experience Cloud 알림 아이콘](assets/experience-cloud-notifications-icon.png)(으)로 이동합니다.

   ![인앱 알림 예](assets/in-app-notification-example.png)

1. 알림을 클릭합니다.

   Workfront Planning에서 레코드 세부 사항 페이지가 열립니다. 레코드를 업데이트하거나 댓글에 답글을 달 수 있습니다.

1. (선택 사항) 모든 알림을 읽었음을 나타내려면 **모두 읽음으로 표시**&#x200B;를 클릭합니다.
1. (선택 사항) 모두 보기를 클릭하여 **Adobe Experience Cloud의 알림** 페이지로 이동합니다&#x200B;**.**

## 권한 요청 및 부여 시 인앱 알림 관리

누군가 보기 또는 작업 영역 권한을 요청하거나 부여하면 인앱 알림을 받습니다.

뷰 또는 작업 영역에 대한 사용 권한 요청, 부여 또는 거부에 대한 자세한 내용은 뷰 또는 작업 영역[에 대한 사용 권한 요청을 참조하세요](/help/quicksilver/planning/access/request-permissions.md).

Workfront Planning 알림 관리에 대한 자세한 내용은 [Adobe Workfront Planning 알림 환경 설정 관리](/help/quicksilver/planning/notifications/manage-notification-preferences.md)를 참조하십시오.
