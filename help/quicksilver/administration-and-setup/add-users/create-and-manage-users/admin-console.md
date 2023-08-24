---
title: Adobe Admin Console에서 사용자 관리
description: Adobe 관리자는 Adobe Admin Console을 사용하여 Adobe Workfront 사용자와 시스템 관리자를 만들 수 있습니다.
author: Becky, Caroline
feature: System Setup and Administration
role: Admin
exl-id: ae657964-d4a5-4c3b-afc6-8dde7695955d
source-git-commit: 01b60a2fab1188c8510857490ea87f609897b0bb
workflow-type: tm+mt
source-wordcount: '1137'
ht-degree: 0%

---

# Adobe Admin Console에서 사용자 관리

>[!IMPORTANT]
>
>이 문서의 기능은 조직의 Workfront 인스턴스가 Adobe 비즈니스 플랫폼에 온보딩된 경우에만 사용할 수 있습니다.
>
>조직이 Adobe 비즈니스 플랫폼에 온보딩되었는지 여부에 따라 다른 절차 목록은 을 참조하십시오. [플랫폼 기반 관리의 차이점(Adobe Workfront/Adobe 비즈니스 플랫폼)](../../../administration-and-setup/get-started-wf-administration/actions-in-admin-console.md).

Adobe 관리자는 Adobe Admin Console을 사용하여 Adobe Workfront 사용자와 시스템 관리자를 만들 수 있습니다. 콘솔은 조직 전체에서 Adobe 권한을 관리하기 위한 중앙 위치입니다. 자세한 내용은 [Admin Console 개요](https://helpx.adobe.com/enterprise/using/admin-console.html).

## 액세스 요구 사항

이 문서의 단계를 수행하려면 다음 액세스 권한이 있어야 합니다.

<table style="table-layout:auto"> 
 <col> 
 </col> 
 <col> 
 </col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront 플랜</td> 
   <td>모든</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe 관리자 권한</td> 
   <td> <p>조직의 제품 Adobe의 제품 구성 관리자여야 합니다.</p> </td> 
  </tr> 
 </tbody> 
</table>

## 전제 조건

Workfront용 Admin Console을 사용하기 전에 콘솔로 초대하는 이메일 수신 을 받아야 합니다.

1. Adobe을 처음 사용하는 경우 이제 조직의 Adobe 소프트웨어 및 서비스를 관리할 수 있는 권한이 있다는 전자 메일을 받은 경우, 전자 메일의 버튼을 클릭하여 Adobe 계정을 만들고 Admin Console을 엽니다.

   또는

   이미 Adobe 계정이 있는 경우 [Adobe Admin Console 페이지](https://adminconsole.adobe.com/).

## Workfront 프로덕션 인스턴스의 사용자 및 관리 영역에 액세스 {#access-the-user-and-admin-area-for-your-production-instance-of-workfront}

1. 다음에서 [Adobe Admin Console 페이지](https://adminconsole.adobe.com/)를 선택하고 **제품** 맨 위 탐색 막대에서 탭을 선택한 다음 **Workfront** 제품 타일.

   ![](assets/admin-product-1.png)

1. 표시되는 목록에서 맨 위에 있는 링크를 선택합니다.

   사용자가 작업하는 프로덕션 인스턴스입니다.

   ![](assets/instances-1.png)

   >[!TIP]
   >
   >목록의 두 번째 링크인 미리보기 인스턴스는 라이브 프로덕션 환경을 복제하는 테스트 환경입니다. 자세한 내용은 [Adobe Workfront 미리보기 샌드박스 환경](../../../administration-and-setup/set-up-workfront/workfront-testing-environments/wf-preview-sandbox-environment.md).
   >
   >
   >목록에 샌드박스 환경에 대한 링크가 표시될 수도 있습니다. 자세한 내용은 [Adobe Workfront 미리보기 샌드박스 환경](../../../administration-and-setup/set-up-workfront/workfront-testing-environments/wf-preview-sandbox-environment.md).

1. 표시되는 목록에서 **제품 프로필** 선택한 탭에서 Workfront 제품 프로필 링크의 이름을 클릭합니다.

   ![](assets/prod-profile-1.png)

   이 목록에는 Workfront의 프로덕션 인스턴스에 이미 할당된 모든 사용자가 포함됩니다.

   >[!IMPORTANT]
   >
   >제품 프로필 자체를 변경하지 마십시오.

1. 이 문서의 다음 섹션 중 하나를 계속 진행하십시오.

   * [Adobe Admin Console을 사용하여 Workfront에서 사용자 만들기](#create-users-in-workfront-with-the-adobe-admin-console)
   * [Adobe Admin Console을 사용하여 Workfront에서 시스템 관리자 만들기](#create-system-administrators-in-workfront-with-the-adobe-admin-console)

## Adobe Admin Console을 사용하여 Workfront에서 사용자 만들기 {#create-users-in-workfront-with-the-adobe-admin-console}

Workfront 사용자를 Adobe Admin Console에 추가해야 합니다. 관리자는 Adobe Admin Console에서 직접 사용자를 만들 수 있습니다. 그룹 관리자는 Workfront에서 사용자를 만든 다음 승인을 위해 제출합니다. 승인되면 사용자는 Adobe Admin Console에 추가됩니다.

* [Adobe Admin Console에서 바로 Workfront에서 사용자 만들기](#create-users-in-workfront-directly-in-the-adobe-admin-console)
* [Workfront에서 사용자를 만들고 Adobe Admin Console에 대해 승인합니다](#create-users-in-workfront-and-approve-them-for-the-adobe-admin-console)

### Adobe Admin Console에서 바로 Workfront에서 사용자 만들기

1. 에 설명된 대로 Admin Console의 사용자 및 관리 영역으로 이동합니다. [Workfront 프로덕션 인스턴스의 사용자 및 관리 영역에 액세스](#access-the-user-and-admin-area-for-your-production-instance-of-workfront) 이 문서에서.
1. 포함 **사용자** 목록 위에서 선택한 탭을 선택합니다. **사용자 추가**.
1. 다음에서 **이 제품 프로필에 사용자 추가** 상자에서 추가하려는 사용자의 이메일 주소 또는 이름을 입력한 다음 을 선택합니다 **저장**.

   사용자는 Workfront에서 요청자 액세스 수준으로 만들어집니다.

   >[!IMPORTANT]
   >
   >제품 프로필 자체를 변경하지 마십시오.

1. Workfront에서 사용자의 액세스 수준을 변경합니다.

   Workfront 관리자가 사용자의 액세스 수준을 변경할 수 있는 방법에 대한 지침은 [사용자 프로필 편집](../../../administration-and-setup/add-users/create-and-manage-users/edit-a-users-profile.md).

1. 사용자를 추가하려면 3단계와 4단계를 반복하십시오.

   >[!NOTE]
   >
   >신규 Adobe Admin Console의 경우 등록 프로세스를 완료하도록 초대하는 이메일을 제공합니다. 모든 사용자가 모든 Adobe 시스템에 액세스하려면 등록 프로세스를 완료해야 합니다.
   >
   >기존 Adobe 사용자의 경우, 사용자는 사용 가능한 Workfront에 대한 이메일을 받을 수도 있고 받지 못할 수도 있습니다. 제품에 대해 Adobe 관리자가 제어하는 기본 설정입니다.

### Workfront에서 사용자를 만들고 Adobe Admin Console에 대해 승인합니다

이 워크플로우를 통해 Adobe Admin Console에 대한 액세스 권한이 없는 그룹 관리자가 사용자를 만들 수 있습니다.

먼저 그룹 관리자가 Workfront에서 사용자를 작성합니다. 이렇게 하면 사용자가 비활성화됨 및 승인 보류 중 상태로 만들어집니다.

그런 다음 Workfront 관리자가 사용자를 승인합니다. 이렇게 하면 Workfront에서 사용자가 활성화되고 Adobe Admin Console에 추가됩니다.

#### Workfront에서 사용자 만들기(그룹 관리자)

Workfront에서 사용자를 만드는 방법에 대한 지침은 [사용자 추가](/help/quicksilver/administration-and-setup/add-users/create-and-manage-users/add-users.md).

#### 사용자 승인(Workfront 관리자)

사용자를 승인하려면:

1. 다음을 클릭합니다. **메인 메뉴** 아이콘 ![](assets/main-menu-icon.png) Adobe Workfront의 오른쪽 상단에서 을(를) 클릭한 다음 **사용자** ![](assets/users-icon-in-main-menu.png).

1. 사용자를 선택한 다음 기타 아이콘을 클릭합니다 ![](assets/more-icon.png).

1. 사용자를 승인하려면 **승인**&#x200B;을 클릭한 다음 을 클릭합니다 **제출**.

   또는

   사용자를 거부하고 Workfront에서 삭제하려면 **거부**&#x200B;을 클릭한 다음 을 클릭합니다 **제출**.

승인된 사용자는 Adobe Admin Console에 자동으로 추가됩니다.

거부된 사용자는 Workfront에서 자동으로 삭제됩니다.



## Adobe Admin Console을 사용하여 Workfront에서 시스템 관리자 만들기 {#create-system-administrators-in-workfront-with-the-adobe-admin-console}

시스템 관리자 액세스 수준은 Adobe Admin Console에만 부여됩니다. Workfront 내에서는 관리자 액세스 권한을 부여하거나 제거할 수 없습니다.

사용자를 Workfront 시스템 관리자로 지정하려면 먼저 Workfront의 프로덕션 인스턴스에 사용자를 추가해야 합니다. 자세한 내용은 [Adobe Admin Console을 사용하여 Workfront에서 사용자 만들기](#create-users-in-workfront-with-the-adobe-admin-console) 이 문서에서.

1. 에 설명된 대로 Admin Console의 사용자 및 관리 영역으로 이동합니다. [Workfront 프로덕션 인스턴스의 사용자 및 관리 영역에 액세스](#access-the-user-and-admin-area-for-your-production-instance-of-workfront) 이 문서에서.
1. 다음 항목 선택 **관리자** 사용자 목록 위에 있는 탭입니다.
1. 선택 **관리자 추가**.
1. 다음에서 **제품 프로필 관리자 추가** 상자에서 추가하려는 관리자의 이메일 주소 또는 이름을 입력한 다음 을 선택합니다 **저장**.

   ![](assets/add-admin-1.png)

   시스템 관리자는 Workfront에서 생성됩니다.

   >[!IMPORTANT]
   >
   >제품 프로필 자체를 변경하지 마십시오.

## Adobe Admin Console에 대한 추가 세부 정보:

* Workfront 시스템 관리자는 Workfront 내에서 Workfront 사용자를 비활성화할 수 있지만 이렇게 해도 Admin Console의 사용자는 비활성화되지 않습니다.

  <!--
  <p data-mc-conditions="QuicksilverOrClassic.Draft mode">For information about deactivating a user in Workfront, see </p>
  -->

* 사용자 **홈 그룹** 은 폴더를 만든 사용자를 기반으로 결정됩니다. 현재 Admin Console 내에서 사용자 지정할 수 없습니다.
* Workfront 시스템 관리자 액세스 수준은 Adobe Admin Console 내에서만 편집할 수 있습니다.

  <!--
  DRAFTED IN FLARE:
  How is this done?
  
  -->

* 시스템 관리자인 사용자를 다른 액세스 수준으로 편집하려면 먼저 Admin Console을 통해 수행해야 합니다.

  <!--
   This is not clear
  -->

* Workfront의 사용자로부터 시스템 관리자 액세스 권한을 제거하려면 Adobe Admin Console을 사용하여 제품 프로필 관리자로 해당 사용자를 제거해야 합니다. 이렇게 하면 사용자의 Workfront 액세스 수준이 시스템 관리자에서 요청자로 변경됩니다.

  >[!IMPORTANT]
  >
  >제품 프로필 자체를 변경하지 마십시오.

<!--
<div data-mc-conditions="QuicksilverOrClassic.Draft mode">
<p>&nbsp;</p>
<p>&nbsp;</p>
<p>&nbsp;</p>
<p>You can create Adobe Workfront users and system administrators with the <a href="https://adminconsole.adobe.com/" alt="Admin Console link">Adobe Admin Console</a>. The console is a central location for managing the Adobe entitlements across your organization. For more information, see the <a href="https://helpx.adobe.com/enterprise/using/admin-console.html" alt="Admin Console Overview">Admin Console Overview</a>.</p>
<p>Before using the Admin Console for Workfront, you should receive a receive an email inviting you to the console. Click in the invitation to accept it and create an account. You can also use an existing account, if already available.</p>
<h2>Create users</h2>
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">Create users in WF with the Adobe admin console</p>
-->

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">May need to add something about oging throug WF -- check with Jonah</p>

<p>To create users in Workfront with the Admin Console:</p>
<ol>
<li value="1"> <p>From the <a href="https://adminconsole.adobe.com/">Admin Console page</a>, select the <b>Products</b> tab and then select the <b>Workfront</b> product tile.</p> </li>
<li value="2"> <p>Select the link to the Workfront instance you want to change.</p> </li>
<li value="3"> <p>Select the Product profile link. This shows a list of the currently-assigned users. If the list is very long, you can also search for users in the search field above the list.</p> </li>
<li value="4"> <p>Select the <b>Add User</b> button.</p> </li>
<li value="5"> <p>In the <b>Add users</b> box, enter the email address or name of the user you want to add. Select <b>Save</b>. The administrator is created in Workfront with <b>Requestor</b> access level.</p> </li>
</ol>
<h2>Create system administrators</h2>
<p>To create system administrators:</p>
<ol>
<li value="1"> <p>Make product profile assignments first. To be a Workfront System Administrator, the user must be assigned the Workfront product profile and be an admin for that product profile.</p> </li>
<li value="2"> <p>From the console, select the <b>Products</b> tab and then select the <b>Admins</b> tab. </p> </li>
<li value="3"> <p>Select <b>Add Admin</b>.</p> </li>
<li value="4"> <p>In the <b>Add product profile administrators</b> box, enter the email address or name of the administrator you want to add. Select <b>Save</b>. The user is created in Workfront with <b>Requestor</b> access level.</p> </li>
</ol>
<h2>Additional details for the Admin Console</h2>
<ul>
<li> <p>System Administrator access level is granted only on the Admin Console. You cannot grant or remove admin access from within Workfront.</p> </li>
</ul>
<ul>
<li> <p>Creating and deleting users inside Workfront is only possible through the Admin Console.</p> </li>
<li> <p>Workfront System Administrators can deactivate Workfront users from within Workfront, but this does not deactivate the user in the Admin Console.</p> </li>
<li> <p>All new users are are assigned <b>Requestor</b> access level upon creation. Also, the user <b>Home Group</b> is determined based on the user who created them. This is currently not customizable from within the Admin Console.</p> </li>
<li> <p>The Workfront System Administrator access level can only be edited from within the Adobe Admin Console.</p> </li>
<li> <p>Editing a user who is a system admin to any other access level must be done through the Admin Console first.</p> </li>
<li> <p>To remove Workfront system admin access, remove users as Product Profile Administrators. This action changes the user access level in Workfront from a system admin to a <b>Requestor</b>.</p> </li>
</ul>
</div>
-->
