---
title: Adobe Workfront Planning 인앱 알림 관리
description: 누군가가 기록 댓글에서 귀하 또는 귀하의 팀에 태그를 지정하면 해당 태그에 대한 이메일 알림을 받게 됩니다.
feature: Workfront Planning
role: User, Admin
author: Alina
recommendations: noDisplay, noCatalog
exl-id: a6eb8c7c-a34d-4c84-a45c-7e7f050a4302
source-git-commit: f2fe6ef78b3032f7a89d4c816cb11b525634c067
workflow-type: tm+mt
source-wordcount: '366'
ht-degree: 0%

---


# Adobe Workfront Planning 인앱 알림 관리

{{planning-important-intro}}

다음 시나리오가 있을 때 Workfront Planning에서 인앱 알림을 받을 수 있습니다.

* 누군가가 기록 댓글에서 귀하 또는 귀하의 팀에 태그를 지정합니다.

  레코드 댓글에 다른 사용자를 태그 지정하는 방법에 대한 자세한 내용은 [레코드 댓글 관리](/help/quicksilver/planning/records/manage-record-comments.md)를 참조하십시오.
* 누군가 보기 또는 작업 영역에 액세스할 수 있는 권한을 요청합니다.
* 누군가 보기 또는 작업 영역 <!--Isk confirmed there is no notification for denying permissions - did not test-->에 대한 액세스 권한이 부여되었음을 확인합니다.

## 액세스 요구 사항

+++ 을 확장하여 이 문서의 기능에 대한 액세스 요구 사항을 봅니다. 

<table style="table-layout:auto"> 
<col> 
</col> 
<col> 
</col> 
<tbody> 
    <tr> 
<tr> 
</tr>   
<tr> 
   <td role="rowheader"><p>Adobe Workfront 패키지</p></td> 
   <td> 
<ul> 
<li><p>모든 Workfront 및 모든 Planning 패키지</p></li>
또는
<li><p>모든 워크플로우 및 모든 Planning 패키지</li></ul>
<p>각 Workfront Planning 패키지에 포함된 내용에 대한 자세한 내용은 Workfront 계정 담당자에게 문의하십시오. </p> 
   </td> 
  <tr> 
   <td role="rowheader"><p>Adobe Workfront 라이선스</p></td> 
   <td><p>밝거나 높음</p>
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><p>개체 권한</p></td> 
   <td>   <p>작업 영역 </a>에 대한 이상의 권한 보기 </p>  
   <p>시스템 관리자는 만들지 않은 작업 영역을 포함하여 모든 작업 영역에 대한 권한을 가집니다</p> </td> 
  </tr> 
<tr>
   <td role="rowheader"><p>레이아웃 템플릿</p></td>
   <td> 라이트 또는 기여자 라이선스가 있는 사용자에게 Planning이 포함된 레이아웃 템플릿을 할당해야 합니다.
   <p>표준 사용자 및 시스템 관리자에게는 기본적으로 계획 영역이 활성화되어 있습니다.</p></div></li></ul>
</td>
  </tr> 
</tbody> 
</table>

Workfront 액세스 요구 사항에 대한 자세한 내용은 Workfront 설명서의 [액세스 요구 사항](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)을 참조하십시오.

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
<p>Your organization's instance of Workfront must be onboarded to the Adobe Unified Experience.</p> 
<p>The users in your organization receive notifications from Workfront Planning only when your organization is onboarded to the Adobe Unified Experience. </p>
<p>For more information, see <a href="/help/quicksilver/workfront-basics/navigate-workfront/workfront-navigation/adobe-unified-experience.md">Adobe Unified Experience for Workfront</a>. </p> 
   </td> 
   </tr> 
  </tr> 
  <tr> 
   <td role="rowheader"><p>Adobe Workfront license*</p></td> 
   <td><p> Standard, Light, or Contributor</p>
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
   <td>   <p>View or higher permissions to a workspace</a> </p>  
   <p>System Administrators have permissions to all workspaces, including the ones they did not create</p>  </td> 
  </tr> 
<tr>
   <td role="rowheader"><p>Layout template</p></td>
   <td> Users with a Light or Contributor license must be assigned a layout template that includes Planning.
   <p>Standard users and System Administrators have the Planning areas enabled by default.</p></div></li></ul>
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
1. (선택 사항) Adobe Experience Cloud의 **알림** 페이지로 이동하려면 **모두 보기**&#x200B;를 클릭합니다.

## 권한 요청 및 부여 시 인앱 알림 관리

누군가 보기 또는 작업 영역에 대한 권한을 요청하거나 부여하면 인앱 알림을 받습니다.

보기 또는 작업 영역에 대한 권한 요청, 부여 또는 거부에 대한 자세한 내용은 [보기 또는 작업 영역에 대한 권한 요청](/help/quicksilver/planning/access/request-permissions.md)을 참조하십시오.

Workfront Planning 알림 관리에 대한 자세한 내용은 [Adobe Workfront Planning 알림 환경 설정 관리](/help/quicksilver/planning/notifications/manage-notification-preferences.md)를 참조하십시오.
