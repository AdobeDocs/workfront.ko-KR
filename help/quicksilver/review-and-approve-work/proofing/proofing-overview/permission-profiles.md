---
content-type: overview
product-area: documents
keywords: 증명,권한
navigation-topic: proofing-overview
title: 증명 권한 프로필 개요
description: 증명 권한 프로필은 사용자가 계정의 모든 증명에 대해 가지고 있는 전체 권한을 결정합니다. 증명 권한 프로필은 사용자 프로필의 사용자에게 할당됩니다. 증명 권한 프로필은 증명 역할과 다릅니다. 증명 역할에 대한 자세한 내용은 증명 역할 개요를 참조하십시오.
author: Courtney
feature: Digital Content and Documents
exl-id: fb6faa48-d97b-4b7b-83ae-fe39d40b3963
source-git-commit: 9b60133c4cc20deb410f507854597f44d0607228
workflow-type: tm+mt
source-wordcount: '516'
ht-degree: 2%

---

# 증명 권한 프로필 개요

증명 권한 프로필은 사용자가 계정의 모든 증명에 대해 가지고 있는 전체 권한을 결정합니다. 증명 권한 프로필은 사용자 프로필의 사용자에게 할당됩니다. 증명 권한 프로필은 증명 역할과 다릅니다. 증명 역할에 대한 자세한 내용은 [증명 역할 개요](../../../review-and-approve-work/proofing/proofing-overview/proof-roles.md).

>[!NOTE]
>
>관리자는 조직의 사용자에 대한 사용자 지정 프로필을 만들 수 있습니다. 자세한 내용은 [Workfront 증명의 사용자 지정 프로필 구성](../../../workfront-proof/wp-acct-admin/account-settings/configure-custom-profiles.md).

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">Consider the following about roles and permissions:</p>
-->

<!--
<ul data-mc-conditions="QuicksilverOrClassic.Draft mode">
<li> <p>Assigned profile permissions relate only to the users and items in your own account. The exception is in the case of Satellite accounts, where the Administrator and Billing Administrator for the main (hub) accounts can access and manage the&nbsp;account settings&nbsp;and billing of those accounts from the hub account level.</p> </li>
<li> <p>Billing Administrators and Administrators can delete users. This can only be done in&nbsp;Account settings.</p> </li>
<li>When Billing Administrators and Administrators view proofs that are owned by other users in their account, they view them with the role of a Reviewer.</li>
<li>Using the Read Only role, Billing Administrators and Administrators can access proofs in folders shared with them or in folders created by them.&nbsp;</li>
</ul>
-->

## 증명 권한 프로필

다음 표에는 각 증명 권한 프로필에서 사용할 수 있는 권한이 표시됩니다.

<table>
  <tr>
   <td colspan="5" ><strong>고유 항목</strong>
   </td>
   <td colspan="3" ><strong>기타 사용자 항목</strong>
   </td>
   <td><strong>관리자</strong>
   </td>
  </tr>
  <tr>
   <td>
   </td>
   <td><strong>추가</strong>
   </td>
   <td><strong></strong> 보기
   </td>
   <td><strong>편집</strong>
   </td>
   <td><strong>삭제</strong>
   </td>
   <td><strong></strong> 보기
   </td>
   <td><strong>편집</strong>
   </td>
   <td><strong>삭제</strong>
   </td>
   <td><strong>편집 및 삭제</strong>
   </td>
  </tr>
  <tr>
   <td>관리자
   </td>
   <td>x
   </td>
   <td>x
   </td>
   <td>x
   </td>
   <td>x
   </td>
   <td>x
   </td>
   <td>x
   </td>
   <td>x
   </td>
   <td>x
   </td>
  </tr>
  <tr>
   <td>감독자
   </td>
   <td>x
   </td>
   <td>x
   </td>
   <td>x
   </td>
   <td>x
   </td>
   <td>x
   </td>
   <td>x
   </td>
   <td>x
   </td>
   <td>
   </td>
  </tr>
  <tr>
   <td>관리자
   </td>
   <td>x
   </td>
   <td>x
   </td>
   <td>x
   </td>
   <td>x
   </td>
   <td>
   </td>
   <td>
   </td>
   <td>
   </td>
   <td>
   </td>
  </tr>
  <tr>
   <td>관찰자
   </td>
   <td>
   </td>
   <td>x
   </td>
   <td>
   </td>
   <td>
   </td>
   <td>
   </td>
   <td>
   </td>
   <td>
   </td>
   <td>
   </td>
  </tr>
</table>

### 관리자

관리자는 [계정 설정](https://support.workfront.com/hc/en-us/sections/115000912147-Account-Settings) 및에 다음 권한이 있습니다.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>관리자는 다음을 수행할 수 있습니다.</td> 
   <td>관리자는 다음을 수행할 수 없습니다.</td> 
  </tr> 
  <tr> 
   <td> 
    <ul> 
     <li> <p>증명 만들기, 파일 업로드 및 폴더 만들기</p> </li> 
     <li> <p>증명 및 파일을 보고 편집하고 삭제합니다</p> </li> 
     <li> <p>조직의 모든 사용자가 만든 증명 및 파일을 보고 편집하고 삭제합니다</p> </li> 
     <li> <p>다른 사용자의 공용 폴더 삭제</p> </li> 
     <li> <p>계정에서 만든 모든 증명 편집</p> </li> 
     <li> <p>Dropzone 소유자로 설정*</p> </li> 
     <li> <p>계정 설정 페이지에 액세스하여 계정 세부 사항을 편집합니다</p> </li> 
     <li> <p>휴지통으로 이동</p> </li> 
     <li> <p>사용자 추가, 편집 및 삭제</p> </li> 
     <li> <p>그룹 만들기 및 새 연락처 추가</p> </li> 
     <li> <p>연락처 삭제</p> </li> 
     <li> <p>답장이 없으면 증명을 편집합니다</p> </li> 
    </ul> </td> 
   <td> 
    <ul> 
     <li> <p>증명 답글을 편집합니다.</p> </li> 
     <li> <p>다른 사용자의 개인 폴더 삭제</p> </li> 
     <li> <p>청구 페이지에 액세스하거나 청구 상세내역을 편집합니다</p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Workfront Proof 독립 실행형 제품에서만 사용할 수 있습니다.

### 감독자

감독자에게는 다음 권한이 있습니다.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>감독자는 다음을 수행할 수 있습니다.</td> 
   <td>감독자는 다음을 수행할 수 없습니다.</td> 
  </tr> 
  <tr> 
   <td> 
    <ul> 
     <li> <p>증명 만들기, 파일 업로드 및 폴더 만들기</p> </li> 
     <li> <p>증명 및 파일을 보고 편집하고 삭제합니다</p> </li> 
     <li> <p>조직의 모든 사용자가 만든 증명 및 파일을 보고 편집하고 삭제합니다</p> </li> 
     <li> <p>다른 사용자의 공용 폴더 삭제</p> </li> 
     <li> <p>계정에서 만든 모든 증명 편집</p> </li> 
     <li> <p>그룹 만들기 및 새 연락처 추가</p> </li> 
     <li> <p>연락처 삭제</p> </li> 
     <li> <p>답장이 없으면 증명을 편집합니다</p> </li> 
    </ul> </td> 
   <td> 
    <ul> 
     <li> <p>증명 답글을 편집합니다.</p> </li> 
     <li> <p>다른 사용자의 개인 폴더 삭제</p> </li> 
     <li> <p>청구 페이지에 액세스하거나 청구 상세내역을 편집합니다</p> </li> 
     <li> <p>사용자 추가, 편집 또는 삭제</p> </li> 
     <li> <p>휴지통으로 이동</p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

### 관리자

관리자는 다음 권한을 가집니다.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>관리자는 다음을 수행할 수 있습니다.</td> 
   <td>관리자는 다음을 수행할 수 없습니다.</td> 
  </tr> 
  <tr> 
   <td> 
    <ul> 
     <li> <p>증명 만들기, 파일 업로드 및 폴더 만들기</p> </li> 
     <li> <p>증명 및 파일을 보고 편집하고 삭제합니다</p> </li> 
     <li> <p>사용자와 명시적으로 공유되는 다른 사용자에 대한 증명을 보고, 검토하고, 승인합니다(공유 폴더의 모든 항목에 대한 읽기 전용 권한)</p> </li> 
     <li> <p>계정에서 만든 모든 증명 편집</p> </li> 
     <li> <p>그룹 만들기 및 새 연락처 추가</p> </li> 
    </ul> </td> 
   <td> 
    <ul> 
     <li> <p>조직의 다른 사용자가 만든 증명 및 파일을 보거나, 편집하거나, 삭제합니다. </p> <p>증명 답글을 편집합니다.</p> </li> 
     <li> <p>다른 사용자의 개인 또는 공용 폴더 삭제</p> </li> 
     <li> <p>청구 페이지에 액세스하거나 청구 상세내역을 편집합니다</p> </li> 
     <li> <p>사용자 추가, 편집 또는 삭제</p> </li> 
     <li> <p> 연락처 삭제</p> </li> 
     <li> <p>휴지통으로 이동</p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

<!--
<h3 data-mc-conditions="QuicksilverOrClassic.Draft mode">Observer</h3>
-->

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">Observers have the following permissions:</p>
-->

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode"> <img src="assets/cleaner2.png">Can see, review, and approve proofs of other users that are explicitly shared with them (Read-only&nbsp;rights to everything in a shared folder). For more information, see <a href="../../../workfront-proof/wp-work-proofsfiles/share-proofs-and-files/manage-proof-roles.md" class="MCXref xref">Manage Proof Roles in Workfront Proof</a>.</p>
-->

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode"> <img src="assets/cleaner2.png">Can view files that are explicitly shared with them.&nbsp;</p>
-->

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode"> <img src="assets/no2.png">Cannot&nbsp;create proofs, upload files, and create folders. For more information, see <a href="../../../workfront-proof/wp-work-proofsfiles/create-proofs-and-files/upload-files-web-content.md" class="MCXref xref">Upload Files and Web Content to Workfront Proof</a>.</p>
-->

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode"> <img src="assets/no2.png">Cannot view, edit, or delete proofs and files created by other users in the organization.</p>
-->

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode"> <img src="assets/no2.png">Cannot edit proofs&nbsp;or replies.</p>
-->

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode"> <img src="assets/no2.png">Cannot delete any items created in the organization.</p>
-->

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode"> <img src="assets/no2.png">Cannot access&nbsp;the Billing page or Account settings. For more information, see <a href="../../../workfront-proof/wp-billingsettings/manage-your-billing/wp-billing-page.md" class="MCXref xref">The Workfront Proof Billing Page</a>&nbsp;and&nbsp;<a href="../../../workfront-proof/wp-acct-admin/account-settings/account-settings.md" class="MCXref xref">Account settings in Workfront Proof</a>.</p>
-->

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode"> <img src="assets/no2.png">Cannot be set as the Dropzone owner. For more information, see <a href="../../../workfront-proof/wp-acct-admin/account-settings/configure-dropzone-in-wp.md" class="MCXref xref">Configure the dropzone in Workfront Proof</a>.</p>
-->

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode"> <img src="assets/no2.png">Cannot empty the&nbsp;trash. For more information, see <a href="../../../workfront-proof/wp-work-proofsfiles/manage-your-work/restore-and-empty-trash.md" class="MCXref xref">Restore and Empty the Trash in Workfront Proof</a>.</p>
-->

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode"> <img src="assets/no2.png">Cannot add, edit, or delete users.&nbsp;</p>
-->

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode"> <img src="assets/no2.png">Cannot create groups or add new contacts.&nbsp;</p>
-->

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode"> <img src="assets/no2.png">Cannot delete contacts.&nbsp;</p>
-->


><!--
><p data-mc-conditions="QuicksilverOrClassic.Draft mode">Menus and functions available to Observers are limited.&nbsp;</p>>
>-->
>  <!--
>  <li data-mc-conditions="QuicksilverOrClassic.Draft mode">Observers do not see the Header menu or the green New menu in their Dashboard</li>>
>  -->
>  <!--
>  <li data-mc-conditions="QuicksilverOrClassic.Draft mode">Observers do not see the following links in their Settings:&nbsp;Account settings,&nbsp;Billing </li>>
>  -->


<!--
<h3 data-mc-conditions="QuicksilverOrClassic.Draft mode">Guest</h3>
-->

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">The Guest profile is used to give access to proofs for reviewers who do not have their own Workfront Proof account. Guests can access proofs shared with them directly via their personal email notifications.</p>
-->

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode"> <img src="assets/cleaner2.png">Can view, review, and approve proofs that are explicitly shared with them.</p>
-->

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode"> <img src="assets/cleaner2.png">Can view files that are explicitly shared with them.</p>
-->

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode"> <img src="assets/no2.png">Cannot access the Dashboard.</p>
-->

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode"> <img src="assets/no2.png">Cannot have folders shared with them. For more information, see <a href="../../../workfront-proof/wp-work-proofsfiles/organize-your-work/manage-folders.md" class="MCXref xref">Manage Folders in Workfront Proof</a>.</p>
-->

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode"> <img src="assets/no2.png">Cannot be added as Authors or Moderators to the proofs. For more information, see <a href="../../../workfront-proof/wp-work-proofsfiles/share-proofs-and-files/manage-proof-roles.md" class="MCXref xref">Manage Proof Roles in Workfront Proof</a>.</p>
-->

<!--
<note type="note">
&nbsp;Guests are not Workfront Proof users, so they cannot see all the proofs shared with them in their own Dashboard.
</note>
-->
