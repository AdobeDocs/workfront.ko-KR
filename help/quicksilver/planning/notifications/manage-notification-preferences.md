---
title: Adobe Workfront Planning 알림 환경 설정 관리
description: Adobe Workfront Planning에 대한 알림 환경 설정을 관리할 수 있습니다. 이 문서에서는 알림 환경 설정을 구성하는 방법에 대해 설명합니다.
author: Alina
feature: Workfront Planning
role: User
recommendations: noDisplay, noCatalog
exl-id: ec549a61-095c-433f-80e2-1be5c0a05180
source-git-commit: 0a65a18678bfc0aa2e080a0a983746040310b079
workflow-type: tm+mt
source-wordcount: '502'
ht-degree: 1%

---


# Adobe Workfront Planning 알림 환경 설정 관리

<!--<span class="preview">The highlighted information on this page refers to functionality not yet generally available. It is available only in the Preview environment for all customers. After the monthly releases to Production, the same features are also available in the Production environment for customers who enabled fast releases. </span>   

<span class="preview">For information about fast releases, see [Enable or disable fast releases for your organization](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/enable-fast-release-process.md). </span>-->

{{planning-important-intro}}

Workfront Planning에서 다음 작업이 발생하면 인앱 또는 이메일 알림을 받을 수 있습니다.

* 누군가가 기록 페이지의 댓글에 귀하를 추가합니다.
* 누군가 보기 또는 작업 영역에 액세스할 수 있는 권한을 요청합니다.
* 누군가가 <!--I could not test this but Isk confirmed--> 보기 또는 작업 영역에 액세스할 수 있는 권한을 부여했습니다.
* Workfront Planning 요청을 제출합니다.
* 누군가가 귀하가 제출한 Workfront Planning 요청을 승인하거나 거부합니다.
* 제출한 Workfront Planning 요청의 상태가 변경됩니다.

## 액세스 요구 사항

+++ 를 확장하여 Workfront Planning에 대한 액세스 요구 사항을 봅니다.

이 문서의 단계를 수행하려면 다음 액세스 권한이 있어야 합니다.

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
   <td><p><p>표준, 라이트 또는 기여자
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


Workfront Planning 알림에 대한 자세한 내용은 다음 문서를 참조하십시오.

* 레코드에 대한 댓글에 대한 자세한 내용은 [레코드 댓글 관리](/help/quicksilver/planning/records/manage-record-comments.md)를 참조하십시오.
* Workfront Planning의 인앱 알림에 대한 자세한 내용은 [Adobe Workfront Planning의 인앱 알림 관리](/help/quicksilver/planning/notifications/manage-planning-in-app-notifications.md)를 참조하십시오.
* Workfront Planning의 전자 메일 알림에 대한 자세한 내용은 [Adobe Workfront Planning의 전자 메일 알림 관리](/help/quicksilver/planning/notifications/manage-planning-email-notifications.md)를 참조하십시오.
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
   <p>In order to receive in-app notifications from Workfront Planning and manage notification preferences, your organization's instance of Workfront must be onboarded to the Adobe Unified Experience. For information, see <a href="/help/quicksilver/workfront-basics/navigate-workfront/workfront-navigation/adobe-unified-experience.md">Adobe Unified Experience for Workfront</a>.</p>
   </td>
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

## 알림 환경 설정 관리

1. Adobe Experience Cloud 자격 증명으로 Workfront에 로그인합니다.
1. 화면 오른쪽 상단의 **계정 메뉴** 아이콘 ![](assets/account-menu-icon-on-experience-cloud.png)을(를) 클릭한 다음 **기본 설정**&#x200B;을(를) 클릭합니다.
1. **알림** 섹션에서 **Workfront**&#x200B;을(를) 클릭합니다.
1. 수신하려는 알림을 선택합니다.
또는
수신을 중지할 알림의 선택을 취소합니다.

   ![](assets/adobe-experience-cloud-notifications-panel-for-workfront-planning.png)
1. Workfront에 사용할 수 있는 알림은 다음과 같습니다.

   * **언급**: 다른 사용자가 Workfront Planning에서 댓글에 태그를 지정하면 알림을 받습니다
   * **요청**: 누군가가 다음 중 하나를 완료하면 알림을 받습니다.

      * Workfront Planning 개체에 대한 권한을 요청하거나 부여합니다.
      * Workfront Planning 요청을 제출했습니다.
      * 변경 사항을 제출한 Workfront Planning 요청의 상태
      * Workfront Planning 요청에 대한 승인 요청, 부여 또는 거부

   알림 관리에 대한 자세한 내용은 [계정 환경 설정 및 알림](https://experienceleague.adobe.com/en/docs/core-services/interface/features/account-preferences)을 참조하세요.

<!--OLD: notifications are not available to non-IMS customers: 

When someone adds you to a comment in the record page, you may receive an in-app as well as an email notification about the comment. 

The following scenarios exist:   

* Adobe Unified Experience customers receive both an in-app notification and an email notification. They can manage their in-app and email notification preferences in the Preferences area of their Adobe Experience Cloud profile for the Workfront product. 

    For more information, see [Account preferences and notifications](https://experienceleague.adobe.com/en/docs/core-services/interface/features/account-preferences).

* Customers who are not on the Adobe Unified Experience receive only an email notification. They cannot manage their email notifications preferences and will always receive an email when someone adds them to a comment on a record in Workfront Planning.   

-->
