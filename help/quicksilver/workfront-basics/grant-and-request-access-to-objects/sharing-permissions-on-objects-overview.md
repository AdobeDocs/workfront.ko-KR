---
content-type: overview
navigation-topic: grant-and-request-access-to-objects
title: 개체에 대한 권한 공유 개요
description: 만든 객체 또는 사용자와 공유된 객체에 대한 권한을 공유하거나 제거할 수 있습니다.
author: Alina
feature: Get Started with Workfront
exl-id: 7c14702e-ac55-4266-88a7-f31618f84218
source-git-commit: 4644edd2aac8c77508e940ec42c597aa702c4df1
workflow-type: tm+mt
source-wordcount: '1156'
ht-degree: 1%

---

# 개체에 대한 권한 공유 개요

<!--
<p style="color: #ff1493;" data-mc-conditions="QuicksilverOrClassic.Draft mode">Redundancy here with the article Permissions for shared objects?</p>
-->

액세스 권한이 있는 개체에 대한 권한을 공유하기 위해 Adobe Workfront 관리자가 될 필요는 없지만, 객체에 대한 권한은 Workfront 관리자가 설정한 액세스 수준 내에서 작동합니다.

만든 객체 또는 사용자와 공유된 객체에 대한 권한을 공유하거나 제거할 수 있습니다. 객체 작성자가 아닌 경우 객체에 대한 공유 권한 외에 액세스 수준에서 공유할 객체에 대한 공유 액세스 권한이 있어야 합니다. 액세스 수준에 대한 자세한 내용은 [새 액세스 수준 개요](/help/quicksilver/administration-and-setup/add-users/how-access-levels-work/access-level-overview.md) 또는 [액세스 수준 개요](../../administration-and-setup/add-users/access-levels-and-object-permissions/access-levels-overview.md).

>[!NOTE]
>
>Workfront 관리자는 해당 항목의 소유자가 아니더라도 모든 사용자에 대해 시스템의 모든 항목에 대한 권한을 추가하거나 제거할 수 있습니다.

## Workfront에서 공유할 수 있는 개체

Workfront에서 다른 사용자와 다음 개체를 공유할 수 있습니다.

* **프로젝트**: 자세한 내용은 [Adobe Workfront에서 프로젝트 공유](../../workfront-basics/grant-and-request-access-to-objects/share-a-project.md).

* **템플릿**: 자세한 내용은 [프로젝트 템플릿 공유](../../manage-work/projects/create-and-manage-templates/share-project-template.md).

* **Portfolio**: 자세한 내용은 [포트폴리오 공유](../../workfront-basics/grant-and-request-access-to-objects/share-a-portfolio..md).

* **프로그램**: 자세한 내용은 [프로그램 공유](../../workfront-basics/grant-and-request-access-to-objects/share-a-program.md) .

* **작업**: 자세한 내용은 [작업 공유](../../workfront-basics/grant-and-request-access-to-objects/share-a-task.md).

* **문제**: 자세한 내용은 [문제 공유](../../workfront-basics/grant-and-request-access-to-objects/share-an-issue.md).

* **문서**: 자세한 내용은 [문서 공유](../../workfront-basics/grant-and-request-access-to-objects/document-permissions.md).

* **문서 폴더**: 자세한 내용은 [문서 폴더 공유](../../workfront-basics/grant-and-request-access-to-objects/share-a-document-folder.md).

* **증명**: 자세한 내용은 [Workfront 증명의 증명 공유](../../workfront-proof/wp-work-proofsfiles/share-proofs-and-files/share-proof.md).

* **보고서, 대시보드 및 달력**: 자세한 내용은 [보고서, 대시보드 및 달력 공유](../../workfront-basics/grant-and-request-access-to-objects/permissions-reports-dashboards-calendars.md). 또한 다음 문서를 참조하십시오.

   * [Adobe Workfront에서 보고서 공유](../../reports-and-dashboards/reports/creating-and-managing-reports/share-report.md)
   * [대시보드 공유](../../reports-and-dashboards/dashboards/creating-and-managing-dashboards/share-dashboard.md)
   * [달력 보고서 공유](../../reports-and-dashboards/reports/calendars/share-a-calendar-report.md)

* **필터, 보기 및 그룹화**: 자세한 내용은 [필터, 보기 또는 그룹화 공유](../../reports-and-dashboards/reports/reporting-elements/share-filter-view-grouping.md).

* **플랜**: 자세한 내용은 [시나리오 계획자에서 계획 공유](../../scenario-planner/share-a-plan.md).

   이 경우 추가 라이센스가 필요합니다.

* **목표**: 자세한 내용은 [Workfront 목표에서 목표 공유](../../workfront-goals/workfront-goals-settings/share-a-goal.md).

   이 경우 추가 라이센스가 필요합니다.

## 개체 공유에 대한 고려 사항

* 개체에 대해 가지고 있는 동일한 수준 또는 낮은 수준의 권한만 공유할 수 있습니다.

   예를 들어 객체에 대한 Contribute 권한이 있는 경우에는 다른 사용자에게 해당 객체에 대한 관리 권한을 부여할 수 없습니다.

* 사용자의 액세스 수준보다 높은 권한 수준을 가진 개체는 공유할 수 없습니다. 예를 들어, 사용자가 액세스 수준에서 프로젝트에 대한 보기 액세스 권한을 가지고 있으면 프로젝트에 대한 관리 권한을 부여할 수 없습니다.
* 적어도 개체 보기에 대한 권한이 있는 사용자는 해당 개체를 다른 사람과 공유할 수 있습니다.
* 활성 사용자, 작업 역할, 팀, 그룹 또는 회사와 객체를 공유할 수 있습니다.

   >[!NOTE]
   >
   >계획이나 목표를 다른 활성 사용자만 공유할 수 있습니다. 이를 위해서는 추가 라이센스가 필요합니다.
   >
   >
   >자세한 내용은 다음을 참조하십시오.
   >
   >* [시나리오 계획자에서 계획 공유](../../scenario-planner/share-a-plan.md)
   >* [Workfront 목표에서 목표 공유](../../workfront-goals/workfront-goals-settings/share-a-goal.md)


## 공유 제한

최대 100개의 엔티티(사용자, 팀, 그룹, 작업 역할, 회사)와 객체를 공유할 수 있습니다. 이러한 제한을 방지하려면 개별 사용자가 아닌 그룹, 팀 또는 회사와 개체를 공유하는 것이 좋습니다.

## 개체에 대한 권한 공유

다음 표에서는 객체를 공유할 때 선택할 수 있는 권한 수준을 보여 줍니다. 일부 객체에는 이러한 설정을 모두 사용할 수 있는 것은 아닙니다. 개체를 보거나 관리할 다른 엔티티 권한을 부여할 수 있습니다. 프로젝트, 작업 또는 문제를 공유하는 경우 Contribute에 권한을 부여할 수도 있습니다.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">보기</td> 
   <td> <p>객체에 대해 다음 작업을 수행할 수 있습니다.</p> 
    <ul> 
     <li>개체 보기</li> 
     <li>객체에 문서 추가</li> 
     <li>객체에 대한 재무 정보 보기</li> 
     <li> <p>개체 공유<br></p> <p>개체를 공유할 때 상위 수준이 아니라 개체에만 있는 동일한 권한 수준을 다른 사용자에게 부여할 수 있습니다.</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">참여</td> 
   <td> <p>객체에 대해 다음 작업을 수행할 수 있습니다.</p> 
    <ul> 
     <li>보기</li> 
     <li>보기 권한에 포함된 모든 작업.</li> 
     <li>여기에 비용 추가</li> 
     <li>문제 추가(작업 또는 프로젝트인 경우)</li> 
     <li>작업에 작업 추가(프로젝트인 경우)</li> 
     <li>사용자 지정 Forms 편집</li> 
     <li>개체에 대한 로그 시간</li> 
     <li>여기에 할당</li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">관리</td> 
   <td> <p>객체에 대해 다음 작업을 수행할 수 있습니다.</p> 
    <ul> 
     <li>보기</li> 
     <li>보기 및 Contribute 권한에 포함된 모든 작업</li> 
     <li>삭제</li> 
     <li>재무 정보 관리</li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">외부 사용자에게 공개로 설정합니다</td> 
   <td> <p>Workfront 계정이 없는 모든 사용자는 해당 개체에 대한 링크를 클릭하여 개체를 볼 수 있습니다. 일부 개체에는 사용할 수 없습니다.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">시스템 전체에 표시</td> 
   <td> <p>개체는 Workfront 계정이 있는 모든 사람이 검색하고 볼 수 있습니다.</p> </td> 
  </tr> 
 </tbody> 
</table>

## 상속된 사용 권한 및 객체 계층 구조 이해

* [상위 개체에서 상속된 권한](#permissions-inherited-from-parent-objects)
* [조직 멤버십을 통해 획득한 권한](#permissions-acquired-through-organizational-memberships) 

### 상위 개체에서 상속된 권한 {#permissions-inherited-from-parent-objects}

Workfront의 권한은 계층적으로 상속됩니다. 즉, 상위 개체에 대해 사용자에게 권한을 부여하는 경우 기본적으로 사용자와 연관된 하위 객체에 대해 동일한 권한을 얻게 됩니다.

예를 들어 사용자에게 프로젝트에 대한 Contribute 권한을 제공하는 경우 사용자는 해당 프로젝트와 관련된 모든 작업 및 문제(하위 개체)에 대한 Contribute 권한을 갖습니다.

위의 예를 계속 사용해도 하위 객체에 대한 권한을 제한할 수 없습니다. 사용자에게 프로젝트와 연결된 하위 객체에 대한 Contribute 권한을 부여하지 않으려면 개체에서 수동으로 상속된 권한을 제거한 다음 고급 설정을 포함하여 개별 사용자에 대한 권한을 조정해야 합니다. 

Workfront에서 개체의 계층 구조 및 상호 종속성에 대한 자세한 내용은 섹션을 참조하십시오 [개체의 상호 종속성 및 계층](../../workfront-basics/navigate-workfront/workfront-navigation/understand-objects.md#understanding-interdependency-and-hierarchy-of-objects) 기사 [Adobe Workfront의 개체 이해](../../workfront-basics/navigate-workfront/workfront-navigation/understand-objects.md).

>[!NOTE]
>
>Workfront 관리자는 액세스 수준에서 문서에 대한 상속된 권한을 비활성화할 수 있습니다. 액세스 수준에서 문서에 대한 상속된 권한을 비활성화하는 방법에 대한 자세한 내용은 [사용자 정의 액세스 수준 만들기 또는 수정](../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md).

### 조직 멤버십을 통해 획득한 권한  {#permissions-acquired-through-organizational-memberships}

객체에 대한 사용자 그룹에 관리 권한을 부여하고 동일한 객체에 대한 해당 그룹의 개별 사용자에게 보기 권한을 부여하는 경우 객체에 대한 그룹 구성원을 통해 부여된 최상위 권한(관리)이 사용자에게 부여됩니다. 

권한 수준이 높은 조직 단위(그룹, 팀, 작업 역할 또는 회사)에 이미 속해 있는 사용자에게 낮은 권한을 부여하려면 조직 단위에서 권한을 제거하고 낮은 수준의 권한을 사용하여 개별적으로 사용자를 추가해야 합니다.

<!--
<div data-mc-conditions="QuicksilverOrClassic.Draft mode">
<h2>Remove permissions from objects</h2>
<p style="color: #ff1493;" data-mc-conditions="QuicksilverOrClassic.Draft mode">AL: draft/ hide this div when Becky makes Remove permissions from objects live and replace with the drafted content with the link at the top of this section</p>
<p>You can remove permissions from objects you have access to Share. Removing permissions from objects is identical for all objects that can be shared.&nbsp;</p> <note type="note">
&nbsp;You cannot remove permissions when you share items in bulk. You can remove permissions only when selecting individual items.&nbsp;
</note>
<p>To remove permissions from objects consider the following:&nbsp;</p>
<ul>
<li><a href="#remove-entities-from-the-sharing-list-of-an-object" class="MCXref xref">Remove entities from the sharing list of an object</a> </li>
<li><a href="#remove-inherited-permissions" class="MCXref xref">Remove inherited permissions</a> </li>
<li><a href="#make-an-object-private" class="MCXref xref">Make an object private</a> </li>
</ul>
<p><strong>Remove entities from the sharing list of an object</strong></p>
<p>You can remove entities from the sharing list of an object to remove their permissions from the object.</p>
<p>To remove permissions from objects:&nbsp;</p>
<ol>
<li value="1">Navigate to an object on which you want to modify the permissions.</li>
<li value="2">Click the <strong>Actions</strong> menu, then click <strong>Sharing</strong>.<br>For example, on a project, click <strong>Project Actions</strong>, then <strong>Sharing</strong>.&nbsp;</li>
<li value="3">Click the <strong>x</strong> next to the name of a user, team, group, company, job role to remove them.<br></li>
<li value="4">In the <strong><User Name>'s Workfront access will be removed from this</strong> drop-down menu, select whether you want their access to be removed just from the object you have selected, or from all children objects associated with it.<br>The following scenarios exist:
<ul>
<li>If you remove the entity only from the object, that entity loses their permissions on the object, and their inherited permissions to the children objects. If they are granted permissions to the children items individually, they retain the same permissions on all children objects associated with it when you select this option.&nbsp;</li>
<li>If you remove the entity from the object and all the children objects, that entity loses their permissions to the object as well as all children objects, even when they have been given individual permission on each child object.&nbsp;</li>
</ul></li>
<li value="5">Click <strong>Save</strong>.</li>
</ol>
<p> <p><strong>Remove inherited permissions</strong></p> </p>
<p>Inherited permissions can be removed from objects allowing for owners to specifically&nbsp;identify who will get access to children objects regardless of the access of a user to a parent object. Only users with Manage permission are able to remove inherited permissions.</p>
<p>To remove inherited permissions:</p>
<ol>
<li value="1">Navigate to an object to which you have Manage permissions. <br>For example, navigate to a task.</li>
<li value="2">Go to the sharing list as described in the <a href="#Share" class="MCXref xref">Overview of sharing permissions on objects</a> section in this article. </li>
<li value="3">Select the <strong>X</strong>&nbsp;mark next to <strong>Inherited Permission</strong>&nbsp;on the sharing box to remove&nbsp;anyone listed there.<br><br>This ensures that no one who is granted permissions to the parent object (for example, the project) has permissions to this task by default. You must list&nbsp; individual entities in the sharing list of the task to grant permissions on the task.<br><note type="note">
You cannot remove individual entities from the Inherited Permissions list. You can only disable the Inherited Permissions for all entities listed.
</note></li>
<li value="4">Click <strong>Save</strong>.&nbsp;</li>
</ol>
<p><strong>Make an object private</strong></p>
<p>If you have shared an object system-wide, or you have shared it with external uses by making it public, you can make it private again by removing the system-wide or public permissions.&nbsp;</p>
<p>For more information about making an object available system-wide, or publicly, see the section <a href="#Share" class="MCXref xref">Overview of sharing permissions on objects</a> in this article.</p>
<p>To make an object private:</p>
<ol>
<li value="1">Go to the object you want to make private.<br>For example, navigate to a report.</li>
<li value="2">Click <strong>Report Actions</strong>, then <strong>Sharing</strong>.<br><br></li>
<li value="3">Click <strong>Remove public access</strong> to remove the access of external users to viewing the report.</li>
<li value="4">Click <strong>Remove system-wide access</strong> to stop sharing it with all Workfront users.&nbsp;</li>
<li value="5">Click <strong>Save</strong>.</li>
</ol>
</div>
-->

## 개체 공유

객체 공유 방법에 대한 자세한 내용은 [개체 공유](../../workfront-basics/grant-and-request-access-to-objects/share-an-object.md).

## 개체에서 권한 제거

개체에서 권한을 제거하는 방법에 대한 자세한 내용은 [개체에서 권한 제거](../../workfront-basics/grant-and-request-access-to-objects/remove-permissions-from-objects.md).

## 개체에 대한 권한 요청

볼 수 있는 권한이 없는 개체에 대한 링크를 다른 사용자에게 보내거나, 개체에 대한 사용 권한이 낮아 더 높은 수준의 사용 권한을 요청하려는 경우, 개체에 대한 사용 권한을 요청할 수 있습니다. 

객체에 대한 공유 권한이 있는 모든 사용자의 객체 액세스를 요청할 수 있습니다. 

객체에 대한 권한 요청에 대한 자세한 내용은 [개체에 대한 액세스 요청](../../workfront-basics/grant-and-request-access-to-objects/request-access.md).
