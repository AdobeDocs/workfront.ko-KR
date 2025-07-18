---
title: 보기 또는 작업 영역 사용 권한 요청
description: 다른 사용자가 액세스 권한이 없는 보기 또는 작업 영역에 대한 링크를 공유하는 경우 이를 열 수 있는 권한을 요청 할 수 있습니다. 이 문서에서는 열 수 없는 공유 링크가 있는 경우 보기 또는 작업 영역에 대한 액세스를 요청 하는 단계를 설명합니다.
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

# 보기 또는 작업 영역 사용 권한 요청

<!--<span class="preview">The highlighted information on this page refers to functionality not yet generally available. It is available only in the Preview environment for all customers. After the monthly releases to Production, the same features are also available in the Production environment for customers who enabled fast releases. </span>   

<span class="preview">For information about fast releases, see [Enable or disable fast releases for your organization](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/enable-fast-release-process.md). </span>-->

>[!IMPORTANT]
>
>이 문서에 설명된 기능은 조직이 Adobe Systems 통합 환경에 온보딩된 경우에만 사용할 수 있습니다.
>
>자세한 내용은 Adobe Systems Unified Experience for Workfront[를 참조하십시오](/help/quicksilver/workfront-basics/navigate-workfront/workfront-navigation/adobe-unified-experience.md).


다른 사용자가 액세스 권한이 없는 보기 또는 작업 영역에 대한 링크를 사용자와 공유하는 경우 보기 또는 작업 영역에 대한 사용 권한을 요청할 수 있습니다.

뷰에 대한 사용 권한을 요청하는 것은 작업 영역 에 대한 사용 권한을 요청하는 것과 비슷합니다.

이 문서에서는 다른 사용자가 사용자와 링크를 공유하고 공유 페이지에 액세스할 수 없는 경우 보기 또는 작업 영역에 대한 액세스를 요청하는 방법을 설명합니다.

보기 및 작업 영역에 권한을 부여하는 방법에 대한 자세한 내용은 다음 문서를 참조하세요.

* [조회수 공유](/help/quicksilver/planning/access/share-views.md)
* [작업 공간 공유](/help/quicksilver/planning/access/share-workspaces.md)


## 액세스 요구 사항

+++ 액세스 요구 사항을 보려면 확장합니다.

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
   <li><p> Adobe Workfront Planning<p></li></ul></td> 
  </tr>   
<tr> 
   <td role="rowheader"><p>Adobe Systems Workfront 플랜*</p></td> 
   <td> 
<p>다음 Workfront 플랜 중 하나:</p> 
<ul><li>선택</li> 
<li>Prime</li> 
<li>Ultimate</li></ul> 
<p>Workfront Planning은 기존 Workfront 플랜에 사용할 수 없습니다</p> 
   </td> 
<tr> 
   <td role="rowheader"><p>Adobe Systems Workfront 계획 패키지*</p></td> 
   <td> 
<p>어떤 </p> 
<p>각 Workfront Planning 플랜에 포함된 항목에 대한 자세한 내용은 Workfront 계정 관리자 관리자에게 문의하십시오. </p> 
   </td> 
 <tr> 
   <td role="rowheader"><p>Adobe Systems Workfront 플랫폼</p></td> 
   <td> 
<p>Workfront Planning에 액세스하려면 조직의 Workfront 인스턴스가 Adobe Systems 통합 환경에 온보딩되어 있어야 합니다.</p> 
<p><b>중요하다</b></p>
<p>조직의 사용자는 조직이 Adobe Systems 통합 환경에 온보딩된 경우에만 보기 및 작업 영역에 대한 권한을 요청 할 수 있습니다. </p>
<p>자세한 내용은 Adobe Systems Unified Experience for Workfront<a href="/help/quicksilver/workfront-basics/navigate-workfront/workfront-navigation/adobe-unified-experience.md">를 참조하십시오</a>. </p> 
   </td> 
   </tr> 
  </tr> 
  <tr> 
   <td role="rowheader"><p>Adobe Systems Workfront 라이선스*</p></td> 
   <td><p> 표준, 경량 또는 참가자</p>
   <p>Workfront Planning은 기존 Workfront 라이선스에 사용할 수 없습니다</p> 
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
   <li><p>작업 영역 보기, Contribute 또는 관리</p></li></ul>  
   <p>작업 영역 및 뷰에 대한 관리 권한이 있는 사용자만 뷰를 공개적으로 공유할 수 있습니다.</p></td> 
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


## 보기 또는 작업 영역 에 대한 사용 권한 요청

뷰에 대한 사용 권한을 요청하는 것은 작업 영역에 대한 권한 요청하는 것과 비슷합니다.

다른 사람이 액세스 권한이 없는 작업 영역 또는 보기에 대한 링크 링크를 공유하는 경우:

1. 보기 또는 작업 영역에 대해 사용자와 공유된 링크 를 클릭합니다.

   A **: 액세스** 권한이 없습니다 페이지 표시를 통해 뷰 또는 작업 영역 액세스 권한이 없음을 알립니다.

   ![보기 액세스 권한 요청](assets/request-access-to-view.png)

1. (조건부) 공유 링크가 액세스 권한이 있는 작업 영역의 보기용인 경우 **기존 보기로 열기**&#x200B;를 클릭합니다. 작업 영역 영역에 액세스할 수 있는 권한이 있는 경우 레코드 종류 페이지 페이지가 기본 보기에서 열립니다.

1. (선택 사항 및 조건부) 작업 영역을 볼 수 있는 권한이 없는 경우 사용 가능한 상자에 개인화된 메시지를 추가한 다음 **액세스 요청**&#x200B;을 클릭합니다.

   보기 또는 작업 영역에 대한 관리 권한이 있는 모든 사용자는 액세스 요청에 대해 다음과 같은 알림을 받습니다.
   * 인앱 알림

     ![액세스 요청에 대한 인앱 알림](assets/in-app-notification-for-access-request.png)
   * 이메일 알림

     ![액세스 요청 위한 이메일 알림](assets/email-notification-for-access-request.png)

1. (조건부) 보기 또는 작업 영역 관리자가 보기 또는 작업 영역에 대한 권한을 부여하면 권한 부여되었다는 확인 알림이메일과 인앱 알림 받게 됩니다. <!--check this - I was not able to test this, but Isk confirmed.-->
