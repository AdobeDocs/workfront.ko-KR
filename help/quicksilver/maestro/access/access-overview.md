---
title: 액세스 개요
description: Adobe Maestro 기능을 사용하려면 라이선스 및 공유 권한 제한이 있습니다.
hidefromtoc: true
hide: true
recommendations: noDisplay, noCatalog
exl-id: 99fac041-a235-4991-b826-d19944164bc9
source-git-commit: 1da2e6448f7ac6f4bd5bd76846fbfc1a23c3da77
workflow-type: tm+mt
source-wordcount: '422'
ht-degree: 0%

---

<!--update the metadata with real things when making this public; also update the description with something like this: Not all users in the organization have the same access and permissions to use Adobe Maestro. This article describes the levels of access that users could have to Adobe Maestro. -->
<!--update the title and the metadata title if Maestro is NOT its own product - because the title is too generic for it being a Workfront capability-->

# 액세스 개요

{{maestro-important-intro}}

Adobe Maestro 기능을 사용하려면 라이선스 및 공유 권한 제한이 있습니다.

## 액세스 요구 사항

Adobe Maestro를 사용하려면 다음 설정이 있어야 합니다.

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
   <p> Adobe Workfront</p> </td>
  </tr>  
 <td role="rowheader"><p>Adobe Workfront 계약</p></td>
   <td>
<p>Adobe Maestro Closed Beta 프로그램에 조직을 등록해야 합니다. </p>
   </td>
  </tr>
  <tr>
   <td role="rowheader"><p>Adobe Workfront 플랜</p></td>
   <td>
<p>임의</p>
   </td>
  </tr>
  <tr>
   <td role="rowheader"><p>Adobe Workfront 라이센스*</p></td>
   <td>
   <p>임의</p>
   <p>작업 공간을 만들려면 다음 라이센스가 있어야 합니다.</p>
   <ul>
   <li>
   새로운 기능: 표준
   </li>
   <li>
   현재: 작업자 이상
   </li>
   </ul>
  </td>
  </tr>
  <tr>
   <td role="rowheader"><p>액세스 수준 구성</p></td>
   <td> <p>Maestro 개체에 대한 액세스 수준 컨트롤이 없습니다.</p>  
</td>
  </tr>
<tr>
   <td role="rowheader"><p>개체 권한</p></td>
   <td>
   <p>작업 공간 및 보기를 편집, 삭제 및 공유하고, 레코드 유형 및 레코드를 생성, 편집 또는 삭제하기 위해 작성하지 않은 작업 공간 및 보기에 대해 또는 그 이상의 권한을 제공하십시오.</p>
    <p>시스템 관리자는 자신이 만들지 않은 작업 공간 및 보기를 관리할 수 있습니다 </p>
   <p>Maestro 객체의 권한 공유에 대한 자세한 내용은  
   <a href="../access/sharing-permissions-overview.md">Adobe Maestro에서의 권한 공유 개요</a> 
  </td>
  </tr>
<tr>
   <td role="rowheader"><p>레이아웃 템플릿</p></td>
   <td> <p>Workfront 관리자를 포함한 모든 사용자에게 메인 메뉴의 마에스트로 영역을 포함하는 레이아웃 템플릿을 할당해야 합니다. </p> <p>자세한 내용은 <a href="/help/quicksilver/maestro/access/access-overview.md">액세스 개요</a>. </p>  
</td>
  </tr>
 </tbody>
</table>

*Workfront 액세스 요구 사항에 대한 자세한 내용은 [Workfront 설명서의 액세스 요구 사항](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).


## 다른 사용자와 메인 메뉴의 마에스트로 영역 공유

<!--First, contact your account manager to obtain access to the current Maestro closed beta program.-->

조직이 Maestro Beta 프로그램에 등록되면 레이아웃 템플릿을 사용하여 모든 사용자의 메인 메뉴에 Maestro 영역을 추가할 수 있습니다.

1. 에 로그인 **Workfront** Workfront 관리자입니다.

1. 추가 **마에스트로** 아이콘 ![](assets/maestro-icon.png) (으)로 **메인 메뉴** 사용 **레이아웃 템플릿**.

   자세한 내용은 [레이아웃 템플릿을 사용하여 메인 메뉴 사용자 정의](../../administration-and-setup/customize-workfront/use-layout-templates/customize-main-menu.md).

1. Maestro에 액세스하려는 사용자에게 레이아웃 템플릿을 할당합니다.

   자세한 내용은 [레이아웃 템플릿에 사용자 할당](../../administration-and-setup/customize-workfront/use-layout-templates/assign-users-to-layout-template.md).

   템플릿에 할당된 모든 사용자는 이제 메인 메뉴에서 Maestro에 액세스할 수 있습니다.

   사용자는 작업 공간, 레코드 유형, 레코드 및 필드를 만들 수 있습니다.

## 액세스 권한 부여

Maestro에 대한 액세스 제어가 없습니다.

모든 유형의 라이선스가 있는 사용자는 Maestro에 액세스할 수 있습니다.

Workfront에서의 액세스 권한 부여에 대한 자세한 내용은 [사용자 정의 액세스 수준 만들기 및 수정](/help/quicksilver/administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md).

## 권한 부여

시스템 관리자가 아닌 사용자에게 작업 공간 및 사용자가 만든 보기에 대한 권한을 부여해야 작업 공간에 액세스할 수 있습니다.

자세한 내용은 [Adobe Maestro의 공유 권한 개요](/help/quicksilver/maestro/access/sharing-permissions-overview.md).

Adobe Workfront 라이선스 유형은 Maestro 권한과 함께 작동하여 Maestro 개체를 보거나, 기여하거나, 관리할 수 있는 액세스 권한을 부여합니다.

라이선스 유형이 Maestro 객체의 권한 수준에 어떤 영향을 미치는지에 대한 자세한 내용은 [Adobe Workfront 계획 기능 사용 시 라이선스 유형 개요](/help/quicksilver/maestro/access/license-type-overview.md).


