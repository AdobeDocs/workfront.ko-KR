---
title: 보기 또는 Workspace에 권한 요청
description: 다른 사용자가 액세스 권한이 없는 보기 또는 작업 영역에 대한 링크를 공유할 경우 열 수 있는 권한을 요청할 수 있습니다. 이 문서에서는 열 수 없는 공유 링크가 있을 때 보기 또는 작업 영역에 대한 액세스를 요청하는 단계에 대해 설명합니다.
feature: Workfront Planning
role: User, Admin
author: Alina
recommendations: noDisplay, noCatalog
exl-id: 94dfa36a-801a-4eef-bcf5-4a3fecc5a3d0
last-update: 2026-04-01T18:03:50.000Z
git-commit-file: b03dbe8e217593e0f3a6fcd522148dcd8b7670b8
TQID: https://experienceleague.adobe.com/FvXVCMMz-PfaT-QAaMq0c5qUruR1MJoMv6etcrAstXA
product_v2: id: c4a86a5d-6562-4fc6-aa00-bfa25833aed9
feature_v2: id: d968a1bc-9a90-4926-a531-bcf272c32aad
role_v2: id: b69b2659-1057-424e-8fc5-ed9e016dc554id: c66ffd68-0f65-42bb-aa23-b4020f12e0bd
topic_v2: id: eddd9b14-83bd-4ff4-9072-54a4a484abb7
source-git-commit: 37be1f25fa54f3efd4113478496e95db3c8bce1c
workflow-type: tm+mt
source-wordcount: 567
ht-degree: 3%

---

# 보기 또는 작업 영역에 대한 권한 요청


<span class="preview">이 페이지에서 강조 표시된 정보는 아직 일반적으로 사용할 수 없는 기능을 참조합니다. 모든 고객을 위한 미리보기 환경에서만 사용할 수 있습니다. 미리보기에 릴리스된 후 빠른 릴리스를 활성화한 고객을 위해 프로덕션 환경에서도 매월 동일한 기능을 사용할 수 있습니다. </span>

<span class="preview">빠른 릴리스에 대한 자세한 내용은 [조직의 빠른 릴리스 사용 또는 사용 안 함](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/enable-fast-release-process.md)을 참조하세요. </span>


<!-- 
no longer needed: 
>[!IMPORTANT]
>
>The functionality described in this article is available only when your organization has been onboarded to the Adobe Unified Experience. 
>
>For more information, see [Adobe Unified Experience for Workfront](/help/quicksilver/workfront-basics/navigate-workfront/workfront-navigation/adobe-unified-experience.md). 
-->

다른 사용자가 액세스 권한이 없는 보기 또는 작업 영역에 대한 링크를 사용자와 공유하는 경우 보기 또는 작업 영역에 대한 권한을 요청할 수 있습니다.

보기에 대한 권한을 요청하는 것은 작업 공간에 권한을 요청하는 것과 비슷합니다.

이 문서에서는 다른 사용자가 나와 링크를 공유하지만 공유 페이지에 액세스할 수 없는 경우 보기 또는 작업 영역에 대한 액세스를 요청하는 방법에 대해 설명합니다.

보기 및 작업 공간에 대한 권한 부여에 대한 자세한 내용은 다음 문서를 참조하십시오.

* [보기 공유](/help/quicksilver/planning/access/share-views.md)
* [작업 공간 공유](/help/quicksilver/planning/access/share-workspaces.md)


## 액세스 요구 사항

+++ 이 문서의 기능에 대한 액세스 요구 사항을 보려면 확장하십시오. 

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
   <td><p>Any</p> 
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
   <li><p>작업 공간에 대한 보기, 기여 또는 관리</p></li>
   <li><p>레코드 종류에 대한 보기, 기여 또는 관리</p></li>
   <li><p><span class="preview">레코드에 대한 보기 또는 관리</span></p></li>
   </ul>  
   <p>작업 공간 및 보기에 대한 관리 권한이 있는 사용자만 보기를 공개적으로 공유할 수 있습니다.</p></td> 
  </tr> 
</tbody> 
</table>

Workfront 액세스 요구 사항에 대한 자세한 내용은 Workfront 설명서의 [액세스 요구 사항](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)을 참조하십시오.

+++

<!--
 Old:
 
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
</table>
-->


## 권한 요청

보기에 대한 권한을 요청하는 것은 작업 영역, 레코드 종류 또는 <span class="preview">레코드</span>에 대한 권한을 요청하는 것과 비슷합니다.

다른 사용자가 작업 영역, 레코드 종류, <span class="preview">레코드</span> 또는 액세스 권한이 없는 보기에 대한 링크를 귀하와 공유하는 경우:

1. 보기 또는 작업 공간에 대해 사용자와 공유되는 링크를 클릭합니다.

   보기 또는 작업 영역에 대한 액세스 권한이 없음을 알리는 **액세스 권한이 없습니다** 페이지가 표시됩니다.

   ![보기에 대한 액세스 권한 요청](assets/request-access-to-view.png)

   >[!NOTE]
   >
   >레코드 종류 또는 <span class="preview">레코드</span>에 대한 액세스 권한이 없는 경우 페이지에 대한 액세스 권한이 없으면 작업 영역에 대한 액세스 권한이 있어야 합니다.


1. (조건부) 공유 링크가 액세스 권한이 있는 작업 영역의 보기용인 경우 **기존 보기로 열기**&#x200B;를 클릭합니다. 작업공간에 액세스할 수 있는 권한이 있는 경우 기본 보기에서 레코드 유형 페이지가 열립니다.

1. (선택 사항 및 조건부) 작업 영역을 볼 수 있는 권한이 없는 경우 사용 가능한 상자에 개인화된 메시지를 추가한 다음 **액세스 요청**&#x200B;을 클릭합니다.

   보기 또는 작업 공간에 대한 관리 권한이 있는 모든 사용자는 액세스 요청에 대해 다음 알림을 받습니다.
   * 인앱 알림
     ![액세스 요청에 대한 인앱 알림](assets/in-app-notification-for-access-request.png)
   * 이메일 알림
     ![액세스 요청에 대한 전자 메일 알림](assets/email-notification-for-access-request.png)

1. (조건부) 보기 또는 작업 영역 관리자가 보기 또는 작업 영역에 대한 권한을 부여하면 권한이 부여되었음을 확인하는 이메일 알림 및 인앱 알림을 받게 됩니다. <!--check this - I was not able to test this, but Isk confirmed.-->
