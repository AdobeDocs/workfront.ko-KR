---
title: 보기 또는 Workspace에 권한 요청
description: 다른 사용자가 액세스 권한이 없는 보기 또는 작업 영역에 대한 링크를 공유할 경우 열 수 있는 권한을 요청할 수 있습니다. 이 문서에서는 열 수 없는 공유 링크가 있을 때 보기 또는 작업 영역에 대한 액세스를 요청하는 단계에 대해 설명합니다.
feature: Workfront Planning
role: User, Admin
author: Alina
recommendations: noDisplay, noCatalog
exl-id: 94dfa36a-801a-4eef-bcf5-4a3fecc5a3d0
source-git-commit: 298c542afea902d9fc14ef6a4470c0bc1d9bd33c
workflow-type: tm+mt
source-wordcount: '629'
ht-degree: 1%

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

+++ 를 확장하여 액세스 요구 사항을 확인합니다.

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
<p>Workfront Planning에 액세스하려면 조직의 Workfront 인스턴스가 Adobe 통합 경험에 온보딩되어야 합니다.</p> 
<p><b>중요 사항</b></p>
<p>조직의 사용자는 조직이 Adobe 통합 환경에 온보딩될 때만 보기 및 작업 영역에 대한 권한을 요청할 수 있습니다. </p>
<p>자세한 내용은 <a href="/help/quicksilver/workfront-basics/navigate-workfront/workfront-navigation/adobe-unified-experience.md">Workfront용 Adobe 통합 환경</a>을 참조하십시오. </p> 
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

*Workfront 액세스 요구 사항에 대한 자세한 내용은 Workfront 설명서의 [액세스 요구 사항](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)을 참조하십시오.

+++


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
