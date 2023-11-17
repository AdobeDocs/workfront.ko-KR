---
title: 액세스 개요
description: 조직의 모든 사용자는 Adobe Maestro에 액세스할 수 있습니다. 현재 Maestro에는 사용자 또는 정보와 연관된 액세스 수준이나 권한이 없습니다.
hidefromtoc: true
hide: true
recommendations: noDisplay, noCatalog
exl-id: 99fac041-a235-4991-b826-d19944164bc9
source-git-commit: 8012b56fda0b4f260f667ac8e5d87cc5d537631c
workflow-type: tm+mt
source-wordcount: '234'
ht-degree: 2%

---

<!--update the metadata with real things when making this public; also update the description with something like this: Not all users in the organization have the same access and permissions to use Adobe Maestro. This article describes the levels of access that users could have to Adobe Maestro. -->

# 액세스 개요

>[!IMPORTANT]
>
>이 문서의 정보는 Adobe Workfront의 새로운 오퍼링인 Adobe Maestro를 참조합니다.
>
>현재 Adobe 마에스트로는 제한된 수의 고객에게 제공되는 베타 프로그램의 일부입니다. Maestro에 액세스하려면 Workfront 고객이어야 합니다.
>
>Maestro용 Beta 프로그램 가입에 대한 자세한 내용은 계정 담당자에게 문의하십시오.
>
>자세한 내용은 [Adobe 마에스트로 개요](../maestro-overview.md).

<!-- the table will change after we implement access levels/ permissions for Maestro-->
<!-- fix the formatting on the table - some lines are way too spaced out-->

## 액세스 요구 사항

Adobe Maestro에는 액세스 수준 제한이 없습니다.

조직의 모든 사용자는 액세스 수준에 관계없이 Maestro에 액세스할 수 있습니다.

Adobe Maestro를 사용하려면 다음 사항이 있어야 합니다.

<table style="table-layout:auto">
 <col>
 </col>
 <col>
 </col>
 <tbody>
    <tr>
<tr>
<td>
   <p> Adobe 제품</p> </td>
   <td>
   <p> Adobe Workfront</p> </td>
  </tr>  
 <td role="rowheader"><p>Adobe Workfront 계약</p></td>
   <td>
<p>Adobe Maestro Closed Beta 프로그램에 조직을 등록해야 합니다. 이 새 제품에 대해 문의하려면 계정 담당자에게 문의하십시오. </p>
   </td>
  </tr>
  <tr>
   <td role="rowheader"><p>Adobe Workfront 플랜</p></td>
   <td>
<p>모든</p>
   </td>
  </tr>
  <tr>
   <td role="rowheader"><p>Adobe Workfront 라이선스</p></td>
   <td>
   <p>모든</p> 
  </td>
  </tr>

<tr>
   <td role="rowheader"><p>액세스 수준</p></td>
   <td> <p>모든</p>  
</td>
  </tr>

<tr>
   <td role="rowheader"><p>레이아웃 템플릿</p></td>
   <td> <p>시스템 관리자는 메인 메뉴의 마에스트로 영역을 레이아웃 템플릿에 추가해야 합니다.</p> 
   <p>자세한 내용은 <a href="../../administration-and-setup/customize-workfront/use-layout-templates/customize-main-menu.md">레이아웃 템플릿을 사용하여 메인 메뉴 사용자 정의</a>. </p>  
</td>
  </tr>
 </tbody>
</table>

<!--After we enable permissions, replace the table above with this: 

<table style="table-layout:auto">
 <col>
 </col>
 <col>
 </col>
 <tbody>
    <tr>
<tr>
<td>
   <p> Adobe product</p> </td>
   <td>
   <p> Adobe Workfront</p> </td>
  </tr>  
 <td role="rowheader"><p>Adobe Workfront agreement</p></td>
   <td>
<p>Your organization must be enrolled in the Adobe Maestro closed beta program. Contact your account representative to inquire about this new offering. </p>
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
   <p>Any license to view, manage, or contribute to Maestro objects</p> 
   <p>System Administrator to create Maestro objects</p>
  </td>
  </tr>
  
  <tr>
   <td role="rowheader"><p>Access level</p></td>
   <td> <p>Any</p>  
</td>
  </tr>

<tr>
   <td role="rowheader"><p>Layout template</p></td>
   <td> <p>Your system administrator must add the Maestro area in the Main Menu to your layout template.</p> 
   <p>For information, see <a href="../../administration-and-setup/customize-workfront/use-layout-templates/customize-main-menu.md">Customize the Main Menu using a layout template</a>. </p>  
</td>
  </tr>
 </tbody>
</table>
-->

<!-- Notes to add for the table: for the "Workfront plans" row: the above is only for closed beta; when going to GA - activate the following plans:    
<p>Current plan: Prime and Ultimate</p>
<p>Legacy plan: Enterprise</p>-->

<!-- Notes for the table: for the "Workfront access" row: <p>For more information, see <a href="../../administration-and-setup/add-users/access-levels-and-object-permissions/wf-licenses.md" class="MCXref xref">Adobe Workfront licenses overview</a>.</p>-->

## 권한 공유

Maestro 오브젝트와 연계된 권한이 없습니다.

해당 환경에서 Maestro가 활성화된 모든 사용자는 다른 사용자가 Maestro에 추가하는 모든 정보를 보고, 편집하고, 삭제할 수 있습니다.

<!--
Replace the Sharing permissions information with this, when we release permissions: 

All users can have access to the Maestro area in the Main Menu. However, only Workfront administrators can create Maestro objects. Users with any other license type can access Maestro workspaces and their information only when workspaces are shared with them. 

Consider the following when sharing permissions to Maestro: 

* You can share only workspaces in Maestro. After a Workfront administrator shares a workspace with you, you can view record types, records, and fields in the workspace. 
* All Workfront administrators have access to edit or delete existing workspaces, even when they are created by other users. 

For information about sharing the Maestro area with users or sharing permissions to Maestro workspaces, see the following articles:

   * [Overview of sharing permissions in Adobe Maestro](../access/sharing-permissions-overview.md)
   * [Grant access to Adobe Maestro](../access/grant-access.md) -->

