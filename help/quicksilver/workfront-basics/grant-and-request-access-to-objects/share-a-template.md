---
title: 템플릿 공유
product-area: templates
navigation-topic: grant-and-request-access-to-objects
description: Adobe Workfront 관리자는 액세스 수준을 할당할 때 사용자에게 템플릿을 보거나 편집할 수 있는 액세스 권한을 부여할 수 있습니다. 템플릿에 액세스하려면 사용자에게 계획 라이센스가 있어야 합니다.
author: Alina
feature: Get Started with Workfront
exl-id: 19fb0de5-7db5-42a9-9f33-a4570acfeef8
source-git-commit: dd7f61fcd92a43303be356dd3209ec6da6a063dd
workflow-type: tm+mt
source-wordcount: '548'
ht-degree: 2%

---

# 템플릿 공유

Adobe Workfront 관리자는 액세스 수준을 할당할 때 사용자에게 템플릿을 보거나 편집할 수 있는 액세스 권한을 부여할 수 있습니다. 템플릿에 액세스하려면 사용자에게 계획 라이센스가 있어야 합니다.

템플릿에 대한 액세스 권한 부여에 대한 자세한 내용은 [템플릿에 대한 액세스 권한 부여](../../administration-and-setup/add-users/configure-and-grant-access/grant-access-templates.md).

부여하는 액세스 수준과 함께 사용자는 특정 템플릿을 공유하는 다른 사용자로부터 보기 또는 관리 권한을 받을 수도 있습니다 .

>[!NOTE]
>
>권한 수준은 액세스 수준 내에서 작동합니다. 예를 들어, 사용자는 액세스 수준으로만 템플릿을 볼 수 있는 경우 템플릿 관리 권한을 받을 수 없습니다.

권한은 Workfront의 한 항목에 한정되며, 해당 항목에 대해 수행할 수 있는 작업을 정의합니다.

## 템플릿 공유 시 고려 사항

* 아래 고려 사항 외에 다음을 참조하십시오 [개체에 대한 권한 공유 개요](../../workfront-basics/grant-and-request-access-to-objects/sharing-permissions-on-objects-overview.md).
* 템플릿 작성자와 템플릿 소유자는 기본적으로 템플릿에 대한 관리 권한이 있습니다. 사용자를 템플릿 소유자로 지정하는 방법에 대한 자세한 내용은 [프로젝트 템플릿 편집](../../manage-work/projects/create-and-manage-templates/edit-templates.md).
* 템플릿을 공유할 때 다음 항목을 공유할 수 있습니다.

   * 템플릿

      템플릿을 공유하는 방법에 대한 자세한 내용은 [프로젝트 템플릿 공유](../../manage-work/projects/create-and-manage-templates/share-project-template.md).

      템플릿에 다음 권한을 부여할 수 있습니다.

      * 보기

         ![](assets/view-on-template-262x221.png)

      * 관리

         ![](assets/manage-on-template-225x280.png)
   * 템플릿을 사용하여 만들어지는 향후 프로젝트입니다. 개별 프로젝트처럼 템플릿에서 만든 프로젝트에 동일한 수준의 권한을 부여할 수 있습니다. 

      템플릿 수준에서 템플릿에서 프로젝트를 공유하는 방법에 대한 자세한 내용은 [프로젝트 템플릿 공유](../../manage-work/projects/create-and-manage-templates/share-project-template.md).


* 템플릿에서 만든 템플릿 또는 프로젝트를 공유하면 사용자는 기본적으로 템플릿 또는 프로젝트와 연결된 모든 하위 객체에 동일한 권한을 상속받습니다.

   Workfront에서 개체의 계층 구조에 대한 자세한 내용은  [Adobe Workfront의 개체 이해](../../workfront-basics/navigate-workfront/workfront-navigation/understand-objects.md).

* 템플릿을 공유하면 템플릿에서 만든 이후 프로젝트의 문제뿐만 아니라 모든 템플릿 작업 및 문서가 별도로 지정되지 않는 한 동일한 권한을 상속합니다.

   프로젝트에 대한 사용자의 권한에 따라 프로젝트의 템플릿 작업 및 문제에 대한 액세스 관리를 위한 자세한 내용은 [액세스](../../manage-work/projects/create-and-manage-templates/edit-templates.md#access) 문서의 섹션 [프로젝트 템플릿 편집](../../manage-work/projects/create-and-manage-templates/edit-templates.md).

* Workfront 관리자는 문서가 사용자의 액세스 수준에서 상위 개체에서 권한을 상속해야 하는지 여부를 지정할 수 있습니다. 문서에 대한 상속된 권한 제한에 대한 자세한 내용은 [사용자 정의 액세스 수준 만들기 또는 수정](../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md).

<!--
<div data-mc-conditions="QuicksilverOrClassic.Draft mode">
<h2>Share a template</h2>
<p>(NOTE: drafted because this is also linked above: Share project templates >> which is an article in the Manage Work section>> Templates)&nbsp;</p>
<ol>
<li value="1"> <p>Go to the template you want to share with other entities, click <strong>Template Actions</strong>, then <strong>Template Sharing</strong>.<br>Or</p> <p>Navigate to a list of templates, and select multiple templates from the list, then click <strong>Share Template</strong>.</p> <note type="note">
If you select multiple templates, you cannot view who already has permissions to the individual templates.
</note> </li>
<li value="2"> <p>Start typing the name of a user, group, team, job role, or company that you want to share the template with in the <strong>Give template access to</strong> or <strong>Edit template access for</strong> fields.</p> <p>Select them when they appear in the list.</p> <note type="tip">
You can share an object only with active users, teams,
<span>roles,</span> or companies.
</note> </li>
<li value="3">From the drop-down menu, select which level of permissions you want to grant:<br>
<ul>
<li><p><strong>View it</strong>: Users with these permissions are able to view the template and create a project using it, or attach it to an existing project.</p><p><img src="assets/template-permissions-350x197.png" alt="template_permissions.png" style="width: 350;height: 197;"></p></li>
<li><strong>Manage it</strong>: Users with these permissions are able to edit or delete the template.</li>
</ul></li>
<li value="4">(Optional) Click <strong>Advanced Settings</strong> to fine-tune your settings for each level of permissions.</li>
<li value="5">Click <strong>Save</strong>.</li>
</ol>
<h2>Share a project at the template level</h2>
<p>You can share the future projects that are created using a template with users at the template level.</p>
<ol>
<li value="1"> <p>Go to the template whose future projects you want to share with other entities, click <strong>Template Actions</strong>, then <strong>Project Sharing</strong>.</p> <p>Or</p> <p>Navigate to a list of templates, and select multiple templates from the list, then click <strong>Share Project</strong>.</p> <note type="note">
If you select multiple templates, you cannot view who already has project permissions to the individual templates.
</note> </li>
<li value="2"> <p>Start typing and then select the name of a user, group, team, job role, or company with whom you want to share future projects created from the template in the <strong>Give project access to</strong> or <strong>Edit template access for</strong> fields.</p> <note type="tip">
You can share an object only with active users, teams,
<span>roles,</span> or companies.
</note> </li>
<li value="3">From the drop-down menu, select which level of permissions you want to grant.<br>Select from the following:<br>
<ul>
<li><strong>No access</strong>: You can specify which users will not have any access to the template.<br>This option is available only when bulk sharing projects from templates.&nbsp;</li>
<li><strong>View</strong>: Users with these permissions can view projects created from the template.</li>
<li><strong>Contribute</strong>: Users with these permissions can contribute to projects created from the template&nbsp;</li>
<li><strong>Manage</strong>: Users with these permissions can manage or delete projects created from this template.<br><img src="assets/share-project-from-template-350x268.png" alt="share_project_from_template.png" style="width: 350;height: 268;"></li>
</ul></li>
<li value="4">(Optional) Click <strong>Advanced Settings</strong> to fine-tune your settings for each level of permissions. </li>
<li value="5">Click <strong>Save</strong>.</li>
</ol>
</div>
-->

## 템플릿 공유에 대한 고급 설정

다음 표에는 사용자에게 템플릿을 보거나 관리할 수 있도록 허용할 수 있는 권한이 표시됩니다. 템플릿 공유에 대한 지침은 섹션을 참조하십시오 [템플릿 공유](../../manage-work/projects/create-and-manage-templates/share-project-template.md#share) 기사 [프로젝트 템플릿 공유](../../manage-work/projects/create-and-manage-templates/share-project-template.md).

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th>액션</th> 
   <th>관리</th> 
   <th>보기</th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td>복사</td> 
   <td>✓</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>삭제</td> 
   <td>✓</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>템플릿 세부 정보 편집</td> 
   <td>✓</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>템플릿 보기</td> 
   <td>✓</td> 
   <td>✓</td> 
  </tr> 
  <tr> 
   <td>공유</td> 
   <td>✓</td> 
   <td>✓</td> 
  </tr> 
  <tr> 
   <td>시스템 전체 공유</td> 
   <td> </td> 
   <td>✓</td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> <p>문서 추가</p> <p>팁: 프로젝트에 문서를 추가한다고 생각하면서 프로젝트 템플릿에 문서를 추가하는 경우가 있습니다. 이 설정을 비활성화하여 수신자에게 이를 방지할 수 있습니다.</p> </td> 
   <td> </td> 
   <td>✓</td> 
  </tr> 
 </tbody> 
</table>

템플릿에서 만든 프로젝트에 사용자에게 부여하는 권한을 이해하려면 를 참조하십시오 [Adobe Workfront에서 프로젝트 공유](../../workfront-basics/grant-and-request-access-to-objects/share-a-project.md).
