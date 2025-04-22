---
title: 프로젝트 공유
product-area: projects
navigation-topic: grant-and-request-access-to-objects
description: Adobe Workfront 관리자는 액세스 수준을 할당할 때 프로젝트를 보거나 편집할 수 있는 액세스 권한을 부여할 수 있습니다. 자세한 내용은 프로젝트에 대한 액세스 권한 부여를 참조하십시오.
author: Courtney
feature: Get Started with Workfront
exl-id: eaeedff8-9114-40d9-8cd4-56996edc7dad
source-git-commit: eb4bf18407562b88bf0c946c905b202e5b62a5fe
workflow-type: tm+mt
source-wordcount: '1579'
ht-degree: 2%

---

# 프로젝트 공유

<!-- Audited: 1/2024 -->

Adobe Workfront 관리자는 액세스 수준을 할당할 때 프로젝트를 보거나 편집할 수 있는 액세스 권한을 부여할 수 있습니다. 자세한 내용은 [프로젝트에 대한 액세스 권한 부여](../../administration-and-setup/add-users/configure-and-grant-access/grant-access-projects.md)를 참조하십시오.

사용자에게 부여된 액세스 수준과 함께 공유할 액세스 권한이 있는 특정 프로젝트를 보거나, 기여하거나, 관리할 수 있는 권한을 부여할 수도 있습니다.

권한은 Workfront의 한 항목에 한정되며, 해당 항목에 대해 수행할 수 있는 작업을 정의합니다.


## 액세스 요구 사항

+++ 을 확장하여 이 문서의 기능에 대한 액세스 요구 사항을 봅니다.

객체를 공유하려면 다음 항목이 있어야 합니다.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront 플랜</td> 
   <td> <p>임의 </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront 라이선스</td> 
   <td> <p>새로운 기능: 표준</p> 
   또는
   <p>현재: 작업 시간 이상</p>
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader">액세스 수준 구성</td> 
   <td> <p>공유할 개체에 대한 액세스 이상의 보기</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">개체 권한</td> 
   <td> <p>공유할 개체에 대한 권한 이상 보기</p></td> 
  </tr> 
 </tbody> 
</table>

자세한 내용은 [Workfront 설명서의 액세스 요구 사항](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)을 참조하십시오.

+++

## 프로젝트 공유에 대한 고려 사항

아래 고려 사항 외에 [개체에 대한 공유 권한 개요](../../workfront-basics/grant-and-request-access-to-objects/sharing-permissions-on-objects-overview.md)를 참조하십시오.

* 기본적으로 프로젝트 작성자는 프로젝트를 관리할 수 있는 권한이 있으며 프로젝트 소유자로도 지정됩니다. 프로젝트가 다른 소유자에게 할당된 경우 해당 사용자도 프로젝트를 관리할 수 있는 권한이 있습니다. 프로젝트 작성자(또는 소유자)가 프로젝트를 다른 사용자와 공유할 때 사용자는 프로젝트에서 작업하면서 수행할 수 있는 작업을 제어할 수 있는 특정 권한을 해당 사용자에게 부여합니다.

  단, 프로젝트 소유자에게 플랜 또는 표준 라이센스가 없는 경우 프로젝트를 관리할 수 있는 전체 액세스 권한이 없습니다. 플랜 또는 Standard 라이선스가 있는 사용자만 프로젝트를 관리할 수 있는 권한을 가질 수 있습니다. 자세한 내용은 [액세스 수준과 사용 권한이 함께 작동하는 방법](../../administration-and-setup/add-users/access-levels-and-object-permissions/how-access-levels-permissions-work-together.md)을 참조하세요.

* 프로젝트를 개별적으로 공유하거나 여러 개의 프로젝트를 한 번에 공유할 수 있습니다. 프로젝트 공유는 다른 오브젝트 공유와 동일합니다. Workfront에서 항목을 공유하는 방법에 대한 자세한 내용은 [개체 공유](../../workfront-basics/grant-and-request-access-to-objects/share-an-object.md)를 참조하십시오.
* 프로젝트에 다음 권한을 부여할 수 있습니다.

   * 보기
   * 관리
   * 참여

* 프로젝트를 공유할 때는 별도로 지정하지 않는 한 모든 작업, 문제 및 문서가 동일한 권한을 상속합니다.

  프로젝트에 대한 사용자의 권한을 기반으로 프로젝트의 작업 및 문제에 대한 액세스 관리에 대한 자세한 내용은 [프로젝트 편집](../../manage-work/projects/manage-projects/edit-projects.md) 문서의 [](../../manage-work/projects/manage-projects/edit-projects.md#access) 섹션을 참조하십시오.

  Workfront 관리자는 문서가 사용자 액세스 수준의 상위 개체에서 권한을 상속해야 하는지 여부를 지정할 수 있습니다. 문서에 대해 상속된 사용 권한을 제한하는 방법에 대한 자세한 내용은 [사용자 지정 액세스 수준 만들기 또는 수정](../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md)을 참조하십시오.

* 하위 개체가 상속되지 않도록 프로젝트에서 상속된 권한을 제거할 수 있습니다. 개체에서 상속된 사용 권한을 제거하는 방법에 대한 자세한 내용은 [개체에서 사용 권한 제거](../../workfront-basics/grant-and-request-access-to-objects/remove-permissions-from-objects.md)를 참조하십시오.

## 다양한 라이선스 유형에 대한 제한 사항

* 작업자 라이선스가 있는 사용자는 프로젝트를 관리할 수 있는 권한이 없습니다. 작업자의 경우 가장 높은 공유 권한은 Contribute입니다.
* 요청 라이선스가 있는 사용자는 프로젝트 정보를 볼 수 있지만 프로젝트 액세스 권한은 제한됩니다.
* 보기 또는 기여 권한이 있는 사용자도 승인 프로세스에 포함된 경우 프로젝트 상태 변경의 예외가 발생합니다. 프로젝트를 승인하여 프로젝트의 상태를 변경할 수 있지만 상태는 승인 또는 거절에 대해 사전 정의된 상태입니다.
* 프로젝트를 복사할 수 있으려면 사용자는 액세스 수준에서도 프로젝트를 만들 수 있는 액세스 권한이 있어야 합니다.

## 프로젝트를 공유하는 방법 {#ways-to-share-a-project}

다음과 같은 방법으로 프로젝트를 공유할 수 있습니다.

* 다음 중 하나를 수행하여 수동으로 수행합니다.

   * 프로젝트 팀에 사용자 추가 프로젝트 팀에 사용자를 추가하면 해당 사용자는 프로젝트에 대한 보기 권한을 자동으로 부여받습니다.\
     프로젝트 팀에 사용자를 추가하는 방법에 대한 자세한 내용은 [프로젝트 팀 개요](../../manage-work/projects/planning-a-project/project-team-overview.md)에서 프로젝트 팀에 사용자 추가 섹션을 참조하십시오.
   * **공유** 옵션을 사용할 때 프로젝트를 개별적으로 또는 대량으로 공유합니다.

* 다음 중 하나를 수행하여 자동으로

   * 이미 다른 사용자와 공유된 **Portfolio** 또는 **프로그램**&#x200B;에 프로젝트를 배치하십시오. 사용자는 포트폴리오 또는 프로그램에 대해 가지고 있는 것과 동일한 권한을 프로젝트에 부여받습니다.\
     **Portfolio**&#x200B;에 프로젝트를 추가하는 방법에 대한 자세한 내용은 [포트폴리오에 프로젝트 추가](../../manage-work/portfolios/create-and-manage-portfolios/add-projects-to-portfolios.md)를 참조하십시오.\
     **Program**&#x200B;에 프로젝트를 추가하는 방법에 대한 자세한 내용은 [프로그램에 프로젝트 추가](../../manage-work/portfolios/create-and-manage-programs/add-project-to-program.md)를 참조하십시오.
개체에 상속된 사용 권한을 보는 방법에 대한 자세한 내용은 [개체에 상속된 사용 권한 보기](../../workfront-basics/grant-and-request-access-to-objects/view-inherited-permissions-on-objects.md)를 참조하십시오.

   * 프로젝트를 만드는 데 사용된 템플릿의 프로젝트 공유에 엔티티를 추가합니다. 템플릿에서 프로젝트를 공유하는 방법에 대한 자세한 내용은 [템플릿 공유](../../workfront-basics/grant-and-request-access-to-objects/share-a-template.md)를 참조하십시오.
   * 프로젝트 액세스 템플릿을 정의합니다.

     >[!TIP]
     >
     >템플릿을 첨부하거나 저장할 때 템플릿 프로젝트 공유 규칙을 지울 수 있습니다.

   * 프로젝트를 편집하고 **누군가 이 프로젝트에 대한 액세스 권한을 받았을 때** 설정을 정의합니다. 자세한 내용은 [프로젝트 편집](../../manage-work/projects/manage-projects/edit-projects.md)을 참조하세요.

<!--
<div data-mc-conditions="QuicksilverOrClassic.Draft mode">
<p>(NOTE: drafted because I created new article and linked it above) </p>
<p>To view what users have inherited the access on the project from a portfolio or a program, do the following:</p>
<ol style="list-style-type: lower-alpha;">
<li value="1">Go to a project whose sharing permissions you want to view. </li>
<li value="2"> Click the <strong>More</strong> menu <img src="assets/more-icon.png">, then click <strong>Sharing</strong>. </li>
<li value="3"> <p>Expand the <strong>Inherited Permissions</strong> list. </p> <p>This list displays the names of users that have access to either the portfolio or the program that the project belongs to and also have permissions to the project. </p>  </li>
</ol>
</div>
-->

<!--
<ol data-mc-conditions="QuicksilverOrClassic.Draft mode">
<li value="1">Go to a project whose sharing permissions you want for all projects you create from scratch. (NOTE: drafted because linked above)&nbsp;</li>
<li value="2"> Click the More menu, then click <strong>Sharing</strong>. </li>
<li value="3"> <p>In the Project Access box that displays, near the upper-right corner, click the gear icon <img src="assets/gear-icon-settings.png">, then click <strong>Set as my project access template</strong>.</p> <p>The entities that are granted permissions on the selected project have the same permissions for all the projects you create from scratch in the future.</p> <p> The project access template overrides the sharing defaults granted to you by the Workfront administrator in your Access Level.<br>For more information about specifying sharing defaults for projects in the Access Level, see <a href="../../administration-and-setup/add-users/configure-and-grant-access/grant-access-projects.md" class="MCXref xref">Grant access to projects</a>.</p> </li>
<li value="4">Click <strong>Save</strong>.</li>
</ol>
-->

## 프로젝트 공유

{{step1-to-projects}}

1. **프로젝트** 페이지의 목록에서 공유할 프로젝트를 선택하십시오. 프로젝트 페이지가 열립니다.

1. 프로젝트 이름 오른쪽에서 **공유**&#x200B;를 클릭합니다. **[프로젝트 이름 공유]** 대화 상자가 열립니다.

   ![프로젝트 공유 단추](assets/share-project.png)

1. **프로젝트 액세스 권한 부여** 필드에서 프로젝트를 공유할 사용자, 팀, 역할, 그룹 또는 회사의 이름을 입력한 다음 드롭다운 목록에 표시될 때 이름을 클릭합니다.

   >[!TIP]
   >
   >활성 사용자, 팀, 역할 또는 회사와만 프로젝트를 공유할 수 있습니다.


1. (선택 사항) **액세스 권한이 있는 사용자** 드롭다운을 선택하고 프로젝트의 액세스 수준을 선택합니다.

   * **초대된 사용자만 액세스할 수 있습니다.** 프로젝트에 초대된 사용자만 액세스할 수 있습니다(기본값).
   * **시스템의 모든 사용자가 볼 수 있습니다**: 시스템의 모든 사용자는 초대장 없이 프로젝트를 볼 수 있습니다.

1. (선택 사항) 선택한 프로젝트 액세스 설정을 모든 새 프로젝트에 자동으로 적용하려면 **톱니바퀴** 아이콘을 클릭합니다![톱니바퀴 아이콘을 선택합니다](assets/gear-icon.png). 그런 다음 **내 프로젝트 액세스 템플릿으로 설정**(으)로 인라인으로 확인란을 선택합니다.

   >[!NOTE]
   >
   >프로젝트 액세스 템플릿은 액세스 수준의 Workfront 관리자가 부여한 공유 기본값을 무시합니다.\
   >액세스 수준의 프로젝트에 대한 공유 기본값을 지정하는 방법에 대한 자세한 내용은 [프로젝트에 대한 액세스 권한 부여](../../administration-and-setup/add-users/configure-and-grant-access/grant-access-projects.md)를 참조하십시오.

   <!--
   >this note also appears in Understanding Project Permissions-->


1. 사용자 이름 오른쪽에 있는 드롭다운을 클릭하고 이 프로젝트에 대한 권한 수준을 선택합니다.


   * **보기**: 사용자가 프로젝트를 검토하고 공유할 수 있습니다.
   * **참여**: 사용자는 업데이트를 수행하고, 정보를 기록하며, 간단한 편집을 수행하고, 프로젝트를 공유할 수 있습니다(모든 보기 권한도 포함).
   * **관리**: 사용자가 액세스 수준에서 부여된 관리 권한 없이 프로젝트에 대한 전체 액세스 권한을 가지고 있습니다(모든 보기 및 기여 권한도 포함).

1. (선택 사항) 프로젝트에서 특정 권한을 구성하기 위해 부여한 권한 수준 옆에 있는 고급 옵션 아이콘을 클릭합니다.

   ![구성된 고급 권한 옵션](assets/advanced-permission-options.png)

1. (선택 사항) 링크를 사용하여 프로젝트를 빠르게 공유하려면 **링크 복사**&#x200B;를 클릭한 다음 받는 사람에게 전달하십시오.

1. **저장**&#x200B;을 클릭합니다.

## 프로젝트 일괄 공유

{{step1-to-projects}}

1. **프로젝트** 페이지에서 공유할 각 프로젝트의 왼쪽에 있는 상자를 선택한 다음 페이지 상단의 **공유** 아이콘 ![공유 아이콘](assets/share-icon.png)을 클릭합니다. 공유 모달이 열립니다.

   ![프로젝트 일괄 공유](assets/bulk-share-icon.png)

1. **프로젝트 액세스 권한 부여** 필드에서 프로젝트를 공유할 사용자, 팀, 역할, 그룹 또는 회사의 이름을 입력한 다음 드롭다운 목록에 표시될 때 이름을 클릭합니다.

   >[!TIP]
   >
   >활성 사용자, 팀, 역할 또는 회사와만 프로젝트를 공유할 수 있습니다.


1. (선택 사항) **액세스 권한이 있는 사용자** 드롭다운을 선택하고 프로젝트의 액세스 수준을 선택합니다.

   * **초대된 사용자만 액세스할 수 있습니다.** 프로젝트에 초대된 사용자만 액세스할 수 있습니다(기본값).
   * **시스템의 모든 사용자가 볼 수 있습니다**: 시스템의 모든 사용자는 초대장 없이 프로젝트를 볼 수 있습니다.


1. 사용자 이름 오른쪽에 있는 드롭다운을 클릭하고 프로젝트에 대한 권한 수준을 선택합니다.

   * **보기**: 사용자가 프로젝트를 검토하고 공유할 수 있습니다.
   * **참여**: 사용자는 업데이트를 수행하고, 정보를 기록하며, 간단한 편집을 수행하고, 프로젝트를 공유할 수 있습니다(모든 보기 권한도 포함).
   * **관리**: 사용자가 액세스 수준에서 부여된 관리 권한 없이 프로젝트에 대한 전체 액세스 권한을 가지고 있습니다(모든 보기 및 기여 권한도 포함).

1. (선택 사항) 프로젝트에서 특정 권한을 구성하기 위해 부여한 권한 수준 옆에 있는 고급 옵션 아이콘을 클릭합니다.

   ![구성된 고급 권한 옵션](assets/advanced-permission-options.png)

1. **저장**&#x200B;을 클릭합니다.


<!--
<div data-mc-conditions="QuicksilverOrClassic.Draft mode">
<h2>Configure default permissions for a project</h2>
<p>(NOTE: drafted because I added one more way to automatically share the project above in the bullet list and linked it to Edit Projects) </p>
<p>As a project owner, you can configure the default permissions for View, Manage, and Contribute access that are used when sharing&nbsp;the project with others. When users share a project, the default permissions are used. Users can then adjust the default permissions when sharing the project, as described in <a title="Project Permissions" href="#ways-to-share-a-project" class="MCXref xref">Ways to share a project</a>. </p>
<p>To configure the default permissions that are included with each access level:</p>
<ol>
<li value="1">Go to the project where you want to set the default permissions.</li>
<li value="2"> <p>Click the More menu <img src="assets/more-icon.png">, then click <strong>Edit</strong>. <img src="assets/edit-icon.png"></p> <p data-mc-conditions="QuicksilverOrClassic.Quicksilver"> </p> </li>
<li value="3">Click <strong>Access</strong> in the list on the left.</li>
<li value="4"> <p>In the <strong>When someone is given access to this PROJECT</strong> section, select permissions that you want to be available when users are given access to the project via sharing.</p> <p>Ensure that any permissions that you want to include in the selected access level are selected and deselect any permissions that you do not want to include in the selected permissions level.</p> <p>To view which permissions are available for each level, see&nbsp;<a title="Project Permissions" href="#Understanding_Project_Permissions" class="MCXref xref">Share a project in Adobe Workfront</a>.</p> <note type="note">
The
<strong>Delete</strong> access in the
<strong>Manage</strong> permission level determines whether users can&nbsp;delete the project itself. Users with
<strong>Manage</strong> access to the project can delete tasks and issues within the project regardless of whether this option is selected, if they have
<strong>Manage</strong> permissions to the tasks and issues.&nbsp;
</note> </li>
<li value="5">Click <strong>Save Changes</strong>.</li>
</ol>
</div>
-->

## 프로젝트 권한 옵션

다음 표에는 사용자가 프로젝트를 공유할 때 부여할 수 있는 권한이 나열되어 있습니다. 사용자가 라이선스에 따라 얻을 수 있는 액세스 권한에 대한 자세한 내용은 [프로젝트에 액세스 권한 부여](../../administration-and-setup/add-users/configure-and-grant-access/grant-access-projects.md)를 참조하십시오.

<table border="1" cellspacing="15" cellpadding="1"> 
 <col> 
 <col> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th> <p><strong>작업</strong> </p> </th> 
   <th> <p><strong>관리</strong> </p> </th> 
   <th> <p><strong>참여</strong> </p> </th> 
   <th> <p><strong>보기</strong> </p> </th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td> <p>사용자 정의 양식 추가</p> </td> 
   <td> <p>✓</p> </td> 
   <td> <p> </p> </td> 
   <td> <p> </p> </td> 
  </tr> 
  <tr> 
   <td> <p>사용자 정의 필드 업데이트</p> </td> 
   <td> <p>✓</p> </td> 
   <td> <p>✓</p> </td> 
   <td> <p> </p> </td> 
  </tr> 
  <tr> 
   <td> <p>승인 프로세스 추가</p> </td> 
   <td> <p>✓</p> </td> 
   <td> <p> </p> </td> 
   <td> <p> </p> </td> 
  </tr> 
  <tr> 
   <td> <p>프로젝트 승인</p> </td> 
   <td> <p>✓</p> </td> 
   <td> <p>✓</p> </td> 
   <td> <p>✓</p> </td> 
  </tr> 
  <tr> 
   <td> <p>시간 승인</p> </td> 
   <td> <p>✓</p> </td> 
   <td> <p>✓ </p> </td> 
   <td> <p> </p> </td> 
  </tr> 
  <tr> 
   <td> <p>프로젝트 만들기</p> </td> 
   <td> <p>✓</p> </td> 
   <td> <p> </p> </td> 
   <td> <p> </p> </td> 
  </tr> 
  <tr> 
   <td> <p>문서 추가</p> </td> 
   <td> <p>✓</p> </td> 
   <td> <p>✓</p> </td> 
   <td> <p>✓</p> </td> 
  </tr> 
  <tr> 
   <td> <p>문제 추가</p> </td> 
   <td> <p>✓</p> </td> 
   <td> <p>✓</p> </td> 
   <td> <p>✓</p> </td> 
  </tr> 
  <tr> 
   <td> <p>작업 추가</p> </td> 
   <td> <p>✓</p> </td> 
   <td> <p>✓</p> </td> 
   <td> <p> </p> </td> 
  </tr> 
  <tr> 
   <td> <p>프로젝트 복사</p> </td> 
   <td> <p> </p> </td> 
   <td> <p>✓</p> </td> 
   <td> <p> </p> </td> 
  </tr> 
  <tr> 
   <td> <p>프로젝트 삭제</p> </td> 
   <td> <p>✓</p> </td> 
   <td> <p> </p> </td> 
   <td> <p> </p> </td> 
  </tr> 
  <tr> 
   <td> <p>계획된 일자 수정</p> </td> 
   <td> <p>✓</p> </td> 
   <td> <p> </p> </td> 
   <td> <p> </p> </td> 
  </tr> 
  <tr> 
   <td> <p>프로젝트 공유</p> </td> 
   <td> <p>✓</p> </td> 
   <td> <p>✓</p> </td> 
   <td> <p>✓</p> </td> 
  </tr> 
  <tr> 
   <td> <p>시스템 전체 공유</p> </td> 
   <td> <p> </p> </td> 
   <td> <p> </p> </td> 
   <td> <p>✓</p> </td> 
  </tr> 
  <tr> 
   <td> <p>프로젝트 보기</p> </td> 
   <td> <p>✓</p> </td> 
   <td> <p>✓</p> </td> 
   <td> <p>✓</p> </td> 
  </tr> 
  <tr> 
   <td> <p>업데이트/주석</p> </td> 
   <td> <p>✓</p> </td> 
   <td> <p>✓</p> </td> 
   <td> <p>✓</p> </td> 
  </tr> 
  <tr> 
   <td> <p>상태 변경</p> </td> 
   <td> <p>✓</p> </td> 
   <td> <p> </p> </td> 
   <td> <p> </p> </td> 
  </tr> 
  <tr> 
   <td> <p>시간 기록</p> </td> 
   <td> <p>✓</p> </td> 
   <td> <p>✓</p> </td> 
   <td> <p> </p> </td> 
  </tr> 
  <tr> 
   <td> <p>할당 편집</p> </td> 
   <td> <p>✓</p> </td> 
   <td> <p>✓</p> </td> 
   <td> <p> </p> </td> 
  </tr> 
  <tr> 
   <td> <p>기준선 관리</p> </td> 
   <td> <p>✓</p> </td> 
   <td> <p> </p> </td> 
   <td> <p> </p> </td> 
  </tr> 
  <tr> 
   <td> <p>위험 관리*</p> </td> 
   <td> <p>✓</p> </td> 
   <td> <p> </p> </td> 
   <td> <p> </p> </td> 
  </tr> 
  <tr> 
   <td> <p>재무 관리*</p> </td> 
   <td> <p>✓</p> </td> 
   <td> <p> </p> </td> 
   <td> <p> </p> </td> 
  </tr> 
  <tr> 
   <td> <p>경비 추가/편집*</p> </td> 
   <td> <p>✓</p> </td> 
   <td> <p>✓</p> </td> 
   <td> <p> </p> </td> 
  </tr> 
  <tr> 
   <td> <p>재무 보기*</p> </td> 
   <td> <p>✓</p> </td> 
   <td> <p>✓</p> </td> 
   <td> <p>✓</p> </td> 
  </tr> 
  <tr> 
   <td> <p>템플릿 첨부</p> </td> 
   <td> <p>✓</p> </td> 
   <td> <p> </p> </td> 
   <td> <p> </p> </td> 
  </tr> 
  <tr> 
   <td> <p>템플릿으로 저장</p> </td> 
   <td> <p>✓</p> </td> 
   <td> <p>✓</p> </td> 
   <td> <p>✓</p> </td> 
  </tr> 
  <tr> 
   <td> <p>비즈니스 사례 추가/편집</p> </td> 
   <td> <p>✓</p> </td> 
   <td> <p> </p> </td> 
   <td> <p> </p> </td> 
  </tr> 
  <tr> 
   <td> <p>프로젝트 세부 정보 편집</p> </td> 
   <td> <p>✓</p> </td> 
   <td> <p> </p> </td> 
   <td> <p> </p> </td> 
  </tr> 
  <tr> 
   <td> <p>직원 편집</p> </td> 
   <td> <p>✓</p> </td> 
   <td> <p> </p> </td> 
   <td> <p> </p> </td> 
  </tr> 
  <tr> 
   <td> <p>MS 프로젝트로 내보내기</p> </td> 
   <td> <p>✓</p> </td> 
   <td> <p>✓</p> </td> 
   <td> <p>✓</p> </td> 
  </tr> 
  <tr> 
   <td> <p>재무/타임라인 다시 계산*</p> </td> 
   <td> <p>✓</p> </td> 
   <td> <p> </p> </td> 
   <td> <p> </p> </td> 
  </tr> 
  <tr> 
   <td> <p>대기열 속성 설정</p> </td> 
   <td> <p>✓</p> </td> 
   <td> <p> </p> </td> 
   <td> <p>  </p> </td> 
  </tr> 
  <tr> 
   <td> <p>목록에서 프로젝트를 일괄적으로 편집</p> </td> 
   <td> <p>✓</p> </td> 
   <td> </td> 
   <td> </td> 
  </tr> 
 </tbody> 
</table>

&#42;재무 데이터에 대한 액세스 권한이 없는 사용자는 프로젝트에 대한 편집 액세스 권한이 있어도 프로젝트의 위험 및 재무 정보를 관리할 수 없습니다. 재무 데이터에 대한 액세스 정보는 [재무 데이터에 대한 액세스 권한 부여](../../administration-and-setup/add-users/configure-and-grant-access/grant-access-financial.md)를 참조하십시오.
