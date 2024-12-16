---
title: Adobe Workfront Planning 이메일 알림 관리
description: 누군가가 Adobe Workfront Planning에서 기록 댓글에 나를 태그하면 해당 태그에 대한 이메일 알림을 받게 됩니다.
author: Alina
feature: Workfront Planning
role: User, Admin
recommendations: noDisplay, noCatalog
exl-id: 3c505b3a-cda7-4e7b-b497-28b820e9bb8f
source-git-commit: 9b5ba629fa2f50f0425f4afbfd4faa891d917845
workflow-type: tm+mt
source-wordcount: '717'
ht-degree: 0%

---


# Adobe Workfront Planning 이메일 알림 관리

<span class="preview">이 페이지에서 강조 표시된 정보는 아직 일반적으로 사용할 수 없는 기능을 참조합니다. 모든 고객을 위한 미리보기 환경에서만 사용할 수 있습니다. 월별 프로덕션 릴리스 이후 빠른 릴리스를 활성화한 고객을 위해 프로덕션 환경에서도 동일한 기능을 사용할 수 있습니다. </span>

<span class="preview">빠른 릴리스에 대한 자세한 내용은 [조직의 빠른 릴리스 사용 또는 사용 안 함](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/enable-fast-release-process.md)을 참조하세요. </span>

{{planning-important-intro}}

다음 시나리오가 있을 때 Workfront Planning에서 이메일 알림을 받을 수 있습니다.

* 누군가가 기록 댓글에서 귀하를 태그합니다.

  레코드 댓글에 다른 사용자를 태그 지정하는 방법에 대한 자세한 내용은 [레코드 댓글 관리](/help/quicksilver/planning/records/manage-record-comments.md)를 참조하십시오.
* 누군가 보기 또는 작업 영역에 액세스할 수 있는 권한을 요청합니다.
* 누군가 보기 또는 작업 영역 <!--Isk confirmed that there is nno email for denying access but did not test-->에 대한 액세스 권한이 부여되었음을 확인합니다.

<div class="preview">

* Workfront Planning 요청을 제출합니다. 자세한 내용은 [Adobe Workfront Planning에서 요청 양식 만들기 및 관리](/help/quicksilver/planning/requests/create-request-form.md)를 참조하십시오.
* 누군가가 귀하가 제출한 Workfront Planning 요청을 승인하거나 거부합니다. 자세한 내용은 [Adobe Workfront Planning에서 요청 승인](/help/quicksilver/planning/requests/approve-request.md)을 참조하십시오.
* 제출한 Workfront Planning 요청의 상태가 변경됩니다.

</div>


## 액세스 요구 사항

+++ 를 확장하여 Workfront Planning에 대한 액세스 요구 사항을 봅니다.

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
   <td role="rowheader"><p>Adobe Workfront 계획 패키지*</p></td> 
   <td> 
<p>임의 </p> 
<p>각 Workfront Planning 계획에 포함된 사항에 대한 자세한 내용은 Workfront 계정 관리자에게 문의하십시오. </p> 
   </td> 
 <tr> 
   <td role="rowheader"><p>Adobe Workfront 플랫폼</p></td> 
   <td> 
<p>조직의 Workfront 인스턴스는 통합 경험 Adobe에 온보딩되어야 합니다.</p> 
<p>조직의 사용자는 조직이 Adobe 통합 경험에 온보딩될 때만 Workfront Planning에서 알림을 받습니다. </p>
<p>자세한 내용은 <a href="/help/quicksilver/workfront-basics/navigate-workfront/workfront-navigation/adobe-unified-experience.md">Workfront용 통합 경험 Adobe</a>를 참조하십시오. </p> 
   </td> 
   </tr> 
  </tr> 
  <tr> 
   <td role="rowheader"><p>Adobe Workfront 라이센스*</p></td> 
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
   <p>시스템 관리자는 만들지 않은 작업 영역을 포함하여 모든 작업 영역에 대한 권한을 가집니다</p> </td> 
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
   <p> Adobe Workfront</p> 
   <p>In order to receive notifications from Workfront Planning and manage notification preferences, your organization's instance of Workfront must be onboarded to the Adobe Unified Experience. For information, see <a href="/help/quicksilver/workfront-basics/navigate-workfront/workfront-navigation/adobe-unified-experience.md">Adobe Unified Experience for Workfront</a>.</p></td>
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
-->


## 다른 사용자가 귀하를 댓글에 태그 지정할 때 이메일 알림 관리

1. (조건부 및 선택 사항) 다른 사용자가 레코드에 있는 댓글에 귀하를 태그하면 태그 및 댓글을 알려 주는 이메일 알림으로 이동합니다. 이메일 발신자는 Adobe Experience Cloud입니다.

   ![](assets/email-notification-example.png)

1. (선택 사항) 전자 메일 내부의 **Workfront** 상자에 있는 메시지를 클릭합니다.

   Workfront에 레코드 세부 정보 페이지가 열립니다. 레코드를 업데이트하거나 댓글에 답글을 달 수 있습니다.

1. (조건부) 사용 가능한 경우 **모든 알림 보기**&#x200B;를 클릭합니다. <!--check with Lilit - do non-IMS users have this button??-->
Adobe Experience Cloud에서 **알림** 페이지가 열립니다. 모든 Adobe Experience Cloud 애플리케이션의 모든 알림이 표시됩니다.

## 권한 요청 및 부여 시 이메일 알림 관리

1. (조건부 및 선택 사항) 누군가 보기 또는 작업 영역에 액세스할 수 있는 권한을 요청하거나 부여하면 권한 요청을 알리는 이메일로 이동합니다. 이메일 발신자는 Adobe Experience Cloud입니다.

1. (선택 사항) 전자 메일 내부의 **Workfront** 상자에 있는 메시지를 클릭합니다.

   Workfront에 레코드 세부 정보 페이지가 열립니다. 레코드를 업데이트하거나 댓글에 답글을 달 수 있습니다.

1. (조건부) 사용 가능한 경우 **모든 알림 보기**를 클릭합니다.
**알림** 페이지가 Adobe Experience Cloud에서 열립니다. 모든 Adobe Experience Cloud 애플리케이션의 모든 알림이 표시됩니다.


보기 또는 작업 영역에 대한 권한 요청, 부여 또는 거부에 대한 자세한 내용은 [보기 또는 작업 영역에 대한 권한 요청](/help/quicksilver/planning/access/request-permissions.md)을 참조하십시오.

Workfront Planning 알림 관리에 대한 자세한 내용은 [Adobe Workfront Planning 알림 환경 설정 관리](/help/quicksilver/planning/notifications/manage-notification-preferences.md)를 참조하십시오.

## Workfront Planning 요청 제출, 승인 또는 거부에 대한 이메일 알림 관리

1. (선택 사항) Workfront이 귀하에게 보내는 이메일로 이동합니다
요청을 제출한 후 또는 제출한 요청이 승인 또는 거부된 후. 이메일을 보낸 사람은 Adobe Workfront입니다.

1. (선택 사항) **요청 열기**&#x200B;를 클릭합니다. 그러면 Workfront Planning에서 요청이 열립니다.

1. 화면 오른쪽 위의 **알림** 아이콘 ![](assets/notifications-area-icon-unified-shell.png)을(를) 클릭하여 **알림** 페이지에 액세스합니다.

   Workfront Planning 알림 관리에 대한 자세한 내용은 [Adobe Workfront Planning 알림 환경 설정 관리](/help/quicksilver/planning/notifications/manage-notification-preferences.md)를 참조하십시오.
