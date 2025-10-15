---
title: 보기 또는 Workspace에 권한 요청
description: 다른 사용자가 액세스 권한이 없는 보기 또는 작업 영역에 대한 링크를 공유할 경우 열 수 있는 권한을 요청할 수 있습니다. 이 문서에서는 열 수 없는 공유 링크가 있을 때 보기 또는 작업 영역에 대한 액세스를 요청하는 단계에 대해 설명합니다.
feature: Workfront Planning
role: User, Admin
author: Alina
recommendations: noDisplay, noCatalog
exl-id: 94dfa36a-801a-4eef-bcf5-4a3fecc5a3d0
source-git-commit: c879d06cfe7ba76df3e974c160a7349f1503f17f
workflow-type: tm+mt
source-wordcount: '519'
ht-degree: 0%

---

# 보기 또는 작업 영역에 대한 권한 요청

<!--<span class="preview">The highlighted information on this page refers to functionality not yet generally available. It is available only in the Preview environment for all customers. After the monthly releases to Production, the same features are also available in the Production environment for customers who enabled fast releases. </span>   

<span class="preview">For information about fast releases, see [Enable or disable fast releases for your organization](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/enable-fast-release-process.md). </span>-->

>[!IMPORTANT]
>
>이 문서에 설명된 기능은 조직이 Adobe 통합 경험에 온보딩되었을 때만 사용할 수 있습니다.
>
>자세한 내용은 [Workfront용 Adobe 통합 환경](/help/quicksilver/workfront-basics/navigate-workfront/workfront-navigation/adobe-unified-experience.md)을 참조하십시오.


다른 사용자가 액세스 권한이 없는 보기 또는 작업 영역에 대한 링크를 사용자와 공유하는 경우 보기 또는 작업 영역에 대한 권한을 요청할 수 있습니다.

보기에 대한 권한을 요청하는 것은 작업 공간에 권한을 요청하는 것과 비슷합니다.

이 문서에서는 다른 사용자가 나와 링크를 공유하지만 공유 페이지에 액세스할 수 없는 경우 보기 또는 작업 영역에 대한 액세스를 요청하는 방법에 대해 설명합니다.

보기 및 작업 공간에 대한 권한 부여에 대한 자세한 내용은 다음 문서를 참조하십시오.

* [보기 공유](/help/quicksilver/planning/access/share-views.md)
* [작업 공간 공유](/help/quicksilver/planning/access/share-workspaces.md)


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
   <td role="rowheader"><p>Adobe Workfront 패키지</p></td> 
   <td> 
<p>모든 Workfront 및 Planning 패키지</p> 
또는
<p>모든 워크플로우 및 계획 패키지</p> 
 </tr>

<tr> 
   <td role="rowheader"><p>Adobe Workfront 라이선스</p></td> 
   <td><p>임의</p> 
  </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><p>액세스 수준 구성</p></td> 
   <td> <p>Adobe Workfront Planning에 대한 액세스 수준 제어가 없습니다.</p>   
</td> 
  </tr> 
<tr> 
   <td role="rowheader"><p>개체 권한</p></td> 
   <td>  <p>권한 요청이 부여되면 다음 권한을 얻을 수 있습니다.</p>
   <ul><li><p>보기에 대한 보기 또는 관리</p></li>
   <li><p>작업 공간에 대한 보기, 기여 또는 관리</p></li></ul>  
   <p>작업 공간 및 보기에 대한 관리 권한이 있는 사용자만 보기를 공개적으로 공유할 수 있습니다.</p></td> 
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
<p><b>IMPORTANT</b></p>
<p>The users in your organization can request permissions for views and workspaces only when your organization is onboarded to the Adobe Unified Experience. </p>
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
   <td>  <p>After your request for permission is granted, you could gain the following permissions:</p>
   <ul><li><p>View or Manage for a view</p></li>
   <li><p>View, Contribute, or Manage to a workspace</p></li></ul>  
   <p>Only users with Manage permissions to a workspace and a view can share a view publicly.</p></td> 
  </tr> 
<tr>
   <td role="rowheader"><p>Layout template</p></td>
   <td> Users with a Light or Contributor license must be assigned a layout template that includes Planning.
   <p>Standard users and System Administrators have the Planning areas enabled by default.</p></div></li></ul>
  
</td>
  </tr>
 
</tbody> 
</table> -->


## 보기 또는 작업 영역에 대한 권한 요청

보기에 대한 권한을 요청하는 것은 작업 공간에 권한을 요청하는 것과 비슷합니다.

다른 사용자가 액세스 권한이 없는 작업 영역 또는 보기에 대한 링크를 귀하와 공유하는 경우:

1. 보기 또는 작업 공간에 대해 사용자와 공유되는 링크를 클릭합니다.

   보기 또는 작업 영역에 대한 액세스 권한이 없음을 알리는 **액세스 권한이 없습니다** 페이지가 표시됩니다.

   ![보기에 대한 액세스 권한 요청](assets/request-access-to-view.png)

1. (조건부) 공유 링크가 액세스 권한이 있는 작업 영역의 보기용인 경우 **기존 보기로 열기**&#x200B;를 클릭합니다. 작업공간에 액세스할 수 있는 권한이 있는 경우 기본 보기에서 레코드 유형 페이지가 열립니다.

1. (선택 사항 및 조건부) 작업 영역을 볼 수 있는 권한이 없는 경우 사용 가능한 상자에 개인화된 메시지를 추가한 다음 **액세스 요청**&#x200B;을 클릭합니다.

   보기 또는 작업 공간에 대한 관리 권한이 있는 모든 사용자는 액세스 요청에 대해 다음 알림을 받습니다.
   * 인앱 알림
     ![액세스 요청에 대한 인앱 알림](assets/in-app-notification-for-access-request.png)
   * 이메일 알림
     ![액세스 요청에 대한 전자 메일 알림](assets/email-notification-for-access-request.png)

1. (조건부) 보기 또는 작업 영역 관리자가 보기 또는 작업 영역에 대한 권한을 부여하면 권한이 부여되었음을 확인하는 이메일 알림 및 인앱 알림을 받게 됩니다. <!--check this - I was not able to test this, but Isk confirmed.-->
